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
ms.openlocfilehash: 583e9c40bb8d161c30440f12331dc8dcbf3db417
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146434"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a><span data-ttu-id="3a4cf-104">Kaizala Pro tek başına aboneliklerini Microsoft 365 veya Office 365 sürümlerine geçirin</span><span class="sxs-lookup"><span data-stu-id="3a4cf-104">Migrate Kaizala Pro Standalone subscriptions to Microsoft 365 or Office 365 versions</span></span>

<span data-ttu-id="3a4cf-105">**Uygun roller**: satış Aracısı</span><span class="sxs-lookup"><span data-stu-id="3a4cf-105">**Appropriate roles**: Sales agent</span></span>

<span data-ttu-id="3a4cf-106">1 Temmuz 2020 ' den itibaren geçerli olan Microsoft, Kaizala Pro tek başına hizmetinin satışlarını sonlandırıyor.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-106">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="3a4cf-107">Müşteriler artık bu tarihten sonra yeni Kaizala Pro abonelikleri satın amayacak ve mevcut Kaizala Pro abonelikleri süreleri dolduğunda otomatik olarak yenilenmeyecektir.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-107">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="3a4cf-108">Müşterilerin devamlılığını sağlamak için, süresi dolan Kaizala Pro tek başına aboneliklerine sahip müşterileri aşağıda listelenen desteklenen bir SKU seçeneğine geçirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-108">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="3a4cf-109">Müşterilerin hizmet kesintilerinden kaçınmak için, aboneliğin yıllık bitiş tarihinden önce müşterileri yeni aboneliklere taşımayı öneririz.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-109">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="3a4cf-110">API 'yi (CREST veya Partner Center) kullanıyorsanız, otomatik yenileme özelliği false olarak ayarlanmış şekilde, aboneliğin bitiş tarihini değerlendirerek süresi dolan abonelikleri bulabilirsiniz: `auto renew = False` .</span><span class="sxs-lookup"><span data-stu-id="3a4cf-110">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="3a4cf-111">E4 abonelikleri `auto renew=False` 1 temmuz 2020 tarihinde olarak ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-111">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="3a4cf-112">Müşterileri dilediğiniz zaman yeni bir plana taşıyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-112">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="3a4cf-113">Kaizala Pro tek başına değiştirme planları</span><span class="sxs-lookup"><span data-stu-id="3a4cf-113">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="3a4cf-114">Yeni planlar sayesinde, müşterileriniz Microsoft 365 yeni özelliklerden ve işlevlerden faydalanabilir.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-114">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="3a4cf-115">Fiyatlandırma ayrıntıları, Iş Ortağı Merkezi 'nde fiyat listesi ve teklif listesi matrisinde bulunur.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-115">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="3a4cf-116">[**İş için Microsoft 365**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), şunlar dahil:</span><span class="sxs-lookup"><span data-stu-id="3a4cf-116">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="3a4cf-117">Microsoft 365 İş temel</span><span class="sxs-lookup"><span data-stu-id="3a4cf-117">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="3a4cf-118">Microsoft 365 İş standart</span><span class="sxs-lookup"><span data-stu-id="3a4cf-118">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="3a4cf-119">Microsoft 365 İş Premium</span><span class="sxs-lookup"><span data-stu-id="3a4cf-119">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="3a4cf-120">[**Frontline için Microsoft 365**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), şunlar dahil:</span><span class="sxs-lookup"><span data-stu-id="3a4cf-120">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="3a4cf-121">Microsoft 365 F3 (eski adıyla Microsoft 365 F1) ve Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="3a4cf-121">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="3a4cf-122">[**Microsoft 365 için şu şekildedir:**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans)</span><span class="sxs-lookup"><span data-stu-id="3a4cf-122">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="3a4cf-123">Office 365 E1</span><span class="sxs-lookup"><span data-stu-id="3a4cf-123">Office 365 E1</span></span>
   - <span data-ttu-id="3a4cf-124">Microsoft 365 E3 ve Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="3a4cf-124">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="3a4cf-125">Microsoft 365 E5 ve Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="3a4cf-125">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="3a4cf-126">[**Microsoft 365 için eğitim,**](https://www.microsoft.com/education/buy-license/microsoft365)örneğin:</span><span class="sxs-lookup"><span data-stu-id="3a4cf-126">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="3a4cf-127">Microsoft 365 A1 ve Office 365 A1</span><span class="sxs-lookup"><span data-stu-id="3a4cf-127">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="3a4cf-128">Microsoft 365 A3 ve Office 365 A3</span><span class="sxs-lookup"><span data-stu-id="3a4cf-128">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="3a4cf-129">Microsoft 365 A5 ve Office 365 A5</span><span class="sxs-lookup"><span data-stu-id="3a4cf-129">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="3a4cf-130">Müşterileri yeni ürün planlarına geçiş</span><span class="sxs-lookup"><span data-stu-id="3a4cf-130">Transition customers to new product plans</span></span>

<span data-ttu-id="3a4cf-131">Microsoft, iş ortaklarımıza sürekli olarak yeni ürün ve hizmetler sunmaktadır.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-131">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="3a4cf-132">Bu gibi durumlarda, müşterileri yeni hizmetlere yükseltmeniz veya aboneliklerini sonunda kapatılacak olan SKUS'lardan geçirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-132">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="3a4cf-133">Müşterileri, eski SKÜ'lerden yeni SKUS'lara şu adımların atılması gerekir:</span><span class="sxs-lookup"><span data-stu-id="3a4cf-133">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="3a4cf-134">A.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-134">A.</span></span> <span data-ttu-id="3a4cf-135">Yeni aboneliği satın alma</span><span class="sxs-lookup"><span data-stu-id="3a4cf-135">Purchase the new subscription</span></span>

<span data-ttu-id="3a4cf-136">B.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-136">B.</span></span> <span data-ttu-id="3a4cf-137">Geçerli kullanıcı lisanslarını yeniden atama</span><span class="sxs-lookup"><span data-stu-id="3a4cf-137">Reassign current user licenses</span></span>

<span data-ttu-id="3a4cf-138">C.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-138">C.</span></span> <span data-ttu-id="3a4cf-139">Eski aboneliği iptal etme</span><span class="sxs-lookup"><span data-stu-id="3a4cf-139">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="3a4cf-140">Müşterilerinizi yeni planlara geçirme</span><span class="sxs-lookup"><span data-stu-id="3a4cf-140">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="3a4cf-141">A.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-141">A.</span></span> <span data-ttu-id="3a4cf-142">Yeni aboneliği satın alma</span><span class="sxs-lookup"><span data-stu-id="3a4cf-142">Purchase the new subscription</span></span>

1. <span data-ttu-id="3a4cf-143">Yeni aboneliği satın almak için, **İş Ortağı Merkezi** menüsünden Müşteriler'i **seçin,** taşımak istediğiniz müşteriyi seçin ve ardından Abonelik **ekle'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="3a4cf-143">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="3a4cf-144">Katalogdan satın almak istediğiniz aboneliği seçin (bu durumda, yukarıdaki seçeneklerden biri), lisans sayısını girin ve gönder'i **seçin.**</span><span class="sxs-lookup"><span data-stu-id="3a4cf-144">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="3a4cf-145">Müşterinizin artık hem eski hem de yeni abonelikleri, eski Kaizala Pro Tek Başına aboneliği ve yeni 'hedef' aboneliği (örneğin, Seçenek 1 - Office 365 Kurumsal F1) olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-145">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="3a4cf-146">B.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-146">B.</span></span> <span data-ttu-id="3a4cf-147">Geçerli kullanıcı lisanslarını yeniden ata</span><span class="sxs-lookup"><span data-stu-id="3a4cf-147">Reassign current user licenses</span></span>

1. <span data-ttu-id="3a4cf-148">Müşterinin kullanıcılarının lisanslarını yeniden atamak için **Iş Ortağı Merkezi** menüsünden **müşteriler**' i seçin, taşıdığınız müşteriyi seçin ve ardından **Kullanıcılar ve lisanslar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-148">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="3a4cf-149">Müşterinin kullanıcılar ve lisanslar sayfası açılır.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-149">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="3a4cf-150">Kullanıcı lisansını yeniden atamak için, yeniden atanacak kullanıcıyı seçin ve ardından **Lisansları Yönet**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-150">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="3a4cf-151">**Lisansları Yönet** sayfasında Kaizala Pro tek başına Lisansı onay kutusunu temizleyin ve müşterinin taşınmakta olduğu abonelik için yeni bir hizmet planı seçin.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-151">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="3a4cf-152">**Gönder**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-152">Select **Submit**.</span></span> <span data-ttu-id="3a4cf-153">Bir onay sayfası yeni lisans atamalarını listeler.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-153">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="3a4cf-154">Lisans atamaları gerektiren diğer kullanıcılar için aynı işleme devam edin.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-154">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="3a4cf-155">C.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-155">C.</span></span> <span data-ttu-id="3a4cf-156">Eski aboneliği iptal et</span><span class="sxs-lookup"><span data-stu-id="3a4cf-156">Cancel old subscription</span></span>

<span data-ttu-id="3a4cf-157">Kullanıcı lisansını yeni hizmete taşıdıktan sonra, kullanımdan kaldırılan aboneliği müşteri düzeyinde güvenle iptal edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-157">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="3a4cf-158">**Iş Ortağı Merkezi** menüsünde **müşteriler**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-158">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="3a4cf-159">Aboneliğini iptal ettiğiniz müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-159">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="3a4cf-160">Abonelik Ayrıntıları sayfasında, aboneliği **askıya alındı** olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-160">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="3a4cf-161">**Gönder**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-161">Select **Submit**.</span></span>

<span data-ttu-id="3a4cf-162">Eski abonelik askıya alındı ve yeni abonelik etkin.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-162">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="3a4cf-163">Askıya alınan abonelik 120 gün sonra otomatik olarak sağlanacaktır.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-163">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="3a4cf-164">Müşteri, eski abonelik için ek maliyet içermez.</span><span class="sxs-lookup"><span data-stu-id="3a4cf-164">The customer incurs no additional costs for the old subscription.</span></span>
