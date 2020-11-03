---
title: İş Ortağı Merkezi Öngörüler abonelikleri raporu
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Müşterilerinizin sattığı ve yönettiğiniz bulut abonelikleriyle ilgili olarak neleri iyileştirebileceğinizi görün.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8df91ec4072b1873a240d42fa2382ebcc00b9bc5
ms.sourcegitcommit: 5f31146f50e01dc4c1922e0a5bc369f0a3cd8162
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/01/2020
ms.locfileid: "92531287"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>Ürün abonelikleri raporu Iş Ortağı Merkezi Öngörüler panosu 'nda mevcuttur

**Uygun roller**
- Genel yönetici
- Yönetim Aracısı
- Rapor Görüntüleyicisi
- Executive rapor Görüntüleyicisi

Ürün abonelikleri raporu, satmış olduğunuz veya müşterileriniz için yönettiğiniz bulut aboneliklerine ilişkin analizler sunar. Bu, Office 365, Azure, Dynamics vb. gibi bulut ürünleriyle ilişkili aboneliklerin performansını içeren ürüne özgü bir rapordur.

Ürün abonelikleri raporundan aşağıdaki bölümleri görüntüleyebilirsiniz.

- Özet
- Aboneliklerin coğrafi yayılmasının
- Abonelikler ekleme/karmaşıklık eğilimi
- İş ortağı konumlarına göre abonelik dağıtımı, satış kanalı, SKU 'Lar, iş ortağı iliştirme türü, segment
- Abonelik durumlarına göre eğilim
- Ürün eğilimi

 > [!NOTE]
 > Bu rapor, Öngörüler panosundan kullanılabilir. Bu raporu görüntülemek için Iş Ortağı Merkezi 'nde genel yönetici, hesap yöneticisi, rapor Görüntüleyicisi veya Executive rapor Görüntüleyicisi gibi belirli bir rol atanması gerekir. Daha fazla bilgi için şirketinizin genel Yöneticisi ' ne bakın. bu rapordaki belirli veri türleri yalnızca, Executive rapor Görüntüleyicisi ayrıcalıklarına sahip kullanıcılar tarafından kullanılabilir.

## <a name="summary"></a>Özet

Özet bölümü, müşterileriniz için sizin tarafınızdan satılan veya yönetilen Aboneliklerle ilgili ana performans göstergelerinin (KPI) bir anlık görüntü görünümünü sunar.  

:::image type="content" source="images/pci/pci-sub-report-summary-1.png" alt-text="abonelik raporu Özeti":::

Özetin her bölümü hakkında daha fazla bilgi için aşağıya bakın.

- Abonelikler:
  - Sizin tarafınızdan satılan veya yönetilen bulut ürün aboneliklerinin güncel sayısı.
  - Seçtiğiniz tarih aralığınızı sırasında aboneliklerin artış veya reddetme yüzdesi.
  - Mikro grafik, seçtiğiniz tarih aralığınızdan abonelik sayısı için aylık bir eğilim gösterir.

- Etkin Abonelikler:
  - Ürün telemetrisine göre ölçülen etkin kullanım ile bulut ürün aboneliklerinin güncel sayısı. Bu, Azure abonelikleri durumunda tüm deneme aboneliklerini dışlar.
  - Seçili zaman dilimi boyunca etkin abonelikler için büyüme veya reddetme yüzdesi.
  - Mikro grafik, seçtiğiniz tarih aralığınızdan etkin abonelikler için aylık bir eğilim gösterir.

- Eklenen abonelikler:
  - Seçilen tarih aralığı sırasında sizin tarafınızdan eklenen (satılan veya yönetilen) toplam müşteri aboneliği. **Etkin** veya **yenilenen** duruma sahip yeni abonelikler, abonelikler eklendiğinde sayılır.
  - Son tam aya eklenen aboneliklerin artış veya reddetme yüzdesi, ilk tam aya göre.
  - Mikro grafik, seçtiğiniz tarih aralığınızı sırasında eklenen aboneliklerin aylık eğilimini gösterir.

- Abonelik tarafından kullanılan:
  - Seçtiğiniz tarih aralığında belirlenen toplam müşteri aboneliği. Söz konusu ayda **sağlanmış** veya **askıya alınmış** durumdaki abonelikler, bir abonelik olarak sayılır.  
  - Seçilen tarih aralığı sırasında abonelik yüzdesi.
  - Mikro grafik, seçilen tarih aralığı boyunca aboneliklerin aylık eğilimini gösterir.

- Ürünlere göre abonelikler: bulut ürünlerine göre geçerli abonelik sayısı dökümü.

## <a name="geographical-spread-of-subscriptions"></a>Aboneliklerin coğrafi yayılmasının

