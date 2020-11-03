---
title: Azure CSP için yeniden devreye sokma yönetici ayrıcalıkları
ms.topic: how-to
ms.date: 07/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Müşterilerin bir müşterinin Azure CSP aboneliklerini yönetmeye yardımcı olması için, ortağın yönetici ayrıcalıklarını yeniden devreye sokmasını nasıl sağlayacağınızı öğrenin.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: c694f48fb62fc031bfaf78be6a1c4e43629a7adb
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2020
ms.locfileid: "92531226"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="f2f85-103">Müşterinin Azure CSP abonelikleri için yeniden devreye sokma yönetici ayrıcalıkları</span><span class="sxs-lookup"><span data-stu-id="f2f85-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="f2f85-104">**Uygulanabilir roller**</span><span class="sxs-lookup"><span data-stu-id="f2f85-104">**Applicable roles**</span></span>

- <span data-ttu-id="f2f85-105">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="f2f85-105">Global admin</span></span>
- <span data-ttu-id="f2f85-106">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="f2f85-106">Admin agent</span></span>

<span data-ttu-id="f2f85-107">Bir CSP iş ortağı olarak, müşterileriniz genellikle Azure kullanımını ve sistemlerini kendileri için yöneteceksiniz.</span><span class="sxs-lookup"><span data-stu-id="f2f85-107">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="f2f85-108">Bunun yapılması yönetici ayrıcalıklarına sahip olmanızı gerektirir.</span><span class="sxs-lookup"><span data-stu-id="f2f85-108">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="f2f85-109">Müşteri ile ilgili satıcı ilişkiniz oluşturulduğunda, bazı ayrıcalıklara izin verilir.</span><span class="sxs-lookup"><span data-stu-id="f2f85-109">Some privileges are granted these when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="f2f85-110">Başkaları sizin tarafınızdan size verilir.</span><span class="sxs-lookup"><span data-stu-id="f2f85-110">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="f2f85-111">CSP 'de Azure için yönetici ayrıcalıkları</span><span class="sxs-lookup"><span data-stu-id="f2f85-111">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="f2f85-112">CSP 'de Azure için iki yönetim ayrıcalıkları düzeyi vardır.</span><span class="sxs-lookup"><span data-stu-id="f2f85-112">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="f2f85-113">**Kiracı düzeyinde yönetici ayrıcalıkları** ( **yönetici ayrıcalıkları temsilcisi** )-CSP Iş ortakları, müşterilerle CSP satıcısı ilişkisi oluştururken bu ayrıcalıkları alır.</span><span class="sxs-lookup"><span data-stu-id="f2f85-113">**Tenant level admin privileges** ( **Delegated admin privileges** ) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="f2f85-114">Bu, CSP iş ortaklarının müşterilerinin kiracılarına erişmesini sağlar ve bu sayede kullanıcıları ekleme/yönetme, parolaları sıfırlama ve kullanıcı lisanslarını yönetme gibi yönetim işlevleri gerçekleştirebilir.</span><span class="sxs-lookup"><span data-stu-id="f2f85-114">This gives CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="f2f85-115">**Abonelik düzeyi yönetici ayrıcalıkları** -CSP iş ortakları, müşterileri IÇIN Azure CSP abonelikleri oluştururken bu ayrıcalıkları alırlar.</span><span class="sxs-lookup"><span data-stu-id="f2f85-115">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="f2f85-116">Bu ayrıcalıklara sahip olmak, CSP iş ortaklarının bu aboneliklerde Azure kaynaklarını sağlamasına ve yönetmesine olanak tanıyan tüm erişimleri olmasını sağlar.</span><span class="sxs-lookup"><span data-stu-id="f2f85-116">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="f2f85-117">Yeniden devreye sokma CSP iş ortakları yönetici ayrıcalıkları</span><span class="sxs-lookup"><span data-stu-id="f2f85-117">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="f2f85-118">Yetkilendirilmiş yönetici ayrıcalıklarını yeniden kazanmak için müşterinizden çalışmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="f2f85-118">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="f2f85-119">Iş Ortağı Merkezi panosunda oturum açın ve Iş Ortağı Merkezi menüsünde **müşteriler** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="f2f85-119">Sign in to Partner Center dashboard and from the Partner Center menu, select **Customers** .</span></span>

