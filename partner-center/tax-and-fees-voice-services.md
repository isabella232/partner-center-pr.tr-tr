---
title: Bölgesel PSTN hizmeti vergileri ve ücretleri
description: Voice Office 365 işlem yapan bir Microsoft 365 iş ortağı olarak PSTN hizmetleri için bölgesel vergiler, ücretler veya mevzuat gereksinimlerine tabi olabilirsiniz.
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 228534aff70db5c60116d408550361477da7302b784c78ea746cd2ae017c70a0
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115691676"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>Bölgesel vergiler, Kamu Anahtarlı Telefon Ağı (PTSN) hizmetleriyle ilgili düzenlemeler

**Uygun roller:** Genel yönetici | Kullanıcı yöneticisi | Yönetici aracısı

Bazı yargı alanlarındaki Kamu Anahtarlı Telefon Ağı (PSTN) hizmetleri, iş ortağı siparişlerini ve faturalamayı etkileyebilecek özel vergi ve mevzuat gereksinimlerine tabi olabilir. Bu Birleşik Devletler, Sesli Konferans, Arama Planları ve İletişim Kredileri de dahil olmak üzere Porto Riko, PSTN hizmetleri özel vergi ve mevzuat gereksinimlerine tabi olur. Microsoft, Birleşik Devletler ve Porto Riko'da PSTN hizmetlerini vergiler dahil olarak fiyatlarına sunar.  Benzersiz PSTN vergileri ve düzenlemeleri, Voice Office 365 işlem Microsoft 365 iş ortaklarını etkiler.  Bir iş ortağı bir Microsoft PSTN Hizmetinin fiyatını işaretlerse PSTN vergilerini ve ücretlerini hesaplamak ve geri almaktan sorumlu olabilir.

## <a name="partner-recommendations"></a>İş ortağı Öneriler

PSTN hizmetlerinin düzenlemesi, vergileri ve ücretleri ve diğer olası zararlarla ilgili olarak, kuruluş sorumluluğunu anlamak için vergi ve yasal sorumlular ile iletişim kurma.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Fatura Sunusu ve İş Ortağı Mutabakat Dosyası

Bulut Çözümü Sağlayıcısı PSTN ve Microsoft 365 Voice hizmetlerini içeren Birleşik Devletler, Porto Skype Kurumsal Riko ve Kanada'daki Microsoft 365 (CSP) faturaları ve CSP mutabakat dosyaları PSTN ve PSTN olmayan bileşenler için ayrı satır öğeleri sağlar.

Ayrıca CSP faturaları aşağıdaki dipnotları görüntüler:

* Görüntülenen fiyat Sesli Konferans ve Arama Planı Hizmetleri için bir ücrettir.  Geçerli tüm işlem vergileri, yalnızca ilgili vergiler içinde yapılan satışlar dışında gösterilen tutarın Birleşik Devletler.  ABD'de görüntülenen fiyat vergi dahildir çünkü Arama Planı ve Sesli Konferans Hizmetleri için bir ücret ve ücret ödememiz gereken vergiler ve ücretler için bir ücret içerir.  Sesli Konferans ve Arama Planı Hizmetleri, bunları sağlama yetkisine sahip Microsoft Bağlı Kuruluş tarafından hizmet sunar.  Ayrıntılar için bkz. [Microsoft Toplu Lisanslama](https://go.microsoft.com/fwlink/?LinkId=690247).

## <a name="reconciliation-file-example"></a>Mutabakat Dosyası Örneği

Office 365 Kurumsal E5, mutabakat dosyasında aynı adlara ve aynı kimliklere sahip iki satır öğesi olarak sunar, ancak her satır öğesinin benzersiz bir birim fiyatı vardır (örneğin: 28,40 ABD doları ve 2,00 ABD doları). Bu, vergileri Skype Kurumsal için Office 365 PSTN Konferans bileşenini birbirinden ayırıyor.

**İş Ortağı Mutabakatı #1 (sütun seçme):**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Kurumsal E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Döngü ücreti   |28.40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Kurumsal E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Döngü ücreti   |2,00   |

**İş Ortağı Mutabakatı örnek #2**

Microsoft 365 Küçük İşletmeler için Ses kanada'da bulunan ve CSP Faturasında birleştirilmiş ek PSTN vergilanabilir bileşenleri vardır (Office 365 E5'ye benzer şekilde, biri PSTN bileşenleri için, diğeri PSTN olmayan bileşenler için olmak Office 365 E5 gibi) iki satır öğe sunulmuştur.  Microsoft 365 Küçük İşletmeler için Ses IÇIN CSP Mutabakat dosyası tüm PSTN vergilenebilir bileşenlerini ayrı ayrı görüntüler (tek pstN bileşenleri .CSV veya API aracında birleştirilemez).  Mutabakat dosyasında bulunan müşteriler için sipariş ayrıntılarının ve faturalanmış tutarların toplamı CSP Faturası ile eşlaşacak.

## <a name="additional-resources"></a>Ek Kaynaklar
Diğer ayrıntılar için İş Ortakları Microsoft 365 [sitesini ziyaret](https://www.microsoft.com/microsoft-365/partners/) edin.

