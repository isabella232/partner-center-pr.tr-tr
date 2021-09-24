---
title: Azure CSP için yönetici ayrıcalıklarını yeniden devreye sokma
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: İş ortağının müşterinin Azure Bulut Çözümü Sağlayıcısı (CSP) aboneliklerini yönetmeye yardımcı olmak için müşterilerin bir iş ortağının yönetici ayrıcalıklarını yeniden Bulut Çözümü Sağlayıcısı nasıl yardımcı olduğunu öğrenin.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 7ec17a386e3ac6e9b41ce0582f0c55e424ce5e64
ms.sourcegitcommit: fceaca54b0ec695cf214209c09b4516e1b40866a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/24/2021
ms.locfileid: "128359440"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Müşterinin abonelikleri için yönetici ayrıcalıklarını yeniden Azure CSP olun  

**Uygun roller:** Genel yönetici | Yönetici aracısı

Bir Bulut Çözümü Sağlayıcısı (CSP) programı iş ortağı olarak müşterileriniz genellikle Azure kullanımlarını ve sistemlerini yönetmeniz için size güveniyor. Onlara yardımcı olmak için yönetici ayrıcalıklarına sahip olmanız gerekir. Henüz yönetici ayrıcalıklarına sahip değilseniz müşteriniz ile birlikte çalışarak bunları yeniden çalışır.

## <a name="admin-privileges-for-azure-in-the-csp-program"></a>CSP programında Azure için yönetici ayrıcalıkları

Bazı yönetici ayrıcalıkları, müşteriyle kurumsal bayi ilişkisi kurduğunda otomatik olarak verir. Başkalarının da size müşteri tarafından verilmesi gerekir. Kullanıcılar için iki yönetici ayrıcalıkları CSP'de Azure.

- **Kiracı düzeyinde yönetici ayrıcalıkları (diğer bir ifadeyle,** yönetici ayrıcalıkları temsilcisi), müşterinizin kiracılarına erişmenizi sağlar. Bu erişim, kullanıcı ekleme ve yönetme, parolaları sıfırlama ve kullanıcı lisanslarını yönetme gibi yönetim işlevlerini uygulamanıza olanak sağlar. Müşterilerle CSP kurumsal bayi ilişkileri kurulurken bu ayrıcalıkları elde edersiniz.
- **Abonelik düzeyinde yönetici ayrıcalıkları,** müşterilerinize ve aboneliklere tam Azure CSP sağlar. Bu erişim, Azure kaynaklarını sağlamanıza ve yönetmenize olanak sağlar. Müşterileriniz için farklı abonelikler Azure CSP bu ayrıcalıkları elde edersiniz.

## <a name="how-to-reinstate-your-csp-admin-privileges"></a>CSP yönetici ayrıcalıklarınızı yeniden yetkiye alma

Temsilci olarak yönetici ayrıcalıklarını geri kazanmak için müşteriyle birlikte çalışabilirsiniz.

1. Panonuza İş Ortağı Merkezi [açın.](https://partner.microsoft.com/dashboard)

2. Veri İş Ortağı Merkezi Müşteriler'i **seçin.**

3. Çalışmakta olduğunu müşteriyi seçin ve bir **kurumsal bayi ilişkisi talep edin.** Bu eylem, müşterinizin bağlantısını e-posta ile iletir.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Kurumsal bayi ilişkisi oluşturma e-posta örneği.":::

4. Müşteriniz sağlanan bağlantı aracılığıyla kurumsal bayi ilişkisi isteğini onayladığı zaman AdminAgents grubunun bağlantısını almak için iş `object ID` ortağı kiracısına bağlanın.
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

5. Müşterinizin şunları sahip olduğundan emin olmak:

   1. Sahip veya **kullanıcı** erişimi **yöneticisi rolü** 
   2. Abonelik düzeyinde rol ataması oluşturma izinleri

6. Süreci tamamlamak için müşterinizin PowerShell veya Azure CLI kullanarak aşağıdaki işlemleri tamamlaması gerekir. 

   1. PowerShell kullanıyorsanız müşterinin modülü güncelleştirmesi `Az.Resources` gerekir.

       ```powershell
       Update-Module Az.Resources
       ```

   2. Müşterinin CSP aboneliğinin mevcut olduğu kiracıya bağlanması gerekir.

      ```powershell
      Connect-AzAccount -TenantID "<Customer tenant>"
      ```

      ```azurecli
      az login --tenant <Customer tenant>
      ```

   3. Müşterinin daha sonra aboneliğe bağlanması gerekir. Bu yalnızca *kullanıcının* kiracıda birden çok abonelik üzerinde rol atama izinlerine sahip olması için geçerlidir.

      ```powershell
      Set-AzContext -SubscriptionID <"CSP Subscription ID">
      ```

      ```azurecli
      az account set --subscription <CSP Subscription ID>
      ```

   4. Müşteri daha sonra rol ataması oluşturabilir.

      ```powershell
      New-AzRoleAssignment -ObjectID "<Object ID of the AdminAgents group from step 4>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
      ```

      ```azurecli
      az role assignment create --role "Owner" --assignee-object-id <Object ID of the AdminAgents group from step 4> --scope "/subscriptions/<CSP Subscription Id>"
      ```

Abonelik düzeyinde sahip izinleri vermek yerine kaynak grubu veya kaynak düzeyinde izin veebilirsiniz: 

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

Yukarıdaki adımlar işe çalışmıyorsa veya deneme sırasında hatalarla karşınıza çıkarsanız, müşteriniz için yönetici haklarını yeniden sağlamak için aşağıdaki "hepsini yakala" yordamını deneyin:

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```
### <a name="troubleshooting"></a>Sorun giderme
Müşteri 6. adımı tamamlayamazsa aşağıdaki komutu önerin ve elde edilen dosyayı daha fazla analiz için `newRoleAssignment.log` Microsoft'a yazın:

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

sırasında "hepsini yakala" yordamı başarısız olursa `Import-Module` aşağıdaki adımları deneyin:
- Modül kullanım durumunda olduğundan içeri aktarma başarısız olursa, tüm pencereleri kapatıp yeniden açarak PowerShell oturumunu yeniden başlatın.
- ile sürümünü `Az.Resources` kontrol `Get-Module Az.Resources -ListAvailable` edin.
- Sürüm 4.1.1 kullanılabilir listede yoksa, kullansanız `Update-Module Az.Resources -Force` gerekir.
- Hata belirli bir sürüm `Az.Accounts` olması gerektiğini belirttiyse, yerine bu modülü de `Az.Resources` `Az.Accounts` güncelleştirin. Ardından PowerShell oturumunu yeniden başlatmanız gerekir.


## <a name="next-steps"></a>Sonraki adımlar

- [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)
