---
title: iş ortağı merkezi Analizler-müşteri raporu
ms.topic: article
ms.date: 06/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: İşletmenizi geliştirmenin yollarını bulun. Belirli müşteri eğilimlerini coğrafya, ürüne ve diğer özniteliklere göre görün.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1b4efb558293313933b9c89d1f44b51058ed9926
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129074753"
---
# <a name="customers-dashboard-reports-from-partner-center-insights"></a>iş ortağı merkezi Analizler müşteriler pano raporları

**Uygun roller**: genel yönetici | Yönetici Aracısı | Rapor Görüntüleyici | Executive rapor Görüntüleyicisi

müşteriler panosu, müşterilerinizin Office, Azure ve Dynamics gibi bulut ürünlerini almış olan verilerini sunar. veya sizin için bu ürünleri kiracılar içinde dağıtmak ve yönetmek için kullanılır. 
 
Müşteriler Panosu aşağıdaki bölümlere sahiptir: 

- Özet  
- Müşterilerinizin coğrafi yayılmasının 
- Müşteriler ekleme/karmaşıklık eğilimleri 
- İş ortağı konumlarına, müşteri segmentlerine, Satış kanalına, iş ortağı atfı by müşterilere dağıtım 
- Ürüne göre müşteri dağıtımı 
- İş ortağı konumlarına, müşteri segmentlerine, fiyatlandırma modeline, iş ortağı atfı 'a göre müşterilerin dağıtım eğilimleri 
- Etkin müşteriler eğilimi 

## <a name="summary"></a>Özet

Özet bölümü müşterileri, etkin müşterileri, abonelikleri, müşteriler eklenen müşterileri, müşteriler tarafından yapılan müşterileri ve müşterilerin her ürüne göre müşterileri gibi çeşitli ana performans göstergelerinin (KPI) bir anlık görüntü görünümünü sunar. Sayfa düzeyi filtreleri her bölüm için geçerlidir.

:::image type="content" source="images/insights/customer-product.png" alt-text="Müşteriler Özet panosunda, çubuk grafikler ve müşterilerin sayısı etkin, son eklenen, kaybolan/veya belirli bir ürün tarafından gösterilir.":::

### <a name="customers"></a>Müşteriler

- kuruluşunuzun tüm bulut ürünlerinde Office, Azure ve Dynamics gibi farklı atfı türleri aracılığıyla ilişkilendirildiği tüm müşterilerin geçerli sayısı. Etkin durumdaki en az bir aboneliğiniz varsa, müşteri sayılır.  
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

- Office 365, Azure ve Dynamics gibi çeşitli bulut ürünlerinde dağıtılan müşterilerin güncel sayısı.  

## <a name="geographical-spread-of-your-customers"></a>Müşterilerinizin coğrafi yayılmasının

Seçilen tarih aralığında yeni eklenen geçerli müşteri sayısı, geçerli etkin müşteriler ve müşteriler, müşterinin ülkesi kullanılarak coğrafi olarak eşleştirilir. Ölçümün altında görüntülenen yüzdeler, bu ölçüm için toplam ülkenin yüzde katkısını gösterir. Bu ülkenin toplam, etkin ve yeni müşterilerini görüntülemek için haritada üzerine gelebilmeniz gerekir. Haritada konum yakınlaştırmak için kılavuzda bir ülke arayabilir ve seçebilirsiniz. Haritadaki **giriş** düğmesini seçerek özgün görünüme dönün. Kılavuzdaki tüm sütunlar sıralanabilir.  

:::image type="content" source="images/insights/customer-geography.png" alt-text="coğrafi olarak iş ortağı merkezi Analizler müşteri raporunun ekran görüntüsü, bölgelere göre dünya haritasını ve toplam, eklenen ve yeni müşterilerin listesini gösterir.":::

## <a name="customer-adds-and-churns"></a>Müşteri eklemeleri ve churns

