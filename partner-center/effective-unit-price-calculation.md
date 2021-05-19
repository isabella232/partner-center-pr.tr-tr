---
title: Geçerli birim fiyat hesaplaması
ms.topic: how-to
ms.date: 04/02/2021
description: Geçerli birim fiyatı ve nasıl hesaplanmış olduğu hakkında bilgi edinmek. Bu makalede ayrıca bir örnek hesaplama da yer alanmıştır.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 84beac77d41b8c11be9ac3cad87460eec9632ac4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147131"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Azure planı tüketimi için geçerli birim fiyat hesaplaması

**Uygun roller:** Faturalama yöneticisi

## <a name="the-effective-unit-price"></a>Geçerli birim fiyatı

Geçerli birim fiyatı ölçüm düzeyinde (kaynak düzeyi yerine) hesaplanır ve ölçüm kullanımına göre günlük olarak ayarlanır.

Geçerli birim fiyatını hesaplamak için aşağıdaki üç faktörü kullanıyoruz:

- Faturalama döngüsü boyunca günlük olarak izlenen tüketim
- Ölçüm için faturalanabilir maliyet
- Katmanlama (varsa)

Faturalama dönemi boyunca tüketimi günlük olarak izlenmiz nedeniyle, geçerli birim fiyatı dalgalı olur. Tüketim hesaplaması durdurduktan ve faturalama dönemini kapatarak, verilen faturalama döneminin son fiyatı kullanılabilir. Dördüncü veya beşinci ondalık ayırıcıdan sonra tüketimde en fazla değişiklik olduğunu görüyorsunuz.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>Ölçümün katmanlı fiyatlandırmayı kullandığını bulma

Ölçümün katmanlı fiyatlandırma mı kullandığını bilmiyorsanız, bunu bulmak için aşağıdaki yordamı kullanın. 

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.
2. **Satış'ı** seçin, Fiyatlandırma **ve teklifler'i ve** ardından Azure **planı fiyatlandırması'ı seçin.**
3. Ölçüm kimliğiniz ile ilgili bilgileri bulun ve fiyatlandırma verilerinizi indirin. 

## <a name="sample-calculation"></a>Örnek hesaplama

Aşağıdaki tabloda, açık dönem boyunca geçerli birim fiyatı nasıl hesaplay geçtiğimize bir örnek verilmiştir.

Tabloda aşağıdaki değerler geçerlidir: 

- **Up** = kaynağın birim fiyatı/saat = 0,868

- **BCU** = ölçüm için faturalandırılabilir tüketim birimi

- **BC** = BCU * UP * 0,85 ölçümü için faturalandırılabilir maliyet. Bu, %15 PEC indirimle ilgili bir ayarlamayı yansıtır. Daha sonra, minimum miktarı ücretlendirmeniz için değeri ondalık işaretinden sonra iki basamakla sınırlamak üzere işlevin alt sınırını kullanıyoruz. 

- **Etkin birim fiyatı** = BCU/BC

>[!NOTE]

>Not: Bu örnekteki ölçüm fiyatlandırma veya diğer indirimlerdeki katmanlara sahip değildir. indirim yüzdeleri ve diğer ayarlamalar için geçerli birim fiyat faktörleri.


| Tarih | BCU (Faturalanabilir tüketim birimi) | BC (Faturalanabilir maliyet) | Geçerli birim fiyatı |
| ------ | ----------- | ----------- | ----------- |  
| 3-Ağu | 29 | 21,39 | 0.737586206896552 |
| 10 Ağu | 210,950039 | 155,63 | 0.737757626107858 |
| 25 Ağu | 555,950039 | 410,17 | 0.737782122900436 |

## <a name="next-steps"></a>Sonraki adımlar

- [Faturalama ve vergiler](billing.md)
