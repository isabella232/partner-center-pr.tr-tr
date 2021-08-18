---
title: Azure portal özel Azure Marketi koleksiyonları oluşturun ve yönetin
description: Yeni koleksiyonlar görünümüyle Azure portal özel Azure Marketi (Önizleme) oluşturun ve yönetin. Özel Azure Marketi (Önizleme), yöneticilerin kullanıcıların hangi üçüncü taraf çözümlerini kullanabileceği konusunda yönetmelerini sağlar.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 08/10/2021
ms.openlocfilehash: 74550d814657a117f62d1e3eae45d46bae040356
ms.sourcegitcommit: 815760499700bf2c947550524cbddd091622081f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "121915357"
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

2. Koleksiyonunuz için bir ad girin.

3. Açılan menüden abonelikler'i seçin.

4. **Seçimlerinizi** yaptıktan sonra alttaki Oluştur'a (aşağıda gösterilmez) tıklayın.

    :::image type="content" source="media/private-azure-new/create-collection.png" alt-text="Koleksiyon Oluştur iletişim kutusunu gösterir.":::

5. Bu, yeni bir boş ve devre dışı özel koleksiyon oluşturur. Yönetmek için bir koleksiyon adı seçin.

    :::image type="content" source="media/private-azure-new/new-empty-collection.png" alt-text="Yeni ve boş bir Koleksiyon Öğeleri penceresi gösterir.":::

### <a name="update-collection-properties"></a>Koleksiyon özelliklerini güncelleştirme

1. Yönetmek istediğiniz koleksiyonun adını seçin.
2. Sol **gezinti menüsünden** Koleksiyon özellikleri'ne tıklayın.

    :::image type="content" source="media/private-azure-new/collection-properties.png" alt-text="Collection Özellikler penceresi.":::

3. Adı ve seçilen abonelikleri gereken şekilde güncelleştirin.
4. **Uygula'ya** (gösterilmez) seçin.

### <a name="delete-a-collection"></a>Koleksiyonu silme

Marketi Yönet sayfasında, koleksiyon adının yanındaki kutuyu işaretleyin ve Koleksiyonu **sil'i seçin.**

:::image type="content" source="media/private-azure-new/collection-delete.png" alt-text="'Koleksiyonu sil Azure Market düğmesi vurgulanmış özel ekran gösterilir.":::

> [!NOTE]
> **Varsayılan Koleksiyon,** sistem tarafından oluşturulan bir koleksiyondur ve silinemez.

## <a name="private-azure-marketplace-notification-center"></a>Özel Azure Market bildirim merkezi

Bildirim Merkezi üç tür bildirimden oluşur ve Market yöneticisinin bildirime göre eyleme olanak sağlar:

