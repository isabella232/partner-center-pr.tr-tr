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
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="e6d46-103">Müşterinin Azure CSP abonelikleri için yeniden devreye sokma yönetici ayrıcalıkları</span><span class="sxs-lookup"><span data-stu-id="e6d46-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="e6d46-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="e6d46-104">**Appropriate roles**</span></span>

- <span data-ttu-id="e6d46-105">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="e6d46-105">Global admin</span></span>
- <span data-ttu-id="e6d46-106">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="e6d46-106">Admin agent</span></span>

<span data-ttu-id="e6d46-107">Bir CSP iş ortağı olarak, müşterileriniz genellikle Azure kullanımını ve sistemlerini kendileri için yöneteceksiniz.</span><span class="sxs-lookup"><span data-stu-id="e6d46-107">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="e6d46-108">Bunun yapılması yönetici ayrıcalıklarına sahip olmanızı gerektirir.</span><span class="sxs-lookup"><span data-stu-id="e6d46-108">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="e6d46-109">Müşteri ile satıcı ilişkiniz oluşturulduğunda bazı ayrıcalıklar verilir.</span><span class="sxs-lookup"><span data-stu-id="e6d46-109">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="e6d46-110">Başkaları sizin tarafınızdan size verilir.</span><span class="sxs-lookup"><span data-stu-id="e6d46-110">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="e6d46-111">CSP 'de Azure için yönetici ayrıcalıkları</span><span class="sxs-lookup"><span data-stu-id="e6d46-111">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="e6d46-112">CSP 'de Azure için iki yönetim ayrıcalıkları düzeyi vardır.</span><span class="sxs-lookup"><span data-stu-id="e6d46-112">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="e6d46-113">**Kiracı düzeyinde yönetici ayrıcalıkları** (**yönetici ayrıcalıkları temsilcisi**)-CSP Iş ortakları, müşterilerle CSP satıcısı ilişkisi oluştururken bu ayrıcalıkları alır.</span><span class="sxs-lookup"><span data-stu-id="e6d46-113">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="e6d46-114">Yönetici ayrıcalıkları, CSP iş ortaklarının müşterilerinin kiracılarına erişmesini sağlar ve bu sayede Kullanıcı ekleme/yönetme, parolaları sıfırlama ve kullanıcı lisanslarını yönetme gibi yönetim işlevleri gerçekleştirebilir.</span><span class="sxs-lookup"><span data-stu-id="e6d46-114">Delegated admin privileges give CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="e6d46-115">**Abonelik düzeyi yönetici ayrıcalıkları** -CSP iş ortakları, müşterileri IÇIN Azure CSP abonelikleri oluştururken bu ayrıcalıkları alırlar.</span><span class="sxs-lookup"><span data-stu-id="e6d46-115">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="e6d46-116">Bu ayrıcalıklara sahip olmak, CSP iş ortaklarının bu aboneliklerde Azure kaynaklarını sağlamasına ve yönetmesine olanak tanıyan tüm erişimleri olmasını sağlar.</span><span class="sxs-lookup"><span data-stu-id="e6d46-116">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="e6d46-117">Yeniden devreye sokma CSP iş ortakları yönetici ayrıcalıkları</span><span class="sxs-lookup"><span data-stu-id="e6d46-117">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="e6d46-118">Müşteriniz, AdminAgents grubunun nesne KIMLIĞINI sağladığınız sürece, CSP rol atamasını yeniden oluşturabilir.</span><span class="sxs-lookup"><span data-stu-id="e6d46-118">Your customer can re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="e6d46-119">Yetkilendirilmiş yönetici ayrıcalıklarını yeniden kazanmak için müşterinizden çalışmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="e6d46-119">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="e6d46-120">Iş Ortağı Merkezi panosunda oturum açın ve Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="e6d46-120">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="e6d46-121">Çalıştığınız müşteriyi seçin ve **bir satıcı ilişkisi isteyin.**</span><span class="sxs-lookup"><span data-stu-id="e6d46-121">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="e6d46-122">Bu eylem, kiracı yönetici haklarına sahip olan müşteriye bir bağlantı oluşturur.</span><span class="sxs-lookup"><span data-stu-id="e6d46-122">This action generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="e6d46-123">Bu müşterinin bağlantıyı seçmesini ve satıcı ilişki isteğini onaylaması gerekir.</span><span class="sxs-lookup"><span data-stu-id="e6d46-123">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Satıcı ilişkisi oluştur e-posta örneği":::

4. <span data-ttu-id="e6d46-125">İş ortağının, AdminAgents grubunun nesne KIMLIĞINI almak için iş ortağı kiracısına bağlanması gerekir.</span><span class="sxs-lookup"><span data-stu-id="e6d46-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="e6d46-126">**Sahibi veya Kullanıcı erişimi Yöneticisi** rolüne sahip olan ve abonelik düzeyinde rol ataması oluşturma izni olan müşteriniz şunları yapar:</span><span class="sxs-lookup"><span data-stu-id="e6d46-126">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="e6d46-127">CSP aboneliğinin bulunduğu kiracıya bağlanır.</span><span class="sxs-lookup"><span data-stu-id="e6d46-127">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="e6d46-128">Aboneliğe bağlanır (yalnızca kullanıcının Kiracıdaki birden çok abonelik üzerinde rol ataması izinleri varsa geçerlidir).</span><span class="sxs-lookup"><span data-stu-id="e6d46-128">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="e6d46-129">PS C:\WINDOWS\system32> Set-AzContext-SubscriptionID "CSP abonelik KIMLIĞI" '</span><span class="sxs-lookup"><span data-stu-id="e6d46-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="e6d46-130">Rol atamasını oluşturur</span><span class="sxs-lookup"><span data-stu-id="e6d46-130">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="e6d46-131">Abonelik kapsamı yerine kaynak grubu düzeyinde veya kaynak düzeyinde sahip rolü izni vermek istiyorsanız aşağıdaki komutlar kullanılabilir:</span><span class="sxs-lookup"><span data-stu-id="e6d46-131">If you want to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="e6d46-132">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="e6d46-132">Next steps</span></span>

- [<span data-ttu-id="e6d46-133">Azure planı kapsamındaki abonelikleri ve kaynakları yönetme</span><span class="sxs-lookup"><span data-stu-id="e6d46-133">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
