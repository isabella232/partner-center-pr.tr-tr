---
title: Lisansa dayalı mutabakat dosyaları
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Iş Ortağı Merkezi 'nde lisans tabanlı mutabakatı dosyalarını okumayı öğrenin. Bu makalede lisans tabanlı keşfi dosyanızdaki her alanın anlamı açıklanmaktadır.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4c311de4a504785e15cefc7a93f1ee3da396ea7d
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441294"
---
# <a name="understand-the-fields-in-partner-center-license-based-reconciliation-files"></a>Iş Ortağı Merkezi lisans tabanlı mutabakat dosyalarındaki alanları anlayın

**Şunlara uygulanır**

- Microsoft Cloud for US Government için İş Ortağı Merkezi

**Uygun roller**

- Genel yönetici
- Kullanıcı Yönetimi Yöneticisi
- Faturalama yöneticisi
- Yönetim Aracısı

Değişikliklerinizin bir müşterinin siparişlerine karşı mutabakatını sağlamak için, **Syndication_Partner_Subscription_Number** mutabakat dosyasındaki, Iş Ortağı Merkezi 'NDEKI **abonelik kimliğiyle** karşılaştırın.

## <a name="fields-in-license-based-reconciliation-files"></a>Lisans tabanlı mutabakat dosyalarındaki alanlar

