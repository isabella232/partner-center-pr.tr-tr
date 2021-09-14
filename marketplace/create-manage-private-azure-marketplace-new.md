---
title: Azure portal özel Azure Marketi koleksiyonları oluşturun ve yönetin
description: Yeni koleksiyonlar görünümüyle Azure portal özel Azure Marketi (Önizleme) oluşturun ve yönetin. Özel Azure Marketi (Önizleme), yöneticilerin kullanıcıların hangi üçüncü taraf çözümlerini kullanabileceği konusunda yönetmelerini sağlar.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 08/10/2021
ms.openlocfilehash: 74550d814657a117f62d1e3eae45d46bae040356
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248438"
---
# <a name="create-and-manage-private-azure-marketplace-collections-in-the-azure-portal"></a>Azure portal özel Azure Marketi koleksiyonları oluşturun ve yönetin

> [!NOTE]
> Bu makalede özel Azure Marketi koleksiyonları ele alınmaktadır. Eski görünüm, bunun yerine [özgün makalede](create-manage-private-azure-marketplace.md) ele alınmıştır.

Özel Azure Marketi, yöneticilerin kullanıcılarının kullanabileceği üçüncü taraf çözümlerini yönetmelerini sağlar. Bu, kullanıcının yalnızca yönetici tarafından onaylanan ve kuruluşunuzun ilkelerine uygun olan teklifleri dağıtmalarına izin vererek bunu yapar. Özel Azure Marketi sayesinde kullanıcılar, satın alıp dağıtmak üzere çevrimiçi mağazalarla uyumlu teklifler arayabilir.

Market Yöneticisi (atanan rol) olarak, devre dışı bırakılmış ve boş bir özel Market ve onaylanan tekliflerinizi ve planlarınızı ekleyebileceğiniz bir koleksiyon ile başlayacaksınız. Bu makalede, gerekli rolü atama, özel bir mağaza oluşturma, koleksiyonları ve öğeleri yönetme, Kullanıcı isteklerini onaylama ve kullanıcılarınız için özel Azure Marketi 'ni etkinleştirme konuları açıklanmaktadır.

> [!NOTE]
> - Özel Azure Marketi bir kiracı düzeyindedir; etkinleştirildikten sonra, kiracı altındaki tüm kullanıcılar için ilkeyi ayarlar.
> - Koleksiyonları kullanarak bir abonelik düzeyindeki onaylanan listeyi yönetin.
> - Tüm Microsoft çözümleri ( [onaylı Linux dağıtımları](/azure/virtual-machines/linux/endorsed-distros)dahil), özel Azure Marketi 'ne otomatik olarak eklenir.

## <a name="assign-the-marketplace-admin-role"></a>Market yönetici rolünü atama

Kiracı Genel Yöneticisi, **Market yönetici** rolünü özel mağazayı yönetecek olan özel Azure Marketi yöneticisine atamalıdır.

>[!IMPORTANT]
> Özel Azure Marketi yönetimine erişim yalnızca Market yönetici rolü atanmış BT yöneticileri tarafından kullanılabilir.

### <a name="prerequisites"></a>Önkoşullar

Bu Önkoşullar, kiracı kapsamındaki bir kullanıcıya Market yönetici rolünü atayabilmeniz için gereklidir:

- Bir **genel yönetici** kullanıcısına erişiminiz var.
- Kiracıda en az bir abonelik (herhangi bir tür olabilir) vardır.
- Genel yönetici kullanıcısına, seçilen abonelik için **katkıda** bulunan rolü veya üzeri atanır.

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>Erişim denetimi (ıAM) ile Market yönetici rolünü atama

