---
title: Yeni ticaret telekomünikasyon Kullandıkça öde
ms.topic: article
ms.date: 09/03/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Kullandıkça Öde fazla kullanımı sağlayan satın alma teklifleri için yeni ticari deneyimler hakkında bilgi edinin.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8265cb3ce77183c4919e9b8e4e028bb66e8cd2f7
ms.sourcegitcommit: 462d6026287b85c9feea602af5bcdf924f3e6976
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/05/2021
ms.locfileid: "129452507"
---
# <a name="introduction-new-commerce-overage-for-telco-pay-as-you-go"></a>Giriş: telekomünikasyon Kullandıkça Öde için yeni ticaret fazla kullanım

**Uygun roller**

- Yönetim Aracısı
- Satış Aracısı
- Genel yönetici

> [!NOTE]
> yeni ticari deneyim değişiklikleri şu anda yalnızca Microsoft 365/dynamics 365 yeni ticaret deneyimi technical preview 'ın parçası olan iş ortakları tarafından kullanılabilir.

Lisans tabanlı bazı ürünler, genellikle lisans başına 120, her ay dakika boyunca lisans başına bir ayırma dahil olmak üzere, ayrılmış çağrı planlarına sahip hizmetleri içerir. 

Geleneksel lisans tabanlı iş ortağı senaryolarında, hizmet kullanımını aylık limitlerin ötesinde etkinleştirmenin bir yolu yoktur. Müşterilerin iletişim kredilerini *veya doğrudan Microsoft 'tan iletişim kredisi* satın alması için 120 dakikadan uzun süre ihtiyaç duyan müşteriler.  Bu iletişim kredileri Iş Ortağı Merkezi 'nde sunulmadı.

## <a name="using-new-commerce-telco-pay-as-you-go"></a>Yeni ticari telekomünikasyon Kullandıkça Öde 'yi kullanma

Bu sınırlama, iş ortağının izin verilen hizmetlere yönelik fazla kullanım yeteneklerini etkinleştirmesine imkan tanıyan yeni ticaret 'ta giderilmiştir. İş ortakları fazla kullanım özellikleri içeren teklifler satın alabilir. Bu teklifler, *ıncludeoverage* için fiyat listesi etiketleri sütununda tanımlanmıştır. Katalog SKU 'SU, fazla kullanım kapasitesini desteklemek için de bir özelliği içerir. İş ortakları yalnızca teklifleri satın alabilir ve sistem ücret ödemeden bir fazla kullanım aboneliği yapılandırır ve yalnızca müşterinin kullanıcıları, satın alınan teklifle birlikte gelen ayrılan aylık arama dakikalarına göre, yalnızca faturalandırılır. 

İş ortakları, hangi Ürün SKU 'larının dahil fazla kullanım özellikleri olduğunu tanımlayabilir 

- İş Ortağı Merkezi kataloğu Ürün SKU 'Larını görüntüleme
- Yeni ticaret fiyat listesini Etiketler sütununda **ıncludesoiçecek** ile filtreleme

Fazla kullanım ile ürün satın alma iş ortakları, abonelikleri Yönet sayfasındaki **fazla kullanımı yönetme** sayfasına erişerek etkinleştirin. Fazla kullanım arabirimi yönetimi, iş ortağının fazla kullanım ücretlerinin hangi Azure aboneliğine akaceğini etkinleştirmesine ve atamasına olanak sağlar. Herhangi bir zamanda iş ortağı, tüketim aboneliğini *none* olarak atayarak fazla kullanımı kapatabilir. 

İş ortakları fazla kullanım veya abonelik listesindeki *fazla kullanımı Yönet* özelliğini tarafından devre dışı bırakır. Bu, yalnızca ortağın fazla kullanım sağlayan abonelikler içeriyorsa erişilebilir olacaktır. Aylık fazla kullanım ücretleri atanan aboneliğe tahakkuk eder ve iş ortakları mutabakatı dosyasında tanımlanır. İş ortakları, Azure portal Azure maliyet yönetimi özelliklerini ziyaret ederek fazla kullanım kullanımını izleyebilir. 

İş ortakları, Azure portal giderek ve maliyet yönetimi özelliklerini ve özelliklerini kullanarak fazla kullanım kullanımını izleyebilir. 

## <a name="important-details-about-overage"></a>Fazla kullanım hakkında önemli ayrıntılar

- Fazla kullanım özellikleri içeren lisans tabanlı bir Ürün SKU 'SU satın almak yalnızca lisans tabanlı ürünü satın alır. İş ortaklarının, abonelik yönetim sayfasına gidip **fazla kullanımı Yönet** ' e tıklayarak fazla kullanım süresini açmak için satın alma işleminden sonra başka bir adım sürmeleri gerekir
- Lisans tabanlı satın alma işleminden sonra yalnızca deneyimidir iş ortağı için yönetim aracıları fazla kullanım sağlayabilir. 
- Fazla kullanım kullanımı, fazla kullanım tüketimi için ücretsiz bir Azure planı ve ilişkili bir varsayılan Azure aboneliği **aboneliği 1** oluşturur. Azure planı zaten mevcutsa, fazla kullanım etkinleştirilmesi, mevcut Azure planı altında yeni aboneliği oluşturur. İş ortakları, **fazla kullanım süresini yönetme** alanındaki diğer aboneliklere her zaman fazla kullanım sağlayabilir veya yeniden atayabilir. Henüz Azure planına (eski Azure) sahip olmayan müşterilerin, fazla kullanım sağlamak için Azure planına geçiş yapması gerekir.

Fazla kullanım ataması, *ilk* kural tarafından belirlenir. Bir iş ortağı, yeni bir müşteri için çağrı planlarına sahip E5 satın alıyorsa, bu iş ortağı tüketim aboneliğine atanmış fazla kullanım yaşına sahip olur. İkinci bir iş ortağı, çağrı planlarına sahip bir E5 kopyasını satın alıyorsa, sistem ilk ortağın satın alma ve atamaya göre yapılır. İş ortakları, fazla kullanım süresini devre dışı bırakmak veya devre dışı *bırakmak için abonelikler* sayfasından her zaman *fazla kullanım yönetimi* sağlayabilir.

Fazla kullanım ayarları, müşteri başına hizmet başına. Tek seferde yalnızca bir fazla kullanım aboneliği atanabilir. Fazla kullanım 'nin bir iş ortağından diğerine değiştirilmesi gerekiyorsa, söz konusu üç taraf öncelikle kabul etmelidir. Var olan ortağın kabul ettikleri zaman, diğer ortağın aboneliklerinde fazla kullanım izni olarak ayarlanmalarına olanak tanımak için fazla kullanım *yok* olarak ayarlanabilir.

## <a name="telco-pay-as-you-go-apis"></a>Telco Kullandıkça Öde API 'Leri

- [SKU özellikleri](/partner-center/develop/product-resources#sku) , ortağın bir SKU 'nun fazla kullanım belirlemesine izin verip kullanmadığını belirlemesine yardımcı olmak Için bir *Tüketimptiontype* özelliği içerir
- Müşteriniz için halen fazla kullanım olduğunu anlamak için [fazla kullanım kazanın](/partner-center/develop/get-subscription-overage)
- Müşterinin fazla kullanım süresini bir Azure aboneliğine güncelleştirmek veya *none* olarak ayarlamak için [fazla kullanımı Güncelleştir](/partner-center/develop/update-subscription-overage)
