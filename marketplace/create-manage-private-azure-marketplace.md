---
title: Azure portal'de Özel Azure Market oluşturma ve yönetme
description: Eski görünümde özel Azure Market (önizleme) oluşturma ve Azure portal hakkında bilgi. Özel Azure Market (önizleme) kullanıcıların hangi üçüncü taraf çözümleri kullanabileceğini yöneticilerin yönetmesini sağlar.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 08/10/2021
ms.openlocfilehash: da44807519f18d6aa17e41d8e81b9ad774e40d2d
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248436"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>Azure portal'de Özel Azure Market oluşturma ve yönetme

> [!NOTE]
> Bu makalede eski Özel Güvenlik Azure Market. Yeni Koleksiyonlar görünümü için bunun yerine bu [yeni makaleye](create-manage-private-azure-marketplace-new.md) bakın.

Özel Azure Market, kullanıcıların hangi üçüncü taraf çözümleri kullanabileceğini yöneticilerin yönetmesini sağlar. Bunu, kullanıcının yalnızca yönetici tarafından onaylanan teklifleri dağıtmasına ve kuruluş ilkelerine uymasına izin vererek yapar. Özel Azure Market ile kullanıcılar çevrimiçi mağazada satın alma ve dağıtmaya uygun teklifler arayabilir.

Bir Market yöneticisi (atanan rol) olarak, onaylanan tekliflerinizi ve planlarınızı ek olarak eklerini ek olarak devre dışı bırakılmış ve boş bir Özel Mağaza ile başlayacaktır. Bu makalede gerekli rolü atama, özel depo oluşturma, öğeleri yönetme, kullanıcı isteklerini onaylama ve kullanıcılarınız için Özel Azure Market etkinleştirme açıklanmıştır.

> [!NOTE]
> - Özel Azure Market kiracı düzeyindedir, bu nedenle kiracı altındaki tüm kullanıcılar aynı curated listesini görebilir.
> - Tüm Microsoft çözümleri [(Onaylanan Linux Dağıtımları dahil)](/azure/virtual-machines/linux/endorsed-distros)otomatik olarak Özel Dağıtımlar'a Azure Market.

## <a name="assign-the-marketplace-admin-role"></a>Market yöneticisi rolünü atama

Kiracının Genel yönetici, market **yöneticisi rolünü** özel depo Azure Market özel yöneticiye ataması gerekir.

>[!IMPORTANT]
> Özel Azure Market erişimi yalnızca Market yöneticisi rolü atanmış OLAN IT yöneticileri tarafından kullanılabilir.

### <a name="prerequisites"></a>Önkoşullar

Bu önkoşullar, kiracı kapsamındaki bir kullanıcıya Market Yöneticisi rolünü ataymadan önce gereklidir:

- Bir kullanıcıya **Genel yönetici.**
- Kiracının en az bir aboneliği vardır (herhangi bir türde olabilir).
- Genel yönetici kullanıcıya, seçilen **abonelik** için Katkıda Bulunan rolü veya daha yüksek bir rol atanır.

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>Erişim denetimiyle Market yöneticisi rolünü atama (IAM)

