---
title: Geçerli birim fiyat hesaplaması
ms.topic: how-to
ms.date: 09/27/2021
description: Geçerli birim fiyatı ve nasıl hesaplanmış olduğu hakkında bilgi edinmek. Bu makalede ayrıca bir örnek hesaplama da yer alanmıştır.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 07085375f6b33bd3aef43bab647410d8e1c1e6cc
ms.sourcegitcommit: e1da62b36420d78bf44e3962358d0af65ebc3402
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129089921"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Azure planı tüketimi için geçerli birim fiyat hesaplaması

**Uygun roller:** Faturalama yöneticisi

## <a name="the-effective-unit-price"></a>Geçerli birim fiyatı

Geçerli birim fiyatı ölçüm düzeyinde (kaynak düzeyi yerine) hesaplanır ve ölçüm kullanımına göre günlük olarak ayarlanır.

Geçerli birim fiyatını hesaplamak için aşağıdaki üç faktörü kullanıyoruz:

- Faturalama döngüsü boyunca günlük olarak izlenen tüketim
- Ölçüm için faturalanabilir maliyet
- Katmanlama (varsa)

Faturalama dönemi boyunca tüketimi günlük olarak izlenmiz nedeniyle geçerli birim fiyatı dalgalı olur. Tüketim hesaplaması durdurduktan ve faturalama dönemini kapatarak, verilen faturalama döneminin son fiyatı kullanılabilir. Dördüncü veya beşinci ondalık ayırıcıdan sonra tüketimde en fazla değişiklik olduğunu görüyorsunuz.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>Ölçümün katmanlı fiyatlandırmayı kullandığını bulma

Ölçümde katmanlı fiyatlandırma kullanıp kullanmay olmadığını bilmiyorsanız, bunu bulmak için aşağıdaki yordamı kullanın.

> [!NOTE]
> Çalışma alanları arabirimi hakkında daha fazla bilgi edinmek için [bkz. İş Ortağı Merkezi.](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Çalışma alanları görünümü](#tab/workspaces-view)

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.

2. Fiyatlandırma **kutucuğunu** ve ardından **Azure planı fiyatlandırması'ı seçin.**

3. Ölçüm kimliğiniz ile ilgili bilgileri bulun ve fiyatlandırma verilerinizi indirin.

#### <a name="current-view"></a>[Geçerli görünüm](#tab/current-view)

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.

2. **Satış'ı** seçin, Fiyatlandırma **ve teklifler'i ve** ardından Azure **planı fiyatlandırması'ı seçin.**

3. Ölçüm kimliğiniz ile ilgili bilgileri bulun ve fiyatlandırma verilerinizi indirin.

* * *

## <a name="sample-calculation"></a>Örnek hesaplama

Aşağıdaki tabloda, açık dönem boyunca geçerli birim fiyatı nasıl hesaplay geçtiğimize bir örnek verilmiştir.

Tabloda aşağıdaki değerler geçerlidir: 

- **UP** = Kaynağın birim fiyatı/saat = 0,868

- **BCU** = Ölçüm için faturalanabilir tüketim birimi

- **BC** = Ölçüm için faturalanabilir maliyet = BCU * UP * 0,85. Bu, %15 PEC indirimi için bir ayarlamayı yansıtıyor. Ardından, minimum tutarı ücret düşürmek için işlevin alt sınırını kullanarak değeri ondalık ayırıcıdan sonra gelen iki basamakla sınırlandırmış oluruz. 

- **Geçerli birim fiyatı** = BCU/BC

> [!NOTE]
> Bu örnekteki ölçüm, fiyatlandırma veya diğer indirimlerde katmana sahip değildir. Geçerli Birim Fiyat, indirim yüzdelerini ve diğer ayarlamaları gösterir.

| Tarih | BCU (Faturalanabilir tüketim birimi) | BC (Faturalanabilir maliyet) | Geçerli birim fiyatı |
| ------ | ----------- | ----------- | ----------- |  
| 3-Ağu | 29 | 21.39 | 0.737586206896552 |
| 10-Ağu | 210.950039 | 155.63 | 0.737757626107858 |
| 25-Ağu | 555.950039 | 410.17 | 0.737782122900436 |

## <a name="next-steps"></a>Sonraki adımlar

- [Faturalama ve vergiler](billing.md)
