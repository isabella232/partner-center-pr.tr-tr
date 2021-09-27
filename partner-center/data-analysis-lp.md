---
title: Abonelik öngörüleri için Analizi kullanma
ms.topic: article
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: İşletmenizi ve müşterilerinizin satın aldığınız lisansları nasıl kullandığını daha iyi anlamak için iş ortağı merkezi 'nde analizler kullanmayı öğrenin.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: aa7352277e241156884f6fda07f64cab5cb5b21a
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129073488"
---
# <a name="use-analytics-to-learn-more-about-subscription-revenue"></a>Abonelik geliri hakkında daha fazla bilgi edinmek için analiz kullanın

**Uygun roller**: genel yönetici | MPN iş ortağı Yöneticisi

CSP işinizi geliştirmenin yollarını planlarken müşterilerinizin Microsoft ürünlerini nasıl kullandığını anlamalısınız. İş Ortağı Merkezi 'nde veri toplamaya yönelik çeşitli seçenekleriniz vardır ve hem işiniz hem de müşterilerinizin satın aldıkları lisansları nasıl kullandığı hakkında veri toplayabilirsiniz. CSP doğrudan modelinde çalışıyorsanız, ek veri toplamak için Power BI için İş Ortağı Merkezi Analiz uygulaması yükleyip kullanabilirsiniz.

## <a name="access-to-the-subscription-analytics"></a>Abonelik analizinden erişim

> [!NOTE]
> Iş Ortağı Merkezi önizleme arabirimi, mantıksal olarak gruplanmış çalışma alanları aracılığıyla daha verimli ve üretken bir kullanıcı deneyimi sağlar. Çalışma alanları arabirimi ve nasıl kullanılacağı hakkında daha fazla bilgi edinmek için bkz. [Iş ortağı merkezini alma](get-around-partner-center.md#turn-workspaces-on-and-off).

#### <a name="workspaces-view"></a>[Çalışma alanları görünümü](#tab/workspaces-view)

1. iş ortağı merkezi [panosunda](https://partner.microsoft.com/dashboard/home)oturum açın ve **Analizler** kutucuğunu seçin.

2. **Çözümle**' yi ve ardından **abonelik Analizi**' ni seçin.

3. Son on iki aylık CSP geliri sayfanın en üstünde görüntülenir

#### <a name="current-view"></a>[Geçerli görünüm](#tab/current-view)

1. Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard/home)oturum açın.

2. Iş Ortağı Merkezi menüsünde **CSP** altında, **Çözümle**' yi seçin ve ardından **abonelik Analizi**' ni seçin.

3. Son on iki aylık CSP geliri sayfanın en üstünde görüntülenir

* * *

## <a name="trailing-twelve-month-ttm-csp-revenue"></a>Sondaki Twelve-Month (TTD) CSP geliri

son 12 aylık CSP gelir bir iş ortağı küresel hesap düzeyinde abd doları cinsinden sondaki Bulut Çözümü Sağlayıcısı program gelirini temsil eder. Veriler, önceki aya kadar son on iki aylık geliri göstermek için her ayın sekizinci ' i üzerinde yenilenir. Örneğin, 9 Eylül 2020 ' de, 5 2020 2019 Eylül ayının 5. ayında, için TTı 'yi görmeniz gerekir. Yazılım abonelikleri hariç tutulur. TTE geliri yalnızca faturaların zaten ödeneceği uygun geliri yansıtır. 

Iş Ortağı Merkezi 'nde görüntülenecek gelir, 12 aylık sabit bir zaman aralığı için hesaplanır ve daha kısa bir zaman dilimine değiştirilemez.

Gelirin bir dökümünü Iş ortağı konum hesap düzeyinize görmek için:

- ' Karşıdan yükleme ayrıntıları ' bağlantısını seçin ve tüm konumlarınızdaki TTı gelirini görüntüleyen bir. tsv dosyasını indirin.

> [!NOTE]
> . Tsv dosyasındaki MPN kimliklerine ait her bir TTK gelir numarasını toplamak, Iş Ortağı Merkezi 'nde görüntülenen genel TTK gelirinden daha büyük olabilir. Bunun nedeni, gelir, indirilen dosyada birden çok iş ortağı attribukatındaki abonelikler için Double olarak sayılır.

## <a name="subscription-summary"></a>Abonelik Özeti

Ekranın alt yarısında, aboneliklerin bir özeti görüntülenir. Gerekli abonelik ayrıntılarını görmek için aşağıdaki filtreleri kullanın:  

1. **Süre** -abonelik özetini görmeyi tercih edebilirsiniz:

- 30D – son 30 gün
- 3Dk – son 3 ay
- 6Dk – son 6 ay
- 12D – son 12 ay

2. **Ürün türü**:

- Office 365
- Microsoft 365
- Dynamics 365
- EMS

Bu filtrelerin uygulanması, bu raporun en üstünde yer alacak olan TTD gelir ölçümünü etkilemez.

## <a name="next-steps"></a>Sonraki adımlar

- [Müşterilerinizin satın aldıkları lisansları nasıl kullandığını çözümleyin](increasing-adoption-and-satisfaction.md)  
- [Müşteri etkinlik günlüklerini görüntüleme](activity-logs.md)
- [Power BI için İş Ortağı Merkezi Analiz uygulaması](power-bi-app-for-direct-partners.md)
