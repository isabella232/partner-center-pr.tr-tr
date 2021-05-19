---
title: Kaizala Pro aboneliklerini Microsoft 365'e geçirme
description: Kaizala Pro aboneliklerini Microsoft 365 veya Office 365 sürümlerine geçirmeyi öğrenin. Müşterilerinizin geçişini hakkında daha fazla bilgi için bu makaleyi okuyun.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 583e9c40bb8d161c30440f12331dc8dcbf3db417
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146434"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a>Kaizala Pro tek başına aboneliklerini Microsoft 365 veya Office 365 sürümlerine geçirin

**Uygun roller**: satış Aracısı

1 Temmuz 2020 ' den itibaren geçerli olan Microsoft, Kaizala Pro tek başına hizmetinin satışlarını sonlandırıyor. Müşteriler artık bu tarihten sonra yeni Kaizala Pro abonelikleri satın amayacak ve mevcut Kaizala Pro abonelikleri süreleri dolduğunda otomatik olarak yenilenmeyecektir.

Müşterilerin devamlılığını sağlamak için, süresi dolan Kaizala Pro tek başına aboneliklerine sahip müşterileri aşağıda listelenen desteklenen bir SKU seçeneğine geçirmeniz gerekir. Müşterilerin hizmet kesintilerinden kaçınmak için, aboneliğin yıllık bitiş tarihinden önce müşterileri yeni aboneliklere taşımayı öneririz.

API 'yi (CREST veya Partner Center) kullanıyorsanız, otomatik yenileme özelliği false olarak ayarlanmış şekilde, aboneliğin bitiş tarihini değerlendirerek süresi dolan abonelikleri bulabilirsiniz: `auto renew = False` .

E4 abonelikleri `auto renew=False` 1 temmuz 2020 tarihinde olarak ayarlanır. Müşterileri dilediğiniz zaman yeni bir plana taşıyabilirsiniz.

## <a name="kaizala-pro-standalone-replacement-plans"></a>Kaizala Pro tek başına değiştirme planları

Yeni planlar sayesinde, müşterileriniz Microsoft 365 yeni özelliklerden ve işlevlerden faydalanabilir. Fiyatlandırma ayrıntıları, Iş Ortağı Merkezi 'nde fiyat listesi ve teklif listesi matrisinde bulunur.

- [**İş için Microsoft 365**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), şunlar dahil:  
   - Microsoft 365 İş temel
   - Microsoft 365 İş standart
   - Microsoft 365 İş Premium
    
- [**Frontline için Microsoft 365**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), şunlar dahil:
   - Microsoft 365 F3 (eski adıyla Microsoft 365 F1) ve Office 365 F3
    
- [**Microsoft 365 için şu şekildedir:**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans) 
   - Office 365 E1
   - Microsoft 365 E3 ve Office 365 E3
   - Microsoft 365 E5 ve Office 365 E5

- [**Microsoft 365 için eğitim,**](https://www.microsoft.com/education/buy-license/microsoft365)örneğin: 
    - Microsoft 365 A1 ve Office 365 A1
    - Microsoft 365 A3 ve Office 365 A3
    - Microsoft 365 A5 ve Office 365 A5

## <a name="transition-customers-to-new-product-plans"></a>Müşterileri yeni ürün planlarına geçiş

Microsoft, iş ortaklarımıza sürekli olarak yeni ürün ve hizmetler sunmaktadır. Bu gibi durumlarda, müşterileri yeni hizmetlere yükseltmeniz veya aboneliklerini sonunda kapatılacak olan SKUS'lardan geçirmeniz gerekir. Müşterileri, eski SKÜ'lerden yeni SKUS'lara şu adımların atılması gerekir:

A. Yeni aboneliği satın alma

B. Geçerli kullanıcı lisanslarını yeniden atama

C. Eski aboneliği iptal etme


## <a name="migrate-your-customers-to-new-plans"></a>Müşterilerinizi yeni planlara geçirme

### <a name="a-purchase-the-new-subscription"></a>A. Yeni aboneliği satın alma

1. Yeni aboneliği satın almak için, **İş Ortağı Merkezi** menüsünden Müşteriler'i **seçin,** taşımak istediğiniz müşteriyi seçin ve ardından Abonelik **ekle'yi seçin.**

2. Katalogdan satın almak istediğiniz aboneliği seçin (bu durumda, yukarıdaki seçeneklerden biri), lisans sayısını girin ve gönder'i **seçin.**

Müşterinizin artık hem eski hem de yeni abonelikleri, eski Kaizala Pro Tek Başına aboneliği ve yeni 'hedef' aboneliği (örneğin, Seçenek 1 - Office 365 Kurumsal F1) olması gerekir.

### <a name="b-reassign-current-user-licenses"></a>B. Geçerli kullanıcı lisanslarını yeniden ata

1. Müşterinin kullanıcılarının lisanslarını yeniden atamak için **Iş Ortağı Merkezi** menüsünden **müşteriler**' i seçin, taşıdığınız müşteriyi seçin ve ardından **Kullanıcılar ve lisanslar**' ı seçin. Müşterinin kullanıcılar ve lisanslar sayfası açılır.

2. Kullanıcı lisansını yeniden atamak için, yeniden atanacak kullanıcıyı seçin ve ardından **Lisansları Yönet**' i seçin.

3. **Lisansları Yönet** sayfasında Kaizala Pro tek başına Lisansı onay kutusunu temizleyin ve müşterinin taşınmakta olduğu abonelik için yeni bir hizmet planı seçin.

4.  **Gönder**’i seçin. Bir onay sayfası yeni lisans atamalarını listeler. Lisans atamaları gerektiren diğer kullanıcılar için aynı işleme devam edin.

### <a name="c-cancel-old-subscription"></a>C. Eski aboneliği iptal et

Kullanıcı lisansını yeni hizmete taşıdıktan sonra, kullanımdan kaldırılan aboneliği müşteri düzeyinde güvenle iptal edebilirsiniz.

1.  **Iş Ortağı Merkezi** menüsünde **müşteriler**' i seçin. Aboneliğini iptal ettiğiniz müşteriyi seçin.

2.  Abonelik Ayrıntıları sayfasında, aboneliği **askıya alındı** olarak ayarlayın.

3.  **Gönder**’i seçin.

Eski abonelik askıya alındı ve yeni abonelik etkin. Askıya alınan abonelik 120 gün sonra otomatik olarak sağlanacaktır. Müşteri, eski abonelik için ek maliyet içermez.
