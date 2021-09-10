---
title: Hizmet olarak yazılım (SaaS) abonelik yaşam döngüsü yönetimi
description: Azure Marketi 'nde hizmet olarak yazılım (SaaS) abonelik yaşam döngüsü yönetimi.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
ms.date: 08/20/2021
ms.author: yonits
author: yonits
ms.openlocfilehash: fed2b2f7b951a7dc6ee16fb126f3f5f774df18c9
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123936990"
---
# <a name="saas-subscription-lifecycle-management"></a>SaaS Abonelik yaşam döngüsü yönetimi

Bu makalede, SaaS kaynağını bulma, SaaS ve SaaS klasik arasındaki farklar ve Azure portal SaaS kaynak yönetimi konuları ele alınmaktadır.

## <a name="find-a-saas-resource"></a>SaaS kaynağı bulma

Azure Marketi 'nden bir SaaS teklifi satın aldığınızda, Azure portal bir hizmet olarak yazılım (SaaS) aboneliği oluşturur (Ayrıntılar için bkz. [Azure Portal bir SaaS teklifi satın alma](purchase-saas-offer-in-azure-portal.md)). Portalda bir SaaS kaynağı bulmak için:

- **Genel arama penceresi** (üst) – SaaS aboneliğinizi adına göre arayın.
- **SaaS** : tüm SaaS aboneliklerinizi listeler. İki tür SaaS listesi vardır; aşağıdaki bölüme bakın.
- **Abonelikler** – kiracınızın bir parçası olarak erişiminiz olan tüm Azure aboneliklerini listeler. Belirli bir aboneliği bulmak için filtre veya arama penceresini kullanın.
- **Tüm kaynaklar** – erişiminiz olan tüm abonelikler altında oluşturulan tüm kaynakları listeler. Belirli bir aboneliği bulmak için filtreyi kullanın (türü > SaaS) veya listede arama yapın.

## <a name="differences-between-saas-and-saas-classic-lists-of-resources-in-the-azure-portal"></a>Azure portal SaaS ve SaaS klasik kaynak listeleri arasındaki farklar

Bu iki tür arasındaki fark, SaaS Classic 'in, kiracınızda oluşturulan ve bir kaynak grubu altında olmayan SaaS aboneliklerini bulmanıza olanak sağlar.
2021 Şubat 'tan önce Azure portal bir SaaS aboneliği satın aldıysanız, kiracınızda oluşturulmuştur ve SaaS klasik altında bulabilirsiniz. Microsoft AppSource ' de yapılan tüm satın almalar bu listede yer alır.

2021 Şubat 'tan önce Azure portal bir SaaS aboneliği satın aldıysanız ve bunu kiracının altındaki bir kaynak grubuna taşımak istiyorsanız (önerilir), **SaaS Classic** bölümünde SaaS aboneliğine gidin ve **kaynak grubuna Taşı**' yı seçin. Abonelikleri yalnızca **bekleyen** veya **etkin** durumda taşıyabilirsiniz. Bir kez taşındıktan sonra SaaS aboneliği, **SaaS klasik** değil **SaaS** görünümünde görüntülenir. Bir SaaS aboneliğini AppSource 'ta satın alınmış bir kaynak grubuna taşıyamazsınız.

Bu taşıma aşağıdaki avantajları sunar:

- Azure aboneliğindeki ve kaynak gruplarındaki (tam RBAC denetimi) devralınan ilke ve izinlerle SaaS kaynağınızın erişimi ve denetimi geliştirildi
- SaaS yaşam döngüsü, aktarım ve silme işlemleri gibi eylemler için Azure aboneliğinin yaşam döngüsüne bağlıdır
- Küresel arama kullanılarak SaaS kaynaklarıyla daha kolay bulunabilirliği
- Azure maliyet yönetimi kullanımı – SaaS kaynaklarında harcama Izleme
- Abonelik düzeyi kaynakların etkinlik günlüğünde kaynaklar olayları vardır

## <a name="manage-your-saas-service"></a>SaaS hizmetinizi yönetme

SaaS aboneliklerinizi yönetmenin birden çok yolu vardır

* Azure portal satın alınan SaaS abonelikleri için bunları orada yönetin.
* appsource 'ta satın alınan SaaS abonelikleri için, onları Azure portal ve [Microsoft 365 Yönetici merkezi](https://admin.microsoft.com/Adminportal/Home?#/subscriptions)' nde yönetin; Microsoft 365 Yönetici merkezini kullanma hakkında ayrıntılı bilgi için bkz. [kuruluşunuz için üçüncü taraf uygulama aboneliklerini yönetme](/microsoft-365/commerce/manage-saas-apps?view=o365-worldwide&preserve-view=true).
* Bazı yayımcılar, SaaS aboneliklerini doğrudan platformlarından yönetmenizi sağlar. Azure portal SaaS aboneliği sayfasındaki bir bağlantıyı kullanarak yayımcının sitesini ziyaret edin.

