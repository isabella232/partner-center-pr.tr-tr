---
title: Yeni ticari eklentiler
ms.topic: article
ms.date: 09/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Eklentiler satın almak için yeni ticari deneyimler hakkında bilgi edinin.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 355c7ae3d4832764f6201613c040eebca998c3b6
ms.sourcegitcommit: a59e1abb470f4847e8f8337ffa4ba705514a0424
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/29/2021
ms.locfileid: "129249341"
---
# <a name="introduction-new-commerce-add-ons"></a>Giriş: Yeni ticari eklentiler

**Uygun roller:** Yönetici aracısı | Satış aracısı | Genel yönetici

> [!NOTE]
> Yeni ticaret deneyimi değişiklikleri şu anda yalnızca Microsoft 365/Dynamics 365 yeni ticaret deneyimi teknik önizlemesinde yer alan iş ortakları tarafından kullanılabilir.

İş ortakları, daha önce satın alınan bir ürünü en iyi şekilde sağlayan diğer hizmetleri etkinleştirmek için yeni ticarette eklentiler satın alınabilir. Eklentilerin bazı örnekleri arasında arama planları, daha fazla disk alanı veya müşterinin temel hizmetleri varsa eklen diğer özellikler yer almaktadır.

## <a name="add-ons-in-new-commerce"></a>Yeni ticarette eklentiler

Yeni ticari eklentiler, geleneksel lisans tabanlı eklentilere benzer kavramlar içerir. Geleneksel lisans tabanlı gibi yeni ticari eklentilerde önkullar kavramı da yer almaktadır. Önkullar, eklentinin düzgün çalışması için müşterinin sahip olması gereken ürün SKI'larıdır. Bir eklentinin önkulları, verili bir SKU için katalog API'lerini ve İş Ortağı Merkezi kullanıcı deneyiminde bulunabilir. Satın alma eklentileri, müşteri kiracısı üzerinde bir veya daha fazla önkul gerektirir.

Geleneksel ve yeni ticari eklentiler arasındaki temel fark, **satın** almalarıdır. İş ortakları, geleneksel lisans tabanlı senaryolarda temel teklif aboneliğine eklentiyi uygulayabilir. İş ortağı, katalogdan yeni ticari eklentiler satın alıyor. Bu satın alma deneyimi, eklenti keşfedebilirliğini temel teklifle uyumlu hale getirir ve eklentileri bulup satın almayı kolaylaştırır.

Hizmetler açısından bakıldığında, eklentilerin nasıl iştığıyla ilgili kavramların çoğu geleneksel ve yeni ticarette doğru olmaya devam ediyor. Hem geleneksel hem de yeni ticari işlemler eklenti hizmetlerini kaydederek sağlar; sağlama her iki durumda da aynı şekilde gerçekleşir. Ayrıca, tek bir eklentinin hizmetleri, eklentinin birlikte çalışmak üzere tasarlansa bile birden fazla temel ürün SKU'suzu tamamlar.

## <a name="identifying-add-ons"></a>Eklentileri tanımlama

İş ortakları API aracılığıyla SKU'ları alma ile ilgili SKU ayrıntılarını gözden geçirerek Eklentileri tanımlayabilir ve önkulların listelerini elde edebilir. Eklentiler, Etiketler sütunundaki yeni ticari lisans tabanlı fiyat listesinde de tanımlanır. Teklif matrisi, her bir eklenti ürünü SKU'su için önkulların listesini içerir.

## <a name="purchasing-add-ons"></a>Eklentileri satın alma

Eklentiler hem geleneksel lisans tabanlı hem de yeni ticari deneyimler için mevcuttur. Önemli fark, eklentilerin nasıl keşfedil olduğudur. Yeni ticari eklentiler keşfedildi ve katalogdan satın alındı. Aynı yerde temel teklifler veya önkullar bulunur. Geleneksel lisans tabanlı eklentiler yalnızca temel teklifin abonelik ayrıntıları sayfasına gidip keşfedilebilir ve eklenir. 

Katalogda yeni ticari deneyim eklentileri keşfedildi ve satın alındı. İş ortakları, ürün türü açılan listesinden yeni ticari eklentilere göre filtre ekleyebilir. Eklenti ürünleri, ürün SKU'su'nun yanındaki bilgi simgesiyle tanımlanır. İş ortakları eklentinin önkoşulları hakkında daha fazla bilgi almak için bu simgeye tıklar.

İş ortakları, iş ortağının verilen bir eklentiyi  satın almaları için mevcut olması gereken Ürün SKI'larının listesini göstermek için Uyumlu temel ürün aboneliklerini görüntüle'ye tıklayarak bir eklenti için gerekli ürünler hakkında daha fazla ayrıntıya ulaşabilirsiniz.

## <a name="add-on-enforcement"></a>Eklenti zorlaması

İş ortakları, müşterinin önkulları yoksa yeni bir ticari eklenti ürünü satın alma girişiminde bulundurarak eklentiler hakkında yararlı bilgiler edinecek. İş ortakları, bir eklentinin önkoşullarının katalogda mevcut olup olmadığını İş Ortağı Merkezi ve sayfa deneyimlerini gözden geçirebilirsiniz. Eklentinin destek önkoşulları yoksa, kullanıcı arabirimi "Eklenti uyumlu bir temel ürün olmadan temizlenebilir değil" iletisi görüntüler. CreateCart API'sini kullanan iş ortakları, eklentide gerekli ürün SKI'ları yoksa sepet satır öğesi üzerinde bir hatayla karşınıza gelir. Hata kodu şu 400041 "Eklenti uyumlu bir temel ürün olmadan temizlenebilir değil" açıklamasıyla birlikte gelecektir.

## <a name="important-details-when-purchasing-add-ons"></a>Eklentileri satın alırken önemli ayrıntılar

Müşteri önkulları karşılarsa eklentiler ayrı ürün SKÜ'leri olarak satın alınabilir. Eklenti aboneliklerinin kendi ayrı terim hizalaması vardır. Eklenti satın alan iş ortakları terimi ve ilişkili bitiş tarihi ile önkullar aynı olmayacaktır. Her iki abonelik de yeni terimlere otomatik olarak yenilene sürece önkul ve eklentiler düzgün çalışmaya devam eder. İş ortağı, önkquisite'ın süresi otomatik olarak yenilenmeden sona ererse, iş ortağının artık gerekli olmadığı sonucuna varırsa eklentinin eklenti süresi sonunda otomatik olarak yenilenmeyecek şekilde güncelleştirilmiş olması gerekir.  İş ortakları, ürün SKU'larını zaten eklenti hizmetleri olan daha yüksek bir SKU'ya dönüştürür ve eklentiyi kapatmak için destekle bir hizmet isteği ekleyebilir.

İş ortaklarının, temel tekliflerde gerekli uyumu sağlamak için edinilen eklentiler için bitiş tarihleri terimini yönetmesi beklenir.
