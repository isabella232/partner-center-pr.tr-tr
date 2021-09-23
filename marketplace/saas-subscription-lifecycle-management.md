---
title: Hizmet Olarak Yazılım (SaaS) aboneliği yaşam döngüsü yönetimi
description: Hizmet Olarak Yazılım (SaaS) aboneliği yaşam döngüsü yönetimi Azure Market.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
ms.date: 08/20/2021
ms.author: yonits
author: yonits
ms.openlocfilehash: c5f06fb88a29def9df8d8cc2936f9eea91d8b2b4
ms.sourcegitcommit: fceaca54b0ec695cf214209c09b4516e1b40866a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/23/2021
ms.locfileid: "128322059"
---
# <a name="saas-subscription-lifecycle-management"></a>SaaS aboneliği yaşam döngüsü yönetimi

Bu makalede SaaS kaynağını bulma, SaaS ile SaaS Klasik arasındaki farklar ve saas kaynak yönetimi arasındaki farklar Azure portal.

## <a name="find-a-saas-resource"></a>SaaS kaynağı bulma

Azure Market'dan bir SaaS teklifi satın aldığınız zaman, Azure portal'da hizmet olarak yazılım (SaaS) aboneliği oluşturur (ayrıntılar için bkz. Azure portal' [da SaaS teklifi satın alma).](purchase-saas-offer-in-azure-portal.md) Portalda bir SaaS kaynağı bulmak için:

- **Genel Arama penceresi** (üst) – SaaS aboneliğinizi adıyla arama.
- **SaaS:** Tüm SaaS aboneliklerinizi listeler. İki tür SaaS listesi vardır; aşağıdaki bölüme bakın.
- **Abonelikler:** Kiracınız kapsamında erişiminiz olan tüm Azure aboneliklerini listeler. Belirli bir aboneliği bulmak için filtre veya arama penceresini kullanın.
- **Tüm kaynaklar** – Erişiminiz olan tüm abonelikler altında oluşturulan tüm kaynakları listeler. Belirli bir aboneliği bulmak için filtresini kullanın (SaaS > yazın) veya listede arama.

## <a name="differences-between-saas-and-saas-classic-lists-of-resources-in-the-azure-portal"></a>SaaS ile SaaS Klasik kaynak listeleri arasındaki farklar Azure portal

Bu iki tür arasındaki fark, SaaS Klasik'in bir kaynak grubu altında değil, kiracınız altında oluşturulan SaaS aboneliklerini bulmanızı sağlar.
Azure portal Şubat 2021'den önce bir SaaS aboneliği satın aldıysanız, bu abonelik kiracınız altında oluşturulmuş ve SaaS Klasik altında bulabilirsiniz. Bu listede Microsoft AppSource satın almalar yer almaktadır.

Azure portal'de Şubat 2021'den önce bir SaaS aboneliği satın aldıysanız ve bunu Kiracı'nın altından bir Kaynak grubuna taşımak (önerilir), SaaS Klasik bölümündeki **SaaS** aboneliğine gidin ve Kaynak Grubuna Taşı'ya **tıklayın.** Abonelikleri yalnızca Beklemede veya **Etkin durumda** **taşıyabilirsiniz.** Taşındıktan sonra SaaS aboneliği artık **SaaS** Klasik görünümünde **değil, SaaS görünümünde görünür.** AppSource'ta satın alınan bir SaaS aboneliğini bir kaynak grubuna taşıyabilirsiniz.

Bu taşıma aşağıdaki avantajları sunar:

- Azure aboneliğinden ve Kaynak gruplarından devralınan ilkeler ve izinlerle SaaS kaynağınıza erişim ve denetimi iyileştirildi (tam RBAC denetimi)
- SaaS'nin yaşam döngüsü, aktarımlar ve silmeler gibi eylemler için Azure aboneliğinin yaşam döngüsüne bağlanır
- SaaS kaynakları ile daha kolay bulunabilirlik, genel arama
- Azure Maliyet Yönetimi kullanımı – SaaS kaynaklarına yapılan harcamaları izleme
- Abonelik düzeyindeki kaynaklarda Etkinlik günlüğünde kaynak olayları var

## <a name="manage-your-saas-service"></a>SaaS hizmetinizi yönetme

SaaS aboneliklerinizi yönetmenin birden çok yolu vardır

* Hizmette satın alınan SaaS abonelikleri Azure portal burada yönetin.
* AppSource'ta satın alınan SaaS abonelikleri için bunları Azure portal ve [Microsoft 365 Yönetim Merkezi'nde yönetin;](https://admin.microsoft.com/Adminportal/Home?#/subscriptions) Microsoft 365 Yönetim Merkezi'ni kullanma hakkında ayrıntılı bilgi için bkz. Üçüncü [taraf uygulama aboneliklerini yönetme.](/microsoft-365/commerce/manage-saas-apps?view=o365-worldwide&preserve-view=true)
* Bazı yayımcılar SaaS aboneliklerini doğrudan platformlarında yönetmenizi sağlar. Uygulamanın SaaS aboneliği sayfasındaki bağlantıyı kullanarak yayımcının sitesini Azure portal.

Satın alımınız sonrasında gerçekleştir eylemler gerçekleştirin; Bazılarında Sahip veya Katkıda Bulunan izinleri gerekir:

### <a name="change-plans"></a>Değişiklik planları

Abone olduğunuz bir planda yaptığınız değişiklikler hemen etkili olur. Faturalama, geçerli planın faturalama dönemine göre provok olarak iki nizamlı olarak hazırlar. Planları değiştirmek için **Sahip veya Katkıda** Bulunan **izinleri** gerekir.

> [!NOTE]
> Yayımcı, kendi hizmetlerinde uygun olmayan değişiklikleri seçerse değişikliği onaylamayı reddedebilir. Bu durumda değişiklik başarısız olur.

Değişiklik planının **çalışmay olabileceği bazı** durumlar vardır:

- Aboneliğiniz Okuma izinlerine sahip Kiracı **düzeyinde** ise planı değiştiremezsiniz. Bu durumda, abonelikte Sahip rolüne sahip **olan kişiden** izin isteğinde bulundurabilirsiniz.
- Azure Aboneliği ile ilişkili ödeme aracı (PI) yoksa ücretsiz planınızı ücretli planla değiştiremezsiniz. Ancak, farklı bir Azure Aboneliği seçebilir ve ardından ücretli bir plan seçebilir veya seçili Azure Aboneliğine pi eklersiniz.
- Seçtiğiniz planda geçerli kullanıcı sayısına dahil olmayan en düşük/en yüksek kullanıcı sınırlaması varsa, satın aldığınız özgün plana dahil edilen kullanıcı sayısına sahip farklı bir plan seçin veya yayımcıyla iletişime geçin.
- Yayımcı isteği yerine getirene kadar doğrudan iletişim kurun.

### <a name="change-number-of-users"></a>Kullanıcı sayısını değiştirme

Lisans tabanlı planlar için, satın alma işlemi sırasında tanımlandığı kullanıcı sayısını ekleyebilir veya azaltabilirsiniz. Abone olduğunuz kullanıcı sayısını değiştirmek hemen geçerli olur ve faturalama geçerli planın faturalama dönemine göre provokasyona tabi olur. Yayımcı tarafından tanımlandığı gibi, yalnızca en düşük ve en yüksek yer aralığı içinde yer alan yer değişiklikleri mümkündür. Bazı durumlarda, yer değiştirmeden önce bir planı değiştirmelisiniz ve bunun tersi de geçerlidir.

- Aboneliğiniz Okuma izinlerine sahip Kiracı düzeyinde ise kullanıcı sayısını değiştiremezsiniz. Bunun yerine, abonelikte Sahip rolüne sahip olan kişiden Katkıda Bulunan izinleri isteğinde bulunabilirsiniz.
- Yayımcı isteği yerine getirene kadar doğrudan iletişim kurun.

> [!NOTE]
> Yayımcı, kendi hizmetlerinde uygulanabilir durumda olmayan değişikliği onaylamayı reddedebilir. Bu durumda değişiklik başarısız olur.

### <a name="edit-recurring-billing"></a>Yinelenen faturalamayı düzenleme

Yinelenen faturalama, SaaS aboneliğinizin yenileme işlemlerini yönetmenize olanak sağlar. Yinelenen faturalama kapalı olduğunda SaaS aboneliği ve hizmeti yenileme tarihine göre sonlandırılır. Yenileme seçeneğini yalnızca abonelik etkinken değiştirebilirsiniz. Sonlandırılan ve/veya iptal edilen Bir SaaS aboneliği yeniden etkinleştirilmemektedir; Yeni bir SaaS aboneliğinin yerinde oluşturulmuş olması gerekir.

### <a name="view-billing"></a>Faturalamayı görüntüleme

Azure aboneliğinizin faturalarını ve bu Azure Market satın alınan ürünleri görüntüleme. Portalda satın alınan SaaS için, Sizi Maliyet Yönetimi'ne yönlendirecek Olan Faturalama bölümündeki SaaS aboneliği sayfasındaki faturalama **sayfasına bakın.** 

Maliyet Yönetimi fatura dökümünü anlamanıza, ödeme hesabınızla aboneliklerinizi yönetmenize, Azure harcamalarınızı izlemenize/denetlemenize ve kaynak kullanımını iyileştirmenize yardımcı olur. Maliyetleri analiz etmenize, bütçeler oluşturmanıza ve yönetmenize ve daha fazlasını sağlar. Örneğin, özel ölçüm kullanımınızı (Şubat 2021'den sonra oluşturulan veya bir kaynak grubuna taşınan SaaS abonelikleri için) izlemenizi sağlar. Maliyet yönetimi hakkında daha fazla bilgi için [Azure Maliyet Yönetimi + Faturalama edinin.](/azure/cost-management-billing/)

Satın alma Microsoft AppSource, Faturalar ve ödemeler altında Microsoft Yönetim **Merkezi'nde & görüntüebilirsiniz.**

### <a name="cancel-subscription"></a>Aboneliği iptal etme

İptal etme işlemi, bu SaaS aboneliğinin bir parçası olarak satın aldığınız yazılıma erişiminizi kaldırır. Para iadeleri para iadesi ilkesine göre işlenir; Ayrıntılar için bkz. [Para iadesi ilkeleri Microsoft AppSource ve Azure Market.](refund-policies.md)

Aboneliğiniz Okuma izinlerine sahip Kiracı **düzeyinde ise** aboneliği iptal etmenize izin vezin. Bunun yerine Sahip izinlerine sahip olan **kişiye** ulaşın.

Aylık SaaS aboneliğiniz 24 saati veya 14 gün boyunca bir yıllık veya çok yıllık aboneliğiniz varsa, aboneliğin geçerli dönemi için para iadesi kullanılmaz (bkz. iptal ilkesi). SaaS hesabı yapılandırıldığında tüketime göre faturalandırma da para iadesi için uygun değildir.

### <a name="delete-subscription"></a>Aboneliği silme

Bu eylem iptal etmek gibi bir işlemdir ve SaaS kaynağını SaaS abonelikleri listesinden kaldırmayı da içerir. Bir aboneliği sildikten sonra abonelikten bu aboneliğe Azure portal.

Aboneliğiniz Okuma izinlerine sahip Kiracı **düzeyinde ise** aboneliği silemezsiniz. Bunun yerine Sahip izinlerine sahip olan **kişiye** ulaşın.

### <a name="change-azure-subscription-andor-resource-group"></a>Azure aboneliğini ve/veya kaynak grubunu değiştirme

Teklifte satın alınan bir teklifle ilişkili bir aboneliği/kaynak grubunu Azure portal:

1. **SaaS bölümüne** gidin.
2. Değiştir istediğiniz aboneliği seçin.
3. **Faturalama'nın** altında **Faturalı aboneliği değiştir'i seçin.**
4. SaaS kaynağını taşımak için istediğiniz aboneliği/kaynak grubunu seçin veya yeni bir kaynak grubu oluşturun.
5. İşlem **tamamlamak** için alttaki Değiştir'i seçin.

Değişikliğin çalışmay olabileceği bazı durumlar vardır:

- SaaS Aboneliğiniz Abone olunan durumda değilse SaaS bölümünde veya **SaaS** aboneliği sayfasında abonelik durumunu kontrol edin.
- SaaS aboneliği kiracı düzeyinde bir kaynaksa:
    - Hedef Azure *aboneliğinde Sahip/Katkıda* Bulunan izinlerine sahipsiniz.
- SaaS aboneliği abonelik düzeyinde bir kaynaksa:
    - Hedef Azure *Aboneliği için* Okuma *veya Sahip/Katkıda* Bulunan izinlerine ihtiyacınız vardır.
    - Hedef kaynak *grubu için Sahip/Katkıda* Bulunan izinlerine ihtiyacınız vardır.
    - Hedef kaynak grubunda aynı adla bir SaaS aboneliği zaten varsa, farklı bir hedef kaynak grubu seçin.
- Hedef Azure aboneliği ve kaynak aboneliği, satın alma sırasında gerçekleştirilen tüm denetimlerden geçiriliyor. Satın alma denetimleri hakkında daha fazla bilgi edinmek için, Azure portal'da SaaS teklifi satın alma bölümündeki [SaaS](purchase-saas-offer-in-azure-portal.md#saas-subscription-and-configuration) **Aboneliği ve yapılandırma bölümüne bakın.**

## <a name="next-steps"></a>Sonraki adımlar

- Market 'te zaten bir teklif satın aldıysanız [faturalandırma ve faturalama](billing-invoicing.md) ' ya gidin.
- [Özel plan](./private-plans.md) seçenekleri hakkında daha fazla bilgi edinin