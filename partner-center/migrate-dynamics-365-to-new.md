---
title: Dynamics 365 Business Edition'ı geçirme
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Tam Dynamics 365 Business Edition tekliflerini süresi dolmadan önce daha yeni sürümlere geçirmeyi öğrenin.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 40be8c8a338f5bbcbc8a10ccd9343f7ef52817902cdf7a5a54e8631a2d2c8b4b
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115681544"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Dynamics 365 Business Edition Tekliflerini daha yeni sürümlere geçirme

**Uygun roller:** Genel yönetici | Kullanıcı yönetimi yönetici | Yönetici aracısı | Satış aracısı

Dynamics 365 Business Edition abonelikleri olan müşteriler 1 Ocak 2019'dan itibaren bu eski tekliflere yenilenmeyecektir; mevcut aboneliklerin süresi dolduğunda otomatik olarak yenilenmez. Aboneliğin ayrıntı sayfasında abonelik durumu "[date]" ile "[date] üzerinde otomatik yenileme" olarak değişir.

Müşterilerin sürekliliğini sağlamak için, süresi dolan abonelikleri aşağıda listelenen desteklenen bir seçen geçişlisiniz. Müşteriler için hizmet kesintilerini önlemek için müşterilerin aboneliğin yıllık bitiş tarihine kadar yeni aboneliklere taşınmalarını öneririz.

API'yi (CREST veya İş Ortağı Merkezi) kullanıyorsanız, aboneliğin bitiş tarihini ve otomatik yenileme = False özelliğini değerlendirerek süresi dolan abonelikleri bulabilirsiniz. Söz konusu abonelikler 1 Ocak 2019'da otomatik olarak yenilenecek=False olarak ayarlanır. Müşterileri yeni bir plana her zaman taşımanız gerekir. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>Dynamics 365 Business Sürümleri kaldırıyor

- Dynamics 365 for Finance and Operations, Business edition
- Dynamics 365 for Team Members, Business sürümü

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central - Dynamics 365 Business Edition yeni teklifleri

Yeni Dynamics Business Central teklifleri ile müşterileriniz iş süreçlerini kolaylaştırma, müşteri etkileşimlerini geliştirme ve daha iyi kararlar alma için finansal, satış, hizmet ve operasyonlarını birbirine bağ hale getirmek için bu teklifleri karşılar. Dynamics 365 Business Central bulut tabanlıdır ve yalnızca Bulut Çözümü Sağlayıcısı (CSP) programı iş ortakları aracılığıyla kullanılabilir.
Dynamics 365 Business Edition müşterileri, 30 Haziran 2020'ye kadar yeni Business Central teklifleri için indirimli geçiş fiyatlandırması almaya hak kazanmaktadır.

## <a name="transition-customers-to-new-product-plans"></a>Müşterileri yeni ürün planlarına geçiş

 Müşterilerin eski SKUS'lardan yeni SKUS'lara taşınmaları için bu sırayla aşağıdaki adımlar gerekir:

- Yeni aboneliği satın alma
- Geçerli kullanıcı lisanslarını yeniden atama
- Eski aboneliği iptal etme

## <a name="purchase-the-new-plan-for-your-customer"></a>Müşteriniz için yeni planı satın alma

1. Sol **gezinti** çubuğundan Müşteriler'i ve ardından yeni aboneliğe taşımak istediğiniz müşteriyi seçin.
2. Abonelik **Ekle'yi seçin.**
3. Katalogdan satın almak istediğiniz aboneliği seçin (bu durumda, yukarıdaki seçeneklerden biri), lisans sayısını girin ve gönder'i **seçin.** 

Müşteriniz artık hem eski aboneliğe hem de yeni aboneliğe sahip olur. Bir sonraki adımınız, lisansları müşterinin kullanıcılarına yeniden atamanızdır.

1. Sol **gezinti** çubuğundan Müşteriler'i ve ardından hareket halindeki müşteriyi seçin.
2. Kullanıcılar **ve lisanslar'ı seçin.**
3. Bir kullanıcıya bir lisansı yeniden atamak için, kullanıcıyı seçin ve ardından Lisansları **yönet'i seçin.** 
4. Lisansları **yönet sayfasında** Temel (Nitelikli Teklif) lisansından Dynamics 365 for Sales/ Customer Engagement Planı'nın onay kutusunu temizleyin ve müşterinin taşınıyor olduğu abonelik için yeni bir hizmet planı seçin. 
5. **Gönder**’i seçin. Bunu yeni lisansa ihtiyacı olan her kullanıcı için yapacaktır. 

Lisansları yeni aboneliğe taşıdıktan sonra eski aboneliği iptal edebilirsiniz. 

1. Sol **gezinti** çubuğundan Müşteriler'i ve ardından hareket halindeki müşteriyi seçin.
2. Abonelik ayrıntıları sayfasında eski aboneliği Askıya Alındı olarak ayarlayın ve **Gönder'i** **seçin.**

Eski abonelik artık askıya alınır ve yeni abonelik etkindir. Askıya alınan abonelik 120 gün sonra otomatik olarak sağlanacak. Müşteriniz eski abonelik için ek ücret ödemez.