Satın alımınızın ardından gerçekleştirebileceğiniz birkaç eylem vardır; Bazıları, sahip veya katkıda bulunan izinleri gerektirecektir:

### <a name="change-plans"></a>Değişiklik planları

Abone olduğunuz bir plana yaptığınız değişiklikler hemen yürürlüğe girer. Faturalandırma, geçerli planın fatura dönemi uyarınca eşit olarak dağıtılır. Planların değiştirilmesi için **sahip** veya **katkıda bulunan** izinleri gerekir.

> [!NOTE]
> Seçtiğiniz değişiklikler kendi Hizmetleri içinde uygun değilse, yayımcı değişikliği onaylamayı reddedebilir. Bu durumda, değişiklik başarısız olur.

**Değişiklik planı** çalışmayabilir bazı durumlar vardır:

- Aboneliğiniz, **okuma** izinleriyle kiracı düzeyi altındaysa planı değiştiremezsiniz. Bu durumda, abonelik üzerinde **sahip** rolüne sahip olan kişiden izin isteyin.
- Azure aboneliğiyle ilişkili bir ödeme aracı (PI) yoksa ücretsiz planınızı ücretli bir plana değiştiremezsiniz. Ancak, farklı bir Azure aboneliği seçip ücretli bir plan seçebilir veya seçili Azure aboneliğine bir PI ekleyebilirsiniz.
- Seçtiğiniz planın geçerli kullanıcı sayısını içermeyen bir minimum/maksimum Kullanıcı sınırlaması varsa, satın aldığınız orijinal plana dahil olan ve aynı sayıda kullanıcı içeren farklı bir plan seçin veya yayımcıya başvurun.
- Yayımcı isteği yerine getiremiyorsa, doğrudan bunlarla iletişim kurun.

### <a name="change-number-of-users"></a>Kullanıcı sayısını değiştirme

Bilgisayar tabanlı planlar için, satın alma işlemi sırasında tanımladığınız kullanıcı sayısını ekleyebilir veya azaltabilirsiniz. Abone olduğunuz kullanıcıların sayısını değiştirmek hemen yürürlüğe girer ve faturalandırma geçerli planın fatura dönemi uyarınca eşit olarak dağıtılır. Yayımlamadaki değişiklikler yalnızca Yayımcı tarafından tanımlanan en düşük ve en fazla koltuk aralığında mümkündür. Bazı durumlarda, bilgisayarları değiştirmeden önce bir planı değiştirmeniz gerekecektir ve tam tersi de geçerlidir.

- Aboneliğiniz, okuma izinleriyle kiracı düzeyi altındaysa, kullanıcı sayısını değiştiremezsiniz. Bunun yerine, abonelik üzerinde sahip rolüne sahip olan kişiden katkıda bulunan izinleri Isteyin.
- Yayımcı isteği yerine getiremiyorsa, doğrudan bunlarla iletişim kurun.

> [!NOTE]
> Yayımcı, hizmeti içinde mümkün değilse değişikliği onaylamayı reddedebilir. Bu durumda, değişiklik başarısız olur.

### <a name="edit-recurring-billing"></a>Yinelenen faturalandırmayı Düzenle

Yinelenen faturalandırma, SaaS aboneliğinizin yenilenmesini yönetmenizi sağlar. Yinelenen faturalandırma devre dışı bırakıldığında, SaaS aboneliği ve hizmeti yenileme tarihinde sona erecek. Yenileme seçeneğini yalnızca abonelik etkin olduğunda değiştirebilirsiniz. Sonlandırılmış bir ve/veya iptal edilen SaaS aboneliği yeniden etkinleştirilemez; Yeni bir SaaS aboneliğinin yerinde oluşturulması gerekir.

### <a name="view-billing"></a>Faturalandırmayı görüntüle

Azure aboneliğiniz ve bu abonelik kullanılarak satın alınan Azure Market ürünleri için faturaları görüntüleyin. Portalda satın alınan SaaS için **faturalandırma** bölümündeki SaaS aboneliği sayfasında faturalandırma sayfasına bakın ve bu, sizi **Maliyet yönetimine** yönlendirmenizi sağlar.

