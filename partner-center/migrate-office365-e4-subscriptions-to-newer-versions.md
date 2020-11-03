---
title: Office 365 E4 aboneliklerini geçirme
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 Enterprise E4 Edition 7 Nisan 2017 tarihinden itibaren kullanımdan kaldırıldı. Müşteri aboneliklerinizi Office 365 ' in daha yeni sürümlerine geçirmeyi öğrenin.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bbd2aceac62a7e726ed81a78305ea23213c94156
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/03/2020
ms.locfileid: "92530946"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="1c92d-104">Office 365 E4 aboneliklerini yeni Office 365 sürümlerine geçirme</span><span class="sxs-lookup"><span data-stu-id="1c92d-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="1c92d-105">**Uygulama hedefi**</span><span class="sxs-lookup"><span data-stu-id="1c92d-105">**Applies to**</span></span>

-  <span data-ttu-id="1c92d-106">İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="1c92d-106">Partner Center</span></span>

<span data-ttu-id="1c92d-107">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="1c92d-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="1c92d-108">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="1c92d-108">Global admin</span></span>
-   <span data-ttu-id="1c92d-109">Kullanıcı yöneticisi</span><span class="sxs-lookup"><span data-stu-id="1c92d-109">User admin</span></span>
-   <span data-ttu-id="1c92d-110">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="1c92d-110">Admin agent</span></span>
-   <span data-ttu-id="1c92d-111">Satış Aracısı</span><span class="sxs-lookup"><span data-stu-id="1c92d-111">Sales agent</span></span>

