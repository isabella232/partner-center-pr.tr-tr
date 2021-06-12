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
ms.openlocfilehash: 90c8f413398fcb9f65f7fef402a1cdcd092abbc4
ms.sourcegitcommit: 212471150efc8fd2c30023bc6a981a7e052e79ef
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/11/2021
ms.locfileid: "112025964"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="cfcfe-103">Müşterinin abonelikleri için yönetici ayrıcalıklarını yeniden Azure CSP olun</span><span class="sxs-lookup"><span data-stu-id="cfcfe-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="cfcfe-104">**Uygun roller:** Genel yönetici | Yönetici aracısı</span><span class="sxs-lookup"><span data-stu-id="cfcfe-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="cfcfe-105">CSP iş ortağı olarak müşterileriniz genellikle Azure kullanımlarını ve sistemlerini onlar için yöneteceklerini bekler.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-105">As a CSP partner, your customers often expect that you'll manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="cfcfe-106">Bunu yapmak için yönetici ayrıcalıklarına sahip olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-106">You must have admin privileges to do so.</span></span> <span data-ttu-id="cfcfe-107">Müşteriyle kurumsal bayi ilişkiniz kurulu olduğunda bazı ayrıcalıklar verir.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="cfcfe-108">Başkalarına da müşteriniz tarafından izin ve verildi.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="cfcfe-109">CSP'de Azure için yönetici ayrıcalıkları</span><span class="sxs-lookup"><span data-stu-id="cfcfe-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="cfcfe-110">Kullanıcılar için iki yönetici ayrıcalıkları CSP'de Azure.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-110">There are two levels of admin privileges for Azure in CSP.</span></span>

- <span data-ttu-id="cfcfe-111">**Kiracı düzeyinde yönetici ayrıcalıkları (Yönetici ayrıcalıkları temsilcisi)**: CSP iş ortakları, müşterilerle CSP kurumsal bayi ilişkisi kurulurken bu ayrıcalıkları alır.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-111">**Tenant level admin privileges (Delegated admin privileges)**:  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="cfcfe-112">Temsilcili yönetici ayrıcalıkları, CSP iş ortaklarının müşterilerinin kiracılarına erişmesini sağlar.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-112">Delegated admin privileges give CSP partners access to their customers' tenants.</span></span> <span data-ttu-id="cfcfe-113">Bu erişim, kullanıcı ekleme/yönetme, parolaları sıfırlama ve kullanıcı lisanslarını yönetme gibi yönetim işlevlerini yapmalarına olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-113">This access allows them to do administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>
- <span data-ttu-id="cfcfe-114">**Abonelik düzeyi yönetici ayrıcalıkları:** CSP iş ortakları, müşterileri için Azure CSP abonelikleri oluştururken bu ayrıcalıkları elde eder.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-114">**Subscription level admin privileges**: CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="cfcfe-115">Bu ayrıcalıklara sahip olmak, CSP iş ortaklarının bu aboneliklere tam erişim sağlamalarını ve Azure kaynaklarını yönetmelerini sağlar.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-115">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-a-partners-admin-privileges"></a><span data-ttu-id="cfcfe-116">İş ortağının yönetici ayrıcalıklarını CSP'ye yeniden iade edin</span><span class="sxs-lookup"><span data-stu-id="cfcfe-116">Reinstate CSP a partner's admin privileges</span></span>

<span data-ttu-id="cfcfe-117">Müşterinize AdminAgents grubunun sağlamasını sağlarsanız müşteriniz CSP rol `object ID` atamasını yeniden oluşturabilir.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-117">Your customer can re-create the CSP role assignment if you provide the `object ID` of the AdminAgents group to your customer.</span></span> <span data-ttu-id="cfcfe-118">Temsilci yönetici ayrıcalıklarını yeniden kazanmak için aşağıdaki adımlarla müşteriyle çalışmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-118">To regain delegated admin privileges, you need to work with your customer through the following steps.</span></span>

1. <span data-ttu-id="cfcfe-119">Panoda İş Ortağı Merkezi açın.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-119">Sign into the Partner Center dashboard.</span></span>

2. <span data-ttu-id="cfcfe-120">Yeni İş Ortağı Merkezi Müşteriler'i **seçin.**</span><span class="sxs-lookup"><span data-stu-id="cfcfe-120">On the Partner Center menu, select **Customers**.</span></span>

3. <span data-ttu-id="cfcfe-121">Üzerinde çalışmakta olduğunu müşteriyi seçin ve **bir kurumsal bayi ilişkisi talep edin.**</span><span class="sxs-lookup"><span data-stu-id="cfcfe-121">Select the customer you are working with and **request a reseller relationship**.</span></span> <span data-ttu-id="cfcfe-122">Bu eylem kiracı yönetici haklarına sahip olan müşteriye bir bağlantı üretir.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-122">This action generates a link to the customer who has tenant admin rights.</span></span>

4. <span data-ttu-id="cfcfe-123">Müşterinizin bağlantıyı seçmesi ve kurumsal bayi ilişkisi isteğini onaylaması gerekir.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-123">Your customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Kurumsal bayi ilişkisi oluşturma e-posta örneği":::

5. <span data-ttu-id="cfcfe-125">İş ortağı olarak AdminAgents grubunun Nesne Kimliğini almak için iş ortağı kiracısına bağlanmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. <span data-ttu-id="cfcfe-126">Daha sonra müşterinizin PowerShell veya Azure CLI kullanarak aşağıdaki adımları gerçekleştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-126">Your customer must then do the following steps using either PowerShell or Azure CLI.</span></span> <span data-ttu-id="cfcfe-127">Müşterinizin şunların olması gerekir:</span><span class="sxs-lookup"><span data-stu-id="cfcfe-127">Your customer must have:</span></span>