Maliyet yönetimi, fatura dökümlerinizi anlamanıza, Faturalandırma hesabınızı ve aboneliklerinizi yönetmenize, Azure harcamalarınızı izlemenize/denetlemenize ve kaynak kullanımını iyileştirmenize yardımcı olur. Maliyetleri analiz etmenizi, bütçelerin oluşturulmasını ve yönetilmesini ve daha fazlasını yapmanızı sağlar. Örneğin, özel ölçüm kullanımınızı izlemenize (2021 Şubat 'tan sonra oluşturulan SaaS abonelikleri için veya bir kaynak grubuna taşındıktan) olanak tanır. Maliyet yönetimi hakkında daha fazla bilgi için bkz. [Azure maliyet yönetimi + faturalandırma belgeleri](/azure/cost-management-billing/).

Satın alımınızın Microsoft AppSource aracılığıyla yapılması durumunda faturanız **& ödemeler** bölümünde Microsoft Yönetim Merkezi 'nde yer alabilir.

### <a name="cancel-subscription"></a>Aboneliği iptal etme

İptal etme, bu SaaS aboneliğinin bir parçası olarak satın aldığınız yazılıma erişiminizi kaldırır. Para iadesi, geri ödeme ilkesine göre işlenir; Ayrıntılar için bkz. [Microsoft AppSource ve Azure Market Için para iadesi ilkeleri](refund-policies.md).

Aboneliğiniz, **okuma** izinleriyle kiracı düzeyi altındaysa, aboneliği iptal edemezsiniz. Bunun yerine, **sahip** izinlerine sahip kişiyle iletişim kurun.

14 günden daha uzun bir süre boyunca 24 saat veya yıllık veya çok yıllık bir abonelik için aylık bir SaaS aboneliğiniz varsa, aboneliğin geçerli dönemi (bkz. iptal ilkesi) için para iadesi kullanılacaktır. SaaS hesabı yapılandırıldıktan sonra tüketimi temel alan faturalandırma, para iadesi için de uygun değildir.

### <a name="delete-subscription"></a>Aboneliği silme

Bu eylem, SaaS abonelikleri listenizden SaaS kaynağını kaldırmanın eklenmesiyle birlikte iptal etme gibidir. Bir aboneliği sildikten sonra, Azure portal buna erişmeniz mümkün olmayacaktır.

Aboneliğiniz, **okuma** izinleriyle kiracı düzeyi altındaysa, bir aboneliği silemezsiniz. Bunun yerine, **sahip** izinlerine sahip kişiyle iletişim kurun.

### <a name="change-azure-subscription-andor-resource-group"></a>Azure aboneliğini ve/veya kaynak grubunu değiştirme

Azure portal satın alınan bir teklifle ilişkili bir aboneliği/kaynak grubunu değiştirmek için:

1. **SaaS** bölümüne gidin.
2. Değiştirilecek aboneliği seçin.
3. **Faturalandırma** bölümünde **faturalandırılan aboneliği Değiştir**' i seçin.
4. SaaS kaynağını taşımak için istenen abonelik/kaynak grubunu seçin veya yeni bir kaynak grubu oluşturun.
5. İşlemi gerçekleştirmek için en altta **Değiştir** ' i seçin.

Değişiklik çalışmamayabilir bazı durumlar vardır:

- SaaS aboneliğiniz abone durumunda değilse, SaaS bölümünde veya **SaaS** abonelik sayfanızda abonelik durumunu kontrol edin.
- SaaS aboneliği bir kiracı düzeyi kaynağı ise:
    - Hedef Azure aboneliğinde *sahip/katkıda bulunan* izinlerinizin olması gerekir.
- SaaS aboneliği bir abonelik düzeyi kaynağı ise:
    - Hedef Azure aboneliğine yönelik *okuma* veya *sahip/katkıda bulunan* izinlerinizin olması gerekir.
    - Hedef kaynak grubu için *sahip/katkıda bulunan Izinlerine sahip* olmanız gerekir.
    - Hedef kaynak grubunda aynı ada sahip bir SaaS aboneliği zaten varsa, farklı bir hedef kaynak grubu seçin.
- Hedef Azure aboneliği ve kaynak aboneliği, satın alma sırasında gerçekleştirilen tüm denetimleri üstlenecek. Satın alma denetimleri hakkında daha fazla bilgi edinmek için **Azure Portal SaaS teklifi satın alma** konusunun [SaaS aboneliği ve yapılandırması](purchase-saas-offer-in-azure-portal.md#saas-subscription-and-configuration) bölümüne bakın.

## <a name="next-steps"></a>Sonraki adımlar

- Markette zaten bir teklif satın aldıysanız [Faturalama'ya gidin](billing-invoicing.md)
- Özel plan seçenekleri hakkında [daha fazla bilgi](private-offers.md)
