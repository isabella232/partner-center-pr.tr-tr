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
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="767f2-103">Müşterinin abonelikleri için yönetici ayrıcalıklarını yeniden Azure CSP olun</span><span class="sxs-lookup"><span data-stu-id="767f2-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="767f2-104">**Uygun roller:** Genel yönetici | Yönetici aracısı</span><span class="sxs-lookup"><span data-stu-id="767f2-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="767f2-105">CSP iş ortağı olarak müşterileriniz genellikle Azure kullanımlarını ve sistemlerini onlar için yöneteceklerini bekler.</span><span class="sxs-lookup"><span data-stu-id="767f2-105">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="767f2-106">Bunu yapmak için yönetici ayrıcalıklarına sahip olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="767f2-106">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="767f2-107">Müşteriyle kurumsal bayi ilişkiniz kurulu olduğunda bazı ayrıcalıklar verir.</span><span class="sxs-lookup"><span data-stu-id="767f2-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="767f2-108">Başkalarına da müşteriniz tarafından izin ve verildi.</span><span class="sxs-lookup"><span data-stu-id="767f2-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="767f2-109">CSP'de Azure için yönetici ayrıcalıkları</span><span class="sxs-lookup"><span data-stu-id="767f2-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="767f2-110">Kullanıcılar için iki yönetici ayrıcalıkları CSP'de Azure.</span><span class="sxs-lookup"><span data-stu-id="767f2-110">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="767f2-111">**Kiracı düzeyi yönetici ayrıcalıkları** (**Yönetici ayrıcalıkları temsilcisi**) - CSP iş ortakları, müşterilerle CSP kurumsal bayi ilişkisi kurulurken bu ayrıcalıkları alır.</span><span class="sxs-lookup"><span data-stu-id="767f2-111">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="767f2-112">Temsilcili yönetici ayrıcalıkları, CSP iş ortaklarının müşterilerinin kiracılarına erişmesini sağlar ve bu sayede kullanıcı ekleme/yönetme, parolaları sıfırlama ve kullanıcı lisanslarını yönetme gibi yönetim işlevlerini gerçekleştirebilir.</span><span class="sxs-lookup"><span data-stu-id="767f2-112">Delegated admin privileges give CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="767f2-113">**Abonelik düzeyi yönetici ayrıcalıkları** - CSP iş ortakları, müşterileri için Azure CSP abonelikleri oluştururken bu ayrıcalıkları elde eder.</span><span class="sxs-lookup"><span data-stu-id="767f2-113">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="767f2-114">Bu ayrıcalıklara sahip olmak, CSP iş ortaklarının bu aboneliklere tam erişim sağlamalarını ve Azure kaynaklarını yönetmelerini sağlar.</span><span class="sxs-lookup"><span data-stu-id="767f2-114">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="767f2-115">CSP iş ortaklarının yönetici ayrıcalıklarını yeniden açıklama</span><span class="sxs-lookup"><span data-stu-id="767f2-115">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="767f2-116">Müşterinize AdminAgents grubunun nesne kimliğini sağlamak sürece müşteriniz CSP rol atamasını yeniden oluşturabilir.</span><span class="sxs-lookup"><span data-stu-id="767f2-116">Your customer can re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="767f2-117">Temsilci yönetici ayrıcalıklarını yeniden kazanmak için müşteriyle çalışmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="767f2-117">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="767f2-118">İş Ortağı Merkezi panosunda oturum açın ve İş Ortağı Merkezi menüsünde Müşteriler'i **seçin.**</span><span class="sxs-lookup"><span data-stu-id="767f2-118">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="767f2-119">Birlikte çalışmakta olduğunu müşteriyi seçin ve **bir kurumsal bayi ilişkisi talep edin.**</span><span class="sxs-lookup"><span data-stu-id="767f2-119">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="767f2-120">Bu eylem kiracı yönetici haklarına sahip olan müşteriye bir bağlantı üretir.</span><span class="sxs-lookup"><span data-stu-id="767f2-120">This action generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="767f2-121">Bu müşterinin bağlantıyı seçmesini ve satıcı ilişki isteğini onaylaması gerekir.</span><span class="sxs-lookup"><span data-stu-id="767f2-121">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Satıcı ilişkisi oluştur e-posta örneği":::

4. <span data-ttu-id="767f2-123">İş ortağının, AdminAgents grubunun nesne KIMLIĞINI almak için iş ortağı kiracısına bağlanması gerekir.</span><span class="sxs-lookup"><span data-stu-id="767f2-123">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="767f2-124">**Sahibi veya Kullanıcı erişimi Yöneticisi** rolüne sahip olan ve abonelik düzeyinde rol ataması oluşturma izni olan müşteriniz şunları yapar:</span><span class="sxs-lookup"><span data-stu-id="767f2-124">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="767f2-125">CSP aboneliğinin bulunduğu kiracıya bağlanır.</span><span class="sxs-lookup"><span data-stu-id="767f2-125">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="767f2-126">Aboneliğe bağlanır (yalnızca kullanıcının Kiracıdaki birden çok abonelik üzerinde rol ataması izinleri varsa geçerlidir).</span><span class="sxs-lookup"><span data-stu-id="767f2-126">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="767f2-127">PS C:\WINDOWS\system32> Set-AzContext-SubscriptionID "CSP abonelik KIMLIĞI" '</span><span class="sxs-lookup"><span data-stu-id="767f2-127">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="767f2-128">Rol atamasını oluşturur</span><span class="sxs-lookup"><span data-stu-id="767f2-128">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="767f2-129">Abonelik kapsamı yerine kaynak grubu düzeyinde veya kaynak düzeyinde sahip rolü izni vermek istiyorsanız aşağıdaki komutlar kullanılabilir:</span><span class="sxs-lookup"><span data-stu-id="767f2-129">If you want to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="767f2-130">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="767f2-130">Next steps</span></span>

- [<span data-ttu-id="767f2-131">Azure planı kapsamındaki abonelikleri ve kaynakları yönetme</span><span class="sxs-lookup"><span data-stu-id="767f2-131">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