**Coğrafya görünümü tarafından abonelikler** , müşteri pazarlarına göre toplam aboneliklerin coğrafi dağılımını gösterir. Toplam abonelik miktarı hem satılan abonelikler hem de etkin abonelikler içerir.

**Ülke/bölge tablosu sayısı** , aboneliklerinizin bulunduğu toplam ülkeleri/bölgeleri ve toplam ve etkin abonelikler için ülke başına miktarı gösterir.

Haritada konum yakınlaştırmak için kılavuzda bir ülke arayabilir ve seçebilirsiniz. Özgün görünüme dönmek için haritanın **giriş** seçeneğine basın. Ülkeye göre tüm abonelikleri ve etkin abonelikleri görüntülemek için haritaya gelin. Kılavuzdaki her iki alan de sıralanabilir.

:::image type="content" source="images/pci/pci-sub-report-sub-by-geography-2.png" alt-text="abonelik raporu Özeti":::

## <a name="subscription-addschurns"></a>Abonelik eklemeleri/churns

Bu görünüm, aboneliklerin eğilimini gösterir. Bunlar, seçilen tarih aralığı için farklı kategorilere ayrılır (yeni, varolan, Çüşsal). X ekseni, seçilen tarih aralığının ayları temsil eder. Y ekseni abonelik sayısını temsil eder. Tek başına abonelikler, Y ekseninin negatif ölçeğinde temsil edilir. 

Yığılmış sütun grafiği, ay için yeni, mevcut ve birlikte bulunan aboneliklerin dökümünü gösterir. Sütun grafiğini, belirli yığın öğeleriyle ayrılmış şekilde yeniden oluşturabilirsiniz. Bunu yapmak için, göstergede söz konusu öğeleri seçin. Ayrıca, belirli bir döneme yakınlaştırmak için grafiğin üstündeki kaydırıcıyı de kullanabilirsiniz.

:::image type="content" source="images/pci/pci-sub-report-sub-adds-churns-3.png" alt-text="abonelik raporu Özeti":::

## <a name="subscription-distribution"></a>Abonelik dağıtımı

Bu görünüm, MPN konumlarınızın, Müşteri segmentlerinin, satış kanalının/Azure fiyatlandırma modelinin ve atısyon türünün (örn. DPOR, DAP vb.) geçerli aboneliklerinizin dökümünü gösterir. Bu kategorilerin dökümünü görüntülemek için ilgili sekmelere tıklayın. Pasta grafiğini belirli öğe kategorilerinin bir dökümü ile oluşturmak için, göstergede bu öğe kategorilerini seçin.

:::image type="content" source="images/pci/pci-sub-report-distribution-4.png" alt-text="abonelik raporu Özeti":::

## <a name="subscription-state-distribution"></a>Abonelik durumu dağılımı

Bu görünüm, geçerli müşteri aboneliklerinizin abonelik durumu veya durumuna göre dağılımını gösterir. Bu, şu abonelik durumlarını içerir: **etkin** , **devre dışı** , **desağlanmamış** , **Open** , **yetkisizkullanımsüresinde** , **Closed** ve **diğerleri** .

:::image type="content" source="images/pci/pci-sub-report-sub-states-5.png" alt-text="abonelik raporu Özeti":::

## <a name="products-trend"></a>Ürün eğilimi

Bu görünüm bir çubuk grafiği ve iki pasta grafiği gösterir. Çubuk grafik, Azure, Office, Dynamics vb. gibi ticari ürünlere göre bölünmüş abonelikler için aylık bir eğilim sunar.

İki pasta grafik, geçerli müşteri aboneliklerinizin dökümünü gösterir. İlk pasta grafik, ürünlere göre abonelikleri ayırır. İkinci pasta grafik, STB veya planlara göre abonelikleri ayırır. **Ürünlere göre** döküm pasta grafiğinde bir ürünü seçtiğinizde, bitişik pasta grafiğinde bu ürüne ait aboneliklerde SKU 'lara ait bir döküm gösterilir.

:::image type="content" source="images/pci/pci-sub-report-prods-trend-6.png" alt-text="abonelik raporu Özeti":::

> [!NOTE]
 > SKU 'Lar tarafından kesilen abonelik sayısı, bu ürün için her zaman toplam abonelik sayısıyla eşleşmeyebilir. Bu durum, bir müşterinin aynı ürün aboneliği kapsamında birden çok SKU satın almış olması durumunda gerçekleşebilir.

## <a name="next-steps"></a>Sonraki adımlar

- Daha fazla rapor için bkz. [Partner Center öngörüleri](partner-center-insights.md).

>[!NOTE] 
> Bu raporu, Öngörüler panosundaki raporları Indir bölümünden elde eden ham verileri indirebilirsiniz. [Daha Fazla Bilgi](pci-download-reports.md) 
