---
title: Yıllık faturalandırma-ortak senaryolar
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: İş Ortağı Merkezi yıllık faturalandırma-yeni abonelikler eklediğinizde, faturalandırma tarihinden önce lisans eklediğinizde, lisans miktarını değiştirmeden veya abonelikleri askıya alabilir/yeniden etkinleştirmelisiniz.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7494fd7cc003d1179c0ed959b21e1be2cbcc3255
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502489"
---
# <a name="common-annual-billing-scenarios-in-partner-center"></a>Iş Ortağı Merkezi 'nde genel yıllık faturalandırma senaryoları

**Uygun roller**

- Yönetim Aracısı
- Faturalama yöneticisi
- Yardım Masası Aracısı
- Satış Aracısı

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

1 Şubat 'ta, lisans miktarınızdan birini iki olarak artırırsınız. 15 Şubat lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırlarını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Bisiklet örneği eşit|-48,00|1|-48,00
1/13/2018|1/31/2018|Bisiklet örneği eşit|2,47|1|2,47
01.02.2018|1/12/2019|Bisiklet örneği eşit|44,98|2|89,96

Yıllık fiyat, 0,13 (48.00/365) günlük fiyatına eşit olan 48,00 ' dir.

Birim fiyatı = servis süresi x gün cinsinden gün sayısı x Lisans sayısı.

1/13/2018 – 1/31/2018 servis döneminde 19 gün vardır.

Bu nedenle, birim fiyatı = 2,47 (19x 0.13 x1)

346 gün süreyle hizmet dönemi 2/1/2018 – 1/12/2019.

Bu nedenle, birim fiyatı = 44,98 (346x 0.13 x2)

## <a name="suspend-before-30-days"></a>30 günden önce askıya al

Fatura faturanızı her ayın 15 ' i vardır. 13 Ocak 'ta, $4/ay için bir lisansa sahip yeni bir abonelik satın alıp yıllık faturalandırmayı seçmeniz gerekir. 15 Ocak lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Satın alma sırasında ücretleri eşit oranda artır|48,00|1|48,00

1 Şubat 'ta aboneliğinizi askıya alırsınız. 15 Şubat lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
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

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Satın alma sırasında ücretleri eşit oranda artır|48,00|1|48,00

1 Şubat 'ta aboneliğinizi askıya alırsınız. 15 Şubat lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Ücreti iptal et|-48,00|1|-48,00

1 Mart 'ta aboneliğinizi yeniden etkinleştirin. 15 Mart lisans tabanlı mutabakat dosyası aşağıdaki faturalandırma satırını içerir:

|Ücret başlangıç tarihi |Ücretlendirme bitiş tarihi |Ücret türü |Birim Fiyatı |Miktar |Miktar |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Satın alma sırasında ücretleri eşit oranda artır|41,34|1|41,34

Yıllık fiyat, 0,13 (48.00/365) günlük fiyatına eşit olan 48,00 ' dir.

Birim fiyatı = servis süresi x gün cinsinden gün sayısı x Lisans sayısı.

318 gün süreyle hizmet dönemi 3/1/2018 – 1/12/2019.

Bu nedenle, birim fiyatı = 41,34 (318x 0.13 x1).
