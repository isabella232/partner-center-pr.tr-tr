---
title: Kısıtlanmış doğrudan fatura özellikleri
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP doğrudan fatura ortağı gereksinimleri hakkında bilgi edinin ve yeteneklerin kısıtlanmasını önlemek için ne yapmanız gerektiğini öğrenin. Olanaklarınızın kısıtlanıp kısıtlanmayacağını öğrenin.
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b3b1f3e1593f7e35bd3b9ed6c56ea28683bff95a
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855497"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>Kısıtlanmış doğrudan fatura özellikleri ve CSP doğrudan fatura ortakları için gereken gereksinimler

**Uygun roller**: genel yönetici

## <a name="overview"></a>Genel Bakış

Doğrudan fatura ortakları, CSP doğrudan fatura ortağı programında kalacak yeni [gereksinimleri](direct-partner-new-requirements.md) karşılamalıdır. Aksi takdirde, doğrudan fatura özelliklerine erişimleri bu süre sonunda kısıtlanmıştır ve müşterileri için yeni satın alma işlemleri gibi belirli görevleri daha fazla gerçekleştirebilir.

> [!Note]
> CSP doğrudan fatura iş ortağı programı için yeni gereksinimleri karşılamayan doğrudan fatura ortakları, doğrudan fatura özellikleri sınırlandırılacağı zaman Microsoft tarafından bilgilendirilir. Bu, [doğrudan fatura ortağından dolaylı satıcılara geçiş](transition-direct-to-indirect.md) yapılıp yapılmayacağını kabul etmeksizin tüm doğrudan fatura ortakları için geçerlidir.  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>Doğrudan fatura olanaklarınızın kısıtlanmasını nasıl söylüyorsunuz

Doğrudan fatura ortağı kiracısından doğrudan fatura özelliklerine erişimin kısıtlanıp kısıtlanmadığını doğrulamak için aşağıdaki adımları izleyin.

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard) oturum açın.

2. **Hesap ayarları**  ->  **yasal profili**' ne gidin.

3. **Program bilgileri** altında **Microsoft bulut çözüm sağlayıcısı durumunu** arayın.

4. Program durumunun **kısıtlı** değeri varsa, doğrudan fatura iş ortağı kiracının doğrudan fatura özelliklerine erişiminin kısıtlandığı anlamına gelir.

## <a name="affected-direct-bill-capabilities"></a>Etkilenen doğrudan fatura özellikleri

Doğrudan fatura olanaklarınız kısıtlanmışsa, Iş Ortağı Merkezi 'nde müşterileriniz için artık yeni satın alma işlemleri yapamamaktadır. Bu kısıtlama şunları içerir:

- Azure abonelikleri

- Lisans tabanlı abonelikler

- Mevcut lisans tabanlı aboneliklere yeni eklentiler ekleyin.

- Yazılım ve rezervasyon ürünlerini tek seferlik satın alma (örneğin, yazılım abonelikleri, kalıcı yazılım ve Azure ayrılmış sanal makine örnekleri) yapın.

Kendi kullanımınız için yeni [Azure abonelikleri satın almak için](shared-services.md) CSP programı kapsamındaki Azure iş ortağı paylaşılan hizmetleri teklifini de kullanamazsınız.

Mevcut doğrudan fatura abonelikleri etkilenmez. Bunlar geçerli kalır ve otomatik olarak yeniler. İptal edilene kadar doğrudan Microsoft tarafından faturalandır olmaya devam edersiniz. Mevcut abonelikleri yönetmek için aşağıdaki yöntemleri kullanabilirsiniz:

- Mevcut abonelikleri askıya alma

- Mevcut lisans tabanlı aboneliklerin lisans sayısını ayarlama

- Bir aboneliğe yapılan mevcut eklentilerin lisans sayısını ayarlayın. 

    >[!Note]
    >Yeni satın alma olarak kabul edilen mevcut aboneliklere yeni eklentiler ek olamazsınız.

- Yeni Azure kaynaklarını dağıtın ve mevcut Azure kaynaklarını mevcut Azure abonelikleri altında yönetin. Bu, Azure Market ve Visual Studio içerir.

Yeni satın almalara ek olarak, aşağıdaki doğrudan fatura özelliklerine de İş Ortağı Merkezi:

- Yeni müşteri kiracıları oluşturamazsiniz. Müşteriler **sayfasındaki** Müşteriler **sayfasında** müşteri İş Ortağı Merkezi seçeneği kullanılamaz.

- Doğrudan kurumsal bayi ilişkisi isteğine davet oluşturamazsiniz. Kurumsal **bayi ilişkisi isteğinde** **bulun sayfasındaki** Müşteriler İş Ortağı Merkezi seçeneği kullanılamaz.

    >[!NOTE]
    >Doğrudan fatura iş ortağından dolaylı kurumsal bayiye geçişin bir parçası olarak, doğrudan fatura iş ortağı kiracınızı dolaylı kurumsal bayi olarak zaten kaydettiynize, bunun yerine dolaylı kurumsal bayi ilişkisi isteğine davet eden müşteriye davette bulunabilirsiniz.

- Yeni korumalı alan kiracısı oluşturamazsiniz. Her doğrudan fatura iş ortağı kiracısı, doğrudan fatura API'si tümleştirmesi için bir korumalı alan kiracısı oluşturabilir. Daha önce oluşturmadıysanız, doğrudan fatura iş ortağı özelliğiniz kısıtlandıktan sonra bunu yapma iznine sahip olmaznız.  

## <a name="next-steps"></a>Sonraki adımlar

- [Dolaylı satıcı olma hakkında ek bilgiler](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [CSP doğrudan iş ortağı yeni gereksinimler](direct-partner-new-requirements.md)
