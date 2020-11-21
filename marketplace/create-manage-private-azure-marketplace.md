---
title: Azure portal 'de özel Azure Marketi oluşturun ve yönetin
description: Azure portal özel Azure Marketi (Önizleme) oluşturma ve yönetme hakkında bilgi edinin.
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 09/18/2020
ms.openlocfilehash: f62c9aef13b51ba2db42b267d7620f506bbdc1ec
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/21/2020
ms.locfileid: "95006948"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a>Azure portal özel Azure Marketi (Önizleme) oluşturma ve yönetme

Özel Azure Marketi (Önizleme), yöneticilerin kullanıcıların hangi üçüncü taraf çözümlerini kullanabileceği konusunda yönetmelerini sağlar. Bunu, yalnızca onayladığınız ve kuruluşunuzun ilkelerine uygun olan teklifleri dağıtmanıza olanak tanıyarak yapar. Özel Azure Marketi sayesinde kullanıcılarınız, satın alıp dağıtmak üzere çevrimiçi mağazalarla uyumlu teklifler arayabilir. 

Market Yöneticisi (atanan rol) olarak, onaylanan tekliflerinizi ve planlarınızı ekleyebileceğiniz devre dışı ve boş bir özel mağaza ile başlayacaksınız. Bu makalede, kullanıcılarınız için özel Azure Marketi oluşturma, yönetme ve etkinleştirme işlemleri açıklanmaktadır.

Notlar:

- Özel Azure Marketi bir kiracı düzeyindedir, bu nedenle kiracı kapsamındaki tüm kullanıcılar aynı seçkin listeyi görür.
- Tüm Microsoft çözümleri özel Azure Marketi 'ne otomatik olarak eklenir.

## <a name="assign-the-marketplace-admin-role"></a>Market yönetici rolünü atama

Kiracı Genel Yöneticisi, **Market yönetici** rolünü özel mağazayı yönetecek olan özel Azure Marketi yöneticisine atamalıdır.

>[!IMPORTANT]
> Özel Azure Marketi yönetimine erişim yalnızca Market yönetici rolü atanmış BT yöneticileri tarafından kullanılabilir.

### <a name="prerequisites"></a>Önkoşullar

Kiracı kapsamındaki bir kullanıcıya Market yönetici rolünü atayabilmeniz için önce bu önkoşulları karşılamanız gerekir:

- Bir **genel yönetici** kullanıcısına erişiminiz var.
- Kiracıda en az bir abonelik (herhangi bir tür olabilir) vardır.
- Genel yönetici kullanıcısına, seçilen abonelik için **katkıda** bulunan rolü veya üzeri atanır.
- Genel yönetici kullanıcının yükseltilmiş erişimi **Evet** olarak ayarlanmış (bkz. [tüm Azure aboneliklerini ve Yönetim gruplarını yönetmek için erişimi yükseltme](/azure/role-based-access-control/elevate-access-global-admin)).

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>Market yönetici rolünü PowerShell ile atama

Market yönetici rolünü atamak için aşağıdaki PowerShell betiğini kullanın; Aşağıdaki parametreleri gerektirir:

- **Tenantıd:** Kapsamdaki kiracının KIMLIĞI (Market yönetim rolü kiracı kapsamında atanabilir).
- **Abonelik kimliği:** Genel yöneticiye **katkıda** bulunan rolü veya daha yüksek bir abonelik atanmış.
- **GlobalAdminUsername:** Genel yöneticinin Kullanıcı adı.
- **UsernameToAssignRoleFor:** Market yönetici rolü atanacak Kullanıcı adı.

> [!NOTE]
> Kiracıya davet edilen Konuk kullanıcılar için, bir hesabı Market yönetici rolü atama için kullanılabilir olana kadar 48 saat kadar sürebilir. Daha fazla bilgi için bkz. [Azure ACTIVE DIRECTORY B2B işbirliği kullanıcısının özellikleri](/azure/active-directory/b2b/user-properties).