1. [Azure Portal](https://portal.azure.com/)’ında oturum açın.

1. **Tüm hizmetler** ' i ve ardından **Market**' i seçin.

1. Sol taraftaki menüden **özel Market** ' i seçin.

   :::image type="content" source="media/private-azure/private-marketplace.png" lightbox="media/private-azure/private-marketplace-zoom.png" alt-text="Market 'in sol tarafındaki özel Market menü seçeneğini gösterir.":::

1. Market yönetici rolünü atamak için **erişim denetimi (IAM)** seçeneğini belirleyin.

   :::image type="content" source="media/private-azure-new/access-control-iam.png" alt-text="M-M erişim denetimi ekranını gösterir.":::

1. **+ Ekle** > **Rol ataması ekle**’yi seçin.

1. **Rol** altında **Market Yöneticisi**' ni seçin.

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Rol atama menüsünü gösterir.":::

1. Açılan listeden istenen kullanıcıyı seçin, sonra **bitti**' yi seçin.

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>Market yönetici rolünü PowerShell ile atama

Market yönetici rolünü atamak için aşağıdaki PowerShell betiğini kullanın; Aşağıdaki parametreleri gerektirir:

- **Tenantıd:** Kapsamdaki kiracının KIMLIĞI (Market yönetim rolü kiracı kapsamında atanabilir).
- **Abonelik kimliği:** Genel yöneticiye **katkıda** bulunan rolü veya daha yüksek bir abonelik atanmış.
- **GlobalAdminUsername:** Genel yöneticinin Kullanıcı adı.
- **UsernameToAssignRoleFor:** Market yönetici rolü atanacak Kullanıcı adı.

> [!NOTE]
> Kiracıya davet edilen Konuk kullanıcılar için, bir hesabı Market yönetici rolü atama için kullanılabilir olana kadar 48 saat kadar sürebilir. daha fazla bilgi için bkz. [Azure Active Directory B2B işbirliği kullanıcısının özellikleri](/azure/active-directory/b2b/user-properties).

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

 

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

 

if($MarketPlaceAdminRole -eq $null) 
{ 
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop 
} 
else 
{ 
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available" 
} 

 

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..." 

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace" 

} 

