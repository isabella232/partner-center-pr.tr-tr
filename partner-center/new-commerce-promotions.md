---
title: Yeni ticari promosyonlar
ms.topic: article
ms.date: 09/03/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Promosyonları keşfetmeye ve satın almaya yönelik yeni ticari deneyimler hakkında bilgi edinin.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc2d52dd444168b32f0cadaeccec1e6d906348d1
ms.sourcegitcommit: 847ad384d44a5a673791cb2950af02225d8174c9
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/16/2021
ms.locfileid: "127886191"
---
# <a name="introduction-new-commerce-promotions"></a>Giriş: Yeni ticari promosyonlar

**Uygun roller**

- Yönetici aracısı
- Satış aracısı
- Genel yönetici

> [!Note] 
> Yeni ticaret deneyimi değişiklikleri şu anda yalnızca Microsoft 365/Dynamics 365 yeni ticaret deneyimi teknik önizlemesinde yer alan iş ortakları tarafından kullanılabilir.

Microsoft, yeni ticarette promosyonları destekleyecektir. Bu promosyonların indirim miktarları ve süreleri değişiklik gösterir. 

## <a name="discovering-promotions"></a>Promosyonları bulma ##

İş ortakları, promosyonlar biriktirme listesi ziyaret ederek veya getPromotions API'sini çağırarak promosyonları keşfeder. Promosyonlar biriktirme listesi, iş ortaklarının bilmek zorunda olduğu kullanılabilir promosyonların Bir Microsoft listesidir. Liste editoryal olarak korunur ve aylık olarak güncelleştirilir. 


## <a name="operationalize-promotions"></a>Yükseltmeleri faaliyete geçirmek ##

İş ortakları, getPromotions API'sini kullanarak yükseltmeleri faaliyete geçirebilirsiniz. Bu API, belirli bir pazar (müşterinin ülkesi) ve segmenti için mevcut olan tüm promosyonları döndürür. API, iş ortağının farklı ülkelerdeki müşteriler için hangi promosyonların kullanılabilir olduğunu an etmesinde yardımcı olmak için promosyonların ve önemli bilgilerin listesini döndürür. 


getPromotions API'si, verilen bir yükseltme için aşağıdaki verileri içerir:

- Yükseltme süresi
- Promosyon için yüzde indirimi
- Promosyon için kullanılabilen ürünler ve SU'lar

Promosyonlar, iş ortağı, promosyon için kullanılabilir olan ürün SKU'larını satın alan iş ortağı merkezi tarafından uygulanır. İş ortağı promosyonları, ürün SKU ayrıntılarında iş ortağı merkezi kataloğu kullanıcı arabiriminde kullanılabilir. Yükseltme hakkında daha fazla bilgi almak için "Yükseltme ayrıntılarını görüntüle"ye tıklarlar. Promosyon ayrıntılarını görüntüleme özelliğine katalog sayfasından SKU ayrıntılarını, satın alma göndermeden önceki inceleme sayfasından, sipariş gönderildikten sonra gelen onaydan ve sipariş geçmişi sayfasından erişilebilir. 


## <a name="verify-eligibility"></a>Uygunluğu doğrulama ##

İş ortakları, ürünü satın almadan önce iş ortağı merkezinde bulunan inceleme sayfasındaki bilgileri görerek müşterinin satın almalarının promosyon için uygun olup olmadığını sıntlar. İş ortakları ayrıca müşteri kiracı kimliğini ve yükseltme kimliğini geçerek verifyPromotionEligibility API'sini çağırabilirsiniz. Müşteri uygunsa çağrı true döndürür. Müşteri uygun değilse API, yükseltmenin geçerli olması için karşılanmayacak koşulları döndürür. 



## <a name="promotions-and-renewals"></a>Promosyonlar ve yenilemeler ##

Uygulandığı promosyon indirimleri, satın alma süresine yöneliktir. Yenileme tarihi yükseltme süresi tarih aralığında ise, uygulanan promosyonlara sahip abonelikler promosyon fiyatını korur. Yükseltme süresi tarih aralığı dışındaki yenilemeler, promosyon olmayan fiyatla (fiyat listesinden) yenilenecektir. İş ortakları abonelik ayrıntıları sayfasındaki fiyat noktalarına ve getSubscription veri yenileme yönergelerine göre yenileme durumunu izleyebilir.


## <a name="promotions-and-upgrades"></a>Yükseltmeler ve yükseltmeler ##
Bir abonelikten başka bir SKU'ya yükselten iş ortakları, yükseltme fiyatını geride bırakır. Bu eylem, yükseltme başka bir SKU'ya yükseltilen SKU için yapılandırıldığında oluşur. Promosyonu olan bir SKU'ya yükselten iş ortakları, yükseltme fiyatını otomatik olarak elde etmez. Taşımak istediğiniz SKU için yükseltme fiyatına ihtiyaçları veya bunu istemeleri, yeni SKU'nun yeni bir abonelik olarak el ile satın alınarak satın almaları gerekir. Şu anda promosyonlar yalnızca yeni abonelik satın alma ve yenileme işlemlerine uygulanır.



