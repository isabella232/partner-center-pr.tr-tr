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
ms.openlocfilehash: 28343b5754546b653bd5a3e6b4a53a002b408668
ms.sourcegitcommit: 078eac1456f68585ff1003b21e5e1fe777af314b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/28/2021
ms.locfileid: "108120843"
---
# <a name="customers-dashboard-reports-from-partner-center-insights"></a>Iş Ortağı Merkezi öngörülerinin müşteriler Pano raporları

**Uygun roller**

- Genel yönetici
- Yönetim Aracısı
- Rapor Görüntüleyicisi
- Executive rapor Görüntüleyicisi

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

- Herhangi bir bulut ürününde etkin kullanım gibi etkin ürün kullanımı olan geçerli müşteri sayısı.
- Seçilen dönemde etkin müşterilerin% büyüme veya reddetme yüzdesi
- Mikro grafik, seçilen tarih aralığında etkin müşterilerin sayından aya göre aylık bir eğilim gösterir.

### <a name="customers-added"></a>Eklenen müşteriler

- Seçilen dönemde eklenen tüm müşterilerin sayısı.
- Seçilen sate aralığında eklenen müşterilerin büyüme veya reddetme yüzdesi.
- Mikro grafik, seçilen tarih aralığı boyunca eklenen müşterilerin ayda bir eğilimini gösterir.

### <a name="customers-churned"></a>Müşteriler tarafından kullanılan
- Seçilen dönemde her ay tüm müşterilerin sayısı. Müşterinin etkin durumu olan tek bir aboneliği yoksa, bir müşteri kaybedilmez olarak kabul edilir. 
- Seçilen tarih aralığı boyunca kullanılan müşterilerin yüzdesi 
- Mikro grafik, seçilen zaman dilimi boyunca geçen müşterilerin aylık eğilimi eğilimlerini gösterir 
 
### <a name="customers-by-products"></a>Ürünlere göre müşteriler

- O365, Azure, Dynamics vb. gibi çeşitli bulut ürünlerinde dağıtılan müşterilerin güncel sayısı.  

## <a name="geographical-spread-of-your-customers"></a>Müşterilerinizin coğrafi yayılmasının

Seçilen tarih aralığında yeni eklenen geçerli müşteri sayısı, geçerli etkin müşteriler ve müşteriler, müşterinin ülkesi kullanılarak coğrafi olarak eşleştirilir. Ölçümün altında görüntülenen yüzdeler, bu ölçüm için toplam ülkenin yüzde katkısını gösterir. Bu ülkenin toplam, etkin ve yeni müşterilerini görüntülemek için haritada üzerine gelebilmeniz gerekir. Haritada konum yakınlaştırmak için kılavuzda bir ülke arayabilir ve seçebilirsiniz. Haritadaki **giriş** düğmesini seçerek özgün görünüme dönün. Kılavuzdaki tüm sütunlar sıralanabilir.  

:::image type="content" source="images/pci/customersgeo.png" alt-text="Coğrafya tarafından Iş Ortağı Merkezi öngörüleri müşteri raporu, bölgelere göre dünya haritasını ve toplam, eklenen ve yeni müşterilerin listesini gösterir.":::

## <a name="customer-adds-and-churns"></a>Müşteri eklemeleri ve churns

Seçili tarih aralığı için yeni, mevcut ve yerleşik olarak dökümdeki müşterilerin eğilimi. X ekseni, seçilen tarih aralığının ve Y ekseninin, müşteriler sayısını temsil eden ayları temsil eder. Tek başına müşteriler, Y ekseninin negatif ölçeğinde temsil edilir. Yığılmış sütun grafiği, aya ait yeni, mevcut ve en fazla müşterilerin dağılımını gösterir. Göstergede olanları seçerek sütun grafiğini belirli yığın öğeleriyle yeniden oluşturabilirsiniz. Belirli bir döneme yakınlaştırmak için grafiğin üstündeki kaydırıcıyı kullanabilirsiniz. 

:::image type="content" source="images/pci/customerslost.png" alt-text="Iş Ortağı Merkezi öngörüleri müşteri raporunun çubuk grafik görüntüsü, belirli bir süre boyunca eklenen ve kaybolan veya ortaya geçen müşterilerin sayısını gösterir.":::

## <a name="customer-distribution"></a>Müşteri dağıtımı

MPN konumlarınıza, müşteri segmentlerinize, Satış kanalına/Azure fiyatlandırma modelinize ve atısyon türüne (örneğin, DPOR, DAP) göre geçerli müşterilerinizin dökümü. Bu kategorilerin dökümünü görüntülemek için grafiğin üzerindeki ilgili sekmeleri seçin. Gösterge öğelerini seçerek belirli boyutları seçerek/seçerek grafiği yeniden oluşturabilirsiniz. 

## <a name="customers-by-products"></a>Ürünlere göre müşteriler

Ürünlerin ve SKU 'Ların/planların geçerli müşterilerinin sayımının dökümünü yapın. Ürünün yanında bulunan SKU 'Ların/planların ölçeğini görüntülemek için ürün yukarı grafik pasta grafiğinde bir ürün seçin.

:::image type="content" source="images/pci/customerbyprod.png" alt-text="Ürün raporuna göre müşterilerin ekran görüntüsü, bir ürüne göre müşteri dökümlerinden biri olan diğeri SKU 'ya göre müşteri dökümlerinden oluşan iki Radyal grafiği gösterir.":::

## <a name="customer-distribution-trend"></a>Müşteri dağıtım eğilimi 

Pazarlara, segmentlere, MPN konumlarınıza ve elde ettikleri ürünlere göre seçilen tarih aralığı boyunca müşterilerinizin dağıtımına yönelik aylık eğilim. Bu kategorilere göre eğilimi görüntülemek için grafikteki ilgili sekmeleri seçin. X ekseni seçtiğiniz tarih aralığı için ayları temsil eder ve Y ekseni seçili kategori (sekme seçimi) için müşteri sayısına sahiptir. Her yığının üzerine yığar değerleri görüntülemek için grafik sütunlarında üzerine gelebilmeniz gerekir. Belirli bir döneme yakınlaştırmak için grafiğin üstündeki kaydırıcıyı kullanabilirsiniz.   

:::image type="content" source="images/pci/customerdistri.png" alt-text="Pazara, segmente, iş ortağı konumuna veya ürünlere göre görüntüleyebileceğiniz çubuk grafiklerini gösteren müşteri dağıtım eğilimi raporunun ekran görüntüsü.":::

## <a name="active-customers"></a>Etkin müşteriler

Seçili tarih aralığı için etkin ve toplam müşterileri karşılaştıran aylık eğilim grafiği. Sütunlar her ay etkin müşteri sayılarını temsil eder ve satır her ay toplam müşteriyi temsil eder. 

:::image type="content" source="images/pci/activecustomer.png" alt-text="Iş Ortağı Merkezi öngörüleri etkin müşterilerin, etkin müşterilerin zaman içindeki çubuk grafiklerini göstermesini rapor eden ekran görüntüsü.":::

## <a name="next-steps"></a>Sonraki adımlar

Daha fazla rapor için bkz. [Partner Center öngörüleri](partner-center-insights.md).

>[!NOTE]
> Bu raporu, Öngörüler panosundaki raporları Indir bölümünden elde eden ham verileri indirebilirsiniz. [Daha Fazla Bilgi](pci-download-reports.md) 
