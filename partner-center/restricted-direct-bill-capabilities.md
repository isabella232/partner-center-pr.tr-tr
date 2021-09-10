---
title: Kısıtlanan doğrudan fatura özellikleri
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Doğrudan fatura Bulut Çözümü Sağlayıcısı (CSP) gereksinimleri hakkında bilgi ve yeteneklerin kısıtlanmış olmasından kaçınmak için ne yapmaları gerekir? Özelliklerinizin kısıtlanmış olup olduğunu bulun.
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: edb67f6ae3054bf5214611ab3ac5ef4ed6713aef
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960734"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>Kısıtlı doğrudan fatura özellikleri ve CSP doğrudan fatura iş ortakları için gereken gereksinimler

**Uygun roller:** Genel yönetici

## <a name="overview"></a>Genel Bakış

Doğrudan fatura iş ortaklarının yeni gereksinimleri [karşılaması](direct-partner-new-requirements.md) ve Bulut Çözümü Sağlayıcısı (CSP) doğrudan fatura iş ortağı programında kalması gerekir. Aksi takdirde, doğrudan fatura özelliklerine erişimleri sonunda kısıtlanır ve müşterileri için yeni satın almalar yapma gibi belirli görevleri daha uzun süre gerçekleştirebilir.

> [!Note]
> CSP doğrudan fatura iş ortağı programı için yeni gereksinimleri karşılamayan doğrudan fatura iş ortakları, doğrudan fatura özellikleri kısıtlansa Microsoft tarafından bilgi sahibi olur. Bu, doğrudan fatura iş ortağından dolaylı kurumsal bayilere geçişi kabul edip edmse de tüm doğrudan fatura [iş ortakları için](transition-direct-to-indirect.md) geçerlidir.  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>Doğrudan fatura özelliklerinizin kısıtlanmış olup olduğunu nasıl söyleyebilirim?

Doğrudan fatura iş ortağı kiracıdan doğrudan fatura özelliklerine erişimin kısıtlanmış olup olmadığını onaylamak için aşağıdaki adımları izleyin.

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard) oturum açın.

2. Hesap ayarları **Yasal**  >  **Profil'e gidin.**

3. Program **bilgileri altında,** durumunu **Microsoft Bulut Çözümü Sağlayıcısı bakın.**

4. Program durumu kısıtlı **değerine sahipse,** doğrudan fatura iş ortağı kiracısının doğrudan fatura özelliklerine erişimi kısıtlanmış demektir.

## <a name="affected-direct-bill-capabilities"></a>Etkilenen doğrudan fatura özellikleri

Doğrudan fatura özellikleriniz kısıtlanmışsa, artık bu hizmette müşterileriniz için yeni satın İş Ortağı Merkezi. Bu kısıtlama şunları içerir:

- Azure abonelikleri

- Lisans tabanlı abonelikler

- Mevcut lisans tabanlı aboneliklere yeni eklentiler ekleyin.

- Yazılım ve rezervasyon ürünleri (örneğin, yazılım abonelikleri, kalıcı yazılım ve Azure Ayrılmış Sanal Makine örnekleri) için tek kullanımlık satın alma işlemleri yapma.

CsP programı [kapsamındaki Azure iş ortağı](shared-services.md) paylaşılan hizmetleri teklifini kendi kullanımınız için yeni Azure abonelikleri satın almak için de kullanamazsınız.

Mevcut doğrudan fatura abonelikleri etkilenmez. Bunlar geçerli kalır ve otomatik olarak yeniler. İptal edilene kadar doğrudan Microsoft tarafından faturalandır olmaya devam edersiniz. Mevcut abonelikleri yönetmek için aşağıdaki yöntemleri kullanabilirsiniz:

- Mevcut abonelikleri askıya alma

- Mevcut lisans tabanlı aboneliklerin lisans sayısını ayarlama

- Bir aboneliğe yapılan mevcut eklentilerin lisans sayısını ayarlayın. 

    >[!Note]
    >Yeni satın alma olarak kabul edilen mevcut aboneliklere yeni eklentiler ek olamazsınız.

- Yeni Azure kaynaklarını dağıtın ve mevcut Azure kaynaklarını mevcut Azure abonelikleri altında yönetin. Bu, Azure Market ve Visual Studio içerir.

Yeni satın almalara ek olarak, aşağıdaki doğrudan fatura özelliklerine de İş Ortağı Merkezi:

- Yeni müşteri kiracıları oluşturamazsiniz. Müşteriler **sayfasındaki** Müşteriler **sayfasında** müşteri İş Ortağı Merkezi seçeneği kullanılamaz.

- Doğrudan kurumsal bayi ilişkisi isteğine davet oluşturamazsiniz. Aşağıdakiler **sayfasındaki** Müşteriler **sayfasındaki** Satıcı İş Ortağı Merkezi isteğinde bulun seçeneği kullanılamaz.

    >[!NOTE]
    >Doğrudan fatura iş ortağından dolaylı kurumsal bayiye geçişin bir parçası olarak, doğrudan fatura iş ortağı kiracınızı dolaylı kurumsal bayi olarak zaten kaydettiynize, bunun yerine dolaylı kurumsal bayi ilişkisi isteğine davet eden müşteriye davette bulunabilirsiniz.

- Yeni korumalı alan kiracısı oluşturamazsiniz. Her doğrudan fatura iş ortağı kiracısı, doğrudan fatura API'si tümleştirmesi için bir korumalı alan kiracısı oluşturabilir. Daha önce oluşturmadıysanız, doğrudan fatura iş ortağı özelliğiniz kısıtlandıktan sonra bunu yapma iznine sahip olmaznız.  

## <a name="next-steps"></a>Sonraki adımlar

- [Dolaylı kurumsal bayi olma hakkında ek bilgiler](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [CSP doğrudan iş ortağı yeni gereksinimleri](direct-partner-new-requirements.md)
