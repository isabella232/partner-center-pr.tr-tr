---
title: Müşteriler için Azure rezervasyonlarını yönetme
description: Rezervasyonu iptal etme, rezervasyon değiştirme veya para iadesi isteği gibi bir müşteri için Azure rezervasyonlarını yönetmeyi öğrenin.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 1184b199d6235dd1d16fe981000bae44b797f76a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149494"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a>Müşteriler için rezervasyonları yönetme, iptal etme, değiştirme Microsoft Azure para iadesi alma

**Uygun roller:** Yönetici aracısı | Genel yönetici | Yardım masası aracısı | Satış aracısı | Kullanıcı yönetimi yöneticisi

Bu makalede, rezervasyonu iptal etme, rezervasyon değiştirme veya para iadesi isteği dahil olmak üzere bir müşteri için Azure rezervasyonlarını yönetme işlemi açıklanmıştır.

> [!NOTE]
> Bu makale yalnızca Bulut Çözümü Sağlayıcısı (CSP) programı iş ortakları için geçerlidir. Diğer abonelik türlerini (kullansanız öde, bireysel, Microsoft Müşteri Sözleşmesi veya Kurumsal Anlaşma abonelikler gibi) kullanan müşterilerin bu Azure rezervasyonları belgelerini [okuması gerekir.](/azure/cost-management-billing/reservations)

Satın alma sonrasında müşterinizin Azure rezervasyonlarını yönetmek için, İş Ortağı Merkezi'de yönetmek istediğiniz müşteriyi ve rezervasyonu seçer ve ardından Azure portal.

1. Çalışmaya başlama **için,** İş Ortağı Merkezi menüsünden Müşteriler'i seçin ve ardından rezervasyonlarını yönetmek istediğiniz müşteriyi seçin. 

2. Müşterinin ayrıntı sayfası menüsünde Azure **rezervasyonları'ı ve** ardından yönetmek istediğiniz rezervasyonu seçin.  

3. **Eylemler'in** **altında Yönet'i** seçerek müşterinin rezervasyon kaydına gidin ve Azure portal. Rezervasyon ayrıntıları sayfasında, görevleri tamamlamak için aşağıdaki adımları izleyin.  

    | **Seç**   | **Kime**    |
    |:-----------------------------|:-----------------|
    | **Genel Bakış**   | Son kullanma tarihi, kapsam ve kullanım verileri de dahil olmak üzere müşterinin rezervasyon ayrıntılarını görüntüleme. **NOT** Para **İadesi'ne** seçerek provok olarak derecelendirilmiş bir para iadesi için destek isteği oluşturun. Rezervasyon **döneminizin** kullanılmayan kısmını değiştirmek için bir destek isteği oluşturmak için Exchange'i seçin.  
    | **Access Control (IAM)**   | Müşterinin rezervasyon bilgilerine erişimi yönetme.|
    | **Yapılandırma**   | Rezervasyonun kapsamını ve/veya rezervasyonun ilişkili olduğu Azure aboneliğini değiştirme.    |
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
|5 veya daha az                         | Yes         | Pro-derecelendirilmiş  | No                              | 50.000 USD   |
|5'in üzerinde                        | No          | Pro-derecelendirilmiş  | %12                             | 50.000 USD   |
|5'in üzerinde                        | Yes         | Pro-derecelendirilmiş  | %12                             | 50.000 USD   |

### <a name="how-exchanges-work"></a>Değişimler nasıl çalışır? 

Müşteri ilk satın aldığı rezervasyondan farklı bir rezervasyon satın almak istiyorsa, değişim isteği alabilir. Rezervasyonun alışverişini yapmak rezervasyonu iptal etmek için cazip bir alternatif olabilir çünkü müşterinin yeni rezervasyonun fiyatı için prorated para iadesi tutarını kullanmalarına olanak sağlar. 

Prorated para iadesi tutarı hesabınıza iade edilir, böylece müşteriye bir değişim teklifi sunabilirsiniz.

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Müşteri adına para iadesi veya değişim isteği

Müşterileriniz adına para iadesi veya değişim isteğinde bulunarak destek isteğinde İş Ortağı Merkezi müşterisini ve rezervasyonu seçerek destek isteğini Azure portal. 

>[!NOTE]
>Microsoft Desteği aracıları sizden rezervasyon kimliğini ve rezervasyon sipariş kimliğini sağlamayı sorabilir. Bu bilgileri, rezervasyonun Özellikler **sayfasındaki** Azure portal.

1. Çalışmaya başlama için, **İş Ortağı Merkezi** menüsünden Müşteriler'i seçin ve para iadesi almak isteyen müşteriyi seçin. 

2. Müşterinin ayrıntı sayfasında Azure rezervasyonları'nın **ardından** müşterinin para iadesi istediği rezervasyonu seçin.  

3. Eylemler **altında** Para **İadesi'ne** seçerek müşterinin rezervasyon kaydına gidin ve Azure portal isteği başlatın.  

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
|CSP 'de Azure ayırmaları genel bakış  | [Ayrılmış Microsoft Azure örnekleri satma](azure-reservations.md) |
|Iş Ortağı Merkezi 'nde müşterileriniz için Azure ayırmaları satın alma   | [Azure ayırmaları satın alma](azure-reservations-buying.md) |
|Doğru VM boyutunu belirleme ve müşteri VM kullanımını doğrulama   | [Maksimum Azure ayırma kullanımı için VM boyutu](azure-usage.md)   |
|Iş Ortağı Merkezi API 'sini kullanarak Azure ayırmaları satın alma | [Geliştirici Azure Ayrılmış VM Örnekleri](/partner-center/develop/purchase-azure-reservations) belgelerinde İş Ortağı Merkezi satın alma   |
|Müşterilere, satın aldığınız abonelikten kendi Azure rezervasyonlarını satın alma izni verme. | [Müşterilere kendi Azure rezervasyonlarını satın alma izni verme](give-customers-permission.md)   |