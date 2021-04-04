---
title: Dynamics 365 Business Edition 'ı geçirme
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Uygun Dynamics 365 Business Edition tekliflerini, kullanım süreleri dolmadan önce daha yeni sürümlere geçirmeyi öğrenin.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e83c06c11638bdde508fd27904038bcb6d8c9e9c
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132647"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="1022e-103">Dynamics 365 Business Edition Tekliflerini daha yeni sürümlere geçirme</span><span class="sxs-lookup"><span data-stu-id="1022e-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="1022e-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="1022e-104">**Appropriate roles**</span></span>

- <span data-ttu-id="1022e-105">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="1022e-105">Global admin</span></span>
- <span data-ttu-id="1022e-106">Kullanıcı Yönetimi Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="1022e-106">User management admin</span></span>
- <span data-ttu-id="1022e-107">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="1022e-107">Admin agent</span></span>
- <span data-ttu-id="1022e-108">Satış Aracısı</span><span class="sxs-lookup"><span data-stu-id="1022e-108">Sales agent</span></span>

<span data-ttu-id="1022e-109">1 Ocak 2019 ' den itibaren, Dynamics 365 Business Edition aboneliklerine sahip müşteriler artık bu eski tekliflere yenilemez; mevcut abonelikler, süreleri dolduğunda otomatik olarak yenilenmeyecektir.</span><span class="sxs-lookup"><span data-stu-id="1022e-109">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="1022e-110">Aboneliğin ayrıntı sayfasında, abonelik durumu "otomatik yenilemede [Tarih]" içinden "süresi doluyor" olarak değişir.</span><span class="sxs-lookup"><span data-stu-id="1022e-110">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="1022e-111">Müşterilerin devamlılığını sağlamak için, süresi dolan aboneliklerle birlikte aşağıda listelenen desteklenen bir seçeneğe geçiş yapmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="1022e-111">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="1022e-112">Müşterilerin hizmet kesintilerinden kaçınmak için, aboneliğin yıllık bitiş tarihinden önce müşterileri yeni aboneliklere taşımayı öneririz.</span><span class="sxs-lookup"><span data-stu-id="1022e-112">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="1022e-113">API 'YI (CREST veya Partner Center) kullanıyorsanız, Otomatik Yenile = false özelliğiyle birlikte Aboneliğin bitiş tarihini değerlendirerek süresi dolan abonelikleri bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1022e-113">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="1022e-114">Söz konusu abonelikler, 1 Ocak 2019 tarihinde otomatik olarak Yenile = false olarak ayarlanacak.</span><span class="sxs-lookup"><span data-stu-id="1022e-114">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="1022e-115">Müşterileri dilediğiniz zaman yeni bir plana taşıyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1022e-115">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="1022e-116">Kullanımdan kalkmakta olan Dynamics 365 Iş sürümleri</span><span class="sxs-lookup"><span data-stu-id="1022e-116">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="1022e-117">Finans ve Işlemler için Dynamics 365, Iş sürümü</span><span class="sxs-lookup"><span data-stu-id="1022e-117">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="1022e-118">Ekip üyeleri için Dynamics 365, Iş sürümü</span><span class="sxs-lookup"><span data-stu-id="1022e-118">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="1022e-119">Dynamics Business Central-Dynamics 365 Business Edition yeni teklifleri</span><span class="sxs-lookup"><span data-stu-id="1022e-119">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="1022e-120">Yeni Dynamics Business merkezi teklifleriyle, müşterileriniz, iş süreçlerini kolaylaştırmak, müşteri etkileşimlerini geliştirmek ve daha iyi kararlar almak için mali bilgilerini, satışları, servis ve işlemlerini birbirine bağlayabilirler.</span><span class="sxs-lookup"><span data-stu-id="1022e-120">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="1022e-121">Dynamics 365 Business Central, bulut tabanlı ve yalnızca bulut çözümü sağlayıcısı (CSP) program iş ortakları aracılığıyla kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="1022e-121">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="1022e-122">Dynamics 365 Business Edition müşterileri, 30 Haziran 2020 ' e kadar yeni Iş Merkezi teklifleri için indirimli geçiş fiyatlandırması almaya uygundur.</span><span class="sxs-lookup"><span data-stu-id="1022e-122">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="1022e-123">Müşterilerin yeni ürün planlarına geçişini sağlar</span><span class="sxs-lookup"><span data-stu-id="1022e-123">Transition customers to new product plans</span></span>

 <span data-ttu-id="1022e-124">Müşterileri kullanımdan kaldırılan SKU 'lardan daha yeni bir sürümüne taşımak, bu sırayla aşağıdaki adımları gerektirir:</span><span class="sxs-lookup"><span data-stu-id="1022e-124">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="1022e-125">Yeni aboneliği satın alın</span><span class="sxs-lookup"><span data-stu-id="1022e-125">Purchase the new subscription</span></span>
