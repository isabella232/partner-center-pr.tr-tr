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
ms.openlocfilehash: 0f97c36c821955570965fcebb006610f4c5c0c79
ms.sourcegitcommit: e1da62b36420d78bf44e3962358d0af65ebc3402
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129089496"
---
# <a name="common-annual-billing-scenarios-in-partner-center"></a>Iş Ortağı Merkezi 'nde genel yıllık faturalandırma senaryoları

**Uygun roller**: yönetici Aracısı | Faturalandırma Yöneticisi | Yardım Masası Aracısı | Satış Aracısı

Bu örnek [genel faturalandırma senaryoları](common-billing-scenarios.md) , Iş Ortağı Merkezi 'nde yıllık faturalandırma kullanıyorsanız geçerlidir.

## <a name="new-annual-subscription"></a>Yeni yıllık abonelik

Fatura faturanızı her ayın 15 ' i vardır. 13 Ocak 'ta, bir ayda $4 için bir lisansa sahip yeni bir abonelik satın alıp yıllık faturalandırmayı seçersiniz. 15 Ocak lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 Ocak 2018|12 Ocak 2019|Satın alma sırasında ücretleri eşit oranda artır|48,00|1|48,00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Abonelik Yıldönümü tarihinden sonra, fatura tarihinden önce lisans Ekle

11 Şubat 2017 tarihinde bir yıllık $211,20 ' de bir lisansa sahip yeni bir abonelik satın alabilirsiniz. Aboneliğiniz yıl dönümü her ayın 11 günü olarak ayarlanmıştır. Microsoft faturalandırma sistemi aşağıdaki faturalandırma satırlarını oluşturur:

- 11 Haziran 2017 için $211,20, – 10, 2018.

12 Şubat 2017 ' de ikinci bir lisans satın alırsınız. Faturalama tarihi 14 Şubat 2017 ' dir. Bir fatura ve mutabakat dosyası oluşturulur. Mutabakat dosyası aşağıdaki faturalandırma satırlarını içerir:

|Ücret başlangıç tarihi  |Ücretlendirme bitiş tarihi  |Ücret türü  |Birim Fiyatı |Miktar | Miktar |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11 Şubat 2017 |10 Şubat 2018 |Satın alma sırasında ücretleri eşit oranda artır |211,20 |1 | 211,20 |

Aboneliğinizde, 11 Mart 2017 ' de, Microsoft faturalandırma sistemi, 12 Şubat 2017 ' de lisans artışı için aşağıdaki fatura satırlarını oluşturur:

- 11 Haziran $211,20 ' de 2018, 10 Şubat 2017 ' ye kadar kredime dönemi.
- 11 Şubat 2017 ' de 11 2017 Şubat $0,58 ' ye kadar bir lisansın lisans başına eşit olarak dağıtılmış ücreti.
- 12 Şubat 2017 ' de 10 Mart ' de iki lisans için lisans başına $15,62 eşit oranda dağıtılmış ücret.
- 11 Mart 2017, 2018 10 Şubat $195,00 tarihine kadar olmak üzere iki lisans için lisans başına eşit oranda dağıtılmış ücret.

11 Şubat 2017 ' de bir abonelik satın alabilirsiniz. 12 Şubat 2017 ' de bir lisans eklersiniz. Faturalama tarihi 14 Şubat 2017 ' dir. 11 Şubat 2018 ' de aboneliğiniz yenilenir.

Sonraki faturalama tarihi 14 Mart 2017, bir fatura ve mutabakat dosyası oluşturulur. Mutabakat dosyası aşağıdaki faturalandırma satırlarını içerir:

|Ücret başlangıç tarihi  |Ücretlendirme bitiş tarihi  |Ücret türü  |Birim Fiyatı |Miktar | Miktar |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11 Şubat 2017 |10 Şubat 2018 |Bisiklet örneği eşit |-211,20 |1 |-211,20 |
|11 Şubat 2017 |11 Şubat 2017 |Bisiklet örneği eşit |0,58 |1 |0,58 |
|12 Şubat 2017 |10 Mart 2017 |Bisiklet örneği eşit |15,62 |2 |31,25 |
|11 Mart 2017 |10 Şubat 2018 |Bisiklet örneği eşit |195,00 |2 |390,00 |

