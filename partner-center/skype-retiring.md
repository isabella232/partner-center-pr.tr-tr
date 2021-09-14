---
title: Skype Kurumsal abonelikleri geçirme
description: yeni Office 365 sürümlerine süresi dolan Skype Kurumsal çevrimiçi Plan 1 abonelikleriyle belirli müşterileri nasıl ve ne zaman geçirebileceğinizi öğrenin.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: 58908e966eb80d219afa0cbc8c043932f5aef1a1
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248577"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Skype Kurumsal Çevrimiçi Plan 1 aboneliklerini yeni Office 365 sürümlerine geçirme

**Uygun roller**: satış Aracısı

Skype Kurumsal çevrimiçi Plan 1, 1 ağustos 2018 tarihinden itibaren kullanımdan kaldırılacaktır. bu tarihten sonra müşteriler artık yeni Skype Kurumsal Plan 1 abonelikleri satın almayabilir ve mevcut abonelikler, süreleri dolduğunda otomatik olarak yenilenmez ve bir yenileme seçeneği sağlamacaktır. aboneliğin ayrıntı sayfasında, Skype Kurumsal çevrimiçi Plan 1 abonelik durumu "otomatik yenilemede [tarih]" içinde "süre sonu" olarak değiştirildi.  

müşterilerin devamlılığını sağlamak için, süresi dolan Skype Kurumsal çevrimiçi Plan 1 abonelikleriyle müşterileri aşağıda listelenen desteklenen bir SKU seçeneğine geçirmeniz gerekir. Müşterilerin hizmet kesintilerinden kaçınmak için, aboneliğin yıllık bitiş tarihinden önce müşterileri yeni aboneliklere taşımayı öneririz. 

>[!NOTE]
>Skype Kurumsal çevrimiçi Plan 1 ticari ve kamu sku 'ları devre dışı bırakıldı.

API 'YI (Commerce REST (CREST) veya Iş Ortağı Merkezi) kullanıyorsanız, Otomatik Yenile = false özelliğiyle birlikte Aboneliğin bitiş tarihini değerlendirerek süresi dolan abonelikleri bulun. Skype Kurumsal çevrimiçi Plan 1 abonelikleri, 1 eylül 2018 ' de otomatik olarak yenile = False olarak ayarlanacak. Müşterileri dilediğiniz zaman yeni bir plana taşıyabilirsiniz. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Skype Kurumsal Çevrimiçi plan 1 değiştirme planları

Yeni planlarla, müşterileriniz Office 365 yeni özelliklerden ve işlevlerden faydalanabilir. Fiyatlandırma ayrıntıları, Iş Ortağı Merkezi 'nde fiyat listesi ve teklif listesi matrisinde bulunur. 

- seçenek 1: F1 Office 365 Kurumsal
- seçenek 2: F1 Microsoft 365 Kurumsal
- seçenek 3: diğer Office 365 planları

|**Özellik**    |**1\. Seçenek**   |**2\. Seçenek**   |**3\. Seçenek**   |
|:-----------------|:-----------------|:-------------|:------------|
|Skype Kurumsal çevrimiçi Plan 1 ' de bulunan tüm özellikleri alın|Yes   |Yes   |Yes   |
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

müşterinizin artık hem eski hem de yeni abonelikleri, eski Skype Kurumsal çevrimiçi Plan 1 aboneliği ve yeni ' target ' aboneliği olması gerekir, örneğin, seçenek 1-Office 365 Kurumsal F1.

3. Müşterinin kullanıcılarının lisanslarını yeniden atamak için **Iş Ortağı Merkezi** menüsünden **müşteriler**' i seçin, taşıdığınız müşteriyi seçin ve ardından **Kullanıcılar ve lisanslar**' ı seçin. Müşterinin kullanıcılar ve lisanslar sayfası açılır.

4. Kullanıcı lisansını yeniden atamak için, yeniden atanacak kullanıcıyı seçin ve ardından **Lisansları Yönet** ' i seçin.

5. **lisansları yönet** sayfasında, Skype Kurumsal çevrimiçi Plan 1 lisansı onay kutusunu temizleyin ve müşterinin taşınmakta olduğu abonelik için yeni bir hizmet planı seçin.

6. **Gönder**’i seçin. Bir onay sayfası yeni lisans atamalarını listeler. Lisans atamaları gerektiren diğer kullanıcılar için aynı işleme devam edin.

Kullanıcı lisansını yeni hizmete taşıdıktan sonra, kullanımdan kaldırılan aboneliği müşteri düzeyinde güvenle iptal edebilirsiniz.

7. **Iş Ortağı Merkezi** menüsünde **müşteriler**' i seçin. Aboneliğini iptal ettiğiniz müşteriyi seçin.

8. Abonelik Ayrıntıları sayfasında, aboneliği **askıya alındı** olarak ayarlayın.

9. Gönder ' i seçin **.**

Eski abonelik askıya alındı ve yeni abonelik etkin. Askıya alınan abonelik 120 gün sonra otomatik olarak sağlanacaktır. Müşteri, eski abonelik için ek maliyet içermez.

## <a name="next-steps"></a>Sonraki adımlar

- [Danışmanları: Office 365 denemek için istemciler için deneme davetiyesi oluşturun ve gönderin](advisors-create-a-trial-invitation.md)
- [Danışmanlar: Office 365 deneme davetleri ve satın alma teklifleriyle müşteri tabanınızı oluşturun](advisors-build-your-business.md)
- [Danışmanları: satın alma teklifi oluşturma](advisor-create-a-purchase-offer.md)
