---
title: Yeni ticaret promosyonları
ms.topic: article
ms.date: 09/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Promosyon ve satın alma promosyonları için yeni ticari deneyimler hakkında bilgi edinin.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 45411827f200f205dc20b9a9c2d60519d4aba4eb
ms.sourcegitcommit: a59e1abb470f4847e8f8337ffa4ba705514a0424
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/29/2021
ms.locfileid: "129249319"
---
# <a name="introduction-new-commerce-promotions"></a>Giriş: yeni ticaret promosyonları

**Uygun roller**

- Yönetim Aracısı
- Satış Aracısı
- Genel yönetici

> [!Note] 
> yeni ticari deneyim değişiklikleri şu anda yalnızca Microsoft 365/dynamics 365 yeni ticaret deneyimi technical preview 'ın parçası olan iş ortakları tarafından kullanılabilir.

Microsoft, yeni ticaret 'daki yükseltmeleri destekleyecektir. Bu promosyonlar, farklı indirim miktarları ve sürelerine sahip olacaktır. 

## <a name="discovering-promotions"></a>Promosyonlar bulunuyor ##

İş ortakları, yükseltmeler biriktirme listesini ziyaret ederek veya Getpromosyonlar API 'sini çağırarak yükseltmeleri bulabilir. Promosyonlar biriktirme listesi, iş ortaklarının hakkında bilgi sahibi olması gereken mevcut promosyonlar için Microsoft listesidir. Liste, aylık olarak korunur ve güncelleştirilir. 


## <a name="operationalize-promotions"></a>İşlem yükseltmeleri ##

İş ortakları, [Getpromosyonlar API](/partner-center/develop/get-promotions)'sini uygulayarak yükseltmeleri gerçekleştirebilir. Bu API, belirli bir Pazar (müşterinin ülkesi) ve segmenti için mevcut olan tüm yükseltmeleri döndürür. API, iş ortağının farklı ülkelerdeki müşteriler için hangi promosyonların kullanılabildiğini anlamalarına yardımcı olmak için promosyon ve önemli bilgilerin listesini döndürür. 


Getpromosyonlar API 'SI, belirli bir yükseltme için aşağıdaki verileri içerir:

- Promosyon süresi
- Promosyon için yüzde indirimi
- Promosyon için sunulan ürünler ve SKU 'Lar

Promosyonlar, iş ortağı tarafından promosyon Ürün SKU 'SU satın aldığında, iş ortağı Merkezi tarafından uygulanır. İş ortağı yükseltmeleri, Ürün SKU 'sunda iş ortağı merkezi kataloğu Kullanıcı arabiriminde bulunabilir. Yükseltme hakkında daha fazla bilgi almak için "promosyon ayrıntılarını görüntüleme" seçeneğine tıklamaları gerekebilir. Yükseltme ayrıntılarını görüntüleyebilme, Katalog sayfasından, satın alma işlemi gönderilmeden önce gözden geçirme sayfasından, Sipariş gönderildikten sonra yapılan onay sayfasından ve sipariş geçmişi sayfasından erişilebilir. 

## <a name="verify-eligibility"></a>Uygunluğu doğrula ##

İş ortakları, ürünü satın almadan önce iş ortağı Merkezi ' nde İnceleme sayfasındaki bilgileri görerek bir promosyon için uygun olup olmadığını görüntüleyebilir. İş ortakları Ayrıca, [Verifypromotionuygunluk API](/partner-center/develop/verify-promotion-eligibility)'sini çağırıp MÜŞTERI Kiracı kimliğini ve yükseltme kimliğini geçirerek. Müşteri uygun olduğunda çağrı true değerini döndürür. Müşteri uygun değilse, API, yükseltmenin geçerli olması için karşılanmayan koşulları döndürür. 

İş ortakları, doğrulama uygunluğunu çağırıp sonuçları geri alabilir. Uygunluk hataları, bir yükseltmenin bir müşterinin Ürün SKU 'suna kaç kez uygulanabileceğini, uyumsuz koşulları veya kullanıcı sayısını temel alabilir.

Yeni ticaret yükseltmeleri API 'Leri için önemli konular:

- [Getpromosyonlar API 'SI](/partner-center/develop/get-promotions)
- [Getpromotionsbyıd API 'SI](/partner-center/develop/get-promotion-by-id)
- [Verifypromtioneligılıklara](/partner-center/develop/verify-promotion-eligibility)
- [Promosyon kaynakları](/partner-center/develop/promotion-resources)

>[!IMPORTANT]
> İş ortaklarının, bir işlem göndermeden önce yükseltmeleri doğrulaması gerekir. İş Ortağı Merkezi *İnceleme sayfasında* , iş ortakları bir yükseltme görmediğinden, bu işlem işleme uygulanmaz, iş ortağı yükseltme olmayan fiyatı alır. İş ortakları Ayrıca, bir işlemi göndermeden önce yükseltmenin mevcut olup olmadığını görmek için sepet çizgisi öğe API 'sine de bakabilirler. İş ortakları, Müşteri Ürün SKU bileşiminin yükseltme için uygun olduğunu ve bu nedenle ineligibility nedenlerini doğrulamak üzere işlemleri göndermeden önce doğrulama yükseltmeleri API 'sini çağırabilir.

Müşterilerin bir promosyon için uygun olmayabilir olmasının üç nedeni vardır. Bu sınırsız türler, müşterinin uygun olmadığı durumlarda yükseltmeyi doğrula API 'sinde döndürülür.

### <a name="seat-count"></a>Koltuk sayısı ###

Birçok promosyon bir koltuk 2400 bilgisayar sayısının en fazla belirtii olabilir. Bu durumlarda 2400 'den fazla bir işlem, yükseltme dışı fiyatlarla gönderilir. Bu izin sayıları, bu limitlere sahip bir promosyon aboneliğine koltuk eklenirken de zorlanır. İş ortakları, bir yükseltme etkin aboneliğini limitlerin ötesinde artırmayı denediğinde bir hata alır. Promosyonların bilgisayar sınırları, iş ortakları arasında zorlanır, böylece bir iş ortağı bir promosyon bilgisayar sayısı sınırı ile 2300 koltuk yükseltmesi satın alıyorsa, 200 bilgisayar satın alan ikinci bir iş ortağı, yükseltme dışı fiyata abonelik fiyatını alır. promosyon, ürün sku 'su düzeyinde zorlanır iş ortağı deneyimidir, bu nedenle bir iş ortağı 2400 bilgisayar Microsoft 365 E3 ve ayrıca farklı bir ürün sku 'su Microsoft 365 E5 için promosyon fiyatlandırması alabilir. İş ortakları, bir müşterinin belirli bir sağlanan SKU için kaç lisansa sahip olduğunu görmek için [SUBSCRIBEDSKUS API](/partner-center/develop/get-a-list-of-available-licenses) 'sini çağırabilir.

Bir iş ortağı 2400 ' ten daha fazla lisans istiyorsa ve bu yükseltmeyi istiyorsa, iş ortağı yalnızca yükseltme fiyatı ve yükseltme dışı fiyata ikinci bir abonelik 2400 için bir abonelik satın alabilir.

### <a name="term"></a>Süre ###

Terim kısıtlamaları hangi Ürün SKU koşullarının belirli bir yükseltmeye hizalanacağını tanımlar. Birçok promosyon, terime göre tanımlanan farklı indirimlere sahiptir. Bir iş ortağı bir işlem gönderse ve terim yükseltme ile hizalanmaz, işlem, bekledikleri yükseltme dışı fiyattan olur. Terim örnekleri *yıllık* veya *aylık* olarak verilebilir.

### <a name="first-purchase"></a>İlk Satın Alım ###

Bazı yükseltmeler yalnızca bir kez alınmış olarak zorlanır. Bir iş ortağı, uygunluğu doğrula API 'sini *Ilk satın alma* hata türüyle bir *yanlış* uygunluk durumu görür. İş ortağı, belirtilen Ürün SKU 'sunu satın almaya devam edebilir, ancak abonelik yükseltme dışı fiyattan olacaktır. Bu kısıtlama, iş ortağı başına değil, müşteri başına değildir. Müşterinin bu kurala sahip bir promosyonu olduktan sonra, ikinci bir iş ortağı tarafından uygulanan yükseltmenin ikinci bir örneğini alamaz.

## <a name="promotions-and-renewals"></a>Promosyonlar ve yenilemeler ##

Uygulanan promosyon iskontoları, satın alma dönemi için geçerlidir. Yenileme tarihi, promosyon süresi Tarih aralığalıyorsa, uygulanan promosyonlara sahip abonelikler promosyon fiyatını korur. Promosyon süresi Tarih aralığının dışında yapılan yenilemeler, yükseltme dışı fiyata (fiyat listesinden) göre yenilenecek. İş ortakları, abonelik ayrıntıları sayfasındaki fiyat noktalarına ve getSubscription veri yenileme yönergelerine göre yenileme durumunu izleyebilir.

## <a name="promotions-and-upgrades"></a>Promosyonlar ve yükseltmeler ##
Bir abonelikten başka bir SKU 'ya yükseltme yapan iş ortakları, promosyon fiyatını geride bırakır. Bu eylem, yükseltmenin başka bir SKU 'ya yükseltildiklerinde terk ettikleri SKU için yapılandırılmış olması nedeniyle oluşur. Bir promosyonu olabilecek bir SKU 'ya yükseltme yapan iş ortakları, promosyon fiyatını otomatik olarak alamaz. Taşımak istedikleri SKU 'nun promosyon fiyatına ihtiyaç duyduklarında veya bu fiyatlara izin vermek istiyorsanız yeni bir abonelik olarak yeni SKU 'YU el ile satın alması gerekir. Şu anda yükseltmeler yalnızca yeni abonelik satın alımları ve yenilemeler için geçerlidir.

## <a name="promotions-and-migrations"></a>Promosyonlar ve geçişler ##
iş ortakları, müşterilerinin aboneliklerini geleneksel Microsoft 365/dynamics 365 ' dan yeni ticaret sürümlerine geçirebilirler. Geçişler, hem Iş Ortağı Merkezi kullanıcı arabiriminden hem de geçiş API 'Leri çağrılmadan kullanılabilir. Geleneksel bir abonelikten yeni ticarete geçiş yapan iş ortakları, geçirdikleri Ürün SKU 'su, yükseltme tanımıyla hizalanmakta olduğu sürece promosyonu alır. İş ortakları, hedef Ürün SKU 'sunun geçişten önce promosyon fiyatını uygulayabilmesi için uygunluğu doğrula API 'sini çağırmalıdır.

## <a name="cross-channel-considerations"></a>Çapraz kanal konuları ##
Bulut Çözümü Sağlayıcısı (CSP) yükseltme sınırları ve kısıtlamaları, kurumsal anlaşma (EA) gibi kanallar arasında zorlanmaz. Bir CSP iş ortağı, müşteri EA 'dan 3.000 ' ye sahip olsa bile 2.400-promosyon kısıtlamasına sahip bir promosyon elde edebilir.  
