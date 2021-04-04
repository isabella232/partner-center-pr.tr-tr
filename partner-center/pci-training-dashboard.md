---
title: Öngörüler Eğitim panosu
ms.topic: article
ms.date: 06/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Iş ortağı merkezi eğitim panosunu gezin. Eğitim, Partner Center Insights (PCI) alanında bulunan raporlardan biridir.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bad11a2f480aaa229708a3e9a108466a130b4127
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/31/2021
ms.locfileid: "106086252"
---
# <a name="trainings-dashboard"></a>Çekim panosu

**Uygun roller**

- Executive rapor Görüntüleyicisi
- Rapor Görüntüleyicisi

Seyahat panosu, şirket çalışanları şirketiniz tarafından gerçekleştirilen sertifikalar, değerlendirmeler ve Examinations hakkında öngörüler sağlar. Seyahat Panosu aşağıdaki bölümleri içerir:

- Özet
- Sertifikalarına, değerlendirmelere ve sınavlarına göre eğitim performansı
- Sertifikalar, değerlendirmeler, sınavlar gibi kimlik bilgilerine göre bireyler
- Etkinlik ayrıntıları

>[!NOTE] 
>Bu rapor, Iş Ortağı Merkezi 'nde Öngörüler hub 'ında bulunur. Bu raporu görüntülemek için, rapor Görüntüleyicisi veya Executive rapor Görüntüleyicisi rolü atanmalıdır. Bu raporun birkaç bölümü yalnızca Executive rapor Izleyicileri olan kullanıcılar için görünür olacaktır. Öngörüler raporları için erişim denetimi hakkında daha fazla bilgi için lütfen bkz. [PCI rolleri](pci-roles.md).

## <a name="summary"></a>Özet

Özet bölümü, taşmalarınız ile ilgili çeşitli performans göstergelerinin bir sayısal anlık görüntü görünümünü sunar. Çeşitli performans göstergeleri, sertifikalı bireyler, sertifikalardır, sınav kimlik bilgileri, sınav kimlik bilgileri, değerlendirme kimlik bilgileri ve değerlendirme kimlik bilgileri olan bireyler. Bu bölümdeki veriler, üç ay (3K), altı ay (6Dk) ve 12 ay (1Y) veya özel bir veri aralığı (özel) olabilen seçili tarih aralığına göre yenilenir. 

:::image type="content" source="images/pci/td-summary.png" alt-text="Özet":::

- **Sertifikalarla olan bireyler**: şirketinizde sertifikaları olan ayrı kişilerin sayısını temsil eder.
- Sertifika **sayısı**: şirketinizdeki bireyler tarafından alınan toplam sertifika sayısını temsil eder.
- **Değerlendirmelere sahip bireyler**: şirketinizde değerlendirme kimlik bilgilerine sahip benzersiz kişilerin sayısını temsil eder. 
- **Değerlendirme sayısı**: şirketinizdeki bireyler tarafından alınan toplam değerlendirme sayısını temsil eder.
- **Examinations Içeren bireyler**: şirketinizdeki kimlik bilgilerini inceleme ile ayrı kişilerin sayısını temsil eder. 
- **İnceleme sayısı**: şirketinizdeki bireyler tarafından alınan toplam Examinations sayısını temsil eder.

## <a name="training-performance"></a>Eğitim performansı

Eğitim performansı, şirket içi kişilerin ay sayısını ve şirketinizde tamamlanan kişileri gösterir. Bu, seçili tarih aralığı için bir grafik biçiminde sertifikalar, değerlendirmeler ve Sınavlar tarafından bölünür. X ekseni, seçili tarih aralığı için ayları temsil eder. Y ekseni, seçilen eğitim türü için farklı bireyler ve gerçekleştirilen seyahat sayısını temsil eder. Dökümü eğitim türüne göre görüntülemek için grafiğin üzerindeki ilgili sekmeleri seçin. Grafik verileri, seçilen tarih aralığı için. tsv biçimindeki indirme simgesiyle indirilebilir.

:::image type="content" source="images/pci/td-training-performance.png" alt-text="Eğitim performansı":::

## <a name="individuals-performance"></a>Bireysel kişilerin performansı

Kişilerin performans bölümü, şirketinizdeki bireyler tarafından seçilen tarih aralığı için alınan eğitimin ayrıntılarını sunar. Bölümün sol bölmesinde bir bireyin adı arayın ve seçin. Seçili bireyin için eğitim ayrıntıları bölümün sağ bölmesinde görüntülenir.

:::image type="content" source="images/pci/td-indiviual-performance.png" alt-text="Indiviual performansı":::

>[!NOTE] 
> Bireyler performans bölümü yalnızca Executive rapor izleyicileri olan kullanıcılar tarafından kullanılabilir. 

## <a name="next-steps"></a>Sonraki Adımlar

[Iş Ortağı Merkezi öngörüleri raporları](partner-center-insights.md)

>[!NOTE] 
> Bu raporu, Öngörüler panosundaki raporları Indir bölümünden elde eden ham verileri indirebilirsiniz. [Daha Fazla Bilgi](pci-download-reports.md)