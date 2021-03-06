---
title: Azure Iş ortağı paylaşılan hizmetleri ekleme
description: Azure Iş ortağı paylaşılan hizmetleri 'ni kullanarak kendi kullanım için Azure abonelikleri satın alın ve Azure 'u satın alma, izleme ve yönetmeye yönelik Tekdüzen bir yönteme sahip olun.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: a59cf0b271a0ccf5fd5a1d8e3e85ff43818a3801
ms.sourcegitcommit: fe867be44de3479607be3309940b904d7ea9fc6e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/06/2021
ms.locfileid: "102247714"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a><span data-ttu-id="8a2f5-103">Azure Iş ortağı paylaşılan hizmetleri 'ni ekleyerek iş ortaklarının kendi kullanımları için Azure abonelikleri satın alabilir</span><span class="sxs-lookup"><span data-stu-id="8a2f5-103">Add Azure Partner Shared Services so partners can buy Azure subscriptions for their own use</span></span>

 
<span data-ttu-id="8a2f5-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="8a2f5-104">**Appropriate roles**</span></span>

- <span data-ttu-id="8a2f5-105">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="8a2f5-105">Global admin</span></span>
- <span data-ttu-id="8a2f5-106">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="8a2f5-106">Admin agent</span></span>
- <span data-ttu-id="8a2f5-107">Satış Aracısı</span><span class="sxs-lookup"><span data-stu-id="8a2f5-107">Sales agent</span></span>

<span data-ttu-id="8a2f5-108">Azure Iş ortağı paylaşılan hizmetleri, iş ortaklarının Azure aboneliklerini kendi kullanımları için satın almasını sağlayan CSP programındaki iş ortakları için yeni bir teklif türüdür.</span><span class="sxs-lookup"><span data-stu-id="8a2f5-108">Azure Partner Shared Services is a new offer type for partners in the CSP program enabling partners to purchase Azure subscriptions for their own use.</span></span><span data-ttu-id="8a2f5-109">İş ortaklarının Azure lisanslarını birleştirme ve Microsoft ile yeniden satma yeteneğine ek olarak Azure 'u satın almak, izlemek ve yönetmek için Tekdüzen bir yöntem kullanması için bir fırsat oluşturur.</span><span class="sxs-lookup"><span data-stu-id="8a2f5-109">  It creates the opportunity for partners to use a uniform method for purchasing, tracking, and managing Azure in addition to the ability to consolidate their Azure licensing and reselling agreements with Microsoft.</span></span> <span data-ttu-id="8a2f5-110">Azure Iş ortağı paylaşılan hizmetleri sayesinde iş ortakları artık Microsoft Kurumsal Anlaşma ve web doğrudan programlarında olduğu gibi CSP 'de Azure aboneliklerini kullanmak için aynı esnekliğe sahiptir: geliştirme ve test ortamları oluşturma, iç iş yüklerini dağıtma ve paylaşılan hizmetleri veya çok kiracılı uygulamaları barındırma.</span><span class="sxs-lookup"><span data-stu-id="8a2f5-110">With Azure Partner Shared Services, partners now have the same flexibility to use Azure subscriptions in CSP as they do in the Microsoft Enterprise Agreement and Web Direct programs, opening up scenarios such as:  build development and test environments, deploy internal workloads, and host shared services or multi-tenant applications.</span></span>  

## <a name="create-the-shared-services-tenant"></a><span data-ttu-id="8a2f5-111">Paylaşılan hizmetler kiracısını oluşturma</span><span class="sxs-lookup"><span data-stu-id="8a2f5-111">Create the shared services tenant</span></span>

1. <span data-ttu-id="8a2f5-112">**Ayarlar**  >  **Hesap ayarları**  >  **paylaşılan hizmetler**' e gidin.</span><span class="sxs-lookup"><span data-stu-id="8a2f5-112">Go to **Settings** > **Account settings** > **Shared services**.</span></span>

   :::image type="content" source="images/sharedservices2.png" alt-text="Hesap ayarları > paylaşılan hizmetler":::

