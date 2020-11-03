---
title: Nitelikli Dynamics 365 aboneliklerini geçirme
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Mevcut aboneliklerin süre dolmadan önce nitelikli, temel Dynamics 365 aboneliklerinden yeni bir aboneliğe nasıl geçiş yapılacağını öğrenin.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8575d87ab3c4c7970135a87b7ef7564c4fe06232
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/17/2020
ms.locfileid: "92531007"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="f7043-103">Dynamics 365 ve Müşteri Etkileşimi Planı’nı Temel’den (uygun teklifler) daha yeni sürümlere geçirme</span><span class="sxs-lookup"><span data-stu-id="f7043-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="f7043-104">**Uygulama hedefi**</span><span class="sxs-lookup"><span data-stu-id="f7043-104">**Applies to**</span></span>

-  <span data-ttu-id="f7043-105">İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="f7043-105">Partner Center</span></span>

<span data-ttu-id="f7043-106">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="f7043-106">**Appropriate roles**</span></span>
-   <span data-ttu-id="f7043-107">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="f7043-107">Global admin</span></span>
-   <span data-ttu-id="f7043-108">Kullanıcı yöneticisi</span><span class="sxs-lookup"><span data-stu-id="f7043-108">User admin</span></span>
-   <span data-ttu-id="f7043-109">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="f7043-109">Admin agent</span></span>
-   <span data-ttu-id="f7043-110">Satış Aracısı</span><span class="sxs-lookup"><span data-stu-id="f7043-110">Sales agent</span></span>

