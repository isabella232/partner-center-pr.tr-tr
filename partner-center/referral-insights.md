---
title: Referans içgörüleri alma
ms.topic: article
ms.date: 04/30/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: İş hedeflerinize ulaşmanıza yardımcı olacak adres veya İş Ortağı Merkezi eğilimlerini görmek için referans içgörüleri verilerinizi düzenli aralıklarla gözden geçirme.
author: rajap-ms
ms.author: rajap
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: b1bb86a493ce81cb02b14c9555f82767d10f841c
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855957"
---
# <a name="get-referral-insights-in-partner-center-and-find-out-how-your-referrals-are-doing"></a>Referans içgörülerini İş Ortağı Merkezi ve referansların nasıl olduğunu öğrenin

**Uygun roller:** Referans yöneticisi

Referanslar **bölümündeki Analiz** bölümünün **altındaki** Ortak satış fırsatları sayfası, referansların nasıl olduğunu görmenizi sağlar. Dikkat gereken eğilimleri veya alanları belirlemek için bu ölçümleri düzenli olarak gözden geçirin ve iş hedeflerinize doğru ilerlenin.

Ortak satış fırsatları içgörü verilerinizi görmek için İş Ortağı Merkezi menüsünden Referanslar > **Analytics > Ortak Satış Fırsatları'ne gidin.**

> [!Important]
> Anlaşma türü filtresi, tüm veriler için **Ortak satış** türü seçili olarak önceden uygulanır. Özel ve iş ortağı tarafından yönlendirilen anlaşmalarla ilgili verileri analiz etmek için filtreyi kaldırın.

## <a name="apply-filters"></a>Filtreleri uygulama

Ortak satış fırsatları **sayfasının üst kısmında,** verileri göstermek istediğiniz zaman dönemini seçin. Varsayılan seçim **3 milyon** (üç ay) olur, ancak bunun yerine altı ay veya bir yıl için verileri göstermeyi seçebilirsiniz. Belirli bir zaman **dönemi içinde tüm** referanslara yönelik verileri görmek için Özel'i de kullanabilirsiniz.

Bu sayfadaki **tüm verileri** Müşteri adı, Ülke, Satış türü, Satış yönü, Çözüm adı ve Durum'a göre filtrelemenizi sağlayan paneli açmak için Filtreler düğmesini seçebilirsiniz. Bu filtrelerin ayrıntıları aşağıda verilmiştir.

- **Müşteri adı:** Varsayılan değer **All**'tir, ancak verileri, seçerek bir veya daha fazla müşteriyle sınırabilirsiniz.
- **Ülke:** Varsayılan **değer All**'tir, ancak verileri, sizin seçerek müşterinin bir veya daha fazla ülkesiyle sınırlandırabilirsiniz.
- **Satış türü:** Varsayılan **değer** Ortak satış'tır ancak Seçiminize bağlı olarak Tüm'i seçerek veya verileri Özel veya İş Ortağı tarafından yönlendirilen satış anlaşmaları ile sınırlandırabilirsiniz.
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

Bu bölümde, anlaşmaların yaşam döngüsü boyunca bir durumdan diğerine nasıl geçilerek ilgili görsel bir gösterge gösterilmektedir. Yaşam döngüsünün tamamını, bu bölümün ana özet bölümüne göre satış hacmine ve ABD doları değerindeki satış anlaşması değerine göre görüntüebilirsiniz. İlk bölüm, birimin veya değerin türüne göre görsel bir göstergesini vermek için hem durum hem de satış anlaşması türü ile etiketlenmiş. Ayrıca, bunları kabul etme/gerileme veya rapor için seçilen zaman dönemi içinde kazanildi/kaybedildi olarak işaretleme eylemini gerçekleştirmiş olduğu anlaşmaları belirtmek için kullanılan, geçmişteki Referanslar bölümü de vardır. Anlaşmaların yaşam döngülerinin çeşitli aşamalarındaki ilerlemesini görüntülemek için filtreler uygulayabilirsiniz.

Ortak satış gelen satış anlaşmaları, iş ortaklarının gelen ortak satış anlaşmalarını Kabul Etmek veya Reddetmek zorunda olduğu için Kabul Edildi, Reddedildi veya Süresi Doldu olarak birleşebilirsiniz.

:::image type="content" source="images/referrals/inbound.png" alt-text="Gelen referansların durumları gösteren resim.":::

İş ortağı tarafından yönlendirilecek, Özel ve Ortak satış giden satış anlaşmaları, Bu tür satış anlaşmaları İş Ortakları tarafından oluşturulduktan sonra Oluşturuldu olarak birleşiyor.

:::image type="content" source="images/referrals/outbound.png" alt-text="Giden referansların eyaletlerini gösteren resim.":::

:::image type="content" source="images/referrals/cosell-analytics-funnel-v2.png" alt-text="Referanslar için dönüştürme hunisi gösteren resim.":::

## <a name="deals-by-geography"></a>Coğrafyaya göre anlaşmalar

Bu bölümde anlaşmaların geldiği ülkeler/bölgeler ve her ülke/bölgeye ilişkin ayrıntılar yer almaktadır. Her ülke için anlaşma ayrıntılarının tablo görünümü ve tüm ülkelerin harita görünümü vardır. Tabloda belirli bir ülkeyi veya harita görünümünü seçerek belirli bir ülkeyi yakınlaştırabilirsiniz.

:::image type="content" source="images/referrals/cosell-analytics-geo-distribution-v2.png" alt-text="Referansların coğrafi dağılımını gösteren resim.":::

## <a name="deals-by-solutions"></a>Çözümlere göre anlaşmalar

