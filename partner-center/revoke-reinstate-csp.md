---
title: Azure CSP için yönetici ayrıcalıklarını yeniden Azure CSP
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: İş ortağının müşterinin iş ortağı aboneliklerini yönetmeye yardımcı olmak için müşterilerin iş ortağının yönetici ayrıcalıklarını yeniden Azure CSP öğrenin.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: ca4c8323562e6c6f1d762465cad86e7ae113eb19
ms.sourcegitcommit: beba696954b62ab5396a893d050d0c2c211aeafc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/28/2021
ms.locfileid: "110601435"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Müşterinin abonelikleri için yönetici ayrıcalıklarını yeniden Azure CSP olun  

**Uygun roller:** Genel yönetici | Yönetici aracısı

CSP iş ortağı olarak müşterileriniz genellikle Azure kullanımlarını ve sistemlerini onlar için yöneteceklerini bekler. Bunu yapmak için yönetici ayrıcalıklarına sahip olmanız gerekir. Müşteriyle kurumsal bayi ilişkiniz kurulu olduğunda bazı ayrıcalıklar verir. Başkalarına da müşteriniz tarafından verildi.

## <a name="admin-privileges-for-azure-in-csp"></a>CSP'de Azure için yönetici ayrıcalıkları

Kullanıcılar için iki yönetici ayrıcalıkları CSP'de Azure.

- **Kiracı düzeyinde yönetici ayrıcalıkları (Yönetici ayrıcalıkları temsilcisi)**: CSP iş ortakları, müşterilerle CSP kurumsal bayi ilişkisi kurulurken bu ayrıcalıkları alır. Temsilcili yönetici ayrıcalıkları, CSP iş ortaklarının müşterilerinin kiracılarına erişmesini sağlar. Bu erişim, kullanıcı ekleme/yönetme, parolaları sıfırlama ve kullanıcı lisanslarını yönetme gibi yönetim işlevlerini yapmalarına olanak sağlar.
- **Abonelik düzeyi yönetici ayrıcalıkları:** CSP iş ortakları, müşterileri için Azure CSP abonelikleri oluştururken bu ayrıcalıkları elde eder. Bu ayrıcalıklara sahip olmak, CSP iş ortaklarının bu aboneliklere tam erişim sağlamalarını ve Azure kaynaklarını yönetmelerini sağlar.

## <a name="reinstate-csp-a-partners-admin-privileges"></a>CsP'yi iş ortağının yönetici ayrıcalıklarını yeniden açıklama

Müşterinize AdminAgents grubunun sağlamasını sağlarsanız müşteriniz `object ID` CSP rol atamasını yeniden oluşturabilir. Temsilci yönetici ayrıcalıklarını yeniden kazanmak için aşağıdaki adımlarla müşteriyle çalışmanız gerekir.

1. Panoda İş Ortağı Merkezi açın.

2. Yeni İş Ortağı Merkezi Müşteriler'i **seçin.**

3. Çalıştığınız müşteriyi seçin ve **bir satıcı ilişkisi isteyin**. Bu eylem, kiracı yönetici haklarına sahip olan müşteriye bir bağlantı oluşturur.

4. Müşterinizin bağlantıyı seçmesini ve satıcı ilişki isteğini onaylaması gerekir.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Satıcı ilişkisi oluştur e-posta örneği":::

5. İş ortağının, AdminAgents grubunun nesne KIMLIĞINI almak için iş ortağı kiracısına bağlanması gerekir.
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. Müşterinizin, PowerShell veya Azure CLı kullanarak aşağıdaki adımları yapması gerekir. Müşterinizin şunları uygulamanız gerekir:

- **Sahip** veya **Kullanıcı erişimi Yöneticisi** rolü 
- Abonelik düzeyinde rol atamaları oluşturma izinleri

   a. Yalnızca PowerShell için, müşterinin modülü güncelleştirmesi gerekir `Az.Resources` .
   ```powershell
   Update-Module Az.Resources
   ```

   b. Müşteri, CSP aboneliğinin bulunduğu kiracıya bağlanır.
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   c. Müşteri, aboneliğe bağlanır. Bu, *yalnızca* kullanıcının Kiracıdaki birden çok abonelik üzerinde rol atama izinlerine sahip olması durumunda geçerlidir.

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   d. Müşteri daha sonra rol atamasını oluşturur.
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

Abonelik kapsamında sahip izinleri vermek yerine, kaynak grubu veya kaynak düzeyinde izin verebilirsiniz. 

- Kaynak grubu düzeyinde

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- Kaynak düzeyinde

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

## <a name="next-steps"></a>Sonraki adımlar

- [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)
