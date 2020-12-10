---
title: Azure CSP için yeniden devreye sokma yönetici ayrıcalıkları
ms.topic: how-to
ms.date: 07/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Müşterilerin bir müşterinin Azure CSP aboneliklerini yönetmeye yardımcı olması için, ortağın yönetici ayrıcalıklarını yeniden devreye sokmasını nasıl sağlayacağınızı öğrenin.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 13fdeb01ecd73dc1a63d174a4ad5cb8e1bdc813a
ms.sourcegitcommit: 455894365fa488368f7572ac72312e84a267ef5e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/10/2020
ms.locfileid: "97011511"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Müşterinin Azure CSP abonelikleri için yeniden devreye sokma yönetici ayrıcalıkları  

**Uygulanabilir roller**

- Genel yönetici
- Yönetim Aracısı

Bir CSP iş ortağı olarak, müşterileriniz genellikle Azure kullanımını ve sistemlerini kendileri için yöneteceksiniz. Bunun yapılması yönetici ayrıcalıklarına sahip olmanızı gerektirir. Müşteri ile ilgili satıcı ilişkiniz oluşturulduğunda, bazı ayrıcalıklara izin verilir. Başkaları sizin tarafınızdan size verilir.

## <a name="admin-privileges-for-azure-in-csp"></a>CSP 'de Azure için yönetici ayrıcalıkları

CSP 'de Azure için iki yönetim ayrıcalıkları düzeyi vardır.

**Kiracı düzeyinde yönetici ayrıcalıkları** (**yönetici ayrıcalıkları temsilcisi**)-CSP Iş ortakları, müşterilerle CSP satıcısı ilişkisi oluştururken bu ayrıcalıkları alır. Bu, CSP iş ortaklarının müşterilerinin kiracılarına erişmesini sağlar ve bu sayede kullanıcıları ekleme/yönetme, parolaları sıfırlama ve kullanıcı lisanslarını yönetme gibi yönetim işlevleri gerçekleştirebilir.

**Abonelik düzeyi yönetici ayrıcalıkları** -CSP iş ortakları, müşterileri IÇIN Azure CSP abonelikleri oluştururken bu ayrıcalıkları alırlar. Bu ayrıcalıklara sahip olmak, CSP iş ortaklarının bu aboneliklerde Azure kaynaklarını sağlamasına ve yönetmesine olanak tanıyan tüm erişimleri olmasını sağlar.

## <a name="reinstate-csp-partners-admin-privileges"></a>Yeniden devreye sokma CSP iş ortakları yönetici ayrıcalıkları

Yetkilendirilmiş yönetici ayrıcalıklarını yeniden kazanmak için müşterinizden çalışmanız gerekir.

1. Iş Ortağı Merkezi panosunda oturum açın ve Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin.

2. Çalıştığınız müşteriyi seçin ve **bir satıcı ilişkisi isteyin.** Bu, kiracı yönetici haklarına sahip olan müşteriye bir bağlantı oluşturur.

3. Bu kullanıcının bağlantıyı seçmesini ve satıcı ilişki isteğini onaylaması gerekir.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Satıcı ilişkisi":::

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a>Yönetici aracıları grubunu Azure CSP aboneliğine sahip olarak ekleme

Müşterinizin, yönetici Aracısı grubunuzu bir Azure CSP Aboneliğinin sahibi, bir kaynak grubu veya kaynak olarak eklemesi gerekir. 

1. PowerShell konsolunu veya PowerShell Tümleşik komut dosyası ortamı 'nı (ıSE) kullanın. AzureAD modüllerinin yüklü olduğundan emin olun.

2. Azure AD Kiracınıza bağlanın.

   ```powershell
   Connect-AzureAD
   ```

3. Yönetici aracıları gruplarının ObjectID 'sini alın.

   ```powershell
   Get-AzureADGroup
   ```
   Aşağıdaki adımlar, Azure CSP aboneliğine sahip erişimi olan müşterinizin şirketindeki Kullanıcı tarafından gerçekleştirilir.

4. Azure CSP aboneliğine sahip erişimi olan Kullanıcı, kimlik bilgilerini kullanarak Azure 'da oturum açar.

   ```powershell
   Connect-AzureRmAccount
   ```

5. Daha sonra, kapsam parametresinde uygun bir kaynak URI 'Si uygulayarak, Yönetim Aracısı grubunuzu CSP Azure aboneliğine, kaynak grubuna veya kaynağa sahip olarak ekleyebilir. 

    ```powershell
    # Grant owner role at subscription level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"

    # Grant owner role at resource group level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>/resourceGroups/<Resource group name>"

    # Grant owner role at resource level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "<Resource Uri>"
    ```

## <a name="next-steps"></a>Sonraki adımlar

[Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)
