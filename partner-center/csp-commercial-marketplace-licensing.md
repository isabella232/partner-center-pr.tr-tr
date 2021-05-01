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
ms.openlocfilehash: f049ffda4c3d9476c09257fc814e5acac393cb54
ms.sourcegitcommit: 6c20c3cc4a226cada70c56df295966696affcec8
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/30/2021
ms.locfileid: "108328024"
---
# <a name="manage-licensing-in-marketplace-offers"></a><span data-ttu-id="6eb26-103">Market teklifte lisanslamayı yönetme</span><span class="sxs-lookup"><span data-stu-id="6eb26-103">Manage licensing in marketplace offers</span></span>

<span data-ttu-id="6eb26-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="6eb26-104">**Appropriate roles**</span></span>

- <span data-ttu-id="6eb26-105">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="6eb26-105">Global admin</span></span>
- <span data-ttu-id="6eb26-106">Hesap yöneticisi</span><span class="sxs-lookup"><span data-stu-id="6eb26-106">Account admin</span></span>

<span data-ttu-id="6eb26-107">Bu makalede, Iş Ortağı Merkezi 'nde bir teklif ayarlama, Microsoft AppSource ' de kullanılabilir hale getirme ve ardından bu teklifin lisanslarını yönetme sürecinde size yol gösterilir.</span><span class="sxs-lookup"><span data-stu-id="6eb26-107">This article walks you through the process of setting up an offer in Partner Center, making it available in Microsoft AppSource, and then managing licenses for that offer.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="6eb26-108">Bu makaledeki yetenekler Şu anda genel önizlemededir.</span><span class="sxs-lookup"><span data-stu-id="6eb26-108">The capabilities in this article are currently in Public Preview.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="6eb26-109">Başlamadan önce</span><span class="sxs-lookup"><span data-stu-id="6eb26-109">Before you begin</span></span>

### <a name="commercial-marketplace-basics"></a><span data-ttu-id="6eb26-110">Ticari Market temelleri</span><span class="sxs-lookup"><span data-stu-id="6eb26-110">Commercial marketplace basics</span></span>

<span data-ttu-id="6eb26-111">Bu işleme başlamadan önce, ticari Market 'in temelleri hakkında bilgi almalısınız.</span><span class="sxs-lookup"><span data-stu-id="6eb26-111">Before you begin this process, you should familiarize yourself with the basics of the commercial marketplace.</span></span> <span data-ttu-id="6eb26-112">Aşağıdaki tablodaki makaleler başlamanıza yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="6eb26-112">The articles in the table below will help get you started.</span></span> 

