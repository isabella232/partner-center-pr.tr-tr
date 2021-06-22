---
title: Azure portal özel Azure Marketi oluşturun ve yönetin
description: Azure portal özel Azure Marketi (Önizleme) oluşturma ve yönetme hakkında bilgi edinin. Özel Azure Marketi (Önizleme), yöneticilerin kullanıcıların hangi üçüncü taraf çözümlerini kullanabileceği konusunda yönetmelerini sağlar.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 9da9eb4944508e815d1664fb44b13bce52f37150
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431663"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>Azure portal özel Azure Marketi oluşturun ve yönetin

Özel Azure Marketi, yöneticilerin kullanıcılarının kullanabileceği üçüncü taraf çözümlerini yönetmelerini sağlar. Bu, kullanıcının yalnızca yönetici tarafından onaylanan ve kuruluşunuzun ilkelerine uygun olan teklifleri dağıtmalarına izin vererek bunu yapar. Özel Azure Marketi sayesinde kullanıcılar, satın alıp dağıtmak üzere çevrimiçi mağazalarla uyumlu teklifler arayabilir.

Market Yöneticisi (atanan rol) olarak, onaylanan tekliflerinizi ve planlarınızı ekleyebileceğiniz devre dışı ve boş bir özel mağaza ile başlayacaksınız. Bu makalede, gerekli rolün nasıl atanacağı, özel bir mağaza oluşturulması, öğelerin yönetilmesi, kullanıcı isteklerinin onaylanması ve kullanıcılarınız için özel Azure Marketi 'nin nasıl etkinleştirileceği açıklanır.

> [!NOTE]
> - Özel Azure Marketi bir kiracı düzeyindedir, bu nedenle kiracı kapsamındaki tüm kullanıcılar aynı seçkin listeyi görür.
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

