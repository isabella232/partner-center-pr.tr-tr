---
title: Günlük olarak derecelendirilmiş kullanım mutabakat dosyaları
ms.topic: article
ms.date: 06/12/2020
description: Günlük olarak derecelendirilmiş kullanım mutabakat dosyalarını okuma hakkında bilgi İş Ortağı Merkezi. Mutabakat dosyasındaki belirli alanlar için açıklamalar içerir.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9b5daf91646324a9d4ace92d25736cfd0361ad6c
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147284"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>Günlük olarak değerlendirilen kullanım mutabakat dosyalarını okuma hakkında bilgi İş Ortağı Merkezi

**Uygulama:** İş Ortağı Merkezi | İş Ortağı Merkezi için Microsoft Cloud for US Government

**Uygun roller:** Yönetici aracısı | Faturalama yöneticisi | Satış aracısı | Yardım masası aracısı

Bu makalede, günlük olarak derecelendirilmiş kullanım mutabakat dosyalarının nasıl okunma durumu açıklanmıştır.

>[!NOTE]
>Günlük olarak derecelendirilmiş kullanımın api'de görünmesi İş Ortağı Merkezi veya API üzerinden erişilebilir olması 24 saat sürer.

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
| Tier2MpnId | Abonelik için kayıt satıcısının MPN tanımlayıcısı. |
| Faturanumarası | Belirtilen hareketin göründüğü fatura numarası. |
| ProductId | Ürün için tanımlayıcı. |
| SkuId | Belirli bir SKU için tanımlayıcı. |
| Kullanılabilirlik kimliği | Belirli bir SKU 'nun kullanılabilirliğine yönelik tanımlayıcı. Bu sütun, SKU 'nun verilen ülke, para birimi, sektör segmenti vb. için kullanılabilir olup olmadığını gösterir. |
| SkuName | Belirli bir SKU için başlık. |
| ProductName | Ürünün adı. |
| PublisherName | Yayımcının adı. |
| PublisherId | GUID biçimindeki yayımcının tanımlayıcısı. |
| Abonelik açıklaması | Fiyat listesinde tanımlandığı şekilde, müşteri tarafından satın alınan hizmet sunumunun adı. (Bu sütun, **Offername** ile özdeş bir alandır). |
| SubscriptionId | Microsoft faturalandırma platformunda bir abonelik için benzersiz tanımlayıcı. Mutabakat için kullanılmıyor. *Bu tanımlayıcı, iş ortağı yönetim konsolundaki **ABONELIK kimliğiyle** aynı değildir.* |
| ChargeStartDate | Fatura döngüsünün başlangıç tarihi (önceki fatura döngüsünden daha önce ücretlendirilmeyen kullanım verilerinin tarihlerini sunmadan hariç). Saat her zaman günün başlangıcıdır (00:00). |
| ChargeEndDate | Fatura döngüsünün bitiş tarihi (önceki fatura döngüsünden daha önce ücretlendirilmeyen kullanım verilerinin tarihlerini sunmadan hariç). Saat daima günün sonu, 23:59. |
| UsageDate | Hizmet kullanımı tarihi. |
| MeterType | Ölçüm türü. |
| MeterCategory | Kullanım için en üst düzey hizmet. |
| MeterId | Kullanılan ölçüm için tanımlayıcı. |
| MeterSubCategory | Hızı etkileyebilecek Azure hizmetinin türü. |
| MeterName | Tüketilmekte olan ölçüm için ölçü birimi. |
| MeterRegion | Bu sütun, MeterRegion 'in uygulanabilir ve doldurulmuş olduğu hizmetler için bölge içindeki bir veri merkezinin konumunu tanımlar. |
| Birim | Kaynak **adının** birimi. |
| ResourceLocation | Ölçüm 'in çalıştığı veri merkezi. |
| ConsumedService | Kullandığınız Azure platform hizmeti. |
| adlı yönetilen örnek, | Bir Azure çözümü için ilgili kaynakları tutan kapsayıcıyı temsil eder. |
| ResourceURI | Kullanılan kaynağın URI 'SI. |
| ChargeType | Ücretin veya düzeltmenin türü.  |
| UnitPrice | Satın alma sırasında fiyat listesinde yayınlanan lisans başına fiyat. Bu fiyatın, mutabakat sırasında faturalandırma sisteminizde depolanan bilgilerle eşleştiğinden emin olun. |
| Miktar | Lisans sayısı. Bu fiyatın, mutabakat sırasında faturalandırma sisteminizde depolanan bilgilerle eşleştiğinden emin olun. |
| UnitType | Ölçüm 'in ücretlendirildiği birim türü.  |
| BillingPreTaxTotal | Vergi öncesi fatura tutarının toplam sayısı.<br/> _**Billingpretaxtotal** = Floor (([ @EffectiveUnitPrice ]*[ @Quantity ]*[ @PCToBCExchangeRate ]), 2)_ |
| BillingCurrency | Müşterinin coğrafi bölgesindeki para birimi. |
| PricingPreTaxTotal | Vergiler dahil olmak üzere fiyatlandırma. |
| PricingCurrency | Fiyat listesindeki para birimi. |
| ServiceInfo1 | Verilen bir gün için sağlanan ve kullanılan Service Bus bağlantısı sayısı. |
| ServiceInfo2 | İsteğe bağlı hizmete özgü meta verileri yakalayan eski bir alan. |
| Etiketler | Kullanıcı tarafından belirlenen bir Azure kaynakları mantıksal organizasyonunu temsil eder. |
| AdditionalInfo | Diğer sütunlarda yer almayan ek bilgiler. |
| Efekt, BirimFiyat | Her türlü iskontolar, kazanılan kredi vb. dahil olmak üzere birim başına ücretlendirilen gerçek değer. |
| PCToBCExchangeRate | Ödeme para birimine fiyatlandırma para birimi için uygulanan döviz kuru. |
| PCToBCExchangeRateDate | Faturalandırma para birimine yönelik fiyatlandırma para biriminin belirlendiği tarih. |
| EntitlementId | Azure Abonelik Kimliğini temsil eder. |
| EntitlementDescription | Azure Abonelik Kimliğinin adını temsil eder. |
| PartnerEarnedCreditPercentage | Satır öğesi için PartnerEarnedCredit öğesini görüntüler. Kazanılan kredi yüzde 0 veya 15 olur |
| CreditPercentage | Azure Tüketim Kredisi'ne göre görüntülenir. Kazanılan kredi yüzde 0 veya 100 olur. |
| CreditType | Kredinin türü. Örneğin, **Azure Kredisi Uygulandı.** |
>[!NOTE]
>Günlük olarak derecelendirilmiş kullanımın normal olarak 24 saat içinde İş Ortağı Merkezi API aracılığıyla erişilebilir.


