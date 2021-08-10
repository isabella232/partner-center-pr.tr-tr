---
title: Yinelenen satın almalar için tek & faturalama
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: İş Ortağı Merkezi için faturalama örneklerini ekleyin ve yinelenen satın almaları seçin. Abonelik satın aldığınız zaman, daha fazla abonelik ekleyin, lisans ekleyin veya lisansları kaldırın.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d79c6d39760aa4bc18eca51654b669e2b81b29a8187aadfbaf79601ee537b15b
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115682292"
---
# <a name="partner-center-billing-scenarios-for-one-time-and-select-recurring-purchases"></a>İş Ortağı Merkezi kez faturalama senaryolarını ve yinelenen satın almaları seçme

**Uygun roller:** Yönetici aracısı | Faturalama yöneticisi | Yardım masası aracısı | Satış aracısı

Bunlar yaygın [faturalama senaryolarıdır.](common-billing-scenarios.md) 

## <a name="purchase-a-subscription-and-add-a-license-on-the-same-day"></a>Aynı gün abonelik satın alma ve lisans ekleme

Senaryo 1'de, 11 Haziran'da 4 ABD doları birim fiyatıyla bir abonelik satın alın. Aynı günün ilerleyen saatlerini aynı fiyatla aynı aboneliklerden bir tane daha satın alasınız.

Mutabakat dosyası aşağıdakileri içerir:

- 10 Haziran – 9 Temmuz hizmet dönemi için 4 ABD doları fatura.
- 11 Haziran – 11 Haziran hizmet dönemi için 4,00 ABD doları olarak sıralandı. Bu, lisansa sahip olduğunuz dönemdir. Hesaplama = (aylık fiyat/hizmet dönemindeki toplam gün sayısı) x proratılmış hizmet döneminde x lisans sayısı = (4/30) x 30 x 1 = 4,00.
- 10 Haziran - 9 Temmuz arasında hizmet dönemi için 8,00 ABD doları provokasyona açık rebill. Bu, iki lisansınız olduğu dönemdir. Hesaplama = (4/30) x 30 x 2 = 8,00.

|**Satın alma tarihi**   |**Ücret başlangıcı** |**Ücret sonu**  |**Birim fiyat**  |**Miktar**  |**Miktar** |**Ücret türü** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |4 ABD doları                |1                 |4 ABD doları            |Yeni         |
|6/11/2019     | 6/10/2019    |7/09/2019        |4 ABD doları        |1        | -4 ABD doları       |addQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |4 ABD doları        | 2      |8 ABD doları         |addQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Abonelik satın alma ve daha sonra daha fazla abonelik ekleme

Senaryo 2'de, 11 Haziran'da 4 ABD doları birim fiyatıyla bir abonelik satın alırsınız ve 12 Haziran'da aynı fiyatla aynı ürün için başka bir abonelik satın alın.

Mutabakat dosyası aşağıdakileri içerir:

- 10 Haziran – 9 Temmuz hizmet dönemi için 4 ABD doları fatura.
- 11 Haziran – 12 Haziran hizmet dönemi için 3,87 ABD doları olarak sıralandı. Bu, bir lisansınız olduğu dönemdir. Hesaplama = (aylık fiyat/hizmet dönemindeki toplam gün sayısı) x proratılmış hizmet döneminde x lisans sayısı = (4/30) x 29 x 1 = 3,87.
- 12 Haziran – 9 Temmuz arasında hizmet dönemi için 7,74 ABD doları açık rebill. Bu, iki lisansınız olduğu dönemdir. Hesaplama = (4/30) x 29 x 2 = 7,74.

|**Satın alma tarihi**   |**Ücret başlangıcı** |**Ücret sonu**  |**Birim fiyat**  |**Miktar**  |**Miktar** |**Ücret türü** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11.06.2019 (bir lisansınız var)     |6/10/2019   |7/09/2019         |4 ABD doları         |1        |4 ABD doları            |Yeni         |
|6/12/2019     | 6/10/2019    |7/09/2019        |4 ABD doları        |1        | -$3,87       |addQuantity           |
|6/12/2019     | 6/10/2019    |7/09/2019        |4 ABD doları        | 2      |7,74 ABD doları       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-license-on-the-same-day"></a>Aynı gün abonelik satın alma ve lisansı kaldırma

Senaryo 3'te aynı ürün için 11 Haziran'da 4 ABD doları birim fiyatıyla iki abonelik satın alın. Aynı gün içinde lisanslardan birini kaldırabilirsiniz.  

Mutabakat dosyası aşağıdakileri içerir:

- 10 Haziran - 9 Temmuz hizmet dönemi için iki lisans için 8 ABD doları fatura.
- 11 Haziran – 11 Haziran hizmet dönemi için 8,00 ABD doları olarak sıralandı. Bu, iki lisansınız olduğu dönemdir. Hesaplama = (aylık fiyat/hizmet dönemindeki toplam gün sayısı) x proratılmış hizmet döneminde x lisans sayısı = (4/30) x 30 x 2 = 8,00.
- Hizmet dönemi için 4,00 ABD doları, 11 Haziran – 9 Temmuz. Bu, bir lisansınız olduğu dönemdir. Hesaplama = (4/30) x 30 x 1 = 4,00.

|**Satın alma tarihi**   |**Ücret başlangıcı** |**Ücret sonu**  |**Birim fiyat**  |**Miktar**  |**Miktar** |**Ücret türü** |
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