| <span data-ttu-id="6eb26-113">Konu</span><span class="sxs-lookup"><span data-stu-id="6eb26-113">Topic</span></span>  | <span data-ttu-id="6eb26-114">Makale</span><span class="sxs-lookup"><span data-stu-id="6eb26-114">Article</span></span>  |
|-------|--------|
|<span data-ttu-id="6eb26-115">Ticari Market planları</span><span class="sxs-lookup"><span data-stu-id="6eb26-115">Commercial marketplace plans</span></span> | [<span data-ttu-id="6eb26-116">Ticari Market teklifleri için planlar ve fiyatlandırma</span><span class="sxs-lookup"><span data-stu-id="6eb26-116">Plans and pricing for commercial marketplace offers</span></span>](/azure/marketplace/plans-pricing)    |
|<span data-ttu-id="6eb26-117">Ticari Market teklifleri</span><span class="sxs-lookup"><span data-stu-id="6eb26-117">Commercial marketplace offers</span></span>  | [<span data-ttu-id="6eb26-118">Liste türleri</span><span class="sxs-lookup"><span data-stu-id="6eb26-118">Listing types</span></span>](/azure/marketplace/determine-your-listing-type)    |
|<span data-ttu-id="6eb26-119">Ticari Market hesapları</span><span class="sxs-lookup"><span data-stu-id="6eb26-119">Commercial marketplace accounts</span></span> |  [<span data-ttu-id="6eb26-120">Iş Ortağı Merkezi 'nde ticari Market hesabı oluşturma</span><span class="sxs-lookup"><span data-stu-id="6eb26-120">Create a commercial marketplace account in Partner Center</span></span>](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a><span data-ttu-id="6eb26-121">Teklif KIMLIĞINIZI belirleme</span><span class="sxs-lookup"><span data-stu-id="6eb26-121">Determine your Offer ID</span></span>

<span data-ttu-id="6eb26-122">Aşağıdaki yordamlarda bir teklif KIMLIĞI girmeniz istenir.</span><span class="sxs-lookup"><span data-stu-id="6eb26-122">In the procedures below, you’ll be prompted to enter an Offer ID.</span></span> <span data-ttu-id="6eb26-123">Aşağıdaki noktaları göz önünde bulundurarak uygun bir teklif KIMLIĞIYLE karşılaşmaya biraz zaman atın:</span><span class="sxs-lookup"><span data-stu-id="6eb26-123">Take some time now to come up with a suitable Offer ID, keeping in mind the following points:</span></span>

- <span data-ttu-id="6eb26-124">Bu KIMLIK, varsa Market teklifi ve Azure Resource Manager şablonları için Web adresinde müşteriler tarafından görülebilir.</span><span class="sxs-lookup"><span data-stu-id="6eb26-124">This ID is visible to customers in the web address for the marketplace offer and Azure Resource Manager templates, if applicable.</span></span>
- <span data-ttu-id="6eb26-125">Yayımcı KIMLIĞIYLE birleştirilmiş teklif KIMLIĞI, 40 karakter uzunluğunda olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="6eb26-125">The Offer ID combined with the Publisher ID must be under 40 characters in length.</span></span>
- <span data-ttu-id="6eb26-126">Yalnızca küçük harfleri ve rakamları kullanın.</span><span class="sxs-lookup"><span data-stu-id="6eb26-126">Use only lowercase letters and numbers.</span></span> <span data-ttu-id="6eb26-127">Teklif KIMLIĞI, kısa çizgiler ve alt çizgiler içerebilir ancak boşluk içeremez.</span><span class="sxs-lookup"><span data-stu-id="6eb26-127">The Offer ID can include hyphens and underscores, but no spaces.</span></span> <span data-ttu-id="6eb26-128">Örneğin, yayımcı KIMLIĞINIZ ise `testpublisherid` ve girerseniz `test-offer-1` , teklif Web adresi olur `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` .</span><span class="sxs-lookup"><span data-stu-id="6eb26-128">For example, if your Publisher ID is `testpublisherid` and you enter `test-offer-1`, the offer web address will be `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1`.</span></span>
- <span data-ttu-id="6eb26-129">Bu KIMLIK, **Oluştur**' u seçtikten sonra değiştirilemez.</span><span class="sxs-lookup"><span data-stu-id="6eb26-129">This ID can't be changed after you select **Create**.</span></span>

### <a name="determine-your-offer-alias"></a><span data-ttu-id="6eb26-130">Teklif diğer adınızı belirleme</span><span class="sxs-lookup"><span data-stu-id="6eb26-130">Determine your Offer alias</span></span>

<span data-ttu-id="6eb26-131">Teklif diğer adı, Iş Ortağı Merkezi 'nde teklif için kullanılan addır.</span><span class="sxs-lookup"><span data-stu-id="6eb26-131">The Offer alias is the name used for the offer in Partner Center.</span></span> <span data-ttu-id="6eb26-132">Ayrıca, aşağıdaki yönergeleri takip eden uygun bir teklif diğer adına ihtiyacınız olacaktır:</span><span class="sxs-lookup"><span data-stu-id="6eb26-132">You’ll also need an appropriate Offer alias that follows the guidelines below:</span></span>

- <span data-ttu-id="6eb26-133">Bu ad Market 'te kullanılmıyor ve teklif adından ve müşterilere gösterilen diğer değerlerden farklı.</span><span class="sxs-lookup"><span data-stu-id="6eb26-133">This name isn't used in the marketplace and is different from the offer name and other values shown to customers.</span></span>
- <span data-ttu-id="6eb26-134">Bu ad, Oluştur ' u seçtikten sonra değiştirilemez.</span><span class="sxs-lookup"><span data-stu-id="6eb26-134">This name can't be changed after you select Create.</span></span>

## <a name="create-your-offer"></a><span data-ttu-id="6eb26-135">Teklifinizi oluşturma</span><span class="sxs-lookup"><span data-stu-id="6eb26-135">Create your offer</span></span>

<span data-ttu-id="6eb26-136">Lisanslama sürecinin ilk adımı, ticari Market teklifinizi oluşturmaktır.</span><span class="sxs-lookup"><span data-stu-id="6eb26-136">The first step in the licensing process is to create your commercial marketplace offer.</span></span> 

1. <span data-ttu-id="6eb26-137">[İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="6eb26-137">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="6eb26-138">Sol gezinti menüsünde **ticari Market/genel bakış**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-138">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="6eb26-139">Genel Bakış sayfasının üst kısmında, **yeni teklif**' i seçin ve ardından Dynamics 365 ' i seçerek **& PowerApps**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-139">At the top of the Overview page, select **New offer**, and then select **Dynamics 365 for Customer Engagement & PowerApps**.</span></span>
4. <span data-ttu-id="6eb26-140">Daha önce oluşturduğunuz **TEKLIF kimliği** ve **teklif diğer adını** girin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-140">Enter the **Offer ID** and **Offer alias** you created earlier.</span></span>
5. <span data-ttu-id="6eb26-141">Teklifi oluşturmak için **Oluştur** ' u seçin ve devam edin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-141">Select **Create** to generate the offer and continue.</span></span>
6. <span data-ttu-id="6eb26-142">Lisanslama seçeneklerinizi belirleyin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-142">Choose your licensing options.</span></span>

    - <span data-ttu-id="6eb26-143">Teklifiniz için lisans yönetimini etkinleştirmek üzere **Microsoft aracılığıyla uygulama lisans yönetimini etkinleştir**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-143">To enable license management for your offer, select **Enable app license management through Microsoft**.</span></span> <span data-ttu-id="6eb26-144">Bu bir kerelik bir ayardır ve teklifiniz yayımlandıktan sonra bu ayarı değiştiremezsiniz.</span><span class="sxs-lookup"><span data-stu-id="6eb26-144">This is a one-time setting, and you can’t change it once your offer is published.</span></span>

    - <span data-ttu-id="6eb26-145">Ayrıca, müşterilerin bir lisans olmadan uygulamanızın temel işlevselliğini çalıştırmasına ve bir lisans satın aldıktan sonra Premium özellikleri çalıştırmasına olanak sağlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6eb26-145">You can also enable customers to run your app’s base functionality without a license, and run premium features once they’ve purchased a license.</span></span> <span data-ttu-id="6eb26-146">Bunu yapmak için, **lisanslar atanmasa bile müşterilerin uygulamamı yüklemesine Izin ver**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-146">To do this, select **Allow customers to install my app even if licenses are not assigned**.</span></span>

    - <span data-ttu-id="6eb26-147">Teklifinizin lisans yönetimi 'nin etkinleştirilmesini istemiyorsanız, **Şimdi al (ücretsiz)**, **ücretsiz deneme** veya **benimle iletişim kurun**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-147">If you don’t want your offer to have license management enabled, select **Get it now (Free)**, **Free trial**, or **Contact me**.</span></span>

## <a name="create-your-plan"></a><span data-ttu-id="6eb26-148">Planınızı oluşturma</span><span class="sxs-lookup"><span data-stu-id="6eb26-148">Create your plan</span></span>

<span data-ttu-id="6eb26-149">Bu adımlarda, teklifiniz için etkinleştirmek istediğiniz planı veya planları tanımlayacaksınız.</span><span class="sxs-lookup"><span data-stu-id="6eb26-149">In these steps you’ll define the plan or plans you want to enable for your offer.</span></span>

1. <span data-ttu-id="6eb26-150">Sol gezinti menüsünde **plana genel bakış**' ı seçin ve ardından **Yeni plan oluştur**' u seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-150">On the left navigation menu, select **Plan overview**, and then select **Create new plan**.</span></span>
2. <span data-ttu-id="6eb26-151">Bir **plan kimliği** ve **Plan adı** girin ve ardından **Oluştur**' u seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-151">Enter a **Plan ID** and **Plan name**, and then select **Create**.</span></span>
3. <span data-ttu-id="6eb26-152">**Plan listeleme** sayfasında **plan açıklamanızı** girin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-152">On the **Plan listing** page, enter your **Plan description**.</span></span>
4. <span data-ttu-id="6eb26-153">Açıklamayı kaydetmek ve daha sonra sona ermesini sağlamak için **Taslağı kaydet**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-153">To save the description and finish later, select **Save draft**.</span></span>

5. <span data-ttu-id="6eb26-154">İşiniz bittiğinde, **gözden geçir ve Yayımla**' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-154">When you’re finished, select **Review and publish**.</span></span> <span data-ttu-id="6eb26-155">Plan bilgileri artık teklif listesi (planlar bölümü) altında appsource.microsoft.com üzerinde görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="6eb26-155">The plan information will now be displayed on appsource.microsoft.com under offer listing (plans section).</span></span>

6. <span data-ttu-id="6eb26-156">Bu teklif için tüm planları oluşturduktan sonra, her planın hizmet KIMLIĞINI kopyalamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="6eb26-156">After you’ve created all of the plans for this offer, you’ll need to copy each plan’s Service ID.</span></span> <span data-ttu-id="6eb26-157">Plan listesi sayfasının en üstünde **plana genel bakış ' ı** seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-157">Select **Plan overview** at the top of the Plan listing page.</span></span> <span data-ttu-id="6eb26-158">Her planın hizmet KIMLIĞINI güvenli bir konuma kopyalayın.</span><span class="sxs-lookup"><span data-stu-id="6eb26-158">Copy the Service ID for each plan to a safe location.</span></span>

## <a name="add-service-ids-to-your-solution"></a><span data-ttu-id="6eb26-159">Çözümünüze hizmet kimlikleri ekleyin</span><span class="sxs-lookup"><span data-stu-id="6eb26-159">Add Service IDs to your solution</span></span>

<span data-ttu-id="6eb26-160">Bir sonraki adım, yeni kopyaladığınız her plana ait hizmet kimliklerini ekleyerek çözümünüzü güncelleştirmedir.</span><span class="sxs-lookup"><span data-stu-id="6eb26-160">The next step is to update your solution by adding the Service IDs for each plan that you just copied.</span></span> <span data-ttu-id="6eb26-161">Bunun hakkında yönergeler için bkz. [çözümünüz Için AppSource paketi oluşturma](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span><span class="sxs-lookup"><span data-stu-id="6eb26-161">For guidance on this, see [Create an AppSource Package for your solution](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span></span>

## <a name="upload-your-package-and-publish-your-offer"></a><span data-ttu-id="6eb26-162">Paketinizi karşıya yükleyin ve teklifinizi yayımlayın</span><span class="sxs-lookup"><span data-stu-id="6eb26-162">Upload your package and publish your offer</span></span>

1. <span data-ttu-id="6eb26-163">Sol gezinti bölmesinde, **ticari Market**' i seçin ve ardından **Teknik yapılandırma**' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-163">On the left navigation pane, select **Commercial Marketplace**, and then select **Technical configuration**.</span></span>
2. <span data-ttu-id="6eb26-164">**Temel lisans modeli** altında **Kullanıcı**' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-164">Under **Base License Model**, select **User**.</span></span>
3. <span data-ttu-id="6eb26-165">**CRM paketi** altında, paket KONUMLARıNıZıN URL 'sini girin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-165">Under **CRM Package**, enter the URL of your package location.</span></span>
4. <span data-ttu-id="6eb26-166">Diğer gerekli bilgileri girmek için sol gezinti bölmesindeki diğer sekmeleri kullanın.</span><span class="sxs-lookup"><span data-stu-id="6eb26-166">Use the other tabs on the left navigation pane to enter any other required information.</span></span> <span data-ttu-id="6eb26-167">İşiniz bittiğinde, **gözden geçir ve Yayımla**' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-167">When you’re done, select **Review and publish**.</span></span>

<span data-ttu-id="6eb26-168">Teklifi yayımladıktan sonra bilgilerinizi gözden geçireceğiz ve doğrulayacağız.</span><span class="sxs-lookup"><span data-stu-id="6eb26-168">After you publish the offer, we’ll review and verify your information.</span></span> <span data-ttu-id="6eb26-169">Bu işlemle ilgili herhangi bir sorun varsa sizi bilgilendireceğiz.</span><span class="sxs-lookup"><span data-stu-id="6eb26-169">If there are any issues with this process, we’ll notify you.</span></span> <span data-ttu-id="6eb26-170">Tüm sorunlar çözümlendikten sonra teklifinizin AppSource 'ta kullanılabildiğini belirten bir bildirim alırsınız.</span><span class="sxs-lookup"><span data-stu-id="6eb26-170">When all issues have been resolved, you’ll get a notification that your offer is available in AppSource.</span></span> <span data-ttu-id="6eb26-171">Bu noktada, onu canlı hale getirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6eb26-171">At that point you can make it live.</span></span>

## <a name="make-your-offer-live-in-partner-center"></a><span data-ttu-id="6eb26-172">Teklifinizi Iş Ortağı Merkezi 'nde canlı hale getirin</span><span class="sxs-lookup"><span data-stu-id="6eb26-172">Make your offer live in Partner Center</span></span>

<span data-ttu-id="6eb26-173">Aşağıdaki yordam, teklifinizi AppSource 'ta canlı hale getirme sürecinde size yol gösterir.</span><span class="sxs-lookup"><span data-stu-id="6eb26-173">The procedure below walks you through the process of making your offer live in AppSource.</span></span> <span data-ttu-id="6eb26-174">Bu işlem hakkında daha fazla bilgi edinmek için bkz. [listeye giriş seçenekleri](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span><span class="sxs-lookup"><span data-stu-id="6eb26-174">To learn more about this process, see [Introduction to listing options](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span></span>

>[!NOTE]
><span data-ttu-id="6eb26-175">Teklifinizi yayımladıktan sonra, bu işlem 4-6 saat sürer.</span><span class="sxs-lookup"><span data-stu-id="6eb26-175">Once you publish your offer, it will take 4-6 hours to go live.</span></span>

1. <span data-ttu-id="6eb26-176">[İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="6eb26-176">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="6eb26-177">Sol gezinti menüsünde **ticari Market/genel bakış**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-177">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="6eb26-178">**Genel bakış** sayfasında, aradığınız teklifi bulun.</span><span class="sxs-lookup"><span data-stu-id="6eb26-178">On the **Overview** page, find the offer you’re looking for.</span></span> <span data-ttu-id="6eb26-179">Yayımlanmaya hazırlanma teklifleri **Önizleme** durumuna sahip olur.</span><span class="sxs-lookup"><span data-stu-id="6eb26-179">Offers ready to be published will have a status of **Preview**.</span></span> <span data-ttu-id="6eb26-180">Teklifi seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-180">Select the offer.</span></span>
4. <span data-ttu-id="6eb26-181">**Teklifin genel bakış** sayfasında **canlı git**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-181">On the **Offer overview** page, select **Go live**.</span></span>
<span data-ttu-id="6eb26-182">Teklif 4-6 saat içinde etkin olacaktır.</span><span class="sxs-lookup"><span data-stu-id="6eb26-182">The offer will be live in 4-6 hours.</span></span>
5. <span data-ttu-id="6eb26-183">AppSource 'ta teklif listelemeyi görmek için, **teklif genel bakış** sayfasının alt kısmındaki **appsource** bağlantısını seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-183">To see your offer listing on AppSource, select the **AppSource** link at the bottom of the **Offer overview** page.</span></span>

    - <span data-ttu-id="6eb26-184">**Lisans etkin teklifler için**: teklifiniz bir lisans denetimi gerektiriyorsa, kullanıcılar bu kişilerle iletişim kurabilmesi Için yalnızca **benimle iletişim** kuracak bir müşteri adayı girebilecektir.</span><span class="sxs-lookup"><span data-stu-id="6eb26-184">**For license-enabled offers**: If your offer requires a license check, users will only be able to enter a lead by clicking **Contact Me**, so that you can communicate with them.</span></span>

    - <span data-ttu-id="6eb26-185">**Ücretsiz yükleme seçeneğiyle lisans etkin teklifler için**: teklifiniz bir lisans denetimi gerektirmiyorsa, yönetici kullanıcılar **bana başvurmaya** ek olarak **Şimdi bir şimdi al** düğmesine sahip olur.</span><span class="sxs-lookup"><span data-stu-id="6eb26-185">**For license-enabled offers with free installation option**: If your offer does not require a license check, admin users will see a **Get It Now** button in addition to **Contact Me**.</span></span> <span data-ttu-id="6eb26-186">Ücretsiz yükleme seçeneğinizi denemek isteyen kullanıcılar **Şimdi al**' a tıklamalıdır, bu, teklifi Power platform yönetim merkezine yüklemeye getirir.</span><span class="sxs-lookup"><span data-stu-id="6eb26-186">Users who want to try your free installation option should click **Get It Now**, which will bring them to install the offer on Power Platform Admin Center.</span></span> <span data-ttu-id="6eb26-187">Kullanıcılar, herhangi bir sorunuz varsa veya ücretli bir plana yükseltmek istediklerinde **benimle Iletişim kurma** 'yı kullanmaya devam edebilir.</span><span class="sxs-lookup"><span data-stu-id="6eb26-187">Users can still use **Contact Me** if they have any questions, or if they want to upgrade to a paid plan.</span></span>

## <a name="register-isv-connect-deal-in-deal-registration"></a><span data-ttu-id="6eb26-188">ISV Connect 'in anlaşmayı kayda kaydetme</span><span class="sxs-lookup"><span data-stu-id="6eb26-188">Register ISV Connect deal in Deal Registration</span></span>

<span data-ttu-id="6eb26-189">Bir müşteriye lisans atayabilmeniz için önce her satışın Iş Ortağı Merkezi 'ne kaydedilmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="6eb26-189">Before you can assign licenses to a customer, each sale needs to be registered in Partner Center.</span></span> <span data-ttu-id="6eb26-190">Bunu yapmak için bkz. [anlaşmaları kaydetme](register-deals.md).</span><span class="sxs-lookup"><span data-stu-id="6eb26-190">To do this, see [Register your deals](register-deals.md).</span></span>

## <a name="invite-the-customer"></a><span data-ttu-id="6eb26-191">Müşteriyi davet etme</span><span class="sxs-lookup"><span data-stu-id="6eb26-191">Invite the customer</span></span>

<span data-ttu-id="6eb26-192">Müşteriyi bu başa katılmaya davet etmek için aşağıdaki yordamı kullanın.</span><span class="sxs-lookup"><span data-stu-id="6eb26-192">Use the following procedure to invite the customer to participate in this deal.</span></span>  

1. <span data-ttu-id="6eb26-193">[İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="6eb26-193">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="6eb26-194">Sol gezinti menüsünde **ticari Market/genel bakış**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-194">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="6eb26-195">Sol gezinti menüsünde, **Başvurular**' ı seçin ve ardından **anlaşma kaydı**' nı seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-195">On the left navigation menu, select **Referrals**, and then select **Deal Registration**.</span></span>
4. <span data-ttu-id="6eb26-196">**Gönderilen** anlaşmalar için filtre uygulayın, **devam eden** sekmesini seçin ve ardından istediğiniz anlaşmayı seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-196">Filter for **Submitted** deals, select the **In Progress** tab, and then select the deal you want.</span></span>
5. <span data-ttu-id="6eb26-197">Bu anlaşma için genel bakış sayfasında **Lisansları Yönet**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-197">On the overview page for this deal, select **Manage licenses**.</span></span>
6. <span data-ttu-id="6eb26-198">**Lisansları Yönet** penceresinde müşteri **ayrıntıları** açılır listesinden müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-198">In the **Manage licenses** window, select the customer from the **Customer details** dropdown list.</span></span> <span data-ttu-id="6eb26-199">Müşteri ilişkisi henüz yoksa, **+ Yeni müşteriyi onay olarak davet et**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-199">If the customer relationship does not exist yet, select **+Invite a new customer to consent**.</span></span>
7. <span data-ttu-id="6eb26-200">Görüntülenen bağlantıyı kopyalayın.</span><span class="sxs-lookup"><span data-stu-id="6eb26-200">Copy the link that is displayed.</span></span>
8. <span data-ttu-id="6eb26-201">Bu bağlantıyı, müşterinizin faturalandırma Yöneticisi veya genel yöneticisine e-posta ile gönderin ve bu bağlantıyı admin.microsoft.com erişmek ve oluşturduğunuz ilişkiyi kabul etmek ve yetkilendirmek için kullanın.</span><span class="sxs-lookup"><span data-stu-id="6eb26-201">Email this link to your customer’s billing admin or global admin, and have them use this link to access admin.microsoft.com and accept and authorize the relationship you’re establishing.</span></span>

    >[!NOTE]
    ><span data-ttu-id="6eb26-202">Müşteri bu adımı gerçekleştirene kadar ilişki kurulmayacak.</span><span class="sxs-lookup"><span data-stu-id="6eb26-202">The relationship will not be established until the customer performs this step.</span></span>

## <a name="activate-manage-and-remove-your-licenses"></a><span data-ttu-id="6eb26-203">Lisanslarınızı etkinleştirin, yönetin ve kaldırın</span><span class="sxs-lookup"><span data-stu-id="6eb26-203">Activate, manage, and remove your licenses</span></span>

<span data-ttu-id="6eb26-204">Müşteriniz sizinle ilişkiyi yetkilendirdikten sonra, teklifinizden planlar eklemeye ve her plana lisans atamaya başlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6eb26-204">Once your customer has authorized the relationship with you, you can start adding plans from your offer and assigning licenses to each plan.</span></span>

1. <span data-ttu-id="6eb26-205">Bu anlaşma için Lisansları Yönet penceresinde **+ plan Ekle**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-205">In the Manage licenses window for this deal, select **+Add a plan**.</span></span>
2. <span data-ttu-id="6eb26-206">**Bu çözüm Için planları** ve lisans alanı **sayısını** tamamlayıp **Lisansları Güncelleştir**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-206">Complete the **Plans for this solution** and **Number of licenses** fields, and then select **Update licenses**.</span></span> <span data-ttu-id="6eb26-207">Lisanslar, müşteriler tarafından yönetilecek ve çalışanlara atanacak admin.microsoft.com adresinde kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="6eb26-207">The licenses will be available at admin.microsoft.com for customers to manage and assign to employees.</span></span>

    - <span data-ttu-id="6eb26-208">Mevcut bir planın lisans sayısını değiştirmek için, **Lisans sayısı** alanına yeni sayıyı girin ve ardından **Lisansları Güncelleştir**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-208">To change the number of licenses for an existing plan, enter the new number in the **Number of licenses** field and then select **Update licenses**.</span></span>

    - <span data-ttu-id="6eb26-209">Bir anlaşma için lisansları devre dışı bırakmak veya kaldırmak için, **Eylemler** alanındaki çöp kutusu simgesini seçin ve ardından **Lisansları Güncelleştir**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="6eb26-209">To deactivate or remove licenses for a deal, select the trash can icon in the **Actions** field and then select **Update licenses**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6eb26-210">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="6eb26-210">Next steps</span></span>

[<span data-ttu-id="6eb26-211">Lisanslama kaynakları</span><span class="sxs-lookup"><span data-stu-id="6eb26-211">Licensing resources</span></span>](support-resources-licensing.md)
