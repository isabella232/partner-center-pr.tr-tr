---
title: Rezervasyonları Microsoft Azure müşterilere satma
description: Bir bulut çözümü sağlayıcısı olarak müşteriler için Azure ayırmaları satın alabilir, sattabilir veya yönetebilirsiniz. Iş Ortağı Merkezi, Azure portal veya Iş Ortağı Merkezi API 'sini kullanın.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 9dc92685503fd4b9b05e40337f72e810c1693779
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534905"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a>Iş Ortağı Merkezi, Azure portal veya API 'Leri kullanarak müşterilere Microsoft Azure ayırmaları satma

**Uygun roller**

- Yönetim Aracısı
- Genel yönetici
- Yardım Masası Aracısı
- Satış Aracısı
- Kullanıcı Yönetimi Yöneticisi

Bulut çözümü sağlayıcısı programı 'nda (CSP) bir iş ortağı olarak müşteriler için Azure ayırmaları satın alabilir, sattabilir veya yönetebilirsiniz. Iş Ortağı Merkezi, Azure portal veya Iş Ortağı Merkezi API 'sini kullanın.

> [!NOTE]
> Bu makale yalnızca CSP 'deki iş ortakları için geçerlidir. Diğer abonelik türleri (örneğin, Kullandıkça öde, bireysel, Microsoft Müşteri Sözleşmesi veya Kurumsal Anlaşma abonelikleri) kullanan müşteriler [Bu Azure ayırmaları belgelerini](/azure/cost-management-billing/reservations)okumalı olmalıdır.

CSP programındaki iş ortakları, müşterilerine Microsoft Azure ayırmaları sunabilir. Müşteriler, önceden ayrıldıklarında önemli tasarruf elde edebilirler. Azure ayırmaları, müşterileri basitliği ve esnekliği aşağıdaki yollarla sunmaktadır:

- Bir veya üç yıllık rezervasyon terimi
- Kullanmaya başlamak kolaydır; Kurulum saniye cinsinden tamamlandı
- Ayarlanmış para iadesi için dilediğiniz zaman ayrılan örnekleri iptal edin veya değiştirin
- Ayrılmış örnek kullanımını kurumsal veya ayrı departman düzeyinde yönetme

Azure ayırmaları, müşterilere aşağıdaki yollarla yol açabilir:

- Rezervasyonlar, Kullandıkça Öde (PAYG) fiyatlandırmasına göre önemli tasarruf sağlayabilir
- Tek yıllık veya üç yıllık şartlar için ön ödeme ile daha iyi bütçeleme ve tahmin
- Azure bölgesinde ofislerine en yakın önceliğe sahip bilgi işlem kapasitesi
- Azure ayırmaları, Microsoft Windows Server ve Azure SQL veritabanı gibi yazılımlarla birleştirildiğinde uçtan uca altyapı çözümlerine yönelik temel sağlar

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