---
title: Yeni ticari promosyonlar
ms.topic: article
ms.date: 09/24/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Promosyonları keşfetmeye ve satın almaya yönelik yeni ticari deneyimler hakkında bilgi edinin.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8abd34ff7cc47edf59be6532dcc7e9c7e0dd1533
ms.sourcegitcommit: dd900161830c59bcf3c5d700d524436ee05cd987
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/24/2021
ms.locfileid: "128714156"
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

İş ortakları uygunluk doğrulamayı çağırarak sonuçları geri alabiliyor. Uygunluk hataları, bir müşterinin ürün SKU'suyla kaç kez promosyon uygulanabiliyorsa, seat sayılarına, uyumsuz terimlere veya sınırlara bağlı olabilir.

>[!IMPORTANT]
> İş ortaklarının bir işlem göndermeden önce yükseltmeleri doğrulamaları gerekir. İş İş Ortağı Merkezi gözden  geçirme sayfasında, iş ortakları bir yükseltme görmüyorsa, işlemde uygulanmaz, iş ortağı promosyon olmayan fiyatı alır. İş ortakları, bir işlem göndermeden önce yükseltmenin mevcut olup olduğunu görmek için sepet satır öğesi API'sine de bakabilirsiniz. İş ortakları, müşteri ürün sku bileşiminin yükseltmeye uygun olduğunu ve uygun olmadığını doğrulamak için işlemleri göndermeden önce doğrulama yükseltmeleri API'sini çağırarak uygun olmayan nedenleri tespit edilebilir.

Müşterinin promosyon için uygun olup olmadığının üç nedeni vardır. Bu önemsiz türler, müşterinin uygun olmayan durumlarda yükseltmeyi doğrulama API'sinde döndürülür.

### <a name="seat-count"></a>Yer Sayısı ###

Birçok promosyonda en fazla 2400 kişilik bir yer olabilir. Bu gibi durumlarda, promosyon dışı fiyatlardan 2400'den fazla içeren bir işlem göndermektedir. Bu sınırlara sahip bir yükseltme aboneliğine yer eklerken de bu yer sayısı uygulanır. İş ortakları, yükseltme etkinleştirilmiş aboneliği sınırların ötesinde artırmaya çalışırsa bir hata alır. Promosyonlara yönelik lisans sınırları iş ortakları arasında uygulanır. Bu nedenle, bir iş ortağı, promosyon lisans sayısı sınırıyla 2300 lisanslık bir promosyon satın aldı ise, 200 lisans satın alan ikinci bir iş ortağı, promosyon dışı fiyattan abonelik fiyatını elde ediyor olabilir. Promosyona uygun olan ürün sku'su, iş ortağının işlemde olduğu ürün sku düzeyinde zorunlu tutularak bir iş ortağı hem 2400 hem Microsoft 365 E3 de farklı bir ürün SKU'su için 2400 kişilik promosyon Microsoft 365 E5. İş ortakları, müşterinin [sağlanan bir](/partner-center/develop/get-a-list-of-available-licenses) SKU için kaç lisansa sahip olduğunu görmek için abone olunanSKU API'sini çağırabilirsiniz.

### <a name="term"></a>Süre ###

Terim kısıtlamaları, belirli bir promosyonla hangi ürün SKU koşullarının uyumlu olduğunu tanımlar. Birçok promosyonda, terime göre tanımlanan farklı indirimler vardır. bir iş ortağı bir işlem gönderse ve süre yükseltmeyle uyumlu yoksa, işlem beklediğiniz promosyon olmayan fiyatta olur. Terimlere örnek olarak *yıllık veya* *aylık terimler verilmiştir.*

### <a name="first-purchase"></a>İlk Satın Alım ###

Bazı yükseltmeler yalnızca bir kez satın alınarak zorlar. İş ortağı, *FirstPurchase* *hata* türüyle uygunluk doğrulama API'sini kullanarak false uygunluğunu görebilir. İş ortağı verilen ürün SKU'larını satın almaya devam edebilirsiniz ancak abonelik promosyon fiyatı üzerindendir. Bu kısıtlama iş ortağı başına değil müşteri başına bir kısıtlamadır. Müşteri bu kuralla promosyona sahip olduktan sonra, ikinci bir iş ortağı tarafından uygulanan yükseltmenin ikinci bir örneğini aamaz.

## <a name="promotions-and-renewals"></a>Promosyonlar ve yenilemeler ##

Uygulandığı promosyon indirimleri, satın alma süresine yöneliktir. Yenileme tarihi yükseltme süresi tarih aralığında ise, uygulanan promosyonlara sahip abonelikler promosyon fiyatını korur. Yükseltme süresi tarih aralığı dışındaki yenilemeler, promosyon olmayan fiyatla (fiyat listesinden) yenilenecektir. İş ortakları abonelik ayrıntıları sayfasındaki fiyat noktalarına ve getSubscription veri yenileme yönergelerine göre yenileme durumunu izleyebilir.

## <a name="promotions-and-upgrades"></a>Yükseltmeler ve yükseltmeler ##
Bir abonelikten başka bir SKU'ya yükselten iş ortakları, yükseltme fiyatını geride bırakır. Bu eylem, yükseltme başka bir SKU'ya yükseltilen SKU için yapılandırıldığında oluşur. Promosyonu olan bir SKU'ya yükselten iş ortakları, yükseltme fiyatını otomatik olarak elde etmez. Taşımak istediğiniz SKU için yükseltme fiyatına ihtiyaçları veya bunu istemeleri, yeni SKU'nun yeni bir abonelik olarak el ile satın alınarak satın almaları gerekir. Şu anda promosyonlar yalnızca yeni abonelik satın alma ve yenileme işlemlerine uygulanır.

## <a name="promotions-and-migrations"></a>Yükseltmeler ve geçişler ##
İş ortakları, müşteri aboneliklerini geleneksel Microsoft 365/Dynamics 365'den aboneliklerinin yeni ticari sürümlerine geçirebilirsiniz. Geçişler hem kullanıcı arabiriminden hem de İş Ortağı Merkezi API'leri çağırmadan kullanılabilir. Geleneksel bir abonelikten yeni ticarete geçişe sahip olan iş ortakları, geçiş sırasında, taşımaları gereken ürün sku'su promosyon tanımıyla uyumlu olduğu sürece promosyona sahip olur. İş ortakları, hedef ürün SKU'slarının geçişten önce yükseltme fiyatını uygulayacaklarından emin olmak için uygunluk doğrulama API'sini çağırması gerekir.




