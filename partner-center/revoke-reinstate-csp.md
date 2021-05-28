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
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="a575c-103">Müşterinin abonelikleri için yönetici ayrıcalıklarını yeniden Azure CSP olun</span><span class="sxs-lookup"><span data-stu-id="a575c-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="a575c-104">**Uygun roller:** Genel yönetici | Yönetici aracısı</span><span class="sxs-lookup"><span data-stu-id="a575c-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="a575c-105">CSP iş ortağı olarak müşterileriniz genellikle Azure kullanımlarını ve sistemlerini onlar için yöneteceklerini bekler.</span><span class="sxs-lookup"><span data-stu-id="a575c-105">As a CSP partner, your customers often expect that you'll manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="a575c-106">Bunu yapmak için yönetici ayrıcalıklarına sahip olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="a575c-106">You must have admin privileges to do so.</span></span> <span data-ttu-id="a575c-107">Müşteriyle kurumsal bayi ilişkiniz kurulu olduğunda bazı ayrıcalıklar verir.</span><span class="sxs-lookup"><span data-stu-id="a575c-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="a575c-108">Başkalarına da müşteriniz tarafından verildi.</span><span class="sxs-lookup"><span data-stu-id="a575c-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="a575c-109">CSP'de Azure için yönetici ayrıcalıkları</span><span class="sxs-lookup"><span data-stu-id="a575c-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="a575c-110">Kullanıcılar için iki yönetici ayrıcalıkları CSP'de Azure.</span><span class="sxs-lookup"><span data-stu-id="a575c-110">There are two levels of admin privileges for Azure in CSP.</span></span>

- <span data-ttu-id="a575c-111">**Kiracı düzeyinde yönetici ayrıcalıkları (Yönetici ayrıcalıkları temsilcisi)**: CSP iş ortakları, müşterilerle CSP kurumsal bayi ilişkisi kurulurken bu ayrıcalıkları alır.</span><span class="sxs-lookup"><span data-stu-id="a575c-111">**Tenant level admin privileges (Delegated admin privileges)**:  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="a575c-112">Temsilcili yönetici ayrıcalıkları, CSP iş ortaklarının müşterilerinin kiracılarına erişmesini sağlar.</span><span class="sxs-lookup"><span data-stu-id="a575c-112">Delegated admin privileges give CSP partners access to their customers' tenants.</span></span> <span data-ttu-id="a575c-113">Bu erişim, kullanıcı ekleme/yönetme, parolaları sıfırlama ve kullanıcı lisanslarını yönetme gibi yönetim işlevlerini yapmalarına olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="a575c-113">This access allows them to do administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>
- <span data-ttu-id="a575c-114">**Abonelik düzeyi yönetici ayrıcalıkları:** CSP iş ortakları, müşterileri için Azure CSP abonelikleri oluştururken bu ayrıcalıkları elde eder.</span><span class="sxs-lookup"><span data-stu-id="a575c-114">**Subscription level admin privileges**: CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="a575c-115">Bu ayrıcalıklara sahip olmak, CSP iş ortaklarının bu aboneliklere tam erişim sağlamalarını ve Azure kaynaklarını yönetmelerini sağlar.</span><span class="sxs-lookup"><span data-stu-id="a575c-115">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-a-partners-admin-privileges"></a><span data-ttu-id="a575c-116">CsP'yi iş ortağının yönetici ayrıcalıklarını yeniden açıklama</span><span class="sxs-lookup"><span data-stu-id="a575c-116">Reinstate CSP a partner's admin privileges</span></span>

<span data-ttu-id="a575c-117">Müşterinize AdminAgents grubunun sağlamasını sağlarsanız müşteriniz `object ID` CSP rol atamasını yeniden oluşturabilir.</span><span class="sxs-lookup"><span data-stu-id="a575c-117">Your customer can re-create the CSP role assignment if you provide the `object ID` of the AdminAgents group to your customer.</span></span> <span data-ttu-id="a575c-118">Temsilci yönetici ayrıcalıklarını yeniden kazanmak için aşağıdaki adımlarla müşteriyle çalışmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="a575c-118">To regain delegated admin privileges, you need to work with your customer through the following steps.</span></span>

1. <span data-ttu-id="a575c-119">Panoda İş Ortağı Merkezi açın.</span><span class="sxs-lookup"><span data-stu-id="a575c-119">Sign into the Partner Center dashboard.</span></span>

2. <span data-ttu-id="a575c-120">Yeni İş Ortağı Merkezi Müşteriler'i **seçin.**</span><span class="sxs-lookup"><span data-stu-id="a575c-120">On the Partner Center menu, select **Customers**.</span></span>

