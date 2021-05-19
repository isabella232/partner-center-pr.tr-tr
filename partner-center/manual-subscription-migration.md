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
ms.openlocfilehash: 5ba6992eff64031aed0dafeb5a5010983396ab63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151653"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="809bd-103">Dynamics 365 ve Müşteri Etkileşimi Planı’nı Temel’den (uygun teklifler) daha yeni sürümlere geçirme</span><span class="sxs-lookup"><span data-stu-id="809bd-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="809bd-104">**Uygun roller**: genel yönetici | Kullanıcı Yönetimi Yöneticisi | Yönetici Aracısı | Satış Aracısı</span><span class="sxs-lookup"><span data-stu-id="809bd-104">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="809bd-105">1 Ocak 2019 ' den itibaren, temel (nitelikli teklifler) aboneliklerden satış/müşteri katılım planı için Dynamics 365 olan müşteriler bu eski teklifleri artık yenilemez; mevcut abonelikler, süreleri dolduğunda otomatik olarak yenilenmeyecektir.</span><span class="sxs-lookup"><span data-stu-id="809bd-105">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="809bd-106">Aboneliğin ayrıntı sayfasında, abonelik durumu "otomatik yenilemede [Tarih]" içinden "süresi doluyor" olarak değişir.</span><span class="sxs-lookup"><span data-stu-id="809bd-106">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="809bd-107">Müşterilerin devamlılığını sağlamak için, süresi dolan aboneliklerle birlikte aşağıda listelenen desteklenen bir seçeneğe geçiş yapmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="809bd-107">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="809bd-108">Müşterilerin hizmet kesintilerinden kaçınmak için, aboneliğin yıllık bitiş tarihinden önce müşterileri yeni aboneliklere taşımayı öneririz.</span><span class="sxs-lookup"><span data-stu-id="809bd-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="809bd-109">API 'YI (CREST veya Partner Center) kullanıyorsanız, Otomatik Yenile = false özelliğiyle birlikte Aboneliğin bitiş tarihini değerlendirerek süresi dolan abonelikleri bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="809bd-109">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="809bd-110">Söz konusu abonelikler, 1 Ocak 2019 tarihinde otomatik olarak Yenile = false olarak ayarlanacak.</span><span class="sxs-lookup"><span data-stu-id="809bd-110">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="809bd-111">Müşterileri dilediğiniz zaman yeni bir plana taşıyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="809bd-111">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="809bd-112">Dynamics 365, kullanımdan kalkmakta olan teklifleri</span><span class="sxs-lookup"><span data-stu-id="809bd-112">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="809bd-113">Sales Enterprise Edition CRMOL Basic (nitelikli teklif) için Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="809bd-113">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="809bd-114">Fakülteler için Dynamics 365 for Sales Enterprise Edition CRMOL Basic (nitelikli teklif)</span><span class="sxs-lookup"><span data-stu-id="809bd-114">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="809bd-115">Öğrenciler için Dynamics 365 for Sales Enterprise Edition CRMOL Basic (nitelikli teklif)</span><span class="sxs-lookup"><span data-stu-id="809bd-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="809bd-116">Sales Enterprise Edition için Dynamics 365 (kamu fiyatlandırması) CRMOL temel (nitelikli teklif)</span><span class="sxs-lookup"><span data-stu-id="809bd-116">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="809bd-117">CRM Basic için SA 'Dan Sales Enterprise Edition için Dynamics 365 (nitelikli teklif)</span><span class="sxs-lookup"><span data-stu-id="809bd-117">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="809bd-118">Dynamics 365 for Sales Enterprise Edition for CRM Basic (uygun teklif) için ŞA</span><span class="sxs-lookup"><span data-stu-id="809bd-118">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="809bd-119">Öğrenciler için Dynamics 365 for Sales Enterprise Edition for CRM Basic (nitelikli teklif)</span><span class="sxs-lookup"><span data-stu-id="809bd-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="809bd-120">Dynamics 365 for Sales Enterprise Edition (kamu fiyatlandırması) için SA 'Dan CRM temel (nitelikli teklif)</span><span class="sxs-lookup"><span data-stu-id="809bd-120">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="809bd-121">CRM Basic için Dynamics 365 for Sales Enterprise Sürümü Add-On (Nitelikli Teklif)</span><span class="sxs-lookup"><span data-stu-id="809bd-121">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="809bd-122">Fakülteler için DYNAMICS 365 for Sales Enterprise Sürümü Add-On CRM Basic (Nitelikli Teklif)</span><span class="sxs-lookup"><span data-stu-id="809bd-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="809bd-123">Dynamics 365 for Sales Enterprise Sürümü Add-On for CRM Basic (Öğrenciler için Nitelikli Teklif)</span><span class="sxs-lookup"><span data-stu-id="809bd-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="809bd-124">Dynamics 365 for Sales Enterprise Sürümü (Kamu Fiyatlandırması) Add-On CRM Temel (Nitelikli Teklif)</span><span class="sxs-lookup"><span data-stu-id="809bd-124">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="809bd-125">DYNAMICS 365 Müşteri Katılımı Planı Enterprise Sürümü CRMOL Basic (Nitelikli Teklif)</span><span class="sxs-lookup"><span data-stu-id="809bd-125">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="809bd-126">Dynamics 365 Customer Engagement Plan Enterprise Sürümü (Kamu Fiyatlandırması) CRMOL Temel (Nitelikli Teklif)</span><span class="sxs-lookup"><span data-stu-id="809bd-126">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="809bd-127">Dynamics 365 Müşteri Katılımı Planı Enterprise Sürümü CRMOL Basic (Nitelikli Teklif)</span><span class="sxs-lookup"><span data-stu-id="809bd-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="809bd-128">Dynamics 365 Müşteri Katılımı Planı Enterprise Sürümü CRMOL Basic (Nitelikli Teklif)</span><span class="sxs-lookup"><span data-stu-id="809bd-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="809bd-129">Dynamics 365 Customer Engagement Planı Enterprise Sürümü CRM Basic için SA'dan (Nitelikli Teklif)</span><span class="sxs-lookup"><span data-stu-id="809bd-129">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="809bd-130">DYNAMICS 365 Customer Engagement Plan Enterprise Sürümü (Kamu Fiyatlandırması) FROM SA for CRM Basic (Nitelikli Teklif)</span><span class="sxs-lookup"><span data-stu-id="809bd-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="809bd-131">Dynamics 365 Müşteri Katılımı Planı Enterprise Sürümü CRM Temel (Nitelikli Teklif) için SA'dan Eğitim</span><span class="sxs-lookup"><span data-stu-id="809bd-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="809bd-132">Dynamics 365 Müşteri Katılımı Planı Enterprise Sürümü CRM Temel (Nitelikli Teklif) için SA'dan Öğretim Üyeleri</span><span class="sxs-lookup"><span data-stu-id="809bd-132">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="809bd-133">DYNAMICS 365 Customer Engagement Plan Enterprise Sürümü Add-On for CRM Basic (Nitelikli Teklif)</span><span class="sxs-lookup"><span data-stu-id="809bd-133">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="809bd-134">DYNAMICS 365 Customer Engagement Plan Enterprise Sürümü (Kamu Fiyatlandırması) Add-On CRM Temel (Nitelikli Teklif)</span><span class="sxs-lookup"><span data-stu-id="809bd-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="809bd-135">Dynamics 365 Customer Engagement Plan Enterprise Sürümü Add-On for CRM Basic (Nitelikli Teklif)</span><span class="sxs-lookup"><span data-stu-id="809bd-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="809bd-136">Dynamics 365 Customer Engagement Plan Enterprise Sürümü Add-On for CRM Basic (Nitelikli Teklif) for Faculty</span><span class="sxs-lookup"><span data-stu-id="809bd-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="809bd-137">Temel (Nitelikli Teklifler) değiştirme planlarından Dynamics 365 for Sales/ Customer Engagement Planı</span><span class="sxs-lookup"><span data-stu-id="809bd-137">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="809bd-138">**Kaldıran teklifler**</span><span class="sxs-lookup"><span data-stu-id="809bd-138">**Retired offers**</span></span>   

