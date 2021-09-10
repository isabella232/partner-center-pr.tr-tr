---
title: İş Ortağı Merkezi Analizler - Müşteri raporu
ms.topic: article
ms.date: 06/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: İşletmenizi geliştirmenin yollarını keşfedin. Coğrafyaya, ürüne ve diğer özniteliklere göre belirli müşteri eğilimlerinizi görme.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 327d2ddd97dc4bf226985523184407f32f7883ad
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960235"
---
# <a name="customers-dashboard-reports-from-partner-center-insights"></a>Müşteri pano raporları İş Ortağı Merkezi Analizler

**Uygun roller:** Genel yönetici | Yönetici aracısı | Rapor görüntüleyicisi | Yönetici raporu görüntüleyicisi

Müşteriler panosu, Office, Azure ve Dynamics gibi bulut ürünlerini satın alan Office verilerini sunar. aracılığıyla veya kiracılarında bu ürünleri dağıtmak ve yönetmek için sizi kullandınız. 
 
Müşteriler panosu aşağıdaki bölümlere sahip: 

- Özet  
- Müşterilerin coğrafi olarak yayılması 
- Müşteriler eğilim ekleme/veri eğilimini geri alıyor 
- İş ortağı konumlara, müşteri segmentlerine, satış kanalına, iş ortağı atfı türüne göre müşterilerin dağıtımı 
- Ürüne göre müşteri dağıtımı 
- İş ortağı konumlara, müşteri segmentlerine, fiyatlandırma modeline, iş ortağı atfı türüne göre müşterilerin dağıtım eğilimleri 
- Etkin müşteriler eğilimi 

## <a name="summary"></a>Özet

Özet bölümünde müşteriler, etkin müşteriler, abonelikler, eklenen müşteriler, müşteriler ve her ürüne göre müşteriler gibi müşterilerinizle ilgili çeşitli ana performans göstergelerinin (KIP) anlık görüntü görünümü yer almaktadır. Sayfa düzeyi filtreleri her bölüm için geçerlidir.

:::image type="content" source="images/insights/customer-product.png" alt-text="Etkin, yakın zamanda eklenen, kaybolan/kaybedilen veya belirli bir ürüne göre müşterilerin çubuk grafiklerini ve sayılarını gösteren Müşteri Özeti panosunun ekran görüntüsü.":::

### <a name="customers"></a>Müşteriler

- Şu anda, Office, Azure ve Dynamics gibi tüm bulut ürünlerinde farklı atfı türleri aracılığıyla, Office tüm müşteri sayısıyla ilişkilendirilmektedir. Etkin durumuna sahip en az bir aboneliği varsa müşteri sayılır.  
- Seçilen tarih aralığındaki müşterilerin %1'ini reddetme 
- Micro chart presents month over month trend of customers count over the selected date range

### <a name="active-customers"></a>Etkin Müşteriler

- Herhangi bir bulut ürününde etkin kullanım gibi etkin ürün kullanımı olan müşterilerin geçerli sayısı.
- Seçili dönemde etkin müşterilerin büyüme veya reddetme oranı
- Mikro grafik, etkin müşterilerin seçili tarih aralığına göre aylara göre bir eğilim gösterir.

### <a name="customers-added"></a>Eklenen müşteriler

- Seçilen zaman dönemi boyunca eklenen tüm müşterilerin sayısı.
- Seçilen aralık sırasında eklenen müşterilerin büyüme veya reddetme oranı.
- Mikro grafik, seçilen tarih aralığına eklenen müşterilerin aylara göre aylık eğilimini gösterir.

### <a name="customers-churned"></a>Müşterilerde bir aksıma oldu
- Seçilen zaman dönemi boyunca her ay daha fazla zaman alan tüm müşterilerin sayısı. Müşterinin etkin durumda tek bir aboneliği yoksa müşteri kayıp olarak kabul edilir. 
- Seçilen tarih aralığındaki müşterilerin oranı düştü 
- Mikro grafik, seçilen zaman dönemi boyunca verim alan müşterilerin aylık eğilimini gösterir 
 
### <a name="customers-by-products"></a>Ürünlere göre müşteriler

- Office 365, Azure ve Dynamics gibi çeşitli Bulut Office 365 dağıtılan müşterilerin sayısı.  

## <a name="geographical-spread-of-your-customers"></a>Müşterilerin coğrafi olarak yayılması

Seçilen tarih aralığında yeni eklenen geçerli müşterilerin, geçerli etkin müşterilerin ve müşterilerin sayısı, müşterinin ülkesi kullanılarak coğrafi olarak eşlenmiştir. Ölçümün altında görüntülenen yüzdeler, söz konusu ölçümün Toplam ülkesi için yüzde katkısını belirtir. Haritanın üzerine gelerek ilgili ülkenin toplam, etkin ve yeni müşterilerini görüntüabilirsiniz. Haritanın konumunu yakınlaştırmak için kılavuzda bir ülke arayabilir ve bu ülkeyi seçin. Haritada Giriş düğmesini seçerek **özgün görünüme** geri dönebilirsiniz. Kılavuzda tüm sütunlar sıralanabilir.  

