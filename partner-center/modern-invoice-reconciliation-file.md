---
title: CSP tek seferlik satın almalar için dosya alanlarının mutabakatı
ms.topic: conceptual
ms.date: 01/29/2021
description: CsP'nizin tek bir kez satın alma mutabakat dosyasındaki tüm öğeler ve örnek İş Ortağı Merkezi hakkında bilgi alın.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: d5d404519c107a3e1f0e926451eef4935c993fbd
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961035"
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
| CustomerName | Müşterinin kuruluş adı, raporlandığı İş Ortağı Merkezi. Bu sütun, faturayı sistem bilgileriyle mu mutabakata varmak için önemlidir. | *Johnny Modern Cust DE2* |
| CustomerDomainName | Müşterinin etki alanı adı. | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | Müşterinizin bulunduğu ülke. Bölgenize [uygun ülkelerin tam](./regional-authorization-overview.md) listesine bakın.  | *DE* |
| InvoiceNumber | Mutabakat dosyasıyla ilişkili fatura numarası.  | *G002297372* |
| MpnId | CSP iş ortağının MPN tanımlayıcısı. Daha fazla bilgi için [bkz. iş ortağına göre öğeleştirme.](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner) | *6034453* |
| ResellerMpnId | Abonelik için kayıt kurumsal bayinin MPN tanımlayıcısı. | *6048879* |
| OrderId | Microsoft faturalama platformunda bir siparişin benzersiz tanımlayıcısı. Destekle iletişim kurmak için siparişi belirlemek yararlı olabilir. Mutabakat için kullanılamaz. | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | Siparişin yerleştiril olduğu UTC tarihi. | *10/3/2020* |
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
| PublisherName | Publisher ürünü.  | *Microsoft* |
| PublisherId | Yayımcıyı tanımlamak İş Ortağı Merkezi benzersiz tanımlayıcı. | *NA* |
| SubscriptionDescription | Fiyat listesinde tanımlandığı gibi müşteri tarafından satın alınan hizmet teklifi adı. Bu sütun, OfferName ile özdeş bir alandır. | *Azure planı* |
| SubscriptionId | Microsoft faturalandırma platformunda bir abonelik için benzersiz tanımlayıcı. Mutabakat için kullanılmıyor. Bu tanımlayıcının iş ortağı yönetim konsolundaki abonelik KIMLIĞIYLE aynı olmadığına unutmayın. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | Bir aboneliğin fatura döneminin başladığı tarih. | *9/1/2020* |
| ChargeEndDate | Bir aboneliğin fatura döneminin sona erdiği tarih. | *30.09.2020* |
| Tertermbillingcycle | Satın alma sırasında aboneliğe devam etme taahhüdünde geçen süre. | *Depolanan veri (GB/ay)* |
| Efekt, BirimFiyat | Fatura döngüsünün maliyetini hesaplamak için eşit olarak dağıtılmış birim fiyatı. İndirimler, faturalandırma günlerindeki ayarlamalar ve diğer faktörler, geçerli birim fiyatını belirlemektir. Daha fazla bilgi için bkz. [geçerli birim fiyat hesaplaması](./effective-unit-price-calculation.md).  | *0,03825* |
| UnitType | Ölçerin ücretlendirildiği birim türü. | *1 GB/Ay* |
| AlternateId | Başvurulan sipariş satırı öğesinin alternatif KIMLIĞI. | *6dc5c039750a* |
| BillableQuantity | Faturalandırılan toplam miktar.  | *0,005001* |
| BillingFrequency | Satın alma sırasında seçilen faturalandırma planı. | *YANA*  |
| PricingCurrency | Fiyat listesindeki para birimi. | *USD* |
| PCToBCExchangeRate | Ödeme para birimine fiyatlandırma para birimi için uygulanan döviz kuru. | *0,846202666* |
| PCToBCExchangeRateDate | Faturalandırma para birimine yönelik fiyatlandırma para biriminin belirlendiği tarih. | *30.09.2020* |
| MeterDescription | Ölçüm açıklaması.  | *Tablolar-LRS depolanan veri (GB/ay)* |
| ReservationOrderId | Rezervasyon sipariş KIMLIĞI. | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | Kredi açıklaması. | *Azure tüketim kredisi* |
| SubscriptionStartDate | Bir aboneliğin satın alındığı tarih. | *5/1/2021* |
| SubscriptionEndDate | Aboneliğin süresi dolan tarih. | *4/30/2022* |
| Referenceıd | Yükseltmeler sırasında oluşan tüm işlemlere olan bağlantı. | *025d68a6-1bd6-42AB-9636-15e8d776a30e* |
| Productniteleyiciler | Eklentinin veya deneme satın alımlarınızı bilen tanımlayıcı. | *["Eklenti"]* |
| Promotionıd | Yükseltmenin bilgilerini getirmek için kullanılacak tanımlayıcı. | *78bcf906-b945-4210-8818-cfb93caf12a1* |

>[!NOTE]
>Azure tüketiminizi tek seferlik satın alma keşfi dosyanızda mutabık hale getirebilirsiniz. Bunu yapmak için, günlük derecelendirdiğiniz kullanım keşfi dosyasına gidin ve SubscriptionID 'nizi arayın. Bu, Azure plan KIMLIĞINIZLE ilişkili tüm maliyetleri görüntüler. Azure SubscriptionID 'niz EntitlementID olarak gösterilir.
>

## <a name="how-to-connect-the-base-subscription-with-the-upgraded-subscription"></a>Temel abonelik yükseltilen abonelikle nasıl bağlanır?

İlgili başvuru kimliklerini bulmak ve ilişkili tüm işlemleri getirmek için bunları kullanmak için temel ürünün abonelik KIMLIĞINI kullanmanız gerekir. Abonelik KIMLIĞI ve başvuru KIMLIĞIYLE birlikte, tek bir olayda gerçekleşen tüm yükseltmeleri bağlayabilirsiniz.

## <a name="next-steps"></a>Sonraki adımlar

- [Faturalama ve vergiler](billing.md)
