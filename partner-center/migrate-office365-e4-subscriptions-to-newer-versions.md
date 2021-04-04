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
ms.openlocfilehash: 8a9662e0ce99fc054149dfbd4149532ce336eff6
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132630"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="ff888-104">Office 365 E4 aboneliklerini yeni Office 365 sürümlerine geçirme</span><span class="sxs-lookup"><span data-stu-id="ff888-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="ff888-105">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="ff888-105">**Appropriate roles**</span></span>

- <span data-ttu-id="ff888-106">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="ff888-106">Global admin</span></span>
- <span data-ttu-id="ff888-107">Kullanıcı Yönetimi Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="ff888-107">User management admin</span></span>
- <span data-ttu-id="ff888-108">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="ff888-108">Admin agent</span></span>
- <span data-ttu-id="ff888-109">Satış Aracısı</span><span class="sxs-lookup"><span data-stu-id="ff888-109">Sales agent</span></span>

<span data-ttu-id="ff888-110">Office 365 Enterprise E4 planı kullanımdan kalkmışsa, 7 Nisan 2017 ' de geçerli değildir.</span><span class="sxs-lookup"><span data-stu-id="ff888-110">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="ff888-111">Bu tarihten sonra yeni Office 365 E4 abonelikleri satın alınmaz ve var olan E4 abonelikleri süreleri dolduğunda otomatik olarak yenilenmeyecektir.</span><span class="sxs-lookup"><span data-stu-id="ff888-111">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="ff888-112">E4 abonelikleri sona erdirmek için iptal edilir.</span><span class="sxs-lookup"><span data-stu-id="ff888-112">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="ff888-113">Müşterilerin devamlılığını sağlamak için, süresi dolan E4 abonelikleriyle müşterileri aşağıda listelenen desteklenen bir SKU seçeneğine geçirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="ff888-113">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="ff888-114">Müşterilerin hizmet kesintilerinden kaçınmak için, aboneliğin yıllık bitiş tarihinden önce müşterileri yeni aboneliklere taşımayı öneririz.</span><span class="sxs-lookup"><span data-stu-id="ff888-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="ff888-115">Hem Office 365 Enterprise E4 ticari hem de kamu SKU 'Ları devre dışı bırakıldı.</span><span class="sxs-lookup"><span data-stu-id="ff888-115">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="ff888-116">Aboneliğin ayrıntı sayfasında, E4 abonelik durumu "otomatik yenilemede [Tarih]" içinde "süre sonu" olarak değiştirildi.</span><span class="sxs-lookup"><span data-stu-id="ff888-116">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="ff888-117">API 'YI (CREST veya Partner Center) kullanıyorsanız, Otomatik Yenile = false özelliğiyle birlikte Aboneliğin bitiş tarihini değerlendirerek süresi dolan abonelikleri bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ff888-117">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="ff888-118">E4 abonelikleri, 7 Nisan 2017 ' de Otomatik Yenile = false olarak ayarlanacak.</span><span class="sxs-lookup"><span data-stu-id="ff888-118">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="ff888-119">Müşterileri dilediğiniz zaman yeni bir plana taşıyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ff888-119">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="ff888-120">Office 365 Enterprise E4 Edition değiştirme planları</span><span class="sxs-lookup"><span data-stu-id="ff888-120">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="ff888-121">E4 ile aynı işlevselliği korumayı seçebilirsiniz veya müşterilerinizin Office 365 ve Skype Kurumsal Çevrimiçi sürüm 'deki yeni özellik ve işlevlerden faydalanmasını sağlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ff888-121">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="ff888-122">Fiyatlandırma ayrıntıları, Iş Ortağı Merkezi 'nde fiyat listesi ve teklif listesi matrisinde bulunur.</span><span class="sxs-lookup"><span data-stu-id="ff888-122">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="ff888-123">Güvenli ürün Kurumsal E3 veya güvenli üretkenlik Kurumsal E5, sırasıyla Office 365 Enterprise E3 veya Office 365 Kurumsal E5 için aşağıdaki seçenekler yerine kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="ff888-123">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="ff888-124">Seçenek 1: Office 365 Kurumsal E5</span><span class="sxs-lookup"><span data-stu-id="ff888-124">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="ff888-125">Seçenek 2: Office 365 Enterprise E3 + Skype Kurumsal Bulut PBX</span><span class="sxs-lookup"><span data-stu-id="ff888-125">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="ff888-126">Seçenek 3: Office 365 Enterprise E3 + Skype Kurumsal Plus CAL (E4 ile fiyat ve işlev eşliği)</span><span class="sxs-lookup"><span data-stu-id="ff888-126">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="ff888-127">4. seçenek: Office 365 Kurumsal E3</span><span class="sxs-lookup"><span data-stu-id="ff888-127">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="ff888-128">Özellik</span><span class="sxs-lookup"><span data-stu-id="ff888-128">Feature</span></span> | <span data-ttu-id="ff888-129">1\. Seçenek</span><span class="sxs-lookup"><span data-stu-id="ff888-129">Option 1</span></span> | <span data-ttu-id="ff888-130">2\. Seçenek</span><span class="sxs-lookup"><span data-stu-id="ff888-130">Option 2</span></span> | <span data-ttu-id="ff888-131">Seçenek 3</span><span class="sxs-lookup"><span data-stu-id="ff888-131">Option 3</span></span> | <span data-ttu-id="ff888-132">4 seçeneği</span><span class="sxs-lookup"><span data-stu-id="ff888-132">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="ff888-133">Office 365 Kurumsal E4 'ye dahil olan tüm özellikler mi alınır?</span><span class="sxs-lookup"><span data-stu-id="ff888-133">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="ff888-134">Yes</span><span class="sxs-lookup"><span data-stu-id="ff888-134">Yes</span></span> | <span data-ttu-id="ff888-135">Yes</span><span class="sxs-lookup"><span data-stu-id="ff888-135">Yes</span></span> | <span data-ttu-id="ff888-136">Yes</span><span class="sxs-lookup"><span data-stu-id="ff888-136">Yes</span></span> | <span data-ttu-id="ff888-137">Hayır</span><span class="sxs-lookup"><span data-stu-id="ff888-137">No</span></span> |
| <span data-ttu-id="ff888-138">Office 365 ' de yönetilen telefon numaraları?</span><span class="sxs-lookup"><span data-stu-id="ff888-138">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="ff888-139">Yes</span><span class="sxs-lookup"><span data-stu-id="ff888-139">Yes</span></span> | <span data-ttu-id="ff888-140">Yes</span><span class="sxs-lookup"><span data-stu-id="ff888-140">Yes</span></span> | <span data-ttu-id="ff888-141">Hayır</span><span class="sxs-lookup"><span data-stu-id="ff888-141">No</span></span> | <span data-ttu-id="ff888-142">Hayır</span><span class="sxs-lookup"><span data-stu-id="ff888-142">No</span></span> |
| <span data-ttu-id="ff888-143">Telefon numaraları hem şirket içinde hem de Office 365 ' de (karma dağıtım) yönetiliyor mu?</span><span class="sxs-lookup"><span data-stu-id="ff888-143">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="ff888-144">Yes</span><span class="sxs-lookup"><span data-stu-id="ff888-144">Yes</span></span> | <span data-ttu-id="ff888-145">Yes</span><span class="sxs-lookup"><span data-stu-id="ff888-145">Yes</span></span> | <span data-ttu-id="ff888-146">Hayır</span><span class="sxs-lookup"><span data-stu-id="ff888-146">No</span></span> | <span data-ttu-id="ff888-147">Hayır</span><span class="sxs-lookup"><span data-stu-id="ff888-147">No</span></span> |
| <span data-ttu-id="ff888-148">PSTN sesli arama planı ekleme seçeneği</span><span class="sxs-lookup"><span data-stu-id="ff888-148">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="ff888-149">Yes</span><span class="sxs-lookup"><span data-stu-id="ff888-149">Yes</span></span> | <span data-ttu-id="ff888-150">Yes</span><span class="sxs-lookup"><span data-stu-id="ff888-150">Yes</span></span> | <span data-ttu-id="ff888-151">Hayır</span><span class="sxs-lookup"><span data-stu-id="ff888-151">No</span></span> | <span data-ttu-id="ff888-152">Hayır</span><span class="sxs-lookup"><span data-stu-id="ff888-152">No</span></span> |
| <span data-ttu-id="ff888-153">PSTN Konferansı?</span><span class="sxs-lookup"><span data-stu-id="ff888-153">PSTN Conferencing?</span></span> | <span data-ttu-id="ff888-154">Yes</span><span class="sxs-lookup"><span data-stu-id="ff888-154">Yes</span></span> | <span data-ttu-id="ff888-155">Hayır</span><span class="sxs-lookup"><span data-stu-id="ff888-155">No</span></span> | <span data-ttu-id="ff888-156">Hayır</span><span class="sxs-lookup"><span data-stu-id="ff888-156">No</span></span> | <span data-ttu-id="ff888-157">Hayır</span><span class="sxs-lookup"><span data-stu-id="ff888-157">No</span></span> |
| <span data-ttu-id="ff888-158">İşbirliği, analiz ve güvenlik için gelişmiş araçlar?</span><span class="sxs-lookup"><span data-stu-id="ff888-158">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="ff888-159">Yes</span><span class="sxs-lookup"><span data-stu-id="ff888-159">Yes</span></span> | <span data-ttu-id="ff888-160">Hayır</span><span class="sxs-lookup"><span data-stu-id="ff888-160">No</span></span> | <span data-ttu-id="ff888-161">Hayır</span><span class="sxs-lookup"><span data-stu-id="ff888-161">No</span></span> | <span data-ttu-id="ff888-162">Hayır</span><span class="sxs-lookup"><span data-stu-id="ff888-162">No</span></span> |
| <span data-ttu-id="ff888-163">Etkileşimli raporlar, panolar ve veri görselleştirmeleri?</span><span class="sxs-lookup"><span data-stu-id="ff888-163">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="ff888-164">Yes</span><span class="sxs-lookup"><span data-stu-id="ff888-164">Yes</span></span> | <span data-ttu-id="ff888-165">Hayır</span><span class="sxs-lookup"><span data-stu-id="ff888-165">No</span></span> | <span data-ttu-id="ff888-166">Hayır</span><span class="sxs-lookup"><span data-stu-id="ff888-166">No</span></span> | <span data-ttu-id="ff888-167">Hayır</span><span class="sxs-lookup"><span data-stu-id="ff888-167">No</span></span> | 
| <span data-ttu-id="ff888-168">Yerleşik gizlilik, saydamlık ve iyileştirilmiş Kullanıcı denetimleriyle veri güvenliği ve uyumluluk üzerinde daha fazla denetim var mı?</span><span class="sxs-lookup"><span data-stu-id="ff888-168">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="ff888-169">Yes</span><span class="sxs-lookup"><span data-stu-id="ff888-169">Yes</span></span> | <span data-ttu-id="ff888-170">Hayır</span><span class="sxs-lookup"><span data-stu-id="ff888-170">No</span></span> | <span data-ttu-id="ff888-171">Hayır</span><span class="sxs-lookup"><span data-stu-id="ff888-171">No</span></span> | <span data-ttu-id="ff888-172">Hayır</span><span class="sxs-lookup"><span data-stu-id="ff888-172">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="ff888-173">Müşterilerin yeni ürün planlarına geçişini sağlar</span><span class="sxs-lookup"><span data-stu-id="ff888-173">Transition customers to new product plans</span></span>

