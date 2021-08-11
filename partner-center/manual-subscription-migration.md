---
title: Nitelikli Dynamics 365 aboneliklerini geçirme
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Mevcut aboneliklerin süre dolmadan önce nitelikli, temel Dynamics 365 aboneliklerinden yeni bir aboneliğe nasıl geçiş yapılacağını öğrenin.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 71c3af5cdb3cb35ff13a455748a93699df43a8b1615116ca7058df3c6a23b7b9
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115694668"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Dynamics 365 ve Müşteri Etkileşimi Planı’nı Temel’den (uygun teklifler) daha yeni sürümlere geçirme

**Uygun roller**: genel yönetici | Kullanıcı Yönetimi Yöneticisi | Yönetici Aracısı | Satış Aracısı

1 Ocak 2019 ' den itibaren, temel (nitelikli teklifler) aboneliklerden satış/müşteri katılım planı için Dynamics 365 olan müşteriler bu eski teklifleri artık yenilemez; mevcut abonelikler, süreleri dolduğunda otomatik olarak yenilenmeyecektir. Aboneliğin ayrıntı sayfasında, abonelik durumu "otomatik yenilemede [Tarih]" içinden "süresi doluyor" olarak değişir. 

Müşterilerin devamlılığını sağlamak için, süresi dolan aboneliklerle birlikte aşağıda listelenen desteklenen bir seçeneğe geçiş yapmanız gerekir. Müşterilerin hizmet kesintilerinden kaçınmak için, aboneliğin yıllık bitiş tarihinden önce müşterileri yeni aboneliklere taşımayı öneririz.

API 'YI (CREST veya Partner Center) kullanıyorsanız, Otomatik Yenile = false özelliğiyle birlikte Aboneliğin bitiş tarihini değerlendirerek süresi dolan abonelikleri bulabilirsiniz. Söz konusu abonelikler, 1 Ocak 2019 tarihinde otomatik olarak Yenile = false olarak ayarlanacak. Müşterileri dilediğiniz zaman yeni bir plana taşıyabilirsiniz. 

### <a name="the-dynamics-365-offers-being-retired"></a>Dynamics 365, kullanımdan kalkmakta olan teklifleri

- Sales Enterprise Sürümü CRMOL Basic (nitelikli teklif) için Dynamics 365
- fakülte Sales Enterprise Sürümü CRMOL Basic (nitelikli teklif) için Dynamics 365
- öğrenciler için Dynamics 365 for Sales Enterprise Sürümü CRMOL Basic (nitelikli teklif)
- Sales Enterprise Sürümü için Dynamics 365 (kamu fiyatlandırması) CRMOL temel (nitelikli teklif)
- CRM Basic için SA 'dan Sales Enterprise Sürümü için Dynamics 365 (nitelikli teklif)
- fakülteler için Dynamics Enterprise Sürümü 365 for CRM Basic (nitelikli teklif) için SA
- öğrenciler için Dynamics 365 for Enterprise Sürümü Sales for CRM Basic (nitelikli teklif)
- Dynamics 365 for Sales Enterprise Sürümü (kamu fiyatlandırması) için SA 'dan CRM temel (nitelikli teklif)
- Dynamics 365 for Sales Enterprise Sürümü for CRM Basic (nitelikli teklif) Add-On
- fakülteler için Dynamics 365 for Sales Enterprise Sürümü Add-On for CRM Basic (nitelikli teklif)
- öğrenciler için Dynamics 365 for Sales Enterprise Sürümü Add-On for CRM Basic (nitelikli teklif)
- Dynamics 365 for Sales Enterprise Sürümü (kamu fiyatlandırması) Add-On CRM Basic (nitelikli teklif) için
- Dynamics 365 müşteri katılımı planı Enterprise Sürümü CRMOL Basic (nitelikli teklif)
- Dynamics 365 müşteri katılımı planı Enterprise Sürümü (kamu fiyatlandırması) CRMOL temel (nitelikli teklif)
- öğrenciler için Dynamics 365 müşteri katılımı planı Enterprise Sürümü CRMOL Basic (nitelikli teklif)
- Dynamics 365 müşteri katılımı planı, fakülteler için CRMOL Basic (nitelikli teklif) Enterprise Sürümü
- Dynamics 365 müşteri katılımı planı Enterprise Sürümü için SA 'dan CRM temel (nitelikli teklif)
- Dynamics 365 müşteri katılımı planı Enterprise Sürümü (kamu fiyatlandırması) için SA 'dan CRM temel (nitelikli teklif)
- Dynamics 365 müşteri katılımı planı, öğrenciler için şa Enterprise Sürümü for CRM Basic (nitelikli teklif)
- Dynamics 365 müşteri katılımı planı, fakülteler için CRM Basic (nitelikli teklif) için SA 'dan Enterprise Sürümü
- Dynamics 365 müşteri katılımı planı Enterprise Sürümü Add-On for CRM Basic (nitelikli teklif)
- Dynamics 365 müşteri katılımı planı Enterprise Sürümü (kamu fiyatlandırması) Add-On CRM temel (nitelikli teklif) için
- Dynamics 365 müşteri katılımı planı, öğrenciler için CRM Basic (nitelikli teklif) için Add-On Enterprise Sürümü
- Dynamics 365 müşteri katılımı planı, fakülteler için CRM Basic (nitelikli teklif) için Add-On Enterprise Sürümü



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Temel (nitelikli teklifler) değiştirme planlarından satış/müşteri katılım planına yönelik Dynamics 365

**Kullanımdan kaldırılan teklifler**   

- CRM Basic veya CRMOL Basic 'ten (nitelikli teklif) satış için Dynamics 365
- Dynamics 365 müşteri katılımı planı CRM Basic veya CRMOL Basic (nitelikli teklif)

**Değiştirme seçenekleri**
- Sales Professional için Dynamics 365 (yeni)
- Sales Professional için Dynamics 365 (yeni)
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
5. **Gönder**’i seçin. Bunu, yeni lisansa ihtiyacı olan her kullanıcı için yapabilirsiniz. 

Lisansları yeni aboneliğe taşındıktan sonra eski aboneliği iptal edebilirsiniz. 

1. Sol gezinti çubuğunda **müşteriler** ' i seçin ve ardından taşıdığınız müşteriyi seçin.
2. Abonelik Ayrıntıları sayfasında, eski aboneliği **askıya alındı** olarak ayarlayın ve **Gönder**' i seçin.

Eski abonelik artık askıya alındı ve yeni abonelik etkin. Askıya alınan abonelik 120 gün sonra otomatik olarak sağlanacaktır. Müşterinizin eski abonelik için ek ücret ödemeyecektir.
 

 