```PowerShell
function Assign-MarketplaceAdminRole {
[CmdletBinding()]
param(
[Parameter(Mandatory)]
[string]$TenantId,

[Parameter(Mandatory)]
[string]$SubscriptionId,

[Parameter(Mandatory)]
[string]$GlobalAdminUsername,

[Parameter(Mandatory)]
[string]$UsernameToAssignRoleFor
)

$MarketplaceAdminRoleDefinitionName = "Marketplace Admin"

Write-Output "TenantId = $TenantId"
Write-Output "SubscriptionId = $SubscriptionId"
Write-Output "GlobalAdminUsername = $GlobalAdminUsername"
Write-Output "UsernameToAssignRoleFor = $UsernameToAssignRoleFor"

Write-Output "$($GlobalAdminUsername) is about to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)"

$profile = Connect-AzAccount -Tenant $TenantId -SubscriptionId $SubscriptionId

if($profile -eq $null)
{
Write-Error -Message "Failed to connect to tenant and/or subscription" -ErrorAction Stop
}
elseif($profile.Context.Account.Id -ne $GlobalAdminUsername)
{
Write-Error "Connected with $($profile.Context.Account.Id) instead of with the global admin that was specified in the script parameters, which is $($GlobalAdminUsername)"
}
else
{
Write-Output "$($GlobalAdminUsername) was connected successfully to Tenant=$($profile.Context.Tenant), Subscription=$($profile.Context.Subscription), AccountId=$($profile.Context.Account.Id), Environment=$($profile.Context.Environment)"
}

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName

if($MarketPlaceAdminRole -eq $null)
{
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop
}
else
{
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available"
}

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..."
$elevatedAccessOnRoot = Get-AzRoleAssignment | where {$_.RoleDefinitionName -eq "User Access Administrator" -and $_.Scope -eq "/" -and $_.SignInName.Trim().ToLower() -eq $GlobalAdminUsername.Trim().ToLower() } | ft -Property SignInName

if($elevatedAccessOnRoot.Count -eq 0)
{
Write-Error -Message "$($GlobalAdminUsername) doesn't have permissions to assign '$($MarketplaceAdminRoleDefinitionName)'. Please verify it has elevated access 'On' in portal, https://docs.microsoft.com/en-us/azure/role-based-access-control/elevate-access-global-admin" -ErrorAction Stop
}
else
{
Write-Output "$GlobalAdminUsername has elevated access on root"
}

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

}

Assign-MarketplaceAdminRole
```

