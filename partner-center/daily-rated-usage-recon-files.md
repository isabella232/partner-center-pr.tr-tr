---
title: Günlük olarak derecelendirilen kullanım mutabakatı dosyaları
ms.topic: article
ms.date: 06/12/2020
description: Iş Ortağı Merkezi 'nde günlük dereceli kullanım mutabakatı dosyalarını nasıl okuyacağınızı öğrenin. Keşfi dosyasındaki belirli alanların açıklamalarını içerir.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 531f28ae2bceed2d854c6fb139d0abb837a047b5
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712248"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>Iş Ortağı Merkezi 'nde günlük dereceli kullanım mutabakatı dosyalarını nasıl okuyacağınızı öğrenin

**Şunlara uygulanır**

- İş Ortağı Merkezi
- Microsoft Cloud for US Government için İş Ortağı Merkezi

**Uygun roller**

- Yönetim Aracısı
- Faturalama yöneticisi
- Satış Aracısı
- Yardım Masası Aracısı

Bu makalede, günlük dereceli kullanım mutabakatı dosyalarının nasıl okunacağı açıklanır.

>[!NOTE]
>Günlük olarak derecelendirilen kullanımlar, Iş Ortağı Merkezi 'nde veya API aracılığıyla erişilecek 24 saat sürer.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Günlük olarak derecelendirilen kullanım mutabakatı dosyalarındaki alanlar

| Sütun | Açıklama |
| ------ | ----------- |
| İş ortağı kimliği | GUID biçiminde iş ortağı tanımlayıcısı. |
| PartnerName | İş ortağının adı. |
| CustomerId | Müşteri için GUID biçiminde benzersiz Microsoft tanımlayıcısı. |
| CustomerName | Iş Ortağı Merkezi 'nde raporlanan müşterinin kuruluş adı. *Bu sütun, faturayı sistem bilgileriniz ile mutabık kılma açısından önemlidir.* |
| CustomerDomainName | Müşterinin etki alanı adı. |
| CustomerCountry | Müşterinin bulunduğu ülke. |
| Mpnıd | CSP iş ortağının MPN tanımlayıcısı. |
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
| EntitlementId | Azure abonelik KIMLIĞINI temsil eder. |
| EntitlementDescription | Azure abonelik KIMLIĞININ adını temsil eder. |
| PartnerEarnedCreditPercentage | Satır öğesi için Partnerearnedkredisini görüntüler. Kazanılan kredi 0 veya %15 olacaktır |
| CreditPercentage | Azure tüketim kredisi ' nı görüntüler. Kazanılan kredi 0 veya yüzde 100 olacaktır. |
| CreditType | Kredi türü. Örneğin, **Azure kredisi uygulandı.** |
>[!NOTE]
>Günlük olarak derecelendirilen kullanımlar, Iş Ortağı Merkezi 'nde veya API aracılığıyla erişilecek 24 saat sürer.