11 Şubat 2018 ' de abonelik başka bir 12 aylık dönem için yenilenir.

## <a name="change-license-quantity"></a>Lisans miktarını değiştir

Fatura faturanızı her ayın 15 ' i vardır. 13 Ocak 'ta, bir ayda $4 için bir lisansa sahip yeni bir abonelik satın alıp yıllık faturalandırmayı seçersiniz. 15 Ocak lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 Ocak 2018|12 Ocak 2019|Satın alma sırasında ücretleri eşit oranda artır|48,00|1|48,00

1 Şubat 'ta, lisans miktarınızdan birini iki olarak artırırsınız. 15 Şubat lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırlarını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 Ocak 2018|12 Ocak 2019|Bisiklet örneği eşit|-48,00|1|-48,00
13 Ocak 2018|31 Ocak 2018|Bisiklet örneği eşit|2,47|1|2,47
1 Şubat 2018|12 Ocak 2019|Bisiklet örneği eşit|44,98|2|89,96

Yıllık fiyat, $0,13 ' nin günlük fiyatına ($48,00/365) eşitleyen $48,00 ' dir.

Birim fiyatı = servis süresi x günlük fiyat x Lisans sayısı.

Hizmet döneminde 13 Ocak 2018, 31 Ocak 2018 arasında 19 gün vardır.

Bu nedenle birim fiyatı $2,47 (19 x 0,13 x 1)

Hizmet döneminde, 1 Şubat 2018 ' de 12 Ocak 2019 346 gün vardır.

Bu nedenle birim fiyatı $44,98 (346 x 0,13 x 2)

## <a name="suspend-before-30-days"></a>30 günden önce askıya al

Fatura faturanızı her ayın 15 ' i vardır. 13 Ocak 'ta, bir ayda $4 için bir lisansa sahip yeni bir abonelik satın alıp yıllık faturalandırma ' i seçmeniz gerekir. 15 Ocak lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 Ocak 2018|12 Ocak 2019|Satın alma sırasında ücretleri eşit oranda artır|48,00|1|48,00

1 Şubat 'ta aboneliğinizi askıya alırsınız. 15 Şubat lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 Ocak 2018|12 Ocak 2019|Ücreti iptal et|-48,00|1|-48,00

## <a name="suspend-after-30-days"></a>30 gün sonra askıya al

Fatura faturanızı her ayın 15 ' i vardır. 13 Ocak 'ta, $4/ay için bir lisansa sahip yeni bir abonelik satın alıp yıllık faturalandırmayı seçersiniz. 15 Ocak lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 Ocak 2018|12 Ocak 2019|Satın alma sırasında ücretleri eşit oranda artır|48,00|1|48,00

15 Şubat lisans tabanlı mutabakat dosyası bu abonelik için herhangi bir faturalandırma satırı içermez.
1 Mart 'ta aboneliğinizi askıya alın. 15 Mart lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1 Mart 2018|12 Ocak 2019|Ücreti iptal et|-41,34|1|-41,34

Yıllık fiyat, 0,13 ' nin günlük fiyatına (48,00/365) eşitleyen $48,00 ' dir.

Birim fiyatı = servis süresi x gün cinsinden gün sayısı x Lisans sayısı.

Hizmet döneminde 1 Mart 2018 ' de 12 Ocak 2019 318 gün vardır.

Bu nedenle birim fiyatı $41,34 (318 x 0,13 x 1). Bu bir kredi olduğundan birim fiyatı-$41,34 ' dir.

## <a name="suspend-and-reactivate"></a>Askıya al ve yeniden etkinleştir

