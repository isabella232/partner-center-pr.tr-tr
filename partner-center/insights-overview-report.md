---
title: İş Ortağı Merkezi Analizler Genel Bakış panosu
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Lisanslar, abonelikler ve Azure tüketimiyle satış ve dağıtım, müşteri büyümesi ve gelir artışı ile ilgili işlemlerinizin anlık görüntüsüne bakın.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 439d49a7286ae9a2a1d61a088d86ec32b3f8fcb5
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129071870"
---
# <a name="overview-dashboard-reports-available-in-partner-center-insights"></a>Genel bakış pano raporları İş Ortağı Merkezi Analizler
 
**Uygun roller:** Genel yönetici | Yönetici aracısı | Rapor görüntüleyici | Yönetici raporu görüntüleyicisi

Genel Analizler panosu Müşteriler, Abonelikler, Azure Tüketim Geliri ve Lisanslar gibi Ana Performans Göstergelerinin (KIP) anlık görüntüsünü sağlar. Genel Bakış raporunda aşağıdaki grafikleri görselleştirebilirsiniz.

- Özet  
- Müşterileriniz, aboneliklerinizi ve lisanslarınızı coğrafi olarak yayma  
- Müşterilerin büyüme eğilimi 
- Aboneliklerin büyüme eğilimi 
- Azure'da tüketilen gelir artışı eğilimi 
- Lisansların büyüme eğilimi 

## <a name="summary"></a>Özet

Özet; müşteriler, Azure Tüketim Geliri (ACR), satılan abonelikler, etkin abonelikler ve dağıtılan lisanslar hakkında bilgi içerir. 

:::image type="content" source="images/insights/summary.png" alt-text="Özet lisansları.":::

Özet'in her bölümü hakkında daha fazla bilgi aşağıda verilmiştir.

### <a name="customers"></a>Müşteriler

Müşteriler **alanı** şunları içerir:

- Farklı asif türleri aracılığıyla ve tüm bulut ürünleri arasında en az bir etkin aboneliği olan tüm müşterilerin geçerli sayısı.
- Seçilen tarih aralığındaki müşterilerin büyüme yüzdesi.
- Mikro grafik, seçilen tarih aralığındaki müşteri sayısına göre aylara göre eğilim gösterir.

### <a name="azure-consumed-revenue-acr"></a>Azure Tüketim Geliri (ACR)

Özet **Azure Tüketim Geliri (ACR)** alanı şunları içerir:

- Seçili tarih aralığı üzerinden size atfedilen toplam ACR (ABD doları olarak).
- Seçilen tarih aralığındaki öznitelikli ACR'de (ABD doları) büyüme veya düşüş yüzdesi.
- Mikro grafik, seçili tarih aralığında size atfedilen AYLıK ACR eğilimini ABD doları olarak gösterir 

> [!NOTE]
> ACR verileri, Yönetici rapor görüntüleyicisi rolü atanmış kullanıcılar tarafından kullanılabilir.
 
### <a name="subscriptions-sold"></a>Satılan abonelikler

**Özet'in Satılan** Abonelikler alanı şunları içerir:

- Bulut ürünü aboneliklerinin (etkin ve etkin olmayan) sizin tarafından satılan veya yönetilen toplam geçerli sayısı.  
- Seçilen tarih aralığındaki aboneliklerdeki büyüme veya düşüş yüzdesi.
- Mikro grafik, seçilen tarih aralığındaki toplam aboneliklerin aylara göre eğilimini gösterir.

### <a name="active-subscriptions"></a>Etkin abonelikler

**Özet'in** Etkin abonelikler alanı şunları içerir:

- Etkin kullanımın ürün telemetri verilerine göre ölçüleceği bulut ürünü aboneliklerinin geçerli sayısı. Bu, tüm azure deneme aboneliklerini dışlar.  
- Etkin aboneliklerin seçilen tarih aralığındaki büyüme yüzdesi.
- Mikro grafik, seçili tarih aralığında etkin aboneliklerin aylara göre eğilimini gösterir.
 
