---
title: Azure portal özel Azure Marketi oluşturun ve yönetin
description: Azure portal özel Azure Marketi (Önizleme) oluşturma ve yönetme hakkında bilgi edinin. Özel Azure Marketi (Önizleme), yöneticilerin kullanıcıların hangi üçüncü taraf çözümlerini kullanabileceği konusunda yönetmelerini sağlar.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: c7238a601653b2c6b066b89403ba43cadddd13ed122355e42cf17b5e640c56a2
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115689972"
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

1. [Azure Portal](https://portal.azure.com/)’ında oturum açın.

1. **Tüm hizmetler** ' i ve ardından **Market**' i seçin.

1. Sol taraftaki menüden **özel Market** ' i seçin.

   :::image type="content" source="media/private-azure/private-marketplace.png" lightbox="media/private-azure/private-marketplace-zoom.png" alt-text="Market 'in sol tarafındaki özel Market menü seçeneğini gösterir.":::

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

3. Sol taraftaki menüden **özel Market** ' i seçin.

4. özel Azure marketi oluşturmak için **Başlarken** seçin (bunu yalnızca bir kez yapmanız gerekir).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="' Başlarken ' ana penceresindeki ' Azure portal ' nin nasıl kullanılacağını gösterir.":::

    Bu kiracı için özel Azure Marketi zaten mevcutsa Market 'i **Yönet** varsayılan olarak seçilidir.

5. Tamamlandıktan sonra boş ve devre dışı bir özel Azure Marketi olur.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Boş özel Azure Marketi ekranını gösterir.":::

## <a name="add-items-from-gallery"></a>Galeriden öğe Ekle

Bir öğe, teklifin ve planın bir birleşimidir. Market 'i Yönet sayfasında öğeleri arayabilir ve ekleyebilirsiniz.

1. **Öğe Ekle**' yi seçin.

2. **Galeriye** gözatıp istediğiniz öğeyi bulmak için arama alanını kullanın.

   :::image type="content" source="media/private-azure/marketplace-gallery.png" lightbox="media/private-azure/marketplace-gallery-zoom.png" alt-text="Galeriye gözatmaya veya arama alanını nasıl kullanacağınızı gösterir.":::

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

   :::image type="content" source="media/private-azure/marketplace-notifications-small.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="Bildirimler menüsünü gösterir.":::

1. Daha fazla eylem için üç nokta menüsünü seçin.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Diğer Seçenekler menüsü sonuçlarını gösterir.":::

1. Plan istekleri için **Istekleri göster** , belirli bir teklifin tüm Kullanıcı isteklerini gözden geçirebileceğiniz onay isteği formunu açar.
1. **Onayla** veya **Reddet**' i seçin.

   :::image type="content" source="media/private-azure/notifications-approve-reject-small.png" lightbox="media/private-azure/notifications-approve-reject.png" alt-text="Onaylama ve reddetme seçeneklerini gösterir.":::

1. Açılan menüden onaylanacak planı seçin.
1. Bir açıklama ekleyin ve **Gönder**' i seçin.

## <a name="browsing-private-azure-marketplace"></a>Özel Azure Marketi 'ne göz atma

Özel Azure Marketi etkinleştirildiğinde, kullanıcılar Market yöneticisinin hangi planları onayladığını görür.

- Yeşil **onaylı** bir bildirimde, onaylanan iş ortağı (Microsoft dışı) teklifi gösterilir.
- Mavi **onaylanmış** bir bildirim, onaylanan bir Microsoft teklifini (onaylanmış [Linux dağıtımları](/azure/virtual-machines/linux/endorsed-distros)dahil) gösterir.

Kullanıcılar, ve onaylanmamış teklifler arasında filtre uygulayabilir:

   :::image type="content" source="media/private-azure/filter-option-small.png" lightbox="media/private-azure/filter-option.png" alt-text="Filtreleme seçeneğini gösterir.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Özel Azure Marketi 'nde satın alın veya dağıtın

Ürün Ayrıntıları sayfası deneyimi küresel Azure Marketi 'ne benzer olsa da, özel Azure Market 'e özgü üç senaryo vardır.

- Kullanıcı onaylı bir plan seçerse Oluştur **düğmesi** etkinleştirilir:

   :::image type="content" source="media/private-azure/button-create-enabled-small.png" lightbox="media/private-azure/button-create-enabled.png" alt-text="Bir planın oluşturulanana kadar teklif başlığı gösterir.":::

- Ürün ayrıntıları sayfasında bir ürün planı seçimi görünmüyorsa ancak yönetici bir veya daha fazla planı  onayladısa, hangi planların onaylandı ve Oluştur düğmesi etkinse bir başlık not alın:

   :::image type="content" source="media/private-azure/button-create-enabled-and-plans-small.png" lightbox="media/private-azure/button-create-enabled-and-plans.png" alt-text="Bir planın oluşturula ve kullanılabilir planların gösteril olduğunu gösteren teklif başlığı gösterir.":::

- Kullanıcı onaylı olmayan bir planı seçerken, bir başlık planı onaylanmadı olarak not alar ve Oluştur **düğmesi devre** dışı bırakılır. Kullanıcı yine de planı onaylanan listeye eklemek için istekte olabilir (sonraki bölüme bakın).

## <a name="request-to-add-offers-or-plans"></a>Teklif veya plan ekleme isteği

Özel Teklif'te şu anda onaylanmadı olan bir genel teklif veya plan Azure Market.

1. Başlıkta **eklemek için** İstek'i seçerek Erişim isteği **formunu açın.**

   :::image type="content" source="media/private-azure/request-banner-small.png" lightbox="media/private-azure/request-banner.png" alt-text="'Ekleme isteği' bağlantısını içeren başlığı gösterir.":::

   :::image type="content" source="media/private-azure/access-request-form-small.png" lightbox="media/private-azure/access-request-form.png" alt-text="Teklifler veya planlar için erişim isteği formunu gösterir.":::

1. İsteke hangi planların eklen bir plan olduğunu seçin (Herhangi bir **Plan** Market yöneticisine teklif içindeki bir plan için tercih olmadığını söyler).

1. Bir Gerekçe **ekleyin ve** İsteğinizi **göndermek için** İstek'i seçin.

   :::image type="content" source="media/private-azure/access-request-form-filled-small.png" lightbox="media/private-azure/access-request-form-filled.png" alt-text="Örnek girişlere sahip teklifler veya planlar için erişim isteği formunu gösterir.":::

1. Bekleyen bir isteğin göstergesi Erişim isteği formunda İsteği geri alma **seçeneğiyle birlikte görüntülenir.**

   :::image type="content" source="media/private-azure/approved-pending-plans-small.png" lightbox="media/private-azure/approved-pending-plans.png" alt-text="Geri Çekme İsteği bağlantısıyla onaylı veya bekleyen planların listesini gösterir.":::

> [!NOTE]
> Gönderilen onay isteği formu, Market yöneticisinin [](#private-azure-marketplace-notification-center) isteği gözden geçirmesi ve eyleme geçirmesi için Bildirim Merkezi'ne gönderilir.

> [!CAUTION]
> Özel Market'e onay, çözümün tedariki için bir işaret değildir.

## <a name="frequently-asked-questions-faqs"></a>Sık Sorulan Sorular (SSS)

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>Market üçüncü taraf uygulamasını Azure İlkesi. Bu durum nasıl farklıdır?

Market'te üçüncü taraf hizmetleri kısıtlamak için şu anda iki yol vardır:

1. EA portalı veya Azure portal üçüncü taraf hizmetleri devre dışı bırakarak veya "Yalnızca Ücretsiz veya BYOL SKÜ'ler" ile kısıtla.

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Hizmet hizmet hizmetlerini kısıtlamayı Azure portal.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="E A portalında hizmetleri kısıtlamayı gösterir.":::

2. Yalnızca belirli VM'lere izin vermek için bir Azure ilkesi oluşturun. Vm'lere ilke uygulama hakkında Windows için bkz. Windows [vm'lere ilke Azure Resource Manager.](/azure/virtual-machines/windows/policy)

Özel Azure Market, belirli teklifleri ve planları kısıtlama ve izin verme konusunda daha fazla esneklik sağlar. Üçüncü taraf hizmetleri dağıtmayı denemeden önce bile son kullanıcıları market galerisinde dağıtım için kullanılabilirlik konusunda bilgi sağlar. Üçüncü taraf hizmetlerin dağıtımına izin vermek için Azure Market/Etkin olarak ayarlayın EA Portal ve Azure portal.

- Özel Azure Market, sanal makineyle sınırlı değil iş ortağı çözümleri de sunar.
- Özel Azure Market, plan düzeyinde ve ayrıca "Geçerli ve gelecek plan" olarak da ayarlandır.
- Özel Azure Market, son kullanıcıları dağıtılabilir ve dağıtılamayabilirsiniz konusunda bilgilendirebilirsiniz.

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>Özel Teklif ile Özel Teklif arasındaki fark Azure Market?

Özel **Teklif,** yayımcıların yalnızca hedeflenen müşterilere görünür planlar oluşturmalarına olanak sağlar. Bu, özelleştirilmiş çözümleri anlaşmalı fiyatlandırma, özel hüküm ve koşullar ve özelleştirilmiş yapılandırmalarla özel olarak paylaşmalarına olanak sağlar. Ayrıntılar için [bkz. Ticari markette özel teklifler.](/azure/marketplace/private-offers)

**Hizmet Azure Market** özel Azure portal, yöneticilerin kullanıcılarının hangi üçüncü taraf çözümleri dağıtalarını önceden onaylamalarına olanak sağlar. Özel Azure Market, kullanıcılar uyumlu teklifleri bularak, Azure Market ve dağıtarak bu avantajların avantajlarından faydalanmalarını sağlar. Özel Market'te abonelik tabanlı Özel Teklifleri yönetmek için Market yöneticisinin belirli abonelikte en az "okuma" rolüne sahip olması gerekir.

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>Özel Teklif'e özel teklif Azure Market, marketi yönet sekmesinde neden gösterm yok?

Abonelik tabanlı Özel Teklifler yalnızca Özel Teklif ayarlarında listelenen abonelikler için görünür. Özel Teklifi görüntülemek için genel abonelik filtresinin tüm abonelikleri gösterdiğine emin olur.

   :::image type="content" source="media/private-azure/private-marketplace-filter.png" lightbox="media/private-azure/private-marketplace-filter.png" alt-text="Özel market filtresini gösterir.":::

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>Özel görsellere özel görüntüler Azure Market?

Hayır. Özel Azure Market, herhangi bir IT yöneticisinin küresel hizmetlerden üçüncü taraf çözümleri yönetmesi ve Azure Market. Özel görüntüler genel görüntü Azure Market, IT yöneticisi özel görüntülerinizi seçe Azure Market seçamaz. Özel görüntüleri paylaşmak için Paylaşılan Görüntü [Galerisi'ni kullanın.](/azure/virtual-machines/shared-image-galleries)

1. Adım adım kılavuz Paylaşılan Görüntü Galerisi oluşturma (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).
2. SIG içinde bir görüntü tanımı oluşturun. Müşterinin işletim sistemi **durumu alanı** için Genelleştirilmiş'i seçmesi gerekir. ([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).
3. Yönetilen görüntüyü Paylaşılan Görüntü Galerisi'ne getir ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).
4. SIG VM görüntüleri bir abonelikte yer aitir. Diğer aboneliklerin kullanımına sağlamak için bir uygulama kaydı[(CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell) kullanın.](/azure/virtual-machines/windows/share-images-across-tenants)

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>Yayımcı Microsoft değilken **neden bazı tekliflerin** varsayılan olarak onaylandı olduğunu görüyorum?

Microsoft, Azure'da Linux ve açık kaynak teknolojisini destekler. [Azure'da desteklenen](/azure/virtual-machines/linux/endorsed-distros) Desteklenen Linux dağıtımları ve fiyatı sanal makinelerde tümleştirilmiştir. Azure Linux Aracısı bir Microsoft Azure Market önceden yüklenmiş olduğundan, bir Microsoft teklifi olarak kabul edilir. Microsoft teklifleri varsayılan olarak onaylandıktan sonra, onaylı Linux dağıtımları Özel Dağıtımlar'da Azure Market ve varsayılan olarak onaylanır.

## <a name="contact-support"></a>Desteğe başvurun

- Daha Azure Market için Microsoft [Q&A'&ziyaret edin.](/answers/products/)