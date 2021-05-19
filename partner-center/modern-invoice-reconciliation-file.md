---
title: CSP tek sefer satın almaları için dosya alanlarının mutabakatı
ms.topic: conceptual
ms.date: 01/29/2021
description: CsP'nizin tek kez satın alma mutabakat dosyasındaki tüm öğeler hakkında bilgi İş Ortağı Merkezi örnek değerler de dahil.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: 85946f44e1265ad5012faf9d782609904100c80e
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146264"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>CSP tek sefer satın alma mutabakat dosyası alanları

**Uygun roller:** Hesap yöneticisi | Faturalama aracısı

## <a name="using-the-recon-file"></a>Mutabakat dosyasını kullanma
Aşağıdaki tabloda, CSP tek sefer satın almaları için mutabakat dosyasındaki alanlar için açıklamalar ve örnek değerler verilmiştir.

Mutabakat dosyaları hakkında daha fazla bilgi için [bkz. Mutabakat dosyalarını kullanma.](use-the-reconciliation-files.md)

| Sütun | Açıklama | Örnek değer |
| ------ | ----------- | ------------ |
| PartnerId | Belirli bir faturalama varlığı için GUID biçiminde benzersiz tanımlayıcı. Mutabakat için gerekli değildir. Tüm satırlarda aynı. | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | Müşteri için GUID biçiminde benzersiz Microsoft tanımlayıcısı. | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | Müşterinin kuruluş adı, İş Ortağı Merkezi. Bu sütun, faturayı sistem bilgileriyle mu mutabakata varmak için önemlidir. | *Johnny Modern Cust DE2* |
| CustomerDomainName | Müşterinin etki alanı adı. | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | Müşterinizin bulunduğu ülke. Bölgeniz için [ülkelerin tam listesini](./regional-authorization-overview.md) görüntüleyin.  | *DE* |
| Faturanumarası | Mutabakat dosyası ile ilişkili fatura numarası.  | *G002297372* |
| Mpnıd | CSP iş ortağının MPN tanımlayıcısı. Daha fazla bilgi için bkz. [iş ortağı tarafından nasıl yapılır](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *6034453* |
| Resellermpnıd | Abonelik için kayıt satıcısının MPN tanımlayıcısı. | *6048879* |
| OrderId | Microsoft faturalandırma platformunda bir sipariş için benzersiz tanımlayıcı. Destek ile iletişim kurulurken sırayı belirlemek yararlı olabilir. Mutabakat için kullanılmıyor. | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | Siparişin yerleştirildiği UTC tarihi. | *10/3/2020* |
| ProductId | Ürünün benzersiz tanımlayıcısı. | *DZH318Z0BNZ5* |
| SkuId | SKU benzersiz tanımlayıcısı. | *006G* |
| AvailabilityId | Kullanılabilirlik benzersiz tanımlayıcısı. | *DZH318Z08B80* |
| SkuName | SKU adı. | *Tablolar - LRS* |
| ProductName | Ürün adı. | *Tablolar* |
| ChargeType | Ücret [veya ayarlama](./recon-file-charge-types.md) türü. | *Yeni* |
| UnitPrice | Satın alma zamanında fiyat listesinde yayımlanan lisans başına fiyat. Bunun mutabakat sırasında faturalama sisteminize depolanmış bilgilerle eş olduğundan emin olun. | *0.045* |
| Miktar | Lisans sayısı. Bunun mutabakat sırasında faturalama sisteminize depolanmış bilgilerle eş olduğundan emin olun. | *1* |
| Ara toplam | Vergiden önceki toplam. Alt toplam, geçerli birim fiyatıyla çarpılan faturalanabilir miktara eşit olması gerekir. | *0* |
| TaxTotal | Vergi tutarı ücreti. Pazar vergi kurallarına ve belirli koşullara göre. | *0* |
| Toplam | Toplam tutar, alt toplam ve vergi tutarına eşittir. | *0* |
| Para Birimi | Faturanız, müşterinin para birimi bağlamında oluşturulur. Yani, farklı faturalanabilir para birimlerinden müşterilerle bir iş ortağı deneyimidir iseniz, her müşteri para birimi türü için bir fatura alacaksınız.  | *EUR* |
| PriceAdjustmentDescription | Birim fiyatındaki ayarlamaların nedenleri. Bunlar ana nedenlerdir, ancak geçerli birim fiyatını belirlemekten sınırlı değildir. | *["15,0% Partner for Services tarafından kazanılan krediler"]* |
| PublisherName | Ürünün yayımcısı.  | *Microsoft* |
| PublisherId | Iş ortağı merkezinin yayımcıyı tanımlamak için kullandığı benzersiz bir tanımlayıcı. | *NA* |
| Abonelik açıklaması | Fiyat listesinde tanımlandığı şekilde, müşteri tarafından satın alınan hizmet sunumunun adı. Bu sütun, OfferName ile özdeş bir alandır. | *Azure planı* |
| SubscriptionId | Microsoft faturalandırma platformunda bir abonelik için benzersiz tanımlayıcı. Mutabakat için kullanılmıyor. Bu tanımlayıcının iş ortağı yönetim konsolundaki abonelik KIMLIĞIYLE aynı olmadığına unutmayın. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | Bir aboneliğin fatura döneminin başladığı tarih. | *9/1/2020* |
| ChargeEndDate | Bir aboneliğin fatura döneminin sona erdiği tarih. | *30.09.2020* |
| Tertermbillingcycle | Satın alma sırasında aboneliğe devam etme taahhüdünde geçen süre. | *Depolanan veri (GB/ay)* |
| Efekt, BirimFiyat | Fatura döngüsünün maliyetini hesaplamak için eşit olarak dağıtılmış birim fiyatı. İndirimler, faturalandırma günlerindeki ayarlamalar ve diğer faktörler, geçerli birim fiyatını belirlemektir. Daha fazla bilgi için bkz. [geçerli birim fiyat hesaplaması](./effective-unit-price-calculation.md).  | *0,03825* |
| UnitType | Ölçerin ücretlendirildiği birim türü. | *1 GB/Ay* |
| AlternateId | Başvurulan sipariş satırı öğesinin alternatif KIMLIĞI. | *6dc5c039750a* |
| BillableQuantity | Faturalandırılan toplam miktar.  | *0,005001* |
| BillingFrequency | Satın alma sırasında seçilen faturalandırma planı. | *NA*  |
| PricingCurrency | Fiyat listesindeki para birimi. | *USD* |
| PCToBCExchangeRate | Fiyatlandırma para birimi için faturalama para birimine uygulanan döviz kuru. | *0.846202666* |
| PCToBCExchangeRateDate | Faturalama para biriminin fiyatlandırma para biriminin belirlen olduğu tarih. | *30.09.2020* |
| MeterDescription | Ölçüm açıklaması.  | *Tablolar - Depolanan LRS Verileri (GB/Ay)* |
| ReservationOrderId | Rezervasyon Sipariş Kimliği. | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | Kredi Açıklaması. | *Azure Tüketim Kredisi* |

>[!NOTE]
>Azure tüketiminizi tek kullanımlık satın alma mutabakat dosyanıza uzlaştırabilirsiniz. Bunu yapmak için günlük olarak derecelendirilmiş kullanım mutabakat dosyanıza gidin ve SubscriptionID'nizi bulun. Bu, Azure Plan Kimliğiniz ile ilişkili tüm maliyetleri görüntüler. Azure SubscriptionID'niz EntitlementID olarak gösterilir.

## <a name="next-steps"></a>Sonraki adımlar

- [Faturalama ve vergiler](billing.md)
