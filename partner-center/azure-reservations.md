---
title: rezervasyonları Microsoft Azure müşterilere satma
description: Bulut Çözümü Sağlayıcısı olarak, müşteriler için Azure ayırmaları satın alabilir, satmanıza veya yönetebilirsiniz. Iş Ortağı Merkezi, Azure portal veya Iş Ortağı Merkezi API 'sini kullanın.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 10a9789d10d03a1a6ddd0aa2cd5ccc0e320b9c07
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123959965"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a>iş ortağı merkezi, Azure portal veya apı 'leri kullanarak müşterilere Microsoft Azure ayırmaları satma

**Uygun roller**: yönetici Aracısı | Genel yönetici | Yardım Masası Aracısı | Satış Aracısı | Kullanıcı Yönetimi Yöneticisi

Bulut Çözümü Sağlayıcısı programında (CSP) bir iş ortağı olarak müşteriler için Azure ayırmaları satın alabilir, sattabilir veya yönetebilirsiniz. Iş Ortağı Merkezi, Azure portal veya Iş Ortağı Merkezi API 'sini kullanın.

> [!NOTE]
> Bu makale yalnızca CSP 'deki iş ortakları için geçerlidir. diğer abonelik türleri (örneğin, kullandıkça öde, bireysel, Microsoft müşteri sözleşmesi veya Kurumsal Anlaşma abonelikleri) kullanan müşteriler [bu Azure ayırmaları belgelerini](/azure/cost-management-billing/reservations)okumalı olmalıdır.

CSP programındaki iş ortakları, müşterilerine Microsoft Azure ayırmaları sunabilir. Müşteriler, önceden ayrıldıklarında önemli tasarruf elde edebilirler. Azure ayırmaları, müşterileri basitliği ve esnekliği aşağıdaki yollarla sunmaktadır:

- Bir veya üç yıllık rezervasyon terimi
- Kullanmaya başlamak kolaydır; Kurulum saniye cinsinden tamamlandı
- Ayarlanmış para iadesi için dilediğiniz zaman ayrılan örnekleri iptal edin veya değiştirin
- Ayrılmış örnek kullanımını kurumsal veya ayrı departman düzeyinde yönetme

Azure ayırmaları, müşterilere aşağıdaki yollarla yol açabilir:

- Rezervasyonlar, Kullandıkça Öde (PAYG) fiyatlandırmasına göre önemli tasarruf sağlayabilir
- Tek yıllık veya üç yıllık şartlar için ön ödeme ile daha iyi bütçeleme ve tahmin
- Azure bölgesinde ofislerine en yakın önceliğe sahip bilgi işlem kapasitesi
- Azure ayırmaları, Microsoft Windows Server ve Azure SQL Veritabanı gibi yazılımlarla birleştirildiğinde uçtan uca altyapı çözümlerine yönelik temel sağlar.

>[!NOTE]
> Azure ayırmalarını hem Iş ortağı merkezi hem de Azure portal satın alabilir, satın alabilir ve yönetebilirsiniz ve Iş Ortağı Merkezi API 'sini kullanabilirsiniz. Müşterilerinize satın almış olduğunuz bir Azure aboneliğinden kendi Azure ayırmalarını satın alma izni verebilirsiniz. Hakkında bilgi edinmek için aşağıdaki bağlantıları izleyin.

## <a name="azure-reservations-resources"></a>Azure ayırmaları kaynakları

|**Hakkında bilgi için**   |**Bunu okuyun**    |
|:-----------------------------|:-----------------|
| Müşterileriniz için Azure ayırmaları belgeleri | [Azure rezervasyonları nedir?](/azure/billing/billing-save-compute-costs-reservations)
|Iş Ortağı Merkezi 'nde müşterileriniz için Azure ayırmaları satın alma   |[Azure ayırmaları satın alma](azure-reservations-buying.md)
|Azure ayırmalarını Iş Ortağı Merkezi 'nde yönetme | [Azure ayırmalarını Iş Ortağı Merkezi 'nde yönetme](azure-reservations-manage.md)
|Doğru VM boyutunu belirleme ve müşteri VM kullanımını doğrulama   |[Maksimum Azure ayırma kullanımı için VM boyutu](azure-usage.md)   |
|Iş Ortağı Merkezi API 'sini kullanarak Azure ayırmaları satın alma | [Azure ayrılmış VM örneklerini](/partner-center/develop/purchase-azure-reservations) Iş Ortağı Merkezi geliştirici belgelerinde satın alma   |
|Kullanıcılara CSP aboneliğinizden kendi Azure ayırmalarını satın alma izni verme. | [Müşterilere kendi Azure ayırmalarını satın alma izni verin](give-customers-permission.md)   |