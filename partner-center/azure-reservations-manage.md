---
title: Müşteriler için Azure ayırmalarını yönetme
description: Bir ayırmayı iptal etme, ayırmayı değiştirme veya para iadesi isteme dahil olmak üzere bir müşterinin Azure ayırmalarını yönetmeyi öğrenin.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 627c6f8d09a904e7d988c4229ec10eeac38dc2e9
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248331"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a>müşteriler için ayırmaları yönetin, iptal edin, exchange veya para iadesi Microsoft Azure

**Uygun roller**: yönetici Aracısı | Genel yönetici | Yardım Masası Aracısı | Satış Aracısı | Kullanıcı Yönetimi Yöneticisi

Bu makalede, bir rezervasyon iptal edilmesi, bir rezervasyon alışverişi veya bir para iadesi istemek dahil olmak üzere bir müşterinin Azure ayırmalarını nasıl yöneteceğiniz açıklanmaktadır.

> [!NOTE]
> bu makale yalnızca Bulut Çözümü Sağlayıcısı (CSP) programındaki iş ortakları için geçerlidir. diğer abonelik türleri (örneğin, kullandıkça öde, bireysel, Microsoft müşteri sözleşmesi veya Kurumsal Anlaşma abonelikleri) kullanan müşteriler [bu Azure ayırmaları belgelerini](/azure/cost-management-billing/reservations)okumalı olmalıdır.

Müşterilerinizin Azure ayırmaları satın alma sonrası 'yı yönetmek için, Iş Ortağı Merkezi 'nde yönetmek istediğiniz müşteriyi ve rezervasyonu seçip Azure portal rezervasyon üzerinde değişiklikler yapmanız gerekir.

1. Başlamak için Iş Ortağı Merkezi menüsünden **müşteriler** ' i seçin ve ardından rezervasyonlarını yönetmek istediğiniz müşteriyi seçin. 

2. Müşterinin ayrıntı sayfası menüsünde **Azure ayırmaları** ' ni seçin ve ardından yönetmek istediğiniz belirli ayırmayı seçin.  

3. **Eylemler**' in altında, Azure Portal müşterinin rezervasyon kaydına gitmek için **Yönet** ' i seçin. Ayırma ayrıntısı sayfasında, görevleri gerçekleştirmek için aşağıdaki adımları izleyin.  

    | **Seç**   | **Kime**    |
    |:-----------------------------|:-----------------|
    | **Genel Bakış**   | Sona erme tarihi, kapsamı ve kullanım verileri dahil olmak üzere müşterinin rezervasyonunun ayrıntılarını görüntüleyin. **Göz önünde** Profesyonel olarak derecelendirilmiş bir para iadesi için destek isteği oluşturmak üzere **para iadesi** ' ni seçin. ayırma döneminizin kullanılmayan kısmını değiştirmek için bir destek isteği oluşturmak üzere **Exchange** ' yi seçin.  
    | **Access Control (ıAM)**   | Müşterinin rezervasyon bilgilerine erişimi yönetin.|
    | **Yapılandırma**   | Rezervasyonun kapsamını ve/veya ayırmanın ilişkilendirildiği Azure aboneliğini değiştirin.    |
    | **Özellikler**   | Rezervasyonun özelliklerini görüntüleyin ve rezervasyon KIMLIĞI ve rezervasyon siparişi KIMLIĞINI panoya kopyalayın. **Göz önünde** Destek, bir müşteri adına destek istediğinizde rezervasyon KIMLIĞI ve rezervasyon siparişi KIMLIĞINI isteyebilir.    |
    | **Yeni destek isteği**    | Microsoft Desteği yardım isteyin.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Bir ayırmayı iptal etme veya değiştirme

Müşterinin iş gereksinimlerinin herhangi bir noktasında değişmesi durumunda, bir ayırmayı iptal etmek ve bir geri ödeme veya Exchange 'in eşit olarak dağıtılmış para iadesi tutarını yeni bir ayırma fiyatına doğru bir şekilde kullanmak isteyebilirler.

Bu senaryoların her ikisinde de, Microsoft bu miktarı, daha sonra müşterilere göre elde edilen mali işlemleri yönetebilmeniz için tutarında bir para iadesi. Microsoft, doğrudan faturalandırma, iptaller veya para iadesi hakkında müşterilerle iletişim kurmaz.

### <a name="how-cancellations-work"></a>İptallerin çalışması

