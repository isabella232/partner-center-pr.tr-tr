---
title: Market ürünlerini ve & yönetme
ms.topic: how-to
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Bulut İş Ortağı Merkezi Kullanarak, Bulut Çözümü Sağlayıcılarının ticari marketten müşteriler için satın alınan üçüncü taraf ISV tekliflerini nasıl yöneteceklerini öğrenin.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e1bb2752dad5325478496c83fc368943780d8afb
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147913"
---
# <a name="manage-commercial-marketplace-products-and-offers-for-your-customers"></a>Müşterileriniz için ticari market ürünlerini ve tekliflerini yönetme


**Uygun roller:** Genel yönetici | Yönetici aracısı

Bulut Çözümü Sağlayıcısı (CSP) programı iş ortakları, ticari marketten müşterileri için İş Ortağı Merkezi ISV SaaS tekliflerini veya aboneliklerini satın almak için İş Ortağı Merkezi portalını kullanabilir. Bir teklifi satın aldığınız zaman, bunu yönetmek için çeşitli yollarınız vardır.

## <a name="view-or-edit-a-subscription"></a>Aboneliği görüntüleme veya düzenleme

Bir üçüncü taraf ISV yayımcısı aboneliği satın aldıktan sonra, aboneliği aşağıdaki gibi gözden geçirebilirsiniz veya düzenleyebilirsiniz:

1. Panoda oturum İş Ortağı Merkezi [ve](https://partner.microsoft.com/dashboard)ardından **sol** gezinti menüsünden Müşteriler'i seçin.

2. Uygun müşteriyi ve ardından Abonelikler'i **seçin.** Bu, müşteri için satın aldığınız tüm lisans tabanlı abonelikleri listeler.

3. Abonelik **sütununda** görüntülemek veya düzenlemek istediğiniz aboneliği seçin. Bu, teklifi ayarlamak veya sağlama hakkında daha fazla bilgi sağlar. (Teklifte daha fazla eylem gerekirse Durum sütununda "Eylem Gerekiyor" durumu da görüntüleniyor olabilir. Buna ISV yayımcısı sitesine bir bağlantı da eşlik ediyor olabilir.)

4. Görüntülemek veya düzenlemek istediğiniz aboneliği seçmenizin ardından abonelik ayrıntı sayfası, aboneliği düzenlemenizi ve aşağıdaki gibi şeyler yapmanizi sağlar:

    - Abonelik takma adını değiştirme

    - Abonelikte lisans ekleme/azaltma

    - Aboneliği iptal etme

    - Otomatik yenilemeyi kapat

    - Varsa Dolaylı Kurumsal Bayi MPN Kimliği ekleme

> [!NOTE]
> Abonelik iptal etme gibi bir abonelikte bazı değişiklikler yapabilmeniz için önce ISV yayımcısı tarafından tanımlanan belirli adımları gerçekleştirmeniz gerekebilir.

## <a name="assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer"></a>Lisans atama ve bir aboneliği müşteri adına etkinleştirme

Ticari Market 'te bağımsız bir yazılım satıcısı (ISV) yayımcısı tarafından sağlanmış bir hizmet olarak yazılım (SaaS) teklifi satın aldığınızda, ISV yayımcısı, lisans atama ve müşterinizin adına abonelik etkinleştirme sürecinin yönetilmesine yardımcı olur.

Yayımcı size kişiselleştirilmiş bir bağlantı ve belirli satın alma bilgilerinizi tanımlayan bir yetkilendirme kodu sağlamalıdır.

1. Bu kişiselleştirilmiş bağlantıyı birkaç yolla ISV yayımcısından bulabilirsiniz:

   - Bir ISV SaaS teklifi satın aldıktan sonra görünen onay sayfasından bağlantıyı görebilirsiniz. Sayfada bu bağlantıyı bulmak için **yayımcının sitesine git**' i bulun ve seçin.

   - Bağlantıyı belirli müşterinin abonelikler sayfasından görebilirsiniz. Bu Yayımcı bağlantısı, müşteri için satın alınan ISV teklifiyle veya abonelikle ilişkili satırda görüntülenir.

   - [Iş Ortağı Merkezi API 'lerini kullanarak bağlantı alabilirsiniz](/partner-center/develop/get-activation-link-by-order-line-item).

   > [!NOTE]
   > Bunu Müşterinizin adına yapmak için, kişiselleştirilmiş bağlantıyı kopyalamanız, özel bir tarayıcıya yapıştırmanız ve müşterinin kimlik bilgilerini girmeniz gerekebilir.

2. ISV yayımcısının sitesinde veya sisteminde olduktan sonra, Yayımcı, müşteri kurulum işlemini tamamlamaya ve lisans sağlamanıza veya atamaya yönelik ek adımlar hakkında bilgi sahibi olur.

3. CSP programında müşteriniz adına çalışan bir iş ortağı olarak, aşağıdaki görevleri gerçekleştirmekten siz sorumlusunuz:

    - Gerekli bilgileri yayımcıya gönderebilirsiniz.

    - Gerekli URL 'YI doğrudan müşterinize gönderin (veya aksi takdirde bu abonelikle ilgili ayrıntıları müşterinize doğrudan gönderin)

4. Yayımcıya gerekli bilgileri sağlamadıktan sonra, yayımcı uygun lisansları sağlayacak ve atayacaktır. Abonelik faturalandırması yalnızca aşağıdaki olaylar gerçekleşdikten sonra başlayacak:

    - ISV yayımcısı uygun lisansları başarıyla atadı

    - ISV yayımcısı Microsoft'a (ayrı bir SaaS gerçekleştirme API'si aracılığıyla) hesap kurulumunun başarıyla tamamlanmıştır

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>ISV yayımcısı için lisans tabanlı SaaS aboneliğini iptal etme

Ticari markette bir ISV yayımcısı tarafından sunulan lisans tabanlı Bir SaaS ürününe abone olursanız, aboneliği belirlenen iptal süresi içinde iptal etme seçeneğiniz vardır. Bu iptal süresi, aylık veya yıllık aboneliğiniz olup olmadığınıza bağlı olarak değişir. Ayrıca aboneliği otomatik olarak yenilemeyi de seçebilirsiniz.

Geçerli iptal dönemleri, aboneliği iptal etme veya bir aboneliği otomatik yenileme hakkında daha fazla bilgi için bkz.

- [Aboneliği iptal etme](create-a-new-subscription.md#cancel-a-subscription)

- [Ticari market aboneliğini otomatik yenileme](create-a-new-subscription.md#choose-whether-to-automatically-renew-a-commercial-marketplace-subscription)

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>SaaS aboneliği için lisans ekleme veya kaldırma

SaaS ticari market tekliflerinde müşteri aboneliği için kullanıcı lisansları ekleyebilir veya kaldırabilirsiniz.

1. Panoda oturum İş Ortağı Merkezi [ve](https://partner.microsoft.com/dashboard)ardından **sol** gezinti menüsünden Müşteriler'i seçin.

2. Uygun müşteriyi ve ardından Abonelikler'i **seçin.** Bu, müşteri için satın aldığınız tüm lisans tabanlı abonelikleri listeler.

3. Abonelik **sütununda** değiştirmek istediğiniz aboneliği seçin.

4. Abonelik ayrıntıları sayfasında **Quantity alanını** bulun. Burada lisans sayısını artırabilir veya azaltabilirsiniz.

5. Miktarı değiştirerek Gönder'i **seçin.**

## <a name="manage-subscriptions-using-partner-center-apis"></a>Api'leri kullanarak İş Ortağı Merkezi yönetme

Ayrıca aboneliklerinize İş Ortağı Merkezi yönetimi gerçekleştirmek ve faturaları yönetmek için api'leri kullanabilirsiniz. Daha fazla bilgi için bkz. [ticari Market ürünleri için abonelik oluşturma](/partner-center/develop/create-subscription-azure-marketplace-products).

## <a name="next-steps"></a>Sonraki adımlar

- [Ticari Market tekliflerini satın alma](csp-commercial-marketplace-purchase.md)
- [Ticari Market 'te faturalandırma hakkında bilgi edinin](csp-commercial-marketplace-billing.md)