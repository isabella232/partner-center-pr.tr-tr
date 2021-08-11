---
title: Lisansa dayalı mutabakat dosyaları
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Bu dosyalarda lisans tabanlı mutabakat dosyalarını okumayı İş Ortağı Merkezi. Bu makalede, lisans tabanlı mutabakat dosyanız içinde yer alan her alanın anlamı açıklanmıştır.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7bb6900ba34c99d497d8273e56e6385aa3bf55690c8729526a5e4c6a1e60ba28
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115694141"
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
| ResellerMpnId | Abonelik için kayıt kurumsal bayinin MPN tanımlayıcısı.  |
| OrderId | Microsoft faturalama platformunda bir siparişin benzersiz tanımlayıcısı. Destekle iletişim kurmak için siparişi belirlemek yararlı olabilir. Mutabakat için kullanılamaz. | *566890604832738111* |
| SubscriptionId | Microsoft faturalama platformunda bir aboneliğin benzersiz tanımlayıcısı. Destekle iletişim kurmak için aboneliği tanımlamak yararlı olabilir. Mutabakat için kullanılamaz. *Bu değer, İş Ortağı Yönetici **Konsolu'nın Abonelik** Kimliği ile aynı değildir. Bunun yerine **bkz. SyndicationPartnerSubscriptionNumber.*** | *usCBMgAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | Abonelikler için benzersiz tanımlayıcı. Bir müşterinin aynı plan için birden çok aboneliği olabilir. Bu sütun mutabakat dosyası analizi için önemlidir. Bu alan, İş Ortağı **Yönetici Konsolu'nu** Abonelik Kimliği ile eşler. | *fb977ab5-test-test-test-24c8d9591708* |
| OfferId | Benzersiz teklif tanımlayıcısı. Fiyat listesinde tanımlandığı gibi standart teklif tanımlayıcısı. *Bu değer fiyat **listesinden Teklif** Kimliği ile eşleşmez. Bunun **yerine durableOfferID'ye** bakın.* | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferId | Fiyat listesinde tanımlandığı gibi benzersiz dayanıklı teklif tanımlayıcısı. *Bu değer fiyat **listesinden Teklif** Kimliği ile eş değerdir.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | Fiyat listesinde tanımlandığı gibi müşteri tarafından satın alınan hizmet teklifi adı. | *Microsoft Office 365 (Plan E3)* |
| SubscriptionStartDate | UTC olarak abonelik başlangıç tarihi. Saat her zaman günün başlangıcıdır (00:00). Bu alan, siparişin gönderildikten sonra olduğu güne ayarlanır. **SubscriptionEndDate** ile birlikte, müşterinin hala aboneliğin ilk yılında olup olmadığını veya aboneliğin bir sonraki yıl için yenilenmesi olup olmadığını belirlemek için kullanılır. | *2/1/2019 0:00* |
| SubscriptionEndDate | UTC olarak abonelik bitiş tarihi. Saat her zaman günün başlangıcıdır (00:00). İş *ortağının faturalama  tarihiyle uyumlu olacak şekilde başlangıç* tarihini takip etmek için 12 ay artı x gün veya yenileme *tarihinden 12 ay sonra.* Yenilemede fiyatlar geçerli fiyat listesine güncelleştirilir. Otomatik yenileme öncesinde müşteri iletişimi gerekebilir. | *2/1/2019 0:00* |
| ChargeStartDate | Ücretlerin başlangıç günü. Saat her zaman günün başlangıcıdır (00:00). Müşteri lisans numaralarını değiştirirken *günlük ücretleri (provoka* ücretleri) hesaplamak için kullanılır. | *2/1/2019 0:00* |
| ChargeEndDate | Ücretlerin bitiş günü. Saat her zaman günün sonu, 23:59'dır. Müşteri lisans numaralarını değiştirirken *günlük ücretleri (provoka* ücretleri) hesaplamak için kullanılır. | *2/28/2019 23:59* |
| ChargeType | Ücret [veya ayarlama](recon-file-charge-types.md) türü. | Bkz. [ücret türleri.](recon-file-charge-types.md) |
| UnitPrice | Satın alma zamanında fiyat listesinde yayımlanan lisans başına fiyat. Bunun mutabakat sırasında faturalama sisteminize depolanmış bilgilerle eş olduğundan emin olun. | *6.82* |
| Miktar | Lisans sayısı. Bunun mutabakat sırasında faturalama sisteminize depolanmış bilgilerle eş olduğundan emin olun. | *2* |
| Miktar | Miktar için toplam fiyat. Tutar hesaplaması ile müşterileriniz için bu değeri hesaplama yönteminizin eş olup olamayrını kontrol etmek için kullanılır. | *13.32* |
| TotalOtherDiscount | Bu ücretlere uygulanan indirim tutarı. Yetkinliğe veya MAPS'e dahil edilen ürün lisansları veya teşvik için uygun yeni abonelikler de bu sütunda indirim tutarı içerir. | *2.32* |
| Ara toplam | Vergiden önceki toplam. İndirim durumunda alt toplamının beklenen toplamla eş olup olamay olduğunu denetler. | *11* |
| Vergi | Vergi tutarı ücreti. Marketin vergi kurallarına ve belirli koşullarına göre. | *0* |
| TotalForCustomer | Vergiden sonra toplam. Faturada vergi ödemesi olup olamaysanız denetler. | *11* |
| Para Birimi | Para birimi türü. Her faturalama varlığının yalnızca bir para birimi vardır. İlk faturanız ile eş olup olamay olduğunu kontrol edin. Ana faturalama platformu güncelleştirmelerinden sonra yeniden kontrol edin. | *EUR* |
| DomainName | Müşterinin etki alanı adı. Bu alan, ikinci faturalama döngüsüne kadar boş görünebilir. *Bu alanı müşteri için benzersiz bir tanımlayıcı olarak kullanma. Müşteri/iş ortağı, özel etki alanını veya varsayılan etki alanını Office 365 güncelleştirebilirsiniz.* | *example.onmicrosoft.com* |
| SubscriptionName | Abonelik takma adı. Takma ad belirtilmezse, İş Ortağı Merkezi **Adını kullanır.** | *PROJECT ONLINE* |
| SubscriptionDescription | Fiyat listesinde tanımlandığı gibi müşteri tarafından satın alınan hizmet teklifi adı. (Bu, OfferName ile aynı **bir alandır.)** | *PROJECT CLIENT OLMADAN PROJECT ONLINE PREMIUM* |
| BillingCycleType | Tek kullanımlık faturalama sıklığı.| *Aylık* |
