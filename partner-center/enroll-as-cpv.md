---
title: Satıcı olarak Denetim Masası kaydetme
description: CSP iş ortağı sistemlerini Denetim Masası API'lerle daha iyi tümleştire İş Ortağı Merkezi bir Satıcı (CPV) İş Ortağı Merkezi öğrenin.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 01/15/2021
ms.openlocfilehash: edc0ea8f0fda58f23cbce82bc7023a3277517cc3
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147148"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a>CSP iş ortağı sistemlerini Denetim Masası API'lerle tümleştirin ve satıcı olarak İş Ortağı Merkezi olun


**Uygun roller:** Genel yönetici

Bir Denetim Masası Satıcısı (CPV), Bulut Çözümü Sağlayıcısı (CSP) iş ortakları tarafından sistemlerini İş Ortağı Merkezi API'lerle tümleştirerek kullanmaları için uygulamalar geliştiren bağımsız bir yazılım satıcısıdır. Bir Denetim Masası satıcı, İş Ortağı Merkezi panosuna veya İş Ortağı Merkezi ERIŞIMI olan bir CSP İş Ortağı Merkezi değildir.

İster mevcut bir Denetim Masası Satıcısı (CPV) ister Microsoft iş ortaklarıyla çalışmak isteyen yeni bir CPV olun, Microsoft artık uygulamalarınızı kaydetmek ve iş ortaklarını desteklemek için İş Ortağı Merkezi'a kaydolmanızı Bulut Çözümü Sağlayıcısı gerektirir. Bir hesap oluşturmak için, CPV iş ortağı var olan bir CSP iş ortağı kiracısını veya mevcut CPV kiracısını kullanabilir ya da ekleme işleminin bir parçası olarak yeni bir kiracı oluşturabilir. CPV iş ortağı mevcut CSP kiracıyı kullanmayı seçerse, ayrı çok kiracılı uygulamalar oluşturmaları ve bunları CPV etkinlikleri için İş Ortağı Merkezi kaydetmeleri gerekir. Bir uygulama hem CSP hem de CPV uygulaması olarak kaydedilene. Uygulamanıza kaydolarak İş Ortağı Merkezi uygulamalarınızı kaydettikten sonra, uygulama API'lerine İş Ortağı Merkezi olur.  Korumalı alan hesabına ihtiyacınız varsa Microsoft Desteği isteğiyle Microsoft'a ulaşın. Zaten bir korumalı alan hesabınız varsa, bunu kullanmaya devam edersiniz. Yeni bir korumalı alana ihtiyacınız olmayacak

Microsoft [Denetim Masası Satıcı sözleşmesini gözden geçirme](https://go.microsoft.com/fwlink/?linkid=2055198)


## <a name="working-in-partner-center"></a>İş Ortağı Merkezi'da çalışma

İş Ortağı Merkezi CPV deneyimine kaydolarak CPV anlaşmasını kabul edin:

- Çok kiracılı uygulamaları yönetme (uygulamalarınızı Azure portal, kaydetme ve uygulama kaydını İş Ortağı Merkezi).

    >[!Note] 
    >Iş Ortağı Merkezi API 'Lerine yetki almak için, CPVs 'in uygulamalarını Iş Ortağı Merkezi 'ne kaydetmesi gerekir. Uygulamaları tek başına Azure portal eklemek, Iş Ortağı Merkezi API 'Leri için CPV uygulamalarına yetki vermez. 

- CPV profilinizi görüntüleyin ve yönetin 

- CPV özelliklerine erişmesi gereken kullanıcılarınızı görüntüleyin ve yönetin. Genel yönetici, bir CPV 'nin sahip olduğu tek roldür.

## <a name="next-steps"></a>Sonraki adımlar

-[Iş Ortağı Merkezi hesabınıza ek kiracılar ekleyin](multi-tenant-account.md)