<span data-ttu-id="1c92d-112">Office 365 Enterprise E4 planı kullanımdan kalkmışsa, 7 Nisan 2017 ' de geçerli değildir.</span><span class="sxs-lookup"><span data-stu-id="1c92d-112">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="1c92d-113">Bu tarihten sonra yeni Office 365 E4 abonelikleri satın alınmaz ve var olan E4 abonelikleri süreleri dolduğunda otomatik olarak yenilenmeyecektir.</span><span class="sxs-lookup"><span data-stu-id="1c92d-113">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="1c92d-114">E4 abonelikleri sona erdirmek için iptal edilir.</span><span class="sxs-lookup"><span data-stu-id="1c92d-114">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="1c92d-115">Müşterilerin devamlılığını sağlamak için, süresi dolan E4 abonelikleriyle müşterileri aşağıda listelenen desteklenen bir SKU seçeneğine geçirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="1c92d-115">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="1c92d-116">Müşterilerin hizmet kesintilerinden kaçınmak için, aboneliğin yıllık bitiş tarihinden önce müşterileri yeni aboneliklere taşımayı öneririz.</span><span class="sxs-lookup"><span data-stu-id="1c92d-116">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="1c92d-117">Hem Office 365 Enterprise E4 ticari hem de kamu SKU 'Ları devre dışı bırakıldı.</span><span class="sxs-lookup"><span data-stu-id="1c92d-117">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="1c92d-118">Aboneliğin ayrıntı sayfasında, E4 abonelik durumu "otomatik yenilemede [Tarih]" içinde "süre sonu" olarak değiştirildi.</span><span class="sxs-lookup"><span data-stu-id="1c92d-118">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="1c92d-119">API 'YI (CREST veya Partner Center) kullanıyorsanız, Otomatik Yenile = false özelliğiyle birlikte Aboneliğin bitiş tarihini değerlendirerek süresi dolan abonelikleri bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1c92d-119">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="1c92d-120">E4 abonelikleri, 7 Nisan 2017 ' de Otomatik Yenile = false olarak ayarlanacak.</span><span class="sxs-lookup"><span data-stu-id="1c92d-120">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="1c92d-121">Müşterileri dilediğiniz zaman yeni bir plana taşıyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1c92d-121">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="1c92d-122">Office 365 Enterprise E4 Edition değiştirme planları</span><span class="sxs-lookup"><span data-stu-id="1c92d-122">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="1c92d-123">E4 ile aynı işlevselliği korumayı seçebilirsiniz veya müşterilerinizin Office 365 ve Skype Kurumsal Çevrimiçi sürüm 'deki yeni özellik ve işlevlerden faydalanmasını sağlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1c92d-123">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="1c92d-124">Fiyatlandırma ayrıntıları, Iş Ortağı Merkezi 'nde fiyat listesi ve teklif listesi matrisinde bulunur.</span><span class="sxs-lookup"><span data-stu-id="1c92d-124">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="1c92d-125">Güvenli ürün Kurumsal E3 veya güvenli üretkenlik Kurumsal E5, sırasıyla Office 365 Enterprise E3 veya Office 365 Kurumsal E5 için aşağıdaki seçenekler yerine kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="1c92d-125">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="1c92d-126">Seçenek 1: Office 365 Kurumsal E5</span><span class="sxs-lookup"><span data-stu-id="1c92d-126">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="1c92d-127">Seçenek 2: Office 365 Enterprise E3 + Skype Kurumsal Bulut PBX</span><span class="sxs-lookup"><span data-stu-id="1c92d-127">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="1c92d-128">Seçenek 3: Office 365 Enterprise E3 + Skype Kurumsal Plus CAL (E4 ile fiyat ve işlev eşliği)</span><span class="sxs-lookup"><span data-stu-id="1c92d-128">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="1c92d-129">4. seçenek: Office 365 Kurumsal E3</span><span class="sxs-lookup"><span data-stu-id="1c92d-129">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="1c92d-130">Özellik</span><span class="sxs-lookup"><span data-stu-id="1c92d-130">Feature</span></span> | <span data-ttu-id="1c92d-131">1\. Seçenek</span><span class="sxs-lookup"><span data-stu-id="1c92d-131">Option 1</span></span> | <span data-ttu-id="1c92d-132">2\. Seçenek</span><span class="sxs-lookup"><span data-stu-id="1c92d-132">Option 2</span></span> | <span data-ttu-id="1c92d-133">Seçenek 3</span><span class="sxs-lookup"><span data-stu-id="1c92d-133">Option 3</span></span> | <span data-ttu-id="1c92d-134">4 seçeneği</span><span class="sxs-lookup"><span data-stu-id="1c92d-134">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="1c92d-135">Office 365 Kurumsal E4 'ye dahil olan tüm özellikler mi alınır?</span><span class="sxs-lookup"><span data-stu-id="1c92d-135">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="1c92d-136">Evet</span><span class="sxs-lookup"><span data-stu-id="1c92d-136">Yes</span></span> | <span data-ttu-id="1c92d-137">Evet</span><span class="sxs-lookup"><span data-stu-id="1c92d-137">Yes</span></span> | <span data-ttu-id="1c92d-138">Evet</span><span class="sxs-lookup"><span data-stu-id="1c92d-138">Yes</span></span> | <span data-ttu-id="1c92d-139">Hayır</span><span class="sxs-lookup"><span data-stu-id="1c92d-139">No</span></span> |
| <span data-ttu-id="1c92d-140">Office 365 ' de yönetilen telefon numaraları?</span><span class="sxs-lookup"><span data-stu-id="1c92d-140">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="1c92d-141">Evet</span><span class="sxs-lookup"><span data-stu-id="1c92d-141">Yes</span></span> | <span data-ttu-id="1c92d-142">Evet</span><span class="sxs-lookup"><span data-stu-id="1c92d-142">Yes</span></span> | <span data-ttu-id="1c92d-143">Hayır</span><span class="sxs-lookup"><span data-stu-id="1c92d-143">No</span></span> | <span data-ttu-id="1c92d-144">Hayır</span><span class="sxs-lookup"><span data-stu-id="1c92d-144">No</span></span> |
| <span data-ttu-id="1c92d-145">Telefon numaraları hem şirket içinde hem de Office 365 ' de (karma dağıtım) yönetiliyor mu?</span><span class="sxs-lookup"><span data-stu-id="1c92d-145">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="1c92d-146">Evet</span><span class="sxs-lookup"><span data-stu-id="1c92d-146">Yes</span></span> | <span data-ttu-id="1c92d-147">Evet</span><span class="sxs-lookup"><span data-stu-id="1c92d-147">Yes</span></span> | <span data-ttu-id="1c92d-148">Hayır</span><span class="sxs-lookup"><span data-stu-id="1c92d-148">No</span></span> | <span data-ttu-id="1c92d-149">Hayır</span><span class="sxs-lookup"><span data-stu-id="1c92d-149">No</span></span> |
| <span data-ttu-id="1c92d-150">PSTN sesli arama planı ekleme seçeneği</span><span class="sxs-lookup"><span data-stu-id="1c92d-150">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="1c92d-151">Evet</span><span class="sxs-lookup"><span data-stu-id="1c92d-151">Yes</span></span> | <span data-ttu-id="1c92d-152">Evet</span><span class="sxs-lookup"><span data-stu-id="1c92d-152">Yes</span></span> | <span data-ttu-id="1c92d-153">Hayır</span><span class="sxs-lookup"><span data-stu-id="1c92d-153">No</span></span> | <span data-ttu-id="1c92d-154">Hayır</span><span class="sxs-lookup"><span data-stu-id="1c92d-154">No</span></span> |
| <span data-ttu-id="1c92d-155">PSTN Konferansı?</span><span class="sxs-lookup"><span data-stu-id="1c92d-155">PSTN Conferencing?</span></span> | <span data-ttu-id="1c92d-156">Evet</span><span class="sxs-lookup"><span data-stu-id="1c92d-156">Yes</span></span> | <span data-ttu-id="1c92d-157">Hayır</span><span class="sxs-lookup"><span data-stu-id="1c92d-157">No</span></span> | <span data-ttu-id="1c92d-158">Hayır</span><span class="sxs-lookup"><span data-stu-id="1c92d-158">No</span></span> | <span data-ttu-id="1c92d-159">Hayır</span><span class="sxs-lookup"><span data-stu-id="1c92d-159">No</span></span> |
| <span data-ttu-id="1c92d-160">İşbirliği, analiz ve güvenlik için gelişmiş araçlar?</span><span class="sxs-lookup"><span data-stu-id="1c92d-160">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="1c92d-161">Evet</span><span class="sxs-lookup"><span data-stu-id="1c92d-161">Yes</span></span> | <span data-ttu-id="1c92d-162">Hayır</span><span class="sxs-lookup"><span data-stu-id="1c92d-162">No</span></span> | <span data-ttu-id="1c92d-163">Hayır</span><span class="sxs-lookup"><span data-stu-id="1c92d-163">No</span></span> | <span data-ttu-id="1c92d-164">Hayır</span><span class="sxs-lookup"><span data-stu-id="1c92d-164">No</span></span> |
| <span data-ttu-id="1c92d-165">Etkileşimli raporlar, panolar ve veri görselleştirmeleri?</span><span class="sxs-lookup"><span data-stu-id="1c92d-165">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="1c92d-166">Evet</span><span class="sxs-lookup"><span data-stu-id="1c92d-166">Yes</span></span> | <span data-ttu-id="1c92d-167">Hayır</span><span class="sxs-lookup"><span data-stu-id="1c92d-167">No</span></span> | <span data-ttu-id="1c92d-168">Hayır</span><span class="sxs-lookup"><span data-stu-id="1c92d-168">No</span></span> | <span data-ttu-id="1c92d-169">Hayır</span><span class="sxs-lookup"><span data-stu-id="1c92d-169">No</span></span> | 
| <span data-ttu-id="1c92d-170">Yerleşik gizlilik, saydamlık ve iyileştirilmiş Kullanıcı denetimleriyle veri güvenliği ve uyumluluk üzerinde daha fazla denetim var mı?</span><span class="sxs-lookup"><span data-stu-id="1c92d-170">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="1c92d-171">Evet</span><span class="sxs-lookup"><span data-stu-id="1c92d-171">Yes</span></span> | <span data-ttu-id="1c92d-172">Hayır</span><span class="sxs-lookup"><span data-stu-id="1c92d-172">No</span></span> | <span data-ttu-id="1c92d-173">Hayır</span><span class="sxs-lookup"><span data-stu-id="1c92d-173">No</span></span> | <span data-ttu-id="1c92d-174">Hayır</span><span class="sxs-lookup"><span data-stu-id="1c92d-174">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="1c92d-175">Müşterilerin yeni ürün planlarına geçişini sağlar</span><span class="sxs-lookup"><span data-stu-id="1c92d-175">Transition customers to new product plans</span></span>

