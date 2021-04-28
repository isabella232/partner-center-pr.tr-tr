---
title: Referans içgörüleri alma
ms.topic: article
ms.date: 02/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: İş hedeflerinize ulaşmanıza yardımcı olacak bilgi veya geliştirme alanı eğilimlerini görmek için, iş ortağı merkezi 'nde başvuru öngörülerinizi düzenli olarak gözden geçirin.
author: rajap-ms
ms.author: rajap
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 4a8227fecae05d3752d65651dea4cdc62c9ea672
ms.sourcegitcommit: 078eac1456f68585ff1003b21e5e1fe777af314b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/28/2021
ms.locfileid: "108120860"
---
# <a name="get-referral-insights-in-partner-center-and-find-out-how-your-referrals-are-doing"></a>Iş Ortağı Merkezi 'nde başvuru öngörülerini alın ve başvurularınızın nasıl çalıştığını öğrenin

**Uygun roller**

- Başvuru Yöneticisi

Başvurularda **analiz** bölümünün altındaki **ortak satış fırsatları** sayfası, başvurularınızın nasıl çalıştığını görmenizi sağlar. Dikkat edilmesi gereken eğilimleri veya alanı belirlemek için bu ölçümleri düzenli olarak gözden geçirin ve iş hedeflerinize doğru bir şekilde sürüyi başlatın.

Ortak satış fırsatları öngörülerinizi görmek için Iş Ortağı Merkezi menüsünden **referanslar > analiz > ortak satış fırsatları**' na gidin.

> [!Important]
> Anlaşma türü filtresi, tüm veriler için seçilen **ortak satış** türüyle önceden uygulandı. Özel ve iş ortağı tarafından yapılan anlaşmalar ile ilgili verileri anlayze istiyorsanız filtreyi kaldırın.

## <a name="apply-filters"></a>Filtreleri uygulama

**Ortak satış fırsatları** sayfasının üst kısmında, verileri göstermek istediğiniz zaman dilimini seçebilirsiniz. Varsayılan seçim **3Dk** 'dir (üç ay), ancak bunun yerine altı ay veya bir yıl boyunca verileri göstermeyi tercih edebilirsiniz. Ayrıca, belirli bir dönemdeki tüm başvuruların verilerini görmek için **özel** ' i de seçebilirsiniz.

Bu sayfadaki tüm verileri müşteri adı, ülke, anlaşma türü, anlaşma yönü, çözüm adı ve durum ile filtrelemenizi sağlayan paneli açmak için **Filtreler** düğmesini seçebilirsiniz. Bu filtrelerin ayrıntıları aşağıda verilmiştir.

- **Müşteri adı**: **Tümü** varsayılandır, ancak verileri seçtiğiniz bir veya daha fazla müşteriyle sınırlayabilirsiniz.
- Ülke: **Tümü** varsayılandır, ancak verileri seçtiğiniz bir veya daha fazla müşterinin bir veya daha fazla **ülkesine** sınırlayabilirsiniz.
- **Anlaşma türü**: varsayılan, **ortak satışdır** , ancak seçiminize göre verileri özel veya iş ortağı olarak sınırlayabilirsiniz.
- **Anlaşma yönü** Varsayılan değer **Tümü**' dir, ancak verileri **gelen** başvuruların (aldığınız olanlar) veya **giden** başvuruların (gönderdiğiniz) sınırlarını seçebilirsiniz.
- **Çözüm adı**: **Tümü** varsayılandır, ancak verileri seçtiğiniz bir veya daha fazla çözümü içeren başvurularda sınırlamayı tercih edebilirsiniz.
- **Durum**: **Tümü** varsayılandır, ancak verileri oluşturulan, kabul edilen, reddedilen, süresi biten, kaybolan ve kazanıldı gibi bir veya daha fazla başvuru durum türü içeren başvurularda sınırlamayı tercih edebilirsiniz.

Aşağıda belirtilen grafiklerin tümünde bulunan bilgiler, aşağıda belirtilenler dışında, tarih aralığını ve seçtiğiniz filtreleri yansıtır. Bazı bölümler, belirli bir çözüme filtreleme gibi ek filtreler uygulamanıza da imkan tanır.

## <a name="referrals-summary"></a>Başvurular Özeti

Bu kartta, ortak satış fırsatlarınızın nasıl yaptığına ilişkin bir genel bakış sunulmaktadır.

Grafik, seçilen dönem için toplam anlaşmalar sayısını, kazanılan numarayı, kaybedilen sayıyı ve toplam anlaşma hacmini (USD cinsinden) gösterir.

