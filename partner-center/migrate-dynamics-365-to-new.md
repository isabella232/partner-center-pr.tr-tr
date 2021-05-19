---
title: Dynamics 365 Business Edition'ı geçirme
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Tam Dynamics 365 Business Edition tekliflerini süresi dolmadan önce daha yeni sürümlere geçirmeyi öğrenin.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8232ab165ea68ebefdfbb30f3ac52c907e1b7278
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151534"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="5fe91-103">Dynamics 365 Business Edition Tekliflerini daha yeni sürümlere geçirme</span><span class="sxs-lookup"><span data-stu-id="5fe91-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="5fe91-104">**Uygun roller:** Genel yönetici | Kullanıcı yönetimi yönetici | Yönetici aracısı | Satış aracısı</span><span class="sxs-lookup"><span data-stu-id="5fe91-104">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="5fe91-105">Dynamics 365 Business Edition abonelikleri olan müşteriler 1 Ocak 2019'dan itibaren bu eski tekliflere yenilenmeyecektir; mevcut aboneliklerin süresi dolduğunda otomatik olarak yenilenmez.</span><span class="sxs-lookup"><span data-stu-id="5fe91-105">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="5fe91-106">Aboneliğin ayrıntı sayfasında abonelik durumu "[date]" ile "[date] üzerinde otomatik yenileme" olarak değişir.</span><span class="sxs-lookup"><span data-stu-id="5fe91-106">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="5fe91-107">Müşterilerin sürekliliğini sağlamak için, süresi dolan abonelikleri aşağıda listelenen desteklenen bir seçen geçişlisiniz.</span><span class="sxs-lookup"><span data-stu-id="5fe91-107">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="5fe91-108">Müşteriler için hizmet kesintilerini önlemek için müşterileri aboneliğin yıllık bitiş tarihi öncesinde yeni aboneliklere taşımanız önerilir.</span><span class="sxs-lookup"><span data-stu-id="5fe91-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="5fe91-109">API'yi (CREST veya İş Ortağı Merkezi) kullanıyorsanız, aboneliğin bitiş tarihini ve otomatik yenileme = False özelliğini değerlendirerek süresi dolan abonelikleri bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5fe91-109">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="5fe91-110">Söz konusu abonelikler 1 Ocak 2019'da otomatik olarak yenilenecek=False olarak ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="5fe91-110">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="5fe91-111">Müşterileri yeni bir plana her zaman taşımanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="5fe91-111">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="5fe91-112">Dynamics 365 Business Sürümleri kaldırıyor</span><span class="sxs-lookup"><span data-stu-id="5fe91-112">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="5fe91-113">Dynamics 365 for Finance and Operations, Business edition</span><span class="sxs-lookup"><span data-stu-id="5fe91-113">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="5fe91-114">Dynamics 365 for Team Members, Business sürümü</span><span class="sxs-lookup"><span data-stu-id="5fe91-114">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="5fe91-115">Dynamics Business Central - Dynamics 365 Business Edition yeni teklifleri</span><span class="sxs-lookup"><span data-stu-id="5fe91-115">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="5fe91-116">Yeni Dynamics Business Central teklifleri ile müşterileriniz iş süreçlerini kolaylaştırma, müşteri etkileşimlerini geliştirme ve daha iyi kararlar alma için finansal, satış, hizmet ve operasyonlarını birbirine bağ hale getirmek için bu teklifleri karşılar.</span><span class="sxs-lookup"><span data-stu-id="5fe91-116">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="5fe91-117">Dynamics 365 Business Central bulut tabanlıdır ve yalnızca Bulut Çözümü Sağlayıcısı (CSP) programı iş ortakları aracılığıyla kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="5fe91-117">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="5fe91-118">Dynamics 365 Business Edition müşterileri, 30 Haziran 2020'ye kadar yeni Business Central teklifleri için indirimli geçiş fiyatlandırması almaya hak kazanmaktadır.</span><span class="sxs-lookup"><span data-stu-id="5fe91-118">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="5fe91-119">Müşterileri yeni ürün planlarına geçiş</span><span class="sxs-lookup"><span data-stu-id="5fe91-119">Transition customers to new product plans</span></span>

 <span data-ttu-id="5fe91-120">Müşterilerin eski SKÜ'lerden yeni SKUS'lara taşınmaları için bu sırayla aşağıdaki adımlar gerekir:</span><span class="sxs-lookup"><span data-stu-id="5fe91-120">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="5fe91-121">Yeni aboneliği satın alma</span><span class="sxs-lookup"><span data-stu-id="5fe91-121">Purchase the new subscription</span></span>
