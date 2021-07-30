---
title: İş Ortağı Merkezi Analizler Azure kullanım raporunu kullanma
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: İyi işlerinizi ve müşterileriniz için satış veya yönetim için azure aboneliklerini kullanımınızı geliştirebilirsiniz.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 75f326fab8ebc59628dadc43b048dfefe48c22cb
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114843995"
---
# <a name="azure-usage-report-available-from-the-partner-center-insights-dashboard"></a>Azure Kullanım raporu, İş Ortağı Merkezi Analizler panosundan kullanılabilir

**Uygun roller:** Genel yönetici | Yönetici aracısı | Rapor görüntüleyici | Yönetici raporu görüntüleyicisi

Azure Kullanım raporu, müşterinizin Azure abonelikleri ile ilgili ölçümleri sunar. Bu rapor, ölçüm kategorilerine göre Azure tüketim gelirini ve kullanımını içerir. Aşağıdaki bölümleri Azure Kullanım raporundan görüntüebilirsiniz.

- Özet
- Coğrafyaya göre Azure kullanımı
- Azure kullanımı

 > [!NOTE]
 > Bu rapor, Analizler kullanılabilir. Bu raporu görüntülemek için Genel Yönetici, Hesap Yöneticisi, Rapor Görüntüleyicisi İş Ortağı Merkezi Yönetici Rapor Görüntüleyicisi gibi belirli bir rol atanmış olması gerekir. Daha fazla bilgi için, bkz. şirketinizin Genel Yöneticisi. Bu rapora özgü veri türleri yalnızca Yönetici Rapor Görüntüleyicisi ayrıcalıklarına sahip kullanıcılar tarafından da kullanılabilir.

## <a name="summary"></a>Özet

Özet bölümünde, müşterileriniz için sizin tarafından satılan veya yönetilen Azure abonelikleri ile ilgili ana performans göstergelerinin (KIP' ler) anlık görüntüsü yer alır.  

- Azure Abonelikleri: Sizin sattığınız veya sizin tarafından yönetilen Azure müşteri aboneliklerinin geçerli sayısı.
Seçilen tarih aralığında bu Azure aboneliklerinin büyüme veya reddetme yüzdesi.

Mikro grafik, seçtiğiniz tarih aralığı için aylık Azure abonelik sayısı eğilimini gösterir.
- Etkin Azure Abonelikleri: Son 30 gün içinde etkin kullanımı olan ve sizin tarafından satılan veya yönetilen Azure aboneliklerinin geçerli sayısı.
Bu aboneliklerin seçilen tarih aralığındaki büyüme veya düşüş yüzdesi.

Mikro grafik, seçtiğiniz tarih aralığı boyunca Azure etkin abonelik sayısına göre aylık eğilimi gösterir.

- Azure Tüketim Geliri (ACR): Azure Tüketim Geliri tarih aralığı üzerinden size atfedilen toplam değer (US$).
Seçilen tarih aralığında öznitelikli ACR US$ artışı veya reddetme yüzdesi. 

Mikro grafik, seçili zaman dönemi boyunca size atfedilen aylık ACR US$ eğilimini gösterir


> [!NOTE]
 > Azure Tüketim Geliri (ACR) yalnızca Yönetici Rapor Görüntüleyicisi Rolü atanmış kullanıcılara görünür.

:::image type="content" source="images/insights/azure-usage-summary.png" alt-text="Azure kullanım özeti.":::

## <a name="azure-usage-by-geography"></a>Coğrafyaya göre Azure kullanımı

Coğrafyaya göre Azure kullanımı **görünümü,** Tüm veya seçili Azure hizmet düzeyi/ölçüm kategorileri için Azure tüketim gelirinin (ACR US$) coğrafi dağılımını veya kullanım saatlerini gösterir. Harita üzerinde daha açık renkler düşük değerleri, koyu renkler ise daha yüksek değerleri temsil eder. Yakınlaştırmak için kılavuzda bir ülke arayabilir ve bu ülkeyi 

**Ülke/bölge sayısı tablosu,** Azure kullanım olaylarının oluşturularak toplam ülke/bölge sayısını gösterir.

Haritanın konumunu yakınlaştırmak için kılavuzda bir ülke arayabilir ve bu ülkeyi seçin. Özgün **görünüme** dönmek için haritada Giriş seçeneğini belirleyin.

:::image type="content" source="images/insights/azure-usage-by-geography.png" alt-text="Coğrafyaya göre Azure kullanımı.":::

## <a name="azure-utilization"></a>Azure kullanımı

Bu görünümde, seçili Azure hizmet düzeyi/ölçüm kategorilerine göre aylık Azure tüketim geliri veya kullanım saati eğilimleri görüntülenir. 

Çubuk grafik, aylık gelir/kullanım saati eğilimini gösterir. Çizgi grafik, seçilen Azure hizmet düzeyi/ölçüm kategorileri için önceki aya göre büyüme eğilimini gösterir.

:::image type="content" source="images/insights/azure-usage-utilization.png" alt-text="Azure kullanımı.":::

## <a name="next-steps"></a>Sonraki adımlar

- Daha fazla rapor için [bkz. İş Ortağı Merkezi Analizler.](partner-center-insights.md)

>[!NOTE] 
> Bu raporu güçlü bir şekilde kullanarak ham verileri panonun Raporları İndir bölümünden Analizler indirebilirsiniz. [Daha Fazla Bilgi](insights-download-reports.md) 