- <span data-ttu-id="809bd-139">CRM Basic veya CRMOL Basic'ten Dynamics 365 for Sales (Nitelikli Teklif)</span><span class="sxs-lookup"><span data-stu-id="809bd-139">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="809bd-140">CRM Basic veya CRMOL Basic'ten Dynamics 365 Customer Engagement Planı (Nitelikli Teklif)</span><span class="sxs-lookup"><span data-stu-id="809bd-140">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="809bd-141">**Değiştirme seçenekleri**</span><span class="sxs-lookup"><span data-stu-id="809bd-141">**Replacement options**</span></span>
- <span data-ttu-id="809bd-142">Sales Professional için Dynamics 365 (yenı)</span><span class="sxs-lookup"><span data-stu-id="809bd-142">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="809bd-143">Sales Professional için Dynamics 365 (yenı)</span><span class="sxs-lookup"><span data-stu-id="809bd-143">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="809bd-144">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="809bd-144">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="809bd-145">Dynamics 365 müşteri katılımı planı veya</span><span class="sxs-lookup"><span data-stu-id="809bd-145">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="809bd-146">Dynamics 365 ekip üyeleri</span><span class="sxs-lookup"><span data-stu-id="809bd-146">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="809bd-147">Müşterilerin yeni ürün planlarına geçişini sağlar</span><span class="sxs-lookup"><span data-stu-id="809bd-147">Transition customers to new product plans</span></span>