<span data-ttu-id="1c92d-176">Microsoft, iş ortaklarımız için sürekli olarak yeni ürün ve hizmetler sunar.</span><span class="sxs-lookup"><span data-stu-id="1c92d-176">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="1c92d-177">Bu gibi durumlarda, müşterileri yeni hizmetlere yükseltmeniz veya sonunda kapatılacak SKU 'lardan aboneliklerini geçirmeniz gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="1c92d-177">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="1c92d-178">Müşterilerin Kullanımdan kaldırılmış SKU 'lardan daha yeni bir sürümüne geçirilmesi aşağıdaki adımları gerektirir:</span><span class="sxs-lookup"><span data-stu-id="1c92d-178">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="1c92d-179">Yeni aboneliği satın alın</span><span class="sxs-lookup"><span data-stu-id="1c92d-179">Purchase the new subscription</span></span>
-   <span data-ttu-id="1c92d-180">Geçerli kullanıcı lisanslarını yeniden ata</span><span class="sxs-lookup"><span data-stu-id="1c92d-180">Reassign current user licenses</span></span>
-   <span data-ttu-id="1c92d-181">Eski aboneliği iptal et</span><span class="sxs-lookup"><span data-stu-id="1c92d-181">Cancel the old subscription</span></span>

<span data-ttu-id="1c92d-182">Müşterinin Office 365 Kurumsal E4 aboneliğini Yukarıdaki tablodaki seçeneklerden birine geçirmek için aşağıdaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="1c92d-182">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="1c92d-183">1. adım-yeni aboneliği satın alma</span><span class="sxs-lookup"><span data-stu-id="1c92d-183">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="1c92d-184">**Iş Ortağı Merkezi** menüsünden **müşteriler** ' i seçin, taşımak istediğiniz müşteriyi seçin ve ardından **Abonelik Ekle** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="1c92d-184">From the **Partner Center** menu, select **Customers** , select the customer you wish to move, and then select **Add subscriptions** .</span></span>

