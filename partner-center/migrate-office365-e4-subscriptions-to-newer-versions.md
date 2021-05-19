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
ms.openlocfilehash: f738ddace805838cdf202c23cca8535c11cbdf54
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151568"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="eac36-104">Office 365 E4 aboneliklerini yeni Office 365 sürümlerine geçirme</span><span class="sxs-lookup"><span data-stu-id="eac36-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="eac36-105">**Uygun roller**: genel yönetici | Kullanıcı Yönetimi Yöneticisi | Yönetici Aracısı | Satış Aracısı</span><span class="sxs-lookup"><span data-stu-id="eac36-105">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="eac36-106">Office 365 Enterprise E4 planı kullanımdan kalkmışsa, 7 Nisan 2017 ' de geçerli değildir.</span><span class="sxs-lookup"><span data-stu-id="eac36-106">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="eac36-107">Bu tarihten sonra yeni Office 365 E4 abonelikleri satın alınmaz ve var olan E4 abonelikleri süreleri dolduğunda otomatik olarak yenilenmeyecektir.</span><span class="sxs-lookup"><span data-stu-id="eac36-107">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="eac36-108">E4 abonelikleri sona erdirmek için iptal edilir.</span><span class="sxs-lookup"><span data-stu-id="eac36-108">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="eac36-109">Müşterilerin devamlılığını sağlamak için, süresi dolan E4 abonelikleriyle müşterileri aşağıda listelenen desteklenen bir SKU seçeneğine geçirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="eac36-109">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="eac36-110">Müşterilerin hizmet kesintilerinden kaçınmak için, aboneliğin yıllık bitiş tarihinden önce müşterileri yeni aboneliklere taşımayı öneririz.</span><span class="sxs-lookup"><span data-stu-id="eac36-110">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="eac36-111">Hem Office 365 Enterprise E4 ticari hem de kamu SKU 'Ları devre dışı bırakıldı.</span><span class="sxs-lookup"><span data-stu-id="eac36-111">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="eac36-112">Aboneliğin ayrıntı sayfasında, E4 abonelik durumu "otomatik yenilemede [Tarih]" içinde "süre sonu" olarak değiştirildi.</span><span class="sxs-lookup"><span data-stu-id="eac36-112">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="eac36-113">API 'YI (CREST veya Partner Center) kullanıyorsanız, Otomatik Yenile = false özelliğiyle birlikte Aboneliğin bitiş tarihini değerlendirerek süresi dolan abonelikleri bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="eac36-113">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="eac36-114">E4 abonelikleri, 7 Nisan 2017 ' de Otomatik Yenile = false olarak ayarlanacak.</span><span class="sxs-lookup"><span data-stu-id="eac36-114">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="eac36-115">Müşterileri dilediğiniz zaman yeni bir plana taşıyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="eac36-115">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="eac36-116">Office 365 Enterprise E4 Edition değiştirme planları</span><span class="sxs-lookup"><span data-stu-id="eac36-116">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="eac36-117">E4 ile aynı işlevselliği korumayı seçebilirsiniz veya müşterilerinizin Office 365 ve Skype Kurumsal Çevrimiçi sürüm 'deki yeni özellik ve işlevlerden faydalanmasını sağlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="eac36-117">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="eac36-118">Fiyatlandırma ayrıntıları, Iş Ortağı Merkezi 'nde fiyat listesi ve teklif listesi matrisinde bulunur.</span><span class="sxs-lookup"><span data-stu-id="eac36-118">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="eac36-119">Güvenli ürün Kurumsal E3 veya güvenli üretkenlik Kurumsal E5, sırasıyla Office 365 Enterprise E3 veya Office 365 Kurumsal E5 için aşağıdaki seçenekler yerine kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="eac36-119">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="eac36-120">Seçenek 1: Office 365 Kurumsal E5</span><span class="sxs-lookup"><span data-stu-id="eac36-120">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="eac36-121">Seçenek 2: Office 365 Enterprise E3 + Skype Kurumsal Bulut PBX</span><span class="sxs-lookup"><span data-stu-id="eac36-121">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="eac36-122">3. Seçenek: Office 365 Kurumsal E3 + Skype Kurumsal Plus CAL (E4 ile fiyat ve işlevsellik eşlik)</span><span class="sxs-lookup"><span data-stu-id="eac36-122">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="eac36-123">4. Seçenek: Office 365 Kurumsal E3</span><span class="sxs-lookup"><span data-stu-id="eac36-123">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="eac36-124">Özellik</span><span class="sxs-lookup"><span data-stu-id="eac36-124">Feature</span></span> | <span data-ttu-id="eac36-125">1\. Seçenek</span><span class="sxs-lookup"><span data-stu-id="eac36-125">Option 1</span></span> | <span data-ttu-id="eac36-126">2\. Seçenek</span><span class="sxs-lookup"><span data-stu-id="eac36-126">Option 2</span></span> | <span data-ttu-id="eac36-127">3. Seçenek</span><span class="sxs-lookup"><span data-stu-id="eac36-127">Option 3</span></span> | <span data-ttu-id="eac36-128">4. Seçenek</span><span class="sxs-lookup"><span data-stu-id="eac36-128">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="eac36-129">Office 365 Kurumsal E4'e dahil olan tüm özellikleri alıyor musunuz?</span><span class="sxs-lookup"><span data-stu-id="eac36-129">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="eac36-130">Yes</span><span class="sxs-lookup"><span data-stu-id="eac36-130">Yes</span></span> | <span data-ttu-id="eac36-131">Yes</span><span class="sxs-lookup"><span data-stu-id="eac36-131">Yes</span></span> | <span data-ttu-id="eac36-132">Yes</span><span class="sxs-lookup"><span data-stu-id="eac36-132">Yes</span></span> | <span data-ttu-id="eac36-133">Hayır</span><span class="sxs-lookup"><span data-stu-id="eac36-133">No</span></span> |
| <span data-ttu-id="eac36-134">Office 365'te yönetilen telefon numaraları</span><span class="sxs-lookup"><span data-stu-id="eac36-134">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="eac36-135">Yes</span><span class="sxs-lookup"><span data-stu-id="eac36-135">Yes</span></span> | <span data-ttu-id="eac36-136">Yes</span><span class="sxs-lookup"><span data-stu-id="eac36-136">Yes</span></span> | <span data-ttu-id="eac36-137">Hayır</span><span class="sxs-lookup"><span data-stu-id="eac36-137">No</span></span> | <span data-ttu-id="eac36-138">Hayır</span><span class="sxs-lookup"><span data-stu-id="eac36-138">No</span></span> |
| <span data-ttu-id="eac36-139">Hem şirket içinde hem de Office 365'te (karma dağıtım) yönetilen telefon numaraları?</span><span class="sxs-lookup"><span data-stu-id="eac36-139">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="eac36-140">Yes</span><span class="sxs-lookup"><span data-stu-id="eac36-140">Yes</span></span> | <span data-ttu-id="eac36-141">Yes</span><span class="sxs-lookup"><span data-stu-id="eac36-141">Yes</span></span> | <span data-ttu-id="eac36-142">Hayır</span><span class="sxs-lookup"><span data-stu-id="eac36-142">No</span></span> | <span data-ttu-id="eac36-143">Hayır</span><span class="sxs-lookup"><span data-stu-id="eac36-143">No</span></span> |
| <span data-ttu-id="eac36-144">PSTN sesli arama planı ekleme seçeneği var mı?</span><span class="sxs-lookup"><span data-stu-id="eac36-144">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="eac36-145">Yes</span><span class="sxs-lookup"><span data-stu-id="eac36-145">Yes</span></span> | <span data-ttu-id="eac36-146">Yes</span><span class="sxs-lookup"><span data-stu-id="eac36-146">Yes</span></span> | <span data-ttu-id="eac36-147">Hayır</span><span class="sxs-lookup"><span data-stu-id="eac36-147">No</span></span> | <span data-ttu-id="eac36-148">Hayır</span><span class="sxs-lookup"><span data-stu-id="eac36-148">No</span></span> |
| <span data-ttu-id="eac36-149">PSTN Konferans?</span><span class="sxs-lookup"><span data-stu-id="eac36-149">PSTN Conferencing?</span></span> | <span data-ttu-id="eac36-150">Yes</span><span class="sxs-lookup"><span data-stu-id="eac36-150">Yes</span></span> | <span data-ttu-id="eac36-151">Hayır</span><span class="sxs-lookup"><span data-stu-id="eac36-151">No</span></span> | <span data-ttu-id="eac36-152">Hayır</span><span class="sxs-lookup"><span data-stu-id="eac36-152">No</span></span> | <span data-ttu-id="eac36-153">Hayır</span><span class="sxs-lookup"><span data-stu-id="eac36-153">No</span></span> |
| <span data-ttu-id="eac36-154">İşbirliği, analiz ve güvenlik için gelişmiş araçlar?</span><span class="sxs-lookup"><span data-stu-id="eac36-154">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="eac36-155">Yes</span><span class="sxs-lookup"><span data-stu-id="eac36-155">Yes</span></span> | <span data-ttu-id="eac36-156">Hayır</span><span class="sxs-lookup"><span data-stu-id="eac36-156">No</span></span> | <span data-ttu-id="eac36-157">Hayır</span><span class="sxs-lookup"><span data-stu-id="eac36-157">No</span></span> | <span data-ttu-id="eac36-158">Hayır</span><span class="sxs-lookup"><span data-stu-id="eac36-158">No</span></span> |
| <span data-ttu-id="eac36-159">Etkileşimli raporlar, panolar ve veri görselleştirmeleri?</span><span class="sxs-lookup"><span data-stu-id="eac36-159">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="eac36-160">Yes</span><span class="sxs-lookup"><span data-stu-id="eac36-160">Yes</span></span> | <span data-ttu-id="eac36-161">Hayır</span><span class="sxs-lookup"><span data-stu-id="eac36-161">No</span></span> | <span data-ttu-id="eac36-162">Hayır</span><span class="sxs-lookup"><span data-stu-id="eac36-162">No</span></span> | <span data-ttu-id="eac36-163">Hayır</span><span class="sxs-lookup"><span data-stu-id="eac36-163">No</span></span> | 
| <span data-ttu-id="eac36-164">Yerleşik gizlilik, saydamlık ve iyileştirilmiş kullanıcı denetimleriyle veri güvenliği ve uyumluluğu üzerinde daha fazla denetime sahip misiniz?</span><span class="sxs-lookup"><span data-stu-id="eac36-164">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="eac36-165">Yes</span><span class="sxs-lookup"><span data-stu-id="eac36-165">Yes</span></span> | <span data-ttu-id="eac36-166">Hayır</span><span class="sxs-lookup"><span data-stu-id="eac36-166">No</span></span> | <span data-ttu-id="eac36-167">Hayır</span><span class="sxs-lookup"><span data-stu-id="eac36-167">No</span></span> | <span data-ttu-id="eac36-168">Hayır</span><span class="sxs-lookup"><span data-stu-id="eac36-168">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="eac36-169">Müşterileri yeni ürün planlarına geçiş</span><span class="sxs-lookup"><span data-stu-id="eac36-169">Transition customers to new product plans</span></span>

