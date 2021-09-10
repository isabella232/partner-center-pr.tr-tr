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
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961044"
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
| Bölge | Kullanımın geçerli olduğu bölge. Ücretler bölgeye göre farklılık gösterdiğinden, öncelikle veri aktarımlarına ücretler atamak için kullanılır. | *Asya Pasifik*, *Avrupa*, *Latin Amerika*, *Kuzey Amerika* |
| Sku | Bir teklif için benzersiz Microsoft tanımlayıcısı. | *7UD-00001* |
| Detaillineıtemıd | Belirli bir fatura döneminde bir hizmet veya kaynak için farklı oranlar için bir tanımlayıcı ve miktar. Azure katmanlı fiyatlandırma için, belirli bir faturalanabilir birim miktarına kadar bir ücret, daha sonra bu miktardan sonraki farklı bir ücret olabilir. | *1* |
| ConsumedQuantity | Raporlama dönemi boyunca tüketilen hizmet miktarı (saat veya GB gibi). Ayrıca, önceki raporlama dönemlerinden faturalandırılmamış kullanım dahil değildir. | *11* |
| IncludedQuantity | Teklifin bir parçası olarak dahil edilen birimler. Genellikle CSP 'de yoktur. | *0* |
| Fazla Agemiktarı | Teklifin bir parçası olarak dahil edilen birimler. Bunlar iş ortağı tarafından ödenmesi gerekir. **Tüketimi miktarı** eksi **ıncludedquantity** değerine eşit. | *11* |
| ListPrice | Aboneliğin başlangıç tarihinde yürürlükte fiyat sunun. | *$0,0808* |
| PretaxCharges | **Listprist** 'e eşit, en yakın bir değere yuvarlayarak, **overagequantity** ile çarpılır. | *$0,085* |
| TaxAmount | Ücret tahsil edilecek vergi tutarı. Marketin vergi kurallarına ve belirli koşullarına göre. | *0,08 ABD doları* |
| PostTaxTotal | Vergiden sonra toplam, vergi geçerli olduğunda. | *0,93 ABD doları* |
| Para Birimi | Para birimi türü. Her faturalama varlığının yalnızca bir para birimi vardır. İlk faturanız ve ardından ana faturalama platformu güncelleştirmelerinden sonra bu faturanın eş olup olamayrını kontrol edin. | *EUR* |
| PretaxEffectiveRate | Birim başına ön fiyat. **PretaxCharges değeri** **overageQuantity değerine bölünerek** en yakın sente yuvarlanır. | *0,08 ABD doları* |
| PostTaxEffectiveRate | Birim başına vergi sonrası fiyat. **PostTaxTotal değerine** eşit olarak **OverageQuantity değerine** bölünerek en yakın sente yuvarlanır. Veya **PretaxEffectiveRate** ile birim tutarı başına vergi oranına ek olarak en yakın sente yuvarlanmış olabilir. | *0,08 ABD doları* |
| ChargeType | Ücret [veya ayarlama](recon-file-charge-types.md) türü. | Bkz. [ücret türleri.](recon-file-charge-types.md) |
| CustomerId | Müşteri için GUID biçiminde benzersiz Microsoft tanımlayıcısı. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Müşterinin etki alanı adı. Bu alan, ikinci faturalama döngüsüne kadar boş görünebilir. | *example.onmicrosoft.com* |
| BillingCycleType | Zaman faturalama sıklığı.| **Aylık**  |
| Birim | Kaynak Adı **birimi.** | *GB veya* *SAAT* |
| CustomerBillableAccount | Microsoft faturalama platformunda benzersiz hesap tanımlayıcısı. | *1280018095* |
| UsageDate | Hizmet dağıtım tarihi. | *2/1/2019 0:00* |
| MeteredRegion | Bölge içindeki bir veri merkezinin konumunu tanımlar (bu değerin geçerli olduğu ve doldurul olduğu hizmetler için). | *Doğu Asya*, *Güney Doğu Asya*, *Kuzey Avrupa,* *Batı Avrupa,* *Orta Kuzey ABD*, *Orta Güney ABD* |
| MeteredService | **ServiceName** sütununda özel olarak tanımlanmayan tek tek Azure hizmet kullanımını tanımlar. Örneğin, veri aktarımları ServiceName *Microsoft Azure - Tüm Hizmetler* olarak **raporlandı.** | *AccessControl*, *CDN*, *Compute*, *Database*, *ServiceBus*, *Depolama* |
| MeteredServiceType | Azure hizmet **kullanımına ek açıklama sağlayan MeteredService** alanı için alt başlık. | *DIŞ* |
| Project | Hizmet örneği için müşteri tanımlı ad. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | Azure Service Bus sağlanan ve kullanılan bağlantıların sayısı. | *1.00000 Bağlantı / 30* gün (30 günlük bir ayda tek tek sağlanan bir bağlantınız varsa), *25 Bağlantı / 30 Gün – Kullanılır: 1.000000* (25 paket Service Bus bağlantınız varsa ve bu gün boyunca 1 kullandıysanız) |

## <a name="next-steps"></a>Sonraki adımlar

- [Lisans tabanlı mutabakat İş Ortağı Merkezi alanları anlama](license-based-recon-files.md)