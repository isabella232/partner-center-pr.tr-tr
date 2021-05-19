---
title: Nitelikli Dynamics 365 aboneliklerini geçirme
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Mevcut aboneliklerin süre dolmadan önce nitelikli, temel Dynamics 365 aboneliklerinden yeni bir aboneliğe nasıl geçiş yapılacağını öğrenin.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5ba6992eff64031aed0dafeb5a5010983396ab63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151653"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Dynamics 365 ve Müşteri Etkileşimi Planı’nı Temel’den (uygun teklifler) daha yeni sürümlere geçirme

**Uygun roller**: genel yönetici | Kullanıcı Yönetimi Yöneticisi | Yönetici Aracısı | Satış Aracısı

1 Ocak 2019 ' den itibaren, temel (nitelikli teklifler) aboneliklerden satış/müşteri katılım planı için Dynamics 365 olan müşteriler bu eski teklifleri artık yenilemez; mevcut abonelikler, süreleri dolduğunda otomatik olarak yenilenmeyecektir. Aboneliğin ayrıntı sayfasında, abonelik durumu "otomatik yenilemede [Tarih]" içinden "süresi doluyor" olarak değişir. 

Müşterilerin devamlılığını sağlamak için, süresi dolan aboneliklerle birlikte aşağıda listelenen desteklenen bir seçeneğe geçiş yapmanız gerekir. Müşterilerin hizmet kesintilerinden kaçınmak için, aboneliğin yıllık bitiş tarihinden önce müşterileri yeni aboneliklere taşımayı öneririz.

API 'YI (CREST veya Partner Center) kullanıyorsanız, Otomatik Yenile = false özelliğiyle birlikte Aboneliğin bitiş tarihini değerlendirerek süresi dolan abonelikleri bulabilirsiniz. Söz konusu abonelikler, 1 Ocak 2019 tarihinde otomatik olarak Yenile = false olarak ayarlanacak. Müşterileri dilediğiniz zaman yeni bir plana taşıyabilirsiniz. 

### <a name="the-dynamics-365-offers-being-retired"></a>Dynamics 365, kullanımdan kalkmakta olan teklifleri

- Sales Enterprise Edition CRMOL Basic (nitelikli teklif) için Dynamics 365
- Fakülteler için Dynamics 365 for Sales Enterprise Edition CRMOL Basic (nitelikli teklif)
- Öğrenciler için Dynamics 365 for Sales Enterprise Edition CRMOL Basic (nitelikli teklif)
- Sales Enterprise Edition için Dynamics 365 (kamu fiyatlandırması) CRMOL temel (nitelikli teklif)
- CRM Basic için SA 'Dan Sales Enterprise Edition için Dynamics 365 (nitelikli teklif)
- Dynamics 365 for Sales Enterprise Edition for CRM Basic (uygun teklif) için ŞA
- Öğrenciler için Dynamics 365 for Sales Enterprise Edition for CRM Basic (nitelikli teklif)
- Dynamics 365 for Sales Enterprise Edition (kamu fiyatlandırması) için SA 'Dan CRM temel (nitelikli teklif)
- CRM Basic için Dynamics 365 for Sales Enterprise Sürümü Add-On (Nitelikli Teklif)
- Fakülteler için DYNAMICS 365 for Sales Enterprise Sürümü Add-On CRM Basic (Nitelikli Teklif)
- Dynamics 365 for Sales Enterprise Sürümü Add-On for CRM Basic (Öğrenciler için Nitelikli Teklif)
- Dynamics 365 for Sales Enterprise Sürümü (Kamu Fiyatlandırması) Add-On CRM Temel (Nitelikli Teklif)
- DYNAMICS 365 Müşteri Katılımı Planı Enterprise Sürümü CRMOL Basic (Nitelikli Teklif)
- Dynamics 365 Customer Engagement Plan Enterprise Sürümü (Kamu Fiyatlandırması) CRMOL Temel (Nitelikli Teklif)
- Dynamics 365 Müşteri Katılımı Planı Enterprise Sürümü CRMOL Basic (Nitelikli Teklif)
- Dynamics 365 Müşteri Katılımı Planı Enterprise Sürümü CRMOL Basic (Nitelikli Teklif)
- Dynamics 365 Customer Engagement Planı Enterprise Sürümü CRM Basic için SA'dan (Nitelikli Teklif)
- DYNAMICS 365 Customer Engagement Plan Enterprise Sürümü (Kamu Fiyatlandırması) FROM SA for CRM Basic (Nitelikli Teklif)
- Dynamics 365 Müşteri Katılımı Planı Enterprise Sürümü CRM Temel (Nitelikli Teklif) için SA'dan Eğitim
- Dynamics 365 Müşteri Katılımı Planı Enterprise Sürümü CRM Temel (Nitelikli Teklif) için SA'dan Öğretim Üyeleri
- DYNAMICS 365 Customer Engagement Plan Enterprise Sürümü Add-On for CRM Basic (Nitelikli Teklif)
- DYNAMICS 365 Customer Engagement Plan Enterprise Sürümü (Kamu Fiyatlandırması) Add-On CRM Temel (Nitelikli Teklif)
- Dynamics 365 Customer Engagement Plan Enterprise Sürümü Add-On for CRM Basic (Nitelikli Teklif)
- Dynamics 365 Customer Engagement Plan Enterprise Sürümü Add-On for CRM Basic (Nitelikli Teklif) for Faculty



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Temel (Nitelikli Teklifler) değiştirme planlarından Dynamics 365 for Sales/ Customer Engagement Planı