<span data-ttu-id="eac36-170">Microsoft, iş ortaklarımıza sürekli olarak yeni ürün ve hizmetler sunmaktadır.</span><span class="sxs-lookup"><span data-stu-id="eac36-170">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="eac36-171">Bu durumlarda, müşterileri yeni hizmetlere yükseltmeniz veya aboneliklerini sonunda kapatılacak olan SKUS'lardan geçirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="eac36-171">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="eac36-172">Müşterileri, eski SKÜ'lerden yeni SKUS'lara şu adımların atılması gerekir:</span><span class="sxs-lookup"><span data-stu-id="eac36-172">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="eac36-173">Yeni aboneliği satın alma</span><span class="sxs-lookup"><span data-stu-id="eac36-173">Purchase the new subscription</span></span>
-   <span data-ttu-id="eac36-174">Geçerli kullanıcı lisanslarını yeniden atama</span><span class="sxs-lookup"><span data-stu-id="eac36-174">Reassign current user licenses</span></span>
-   <span data-ttu-id="eac36-175">Eski aboneliği iptal etme</span><span class="sxs-lookup"><span data-stu-id="eac36-175">Cancel the old subscription</span></span>

<span data-ttu-id="eac36-176">Müşterinin Office 365 Kurumsal E4 aboneliğini yukarıdaki tabloda yer alan seçeneklerden biri olarak geçirmek için bu adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="eac36-176">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="eac36-177">1. adım-yeni aboneliği satın alma</span><span class="sxs-lookup"><span data-stu-id="eac36-177">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="eac36-178">**Iş Ortağı Merkezi** menüsünden **müşteriler**' i seçin, taşımak istediğiniz müşteriyi seçin ve ardından **Abonelik Ekle**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="eac36-178">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="eac36-179">Katalogdan satın almak istediğiniz aboneliği seçin (Bu durumda yukarıdaki seçeneklerden biri), lisansların sayısını girin ve ardından **Gönder**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="eac36-179">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="eac36-180">Müşterinizin artık eski ve yeni abonelikleri, eski Office 365 Enterprise E4 aboneliği ve yeni ' Target ' aboneliği olmalıdır; örneğin, 1-Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="eac36-180">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="eac36-181">2. adım-müşterinin kullanıcılarının lisanslarını yeniden atama</span><span class="sxs-lookup"><span data-stu-id="eac36-181">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="eac36-182">**Iş Ortağı Merkezi** menüsünden **müşteriler**' i seçin, taşımak istediğiniz müşteriyi seçin ve ardından **Kullanıcılar ve lisanslar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="eac36-182">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="eac36-183">Müşterinin kullanıcılar ve lisanslar sayfası açılır.</span><span class="sxs-lookup"><span data-stu-id="eac36-183">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="eac36-184">Kullanıcı lisanslarını yeniden atamak için, yeniden atanacak kullanıcıyı seçin ve ardından **Lisansları Yönet**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="eac36-184">To reassign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="eac36-185">**Lisansları Yönet** sayfasında, **Office 365 Kurumsal E4** Lisansı onay kutusunu temizleyin ve müşterinin taşınmakta olduğu abonelik için yeni bir hizmet planı seçin.</span><span class="sxs-lookup"><span data-stu-id="eac36-185">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="eac36-186">**Gönder**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="eac36-186">Select **Submit**.</span></span> <span data-ttu-id="eac36-187">Bir onay sayfası yeni lisans atamalarını listeler.</span><span class="sxs-lookup"><span data-stu-id="eac36-187">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="eac36-188">Lisans yeniden ataması gerektiren diğer müşteri kullanıcılarıyla aynı adımlara devam edin.</span><span class="sxs-lookup"><span data-stu-id="eac36-188">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="eac36-189">Kullanıcı lisanslarını yeni hizmete taşıdıktan sonra, kullanımdan kaldırılan aboneliği en üst müşteri düzeyinde güvenle iptal edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="eac36-189">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="eac36-190">3. adım-eski aboneliği Iptal et</span><span class="sxs-lookup"><span data-stu-id="eac36-190">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="eac36-191">**Iş Ortağı Merkezi** menüsünde **müşteriler**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="eac36-191">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="eac36-192">Taşımak istediğiniz müşteriyi seçin ve iptal etmek istediğiniz aboneliği seçin.</span><span class="sxs-lookup"><span data-stu-id="eac36-192">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="eac36-193">Abonelik Ayrıntıları sayfasında, abonelik durumunu **askıya alındı** olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="eac36-193">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="eac36-194">**Gönder**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="eac36-194">Select **Submit**.</span></span>

<span data-ttu-id="eac36-195">Eski abonelik askıya alındı ve yeni abonelik etkin.</span><span class="sxs-lookup"><span data-stu-id="eac36-195">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="eac36-196">Askıya alınan abonelik 120 gün sonra otomatik olarak sağlanacaktır.</span><span class="sxs-lookup"><span data-stu-id="eac36-196">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="eac36-197">Müşteri, eski abonelik için ek maliyet içermez.</span><span class="sxs-lookup"><span data-stu-id="eac36-197">The customer incurs no additional costs for the old subscription.</span></span>



 



