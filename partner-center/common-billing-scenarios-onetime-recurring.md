---
title: Tek seferlik & yinelenen satın alma işlemleri için faturalandırma
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: İş ortağı merkezi faturalama örnekleri bir kerelik bir süre ve yinelenen satın alımları seçin-abonelikler satın aldığınızda, daha fazla abonelik ekleyin, lisans ekleyin veya kaldırın.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 44594df78ba99a3762549b916265de9faa667e7b
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114844114"
---
# <a name="partner-center-billing-scenarios-for-one-time-and-select-recurring-purchases"></a>Bir kerelik iş ortağı merkezi faturalama senaryoları ve yinelenen satın alımları seçin

**Uygun roller**: yönetici Aracısı | Faturalandırma Yöneticisi | Yardım Masası Aracısı | Satış Aracısı

Bunlar [yaygın faturalandırma senaryolardır](common-billing-scenarios.md). 

## <a name="purchase-a-subscription-and-add-a-license-on-the-same-day"></a>Bir abonelik satın alın ve aynı günde bir lisans ekleyin

Senaryo 1 ' de, $4 Haziran tarihinde bir abonelik satın alabilirsiniz. Daha sonra aynı günde aynı fiyattan başka bir abonelik satın alırsınız.

Keşfi dosyası şunları içerir:

- servis dönemi için $4 fatura, 10 Haziran – 9 Temmuz.
- hizmet dönemi için $-4,00 eşit olarak dağıtılmış yeniden faturalandırılır – 11 Haziran. Bu, lisanslandıklarınızı belirttikleriniz. Hesaplama = (aylık fiyat/hizmet dönemindeki toplam gün) x gün, eşit olarak dağıtılmış hizmet döneminde x gün sayısı = (4/30) x 30 x 1 = 4,00.
- servis dönemi 10 Haziran 9 Temmuz $8,00 için eşit olarak dağıtılmış yeniden faturalandırılır. Bu, iki lisansa sahip olduğunuz bir dönemdir. Hesaplama = (4/30) x 30 x 2 = 8,00.

|**Satın alma tarihi**   |**Ücret başlangıcı** |**Ücret bitişi**  |**Birim Fiyat**  |**Miktar**  |**Miktar** |**Ücret türü** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |$4                |1                 |$4            |Yeni         |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        |1        | -$4       |addQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        | 2      |$8         |addQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Bir abonelik satın alın ve daha sonra daha fazla abonelik ekleyin

Senaryo 2 ' de, 1 Haziran tarihinde $4 11 Haziran tarihinde bir abonelik satın alırsınız ve 12 Haziran tarihinde aynı ürün için aynı fiyata başka bir abonelik satın alırsınız.

Keşfi dosyası şunları içerir:

- servis dönemi için $4 fatura, 10 Haziran – 9 Temmuz.
- hizmet dönemi için $-3,87 eşit olarak dağıtılmış yeniden faturalandırılır – 12 Haziran. Bu, bir lisansa sahip olduğunuz bir dönemdir. Hesaplama = (aylık fiyat/hizmet dönemindeki toplam gün) x gün, eşit olarak dağıtılmış hizmet dönemi x/Lisans sayısı = (4/30) x 29 x 1 = 3,87.
- 12 Haziran 9 ' a kadar servis dönemi için $7,74 eşit olarak dağıtılmış yeniden faturalandırılır. Bu, iki lisansa sahip olduğunuz bir dönemdir. Hesaplama = (4/30) x 29 x 2 = 7,74.

|**Satın alma tarihi**   |**Ücret başlangıcı** |**Ücret bitişi**  |**Birim Fiyat**  |**Miktar**  |**Miktar** |**Ücret türü** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019 (bir lisansınız var)     |6/10/2019   |7/09/2019         |$4         |1        |$4            |Yeni         |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        |1        | -$3,87       |addQuantity           |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        | 2      |$7,74       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-license-on-the-same-day"></a>Aynı günde bir abonelik satın alın ve lisans kaldırın

Senaryo 3 ' te, aynı ürün için $4 Haziran tarihinde bir birim fiyatı üzerinden iki abonelik satın alırsınız. Aynı günde daha sonra lisanslardan birini kaldırırsınız.  

Keşfi dosyası şunları içerir:

- hizmet dönemi için $8 Haziran – 9 Temmuz olmak üzere iki lisans için fatura.
- hizmet dönemi için $-8,00 eşit olarak dağıtılmış yeniden faturalandırılır – 11 Haziran. Bu, iki lisansa sahip olduğunuz bir dönemdir. Hesaplama = (aylık fiyat/hizmet dönemindeki toplam gün) x gün, eşit olarak dağıtılmış hizmet dönemi x/Lisans sayısı = (4/30) x 30 x 2 = 8,00.
- hizmet dönemi için $4,00 ile eşit olarak dağıtılmış yeniden faturalandırılır – 9 Temmuz. Bu, bir lisansa sahip olduğunuz bir dönemdir. Hesaplama = (4/30) x 30 x 1 = 4,00.

|**Satın alma tarihi**   |**Ücret başlangıcı** |**Ücret bitişi**  |**Birim Fiyat**  |**Miktar**  |**Miktar** |**Ücret türü** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |4 ABD doları                |2                 |8 ABD doları            |Yeni         |
|6/11/2019     | 6/10/2019    |7/09/2019        |4 ABD doları        |2        | -8 ABD doları       |removeQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |4 ABD doları        | 1      |4 ABD doları         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-licenses-later"></a>Abonelik satın alma ve lisansları daha sonra kaldırma

Senaryo 4'te, 11 Haziran'da 4 ABD doları birim fiyatıyla iki abonelik satın alırsınız ve 12 Haziran'da lisanslardan birini kaldırırsınız.

Mutabakat dosyası aşağıdakileri içerir:

- 10 Haziran – 9 Temmuz hizmet dönemi için 8 ABD doları fatura.
- 11 Haziran – 12 Haziran hizmet dönemi için abd doları-7,74 prokratlı rebill. Bu, iki lisansınız olduğu dönemdir. Hesaplama = (hizmet dönemindeki aylık fiyat/toplam gün sayısı) x proratılmış hizmet döneminde x lisans sayısı = (4/30) x 29 x 2 = 7,74.
- Hizmet dönemi için 3,87 ABD doları, 12 Haziran – 9 Temmuz. Bu, bir lisansınız olduğu dönemdir. Hesaplama = (4/30) x 29 x 1 = 3,87.

|**Satın alma tarihi**   |**Ücret başlangıcı** |**Ücret sonu**  |**Birim fiyat**  |**Miktar**  |**Miktar** |**Ücret türü** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11.06.2019 (iki lisansınız var)     |6/10/2019   |7/09/2019         |4 ABD doları         |2        |8 ABD doları       |Yeni       |
|6/12/2019     | 6/10/2019    |7/09/2019        |4 ABD doları        |2        | -$7,74       |removeQuantity           |
|12.06.2019 (bir lisansınız var)    | 6/10/2019    |7/09/2019   |4 ABD doları    |1      |3,87 ABD doları    |removeQuantity |

## <a name="next-steps"></a>Sonraki adımlar

- [Yeni abonelikler, lisans tutarlarını değiştirme veya askıya alma işlemleri için örnek aylık faturalama senaryoları](common-billing-scenarios-monthly.md)