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
ms.openlocfilehash: f536d975d3c644a7afa29a95a3cb45608f6b2c9f
ms.sourcegitcommit: 89be77c9f35c77463d9558826293202afc6dec56
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/13/2021
ms.locfileid: "107315856"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="95237-103">Müşterinin Azure CSP abonelikleri için yeniden devreye sokma yönetici ayrıcalıkları</span><span class="sxs-lookup"><span data-stu-id="95237-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="95237-104">**Uygulanabilir roller**</span><span class="sxs-lookup"><span data-stu-id="95237-104">**Applicable roles**</span></span>

- <span data-ttu-id="95237-105">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="95237-105">Global admin</span></span>
- <span data-ttu-id="95237-106">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="95237-106">Admin agent</span></span>

<span data-ttu-id="95237-107">Bir CSP iş ortağı olarak, müşterileriniz genellikle Azure kullanımını ve sistemlerini kendileri için yöneteceksiniz.</span><span class="sxs-lookup"><span data-stu-id="95237-107">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="95237-108">Bunun yapılması yönetici ayrıcalıklarına sahip olmanızı gerektirir.</span><span class="sxs-lookup"><span data-stu-id="95237-108">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="95237-109">Müşteri ile satıcı ilişkiniz oluşturulduğunda bazı ayrıcalıklar verilir.</span><span class="sxs-lookup"><span data-stu-id="95237-109">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="95237-110">Başkaları sizin tarafınızdan size verilir.</span><span class="sxs-lookup"><span data-stu-id="95237-110">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="95237-111">CSP 'de Azure için yönetici ayrıcalıkları</span><span class="sxs-lookup"><span data-stu-id="95237-111">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="95237-112">CSP 'de Azure için iki yönetim ayrıcalıkları düzeyi vardır.</span><span class="sxs-lookup"><span data-stu-id="95237-112">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="95237-113">**Kiracı düzeyinde yönetici ayrıcalıkları** (**yönetici ayrıcalıkları temsilcisi**)-CSP Iş ortakları, müşterilerle CSP satıcısı ilişkisi oluştururken bu ayrıcalıkları alır.</span><span class="sxs-lookup"><span data-stu-id="95237-113">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="95237-114">Yönetici ayrıcalıkları, CSP iş ortaklarının müşterilerinin kiracılarına erişmesini sağlar ve bu sayede kullanıcıları ekleme/yönetme, parolaları sıfırlama ve kullanıcı lisanslarını yönetme gibi yönetim işlevleri gerçekleştirebilir.</span><span class="sxs-lookup"><span data-stu-id="95237-114">Delegated admin privileges gives CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="95237-115">**Abonelik düzeyi yönetici ayrıcalıkları** -CSP iş ortakları, müşterileri IÇIN Azure CSP abonelikleri oluştururken bu ayrıcalıkları alırlar.</span><span class="sxs-lookup"><span data-stu-id="95237-115">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="95237-116">Bu ayrıcalıklara sahip olmak, CSP iş ortaklarının bu aboneliklerde Azure kaynaklarını sağlamasına ve yönetmesine olanak tanıyan tüm erişimleri olmasını sağlar.</span><span class="sxs-lookup"><span data-stu-id="95237-116">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="95237-117">Yeniden devreye sokma CSP iş ortakları yönetici ayrıcalıkları</span><span class="sxs-lookup"><span data-stu-id="95237-117">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="95237-118">Müşteriniz, AdminAgents grubunun nesne KIMLIĞINI sağladığınız sürece, CSP rol atamasını yeniden oluşturabilir.</span><span class="sxs-lookup"><span data-stu-id="95237-118">Your customer is able to re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="95237-119">Yetkilendirilmiş yönetici ayrıcalıklarını yeniden kazanmak için müşterinizden çalışmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="95237-119">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="95237-120">Iş Ortağı Merkezi panosunda oturum açın ve Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="95237-120">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="95237-121">Çalıştığınız müşteriyi seçin ve **bir satıcı ilişkisi isteyin.**</span><span class="sxs-lookup"><span data-stu-id="95237-121">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="95237-122">Bu, kiracı yönetici haklarına sahip olan müşteriye bir bağlantı oluşturur.</span><span class="sxs-lookup"><span data-stu-id="95237-122">This generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="95237-123">Bu müşterinin bağlantıyı seçmesini ve satıcı ilişki isteğini onaylaması gerekir.</span><span class="sxs-lookup"><span data-stu-id="95237-123">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Satıcı ilişkisi oluştur e-posta örneği":::

4. <span data-ttu-id="95237-125">İş ortağının, AdminAgents grubunun nesne KIMLIĞINI almak için iş ortağı kiracısına bağlanması gerekir.</span><span class="sxs-lookup"><span data-stu-id="95237-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="95237-126">**Sahibi veya Kullanıcı erişimi Yöneticisi** rolüne sahip olan ve abonelik düzeyinde rol ataması oluşturma izni olan müşteriniz şunları yapar:</span><span class="sxs-lookup"><span data-stu-id="95237-126">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="95237-127">CSP aboneliğinin bulunduğu kiracıya bağlanır.</span><span class="sxs-lookup"><span data-stu-id="95237-127">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="95237-128">Aboneliğe bağlanır (yalnızca kullanıcının Kiracıdaki birden çok abonelik üzerinde rol ataması izinleri varsa geçerlidir).</span><span class="sxs-lookup"><span data-stu-id="95237-128">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="95237-129">PS C:\WINDOWS\system32> Set-AzContext-SubscriptionID "CSP abonelik KIMLIĞI" '</span><span class="sxs-lookup"><span data-stu-id="95237-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="95237-130">Rol atamasını oluşturur</span><span class="sxs-lookup"><span data-stu-id="95237-130">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="95237-131">Abonelik kapsamı yerine kaynak grubu düzeyinde veya kaynak düzeyinde sahip rolü izni vermek istiyorsanız, aşağıdaki komutlar kullanılabilir:</span><span class="sxs-lookup"><span data-stu-id="95237-131">If the desire is to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="95237-132">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="95237-132">Next steps</span></span>

- [<span data-ttu-id="95237-133">Azure planı kapsamındaki abonelikleri ve kaynakları yönetme</span><span class="sxs-lookup"><span data-stu-id="95237-133">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