Az. Portal PowerShell modülünde bulunan cmdlet 'ler hakkında daha fazla bilgi için bkz. [Microsoft Azure PowerShell: Portal panosu cmdlet 'leri](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Özel Azure Marketi oluştur

1. [Azure portalında](https://portal.azure.com/) oturum açın.
2. **Tüm hizmetler** ' i ve ardından **Market**' i seçin.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Ana pencere Azure portal.":::

3. Soldaki seçeneklerden **özel Market** ' i seçin.

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Azure portal ana penceresinde özel Market seçme.":::

4. Özel Azure Marketi oluşturmak için **başlayın** ' ı seçin (bunu yalnızca bir kez yapmanız gerekir).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Azure portal ana penceresinde Başlarken ' i seçin.":::

    Bu kiracı için özel Azure Marketi zaten mevcutsa Market 'i **Yönet** varsayılan olarak seçilidir.

5. Tamamlandıktan sonra boş ve devre dışı bir özel Azure Marketi olur.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Boş özel Azure Marketi ekranı.":::

## <a name="add-items-from-gallery"></a>Galeriden öğe Ekle

Bir öğe, teklifin ve planın bir birleşimidir. Market 'i Yönet sayfasında öğe arayabilir ve ekleyebilirsiniz.

1. **Öğe Ekle**' yi seçin.

2. **Galeriye** gözatıp istediğiniz öğeyi bulmak için arama alanını kullanın.

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Galeriye göz atma veya arama alanını kullanma.":::

3. Varsayılan olarak, yeni bir teklif eklenirken, tüm geçerli planlar izin verilenler listesine eklenir. Seçilen öğeleri eklemeden önce plan seçimini değiştirmek için, teklifin kutucuğunda açılan menüyü seçin ve gerekli planları güncelleştirin.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Gerekli planları güncelleştirin.":::

4. Seçimlerinizi yaptıktan sonra sol alttaki **bitti** ' yi seçin.

>[!Note]
> Market 'e **öğe eklemek** yalnızca Microsoft dışı teklifler için kullanılabilir olacaktır. Varsayılan olarak Microsoft tekliflere izin verilir.

## <a name="edit-item-plans"></a>Öğe planlarını Düzenle

Market 'i Yönet sayfasında bir öğenin planlarını düzenleyebilirsiniz.

1. **Planlar** sütununda, bu öğenin açılan menüsünden kullanılabilir planları gözden geçirin.
2. Kullanıcılarınız için hangi planların kullanılabilir olduğunu seçmek için onay kutularını işaretleyin veya temizleyin.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Gerekli öğe için onay kutusunu seçme veya temizleme.":::

> [!NOTE]
> Her teklifin, güncelleştirmenin gerçekleşmesi için en az bir plan seçilmiş olması gerekir. Bir teklifle ilgili tüm planları kaldırmak için teklifin tamamını silin (sonraki bölüme bakın).

## <a name="delete-offers"></a>Teklifleri silme

Market 'i Yönet sayfasında, teklif adının yanındaki onay kutusunu işaretleyin (yukarıdaki ekrana bakın) ve **öğeleri sil**' i seçin.

## <a name="enabledisable-private-azure-marketplace"></a>Özel Azure Marketi 'ni etkinleştir/devre dışı bırak

Market 'i Yönet sayfasında, özel Azure Marketi 'nin geçerli durumunu gösteren bu başlık sayfasından birini görürsünüz:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Durum başlığını devre dışı bırak":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Durum başlığını etkinleştir":::

Özel Azure Marketi 'ni gerektiği şekilde etkinleştirebilir veya devre dışı bırakabilirsiniz.

1. Devre dışı bırakılırsa, etkinleştirmek için **özel marketi etkinleştir** ' i seçin.
2. Etkinleştirilirse, devre dışı bırakmak için **özel marketi devre dışı bırak** seçeneğini belirleyin.

## <a name="browsing-private-azure-marketplace"></a>Özel Azure Marketi 'ne göz atma

Özel Azure Marketi etkinleştirildiğinde, kullanıcılar Market yöneticisinin hangi planlara izin verileceğini görür.

- Yeşil **izin** verilen bir bildirimde, izin verilen bir iş ortağı (Microsoft dışı) teklifi gösterilir.
- Bir mavi **izin** verilen bildirim, izin verilen bir Microsoft teklifini gösterir.

Kullanıcılar, ve izin verilmeyen teklifler arasında filtre uygulayabilir:

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Filtreleme seçeneği.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Özel Azure Marketi 'nde satın alın veya dağıtın

Ürün Ayrıntıları sayfası deneyimi Genel Azure Marketi 'ne benzer olsa da, özel Azure Market 'e özgü üç senaryo vardır.

- Kullanıcı izin verilen bir planı seçtiğinde **Oluştur** düğmesi etkinleştirilir:

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Bir planın oluşturulabileceği teklif başlığı.":::

- Kullanıcı izin verilmeyen bir plan seçtiğinde, plana izin verilmeyen bir başlık ve **Oluştur** düğmesi devre dışı bırakılır.

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Bir plana dikkat eden teklif başlığı oluşturulamıyor.":::

- Ürün planı seçimi ürün ayrıntıları sayfasında görünmezse, ancak yönetici bir veya daha fazla planı onayladıysa, bir başlık, planlara izin verilen ve **Oluştur** düğmesi etkin olur:

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Bir planın oluşturulup kullanılabilir planları göstermediğini gösteren teklif başlığı.":::

## <a name="contact-support"></a>Desteğe başvurun

Azure Marketi desteği için [Microsoft Q&A](/answers/products/)adresini ziyaret edin. 