1. [Azure Portal](https://portal.azure.com/)’ında oturum açın.

1. Tüm **hizmetler'i ve** ardından Market'i **seçin.**

1. Sol **menüden** Özel Market'i seçin.

   :::image type="content" source="media/private-azure/private-marketplace.png" lightbox="media/private-azure/private-marketplace-zoom.png" alt-text="Market'in sol tarafındaki özel market menü seçeneğini gösterir.":::

1. Market **yöneticisi rolünü atamak için Erişim denetimi (IAM)** öğesini seçin.

   :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="I A M erişim denetimi ekranı gösterilir.":::

1. **+ Ekle** > **Rol ataması ekle**’yi seçin.

1. Rol **altında Market** **Yöneticisi'ni seçin.**

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Rol atama menüsünü gösterir.":::

1. Açılan listeden istenen kullanıcıyı seçin ve bitti'yi **seçin.**

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>PowerShell ile Market yöneticisi rolünü atama

Market Yöneticisi rolünü atamak için aşağıdaki PowerShell betiği kullanın; Aşağıdaki parametreleri gerektirir:

- **TenantId:** Kapsam içinde kiracının kimliği (Market yöneticisi rolü kiracı kapsamında atanabilir).
- **SubscriptionId:** Genel yöneticinin Katkıda Bulunan rolüne veya **daha üst bir** role sahip olduğu abonelik.
- **GlobalAdminUsername:** Genel yöneticinin kullanıcı adı.
- **UsernameToAssignRoleFor:** Market yöneticisi rolünün atandığı kullanıcı adı.

> [!NOTE]
> Kiracıya davet edilen konuk kullanıcılar için, hesaplarının Market Yöneticisi rolünün atanma uygun olduğu zamana kadar 48 saat kadar sürebilir. Daha fazla bilgi için [bkz. B2B işbirliği kullanıcı Azure Active Directory özellikleri.](/azure/active-directory/b2b/user-properties)

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

Az.Portal PowerShell modülünde yer alan cmdlet'ler hakkında daha fazla bilgi için [bkz. Microsoft Azure PowerShell: Portal Panosu cmdlet'leri.](/powershell/module/az.portal/)

## <a name="create-private-azure-marketplace"></a>Özel Uygulama Azure Market