<span data-ttu-id="f7043-111">1 Ocak 2019 ' den itibaren, temel (nitelikli teklifler) aboneliklerden satış/müşteri katılım planı için Dynamics 365 olan müşteriler bu eski teklifleri artık yenilemez; mevcut abonelikler, süreleri dolduğunda otomatik olarak yenilenmeyecektir.</span><span class="sxs-lookup"><span data-stu-id="f7043-111">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="f7043-112">Aboneliğin ayrıntı sayfasında, abonelik durumu "otomatik yenilemede [Tarih]" içinden "süresi doluyor" olarak değişir.</span><span class="sxs-lookup"><span data-stu-id="f7043-112">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="f7043-113">Müşterilerin devamlılığını sağlamak için, süresi dolan aboneliklerle birlikte aşağıda listelenen desteklenen bir seçeneğe geçiş yapmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="f7043-113">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="f7043-114">Müşterilerin hizmet kesintilerinden kaçınmak için, aboneliğin yıllık bitiş tarihinden önce müşterileri yeni aboneliklere taşımayı öneririz.</span><span class="sxs-lookup"><span data-stu-id="f7043-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="f7043-115">API 'YI (CREST veya Partner Center) kullanıyorsanız, Otomatik Yenile = false özelliğiyle birlikte Aboneliğin bitiş tarihini değerlendirerek süresi dolan abonelikleri bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f7043-115">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="f7043-116">Söz konusu abonelikler, 1 Ocak 2019 ' de otomatik yenileme = false olarak ayarlanacak.</span><span class="sxs-lookup"><span data-stu-id="f7043-116">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="f7043-117">Müşterileri dilediğiniz zaman yeni bir plana taşıyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f7043-117">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="f7043-118">Dynamics 365, kullanımdan kalkmakta olan teklifleri</span><span class="sxs-lookup"><span data-stu-id="f7043-118">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="f7043-119">Sales Enterprise Edition CRMOL Basic (nitelikli teklif) için Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="f7043-119">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f7043-120">Fakülteler için Dynamics 365 for Sales Enterprise Edition CRMOL Basic (nitelikli teklif)</span><span class="sxs-lookup"><span data-stu-id="f7043-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f7043-121">Öğrenciler için Dynamics 365 for Sales Enterprise Edition CRMOL Basic (nitelikli teklif)</span><span class="sxs-lookup"><span data-stu-id="f7043-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f7043-122">Sales Enterprise Edition için Dynamics 365 (kamu fiyatlandırması) CRMOL temel (nitelikli teklif)</span><span class="sxs-lookup"><span data-stu-id="f7043-122">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f7043-123">CRM Basic için SA 'Dan Sales Enterprise Edition için Dynamics 365 (nitelikli teklif)</span><span class="sxs-lookup"><span data-stu-id="f7043-123">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f7043-124">Dynamics 365 for Sales Enterprise Edition for CRM Basic (uygun teklif) için ŞA</span><span class="sxs-lookup"><span data-stu-id="f7043-124">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f7043-125">Öğrenciler için Dynamics 365 for Sales Enterprise Edition for CRM Basic (nitelikli teklif)</span><span class="sxs-lookup"><span data-stu-id="f7043-125">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f7043-126">Dynamics 365 for Sales Enterprise Edition (kamu fiyatlandırması) için SA 'Dan CRM temel (nitelikli teklif)</span><span class="sxs-lookup"><span data-stu-id="f7043-126">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f7043-127">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (nitelikli teklif)</span><span class="sxs-lookup"><span data-stu-id="f7043-127">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f7043-128">Dynamics 365 for Sales Enterprise Add-On Edition for CRM Basic (uygun teklif)-Fakülteler</span><span class="sxs-lookup"><span data-stu-id="f7043-128">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f7043-129">Öğrenciler için Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (nitelikli teklif)</span><span class="sxs-lookup"><span data-stu-id="f7043-129">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f7043-130">Sales Enterprise Edition için Dynamics 365 (kamu fiyatlandırması) Add-On for CRM Basic (nitelikli teklif)</span><span class="sxs-lookup"><span data-stu-id="f7043-130">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f7043-131">Dynamics 365 müşteri katılımı planı Enterprise Edition CRMOL Basic (nitelikli teklif)</span><span class="sxs-lookup"><span data-stu-id="f7043-131">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f7043-132">Dynamics 365 müşteri katılımı planı Enterprise Edition (kamu fiyatlandırması) CRMOL temel (nitelikli teklif)</span><span class="sxs-lookup"><span data-stu-id="f7043-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f7043-133">Öğrenciler için Dynamics 365 müşteri katılımı planı Enterprise Edition CRMOL Basic (nitelikli teklif)</span><span class="sxs-lookup"><span data-stu-id="f7043-133">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f7043-134">Dynamics 365 müşteri katılımı planı, Fakülteler için Enterprise Edition CRMOL Basic (nitelikli teklif)</span><span class="sxs-lookup"><span data-stu-id="f7043-134">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f7043-135">Dynamics 365 müşteri katılımı planı CRM temel için SA 'Dan Enterprise Edition (nitelikli teklif)</span><span class="sxs-lookup"><span data-stu-id="f7043-135">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f7043-136">Dynamics 365 müşteri katılımı planı Enterprise Edition (kamu fiyatlandırması) için SA 'Dan CRM temel (nitelikli teklif)</span><span class="sxs-lookup"><span data-stu-id="f7043-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f7043-137">Dynamics 365 müşteri katılımı planı, öğrenciler için CRM Basic (nitelikli teklif) için SA 'Dan Enterprise Edition</span><span class="sxs-lookup"><span data-stu-id="f7043-137">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f7043-138">Dynamics 365 müşteri katılımı planı, Fakülteler için CRM Basic (nitelikli teklif) için SA 'Dan Enterprise Edition</span><span class="sxs-lookup"><span data-stu-id="f7043-138">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f7043-139">Dynamics 365 müşteri katılımı planı Add-On Enterprise Edition for CRM Basic (nitelikli teklif)</span><span class="sxs-lookup"><span data-stu-id="f7043-139">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f7043-140">Dynamics 365 müşteri katılımı planı Enterprise Edition (kamu fiyatlandırması) Add-On for CRM Basic (nitelikli teklif)</span><span class="sxs-lookup"><span data-stu-id="f7043-140">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f7043-141">Dynamics 365 müşteri katılımı planı öğrenciler için Enterprise Edition Add-On for CRM Basic (nitelikli teklif)</span><span class="sxs-lookup"><span data-stu-id="f7043-141">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f7043-142">Dynamics 365 müşteri katılımı planı CRM Basic için Enterprise Edition Add-On, Fakülteler için</span><span class="sxs-lookup"><span data-stu-id="f7043-142">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="f7043-143">Temel (nitelikli teklifler) değiştirme planlarından satış/müşteri katılım planına yönelik Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="f7043-143">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="f7043-144">**Kullanımdan kaldırılan teklifler**</span><span class="sxs-lookup"><span data-stu-id="f7043-144">**Retired offers**</span></span>   

- <span data-ttu-id="f7043-145">CRM Basic veya CRMOL Basic 'ten (nitelikli teklif) satış için Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="f7043-145">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f7043-146">Dynamics 365 müşteri katılımı planı CRM Basic veya CRMOL Basic (nitelikli teklif)</span><span class="sxs-lookup"><span data-stu-id="f7043-146">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="f7043-147">**Değiştirme seçenekleri**</span><span class="sxs-lookup"><span data-stu-id="f7043-147">**Replacement options**</span></span>
- <span data-ttu-id="f7043-148">Sales Professional için Dynamics 365 (yenı)</span><span class="sxs-lookup"><span data-stu-id="f7043-148">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="f7043-149">Sales Professional için Dynamics 365 (yenı)</span><span class="sxs-lookup"><span data-stu-id="f7043-149">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="f7043-150">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="f7043-150">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="f7043-151">Dynamics 365 müşteri katılımı planı veya</span><span class="sxs-lookup"><span data-stu-id="f7043-151">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="f7043-152">Dynamics 365 ekip üyeleri</span><span class="sxs-lookup"><span data-stu-id="f7043-152">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="f7043-153">Müşterilerin yeni ürün planlarına geçişini sağlar</span><span class="sxs-lookup"><span data-stu-id="f7043-153">Transition customers to new product plans</span></span>