2. <span data-ttu-id="f2f85-120">Çalıştığınız müşteriyi seçin ve **bir satıcı ilişkisi isteyin.**</span><span class="sxs-lookup"><span data-stu-id="f2f85-120">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="f2f85-121">Bu, kiracı yönetici haklarına sahip olan müşteriye bir bağlantı oluşturur.</span><span class="sxs-lookup"><span data-stu-id="f2f85-121">This generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="f2f85-122">Bu kullanıcının bağlantıyı seçmesini ve satıcı ilişki isteğini onaylaması gerekir.</span><span class="sxs-lookup"><span data-stu-id="f2f85-122">That user needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Satıcı ilişkisi":::

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a><span data-ttu-id="f2f85-124">Yönetici aracıları grubunu Azure CSP aboneliğine sahip olarak ekleme</span><span class="sxs-lookup"><span data-stu-id="f2f85-124">Adding the admin agents group as an owner for the Azure CSP subscription</span></span>

<span data-ttu-id="f2f85-125">Müşterinizin, Azure CSP Aboneliğinin sahibi olarak Yönetim Aracısı grubunuzu eklemesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="f2f85-125">Your customer will need to add your admin agent group as the owner of the Azure CSP subscription.</span></span>

1. <span data-ttu-id="f2f85-126">PowerShell konsolunu veya PowerShell Tümleşik komut dosyası ortamı 'nı (ıSE) kullanın.</span><span class="sxs-lookup"><span data-stu-id="f2f85-126">Use either PowerShell Console or PowerShell Integrated Scripting Environment(ISE).</span></span> <span data-ttu-id="f2f85-127">AzureAD modüllerinin yüklü olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="f2f85-127">Ensure that AzureAD modules are installed.</span></span>

2. <span data-ttu-id="f2f85-128">Azure AD Kiracınıza bağlanın.</span><span class="sxs-lookup"><span data-stu-id="f2f85-128">Connect to your Azure AD Tenant.</span></span>

   ```powershell
   Connect-AzureAD
   ```

3. <span data-ttu-id="f2f85-129">Yönetici aracıları gruplarının ObjectID 'sini alın.</span><span class="sxs-lookup"><span data-stu-id="f2f85-129">Get ObjectId of the Admin Agents groups.</span></span>

   ```powershell
   Get-AzureADGroup
   ```
   <span data-ttu-id="f2f85-130">Aşağıdaki adımlar, Azure CSP aboneliğine sahip erişimi olan müşterinizin şirketindeki Kullanıcı tarafından gerçekleştirilir.</span><span class="sxs-lookup"><span data-stu-id="f2f85-130">The following steps are performed by the user in your customer's company who has owner access to the Azure CSP subscription.</span></span>

4. <span data-ttu-id="f2f85-131">Azure CSP aboneliğine sahip erişimi olan Kullanıcı, kimlik bilgilerini kullanarak Azure 'da oturum açar.</span><span class="sxs-lookup"><span data-stu-id="f2f85-131">The user with owner access to the Azure CSP subscription, signs into Azure using her credentials.</span></span>

   ```powershell
   Connect-AzAccount
   ```

5. <span data-ttu-id="f2f85-132">Daha sonra, CSP Azure aboneliğine yönetici aracı grubunuzu sahip olarak ekleyebilir.</span><span class="sxs-lookup"><span data-stu-id="f2f85-132">She can then add your admin agent group as owner to the CSP Azure subscription.</span></span>

    ```powershell
    New-AzureRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"
    ```

## <a name="next-steps"></a><span data-ttu-id="f2f85-133">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="f2f85-133">Next steps</span></span>

[<span data-ttu-id="f2f85-134">Azure planı kapsamındaki abonelikleri ve kaynakları yönetme</span><span class="sxs-lookup"><span data-stu-id="f2f85-134">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