1. [Azure Portal](https://portal.azure.com/)’ında oturum açın.
2. Tüm **hizmetler'i ve** ardından Market'i **seçin.**

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Ana Azure portal gösterir.":::

3. Sol **menüden** Özel Market'i seçin.

4. Özel **Başlarken** oluşturmak için Azure Market seçin (bunu yalnızca bir kez yapmak zorunda olur).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Ana pencerede 'Başlarken' Azure portal seçmeyi gösterir.":::

    Özel Azure Market kiracı için zaten varsa, **Marketi Yönet** varsayılan olarak seçilir.

5. Tamamlandıktan sonra boş ve devre dışı bırakılmış özel bir özel Azure Market.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Boş Özel Ekran Azure Market gösterir.":::

## <a name="add-items-from-gallery"></a>Galeriden öğe ekleme

Öğe, teklif ve planın birleşimidir. Marketi Yönet sayfasında öğeleri arayabilir ve ekleyebilirsiniz.

1. Öğe **ekle'yi seçin.**

2. İstediğiniz **öğeyi bulmak** için Galeri'ye göz atabilir veya arama alanını kullanabilirsiniz.

   :::image type="content" source="media/private-azure/marketplace-gallery.png" lightbox="media/private-azure/marketplace-gallery-zoom.png" alt-text="Galeriye göz atma veya arama alanını kullanma hakkında bilgi gösterir.":::

3. Varsayılan olarak, yeni bir teklif eklerken tüm geçerli planlar onaylanan listeye eklenir. Seçili öğeleri eklemeden önce plan seçimini değiştirmek için teklifin kutucuğunun açılan menüsünü seçin ve gerekli planları güncelleştirin.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Gerekli planları güncelleştirmeyi gösterir.":::

4. **Seçimlerinizi** tamamladikten sonra sol altta Bitti'yi seçin.

>[!Note]
> **Markete** Öğe Ekle, yalnızca Microsoft dışı tekliflerde kullanılabilir. Microsoft çözümleri [(Onaylı Linux Dağıtımları dahil)](/azure/virtual-machines/linux/endorsed-distros)"Varsayılan olarak onaylandı" olarak etiketlenir ve Özel Market'te yönetil kullanılamaz.

## <a name="edit-items-plans"></a>Öğenin planlarını düzenleme

Bir öğenin planlarını Marketi Yönet sayfasında düzenleyebilirsiniz.

1. Planlar **sütununda,** ilgili öğenin açılan menüsünden kullanılabilir planları gözden geçirebilirsiniz.

2. Kullanıcılarınıza hangi planların kullanılabilir hale geleceklerini seçmek için onay kutularını seçin veya temizleyin.

   :::image type="content" source="media/private-azure/edit-items.png" alt-text="Gerekli öğenin onay kutusunu seçmeyi veya temizlemeyi gösterir.":::

   > [!NOTE]
   > Güncelleştirmenin gerçekleşmesi için her teklif için en az bir plan seçilmiş olması gerekir. Teklifle ilgili tüm planları kaldırmak için teklifin tamamını silin (sonraki bölüme bakın).

## <a name="delete-offers"></a>Teklifleri silme

Marketi Yönet sayfasında teklif adının yanındaki onay kutusunu işaretleyin (yukarıdaki ekrana bakın) ve Öğeleri **sil'i seçin.**

## <a name="enabledisable-private-azure-marketplace"></a>Özel Güvenlik Ayarlarını Etkinleştirme/Devre Dışı Azure Market

Marketi Yönet sayfasında, Özel Güvenlik Yönetimi'nin geçerli durumunun yer Azure Market:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="'Durumu devre dışı bırak' başlığı gösterir.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="'Durumu etkinleştir' başlığı gösterir.":::

Gerektiğinde Özel Ağ'ı etkinleştir veya Azure Market devre dışı 3.

- Devre dışı bırakılırsa etkinleştirmek **için Özel Market'i Etkinleştir'i** seçin.
- Etkinleştirilirse, devre dışı bırakmak **için Özel Market'i Devre Dışı** Bırak'ı seçin.

## <a name="private-azure-marketplace-notification-center"></a>Özel Azure Market bildirim merkezi

Bildirim Merkezi üç tür bildirimden oluşur ve Market yöneticisinin bildirime göre eyleme olanak sağlar:

- Kullanıcılardan onaylanan listede yer alan öğeler için onay istekleri (aşağıdaki Teklif veya [plan ekleme isteğine bakın).](#request-to-add-offers-or-plans)
- Onaylanan listede zaten bir veya daha fazla planı olan teklifler için yeni plan bildirimleri.
- Onaylanan listede yer alan ancak genel listeden kaldırılan öğeler için plan bildirimleri Azure Market.

Bildirim merkezine erişmek için:

1. Sol **menüden** Bildirimler'i seçin.

   :::image type="content" source="media/private-azure/marketplace-notifications-small.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="Bildirimler menüsünü gösterir.":::

1. Diğer eylemler için üç nokta menüsünü seçin.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Diğer Seçenekler menü sonuçlarını gösterir.":::

1. Plan istekleri için **İstekleri göster,** belirli bir teklife yönelik tüm kullanıcı isteklerini gözden geçirebilirsiniz onay isteği formunu açar.
1. Onayla **veya Reddet'i** **seçin.**

   :::image type="content" source="media/private-azure/notifications-approve-reject-small.png" lightbox="media/private-azure/notifications-approve-reject.png" alt-text="Onaylama ve reddetme seçeneklerini gösterir.":::

1. Açılan menüden onay için planı seçin.
1. Bir açıklama ekleyin ve Gönder'i **seçin.**

## <a name="browsing-private-azure-marketplace"></a>Özel Azure Market'a göz atma

Özel Azure Market etkinleştirildiğinde, kullanıcılar Market yöneticisinin hangi planları onaylar olduğunu görebilir.

- Yeşil onaylı **bildirim,** onaylanan bir İş Ortağı (Microsoft olmayan) teklifini gösterir.
- Onaylanan mavi **bir** bildirim, onaylanan bir Microsoft teklifini [(Onaylı Linux dağıtımları](/azure/virtual-machines/linux/endorsed-distros)dahil) gösterir.

Kullanıcılar, onaylanan ve onaylanmadı olan teklifler arasında filtre uygulama:

   :::image type="content" source="media/private-azure/filter-option-small.png" lightbox="media/private-azure/filter-option.png" alt-text="Filtreleme seçeneğini gösterir.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Özel Azure Marketi 'nde satın alın veya dağıtın

Ürün Ayrıntıları sayfası deneyimi küresel Azure Marketi 'ne benzer olsa da, özel Azure Market 'e özgü üç senaryo vardır.

- Bir Kullanıcı onaylanan bir planı seçtiğinde **Oluştur** düğmesi etkinleştirilir:

   :::image type="content" source="media/private-azure/button-create-enabled-small.png" lightbox="media/private-azure/button-create-enabled.png" alt-text="Bir planın oluşturulabileceği teklif başlığını gösterir.":::

- Ürün planı seçimi ürün ayrıntıları sayfasında görünmezse ancak yönetici bir veya daha fazla planı onayladıysa, bir başlık hangi planların onaylandığını ve **Oluştur** düğmesi etkin ' i not edin:

   :::image type="content" source="media/private-azure/button-create-enabled-and-plans-small.png" lightbox="media/private-azure/button-create-enabled-and-plans.png" alt-text="Bir planın oluşturulup kullanılabilir planların gösterilmediğini belirten teklif başlığını gösterir.":::

- Kullanıcı onaylanmamış bir plan seçtiğinde, bir başlık planı onaylanmamış olarak not edin ve **Oluştur** düğmesi devre dışıdır. Kullanıcı yine de planı onaylanan listeye ekleme isteğinde bulunabilir (sonraki bölüme bakın).

## <a name="request-to-add-offers-or-plans"></a>Teklif veya plan ekleme isteği

Özel Azure Marketi 'nde Şu anda onaylanmamış olan bir genel teklif veya plan ekleme isteyebilirsiniz.

1. **Erişim isteği formunu** açmak için başlıkta **eklenecek isteği** seçin.

   :::image type="content" source="media/private-azure/request-banner-small.png" lightbox="media/private-azure/request-banner.png" alt-text="' Ekleme Isteği ' bağlantısı olan başlığı gösterir.":::

   :::image type="content" source="media/private-azure/access-request-form-small.png" lightbox="media/private-azure/access-request-form.png" alt-text="Teklifler veya planlar için erişim isteği formunu gösterir.":::

1. İsteğe hangi planların ekleneceğini seçin (**herhangi bir plan** , Market yöneticisine bir teklif içindeki bir plan için bir tercih olmadığını söyler).

1. İsteğinizi göndermek için bir **gerekçe** ve seçme **isteği** ekleyin.

   :::image type="content" source="media/private-azure/access-request-form-filled-small.png" lightbox="media/private-azure/access-request-form-filled.png" alt-text="Örnek girişleri olan tekliflere veya planlara yönelik erişim isteği formunu gösterir.":::

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

**Özel bir teklif** , yayımcıların yalnızca hedeflenen müşterilere görünen planlar oluşturmalarına olanak tanır. Bu, özelleştirilmiş çözümleri, anlaşmalı fiyatlandırma, özel hüküm ve koşullar ve özelleştirilmiş yapılandırmalarda özel olarak paylaşmasına olanak tanır. Ayrıntılar için bkz. [ticari Market 'Teki özel teklifler](/azure/marketplace/private-offers).

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

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>Yayımcı Microsoft olmasa da, neden **Varsayılan olarak onaylanan** bazı teklifleri görüyorum?

Microsoft, Azure 'da Linux ve açık kaynaklı teknolojiyi destekler. Desteklenen [Linux dağıtımları](/azure/virtual-machines/linux/endorsed-distros) Azure 'da desteklenir ve fiyat sanal makinelerde tümleşiktir. Azure Linux Aracısı zaten Azure Marketi 'nde önceden yüklenmiş olduğundan, Microsoft teklifi gibi davranılır. Microsoft teklifleri varsayılan olarak onaylandığından, onaylanmış Linux dağıtımları özel Azure Marketi 'nde yönetilemez ve varsayılan olarak onaylanır.

## <a name="contact-support"></a>Desteğe başvurun

- Azure Marketi desteği için [Microsoft Q&A](/answers/products/)adresini ziyaret edin.