**Kaldıran teklifler**   

- CRM Basic veya CRMOL Basic'ten Dynamics 365 for Sales (Nitelikli Teklif)
- CRM Basic veya CRMOL Basic'ten Dynamics 365 Customer Engagement Planı (Nitelikli Teklif)

**Değiştirme seçenekleri**
- Sales Professional için Dynamics 365 (yenı)
- Sales Professional için Dynamics 365 (yenı)
- Dynamics 365 for Customer Service
- Dynamics 365 müşteri katılımı planı veya
- Dynamics 365 ekip üyeleri



## <a name="transition-customers-to-new-product-plans"></a>Müşterilerin yeni ürün planlarına geçişini sağlar

Müşterileri kullanımdan kaldırılan SKU 'lardan daha yeni bir sürümüne taşımak, bu sırayla aşağıdaki adımları gerektirir:

- Yeni aboneliği satın alın
- Geçerli kullanıcı lisanslarını yeniden ata
- Eski aboneliği iptal et

## <a name="purchase-the-new-plan-for-your-customer"></a>Müşteriniz için yeni planı satın alın

1. Sol gezinti bölmesinde **müşteriler** ' i seçin ve sonra yeni aboneliğe taşımak istediğiniz müşteriyi seçin.
2. **Abonelik Ekle**' yi seçin.
3. Katalogdan satın almak istediğiniz aboneliği seçin (Bu durumda yukarıdaki seçeneklerden biri), lisansların sayısını girin ve ardından **Gönder**' i seçin. 

Müşterinizin artık hem eski hem de yeni bir abonelik olacak. Bir sonraki adımınız, lisansları müşterinin kullanıcılarına yeniden atamak olur.

1. Sol gezinti çubuğunda **müşteriler** ' i seçin ve ardından taşıdığınız müşteriyi seçin.
2. **Kullanıcılar ve lisanslar ' ı** seçin.
3. Bir kullanıcıya bir lisansı yeniden atamak için kullanıcıyı seçin ve ardından **Lisansları Yönet**' i seçin. 
4. **Lisansları Yönet** sayfasında, temel (nitelikli teklif) lisanstan satış/müşteri katılım planı için Dynamics 365 ' i temizleyin ve müşterinin taşınmakta olduğu abonelik için yeni bir hizmet planı seçin. 
5. **Gönder**’i seçin. Bunu yeni lisansa ihtiyacı olan her kullanıcı için yapacaktır. 

Lisansları yeni aboneliğe taşıdıktan sonra eski aboneliği iptal edebilirsiniz. 

1. Sol **gezinti** çubuğundan Müşteriler'i ve ardından hareket halindeki müşteriyi seçin.
2. Abonelik ayrıntıları sayfasında eski aboneliği Askıya Alındı olarak ayarlayın ve **Gönder'i** **seçin.**

Eski abonelik artık askıya alınır ve yeni abonelik etkindir. Askıya alınan abonelik, 120 gün sonra otomatik olarak sağlanacak. Müşteriniz eski abonelik için ek ücret ödemez.
 

 



