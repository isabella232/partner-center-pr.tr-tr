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
ms.openlocfilehash: 38fe5d03784d0fcf0796545d31e8272f316d2878
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/06/2021
ms.locfileid: "99623992"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>Kısıtlanmış doğrudan fatura özellikleri ve CSP doğrudan fatura ortakları için gereken gereksinimler  

## <a name="overview"></a>Genel Bakış

Doğrudan fatura ortakları, CSP doğrudan fatura ortağı programında kalacak yeni [gereksinimleri](direct-partner-new-requirements.md) karşılamalıdır. Aksi takdirde, doğrudan fatura özelliklerine erişimleri bu süre sonunda kısıtlanmıştır ve müşterileri için yeni satın alma işlemleri gibi belirli görevleri daha fazla gerçekleştirebilir.

> [!Note]
> CSP doğrudan fatura iş ortağı programı için yeni gereksinimleri karşılamayan doğrudan fatura ortakları, doğrudan fatura özellikleri sınırlandırılacağı zaman Microsoft tarafından bilgilendirilir. Bu, [doğrudan fatura ortağından dolaylı satıcılara geçiş](transition-direct-to-indirect.md) yapılıp yapılmayacağını kabul etmeksizin tüm doğrudan fatura ortakları için geçerlidir.  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>Doğrudan fatura olanaklarınızın kısıtlanmasını nasıl söylüyorsunuz

Doğrudan fatura ortağı kiracısından doğrudan fatura özelliklerine erişimin kısıtlanıp kısıtlanmadığını doğrulamak için aşağıdaki adımları izleyin.

1. [Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard)oturum açın.

2. **Hesap ayarları**  ->  **yasal profili**' ne gidin.

3. **Program bilgileri** altında **Microsoft bulut çözüm sağlayıcısı durumunu** arayın.

4. Program durumunun **kısıtlı** değeri varsa, doğrudan fatura iş ortağı kiracının doğrudan fatura özelliklerine erişiminin kısıtlandığı anlamına gelir.

## <a name="affected-direct-bill-capabilities"></a>Etkilenen doğrudan fatura özellikleri

Doğrudan fatura olanaklarınız kısıtlanmışsa, Iş Ortağı Merkezi 'nde müşterileriniz için artık yeni satın alma işlemleri yapamamaktadır. Bu kısıtlama şunları içerir:

- Azure abonelikleri

- Lisans tabanlı abonelikler

- Mevcut lisans tabanlı aboneliklere yeni eklentiler ekleyin.

- Yazılım ve rezervasyon ürünlerini tek seferlik satın alma (örneğin, yazılım abonelikleri, kalıcı yazılım ve Azure ayrılmış sanal makine örnekleri) yapın.

Ayrıca, CSP programı kapsamındaki [Azure iş ortağı paylaşılan hizmetleri teklifini](shared-services.md) kullanarak kendi kullanım Için yeni Azure abonelikleri satın alabilirsiniz.

Mevcut doğrudan fatura abonelikleri etkilenmez. Bunlar geçerli kalır ve otomatik olarak yenilenir. İptal edilene kadar doğrudan Microsoft tarafından faturalandırılmaya devam edersiniz. Mevcut abonelikleri şu yollarla yönetmeye devam edebilirsiniz:

- Mevcut abonelikleri askıya al

- Lisans tabanlı mevcut aboneliklerin lisans sayısını ayarla

- Mevcut eklentilerin lisans sayısını bir aboneliğe ayarlayın. 
 
    >[!Note] 
    >Yeni satın alma işlemi kabul edildiği için mevcut aboneliklere yeni eklentiler ekleyemezsiniz.

- Yeni Azure kaynaklarını dağıtın ve mevcut Azure aboneliklerinden mevcut Azure kaynaklarını yönetin. Bu, Azure Marketi ve Visual Studio abonelikleri aracılığıyla kullanılabilen kaynakları içerir.

Yeni satın alımlara ek olarak, Iş Ortağı Merkezi 'nde aşağıdaki doğrudan fatura özelliklerine erişemezsiniz:

- Yeni müşteri kiracılarını oluşturamazsınız. Iş Ortağı Merkezi 'ndeki **müşteriler** sayfasında **Müşteri Oluştur** seçeneği kullanılamaz.

- Müşterinin doğrudan satıcı ilişkisi talep etmek için davet oluşturamazsınız. Iş Ortağı Merkezi 'ndeki **müşteriler** sayfasında **bir satıcı ilişkisi iste** seçeneği kullanılamayacak.

    >[!NOTE]
    >Doğrudan fatura ortağından dolaylı satıcıya geçiş bir parçası olarak doğrudan fatura ortağı kiracınızı dolaylı satıcı olarak kaydettiyseniz, bunun yerine dolaylı satıcı ilişkisi isteyen müşteri için davet oluşturabilirsiniz.

- Yeni korumalı alan kiracısı oluşturamazsınız. Her bir doğrudan fatura ortağı kiracısı, doğrudan Bill API tümleştirmesi amacıyla bir korumalı alan kiracısı oluşturabilir. Daha önce bir tane oluşturmadıysanız, doğrudan fatura ortağı özelliği sınırlandırdıktan sonra bunu yapma izniniz yoktur.  

## <a name="next-steps"></a>Sonraki adımlar

- [Dolaylı satıcı olma hakkında ek bilgiler](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [CSP doğrudan iş ortağı yeni gereksinimler](direct-partner-new-requirements.md)
