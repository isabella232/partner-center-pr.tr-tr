---
title: İş Ortağı Merkezi Insights abonelikleri raporu
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: İyi işlerinizi ve müşterileriniz için satış veya yönetimle ilgili bulut aboneliklerini geliştirebilirsiniz.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cd226122f8e69e0667006f274d2ef080bbe47b9b
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565432"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>İş Ortağı Merkezi Insights panosundan kullanılabilen Ürün Abonelikleri raporu

**Uygun roller:** Genel yönetici | Yönetici aracısı | Rapor görüntüleyici | Yönetici raporu görüntüleyicisi

Ürün Abonelikleri raporu, müşterileriniz için sattığınız veya sizin yönettiğiniz bulut abonelikleri üzerinde analiz sunar. Bu rapor Office 365, Azure, Dynamics ve diğerleri gibi bulut ürünleriyle ilişkili aboneliklerin performansını içeren ürüne özgü bir rapordür.

Ürün Abonelikleri raporundan aşağıdaki bölümleri görüntüebilirsiniz.

- Özet
- Aboneliklerin coğrafi yayılması
- Abonelik ekleme/veri eğilimi
- İş ortağı konumlara, satış kanalına, STU'lara, iş ortağı ekleme türüne, segmente göre abonelik dağıtımı
- Abonelik eyaletlere göre eğilim
- Ürün eğilimi

 > [!NOTE]
 > Bu rapor, Öngörüler panosundan edinebilirsiniz. Bu raporu görüntülemek için genel yönetici, hesap İş Ortağı Merkezi, Rapor görüntüleyicisi veya Yönetici rapor görüntüleyicisi gibi belirli bir rol atanmış olması gerekir. Daha fazla bilgi için bkz. şirketin Genel yöneticisi. Bu rapora özgü veri türleri yalnızca Yönetici rapor görüntüleyici ayrıcalıklarına sahip kullanıcılar tarafından da kullanılabilir.

## <a name="summary"></a>Özet

Özet bölümü, müşterileriniz için sizin tarafından satılan veya yönetilen aboneliklerle ilgili ana performans göstergelerinin (KIP) anlık görüntü görünümünü sunar.  

:::image type="content" source="images/pci/pci-sub-report-summary-1.png" alt-text="abonelikler rapor özeti.":::

Özetin her bölümü hakkında daha fazla bilgi için aşağıya bakın:

- Abonelikler:
  - Sizin tarafından satılan veya yönetilen bulut ürünü aboneliklerinin geçerli sayısı.
  - Seçtiğiniz tarih aralığı boyunca aboneliklerin büyüme veya reddetme yüzdesi.
  - Mikro grafik, seçtiğiniz tarih aralığında aylık abonelik sayısı eğilimini gösterir.

- Etkin abonelikler:
  - Etkin kullanımın ürün telemetri verilerine göre ölçüleceği bulut ürünü aboneliklerinin geçerli sayısı. Bu, Azure abonelikleri için tüm deneme aboneliklerini dışlar.
  - Seçili zaman dönemi boyunca etkin aboneliklerin büyüme veya reddetme yüzdesi.
  - Mikro grafik, seçtiğiniz tarih aralığı boyunca etkin aboneliklerin aylık eğilimini gösterir.

- Abonelikler eklendi:
  - Seçilen tarih aralığı boyunca sizin tarafından eklenen (satılan veya yönetilen) toplam müşteri aboneliği sayısı. Etkin veya **Yenilendi** **durumuna sahip** yeni abonelikler, Eklenen Abonelikler olarak sayılır.
  - Son tam aya eklenen aboneliklerin ilk tam aya göre büyüme veya düşüş yüzdesi.
  - Mikro grafik, seçtiğiniz tarih aralığı boyunca eklenen aboneliklerin aylık eğilimini gösterir.

- Abonelikler şu şekildedir:
  - Seçtiğiniz tarih aralığı boyunca geçen toplam müşteri aboneliği sayısı. O ayki **Aboneliğin Aboneliği Kaldırıldı** veya **Askıya** Alındı durumuna sahip abonelikler, geçici abonelik olarak sayılır.  
  - Seçilen tarih aralığındaki aboneliklerin yüzdesi.
  - Mikro grafik, seçili tarih aralığındaki aylık abonelik eğilimini gösterir.

- Ürünlere göre abonelikler: Bulut ürünlerine göre geçerli abonelik sayısı dökümünü içerir.

## <a name="geographical-spread-of-subscriptions"></a>Aboneliklerin coğrafi yayılması