2. <span data-ttu-id="1c92d-185">Katalogdan satın almak istediğiniz aboneliği seçin (Bu durumda yukarıdaki seçeneklerden biri), lisansların sayısını girin ve ardından **Gönder** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="1c92d-185">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit** .</span></span>

   <span data-ttu-id="1c92d-186">Müşterinizin artık eski ve yeni abonelikleri, eski Office 365 Enterprise E4 aboneliği ve yeni ' Target ' aboneliği olmalıdır; örneğin, 1-Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="1c92d-186">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="1c92d-187">2. adım-müşterinin kullanıcılarının lisanslarını yeniden atama</span><span class="sxs-lookup"><span data-stu-id="1c92d-187">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="1c92d-188">**Iş Ortağı Merkezi** menüsünden **müşteriler** ' i seçin, taşımak istediğiniz müşteriyi seçin ve ardından **Kullanıcılar ve lisanslar** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="1c92d-188">From the **Partner Center** menu, select **Customers** , select the customer you wish to move, and then select **Users and licenses** .</span></span> <span data-ttu-id="1c92d-189">Müşterinin kullanıcılar ve lisanslar sayfası açılır.</span><span class="sxs-lookup"><span data-stu-id="1c92d-189">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="1c92d-190">Kullanıcı lisanslarını yeniden atamak için, yeniden atanacak kullanıcıyı seçin ve ardından **Lisansları Yönet** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="1c92d-190">To re-assign user licenses, select the user to reassign and then select **Manage licenses** .</span></span>

3. <span data-ttu-id="1c92d-191">**Lisansları Yönet** sayfasında, **Office 365 Kurumsal E4** Lisansı onay kutusunu temizleyin ve müşterinin taşınmakta olduğu abonelik için yeni bir hizmet planı seçin.</span><span class="sxs-lookup"><span data-stu-id="1c92d-191">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="1c92d-192">**Gönder** ’i seçin.</span><span class="sxs-lookup"><span data-stu-id="1c92d-192">Select **Submit** .</span></span> <span data-ttu-id="1c92d-193">Bir onay sayfası yeni lisans atamalarını listeler.</span><span class="sxs-lookup"><span data-stu-id="1c92d-193">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="1c92d-194">Lisans yeniden ataması gerektiren diğer müşteri kullanıcılarıyla aynı adımlara devam edin.</span><span class="sxs-lookup"><span data-stu-id="1c92d-194">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="1c92d-195">Kullanıcı lisanslarını yeni hizmete taşıdıktan sonra, kullanımdan kaldırılan aboneliği en üst müşteri düzeyinde güvenle iptal edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1c92d-195">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="1c92d-196">3. adım-eski aboneliği Iptal et</span><span class="sxs-lookup"><span data-stu-id="1c92d-196">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="1c92d-197">**Iş Ortağı Merkezi** menüsünde **müşteriler** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="1c92d-197">From the **Partner Center** menu, select **Customers** .</span></span> <span data-ttu-id="1c92d-198">Taşımak istediğiniz müşteriyi seçin ve iptal etmek istediğiniz aboneliği seçin.</span><span class="sxs-lookup"><span data-stu-id="1c92d-198">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="1c92d-199">Abonelik Ayrıntıları sayfasında, abonelik durumunu **askıya alındı** olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="1c92d-199">In the subscription details page, set the subscription status to **Suspended** .</span></span>

3. <span data-ttu-id="1c92d-200">**Gönder** ’i seçin.</span><span class="sxs-lookup"><span data-stu-id="1c92d-200">Select **Submit** .</span></span>

<span data-ttu-id="1c92d-201">Eski abonelik askıya alındı ve yeni abonelik etkin.</span><span class="sxs-lookup"><span data-stu-id="1c92d-201">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="1c92d-202">Askıya alınan abonelik 120 gün sonra otomatik olarak sağlanacaktır.</span><span class="sxs-lookup"><span data-stu-id="1c92d-202">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="1c92d-203">Müşteri, eski abonelik için ek maliyet içermez.</span><span class="sxs-lookup"><span data-stu-id="1c92d-203">The customer incurs no additional costs for the old subscription.</span></span>



 