Yüzde değişiklik ölçümleri (kırmızı veya yeşil renkle gösterilir, ok göstergesi ile), **Seçilen tarih aralığındaki son tam ay** ve **Bu aralıktaki ilk tam ay** arasındaki farkı gösterir. Örneğin, geçerli tarih 15 Haziran ve son üç aya ait verileri göstermek için **3D** filtresini seçtiğinizi varsayalım. Bu durumda, bu ölçümler, Mayıs (seçili zaman aralığındaki son tam ay) ve Mart (seçili dönemdeki ilk tam ay) arasındaki farkı gösterir. Seçili tarih aralığı son **3H** ise, karşılaştırma için veriler ve Mart verileri arasında olur.

:::image type="content" source="images/referrals/cosellanalyticssummary.png" alt-text="Ortak satış fırsatları analizinin Özet kartını gösteren resim.":::

## <a name="conversion-funnel"></a>Dönüştürme huni

Bu bölümde, anlaşmaların yaşam döngüsü boyunca bir durumdan diğerine nasıl geçilerek ilgili görsel bir gösterge gösterilmektedir. Bu bölümün ana özetine bağlı olarak, tüm yaşam döngüsünü, işlem hacmine ve ABD Doları cinsinden anlaşma değerine göre görüntüleyebilirsiniz. İlk bölüm her ikisi de durum ve türe göre birim ya da değer için bir görsel gösterge sağlamak için anlaşma türüyle etiketlidir. Ayrıca, **geçmişteki bir başvuru** da vardır ve bu, bu işlemleri kabul ediyor/reddediliyor veya rapor için seçili olan süre içinde kazanıldı/kaybedildi olarak işaretleme eylemi gerçekleştirmiş olan anlaşmaları göstermek için kullanılır. Tüm yaşam döngülerinde çeşitli aşamalardaki anlaşmalar ilerlemesini görüntülemek için filtreler uygulayabilirsiniz.

Ortak satış gelen anlaşmalar, iş ortaklarının gelen ortak satış anlaşmaları kabul etmesi veya reddetmesi için kabul edilebilir, reddedildi veya sona ermemiş olarak birleştirilemez.

:::image type="content" source="images/referrals/inbound.png" alt-text="Gelen başvuruların durumlarını gösteren resim.":::

İş ortakları tarafından bu tür anlaşmalar oluşturulduğu için iş ortağı LED, özel ve ortak satış giden anlaşmaları oluşturulacak şekilde birleştirilir.

:::image type="content" source="images/referrals/outbound.png" alt-text="Giden başvuruların durumlarını gösteren resim.":::

:::image type="content" source="images/referrals/cosell-analytics-funnel-v2.png" alt-text="Başvurular için dönüştürme huni gösteren resim.":::

## <a name="deals-by-geography"></a>Coğrafya ile anlaşmalar

Bu bölümde, her bir ülke/bölge ile ilgili ayrıntıların yanı bilgi verilen anlaşmalar/bölgeler gösterilir. Her ülkenin işlem ayrıntılarının, tüm ülkelerin harita görünümüyle birlikte bir tablo görünümü vardır. Tablodaki belirli bir ülkeyi seçebilir veya belirli bir ülkeyi yakınlaştırmak için harita görünümünü seçebilirsiniz.

:::image type="content" source="images/referrals/cosell-analytics-geo-distribution-v2.png" alt-text="Başvuruların coğrafi dağılımını gösteren resim.":::

## <a name="deals-by-solutions"></a>Çözümlere göre anlaşmalar

Bu grafik, en fazla başvuruları ve en yüksek anlaşma değerini hangi çözümlerinizin yönlendirdiğini görmenizi sağlar. Tabloda üç Özette, ortak satış, iş ortağı ve özel olmak üzere üç özet vardır.
Özet seçiminize bağlı olarak, çözüme göre toplanan anlaşmalar performansını görebilirsiniz.

> [!NOTE]
> Bir anlaşma için birden çok çözüm varsa, tablo tüm bu çözümlere karşı sayılan aynı anlaşmayı gösterir. Çözümlerle ilgili değerleri eklememelisiniz ve diğer başvuru birimi ölçümleriyle karşılaştırmamalıdır. Bu görünüm çözüm özeti ile anlaşma performansını anlamanıza yardımcı olmak için tasarlanmıştır.

