---
title: Denetim Masası satıcısı olarak kaydetme
description: CSP iş ortağı sistemlerini Iş Ortağı Merkezi API 'Leriyle daha iyi tümleştirebilmeniz için Iş Ortağı Merkezi 'nde bir denetim masası satıcısı (CPV) olarak nasıl kaydolacağınızı öğrenin.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/20/2020
ms.openlocfilehash: 1bfcb4de27233283b6188903b3e1f6bbdf67698c
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/14/2020
ms.locfileid: "92531943"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a>CSP iş ortağı sistemlerini Iş Ortağı Merkezi API 'Leriyle tümleştirmenize yardımcı olmak için Denetim Masası satıcısı olarak kaydetme

**Uygulama hedefi**

- İş Ortağı Merkezi

**Uygun roller**

- Genel yönetici

Bir denetim masası satıcısı (CPV), bulut çözümü sağlayıcısı (CSP) iş ortakları tarafından sistemlerini Iş Ortağı Merkezi API 'Leri ile tümleştirmelerini sağlamak üzere uygulamalar geliştiren bağımsız bir yazılım satıcıdır. Bir denetim masası satıcısı, Iş Ortağı Merkezi panosuna veya Iş Ortağı Merkezi API 'Lerine doğrudan erişimli bir CSP Iş ortağı değildir.

Microsoft iş ortaklarıyla çalışmak isteyen geçerli bir denetim masası satıcısı (CPV) veya yeni bir CPV olun, Microsoft artık uygulamalarınızı kaydetmek ve bulut çözümü sağlayıcısı iş ortaklarını desteklemek için Iş Ortağı Merkezi 'ne kaydolmanızı gerektirir. Bir hesap oluşturmak için, bir CPV iş ortağı mevcut bir CSP iş ortağı kiracısı veya mevcut bir CPV kiracısı kullanabilir ya da ekleme sürecinin bir parçası olarak yeni bir kiracı oluşturabilir. CPV iş ortağı mevcut CSP kiracısını kullanmayı seçerse, ayrı bir çok kiracılı uygulamalar oluşturmalı ve bunları CPV etkinlikleri için Iş Ortağı Merkezi 'ne kaydetmeleri gerekir. Bir uygulama hem CSP hem de CPV uygulaması olarak kaydedilemez. Iş Ortağı Merkezi 'ne kaydolduktan ve uygulamalarınızı kaydettirdikten sonra, Iş Ortağı Merkezi API 'Lerine erişebilirsiniz.  Microsoft, korumalı alan bilgileriniz ile bir Iş Ortağı Merkezi bildirimi aracılığıyla sizinle iletişim kuracaktır. Zaten bir korumalı alan hesabınız varsa, bu hesabı kullanmaya devam edin. Yeni bir korumalı alana ihtiyacınız olmayacaktır.

[Microsoft Denetim Masası satıcı sözleşmesini](https://go.microsoft.com/fwlink/?linkid=2055198) gözden geçirin


## <a name="working-in-partner-center"></a>Iş Ortağı Merkezi 'nde çalışma
Iş Ortağı Merkezi CPV deneyimine kaydolduktan ve CPV sözleşmesini kabul etmeniz durumunda şunları yapabilirsiniz:

- Çok kiracılı uygulamaları yönetme (Iş Ortağı Merkezi 'nde uygulamaları Azure portal, kaydetmek ve kayıt silmek için uygulama ekleme).

    >[!Note] 
    >Iş Ortağı Merkezi API 'Lerine yetki almak için, CPVs 'in uygulamalarını Iş Ortağı Merkezi 'ne kaydetmesi gerekir. Uygulamaları tek başına Azure portal eklemek, Iş Ortağı Merkezi API 'Leri için CPV uygulamalarına yetki vermez. 

- CPV profilinizi görüntüleyin ve yönetin 

- CPV özelliklerine erişmesi gereken kullanıcılarınızı görüntüleyin ve yönetin. Genel yönetici, bir CPV 'nin sahip olduğu tek roldür.


