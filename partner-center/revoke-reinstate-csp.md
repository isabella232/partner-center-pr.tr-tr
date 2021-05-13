---
title: Azure CSP için yönetici ayrıcalıklarını yeniden Azure CSP
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: İş ortağının müşterinin iş ortağı aboneliklerini yönetmeye yardımcı olmak için müşterilerin iş ortağının yönetici ayrıcalıklarını yeniden Azure CSP öğrenin.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: ad29283001ec542944da4f0cac835c6a5d339251
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855429"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Müşterinin abonelikleri için yönetici ayrıcalıklarını yeniden Azure CSP olun  

**Uygun roller:** Genel yönetici | Yönetici aracısı

CSP iş ortağı olarak müşterileriniz genellikle Azure kullanımlarını ve sistemlerini onlar için yöneteceklerini bekler. Bunu yapmak için yönetici ayrıcalıklarına sahip olmanız gerekir. Müşteriyle kurumsal bayi ilişkiniz kurulu olduğunda bazı ayrıcalıklar verir. Başkalarına da müşteriniz tarafından izin ve verildi.

## <a name="admin-privileges-for-azure-in-csp"></a>CSP'de Azure için yönetici ayrıcalıkları

Kullanıcılar için iki yönetici ayrıcalıkları CSP'de Azure.

**Kiracı düzeyi yönetici ayrıcalıkları** (**Yönetici ayrıcalıkları temsilcisi**) - CSP iş ortakları, müşterilerle CSP kurumsal bayi ilişkisi kurulurken bu ayrıcalıkları alır. Temsilcili yönetici ayrıcalıkları, CSP iş ortaklarının müşterilerinin kiracılarına erişmesini sağlar ve bu sayede kullanıcı ekleme/yönetme, parolaları sıfırlama ve kullanıcı lisanslarını yönetme gibi yönetim işlevlerini gerçekleştirebilir.

**Abonelik düzeyi yönetici ayrıcalıkları** - CSP iş ortakları, müşterileri için Azure CSP abonelikleri oluştururken bu ayrıcalıkları elde eder. Bu ayrıcalıklara sahip olmak, CSP iş ortaklarının bu aboneliklere tam erişim sağlamalarını ve Azure kaynaklarını yönetmelerini sağlar.

## <a name="reinstate-csp-partners-admin-privileges"></a>CSP iş ortaklarının yönetici ayrıcalıklarını yeniden açıklama

Müşterinize AdminAgents grubunun nesne kimliğini sağlamak sürece müşteriniz CSP rol atamasını yeniden oluşturabilir. Temsilci yönetici ayrıcalıklarını yeniden kazanmak için müşteriyle çalışmanız gerekir.

1. İş Ortağı Merkezi panosunda oturum açın ve İş Ortağı Merkezi menüsünde Müşteriler'i **seçin.**

2. Birlikte çalışmakta olduğunu müşteriyi seçin ve **bir kurumsal bayi ilişkisi talep edin.** Bu eylem kiracı yönetici haklarına sahip olan müşteriye bir bağlantı üretir.

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