Assign-MarketplaceAdminRole 
```

Az. portal PowerShell modülünde bulunan cmdlet 'ler hakkında daha fazla bilgi için bkz. [Microsoft Azure PowerShell: portal panosu cmdlet 'leri](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Özel Azure Marketi oluştur

1. [Azure Portal](https://portal.azure.com/)’ında oturum açın.
2. **Tüm hizmetler** ' i ve ardından **Market**' i seçin.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Ana pencereyi Azure portal gösterir.":::

3. Sol gezinti menüsünden **özel Market** ' i seçin.

4. özel Azure marketi oluşturmak için **Başlarken** seçin (bunu yalnızca bir kez yapmanız gerekir).

    :::image type="content" source="media/private-azure-new/private-marketplace-get-started.png" alt-text="' Başlarken ' ana penceresindeki ' Azure portal ' nin nasıl kullanılacağını gösterir.":::

    Bu kiracı için özel Azure Marketi zaten mevcutsa Market 'i **Yönet** varsayılan olarak seçilidir.

5. Tamamlandıktan sonra, tek bir **varsayılan koleksiyon** ile devre dışı bırakılmış bir özel Azure Market 'e sahip olursunuz.

    :::image type="content" source="media/private-azure-new/new-private-marketplace.png" alt-text="Boş özel Azure Marketi ekranını gösterir.":::

    > [!NOTE]
    > - **Varsayılan koleksiyon** , aynı kiracı kapsamındaki tüm aboneliklerin kapsamına sahip sistem tarafından üretilmiş bir koleksiyon kümesidir.
    > - Varsayılan koleksiyonun adı ve kapsamı değiştirilemez ve koleksiyon silinemez.

## <a name="add-collection-items-from-gallery"></a>Galeriden koleksiyon öğeleri ekle

Bir öğe, teklifin ve planın bir birleşimidir. Koleksiyon sayfasında öğeleri arayabilir ve ekleyebilirsiniz.

1. Bu koleksiyonu yönetmek için koleksiyon adını seçin.

2. **Öğe Ekle**' yi seçin.

3. **Galeriye** gözatıp istediğiniz öğeyi bulmak için arama alanını kullanın.

   :::image type="content" source="media/private-azure/marketplace-gallery.png" lightbox="media/private-azure/marketplace-gallery-zoom.png" alt-text="Galeriye gözatmaya veya arama alanını nasıl kullanacağınızı gösterir.":::

4. Varsayılan olarak, yeni bir teklif eklerken, tüm geçerli planlar onaylanan listeye eklenecektir. Seçilen öğeleri eklemeden önce plan seçimini değiştirmek için, teklifin kutucuğunda açılan menüyü seçin ve gerekli planları güncelleştirin.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Gerekli planların nasıl güncelleştirilmesini gösterir.":::

5. Seçimlerinizi yaptıktan sonra sol alttaki **bitti** ' yi seçin.

>[!Note]
> Market 'e **öğe eklemek** yalnızca Microsoft dışı teklifler için kullanılabilir olacaktır. Microsoft Solutions ( [onaylı Linux dağıtımları](/azure/virtual-machines/linux/endorsed-distros)dahil) "varsayılan olarak onaylandı" olarak etiketlenecek ve özel Market 'te yönetilemez.

## <a name="edit-item-plans"></a>Öğe planlarını Düzenle

Koleksiyon sayfasında bir öğenin planlarını düzenleyin.

1. **Planlar** sütununda, bu öğenin açılan menüsünden kullanılabilir planları gözden geçirin.

2. Kullanıcılarınız için hangi planların kullanılabilir olduğunu seçmek için onay kutularını işaretleyin veya temizleyin.

   :::image type="content" source="media/private-azure-new/edit-items.png" alt-text="Gerekli öğe için onay kutusunu seçme veya temizleme işlemlerinin nasıl yapılacağını gösterir.":::

   > [!NOTE]
   > Her teklifin, güncelleştirmenin gerçekleşmesi için en az bir plan seçilmiş olması gerekir. Bir teklifle ilgili tüm planları kaldırmak için teklifin tamamını silin (sonraki bölüme bakın).

### <a name="delete-items"></a>Öğeleri sil

Koleksiyon sayfasında, teklif adının yanındaki kutuyu işaretleyin ve **öğeleri sil**' i seçin.

:::image type="content" source="media/private-azure-new/delete-item.png" alt-text="Onay kutusunun nasıl kullanılacağını gösterir ve ' öğeleri sil ' seçeneğini belirleyin.":::

### <a name="copy-items"></a>Öğeleri Kopyala

1. Koleksiyonu Yönet sayfasında, teklif adının yanındaki kutuyu işaretleyin ve **öğeleri Kopyala**' yı seçin.  

   :::image type="content" source="media/private-azure-new/copy-items.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="Öğeleri Kopyala düğmesini gösterir.":::

1. Sağ bölmede, hedef koleksiyonu seçin (gerekiyorsa, **Yeni koleksiyon oluştur**' u seçerek yeni bir koleksiyon oluşturun).

   :::image type="content" source="media/private-azure-new/create-new-collection.png" alt-text="Koleksiyon Oluştur iletişim kutusunu gösterir.":::

1. **Kopyala**’yı seçin.

### <a name="enabledisable-a-collection"></a>Bir koleksiyonu etkinleştirme/devre dışı bırakma

1. **Koleksiyonu Yönet** sayfasında, koleksiyonun geçerli durumunu gösteren bir başlık görüntülenir:

   :::image type="content" source="media/private-azure-new/collection-disabled.png" alt-text="Koleksiyonun devre dışı başlığını gösterir.":::
   :::image type="content" source="media/private-azure-new/collection-enabled.png" alt-text="Koleksiyon etkin başlığını gösterir.":::

1. **Marketi Yönet** sayfasında, koleksiyonu seçin ve koleksiyonu etkinleştirmek veya devre dışı bırakmak için üst eylem çubuğunu kullanın.

   :::image type="content" source="media/private-azure-new/action-bar.png" alt-text="Koleksiyonu etkinleştir ve devre dışı bırak düğmeleriyle marketi yönetme eylem çubuğunu gösterir.":::

### <a name="enabledisable-private-azure-marketplace"></a>Özel Azure Marketi 'ni etkinleştir/devre dışı bırak

Market 'i Yönet sayfasında, özel Azure Marketi 'nin geçerli durumunu gösteren bu başlık sayfaları görüntülenir:

   :::image type="content" source="media/private-azure-new/state-disable.png" alt-text="Özel Azure Marketi devre dışı başlığını gösterir.":::
   :::image type="content" source="media/private-azure-new/state-enable.png" alt-text="Özel Azure Marketi etkin başlığını gösterir.":::

Özel Azure Marketi 'ni etkinleştirmek veya devre dışı bırakmak için:

1. sol gezinti menüsünden **Ayarlar** ' yi seçin.
1. İstediğiniz durum için radyo düğmesini seçin.
1. Sayfanın alt kısmında **Uygula** ' yı seçin.

### <a name="add-new-collection"></a>Yeni koleksiyon Ekle

Koleksiyonlar sayesinde Market Yöneticisi (atanan rol), kuruluşları genelinde farklı abonelikler için kullanılabilecek birden fazla onaylanan öğe listesi oluşturabilir.

1. **Koleksiyon Ekle**' yi seçin.

2. Koleksiyonunuzu adlandırın.

3. Açılır menüden abonelikler ' i seçin.

4. Seçimlerinizi yaptıktan sonra alt kısımdaki **Oluştur** ' u (aşağıda gösterilmez) seçin.

    :::image type="content" source="media/private-azure-new/create-collection.png" alt-text="Koleksiyon Oluştur iletişim kutusunu gösterir.":::

5. Bu, yeni bir boş ve devre dışı özel koleksiyon oluşturur. Yönetmek için bir koleksiyon adı seçin.

    :::image type="content" source="media/private-azure-new/new-empty-collection.png" alt-text="Yeni ve boş bir koleksiyon öğeleri penceresi gösterir.":::

### <a name="update-collection-properties"></a>Koleksiyon özelliklerini güncelleştirme

1. Yönetmek istediğiniz koleksiyonun adını seçin.
2. Sol gezinti menüsünden **koleksiyon özellikleri** ' ni seçin.

    :::image type="content" source="media/private-azure-new/collection-properties.png" alt-text="Koleksiyon Özellikler penceresi gösterir.":::

3. Gerekirse adı ve Seçili abonelikleri güncelleştirin.
4. **Uygula** ' yı (gösterilmez) seçin.

### <a name="delete-a-collection"></a>Koleksiyonu silme

Market 'i Yönet sayfasında, koleksiyon adının yanındaki kutuyu işaretleyin ve **koleksiyonu Sil**' i seçin.

:::image type="content" source="media/private-azure-new/collection-delete.png" alt-text="' Koleksiyonu Sil ' düğmesi vurgulanmış şekilde özel Azure Marketi ekranını gösterir.":::

> [!NOTE]
> **Varsayılan koleksiyon** , sistem tarafından oluşturulan bir koleksiyondur ve silinemez.

## <a name="private-azure-marketplace-notification-center"></a>Özel Azure Marketi Bildirim Merkezi

Bildirim Merkezi üç tür bildirimden oluşur ve Market yöneticisinin bildirime göre eylem almasına izin verir:

- Onaylanan listede olmayan öğeler için kullanıcılardan onay istekleri (bkz. [teklif veya plan ekleme isteği](#request-to-add-offers-or-plans) ).
- Onaylanan listede zaten bir veya daha fazla plana sahip olan tekliflere yönelik yeni plan bildirimleri.
- Onaylanan listede bulunan ancak genel Azure Marketi 'nden kaldırılan öğeler için plan bildirimleri kaldırıldı.

Bildirim merkezine erişmek için:

1. Sol gezinti menüsünden **Bildirimler** ' i seçin.

   :::image type="content" source="media/private-azure-new/marketplace-notifications-small.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="Bildirimler menüsünü gösterir.":::

1. Daha fazla eylem için sağdaki bir üç nokta menüsünü seçin.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Diğer Seçenekler menüsü sonuçlarını gösterir.":::

1. Plan istekleri için **Istekleri göster** , belirli bir teklifin tüm Kullanıcı isteklerini gözden geçirebileceğiniz onay isteği formunu açar.

1. **Onayla** veya **Reddet**' i seçin.

   :::image type="content" source="media/private-azure-new/notifications-approve-reject-small.png" lightbox="media/private-azure/notifications-approve-reject.png" alt-text="Onaylama ve reddetme seçeneklerini gösterir.":::

1. Açılan menüden onaylanacak planı seçin.

1. Teklifleri/planları eklemek için koleksiyonu seçin.

1. Bir açıklama ekleyin ve **Gönder**' i seçin.

## <a name="browsing-private-azure-marketplace-user-experience"></a>Özel Azure Marketi 'ne göz atma (Kullanıcı deneyimi)

Özel Azure Marketi etkinleştirildiğinde, kullanıcılar Market yöneticisinin hangi planları onayladığını görür.

- Yeşil **onaylı** bir bildirimde, onaylanan iş ortağı (Microsoft dışı) teklifi gösterilir.
- Mavi **onaylanmış** bir bildirim, onaylanan bir Microsoft teklifini (onaylanmış [Linux dağıtımları](/azure/virtual-machines/linux/endorsed-distros)dahil) gösterir.

Kullanıcılar, ve onaylanmamış teklifler arasında filtre uygulayabilir:

   :::image type="content" source="media/private-azure/filter-option-small.png" lightbox="media/private-azure/filter-option.png" alt-text="Filtreleme seçeneğini gösterir.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Özel Azure Marketi 'nde satın alın veya dağıtın

Ürün Ayrıntıları sayfası deneyimi küresel Azure Marketi 'ne benzer olsa da, özel Azure Market 'e özgü üç senaryo vardır.

- Bir Kullanıcı onaylanan planın ve onaylanan aboneliğin birleşimini seçtiğinde **Oluştur** düğmesi etkinleştirilir:

   :::image type="content" source="media/private-azure/button-create-enabled-small.png" lightbox="media/private-azure/button-create-enabled.png" alt-text="Bir planın oluşturulabileceği teklif başlığını gösterir.":::

- Ürün planı seçimi ürün ayrıntıları sayfasında görünmezse ancak yönetici bir veya daha fazla planı onayladıysa, bir başlık hangi planların onaylandığını ve **Oluştur** düğmesi etkin ' i not edin:

   :::image type="content" source="media/private-azure/button-create-enabled-and-plans-small.png" lightbox="media/private-azure/button-create-enabled-and-plans.png" alt-text="Bir planın oluşturulup kullanılabilir planların gösterilmediğini belirten teklif başlığını gösterir.":::

- Kullanıcı onaylanmamış bir plan veya abonelik seçtiğinde, bir başlık, planı seçili abonelik için onaylanmamış olarak Not ve **Oluştur** düğmesi devre dışı bırakılır. Kullanıcı yine de planı onaylanan listeye ekleme isteğinde bulunabilir (sonraki bölüme bakın).

## <a name="request-to-add-offers-or-plans"></a>Teklif veya plan ekleme isteği

Özel Azure Marketi 'nde Şu anda onaylanmamış olan bir genel teklif veya plan ekleme isteyebilirsiniz.

1. **Erişim isteği formunu** açmak için başlıkta **eklenecek isteği** seçin.

   :::image type="content" source="media/private-azure-new/access-request-form-small.png" lightbox="media/private-azure/access-request-form.png" alt-text="Teklifler veya planlar için erişim isteği formunu gösterir.":::

1. İsteğe hangi planların ekleneceğini seçin (**herhangi bir plan** , Market yöneticisine, bir teklif içindeki belirli bir plan için bir tercih olmadığını söyler).

1. İsteğinizi göndermek için bir **gerekçe** ve seçme **isteği** ekleyin.

1. Bekleyen bir istek için gösterge, **istek geri çekme** seçeneğiyle birlikte erişim isteği formunda görünür.

   :::image type="content" source="media/private-azure/approved-pending-plans-small.png" lightbox="media/private-azure/approved-pending-plans.png" alt-text="Geri çekme Isteği bağlantısıyla onaylanan veya bekleyen planların listesini gösterir.":::

> [!NOTE]
> Gönderildikten sonra, onay isteği formu Market yöneticisinin isteği gözden geçirmesi ve işlem yapması için [bildirim merkezine](#private-azure-marketplace-notification-center) gönderilir.

> [!CAUTION]
> Özel Market 'e onay, bir çözümün temin ini göstermez.

## <a name="frequently-asked-questions-faqs"></a>Sık sorulan sorular (SSS)

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>Azure Ilkesi aracılığıyla Market üçüncü taraf uygulamasını zaten engelliyor. Bu farklı midir?

Market 'te üçüncü taraf hizmetleri kısıtlamak için şu anda iki yol vardır:

1. EA Portalı veya Azure portal aracılığıyla, üçüncü taraf hizmetleri devre dışı bırakın veya yalnızca "ücretsiz veya KLG SKU 'Ları" ile kısıtlayın.

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Azure portal hizmetleri nasıl kısıtlayabileceğini gösterir.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="E-portalda hizmetleri nasıl kısıtlayabileceğini gösterir.":::

2. Yalnızca belirli VM 'Lere izin vermek için bir Azure ilkesi oluşturun. Windows sanal makinelere ilke zorlama hakkında daha fazla bilgi için, bkz. [Azure Resource Manager ile Windows sanal](/azure/virtual-machines/windows/policy)makinelere ilke uygulama.

Özel Azure Marketi, belirli tekliflere ve planlara kısıtlama ve izin verme konusunda daha fazla esneklik sağlar. Son kullanıcılara, üçüncü taraf hizmetleri dağıtmayı denemeden önce Market galerisinde dağıtım için kullanılabilirliği bildirir. Üçüncü taraf hizmetlerin dağıtımına izin vermek için, Azure Marketi ' ni EA portalında açık/etkin olarak ayarlayın ve Azure portal.

- Özel Azure Marketi, sanal makinelerle sınırlı olmamak üzere iş ortağı çözümlerini açabilir.
- Özel Azure Marketi, plan düzeyinde bulunabilir ve "geçerli ve gelecekteki plan" i de ayarlayabilir.
- Özel Azure Marketi, son kullanıcıları, ne yapabilecekleri ve dağıtılamayacağını en baştan haberdar edebilir.

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>Özel bir teklif ve özel Azure Marketi arasındaki fark nedir?

**Özel bir teklif** , iş ortaklarının yalnızca hedeflenen müşterilere görünen planlar oluşturmalarına olanak tanır. Bu, özelleştirilmiş çözümleri, anlaşmalı fiyatlandırma, özel hüküm ve koşullar ve özelleştirilmiş yapılandırmalarda özel olarak paylaşmasına olanak tanır. Ayrıntılar için bkz. [ticari Market 'Teki özel teklifler](/azure/marketplace/private-offers).

Azure portal **özel Azure Marketi** , yöneticilerin kullanıcıların dağıtabilecek üçüncü taraf çözümlerini önceden onaylamasını sağlar. Özel bir Azure Marketi sayesinde kullanıcılar, uyumlu teklifleri bularak, satın alarak ve dağıtarak Azure Marketi 'nin avantajlarından faydalanarak yararlanabilir. Özel Market 'teki abonelik tabanlı özel teklifleri yönetmek için Market yöneticisinin, belirli abonelikte en az "okuma" rolüne sahip olması gerekir.

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>Özel Azure Marketi 'ne özel bir teklif ekledim, neden Market 'i Yönet sekmesinde gösterilmiyor?

Abonelik tabanlı özel teklifler yalnızca özel teklif ayarlarındaki listelenen abonelikler için görülebilir. Özel teklifi görüntülemek için genel abonelik filtresinin tüm abonelikleri belirttiğinden emin olun.

   :::image type="content" source="media/private-azure/private-marketplace-filter.png" lightbox="media/private-azure/private-marketplace-filter.png" alt-text="Özel Market filtresini gösterir.":::

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>Özel Azure Marketi 'ne özel görüntüler ekleyebilir mi?

Hayır. Özel Azure Marketi, BT yöneticisinin küresel Azure Marketi 'nden üçüncü taraf çözümleri yönetmesine ve seçmesine olanak sağlar. Özel görüntüler küresel Azure Marketi 'nde olmadığından, BT Yöneticisi özel görüntülerinizi seçip seçemez. Özel görüntüleri paylaştırmak istiyorsanız [paylaşılan görüntü Galerisi](/azure/virtual-machines/shared-image-galleries)' ni kullanın.

1. Adım adım kılavuz paylaşılan görüntü Galerisi (SıG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)) oluşturma.
2. Bir SıG içinde bir görüntü tanımı oluşturun. Müşteri, işletim sistemi durumu alanı için **Genelleştirilmiş** ' ı seçmelidir. ([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).
3. Yönetilen görüntüyü paylaşılan görüntü galerisine getirin ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).
4. SıG VM görüntüleri bir abonelikte yer alır. Başka abonelikler için kullanılabilir hale getirmek için, bir uygulama kaydı ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)) kullanın.

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-partner-is-not-microsoft"></a>İş ortağı Microsoft olmasa da, neden **Varsayılan olarak onaylanan** bazı teklifleri görüyorum?

Microsoft, Azure 'da Linux ve açık kaynaklı teknolojiyi destekler. Desteklenen [Linux dağıtımları](/azure/virtual-machines/linux/endorsed-distros) Azure 'da desteklenir ve fiyat sanal makinelerde tümleşiktir. Azure Linux Aracısı zaten Azure Marketi 'nde önceden yüklenmiş olduğundan, Microsoft teklifi gibi davranılır. Microsoft teklifleri varsayılan olarak onaylandığından, onaylanmış Linux dağıtımları özel Azure Marketi 'nde yönetilemez ve varsayılan olarak onaylanır.

## <a name="contact-support"></a>Desteğe başvurun

- Azure Marketi desteği için [Microsoft Q&A](/answers/products/)adresini ziyaret edin.
<!-- images to delete when we retire old version: request-banner-small and access-request-form-filled-small>
