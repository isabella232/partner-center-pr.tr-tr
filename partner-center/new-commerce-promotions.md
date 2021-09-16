---
title: Yeni ticaret promosyonları
ms.topic: article
ms.date: 09/03/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Promosyon ve satın alma promosyonları için yeni ticari deneyimler hakkında bilgi edinin.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc2d52dd444168b32f0cadaeccec1e6d906348d1
ms.sourcegitcommit: 847ad384d44a5a673791cb2950af02225d8174c9
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/16/2021
ms.locfileid: "127877028"
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

İş ortakları, Getpromosyonlar API 'sini uygulayarak yükseltmeleri gerçekleştirebilir. Bu API, belirli bir Pazar (müşterinin ülkesi) ve segmenti için mevcut olan tüm yükseltmeleri döndürür. API, iş ortağının farklı ülkelerdeki müşteriler için hangi promosyonların kullanılabildiğini anlamalarına yardımcı olmak için promosyon ve önemli bilgilerin listesini döndürür. 


Getpromosyonlar API 'SI, belirli bir yükseltme için aşağıdaki verileri içerir:

- Promosyon süresi
- Promosyon için yüzde indirimi
- Promosyon için sunulan ürünler ve SKU 'Lar

Promosyonlar, iş ortağı tarafından promosyon Ürün SKU 'SU satın aldığında, iş ortağı Merkezi tarafından uygulanır. İş ortağı yükseltmeleri, Ürün SKU 'sunda iş ortağı merkezi kataloğu Kullanıcı arabiriminde bulunabilir. Yükseltme hakkında daha fazla bilgi almak için "promosyon ayrıntılarını görüntüleme" seçeneğine tıklamaları gerekebilir. Yükseltme ayrıntılarını görüntüleyebilme, Katalog sayfasından, satın alma işlemi gönderilmeden önce gözden geçirme sayfasından, Sipariş gönderildikten sonra yapılan onay sayfasından ve sipariş geçmişi sayfasından erişilebilir. 


## <a name="verify-eligibility"></a>Uygunluğu doğrula ##

İş ortakları, ürünü satın almadan önce iş ortağı Merkezi ' nde İnceleme sayfasındaki bilgileri görerek bir promosyon için uygun olup olmadığını görüntüleyebilir. İş ortakları Ayrıca, Verifypromotionuygunluk API 'sini çağırıp müşteri kiracı KIMLIĞINI ve yükseltme KIMLIĞINI geçirerek. Müşteri uygun olduğunda çağrı true değerini döndürür. Müşteri uygun değilse, API, yükseltmenin geçerli olması için karşılanmayan koşulları döndürür. 



## <a name="promotions-and-renewals"></a>Promosyonlar ve yenilemeler ##

Uygulanan promosyon iskontoları, satın alma dönemi için geçerlidir. Yenileme tarihi, promosyon süresi Tarih aralığalıyorsa, uygulanan promosyonlara sahip abonelikler promosyon fiyatını korur. Promosyon süresi Tarih aralığının dışında yapılan yenilemeler, yükseltme dışı fiyata (fiyat listesinden) göre yenilenecek. İş ortakları, abonelik ayrıntıları sayfasındaki fiyat noktalarına ve getSubscription veri yenileme yönergelerine göre yenileme durumunu izleyebilir.


## <a name="promotions-and-upgrades"></a>Promosyonlar ve yükseltmeler ##
Bir abonelikten başka bir SKU 'ya yükseltme yapan iş ortakları, promosyon fiyatını geride bırakır. Bu eylem, yükseltmenin başka bir SKU 'ya yükseltildiklerinde terk ettikleri SKU için yapılandırılmış olması nedeniyle oluşur. Bir promosyonu olabilecek bir SKU 'ya yükseltme yapan iş ortakları, promosyon fiyatını otomatik olarak alamaz. Taşımak istedikleri SKU 'nun promosyon fiyatına ihtiyaç duyduklarında veya bu fiyatlara izin vermek istiyorsanız yeni bir abonelik olarak yeni SKU 'YU el ile satın alması gerekir. Şu anda yükseltmeler yalnızca yeni abonelik satın alımları ve yenilemeler için geçerlidir.



