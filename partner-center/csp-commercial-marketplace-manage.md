---
title: Market ürünlerini ve & yönetme
ms.topic: how-to
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Bulut İş Ortağı Merkezi Kullanarak, Bulut Çözümü Sağlayıcılarının ticari marketten müşteriler için satın alınan üçüncü taraf ISV tekliflerini nasıl yöneteceklerini öğrenin.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14901b47b7363b2d87861be43a7071d9f23545cc
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248619"
---
# <a name="manage-commercial-marketplace-products-and-offers-for-your-customers"></a>Müşterileriniz için ticari market ürünlerini ve tekliflerini yönetme


**Uygun roller:** Genel yönetici | Yönetici aracısı

Bulut Çözümü Sağlayıcısı (CSP) programı iş ortakları, ticari marketten müşterileri için İş Ortağı Merkezi ISV SaaS tekliflerini veya aboneliklerini satın almak için İş Ortağı Merkezi portalını kullanabilir. Bir teklifi satın aldığınız zaman, teklifi yönetmek için çeşitli yollarınız vardır.

## <a name="view-or-edit-a-subscription"></a>Aboneliği görüntüleme veya düzenleme

Bir üçüncü taraf ISV yayımcısı aboneliği satın aldıktan sonra, aboneliği aşağıdaki gibi gözden geçirebilirsiniz veya düzenleyebilirsiniz:

1. Panoda oturum İş Ortağı Merkezi [ve](https://partner.microsoft.com/dashboard)ardından **sol** gezinti menüsünden Müşteriler'i seçin.

2. Uygun müşteriyi ve ardından Abonelikler'i **seçin.** Bu, müşteri için satın aldığınız lisans tabanlı abonelikleri listeler.

3. Abonelik **sütununda** görüntülemek veya düzenlemek istediğiniz aboneliği seçin. Bu, teklifi ayarlamak veya sağlama hakkında daha fazla bilgi sağlar. (Teklifte daha fazla eylem gerekirse Durum sütununda "Eylem Gerekiyor" durumu da görüntüleniyor olabilir. Buna ISV yayımcısı sitesine bir bağlantı da eşlik ediyor olabilir.)

4. Görüntülemek veya düzenlemek istediğiniz aboneliği seçmenizin ardından abonelik ayrıntı sayfası, aboneliği düzenlemenizi ve aşağıdaki gibi şeyler yapmanizi sağlar:

    - Abonelik takma adını değiştirme

    - Abonelikte lisans ekleme/azaltma

    - Aboneliği iptal etme

    - Otomatik yenilemeyi kapat

    - Varsa Dolaylı Kurumsal Bayi MPN Kimliği ekleme

> [!NOTE]
> Bir abonelikte bazı değişiklikler (aboneliği iptal etme gibi) gerçekleştiremeden önce ISV yayımcısı tarafından tanımlanan belirli adımları tamamlamanız gerekir.

## <a name="assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer"></a>Müşteri adına lisans atama ve aboneliği etkinleştirme

Ticari markette Bağımsız Yazılım Satıcısı (ISV) yayımcısı tarafından sağlanan bir Hizmet Olarak Yazılım (SaaS) teklifi satın aldığınız zaman, ISV yayımcısı, müşteriniz adına lisans atama ve aboneliği etkinleştirme işlemini yönetmeye yardımcı olur.

Yayımcı size kişiselleştirilmiş bir bağlantı ve satın almanızı tanımlayan bir yetkilendirme kodu sağlatır.

1. IsV yayımcısı bu kişiselleştirilmiş bağlantıyı birkaç şekilde bulabilirsiniz:

   - IsV SaaS teklifi satın aldıktan sonra görüntülenen onay sayfasından bağlantıyı görebilirsiniz. Sayfada bu bağlantıyı bulmak için Yayımcının sitesine **git'i bulun ve seçin.**

   - Bağlantıyı belirli bir müşterinin Abonelikler sayfasında görebilirsiniz. Bu yayımcı bağlantısı, müşteri için satın alınan ISV teklifi veya aboneliğiyle ilişkili satırda görünür.

   - Bağlantıyı [api'leri kullanarak İş Ortağı Merkezi edinebilirsiniz.](/partner-center/develop/get-activation-link-by-order-line-item)

   > [!NOTE]
   > Bunu müşteriniz adına yapmak için kişiselleştirilmiş bağlantıyı kopyalamanız, özel bir tarayıcıya yapıştırmanız ve müşterinin kimlik bilgilerini girmeniz gerekir.

2. ISV yayımcısı sitesine veya sistemine başladıktan sonra, yayımcı müşteri kurulum işlemini tamamlamak ve lisans sağlamak veya atamak için atılması gereken ek adımları size sağlar.

3. CSP programında müşteriniz adına çalışan bir iş ortağı olarak, aşağıdaki görevleri gerçekleştirmek sizin sorumluluğundadır:

    - Yayımcıya gerekli bilgileri gönderin.

    - Gerekli URL'leri doğrudan müşterinize gönderin (veya bu abonelikle ilgili ayrıntıları doğrudan müşterinize iletebilirsiniz)

4. Yayımcıya gerekli bilgileri verdiktan sonra yayımcı uygun lisansları sağlar ve atar. Abonelik faturalaması ancak aşağıdaki olaylar olduktan sonra başlar:

    - ISV yayımcısı uygun lisansları başarıyla atadı

    - ISV yayımcısı Microsoft'a (ayrı bir SaaS gerçekleştirme API'si aracılığıyla) hesap kurulumunun başarıyla tamamlanmıştır

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>ISV yayımcısı için lisans tabanlı SaaS aboneliğini iptal etme

Ticari markette bir ISV yayımcısı tarafından sunulan lisans tabanlı Bir SaaS ürününe abone olursanız, aboneliği belirlenen iptal süresi içinde iptal etme seçeneğiniz vardır. Bu iptal süresi aylık veya yıllık aboneliğiniz olup olmadığınıza bağlı olarak değişir. Ayrıca aboneliği otomatik olarak yenilemeyi de seçebilirsiniz.

Geçerli iptal dönemleri, aboneliği iptal etme veya otomatik yenileme hakkında daha fazla bilgi için bkz. [Aboneliği iptal etme.](create-a-new-subscription.md#cancel-a-subscription)

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>SaaS aboneliği için lisans ekleme veya kaldırma

SaaS ticari market tekliflerinde müşteri aboneliği için kullanıcı lisansları ekleyebilir veya kaldırabilirsiniz.

1. Panoda oturum İş Ortağı Merkezi [ve](https://partner.microsoft.com/dashboard)ardından **sol** gezinti menüsünden Müşteriler'i seçin.

2. Uygun müşteriyi ve ardından Abonelikler'i **seçin.** Bu, müşteri için satın aldığınız lisans tabanlı abonelikleri listeler.

3. Abonelik **sütununda** değiştirmek istediğiniz aboneliği seçin.

4. Abonelik ayrıntıları sayfasında **Quantity alanını** bulun. Burada lisans sayısını artırabilir veya azaltabilirsiniz.

5. Miktarı değiştirerek Gönder'i **seçin.**

## <a name="manage-subscriptions-using-partner-center-apis"></a>Api'leri kullanarak İş Ortağı Merkezi yönetme

Ayrıca abonelikleriniz için İş Ortağı Merkezi yönetimi gerçekleştirmek ve faturaları yönetmek için api'leri kullanabilirsiniz. Daha fazla bilgi için [bkz. Ticari market ürünleri için abonelik oluşturma.](/partner-center/develop/create-subscription-azure-marketplace-products)

## <a name="next-steps"></a>Sonraki adımlar

- [Ticari market tekliflerini satın alma](csp-commercial-marketplace-purchase.md)
- [Ticari markette faturalama hakkında bilgi alın](csp-commercial-marketplace-billing.md)