<span data-ttu-id="f7043-154">Müşterileri kullanımdan kaldırılan SKU 'lardan daha yeni bir sürümüne taşımak, bu sırayla aşağıdaki adımları gerektirir:</span><span class="sxs-lookup"><span data-stu-id="f7043-154">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="f7043-155">Yeni aboneliği satın alın</span><span class="sxs-lookup"><span data-stu-id="f7043-155">Purchase the new subscription</span></span>
- <span data-ttu-id="f7043-156">Geçerli kullanıcı lisanslarını yeniden ata</span><span class="sxs-lookup"><span data-stu-id="f7043-156">Reassign current user licenses</span></span>
- <span data-ttu-id="f7043-157">Eski aboneliği iptal et</span><span class="sxs-lookup"><span data-stu-id="f7043-157">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="f7043-158">Müşteriniz için yeni planı satın alın</span><span class="sxs-lookup"><span data-stu-id="f7043-158">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="f7043-159">Sol gezinti bölmesinde **müşteriler** ' i seçin ve sonra yeni aboneliğe taşımak istediğiniz müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="f7043-159">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="f7043-160">**Abonelik Ekle** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="f7043-160">Select **Add Subscription** .</span></span>
3. <span data-ttu-id="f7043-161">Katalogdan satın almak istediğiniz aboneliği seçin (Bu durumda yukarıdaki seçeneklerden biri), lisansların sayısını girin ve ardından **Gönder** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="f7043-161">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit** .</span></span> 

<span data-ttu-id="f7043-162">Müşterinizin artık hem eski hem de yeni bir abonelik olacak.</span><span class="sxs-lookup"><span data-stu-id="f7043-162">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="f7043-163">Bir sonraki adımınız, lisansları müşterinin kullanıcılarına yeniden atamak olur.</span><span class="sxs-lookup"><span data-stu-id="f7043-163">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="f7043-164">Sol gezinti çubuğunda **müşteriler** ' i seçin ve ardından taşıdığınız müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="f7043-164">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="f7043-165">**Kullanıcılar ve lisanslar ' ı** seçin.</span><span class="sxs-lookup"><span data-stu-id="f7043-165">Select **Users and licenses** .</span></span>
3. <span data-ttu-id="f7043-166">Bir kullanıcıya bir lisansı yeniden atamak için kullanıcıyı seçin ve ardından **Lisansları Yönet** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="f7043-166">To reassign a license to a user, select the user and then select **Manage licenses** .</span></span> 
4. <span data-ttu-id="f7043-167">**Lisansları Yönet** sayfasında, temel (nitelikli teklif) lisanstan satış/müşteri katılım planı için Dynamics 365 ' i temizleyin ve müşterinin taşınmakta olduğu abonelik için yeni bir hizmet planı seçin.</span><span class="sxs-lookup"><span data-stu-id="f7043-167">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="f7043-168">**Gönder** ’i seçin.</span><span class="sxs-lookup"><span data-stu-id="f7043-168">Select **Submit** .</span></span> <span data-ttu-id="f7043-169">Bunu, yeni lisansa ihtiyacı olan her kullanıcı için yapabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f7043-169">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="f7043-170">Lisansları yeni aboneliğe taşındıktan sonra eski aboneliği iptal edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f7043-170">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="f7043-171">Sol gezinti çubuğunda **müşteriler** ' i seçin ve ardından taşıdığınız müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="f7043-171">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="f7043-172">Abonelik Ayrıntıları sayfasında, eski aboneliği **askıya alındı** olarak ayarlayın ve **Gönder** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="f7043-172">On the subscription detail page, set the old subscription to **Suspended** and select **Submit** .</span></span>

<span data-ttu-id="f7043-173">Eski abonelik artık askıya alındı ve yeni abonelik etkin.</span><span class="sxs-lookup"><span data-stu-id="f7043-173">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="f7043-174">Askıya alınan abonelik 120 gün sonra otomatik olarak sağlanacaktır.</span><span class="sxs-lookup"><span data-stu-id="f7043-174">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="f7043-175">Müşterinizin eski abonelik için ek ücret ödemeyecektir.</span><span class="sxs-lookup"><span data-stu-id="f7043-175">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



