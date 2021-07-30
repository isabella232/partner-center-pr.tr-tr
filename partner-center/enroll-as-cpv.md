---
title: Satıcı olarak Denetim Masası kaydetme
description: CSP iş ortağı sistemlerini Denetim Masası API'lerle daha iyi tümleştire İş Ortağı Merkezi bir Satıcı (CPV) İş Ortağı Merkezi öğrenin.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 01/15/2021
ms.openlocfilehash: 6e31dfd73d2563bc6b41227a702690d74b7f306d
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114845729"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a>CSP iş ortağı sistemlerini Denetim Masası API'lerle tümleştirin ve satıcı olarak İş Ortağı Merkezi olun


**Uygun roller:** Genel yönetici

Bir Denetim Masası Satıcısı (CPV), Bulut Çözümü Sağlayıcısı (CSP) iş ortakları tarafından sistemlerini İş Ortağı Merkezi API'lerle tümleştirerek kullanmaları için uygulamalar geliştiren bağımsız bir yazılım satıcısıdır. Bir Denetim Masası satıcı, İş Ortağı Merkezi panosuna veya İş Ortağı Merkezi ERIŞIMI olan bir CSP İş Ortağı Merkezi değildir.

Microsoft iş ortaklarıyla çalışmak isteyen mevcut Denetim Masası Satıcısı (CPV) veya yeni bir CPV olun, Microsoft artık uygulamalarınızı kaydetmek ve iş ortaklarını desteklemek için İş Ortağı Merkezi'a kaydolmanızı Bulut Çözümü Sağlayıcısı gerektirir. Bir hesap oluşturmak için, CPV iş ortağı var olan bir CSP iş ortağı kiracısını veya mevcut CPV kiracısını kullanabilir ya da ekleme işleminin bir parçası olarak yeni bir kiracı oluşturabilir. CPV iş ortağı mevcut CSP kiracıyı kullanmayı seçerse, ayrı çok kiracılı uygulamalar oluşturmaları ve bunları CPV etkinlikleri için İş Ortağı Merkezi kaydetmeleri gerekir. Bir uygulama hem CSP hem de CPV uygulaması olarak kaydedileyemz. Uygulamanıza kaydolarak İş Ortağı Merkezi uygulamalarınızı kaydettikten sonra, uygulama API'lerine İş Ortağı Merkezi olur.  Korumalı alan hesabına ihtiyacınız varsa Microsoft Desteği isteğiyle Microsoft'a ulaşın. Zaten bir korumalı alan hesabınız varsa, bunu kullanmaya devam edersiniz. Yeni bir korumalı alana ihtiyacınız olmayacak

Microsoft [Denetim Masası Satıcı sözleşmesini gözden geçirme](https://go.microsoft.com/fwlink/?linkid=2055198)


## <a name="working-in-partner-center"></a>İş Ortağı Merkezi'da çalışma

İş Ortağı Merkezi CPV deneyimine kaydolarak CPV anlaşmasını kabul edin:

- Çok kiracılı uygulamaları yönetme (uygulamalarınızı Azure portal, kaydetme ve uygulama kaydını İş Ortağı Merkezi).

    >[!Note] 
    >CPV'lerin api'ler İş Ortağı Merkezi için yetki almak için uygulamalarını İş Ortağı Merkezi gerekir. Uygulamalar tek başına Azure portal api'ler için CPV uygulamalarını İş Ortağı Merkezi yetkilendirmez. 

- CPV profilinizi görüntüleme ve yönetme 

- CPV özelliklerine erişmesi gereken kullanıcılarınızı görüntüleme ve yönetme. CPV'nin sahip olduğu tek rol genel yöneticidir.

## <a name="next-steps"></a>Sonraki adımlar

-[Hesap hesabınıza başka kiracılar İş Ortağı Merkezi ekleme](multi-tenant-account.md)