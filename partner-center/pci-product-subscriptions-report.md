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
ms.openlocfilehash: 89806b08485bc4bd286c2e14a19924ca0e281b6d
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854477"
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
- Ürünler eğilimi

 > [!NOTE]
 > Bu rapor, Öngörüler panosundan edinebilirsiniz. Bu raporu görüntülemek için Genel Yönetici, Hesap Yöneticisi, Rapor Görüntüleyicisi İş Ortağı Merkezi Yönetici Rapor Görüntüleyicisi gibi belirli bir rol atanmış olması gerekir. Daha fazla bilgi için, bkz. şirketinizin Genel Yöneticisi. Bu rapora özgü veri türleri yalnızca Yönetici Rapor Görüntüleyicisi ayrıcalıklarına sahip kullanıcılar tarafından da kullanılabilir.

## <a name="summary"></a>Özet

Özet bölümü, müşterileriniz için sizin tarafından satılan veya yönetilen aboneliklerle ilgili ana performans göstergelerinin (KIP) anlık görüntü görünümünü sunar.  

:::image type="content" source="images/pci/pci-sub-report-summary-1.png" alt-text="abonelikler rapor özeti":::

Özetin her bölümü hakkında daha fazla bilgi için aşağıya bakın:

- Abonelikler:
  - Sizin tarafından satılan veya yönetilen bulut ürünü aboneliklerinin geçerli sayısı.
  - Seçtiğiniz tarih aralığı boyunca aboneliklerin büyüme veya reddetme yüzdesi.
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

**Coğrafya görünümüne göre abonelikler** , toplam aboneliklerin müşteri pazarlarına göre coğrafi dağılımını gösterir. Toplam abonelik miktarı hem satılan abonelikler hem de etkin abonelikler içerir.

**Ülke/bölge sayısı tablosu,** abonelikleri olan toplam ülkeler/bölgeler ile toplam ve etkin aboneliklerin ülke başına tutarını gösterir.

Haritanın konumunu yakınlaştırmak için kılavuzda bir ülke arayabilir ve bu ülkeyi seçin. Özgün **görünüme** dönmek için haritada Giriş seçeneğine basın. Ülkeye göre tüm abonelikleri ve etkin abonelikleri görüntülemek için haritanın üzerine gelin. Kılavuzda her iki alan da sıralanabilir.

:::image type="content" source="images/pci/pci-sub-report-sub-by-geography-2.png" alt-text="coğrafyaya göre abonelikler":::

## <a name="subscription-addschurns"></a>Abonelik ekleri/veri churn'ları

Bu görünüm bir abonelik eğilimi sunar. Bunlar, seçilen tarih aralığı için farklı kategorilere (Yeni, Mevcut, Eski) ayrılır. X ekseni seçilen tarih aralığının aylarını temsil eder. Y ekseni abonelik sayısını temsil eder. Churned abonelikler Y ekseninin negatif ölçeğinde temsil eder. 

Yığılmış sütun grafiği, ay için yeni, mevcut ve eskitılmış aboneliklerin dökümünü sunar. Sütun grafiğini belirli yığın öğeleriyle birlikte yeniden oluşturabilirsiniz. Bunu yapmak için göstergedeki belirli öğeleri seçin. Ayrıca grafiğin üst kısmında yer alan kaydırıcıyı kullanarak belirli bir dönemi yakınlaştırabilirsiniz.

:::image type="content" source="images/pci/pci-sub-report-sub-adds-churns-3.png" alt-text="abonelik ekleri ve veri churn'ları":::

## <a name="subscription-distribution"></a>Abonelik dağıtımı

Bu görünüm MPN konumlarınızı, müşteri segmentlerinizi, satış kanalınızı/Azure fiyatlandırma modelinizi ve asif türünü (örneğin, DPOR, DAP ve diğerleri) kullanarak geçerli aboneliklerinizi dökümünü sunar. Bu kategorilere göre dökümünü görüntülemek için ilgili sekmeleri seçin. Pasta grafiğini belirli öğe kategorilerinin bir dökümü ile oluşturmak için, göstergede bu öğe kategorilerini seçin.

:::image type="content" source="images/pci/pci-sub-report-distribution-4.png" alt-text="abonelik dağıtımı":::

## <a name="subscription-state-distribution"></a>Abonelik durumu dağılımı

Bu görünüm, geçerli müşteri aboneliklerinizin abonelik durumu veya durumuna göre dağılımını gösterir. Bu, şu abonelik durumlarını içerir: **etkin**, **devre dışı**, **desağlanmamış**, **Open**, **yetkisizkullanımsüresinde**, **Closed** ve **diğerleri**.

:::image type="content" source="images/pci/pci-sub-report-sub-states-5.png" alt-text="Abonelik durumu dağılımı":::

## <a name="products-trend"></a>Ürün eğilimi

Bu görünüm bir çubuk grafiği ve iki pasta grafiği gösterir. Çubuk grafik, Azure, Office, Dynamics vb. gibi ticari ürünlere göre bölünmüş abonelikler için aylık bir eğilim sunar.

İki pasta grafik, geçerli müşteri aboneliklerinizin dökümünü gösterir. İlk pasta grafik, ürünlere göre abonelikleri ayırır. İkinci pasta grafik, STB veya planlara göre abonelikleri ayırır. **Ürünlere göre** döküm pasta grafiğinde bir ürünü seçtiğinizde, bitişik pasta grafiğinde bu ürüne ait aboneliklerde SKU 'lara ait bir döküm gösterilir.

:::image type="content" source="images/pci/pci-sub-report-prods-trend-6.png" alt-text="Ürün eğilimi":::

> [!NOTE]
 > SKU 'Lar tarafından kesilen abonelik sayısı, bu ürün için her zaman toplam abonelik sayısıyla eşleşmeyebilir. Bu durum, bir müşterinin aynı ürün aboneliği kapsamında birden çok SKU satın almış olması durumunda gerçekleşebilir.

## <a name="next-steps"></a>Sonraki adımlar

- Daha fazla rapor için bkz. [Partner Center öngörüleri](partner-center-insights.md).

>[!NOTE] 
> Bu raporu, Öngörüler panosundaki raporları Indir bölümünden elde eden ham verileri indirebilirsiniz. [Daha Fazla Bilgi](pci-download-reports.md) 
