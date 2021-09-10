---
title: E4 Office 365 geçirme
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Microsoft Office 365 Enterprise E4 sürümü 7 Nisan 2017'den itibaren kaldırıldı. Müşteri aboneliklerinizi daha yeni sürümlere geçirmeyi Office 365.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a1b47860f0af3427342d89945528e9118ecfc0aa
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961485"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Office 365 E4 aboneliklerini yeni Office 365 sürümlerine geçirme

**Uygun roller:** Genel yönetici | Kullanıcı yönetimi yönetici | Yönetici aracısı | Satış aracısı

Bu Office 365 Kurumsal E4 planı, 7 Nisan 2017'den itibaren geçerli olacak şekilde kaldırıldı. Bu tarihten sonra yeni E4 Office 365 satın alınamazsınız ve mevcut E4 abonelikleri süresi dolduğunda otomatik olarak yenilenmez.

E4 abonelikleri sona erer ve iptal edilir. Müşterilerin sürekliliğini sağlamak için, süresi dolan E4 abonelikleri olan müşterileri aşağıda listelenen desteklenen bir SKU seçeneğine geçişlisiniz. Müşteriler için hizmet kesintilerini önlemek için müşterileri aboneliğin yıllık bitiş tarihi öncesinde yeni aboneliklere taşımanız önerilir. 

> [!NOTE]  
> Hem Office 365 Kurumsal E4 kamu SKUS'ları kullanımdan kaldırıldı.
 
Aboneliğin ayrıntı sayfasındaki "[date]" ile E4 aboneliğinin durumu "[date] üzerinde otomatik yenileme" ile "[date]" olarak değiştirilmiştir. 

API'yi (CREST veya İş Ortağı Merkezi) kullanıyorsanız, aboneliğin bitiş tarihini ve otomatik yenileme = False özelliğini değerlendirerek süresi dolan abonelikleri keşfedebilirsiniz. 

E4 abonelikleri 7 Nisan 2017'de otomatik yenileme=False olarak ayarlanacak. Müşterileri yeni bir plana her zaman taşımanız gerekir. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Office 365 Kurumsal E4 sürümü değiştirme planları

E4 ile aynı işlevselliği sürdürmeyi veya müşterilerinize Office 365 ve Skype Kurumsal Online'daki yeni özelliklerden ve işlevlerden yararlanmayı seçebilirsiniz. Fiyatlandırma ayrıntıları, fiyat listesinde ve teklif listesi matrisinde İş Ortağı Merkezi. Güvenli Ürün Enterprise E3 veya Secure Productive Enterprise E5 sırasıyla E3 veya Office 365 Kurumsal E5 için Office 365 Kurumsal kullanılabilir.

- 1. Seçenek: Office 365 Kurumsal E5

- 2. Seçenek: Office 365 Kurumsal E3 + Skype Kurumsal Cloud PBX

- 3. Seçenek: Office 365 Kurumsal E3 + Skype Kurumsal Plus CAL (E4 ile fiyat ve işlevsellik eşlik)

- 4. Seçenek: Office 365 Kurumsal E3


| Özellik | 1\. Seçenek | 2\. Seçenek | 3\. Seçenek | 4\. Seçenek |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Bu pakete dahil olan tüm özellikleri Office 365 Kurumsal E4? | Yes | Yes | Yes | Hayır |
| Telefon yönetilen sayılar Office 365? | Yes | Yes | Hayır | Hayır |
| Telefon (karma dağıtım) hem şirket içinde hem de Office 365 yönetilen sayılar var mı? | Yes | Yes | Hayır | Hayır |
| PSTN sesli arama planı ekleme seçeneği var mı? | Yes | Yes | Hayır | Hayır |
| PSTN Konferans? | Yes | Hayır | Hayır | Hayır |
| İşbirliği, analiz ve güvenlik için gelişmiş araçlar? | Yes | Hayır | Hayır | Hayır |
| Etkileşimli raporlar, panolar ve veri görselleştirmeleri? | Yes | Hayır | Hayır | Hayır | 
| Yerleşik gizlilik, saydamlık ve iyileştirilmiş kullanıcı denetimleriyle veri güvenliği ve uyumluluğu üzerinde daha fazla denetime sahip misiniz? | Yes | Hayır | Hayır | Hayır | 

## <a name="transition-customers-to-new-product-plans"></a>Müşterileri yeni ürün planlarına geçiş

Microsoft, iş ortaklarımıza sürekli olarak yeni ürün ve hizmetler sunmaktadır. Bu gibi durumlarda, müşterileri yeni hizmetlere yükseltmeniz veya aboneliklerini sonunda kapatılacak olan SKUS'lardan geçirmeniz gerekir. Müşterileri, eski SKÜ'lerden yeni SKUS'lara şu adımların atılması gerekir:

-   Yeni aboneliği satın alma
-   Geçerli kullanıcı lisanslarını yeniden atama
-   Eski aboneliği iptal etme

Müşterinin abonelik aboneliğini yukarıdaki tabloda Office 365 Kurumsal E4 seçeneklerine geçirmek için bu adımları izleyin.

### <a name="step-1---purchase-the-new-subscription"></a>1. Adım - Yeni aboneliği satın alma

1. İş Ortağı Merkezi **menüsünden** **Müşteriler'i** seçin, taşımak istediğiniz müşteriyi seçin ve ardından Abonelik **ekle'yi seçin.**

2. Katalogdan satın almak istediğiniz aboneliği seçin (bu durumda, yukarıdaki seçeneklerden biri), lisans sayısını girin ve gönder'i **seçin.**

   Müşterinizin artık hem eski hem de yeni abonelikleri, eski Office 365 Kurumsal E4 aboneliği ve yeni 'hedef' aboneliğine sahip olması gerekir. Örneğin, Seçenek 1 - Office 365 Kurumsal E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>2. Adım: Müşterinin kullanıcı lisanslarını yeniden atama

1. Uygulama **İş Ortağı Merkezi** Müşteriler'i seçin, taşımak istediğiniz müşteriyi ve ardından Kullanıcılar ve **lisanslar'ı seçin.** Müşterinin Kullanıcılar ve Lisanslar sayfası açılır.

2. Kullanıcı lisanslarını yeniden atamak için, yeniden ataması yapılan kullanıcıyı seçin ve ardından Lisansları **yönet'i seçin.**

3. Lisansları **yönet sayfasında** lisans  Office 365 Kurumsal E4 kutusunun işaretini kaldırın ve müşterinin taşınarak aboneliğe yeni bir hizmet planı seçin.

4. **Gönder**’i seçin. Onay sayfasında yeni lisans atamaları listelemektedir.

5. Lisans yeniden ataması gereken diğer tüm müşteri kullanıcılarının adımlarına devam edin.

Kullanıcı lisanslarını yeni hizmete taşımanın ardından, kullanımdan kaldıran aboneliği en üst Müşteri düzeyinde güvenli bir şekilde iptal edebilirsiniz.

### <a name="step-3---cancel-the-old-subscription"></a>3. Adım - Eski aboneliği iptal etme

1. Veri **İş Ortağı Merkezi** Müşteriler'i **seçin.** Taşımak istediğiniz müşteriyi seçin ve iptal etmek istediğiniz aboneliği seçin.

2. Abonelik ayrıntıları sayfasında abonelik durumunu Askıya Alındı olarak **ayarlayın.**

3. **Gönder**’i seçin.

Eski abonelik askıya alınır ve yeni abonelik etkindir. Askıya alınan abonelik, 120 gün sonra otomatik olarak sağlanacak. Müşteri, eski abonelik için ek ücret ödemez.



 



