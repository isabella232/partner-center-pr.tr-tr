---
title: Yeni ticaret eklentileri
ms.topic: article
ms.date: 08/30/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Eklentiler satın alma için yeni ticaret deneyimleri hakkında bilgi edinin.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 539aa939d980f7b40abc44789a08d153a8abdfaa
ms.sourcegitcommit: 09d2c10491244775e656b48fce35b5648262ce59
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/03/2021
ms.locfileid: "123458317"
---
# <a name="introduction-new-commerce-add-ons"></a>Giriş: Yeni Ticari Eklentiler

**Uygun roller**

- Yönetim Aracısı
- Satış Aracısı
- Genel yönetici

> [!Note] 
> yeni ticari deneyim değişiklikleri şu anda yalnızca Microsoft 365/dynamics 365 yeni ticaret deneyimi technical preview 'ın parçası olan iş ortakları tarafından kullanılabilir.

İş ortakları, daha önce satın alınan bir ürünü karmaşıklama diğer hizmetleri etkinleştirmek için yeni ticarete eklentiler satın alabilir. Bu örneklere örnek olarak planlar, daha fazla disk alanı veya müşterinin temel hizmetleri varsa eklenebilecek diğer özellikler verilebilir.



## <a name="add-ons-in-new-commerce"></a>Yeni ticaret 'daki eklentiler ## 

Yeni ticaret eklentileri, geleneksel lisans tabanlı eklentilere benzer kavramlar içerir. Geleneksel lisans tabanlı gibi yeni ticaret eklentileri, önkoşulların kavramını içerir. Bunlar, müşterinin eklentinin doğru çalışması için sahip olması gereken Ürün SKU 'lardır. Bir eklentiye yönelik önkoşulların önkoşulları, belirli bir SKU için katalog API 'Leri ve Iş Ortağı Merkezi kataloğu kullanıcı deneyiminde bulunabilir. Eklenti satın alma, müşteri kiracısında bir veya daha fazla önkoşulların mevcut olmasını gerektirir.
 
Geleneksel lisans tabanlı ve yeni ticaret arasında eklentilerin *satın alındığı önemli* fark, satın almalardır. Geleneksel lisans tabanlı iş ortağı, eklentiyi mevcut bir temel teklif aboneliğine uygular. Yeni ticaret 'ta iş ortakları, eklentileri kataloğun kendisinden satın almasından, artık temel tekliflerde ve eklentilerde bifurta satın alma deneyimine sahip olmadığından, her şey yeni ticaret ' de katalogda bulunur.

Eklentilerin nasıl çalıştığı hakkında bir hizmetler perspektifinden, geleneksel ve yeni ticaret genelinde doğru olmaya devam eder. Hem eklenti hizmetlerini kaydedin hem de sağlayın, sağlama işleminin nasıl gerçekleştemediğinde farklı bir şey yoktur. Ayrıca, tek bir eklentinin Hizmetleri, eklenti ile çalışmak üzere tasarlanan birden fazla temel Ürün SKU 'SU karmaşık hale getirebilir.

## <a name="identifying-add-ons"></a>Eklentileri tanımlama ##

İş ortakları, API 'ler aracılığıyla SKU 'Ları alırken SKU ayrıntılarını inceleyerek, eklentileri tanımlayabilir ve önkoşulların listesini alabilir. Eklentiler, Etiketler sütunundaki yeni ticaret lisansı tabanlı fiyat listesinde de tanımlanır. Teklif matrisi, her eklenti Ürün SKU 'SU için önkoşulların listesini içerir.

## <a name="purchasing-add-ons"></a>Eklentileri satın alma ##

Hem geleneksel lisans tabanlı hem de yeni ticaret deneyimleri için eklentiler bulunur. Temel fark, yeni ticaret 'nin keşfedime ve katalogdan satın alma olanağı sağladığından, taban tekliflerinin veya önkoşulların bulunduğu yerden aynı yerde bulunabilirliğin bulunduğu yerdir. Geleneksel lisans tabanlı eklentiler yalnızca temel teklifin abonelik ayrıntıları sayfasına giderek bulunabilir ve satın alınır. Bir eklenti orada listelendikten sonra, iş ortağı istenen eklentiyi uygular.


Yeni ticaret deneyimi eklentileri, kataloğun kendisinde keşfedilir ve satın alınır. İş ortakları, ürün türü açılan listesini seçerek yeni ticari eklentilere filtre uygulayabilir. Eklentinin yanında bir bilgi simgesine sahip oldukları için eklenti ürünlerinin de kolayca görüleneceği, bu, eklenti durumunu ve anlamını açıklar.


İş ortakları, belirli bir eklentiyi satın alması için olması gereken Ürün SKU 'Larının listesini göstermek üzere *uyumlu temel ürün aboneliklerini görüntüle* ' ye tıklayarak bir eklentiye yönelik gerekli ürünler hakkında daha fazla ayrıntı alabilir.


## <a name="add-on-enforcement"></a>Eklenti zorlaması ##

İş ortakları, müşterinin önkoşulların herhangi birine sahip olmadığı yeni bir ticari eklenti ürünü satın almaya çalışırken hata görür. İş ortakları, iş ortağı merkezi 'nde validateAddon API 'sini çağırarak bir müşterinin önkoşulları karşıladığını doğrulayabilirler.

## <a name="important-details-when-purchasing-add-ons"></a>Eklentiler satın alınırken önemli ayrıntılar ##

Müşteriler önkoşulları karşılıyorsa, eklentiler ayrı Ürün SKU 'Ları olarak satın alınır. Eklenti aboneliklerinin kendi farklı bir terim hizalaması vardır. Eklentileri satın alan iş ortakları, dönem ve ilişkili bitiş tarihinin önkoşul ile aynı olabileceğini fark eder. Her iki abonelik de yeni koşullara otomatik yenileme yaptığı sürece, önkoşul ve eklentiler oldukça iyi çalışacaktır. İş ortağı otomatik Yenilemesiz önkoşul terimini sona ermeye karar verirse, iş ortağının sona ermemesi durumunda eklenti, eklenti teriminin sonunda otomatik yenilemeyen olarak da güncelleştirilecektir.  İş ortakları bir Ürün SKU 'sunu, eklenti hizmetleri zaten olan daha yüksek bir SKU 'ya dönüştürür bir eklentiyi devre dışı bırakma desteğiyle bir hizmet isteği verebilir.

İş ortaklarının, temel tekliflerde gerektiği şekilde hizalama olduğundan emin olmak için edindikleri eklentilerin dönem bitiş tarihlerini yönetmesi beklenir.