- Kullanıcılardan onaylanan listede yer alan öğeler için onay istekleri (aşağıdaki [Teklif veya plan ekleme isteğine bakın).](#request-to-add-offers-or-plans)
- Onaylanan listede zaten bir veya daha fazla planı olan teklifler için yeni plan bildirimleri.
- Onaylanan listede yer alan ancak genel listeden kaldırılan öğeler için plan bildirimleri Azure Market.

Bildirim merkezine erişmek için:

1. Sol **gezinti menüsünden** Bildirimler'i seçin.

   :::image type="content" source="media/private-azure-new/marketplace-notifications-small.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="Bildirimler menüsünü gösterir.":::

1. Daha fazla eylem için sağdan bir üç nokta menüsü seçin.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Diğer Seçenekler menü sonuçlarını gösterir.":::

1. Plan istekleri için **İstekleri göster,** belirli bir teklife yönelik tüm kullanıcı isteklerini gözden geçirebilirsiniz onay isteği formunu açar.

1. Onayla **veya Reddet'i** **seçin.**

   :::image type="content" source="media/private-azure-new/notifications-approve-reject-small.png" lightbox="media/private-azure/notifications-approve-reject.png" alt-text="Onaylama ve reddetme seçeneklerini gösterir.":::

1. Açılan menüden onay için planı seçin.

1. Tekliflerin/planların eksern koleksiyonu seçin.

1. Bir açıklama ekleyin ve **Gönder'i seçin.**

## <a name="browsing-private-azure-marketplace-user-experience"></a>Özel Azure Market'a Göz Atma (Kullanıcı deneyimi)

Özel Azure Market etkinleştirildiğinde, kullanıcılar Market yöneticisinin hangi planları onaylar olduğunu görebilir.

- Yeşil onaylı **bildirim,** onaylanan bir İş Ortağı (Microsoft olmayan) teklifini gösterir.
- Onaylanan mavi **bir** bildirim, onaylanan bir Microsoft [teklifini (Onaylı Linux dağıtımları](/azure/virtual-machines/linux/endorsed-distros)dahil) gösterir.

Kullanıcılar, onaylanan ve onaylanmadı olan teklifler arasında filtre uygulama:

   :::image type="content" source="media/private-azure/filter-option-small.png" lightbox="media/private-azure/filter-option.png" alt-text="Filtreleme seçeneğini gösterir.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Özel Dağıtım'da satın alma veya Azure Market

Ürün ayrıntıları sayfası deneyimi genel ürün deneyimine benzer Azure Market, ancak özel Azure Market vardır.

- Bir kullanıcı onaylı plan ve onaylanan abonelik birleşimini seçerse Oluştur **düğmesi** etkinleştirilir:

   :::image type="content" source="media/private-azure/button-create-enabled-small.png" lightbox="media/private-azure/button-create-enabled.png" alt-text="Plan oluşturulanana kadar teklif başlığı gösterir.":::

- Ürün ayrıntıları sayfasında bir ürün planı seçimi görünmüyorsa ancak yönetici bir veya daha fazla planı  onaylarsa, hangi planların onaylandı ve Oluştur düğmesi etkinse bir başlık not alın:

   :::image type="content" source="media/private-azure/button-create-enabled-and-plans-small.png" lightbox="media/private-azure/button-create-enabled-and-plans.png" alt-text="Bir planın oluşturula ve kullanılabilir planların gösteriLl olduğunu gösteren teklif başlığı gösterir.":::

- Kullanıcı onaylı olmayan bir plan veya abonelik seçerse, başlığı planı seçili abonelik için onaylanmadı olarak not edin ve Oluştur **düğmesi devre** dışı bırakılır. Kullanıcı yine de planı onaylanan listeye eklemek için istekte olabilir (sonraki bölüme bakın).

## <a name="request-to-add-offers-or-plans"></a>Teklif veya plan ekleme isteği

Özel Teklif'te şu anda onaylanmayacak bir genel teklif veya plan Azure Market.

1. Başlıkta **eklemek için** İstek'i seçerek Erişim isteği **formunu açın.**

   :::image type="content" source="media/private-azure-new/access-request-form-small.png" lightbox="media/private-azure/access-request-form.png" alt-text="Teklifler veya planlar için erişim isteği formunu gösterir.":::

1. İsteke hangi planların eklen bir plan olduğunu seçin (Herhangi bir **Plan** Market yöneticisine teklif içindeki belirli bir plan için tercih olmadığını söyler).

1. Bir Gerekçe **ekleyin ve** isteğinizi **göndermek için** İstek'i seçin.

1. Bekleyen bir isteğin göstergesi Erişim isteği formunda İsteği geri alma **seçeneğiyle birlikte görüntülenir.**

   :::image type="content" source="media/private-azure/approved-pending-plans-small.png" lightbox="media/private-azure/approved-pending-plans.png" alt-text="Geri Çekme İsteği bağlantısıyla onaylanan veya bekleyen planların listesini gösterir.":::

> [!NOTE]
> Gönderilen onay isteği formu, Market yöneticisinin [](#private-azure-marketplace-notification-center) isteği gözden geçirmesi ve eyleme geçirmesi için Bildirim Merkezi'ne gönderilir.

> [!CAUTION]
> Özel Market'e onay, çözümün tedariki için bir işaret değildir.

## <a name="frequently-asked-questions-faqs"></a>Sık Sorulan Sorular (SSS)

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>Market üçüncü taraf uygulamasını Azure İlkesi. Bu durum nasıl farklıdır?

Şu anda Market'te üçüncü taraf hizmetleri kısıtlamanın iki yolu vardır:

1. EA portalı veya Azure portal üçüncü taraf hizmetleri devre dışı bırakarak veya "Yalnızca Ücretsiz veya BYOL SKÜ'ler" ile kısıtla.

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Hizmet hizmet hizmetlerini kısıtlamayı Azure portal.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="E A portalında hizmetleri kısıtlamayı gösterir.":::

2. Yalnızca belirli VM'lere izin vermek için bir Azure ilkesi oluşturun. Vm'lere ilke uygulama hakkında Windows ayrıntılar için bkz. Azure Resource Manager ile Windows [VM'lere ilke uygulama.](/azure/virtual-machines/windows/policy)

Özel Azure Market, belirli teklifleri ve planları kısıtlama ve izin verme konusunda daha fazla esneklik sağlar. Üçüncü taraf hizmetleri dağıtmayı denemeden önce bile son kullanıcıları market galerisinde dağıtım için kullanılabilirlik konusunda bilgi sağlar. Üçüncü taraf hizmetlerin dağıtımına izin vermek için Azure Market/Etkin olarak EA Portal ve Azure portal.

- Özel Azure Market, sanal makineyle sınırlı değil iş ortağı çözümleri de sunar.
- Özel Azure Market, plan düzeyinde ve ayrıca "Geçerli ve gelecek plan" olarak da ayarlandır.
- Özel Azure Market, son kullanıcıları dağıtılabilir ve dağıtılamayabilirsiniz konusunda bilgilendirebilirsiniz.

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>Özel Teklif ile Özel Teklif arasındaki fark Azure Market?

Özel **Teklif,** iş ortaklarının yalnızca hedeflenen müşterilere görünür olan planlar oluşturmalarına olanak sağlar. Bu, özelleştirilmiş çözümleri anlaşmalı fiyatlandırma, özel hüküm ve koşullar ve özelleştirilmiş yapılandırmalarla özel olarak paylaşmalarına olanak sağlar. Ayrıntılar için [bkz. Ticari markette özel teklifler.](/azure/marketplace/private-offers)

**Özel Azure Market,** Azure portal üçüncü taraf çözümlerin kullanıcılarının hangilerini dağıtalarını önceden onaylamalarına olanak sağlar. Özel Azure Market, kullanıcılar uyumlu teklifleri bularak, Azure Market ve dağıtarak bu avantajların avantajlarından faydalanmalarını sağlar. Özel Market'te abonelik tabanlı Özel Teklifleri yönetmek için Market yöneticisinin belirli abonelikte en az "okuma" rolüne sahip olması gerekir.

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>Özel Teklif'e Özel Teklif Azure Market, marketi yönet sekmesinde neden gösterm yok?

Abonelik tabanlı Özel Teklifler yalnızca Özel Teklif ayarlarında listelenen abonelikler için görünür. Özel Teklifi görüntülemek için genel abonelik filtresinin tüm abonelikleri gösterdiğine emin olur.

   :::image type="content" source="media/private-azure/private-marketplace-filter.png" lightbox="media/private-azure/private-marketplace-filter.png" alt-text="Özel market filtresini gösterir.":::

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>Özel görsellere özel görüntüler Azure Market?

Hayır. Özel Azure Market, herhangi bir IT yöneticisinin küresel hizmetlerden üçüncü taraf çözümleri yönetmesi ve Azure Market. Özel görüntüler genel görüntü Azure Market, IT yöneticisi özel görüntülerinizi seçe Azure Market seçamaz. Özel görüntüleri paylaşmak için Paylaşılan Görüntü [Galerisi'ni kullanın.](/azure/virtual-machines/shared-image-galleries)

1. Adım adım kılavuz Paylaşılan Görüntü Galerisi oluşturma (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).
2. SIG içinde bir görüntü tanımı oluşturun. Müşterinin işletim sistemi **durumu alanı** için Genelleştirilmiş'i seçmesi gerekir. ([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).
3. Yönetilen görüntüyü Paylaşılan Görüntü Galerisi'ne getir ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).
4. SIG VM görüntüleri bir abonelikte yer aitir. Diğer aboneliklerin kullanımına sağlamak için bir uygulama kaydı[(CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell) kullanın.](/azure/virtual-machines/windows/share-images-across-tenants)

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-partner-is-not-microsoft"></a>İş ortağı Microsoft değilken **neden bazı tekliflerin** varsayılan olarak onaylandı olduğunu görüyorum?

Microsoft, Azure'da Linux ve açık kaynak teknolojisini destekler. [Azure'da desteklenen](/azure/virtual-machines/linux/endorsed-distros) Desteklenen Linux dağıtımları ve fiyatı sanal makinelerde tümleştirilmiştir. Azure Linux Aracısı bir Microsoft Azure Market önceden yüklenmiş olduğundan, bir Microsoft teklifi olarak kabul edilir. Microsoft teklifleri varsayılan olarak onaylandıktan sonra, onaylı Linux dağıtımları Özel Dağıtımlar'da Azure Market ve varsayılan olarak onaylanır.

## <a name="contact-support"></a>Desteğe başvurun

- Azure Marketi desteği için [Microsoft Q&A](/answers/products/)adresini ziyaret edin.
<!-- images to delete when we retire old version: request-banner-small and access-request-form-filled-small>
