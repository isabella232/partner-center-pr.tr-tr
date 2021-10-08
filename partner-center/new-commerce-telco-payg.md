---
title: Yeni ticari telco pay-as-you-go
ms.topic: article
ms.date: 09/03/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Uzun süre ödemeye olanak sağlayan teklif satın almak için yeni ticari deneyimler hakkında bilgi edinin.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 44e999987021ca450da1eb24cbd310a3e35b0873
ms.sourcegitcommit: cf73ea8967a285cc14b281e7b938962c02b18e67
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/08/2021
ms.locfileid: "129689709"
---
# <a name="introduction-new-commerce-overage-for-telco-pay-as-you-go"></a>Giriş: Telco pay-as-you-go için yeni ticari fazla veri

**Uygun roller**

- Yönetici aracısı
- Satış aracısı
- Genel yönetici

> [!NOTE]
> Yeni ticaret deneyimi değişiklikleri şu anda yalnızca Microsoft 365/Dynamics 365 yeni ticaret deneyimi teknik önizlemesinde yer alan iş ortakları tarafından kullanılabilir.

Bazı lisans tabanlı ürünler, ayrılmış arama planlarına sahip hizmetler içerir. Bu hizmetler genellikle aylık dakika başına lisans başına ayırmayı (genellikle lisans başına 120) içerir. 

Geleneksel lisans tabanlı iş ortağı senaryolarında hizmet kullanımını aylık sınırların ötesinde etkinleştirmenin bir yolu yoktu. İletişim kredileri satın almak için 120 dakikadan fazla dakika veya doğrudan Microsoft'tan iletişim *kredileri* satın almak zorunda olan müşteriler.  Bu iletişim kredileri, daha önce İş Ortağı Merkezi.

## <a name="using-new-commerce-telco-pay-as-you-go"></a>Yeni ticari telco kullan-kullan-kullan-kullan ını kullanma

Bu sınırlama yeni ticarette ele alınarak iş ortağının izin veren hizmetler için fazlalık özelliklerini etkinleştirmesine olanak sağlar. İş ortakları fazlalık özellikleri içeren teklifler satın alınabilir. Bu teklifler, *IncludeOverage* olan fiyat listesi etiketleri sütununda tanımlanır. Katalog SKU'su ayrıca SKU'nun fazla kullanılabilirlik özelliğini desteklediğini belirlemek için bir özellik içerir. İş ortakları yalnızca teklifleri satın alır ve sistem maliyet ödemeden bir fazlalık aboneliği yapılandırır ve yalnızca müşterinin kullanıcıları satın alınan teklifle birlikte ayrılan aylık arama dakikalarını karşılasa faturalama tahakkuk eder. 

İş ortakları, hangi ürün SKU'larının fazla çalışma özelliklerine sahip olduğunu şu şekilde tanımlayabilir: 

- İş ortağı merkezi kataloğu ürün SU'larını görüntüleme
- Etiketler sütunundaki **includesOverage'a göre yeni** ticari fiyat listesini filtreleme

Fazla kullanılabilirlik özelliğine sahip ürünler satın alan iş ortakları, Abonelikleri Yönet sayfasında **Fazla** Kullanılabilirlik Yönetimi sayfasına erişerek ürüne olanak sağlar. Fazla kullanım yönetimi arabirimi, iş ortağının fazla kullanım ücretlerini hangi Azure aboneliğine atayacaklarını etkinleştirmelerini ve atamalarını sağlar. İş ortağı, herhangi bir zamanda tüketim aboneliğini Yok olarak ataarak fazla kullanımı *kapatabilirsiniz.* 

