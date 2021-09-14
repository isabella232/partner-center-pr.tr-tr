---
title: Yıllık faturalandırma-ortak senaryolar
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: İş Ortağı Merkezi yıllık faturalandırma-yeni abonelikler eklediğinizde, faturalandırma tarihinden önce lisans eklediğinizde, lisans miktarını değiştirmeden veya abonelikleri askıya alabilir/yeniden etkinleştirmelisiniz.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9cf6ddd8ed73fcd9a7ee20a180072ad51cc5b7c4
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248561"
---
# <a name="common-annual-billing-scenarios-in-partner-center"></a>Iş Ortağı Merkezi 'nde genel yıllık faturalandırma senaryoları

**Uygun roller**: yönetici Aracısı | Faturalandırma Yöneticisi | Yardım Masası Aracısı | Satış Aracısı

Bu örnek [genel faturalandırma senaryoları](common-billing-scenarios.md) , Iş Ortağı Merkezi 'nde yıllık faturalandırma kullanıyorsanız geçerlidir.

## <a name="new-annual-subscription"></a>Yeni yıllık abonelik

Fatura faturanızı her ayın 15 ' i vardır. 13 Ocak 'ta, $4/ay için bir lisansa sahip yeni bir abonelik satın alıp yıllık faturalandırmayı seçmeniz gerekir. 15 Ocak lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Satın alma sırasında ücretleri eşit oranda artır|48,00|1|48,00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Abonelik Yıldönümü tarihinden sonra, fatura tarihinden önce lisans Ekle

2/11/17 tarihinde $211.20/Year için bir lisansa sahip yeni bir abonelik satın alırsınız. Aboneliğiniz yıl dönümü her ayın 11 günü olarak ayarlanmıştır. Microsoft faturalandırma sistemi aşağıdaki faturalandırma satırlarını oluşturur:

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

2/11/17 tarihinde bir abonelik satın alırsınız. 2/12/17 ' de bir lisans eklersiniz. Faturalama tarihi 2/14/17 ' dir. 2/11/18 tarihinde aboneliğiniz yenilenir.

Bir sonraki faturalama tarihi 3/14/17, bir fatura ve mutabakat dosyası oluşturulur. Mutabakat dosyası aşağıdaki faturalandırma satırlarını içerir:

|Ücret başlangıç tarihi  |Ücretlendirme bitiş tarihi  |Ücret türü  |Birim Fiyatı |Miktar | Miktar |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Bisiklet örneği eşit |-211,20 |1 |-211,20 |
|2/11/2017 |2/11/2017 |Bisiklet örneği eşit |0,58 |1 |0,58 |
|2/12/2017 |3/10/2017 |Bisiklet örneği eşit |15,62 |2 |31,25 |
|3/11/2017 |2/10/2018 |Bisiklet örneği eşit |195,00 |2 |390,00 |

2/11/18 tarihinde abonelik başka bir 12 aylık dönem için yenilenir.

## <a name="change-license-quantity"></a>Lisans miktarını değiştir

Fatura faturanızı her ayın 15 ' i vardır. 13 Ocak 'ta, $4/ay için bir lisansa sahip yeni bir abonelik satın alıp yıllık faturalandırmayı seçmeniz gerekir. 15 Ocak lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Satın alma sırasında ücretleri eşit oranda artır|48,00|1|48,00

1 Şubat'ta lisans miktarınızı birden ikiye artıracaktır. 15 Şubat lisans tabanlı mutabakat dosyası aşağıdaki fatura satırlarını içerir:

|Ücret Başlangıç Tarihi |Ücret Bitiş Tarihi |Ücret Türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Döngü Örneği Hızı|-48.00|1|-48.00
1/13/2018|1/31/2018|Döngü Örneği Hızı|2.47|1|2.47
01.02.2018|1/12/2019|Döngü Örneği Hızı|44.98|2|89.96

Yıllık fiyat 48,00'dır ve günlük fiyatı 0,13'e (48,00/365) eşit olur.

Birim fiyat = hizmet dönemindeki gün sayısı x günlük fiyat x lisans sayısı.

13.01.2018 – 31.01.2018 hizmet döneminde 19 gün vardır.

