---
title: Market teklifte lisanslamayı yönetme
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: ISV ticari Market tekliflerinizi için lisanslamayı ayarlamayı ve yönetmeyi öğrenin.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c128b99b034564bcaa100ca975253f8b1bad7a42
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147964"
---
# <a name="manage-licensing-in-marketplace-offers"></a><span data-ttu-id="ad5a2-103">Market teklifte lisanslamayı yönetme</span><span class="sxs-lookup"><span data-stu-id="ad5a2-103">Manage licensing in marketplace offers</span></span>

<span data-ttu-id="ad5a2-104">**Uygun roller**: genel yönetici | Hesap Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="ad5a2-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="ad5a2-105">Bu makalede, Iş Ortağı Merkezi 'nde bir teklif ayarlama, Microsoft AppSource ' de kullanılabilir hale getirme ve ardından bu teklifin lisanslarını yönetme sürecinde size yol gösterilir.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-105">This article walks you through the process of setting up an offer in Partner Center, making it available in Microsoft AppSource, and then managing licenses for that offer.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="ad5a2-106">Bu makaledeki yetenekler Şu anda genel önizlemededir.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-106">The capabilities in this article are currently in Public Preview.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="ad5a2-107">Başlamadan önce</span><span class="sxs-lookup"><span data-stu-id="ad5a2-107">Before you begin</span></span>

### <a name="commercial-marketplace-basics"></a><span data-ttu-id="ad5a2-108">Ticari Market temelleri</span><span class="sxs-lookup"><span data-stu-id="ad5a2-108">Commercial marketplace basics</span></span>

<span data-ttu-id="ad5a2-109">Bu işleme başlamadan önce, ticari Market 'in temelleri hakkında bilgi almalısınız.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-109">Before you begin this process, you should familiarize yourself with the basics of the commercial marketplace.</span></span> <span data-ttu-id="ad5a2-110">Aşağıdaki tablodaki makaleler başlamanıza yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-110">The articles in the table below will help get you started.</span></span> 

