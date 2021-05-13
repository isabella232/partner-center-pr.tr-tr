---
title: Kısıtlanmış doğrudan fatura özellikleri
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP doğrudan fatura ortağı gereksinimleri hakkında bilgi edinin ve yeteneklerin kısıtlanmasını önlemek için ne yapmanız gerektiğini öğrenin. Olanaklarınızın kısıtlanıp kısıtlanmayacağını öğrenin.
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b3b1f3e1593f7e35bd3b9ed6c56ea28683bff95a
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855497"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a><span data-ttu-id="9fe33-104">Kısıtlanmış doğrudan fatura özellikleri ve CSP doğrudan fatura ortakları için gereken gereksinimler</span><span class="sxs-lookup"><span data-stu-id="9fe33-104">Restricted direct bill capabilities and the requirements needed for CSP direct bill partners</span></span>

<span data-ttu-id="9fe33-105">**Uygun roller**: genel yönetici</span><span class="sxs-lookup"><span data-stu-id="9fe33-105">**Appropriate roles**: Global admin</span></span>

## <a name="overview"></a><span data-ttu-id="9fe33-106">Genel Bakış</span><span class="sxs-lookup"><span data-stu-id="9fe33-106">Overview</span></span>

<span data-ttu-id="9fe33-107">Doğrudan fatura ortakları, CSP doğrudan fatura ortağı programında kalacak yeni [gereksinimleri](direct-partner-new-requirements.md) karşılamalıdır.</span><span class="sxs-lookup"><span data-stu-id="9fe33-107">Direct bill partners must meet the new [requirements](direct-partner-new-requirements.md) to remain in the CSP direct bill partner program.</span></span> <span data-ttu-id="9fe33-108">Aksi takdirde, doğrudan fatura özelliklerine erişimleri bu süre sonunda kısıtlanmıştır ve müşterileri için yeni satın alma işlemleri gibi belirli görevleri daha fazla gerçekleştirebilir.</span><span class="sxs-lookup"><span data-stu-id="9fe33-108">Otherwise, their access to direct bill capabilities will eventually be restricted and can longer perform specific tasks, such as making new purchases for their customers.</span></span>

> [!Note]
> <span data-ttu-id="9fe33-109">CSP doğrudan fatura iş ortağı programı için yeni gereksinimleri karşılamayan doğrudan fatura ortakları, doğrudan fatura özellikleri sınırlandırılacağı zaman Microsoft tarafından bilgilendirilir.</span><span class="sxs-lookup"><span data-stu-id="9fe33-109">Direct bill partners who do not meet the new requirements for CSP direct bill partner program will be informed by Microsoft when their direct bill capabilities will be restricted.</span></span> <span data-ttu-id="9fe33-110">Bu, [doğrudan fatura ortağından dolaylı satıcılara geçiş](transition-direct-to-indirect.md) yapılıp yapılmayacağını kabul etmeksizin tüm doğrudan fatura ortakları için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="9fe33-110">This applies to all direct bill partners, whether they have opted for [transition from direct bill partner to indirect resellers](transition-direct-to-indirect.md) or not.</span></span>  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a><span data-ttu-id="9fe33-111">Doğrudan fatura olanaklarınızın kısıtlanmasını nasıl söylüyorsunuz</span><span class="sxs-lookup"><span data-stu-id="9fe33-111">How to tell if your direct bill capabilities has been restricted</span></span>

<span data-ttu-id="9fe33-112">Doğrudan fatura ortağı kiracısından doğrudan fatura özelliklerine erişimin kısıtlanıp kısıtlanmadığını doğrulamak için aşağıdaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="9fe33-112">To confirm whether access from the direct bill partner tenant to direct bill capabilities has been restricted, follow these steps.</span></span>