### <a name="licenses-deployed"></a>Dağıtılan lisanslar

**Özet'e dağıtılan** Lisanslar alanı şunları içerir:
 
- Seçilen zaman dönemi içinde müşteri aboneliklerinize dağıtılan tüm Bulut ürünü lisanslarının sayısı. 
- Seçilen tarih aralığı boyunca bu lisanslardaki büyüme veya düşüş yüzdesi. 
- Mikro grafik, seçilen tarih aralığına göre atanan bu lisans sayısına göre aylık eğilimini gösterir.

## <a name="geographical-spread-of-your-customers-subscriptions-and-licenses"></a>Müşterileriniz, aboneliklerinizi ve lisanslarınızı coğrafi olarak yayma

Bu görünüm, toplam müşterilerin, aboneliklerin ve lisansların müşteri ülkelerinin coğrafi dağılımıdır. Bu içgörüleri haritada görüntülemek için farklı sekmeleri seçin. Haritanın konumunu yakınlaştırmak için kılavuzda bir ülke arayabilir ve bu ülkeyi seçin. Haritada Giriş düğmesine basarak özgün görünüme geri dönebilirsiniz. Her sekmeye (örneğin Müşteriler, Abonelikler) tıklarken her ülke için ölçümün değeri ve ülke için Toplam değeri görüntülenir.  

:::image type="content" source="images/insights/geosummary.png" alt-text="Coğrafi özet.":::

## <a name="customers-growth-trend"></a>Müşterilerin büyüme eğilimi

Seçilen tarih aralığı için toplam müşteri sayılarının aylık eğilimi. X ekseni seçilen tarih aralığının aylarını, Y ekseni ise söz konusu aya göre toplam müşteri sayısını temsil eder. 

:::image type="content" source="images/insights/customer-growth.png" alt-text="müşteri büyüme eğilimi.":::

## <a name="subscriptions-growth-trend"></a>Aboneliklerin büyüme eğilimi

Bu, seçilen tarih aralığı için müşteri abonelik sayısı eğilimini gösterir. X ekseni seçilen tarih aralığının aylarını, Y ekseni ise ürünün seçili abonelik sayısını temsil eder. Grafiği belirli bir zaman dönemine yakınlaştırmak için grafiğin üst kısmında kaydırıcıyı kaydırın. 

:::image type="content" source="images/insights/subscription-growth.png" alt-text="Abonelik büyüme eğilimi.":::

## <a name="azure-consumed-revenue-growth-trend"></a>Azure Tüketim Geliri büyüme eğilimi

Seçili tarih aralığında size atfedilen ABD doları olarak tüketilen Azure gelirinin aylık eğilimi. X ekseni seçilen tarih aralığının aylarını, Y ekseni ise ay boyunca size atfedilen ABD doları olarak tüketilen toplam Azure gelirini temsil eder.

> [!NOTE]
> ACR yalnızca Yönetici rapor görüntüleyicisi rolü atanmış kullanıcılara görünür. 

:::image type="content" source="images/insights/azure-consumed.png" alt-text="Azure tüketimi.":::

## <a name="licenses-growth-trend"></a>Lisansların büyüme eğilimi
 
Seçilen tarih aralığı boyunca tüm müşteriler tarafından atanan lisansların eğilimi. X ekseni seçilen tarih aralığının aylarını, Y ekseni ise seçtiğiniz ürünün lisans sayısını temsil eder. Grafiği belirli bir zaman dönemine yakınlaştırmak için grafiğin üst kısmında kaydırıcıyı kaydırın.  

:::image type="content" source="images/insights/licenses-growth.png" alt-text="Lisans.":::

## <a name="next-steps"></a>Sonraki adımlar

Daha fazla rapor için [bkz. İş Ortağı Merkezi Analizler.](partner-center-insights.md)
