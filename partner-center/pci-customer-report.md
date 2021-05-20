---
title: İş Ortağı Merkezi öngörüleri-müşteri raporu
ms.topic: article
ms.date: 06/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: İşletmenizi geliştirmenin yollarını bulun. Belirli müşteri eğilimlerini coğrafya, ürüne ve diğer özniteliklere göre görün.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a9207e793865bcf7fa2f205fc69b0b5def65b4d
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152911"
---
# <a name="customers-dashboard-reports-from-partner-center-insights"></a>Iş Ortağı Merkezi öngörülerinin müşteriler Pano raporları

**Uygun roller**: genel yönetici | Yönetici Aracısı | Rapor Görüntüleyici | Executive rapor Görüntüleyicisi

Müşteriler panosu, sizin için Office, Azure, Dynamics vb. gibi bulut ürünlerini almış veya sizin için bu ürünleri kiracılar içinde dağıtmak ve yönetmek için kullandığınız müşterilerin verilerini sunar. 
 
Müşteriler Panosu aşağıdaki bölümlere sahiptir: 

- Özet  
- Müşterilerinizin coğrafi yayılmasının 
- Müşteriler ekleme/karmaşıklık eğilimleri 
- İş ortağı konumlarına, müşteri segmentlerine, Satış kanalına, iş ortağı atfı by müşterilere dağıtım 
- Ürüne göre müşteri dağıtımı 
- İş ortağı konumlarına, müşteri segmentlerine, fiyatlandırma modeline, iş ortağı atfı 'a göre müşterilerin dağıtım eğilimleri 
- Etkin müşteriler eğilimi 

## <a name="summary"></a>Özet

Özet bölümü, müşterilerinizle ilgili müşteriler, etkin müşteriler, abonelikler, müşteriler, eklenen müşteriler ve müşteriler gibi çeşitli KPI 'lerin bir anlık görüntü görünümünü sunar. Sayfa düzeyi filtreleri her bölüm için geçerlidir.

:::image type="content" source="images/pci/customerproduct.png" alt-text="Müşteriler Özet panosunda, çubuk grafikler ve müşterilerin sayısı etkin, son eklenen, kaybolan/veya belirli bir ürün tarafından gösterilir.":::

### <a name="customers"></a>Müşteriler

- Kuruluşunuzun, Office, Azure, Dynamics vb. gibi tüm bulut ürünlerinde farklı atfı türleri aracılığıyla ilişkilendirildiği tüm müşterilerin geçerli sayısı. Etkin durumdaki en az bir aboneliğiniz varsa, müşteri sayılır.  
- Seçilen tarih aralığında müşterilerin% ' i reddetme 
- Mikro grafik, müşterilerin seçili tarih aralığında sayımında bir ay boyunca aylık bir eğilim sunar

### <a name="active-customers"></a>Etkin müşteriler

- Herhangi bir bulut ürününde etkin kullanım gibi etkin ürün kullanımı olan müşterilerin geçerli sayısı.
- Seçili dönemde etkin müşterilerin büyüme veya reddetme oranı
- Mikro grafik, etkin müşterilerin seçili tarih aralığına göre aylara göre bir eğilim gösterir.

### <a name="customers-added"></a>Eklenen müşteriler

- Seçilen zaman dönemi boyunca eklenen tüm müşterilerin sayısı.
- Seçilen aralık sırasında eklenen müşterilerin büyüme veya reddetme oranı.
- Mikro grafik, seçilen tarih aralığına eklenen müşterilerin aylara göre aylık eğilimini gösterir.

### <a name="customers-churned"></a>Müşterilerde bir aksıma oldu
- Seçilen zaman dönemi boyunca her ay daha fazla zaman alan tüm müşterilerin sayısı. Müşterinin etkin durumu olan tek bir aboneliği yoksa müşteri kayıp olarak kabul edilir. 
- Seçilen tarih aralığındaki müşterilerin oranı düştü 
- Mikro grafik, seçilen zaman dönemi boyunca verim alan müşterilerin aylık eğilimini gösterir 
 
### <a name="customers-by-products"></a>Ürünlere göre müşteriler

- O365, Azure, Dynamics gibi çeşitli Bulut ürünlerine dağıtılmış olan müşterilerin geçerli sayısı.  

## <a name="geographical-spread-of-your-customers"></a>Müşterilerin coğrafi olarak yayılması

Seçilen tarih aralığında yeni eklenen geçerli müşterilerin, geçerli etkin müşterilerin ve müşterilerin sayısı, müşterinin ülkesi kullanılarak coğrafi olarak eşlenmiştir. Ölçümün altında görüntülenen yüzdeler, söz konusu ölçümün Toplam ülkesi için yüzde katkı yüzdesini belirtir. Haritanın üzerine gelerek ilgili ülkenin toplam, etkin ve yeni müşterilerini görüntüabilirsiniz. Haritanın konumunu yakınlaştırmak için kılavuzda bir ülke arayabilir ve bu ülkeyi seçin. Haritada Giriş düğmesini seçerek **özgün görünüme** geri dönebilirsiniz. Kılavuzda tüm sütunlar sıralanabilir.  