Bu grafik, çözümlerinizin hangilerinin en çok referans ve en yüksek anlaşma değerine sahip olduğunu görmenizi sağlar. Tabloda üç özet vardır: Ortak satış, İş ortağı liderliğinde ve Özel.
Özet seçiminize bağlı olarak, çözüme göre toplu anlaşmaların performansını görebilir.

> [!NOTE]
> Bir anlaşmaya birden çok çözüm dahil edilirse tabloda tüm bu çözümler için aynı anlaşma sayısı göstereceğiz. Çözümlerle ilgili değerleri eklemeli ve diğer referans hacmi ölçümleriyle karşılaştırmamalısınız. Bu görünüm çözüm özeti ile anlaşma performansını anlamanıza yardımcı olmak için tasarlanmıştır.

Tabloda, çözüme dahil edilen toplam anlaşmalar ve kazanılan anlaşmalar, anlaşmalar kaybı, kaybedilen anlaşmalar ve ABD para birimi cinsinden kaybedilen anlaşmalar gibi ilgili durumlar bulunur. Ayrıca, toplam anlaşmalar sayısını gösteren tablo sağında bir anlaşmalar eğilimi grafiği ve seçilen çözüme bağlı olarak ABD Doları para biriminde kazanılan anlaşma değeri mevcuttur. Varsayılan seçim tüm çözümlerdir.

:::image type="content" source="images/referrals/cosell-analytics-solutions-v2.png" alt-text="Çözüm performansını gösteren resim.":::

## <a name="declined--lost-reasons"></a>& kayıp nedeni reddedildi

Bu bölüm, anlaşmanızın şirketiniz tarafından **reddedildi** veya **kaybedilir** olarak işaretlenme nedenlerini analiz etmenize yardımcı olur. Bu temsiller içindeki seçenekler, satıcılarınızın reddettiği veya kaybolduğu sürece, satıcılarınızın seçtiği nedenlerdir.

:::image type="content" source="images/referrals/cosellanalyticsreasons.png" alt-text="Reddetme veya kayıp olarak bir anlaşma yaparken iş ortağı tarafından seçilen nedenleri gösteren resim.":::

## <a name="comparison-charts"></a>Karşılaştırma grafikleri

Karşılaştırma bölümü, her ikisi de birimdeki birden çok boyut ve ABD Doları Özeti kazanılan anlaşmalar değeri temelinde başvurularıyla ilgili verileri karşılaştırmanıza yardımcı olur. Verileri karşılaştırmak için seçebileceğiniz üç boyut şunlardır:

- Anlaşma türü
- Pazar
- Çözümler

Anlaşma türü seçildiğinde, başvuru performansını ortak satış fırsatları, Iş ortağı ve özel anlaşmalar açısından karşılaştırabilirsiniz. Hem pazarlar hem de çözümler için performanslarını karşılaştırmak üzere üç farklı seçenek belirleyebilirsiniz. Bir çubuk grafik olan ilk grafikte, hacim veya anlaşmalar değeri kazanılan ana özete göre ayda ay eğilimi ile sunulan veriler bulunur. Ayrıca, çubuk grafiğin sağında aynı veriler için dağılımı yüzde olarak gösteren bir pasta grafiği de vardır.

:::image type="content" source="images/referrals/cosell-analytics-compare-v2.png" alt-text="Karşılaştırma bölümünü gösteren resim.":::

## <a name="raw-data-table"></a>Ham veri tablosu

Ortak satış fırsatlarıyla ilgili tüm ham veriler aşağıdaki tabloda, gerçekleştirmek  istediğiniz ayrıntılı veya özel analizler için verileri hızla dışarı aktarmanıza yardımcı olacaktır.

:::image type="content" source="images/referrals/cosellanalyticsrawdata.png" alt-text="Referanslar için ham veri tablosu gösteren resim.":::

## <a name="no-data"></a>Veri yok

Aşağıda açıklandığı gibi Ortak satış analizine erişirken aşağıdaki gibi boş bir grafik elde edebilirsiniz.

- Bu hesap için veri yok. Bu raporun doldurulması için anlaşma oluşturmayı deneyin.
- Bazı ağ bağlantısı sorunları var. İnternet bağlantınızı kontrol edin ve yeniden deneyin.
- Sayfa, Ortak satış anlaşmaları için varsayılan filtreyle birlikte yüklenir. Yalnızca Özel anlaşmalar varsa anlaşma türü filtresini sıfırlayın.
- Uygulanan filtrelerle eşleşen kayıt yoktur. Filtreleri sıfırlamayı deneyin.
- Fırsat durumu değişikliği ile aynı değişikliğin analiz raporunda güncelleştirilmesinde bir gecikme vardır. 24 saat sonra raporu kontrol edin.

:::image type="content" source="images/referrals/nodata.png" alt-text="Referanslar için veri görselleştirmesi olmadığını gösteren resim.":::

> [!NOTE]
> **Referanslar** içgörü sayfasında yalnızca İş Ortağı Merkezi'nde oluşturulan tavsiyelere ait veriler gösteriliyor. İş Ortağı Satış Bağlantısı veya başka bir mekanizma aracılığıyla [oluşturulan referanslara](psc-to-pc.md) yönelik verileri göstermez.

> [!TIP]
> İş profilinizin nasıl bir çözüm sağlayıcısı deneyimi [bul'da](https://www.microsoft.com/solution-providers/home) nasıl performans sergile olduğunu görmek için İş profili [içgörüleri sayfasını gözden geçirebilirsiniz.](analyze-your-marketing-profile.md)

## <a name="next-steps"></a>Sonraki adımlar

- [Microsoft referansları ile işlerinizi büyütin](referrals.md)
- [Müşteri adaylarınızı analiz etme](analyze-your-marketing-profile.md)