2. <span data-ttu-id="8a2f5-114">Zaten bir paylaşılan hizmetler kiracınız yoksa, **paylaşılan hizmetler oluştur**' a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="8a2f5-114">If you don't already have a shared services tenant, click **Create shared services**.</span></span>

   :::image type="content" source="images/sharedservices3.png" alt-text="Paylaşılan hizmetler oluştur":::

3. <span data-ttu-id="8a2f5-116">Bu, paylaşılan kaynaklar ve iç iş yükü için kullanılmak üzere paylaşılan bir hizmet kiracısı oluşturur ve Azure CSP paylaşılan hizmetleri aboneliğini satın alır.</span><span class="sxs-lookup"><span data-stu-id="8a2f5-116">This creates a shared services tenant and purchases the Azure CSP Shared Services subscription, to be used for shared resources and internal workload.</span></span>

   :::image type="content" source="images/sharedservices5.png" alt-text="Kiracıyı oluşturma ve aboneliği satın alma":::

## <a name="about-the-azure--internalshared-services-offer"></a><span data-ttu-id="8a2f5-118">Azure Dahili/Paylaşılan Hizmetler teklifi hakkında</span><span class="sxs-lookup"><span data-stu-id="8a2f5-118">About the Azure- Internal/Shared Services offer</span></span>

- <span data-ttu-id="8a2f5-119">Azure Dahili/Paylaşılan Hizmetler aboneliği, iş ortaklarının kendi Azure kullanımlarını aldığı Iş Ortağı Merkezi aracılığıyla erişilebilen CSP 'de yeni bir Azure teklif türüdür.</span><span class="sxs-lookup"><span data-stu-id="8a2f5-119">The Azure - Internal/Shared Services subscription is a new Azure offer type in CSP accessed through Partner Center that partners get for their own use of Azure.</span></span>

- <span data-ttu-id="8a2f5-120">Azure Iş ortağı paylaşılan hizmetleri abonelikleri uygun ve RIS satın almak için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="8a2f5-120">Azure Partner Shared Services subscriptions are eligible and can be used to purchase RIs.</span></span>

- <span data-ttu-id="8a2f5-121">Azure Dahili/Paylaşılan Hizmetler teklif yalnızca paylaşılan hizmetler kiracısına uygulanabilir.</span><span class="sxs-lookup"><span data-stu-id="8a2f5-121">The Azure - Internal/Shared Services offer can only be applied to the shared services tenant.</span></span>

- <span data-ttu-id="8a2f5-122">Azure Dahili/Paylaşılan Hizmetler aboneliğin birincil kullanımı, kendi geliştirme amaçlarınız için Azure 'ı kullanabilmeniz için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="8a2f5-122">The primary use for the Azure - Internal/Shared Services subscription is so that you can use Azure for your own development purposes.</span></span> <span data-ttu-id="8a2f5-123">Bu teklifi sağlamak için kullandığınız paylaşılan kiracı, Office 365 veya Dynamics lisansları gibi diğer hizmetler için kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="8a2f5-123">The shared tenant you use to provision this offer cannot be used for other services such as Office 365 or Dynamics licenses.</span></span>

- <span data-ttu-id="8a2f5-124">Aboneliği diğer abonelikler gibi iptal edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8a2f5-124">You can cancel the subscription like any other subscription.</span></span> <span data-ttu-id="8a2f5-125">**Ayarlar**  >  **Tüm ayarlar**  >  **paylaşılan hizmetleri**' ne bakın.</span><span class="sxs-lookup"><span data-stu-id="8a2f5-125">Go to the **settings** > **View all settings** > **Shared services**.</span></span> <span data-ttu-id="8a2f5-126">Azure Dahili/Paylaşılan Hizmetler aboneliğini seçin ve iptal edin.</span><span class="sxs-lookup"><span data-stu-id="8a2f5-126">Select the Azure - Internal/Shared Services subscription and cancel it.</span></span>