Seçili tarih aralığı için yeni, mevcut ve yerleşik olarak dökümdeki müşterilerin eğilimi. X ekseni, seçilen tarih aralığının ve Y ekseninin, müşteriler sayısını temsil eden ayları temsil eder. Tek başına müşteriler, Y ekseninin negatif ölçeğinde temsil edilir. Yığılmış sütun grafiği, aya ait yeni, mevcut ve en fazla müşterilerin dağılımını gösterir. Göstergede olanları seçerek sütun grafiğini belirli yığın öğeleriyle yeniden oluşturabilirsiniz. Belirli bir döneme yakınlaştırmak için grafiğin üstündeki kaydırıcıyı kullanabilirsiniz. 

:::image type="content" source="images/insights/customer-lost.png" alt-text="bar grafik ile iş ortağı merkezi Analizler müşteri raporu, belirli bir süre boyunca eklenen ve kaybolan ve kesilen müşterilerin sayısını gösterir.":::

## <a name="customer-distribution"></a>Müşteri dağıtımı

Geçerli müşterilerinizin Microsoft İş Ortağı Ağı (MPN) konumlarınıza, müşteri segmentlerine, Satış kanalına/Azure fiyatlandırma modeline ve atısyon türüne göre dökümünü yapın. Bu kategorilerin dökümünü görüntülemek için grafiğin üzerindeki ilgili sekmeleri seçin. Gösterge öğelerini seçerek belirli boyutları seçerek/seçerek grafiği yeniden oluşturabilirsiniz. 

## <a name="customers-by-products"></a>Ürünlere göre müşteriler

Ürünlerin ve SKU 'Ların/planların geçerli müşterilerinin sayımının dökümünü yapın. Ürünün yanında bulunan SKU 'Ların/planların ölçeğini görüntülemek için ürün yukarı grafik pasta grafiğinde bir ürün seçin.

:::image type="content" source="images/insights/customer-by-product.png" alt-text="Ürün raporuna göre müşterilerin ekran görüntüsü, bir ürüne göre müşteri dökümlerinden biri olan diğeri SKU 'ya göre müşteri dökümlerinden oluşan iki Radyal grafiği gösterir.":::

## <a name="customer-distribution-trend"></a>Müşteri dağıtım eğilimi 

Pazarlara, segmentlere, MPN konumlarınıza ve elde ettikleri ürünlere göre seçilen tarih aralığı boyunca müşterilerinizin dağıtımına yönelik aylık eğilim. Bu kategorilere göre eğilimi görüntülemek için grafikteki ilgili sekmeleri seçin. X ekseni seçtiğiniz tarih aralığı için ayları temsil eder ve Y ekseni seçili kategori (sekme seçimi) için müşteri sayısına sahiptir. Her yığının üzerine yığar değerleri görüntülemek için grafik sütunlarında üzerine gelebilmeniz gerekir. Belirli bir döneme yakınlaştırmak için grafiğin üstündeki kaydırıcıyı kullanabilirsiniz.   

:::image type="content" source="images/insights/customer-by-distribution.png" alt-text="Pazara, segmente, iş ortağı konumuna veya ürünlere göre görüntüleyebileceğiniz çubuk grafiklerini gösteren müşteri dağıtım eğilimi raporunun ekran görüntüsü.":::

## <a name="active-customers"></a>Etkin müşteriler

Seçili tarih aralığı için etkin ve toplam müşterileri karşılaştıran aylık eğilim grafiği. Sütunlar her ay etkin müşteri sayılarını temsil eder ve satır her ay toplam müşteriyi temsil eder. 

:::image type="content" source="images/insights/active-customer.png" alt-text="etkin müşterilerin zaman içindeki çubuk grafiklerini gösteren iş ortağı merkezi Analizler etkin müşteriler ekran görüntüsü.":::

## <a name="next-steps"></a>Sonraki adımlar

daha fazla rapor için bkz. [iş ortağı merkezi Analizler](partner-center-insights.md).

>[!NOTE]
> ham verileri, Analizler panosundaki raporları indir bölümünden bu raporu güçden indirebilirsiniz. [Daha Fazla Bilgi](insights-download-reports.md) 