- <span data-ttu-id="5fe91-122">Geçerli kullanıcı lisanslarını yeniden atama</span><span class="sxs-lookup"><span data-stu-id="5fe91-122">Reassign current user licenses</span></span>
- <span data-ttu-id="5fe91-123">Eski aboneliği iptal etme</span><span class="sxs-lookup"><span data-stu-id="5fe91-123">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="5fe91-124">Müşteriniz için yeni planı satın alma</span><span class="sxs-lookup"><span data-stu-id="5fe91-124">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="5fe91-125">Sol **gezinti** çubuğundan Müşteriler'i ve ardından yeni aboneliğe taşımak istediğiniz müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="5fe91-125">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="5fe91-126">Abonelik **Ekle'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="5fe91-126">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="5fe91-127">Katalogdan satın almak istediğiniz aboneliği seçin (bu durumda, yukarıdaki seçeneklerden biri), lisans sayısını girin ve gönder'i **seçin.**</span><span class="sxs-lookup"><span data-stu-id="5fe91-127">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="5fe91-128">Müşteriniz artık hem eski aboneliğe hem de yeni aboneliğe sahip olur.</span><span class="sxs-lookup"><span data-stu-id="5fe91-128">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="5fe91-129">Sonraki adımınız, lisansları müşterinin kullanıcılarına yeniden atamanızdır.</span><span class="sxs-lookup"><span data-stu-id="5fe91-129">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="5fe91-130">Sol **gezinti** çubuğundan Müşteriler'i ve ardından hareket halindeki müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="5fe91-130">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="5fe91-131">Kullanıcılar **ve lisanslar'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="5fe91-131">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="5fe91-132">Bir kullanıcıya bir lisansı yeniden atamak için, kullanıcıyı seçin ve ardından Lisansları **yönet'i seçin.**</span><span class="sxs-lookup"><span data-stu-id="5fe91-132">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="5fe91-133">Lisansları **yönet sayfasında** Temel (Nitelikli Teklif) lisansından Dynamics 365 for Sales/ Customer Engagement Planı'nın onay kutusunu temizleyin ve müşterinin taşınıyor olduğu abonelik için yeni bir hizmet planı seçin.</span><span class="sxs-lookup"><span data-stu-id="5fe91-133">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="5fe91-134">**Gönder**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="5fe91-134">Select **Submit**.</span></span> <span data-ttu-id="5fe91-135">Bunu yeni lisansa ihtiyacı olan her kullanıcı için yapacaktır.</span><span class="sxs-lookup"><span data-stu-id="5fe91-135">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="5fe91-136">Lisansları yeni aboneliğe taşıdıktan sonra eski aboneliği iptal edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5fe91-136">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="5fe91-137">Sol **gezinti** çubuğundan Müşteriler'i ve ardından hareket halindeki müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="5fe91-137">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="5fe91-138">Abonelik ayrıntıları sayfasında eski aboneliği Askıya Alındı olarak ayarlayın ve **Gönder'i** **seçin.**</span><span class="sxs-lookup"><span data-stu-id="5fe91-138">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="5fe91-139">Eski abonelik artık askıya alınır ve yeni abonelik etkindir.</span><span class="sxs-lookup"><span data-stu-id="5fe91-139">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="5fe91-140">Askıya alınan abonelik 120 gün sonra otomatik olarak sağlanacak.</span><span class="sxs-lookup"><span data-stu-id="5fe91-140">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="5fe91-141">Müşteriniz eski abonelik için ek ücret ödemez.</span><span class="sxs-lookup"><span data-stu-id="5fe91-141">Your customer will incur no additional costs for the old subscription.</span></span>
