---
title: CSP tek seferlik satın alma işlemleri için keşfi dosya alanları
ms.topic: conceptual
ms.date: 11/10/2020
description: Örnek değerler de dahil olmak üzere Iş Ortağı Merkezi 'nde CSP tek seferlik satın alma mutabakatı dosyanızdaki tüm öğeler hakkında bilgi edinin.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: 29574dad6c3dd5eedbcf93dd555509cb04144ef5
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182588"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>CSP tek seferlik satın alma mutabakatı dosya alanları

## <a name="using-the-recon-file"></a>Keşfi dosyasını kullanma
Aşağıdaki tablo, CSP tek seferlik satın alma işlemleri için mutabakat dosyasındaki alanlarla ilgili açıklamaları ve örnek değerleri sağlar.

Karşılaştırma dosyaları hakkında daha fazla bilgi için bkz. [karşılaştırma dosyalarını kullanma](use-the-reconciliation-files.md).

| Sütun | Açıklama | Örnek değer |
| ------ | ----------- | ------------ |
| İş ortağı kimliği | Belirli bir faturalandırma varlığı için GUID biçimindeki benzersiz tanımlayıcı. Mutabakat için gerekli değildir. Tüm satırlarda aynı. | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | Müşteri için GUID biçiminde benzersiz Microsoft tanımlayıcısı. | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | Iş Ortağı Merkezi 'nde raporlanan müşterinin kuruluş adı. Bu sütun, faturayı sistem bilgileriniz ile mutabık kılma açısından önemlidir. | *Modern Müşt. canDE2* |
| CustomerDomainName | Müşterinin etki alanı adı. | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | Müşterinizin bulunduğu ülke. Bölgeniz için [ülkelerin tam listesini](./regional-authorization-overview.md) görüntüleyin.  | *DE* |
| Faturanumarası | Mutabakat dosyası ile ilişkili fatura numarası.  | *G002297372* |
| Mpnıd | CSP iş ortağının MPN tanımlayıcısı. Daha fazla bilgi için bkz. [iş ortağı tarafından nasıl yapılır](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *6034453* |
| Resellermpnıd | Abonelik için kayıt satıcısının MPN tanımlayıcısı. | *6048879* |
| OrderId | Microsoft faturalandırma platformunda bir sipariş için benzersiz tanımlayıcı. Destek ile iletişim kurulurken sırayı belirlemek yararlı olabilir. Mutabakat için kullanılmıyor. | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | Siparişin yerleştirildiği tarih. | *10/3/2020* |
| ProductId | Ürünün benzersiz tanımlayıcısı. | *DZH318Z0BNZ5* |
| SkuId | SKU benzersiz tanımlayıcısı. | *006G* |
| Kullanılabilirlik kimliği | Kullanılabilirlik benzersiz tanımlayıcısı. | *DZH318Z08B80* |
| SkuName | SKU adı. | *Tablolar-LRS* |
| ProductName | Ürün adı. | *Tablolar* |
| ChargeType | Ücret veya ayarlamanın [türü](./recon-file-charge-types.md) . | *Yeni* |
| UnitPrice | Satın alma sırasında fiyat listesinde yayınlanan lisans başına fiyat. Bunun, mutabakat sırasında faturalandırma sisteminizde depolanan bilgilerle eşleştiğinden emin olun. | *0,045* |
| Miktar | Lisans sayısı. Bunun, mutabakat sırasında faturalandırma sisteminizde depolanan bilgilerle eşleştiğinden emin olun. | *1* |
| Ara toplam | Vergi öncesi toplam. Alt toplam, geçerli birim fiyatı ile çarpılan faturalandırılabilir miktara eşit olmalıdır. | *0* |
| Toplam vergi | Vergi tutarı ücreti. Pazar vergi kurallarına ve belirli koşullara göre. | *0* |
| Toplam | Toplam tutar, alt toplam ve vergi tutarına eşittir. | *0* |
| Para Birimi | Faturanız, müşterinin para birimi bağlamında oluşturulur. Yani, farklı faturalanabilir para birimlerinden müşterilerle bir iş ortağı deneyimidir iseniz, her müşteri para birimi türü için bir fatura alacaksınız.  | *EUR* |
| PriceAdjustmentDescription | Birim fiyatındaki ayarlamaların nedenleri. Bunlar ana nedenlerdir, ancak geçerli birim fiyatını belirlemekten sınırlı değildir. | *["15,0% Partner for Services tarafından kazanılan krediler"]* |
| PublisherName | Ürünün yayımcısı.  | *Microsoft* |
| PublisherId | Iş ortağı merkezinin yayımcıyı tanımlamak için kullandığı benzersiz bir tanımlayıcı. | *YANA* |
| Abonelik açıklaması | Fiyat listesinde tanımlandığı şekilde, müşteri tarafından satın alınan hizmet sunumunun adı. Bu sütun, OfferName ile özdeş bir alandır. | *Azure planı* |
| SubscriptionId | Microsoft faturalandırma platformunda bir abonelik için benzersiz tanımlayıcı. Mutabakat için kullanılmıyor. Bu tanımlayıcının iş ortağı yönetim konsolundaki abonelik KIMLIĞIYLE aynı olmadığına unutmayın. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | İş ortağı merkezinin abonelik ücreti için ücretlendirdiği tarih. Abonelik bir yıllık faturalandırma dönemi ve aylık faturalandırma planıyla satın alındığında, ilk mutabakat dosyasında bu, aboneliğin satın alındığı gün olur. Sonraki mutabakat dosyasıyla başlayarak, 30 güne kadar artırılır. | *9/1/2020* |
| ChargeEndDate | Aboneliğin fatura döngüsünün bitiş günü. Abonelik bir yıllık faturalandırma dönemi ve aylık faturalandırma planıyla satın alındığında, ilk mutabakat dosyasında, abonelik satın alındıktan sonra bu 30 gün olur. Sonraki mutabakat dosyasıyla başlayarak, 30 güne kadar artırılır. | *30.09.2020* |
| Tertermbillingcycle | Satın alma sırasında aboneliğe devam etme taahhüdünde geçen süre. | *Depolanan veri (GB/ay)* |
| Efekt, BirimFiyat | Fatura döngüsünün maliyetini hesaplamak için eşit olarak dağıtılmış birim fiyatı. İndirimler, faturalandırma günlerindeki ayarlamalar ve diğer faktörler, geçerli birim fiyatını belirlemektir. Daha fazla bilgi için bkz. [geçerli birim fiyat hesaplaması](./effective-unit-price-calculation.md).  | *0,03825* |
| UnitType | Ölçerin ücretlendirildiği birimin türü. | *1 GB/Ay* |
| AlternateId | Başvurulan sipariş satırı öğesinin alternatif KIMLIĞI. | *6dc5c039750a* |
| BillableQuantity | Faturalandırılan toplam miktar.  | *0,005001* |
| BillingFrequency | Satın alma sırasında seçilen faturalandırma planı. | *YANA*  |
| PricingCurrency | Fiyat listesindeki para birimi. | *USD* |
| PCToBCExchangeRate | Ödeme para birimine fiyatlandırma para birimi için uygulanan döviz kuru. | *0,846202666* |
| PCToBCExchangeRateDate | Faturalandırma para birimine yönelik fiyatlandırma para biriminin belirlendiği tarih. | *30.09.2020* |
| MeterDescription | Ölçüm açıklaması.  | *Tablolar-LRS depolanan veri (GB/ay)* |
| ReservationOrderId | Rezervasyon sipariş kimliği. | *E21A6344E398FFC1C4D7...* |

## <a name="next-steps"></a>Sonraki adımlar

- [Faturalama ve vergiler](billing.md)