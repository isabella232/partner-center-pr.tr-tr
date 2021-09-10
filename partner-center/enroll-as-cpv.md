---
title: Denetim Masası satıcısı olarak kaydetme
description: CSP iş ortağı sistemlerini Iş Ortağı Merkezi API 'Leriyle daha iyi tümleştirebilmeniz için Iş Ortağı Merkezi 'nde bir denetim masası satıcısı (CPV) olarak nasıl kaydolacağınızı öğrenin.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 01/15/2021
ms.openlocfilehash: 6e31dfd73d2563bc6b41227a702690d74b7f306d
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960804"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a>CSP iş ortağı sistemlerini Iş Ortağı Merkezi API 'Leriyle tümleştirmenize yardımcı olmak için Denetim Masası satıcısı olarak kaydetme


**Uygun roller**: genel yönetici

denetim masası satıcısı (cpv), sistemlerini iş ortağı merkezi apı 'leriyle tümleştirmelerini sağlamak üzere Bulut Çözümü Sağlayıcısı (CSP) iş ortakları tarafından kullanılmak üzere uygulamalar geliştiren bağımsız bir yazılım satıcığıdır. Bir denetim masası satıcısı, Iş Ortağı Merkezi panosuna veya Iş Ortağı Merkezi API 'Lerine doğrudan erişimli bir CSP Iş ortağı değildir.

microsoft iş ortaklarıyla çalışmak isteyen geçerli bir denetim masası satıcısı (cpv) veya yeni bir cpv olsun, microsoft artık uygulamalarınızı kaydetmek ve Bulut Çözümü Sağlayıcısı iş ortaklarını desteklemek için iş ortağı merkezi 'ne kaydolmanızı gerektirir. Bir hesap oluşturmak için, bir CPV iş ortağı mevcut bir CSP iş ortağı kiracısı veya mevcut bir CPV kiracısı kullanabilir ya da ekleme sürecinin bir parçası olarak yeni bir kiracı oluşturabilir. CPV iş ortağı mevcut CSP kiracısını kullanmayı seçerse, ayrı bir çok kiracılı uygulamalar oluşturmalı ve bunları CPV etkinlikleri için Iş Ortağı Merkezi 'ne kaydetmeleri gerekir. Bir uygulama hem CSP hem de CPV uygulaması olarak kaydedilemez. Iş Ortağı Merkezi 'ne kaydolduktan ve uygulamalarınızı kaydettirdikten sonra, Iş Ortağı Merkezi API 'Lerine erişebilirsiniz.  Bir sandbox hesabına ihtiyacınız varsa Microsoft Desteği isteğiyle Microsoft ile iletişim kurun. Zaten bir korumalı alan hesabınız varsa, bu hesabı kullanmaya devam edin. Yeni bir korumalı alan gerekmez

[Microsoft Denetim Masası satıcı sözleşmesini](https://go.microsoft.com/fwlink/?linkid=2055198) gözden geçirin


## <a name="working-in-partner-center"></a>Iş Ortağı Merkezi 'nde çalışma

Iş Ortağı Merkezi CPV deneyimine kaydolduktan ve CPV sözleşmesini kabul etmeniz durumunda şunları yapabilirsiniz:

- Çok kiracılı uygulamaları yönetme (Iş Ortağı Merkezi 'nde uygulamaları Azure portal, kaydetmek ve kayıt silmek için uygulama ekleme).

    >[!Note] 
    >Iş Ortağı Merkezi API 'Lerine yetki almak için, CPVs 'in uygulamalarını Iş Ortağı Merkezi 'ne kaydetmesi gerekir. Uygulamaları tek başına Azure portal eklemek, Iş Ortağı Merkezi API 'Leri için CPV uygulamalarına yetki vermez. 

- CPV profilinizi görüntüleyin ve yönetin 

- CPV özelliklerine erişmesi gereken kullanıcılarınızı görüntüleyin ve yönetin. Genel yönetici, bir CPV 'nin sahip olduğu tek roldür.

## <a name="next-steps"></a>Sonraki adımlar

-[Iş Ortağı Merkezi hesabınıza ek kiracılar ekleyin](multi-tenant-account.md)