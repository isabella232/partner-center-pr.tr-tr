---
title: Office 365 E4 aboneliklerini geçirme
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 Enterprise E4 Edition 7 Nisan 2017 tarihinden itibaren kullanımdan kaldırıldı. Müşteri aboneliklerinizi Office 365 ' in daha yeni sürümlerine geçirmeyi öğrenin.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bbd2aceac62a7e726ed81a78305ea23213c94156
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/03/2020
ms.locfileid: "92530946"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Office 365 E4 aboneliklerini yeni Office 365 sürümlerine geçirme

**Uygulama hedefi**

-  İş Ortağı Merkezi

**Uygun roller**
-   Genel yönetici
-   Kullanıcı yöneticisi
-   Yönetim Aracısı
-   Satış Aracısı

Office 365 Enterprise E4 planı kullanımdan kalkmışsa, 7 Nisan 2017 ' de geçerli değildir. Bu tarihten sonra yeni Office 365 E4 abonelikleri satın alınmaz ve var olan E4 abonelikleri süreleri dolduğunda otomatik olarak yenilenmeyecektir.

E4 abonelikleri sona erdirmek için iptal edilir. Müşterilerin devamlılığını sağlamak için, süresi dolan E4 abonelikleriyle müşterileri aşağıda listelenen desteklenen bir SKU seçeneğine geçirmeniz gerekir. Müşterilerin hizmet kesintilerinden kaçınmak için, aboneliğin yıllık bitiş tarihinden önce müşterileri yeni aboneliklere taşımayı öneririz. 

> [!NOTE]  
> Hem Office 365 Enterprise E4 ticari hem de kamu SKU 'Ları devre dışı bırakıldı.
 
Aboneliğin ayrıntı sayfasında, E4 abonelik durumu "otomatik yenilemede [Tarih]" içinde "süre sonu" olarak değiştirildi. 

API 'YI (CREST veya Partner Center) kullanıyorsanız, Otomatik Yenile = false özelliğiyle birlikte Aboneliğin bitiş tarihini değerlendirerek süresi dolan abonelikleri bulabilirsiniz. 

E4 abonelikleri, 7 Nisan 2017 ' de Otomatik Yenile = false olarak ayarlanacak. Müşterileri dilediğiniz zaman yeni bir plana taşıyabilirsiniz. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Office 365 Enterprise E4 Edition değiştirme planları

E4 ile aynı işlevselliği korumayı seçebilirsiniz veya müşterilerinizin Office 365 ve Skype Kurumsal Çevrimiçi sürüm 'deki yeni özellik ve işlevlerden faydalanmasını sağlayabilirsiniz. Fiyatlandırma ayrıntıları, Iş Ortağı Merkezi 'nde fiyat listesi ve teklif listesi matrisinde bulunur. Güvenli ürün Kurumsal E3 veya güvenli üretkenlik Kurumsal E5, sırasıyla Office 365 Enterprise E3 veya Office 365 Kurumsal E5 için aşağıdaki seçenekler yerine kullanılabilir.

- Seçenek 1: Office 365 Kurumsal E5

- Seçenek 2: Office 365 Enterprise E3 + Skype Kurumsal Bulut PBX

- Seçenek 3: Office 365 Enterprise E3 + Skype Kurumsal Plus CAL (E4 ile fiyat ve işlev eşliği)

- 4. seçenek: Office 365 Kurumsal E3


| Özellik | 1\. Seçenek | 2\. Seçenek | Seçenek 3 | 4 seçeneği |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Office 365 Kurumsal E4 'ye dahil olan tüm özellikler mi alınır? | Evet | Evet | Evet | Hayır |
| Office 365 ' de yönetilen telefon numaraları? | Evet | Evet | Hayır | Hayır |
| Telefon numaraları hem şirket içinde hem de Office 365 ' de (karma dağıtım) yönetiliyor mu? | Evet | Evet | Hayır | Hayır |
| PSTN sesli arama planı ekleme seçeneği | Evet | Evet | Hayır | Hayır |
| PSTN Konferansı? | Evet | Hayır | Hayır | Hayır |
| İşbirliği, analiz ve güvenlik için gelişmiş araçlar? | Evet | Hayır | Hayır | Hayır |
| Etkileşimli raporlar, panolar ve veri görselleştirmeleri? | Evet | Hayır | Hayır | Hayır | 
| Yerleşik gizlilik, saydamlık ve iyileştirilmiş Kullanıcı denetimleriyle veri güvenliği ve uyumluluk üzerinde daha fazla denetim var mı? | Evet | Hayır | Hayır | Hayır | 

