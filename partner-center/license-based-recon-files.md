---
title: Lisansa dayalı mutabakat dosyaları
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Bu dosyalarda lisans tabanlı mutabakat dosyalarını okumayı İş Ortağı Merkezi. Bu makalede, lisans tabanlı mutabakat dosyanız içinde yer alan her alanın anlamı açıklanmıştır.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 041f0fadfea107027ae1d9796d235700e66e6834
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146587"
---
# <a name="understand-the-fields-in-partner-center-license-based-reconciliation-files"></a>Lisans tabanlı mutabakat İş Ortağı Merkezi alanları anlama

**Için geçerlidir:** İş Ortağı Merkezi | İş Ortağı Merkezi için Microsoft Cloud for US Government

**Uygun roller:** Genel yönetici | Kullanıcı yönetimi yönetici | Faturalama yöneticisi | Yönetici aracısı

Değişikliklerinizi müşterinin siparişlerine göre mu mutabakata varmak için mutabakat **Syndication_Partner_Subscription_Number**  gelen abonelik kimliğiyle karşılaştırma İş Ortağı Merkezi.

## <a name="fields-in-license-based-reconciliation-files"></a>Lisans tabanlı mutabakat dosyalarında alanlar

| Sütun | Açıklama | Örnek değer |
| ------ | ----------- | ------------ |
| PartnerId | Belirli bir faturalama varlığı için GUID biçiminde benzersiz tanımlayıcı. Mutabakat için gerekli değildir. Tüm satırlarda aynı. | *8ddd03642-test-test-test-46b58d356b4e* |
| CustomerId | Müşteri için GUID biçiminde benzersiz Microsoft tanımlayıcısı. | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| CustomerName | Müşterinin kuruluş adı ( İş Ortağı Merkezi. *Faturayı sistem bilgileriyle mutabık kılınan çok önemli bir alandır.* | *Test Müşterisi A* |
| MpnId | CSP iş ortağının MPN tanımlayıcısı. İş [ortağına göre öğeleştirmeye bakın.](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner) | *4390934* |
| Resellermpnıd | Abonelik için kayıt satıcısının MPN tanımlayıcısı.  |
| OrderId | Microsoft faturalandırma platformunda bir sipariş için benzersiz tanımlayıcı. Destek ile iletişim kurulurken sırayı belirlemek yararlı olabilir. Mutabakat için kullanılmıyor. | *566890604832738111* |
| SubscriptionId | Microsoft faturalandırma platformunda bir abonelik için benzersiz tanımlayıcı. Destek ile iletişim kurulurken aboneliği belirlemek yararlı olabilir. Mutabakat için kullanılmıyor. *Bu değer, Iş ortağı yönetim konsolundaki **ABONELIK kimliğiyle** aynı değildir. Lütfen bunun yerine **SyndicationPartnerSubscriptionNumber** bakın.* | *usCBMgAAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | Abonelikler için benzersiz tanımlayıcı. Müşterinin aynı plan için birden fazla aboneliği olabilir. Bu sütun, mutabakat Dosya Analizi için önemlidir. Bu alan, Iş ortağı yönetim konsolundaki **ABONELIK kimliğiyle** eşlenir. | *fb977ab5-test-test-test-24c8d9591708* |
| OfferId | Benzersiz teklif tanımlayıcısı. Fiyat listesinde tanımlandığı gibi standart teklif tanımlayıcısı. *Bu değer fiyat **listesinden Teklif Kimliği** ile eşleşmez. Bunun **yerine bkz. DurableOfferID.*** | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferId | Fiyat listesinde tanımlandığı gibi benzersiz dayanıklı teklif tanımlayıcısı. *Bu değer fiyat **listesinden Teklif** Kimliği ile eş değerdir.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | Fiyat listesinde tanımlandığı gibi müşteri tarafından satın alınan hizmet teklifi adı. | *Microsoft Office 365 (Plan E3)* |
| SubscriptionStartDate | UTC olarak abonelik başlangıç tarihi. Saat her zaman günün başlangıcıdır (00:00). Bu alan, siparişin gönderildikten sonra olduğu güne ayarlanır. **SubscriptionEndDate** ile birlikte, müşterinin hala aboneliğin ilk yılında olup olmadığını veya aboneliğin bir sonraki yıl için yenilenmesi olup olmadığını belirlemek için kullanılır. | *2/1/2019 0:00* |
| SubscriptionEndDate | UTC olarak abonelik bitiş tarihi. Saat her zaman günün başlangıcıdır (00:00). İş *ortağının faturalama  tarihiyle uyumlu olacak şekilde başlangıç tarihinden 12* ay artı x gün sonra veya yenileme *tarihinden 12 ay sonra.* Yenilemede fiyatlar geçerli fiyat listesine güncelleştirilir. Otomatik yenileme öncesinde müşteri iletişimi gerekebilir. | *2/1/2019 0:00* |
| ChargeStartDate | Ücretlerin başlangıç günü. Saat her zaman günün başlangıcıdır (00:00). Bir müşteri Lisans numaralarını değiştirdiğinde günlük ücretleri (*Pro rampaücreti* ) hesaplamak için kullanılır. | *2/1/2019 0:00* |
| ChargeEndDate | Ücretlerin bitiş günü. Saat daima günün sonu, 23:59. Bir müşteri Lisans numaralarını değiştirdiğinde günlük ücretleri (*Pro rampaücreti* ) hesaplamak için kullanılır. | *2/28/2019 23:59* |
| ChargeType | Ücret veya ayarlamanın [türü](recon-file-charge-types.md) . | Bkz. [ücretlendirme türleri](recon-file-charge-types.md). |
| UnitPrice | Satın alma sırasında fiyat listesinde yayınlanan lisans başına fiyat. Bunun, mutabakat sırasında faturalandırma sisteminizde depolanan bilgilerle eşleştiğinden emin olun. | *6,82* |
| Miktar | Lisans sayısı. Bunun, mutabakat sırasında faturalandırma sisteminizde depolanan bilgilerle eşleştiğinden emin olun. | *2* |
| Miktar | Miktar için fiyat toplamı. Tutar hesaplamasının müşterileriniz için bu değeri nasıl hesapladığını denetlemek için kullanılır. | *13,32* |
| TotalOtherDiscount | Bu ücretlere uygulanan indirim tutarı. Yetkinliğe veya MAPS'e dahil edilen ürün lisansları veya teşvik için uygun yeni abonelikler de bu sütunda indirim tutarı içerir. | *2.32* |
| Ara toplam | Vergiden önceki toplam. İndirim durumunda alt toplamının beklenen toplamla eş olup olamayrını denetler. | *11* |
| Vergi | Vergi tutarı ücreti. Marketin vergi kurallarına ve belirli koşullarına göre. | *0* |
| TotalForCustomer | Vergiden sonra toplam. Faturada vergi ödemesi olup olamaysanız denetler. | *11* |
| Para Birimi | Para birimi türü. Her faturalama varlığının yalnızca bir para birimi vardır. İlk faturanız ile eş olup olamay olduğunu kontrol edin. Ana faturalama platformu güncelleştirmelerinden sonra yeniden kontrol edin. | *EUR* |
| DomainName | Müşterinin etki alanı adı. Bu alan, ikinci faturalama döngüsüne kadar boş görünebilir. *Bu alanı müşteri için benzersiz bir tanımlayıcı olarak kullanmayın. Müşteri/iş ortağı, Office 365 portalı üzerinden özel etki alanını veya varsayılan etki alanını güncelleştirebilirsiniz.* | *example.onmicrosoft.com* |
| SubscriptionName | Abonelik takma adı. Takma ad belirtilmezse, İş Ortağı Merkezi **Adını kullanır.** | *PROJECT ONLINE* |
| Abonelik açıklaması | Fiyat listesinde tanımlandığı şekilde, müşteri tarafından satın alınan hizmet sunumunun adı. (Bu, **Offername** ile aynı alandır.) | *PROJECT CLIENT OLMADAN PROJECT ONLINE PREMIUM* |
| BillingCycleType | Bir kerelik faturalandırma sıklığı.| *Aylık* |
