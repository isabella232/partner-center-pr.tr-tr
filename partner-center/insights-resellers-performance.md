---
title: İş Ortağı Merkezi Analizler Kurumsal Bayi Performansı panosu
ms.topic: article
ms.date: 09/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: İş Ortağı Merkezi Analizler'daki kurumsal İş Ortağı Merkezi Analizler panosu, bir Bulut Çözümü Sağlayıcısı (CSP) Indirect Provider'ın dolaylı kurumsal bayilerinin performansına genel bir bakış sağlar.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 796af99cc405a72bebcd467b242dafb83ac756e5
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960814"
---
# <a name="reseller-performance-dashboard-in-partner-center-insights"></a>İş Ortağı Merkezi Analizler'de Bayi Performansı panosu

**Uygun roller:** Genel yönetici | Yönetici aracısı | Rapor görüntüleyici | Yönetici raporu görüntüleyicisi

İş Ortağı Merkezi Analizler'daki kurumsal İş Ortağı Merkezi Analizler panosu, bir Bulut Çözümü Sağlayıcısı (CSP) Dolaylı Sağlayıcısının dolaylı kurumsal bayilerinin performansına genel bir bakış sağlar. Pano etkin olan kurumsal bayiler, ne kadar gelir elde edildileri ve geliri sağlayan ürünlerle ilgili veriler sağlar. Dolaylı Sağlayıcılar, adına göre belirli bir kurumsal bayiyi arayabilir ve kurumsal bayi performans panosunda kurumsal bayinin ayrıntılarını arayabilir.

Bayi Performansı panosundan aşağıdaki bölümleri görüntüleyebilirsiniz.

- Özet
- Kurumsal bayilerin coğrafi yayılması
- Kurumsal bayiler ekleme/veri churns 
- Kurumsal bayi gelir eğilimi 
- Ürünlere göre bayi performansı
- İş ortağı konumlara göre etkin kurumsal bayiler
- Gelir coğrafi dağıtım eğilimi
- Müşteri kesimine göre kurumsal bayi performansı
- Kurumsal Microsoft İş Ortağı Sözleşmesi (MPA) imzalama durumu

 > [!NOTE]
 > Bu rapor, Analizler kullanılabilir. Bu raporu görüntülemek için genel yönetici, hesap İş Ortağı Merkezi, Rapor görüntüleyicisi veya Yönetici rapor görüntüleyicisi gibi belirli bir rol atanmış olması gerekir. Daha fazla bilgi için bkz. şirketin Genel yöneticisi. Bu rapora özgü veri türleri yalnızca Yönetici rapor görüntüleyici ayrıcalıklarına sahip kullanıcılar tarafından da kullanılabilir.

## <a name="summary"></a>Özet

