---
title: Abonelikleri Skype Kurumsal geçirme
description: Süresi dolan Skype Kurumsal Online Plan 1 abonelikleri olan belirli müşterilerin yeni sürümlere nasıl ve ne zaman geçir Office 365 öğrenin.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: 58908e966eb80d219afa0cbc8c043932f5aef1a1
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114842516"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Skype Kurumsal Çevrimiçi Plan 1 aboneliklerini yeni Office 365 sürümlerine geçirme

**Uygun roller:** Satış aracısı

Skype Kurumsal Online Plan 1, 1 Ağustos 2018'den itibaren geçerli olacak şekilde, kaldırılamayacak. Bu tarihten sonra müşteriler Skype Kurumsal Plan 1 aboneliklerini satın alamayacak ve mevcut abonelikler süresi dolduğunda otomatik olarak yenilenmez ve bir yenileme seçeneği sağlanmaz. Aboneliğin ayrıntı sayfasında, Skype Kurumsal Online Plan 1 aboneliğinin durumu "[date]" tarihinde otomatik yenileme"den "[date] tarihinde süresi dolmaktadır" olarak değiştirildi.  

Müşterilerin sürekliliğini sağlamak için süresi dolan Skype Kurumsal Online Plan 1 aboneliklerini aşağıda listelenen desteklenen bir SKU seçeneğine geçişlisiniz. Müşteriler için hizmet kesintilerini önlemek için müşterilerin aboneliğin yıllık bitiş tarihine kadar yeni aboneliklere taşınmalarını öneririz. 

>[!NOTE]
>Hem Skype Kurumsal Plan 1 ticari hem de kamu SKUS'ları kullanımdan kaldırıldı.

API'yi (Ticari REST (CREST) veya İş Ortağı Merkezi kullanıyorsanız, aboneliğin bitiş tarihini ve otomatik yenileme = False özelliğini değerlendirerek süresi dolan abonelikleri bulun. Skype Kurumsal Online Plan 1 abonelikleri, 1 Eylül 2018'de otomatik olarak yenilenecek=False olarak ayarlanır. Müşterileri yeni bir plana her zaman taşımanız gerekir. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Skype Kurumsal Çevrimiçi Plan 1 değiştirme planları

Yeni planlar ile müşterileriniz, yeni özelliklerden ve işlevlerden faydalanarak Office 365. Fiyatlandırma ayrıntıları, fiyat listesinde ve teklif listesi matrisinde İş Ortağı Merkezi. 

- 1. Seçenek: Office 365 Kurumsal F1
- 2. Seçenek: Microsoft 365 Kurumsal F1
- 3. Seçenek: Diğer Office 365 planları

|**Özellik**    |**1\. Seçenek**   |**2\. Seçenek**   |**3\. Seçenek**   |
|:-----------------|:-----------------|:-------------|:------------|
|Skype Kurumsal Online Plan 1'de yer alan tüm özellikleri alın|Yes   |Yes   |Yes   |
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

Müşterinizin artık hem eski hem de yeni abonelikleri, eski Skype Kurumsal Online Plan 1 aboneliği ve yeni 'hedef' aboneliği (örneğin, Seçenek 1 - Office 365 Kurumsal F1) olması gerekir.

3. Müşterinin kullanıcı lisanslarını yeniden atamak için, **İş Ortağı Merkezi** menüsünden Müşteriler'i, hareket halindeki müşteriyi ve ardından Kullanıcılar ve lisanslar'ı **seçin.** Müşterinin Kullanıcılar ve Lisanslar sayfası açılır.

4. Kullanıcı lisansını yeniden atamak için, yeniden ataması yapılan kullanıcıyı seçin ve ardından Lisansları **yönet'i seçin.**

5. Lisansları **yönet sayfasında,** Skype Kurumsal Online Plan 1 lisansı onay kutusunun işaretini kaldırın ve müşterinin taşınıyor olduğu abonelik için yeni bir hizmet planı seçin.

6. **Gönder**’i seçin. Onay sayfasında yeni lisans atamaları listelemektedir. Lisans ataması gereken diğer kullanıcılar için de aynı işlemi devam eder.

Kullanıcı lisansını yeni hizmete taşımanın ardından kullanımdan kaldıran aboneliği müşteri düzeyinde güvenli bir şekilde iptal edebilirsiniz.

7. Veri **İş Ortağı Merkezi** Müşteriler'i **seçin.** Aboneliğini iptal etmek istediğiniz müşteriyi seçin.

8. Abonelik ayrıntıları sayfasında aboneliği Askıya Alındı olarak **ayarlayın.**

9. **Gönder'i seçin.**

Eski abonelik askıya alınır ve yeni abonelik etkindir. Askıya alınan abonelik 120 gün sonra otomatik olarak sağlanacak. Müşteri, eski abonelik için ek ücret ödemez.

## <a name="next-steps"></a>Sonraki adımlar

- [Danışmanlar: İstemcilerin denemesi için deneme daveti oluşturun ve Office 365](advisors-create-a-trial-invitation.md)
- [Danışmanlar: Office 365 deneme davetleri ve satın alma teklifleriyle müşteri tabanınızı oluşturun](advisors-build-your-business.md)
- [Danışmanlar: Satın alma teklifi oluşturma](advisor-create-a-purchase-offer.md)