## <a name="accessing-azure-partner-shared-services-consumption-details"></a><span data-ttu-id="8a2f5-127">Azure Iş ortağı paylaşılan hizmetleri tüketim ayrıntılarına erişme</span><span class="sxs-lookup"><span data-stu-id="8a2f5-127">Accessing Azure Partner Shared Services consumption details</span></span>

<span data-ttu-id="8a2f5-128">Azure kullanımını CSP faturanızda ve mutabakat dosyasında bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8a2f5-128">You will find the Azure consumption on your CSP invoice and the reconciliation file.</span></span> <span data-ttu-id="8a2f5-129">Faturaya Microsoft Azure satırı öğesinin bir parçası olarak dahil edilir.</span><span class="sxs-lookup"><span data-stu-id="8a2f5-129">It will be included as part of Microsoft Azure line item in the invoice.</span></span> <span data-ttu-id="8a2f5-130">Ayrıntılı tüketim bilgileri, bu teklif için oluşturulan kiracıya yönelik olarak günlüğe kaydedilen mutabakat dosyasında kullanıma sunulacaktır.</span><span class="sxs-lookup"><span data-stu-id="8a2f5-130">The detailed consumption information will be available in the reconciliation file logged against the tenant that was created for this offer.</span></span>

## <a name="azure-partner-shared-services-pricing"></a><span data-ttu-id="8a2f5-131">Azure Iş ortağı Paylaşılan Hizmetleri Fiyatlandırması</span><span class="sxs-lookup"><span data-stu-id="8a2f5-131">Azure Partner Shared Services pricing</span></span>

<span data-ttu-id="8a2f5-132">Azure iş ortağı paylaşılan hizmetleri için yeni fiyatlandırma dosyasını görmek için   >  **fiyatlandırma ve teklifleri** satma bölümüne gidin ve geçerli ayın fiyat listesini seçin.</span><span class="sxs-lookup"><span data-stu-id="8a2f5-132">To see the new pricing file for Azure Partner Shared Services go to **Sell** > **Pricing and offers** and select the current month's price list.</span></span> <span data-ttu-id="8a2f5-133">Önümüzdeki haftalarda, belirli bir ücret kartı API 'si de yayımlanır.</span><span class="sxs-lookup"><span data-stu-id="8a2f5-133">In the coming weeks, a specific rate card api will also be released.</span></span>

## <a name="marketplace-offers-and-azure-partner-shared-services"></a><span data-ttu-id="8a2f5-134">Market teklifleri ve Azure Iş ortağı paylaşılan hizmetleri</span><span class="sxs-lookup"><span data-stu-id="8a2f5-134">Marketplace offers and Azure Partner Shared Services</span></span>

<span data-ttu-id="8a2f5-135">Azure Iş ortağı paylaşılan hizmetleri (APSS), 1 Mart 2019 itibariyle artık Market tekliflerini desteklememektedir.</span><span class="sxs-lookup"><span data-stu-id="8a2f5-135">As of March 1, 2019, Azure Partner Shared Services (APSS) no longer supports Marketplace offers.</span></span>

