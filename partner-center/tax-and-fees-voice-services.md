---
title: Bölgesel PSTN hizmeti vergileri ve ücretleri
description: sesli ürünler Microsoft 365 bir Office 365 iş ortağı olarak, PSTN hizmetleri için bölgesel vergiler, ücretler veya yasal gereksinimlere tabi olabilirsiniz.
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 85eefb49cf62c4bcfa5533683abd8ddb0e854463
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961516"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>Bölgesel vergiler, ortak anahtarlı telefon ağı (PTSN) Hizmetleri için yönetmelikler

**Uygun roller**: genel yönetici | Kullanıcı Yöneticisi | Yönetim Aracısı

Bazı dairelerde ortak anahtarlı telefon ağı (PSTN) Hizmetleri, iş ortağı siparişi ve faturalamayı etkileyebilecek özel vergi ve mevzuata gereksinimlere tabi olabilir. Birleşik Devletler, Porto Riko da dahil olmak üzere, ses konferansı, çağrı planlarını ve Iletişim kredilerini içeren PSTN Hizmetleri, özel vergi ve yasal gereksinimlere tabidir. Birleşik Devletler ve Porto Riko 'da, Microsoft, PSTN hizmetlerini vergi dahil olarak ücretlidir.  benzersiz PSTN vergileri ve yönetmelikleri, Office 365 iş ortakları Microsoft 365 ses ürünlerini etkiler.  Bir iş ortağı bir Microsoft PSTN hizmetinin fiyatını işaretlerse, PSTN vergileri ve ücretleri hesaplanmaktan ve yeniden dağıtmanıza yardımcı olabilirler.

## <a name="partner-recommendations"></a>iş ortağı Öneriler

Uygun bir şekilde, PSTN Hizmetleri mevzuata, vergiler ve ücretler ve diğer olası Borçlar hakkında kuruluşunuzun sorumluluğunu anlamak için vergi ve yasal Konseyi kullanım bilgilerinizi izleyin.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Fatura sunumu ve Iş ortağı mutabakatı dosyası

Bulut Çözümü Sağlayıcısı (CSP) Birleşik Devletler, porto riko ve kanada 'daki Skype Kurumsal pstn ve Microsoft 365 Voice services dahil olmak üzere) faturalar ve CSP mutabakatı dosyaları, pstn ve pstn olmayan bileşenlere yönelik ayrı satır öğeleri sağlar.

Ayrıca, CSP faturalarında aşağıdaki dipnot görüntülenir:

* Gösterilecek Fiyat, sesli konferans ve çağrı planı Hizmetleri için ücretlendirilir.  Geçerli işlem vergileri, yalnızca Birleşik Devletler içinde yapılan satışlar dışında gösterilen tutardan ücretlendirilir.  ABD 'de, arama planı ve ses konferansı Hizmetleri için bir ücret ve ücretlendiriyoruz vergiler ve ücretler için ücret dahil olmak üzere, görüntülenen fiyata vergi dahildir.  Ses konferansı ve arama planı Hizmetleri, bunları sağlama yetkisine sahip Microsoft bağlı kuruluşlarına göre hizmet verir.  Ayrıntılar için bkz. [Microsoft Toplu Lisanslama](https://go.microsoft.com/fwlink/?LinkId=690247).

## <a name="reconciliation-file-example"></a>Karşılaştırma dosyası örneği

Office 365 Kurumsal E5, aynı adlara ve özdeş kimliklere sahip iki satırlık öğe olarak mutabakat dosyası gösterir, ancak her satır öğesi benzersiz bir birim fiyatına sahiptir (örnek: $28,40 ve $2,00). bu, Office 365 teklifinin Skype Kurumsal PSTN konferans bileşenini ayırır, böylece vergileri doğru bir şekilde uygulayabilirsiniz.

**İş ortağı mutabakatı örnek #1 (sütun Seç):**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Kurumsal E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Bisiklet ücreti   |28.40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Kurumsal E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Bisiklet ücreti   |2,00   |

**İş ortağı mutabakatı örnek #2**

kanada 'da kullanılabilir Microsoft 365 Küçük İşletmeler için Ses, CSP faturasında birleştirilmiş ek PSTN vergilendirilebilir bileşenlere sahiptir (Office 365 E5 benzer şekilde, bir tane, pstn bileşenleri için, diğeri ise pstn olmayan bileşenler için olmak üzere iki satırlık öğe sunulur).  Microsoft 365 Küçük İşletmeler için Ses CSP mutabakatı dosyasında tüm pstn vergilendirilebilir bileşenleri ayrı ayrı görüntülenir (bireysel pstn bileşenleri, .CSV veya apı aracında birleştirilmeyecektir).  Mutabakat dosyasında bulunan müşterilere ait sipariş ayrıntılarının ve faturalandırılan tutarların toplamı, CSP faturasıyla eşleşmeyecektir.

## <a name="additional-resources"></a>Ek Kaynaklar
daha fazla ayrıntı için [iş ortakları sitesini Microsoft 365](https://www.microsoft.com/microsoft-365/partners/) ziyaret edin.

