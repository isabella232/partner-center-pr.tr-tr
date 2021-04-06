---
title: Bölgesel PSTN hizmeti vergileri ve ücretleri
description: Sesli ürünleri transacts Microsoft 365 bir Office 365 iş ortağı olarak, PSTN Hizmetleri için bölgesel vergiler, ücretler veya yasal gereksinimlere tabi olabilirsiniz.
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 411932923e6bd35732e64521abe567f40f7499e9
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441498"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>Bölgesel vergiler, ortak anahtarlı telefon ağı (PTSN) Hizmetleri için yönetmelikler

**Uygun roller**

- Genel yönetici
- Kullanıcı yöneticisi
- Yönetim Aracısı

Bazı dairelerde ortak anahtarlı telefon ağı (PSTN) Hizmetleri, iş ortağı siparişi ve faturalamayı etkileyebilecek özel vergi ve mevzuata gereksinimlere tabi olabilir. Birleşik Devletler, Porto Riko da dahil olmak üzere, ses konferansı, çağrı planlarını ve Iletişim kredilerini içeren PSTN Hizmetleri, özel vergi ve yasal gereksinimlere tabidir. Birleşik Devletler ve Porto Riko 'da, Microsoft, PSTN hizmetlerini vergi dahil olarak ücretlidir.  Benzersiz PSTN vergileri ve düzenlemeleri, Office 365 iş ortakları deneyimidir Microsoft 365 ses ürünlerini etkileyecektir.  Bir iş ortağı bir Microsoft PSTN hizmetinin fiyatını işaretlerse, PSTN vergileri ve ücretleri hesaplanmaktan ve yeniden dağıtmanıza yardımcı olabilirler.

## <a name="partner-recommendations"></a>İş ortağı önerileri

Uygun bir şekilde, PSTN Hizmetleri mevzuata, vergiler ve ücretler ve diğer olası Borçlar hakkında kuruluşunuzun sorumluluğunu anlamak için vergi ve yasal Konseyi kullanım bilgilerinizi izleyin.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Fatura sunumu ve Iş ortağı mutabakatı dosyası

Skype Kurumsal PSTN ve Microsoft 365 Voice Services içeren Birleşik Devletler, Porto Riko ve Kanada 'da bulunan CSP faturaları ve CSP mutabakatı dosyaları, PSTN ve PSTN olmayan bileşenler için ayrı satır öğeleri sağlar.

Ayrıca, CSP faturalarında aşağıdaki dipnot görüntülenir:

* Gösterilecek Fiyat, sesli konferans ve çağrı planı Hizmetleri için ücretlendirilir.  Geçerli işlem vergileri, yalnızca Birleşik Devletler içinde yapılan satışlar dışında gösterilen tutardan ücretlendirilir.  ABD 'de, arama planı ve ses konferansı Hizmetleri için bir ücret ve ücretlendiriyoruz vergiler ve ücretler için ücret dahil olmak üzere, görüntülenen fiyata vergi dahildir.  Ses konferansı ve arama planı Hizmetleri, bunları sağlama yetkisine sahip Microsoft bağlı kuruluşlarına göre hizmet verir.  Ayrıntılar için bkz. [Microsoft Toplu Lisanslama](https://go.microsoft.com/fwlink/?LinkId=690247).

## <a name="reconciliation-file-example"></a>Karşılaştırma dosyası örneği

Office 365 Kurumsal E5, aynı adlara ve özdeş kimliklere sahip iki satırlık öğe olarak mutabakat dosyası sunar, ancak her satır öğesi benzersiz bir birim fiyatına sahiptir (örnek: $28,40 ve $2,00). Bu, Office 365 teklifinin Skype Kurumsal PSTN Konferansı bileşenini ayırır, böylece vergileri doğru bir şekilde uygulayabilirsiniz.

**İş ortağı mutabakatı örnek #1 (sütun Seç):**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Kurumsal E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Bisiklet ücreti   |28.40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Kurumsal E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Bisiklet ücreti   |2,00   |

**İş ortağı mutabakatı örnek #2**

Kanada 'da kullanılabilir Microsoft 365 İş ses, CSP faturasında birleştirilmiş ek PSTN vergilendirilebilir bileşenlere sahiptir (Office 365 E5 benzer, biri PSTN bileşenleri için, diğeri ise PSTN olmayan bileşenler için olmak üzere iki satırlık öğe sunulur).  Microsoft 365 İş Voice için CSP mutabakatı dosyası tüm PSTN vergilendirilebilir bileşenlerini ayrı ayrı görüntüler (bireysel PSTN bileşenleri içinde birleştirilecektir. CSV veya API aracı).  Mutabakat dosyasında bulunan müşterilere ait sipariş ayrıntılarının ve faturalandırılan tutarların toplamı, CSP faturasıyla eşleşmeyecektir.

## <a name="additional-resources"></a>Ek Kaynaklar
Daha fazla ayrıntı için [Iş ortakları sitesini Microsoft 365](https://www.microsoft.com/microsoft-365/partners/) ziyaret edin.