|<span data-ttu-id="8a2f5-136">**Market desteği**</span><span class="sxs-lookup"><span data-stu-id="8a2f5-136">**Marketplace support**</span></span>   |<span data-ttu-id="8a2f5-137">**APSS, 1 Mart 2019 ' den önce destekleniyor**</span><span class="sxs-lookup"><span data-stu-id="8a2f5-137">**APSS supported before March 1, 2019**</span></span>|<span data-ttu-id="8a2f5-138">**1 Mart 2019 ' den sonra**</span><span class="sxs-lookup"><span data-stu-id="8a2f5-138">**After March 1, 2019**</span></span>|
|---------------------------|:----------------------------|:-------------------|
|<span data-ttu-id="8a2f5-139">Kendi lisansınızı getirin (KLG) ve ücretsiz hizmetler</span><span class="sxs-lookup"><span data-stu-id="8a2f5-139">Bring your own license (BYOL) and free services</span></span>   | <span data-ttu-id="8a2f5-140">Yes</span><span class="sxs-lookup"><span data-stu-id="8a2f5-140">Yes</span></span>   | <span data-ttu-id="8a2f5-141">Hayır</span><span class="sxs-lookup"><span data-stu-id="8a2f5-141">No</span></span>|
|<span data-ttu-id="8a2f5-142">Diğer üçüncü taraf Market teklifleri</span><span class="sxs-lookup"><span data-stu-id="8a2f5-142">Other third-party marketplace offers</span></span>   | <span data-ttu-id="8a2f5-143">Hayır</span><span class="sxs-lookup"><span data-stu-id="8a2f5-143">No</span></span>   |<span data-ttu-id="8a2f5-144">Hayır</span><span class="sxs-lookup"><span data-stu-id="8a2f5-144">No</span></span>|

<span data-ttu-id="8a2f5-145">APSS kullanılarak dağıtılan KLG veya ücretsiz hizmetleri olan iş ortakları bundan etkilenmez; Ancak, 1 Mart 2019 ' den sonra yeni KLG veya ücretsiz hizmetler satın amazlar.</span><span class="sxs-lookup"><span data-stu-id="8a2f5-145">Partners who have BYOL or free services deployed using APSS will not be impacted; however after March 1, 2019 they will not be able to purchase new BYOL or free services.</span></span>

<span data-ttu-id="8a2f5-146">Market tekliflerinin (yalnızca KLG ve ücretsiz hizmetler değil) tam kataloğundan faydalanmak için, CSP iş ortaklarının Web doğrudan Azure abonelikleri kullanarak paylaşılan hizmetleri dağıtmalarını öneririz.</span><span class="sxs-lookup"><span data-stu-id="8a2f5-146">To take advantage of the full catalog of Marketplace offers available (not just BYOL and free services), we recommend CSP partners deploy shared services using web direct Azure subscriptions.</span></span>  <span data-ttu-id="8a2f5-147">Daha önce Market 'ten üçüncü taraf KLG ve ücretsiz hizmet kaynakları dağıtmış olan CSP iş ortakları ve bunları kullanmaya devam etmek ve daha fazla üçüncü taraf teklifi dağıtmak, APSS aboneliğini [mevcut Azure aboneliklerinin doğrudan geçişine](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)Web 'e geçirmeye önerilir.</span><span class="sxs-lookup"><span data-stu-id="8a2f5-147">CSP partners who have deployed third-party BYOL and free service resources from the Marketplace previously and wish to continue using them and deploy more third-party offerings are encouraged to migrate the APSS subscription to web direct [Migrating Existing Azure Subscriptions](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).</span></span>

<span data-ttu-id="8a2f5-148">İş ortakları, 1 Mart 2019 ' den sonra APSS aboneliğini kullanmaya devam etmeyi planlıyor ve yeni üçüncü taraf [KLG hizmetlerini](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) veya ücretsiz hizmetleri dağıtmak istiyor. BUNLARı APSS aboneliklerine dağıtmak için ISV 'lerden gelen yönergeleri uygulayabilir.</span><span class="sxs-lookup"><span data-stu-id="8a2f5-148">Partners, who plan to continue using APSS subscription after the March 1, 2019 and wish to deploy new third-party [BYOL services](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) or free services, can follow the instructions from ISVs to deploy these to their APSS subscriptions.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8a2f5-149">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="8a2f5-149">Next steps</span></span>

- [<span data-ttu-id="8a2f5-150">CSP üzerinden yazılım aboneliği satma</span><span class="sxs-lookup"><span data-stu-id="8a2f5-150">Sell software subscriptions through CSP</span></span>](csp-software-subscriptions.md)