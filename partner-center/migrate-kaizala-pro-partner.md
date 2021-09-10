---
title: Kaizala Pro aboneliklerini Microsoft 365'e geçirme
description: Kaizala Pro aboneliklerini Microsoft 365 veya Office 365 öğrenin. Müşterilerinize geçiş hakkında daha fazla ayrıntı için bu makaleyi okuyun.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: e248657b9b4d4cf50cb7d38b2a0593ae6445bd28
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961415"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a>Tek Kaizala Pro abonelikleri Microsoft 365 veya Office 365 geçirme

**Uygun roller:** Satış aracısı

Microsoft, 1 Temmuz 2020'den itibaren tek başına Kaizala Pro satışlarını sonlandırdı. Müşteriler bu tarihten sonra yeni Kaizala Pro abonelikleri satın alamayacak ve Kaizala Pro süresi dolduğunda mevcut abonelikler otomatik olarak yenilenmeyecek.

Müşterilerin sürekliliğini sağlamak için, süresi dolan ve tek başına Kaizala Pro olan müşterileri aşağıda listelenen desteklenen bir SKU seçeneğine geçişlisiniz. Müşteriler için hizmet kesintilerini önlemek için müşterilerin aboneliğin yıllık bitiş tarihine kadar yeni aboneliklere taşınmalarını öneririz.

API'yi (CREST veya İş Ortağı Merkezi) kullanıyorsanız, aboneliğin bitiş tarihini ve otomatik yenileme özelliğini false olarak ayar kullanarak süresi dolan abonelikleri keşfedebilirsiniz: `auto renew = False` .

E4 abonelikleri 1 Temmuz `auto renew=False` 2020'de olarak ayarlanır. Müşterileri yeni bir plana her zaman taşımanız gerekir.

## <a name="kaizala-pro-standalone-replacement-plans"></a>Kaizala Pro Tek başına değiştirme planları

Yeni planlar ile müşterileriniz yeni özelliklerden ve işlevlerden faydalanarak yeni Microsoft 365. Fiyatlandırma ayrıntıları, fiyat listesinde ve teklif listesi matrisinde İş Ortağı Merkezi.

- [**Microsoft 365 için şu şekildedir:**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2)  
   - Microsoft 365 İş Temel
   - Microsoft 365 İş Standart
   - Microsoft 365 İş Ekstra
    
- [**Microsoft 365 için şu şekildedir:**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)
   - Microsoft 365 F3 (eski adı Microsoft 365 F1) ve Office 365 F3
    
- [**Microsoft 365 için Enterprise,**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans)örneğin: 
   - Office 365 E1
   - Microsoft 365 E3 ve Office 365 E3
   - Microsoft 365 E5 ve Office 365 E5

- [**Microsoft 365 eğitim için şu**](https://www.microsoft.com/education/buy-license/microsoft365)şekildedir: 
    - Microsoft 365 A1 ve Office 365 A1
    - Microsoft 365 A3 ve Office 365 A3
    - Microsoft 365 A5 ve Office 365 A5

## <a name="transition-customers-to-new-product-plans"></a>Müşterileri yeni ürün planlarına geçiş

Microsoft, iş ortaklarımıza sürekli olarak yeni ürün ve hizmetler sunmaktadır. Bu durumlarda, müşterileri yeni hizmetlere yükseltmeniz veya sonunda kapatılacak olan aboneliklerini SKUS'lardan geçirmeniz gerekir. Müşterileri, eski SKÜ'lerden yeni SKUS'lara şu adımların atılması gerekir:

A. Yeni aboneliği satın alma

B. Geçerli kullanıcı lisanslarını yeniden atama

C. Eski aboneliği iptal etme


## <a name="migrate-your-customers-to-new-plans"></a>Müşterilerinizi yeni planlara geçirme

### <a name="a-purchase-the-new-subscription"></a>A. Yeni aboneliği satın alma

1. Yeni aboneliği satın almak için, **İş Ortağı Merkezi** menüsünden Müşteriler'i **seçin,** taşımak istediğiniz müşteriyi seçin ve ardından Abonelik **ekle'yi seçin.**

2. Katalogdan satın almak istediğiniz aboneliği seçin (bu durumda, yukarıdaki seçeneklerden biri), lisans sayısını girin ve gönder'i **seçin.**

Müşterinizin artık hem eski hem de yeni abonelikleri, eski Kaizala Pro Tek Başına aboneliği ve yeni 'hedef' aboneliği (örneğin, Seçenek 1 - Office 365 Kurumsal F1) olması gerekir.

### <a name="b-reassign-current-user-licenses"></a>B. Geçerli kullanıcı lisanslarını yeniden atama

1. Müşterinin kullanıcı lisanslarını yeniden atamak için, **İş Ortağı Merkezi** menüsünden Müşteriler'i, hareket halindeki müşteriyi ve ardından Kullanıcılar ve lisanslar'ı **seçin.** Müşterinin Kullanıcılar ve Lisanslar sayfası açılır.

2. Kullanıcı lisansını yeniden atamak için, yeniden ataması yapılan kullanıcıyı seçin ve ardından Lisansları **yönet'i seçin.**

3. Lisansları **yönet sayfasında,** Kaizala Pro Tek Başına lisans onay kutusunu temizleyin ve müşterinin taşınarak aboneliğe yeni bir hizmet planı seçin.

4.  **Gönder**’i seçin. Onay sayfasında yeni lisans atamaları listelemektedir. Lisans ataması gereken diğer kullanıcılar için de aynı işlemi devam eder.

### <a name="c-cancel-old-subscription"></a>C. Eski aboneliği iptal etme

Kullanıcı lisansını yeni hizmete taşımanın ardından kullanımdan kaldıran aboneliği müşteri düzeyinde güvenli bir şekilde iptal edebilirsiniz.

1.  Veri **İş Ortağı Merkezi** Müşteriler'i **seçin.** Aboneliğini iptal etmek istediğiniz müşteriyi seçin.

2.  Abonelik ayrıntıları sayfasında aboneliği Askıya Alındı olarak **ayarlayın.**

3.  **Gönder**’i seçin.

Eski abonelik askıya alınır ve yeni abonelik etkindir. Askıya alınan abonelik, 120 gün sonra otomatik olarak sağlanacak. Müşteri, eski abonelik için ek ücret ödemez.