| <span data-ttu-id="ad5a2-111">Konu</span><span class="sxs-lookup"><span data-stu-id="ad5a2-111">Topic</span></span>  | <span data-ttu-id="ad5a2-112">Makale</span><span class="sxs-lookup"><span data-stu-id="ad5a2-112">Article</span></span>  |
|-------|--------|
|<span data-ttu-id="ad5a2-113">Ticari Market planları</span><span class="sxs-lookup"><span data-stu-id="ad5a2-113">Commercial marketplace plans</span></span> | [<span data-ttu-id="ad5a2-114">Ticari Market teklifleri için planlar ve fiyatlandırma</span><span class="sxs-lookup"><span data-stu-id="ad5a2-114">Plans and pricing for commercial marketplace offers</span></span>](/azure/marketplace/plans-pricing)    |
|<span data-ttu-id="ad5a2-115">Ticari Market teklifleri</span><span class="sxs-lookup"><span data-stu-id="ad5a2-115">Commercial marketplace offers</span></span>  | [<span data-ttu-id="ad5a2-116">Liste türleri</span><span class="sxs-lookup"><span data-stu-id="ad5a2-116">Listing types</span></span>](/azure/marketplace/determine-your-listing-type)    |
|<span data-ttu-id="ad5a2-117">Ticari Market hesapları</span><span class="sxs-lookup"><span data-stu-id="ad5a2-117">Commercial marketplace accounts</span></span> |  [<span data-ttu-id="ad5a2-118">Iş Ortağı Merkezi 'nde ticari Market hesabı oluşturma</span><span class="sxs-lookup"><span data-stu-id="ad5a2-118">Create a commercial marketplace account in Partner Center</span></span>](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a><span data-ttu-id="ad5a2-119">Teklif KIMLIĞINIZI belirleme</span><span class="sxs-lookup"><span data-stu-id="ad5a2-119">Determine your Offer ID</span></span>

<span data-ttu-id="ad5a2-120">Aşağıdaki yordamlarda bir teklif KIMLIĞI girmeniz istenir.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-120">In the procedures below, you’ll be prompted to enter an Offer ID.</span></span> <span data-ttu-id="ad5a2-121">Aşağıdaki noktaları göz önünde bulundurarak uygun bir teklif KIMLIĞIYLE karşılaşmaya biraz zaman atın:</span><span class="sxs-lookup"><span data-stu-id="ad5a2-121">Take some time now to come up with a suitable Offer ID, keeping in mind the following points:</span></span>

- <span data-ttu-id="ad5a2-122">Bu KIMLIK, varsa Market teklifi ve Azure Resource Manager şablonları için Web adresinde müşteriler tarafından görülebilir.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-122">This ID is visible to customers in the web address for the marketplace offer and Azure Resource Manager templates, if applicable.</span></span>
- <span data-ttu-id="ad5a2-123">Yayımcı KIMLIĞIYLE birleştirilmiş teklif KIMLIĞI, 40 karakter uzunluğunda olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-123">The Offer ID combined with the Publisher ID must be under 40 characters in length.</span></span>
- <span data-ttu-id="ad5a2-124">Yalnızca küçük harfleri ve rakamları kullanın.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-124">Use only lowercase letters and numbers.</span></span> <span data-ttu-id="ad5a2-125">Teklif Kimliği kısa çizgi ve alt çizgi içerebilir ancak boşluk içermez.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-125">The Offer ID can include hyphens and underscores, but no spaces.</span></span> <span data-ttu-id="ad5a2-126">Örneğin, Yayımcı Kimliğiniz ise ve `testpublisherid` `test-offer-1` girersiniz, teklif web adresi `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` olur.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-126">For example, if your Publisher ID is `testpublisherid` and you enter `test-offer-1`, the offer web address will be `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1`.</span></span>
- <span data-ttu-id="ad5a2-127">Oluştur'ı seçdikten sonra bu kimlik **değiştirilemez.**</span><span class="sxs-lookup"><span data-stu-id="ad5a2-127">This ID can't be changed after you select **Create**.</span></span>

### <a name="determine-your-offer-alias"></a><span data-ttu-id="ad5a2-128">Teklif diğer adını belirleme</span><span class="sxs-lookup"><span data-stu-id="ad5a2-128">Determine your Offer alias</span></span>

<span data-ttu-id="ad5a2-129">Teklif diğer adı, teklifte teklif için kullanılan İş Ortağı Merkezi.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-129">The Offer alias is the name used for the offer in Partner Center.</span></span> <span data-ttu-id="ad5a2-130">Ayrıca aşağıdaki yönergelere uygun bir Teklif diğer adı da gerekir:</span><span class="sxs-lookup"><span data-stu-id="ad5a2-130">You’ll also need an appropriate Offer alias that follows the guidelines below:</span></span>

- <span data-ttu-id="ad5a2-131">Bu ad markette kullanılmamaktadır ve müşterilere gösterilen teklif adı ile diğer değerlerden farklıdır.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-131">This name isn't used in the marketplace and is different from the offer name and other values shown to customers.</span></span>
- <span data-ttu-id="ad5a2-132">Oluştur'ı seçdikten sonra bu ad değiştirilemez.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-132">This name can't be changed after you select Create.</span></span>

## <a name="create-your-offer"></a><span data-ttu-id="ad5a2-133">Teklifinizi oluşturma</span><span class="sxs-lookup"><span data-stu-id="ad5a2-133">Create your offer</span></span>

<span data-ttu-id="ad5a2-134">Lisanslama sürecinin ilk adımı, ticari market teklifinizi oluşturmaktır.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-134">The first step in the licensing process is to create your commercial marketplace offer.</span></span> 

1. <span data-ttu-id="ad5a2-135">[İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-135">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="ad5a2-136">Sol gezinti menüsünde Ticari **Market/Genel Bakış'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="ad5a2-136">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="ad5a2-137">Genel Bakış sayfasının üst kısmında Yeni **teklif'i** seçin ve ardından **Dynamics 365 for Customer Engagement & PowerApps'i seçin.**</span><span class="sxs-lookup"><span data-stu-id="ad5a2-137">At the top of the Overview page, select **New offer**, and then select **Dynamics 365 for Customer Engagement & PowerApps**.</span></span>
4. <span data-ttu-id="ad5a2-138">Daha önce **oluşturduğunuz Teklif** Kimliği ve **Teklif diğer** adını girin.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-138">Enter the **Offer ID** and **Offer alias** you created earlier.</span></span>
5. <span data-ttu-id="ad5a2-139">Teklifi **oluşturmak ve** devam etmek için Oluştur'a seçin.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-139">Select **Create** to generate the offer and continue.</span></span>
6. <span data-ttu-id="ad5a2-140">Lisanslama seçeneklerinizi belirleyin.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-140">Choose your licensing options.</span></span>

    - <span data-ttu-id="ad5a2-141">Teklifiniz için lisans yönetimini etkinleştirmek için Microsoft aracılığıyla **uygulama lisans yönetimini etkinleştir'i seçin.**</span><span class="sxs-lookup"><span data-stu-id="ad5a2-141">To enable license management for your offer, select **Enable app license management through Microsoft**.</span></span> <span data-ttu-id="ad5a2-142">Bu tek seferlik bir ayardır ve teklifiniz yayımlandıktan sonra bunu değiştiremezsiniz.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-142">This is a one-time setting, and you can’t change it once your offer is published.</span></span>

    - <span data-ttu-id="ad5a2-143">Ayrıca, müşterilerin uygulama temel işlevselliğini lisans olmadan çalıştırmasını ve lisans satın alan premium özellikleri çalıştırmasını da sebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-143">You can also enable customers to run your app’s base functionality without a license, and run premium features once they’ve purchased a license.</span></span> <span data-ttu-id="ad5a2-144">Bunu yapmak için Lisans **atanmasa bile müşterilerin uygulamamı yüklemesine izin ver'i seçin.**</span><span class="sxs-lookup"><span data-stu-id="ad5a2-144">To do this, select **Allow customers to install my app even if licenses are not assigned**.</span></span>

    - <span data-ttu-id="ad5a2-145">Teklifinizin lisans yönetiminin etkinleştirilmesi istemiyorsanız Şimdi al **(Ücretsiz)** **,** Ücretsiz deneme veya Bana ulaşın'ı **seçin.**</span><span class="sxs-lookup"><span data-stu-id="ad5a2-145">If you don’t want your offer to have license management enabled, select **Get it now (Free)**, **Free trial**, or **Contact me**.</span></span>

## <a name="create-your-plan"></a><span data-ttu-id="ad5a2-146">Planınızı oluşturma</span><span class="sxs-lookup"><span data-stu-id="ad5a2-146">Create your plan</span></span>

<span data-ttu-id="ad5a2-147">Bu adımlarda, teklifiniz için etkinleştirmek istediğiniz planı veya planları tanımlayacaksınız.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-147">In these steps you’ll define the plan or plans you want to enable for your offer.</span></span>

1. <span data-ttu-id="ad5a2-148">Sol gezinti menüsünde **plana genel bakış**' ı seçin ve ardından **Yeni plan oluştur**' u seçin.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-148">On the left navigation menu, select **Plan overview**, and then select **Create new plan**.</span></span>
2. <span data-ttu-id="ad5a2-149">Bir **plan kimliği** ve **Plan adı** girin ve ardından **Oluştur**' u seçin.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-149">Enter a **Plan ID** and **Plan name**, and then select **Create**.</span></span>
3. <span data-ttu-id="ad5a2-150">**Plan listeleme** sayfasında **plan açıklamanızı** girin.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-150">On the **Plan listing** page, enter your **Plan description**.</span></span>
4. <span data-ttu-id="ad5a2-151">Açıklamayı kaydetmek ve daha sonra sona ermesini sağlamak için **Taslağı kaydet**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-151">To save the description and finish later, select **Save draft**.</span></span>

5. <span data-ttu-id="ad5a2-152">İşiniz bittiğinde, **gözden geçir ve Yayımla**' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-152">When you’re finished, select **Review and publish**.</span></span> <span data-ttu-id="ad5a2-153">Plan bilgileri artık teklif listesi (planlar bölümü) altında appsource.microsoft.com üzerinde görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-153">The plan information will now be displayed on appsource.microsoft.com under offer listing (plans section).</span></span>

6. <span data-ttu-id="ad5a2-154">Bu teklif için tüm planları oluşturduktan sonra, her planın hizmet KIMLIĞINI kopyalamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-154">After you’ve created all of the plans for this offer, you’ll need to copy each plan’s Service ID.</span></span> <span data-ttu-id="ad5a2-155">Plan listesi sayfasının en üstünde **plana genel bakış ' ı** seçin.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-155">Select **Plan overview** at the top of the Plan listing page.</span></span> <span data-ttu-id="ad5a2-156">Her planın hizmet KIMLIĞINI güvenli bir konuma kopyalayın.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-156">Copy the Service ID for each plan to a safe location.</span></span>

## <a name="add-service-ids-to-your-solution"></a><span data-ttu-id="ad5a2-157">Çözümünüze hizmet kimlikleri ekleyin</span><span class="sxs-lookup"><span data-stu-id="ad5a2-157">Add Service IDs to your solution</span></span>

<span data-ttu-id="ad5a2-158">Bir sonraki adım, yeni kopyaladığınız her plana ait hizmet kimliklerini ekleyerek çözümünüzü güncelleştirmedir.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-158">The next step is to update your solution by adding the Service IDs for each plan that you just copied.</span></span> <span data-ttu-id="ad5a2-159">Bunun hakkında yönergeler için bkz. [çözümünüz Için AppSource paketi oluşturma](/powerapps/developer/data-platform/create-package-app-appsource).</span><span class="sxs-lookup"><span data-stu-id="ad5a2-159">For guidance on this, see [Create an AppSource Package for your solution](/powerapps/developer/data-platform/create-package-app-appsource).</span></span>

## <a name="upload-your-package-and-publish-your-offer"></a><span data-ttu-id="ad5a2-160">Paketinizi karşıya yükleyin ve teklifinizi yayımlayın</span><span class="sxs-lookup"><span data-stu-id="ad5a2-160">Upload your package and publish your offer</span></span>

1. <span data-ttu-id="ad5a2-161">Sol gezinti bölmesinde, **ticari Market**' i seçin ve ardından **Teknik yapılandırma**' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-161">On the left navigation pane, select **Commercial Marketplace**, and then select **Technical configuration**.</span></span>
2. <span data-ttu-id="ad5a2-162">**Temel lisans modeli** altında **Kullanıcı**' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-162">Under **Base License Model**, select **User**.</span></span>
3. <span data-ttu-id="ad5a2-163">**CRM paketi** altında, paket KONUMLARıNıZıN URL 'sini girin.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-163">Under **CRM Package**, enter the URL of your package location.</span></span>
4. <span data-ttu-id="ad5a2-164">Diğer gerekli bilgileri girmek için sol gezinti bölmesindeki diğer sekmeleri kullanın.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-164">Use the other tabs on the left navigation pane to enter any other required information.</span></span> <span data-ttu-id="ad5a2-165">İşiniz bittiğinde, **gözden geçir ve Yayımla**' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-165">When you’re done, select **Review and publish**.</span></span>

<span data-ttu-id="ad5a2-166">Teklifi yayımladıktan sonra bilgilerinizi gözden geçireceğiz ve doğrulayacağız.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-166">After you publish the offer, we’ll review and verify your information.</span></span> <span data-ttu-id="ad5a2-167">Bu işlemle ilgili herhangi bir sorun varsa sizi bilgilendireceğiz.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-167">If there are any issues with this process, we’ll notify you.</span></span> <span data-ttu-id="ad5a2-168">Tüm sorunlar çözümlendikten sonra teklifinizin AppSource 'ta kullanılabildiğini belirten bir bildirim alırsınız.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-168">When all issues have been resolved, you’ll get a notification that your offer is available in AppSource.</span></span> <span data-ttu-id="ad5a2-169">Bu noktada, onu canlı hale getirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-169">At that point you can make it live.</span></span>

## <a name="make-your-offer-live-in-partner-center"></a><span data-ttu-id="ad5a2-170">Teklifinizi Iş Ortağı Merkezi 'nde canlı hale getirin</span><span class="sxs-lookup"><span data-stu-id="ad5a2-170">Make your offer live in Partner Center</span></span>

<span data-ttu-id="ad5a2-171">Aşağıdaki yordam, teklifinizi AppSource 'ta canlı hale getirme sürecinde size yol gösterir.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-171">The procedure below walks you through the process of making your offer live in AppSource.</span></span> <span data-ttu-id="ad5a2-172">Bu işlem hakkında daha fazla bilgi edinmek için bkz. [listeye giriş seçenekleri](/azure/marketplace/determine-your-listing-type).</span><span class="sxs-lookup"><span data-stu-id="ad5a2-172">To learn more about this process, see [Introduction to listing options](/azure/marketplace/determine-your-listing-type).</span></span>

>[!NOTE]
><span data-ttu-id="ad5a2-173">Teklifinizi yayımladıktan sonra, bu işlem 4-6 saat sürer.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-173">Once you publish your offer, it will take 4-6 hours to go live.</span></span>

1. <span data-ttu-id="ad5a2-174">[İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-174">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="ad5a2-175">Sol gezinti menüsünde **ticari Market/genel bakış**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-175">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="ad5a2-176">**Genel bakış** sayfasında, aradığınız teklifi bulun.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-176">On the **Overview** page, find the offer you’re looking for.</span></span> <span data-ttu-id="ad5a2-177">Yayımlanmaya hazırlanma teklifleri **Önizleme** durumuna sahip olur.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-177">Offers ready to be published will have a status of **Preview**.</span></span> <span data-ttu-id="ad5a2-178">Teklifi seçin.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-178">Select the offer.</span></span>
4. <span data-ttu-id="ad5a2-179">**Teklifin genel bakış** sayfasında **canlı git**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-179">On the **Offer overview** page, select **Go live**.</span></span>
<span data-ttu-id="ad5a2-180">Teklif 4-6 saat içinde etkin olacaktır.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-180">The offer will be live in 4-6 hours.</span></span>
5. <span data-ttu-id="ad5a2-181">AppSource 'ta teklif listelemeyi görmek için, **teklif genel bakış** sayfasının alt kısmındaki **appsource** bağlantısını seçin.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-181">To see your offer listing on AppSource, select the **AppSource** link at the bottom of the **Offer overview** page.</span></span>

    - <span data-ttu-id="ad5a2-182">**Lisans etkin teklifler için**: teklifiniz bir lisans denetimi gerektiriyorsa, kullanıcılar bu kişilerle iletişim kurabilmesi Için yalnızca **benimle iletişim** kuracak bir müşteri adayı girebilecektir.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-182">**For license-enabled offers**: If your offer requires a license check, users will only be able to enter a lead by clicking **Contact Me**, so that you can communicate with them.</span></span>

    - <span data-ttu-id="ad5a2-183">**Ücretsiz yükleme seçeneğiyle lisans etkin teklifler için**: teklifiniz bir lisans denetimi gerektirmiyorsa, yönetici kullanıcılar **bana başvurmaya** ek olarak **Şimdi bir şimdi al** düğmesine sahip olur.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-183">**For license-enabled offers with free installation option**: If your offer does not require a license check, admin users will see a **Get It Now** button in addition to **Contact Me**.</span></span> <span data-ttu-id="ad5a2-184">Ücretsiz yükleme seçeneğinizi denemek isteyen kullanıcılar **Şimdi al**' a tıklamalıdır, bu, teklifi Power platform yönetim merkezine yüklemeye getirir.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-184">Users who want to try your free installation option should click **Get It Now**, which will bring them to install the offer on Power Platform Admin Center.</span></span> <span data-ttu-id="ad5a2-185">Kullanıcılar, herhangi bir sorunuz varsa veya ücretli bir plana yükseltmek istediklerinde **benimle Iletişim kurma** 'yı kullanmaya devam edebilir.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-185">Users can still use **Contact Me** if they have any questions, or if they want to upgrade to a paid plan.</span></span>

## <a name="register-isv-connect-deal-in-deal-registration"></a><span data-ttu-id="ad5a2-186">ISV Connect 'in anlaşmayı kayda kaydetme</span><span class="sxs-lookup"><span data-stu-id="ad5a2-186">Register ISV Connect deal in Deal Registration</span></span>

<span data-ttu-id="ad5a2-187">Bir müşteriye lisans atayabilmeniz için önce her satışın Iş Ortağı Merkezi 'ne kaydedilmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-187">Before you can assign licenses to a customer, each sale needs to be registered in Partner Center.</span></span> <span data-ttu-id="ad5a2-188">Bunu yapmak için [bkz. Anlaşmalarınızı kaydetme.](register-deals.md)</span><span class="sxs-lookup"><span data-stu-id="ad5a2-188">To do this, see [Register your deals](register-deals.md).</span></span>

## <a name="invite-the-customer"></a><span data-ttu-id="ad5a2-189">Müşteriyi davet etme</span><span class="sxs-lookup"><span data-stu-id="ad5a2-189">Invite the customer</span></span>

<span data-ttu-id="ad5a2-190">Müşteriyi bu satış anlaşmasına katılmaya davet etmek için aşağıdaki yordamı kullanın.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-190">Use the following procedure to invite the customer to participate in this deal.</span></span>  

1. <span data-ttu-id="ad5a2-191">[İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-191">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="ad5a2-192">Sol gezinti menüsünde Ticari **Market/Genel Bakış'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="ad5a2-192">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="ad5a2-193">Sol gezinti menüsünde Referanslar'ı **ve ardından** Anlaşma **Kaydı'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="ad5a2-193">On the left navigation menu, select **Referrals**, and then select **Deal Registration**.</span></span>
4. <span data-ttu-id="ad5a2-194">Gönderilen **anlaşmalar için** filtrele, **Devam Ediyor sekmesini** ve ardından istediğiniz anlaşmayı seçin.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-194">Filter for **Submitted** deals, select the **In Progress** tab, and then select the deal you want.</span></span>
5. <span data-ttu-id="ad5a2-195">Bu anlaşmayı genel bakış sayfasında Lisansları **yönet'i seçin.**</span><span class="sxs-lookup"><span data-stu-id="ad5a2-195">On the overview page for this deal, select **Manage licenses**.</span></span>
6. <span data-ttu-id="ad5a2-196">Lisansları **yönet penceresinde** Müşteri ayrıntıları açılan **listesinden** müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-196">In the **Manage licenses** window, select the customer from the **Customer details** dropdown list.</span></span> <span data-ttu-id="ad5a2-197">Müşteri ilişkisi henüz yoksa onay için +Yeni müşteri **davet et'i seçin.**</span><span class="sxs-lookup"><span data-stu-id="ad5a2-197">If the customer relationship does not exist yet, select **+Invite a new customer to consent**.</span></span>
7. <span data-ttu-id="ad5a2-198">Görüntülenen bağlantıyı kopyalayın.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-198">Copy the link that is displayed.</span></span>
8. <span data-ttu-id="ad5a2-199">Bu bağlantıyı müşterinizin faturalama yöneticisine veya genel yöneticisine e-posta ile gönderin ve bu bağlantıyı kullanarak admin.microsoft.com ilişkileri kabul etmelerini ve yetkilendirmelerini snın.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-199">Email this link to your customer’s billing admin or global admin, and have them use this link to access admin.microsoft.com and accept and authorize the relationship you’re establishing.</span></span>

    >[!NOTE]
    ><span data-ttu-id="ad5a2-200">Müşteri bu adımı gerçekleştirene kadar ilişki kurulmayacak.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-200">The relationship will not be established until the customer performs this step.</span></span>

## <a name="activate-manage-and-remove-your-licenses"></a><span data-ttu-id="ad5a2-201">Lisanslarınızı etkinleştirme, yönetme ve kaldırma</span><span class="sxs-lookup"><span data-stu-id="ad5a2-201">Activate, manage, and remove your licenses</span></span>

<span data-ttu-id="ad5a2-202">Müşteriniz size ilişkinin yetkilerini verdiktan sonra teklifinizin planlarını eklemeye ve her plana lisans atamaya başlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-202">Once your customer has authorized the relationship with you, you can start adding plans from your offer and assigning licenses to each plan.</span></span>

1. <span data-ttu-id="ad5a2-203">Bu anlaşma için Lisansları yönet penceresinde **+Plan ekle'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="ad5a2-203">In the Manage licenses window for this deal, select **+Add a plan**.</span></span>
2. <span data-ttu-id="ad5a2-204">Bu çözüm **için planlar ve Lisans** sayısı alanlarını **doldurun** ve ardından Lisansları **güncelleştir'i seçin.**</span><span class="sxs-lookup"><span data-stu-id="ad5a2-204">Complete the **Plans for this solution** and **Number of licenses** fields, and then select **Update licenses**.</span></span> <span data-ttu-id="ad5a2-205">Lisanslar, müşterilerin admin.microsoft.com atanmalarını sağlamak için şirket içinde kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="ad5a2-205">The licenses will be available at admin.microsoft.com for customers to manage and assign to employees.</span></span>

    - <span data-ttu-id="ad5a2-206">Mevcut bir planın lisans sayısını değiştirmek için Lisans sayısı  alanına yeni numarayı girin ve Lisansları **güncelleştir'i seçin.**</span><span class="sxs-lookup"><span data-stu-id="ad5a2-206">To change the number of licenses for an existing plan, enter the new number in the **Number of licenses** field and then select **Update licenses**.</span></span>

    - <span data-ttu-id="ad5a2-207">Bir anlaşma için lisansları devre dışı bırakmak veya kaldırmak için Eylemler alanında çöp kutusu **simgesini ve** ardından Lisansları **güncelleştir'i seçin.**</span><span class="sxs-lookup"><span data-stu-id="ad5a2-207">To deactivate or remove licenses for a deal, select the trash can icon in the **Actions** field and then select **Update licenses**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ad5a2-208">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="ad5a2-208">Next steps</span></span>

[<span data-ttu-id="ad5a2-209">Lisanslama kaynakları</span><span class="sxs-lookup"><span data-stu-id="ad5a2-209">Licensing resources</span></span>](support-resources-licensing.md)