- <span data-ttu-id="1022e-126">Geçerli kullanıcı lisanslarını yeniden ata</span><span class="sxs-lookup"><span data-stu-id="1022e-126">Reassign current user licenses</span></span>
- <span data-ttu-id="1022e-127">Eski aboneliği iptal et</span><span class="sxs-lookup"><span data-stu-id="1022e-127">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="1022e-128">Müşteriniz için yeni planı satın alın</span><span class="sxs-lookup"><span data-stu-id="1022e-128">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="1022e-129">Sol gezinti bölmesinde **müşteriler** ' i seçin ve sonra yeni aboneliğe taşımak istediğiniz müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="1022e-129">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="1022e-130">**Abonelik Ekle**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="1022e-130">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="1022e-131">Katalogdan satın almak istediğiniz aboneliği seçin (Bu durumda yukarıdaki seçeneklerden biri), lisansların sayısını girin ve ardından **Gönder**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="1022e-131">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="1022e-132">Müşterinizin artık hem eski hem de yeni bir abonelik olacak.</span><span class="sxs-lookup"><span data-stu-id="1022e-132">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="1022e-133">Bir sonraki adımınız, lisansları müşterinin kullanıcılarına yeniden atamak olur.</span><span class="sxs-lookup"><span data-stu-id="1022e-133">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="1022e-134">Sol gezinti çubuğunda **müşteriler** ' i seçin ve ardından taşıdığınız müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="1022e-134">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="1022e-135">**Kullanıcılar ve lisanslar ' ı** seçin.</span><span class="sxs-lookup"><span data-stu-id="1022e-135">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="1022e-136">Bir kullanıcıya bir lisansı yeniden atamak için kullanıcıyı seçin ve ardından **Lisansları Yönet**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="1022e-136">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="1022e-137">**Lisansları Yönet** sayfasında, temel (nitelikli teklif) lisanstan satış/müşteri katılım planı için Dynamics 365 ' i temizleyin ve müşterinin taşınmakta olduğu abonelik için yeni bir hizmet planı seçin.</span><span class="sxs-lookup"><span data-stu-id="1022e-137">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="1022e-138">**Gönder**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="1022e-138">Select **Submit**.</span></span> <span data-ttu-id="1022e-139">Bunu, yeni lisansa ihtiyacı olan her kullanıcı için yapabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1022e-139">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="1022e-140">Lisansları yeni aboneliğe taşındıktan sonra eski aboneliği iptal edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1022e-140">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="1022e-141">Sol gezinti çubuğunda **müşteriler** ' i seçin ve ardından taşıdığınız müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="1022e-141">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="1022e-142">Abonelik Ayrıntıları sayfasında, eski aboneliği **askıya alındı** olarak ayarlayın ve **Gönder**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="1022e-142">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="1022e-143">Eski abonelik artık askıya alındı ve yeni abonelik etkin.</span><span class="sxs-lookup"><span data-stu-id="1022e-143">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="1022e-144">Askıya alınan abonelik 120 gün sonra otomatik olarak sağlanacaktır.</span><span class="sxs-lookup"><span data-stu-id="1022e-144">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="1022e-145">Müşterinizin eski abonelik için ek ücret ödemeyecektir.</span><span class="sxs-lookup"><span data-stu-id="1022e-145">Your customer will incur no additional costs for the old subscription.</span></span>
