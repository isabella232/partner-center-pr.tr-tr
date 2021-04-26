---
title: Bazı Skype Kurumsal abonelikleri geçirin
description: Süresi dolan Skype Kurumsal Çevrimiçi sürüm planı 1 abonelikleriyle belirli müşterileri yeni Office 365 sürümlerine nasıl ve ne zaman geçirebileceğinizi öğrenin.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: f395987ef647fa6f7ed264c6476ddae419eabc34
ms.sourcegitcommit: 26e6b470756aa9c1b3b0b919301b0eb38a335a52
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/26/2021
ms.locfileid: "108002867"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Skype Kurumsal Çevrimiçi Plan 1 aboneliklerini yeni Office 365 sürümlerine geçirme

**Uygun roller**

- Satış Aracısı

Skype Kurumsal Çevrimiçi kullanım planı 1, 1 Ağustos 2018 ' ten itibaren kullanımdan kaldırılacaktır. Bu tarihten sonra müşteriler artık yeni Skype Kurumsal plan 1 abonelikleri satın almayabilir ve mevcut abonelikler, süreleri dolduğunda otomatik olarak yenilenmez ve bir yenileme seçeneği sağlamacaktır. Aboneliğin ayrıntı sayfasında, Skype Kurumsal Çevrimiçi kullanım planı 1 abonelik durumu "otomatik yenilemede [Tarih]" içinde "süresi doluyor" olarak değiştirilmiştir.  

Müşterilerin devamlılığını sağlamak için, süresi dolan Skype Kurumsal çevrimiçi çalışma planı 1 aboneliklerine, aşağıda listelenen desteklenen bir SKU seçeneğine geçiş yapmanız gerekir. Müşterilerin hizmet kesintilerinden kaçınmak için, aboneliğin yıllık bitiş tarihinden önce müşterileri yeni aboneliklere taşımayı öneririz. 

>[!NOTE]
>Hem Skype Kurumsal Çevrimiçi kullanım planı 1 ticari hem de kamu SKU 'Ları devre dışı bırakıldı.

API 'YI (CREST veya Partner Center) kullanıyorsanız, Otomatik Yenile = false özelliğiyle birlikte Aboneliğin bitiş tarihini değerlendirerek süresi dolan abonelikleri bulun. Skype Kurumsal çevrimiçi çalışma planı 1 abonelikleri, 1 Eylül 2018 ' de otomatik yenileme = false olarak ayarlanacak. Müşterileri dilediğiniz zaman yeni bir plana taşıyabilirsiniz. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Skype Kurumsal Çevrimiçi için plan 1 yenileme planları

Yeni planlarla, müşterileriniz Office 365 ' deki yeni özelliklerden ve işlevlerden yararlanabilir. Fiyatlandırma ayrıntıları, Iş Ortağı Merkezi 'nde fiyat listesi ve teklif listesi matrisinde bulunur. 

- Seçenek 1: Office 365 Kurumsal F1
- Seçenek 2: F1 Microsoft 365 Kurumsal
- Seçenek 3: diğer Office 365 planları

|**Özellik**    |**1\. Seçenek**   |**2\. Seçenek**   |**Seçenek 3**   |
|:-----------------|:-----------------|:-------------|:------------|
|Skype Kurumsal çevrimiçi çalışma planı 1 ' de bulunan tüm özellikleri alın|Yes   |Yes   |Yes   |
|Anlık ileti ve varlık |Yes   |Yes   |Yes   |
|Uçtan uca ses ve IP üzerinden video|Yes   |Yes   |Yes   
|Toplantıları kimliği doğrulanmış bir kullanıcı olarak birleştirin| Yes   |Yes   |Yes   |

## <a name="transition-customers-to-new-product-plans"></a>Müşterilerin yeni ürün planlarına geçişini sağlar

Microsoft, iş ortaklarımız için sürekli olarak yeni ürün ve hizmetler sunar. Bu gibi durumlarda, müşterileri yeni hizmetlere yükseltmeniz veya sonunda kapatılacak SKU 'lardan aboneliklerini geçirmeniz gerekebilir. Müşterilerin Kullanımdan kaldırılmış SKU 'lardan daha yeni bir sürümüne geçirilmesi aşağıdaki adımları gerektirir:

- Yeni aboneliği satın alın
- Geçerli kullanıcı lisanslarını yeniden ata
- Eski aboneliği iptal et

### <a name="migrate-your-customers-to-new-plans"></a>Müşterilerinizi yeni planlara geçirin

1. Yeni aboneliği satın almak için **Iş Ortağı Merkezi menüsünden** **müşteriler**' i seçin, taşımak istediğiniz müşteriyi seçin ve ardından **Abonelik Ekle**' yi seçin.

2. Katalogdan satın almak istediğiniz aboneliği seçin (Bu durumda yukarıdaki seçeneklerden biri), lisansların sayısını girin ve ardından **Gönder**' i seçin. 

Müşterinizin artık eski ve yeni abonelikleri, eski Skype Kurumsal Çevrimiçi plan 1 aboneliğiniz ve yeni ' Target ' aboneliği olması gerekir. Örneğin, 1-Office 365 Kurumsal F1.

3. Müşterinin kullanıcılarının lisanslarını yeniden atamak için **Iş Ortağı Merkezi** menüsünden **müşteriler**' i seçin, taşıdığınız müşteriyi seçin ve ardından **Kullanıcılar ve lisanslar**' ı seçin. Müşterinin kullanıcılar ve lisanslar sayfası açılır.

4. Kullanıcı lisansını yeniden atamak için, yeniden atanacak kullanıcıyı seçin ve ardından **Lisansları Yönet** ' i seçin.

5. **Lisansları Yönet** sayfasında, Skype Kurumsal Çevrimiçi plan 1 Lisansı onay kutusunu temizleyin ve müşterinin hareket ettirilmesi için kullanılacak abonelik için yeni bir hizmet planı seçin.

6. **Gönder**’i seçin. Bir onay sayfası yeni lisans atamalarını listeler. Lisans atamaları gerektiren diğer kullanıcılar için aynı işleme devam edin.

Kullanıcı lisansını yeni hizmete taşıdıktan sonra, kullanımdan kaldırılan aboneliği müşteri düzeyinde güvenle iptal edebilirsiniz.

7. **Iş Ortağı Merkezi** menüsünde **müşteriler**' i seçin. Aboneliğini iptal ettiğiniz müşteriyi seçin.

8. Abonelik Ayrıntıları sayfasında, aboneliği **askıya alındı** olarak ayarlayın.

9. Gönder ' i seçin **.**

Eski abonelik askıya alındı ve yeni abonelik etkin. Askıya alınan abonelik 120 gün sonra otomatik olarak sağlanacaktır. Müşteri, eski abonelik için ek maliyet içermez.

## <a name="next-steps"></a>Sonraki adımlar

- [Danışmanları: Office 365 ' i denemek için istemciler için deneme daveti oluşturma ve gönderme](advisors-create-a-trial-invitation.md)
- [Danışmanları: Office 365 deneme davetleri ve satın alma tekliflerle istemci tabanınızı derleme](advisors-build-your-business.md)
- [Danışmanları: satın alma teklifi oluşturma](advisor-create-a-purchase-offer.md)
