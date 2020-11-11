---
title: Geçerli birim fiyat hesaplaması
ms.topic: how-to
ms.date: 11/10/2020
description: Geçerli fiyat birimi ve nasıl hesaplandığı hakkında bilgi edinin. Örnek bir hesaplama içerir.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7b65a79232656af6ddb69fede7a9ee35fe426a9d
ms.sourcegitcommit: 95a5afdf68d88b6be848729830dcd114e3fb0c0f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/11/2020
ms.locfileid: "94499149"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Azure plan tüketimi için geçerli birim fiyat hesaplaması

## <a name="the-effective-unit-price"></a>Geçerli birim fiyatı

Etkin birim fiyatı ölçüm düzeyinde hesaplanır (kaynak düzeyinden farklı olarak) ve ölçüm kullanımına göre günlük olarak ayarlanır.

Geçerli birim fiyatını aşağıdaki üç faktörle hesapladık:

- Fatura döngüsünün tamamında günlük izlenen tüketim
- Ölçüm için faturalandırılabilir maliyet
- Katmanlama (varsa)

Tüketimi faturalandırma döngüsünün tamamında günlük olarak izleyediğimiz için, etkin birim fiyatı dalgalanacaktır. Belirli bir faturalandırma döngüsünün son fiyatı, tüketim hesaplamasını durdurup faturalandırma dönemini kapatdığımızda kullanılabilir olacaktır. En fazla değişikliğin dördüncü veya beşinci ondalık konumdan sonra olduğunu görürsünüz.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>Ölçenin katmanlı fiyatlandırma kullanıp kullanmadığını öğrenin

Ölçmeniz katmanlı fiyatlandırma kullanıp kullanmadığını bilmiyorsanız, öğrenmek için aşağıdaki yordamı kullanın. 

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.
2. **Satış** öğesini seçin, **fiyatlandırma ve teklifler** ' i seçin ve ardından **Azure plan fiyatlandırması** ' nı seçin.
3. Ölçerinizi KIMLIĞE göre bulun ve ardından fiyatlandırma verilerinizi indirin. 

## <a name="sample-calculation"></a>Örnek hesaplama

Aşağıdaki tabloda, açık dönemde geçerli birim fiyatını nasıl hesapladığımızda bir örnek verilmiştir.

Tabloda aşağıdaki değerler geçerlidir: 

- **Up** = kaynağın birim fiyatı/saat = 0,868

- **BCU** = ölçüm için faturalandırılabilir tüketim birimi

- **BC** = BCU * UP * 0,85 ölçümü için faturalandırılabilir maliyet. Bu, %15 PEC indirimle ilgili bir ayarlamayı yansıtır. Daha sonra, minimum miktarı ücretlendirmeniz için değeri ondalık işaretinden sonra iki basamakla sınırlamak üzere işlevin alt sınırını kullanıyoruz. 

- **Etkin birim fiyatı** = BCU/BC

>[!NOTE]
>Not: Bu örnekteki ölçerin fiyatlandırma katmanı yoktur.

| Tarih | BCU (Faturalanabilir tüketim birimi) | BC (Faturalanabilir maliyet) | Geçerli birim fiyatı |
| ------ | ----------- | ----------- | ----------- |  
| 3-Ağu | 29 | 21,39 | 0.737586206896552 |
| 10 Ağu | 210,950039 | 155,63 | 0.737757626107858 |
| 25 Ağu | 555,950039 | 410,17 | 0.737782122900436 |

## <a name="next-steps"></a>Sonraki adımlar

- [Faturalama ve vergiler](billing.md)