> [!NOTE]
> Fazla kullanım yönetimi için bir Azure planı oluşturma gerekir. Varsayılan olarak iş ortakları kendi korumalı alan hesaplarını kullanarak Azure planları sağlayamaz. Bunu kendi korumalı alan hesaplarıyla yapması gereken iş ortaklarının erişim için başvurması gerekir. Daha fazla kaynak, Azure planı korumalı [alan belgelerinde bulunabilir.](/partner-center/develop/test-and-debug#azure-plan)

İş ortakları fazlalık atar veya abonelikler listesinde *Fazla kullanılabilirlik* yönetimi özelliği tarafından devre dışı ekleyebilirsiniz. Bu, yalnızca iş ortağının fazla kullanılabilirlik sağlayan abonelikleri varsa erişilebilir. Aylık fazla çalışma ücretleri atanan aboneliğe tahakkukır ve iş ortakları mutabakat dosyasında tanımlanır. İş ortakları, azure maliyet yönetimi özelliklerini kullanarak fazla kullanım Azure portal. 

İş ortakları, maliyet yönetimi özelliklerini ve özelliklerini kullanarak Azure portal fazla kullanım kullanımını takip ediyor olabilir. 

## <a name="pricing-and-margins"></a>Fiyatlandırma ve marjlar

Müşteri sahip olduğu plan için ayrılan arama dakikası miktarını kullandığında, telco kullanabiliyorsa aylık kullanım temel alarak faturalandır. İş ortakları, bu ücretlerin fiyatlandırmalarını Microsoft Teams Telefon [sitesinden indirebilir.](https://www.microsoft.com/microsoft-teams/voice-calling) İş ortakları çeşitli **arama planlarının** ücretlerini indirmek ve görüntülemek için bu sayfada aramak istediğiniz Fiyatları görüntüle sayfasına gidebilir. 

CsP hedef kitlesi için fiyatlandırma ve arama planı fazla kullanımı ücretleri belirli değildir veya azaltılamaz, kanaldan bağımsızdır. Fazlalık ücretleri için CSP indirimleri veya marjları yoktur. 

## <a name="important-details-about-overage"></a>Fazlalık hakkında önemli ayrıntılar

- Fazlalık özellikleri içeren lisans tabanlı bir ürün SKU'su satın almak yalnızca lisans tabanlı ürünü satın alar. İş ortaklarının satın alma sonrasında abonelik yönetimi sayfasına gidip Fazla kullanılabilirliği yönet'e tıklayarak satın alma sonrasında başka bir **adım atları gerekir**
- Lisans tabanlı satın alma sonrasında fazlalıkları yalnızca işlem ortağı için Yönetici Aracılar etkinleştir olabilir. 
- Fazla kullanımın etkinleştirilmesi, özellikle fazla kullanım tüketimi için ücretsiz bir Azure planı ve ilişkili varsayılan Azure aboneliği **1** aboneliğini oluşturmanızı sağlar. Azure planı zaten varsa fazla kullanım etkinleştirerek yeni aboneliği mevcut Azure planı altında oluşturabilirsiniz. İş ortakları, Fazla kullanılabilirlik yönetimi sayfasındaki diğer abonelikleri her zaman görüntüleme veya yeniden **atama işlemleri için kullanılabilir.** Henüz Azure planında (eski Azure) yer alan müşterilerin fazla kullanım için azure planına geçişleri gerekir.

Fazla çalışma ataması, kuralda *ilki tarafından* belirlenir. bir iş ortağı yeni müşteri için arama planları ile E5 satın aldı ise bu iş ortağının tüketim aboneliğine fazla kullanımı atanır. İkinci bir iş ortağı arama planlarına sahip başka bir E5 kopyası satın aldı ise, sistem ilk iş ortağının satın alma ve atamaya saygı gösterir. İş ortakları, *abonelikler sayfasından* her zaman fazlalıkları yöneterek Yok'a fazla çalışma ataarak devre dışı bırakarak veya devre dışı bırakarak devre dışı *bırakabilirsiniz.*

Fazlalık ayarları müşteri başına hizmet başınadır. Aynı anda yalnızca bir fazla çalışma aboneliği atanabilir. Fazla kesintinin bir iş ortağından diğerine değişmesi gerekirse, ilgili üç taraf ilk olarak bunu kabul eder. Mevcut iş ortağının fazlalık özelliğini  Hiçbiri olarak ayarlaması, diğer iş ortağının aboneliğine fazlalık ayarlaması için kabul etti.

## <a name="telco-pay-as-you-go-apis"></a>Telco-as-you-go API'leri

- [SKU özellikleri,](/partner-center/develop/product-resources#sku) iş ortağının bir SKU'nun fazla kullanımı olanaklıp olanaklı olmadığını belirlemeye yardımcı olmak için *bir consumptionType* özelliği içerir
- [Müşteriniz için](/partner-center/develop/get-subscription-overage) şu anda herhangi bir fazlalık ayar olup o anda ayarlansa da fazlalık elde etmek
- [Müşterinin fazla kullanımlarını](/partner-center/develop/update-subscription-overage) bir Azure aboneliğine güncelleştirmek veya Yok olarak ayarlamak için fazla kullanım *güncelleştirme*