1. [Azure portalında](https://portal.azure.com/) oturum açın.
1. **Tüm hizmetler** ' i ve ardından **Market**' i seçin.
1. Sol taraftaki menüden **özel Market** ' i seçin.

    [![Market 'in sol tarafındaki özel Market menü seçeneğini gösterir.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)

1. Market yönetici rolünü atamak için **erişim denetimi (IAM)** seçeneğini belirleyin.

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="M-M erişim denetimi ekranını gösterir.":::

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

Az. Portal PowerShell modülünde bulunan cmdlet 'ler hakkında daha fazla bilgi için bkz. [Microsoft Azure PowerShell: Portal panosu cmdlet 'leri](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Özel Azure Marketi oluştur

1. [Azure portalında](https://portal.azure.com/) oturum açın.
2. **Tüm hizmetler** ' i ve ardından **Market**' i seçin.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Ana pencereyi Azure portal gösterir.":::

3. Sol taraftaki menüden **özel Market** ' i seçin.

4. Özel Azure Marketi oluşturmak için **başlayın** ' ı seçin (bunu yalnızca bir kez yapmanız gerekir).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="' Azure portal ' ın ana penceresindeki ' kullanmaya başlayın ' seçeneğini nasıl kullanacağınızı gösterir.":::

    Bu kiracı için özel Azure Marketi zaten mevcutsa Market 'i **Yönet** varsayılan olarak seçilidir.

5. Tamamlandıktan sonra boş ve devre dışı bir özel Azure Marketi olur.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Boş özel Azure Marketi ekranını gösterir.":::

## <a name="add-items-from-gallery"></a>Galeriden öğe Ekle

Bir öğe, teklifin ve planın bir birleşimidir. Market 'i Yönet sayfasında öğeleri arayabilir ve ekleyebilirsiniz.

1. **Öğe Ekle**' yi seçin.

2. **Galeriye** gözatıp istediğiniz öğeyi bulmak için arama alanını kullanın.

    [![Galeriye gözatmaya veya arama alanını nasıl kullanacağınızı gösterir.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)

3. Varsayılan olarak, yeni bir teklif eklerken, tüm geçerli planlar onaylanan listeye eklenecektir. Seçilen öğeleri eklemeden önce plan seçimini değiştirmek için, teklifin kutucuğunda açılan menüyü seçin ve gerekli planları güncelleştirin.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Gerekli planların nasıl güncelleştirilmesini gösterir.":::

4. Seçimlerinizi yaptıktan sonra sol alttaki **bitti** ' yi seçin.

>[!Note]
> Market 'e **öğe eklemek** yalnızca Microsoft dışı teklifler için kullanılabilir olacaktır. Microsoft Solutions ( [onaylı Linux dağıtımları](/azure/virtual-machines/linux/endorsed-distros)dahil) "varsayılan olarak onaylandı" olarak etiketlenecek ve özel Market 'te yönetilemez.

## <a name="edit-items-plans"></a>Öğenin planlarını Düzenle

Bir öğenin planlarını Market yönetimi sayfasında düzenleyebilirsiniz.

1. **Planlar** sütununda, bu öğenin açılan menüsünden kullanılabilir planları gözden geçirin.
2. Kullanıcılarınız için hangi planların kullanılabilir olduğunu seçmek için onay kutularını işaretleyin veya temizleyin.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Gerekli öğe için onay kutusunu seçme veya temizleme işlemlerinin nasıl yapılacağını gösterir.":::

> [!NOTE]
> Her teklifin, güncelleştirmenin gerçekleşmesi için en az bir plan seçilmiş olması gerekir. Bir teklifle ilgili tüm planları kaldırmak için teklifin tamamını silin (sonraki bölüme bakın).

## <a name="delete-offers"></a>Teklifleri silme

Market 'i Yönet sayfasında, teklif adının yanındaki onay kutusunu işaretleyin (yukarıdaki ekrana bakın) ve **öğeleri sil**' i seçin.

## <a name="enabledisable-private-azure-marketplace"></a>Özel Azure Marketi 'ni etkinleştir/devre dışı bırak

Market 'i Yönet sayfasında, özel Azure Marketi 'nin geçerli durumunu gösteren bu başlık sayfasından birini görürsünüz:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="' Durumu devre dışı bırak ' başlığını gösterir.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="' Durumu etkinleştir ' başlığını gösterir.":::

Özel Azure Marketi 'ni gerektiği şekilde etkinleştirebilir veya devre dışı bırakabilirsiniz.

- Devre dışı bırakılırsa, etkinleştirmek için **özel marketi etkinleştir** ' i seçin.
- Etkinleştirilirse, devre dışı bırakmak için **özel marketi devre dışı bırak** seçeneğini belirleyin.

## <a name="private-azure-marketplace-notification-center"></a>Özel Azure Marketi Bildirim Merkezi

Bildirim Merkezi üç tür bildirimden oluşur ve Market yöneticisinin bildirime göre eylem almasına izin verir:

- Onaylanan listede olmayan öğeler için kullanıcılardan onay istekleri (bkz. [teklif veya plan ekleme isteği](#request-to-add-offers-or-plans) ).
- Onaylanan listede zaten bir veya daha fazla plana sahip olan tekliflere yönelik yeni plan bildirimleri.
- Onaylanan listede bulunan ancak genel Azure Marketi 'nden kaldırılan öğeler için plan bildirimleri kaldırıldı.

Bildirim merkezine erişmek için:

1. Sol taraftaki menüden **Bildirimler** ' i seçin.

    [![Bildirimler menüsünü gösterir.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)

1. Daha fazla eylem için üç nokta menüsünü seçin.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Diğer Seçenekler menüsü sonuçlarını gösterir.":::

1. Plan istekleri için **Istekleri göster** , belirli bir teklifin tüm Kullanıcı isteklerini gözden geçirebileceğiniz onay isteği formunu açar.
1. **Onayla** veya **Reddet**' i seçin.

    [![Onaylama ve reddetme seçeneklerini gösterir.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)

1. Açılan menüden onaylanacak planı seçin.
1. Bir açıklama ekleyin ve **Gönder**' i seçin.

## <a name="browsing-private-azure-marketplace"></a>Özel Azure Marketi 'ne göz atma

Özel Azure Marketi etkinleştirildiğinde, kullanıcılar Market yöneticisinin hangi planları onayladığını görür.

- Yeşil **onaylı** bir bildirimde, onaylanan iş ortağı (Microsoft dışı) teklifi gösterilir.
- Mavi **onaylanmış** bir bildirim, onaylanan bir Microsoft teklifini (onaylanmış [Linux dağıtımları](/azure/virtual-machines/linux/endorsed-distros)dahil) gösterir.

Kullanıcılar, ve onaylanmamış teklifler arasında filtre uygulayabilir:

[![Filtreleme seçeneğini gösterir.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Özel Azure Marketi 'nde satın alın veya dağıtın

Ürün Ayrıntıları sayfası deneyimi küresel Azure Marketi 'ne benzer olsa da, özel Azure Market 'e özgü üç senaryo vardır.

- Bir Kullanıcı onaylanan bir planı seçtiğinde **Oluştur** düğmesi etkinleştirilir:

    [![Bir planın oluşturulabileceği teklif başlığını gösterir.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)

- Ürün planı seçimi ürün ayrıntıları sayfasında görünmezse ancak yönetici bir veya daha fazla planı onayladıysa, bir başlık hangi planların onaylandığını ve **Oluştur** düğmesi etkin ' i not edin:

    [![Bir planın oluşturulup kullanılabilir planların gösterilmediğini belirten teklif başlığını gösterir.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)

- Kullanıcı onaylanmamış bir plan seçtiğinde, bir başlık planı onaylanmamış olarak not edin ve **Oluştur** düğmesi devre dışıdır. Kullanıcı yine de planı onaylanan listeye ekleme isteğinde bulunabilir (sonraki bölüme bakın).

## <a name="request-to-add-offers-or-plans"></a>Teklif veya plan ekleme isteği

Özel Azure Marketi 'nde Şu anda onaylanmamış olan bir genel teklif veya plan ekleme isteyebilirsiniz.

1. **Erişim isteği formunu** açmak için başlıkta **eklenecek isteği** seçin.

    [![' Ekleme Isteği ' bağlantısı olan başlığı gösterir.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)

    [![Teklifler veya planlar için erişim isteği formunu gösterir.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)

1. İsteğe hangi planların ekleneceğini seçin (**herhangi bir plan** , Market yöneticisine bir teklif içindeki bir plan için bir tercih olmadığını söyler).

1. İsteğinizi göndermek için bir **gerekçe** ve seçme **isteği** ekleyin.
  
    [![Örnek girişleri olan tekliflere veya planlara yönelik erişim isteği formunu gösterir.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)

1. Bekleyen bir istek için gösterge, **istek geri çekme** seçeneğiyle birlikte erişim isteği formunda görünür.

    [![Geri çekme Isteği bağlantısıyla onaylanan veya bekleyen planların listesini gösterir.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)

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

2. Yalnızca belirli VM 'Lere izin vermek için bir Azure ilkesi oluşturun. Windows VM 'lerine ilke zorlama hakkında daha fazla bilgi için bkz. [Azure Resource Manager Ile Windows VM](/azure/virtual-machines/windows/policy)'Lerine ilke uygulama.

Özel Azure Marketi, belirli tekliflere ve planlara kısıtlama ve izin verme konusunda daha fazla esneklik sağlar. Son kullanıcılara, üçüncü taraf hizmetleri dağıtmayı denemeden önce Market galerisinde dağıtım için kullanılabilirliği bildirir. Üçüncü taraf hizmetlerin dağıtımına izin vermek için, Azure Marketi ' ni EA portalında açık/etkin olarak ayarlayın ve Azure portal.

- Özel Azure Marketi, sanal makinelerle sınırlı olmamak üzere iş ortağı çözümlerini açabilir.
- Özel Azure Marketi, plan düzeyinde bulunabilir ve "geçerli ve gelecekteki plan" i de ayarlayabilir.
- Özel Azure Marketi, son kullanıcıları, ne yapabilecekleri ve dağıtılamayacağını en baştan haberdar edebilir.

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>Özel bir teklif ve özel Azure Marketi arasındaki fark nedir?

**Özel bir teklif** , yayımcıların yalnızca hedeflenen müşterilere görünen planlar oluşturmalarına olanak tanır. Bu, özelleştirilmiş çözümleri, anlaşmalı fiyatlandırma, özel hüküm ve koşullar ve özelleştirilmiş yapılandırmalarda özel olarak paylaşmasına olanak tanır. Ayrıntılar için bkz. [ticari Market 'Teki özel teklifler](/azure/marketplace/private-offers).

Azure portal **özel Azure Marketi** , yöneticilerin kullanıcıların dağıtabilecek üçüncü taraf çözümlerini önceden onaylamasını sağlar. Özel bir Azure Marketi sayesinde kullanıcılar, uyumlu teklifleri bularak, satın alarak ve dağıtarak Azure Marketi 'nin avantajlarından faydalanarak yararlanabilir. Özel Market 'teki abonelik tabanlı özel teklifleri yönetmek için Market yöneticisinin, belirli abonelikte en az "okuma" rolüne sahip olması gerekir.

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>Özel Azure Marketi 'ne özel bir teklif ekledim, neden Market 'i Yönet sekmesinde gösterilmiyor?

Abonelik tabanlı özel teklifler yalnızca özel teklif ayarlarındaki listelenen abonelikler için görülebilir. Özel teklifi görüntülemek için genel abonelik filtresinin tüm abonelikleri belirttiğinden emin olun.

[![Özel Market filtresini gösterir.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>Özel Azure Marketi 'ne özel görüntüler ekleyebilir mi?

Hayır. Özel Azure Marketi, BT yöneticisinin küresel Azure Marketi 'nden üçüncü taraf çözümleri yönetmesine ve seçmesine olanak sağlar. Özel görüntüler küresel Azure Marketi 'nde olmadığından, BT Yöneticisi özel görüntülerinizi seçip seçemez. Özel görüntüleri paylaştırmak istiyorsanız [paylaşılan görüntü Galerisi](/azure/virtual-machines/shared-image-galleries)' ni kullanın.

1. Adım adım kılavuz paylaşılan görüntü Galerisi (SıG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)) oluşturma.
2. Bir SıG içinde bir görüntü tanımı oluşturun. Müşteri, işletim sistemi durumu alanı için **Genelleştirilmiş** ' ı seçmelidir. ([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).
3. Yönetilen görüntüyü paylaşılan görüntü galerisine getirin ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).
4. SıG VM görüntüleri bir abonelikte yer alır. Başka abonelikler için kullanılabilir hale getirmek için, bir uygulama kaydı ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)) kullanın.

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>Yayımcı Microsoft olmasa da, neden **Varsayılan olarak onaylanan** bazı teklifleri görüyorum?

Microsoft, Azure 'da Linux ve açık kaynaklı teknolojiyi destekler. Desteklenen [Linux dağıtımları](/azure/virtual-machines/linux/endorsed-distros) Azure 'da desteklenir ve fiyat sanal makinelerde tümleşiktir. Azure Linux Aracısı zaten Azure Marketi 'nde önceden yüklenmiş olduğundan, Microsoft teklifi gibi davranılır. Microsoft teklifleri varsayılan olarak onaylandığından, onaylanmış Linux dağıtımları özel Azure Marketi 'nde yönetilemez ve varsayılan olarak onaylanır.

## <a name="contact-support"></a>Desteğe başvurun

- Azure Marketi desteği için [Microsoft Q&A](/answers/products/)adresini ziyaret edin.