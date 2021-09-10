---
title: Azure CSP için yönetici ayrıcalıklarını yeniden devreye sokma
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: müşterilerin bir müşterinin Azure Bulut Çözümü Sağlayıcısı (CSP) aboneliklerinin yönetilmesine yardımcı olması için, ortağın yönetici ayrıcalıklarını yeniden devreye sokmasını nasıl sağlayacağınızı öğrenin.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 0a3af74158b36442118d41662744fc921277963c
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123959974"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Müşterinin Azure CSP abonelikleri için yeniden devreye sokma yönetici ayrıcalıkları  

**Uygun roller**: genel yönetici | Yönetim Aracısı

Bulut Çözümü Sağlayıcısı (CSP) iş ortağı olarak, müşterileriniz genellikle Azure kullanımını ve sistemlerini kendileri için yöneteceksiniz. Bunu yapmak için yönetici ayrıcalıklarına sahip olmanız gerekir. Müşteri ile satıcı ilişkiniz oluşturulduğunda bazı ayrıcalıklar verilir. Başkaları sizin tarafınızdan size verilir.

## <a name="admin-privileges-for-azure-in-csp"></a>CSP 'de Azure için yönetici ayrıcalıkları

CSP 'de Azure için iki yönetim ayrıcalıkları düzeyi vardır.

- **Kiracı düzeyinde yönetici ayrıcalıkları (yönetici ayrıcalıkları temsilcisi)**: CSP iş ortakları, müşterilerle CSP satıcısı ilişkisi oluştururken bu ayrıcalıkları alır. Yönetici ayrıcalıkları, CSP iş ortaklarının müşterilerinin kiracılarına erişmesini sağlar. Bu erişim, kullanıcıların kullanıcı ekleme/yönetme, parolaları sıfırlama ve kullanıcı lisanslarını yönetme gibi yönetim işlevleri yapmasına izin verir.
- **Abonelik düzeyi yönetici ayrıcalıkları**: CSP iş ortakları, müşterileri IÇIN Azure CSP abonelikleri oluştururken bu ayrıcalıkları alır. Bu ayrıcalıklara sahip olmak, CSP iş ortaklarının bu aboneliklerde Azure kaynaklarını sağlamasına ve yönetmesine olanak tanıyan tüm erişimleri olmasını sağlar.

## <a name="reinstate-csp-a-partners-admin-privileges"></a>Yeniden devreye alındı CSP bir ortağın yönetici ayrıcalıkları

Müşterinizden AdminAgents grubunu sağlarsanız, müşteriniz CSP rol atamasını yeniden oluşturabilir `object ID` . Yetkilendirilmiş yönetici ayrıcalıklarını yeniden kazanmak için aşağıdaki adımlar aracılığıyla müşterinizden çalışmanız gerekir.

1. Iş Ortağı Merkezi panosunda oturum açın.

2. Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin.

3. Çalıştığınız müşteriyi seçin ve **bir satıcı ilişkisi isteyin**. Bu eylem, kiracı yönetici haklarına sahip olan müşteriye bir bağlantı oluşturur.

4. Müşterinizin bağlantıyı seçmesini ve satıcı ilişki isteğini onaylaması gerekir.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Satıcı ilişkisi oluştur e-posta örneği.":::

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

Yukarıdaki adımlar işe yoksa veya bu işlemleri gerçekleştirmeye çalışırken hata alırsanız, müşterinizin yönetici haklarını yeniden devreye sokmak için aşağıdaki "catch-all" yordamını deneyin.

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a>Sorun giderme

Müşteri yukarıdaki 6. adımı tamamlayamadıysanız, müşterinin aşağıdaki komutu denemesini sağlayabilirsiniz:

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

`newRoleAssignment.log`Daha fazla analiz için elde edilen dosyayı Microsoft 'a sağlayın.

Sırasında "catch-all" yordamı başarısız olursa `Import-Module` , aşağıdaki adımları deneyin:
- Modül kullanımda olduğundan içeri aktarma başarısız olursa, tüm pencereleri kapatıp yeniden açarak PowerShell oturumunu yeniden başlatın.
- Sürümünü ile denetleyin `Az.Resources` `Get-Module Az.Resources -ListAvailable` .
- Sürüm 4.1.1, kullanılabilir liste içinde değilse, kullanmanız gerekir `Update-Module Az.Resources -Force` .
- Hata, `Az.Accounts` belirli bir sürüm olması gerektiğini belirtir, bu modülü de `Az.Resources` ile değiştirin `Az.Accounts` . Ardından PowerShell oturumunu yeniden başlatmanız gerekir.


## <a name="next-steps"></a>Sonraki adımlar

- [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)
