---
title: Yaygın aylık faturalama senaryoları
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: 'Aylık faturalamayı İş Ortağı Merkezi yaygın senaryolar: yeni abonelikler ekleme, lisans miktarını değiştirme ve abonelikleri askıya alma gibi senaryolar.'
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dad132f9ad749076dc52a45f1ce77f23839e8671
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960064"
---
# <a name="sample-monthly-billing-scenarios-for-new-subscriptions-changing-license-amounts-or-suspensions"></a>Yeni abonelikler, lisans tutarlarını değiştirme veya askıya alma işlemleri için örnek aylık faturalama senaryoları

**Uygun roller:** Yönetici aracısı | Faturalama yöneticisi | Yardım masası aracısı | Satış aracısı

Bu örnek [yaygın faturalama senaryoları,](common-billing-scenarios.md) faturalar için aylık faturalama İş Ortağı Merkezi.

## <a name="new-monthly-subscription"></a>Yeni aylık abonelik

Faturalama tarihiniz her ayın 15'indedir. 13 Ocak'ta, aylık 4 ABD doları için tek lisansa sahip yeni bir abonelik satın alın ve aylık faturalamayı seçin. 15 Ocak lisans tabanlı mutabakat dosyası aşağıdaki fatura satırlarını içerir:

|Ücret Başlangıç Tarihi |Ücret Bitiş Tarihi |Ücret Türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Döngü ücreti   |4.00       |1        |4.00 |

15 Şubat lisans tabanlı mutabakat dosyası aşağıdaki fatura satırına sahip olur:

|Ücret Başlangıç Tarihi |Ücret Bitiş Tarihi |Ücret Türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2/13/2018         |3/12/2018    |Döngü ücreti   |4.00       |1        |4.00 |

## <a name="change-license-quantity"></a>Lisans miktarını değiştir

Faturalama tarihiniz her ayın 15'indedir. 13 Ocak'ta, aylık 4 ABD doları için tek lisansa sahip yeni bir abonelik satın alın ve aylık faturalamayı seçin. 15 Ocak lisans tabanlı mutabakat dosyası aşağıdaki fatura satırlarını içerir:

|Ücret Başlangıç Tarihi |Ücret Bitiş Tarihi |Ücret Türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Döngü ücreti   |4.00       |1        |4.00    |

1 Şubat'ta lisans miktarınızı birden ikiye artıracaktır. 15 Şubat lisans tabanlı mutabakat dosyası aşağıdaki fatura satırlarını içerir:

|Ücret Başlangıç Tarihi |Ücret Bitiş Tarihi |Ücret Türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 1/13/2018        |2/12/2018    |Döngü Örneği Hızı   |-4.00       |1        |-4.00   |
|1/13/2018         |1/31/2018    | Döngü Örneği Hızı   |2.45       |1        |2.45    |
|01.02.2018         |2/12/2018    | Döngü Örneği Hızı   |1,55       |2        |3.10    |
|2/13/2018         |3/12/2018    | Döngü Örneği Hızı   |4.00       |2        |8.00    |

Aylık fiyat 4,00'dır ve 13.01.2018 – 12.02.2018 hizmet döneminde 31 gün vardır. Bu, günlük 0,129 (4/31) fiyatına eşit olur.

13.01.2018 – 31.01.2018 tarihindeki proration döneminde 19 gün vardır.

Proration birim fiyatı = 2,451 = 19 x 0,129

1/2/2018 – 12.02.2018 tarihindeki proration döneminde 12 gün vardır.

Proration birim fiyatı = 1,54 = 12 x 0,129

## <a name="suspend-before-30-days"></a>30 gün önce askıya alma

Faturalama tarihiniz her ayın 15'indedir. 13 Ocak'ta, aylık 4 ABD doları için tek lisansa sahip yeni bir abonelik satın alın ve aylık faturalamayı seçin. 15 Ocak lisans tabanlı mutabakat dosyası aşağıdaki fatura satırlarını içerir:

|Ücret Başlangıç Tarihi |Ücret Bitiş Tarihi |Ücret Türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Döngü ücreti   |4.00       |1        |4.00    |

1 Şubat'ta aboneliği askıya alırsınız. 15 Şubat lisans tabanlı mutabakat dosyası aşağıdaki fatura satırına sahip olur:

|Ücret Başlangıç Tarihi |Ücret Bitiş Tarihi |Ücret Türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|Ücreti İptal Etme|-4.00|1|-4.00

## <a name="suspend-after-30-days"></a>30 gün sonra askıya alma

Faturalama tarihiniz her ayın 15'indedir. 13 Ocak'ta, aylık 4 ABD doları için tek lisansla yeni bir abonelik satın alın ve aylık faturalamayı seçin. 15 Ocak lisans tabanlı mutabakat dosyası aşağıdaki fatura satırlarını içerir:

|Ücret Başlangıç Tarihi |Ücret Bitiş Tarihi |Ücret Türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|Döngü Ücreti|4.00|1|4.00

15 Şubat lisans tabanlı mutabakat dosyası aşağıdaki fatura satırına sahip olur:

|Ücret Başlangıç Tarihi |Ücret Bitiş Tarihi |Ücret Türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2/13/2018|3/12/2018|Döngü Ücreti|4.00|1|4.00

1 Mart'ta aboneliği askıya alırsınız. 15 Mart lisans tabanlı mutabakat dosyasında aşağıdaki fatura satırı yer alacağız:

|Ücret Başlangıç Tarihi |Ücret Bitiş Tarihi |Ücret Türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|3/12/2018|Ücreti İptal Etme|-1.72|1|-1.72

Aylık fiyat 4,00'dır ve 13.02.2018 – 12.03.2018 hizmet döneminde 28 gün vardır. Bu, günlük 0,143 (4/28) fiyatına eşit olur.

Birim fiyat = hizmet dönemindeki gün sayısı x günlük fiyat x lisans sayısı.

12.03.2018 – 12.03.2018 iptal döneminde 12 gün var.

Bu nedenle birim fiyatı = -1,716 (12 x 0,143 x (-1)).

## <a name="next-steps"></a>Sonraki adımlar

- [Bir kezlik faturalama senaryoları ve yinelenen satın almaları seçme](common-billing-scenarios-onetime-recurring.md)