---
title: Kullanım tabanlı mutabakat dosyaları
ms.topic: article
ms.date: 06/08/2020
description: Iş Ortağı Merkezi 'nde kullanım tabanlı mutabakat dosyanızdaki tüm öğeler hakkında bilgi edinin. Birkaç örnek içerir.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: fc31915660b6a82954daee5fcc8fb2d5292e725c
ms.sourcegitcommit: 837d3c5b52ab056b2b761cd85eb2426f56b62614
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/12/2021
ms.locfileid: "109795015"
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
| CustomerCompanyName | Iş Ortağı Merkezi 'nde raporlanan müşterinin kuruluş adı. *Sistem bilgileriniz ile faturayı mutabık kılma konusunda çok önemli.* | *Test müşterisi* |
| MpnId | CSP iş ortağının MPN tanımlayıcısı. | *4390934* |
| ResellerMpnId | Abonelik için kayıt kurumsal bayinin MPN tanımlayıcısı.  |
| InvoiceNumber | Belirtilen işlemi görünen fatura numarası. | *D020001IVK* |
| ChargeStartDate | Daha önce ücret ödememiş olan gizli kullanım verilerini (önceki fatura döngüsünden) sunmak dışında faturalama döngüsünün başlangıç tarihi. Saat her zaman günün başlangıcıdır (00:00). | *2/1/2019 0:00* |
| ChargeEndDate | Daha önce ücret ödememiş olan gizli kullanım verilerini (önceki fatura döngüsünden) sunmak dışında faturalama döngüsünün bitiş tarihi. Saat her zaman günün sonu, 23:59'dır. | *2/28/2019 23:59* |
| SubscriptionId | Microsoft faturalama platformunda bir aboneliğin benzersiz tanımlayıcısı. Destekle iletişim kurmak için aboneliği tanımlamak yararlı olabilir. Mutabakat için kullanılamaz. *Bu, İş Ortağı Yönetici **Konsolu'nın Abonelik** Kimliği ile aynı değildir.* | *usCBMgAAAAAAIA* |
| SubscriptionName | Hizmet teklifi için takma ad. | *Microsoft Azure* |
| SubscriptionDescription | Hizmet teklifi iş hattı. | *Microsoft Azure* |
| OrderID | Microsoft faturalama platformunda bir siparişin benzersiz tanımlayıcısı. Destekle iletişim kurmak için aboneliği tanımlamak yararlı olabilir. Mutabakat için kullanılamaz. | *566890604832738111* |
| ServiceName | Söz konusu Azure hizmetinin adı. | *SANAL MAKINELER* |
| ServiceType | Belirli bir Azure hizmeti türü. | *Service Bus – Bireysel veya Paket,* *SQL Azure veritabanı – İş veya Web Edition* |
| ResourceGuid | Tüm hizmet verileri ve fiyatlandırma yapısı için belirli benzersiz tanımlayıcı. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| ResourceName | Azure kaynağının adı. | *Gelen Veri Aktarımı (GB)*, *Veri Aktarımı (GB)* |
| Region | Kullanımın uygulandığı bölge. Hızlar bölgeye göre farklılık göstere olduğundan öncelikli olarak veri aktarımları için hız atamak için kullanılır. | *Asya Pasifik*, *Avrupa*, *Latin Amerika*, *Kuzey Amerika* |
| Sku | Teklif için benzersiz Microsoft tanımlayıcısı. | *7UD-00001* |
| Detaillineıtemıd | Belirli bir fatura döneminde bir hizmet veya kaynak için farklı oranlar için bir tanımlayıcı ve miktar. Azure katmanlı fiyatlandırma için, belirli bir faturalanabilir birim miktarına kadar bir ücret, daha sonra bu miktardan sonraki farklı bir ücret olabilir. | *1* |
| ConsumedQuantity | Raporlama dönemi boyunca tüketilen hizmet miktarı (saat veya GB gibi). Ayrıca, önceki raporlama dönemlerinden faturalandırılmamış kullanım dahil değildir. | *11* |
| IncludedQuantity | Teklifin bir parçası olarak dahil edilen birimler. Genellikle CSP 'de yoktur. | *0* |
| Fazla Agemiktarı | Teklifin bir parçası olarak dahil edilen birimler. Bunlar iş ortağı tarafından ödenmesi gerekir. **Tüketimi miktarı** eksi **ıncludedquantity** değerine eşit. | *11* |
| ListPrice | Aboneliğin başlangıç tarihinde yürürlükte fiyat sunun. | *$0,0808* |
| PretaxCharges | **Listprist** 'e eşit, en yakın bir değere yuvarlayarak, **overagequantity** ile çarpılır. | *$0,085* |
| TaxAmount | Ücretlendirilen vergi tutarı. Pazar vergi kurallarına ve belirli koşullara göre. | *0,08 ABD doları* |
| PostTaxTotal | Vergi geçerli olduğunda toplam vergi sonrası. | *0,93 ABD doları* |
| Para Birimi | Para birimi türü. Her faturalama varlığının yalnızca bir para birimi vardır. İlk faturanız ve ardından ana faturalama platformu güncelleştirmelerinden sonra bu faturanın eş olup olamayrını kontrol edin. | *EUR* |
| PretaxEffectiveRate | Birim başına ön fiyat. **PretaxCharges değeri** **overageQuantity değerine bölünerek** en yakın sente yuvarlanır. | *0,08 ABD doları* |
| PostTaxEffectiveRate | Birim başına vergi sonrası fiyat. **PostTaxTotal değerine** eşit olarak **OverageQuantity değerine bölünerek** en yakın sente yuvarlanır. Veya **PretaxEffectiveRate** ile birim tutarı başına vergi oranına ek olarak en yakın sente yuvarlanmış olabilir. | *0,08 ABD doları* |
| ChargeType | Ücret [veya ayarlama](recon-file-charge-types.md) türü. | Bkz. [ücret türleri.](recon-file-charge-types.md) |
| CustomerId | Müşteri için GUID biçiminde benzersiz Microsoft tanımlayıcısı. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Müşterinin etki alanı adı. Bu alan, ikinci faturalandırma döngüsüne kadar boş görünebilir. | *example.onmicrosoft.com* |
| BillingCycleType | Saat faturalandırma sıklığı.| **Aylık**  |
| Birim | Kaynak **adının** birimi. | *GB* veya *saat* |
| CustomerBillableAccount | Microsoft faturalandırma platformunda benzersiz hesap tanımlayıcısı. | *1280018095* |
| UsageDate | Hizmet dağıtımının tarihi. | *2/1/2019 0:00* |
| MeteredRegion | Bölge içindeki bir veri merkezinin konumunu tanımlar (Bu değerin uygulanabilir ve doldurulmuş olduğu hizmetler için). | *Doğu Asya*, *güney Doğu Asya*, *Kuzey Avrupa*, *Batı Avrupa*, *Orta Kuzey ABD*, *Orta Güney ABD* |
| MeteredService | Her bir Azure hizmeti kullanımını, **ServiceName** sütununda özellikle tanımlanmadıkça tanımlar. Örneğin, veri aktarımları **ServiceName** sütunundaki *Microsoft Azure-tüm hizmetler* olarak bildirilir. | *AccessControl*, *CDN*, *işlem*, *veritabanı*, *ServiceBus*, *depolama* |
| MeteredServiceType | Azure hizmeti kullanımı hakkında ek açıklama sağlayan **MeteredService** alanı için alt başlık. | *DıŞARıDAKI* |
| Project | Hizmet örneği için müşteri tanımlı ad. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | Verilen bir gün için sağlanan ve kullanılan Azure Service Bus bağlantısı sayısı. | *1,000000 bağlantı/30 gün* (30 günlük bir ayda tek bir sağlanan bağlantınız varsa), *25 bağlantı/30 gün – kullanılır: 1,000000* (Service Bus bir bağlantı sağlanan 25 paketiniz varsa ve bu gün boyunca 1 ' i kullandıysanız) |

## <a name="next-steps"></a>Sonraki adımlar

- [Iş Ortağı Merkezi lisans tabanlı mutabakat dosyalarındaki alanları anlayın](license-based-recon-files.md)