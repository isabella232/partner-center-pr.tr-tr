---
title: Dynamics 365 Business Edition 'ı geçirme
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Uygun Dynamics 365 Business Edition tekliflerini, kullanım süreleri dolmadan önce daha yeni sürümlere geçirmeyi öğrenin.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d441d121c28c2762d1f1c71d6f6a1e81d089f99c
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/17/2020
ms.locfileid: "92531006"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Dynamics 365 Business Edition Tekliflerini daha yeni sürümlere geçirme

**Uygulama hedefi**

- İş Ortağı Merkezi

**Uygun roller**
- Genel yönetici
- Kullanıcı yöneticisi
- Yönetim Aracısı
- Satış Aracısı

1 Ocak 2019 ' den itibaren, Dynamics 365 Business Edition aboneliklerine sahip müşteriler artık bu eski tekliflere yenilemez; mevcut abonelikler, süreleri dolduğunda otomatik olarak yenilenmeyecektir. Aboneliğin ayrıntı sayfasında, abonelik durumu "otomatik yenilemede [Tarih]" içinden "süresi doluyor" olarak değişir.

Müşterilerin devamlılığını sağlamak için, süresi dolan aboneliklerle birlikte aşağıda listelenen desteklenen bir seçeneğe geçiş yapmanız gerekir. Müşterilerin hizmet kesintilerinden kaçınmak için, aboneliğin yıllık bitiş tarihinden önce müşterileri yeni aboneliklere taşımayı öneririz.

API 'YI (CREST veya Partner Center) kullanıyorsanız, Otomatik Yenile = false özelliğiyle birlikte Aboneliğin bitiş tarihini değerlendirerek süresi dolan abonelikleri bulabilirsiniz. Söz konusu abonelikler, 1 Ocak 2019 ' de otomatik yenileme = false olarak ayarlanacak. Müşterileri dilediğiniz zaman yeni bir plana taşıyabilirsiniz. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>Kullanımdan kalkmakta olan Dynamics 365 Iş sürümleri

- Finans ve Işlemler için Dynamics 365, Iş sürümü
- Ekip üyeleri için Dynamics 365, Iş sürümü

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central-Dynamics 365 Business Edition yeni teklifleri

Yeni Dynamics Business merkezi teklifleriyle, müşterileriniz, iş süreçlerini kolaylaştırmak, müşteri etkileşimlerini geliştirmek ve daha iyi kararlar almak için mali bilgilerini, satışları, servis ve işlemlerini birbirine bağlayabilirler. Dynamics 365 Business Central, bulut tabanlı ve yalnızca bulut çözümü sağlayıcısı (CSP) program iş ortakları aracılığıyla kullanılabilir.
Dynamics 365 Business Edition müşterileri, 30 Haziran 2020 ' e kadar yeni Iş Merkezi teklifleri için indirimli geçiş fiyatlandırması almaya uygundur.

## <a name="transition-customers-to-new-product-plans"></a>Müşterilerin yeni ürün planlarına geçişini sağlar

 Müşterileri kullanımdan kaldırılan SKU 'lardan daha yeni bir sürümüne taşımak, bu sırayla aşağıdaki adımları gerektirir:

- Yeni aboneliği satın alın
- Geçerli kullanıcı lisanslarını yeniden ata
- Eski aboneliği iptal et

## <a name="purchase-the-new-plan-for-your-customer"></a>Müşteriniz için yeni planı satın alın

1. Sol gezinti bölmesinde **müşteriler** ' i seçin ve sonra yeni aboneliğe taşımak istediğiniz müşteriyi seçin.
2. **Abonelik Ekle** ' yi seçin.
3. Katalogdan satın almak istediğiniz aboneliği seçin (Bu durumda yukarıdaki seçeneklerden biri), lisansların sayısını girin ve ardından **Gönder** ' i seçin. 

Müşterinizin artık hem eski hem de yeni bir abonelik olacak. Bir sonraki adımınız, lisansları müşterinin kullanıcılarına yeniden atamak olur.

1. Sol gezinti çubuğunda **müşteriler** ' i seçin ve ardından taşıdığınız müşteriyi seçin.
2. **Kullanıcılar ve lisanslar ' ı** seçin.
3. Bir kullanıcıya bir lisansı yeniden atamak için kullanıcıyı seçin ve ardından **Lisansları Yönet** ' i seçin. 
4. **Lisansları Yönet** sayfasında, temel (nitelikli teklif) lisanstan satış/müşteri katılım planı için Dynamics 365 ' i temizleyin ve müşterinin taşınmakta olduğu abonelik için yeni bir hizmet planı seçin. 
5. **Gönder** ’i seçin. Bunu, yeni lisansa ihtiyacı olan her kullanıcı için yapabilirsiniz. 

Lisansları yeni aboneliğe taşındıktan sonra eski aboneliği iptal edebilirsiniz. 

1. Sol gezinti çubuğunda **müşteriler** ' i seçin ve ardından taşıdığınız müşteriyi seçin.
2. Abonelik Ayrıntıları sayfasında, eski aboneliği **askıya alındı** olarak ayarlayın ve **Gönder** ' i seçin.

Eski abonelik artık askıya alındı ve yeni abonelik etkin. Askıya alınan abonelik 120 gün sonra otomatik olarak sağlanacaktır. Müşterinizin eski abonelik için ek ücret ödemeyecektir.
