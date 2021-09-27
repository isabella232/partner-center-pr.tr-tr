---
title: Yeni ticari telco pay (siz git)
ms.topic: article
ms.date: 09/03/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Fazlalıklar için ödemeye olanak sağlayan teklif satın almak için yeni ticari deneyimler hakkında bilgi edinin.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e6ca40f44b97a9b60b48ccedbed7a3df7baad465
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129070228"
---
# <a name="introduction-new-commerce-overage-for-telco-pay-as-you-go"></a>Giriş: Telco pay-as-you-go için yeni ticari fazla veri

**Uygun roller**

- Yönetici aracısı
- Satış aracısı
- Genel yönetici

> [!NOTE]
> Yeni ticaret deneyimi değişiklikleri şu anda yalnızca Microsoft 365/Dynamics 365 yeni ticaret deneyimi teknik önizlemesinde yer alan iş ortakları tarafından kullanılabilir.

Lisans tabanlı bazı ürünler ayrılmış arama planlarına sahip hizmetleri içerir. Bu arama planları genellikle aylık dakikalar için lisans başına ayırma ile birlikte gelir ve genellikle lisans başına 120 olur. 

Geleneksel lisans tabanlı iş ortağı senaryolarında hizmet kullanımını aylık sınırların ötesinde etkinleştirmenin bir yolu yoktu. İletişim kredileri satın almak için 120 dakikadan fazla dakika veya doğrudan Microsoft'tan iletişim *kredileri* satın almak zorunda olan müşteriler.  Bu iletişim kredileri daha önce İş Ortağı Merkezi.

## <a name="using-new-commerce-telco-pay-as-you-go"></a>Yeni ticari telco pay'ı kullansanız da kullanma

Bu sınırlama yeni ticarette ele alınarak iş ortağının izin veren hizmetler için fazlalık özelliklerini etkinleştirmesine olanak sağlar. İş ortakları fazlalık özellikleri içeren teklifler satın alınabilir. Bu teklifler, *IncludeOverage* olan fiyat listesi etiketleri sütununda tanımlanır. Katalog SKU'su ayrıca SKU'nun fazla kullanılabilirlik özelliğini desteklediğini belirlemek için bir özellik içerir. İş ortakları yalnızca teklifleri satın alır ve sistem, maliyetle ilgili bir ücret ödemeden fazlalık abonelik yapılandırır ve yalnızca müşterinin kullanıcıları satın alınan teklifle birlikte ayrılan aylık arama dakikalarını karşılasa faturalama tahakkuk eder. 

İş ortakları, maliyet yönetimi özelliklerini ve özelliklerini kullanarak Azure portal fazla kullanım kullanımını takip ediyor olabilir. İş ortakları ayrıca, herhangi bir zamanda fazlalıkları devre dışı bırakmak veya devre dışı bırakmak isteyen iş ortakları, fazlalıkları Hiçbiri olarak ayarlama seçeneğine de sahip olur. 

İş ortakları, iş ortağı merkezi kataloğu ürün S SU'larını görüntüerek hangi ürünlerin fazla kullanılabilirlik özelliklerine sahip olduğunu tanımlayabilir. 

Fazlalık ile ürün satın alan iş ortakları, Abonelikleri Yönet sayfasında *FazlaLıkLarı* Yönet sayfasına erişerek fazlalıkları etkinleştirir. Bu, iş ortağının fazla kullanımı etkinleştirmesi ve fazla kullanımın akışa alınarak istenen tüketim aboneliğini ataması için olanak sağlar. İş ortağı, herhangi bir zamanda tüketim aboneliğini Yok olarak ataarak fazla kullanımı *kapatabilirsiniz.* 

İş ortakları fazlalık atar veya abonelikler listesinde *Fazla kullanılabilirlik* yönetimi özelliği tarafından devre dışı ekleyebilirsiniz. Bu, yalnızca iş ortağının fazla kullanılabilirlik sağlayan abonelikleri varsa erişilebilir. Aylık fazla çalışma ücretleri atanan aboneliğe tahakkukır ve iş ortakları mutabakat dosyasında tanımlanır. İş ortakları, azure maliyet yönetimi özelliklerini ziyaret ederek fazla kullanım Azure portal. 

## <a name="important-details-about-overage"></a>Fazlalık hakkında önemli ayrıntılar

Fazla kesintiye olanak sağlayan bir ürün SKU'su satın almak, iş ortağının müşterisinde fazla veri akışının otomatik olarak ayarlanmış olmasını sağlar. Buna ücretsiz bir Azure planı, ilişkili bir varsayılan Azure aboneliği ve özellikle fazla kullanım tüketimine yönelik bir abonelik oluşturma dahildir. İş ortakları Fazla kullanılabilirlik yönetimi'nin altında fazla verinin tahakkuk etmek istediğiniz aboneliği görebilir ve atayabilirsiniz.

Fazla çalışma ataması, kuralda *ilki tarafından* belirlenir. bir iş ortağı yeni müşteri için arama planları ile E5 satın aldı ise bu iş ortağının tüketim aboneliğine fazla kullanımı atanır. İkinci bir iş ortağı, arama planlarına sahip başka bir E5 kopyası satın aldı ise sistem ilk iş ortağının satın alma ve ataması ile ilgili bir karara varacaktır. İş ortakları, *abonelikler sayfasından* her zaman fazlalıkları yöneterek Yok'a fazla çalışma ataarak devre dışı bırakarak veya devre dışı bırakarak devre dışı *bırakabilirsiniz.*

Fazlalık ayarları müşteri başına hizmet başınadır. Müşteri farklı iş ortaklarından aynı fazla kullanılabilirliğe sahipse aynı anda yalnızca bir fazla çalışma aboneliği atanabilir. Fazla kesintinin bir iş ortağından diğerine değişmesi gerekirse, ilgili üç taraf da ilk olarak bunu kabul eder. Mevcut iş ortağının fazlalık özelliğini  Hiçbiri olarak ayarlaması, diğer iş ortağının aboneliğine fazlalık ayarlaması için kabul etti.

Telco pay as you go özellikleri için API desteği şunları içerir:

- İş ortağının bir SKU'nun fazla kullanılabilirlik özelliğine sahip olup olmadığını belirlemeye yardımcı olmak için SKU özellikleri
- Mevcut aboneliğe fazla kullanımı atamak veya fazla kullanımı  Yok olarak ayarlamak için yeni bir API
