---
title: Yıllık faturalama - yaygın senaryolar
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'İş Ortağı Merkezi faturalama: Yeni abonelikler eklerken, faturalama tarihi öncesinde lisans eklerken, lisans miktarını değiştirirken veya abonelikleri askıya alır/yeniden etkinleştirebilirsiniz.'
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a6392094e000b899e0545655ecf9ed6117535f7f
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148712"
---
# <a name="common-annual-billing-scenarios-in-partner-center"></a>İş Ortağı Merkezi'da yaygın yıllık faturalama İş Ortağı Merkezi

**Uygun roller:** Yönetici aracısı | Faturalama yöneticisi | Yardım masası aracısı | Satış aracısı

Bu örnek [yaygın faturalama senaryoları,](common-billing-scenarios.md) yıllık faturalamayı faturalarda İş Ortağı Merkezi.

## <a name="new-annual-subscription"></a>Yeni yıllık abonelik

Faturalama tarihiniz her ayın 15'indedir. 13 Ocak'ta, aylık 4 ABD doları için tek lisansla yeni bir abonelik satın alın ve yıllık faturalamayı seçin. 15 Ocak lisans tabanlı mutabakat dosyası aşağıdaki fatura satırına sahip olur:

|Ücret Başlangıç Tarihi |Ücret Bitiş Tarihi |Ücret Türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Satın almada ücret prorate|48.00|1|48.00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Abonelik yıl dönümü tarihten sonra ancak faturalama tarihi öncesinde lisans ekleme

11/2/2/17 tarihinde 211,20 ABD doları yıllık bir lisansa sahip yeni bir abonelik satın asınız. Abonelik yıl dönümü her ayın 11.'i olarak ayarlanır. Microsoft faturalandırma sistemi aşağıdaki faturalandırma satırlarını oluşturur:

- $211,20:2/11/17 – 2/10/18 için ücret.

2/12/17 tarihinde ikinci bir lisans satın alırsınız. Faturalama tarihi 2/14/17 ' dir. Bir fatura ve mutabakat dosyası oluşturulur. Mutabakat dosyası aşağıdaki faturalandırma satırlarını içerir:

|Ücret başlangıç tarihi  |Ücretlendirme bitiş tarihi  |Ücret türü  |Birim Fiyatı |Miktar | Miktar |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Satın alma sırasında ücretleri eşit oranda artır |211,20 |1 | 211,20 |

Aboneliğinizde yıldönümü 3/11/17, Microsoft faturalandırma sistemi, 2/12/17 tarihinde lisans artışı için aşağıdaki fatura satırlarını oluşturur:

- $211,20 – 2/11/17 dönemi için kredi: 2/10/18.
- $0,58 – 2/11/17 2/11/17 için bir lisansın lisans başına eşit olarak dağıtılmış ücreti.
- 2/12/17 – 3/10/2017 için iki lisans için lisans başına $15,62 eşit oranda dağıtılmış ücret.
- 3/11/2017 – 2/10/2018 için iki lisans için lisans başına $195,00 eşit oranda dağıtılmış ücret.

2/11/17 tarihinde bir abonelik satın alırsınız. 12.02.17'de bir lisans eklersiniz. Faturalama tarihiniz 14.02.17'tir. Aboneliğiniz 11.02.18'de yenilenecektir.

Sonraki faturalama tarihiniz 14.03.17'tir ve bir fatura ve mutabakat dosyası oluşturulur. Mutabakat dosyası aşağıdaki faturalama satırlarını içerir:

|Ücret Başlangıç Tarihi  |Ücret Bitiş Tarihi  |Ücret Türü  |Birim Fiyatı |Miktar | Miktar |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Döngü Örneği Hızı |-211.20 |1 |-211.20 |
|2/11/2017 |2/11/2017 |Döngü Örneği Hızı |0.58 |1 |0.58 |
|2/12/2017 |3/10/2017 |Döngü Örneği Hızı |15.62 |2 |31.25 |
|3/11/2017 |2/10/2018 |Döngü Örneği Hızı |195.00 |2 |390.00 |

11/2/18 tarihinde abonelik 12 aylık bir süre daha yenilenecektir.

## <a name="change-license-quantity"></a>Lisans miktarını değiştir

Faturalama tarihiniz her ayın 15'indedir. 13 Ocak'ta, aylık 4 ABD doları için tek lisansla yeni bir abonelik satın alın ve yıllık faturalamayı seçin. 15 Ocak lisans tabanlı mutabakat dosyası aşağıdaki fatura satırına sahip olur:

|Ücret Başlangıç Tarihi |Ücret Bitiş Tarihi |Ücret Türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Satın almada ücret prorate|48.00|1|48.00

1 Şubat 'ta, lisans miktarınızdan birini iki olarak artırırsınız. 15 Şubat lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırlarını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Bisiklet örneği eşit|-48,00|1|-48,00
1/13/2018|1/31/2018|Bisiklet örneği eşit|2,47|1|2,47
01.02.2018|1/12/2019|Bisiklet örneği eşit|44,98|2|89,96

Yıllık fiyat, 0,13 (48.00/365) günlük fiyatına eşit olan 48,00 ' dir.

Birim fiyat = hizmet dönemindeki gün sayısı x günlük fiyat x lisans sayısı.

13.01.2018 – 31.01.2018 hizmet döneminde 19 gün vardır.

Bu nedenle birim fiyat = 2,47 (19x0,13x1)

1/2/2018 – 12.01.2019 hizmet döneminde 346 gün vardır.

Bu nedenle birim fiyat = 44,98 (346x0,13x2)

## <a name="suspend-before-30-days"></a>30 gün önce askıya alma

Faturalama tarihiniz her ayın 15'indedir. 13 Ocak'ta, aylık 4 ABD doları için tek lisansla yeni bir abonelik satın alın ve yıllık faturalamayı seçin. 15 Ocak lisans tabanlı mutabakat dosyası aşağıdaki fatura satırına sahip olur:

|Ücret Başlangıç Tarihi |Ücret Bitiş Tarihi |Ücret Türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Satın almada ücret prorate|48.00|1|48.00

1 Şubat'ta aboneliğinizi askıya alırsınız. 15 Şubat lisans tabanlı mutabakat dosyası aşağıdaki fatura satırına sahip olur:

|Ücret Başlangıç Tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Ücreti iptal et|-48,00|1|-48,00

## <a name="suspend-after-30-days"></a>30 gün sonra askıya al

Fatura faturanızı her ayın 15 ' i vardır. 13 Ocak 'ta, $4/ay için bir lisansa sahip yeni bir abonelik satın alıp yıllık faturalandırmayı seçmeniz gerekir. 15 Ocak lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Satın alma sırasında ücretleri eşit oranda artır|48,00|1|48,00

15 Şubat lisans tabanlı mutabakat dosyası bu abonelik için herhangi bir faturalandırma satırı içermez.
1 Mart 'ta aboneliğinizi askıya alın. 15 Mart lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Ücreti iptal et|-41,34|1|-41,34

Yıllık fiyat, 0,13 (48.00/365) günlük fiyatına eşit olan 48,00 ' dir.

Birim fiyatı = servis süresi x gün cinsinden gün sayısı x Lisans sayısı.

318 gün süreyle hizmet dönemi 3/1/2018 – 1/12/2019.

Bu nedenle, birim fiyatı = 41,34 (318x 0.13 x1). Bu bir kredi olduğundan birim fiyatı-41,34 olur.

## <a name="suspend-and-reactivate"></a>Askıya al ve yeniden etkinleştir

Fatura faturanızı her ayın 15 ' i vardır. 13 Ocak 'ta, $4/ay için bir lisansa sahip yeni bir abonelik satın alıp yıllık faturalandırmayı seçmeniz gerekir. 15 Ocak lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırını içerir:

|Ücret başlangıç tarihi |Ücret Bitiş Tarihi |Ücret Türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Satın almada ücret prorate|48.00|1|48.00

1 Şubat'ta aboneliğinizi askıya alırsınız. 15 Şubat lisans tabanlı mutabakat dosyası aşağıdaki fatura satırına sahip olur:

|Ücret Başlangıç Tarihi |Ücret Bitiş Tarihi |Ücret Türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Ücreti İptal Etme|-48.00|1|-48.00

1 Mart'ta aboneliğinizi yeniden etkinleştirebilirsiniz. 15 Mart lisans tabanlı mutabakat dosyasında aşağıdaki fatura satırı yer alacağız:

|Ücret Başlangıç Tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Satın alma sırasında ücretleri eşit oranda artır|41,34|1|41,34

Yıllık fiyat, 0,13 (48.00/365) günlük fiyatına eşit olan 48,00 ' dir.

Birim fiyatı = servis süresi x gün cinsinden gün sayısı x Lisans sayısı.

318 gün süreyle hizmet dönemi 3/1/2018 – 1/12/2019.

Bu nedenle, birim fiyatı = 41,34 (318x 0.13 x1).