<span data-ttu-id="ff888-174">Microsoft, iş ortaklarımız için sürekli olarak yeni ürün ve hizmetler sunar.</span><span class="sxs-lookup"><span data-stu-id="ff888-174">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="ff888-175">Bu gibi durumlarda, müşterileri yeni hizmetlere yükseltmeniz veya sonunda kapatılacak SKU 'lardan aboneliklerini geçirmeniz gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="ff888-175">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="ff888-176">Müşterilerin Kullanımdan kaldırılmış SKU 'lardan daha yeni bir sürümüne geçirilmesi aşağıdaki adımları gerektirir:</span><span class="sxs-lookup"><span data-stu-id="ff888-176">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="ff888-177">Yeni aboneliği satın alın</span><span class="sxs-lookup"><span data-stu-id="ff888-177">Purchase the new subscription</span></span>
-   <span data-ttu-id="ff888-178">Geçerli kullanıcı lisanslarını yeniden ata</span><span class="sxs-lookup"><span data-stu-id="ff888-178">Reassign current user licenses</span></span>
-   <span data-ttu-id="ff888-179">Eski aboneliği iptal et</span><span class="sxs-lookup"><span data-stu-id="ff888-179">Cancel the old subscription</span></span>

<span data-ttu-id="ff888-180">Müşterinin Office 365 Kurumsal E4 aboneliğini Yukarıdaki tablodaki seçeneklerden birine geçirmek için aşağıdaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="ff888-180">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="ff888-181">1. adım-yeni aboneliği satın alma</span><span class="sxs-lookup"><span data-stu-id="ff888-181">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="ff888-182">**Iş Ortağı Merkezi** menüsünden **müşteriler**' i seçin, taşımak istediğiniz müşteriyi seçin ve ardından **Abonelik Ekle**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="ff888-182">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="ff888-183">Katalogdan satın almak istediğiniz aboneliği seçin (Bu durumda yukarıdaki seçeneklerden biri), lisansların sayısını girin ve ardından **Gönder**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="ff888-183">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="ff888-184">Müşterinizin artık eski ve yeni abonelikleri, eski Office 365 Enterprise E4 aboneliği ve yeni ' Target ' aboneliği olmalıdır; örneğin, 1-Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="ff888-184">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="ff888-185">2. adım-müşterinin kullanıcılarının lisanslarını yeniden atama</span><span class="sxs-lookup"><span data-stu-id="ff888-185">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="ff888-186">**Iş Ortağı Merkezi** menüsünden **müşteriler**' i seçin, taşımak istediğiniz müşteriyi seçin ve ardından **Kullanıcılar ve lisanslar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="ff888-186">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="ff888-187">Müşterinin kullanıcılar ve lisanslar sayfası açılır.</span><span class="sxs-lookup"><span data-stu-id="ff888-187">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="ff888-188">Kullanıcı lisanslarını yeniden atamak için, yeniden atanacak kullanıcıyı seçin ve ardından **Lisansları Yönet**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="ff888-188">To reassign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="ff888-189">**Lisansları Yönet** sayfasında, **Office 365 Kurumsal E4** Lisansı onay kutusunu temizleyin ve müşterinin taşınmakta olduğu abonelik için yeni bir hizmet planı seçin.</span><span class="sxs-lookup"><span data-stu-id="ff888-189">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="ff888-190">**Gönder**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="ff888-190">Select **Submit**.</span></span> <span data-ttu-id="ff888-191">Bir onay sayfası yeni lisans atamalarını listeler.</span><span class="sxs-lookup"><span data-stu-id="ff888-191">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="ff888-192">Lisans yeniden ataması gerektiren diğer müşteri kullanıcılarıyla aynı adımlara devam edin.</span><span class="sxs-lookup"><span data-stu-id="ff888-192">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="ff888-193">Kullanıcı lisanslarını yeni hizmete taşıdıktan sonra, kullanımdan kaldırılan aboneliği en üst müşteri düzeyinde güvenle iptal edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ff888-193">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="ff888-194">3. adım-eski aboneliği Iptal et</span><span class="sxs-lookup"><span data-stu-id="ff888-194">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="ff888-195">**Iş Ortağı Merkezi** menüsünde **müşteriler**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="ff888-195">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="ff888-196">Taşımak istediğiniz müşteriyi seçin ve iptal etmek istediğiniz aboneliği seçin.</span><span class="sxs-lookup"><span data-stu-id="ff888-196">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="ff888-197">Abonelik Ayrıntıları sayfasında, abonelik durumunu **askıya alındı** olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="ff888-197">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="ff888-198">**Gönder**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="ff888-198">Select **Submit**.</span></span>

<span data-ttu-id="ff888-199">Eski abonelik askıya alındı ve yeni abonelik etkin.</span><span class="sxs-lookup"><span data-stu-id="ff888-199">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="ff888-200">Askıya alınan abonelik 120 gün sonra otomatik olarak sağlanacaktır.</span><span class="sxs-lookup"><span data-stu-id="ff888-200">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="ff888-201">Müşteri, eski abonelik için ek maliyet içermez.</span><span class="sxs-lookup"><span data-stu-id="ff888-201">The customer incurs no additional costs for the old subscription.</span></span>



 



