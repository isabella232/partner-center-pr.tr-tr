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
ms.openlocfilehash: 0e8289ad06dbc8a95f5cff22ca386176d6ba65ab
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854834"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Skype Kurumsal Çevrimiçi Plan 1 aboneliklerini yeni Office 365 sürümlerine geçirme

**Uygun roller**: satış Aracısı

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
|IM ve varlık |Yes   |Yes   |Yes   |
|IP üzerinden eşler arası Ses ve Video|Yes   |Yes   |Yes   
|Kimliği doğrulanmış kullanıcı olarak toplantılara katılın| Yes   |Yes   |Yes   |

## <a name="transition-customers-to-new-product-plans"></a>Müşterileri yeni ürün planlarına geçiş

Microsoft, iş ortaklarımıza sürekli olarak yeni ürün ve hizmetler sunmaktadır. Bu durumlarda, müşterileri yeni hizmetlere yükseltmeniz veya aboneliklerini sonunda kapatılacak olan SKUS'lardan geçirmeniz gerekir. Müşterileri, eski SKÜ'lerden yeni SKUS'lara şu adımların atılması gerekir:

- Yeni aboneliği satın alma
- Geçerli kullanıcı lisanslarını yeniden atama
- Eski aboneliği iptal etme

### <a name="migrate-your-customers-to-new-plans"></a>Müşterilerinizi yeni planlara geçirme

1. Yeni aboneliği satın almak için, **İş Ortağı Merkezi menüsünde** Müşteriler'i **seçin,** taşımak istediğiniz müşteriyi seçin ve ardından Abonelik **ekle'yi seçin.**

2. Katalogdan satın almak istediğiniz aboneliği seçin (bu durumda, yukarıdaki seçeneklerden biri), lisans sayısını girin ve gönder'i **seçin.** 

Müşterinizin artık hem eski hem de yeni abonelikleri, eski Skype Kurumsal Çevrimiçi Plan 1 aboneliği ve yeni 'hedef' aboneliği (örneğin, Seçenek 1 - Office 365 Kurumsal F1) olması gerekir.

3. Müşterinin kullanıcı lisanslarını yeniden atamak için, **İş Ortağı Merkezi** menüsünden Müşteriler'i **seçin,** hareket halindeki müşteriyi seçin ve ardından Kullanıcılar ve **lisanslar'ı seçin.** Müşterinin Kullanıcılar ve Lisanslar sayfası açılır.

4. Kullanıcı lisansını yeniden atamak için, yeniden ataması yapılan kullanıcıyı seçin ve ardından Lisansları **yönet'i seçin.**

5. Lisansları **yönet sayfasında,** Skype Kurumsal Çevrimiçi Plan 1 lisansı onay kutusunun işaretini kaldırın ve müşterinin taşınıyor olduğu abonelik için yeni bir hizmet planı seçin.

6. **Gönder**’i seçin. Onay sayfasında yeni lisans atamaları listelemektedir. Lisans ataması gereken diğer kullanıcılar için de aynı işlemi devam eder.

Kullanıcı lisansını yeni hizmete taşıdıktan sonra, kullanımdan kaldırılan aboneliği müşteri düzeyinde güvenle iptal edebilirsiniz.

7. **Iş Ortağı Merkezi** menüsünde **müşteriler**' i seçin. Aboneliğini iptal ettiğiniz müşteriyi seçin.

8. Abonelik Ayrıntıları sayfasında, aboneliği **askıya alındı** olarak ayarlayın.

9. Gönder ' i seçin **.**

Eski abonelik askıya alındı ve yeni abonelik etkin. Askıya alınan abonelik 120 gün sonra otomatik olarak sağlanacaktır. Müşteri, eski abonelik için ek maliyet içermez.

## <a name="next-steps"></a>Sonraki adımlar

- [Danışmanları: Office 365 ' i denemek için istemciler için deneme daveti oluşturma ve gönderme](advisors-create-a-trial-invitation.md)
- [Danışmanları: Office 365 deneme davetleri ve satın alma tekliflerle istemci tabanınızı derleme](advisors-build-your-business.md)
- [Danışmanları: satın alma teklifi oluşturma](advisor-create-a-purchase-offer.md)
