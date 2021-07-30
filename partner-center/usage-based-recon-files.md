---
title: Kullanım tabanlı mutabakat dosyaları
ms.topic: article
ms.date: 06/08/2020
description: Iş Ortağı Merkezi 'nde kullanım tabanlı mutabakat dosyanızdaki tüm öğeler hakkında bilgi edinin. Birkaç örnek içerir.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3048bad7912f101e1c332e54eff981473f0f31d7
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114839660"
---
# <a name="understand-usage-based-reconciliation-files-and-their-specific-fields-in-partner-center"></a>Iş Ortağı Merkezi 'nde kullanım tabanlı karşılaştırma dosyalarını ve belirli alanlarını anlayın

**Uygun roller**: Hesap Yöneticisi | Faturalama yöneticisi

Ücretlerinizi bir müşterinin kullanımına karşı mutabık kılmak için **ResellerID**, **ResellerName** ve **Resellerbilurlableaccount** öğesini, iş ortağı MERKEZI 'ndeki **müşteri adı** ve **abonelik kimliği** ile karşılaştırma dosyasından karşılaştırın.

## <a name="fields-in-usage-based-reconciliation-files"></a>Kullanım tabanlı mutabakat dosyalarındaki alanlar

Aşağıdaki alanlar hangi hizmetlerin kullanıldığını ve oranını açıklamaktadır.

