---
title: Azure CSP için yeniden devreye sokma yönetici ayrıcalıkları
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Müşterilerin bir müşterinin Azure CSP aboneliklerini yönetmeye yardımcı olması için, ortağın yönetici ayrıcalıklarını yeniden devreye sokmasını nasıl sağlayacağınızı öğrenin.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 81df7578f7f15def64a3c20b15f95f3b89a28d1c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277785"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="0642b-103">Müşterinin Azure CSP abonelikleri için yeniden devreye sokma yönetici ayrıcalıkları</span><span class="sxs-lookup"><span data-stu-id="0642b-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="0642b-104">**Uygun roller**: genel yönetici | Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="0642b-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="0642b-105">Bir CSP iş ortağı olarak, müşterileriniz genellikle Azure kullanımını ve sistemlerini kendileri için yöneteceksiniz.</span><span class="sxs-lookup"><span data-stu-id="0642b-105">As a CSP partner, your customers often expect that you'll manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="0642b-106">Bunu yapmak için yönetici ayrıcalıklarına sahip olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="0642b-106">You must have admin privileges to do so.</span></span> <span data-ttu-id="0642b-107">Müşteri ile satıcı ilişkiniz oluşturulduğunda bazı ayrıcalıklar verilir.</span><span class="sxs-lookup"><span data-stu-id="0642b-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="0642b-108">Başkaları sizin tarafınızdan size verilir.</span><span class="sxs-lookup"><span data-stu-id="0642b-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="0642b-109">CSP 'de Azure için yönetici ayrıcalıkları</span><span class="sxs-lookup"><span data-stu-id="0642b-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="0642b-110">CSP 'de Azure için iki yönetim ayrıcalıkları düzeyi vardır.</span><span class="sxs-lookup"><span data-stu-id="0642b-110">There are two levels of admin privileges for Azure in CSP.</span></span>

- <span data-ttu-id="0642b-111">**Kiracı düzeyinde yönetici ayrıcalıkları (yönetici ayrıcalıkları temsilcisi)**: CSP iş ortakları, müşterilerle CSP satıcısı ilişkisi oluştururken bu ayrıcalıkları alır.</span><span class="sxs-lookup"><span data-stu-id="0642b-111">**Tenant level admin privileges (Delegated admin privileges)**:  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="0642b-112">Yönetici ayrıcalıkları, CSP iş ortaklarının müşterilerinin kiracılarına erişmesini sağlar.</span><span class="sxs-lookup"><span data-stu-id="0642b-112">Delegated admin privileges give CSP partners access to their customers' tenants.</span></span> <span data-ttu-id="0642b-113">Bu erişim, kullanıcıların kullanıcı ekleme/yönetme, parolaları sıfırlama ve kullanıcı lisanslarını yönetme gibi yönetim işlevleri yapmasına izin verir.</span><span class="sxs-lookup"><span data-stu-id="0642b-113">This access allows them to do administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>
- <span data-ttu-id="0642b-114">**Abonelik düzeyi yönetici ayrıcalıkları**: CSP iş ortakları, müşterileri IÇIN Azure CSP abonelikleri oluştururken bu ayrıcalıkları alır.</span><span class="sxs-lookup"><span data-stu-id="0642b-114">**Subscription level admin privileges**: CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="0642b-115">Bu ayrıcalıklara sahip olmak, CSP iş ortaklarının bu aboneliklerde Azure kaynaklarını sağlamasına ve yönetmesine olanak tanıyan tüm erişimleri olmasını sağlar.</span><span class="sxs-lookup"><span data-stu-id="0642b-115">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-a-partners-admin-privileges"></a><span data-ttu-id="0642b-116">Yeniden devreye alındı CSP bir ortağın yönetici ayrıcalıkları</span><span class="sxs-lookup"><span data-stu-id="0642b-116">Reinstate CSP a partner's admin privileges</span></span>

<span data-ttu-id="0642b-117">Müşterinizden AdminAgents grubunu sağlarsanız, müşteriniz CSP rol atamasını yeniden oluşturabilir `object ID` .</span><span class="sxs-lookup"><span data-stu-id="0642b-117">Your customer can re-create the CSP role assignment if you provide the `object ID` of the AdminAgents group to your customer.</span></span> <span data-ttu-id="0642b-118">Yetkilendirilmiş yönetici ayrıcalıklarını yeniden kazanmak için aşağıdaki adımlar aracılığıyla müşterinizden çalışmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="0642b-118">To regain delegated admin privileges, you need to work with your customer through the following steps.</span></span>