Coğrafyaya **göre abonelikler görünümü,** toplam aboneliklerin müşteri pazarlarına göre coğrafi dağılımını gösterir. Toplam abonelik tutarı hem satılan abonelikleri hem de etkin abonelikleri içerir.

**Ülke/bölge sayısı tablosu,** abonelikleri olan toplam ülkeler/bölgeler ile toplam ve etkin aboneliklerin ülke başına tutarını gösterir.

Haritanın konumunu yakınlaştırmak için kılavuzda bir ülke arayabilir ve bu ülkeyi seçin. Özgün **görünüme** dönmek için haritada Giriş seçeneğine basın. Ülkeye göre tüm abonelikleri ve etkin abonelikleri görüntülemek için haritanın üzerine gelin. Kılavuzda her iki alan da sıralanabilir.

:::image type="content" source="images/pci/pci-sub-report-sub-by-geography-2.png" alt-text="coğrafyaya göre abonelikler.":::

## <a name="subscription-addschurns"></a>Abonelik ekleri/veri churn'ları

Bu görünüm bir abonelik eğilimi sunar. Bunlar, seçilen tarih aralığı için farklı kategorilere (Yeni, Mevcut, Eski) ayrılır. X ekseni seçilen tarih aralığının aylarını temsil eder. Y ekseni abonelik sayısını temsil eder. Churned abonelikler Y ekseninin negatif ölçeğinde temsil eder. 

Yığılmış sütun grafiği, ay için yeni, mevcut ve eskitılmış aboneliklerin dökümünü sunar. Sütun grafiğini belirli yığın öğeleriyle birlikte yeniden oluşturabilirsiniz. Bunu yapmak için göstergedeki belirli öğeleri seçin. Ayrıca grafiğin üst kısmında yer alan kaydırıcıyı kullanarak belirli bir dönemi yakınlaştırabilirsiniz.

:::image type="content" source="images/pci/pci-sub-report-sub-adds-churns-3.png" alt-text="subscription adds and churns.":::

## <a name="subscription-distribution"></a>Abonelik dağıtımı

Bu görünüm, geçerli aboneliklerinizi Microsoft İş Ortağı Ağı (MPN) konumlara, müşteri segmentlerine, satış kanalına/Azure fiyatlandırma modeline ve asif türüne göre gösterir. Bu kategorilere göre dökümü görüntülemek için ilgili sekmeleri seçin. Pasta grafiğini belirli öğe kategorilerinin dökümüyle oluşturmak için göstergede bu öğe kategorilerini seçin.

:::image type="content" source="images/pci/pci-sub-report-distribution-4.png" alt-text="abonelik dağıtımı.":::

## <a name="subscription-state-distribution"></a>Abonelik durumu dağıtımı

Bu görünüm, geçerli müşteri aboneliklerinizi abonelik durumuna veya durumuna göre dağılımını gösterir. Bu, şu abonelik durumlarını içerir: **Etkin,** **Devre** **Dışı,** Onaysız , **Açık,** **InGracePeriod,** **Kapalı** ve **Diğerleri**.

:::image type="content" source="images/pci/pci-sub-report-sub-states-5.png" alt-text="abonelik durumu dağıtımı.":::

## <a name="products-trend"></a>Ürün eğilimi

Bu görünümde bir çubuk grafik ve iki pasta grafiği görüntülenir. Çubuk grafik, Azure, Office ve Dynamics gibi ticari ürünlere göre aylık abonelik eğilimini sunar.

İki pasta grafiği, geçerli müşteri aboneliklerinin dökümünü gösterir. İlk pasta grafiği abonelikleri ürünlere göre böler. İkinci pasta grafiği, abonelikleri SKUS'lara veya planlara göre böler. Products pasta grafiğine göre **dökümde bir** ürün seçerek bitişik pasta grafiğinde ilgili ürünün aboneliklerinin SSU'lara göre dökümü görüntülenir.

:::image type="content" source="images/pci/pci-sub-report-prods-trend-6.png" alt-text="ürün eğilimi.":::

> [!NOTE]
 > STU'lara göre kopan abonelik sayısı her zaman söz konusu ürün için toplam abonelik sayısıyla eşleşmez. Bir müşteri aynı ürün aboneliği altında birden çok SKUS satın alan bir durumda bu durum oluşabilir.

## <a name="next-steps"></a>Sonraki adımlar

- Daha fazla rapor için [bkz. İş Ortağı Merkezi Insights](partner-center-insights.md).

>[!NOTE] 
> Bu raporu güçlü bir şekilde kullanarak ham verileri Öngörüler panosunun Raporları İndir bölümünden indirebilirsiniz. [Daha Fazla Bilgi](pci-download-reports.md) 
