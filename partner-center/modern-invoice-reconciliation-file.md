---
title: CSP tek sefer satın almaları için dosya alanlarının mutabakatı
ms.topic: conceptual
ms.date: 01/29/2021
description: CsP'nizin tek bir kez satın alma mutabakat dosyasındaki tüm öğeler ve örnek İş Ortağı Merkezi hakkında bilgi alın.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: d5d404519c107a3e1f0e926451eef4935c993fbd
ms.sourcegitcommit: 90bf27df911b428b1222f483c32ba6367870e7c5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/04/2021
ms.locfileid: "115100714"
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
| CustomerCountry | Müşterinizin bulunduğu ülke. Bölgenize [uygun ülkelerin tam](./regional-authorization-overview.md) listesine bakın.  | *DE* |
| InvoiceNumber | Mutabakat dosyasıyla ilişkili fatura numarası.  | *G002297372* |
| MpnId | CSP iş ortağının MPN tanımlayıcısı. Daha fazla bilgi için [bkz. iş ortağına göre öğeleştirme.](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner) | *6034453* |
| ResellerMpnId | Abonelik için kayıt kurumsal bayinin MPN tanımlayıcısı. | *6048879* |
| OrderId | Microsoft faturalama platformunda bir siparişin benzersiz tanımlayıcısı. Destekle iletişim kurmak için siparişi belirlemek yararlı olabilir. Mutabakat için kullanılamaz. | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | Siparişin yerleştirilma tarihi (UTC). | *10/3/2020* |
| ProductId | Ürünün benzersiz tanımlayıcısı. | *DZH318Z0BNZ5* |
| SkuId | SKU benzersiz tanımlayıcısı. | *006G* |
| AvailabilityId | Kullanılabilirlik benzersiz tanımlayıcısı. | *DZH318Z08B80* |
| SkuName | SKU adı. | *Tablolar - LRS* |
| ProductName | Ürün adı. | *Tablolar* |
| ChargeType | Ücret [veya ayarlama](./recon-file-charge-types.md) türü. | *Yeni* |
| UnitPrice | Satın alma zamanında fiyat listesinde yayımlanan lisans başına fiyat. Bunun mutabakat sırasında faturalama sisteminize depolanmış bilgilerle eş olduğundan emin olun. | *0.045* |
| Miktar | Lisans sayısı. Bunun mutabakat sırasında faturalama sisteminize depolanmış bilgilerle eş olduğundan emin olun. | *1* |
| Ara toplam | Vergiden önceki toplam. Alt toplam, geçerli birim fiyatıyla çarpılan faturalanabilir miktara eşit olması gerekir. | *0* |
| TaxTotal | Vergi tutarı ücreti. Marketin vergi kurallarına ve belirli koşullarına göre. | *0* |
| Toplam | Toplam tutar, alt toplam artı vergi tutarına eşittir. | *0* |
| Para Birimi | Faturanız müşterinin para birimi bağlamında oluşturulur. Başka bir ifadeyle, farklı faturalanabilir para birimlerinden müşterilerle işlem yapılan bir iş ortağıysanız her müşterinin para birimi türü için bir fatura alırsınız.  | *EUR* |
| PriceAdjustmentDescription | Birim fiyatta ayarlamaların nedenleri. Ana nedenler bunlardır ancak geçerli birim fiyatı belirlemekle sınırlı değildir. | *["Yönetilen hizmetler için %15,0 İş ortağı tarafından kazanılan kredi"]* |
| PublisherName | Publisher için.  | *Microsoft* |
| PublisherId | Yayımcıyı tanımlamak İş Ortağı Merkezi benzersiz tanımlayıcı. | *Na* |
| SubscriptionDescription | Fiyat listesinde tanımlandığı gibi müşteri tarafından satın alınan hizmet teklifi adı. Bu sütun, OfferName ile aynı alandır. | *Azure planı* |
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