1. <span data-ttu-id="0642b-119">Iş Ortağı Merkezi panosunda oturum açın.</span><span class="sxs-lookup"><span data-stu-id="0642b-119">Sign into the Partner Center dashboard.</span></span>

2. <span data-ttu-id="0642b-120">Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="0642b-120">On the Partner Center menu, select **Customers**.</span></span>

3. <span data-ttu-id="0642b-121">Çalıştığınız müşteriyi seçin ve **bir satıcı ilişkisi isteyin**.</span><span class="sxs-lookup"><span data-stu-id="0642b-121">Select the customer you are working with and **request a reseller relationship**.</span></span> <span data-ttu-id="0642b-122">Bu eylem, kiracı yönetici haklarına sahip olan müşteriye bir bağlantı oluşturur.</span><span class="sxs-lookup"><span data-stu-id="0642b-122">This action generates a link to the customer who has tenant admin rights.</span></span>

4. <span data-ttu-id="0642b-123">Müşterinizin bağlantıyı seçmesini ve satıcı ilişki isteğini onaylaması gerekir.</span><span class="sxs-lookup"><span data-stu-id="0642b-123">Your customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Satıcı ilişkisi oluştur e-posta örneği.":::

5. <span data-ttu-id="0642b-125">İş ortağının, AdminAgents grubunun nesne KIMLIĞINI almak için iş ortağı kiracısına bağlanması gerekir.</span><span class="sxs-lookup"><span data-stu-id="0642b-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. <span data-ttu-id="0642b-126">Müşterinizin, PowerShell veya Azure CLı kullanarak aşağıdaki adımları yapması gerekir.</span><span class="sxs-lookup"><span data-stu-id="0642b-126">Your customer must then do the following steps using either PowerShell or Azure CLI.</span></span> <span data-ttu-id="0642b-127">Müşterinizin şunları uygulamanız gerekir:</span><span class="sxs-lookup"><span data-stu-id="0642b-127">Your customer must have:</span></span>

- <span data-ttu-id="0642b-128">**Sahip** veya **Kullanıcı erişimi Yöneticisi** rolü</span><span class="sxs-lookup"><span data-stu-id="0642b-128">The role of **owner** or **user access administrator**</span></span> 
- <span data-ttu-id="0642b-129">Abonelik düzeyinde rol atamaları oluşturma izinleri</span><span class="sxs-lookup"><span data-stu-id="0642b-129">Permissions to create role assignments at the subscription level</span></span>

   <span data-ttu-id="0642b-130">a.</span><span class="sxs-lookup"><span data-stu-id="0642b-130">a.</span></span> <span data-ttu-id="0642b-131">Yalnızca PowerShell için, müşterinin modülü güncelleştirmesi gerekir `Az.Resources` .</span><span class="sxs-lookup"><span data-stu-id="0642b-131">For PowerShell only, the customer must update the `Az.Resources` module.</span></span>
   ```powershell
   Update-Module Az.Resources
   ```

   <span data-ttu-id="0642b-132">b.</span><span class="sxs-lookup"><span data-stu-id="0642b-132">b.</span></span> <span data-ttu-id="0642b-133">Müşteri, CSP aboneliğinin bulunduğu kiracıya bağlanır.</span><span class="sxs-lookup"><span data-stu-id="0642b-133">The customer connects to the tenant where the CSP subscription exists.</span></span>
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   <span data-ttu-id="0642b-134">c.</span><span class="sxs-lookup"><span data-stu-id="0642b-134">c.</span></span> <span data-ttu-id="0642b-135">Müşteri, aboneliğe bağlanır.</span><span class="sxs-lookup"><span data-stu-id="0642b-135">The customer connects to the subscription.</span></span> <span data-ttu-id="0642b-136">Bu, *yalnızca* kullanıcının Kiracıdaki birden çok abonelik üzerinde rol atama izinlerine sahip olması durumunda geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="0642b-136">This is *only* applicable if the user has role assignment permissions over multiple subscriptions in the tenant.</span></span>

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   <span data-ttu-id="0642b-137">d.</span><span class="sxs-lookup"><span data-stu-id="0642b-137">d.</span></span> <span data-ttu-id="0642b-138">Müşteri daha sonra rol atamasını oluşturur.</span><span class="sxs-lookup"><span data-stu-id="0642b-138">The customer then creates the role assignment.</span></span>
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