3. <span data-ttu-id="a575c-121">Çalıştığınız müşteriyi seçin ve **bir satıcı ilişkisi isteyin**.</span><span class="sxs-lookup"><span data-stu-id="a575c-121">Select the customer you are working with and **request a reseller relationship**.</span></span> <span data-ttu-id="a575c-122">Bu eylem, kiracı yönetici haklarına sahip olan müşteriye bir bağlantı oluşturur.</span><span class="sxs-lookup"><span data-stu-id="a575c-122">This action generates a link to the customer who has tenant admin rights.</span></span>

4. <span data-ttu-id="a575c-123">Müşterinizin bağlantıyı seçmesini ve satıcı ilişki isteğini onaylaması gerekir.</span><span class="sxs-lookup"><span data-stu-id="a575c-123">Your customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Satıcı ilişkisi oluştur e-posta örneği":::

5. <span data-ttu-id="a575c-125">İş ortağının, AdminAgents grubunun nesne KIMLIĞINI almak için iş ortağı kiracısına bağlanması gerekir.</span><span class="sxs-lookup"><span data-stu-id="a575c-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. <span data-ttu-id="a575c-126">Müşterinizin, PowerShell veya Azure CLı kullanarak aşağıdaki adımları yapması gerekir.</span><span class="sxs-lookup"><span data-stu-id="a575c-126">Your customer must then do the following steps using either PowerShell or Azure CLI.</span></span> <span data-ttu-id="a575c-127">Müşterinizin şunları uygulamanız gerekir:</span><span class="sxs-lookup"><span data-stu-id="a575c-127">Your customer must have:</span></span>

- <span data-ttu-id="a575c-128">**Sahip** veya **Kullanıcı erişimi Yöneticisi** rolü</span><span class="sxs-lookup"><span data-stu-id="a575c-128">The role of **owner** or **user access administrator**</span></span> 
- <span data-ttu-id="a575c-129">Abonelik düzeyinde rol atamaları oluşturma izinleri</span><span class="sxs-lookup"><span data-stu-id="a575c-129">Permissions to create role assignments at the subscription level</span></span>

   <span data-ttu-id="a575c-130">a.</span><span class="sxs-lookup"><span data-stu-id="a575c-130">a.</span></span> <span data-ttu-id="a575c-131">Yalnızca PowerShell için, müşterinin modülü güncelleştirmesi gerekir `Az.Resources` .</span><span class="sxs-lookup"><span data-stu-id="a575c-131">For PowerShell only, the customer must update the `Az.Resources` module.</span></span>
   ```powershell
   Update-Module Az.Resources
   ```

   <span data-ttu-id="a575c-132">b.</span><span class="sxs-lookup"><span data-stu-id="a575c-132">b.</span></span> <span data-ttu-id="a575c-133">Müşteri, CSP aboneliğinin bulunduğu kiracıya bağlanır.</span><span class="sxs-lookup"><span data-stu-id="a575c-133">The customer connects to the tenant where the CSP subscription exists.</span></span>
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   <span data-ttu-id="a575c-134">c.</span><span class="sxs-lookup"><span data-stu-id="a575c-134">c.</span></span> <span data-ttu-id="a575c-135">Müşteri, aboneliğe bağlanır.</span><span class="sxs-lookup"><span data-stu-id="a575c-135">The customer connects to the subscription.</span></span> <span data-ttu-id="a575c-136">Bu, *yalnızca* kullanıcının Kiracıdaki birden çok abonelik üzerinde rol atama izinlerine sahip olması durumunda geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="a575c-136">This is *only* applicable if the user has role assignment permissions over multiple subscriptions in the tenant.</span></span>

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   <span data-ttu-id="a575c-137">d.</span><span class="sxs-lookup"><span data-stu-id="a575c-137">d.</span></span> <span data-ttu-id="a575c-138">Müşteri daha sonra rol atamasını oluşturur.</span><span class="sxs-lookup"><span data-stu-id="a575c-138">The customer then creates the role assignment.</span></span>
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

<span data-ttu-id="a575c-139">Abonelik kapsamında sahip izinleri vermek yerine, kaynak grubu veya kaynak düzeyinde izin verebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a575c-139">Instead of granting owner permissions at the subscription scope, you can grant at the resource group or resource level.</span></span> 

- <span data-ttu-id="a575c-140">Kaynak grubu düzeyinde</span><span class="sxs-lookup"><span data-stu-id="a575c-140">At the resource group level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- <span data-ttu-id="a575c-141">Kaynak düzeyinde</span><span class="sxs-lookup"><span data-stu-id="a575c-141">At the resource level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

## <a name="next-steps"></a><span data-ttu-id="a575c-142">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="a575c-142">Next steps</span></span>

- [<span data-ttu-id="a575c-143">Azure planı kapsamındaki abonelikleri ve kaynakları yönetme</span><span class="sxs-lookup"><span data-stu-id="a575c-143">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