Özet bölümünde, verilerle ilgili ana performans göstergelerinin (KIP' ler) anlık görüntü CSP Indirect Provider.

- Etkin kurumsal bayiler: O ay boyunca en az bir etkin aboneliğe sahip olan kurumsal bayilerin sayısı.

Mikro grafik, seçili tarih aralığında etkin olan farklı kurumsal bayilerin aylara göre eğilimini gösterir.

- Kurumsal bayileri işlemden geçen: Bu ay boyunca en az bir abonelik satılan kurumsal bayi sayısı. 

Mikro grafik, seçilen tarih aralığına kayıtlı bayilerin aylara göre eğilimini gösterir.

- Yeni kurumsal bayiler: Bu ay içinde Dolaylı Sağlayıcı ile işlem yapmaya başlayan kurumsal bayilerin sayısı. 

Micro grafiği, seçilen tarih aralığındaki toplam yeni kurumsal bayi sayısına göre aylara göre eğilim gösterir.

- Faturalandırılacak gelir USD: Söz konusu ay boyunca bayiler tarafından yönlendirilecek OLAN ABD doları gelir. 

Micro grafiği, seçilen tarih aralığında aylık gelir eğilimini gösterir.

- Ürünlere göre faturalandırılmış gelir bölümü, ABD doları olarak faturalandırılmış gelirin satılan ürünlere göre bölünmüş aylık dökümünü sağlar. 

:::image type="content" source="images/insights/resellers-performance-summary.png" alt-text="kurumsal bayi performans özeti.":::

## <a name="geographical-spread-of-resellers"></a>Kurumsal bayilerin coğrafi yayılması

**Coğrafyaya göre kurumsal bayiler görünümü, Kurumsal Bayilerin coğrafi dağıtımını sağlar. bu pencere öğesi kullanılarak iş ortakları, çeşitli **coğrafyalara** göre ayrılmış toplam Kurumsal **Bayiler,** Yeni bayiler ve Faturalandırmış Gelir **(USD)** öğelerini görüntülemenizi sağlar.

Haritanın konumunu yakınlaştırmak için kılavuzda bir ülke arayabilir ve bu ülkeyi seçin. Özgün **görünüme** dönmek için haritada Giriş seçeneğine basın. Ülkeye göre Faturalandırilen **Geliri (USD) görüntülemek için haritanın** üzerine gelin. Kılavuzda Faturalanmış Gelir (USD) alanı sıralanabilir.

:::image type="content" source="images/insights/resellers-performance-by-geo.png" alt-text="Coğrafyaya göre bayiler.":::

## <a name="resellers-addchurns"></a>Kurumsal bayiler ekleme/veri churns

Bu görünüm, Yeni kurumsal bayi sayısı, **Churned** **Resellers** ve Mevcut Kurumsal Bayi sayısının aylara **bölünmesini sağlar.** 

- Yeni kurumsal bayiler: Seçilen tarih aralığında Dolaylı Sağlayıcıya yeni kaydolan kurumsal bayilerin sayısı.
- Farklı bayiler: Geçerli ay hariç son altı ay boyunca işlem yapan kurumsal bayilerin sayısı.
- Mevcut kurumsal bayiler: Önceki ay işlem yapan kurumsal bayilerin sayısı.

:::image type="content" source="images/insights/resellers-performance-add-churn.png" alt-text="Kurumsal bayiler ekleme/alma/":::

## <a name="resellers-revenue-trend"></a>Kurumsal bayi gelir eğilimi 

Bu görünüm; Office 365, Dynamics 365, Enterprise Mobility and Security (EMS), Microsoft Power BI ve Azure gibi ürünlere göre bölünmüş aylık faturalı gelir eğilimini sağlar. Genel ölçümler her ay için çeşitli ürünler genelinde toplanır. İş ortağı, adına göre belirli bir kurumsal bayiyi arayabilir ve bu kurumsal bayiye yönelik verileri arayabilir. Kılavuzda Faturalanmış Gelir (USD) alanı sıralanabilir.

:::image type="content" source="images/insights/resellers-performance-revenue-trend.png" alt-text="Kurumsal bayi gelir eğilimi.":::

## <a name="reseller-performance-by-products"></a>Ürünlere göre bayi performansı

Bu görünüm, aylık olarak Faturalandırılacak Gelir, abonelik sayısı ve çeşitli ürünlere göre lisans sayısı gibi temel ölçümlerin bölünmesi sağlar. Sağ bölmede yer alan pasta grafiği, ölçümlerin çeşitli ürünlere göre genel olarak ayrıldığını gösterir. Böylece iş ortağı, kurumsal bayinin satışını yapan çeşitli ürünlere göre ayırmaya hızlı bir bakış elde ediyor.

:::image type="content" source="images/insights/resellers-performance-product.png" alt-text="Ürünlere göre bayi performansı.":::

## <a name="active-resellers-by-partner-locations"></a>İş ortağı konumlara göre etkin kurumsal bayiler

Bu görünüm, etkin kurumsal bayilerin iş ortağı coğrafyalara göre bölünmelerini sağlar. İlk beş coğrafya, göstergede gösterilir ve kalanlar 'Diğer' kategorisine ayrılmıştır.

:::image type="content" source="images/insights/resellers-performance-location.png" alt-text="İş ortağı konumlara göre etkin kurumsal bayiler.":::

## <a name="revenue-geo-distribution-trend"></a>Gelir coğrafi dağıtım eğilimi

Bu görünüm, faturalandırılacak gelirin (USD) ilk beş coğrafyaya göre aylara göre eğilimini sağlar.  Gelirin geri kalanı 'Diğer' kategorisine ayrılmıştır.

:::image type="content" source="images/insights/resellers-performance-revenue-geo-trend.png" alt-text="Gelir coğrafi dağıtım eğilimi.":::

## <a name="reseller-performance-by-customer-segment"></a>Müşteri kesimine göre kurumsal bayi performansı

Bu görünüm, bir iş ortağının çeşitli müşteri segmentlerine göre bölünmüş aylık gelir abd doları eğilimini, abonelik ve lisans sayısını anlayabilir. Grafikte ilk beş müşteri segmenti gösterilir ve kalan segmentler 'Diğer' kategorisine ayrılmıştır.

:::image type="content" source="images/insights/resellers-performance-customer-segment.png" alt-text="Müşteri kesimine göre bayi performansı.":::

## <a name="reseller-mpa-signing-status"></a>Kurumsal Bayi MPA imzalama durumu

Bu görünüm, kurumsal bayiler için MPA imzalama durumunun yanı sıra Microsoft İş Ortağı Ağı (MPN) yoklama durumu ve Geçiş durumu için Partner Membership Center (PMC) İş Ortağı Merkezi sağlar.

:::image type="content" source="images/insights/resellers-performance-mpa-status.png" alt-text="Kurumsal Bayi MPA imzalama durumu.":::

## <a name="next-steps"></a>Sonraki adımlar

- Daha fazla rapor için [bkz. İş Ortağı Merkezi Analizler.](partner-center-insights.md)

>[!NOTE] 
> Bu raporu güçlü bir şekilde kullanarak ham verileri panonun Raporları İndir bölümünden Analizler indirebilirsiniz. [Daha Fazla Bilgi](insights-download-reports.md) 