<span data-ttu-id="0642b-139">Abonelik kapsamında sahip izinleri vermek yerine, kaynak grubu veya kaynak düzeyinde izin verebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0642b-139">Instead of granting owner permissions at the subscription scope, you can grant at the resource group or resource level.</span></span> 

- <span data-ttu-id="0642b-140">Kaynak grubu düzeyinde</span><span class="sxs-lookup"><span data-stu-id="0642b-140">At the resource group level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- <span data-ttu-id="0642b-141">Kaynak düzeyinde</span><span class="sxs-lookup"><span data-stu-id="0642b-141">At the resource level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

<span data-ttu-id="0642b-142">Yukarıdaki adımlar işe yoksa veya bu işlemleri gerçekleştirmeye çalışırken hata alırsanız, müşterinizin yönetici haklarını yeniden devreye sokmak için aşağıdaki "catch-all" yordamını deneyin.</span><span class="sxs-lookup"><span data-stu-id="0642b-142">If the above steps don't work or you get errors when attempting them, try the following "catch-all" procedure to reinstate admin rights for your customer.</span></span>

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a><span data-ttu-id="0642b-143">Sorun giderme</span><span class="sxs-lookup"><span data-stu-id="0642b-143">Troubleshooting</span></span>

<span data-ttu-id="0642b-144">Müşteri yukarıdaki 6. adımı tamamlayamadıysanız, müşterinin aşağıdaki komutu denemesini sağlayabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="0642b-144">If the customer is unable to complete step 6 above, have the customer try the following command:</span></span>

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

<span data-ttu-id="0642b-145">`newRoleAssignment.log`Daha fazla analiz için elde edilen dosyayı Microsoft 'a sağlayın.</span><span class="sxs-lookup"><span data-stu-id="0642b-145">Provide the resulting `newRoleAssignment.log` file to Microsoft for further analysis.</span></span>

<span data-ttu-id="0642b-146">Sırasında "catch-all" yordamı başarısız olursa `Import-Module` , aşağıdaki adımları deneyin:</span><span class="sxs-lookup"><span data-stu-id="0642b-146">If the "catch-all" procedure fails during the `Import-Module`, try the following steps:</span></span>
- <span data-ttu-id="0642b-147">Modül kullanımda olduğundan içeri aktarma başarısız olursa, tüm pencereleri kapatıp yeniden açarak PowerShell oturumunu yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="0642b-147">If the import fails because the module is in use, restart the PowerShell session by closing and reopening all windows.</span></span>
- <span data-ttu-id="0642b-148">Sürümünü ile denetleyin `Az.Resources` `Get-Module Az.Resources -ListAvailable` .</span><span class="sxs-lookup"><span data-stu-id="0642b-148">Check version of `Az.Resources` with `Get-Module Az.Resources -ListAvailable`.</span></span>
- <span data-ttu-id="0642b-149">Sürüm 4.1.1, kullanılabilir liste içinde değilse, kullanmanız gerekir `Update-Module Az.Resources -Force` .</span><span class="sxs-lookup"><span data-stu-id="0642b-149">If version 4.1.1 is not within the available list, you must use `Update-Module Az.Resources -Force`.</span></span>
- <span data-ttu-id="0642b-150">Hata, `Az.Accounts` belirli bir sürüm olması gerektiğini belirtir, bu modülü de `Az.Resources` ile değiştirin `Az.Accounts` .</span><span class="sxs-lookup"><span data-stu-id="0642b-150">If the error states that `Az.Accounts` needs to be a specific version, update that module as well, replacing `Az.Resources` with `Az.Accounts`.</span></span> <span data-ttu-id="0642b-151">Ardından PowerShell oturumunu yeniden başlatmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="0642b-151">You must then restart the PowerShell session.</span></span>


## <a name="next-steps"></a><span data-ttu-id="0642b-152">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="0642b-152">Next steps</span></span>

- [<span data-ttu-id="0642b-153">Azure planı kapsamındaki abonelikleri ve kaynakları yönetme</span><span class="sxs-lookup"><span data-stu-id="0642b-153">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