| Sütun | Açıklama | Örnek değer |
| ------ | ----------- | ------------ |
| İş ortağı kimliği | Belirli bir faturalandırma varlığı için GUID biçimindeki benzersiz tanımlayıcı. Mutabakat için gerekli değildir. Tüm satırlarda aynı. | *8ddd03642-test-test-test-46b58d356b4e* |
| CustomerId | Müşteri için GUID biçiminde benzersiz Microsoft tanımlayıcısı. | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| CustomerName | Iş Ortağı Merkezi 'nde raporlanan müşterinin kuruluş adı. *Fatura sistem bilgileriniz ile mutabık kılma için çok önemli alan.* | *Test müşterisi A* |
| Mpnıd | CSP iş ortağının MPN tanımlayıcısı. Bkz. [iş ortağı tarafından nasıl yapılır](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| Resellermpnıd | Abonelik için kayıt satıcısının MPN tanımlayıcısı.  |
| OrderId | Microsoft faturalandırma platformunda bir sipariş için benzersiz tanımlayıcı. Destek ile iletişim kurulurken sırayı belirlemek yararlı olabilir. Mutabakat için kullanılmıyor. | *566890604832738111* |
| SubscriptionId | Microsoft faturalandırma platformunda bir abonelik için benzersiz tanımlayıcı. Destek ile iletişim kurulurken aboneliği belirlemek yararlı olabilir. Mutabakat için kullanılmıyor. *Bu değer, Iş ortağı yönetim konsolundaki **ABONELIK kimliğiyle** aynı değildir. Lütfen bunun yerine **SyndicationPartnerSubscriptionNumber** bakın.* | *usCBMgAAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | Abonelikler için benzersiz tanımlayıcı. Müşterinin aynı plan için birden fazla aboneliği olabilir. Bu sütun, mutabakat Dosya Analizi için önemlidir. Bu alan, Iş ortağı yönetim konsolundaki **ABONELIK kimliğiyle** eşlenir. | *fb977ab5-test-test-test-24c8d9591708* |
| OfferId | Benzersiz teklif tanımlayıcısı. Fiyat listesinde tanımlandığı gibi standart teklif tanımlayıcısı. *Bu değer, Fiyat listesindeki **TEKLIF kimliğiyle** eşleşmez. Bunun yerine **Durableofferıd** bölümüne bakın.* | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| Durableofferıd | Fiyat listesinde tanımlandığı şekilde benzersiz dayanıklı teklif tanımlayıcısı. *Bu değer, Fiyat listesindeki **TEKLIF kimliğiyle** eşleşir.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | Fiyat listesinde tanımlandığı şekilde, müşteri tarafından satın alınan hizmet sunumunun adı. | *Microsoft Office 365 (plan E3)* |
| SubscriptionStartDate | Abonelik başlangıç tarihi. Saat her zaman günün başlangıcıdır (00:00). Bu alan, Sipariş gönderildikten sonraki güne ayarlanır. Şunları öğrenmek için **SubscriptionEndDate** ile kullanılır: müşteri aboneliğin ilk yılında hala içindeyse veya abonelik aşağıdaki yıl için yenilenmişse. | *2/1/2019 0:00* |
| SubscriptionEndDate | Abonelik bitiş tarihi. Saat her zaman günün başlangıcıdır (00:00). *Başlangıç tarihinden sonraki 12 ay artı **x** gün sonra* , iş ortağının faturalandırma tarihi veya *yenileme tarihinden itibaren 12 ay* ile hizalanacaktır. Yenileme sırasında fiyatlar geçerli fiyat listesine güncelleştirilir. Müşteri iletişimi otomatik yenilemeyle önceden gerekli olabilir. | *2/1/2019 0:00* |
| ChargeStartDate | Ücretlerin başlangıç günü. Saat her zaman günün başlangıcıdır (00:00). Bir müşteri Lisans numaralarını değiştirdiğinde günlük ücretleri (*Pro rampaücreti* ) hesaplamak için kullanılır. | *2/1/2019 0:00* |
| ChargeEndDate | Ücretlerin bitiş günü. Saat daima günün sonu, 23:59. Bir müşteri Lisans numaralarını değiştirdiğinde günlük ücretleri (*Pro rampaücreti* ) hesaplamak için kullanılır. | *2/28/2019 23:59* |
| ChargeType | Ücret veya ayarlamanın [türü](recon-file-charge-types.md) . | Bkz. [ücretlendirme türleri](recon-file-charge-types.md). |
| UnitPrice | Satın alma sırasında fiyat listesinde yayınlanan lisans başına fiyat. Bunun, mutabakat sırasında faturalandırma sisteminizde depolanan bilgilerle eşleştiğinden emin olun. | *6,82* |
| Miktar | Lisans sayısı. Bunun, mutabakat sırasında faturalandırma sisteminizde depolanan bilgilerle eşleştiğinden emin olun. | *2* |
| Miktar | Miktar için fiyat toplamı. Tutar hesaplamasının müşterileriniz için bu değeri nasıl hesapladığını denetlemek için kullanılır. | *13,32* |
| TotalOtherDiscount | Bu ücretlere uygulanan indirim miktarı. Bir uzmanlığa veya MAPS 'e dahil edilen ürün lisansları veya bir teşvik için uygun yeni abonelikler, bu sütunda bir indirim tutarı da içerecektir. | *2,32* |
| Ara toplam | Vergi öncesi toplam. Bir indirimle, ara toplamın beklenen toplamyla eşleşip eşleşmediğini denetler. | *11* |
| Vergi | Vergi tutarı ücreti. Pazar vergi kurallarına ve belirli koşullara göre. | *0* |
| TotalForCustomer | Vergi sonrası toplam. Faturada ücretlendirildiğiniz bir vergi olup olmadığını denetler. | *11* |
| Para Birimi | Para birimi türü. Her faturalandırma varlığının yalnızca bir para birimi vardır. İlk faturanızdan eşleşip eşleşmediğini denetleyin. Ana faturalandırma platformu güncelleştirmelerinden sonra yeniden kontrol edin. | *EUR* |
| DomainName | Müşterinin etki alanı adı. Bu alan, ikinci faturalandırma döngüsüne kadar boş görünebilir. *Bu alanı müşteri için benzersiz bir tanımlayıcı olarak kullanmayın. Müşteri/iş ortağı, Office 365 portalından gösterim veya varsayılan etki alanını güncelleştirebilir.* | *example.onmicrosoft.com* |
| SubscriptionName | Abonelik takma adı. Takma ad belirtilmemişse, Iş Ortağı Merkezi, **Offername** kullanır. | *PROJECT ONLINE* |
| Abonelik açıklaması | Fiyat listesinde tanımlandığı şekilde, müşteri tarafından satın alınan hizmet sunumunun adı. (Bu, **Offername** ile aynı alandır.) | *PROJECT CLIENT OLMADAN PROJECT ONLINE PREMIUM* |
| BillingCycleType | Bir kerelik faturalandırma sıklığı.| *Aylık* |