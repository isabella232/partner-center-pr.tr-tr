---
title: Yeni ticaret telekomünikasyon Kullandıkça öde
ms.topic: article
ms.date: 08/30/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Fazla kullanım Kullandıkça Öde teklifi sağlayan yeni ticari deneyimler hakkında bilgi edinin.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0f934b8d858c1fc30d0140d19fb0697ba6bd9001
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961464"
---
# <a name="introduction-new-commerce-overage-for-telco-pay-as-you-go"></a>Giriş: telefon Kullandıkça Öde için yeni ticaret fazla kullanım

**Uygun roller**

- Yönetim Aracısı
- Satış Aracısı
- Genel yönetici

> [!Note] 
> yeni ticari deneyim değişiklikleri şu anda yalnızca Microsoft 365/dynamics 365 yeni ticaret deneyimi technical preview 'ın parçası olan iş ortakları tarafından kullanılabilir.

Lisans tabanlı bazı ürünler, ayrılan çağrı planlarına sahip hizmetleri içerir. Bu çağrı planları genellikle lisans başına 120, genellikle her ay için lisans başına bir ayırma ile gelir. 

Geleneksel lisans tabanlı iş ortağı senaryolarında, hizmet kullanımını aylık limitlerin ötesinde etkinleştirmenin bir yolu yoktur. Müşterilerin iletişim kredilerini *veya doğrudan Microsoft 'tan iletişim kredisi* satın alması için 120 dakikadan uzun süre ihtiyaç duyan müşteriler.  Bu iletişim kredileri Iş Ortağı Merkezi 'nde sunulmadı.

## <a name="using-new-commerce-telco-pay-as-you-go"></a>Yeni ticaret teller, Kullandıkça Öde 'yi kullanma ##

Bu sınırlama, iş ortağının izin verilen hizmetlere yönelik fazla kullanım yeteneklerini etkinleştirmesine imkan tanıyan yeni ticaret 'ta giderilmiştir. İş ortakları fazla kullanım özellikleri içeren teklifler satın alabilir. Bu teklifler, *ıncludeoverage* için fiyat listesi etiketleri sütununda tanımlanmıştır. Katalog SKU 'SU, fazla kullanım kapasitesini desteklemek için de bir özelliği içerir. İş ortakları yalnızca teklifleri ve sistem yapılandırma ve fazla kullanım aboneliği satın alabilir ve yalnızca müşterinin kullanıcıları, satın alınan teklifle birlikte gelen ayrılmış aylık arama dakikalarına göre faturalandırılır. 

İş ortakları, Azure portal giderek ve maliyet yönetimi özelliklerini ve özelliklerini kullanarak fazla kullanım kullanımını izleyebilir. Ayrıca iş ortakları, herhangi bir zamanda fazla kullanım süresini devre dışı bırakmak veya kapatmak istediklerinde, fazla kullanımı herhangi bir zamanda *yok* olarak ayarlamak için seçeneği de vardır.

İş ortakları, iş ortağı merkezi kataloğu Ürün SKU 'Larını görüntüleyerek fazla kullanım özellikleri dahil olmak üzere ürünleri tanımlayabilir. 

Fazla kullanım ile ürün satın alma iş ortakları, abonelikleri Yönet sayfasındaki *fazla kullanımı yönetme* sayfasına erişerek fazla kullanım sağlar. Bu, iş ortağının fazla kullanım süresini etkinleştirmesine ve fazla kullanım ücretleri üzerinden akacak olan istenen tüketim aboneliğini atamasına olanak sağlar. Herhangi bir zamanda iş ortağı, tüketim aboneliğini *none* olarak atayarak fazla kullanımı kapatabilir. 

İş ortakları fazla kullanım veya abonelik listesindeki *fazla kullanımı Yönet* özelliğini tarafından devre dışı bırakır. Bu, yalnızca ortağın fazla kullanım sağlayan abonelikler içeriyorsa erişilebilir olacaktır. Aylık fazla kullanım ücretleri atanan aboneliğe tahakkuk eder ve iş ortakları mutabakatı dosyasında tanımlanır. İş ortakları, Azure portal Azure maliyet yönetimi özelliklerini ziyaret ederek fazla kullanım kullanımını izleyebilir. 

## <a name="important-details-about-overage"></a>Fazla kullanım hakkında önemli ayrıntılar ##

Fazla kullanım sağlayan bir Ürün SKU 'SU satın alma, iş ortağının müşterinin Flow için fazla kullanım için ayarlanmış olmasını otomatik olarak sağlayacaktır. Bu, Azure planı, ilişkili bir varsayılan Azure aboneliği ve özel olarak fazla kullanım tüketimi için bir abonelik oluşturmayı içerir. İş ortakları, fazla kullanım ömrü boyunca fazla kullanım süresi boyunca tahakkuk ettirmek istedikleri abonelikleri görebilir ve atayabilir.

Fazla kullanım ataması, *ilk* kural tarafından belirlenir. Bir iş ortağı, yeni bir müşteri için çağrı planlarına sahip E5 satın alıyorsa, bu iş ortağı tüketim aboneliğine atanmış fazla kullanım yaşına sahip olur. İkinci bir iş ortağı, çağrı planlarına sahip bir E5 kopyasını satın alıyorsa, sistem ilk ortağın satın alma ve atamaya göre yapılır. İş ortakları, fazla kullanım süresini devre dışı bırakmak veya devre dışı *bırakmak için abonelikler* sayfasından her zaman *fazla kullanım yönetimi* sağlayabilir.

Fazla kullanım ayarları, müşteri başına hizmet başına. Müşterinin farklı iş ortaklarından aynı fazla kullanım hizmetleri varsa, aynı anda yalnızca bir fazla kullanım aboneliği atanabilir. Fazla kullanım 'nin bir iş ortağından diğerine değiştirilmesi gerekiyorsa, söz konusu üç taraf öncelikle kabul etmelidir. Var olan ortağın kabul ettikleri zaman, diğer ortağın aboneliklerinde fazla kullanım izni olarak ayarlanmalarına olanak tanımak için fazla kullanım *yok* olarak ayarlanabilir.

Kullandıkça Öde özellikleri için API desteği şunları içerir:

- İş ortağının fazla kullanım için izin verip etmediğini belirlemesine yardımcı olmak için SKU özellikleri
- Mevcut bir aboneliğe fazla kullanım atama veya fazla kullanım *yok* olarak ayarlama için yenı bir API
