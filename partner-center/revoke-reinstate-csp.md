---
title: Azure CSP için yönetici ayrıcalıklarını yeniden Azure CSP
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: İş ortağının müşterinin Azure Bulut Çözümü Sağlayıcısı (CSP) aboneliklerini yönetmeye yardımcı olmak için müşterilerin bir iş ortağının yönetici ayrıcalıklarını yeniden Bulut Çözümü Sağlayıcısı nasıl yardımcı olduğunu öğrenin.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 53f9cf6533127231c152fbba0d7d7fbdadd6a897424f3d9383818fb45edf3465
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115682666"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Müşterinin abonelikleri için yönetici ayrıcalıklarını yeniden Azure CSP olun  

**Uygun roller:** Genel yönetici | Yönetici aracısı

Bir Bulut Çözümü Sağlayıcısı (CSP) iş ortağı olarak müşterileriniz genellikle Azure kullanımlarını ve sistemlerini onlar için yöneteceklerini bekler. Bunu yapmak için yönetici ayrıcalıklarına sahip olmanız gerekir. Müşteriyle kurumsal bayi ilişkiniz kurulu olduğunda bazı ayrıcalıklar verir. Başkalarına da müşteriniz tarafından izin ve verildi.

## <a name="admin-privileges-for-azure-in-csp"></a>CSP'de Azure için yönetici ayrıcalıkları

Kullanıcılar için iki yönetici ayrıcalıkları CSP'de Azure.

- **Kiracı düzeyinde yönetici ayrıcalıkları (Yönetici ayrıcalıkları temsilcisi)**: CSP iş ortakları, müşterilerle CSP kurumsal bayi ilişkisi kurulurken bu ayrıcalıkları alır. Temsilcili yönetici ayrıcalıkları, CSP iş ortaklarının müşterilerinin kiracılarına erişmesini sağlar. Bu erişim, kullanıcı ekleme/yönetme, parolaları sıfırlama ve kullanıcı lisanslarını yönetme gibi yönetim işlevlerini yapmalarına olanak sağlar.
- **Abonelik düzeyi yönetici ayrıcalıkları:** CSP iş ortakları, müşterileri için Azure CSP abonelikleri oluştururken bu ayrıcalıkları elde eder. Bu ayrıcalıklara sahip olmak, CSP iş ortaklarının bu aboneliklere tam erişim sağlamalarını ve Azure kaynaklarını yönetmelerini sağlar.

## <a name="reinstate-csp-a-partners-admin-privileges"></a>İş ortağının yönetici ayrıcalıklarını CSP'ye yeniden iade edin

Müşterinize AdminAgents grubunun sağlamasını sağlarsanız müşteriniz CSP rol `object ID` atamasını yeniden oluşturabilir. Temsilci yönetici ayrıcalıklarını yeniden kazanmak için aşağıdaki adımlarla müşteriyle çalışmanız gerekir.

1. Panoda İş Ortağı Merkezi açın.

2. Yeni İş Ortağı Merkezi Müşteriler'i **seçin.**

3. Üzerinde çalışmakta olduğunu müşteriyi seçin ve **bir kurumsal bayi ilişkisi talep edin.** Bu eylem kiracı yönetici haklarına sahip olan müşteriye bir bağlantı üretir.

4. Müşterinizin bağlantıyı seçmesi ve kurumsal bayi ilişkisi isteğini onaylaması gerekir.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Kurumsal bayi ilişkisi oluşturma e-posta örneği.":::

5. İş ortağı olarak AdminAgents grubunun Nesne Kimliğini almak için iş ortağı kiracısına bağlanmanız gerekir.
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. Daha sonra müşterinizin PowerShell veya Azure CLI kullanarak aşağıdaki adımları gerçekleştirebilirsiniz. Müşterinizin şunların olması gerekir:

- Sahip veya **kullanıcı** erişimi **yöneticisi rolü** 
- Abonelik düzeyinde rol ataması oluşturma izinleri

   a. Yalnızca PowerShell için müşterinin modülü güncelleştirmesi `Az.Resources` gerekir.
   ```powershell
   Update-Module Az.Resources
   ```

   b. Müşteri CSP aboneliğinin bulunduğu kiracıya bağlanır.
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   c. Müşteri aboneliğe bağlanır. Bu yalnızca *kullanıcının* kiracıda birden çok abonelik üzerinde rol atama izinlerine sahip olması için geçerlidir.

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   d. Müşteri daha sonra rol ataması oluşturur.
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

Abonelik kapsamında sahip izinleri vermek yerine kaynak grubu veya kaynak düzeyinde izin veebilirsiniz. 

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

Yukarıdaki adımlar işe çalışmıyorsa veya deneme sırasında hatalarla karşınıza çıkarsanız, müşteriniz için yönetici haklarını yeniden sağlamak için aşağıdaki "hepsini yakala" yordamını deneyin.

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a>Sorun giderme

Müşteri yukarıdaki 6. adımı tamamlayamazsa müşterinin aşağıdaki komutu denemesi gerekir:

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

Daha fazla analiz için `newRoleAssignment.log` elde edilen dosyayı Microsoft'a sağlama.

sırasında "hepsini yakala" yordamı başarısız olursa `Import-Module` aşağıdaki adımları deneyin:
- Modül kullanımda olduğundan içeri aktarma başarısız olursa, tüm pencereleri kapatıp yeniden açarak PowerShell oturumunu yeniden başlatın.
- ile sürümünü `Az.Resources` kontrol `Get-Module Az.Resources -ListAvailable` edin.
- Sürüm 4.1.1 kullanılabilir listede yoksa, kullansanız `Update-Module Az.Resources -Force` gerekir.
- Hata belirli bir sürüm `Az.Accounts` olması gerektiğini belirttiyse, yerine bu modülü de `Az.Resources` `Az.Accounts` güncelleştirin. Ardından PowerShell oturumunu yeniden başlatmanız gerekir.


## <a name="next-steps"></a>Sonraki adımlar

- [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)
