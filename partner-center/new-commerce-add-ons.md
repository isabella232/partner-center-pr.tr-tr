---
title: Yeni ticari eklentiler
ms.topic: article
ms.date: 09/03/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Eklentiler satın almak için yeni ticari deneyimler hakkında bilgi edinin.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c944dc5de89ad0e9d6332252d722de90250c82c6
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129072759"
---
# <a name="introduction-new-commerce-add-ons"></a>Giriş: Yeni ticari eklentiler

**Uygun roller:** Yönetici aracısı | Satış aracısı | Genel yönetici

> [!NOTE]
> Yeni ticaret deneyimi değişiklikleri şu anda yalnızca Microsoft 365/Dynamics 365 yeni ticaret deneyimi teknik önizlemesinde yer alan iş ortakları tarafından kullanılabilir.

İş ortakları, daha önce satın alınan bir ürünü en iyi şekilde sağlayan diğer hizmetleri etkinleştirmek için yeni ticarette eklentiler satın alınabilir. Bunlara örnek olarak arama planları, daha fazla disk alanı veya müşterinin temel hizmetleri varsa eklen diğer özellikler örnek olarak verilmiştir.

## <a name="add-ons-in-new-commerce"></a>Yeni ticarette eklentiler

Yeni ticari eklentiler, geleneksel lisans tabanlı eklentilere benzer kavramlar içerir. Geleneksel lisans tabanlı gibi yeni ticari eklentilerde önkullar kavramı da yer almaktadır. Bunlar, eklentinin düzgün çalışması için müşterinin sahip olması gereken ürün SKI'larıdır. Bir eklentinin önkulları, verili bir SKU için katalog API'leri bulunabilir ve İş Ortağı Merkezi kullanıcı deneyiminde bulunabilir. Satın alma eklentileri, müşteri kiracısı üzerinde bir veya daha fazla önkul gerektirir.

Geleneksel lisans tabanlı ve yeni ticaret arasındaki eklentilerin satın alımında en önemli fark, *satın* almalarıdır. Geleneksel lisans tabanlında iş ortağı, eklentiyi mevcut bir temel teklif aboneliğine uygular. Yeni ticarette iş ortakları eklentileri katalogdan satın alıyor, artık temel teklifler ve eklentiler için iki yönlü satın alma deneyimine sahip değil, her şey yeni ticarette katalogda yer alıyor.

Hizmetler açısından bakıldığında, eklentilerin nasıl iştığıyla ilgili kavramların çoğu geleneksel ve yeni ticarette doğru olmaya devam ediyor. Hem kaydolma hem de eklenti hizmetlerini sağlama, sağlamanın nasıl olduğu konusunda hiçbir fark yoktur. Ayrıca, tek bir eklentinin hizmetleri, eklentinin birlikte çalışmak üzere tasarlansa bile birden fazla temel ürün SKU'suzu tamamlar.

## <a name="identifying-add-ons"></a>Eklentileri tanımlama

İş ortakları API aracılığıyla SKU'ları alma ile ilgili SKU ayrıntılarını gözden geçirerek Eklentileri tanımlayabilir ve önkulların listelerini elde edebilir. Eklentiler, Etiketler sütunundaki yeni ticari lisans tabanlı fiyat listesinde de tanımlanır. Teklif matrisi, her bir eklenti ürünü SKU'su için önkulların listesini içerir.

## <a name="purchasing-add-ons"></a>Eklentileri satın alma

Eklentiler hem geleneksel lisans tabanlı hem de yeni ticari deneyimler için mevcuttur. Önemli fark, yeni ticarinin katalogdan bulunabilirliği ve satın almayı, temel tekliflerin veya önkulların bulunduğu yerde olanaklı olmasıdır. Geleneksel lisans tabanlı eklentiler yalnızca temel teklifin abonelik ayrıntıları sayfasına gidip keşfedilebilir ve satın alınabilir. Burada bir eklenti listelendikten sonra iş ortağı istenen eklentiyi uygular.

Katalogda yeni ticari deneyim eklentileri keşfedildi ve satın alındı. İş ortakları, ürün türü açılan listesinden yeni ticari eklentilere göre filtre ekleyebilir. Add-on ürünlerinin yanında bir bilgi simgesi olduğu için bunları görmek de kolaydır. Bu, Eklenti durumlarını ve anlamını açıklar.

İş ortakları, iş ortağının verilen bir eklentiyi  satın almaları için mevcut olması gereken Ürün SKI'larının listesini göstermek için Uyumlu temel ürün aboneliklerini görüntüle'ye tıklayarak bir eklenti için gerekli ürünler hakkında daha fazla ayrıntıya ulaşabilirsiniz.

## <a name="add-on-enforcement"></a>Eklenti zorlaması

İş ortakları yeni bir ticari eklenti ürünü satın alma girişiminde bulundurarak müşterinin önkquisite sahip olmadığını hatalarla karşılar. İş ortakları, iş ortağı merkezinde validateAddon API'sini çağırarak müşterinin önkullara uygun olduğunu doğrular.

## <a name="important-details-when-purchasing-add-ons"></a>Eklentileri satın alırken önemli ayrıntılar

Müşteri önkulları karşılarsa eklentiler ayrı ürün SKÜ'leri olarak satın alınabilir. Eklenti aboneliklerinin kendi ayrı terim hizalaması vardır. Eklenti satın alan iş ortakları terimi ve ilişkili bitiş tarihi ile önkullar aynı olmayacaktır. Her iki abonelik de yeni terimlere otomatik olarak yenilendikse önkul ve eklentiler yeterli olacaktır. İş ortağı, önkquisite'ın süresi otomatik olarak yenilenmeden sona ererse, iş ortağının artık gerekli olmadığı sonucuna varırsa eklentinin eklenti süresi sonunda otomatik olarak yenilenmeyecek şekilde güncelleştirilmiş olması gerekir.  İş ortakları, ürün SKU'larını zaten eklenti hizmetleri olan daha yüksek bir SKU'ya dönüştürür ve eklentiyi kapatmak için destekle bir hizmet isteği ekleyebilir.

İş ortaklarının temel tekliflerde gerekli uyumu sağlamak için edinilen eklentiler için bitiş tarihleri terimini yönetmesi beklenir.