## <a name="transition-customers-to-new-product-plans"></a>Müşterilerin yeni ürün planlarına geçişini sağlar

Microsoft, iş ortaklarımız için sürekli olarak yeni ürün ve hizmetler sunar. Bu gibi durumlarda, müşterileri yeni hizmetlere yükseltmeniz veya sonunda kapatılacak SKU 'lardan aboneliklerini geçirmeniz gerekebilir. Müşterilerin Kullanımdan kaldırılmış SKU 'lardan daha yeni bir sürümüne geçirilmesi aşağıdaki adımları gerektirir:

-   Yeni aboneliği satın alın
-   Geçerli kullanıcı lisanslarını yeniden ata
-   Eski aboneliği iptal et

Müşterinin Office 365 Kurumsal E4 aboneliğini Yukarıdaki tablodaki seçeneklerden birine geçirmek için aşağıdaki adımları izleyin.

### <a name="step-1---purchase-the-new-subscription"></a>1. adım-yeni aboneliği satın alma

1. **Iş Ortağı Merkezi** menüsünden **müşteriler** ' i seçin, taşımak istediğiniz müşteriyi seçin ve ardından **Abonelik Ekle** ' yi seçin.

2. Katalogdan satın almak istediğiniz aboneliği seçin (Bu durumda yukarıdaki seçeneklerden biri), lisansların sayısını girin ve ardından **Gönder** ' i seçin.

   Müşterinizin artık eski ve yeni abonelikleri, eski Office 365 Enterprise E4 aboneliği ve yeni ' Target ' aboneliği olmalıdır; örneğin, 1-Office 365 Enterprise E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>2. adım-müşterinin kullanıcılarının lisanslarını yeniden atama

1. **Iş Ortağı Merkezi** menüsünden **müşteriler** ' i seçin, taşımak istediğiniz müşteriyi seçin ve ardından **Kullanıcılar ve lisanslar** ' ı seçin. Müşterinin kullanıcılar ve lisanslar sayfası açılır.

2. Kullanıcı lisanslarını yeniden atamak için, yeniden atanacak kullanıcıyı seçin ve ardından **Lisansları Yönet** ' i seçin.

3. **Lisansları Yönet** sayfasında, **Office 365 Kurumsal E4** Lisansı onay kutusunu temizleyin ve müşterinin taşınmakta olduğu abonelik için yeni bir hizmet planı seçin.

4. **Gönder** ’i seçin. Bir onay sayfası yeni lisans atamalarını listeler.

5. Lisans yeniden ataması gerektiren diğer müşteri kullanıcılarıyla aynı adımlara devam edin.

Kullanıcı lisanslarını yeni hizmete taşıdıktan sonra, kullanımdan kaldırılan aboneliği en üst müşteri düzeyinde güvenle iptal edebilirsiniz.

### <a name="step-3---cancel-the-old-subscription"></a>3. adım-eski aboneliği Iptal et

1. **Iş Ortağı Merkezi** menüsünde **müşteriler** ' i seçin. Taşımak istediğiniz müşteriyi seçin ve iptal etmek istediğiniz aboneliği seçin.

2. Abonelik Ayrıntıları sayfasında, abonelik durumunu **askıya alındı** olarak ayarlayın.

3. **Gönder** ’i seçin.

Eski abonelik askıya alındı ve yeni abonelik etkin. Askıya alınan abonelik 120 gün sonra otomatik olarak sağlanacaktır. Müşteri, eski abonelik için ek maliyet içermez.



 