Müşteriler herhangi bir zamanda rezervasyon iptal etme isteğinde bulunabilir (para iadesi miktarı yıl başına $50.000). Bir ayırmanın iptal edilmesi, müşterinin erken sonlandırma ücreti için bir Azure rezervasyonunun kalan ayların miktarını döndürmesini sağlar. Kalan eşit oranda dağıtılmış Bakiye, eksi erken sonlandırma ücreti, müşterinin hesabını iade edebilmeniz için hesabınıza iade edilir. 

İptal ayrıntıları ve ücretleri için aşağıya bakın.


|**İptal tarihi**<br> miş   |**Kullanım**    |**Kredi**  |**Erken sonlandırma**<br> masraf    |**Para iadesi üst sınırı** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 veya daha az                         | No          | %100       | No                              | $50.000 ABD DOLARı   |
|5 veya daha az                         | Yes         | Pro dereceli  | No                              | $50.000 ABD DOLARı   |
|5 ' ten fazla                        | No          | Pro dereceli  | %12                             | $50.000 ABD DOLARı   |
|5 ' ten fazla                        | Yes         | Pro dereceli  | %12                             | $50.000 ABD DOLARı   |

### <a name="how-exchanges-work"></a>Alışverişlerde nasıl çalışır? 

Bir müşteri, sizin için ilk satın alındıklarından farklı bir ayırma satın almak isterse bir Exchange isteğinde bulunabilir. Bir ayırmayı değiştirmek, müşterinin, eşit olarak dağıtılan para iadesi miktarını yeni ayırma fiyatına doğru kullanmasına izin verdiğinden bir ayırmayı iptal etme konusunda etkileyici bir alternatif olabilir. 

Müşteriye bir Exchange sunabilmeniz için eşit olarak dağıtılmış para iadesi miktarı hesabınıza alacaklandırılır.

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Müşteri adına bir para iadesi veya değişim isteme

Müşterileriniz adına bir para iadesi veya Exchange için destek talebi sağlamak üzere, Iş Ortağı Merkezi 'nde müşteriyi ve rezervasyonu seçin ve ardından Azure portal Destek isteğini oluşturun. 

>[!NOTE]
>Microsoft Desteği aracılar, rezervasyon KIMLIĞI ve rezervasyon siparişi KIMLIĞINI sağlamanızı isteyebilir. Bu bilgileri, Azure portal rezervasyon 'nin **Özellikler** sayfasında bulabilirsiniz.

1. Başlamak için Iş Ortağı Merkezi menüsünden **müşteriler** ' i seçin ve ardından para iadesi isteyen müşteriyi seçin. 

2. Müşterinin ayrıntı sayfasında, **Azure ayırmaları** ' i seçin ve müşterinin iade etmek istediği belirli bir ayırmayı seçin.  

3. **Eylemler**' in altında, Azure Portal müşterinin rezervasyon kaydına gidip bir destek talebi başlatmak Için **para iadesi** ' ni seçin.  

4. **Yeni destek isteği** sayfasında, bir para iadesi istemek için aşağıdaki adımları izleyin. Her adımdan sonra **İleri ' yi** seçin. 

   |**Adım**                    |**Seçenek**    |
   |:---------------------------|:-----------------|
   |**1 temel bilgiler**                |Sorun türü: Faturalandırma.  |
   |**2 sorun**               |Sorun türü: ayırma yönetimi. Kategori: alışverişlerde ve para iadesi. |
   |**3 iletişim bilgileri**   |Tercihlerinizi seçin ve gerekli bilgileri girin. 

5. İşiniz bittiğinde **Oluştur** ' u seçin.

## <a name="azure-reservations-resources"></a>Azure ayırmaları kaynakları

|**Hakkında bilgi için**   |**Bunu okuyun**    |
|:-----------------------------|:-----------------|
|CSP 'de Azure ayırmaları genel bakış  | [ayrılmış Microsoft Azure örnekleri satma](azure-reservations.md) |
|Iş Ortağı Merkezi 'nde müşterileriniz için Azure ayırmaları satın alma   | [Azure ayırmaları satın alma](azure-reservations-buying.md) |
|Doğru VM boyutunu belirleme ve müşteri VM kullanımını doğrulama   | [Maksimum Azure ayırma kullanımı için VM boyutu](azure-usage.md)   |
|Iş Ortağı Merkezi API 'sini kullanarak Azure ayırmaları satın alma | [Azure ayrılmış VM örneklerini](/partner-center/develop/purchase-azure-reservations) Iş Ortağı Merkezi geliştirici belgelerinde satın alma   |
|Müşterilere satın almış olduğunuz bir abonelikten kendi Azure ayırmalarını satın alma izni verme. | [Müşterilere kendi Azure ayırmalarını satın alma izni verin](give-customers-permission.md)   |