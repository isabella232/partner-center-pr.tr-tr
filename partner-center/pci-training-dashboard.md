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
ms.openlocfilehash: e3beb1d051d2407229deebbb94b938a8f8b7218e
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854562"
---
# <a name="trainings-dashboard"></a>Çekim panosu

**Uygun roller**: Executive rapor Görüntüleyici | Rapor Görüntüleyicisi

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
- **Sınavları olan bireyler:** şirketiniz içinde sınav kimlik bilgilerine sahip olan ayrı bireylerin sayısını temsil eder. 
- **Sınav sayısı:** Şirketinizin bireyleri tarafından yapılan toplam sınav sayısını temsil eder.

## <a name="training-performance"></a>Eğitim performansı

Eğitim performansı, aylık kişi sayısını ve şirketinizin bireyler tarafından tamamlanan eğitimlerini sunar. Seçilen tarih aralığı için grafik şeklinde sertifikalara, değerlendirmelere ve sınavlara göre ayrılır. X ekseni, seçilen tarih aralığı için ayları temsil eder. Y ekseni, seçilen eğitim türü için ayrı kişi sayısını ve alınan eğitim sayısını temsil eder. Dökümü eğitim türüne göre görüntülemek için grafiğin üzerindeki ilgili sekmeleri seçin. Grafik verileri, seçilen tarih aralığı için .tsv biçimindeki indirme simgesi aracılığıyla indirilebilir.

:::image type="content" source="images/pci/td-training-performance.png" alt-text="Eğitim Performansı":::

## <a name="individuals-performance"></a>Kişilerin performansı

Kişiler'in performans bölümünde, seçilen tarih aralığı için şirketiniz içinde yer alan kişiler tarafından alınan eğitimin ayrıntıları yer almaktadır. Bölümün sol panelinde bir kişinin adını arama ve seçme. Seçilen kişiye ilişkin eğitim ayrıntıları, bölümün sağ panelinde görüntülenir.

:::image type="content" source="images/pci/td-indiviual-performance.png" alt-text="Gerçek Performans":::

>[!NOTE] 
> Bireysel performans bölümü yalnızca yönetici rapor görüntüleyicisi olan kullanıcılar tarafından kullanılabilir. 

## <a name="next-steps"></a>Sonraki Adımlar

[İş Ortağı Merkezi Insights'ta raporlar](partner-center-insights.md)

>[!NOTE] 
> Bu raporu güçlü bir şekilde kullanarak ham verileri Öngörüler panosunun Raporları İndir bölümünden indirebilirsiniz. [Daha Fazla Bilgi](pci-download-reports.md)