:::image type="content" source="images/pci/customersgeo.png" alt-text="Coğrafyaya İş Ortağı Merkezi Insights Müşteri raporunun ekran görüntüsü, bölgeye göre toplam, eklenen ve yeni müşterilerin dünya haritasını ve listesini gösterir.":::

## <a name="customer-adds-and-churns"></a>Müşteri ekler ve veri verisi ekler

Seçilen tarih aralığı için yeni, mevcut ve verim verisi alınarak dökümünü alan müşterilerin eğilimi. X ekseni seçilen tarih aralığının aylarını, Y ekseni ise müşterilerin sayısını temsil eder. Verim verisi alan müşteriler Y Ekseninin negatif ölçeğinde temsil edildi. Yığılmış sütun grafik, ay için yeni, mevcut ve verim alan müşterilerin ayrılmalarını gösterir. Göstergedeki öğeleri seçerek sütun grafiğini belirli yığın öğeleriyle yeniden oluşturabilirsiniz. Grafiği belirli bir süre yakınlaştırmak için grafiğin üst kısmında kaydırıcıdan faydalanabilirsiniz. 

:::image type="content" source="images/pci/customerslost.png" alt-text="Çubuk İş Ortağı Merkezi içgörüler Müşteri raporunun ekran görüntüsü, belirli bir süre içinde eklenen ve kaybolan veya kaybedilen müşteri sayısını gösterir.":::

## <a name="customer-distribution"></a>Müşteri dağıtımı

Geçerli müşterinizin MPN konumlarınızı, müşteri segmentlerinizi, satış kanalınızı/Azure fiyatlandırma modelinizi ve adisyon türünü (örneğin, DPOR, DAP) göre dökümü. Bu kategorilere göre dökümü görüntülemek için grafiğin üzerindeki ilgili sekmeleri seçin. Gösterge öğelerini seçerek/belirli boyutları seçerek grafiği yeniden oluşturabilirsiniz. 

## <a name="customers-by-products"></a>Ürünlere göre müşteriler

Geçerli müşteri saylarınızı ürünlere ve SKUS'lara/planlara göre çözümleme. Ürün kesme pasta grafiğinde bir ürün seçerek SKUS'lara/planlara göre ayrılmayı yanındaki grafikte görüntüebilirsiniz.

:::image type="content" source="images/pci/customerbyprod.png" alt-text="Ürüne göre müşteriler raporunun ekran görüntüsü, biri ürüne göre müşteri dökümü, diğeri SKU'ya göre müşteri dökümü olan iki radyal grafik gösterir.":::

## <a name="customer-distribution-trend"></a>Müşteri dağıtım eğilimi 

Pazarlara, segmentlere, MPN konumlarına ve edinilen ürünlere göre seçilen tarih aralığındaki müşteri dağılımının aylık eğilimi. Bu kategorilere göre eğilimi görüntülemek için grafikteki ilgili sekmeleri seçin. X ekseni seçtiğiniz tarih aralığı için ayları temsil eder ve Y ekseni seçili kategori (sekme seçimi) için müşteri sayısına sahiptir. Her yığının üzerine yığar değerleri görüntülemek için grafik sütunlarında üzerine gelebilmeniz gerekir. Belirli bir döneme yakınlaştırmak için grafiğin üstündeki kaydırıcıyı kullanabilirsiniz.   

:::image type="content" source="images/pci/customerdistri.png" alt-text="Pazara, segmente, iş ortağı konumuna veya ürünlere göre görüntüleyebileceğiniz çubuk grafiklerini gösteren müşteri dağıtım eğilimi raporunun ekran görüntüsü.":::

## <a name="active-customers"></a>Etkin müşteriler

Seçili tarih aralığı için etkin ve toplam müşterileri karşılaştıran aylık eğilim grafiği. Sütunlar her ay etkin müşteri sayılarını temsil eder ve satır her ay toplam müşteriyi temsil eder. 

:::image type="content" source="images/pci/activecustomer.png" alt-text="Iş Ortağı Merkezi öngörüleri etkin müşterilerin, etkin müşterilerin zaman içindeki çubuk grafiklerini göstermesini rapor eden ekran görüntüsü.":::

## <a name="next-steps"></a>Sonraki adımlar

Daha fazla rapor için bkz. [Partner Center öngörüleri](partner-center-insights.md).

>[!NOTE]
> Bu raporu, Öngörüler panosundaki raporları Indir bölümünden elde eden ham verileri indirebilirsiniz. [Daha Fazla Bilgi](pci-download-reports.md) 
