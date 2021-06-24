---
title: Insights Eğitim Panosu
ms.topic: article
ms.date: 06/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Eğitim İş Ortağı Merkezi'i keşfedin. Eğitim, İş Ortağı Merkezi Insights (PCI) alanında bulunan raporlardan biri.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 37a4f6cdce2b77f194fc91e0490e1c87ee137b43
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565109"
---
# <a name="trainings-dashboard"></a>Eğitimler panosu

**Uygun roller:** Yönetici rapor görüntüleyicisi | Rapor görüntüleyicisi

Eğitimler panosu, şirket çalışanları şirketi tarafından alınan sertifikalar, değerlendirmeler ve incelemeler hakkında içgörüler sağlar. Eğitimler panosu aşağıdaki bölümleri içerir:

- Özet
- Eğitim Performansı sertifikalara, değerlendirmelere, sınavlara göre bölündü
- Sertifikalar, değerlendirmeler, sınavlar gibi kimlik bilgilerine göre kişiler
- Etkinlik ayrıntıları

>[!NOTE] 
>Bu rapor, İş Ortağı Merkezi'daki Insights merkezi altında İş Ortağı Merkezi. Bu raporu görüntülemek için Size Rapor görüntüleyicisi veya Yönetici rapor görüntüleyicisi rolü atanmalı. Bu raporun birkaç bölümü yalnızca Yönetici Rapor Görüntüleyicileri olan kullanıcılar tarafından görülebilir. Insights raporlarına yönelik erişim denetimi hakkında daha fazla bilgi için bkz. [PCI rolleri.](pci-roles.md)

## <a name="summary"></a>Özet

Özet bölümü, eğitimlerinize ilişkin çeşitli performans göstergelerinin sayısal bir anlık görüntü görünümünü sunar. Çeşitli performans göstergeleri Sertifikalı Bireyler, Sertifikalar, Sınav Kimlik Bilgilerine Sahip Bireyler, Sınav Kimlik Bilgileri, Değerlendirme Kimlik Bilgilerine sahip Bireyler ve Değerlendirme Kimlik Bilgileridir. Bu bölümdeki veriler seçilen tarih aralığına göre yenilenir. Bu aralık üç ay (3 milyon), altı ay (6 milyon) ve 12 ay (1Y) veya özel veri aralığı (Özel) olabilir. 

:::image type="content" source="images/pci/td-summary.png" alt-text="Özet.":::

- **Sertifikalara sahip kişiler:** Şirketiniz içinde sertifikalara sahip olan ayrı bireylerin sayısını temsil eder.
- **Sertifikasyon sayısı:** Şirketiniz içinde yer alan kişilerin ettiği toplam sertifika sayısını temsil eder.
- **Değerlendirmeleri olan bireyler:** şirketinizin değerlendirme kimlik bilgilerine sahip olan ayrı bireylerin sayısını temsil eder. 
- **Değerlendirme sayısı:** şirketinizin bireyleri tarafından yapılan toplam değerlendirme sayısını temsil eder.
- **Sınavları olan bireyler:** şirketiniz içinde sınav kimlik bilgilerine sahip olan ayrı bireylerin sayısını temsil eder. 
- **Sınav sayısı:** Şirketinizin bireyleri tarafından yapılan toplam sınav sayısını temsil eder.

## <a name="training-performance"></a>Eğitim performansı

Eğitim performansı, aylık kişi sayısını ve şirketinizin bireyler tarafından tamamlanan eğitimlerini sunar. Seçilen tarih aralığı için grafik şeklinde sertifikalara, değerlendirmelere ve sınavlara göre ayrılır. X ekseni, seçilen tarih aralığı için ayları temsil eder. Y ekseni, seçilen eğitim türü için ayrı kişi sayısını ve alınan eğitim sayısını temsil eder. Dökümü eğitim türüne göre görüntülemek için grafiğin üzerindeki ilgili sekmeleri seçin. Grafik verileri, seçilen tarih aralığı için .tsv biçimindeki indirme simgesi aracılığıyla indirilebilir.

:::image type="content" source="images/pci/td-training-performance.png" alt-text="Eğitim Performansı.":::

## <a name="individuals-performance"></a>Kişilerin performansı

Kişiler'in performans bölümünde, seçilen tarih aralığı için şirketiniz içinde yer alan kişiler tarafından alınan eğitimin ayrıntıları yer almaktadır. Bölümün sol panelinde bir kişinin adını arama ve seçme. Seçilen kişiye ilişkin eğitim ayrıntıları, bölümün sağ panelinde görüntülenir.

:::image type="content" source="images/pci/td-indiviual-performance.png" alt-text="Gerçek Performans.":::

>[!NOTE] 
> Kişiler performansı bölümü yalnızca yönetici rapor görüntüleyicisi olan kullanıcılar tarafından kullanılabilir. 

## <a name="next-steps"></a>Sonraki Adımlar

[İş Ortağı Merkezi Insights'ta raporlar](partner-center-insights.md)

>[!NOTE] 
> Bu raporu güçlü bir şekilde kullanarak ham verileri Öngörüler panosunun Raporları İndir bölümünden indirebilirsiniz. [Daha Fazla Bilgi](pci-download-reports.md)