- <span data-ttu-id="cfcfe-128">Sahip veya **kullanıcı** erişimi **yöneticisi rolü**</span><span class="sxs-lookup"><span data-stu-id="cfcfe-128">The role of **owner** or **user access administrator**</span></span> 
- <span data-ttu-id="cfcfe-129">Abonelik düzeyinde rol ataması oluşturma izinleri</span><span class="sxs-lookup"><span data-stu-id="cfcfe-129">Permissions to create role assignments at the subscription level</span></span>

   <span data-ttu-id="cfcfe-130">a.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-130">a.</span></span> <span data-ttu-id="cfcfe-131">Yalnızca PowerShell için müşterinin modülü güncelleştirmesi `Az.Resources` gerekir.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-131">For PowerShell only, the customer must update the `Az.Resources` module.</span></span>
   ```powershell
   Update-Module Az.Resources
   ```

   <span data-ttu-id="cfcfe-132">b.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-132">b.</span></span> <span data-ttu-id="cfcfe-133">Müşteri CSP aboneliğinin bulunduğu kiracıya bağlanır.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-133">The customer connects to the tenant where the CSP subscription exists.</span></span>
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   <span data-ttu-id="cfcfe-134">c.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-134">c.</span></span> <span data-ttu-id="cfcfe-135">Müşteri aboneliğe bağlanır.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-135">The customer connects to the subscription.</span></span> <span data-ttu-id="cfcfe-136">Bu yalnızca *kullanıcının* kiracıda birden çok abonelik üzerinde rol atama izinlerine sahip olması için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-136">This is *only* applicable if the user has role assignment permissions over multiple subscriptions in the tenant.</span></span>

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   <span data-ttu-id="cfcfe-137">d.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-137">d.</span></span> <span data-ttu-id="cfcfe-138">Müşteri daha sonra rol ataması oluşturur.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-138">The customer then creates the role assignment.</span></span>
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

<span data-ttu-id="cfcfe-139">Abonelik kapsamında sahip izinleri vermek yerine kaynak grubu veya kaynak düzeyinde izin veebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-139">Instead of granting owner permissions at the subscription scope, you can grant at the resource group or resource level.</span></span> 

- <span data-ttu-id="cfcfe-140">Kaynak grubu düzeyinde</span><span class="sxs-lookup"><span data-stu-id="cfcfe-140">At the resource group level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- <span data-ttu-id="cfcfe-141">Kaynak düzeyinde</span><span class="sxs-lookup"><span data-stu-id="cfcfe-141">At the resource level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

<span data-ttu-id="cfcfe-142">Yukarıdaki adımlar işe çalışmıyorsa veya deneme sırasında hatalarla karşınıza çıkarsanız, müşteriniz için yönetici haklarını yeniden sağlamak için aşağıdaki "hepsini yakala" yordamını deneyin.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-142">If the above steps don't work or you get errors when attempting them, try the following "catch-all" procedure to reinstate admin rights for your customer.</span></span>

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a><span data-ttu-id="cfcfe-143">Sorun giderme</span><span class="sxs-lookup"><span data-stu-id="cfcfe-143">Troubleshooting</span></span>

<span data-ttu-id="cfcfe-144">Müşteri yukarıdaki 6. adımı tamamlayamazsa müşterinin aşağıdaki komutu denemesi gerekir:</span><span class="sxs-lookup"><span data-stu-id="cfcfe-144">If the customer is unable to complete step 6 above, have the customer try the following command:</span></span>

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

<span data-ttu-id="cfcfe-145">Daha fazla analiz için `newRoleAssignment.log` elde edilen dosyayı Microsoft'a sağlama.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-145">Provide the resulting `newRoleAssignment.log` file to Microsoft for further analysis.</span></span>

<span data-ttu-id="cfcfe-146">sırasında "hepsini yakala" yordamı başarısız olursa `Import-Module` aşağıdaki adımları deneyin:</span><span class="sxs-lookup"><span data-stu-id="cfcfe-146">If the "catch-all" procedure fails during the `Import-Module`, try the following steps:</span></span>
- <span data-ttu-id="cfcfe-147">Modül kullanımda olduğundan içeri aktarma başarısız olursa, tüm pencereleri kapatıp yeniden açarak PowerShell oturumunu yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-147">If the import fails because the module is in use, restart the PowerShell session by closing and reopening all windows.</span></span>
- <span data-ttu-id="cfcfe-148">ile sürümünü `Az.Resources` kontrol `Get-Module Az.Resources -ListAvailable` edin.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-148">Check version of `Az.Resources` with `Get-Module Az.Resources -ListAvailable`.</span></span>
- <span data-ttu-id="cfcfe-149">Sürüm 4.1.1 kullanılabilir listede yoksa, kullansanız `Update-Module Az.Resources -Force` gerekir.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-149">If version 4.1.1 is not within the available list, you must use `Update-Module Az.Resources -Force`.</span></span>
- <span data-ttu-id="cfcfe-150">Hata belirli bir sürüm `Az.Accounts` olması gerektiğini belirttiyse, yerine bu modülü de `Az.Resources` `Az.Accounts` güncelleştirin.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-150">If the error states that `Az.Accounts` needs to be a specific version, update that module as well, replacing `Az.Resources` with `Az.Accounts`.</span></span> <span data-ttu-id="cfcfe-151">Ardından PowerShell oturumunu yeniden başlatmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="cfcfe-151">You must then restart the PowerShell session.</span></span>


## <a name="next-steps"></a><span data-ttu-id="cfcfe-152">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="cfcfe-152">Next steps</span></span>

- [<span data-ttu-id="cfcfe-153">Azure planı kapsamındaki abonelikleri ve kaynakları yönetme</span><span class="sxs-lookup"><span data-stu-id="cfcfe-153">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
