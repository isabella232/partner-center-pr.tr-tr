---
title: Bölgesel PSTN hizmeti vergileri ve ücretleri
description: Microsoft 365 Voice ürünlerinde işlem yapan bir Office 365 iş ortağı olarak PSTN hizmetleri için bölgesel vergilere, ücretlere veya mevzuat gereksinimlerine tabi olabilirsiniz.
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 80cb5503323f483c13c983375559baf70f9d0b6f
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854732"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>Bölgesel vergiler, Kamu Anahtarlı Telefon Ağı (PTSN) hizmetleriyle ilgili düzenlemeler

**Uygun roller:** Genel yönetici | Kullanıcı yöneticisi | Yönetici aracısı

Bazı yargı alanlarındaki Kamu Anahtarlı Telefon Ağı (PSTN) hizmetleri, iş ortağı siparişlerini ve faturalamayı etkileyebilecek özel vergi ve mevzuat gereksinimlerine tabi olabilir. Bu Birleşik Devletler, Sesli Konferans, Arama Planları ve İletişim Kredileri de dahil olmak üzere Porto Riko, PSTN hizmetleri özel vergi ve mevzuat gereksinimlerine tabi olur. Microsoft, Birleşik Devletler ve Porto Riko'da PSTN hizmetlerini vergiler dahil olarak fiyatlarına sunar.  Benzersiz PSTN vergileri ve düzenlemeleri, Voice ürünleri üzerinde işlem Microsoft 365 Office 365 iş ortaklarını etkiler.  Bir iş ortağı bir Microsoft PSTN Hizmetinin fiyatını işaretlerse PSTN vergilerini ve ücretlerini hesaplamak ve geri almaktan sorumlu olabilir.

## <a name="partner-recommendations"></a>İş Ortağı Önerileri

PSTN hizmetlerinin düzenlemesi, vergileri ve ücretleri ve diğer olası zararlarla ilgili olarak, kuruluş sorumluluğunu anlamak için vergi ve yasal sorumlular ile iletişim kurma.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Fatura Sunusu ve İş Ortağı Mutabakat Dosyası

Skype Kurumsal PSTN ve Microsoft 365 Voice hizmetlerini içeren Birleşik Devletler, Porto Riko ve Kanada'daki CSP faturaları ve CSP mutabakat dosyaları PSTN ve PSTN olmayan bileşenler için ayrı satır öğeleri sağlar.

Ayrıca CSP faturaları aşağıdaki dipnotları görüntüler:

* Görüntülenen fiyat Sesli Konferans ve Arama Planı Hizmetleri için bir ücrettir.  Geçerli tüm işlem vergileri, yalnızca ilgili vergiler içinde yapılan satışlar dışında gösterilen tutarın Birleşik Devletler.  ABD'de görüntülenen fiyat vergi dahildir çünkü Arama Planı ve Sesli Konferans Hizmetleri için bir ücret ve ücret ödememiz gereken vergiler ve ücretler için bir ücret içerir.  Ses konferansı ve arama planı Hizmetleri, bunları sağlama yetkisine sahip Microsoft bağlı kuruluşlarına göre hizmet verir.  Ayrıntılar için bkz. [Microsoft Toplu Lisanslama](https://go.microsoft.com/fwlink/?LinkId=690247).

## <a name="reconciliation-file-example"></a>Karşılaştırma dosyası örneği

Office 365 Kurumsal E5, aynı adlara ve özdeş kimliklere sahip iki satırlık öğe olarak mutabakat dosyası sunar, ancak her satır öğesi benzersiz bir birim fiyatına sahiptir (örnek: $28,40 ve $2,00). Bu, Office 365 teklifinin Skype Kurumsal PSTN Konferansı bileşenini ayırır, böylece vergileri doğru bir şekilde uygulayabilirsiniz.

**İş ortağı mutabakatı örnek #1 (sütun Seç):**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Kurumsal E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Bisiklet ücreti   |28.40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Kurumsal E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Döngü ücreti   |2,00   |

**İş Ortağı Mutabakatı örnek #2**

Microsoft 365 Business Voice,CSP Faturasında birleştirilmiş ek PSTN vergilanabilir bileşenlerine sahiptir (Office 365 E5'e benzer şekilde, biri PSTN bileşenleri için, diğeri PSTN olmayan bileşenler için olmak sıralanmış iki satır öğe sunulmaktadır).  Microsoft 365 Business Voice için CSP Mutabakat dosyası tüm PSTN vergilenebilir bileşenlerini ayrı ayrı görüntüler (tek tek PSTN bileşenleri içinde birleştirilemez). CSV veya API aracı).  Mutabakat dosyasında bulunan müşteriler için sipariş ayrıntılarının ve faturalanmış tutarların toplamı CSP Faturası ile eşlaşacak.

## <a name="additional-resources"></a>Ek Kaynaklar
Diğer ayrıntılar için İş Ortakları Microsoft 365 [sitesini ziyaret](https://www.microsoft.com/microsoft-365/partners/) edin.

