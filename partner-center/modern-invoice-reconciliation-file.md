---
title: CSP tek seferlik satın alma işlemleri için keşfi dosya alanları
ms.topic: conceptual
ms.date: 01/29/2021
description: Örnek değerler de dahil olmak üzere Iş Ortağı Merkezi 'nde CSP tek seferlik satın alma mutabakatı dosyanızdaki tüm öğeler hakkında bilgi edinin.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: 34ba1c906b2b00b96511aec20d44c358a57925269454345237661e5b403d0099
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115697253"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>CSP tek seferlik satın alma mutabakatı dosya alanları

**Uygun roller**: Hesap Yöneticisi | Faturalandırma Aracısı

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
| OrderDate | Siparişin yerleştirildiği UTC tarihi. | *10/3/2020* |
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
| PublisherName | ürünün Publisher.  | *Microsoft* |
| PublisherId | Iş ortağı merkezinin yayımcıyı tanımlamak için kullandığı benzersiz bir tanımlayıcı. | *YANA* |
| Abonelik açıklaması | Fiyat listesinde tanımlandığı şekilde, müşteri tarafından satın alınan hizmet sunumunun adı. Bu sütun, OfferName ile aynı alandır. | *Azure planı* |
| SubscriptionId | Microsoft faturalama platformunda bir aboneliğin benzersiz tanımlayıcısı. Mutabakat için kullanılamaz. Bu tanımlayıcının, iş ortağı yönetici konsolunda Abonelik Kimliği ile aynı olmadığını unutmayın. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | Aboneliğin faturalama döneminin başladığı tarih. | *9/1/2020* |
| ChargeEndDate | Bir aboneliğin faturalama döneminin bitiş tarihi. | *30.09.2020* |
| TermAndBillingCycle | Satın alma zamanında aboneliğin devam etme süresi taahhüdü. | *Depolanan Veriler (GB/Ay)* |
| EffectiveUnitPrice | Faturalama döngüsünün maliyetini hesaplamak için prorated birim fiyatı. Geçerli birim fiyatı, fatura günlerinde yapılan indirimler, düzeltmeler ve diğer faktörler tarafından belirlenmektedir. Daha fazla bilgi için [bkz. Effective Unit Price Calculation](./effective-unit-price-calculation.md).  | *0.03825* |
| Unittype | Ölçümün ücret ödemesi yapılan birimin türü. | *1 GB/Ay* |
| AlternateId | Başvurulan sipariş satırı öğesinin alternatif kimliği. | *6dc5c039750a* |
| BillableQuantity | Faturalandırılan toplam miktar.  | *0.005001* |
| BillingFrequency | Satın alma zamanında seçilen faturalama planı. | *Na*  |
| PricingCurrency | Fiyat listesindeki para birimi. | *USD* |
| PCToBCExchangeRate | Fiyatlandırma para birimi için faturalama para birimine uygulanan döviz kuru. | *0.846202666* |
| PCToBCExchangeRateDate | Faturalama para biriminin fiyatlandırma para biriminin belirlen olduğu tarih. | *30.09.2020* |
| MeterDescription | Ölçüm açıklaması.  | *Tablolar - Depolanan LRS Verileri (GB/Ay)* |
| ReservationOrderId | Rezervasyon Sipariş Kimliği. | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | Kredi Açıklaması. | *Azure Tüketim Kredisi* |
| SubscriptionStartDate | Aboneliğin satın alınma tarihi. | *5/1/2021* |
| SubscriptionEndDate | Aboneliğin süresinin dol olduğu tarih. | *4/30/2022* |
| ReferenceID | Yükseltmeler sırasında oluşan tüm işlemlere bağlantı. | *025d68a6-1bd6-42ab-9636-15e8d776a30e* |
| ProductQualifiers | Eklenti veya Deneme satın almalarını bilmek için tanımlayıcı. | *["Eklenti"]* |
| PromotionID | Yükseltme bilgilerini getirmek için kullanabileceğiniz tanımlayıcı. | *78bcf906-b945-4210-8818-cfb93caf12a1* |

>[!NOTE]
>Azure tüketiminizi tek kullanımlık satın alma mutabakat dosyanıza uzlaştırabilirsiniz. Bunu yapmak için günlük olarak derecelendirilmiş kullanım mutabakat dosyanıza gidin ve SubscriptionID'nizi bulun. Bu, Azure plan kimliğinizle ilişkili tüm maliyetleri görüntüler. Azure SubscriptionID'niz EntitlementID olarak gösterilir.
>

## <a name="how-to-connect-the-base-subscription-with-the-upgraded-subscription"></a>Yükseltilmiş aboneliğe temel abonelik nasıl bağlansın?

İlgili Başvuru kimliklerini bulmak için temel ürünün Abonelik Kimliğini ve bunları kullanarak ilişkili tüm işlemleri getirmeniz gerekir. Abonelik Kimliği ve Başvuru Kimliği ile birlikte, tek bir olayda meydana gelen tüm yükseltmeleri bebilirsiniz.

## <a name="next-steps"></a>Sonraki adımlar

- [Faturalama ve vergiler](billing.md)