Fatura faturanızı her ayın 15 ' i vardır. 13 Ocak 'ta, bir ayda $4 için bir lisansa sahip yeni bir abonelik satın alıp yıllık faturalandırmayı seçersiniz. 15 Ocak lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 Ocak 2018|12 Ocak 2019|Satın alma sırasında ücretleri eşit oranda artır|48,00|1|48,00

1 Şubat 'ta aboneliğinizi askıya alırsınız. 15 Şubat lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 Ocak 2018|12 Ocak 2019|Ücreti iptal et|-48,00|1|-48,00

1 Mart 'ta aboneliğinizi yeniden etkinleştirin. 15 Mart lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1 Mart 2018|12 Ocak 2019|Satın alma sırasında ücretleri eşit oranda artır|41,34|1|41,34

Yıllık fiyat, 0,13 (48.00/365) günlük fiyatına eşit olan 48,00 ' dir.

Birim fiyatı = servis süresi x gün cinsinden gün sayısı x Lisans sayısı.

Hizmet döneminde 1 Mart 2018 – 12 Ocak 2019 318 gün daha vardır.

Bu nedenle birim fiyatı $41,34 (318 x 0,13 x 1).

## <a name="multiyear-offers-with-annual-billing"></a>Yıllık faturalandırmayla çoklu yıl teklifleri

Yıllık faturalandırmayla ilgili çoklu yıl teklifleri için ücretler, satın alma tarihinde başlar ve bir yıl boyunca devam eder.

( [Çok yıllık faturalandırma örneğinde](#example-of-multiyear-billing) , ilk yılın ücreti 20 Mart 2020 ' de başlar ve 19 Mart 2021 ' de daha sonra bir yıl sona erdir.)

İkinci yıl için ücretler, ilk yılın ücretlendirme bitiş tarihinden bir ay önce başlar.

(Örnekte, ikinci yıl için ücretler 20 Şubat 2021 tarihinden itibaren ilk yılın ücretinden önce, 19 Mart 2021 ' de bir ay başlar.)

Bu yıllık faturalandırma işleminin, üçüncü yılın abonelik bitiş tarihi ve ücreti bitiş tarihi arasında bir aylık farkı vardır. Ancak abonelik, abonelik bitiş tarihine kadar etkin kalır.

(Örnekte, üçüncü yılda 19 Mart 2023 ' nin abonelik bitiş tarihi, 19 Şubat 2023 ' nin ücretlendirmesinden sonraki bir aydır.)

### <a name="example-of-multiyear-billing"></a>Çok yıllık faturalandırma örneği

20 Mart 2020 tarihinde, izleyen tablolarda gösterilen 36 aylık bir teklif için mutabakat dosyası şöyle olacaktır:

#### <a name="first-year"></a>İlk yıl

|Abonelik başlangıç tarihi  |Abonelik bitiş tarihi  |Ücret başlangıç tarihi  |Ücretlendirme bitiş tarihi  |Ücret türü  |
|:-:|:-:|:-:|:-:|:-:|
|20 Mart 2020|19 Mart 2023|20 Mart 2020|19 Mart 2021|Satın alındığında eşit ücretler ücretleri|

#### <a name="second-year"></a>İkinci yıl

|Abonelik başlangıç tarihi  |Abonelik bitiş tarihi  |Ücret başlangıç tarihi  |Ücretlendirme bitiş tarihi  |Ücret türü  |
|:-:|:-:|:-:|:-:|:-:|
|20 Mart 2020|19 Mart 2023|20 Şubat 2021|19 Şubat 2022|Bisiklet ücreti|

#### <a name="third-year"></a>Üçüncü yıl

|Abonelik başlangıç tarihi  |Abonelik bitiş tarihi  |Ücret başlangıç tarihi  |Ücretlendirme bitiş tarihi  |Ücret türü  |
|:-:|:-:|:-:|:-:|:-:|
|20 Mart 2020|19 Mart 2023|20 Şubat 2022|19 Şubat 2023|Bisiklet ücreti|
