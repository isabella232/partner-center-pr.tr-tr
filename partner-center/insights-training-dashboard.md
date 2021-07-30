---
title: Analizler Eğitim Panosu
ms.topic: article
ms.date: 06/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Eğitim İş Ortağı Merkezi'i keşfedin. Eğitim, İş Ortağı Merkezi Analizler (PCI) alanında bulunan raporlardan birisidir.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8749bdc1c2249f97d5db288f953eded1c4c06b02
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114843179"
---
# <a name="trainings-dashboard"></a>Eğitimler panosu

**Uygun roller:** Yönetici rapor görüntüleyicisi | Rapor görüntüleyicisi

Eğitimler panosu, şirket çalışanları şirketi tarafından alınan sertifikalar, değerlendirmeler ve incelemeler hakkında içgörüler sağlar. Eğitimler panosu aşağıdaki bölümleri içerir:

- Özet
- Eğitim Performansı sertifikalara, değerlendirmelere, sınavlara göre bölündü
- Sertifikalar, değerlendirmeler, sınavlar gibi kimlik bilgilerine göre bireyler
- Etkinlik ayrıntıları

>[!NOTE] 
>Bu rapor, Analizler hub' İş Ortağı Merkezi. Bu raporu görüntülemek için Size Rapor görüntüleyicisi veya Yönetici rapor görüntüleyicisi rolü atanmalı. Bu raporun birkaç bölümü yalnızca Yönetici Rapor Görüntüleyicisi olan kullanıcılar tarafından görülebilir. Raporlarda erişim denetimi hakkında daha fazla bilgi Analizler bkz. [PCI rolleri.](insights-roles.md)

## <a name="summary"></a>Özet

Özet bölümü, eğitimlerinize ilişkin çeşitli performans göstergelerinin sayısal bir anlık görüntü görünümünü sunar. Çeşitli performans göstergeleri Sertifikalı Bireyler, Sertifikalar, Sınav Kimlik Bilgilerine Sahip Bireyler, Sınav Kimlik Bilgileri, Değerlendirme Kimlik Bilgilerine sahip Bireyler ve Değerlendirme Kimlik Bilgileridir. Bu bölümdeki veriler seçilen tarih aralığına göre yenilenir. Bu aralık üç ay (3 milyon), altı ay (6 milyon) ve 12 ay (1Y) veya özel veri aralığı (Özel) olabilir. 

:::image type="content" source="images/insights/training-dashboard-summary.png" alt-text="Özet.":::

- **Sertifikalara sahip kişiler:** Şirketiniz içinde sertifikalara sahip olan ayrı bireylerin sayısını temsil eder.
- **Sertifikasyon sayısı:** Şirketiniz içinde yer alan kişilerin toplam sertifika sayısını temsil eder.
- **Değerlendirmeleri olan bireyler:** şirketinizin değerlendirme kimlik bilgilerine sahip olan ayrı bireylerin sayısını temsil eder. 
- **Değerlendirme sayısı:** şirketinizin bireyleri tarafından yapılan toplam değerlendirme sayısını temsil eder.
- **Sınavları olan bireyler:** Şirketiniz içinde sınav kimlik bilgilerine sahip olan ayrı bireylerin sayısını temsil eder. 
- **Sınav sayısı:** Şirketinizin bireyleri tarafından yapılan toplam sınav sayısını temsil eder.

## <a name="training-performance"></a>Eğitim performansı

Eğitim performansı, aylık kişi sayısını ve şirketinizin bireyler tarafından tamamlanan eğitimlerini sunar. Seçilen tarih aralığı için grafik şeklinde sertifikalara, değerlendirmelere ve sınavlara göre ayrılır. X ekseni, seçilen tarih aralığı için ayları temsil eder. Y ekseni, seçilen eğitim türü için ayrı kişi sayısını ve alınan eğitim sayısını temsil eder. Dökümü eğitim türüne göre görüntülemek için grafiğin üzerindeki ilgili sekmeleri seçin. Grafik verileri, seçilen tarih aralığı için .tsv biçimindeki indirme simgesi aracılığıyla indirilebilir.

:::image type="content" source="images/insights/training-dashboard-training-performance.png" alt-text="Eğitim Performansı.":::

## <a name="individuals-performance"></a>Kişilerin performansı

Kişiler'in performans bölümünde, seçilen tarih aralığı için şirketiniz içinde yer alan kişiler tarafından alınan eğitimin ayrıntıları yer almaktadır. Bölümün sol panelinde bir kişinin adını arama ve seçme. Seçilen kişiye ilişkin eğitim ayrıntıları, bölümün sağ panelinde görüntülenir.

:::image type="content" source="images/insights/training-dashboard-individual-performance.png" alt-text="Bireysel Performans.":::

>[!NOTE] 
> Bireysel performans bölümü yalnızca yönetici rapor görüntüleyicisi olan kullanıcılar tarafından kullanılabilir. 

## <a name="next-steps"></a>Sonraki Adımlar

[Raporlarda İş Ortağı Merkezi Analizler](partner-center-insights.md)

>[!NOTE] 
> Bu raporu güçlü bir şekilde kullanarak ham verileri panonun Raporları İndir bölümünden Analizler indirebilirsiniz. [Daha Fazla Bilgi](insights-download-reports.md)