Bu nedenle birim fiyat = 2,47 (19x0,13x1)

1/2/2018 – 12.01.2019 hizmet döneminde 346 gün vardır.

Bu nedenle birim fiyat = 44,98 (346x0,13x2)

## <a name="suspend-before-30-days"></a>30 gün önce askıya alma

Faturalama tarihiniz her ayın 15'indedir. 13 Ocak'ta, aylık 4 ABD doları için tek lisansla yeni bir abonelik satın alın ve yıllık faturalamayı seçin. 15 Ocak lisans tabanlı mutabakat dosyası aşağıdaki fatura satırına sahip olur:

|Ücret Başlangıç Tarihi |Ücret Bitiş Tarihi |Ücret Türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Satın almada ücretleri prorate|48.00|1|48.00

1 Şubat'ta aboneliğinizi askıya alırsınız. 15 Şubat lisans tabanlı mutabakat dosyası aşağıdaki fatura satırına sahip olur:

|Ücret Başlangıç Tarihi |Ücret Bitiş Tarihi |Ücret Türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Ücreti İptal Etme|-48.00|1|-48.00

## <a name="suspend-after-30-days"></a>30 gün sonra askıya alma

Faturalama tarihiniz her ayın 15'indedir. 13 Ocak'ta, aylık 4 ABD doları için tek lisansla yeni bir abonelik satın alın ve yıllık faturalamayı seçin. 15 Ocak lisans tabanlı mutabakat dosyası aşağıdaki fatura satırına sahip olur:

|Ücret Başlangıç Tarihi |Ücret Bitiş Tarihi |Ücret Türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Satın almada ücretleri prorate|48.00|1|48.00

15 Şubat lisans tabanlı mutabakat dosyasında bu abonelik için herhangi bir faturalama satırı yer almaz.
1 Mart'ta aboneliğinizi askıya alırsınız. 15 Mart lisans tabanlı mutabakat dosyasında aşağıdaki fatura satırı yer alacağız:

|Ücret Başlangıç Tarihi |Ücret Bitiş Tarihi |Ücret Türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Ücreti İptal Etme|-41.34|1|-41.34

Yıllık fiyat 48,00'dır ve günlük fiyatı 0,13'e (48,00/365) eşit olur.

Birim fiyat = hizmet dönemindeki gün sayısı x günlük fiyat x lisans sayısı.

1/3/2018 – 12.01.2019 hizmet döneminde 318 gün vardır.

Bu nedenle birim fiyat = 41,34 (318x0,13x1). Bu bir kredi olduğundan birim fiyatı -41,34'tir.

## <a name="suspend-and-reactivate"></a>Askıya alma ve yeniden etkinleştirme

Faturalama tarihiniz her ayın 15'indedir. 13 Ocak'ta, aylık 4 ABD doları için tek lisansla yeni bir abonelik satın alın ve yıllık faturalamayı seçin. 15 Ocak lisans tabanlı mutabakat dosyası aşağıdaki fatura satırına sahip olur:

|Ücret Başlangıç Tarihi |Ücret Bitiş Tarihi |Ücret Türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Satın almada ücretleri prorate|48.00|1|48.00

1 Şubat'ta aboneliğinizi askıya alırsınız. 15 Şubat lisans tabanlı mutabakat dosyası aşağıdaki fatura satırına sahip olur:

|Ücret Başlangıç Tarihi |Ücret Bitiş Tarihi |Ücret Türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Ücreti İptal Etme|-48.00|1|-48.00

1 Mart'ta aboneliğinizi yeniden etkinleştirebilirsiniz. 15 Mart lisans tabanlı mutabakat dosyasında aşağıdaki fatura satırı yer alacağız:

|Ücret Başlangıç Tarihi |Ücret Bitiş Tarihi |Ücret Türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Satın almada ücretleri prorate|41.34|1|41.34

Yıllık fiyat 48,00'dır ve günlük fiyatı 0,13'e (48,00/365) eşit olur.

Birim fiyat = hizmet dönemindeki gün sayısı x günlük fiyat x lisans sayısı.

1/3/2018 – 12.01.2019 hizmet döneminde 318 gün vardır.

Bu nedenle birim fiyat = 41,34 (318x0,13x1).
