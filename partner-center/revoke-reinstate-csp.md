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
ms.openlocfilehash: ea64a6030acbc41aec085b3a0a7927d8ed28cc88
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129070175"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Müşterinin Azure CSP abonelikleri için yeniden devreye sokma yönetici ayrıcalıkları  

**Uygun roller**: genel yönetici | Yönetim Aracısı

Bulut Çözümü Sağlayıcısı (CSP) program ortağı olarak, müşterileriniz genellikle Azure kullanımını ve sistemlerini yönetmenize olanak sağlar. Bunlara yardımcı olmak için yönetici ayrıcalıklarına sahip olmanız gerekir. Yönetici ayrıcalıklarınız yoksa, yeniden devreye sokmak için müşterinizden çalışabilirsiniz.

## <a name="admin-privileges-for-azure-in-the-csp-program"></a>CSP programında Azure için yönetici ayrıcalıkları

Müşteriyle bir satıcı ilişkisi oluşturduğunuzda, bazı yönetici ayrıcalıkları otomatik olarak verilir. Müşteri tarafından sizin için diğer kullanıcılar verilmelidir. CSP 'de Azure için iki yönetim ayrıcalıkları düzeyi vardır.

- **Kiracı düzeyinde yönetici ayrıcalıkları (yani, yönetici ayrıcalıkları temsilcisi)** , müşterilerinizin kiracılarına erişmenizi sağlar. Bu erişim, Kullanıcı ekleme ve yönetme, parolaları sıfırlama ve kullanıcı lisanslarını yönetme gibi yönetim işlevleri yapmanıza olanak sağlar. Müşteriler ile CSP satıcı ilişkilerini kurarken bu ayrıcalıkları alırsınız.
- **Abonelik düzeyinde yönetici ayrıcalıkları** , MÜŞTERILERINIZIN Azure CSP aboneliklerine tam erişim sağlar. Bu erişim, Azure kaynaklarını sağlamanızı ve yönetmenizi sağlar. Müşterileriniz için Azure CSP abonelikleri oluştururken bu ayrıcalıkları alırsınız.

## <a name="how-to-reinstate-your-csp-admin-privileges"></a>CSP yönetici ayrıcalıklarınızı yeniden devreye sokma

Yönetici ayrıcalıklarını yeniden kazanmak için müşterinizden çalışabilirsiniz.

> [!NOTE]
> Iş Ortağı Merkezi önizleme arabirimi, mantıksal olarak gruplanmış çalışma alanları aracılığıyla daha verimli ve üretken bir kullanıcı deneyimi sağlar. Çalışma alanları arabirimi ve nasıl kullanılacağı hakkında daha fazla bilgi edinmek için bkz. [Iş ortağı merkezini alma](get-around-partner-center.md#turn-workspaces-on-and-off).

#### <a name="workspaces-view"></a>[Çalışma alanları görünümü](#tab/workspaces-view)

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard) oturum açın.

2. **Müşteriler** kutucuğunu seçin.

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

#### <a name="current-view"></a>[Geçerli görünüm](#tab/current-view)

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard) oturum açın.

2. Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin.

3. Kullanmakta olduğunuz müşteriyi seçin ve **bir satıcı ilişkisi isteyin**. Bu eylem, müşterinizin bağlantısını e-posta ile gönderir.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Satıcı ilişkisi oluştur e-posta örneği.":::

4. Müşteriniz, sunulan bağlantı aracılığıyla satıcı ilişki isteğini onayladığında, AdminAgents grubunu almak için iş ortağı kiracıya bağlanın `object ID` .
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

5. Müşterinizin şunları içerdiğinden emin olun:

   1. **Sahip** veya **Kullanıcı erişimi Yöneticisi** rolü 
   2. Abonelik düzeyinde rol atamaları oluşturma izinleri

6. Bu işlemi gerçekleştirmek için, müşterinizin PowerShell veya Azure CLı kullanarak aşağıdaki işlemleri yapması gerekir. 

   1. PowerShell kullanılıyorsa, müşterinin modülü güncelleştirmesi gerekir `Az.Resources` .

       ```powershell
       Update-Module Az.Resources
       ```

   2. Müşteri, CSP aboneliğinin bulunduğu kiracıya bağlanmalıdır.

      ```powershell
      Connect-AzAccount -TenantID "<Customer tenant>"
      ```

      ```azurecli
      az login --tenant <Customer tenant>
      ```

   3. Müşterinin daha sonra aboneliğe bağlanması gerekir. Bu, *yalnızca* kullanıcının Kiracıdaki birden çok abonelik üzerinde rol atama izinlerine sahip olması durumunda geçerlidir.

      ```powershell
      Set-AzContext -SubscriptionID <"CSP Subscription ID">
      ```

      ```azurecli
      az account set --subscription <CSP Subscription ID>
      ```

   4. Müşteri daha sonra rol atamasını oluşturabilir.

      ```powershell
      New-AzRoleAssignment -ObjectID "<Object ID of the AdminAgents group from step 4>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
      ```

      ```azurecli
      az role assignment create --role "Owner" --assignee-object-id <Object ID of the AdminAgents group from step 4> --scope "/subscriptions/<CSP Subscription Id>"
      ```

Abonelik düzeyinde sahip izinleri vermek yerine, bunlara kaynak grubu veya kaynak düzeyinde izin verebilirsiniz: 

- Kaynak grubu düzeyinde

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the AdminAgents group from step 4>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object ID of the AdminAgents group from step 4> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- Kaynak düzeyinde

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the AdminAgents group from step 4>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object ID of the AdminAgents group from step 4> --scope "<Resource URI>"
   ```

Yukarıdaki adımlar işe yoksa veya bu işlemleri gerçekleştirmeye çalışırken hata alırsanız, müşterinizin yönetici haklarını yeniden devreye sokmak için aşağıdaki "catch-all" yordamını deneyin:

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

* * *

### <a name="troubleshooting"></a>Sorun giderme
Müşteri 6. adımı tamamlayamadıysanız aşağıdaki komutu önerin ve elde edilen `newRoleAssignment.log` dosyayı daha fazla analiz Için Microsoft 'a sağlayın:

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

Sırasında "catch-all" yordamı başarısız olursa `Import-Module` , aşağıdaki adımları deneyin:
- Modül kullanımda olduğundan içeri aktarma başarısız olursa, tüm pencereleri kapatıp yeniden açarak PowerShell oturumunu yeniden başlatın.
- Sürümünü `Az.Resources` ile denetleyin `Get-Module Az.Resources -ListAvailable` .
- 4.1.1 sürümü kullanılabilir listede değilse, kullanmanız gerekir `Update-Module Az.Resources -Force` .
- Hata, `Az.Accounts` belirli bir sürüm olması gerektiğini belirtir, bu modülü de `Az.Resources` ile değiştirin `Az.Accounts` . Ardından PowerShell oturumunu yeniden başlatmanız gerekir.


## <a name="next-steps"></a>Sonraki adımlar

- [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)