Tabloda, çözüme dahil edilen toplam anlaşmalar ve kazanılan anlaşmalar, anlaşmalar kaybı, kaybedilen anlaşmalar ve ABD para birimi cinsinden kaybedilen anlaşmalar gibi ilgili durumlar bulunur. Ayrıca, toplam anlaşmalar sayısını gösteren tablo sağında bir anlaşmalar eğilimi grafiği ve seçilen çözüme bağlı olarak ABD Doları para biriminde kazanılan anlaşma değeri mevcuttur. Varsayılan seçim tüm çözümlerdir.

:::image type="content" source="images/referrals/cosell-analytics-solutions-v2.png" alt-text="Çözüm performansını gösteren resim.":::

## <a name="declined--lost-reasons"></a>& kayıp nedeni reddedildi

Bu bölüm, anlaşmanızın şirketiniz tarafından **reddedildi** veya **kaybedilir** olarak işaretlenme nedenlerini analiz etmenize yardımcı olur. Bu temsiller içindeki seçenekler, satıcılarınızın reddettiği veya kaybolduğu sürece, satıcılarınızın seçtiği nedenlerdir.

:::image type="content" source="images/referrals/cosellanalyticsreasons.png" alt-text="Reddetme veya kayıp olarak bir anlaşma yaparken iş ortağı tarafından seçilen nedenleri gösteren resim.":::

## <a name="comparison-charts"></a>Karşılaştırma grafikleri

Karşılaştırma bölümü, her ikisi de birimdeki birden çok boyut ve ABD Doları Özeti kazanılan anlaşmalar değeri temelinde başvurularıyla ilgili verileri karşılaştırmanıza yardımcı olur.
Verileri karşılaştırmak için seçebileceğiniz üç boyut

- Anlaşma türü
- Pazar
- Çözümler

Anlaşma türü seçildiğinde, başvuru performansını ortak satış fırsatları, iş ortağı ve özel anlaşmalar açısından karşılaştırabilirsiniz. Hem pazarlar hem de çözümler için performanslarını karşılaştırmak üzere üç farklı seçenek belirleyebilirsiniz. Bir çubuk grafik olan ilk grafikte, hacim veya anlaşmalar değeri kazanılan ana özete göre ayda ay eğilimi ile sunulan veriler bulunur. Ayrıca, çubuk grafiğin sağında aynı veriler için dağılımı yüzde olarak gösteren bir pasta grafiği de vardır.

:::image type="content" source="images/referrals/cosell-analytics-compare-v2.png" alt-text="Karşılaştırma bölümünü gösteren resim.":::

## <a name="raw-data-table"></a>Ham veri tablosu

Ortak satış fırsatlarıyla ilgili tüm ham verilerin bulunduğu aşağıdaki tablo, gerçekleştirmek istediğiniz ayrıntılı veya özel analizin için verileri hızlı bir şekilde **dışa aktarmaya** yardımcı olur.

:::image type="content" source="images/referrals/cosellanalyticsrawdata.png" alt-text="Başvurular için ham veri tablosunu gösteren resim.":::

## <a name="no-data"></a>Veri yok

Aşağıda açıklandığı gibi ortak satış analizlerine erişirken aşağıdaki gibi boş bir grafik almanızı sağlayabilirsiniz.

- Bu hesap için veri yok. Bu raporun doldurulduğu anlaşmalar oluşturmayı deneyin.
- Bazı ağ bağlantısı sorunu var. İnternet bağlantınızı denetleyip yeniden deneyin.
- Sayfa, ortak satış anlaşmaları için varsayılan filtreyle yüklenir. Yalnızca özel anlaşmalar varsa, anlaşma türü filtresini sıfırlayın.
- Uyguladığınız filtrelerle eşleşen bir kayıt yok. Filtreleri sıfırlamayı deneyin.
- Fırsat durumu değişikliği ve analiz raporunda aynı şekilde güncelleştirileceği bir gecikme vardır. 24 saat sonra raporu kontrol edin.

:::image type="content" source="images/referrals/nodata.png" alt-text="Başvurular için veri görselleştirmesi olmadığını gösteren resim.":::

> [!NOTE]
> **Referanslar** içgörü sayfasında yalnızca İş Ortağı Merkezi'nde oluşturulan tavsiyelere ait veriler gösteriliyor. [Iş ortağı satış bağlantısı](psc-to-pc.md) veya diğer mekanizmalarla oluşturulan başvuruların verilerini göstermez.

> [!TIP]
> [Bir çözüm sağlayıcısı bulma](https://www.microsoft.com/solution-providers/home) deneyiminde iş profilinizin nasıl çalıştığını görmek için [iş profili öngörüleri sayfasını](analyze-your-marketing-profile.md)gözden geçirin.
