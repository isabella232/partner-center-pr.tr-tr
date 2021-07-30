---
title: Günlük olarak derecelendirilmiş kullanım mutabakat dosyaları
ms.topic: article
ms.date: 06/12/2020
description: Günlük olarak derecelendirilmiş kullanım mutabakat dosyalarını okuma hakkında bilgi İş Ortağı Merkezi. Mutabakat dosyasındaki belirli alanlar için açıklamalar içerir.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9b9c422124227804dcf1ac70286a73155d2e71d3
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114844080"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>Günlük olarak değerlendirilen kullanım mutabakat dosyalarını okuma hakkında bilgi İş Ortağı Merkezi

**Uygulama:** İş Ortağı Merkezi | İş Ortağı Merkezi için Microsoft Cloud for US Government

**Uygun roller:** Yönetici aracısı | Faturalama yöneticisi | Satış aracısı | Yardım masası aracısı

Bu makalede, günlük olarak derecelendirilmiş kullanım mutabakat dosyalarının nasıl okunma durumu açıklanmıştır.

>[!NOTE]
>Günlük olarak derecelendirilmiş kullanımın api'de görünmesi İş Ortağı Merkezi veya API üzerinden erişilemediklerinden 24 saat sürer.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Günlük olarak derecelendirilmiş kullanım mutabakat dosyalarında alanlar

| Sütun | Açıklama |
| ------ | ----------- |
| PartnerId | GUID biçiminde iş ortağı tanımlayıcısı. |
| PartnerName | İş ortağının adı. |
| CustomerId | Müşteri için GUID biçiminde benzersiz Microsoft tanımlayıcısı. |
| CustomerName | Müşterinin kuruluş adı, İş Ortağı Merkezi. *Bu sütun, faturayı sistem bilgileriyle mu mutabakata varmak için önemlidir.* |
| CustomerDomainName | Müşterinin etki alanı adı. |
| CustomerCountry | Müşterinin bulunduğu ülke. |
| MpnId | CSP iş ortağının MPN tanımlayıcısı. |
| Tier2MpnId | Abonelik için kayıt kurumsal bayinin MPN tanımlayıcısı. |
| InvoiceNumber | Belirtilen işlemi görünen fatura numarası. |
| ProductId | Ürünün tanımlayıcısı. |
| SkuId | Belirli bir SKU için tanımlayıcı. |
| AvailabilityId | Belirli bir SKU'nun kullanılabilirliği için tanımlayıcı. Bu sütunda SKU'nun belirli bir ülkede, para biriminde, sektör segmentinde vb. satın alınıp alınamayabiliyor olduğu gösterir. |
| SkuName | Belirli bir SKU'nun başlığı. |
| ProductName | Ürünün adı. |
| PublisherName | Yayımcının adı. |
| PublisherId | YAYıMCının GUID biçimindeki tanımlayıcısı. |
| SubscriptionDescription | Fiyat listesinde tanımlandığı gibi müşteri tarafından satın alınan hizmet teklifi adı. (Bu sütun OfferName ile aynı **alandır).** |
| SubscriptionId | Microsoft faturalama platformunda bir aboneliğin benzersiz tanımlayıcısı. Mutabakat için kullanılamaz. *Bu tanımlayıcı, iş ortağı yönetici **konsolunda Abonelik Kimliği** ile aynı değildir.* |
| ChargeStartDate | Faturalama döngüsünün başlangıç tarihi (önceki faturalama döngüsünden daha önce ücret ödememiş olan gizli kullanım verilerini sunmak dışında). Saat her zaman günün başlangıcıdır (00:00). |
| ChargeEndDate | Faturalama döngüsünün bitiş tarihi (önceki faturalama döngüsünden daha önce ücret ödememiş olan gizli kullanım verilerini gösterirken olduğu tarihler hariç). Saat her zaman günün sonu, 23:59'dır. |
| UsageDate | Hizmet kullanım tarihi. |
| MeterType | Ölçüm türü. |
| MeterCategory | Kullanım için en üst düzey hizmet. |
| MeterId | Kullanılan ölçümün tanımlayıcısı. |
| MeterSubCategory | Hızı etkileyebilecek Azure hizmeti türü. |
| MeterName | Tüketilen ölçüm için ölçü birimi. |
| MeterRegion | Bu sütun, MeterRegion'ın geçerli ve doldurulmuş olduğu hizmetler için bölge içindeki bir veri merkezinin konumunu tanımlar. |
| Birim | Kaynak Adı **birimi.** |
| ResourceLocation | Ölçümün çalıştır bulunduğu veri merkezi. |
| ConsumedService | Kullanılan Azure platform hizmeti. |
| adlı yönetilen örnek, | Azure çözümü için ilgili kaynakları tutan bir kapsayıcıyı temsil eder. |
| ResourceURI | Kullanılan kaynağın URI'si. |
| ChargeType | Ücretin veya düzeltmenin türü.  |
| UnitPrice | Satın alma zamanında fiyat listesinde yayımlanan lisans başına fiyat. Bu fiyatın mutabakat sırasında faturalama sisteminize depolanmış bilgilerle eş olduğundan emin olun. |
| Miktar | Lisans sayısı. Bu fiyatın mutabakat sırasında faturalama sisteminize depolanmış bilgilerle eş olduğundan emin olun. |
| Unittype | Ölçümün ücret ödemesi yapılan birim türü.  |
| BillingPreTaxTotal | Vergilerden önceki toplam fatura tutarı.<br/> _**BillingPreTaxTotal** = FLOOR(([ @EffectiveUnitPrice ]*[ @Quantity ]*[ @PCToBCExchangeRate ]), 2)_ |
| BillingCurrency | Müşterinin coğrafi bölgesinde para birimi. |
| PricingPreTaxTotal | Vergiler eklenmeden önce fiyatlandırma. |
| PricingCurrency | Fiyat listesindeki para birimi. |
| ServiceInfo1 | verilen bir gün için sağlanan ve kullanılan Service Bus bağlantısı sayısı. |
| ServiceInfo2 | İsteğe bağlı hizmete özgü meta verileri yakalayan eski bir alan. |
| Etiketler | Kullanıcı tarafından belirlenen bir Azure kaynakları mantıksal organizasyonunu temsil eder. |
| AdditionalInfo | Diğer sütunlarda yer almayan ek bilgiler. |
| Efekt, BirimFiyat | Her türlü iskontolar, kazanılan kredi vb. dahil olmak üzere birim başına ücretlendirilen gerçek değer. |
| PCToBCExchangeRate | ödeme para birimine fiyatlandırma para birimi için Exchange ücret uygulandı. |
| PCToBCExchangeRateDate | Faturalandırma para birimine yönelik fiyatlandırma para biriminin belirlendiği tarih. |
| EntitlementId | Azure abonelik KIMLIĞINI temsil eder. |
| EntitlementDescription | Azure abonelik KIMLIĞININ adını temsil eder. |
| PartnerEarnedCreditPercentage | Satır öğesi için Partnerearnedkredisini görüntüler. Kazanılan kredi 0 veya %15 olacaktır |
| CreditPercentage | Azure tüketim kredisi ' nı görüntüler. Kazanılan kredi 0 veya yüzde 100 olacaktır. |
| CreditType | Kredi türü. Örneğin, **Azure kredisi uygulandı.** |
>[!NOTE]
>Günlük olarak derecelendirilen kullanımlar, Iş Ortağı Merkezi 'nde veya API aracılığıyla erişilecek 24 saat sürer.


