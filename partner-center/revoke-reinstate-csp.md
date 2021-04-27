---
title: Azure CSP için yeniden devreye sokma yönetici ayrıcalıkları
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Müşterilerin bir müşterinin Azure CSP aboneliklerini yönetmeye yardımcı olması için, ortağın yönetici ayrıcalıklarını yeniden devreye sokmasını nasıl sağlayacağınızı öğrenin.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 26768bdf33c03145a893fa445eab6ebf92ca9b1c
ms.sourcegitcommit: efd711b0e65c55f24ce5b9636abd7b5a8cc719fe
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/27/2021
ms.locfileid: "108018196"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Müşterinin Azure CSP abonelikleri için yeniden devreye sokma yönetici ayrıcalıkları  

**Uygun roller**

- Genel yönetici
- Yönetim Aracısı

Bir CSP iş ortağı olarak, müşterileriniz genellikle Azure kullanımını ve sistemlerini kendileri için yöneteceksiniz. Bunun yapılması yönetici ayrıcalıklarına sahip olmanızı gerektirir. Müşteri ile satıcı ilişkiniz oluşturulduğunda bazı ayrıcalıklar verilir. Başkaları sizin tarafınızdan size verilir.

## <a name="admin-privileges-for-azure-in-csp"></a>CSP 'de Azure için yönetici ayrıcalıkları

CSP 'de Azure için iki yönetim ayrıcalıkları düzeyi vardır.

**Kiracı düzeyinde yönetici ayrıcalıkları** (**yönetici ayrıcalıkları temsilcisi**)-CSP Iş ortakları, müşterilerle CSP satıcısı ilişkisi oluştururken bu ayrıcalıkları alır. Yönetici ayrıcalıkları, CSP iş ortaklarının müşterilerinin kiracılarına erişmesini sağlar ve bu sayede Kullanıcı ekleme/yönetme, parolaları sıfırlama ve kullanıcı lisanslarını yönetme gibi yönetim işlevleri gerçekleştirebilir.

**Abonelik düzeyi yönetici ayrıcalıkları** -CSP iş ortakları, müşterileri IÇIN Azure CSP abonelikleri oluştururken bu ayrıcalıkları alırlar. Bu ayrıcalıklara sahip olmak, CSP iş ortaklarının bu aboneliklerde Azure kaynaklarını sağlamasına ve yönetmesine olanak tanıyan tüm erişimleri olmasını sağlar.

## <a name="reinstate-csp-partners-admin-privileges"></a>Yeniden devreye sokma CSP iş ortakları yönetici ayrıcalıkları

Müşteriniz, AdminAgents grubunun nesne KIMLIĞINI sağladığınız sürece, CSP rol atamasını yeniden oluşturabilir. Yetkilendirilmiş yönetici ayrıcalıklarını yeniden kazanmak için müşterinizden çalışmanız gerekir.

1. Iş Ortağı Merkezi panosunda oturum açın ve Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin.

2. Çalıştığınız müşteriyi seçin ve **bir satıcı ilişkisi isteyin.** Bu eylem, kiracı yönetici haklarına sahip olan müşteriye bir bağlantı oluşturur.

3. Bu müşterinin bağlantıyı seçmesini ve satıcı ilişki isteğini onaylaması gerekir.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Satıcı ilişkisi oluştur e-posta örneği":::

4. İş ortağının, AdminAgents grubunun nesne KIMLIĞINI almak için iş ortağı kiracısına bağlanması gerekir.

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. **Sahibi veya Kullanıcı erişimi Yöneticisi** rolüne sahip olan ve abonelik düzeyinde rol ataması oluşturma izni olan müşteriniz şunları yapar:


    1. CSP aboneliğinin bulunduğu kiracıya bağlanır.
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. Aboneliğe bağlanır (yalnızca kullanıcının Kiracıdaki birden çok abonelik üzerinde rol ataması izinleri varsa geçerlidir).
   
         PS C:\WINDOWS\system32> Set-AzContext-SubscriptionID "CSP abonelik KIMLIĞI" '


    3. Rol atamasını oluşturur
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


Abonelik kapsamı yerine kaynak grubu düzeyinde veya kaynak düzeyinde sahip rolü izni vermek istiyorsanız aşağıdaki komutlar kullanılabilir:


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a>Sonraki adımlar

- [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)