:::image type="content" source="images/insights/customer-geography.png" alt-text="Bölgeye İş Ortağı Merkezi Analizler Müşteri raporunun ekran görüntüsü, bölgeye göre toplam, eklenen ve yeni müşterilerin dünya haritasını ve listesini gösterir.":::

## <a name="customer-adds-and-churns"></a>Müşteri ek ve veri verisi ekler

Seçili tarih aralığı için yeni, mevcut ve verim verisi alınarak dökümü alınarak verim alan müşterilerin eğilimi. X ekseni seçilen tarih aralığının aylarını, Y ekseni ise müşterilerin sayısını temsil eder. Verim verisi alan müşteriler Y Ekseninin negatif ölçeğinde temsil eder. Yığılmış sütun grafik, ay için yeni, mevcut ve verim alan müşterilerin ayrılmalarını gösterir. Göstergedeki öğeleri seçerek sütun grafiğini belirli yığın öğeleriyle yeniden oluşturabilirsiniz. Grafiği belirli bir süre yakınlaştırmak için grafiğin üst kısmında kaydırıcıdan faydalanabilirsiniz. 

:::image type="content" source="images/insights/customer-lost.png" alt-text="Çubuk İş Ortağı Merkezi Analizler müşteri raporunun ekran görüntüsü, belirli bir süre içinde eklenen ve kaybolan veya kaybedilen müşteri sayısını gösterir.":::

## <a name="customer-distribution"></a>Müşteri dağıtımı

Geçerli müşterinizin Microsoft İş Ortağı Ağı (MPN) konumlara, müşteri segmentlerine, satış kanalına/Azure fiyatlandırma modeline ve asif türüne göre dökümü. Bu kategorilere göre dökümü görüntülemek için grafiğin üzerindeki ilgili sekmeleri seçin. Gösterge öğelerini seçerek/belirli boyutları seçerek grafiği yeniden oluşturabilirsiniz. 

## <a name="customers-by-products"></a>Ürünlere göre müşteriler

Geçerli müşteri saylarınızı ürünlere ve SKUS'lara/planlara göre çözümleme. Ürün kesme pasta grafiğinde bir ürün seçerek SKUS'lara/planlara göre ayrılmayı yanındaki grafikte görüntüebilirsiniz.

:::image type="content" source="images/insights/customer-by-product.png" alt-text="Ürüne göre müşteriler raporunun ekran görüntüsü, biri ürüne göre müşteri dökümü, diğeri SKU'ya göre müşteri dökümü olan iki radyal grafik gösterir.":::

## <a name="customer-distribution-trend"></a>Müşteri dağıtım eğilimi 

Pazarlara, segmentlere, MPN konumlarına ve edinilen ürünlere göre seçilen tarih aralığındaki müşteri dağılımının aylık eğilimi. Bu kategorilere göre eğilimi görüntülemek için grafikte ilgili sekmeleri seçin. X ekseni, seçtiğiniz tarih aralığı için ayları temsil eder ve Y ekseni seçilen kategoriye (Sekme seçimi) ait müşteri sayısını gösterir. Her bir yığının değerlerinin ayrımlarını görüntülemek için grafik sütunlarının üzerine gelin. Grafiği belirli bir süre yakınlaştırmak için grafiğin üst kısmında kaydırıcıdan faydalanabilirsiniz.   

:::image type="content" source="images/insights/customer-by-distribution.png" alt-text="Pazara, segmente, iş ortağı konuma veya ürünlere göre görüntülebilirsiniz çubuk grafikleri gösteren Müşteri dağıtımı eğilim raporunun ekran görüntüsü.":::

## <a name="active-customers"></a>Etkin müşteriler

Seçili tarih aralığı için etkin ve toplam müşterileri karşılaştıran aylık eğilim grafiği. Sütunlar her ay etkin müşteri sayısını, satır ise her ay toplam müşteri sayısını temsil eder. 

:::image type="content" source="images/insights/active-customer.png" alt-text="Etkin İş Ortağı Merkezi Analizler zaman içinde çubuk grafikleri gösteren Etkin müşteriler raporunun ekran görüntüsü.":::

## <a name="next-steps"></a>Sonraki adımlar

Daha fazla rapor için [bkz. İş Ortağı Merkezi Analizler.](partner-center-insights.md)

>[!NOTE]
> Bu raporu güçlü bir şekilde kullanarak ham verileri panonun Raporları İndir bölümünden Analizler indirebilirsiniz. [Daha Fazla Bilgi](insights-download-reports.md) 
