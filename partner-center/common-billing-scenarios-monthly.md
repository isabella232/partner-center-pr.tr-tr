---
title: Genel Aylık faturalandırma senaryoları
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Aylık faturalandırma kullandığınızda Iş Ortağı Merkezi 'ndeki yaygın senaryolar-yeni abonelikler ekleme, lisans miktarını değiştirme ve abonelikleri askıya alma dahildir.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f6486f391925b7b283bec6b14c93c51ede095be033a307031b20bc604a2629e5
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115682326"
---
# <a name="sample-monthly-billing-scenarios-for-new-subscriptions-changing-license-amounts-or-suspensions"></a>Yeni abonelikler için örnek aylık faturalandırma senaryoları, lisans tutarlarını değiştirme veya getirilmesi

**Uygun roller**: yönetici Aracısı | Faturalandırma Yöneticisi | Yardım Masası Aracısı | Satış Aracısı

Bu örnek [genel faturalandırma senaryoları](common-billing-scenarios.md) , Iş Ortağı Merkezi 'nde aylık faturalandırma kullanıyorsanız geçerlidir.

## <a name="new-monthly-subscription"></a>Yeni aylık abonelik

Fatura faturanızı her ayın 15 ' i vardır. 13 Ocak 'ta, $4/ay için bir lisansa sahip yeni bir abonelik satın alıp aylık faturalandırma ' i seçersiniz. 15 Ocak lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırlarını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Bisiklet ücreti   |4.00       |1        |4.00 |

15 Şubat lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2/13/2018         |3/12/2018    |Bisiklet ücreti   |4.00       |1        |4.00 |

## <a name="change-license-quantity"></a>Lisans miktarını değiştir

Fatura faturanızı her ayın 15 ' i vardır. 13 Ocak 'ta, $4/ay için bir lisansa sahip yeni bir abonelik satın alıp aylık faturalandırma ' i seçersiniz. 15 Ocak lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırlarını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Bisiklet ücreti   |4.00       |1        |4.00    |

1 Şubat 'ta, lisans miktarınızdan birini iki olarak artırırsınız. 15 Şubat lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırlarını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 1/13/2018        |2/12/2018    |Bisiklet örneği eşit   |-4,00       |1        |-4,00   |
|1/13/2018         |1/31/2018    | Bisiklet örneği eşit   |2.45       |1        |2.45    |
|01.02.2018         |2/12/2018    | Bisiklet örneği eşit   |1,55       |2        |3,10    |
|2/13/2018         |3/12/2018    | Bisiklet örneği eşit   |4.00       |2        |8,00    |

Aylık fiyat 4,00 ' dir ve – 2/12/2018 servis 1/13/2018 döneminde 31 gün vardır. Bu, gün 0,129 (4/31) günlük fiyatına karşılık gelir.

1/13/2018 – 1/31/2018 ' de, eşit dönemde 19 gün vardır.

Eşit bir birim fiyatı = 2,451 = 19 x 0,129

2/1/2018 – 2/12/2018 olan eşit dönemde 12 gün vardır.

Proration birim fiyatı = 1,54 = 12 x 0,129

## <a name="suspend-before-30-days"></a>30 günden önce askıya al

Fatura faturanızı her ayın 15 ' i vardır. 13 Ocak 'ta, $4/ay için bir lisansa sahip yeni bir abonelik satın alıp aylık faturalandırma ' i seçersiniz. 15 Ocak lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırlarını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Bisiklet ücreti   |4.00       |1        |4.00    |

1 Şubat 'ta bir aboneliği askıya alırsınız. 15 Şubat lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|Ücreti iptal et|-4,00|1|-4,00

## <a name="suspend-after-30-days"></a>30 gün sonra askıya al

Fatura faturanızı her ayın 15 ' i vardır. 13 Ocak 'ta, $4/ay için bir lisansa sahip yeni bir abonelik satın alıp aylık faturalandırma ' i seçersiniz. 15 Ocak lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırlarını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|Bisiklet ücreti|4.00|1|4.00

15 Şubat lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2/13/2018|3/12/2018|Bisiklet ücreti|4.00|1|4.00

1 Mart 'ta aboneliği askıya alırsınız. 15 Mart lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|3/12/2018|Ücreti iptal et|-1,72|1|-1,72

Aylık fiyat 4,00 ' dir ve – 3/12/2018 hizmet 2/13/2018 döneminde 28 gün vardır. Bu, gün 0,143 (4/28) günlük fiyatına karşılık gelir.

Birim fiyatı = servis süresi x gün cinsinden gün sayısı x Lisans sayısı.

3/1/2018 – 3/12/2018 iptal döneminde 12 gün vardır.

Bu nedenle, birim fiyatı =-1,716 (12 x 0,143 x (-1)).

## <a name="next-steps"></a>Sonraki adımlar

- [Bir kerelik faturalama senaryoları ve yinelenen satın alımları seçin](common-billing-scenarios-onetime-recurring.md)