1. <span data-ttu-id="9fe33-113">[İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="9fe33-113">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="9fe33-114">**Hesap ayarları**  ->  **yasal profili**' ne gidin.</span><span class="sxs-lookup"><span data-stu-id="9fe33-114">Go to **Account settings** -> **Legal Profile**.</span></span>

3. <span data-ttu-id="9fe33-115">**Program bilgileri** altında **Microsoft bulut çözüm sağlayıcısı durumunu** arayın.</span><span class="sxs-lookup"><span data-stu-id="9fe33-115">Under **Program info**, look for **Microsoft Cloud Solution Provider status**.</span></span>

4. <span data-ttu-id="9fe33-116">Program durumunun **kısıtlı** değeri varsa, doğrudan fatura iş ortağı kiracının doğrudan fatura özelliklerine erişiminin kısıtlandığı anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="9fe33-116">If the program status has value **restricted**, it means that your direct bill partner tenant's access to direct bill capabilities has been restricted.</span></span>

## <a name="affected-direct-bill-capabilities"></a><span data-ttu-id="9fe33-117">Etkilenen doğrudan fatura özellikleri</span><span class="sxs-lookup"><span data-stu-id="9fe33-117">Affected direct bill capabilities</span></span>

<span data-ttu-id="9fe33-118">Doğrudan fatura olanaklarınız kısıtlanmışsa, Iş Ortağı Merkezi 'nde müşterileriniz için artık yeni satın alma işlemleri yapamamaktadır.</span><span class="sxs-lookup"><span data-stu-id="9fe33-118">If your direct bill capabilities have been restricted, you can no longer make new purchases for your customers in Partner Center.</span></span> <span data-ttu-id="9fe33-119">Bu kısıtlama şunları içerir:</span><span class="sxs-lookup"><span data-stu-id="9fe33-119">This restriction includes:</span></span>

- <span data-ttu-id="9fe33-120">Azure abonelikleri</span><span class="sxs-lookup"><span data-stu-id="9fe33-120">Azure subscriptions</span></span>

- <span data-ttu-id="9fe33-121">Lisans tabanlı abonelikler</span><span class="sxs-lookup"><span data-stu-id="9fe33-121">License-based subscriptions</span></span>

- <span data-ttu-id="9fe33-122">Mevcut lisans tabanlı aboneliklere yeni eklentiler ekleyin.</span><span class="sxs-lookup"><span data-stu-id="9fe33-122">Add new add-ons to existing license-based subscriptions.</span></span>

- <span data-ttu-id="9fe33-123">Yazılım ve rezervasyon ürünlerini tek seferlik satın alma (örneğin, yazılım abonelikleri, kalıcı yazılım ve Azure ayrılmış sanal makine örnekleri) yapın.</span><span class="sxs-lookup"><span data-stu-id="9fe33-123">Make one-time purchases of software and reservation products (for example, software subscriptions, perpetual software, and Azure Reserved Virtual Machine instances).</span></span>

<span data-ttu-id="9fe33-124">Kendi kullanımınız için yeni [Azure abonelikleri satın almak için](shared-services.md) CSP programı kapsamındaki Azure iş ortağı paylaşılan hizmetleri teklifini de kullanamazsınız.</span><span class="sxs-lookup"><span data-stu-id="9fe33-124">You also cannot use the [Azure partner shared services offer](shared-services.md) under the CSP program to purchase new Azure subscriptions for your own use.</span></span>

<span data-ttu-id="9fe33-125">Mevcut doğrudan fatura abonelikleri etkilenmez.</span><span class="sxs-lookup"><span data-stu-id="9fe33-125">Existing direct bill subscriptions are not affected.</span></span> <span data-ttu-id="9fe33-126">Bunlar geçerli kalır ve otomatik olarak yeniler.</span><span class="sxs-lookup"><span data-stu-id="9fe33-126">They remain valid and are auto-renewed.</span></span> <span data-ttu-id="9fe33-127">İptal edilene kadar doğrudan Microsoft tarafından faturalandır olmaya devam edersiniz.</span><span class="sxs-lookup"><span data-stu-id="9fe33-127">You will continue to be billed directly by Microsoft until they are canceled.</span></span> <span data-ttu-id="9fe33-128">Mevcut abonelikleri yönetmek için aşağıdaki yöntemleri kullanabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="9fe33-128">You can still manage existing subscriptions in the following ways:</span></span>

- <span data-ttu-id="9fe33-129">Mevcut abonelikleri askıya alma</span><span class="sxs-lookup"><span data-stu-id="9fe33-129">Suspend existing subscriptions</span></span>

- <span data-ttu-id="9fe33-130">Mevcut lisans tabanlı aboneliklerin lisans sayısını ayarlama</span><span class="sxs-lookup"><span data-stu-id="9fe33-130">Adjust license count of existing license-based subscriptions</span></span>

- <span data-ttu-id="9fe33-131">Bir aboneliğe yapılan mevcut eklentilerin lisans sayısını ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="9fe33-131">Adjust license count of existing add-ons to a subscription.</span></span> 

    >[!Note]
    ><span data-ttu-id="9fe33-132">Yeni satın alma olarak kabul edilen mevcut aboneliklere yeni eklentiler ek olamazsınız.</span><span class="sxs-lookup"><span data-stu-id="9fe33-132">You cannot add new add-ons to existing subscriptions as it is treated as new purchase.</span></span>

- <span data-ttu-id="9fe33-133">Yeni Azure kaynaklarını dağıtın ve mevcut Azure kaynaklarını mevcut Azure abonelikleri altında yönetin.</span><span class="sxs-lookup"><span data-stu-id="9fe33-133">Deploy new Azure resources and manage existing Azure resources under existing Azure subscriptions.</span></span> <span data-ttu-id="9fe33-134">Bu, Azure Market ve Visual Studio içerir.</span><span class="sxs-lookup"><span data-stu-id="9fe33-134">This includes resources, which are available through Azure Marketplace and Visual Studio subscriptions.</span></span>

<span data-ttu-id="9fe33-135">Yeni satın almalara ek olarak, aşağıdaki doğrudan fatura özelliklerine de İş Ortağı Merkezi:</span><span class="sxs-lookup"><span data-stu-id="9fe33-135">In addition to new purchases, you cannot access the following direct bill capabilities in Partner Center:</span></span>

- <span data-ttu-id="9fe33-136">Yeni müşteri kiracıları oluşturamazsiniz.</span><span class="sxs-lookup"><span data-stu-id="9fe33-136">You cannot create new customer tenants.</span></span> <span data-ttu-id="9fe33-137">Müşteriler **sayfasındaki** Müşteriler **sayfasında** müşteri İş Ortağı Merkezi seçeneği kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="9fe33-137">The **Create customer** option under **Customers** page in Partner Center will not be available.</span></span>

- <span data-ttu-id="9fe33-138">Doğrudan kurumsal bayi ilişkisi isteğine davet oluşturamazsiniz.</span><span class="sxs-lookup"><span data-stu-id="9fe33-138">You cannot generate invitation to customer requesting for direct reseller relationship.</span></span> <span data-ttu-id="9fe33-139">Kurumsal **bayi ilişkisi isteğinde** **bulun sayfasındaki** Müşteriler İş Ortağı Merkezi seçeneği kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="9fe33-139">The **Request a reseller relationship** option under **Customers** page in Partner Center will not be available.</span></span>

    >[!NOTE]
    ><span data-ttu-id="9fe33-140">Doğrudan fatura iş ortağından dolaylı kurumsal bayiye geçişin bir parçası olarak, doğrudan fatura iş ortağı kiracınızı dolaylı kurumsal bayi olarak zaten kaydettiynize, bunun yerine dolaylı kurumsal bayi ilişkisi isteğine davet eden müşteriye davette bulunabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="9fe33-140">As part of transitioning from direct bill partner to indirect reseller, if you have already enrolled your direct bill partner tenant as indirect reseller, you can generate invitation to customer requesting for indirect reseller relationship instead.</span></span>

- <span data-ttu-id="9fe33-141">Yeni korumalı alan kiracısı oluşturamazsiniz.</span><span class="sxs-lookup"><span data-stu-id="9fe33-141">You cannot create new sandbox tenant.</span></span> <span data-ttu-id="9fe33-142">Her doğrudan fatura iş ortağı kiracısı, doğrudan fatura API'si tümleştirmesi için bir korumalı alan kiracısı oluşturabilir.</span><span class="sxs-lookup"><span data-stu-id="9fe33-142">Each direct bill partner tenant can create one sandbox tenant for direct bill API integration.</span></span> <span data-ttu-id="9fe33-143">Daha önce oluşturmadıysanız, doğrudan fatura iş ortağı özelliğiniz kısıtlandıktan sonra bunu yapma iznine sahip olmaznız.</span><span class="sxs-lookup"><span data-stu-id="9fe33-143">If you haven't created one previously, you are not allowed to do so after your direct bill partner capability has been restricted.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="9fe33-144">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="9fe33-144">Next steps</span></span>

- [<span data-ttu-id="9fe33-145">Dolaylı satıcı olma hakkında ek bilgiler</span><span class="sxs-lookup"><span data-stu-id="9fe33-145">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [<span data-ttu-id="9fe33-146">CSP doğrudan iş ortağı yeni gereksinimler</span><span class="sxs-lookup"><span data-stu-id="9fe33-146">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)
