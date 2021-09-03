---
title: Yeni ticari telco pay you go
ms.topic: article
ms.date: 08/30/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Fazlalıklar için ödemeye olanak sağlayan teklif satın almak için yeni ticari deneyimler hakkında bilgi edinin.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0f934b8d858c1fc30d0140d19fb0697ba6bd9001
ms.sourcegitcommit: 09d2c10491244775e656b48fce35b5648262ce59
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/03/2021
ms.locfileid: "123458310"
---
# <a name="introduction-new-commerce-overage-for-telco-pay-as-you-go"></a>Giriş: Telco ödemesi için yeni ticari fazla veri kesintisi

**Uygun roller**

- Yönetici aracısı
- Satış aracısı
- Genel yönetici

> [!Note] 
> Yeni ticaret deneyimi değişiklikleri şu anda yalnızca Microsoft 365/Dynamics 365 yeni ticaret deneyimi teknik önizlemesinde yer alan iş ortakları tarafından kullanılabilir.

Lisans tabanlı bazı ürünler ayrılmış arama planlarına sahip hizmetleri içerir. Bu arama planları genellikle aylık dakikalar için lisans başına ayırma ile birlikte gelir ve genellikle lisans başına 120 olur. 

Geleneksel lisans tabanlı iş ortağı senaryolarında hizmet kullanımını aylık sınırların ötesinde etkinleştirmenin bir yolu yoktu. İletişim kredileri veya doğrudan Microsoft'tan iletişim kredileri satın almak için 120 *dakikadan* fazla zaman ihtiyacı olan müşteriler.  Bu iletişim kredileri, daha önce İş Ortağı Merkezi.

## <a name="using-new-commerce-telco-pay-as-you-go"></a>Yeni ticari telco pay'ı kullansanız da kullanma ##

Bu sınırlama yeni ticarette ele alınarak iş ortağının izin veren hizmetler için fazlalık özelliklerini etkinleştirmesine olanak sağlar. İş ortakları fazlalık özellikleri içeren teklifler satın alınabilir. Bu teklifler, *IncludeOverage* olan fiyat listesi etiketleri sütununda tanımlanır. Katalog SKU'su, SKU'nun fazla kullanılabilirlik özelliğini desteklediğini belirlemek için bir özellik de içerir. İş ortakları yalnızca teklifleri satın alır ve sistem, maliyetle ilgili bir ücret ödemeden fazlalık abonelik yapılandırır ve yalnızca müşterinin kullanıcıları satın alınan teklifle birlikte ayrılan aylık arama dakikalarını karşılasa faturalama tahakkuk eder. 

İş ortakları, maliyet yönetimi özelliklerini ve özelliklerini kullanarak Azure portal fazla kullanım kullanımını takip ediyor olabilir. ayrıca iş ortakları, zaman zaman fazlalıkları  devre dışı bırakmak veya devre dışı bırakmak için fazlalıkları Hiçbiri olarak ayarlama seçeneğine de sahip olur.

İş ortakları, iş ortağı merkezi kataloğu ürün S SU'larını görüntüerek hangi ürünlerin fazla kullanılabilirlik özelliklerine sahip olduğunu tanımlayabilir. 

Fazlalık ile ürün satın alan iş ortakları, Abonelikleri Yönet sayfasında *FazlaLıkLarı* Yönet sayfasına erişerek fazlalıkları etkinleştirir. Bu, iş ortağının fazla kullanımı etkinleştirmesi ve fazla kullanımın akışa alınarak istenen tüketim aboneliğini ataması için olanak sağlar. İş ortağı, herhangi bir zamanda tüketim aboneliğini Yok olarak ataarak fazla kullanımı *kapatabilirsiniz.* 

İş ortakları fazlalık atar veya abonelikler listesinde *Fazla kullanılabilirlik* yönetimi özelliği tarafından devre dışı ekleyebilirsiniz. Bu, yalnızca iş ortağının fazla kullanılabilirlik sağlayan abonelikleri varsa erişilebilir. Aylık fazla çalışma ücretleri atanan aboneliğe tahakkukır ve iş ortakları mutabakat dosyasında tanımlanır. İş ortakları, azure maliyet yönetimi özelliklerini ziyaret ederek fazla kullanım Azure portal. 

## <a name="important-details-about-overage"></a>Fazlalık hakkında önemli ayrıntılar ##

Fazla kesintiye olanak sağlayan bir ürün SKU'su satın almak, iş ortağının müşterisinde fazla veri akışının otomatik olarak ayarlanmış olmasını sağlar. Buna ücretsiz bir Azure planı, ilişkili bir varsayılan Azure aboneliği ve özellikle fazla kullanım tüketimine yönelik bir abonelik oluşturma dahildir. İş ortakları Fazla kullanılabilirlik yönetimi'nin altında fazla verinin tahakkuk etmek istediğiniz aboneliği görebilir ve atayabilirsiniz.

Fazla çalışma ataması, kuralda *ilki tarafından* belirlenir. bir iş ortağı yeni müşteri için arama planları ile E5 satın aldı ise bu iş ortağının tüketim aboneliğine fazla kullanımı atanır. İkinci bir iş ortağı arama planlarına sahip başka bir E5 kopyası satın aldı ise, sistem ilk iş ortağının satın alma ve atamaya saygı gösterir. İş ortakları, *abonelikler sayfasından* her zaman fazlalıkları yöneterek Yok'a fazla çalışma ataarak devre dışı bırakarak veya devre dışı bırakarak devre dışı *bırakabilirsiniz.*

Fazlalık ayarları müşteri başına hizmet başınadır. Müşteri farklı iş ortaklarından aynı fazla kullanılabilirliğe sahipse aynı anda yalnızca bir fazla çalışma aboneliği atanabilir. Fazla kesintinin bir iş ortağından diğerine değişmesi gerekirse, ilgili üç taraf ilk olarak bunu kabul eder. Mevcut iş ortağının fazlalık özelliğini  Yok olarak ayarlaması, diğer iş ortağının aboneliğine fazla verim ayarlaması için kabul etti.

Telco pay as you go özellikleri için API desteği şunları içerir:

- İş ortağının bir SKU'nun fazla kullanılabilirlik özelliğine sahip olup olmadığını belirlemeye yardımcı olmak için SKU özellikleri
- Mevcut aboneliğe fazla kullanımı atamak veya fazla kullanımı  Yok olarak ayarlamak için yeni bir API
