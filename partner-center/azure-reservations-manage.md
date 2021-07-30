---
title: Müşteriler için Azure rezervasyonlarını yönetme
description: Rezervasyonu iptal etme, rezervasyon değiştirme veya para iadesi isteği gibi bir müşteri için Azure rezervasyonlarını yönetmeyi öğrenin.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 627c6f8d09a904e7d988c4229ec10eeac38dc2e9
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114841479"
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
    | **Genel Bakış**   | Son kullanma tarihi, kapsam ve kullanım verileri de dahil olmak üzere müşterinin rezervasyon ayrıntılarını görüntüleme. **NOT** Para **İadesi'ne** seçerek provok olarak derecelendirilmiş bir para iadesi için destek isteği oluşturun. Rezervasyon **Exchange** kullanılmayan kısmını değiştirmek için bir destek isteği oluşturmak için Exchange'ı seçin.  
    | **Access Control (IAM)**   | Müşterinin rezervasyon bilgilerine erişimi yönetme.|
    | **Yapılandırma**   | Rezervasyonun kapsamını ve/veya rezervasyonun ilişkili olduğu Azure aboneliğini değiştirme.    |
    | **Özellikler**   | Rezervasyonun özelliklerini görüntülayıp panoya rezervasyon kimliği ile rezervasyon siparişi kimliğini kopyalayın. **NOT** Müşteri adına destek isteğide bulunduktan sonra destek sizden rezervasyon kimliğini ve rezervasyon sipariş kimliğini sorabilir.    |
    | **Yeni destek isteği**    | Microsoft Desteği.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Rezervasyonu iptal etme veya değiştirme

Müşterinin herhangi bir noktada iş ihtiyaçları değişirse, rezervasyonu iptal etmek ve bir para iadesi almak ya da yeni rezervasyonun fiyatında kullanılacak rezervasyonun prorat edilen para iadesi tutarını değiştirmek istiyor olabilir.

Bu senaryoların her ikisinde de Microsoft, elde edilen finansal işlemleri müşterilerinizle yönetecek şekilde size para iadesi sağlar. Microsoft faturalama, iptaller veya para iadeleri hakkında doğrudan müşterilerle iletişim kurmaz.

### <a name="how-cancellations-work"></a>İptaller nasıl çalışır?

Müşteriler, herhangi bir zamanda rezervasyonu iptal etmek için istekte olabilir (yıllık 50.000 ABD dolarına eşlenen para iadesi tutarı). Rezervasyonun iptal edilmesi, müşterinin azure rezervasyonlarının kalan aylarını erken sonlandırma ücreti karşılığında iade etmelerine olanak sağlar. Kalan dengeli bakiye (erken sonlandırma ücreti eksi) hesabınıza iade edilir ve böylece müşterinin hesabına para iadesi alabilirsiniz. 

İptal ayrıntıları ve ücretleri için aşağıya bakın.


|**İptal tarihi**<br> (gün)   |**Kullanım**    |**Kredi**  |**Erken sonlandırma**<br> Ücreti    |**Para iadesi sınırı** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 veya daha az                         | No          | %100       | No                              | 50.000 USD   |
|5 veya daha az                         | Yes         | Pro derecelendirilmiş  | No                              | 50.000 USD   |
|5'in üzerinde                        | No          | Pro derecelendirilmiş  | %12                             | 50.000 USD   |
|5'in üzerinde                        | Yes         | Pro derecelendirilmiş  | %12                             | 50.000 USD   |

### <a name="how-exchanges-work"></a>Değişimler nasıl çalışır? 

Müşteri ilk satın aldığı rezervasyondan farklı bir rezervasyon satın almak istiyorsa, değişim isteği alabilir. Rezervasyonun alışverişini yapmak, rezervasyonu iptal etmek için cazip bir alternatif olabilir çünkü müşterinin yeni rezervasyonun fiyatı için prorated para iadesi tutarını kullanmalarına olanak sağlar. 

Prorated para iadesi tutarı hesabınıza iade edilir, böylece müşteriye bir değişim teklifi sunabilirsiniz.

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Müşteri adına para iadesi veya değişim isteği

Müşterileriniz adına para iadesi veya değişim isteğinde bulunarak destek isteğinde bulunarak İş Ortağı Merkezi'de müşteriyi ve rezervasyonu seçerek destek isteğini Azure portal. 

>[!NOTE]
>Microsoft Desteği aracıları sizden rezervasyon kimliğini ve rezervasyon sipariş kimliğini sağlamayı sorabilir. Bu bilgileri, rezervasyonun Özellikler **sayfasındaki** Azure portal.

1. Çalışmaya başlama için, **İş Ortağı Merkezi** menüsünden Müşteriler'i seçin ve para iadesi almak isteyen müşteriyi seçin. 

2. Müşterinin ayrıntı sayfasında Azure rezervasyonları'nın **ardından** müşterinin para iadesi istediği rezervasyonu seçin.  

3. Eylemler **altında** Para **İadesi'ne** seçerek müşterinin rezervasyon kaydına gidin ve Azure portal isteği başlatın.  

4. Yeni **destek isteği sayfasında,** para iadesi isteği için aşağıdaki adımları izleyin. Her **adımdan** sonra Sonraki'yi seçin. 

   |**Adım**                    |**Seçim**    |
   |:---------------------------|:-----------------|
   |**1 Temel Bilgiler**                |Sorun türü: Faturalama.  |
   |**2 Sorun**               |Sorun türü: Rezervasyon yönetimi. Kategori: Değişimler ve para iadeleri. |
   |**3 İletişim bilgileri**   |Tercihlerinizi seçin ve gerekli bilgileri girin. 

5. Bittiğinde **Oluştur'a** seçin.

## <a name="azure-reservations-resources"></a>Azure rezervasyon kaynakları

|**Hakkında bilgi için**   |**Bunu okuyun**    |
|:-----------------------------|:-----------------|
|CSP'de Azure rezervasyonları genel bakış  | [Ayrılmış Microsoft Azure Satış](azure-reservations.md) |
|İş Ortağı Merkezi'de müşterileriniz için Azure rezervasyonları satın İş Ortağı Merkezi   | [Azure rezervasyonları satın alma](azure-reservations-buying.md) |
|Doğru VM boyutunu belirleme ve müşteri VM kullanımını doğrulama   | [Maksimum Azure rezervasyon kullanımı için VM boyutlandırması](azure-usage.md)   |
|İş Ortağı Merkezi API'sini kullanarak Azure rezervasyonları satın alma | [Geliştirici Azure Ayrılmış VM Örnekleri](/partner-center/develop/purchase-azure-reservations) belgelerinde İş Ortağı Merkezi satın alma   |
|Müşterilere, satın aldığınız abonelikten kendi Azure rezervasyonlarını satın alma izni verme. | [Müşterilere kendi Azure rezervasyonlarını satın alma izni verme](give-customers-permission.md)   |