<span data-ttu-id="809bd-148">Müşterileri kullanımdan kaldırılan SKU 'lardan daha yeni bir sürümüne taşımak, bu sırayla aşağıdaki adımları gerektirir:</span><span class="sxs-lookup"><span data-stu-id="809bd-148">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="809bd-149">Yeni aboneliği satın alın</span><span class="sxs-lookup"><span data-stu-id="809bd-149">Purchase the new subscription</span></span>
- <span data-ttu-id="809bd-150">Geçerli kullanıcı lisanslarını yeniden ata</span><span class="sxs-lookup"><span data-stu-id="809bd-150">Reassign current user licenses</span></span>
- <span data-ttu-id="809bd-151">Eski aboneliği iptal et</span><span class="sxs-lookup"><span data-stu-id="809bd-151">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="809bd-152">Müşteriniz için yeni planı satın alın</span><span class="sxs-lookup"><span data-stu-id="809bd-152">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="809bd-153">Sol gezinti bölmesinde **müşteriler** ' i seçin ve sonra yeni aboneliğe taşımak istediğiniz müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="809bd-153">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="809bd-154">**Abonelik Ekle**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="809bd-154">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="809bd-155">Katalogdan satın almak istediğiniz aboneliği seçin (Bu durumda yukarıdaki seçeneklerden biri), lisansların sayısını girin ve ardından **Gönder**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="809bd-155">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="809bd-156">Müşterinizin artık hem eski hem de yeni bir abonelik olacak.</span><span class="sxs-lookup"><span data-stu-id="809bd-156">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="809bd-157">Bir sonraki adımınız, lisansları müşterinin kullanıcılarına yeniden atamak olur.</span><span class="sxs-lookup"><span data-stu-id="809bd-157">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="809bd-158">Sol gezinti çubuğunda **müşteriler** ' i seçin ve ardından taşıdığınız müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="809bd-158">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="809bd-159">**Kullanıcılar ve lisanslar ' ı** seçin.</span><span class="sxs-lookup"><span data-stu-id="809bd-159">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="809bd-160">Bir kullanıcıya bir lisansı yeniden atamak için kullanıcıyı seçin ve ardından **Lisansları Yönet**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="809bd-160">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="809bd-161">**Lisansları Yönet** sayfasında, temel (nitelikli teklif) lisanstan satış/müşteri katılım planı için Dynamics 365 ' i temizleyin ve müşterinin taşınmakta olduğu abonelik için yeni bir hizmet planı seçin.</span><span class="sxs-lookup"><span data-stu-id="809bd-161">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="809bd-162">**Gönder**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="809bd-162">Select **Submit**.</span></span> <span data-ttu-id="809bd-163">Bunu yeni lisansa ihtiyacı olan her kullanıcı için yapacaktır.</span><span class="sxs-lookup"><span data-stu-id="809bd-163">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="809bd-164">Lisansları yeni aboneliğe taşıdıktan sonra eski aboneliği iptal edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="809bd-164">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="809bd-165">Sol **gezinti** çubuğundan Müşteriler'i ve ardından hareket halindeki müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="809bd-165">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="809bd-166">Abonelik ayrıntıları sayfasında eski aboneliği Askıya Alındı olarak ayarlayın ve **Gönder'i** **seçin.**</span><span class="sxs-lookup"><span data-stu-id="809bd-166">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="809bd-167">Eski abonelik artık askıya alınır ve yeni abonelik etkindir.</span><span class="sxs-lookup"><span data-stu-id="809bd-167">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="809bd-168">Askıya alınan abonelik, 120 gün sonra otomatik olarak sağlanacak.</span><span class="sxs-lookup"><span data-stu-id="809bd-168">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="809bd-169">Müşteriniz eski abonelik için ek ücret ödemez.</span><span class="sxs-lookup"><span data-stu-id="809bd-169">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