| Sütun | Açıklama | Örnek değer (ler) |
| ------ | ----------- | ------------ |
| İş ortağı kimliği | GUID biçiminde iş ortağı tanımlayıcısı. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | İş ortağının adı. | *Contoso, Ltd.* |
| Partnerbillableaccountıd | İş ortağı hesap tanımlayıcısı. | *1010578050* |
| CustomerCompanyName | Iş Ortağı Merkezi 'nde raporlanan müşterinin kuruluş adı. *Bu, faturanın sistem bilgileriyle mutabık olması için çok önemlidir.* | *Test müşterisi* |
| Mpnıd | Bulut Çözümü Sağlayıcısı (CSP) ortağının tanımlayıcısı Microsoft İş Ortağı Ağı (mpn). | *4390934* |
| Resellermpnıd | Abonelik için kayıt satıcısının MPN tanımlayıcısı.  |
| Faturanumarası | Belirtilen hareketin göründüğü fatura numarası. | *D020001IVK* |
| ChargeStartDate | Önceden ücretlendirilmeyen kullanım verilerinin (önceki fatura döngüsünden) tarihleri sunulmasının dışında, fatura döngüsünün başlangıç tarihi. Saat her zaman günün başlangıcıdır (00:00). | *2/1/2019 0:00* |
| ChargeEndDate | Fatura döngüsünün bitiş tarihi, önceden ücretlendirilmeyen kullanıma alınan kullanım verilerinin (önceki fatura döngüsünden) tarihleri sunulmasının dışında. Saat daima günün sonu, 23:59. | *2/28/2019 23:59* |
| SubscriptionId | Microsoft faturalandırma platformunda bir abonelik için benzersiz tanımlayıcı. Destek ile iletişim kurulurken aboneliği belirlemek yararlı olabilir. Mutabakat için kullanılmıyor. *Bu, Iş ortağı yönetim konsolundaki **ABONELIK kimliğiyle** aynı değildir.* | *usCBMgAAAAAAAAIA* |
| SubscriptionName | Hizmet sunumunun takma adı. | *Microsoft Azure* |
| Abonelik açıklaması | Hizmet sunumunun iş kolu. | *Microsoft Azure* |
| OrderID | Microsoft faturalandırma platformunda bir sipariş için benzersiz tanımlayıcı. Destek ile iletişim kurulurken aboneliği belirlemek yararlı olabilir. Mutabakat için kullanılmıyor. | *566890604832738111* |
| ServiceName | Söz konusu Azure hizmetinin adı. | *SANAL MAKINELER* |
| ServiceType | Belirli Azure hizmeti türü. | *Service Bus – bireysel veya paket*, *SQL Azure veritabanı – iş veya Web sürümü* |
| ResourceGuid | Tüm hizmet verileri ve fiyatlandırma yapısına özgü benzersiz tanımlayıcı. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| ResourceName | Azure kaynağının adı. | *Veri aktarımı (GB)*, *giden veri aktarımı (GB)* |
| Region | Kullanımın geçerli olduğu bölge. Ücretler bölgeye göre farklılık gösterdiğinden, öncelikle veri aktarımlarına ücretler atamak için kullanılır. | *Asya Pasifik*, *Avrupa*, *Latin Amerika*, *Kuzey Amerika* |
| Sku | Bir teklif için benzersiz Microsoft tanımlayıcısı. | *7UD-00001* |
| Detaillineıtemıd | Belirli bir fatura döneminde bir hizmet veya kaynak için farklı oranlar için bir tanımlayıcı ve miktar. Azure katmanlı fiyatlandırma için, belirli bir faturalanabilir birim miktarına kadar bir ücret, daha sonra bu miktardan sonraki farklı bir ücret olabilir. | *1* |
| ConsumedQuantity | Raporlama dönemi boyunca tüketilen hizmet miktarı (saat veya GB gibi). Ayrıca, önceki raporlama dönemlerinden faturalandırılmamış kullanım dahil değildir. | *11* |
| IncludedQuantity | Teklifin bir parçası olarak dahil edilen birimler. Genellikle CSP 'de yoktur. | *0* |
| Fazla Agemiktarı | Teklifin bir parçası olarak dahil edilen birimler. Bunlar iş ortağı tarafından ödenmesi gerekir. **Tüketimi miktarı** eksi **ıncludedquantity** değerine eşit. | *11* |
| ListPrice | Aboneliğin başlangıç tarihinde yürürlükte fiyat sunun. | *$0,0808* |
| PretaxCharges | **Listprist** 'e eşit, en yakın bir değere yuvarlayarak, **overagequantity** ile çarpılır. | *$0,085* |
| TaxAmount | Ücretlendirilen vergi tutarı. Pazar vergi kurallarına ve belirli koşullara göre. | *$0,08* |
| PostTaxTotal | Vergi geçerli olduğunda verginin toplam sayısı. | *$0,93* |
| Para Birimi | Para birimi türü. Her faturalandırma varlığının yalnızca bir para birimi vardır. İlk faturanızla ve sonra önemli faturalandırma platformu güncelleştirmelerinden sonra eşleşip eşleşmediğini denetleyin. | *EUR* |
| PretaxEffectiveRate | Birim başına ön vergi fiyatı. **Fazla ödeme miktarına** bölünen, en yakın ilayana yuvarlanmış olan **pretaxcharges** 'e eşit. | *$0,08* |
| PostTaxEffectiveRate | Birim başına vergi fiyatı. **Posttaxtotal** ile eşit olan, en yakın ilayana yuvarlanmış **miktarı fazla** Ya da, **PretaxEffectiveRate** değerine eşit ve birim miktarı başına vergi fiyatı, en yakın bir değere yuvarlanır. | *$0,08* |
| ChargeType | Ücret veya ayarlamanın [türü](recon-file-charge-types.md) . | Bkz. [ücretlendirme türleri](recon-file-charge-types.md). |
| CustomerId | Müşteri için GUID biçiminde benzersiz Microsoft tanımlayıcısı. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Müşterinin etki alanı adı. Bu alan, ikinci faturalandırma döngüsüne kadar boş görünebilir. | *example.onmicrosoft.com* |
| BillingCycleType | Saat faturalandırma sıklığı.| **Aylık**  |
| Birim | Kaynak **adının** birimi. | *GB* veya *saat* |
| CustomerBillableAccount | Microsoft faturalandırma platformunda benzersiz hesap tanımlayıcısı. | *1280018095* |
| UsageDate | Hizmet dağıtımının tarihi. | *2/1/2019 0:00* |
| MeteredRegion | Bölge içindeki bir veri merkezinin konumunu tanımlar (Bu değerin uygulanabilir ve doldurulmuş olduğu hizmetler için). | *Doğu Asya*, *güney Doğu Asya*, *Kuzey Avrupa*, *Batı Avrupa*, *Orta Kuzey ABD*, *Orta Güney ABD* |
| MeteredService | Her bir Azure hizmeti kullanımını, **ServiceName** sütununda özellikle tanımlanmadıkça tanımlar. örneğin, veri aktarımları **ServiceName** sütunundaki *Microsoft Azure-tüm hizmetler* olarak bildirilir. | *AccessControl*, *CDN*, *işlem*, *veritabanı*, *servicebus*, *Depolama* |
| MeteredServiceType | Azure hizmeti kullanımı hakkında ek açıklama sağlayan **MeteredService** alanı için alt başlık. | *DıŞARıDAKI* |
| Project | Hizmet örneği için müşteri tanımlı ad. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | belirli bir günde sağlanan ve kullanılan Azure Service Bus bağlantılarının sayısı. | *1,000000 bağlantı/30 gün* (30 günlük bir ayda tek bir sağlanan bağlantınız varsa), *25 bağlantı/30 gün – kullanılır: 1,000000* (Service Bus bir bağlantı sağlanan 25 paketiniz varsa ve bu gün boyunca 1 ' i kullandıysanız) |

## <a name="next-steps"></a>Sonraki adımlar

- [Iş Ortağı Merkezi lisans tabanlı mutabakat dosyalarındaki alanları anlayın](license-based-recon-files.md)