---
title: Kaizala Pro aboneliklerini Microsoft 365'e geçirme
description: Kaizala Pro aboneliklerini Microsoft 365 veya Office 365 sürümlerine geçirmeyi öğrenin. Müşterilerinizin geçişini hakkında daha fazla bilgi için bu makaleyi okuyun.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 96d18c8f728c56b705d378ac56dcf46e777157f0
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172436"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a><span data-ttu-id="8af2a-104">Kaizala Pro tek başına aboneliklerini Microsoft 365 veya Office 365 sürümlerine geçirin</span><span class="sxs-lookup"><span data-stu-id="8af2a-104">Migrate Kaizala Pro Standalone subscriptions to Microsoft 365 or Office 365 versions</span></span>

<span data-ttu-id="8af2a-105">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="8af2a-105">**Appropriate roles**</span></span>

- <span data-ttu-id="8af2a-106">Satış Aracısı</span><span class="sxs-lookup"><span data-stu-id="8af2a-106">Sales agent</span></span>

<span data-ttu-id="8af2a-107">1 Temmuz 2020 ' den itibaren geçerli olan Microsoft, Kaizala Pro tek başına hizmetinin satışlarını sonlandırıyor.</span><span class="sxs-lookup"><span data-stu-id="8af2a-107">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="8af2a-108">Müşteriler artık bu tarihten sonra yeni Kaizala Pro abonelikleri satın amayacak ve mevcut Kaizala Pro abonelikleri süreleri dolduğunda otomatik olarak yenilenmeyecektir.</span><span class="sxs-lookup"><span data-stu-id="8af2a-108">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="8af2a-109">Müşterilerin devamlılığını sağlamak için, süresi dolan Kaizala Pro tek başına aboneliklerine sahip müşterileri aşağıda listelenen desteklenen bir SKU seçeneğine geçirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="8af2a-109">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="8af2a-110">Müşterilerin hizmet kesintilerinden kaçınmak için, aboneliğin yıllık bitiş tarihinden önce müşterileri yeni aboneliklere taşımayı öneririz.</span><span class="sxs-lookup"><span data-stu-id="8af2a-110">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="8af2a-111">API 'yi (CREST veya Partner Center) kullanıyorsanız, otomatik yenileme özelliği false olarak ayarlanmış şekilde, aboneliğin bitiş tarihini değerlendirerek süresi dolan abonelikleri bulabilirsiniz: `auto renew = False` .</span><span class="sxs-lookup"><span data-stu-id="8af2a-111">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="8af2a-112">E4 abonelikleri `auto renew=False` 1 temmuz 2020 tarihinde olarak ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="8af2a-112">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="8af2a-113">Müşterileri dilediğiniz zaman yeni bir plana taşıyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8af2a-113">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="8af2a-114">Kaizala Pro tek başına değiştirme planları</span><span class="sxs-lookup"><span data-stu-id="8af2a-114">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="8af2a-115">Yeni planlar sayesinde, müşterileriniz Microsoft 365 yeni özelliklerden ve işlevlerden faydalanabilir.</span><span class="sxs-lookup"><span data-stu-id="8af2a-115">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="8af2a-116">Fiyatlandırma ayrıntıları, Iş Ortağı Merkezi 'nde fiyat listesi ve teklif listesi matrisinde bulunur.</span><span class="sxs-lookup"><span data-stu-id="8af2a-116">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="8af2a-117">[**İş için Microsoft 365**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), şunlar dahil:</span><span class="sxs-lookup"><span data-stu-id="8af2a-117">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="8af2a-118">Microsoft 365 İş temel</span><span class="sxs-lookup"><span data-stu-id="8af2a-118">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="8af2a-119">Microsoft 365 İş standart</span><span class="sxs-lookup"><span data-stu-id="8af2a-119">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="8af2a-120">Microsoft 365 İş Premium</span><span class="sxs-lookup"><span data-stu-id="8af2a-120">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="8af2a-121">[**Frontline için Microsoft 365**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), şunlar dahil:</span><span class="sxs-lookup"><span data-stu-id="8af2a-121">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="8af2a-122">Microsoft 365 F3 (eski adıyla Microsoft 365 F1) ve Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="8af2a-122">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="8af2a-123">Aşağıdakiler dahil olmak üzere [**Microsoft 365**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans):</span><span class="sxs-lookup"><span data-stu-id="8af2a-123">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="8af2a-124">Office 365 E1</span><span class="sxs-lookup"><span data-stu-id="8af2a-124">Office 365 E1</span></span>
   - <span data-ttu-id="8af2a-125">Microsoft 365 E3 ve Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="8af2a-125">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="8af2a-126">Microsoft 365 E5 ve Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="8af2a-126">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="8af2a-127">[**Eğitim için Microsoft 365**](https://www.microsoft.com/education/buy-license/microsoft365), şunlar dahil:</span><span class="sxs-lookup"><span data-stu-id="8af2a-127">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="8af2a-128">Microsoft 365 a1 ve Office 365 a1</span><span class="sxs-lookup"><span data-stu-id="8af2a-128">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="8af2a-129">Microsoft 365 a3 ve Office 365 a3</span><span class="sxs-lookup"><span data-stu-id="8af2a-129">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="8af2a-130">Microsoft 365 a5 ve Office 365 a5</span><span class="sxs-lookup"><span data-stu-id="8af2a-130">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="8af2a-131">Müşterilerin yeni ürün planlarına geçişini sağlar</span><span class="sxs-lookup"><span data-stu-id="8af2a-131">Transition customers to new product plans</span></span>

<span data-ttu-id="8af2a-132">Microsoft, iş ortaklarımız için sürekli olarak yeni ürün ve hizmetler sunar.</span><span class="sxs-lookup"><span data-stu-id="8af2a-132">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="8af2a-133">Bu gibi durumlarda, müşterileri yeni hizmetlere yükseltmeniz veya sonunda kapatılacak SKU 'lardan aboneliklerini geçirmeniz gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="8af2a-133">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="8af2a-134">Müşterilerin Kullanımdan kaldırılmış SKU 'lardan daha yeni bir sürümüne geçirilmesi aşağıdaki adımları gerektirir:</span><span class="sxs-lookup"><span data-stu-id="8af2a-134">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="8af2a-135">A.</span><span class="sxs-lookup"><span data-stu-id="8af2a-135">A.</span></span> <span data-ttu-id="8af2a-136">Yeni aboneliği satın alın</span><span class="sxs-lookup"><span data-stu-id="8af2a-136">Purchase the new subscription</span></span>

<span data-ttu-id="8af2a-137">B.</span><span class="sxs-lookup"><span data-stu-id="8af2a-137">B.</span></span> <span data-ttu-id="8af2a-138">Geçerli kullanıcı lisanslarını yeniden ata</span><span class="sxs-lookup"><span data-stu-id="8af2a-138">Reassign current user licenses</span></span>

<span data-ttu-id="8af2a-139">C.</span><span class="sxs-lookup"><span data-stu-id="8af2a-139">C.</span></span> <span data-ttu-id="8af2a-140">Eski aboneliği iptal et</span><span class="sxs-lookup"><span data-stu-id="8af2a-140">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="8af2a-141">Müşterilerinizi yeni planlara geçirin</span><span class="sxs-lookup"><span data-stu-id="8af2a-141">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="8af2a-142">A.</span><span class="sxs-lookup"><span data-stu-id="8af2a-142">A.</span></span> <span data-ttu-id="8af2a-143">Yeni aboneliği satın alın</span><span class="sxs-lookup"><span data-stu-id="8af2a-143">Purchase the new subscription</span></span>

1. <span data-ttu-id="8af2a-144">Yeni aboneliği satın almak için **Iş Ortağı Merkezi** menüsünden **müşteriler**' i seçin, taşımak istediğiniz müşteriyi seçin ve ardından **Abonelik Ekle**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="8af2a-144">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="8af2a-145">Katalogdan satın almak istediğiniz aboneliği seçin (Bu durumda yukarıdaki seçeneklerden biri), lisansların sayısını girin ve ardından **Gönder**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="8af2a-145">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="8af2a-146">Müşterinizin artık eski ve yeni abonelikleri, eski Kaizala Pro tek başına aboneliği ve yeni ' Target ' aboneliği olmalıdır; örneğin, 1-Office 365 Kurumsal F1.</span><span class="sxs-lookup"><span data-stu-id="8af2a-146">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="8af2a-147">B.</span><span class="sxs-lookup"><span data-stu-id="8af2a-147">B.</span></span> <span data-ttu-id="8af2a-148">Geçerli kullanıcı lisanslarını yeniden ata</span><span class="sxs-lookup"><span data-stu-id="8af2a-148">Reassign current user licenses</span></span>

1. <span data-ttu-id="8af2a-149">Müşterinin kullanıcılarının lisanslarını yeniden atamak için **Iş Ortağı Merkezi** menüsünden **müşteriler**' i seçin, taşıdığınız müşteriyi seçin ve ardından **Kullanıcılar ve lisanslar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="8af2a-149">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="8af2a-150">Müşterinin kullanıcılar ve lisanslar sayfası açılır.</span><span class="sxs-lookup"><span data-stu-id="8af2a-150">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="8af2a-151">Kullanıcı lisansını yeniden atamak için, yeniden atanacak kullanıcıyı seçin ve ardından **Lisansları Yönet**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="8af2a-151">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="8af2a-152">**Lisansları Yönet** sayfasında Kaizala Pro tek başına Lisansı onay kutusunu temizleyin ve müşterinin taşınmakta olduğu abonelik için yeni bir hizmet planı seçin.</span><span class="sxs-lookup"><span data-stu-id="8af2a-152">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="8af2a-153">**Gönder**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="8af2a-153">Select **Submit**.</span></span> <span data-ttu-id="8af2a-154">Bir onay sayfası yeni lisans atamalarını listeler.</span><span class="sxs-lookup"><span data-stu-id="8af2a-154">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="8af2a-155">Lisans atamaları gerektiren diğer kullanıcılar için aynı işleme devam edin.</span><span class="sxs-lookup"><span data-stu-id="8af2a-155">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="8af2a-156">C.</span><span class="sxs-lookup"><span data-stu-id="8af2a-156">C.</span></span> <span data-ttu-id="8af2a-157">Eski aboneliği iptal et</span><span class="sxs-lookup"><span data-stu-id="8af2a-157">Cancel old subscription</span></span>

<span data-ttu-id="8af2a-158">Kullanıcı lisansını yeni hizmete taşıdıktan sonra, kullanımdan kaldırılan aboneliği müşteri düzeyinde güvenle iptal edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8af2a-158">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="8af2a-159">**Iş Ortağı Merkezi** menüsünde **müşteriler**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="8af2a-159">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="8af2a-160">Aboneliğini iptal ettiğiniz müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="8af2a-160">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="8af2a-161">Abonelik Ayrıntıları sayfasında, aboneliği **askıya alındı** olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="8af2a-161">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="8af2a-162">**Gönder**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="8af2a-162">Select **Submit**.</span></span>

<span data-ttu-id="8af2a-163">Eski abonelik askıya alındı ve yeni abonelik etkin.</span><span class="sxs-lookup"><span data-stu-id="8af2a-163">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="8af2a-164">Askıya alınan abonelik 120 gün sonra otomatik olarak sağlanacaktır.</span><span class="sxs-lookup"><span data-stu-id="8af2a-164">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="8af2a-165">Müşteri, eski abonelik için ek maliyet içermez.</span><span class="sxs-lookup"><span data-stu-id="8af2a-165">The customer incurs no additional costs for the old subscription.</span></span>
