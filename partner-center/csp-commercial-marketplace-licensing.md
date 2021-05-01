---
title: Market teklifte lisanslamayı yönetme
ms.topic: how-to
ms.date: 04/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: ISV ticari Market tekliflerinizi için lisanslamayı ayarlamayı ve yönetmeyi öğrenin.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3b2281696a2fe69253cd033eb2a7eef7fb3046f3
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284894"
---
# <a name="manage-licensing-in-marketplace-offers"></a><span data-ttu-id="f43f5-103">Market teklifte lisanslamayı yönetme</span><span class="sxs-lookup"><span data-stu-id="f43f5-103">Manage licensing in marketplace offers</span></span>

<span data-ttu-id="f43f5-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="f43f5-104">**Appropriate roles**</span></span>

- <span data-ttu-id="f43f5-105">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="f43f5-105">Global admin</span></span>
- <span data-ttu-id="f43f5-106">Hesap yöneticisi</span><span class="sxs-lookup"><span data-stu-id="f43f5-106">Account admin</span></span>

<span data-ttu-id="f43f5-107">Bu makalede, Iş Ortağı Merkezi 'nde bir teklif ayarlama, Microsoft AppSource ' de kullanılabilir hale getirme ve ardından bu teklifin lisanslarını yönetme sürecinde size yol gösterilir.</span><span class="sxs-lookup"><span data-stu-id="f43f5-107">This article walks you through the process of setting up an offer in Partner Center, making it available in Microsoft AppSource, and then managing licenses for that offer.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="f43f5-108">Bu makaledeki yetenekler Şu anda genel önizlemededir.</span><span class="sxs-lookup"><span data-stu-id="f43f5-108">The capabilities in this article are currently in Public Preview.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="f43f5-109">Başlamadan önce</span><span class="sxs-lookup"><span data-stu-id="f43f5-109">Before you begin</span></span>

<span data-ttu-id="f43f5-110">Bu işleme başlamadan önce, aşağıdaki bilgileri öğrenmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="f43f5-110">Before beginning this process, you should familiarize yourself with the information below.</span></span>

### <a name="review-the-azure-marketplace-documentation"></a><span data-ttu-id="f43f5-111">Azure Marketi belgelerini gözden geçirin</span><span class="sxs-lookup"><span data-stu-id="f43f5-111">Review the Azure Marketplace documentation</span></span>

<span data-ttu-id="f43f5-112">Aşağıdaki makalelerde, devam etmeden önce bilmeniz gereken bilgiler yer almalıdır.</span><span class="sxs-lookup"><span data-stu-id="f43f5-112">The articles below contain information you should know before continuing.</span></span> 

- [<span data-ttu-id="f43f5-113">Dynamics 365 for Customer Engagement ve PowerApps teklifi oluşturma</span><span class="sxs-lookup"><span data-stu-id="f43f5-113">Create a Dynamics 365 for Customer Engagement & PowerApps offer</span></span>](https://docs.microsoft.com/azure/marketplace/dynamics-365-customer-engage-offer-setup)
- [<span data-ttu-id="f43f5-114">Iş Ortağı Merkezi 'nde ticari Market hesabı oluşturma</span><span class="sxs-lookup"><span data-stu-id="f43f5-114">Create a commercial marketplace account in Partner Center</span></span>](https://docs.microsoft.com/azure/marketplace/create-account)

### <a name="create-your-offer-id"></a><span data-ttu-id="f43f5-115">Teklif KIMLIĞINIZI oluşturma</span><span class="sxs-lookup"><span data-stu-id="f43f5-115">Create your Offer ID</span></span>

<span data-ttu-id="f43f5-116">Aşağıdaki yordamlarda bir teklif KIMLIĞI girmeniz istenir.</span><span class="sxs-lookup"><span data-stu-id="f43f5-116">In the procedures below, you’ll be prompted to enter an Offer ID.</span></span> <span data-ttu-id="f43f5-117">Aşağıdaki noktaları göz önünde bulundurarak uygun bir teklif KIMLIĞIYLE karşılaşmaya biraz zaman atın:</span><span class="sxs-lookup"><span data-stu-id="f43f5-117">Take some time now to come up with a suitable Offer ID, keeping in mind the following points:</span></span>

- <span data-ttu-id="f43f5-118">Bu KIMLIK, varsa Market teklifi ve Azure Resource Manager şablonları için Web adresinde müşteriler tarafından görülebilir.</span><span class="sxs-lookup"><span data-stu-id="f43f5-118">This ID is visible to customers in the web address for the marketplace offer and Azure Resource Manager templates, if applicable.</span></span>
- <span data-ttu-id="f43f5-119">Yayımcı KIMLIĞIYLE birleştirilmiş teklif KIMLIĞI, 40 karakter uzunluğunda olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="f43f5-119">The Offer ID combined with the Publisher ID must be under 40 characters in length.</span></span>
- <span data-ttu-id="f43f5-120">Yalnızca küçük harfleri ve rakamları kullanın.</span><span class="sxs-lookup"><span data-stu-id="f43f5-120">Use only lowercase letters and numbers.</span></span> <span data-ttu-id="f43f5-121">Teklif KIMLIĞI, kısa çizgiler ve alt çizgiler içerebilir ancak boşluk içeremez.</span><span class="sxs-lookup"><span data-stu-id="f43f5-121">The Offer ID can include hyphens and underscores, but no spaces.</span></span> <span data-ttu-id="f43f5-122">Örneğin, yayımcı KIMLIĞINIZ testpublisherıd ise ve test-teklif-1 girerseniz, teklif Web adresi olur https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1 .</span><span class="sxs-lookup"><span data-stu-id="f43f5-122">For example, if your Publisher ID is testpublisherid and you enter test-offer-1, the offer web address will be https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1.</span></span>
- <span data-ttu-id="f43f5-123">Bu KIMLIK, **Oluştur**' u seçtikten sonra değiştirilemez.</span><span class="sxs-lookup"><span data-stu-id="f43f5-123">This ID can't be changed after you select **Create**.</span></span>

### <a name="create-your-offer-alias"></a><span data-ttu-id="f43f5-124">Teklif diğer adınızı oluşturma</span><span class="sxs-lookup"><span data-stu-id="f43f5-124">Create your Offer alias</span></span>

<span data-ttu-id="f43f5-125">Teklif diğer adı, Iş Ortağı Merkezi 'nde teklif için kullanılan addır.</span><span class="sxs-lookup"><span data-stu-id="f43f5-125">The Offer alias is the name used for the offer in Partner Center.</span></span> <span data-ttu-id="f43f5-126">Ayrıca, aşağıdaki yönergeleri takip eden uygun bir teklif diğer adına ihtiyacınız olacaktır:</span><span class="sxs-lookup"><span data-stu-id="f43f5-126">You’ll also need an appropriate Offer alias that follows the guidelines below:</span></span>

- <span data-ttu-id="f43f5-127">Bu ad Market 'te kullanılmıyor ve teklif adından ve müşterilere gösterilen diğer değerlerden farklı.</span><span class="sxs-lookup"><span data-stu-id="f43f5-127">This name isn't used in the marketplace and is different from the offer name and other values shown to customers.</span></span>
- <span data-ttu-id="f43f5-128">Bu ad, Oluştur ' u seçtikten sonra değiştirilemez.</span><span class="sxs-lookup"><span data-stu-id="f43f5-128">This name can't be changed after you select Create.</span></span>

## <a name="create-your-offer"></a><span data-ttu-id="f43f5-129">Teklifinizi oluşturma</span><span class="sxs-lookup"><span data-stu-id="f43f5-129">Create your offer</span></span>

<span data-ttu-id="f43f5-130">Lisanslama sürecinin ilk adımı, ticari Market teklifinizi oluşturmaktır.</span><span class="sxs-lookup"><span data-stu-id="f43f5-130">The first step in the licensing process is to create your commercial marketplace offer.</span></span> 

1. <span data-ttu-id="f43f5-131">[İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="f43f5-131">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="f43f5-132">Sol gezinti menüsünde **ticari Market/genel bakış**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-132">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="f43f5-133">Genel Bakış sayfasının üst kısmında, **yeni teklif**' i seçin ve ardından Dynamics 365 ' i seçerek **& PowerApps**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-133">At the top of the Overview page, select **New offer**, and then select **Dynamics 365 for Customer Engagement & PowerApps**.</span></span>
4. <span data-ttu-id="f43f5-134">Daha önce oluşturduğunuz **TEKLIF kimliği** ve **teklif diğer adını** girin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-134">Enter the **Offer ID** and **Offer alias** you created earlier.</span></span>
5. <span data-ttu-id="f43f5-135">Teklifi oluşturmak için **Oluştur** ' u seçin ve devam edin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-135">Select **Create** to generate the offer and continue.</span></span>
6. <span data-ttu-id="f43f5-136">Lisanslama seçeneklerinizi belirleyin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-136">Choose your licensing options.</span></span>

    - <span data-ttu-id="f43f5-137">Teklifiniz için lisans yönetimini etkinleştirmek üzere **Microsoft aracılığıyla uygulama lisans yönetimini etkinleştir**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-137">To enable license management for your offer, select **Enable app license management through Microsoft**.</span></span> <span data-ttu-id="f43f5-138">Bu bir kerelik bir ayardır ve teklifiniz yayımlandıktan sonra bu ayarı değiştiremezsiniz.</span><span class="sxs-lookup"><span data-stu-id="f43f5-138">This is a one-time setting, and you can’t change it once your offer is published.</span></span>

    - <span data-ttu-id="f43f5-139">Ayrıca, müşterilerin bir lisans olmadan uygulamanızın temel işlevselliğini çalıştırmasına ve bir lisans satın aldıktan sonra Premium özellikleri çalıştırmasına olanak sağlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f43f5-139">You can also enable customers to run your app’s base functionality without a license, and run premium features once they’ve purchased a license.</span></span> <span data-ttu-id="f43f5-140">Bunu yapmak için, **lisanslar atanmasa bile müşterilerin uygulamamı yüklemesine Izin ver**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-140">To do this, select **Allow customers to install my app even if licenses are not assigned**.</span></span>

    - <span data-ttu-id="f43f5-141">Teklifinizin lisans yönetimi 'nin etkinleştirilmesini istemiyorsanız, **Şimdi al (ücretsiz)**, **ücretsiz deneme** veya **benimle iletişim kurun**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-141">If you don’t want your offer to have license management enabled, select **Get it now (Free)**, **Free trial**, or **Contact me**.</span></span>

## <a name="create-your-plan"></a><span data-ttu-id="f43f5-142">Planınızı oluşturma</span><span class="sxs-lookup"><span data-stu-id="f43f5-142">Create your plan</span></span>

<span data-ttu-id="f43f5-143">Bu adımlarda, teklifiniz için etkinleştirmek istediğiniz planı veya planları tanımlayacaksınız.</span><span class="sxs-lookup"><span data-stu-id="f43f5-143">In these steps you’ll define the plan or plans you want to enable for your offer.</span></span>

1. <span data-ttu-id="f43f5-144">Sol gezinti menüsünde **plana genel bakış**' ı seçin ve ardından **Yeni plan oluştur**' u seçin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-144">On the left navigation menu, select **Plan overview**, and then select **Create new plan**.</span></span>
2. <span data-ttu-id="f43f5-145">Bir **plan kimliği** ve **Plan adı** girin ve ardından **Oluştur**' u seçin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-145">Enter a **Plan ID** and **Plan name**, and then select **Create**.</span></span>
3. <span data-ttu-id="f43f5-146">**Plan listeleme** sayfasında **plan açıklamanızı** girin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-146">On the **Plan listing** page, enter your **Plan description**.</span></span>
4. <span data-ttu-id="f43f5-147">Açıklamayı kaydetmek ve daha sonra sona ermesini sağlamak için **Taslağı kaydet**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-147">To save the description and finish later, select **Save draft**.</span></span>

5. <span data-ttu-id="f43f5-148">İşiniz bittiğinde, **gözden geçir ve Yayımla**' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-148">When you’re finished, select **Review and publish**.</span></span> <span data-ttu-id="f43f5-149">Plan bilgileri artık teklif listesi (planlar bölümü) altında appsource.microsoft.com üzerinde görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="f43f5-149">The plan information will now be displayed on appsource.microsoft.com under offer listing (plans section).</span></span>

6. <span data-ttu-id="f43f5-150">Bu teklif için tüm planları oluşturduktan sonra, her planın hizmet KIMLIĞINI kopyalamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="f43f5-150">After you’ve created all of the plans for this offer, you’ll need to copy each plan’s Service ID.</span></span> <span data-ttu-id="f43f5-151">Plan listesi sayfasının en üstünde **plana genel bakış ' ı** seçin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-151">Select **Plan overview** at the top of the Plan listing page.</span></span> <span data-ttu-id="f43f5-152">Her planın hizmet KIMLIĞINI güvenli bir konuma kopyalayın.</span><span class="sxs-lookup"><span data-stu-id="f43f5-152">Copy the Service ID for each plan to a safe location.</span></span>

## <a name="add-service-ids-to-your-solution"></a><span data-ttu-id="f43f5-153">Çözümünüze hizmet kimlikleri ekleyin</span><span class="sxs-lookup"><span data-stu-id="f43f5-153">Add Service IDs to your solution</span></span>

<span data-ttu-id="f43f5-154">Bir sonraki adım, yeni kopyaladığınız her plana ait hizmet kimliklerini ekleyerek çözümünüzü güncelleştirmedir.</span><span class="sxs-lookup"><span data-stu-id="f43f5-154">The next step is to update your solution by adding the Service IDs for each plan that you just copied.</span></span> <span data-ttu-id="f43f5-155">Bunun hakkında yönergeler için bkz. [çözümünüz Için AppSource paketi oluşturma](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span><span class="sxs-lookup"><span data-stu-id="f43f5-155">For guidance on this, see [Create an AppSource Package for your solution](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span></span>

## <a name="upload-your-package-and-publish-your-offer"></a><span data-ttu-id="f43f5-156">Paketinizi karşıya yükleyin ve teklifinizi yayımlayın</span><span class="sxs-lookup"><span data-stu-id="f43f5-156">Upload your package and publish your offer</span></span>

1. <span data-ttu-id="f43f5-157">Sol gezinti bölmesinde, **ticari Market**' i seçin ve ardından **Teknik yapılandırma**' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-157">On the left navigation pane, select **Commercial Marketplace**, and then select **Technical configuration**.</span></span>
2. <span data-ttu-id="f43f5-158">**Temel lisans modeli** altında **Kullanıcı**' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-158">Under **Base License Model**, select **User**.</span></span>
3. <span data-ttu-id="f43f5-159">**CRM paketi** altında, paket KONUMLARıNıZıN URL 'sini girin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-159">Under **CRM Package**, enter the URL of your package location.</span></span>
4. <span data-ttu-id="f43f5-160">Diğer gerekli bilgileri girmek için sol gezinti bölmesindeki diğer sekmeleri kullanın.</span><span class="sxs-lookup"><span data-stu-id="f43f5-160">Use the other tabs on the left navigation pane to enter any other required information.</span></span> <span data-ttu-id="f43f5-161">İşiniz bittiğinde, **gözden geçir ve Yayımla**' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-161">When you’re done, select **Review and publish**.</span></span>

<span data-ttu-id="f43f5-162">Teklifi yayımladıktan sonra bilgilerinizi gözden geçireceğiz ve doğrulayacağız.</span><span class="sxs-lookup"><span data-stu-id="f43f5-162">After you publish the offer, we’ll review and verify your information.</span></span> <span data-ttu-id="f43f5-163">Bu işlemle ilgili herhangi bir sorun varsa sizi bilgilendireceğiz.</span><span class="sxs-lookup"><span data-stu-id="f43f5-163">If there are any issues with this process, we’ll notify you.</span></span> <span data-ttu-id="f43f5-164">Tüm sorunlar çözümlendikten sonra teklifinizin AppSource 'ta kullanılabildiğini belirten bir bildirim alırsınız.</span><span class="sxs-lookup"><span data-stu-id="f43f5-164">When all issues have been resolved, you’ll get a notification that your offer is available in AppSource.</span></span> <span data-ttu-id="f43f5-165">Bu noktada, onu canlı hale getirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f43f5-165">At that point you can make it live.</span></span>

## <a name="make-your-offer-live-in-partner-center"></a><span data-ttu-id="f43f5-166">Teklifinizi Iş Ortağı Merkezi 'nde canlı hale getirin</span><span class="sxs-lookup"><span data-stu-id="f43f5-166">Make your offer live in Partner Center</span></span>

<span data-ttu-id="f43f5-167">Aşağıdaki yordam, teklifinizi AppSource 'ta canlı hale getirme sürecinde size yol gösterir.</span><span class="sxs-lookup"><span data-stu-id="f43f5-167">The procedure below walks you through the process of making your offer live in AppSource.</span></span> <span data-ttu-id="f43f5-168">Bu işlem hakkında daha fazla bilgi edinmek için bkz. [listeye giriş seçenekleri](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span><span class="sxs-lookup"><span data-stu-id="f43f5-168">To learn more about this process, see [Introduction to listing options](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span></span>

>[!NOTE]
><span data-ttu-id="f43f5-169">Teklifinizi yayımladıktan sonra, bu işlem 4-6 saat sürer.</span><span class="sxs-lookup"><span data-stu-id="f43f5-169">Once you publish your offer, it will take 4-6 hours to go live.</span></span>

1. <span data-ttu-id="f43f5-170">[İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="f43f5-170">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="f43f5-171">Sol gezinti menüsünde **ticari Market/genel bakış**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-171">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="f43f5-172">**Genel bakış** sayfasında, aradığınız teklifi bulun.</span><span class="sxs-lookup"><span data-stu-id="f43f5-172">On the **Overview** page, find the offer you’re looking for.</span></span> <span data-ttu-id="f43f5-173">Yayımlanmaya hazırlanma teklifleri **Önizleme** durumuna sahip olur.</span><span class="sxs-lookup"><span data-stu-id="f43f5-173">Offers ready to be published will have a status of **Preview**.</span></span> <span data-ttu-id="f43f5-174">Teklifi seçin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-174">Select the offer.</span></span>
4. <span data-ttu-id="f43f5-175">**Teklifin genel bakış** sayfasında **canlı git**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-175">On the **Offer overview** page, select **Go live**.</span></span>
<span data-ttu-id="f43f5-176">Teklif 4-6 saat içinde etkin olacaktır.</span><span class="sxs-lookup"><span data-stu-id="f43f5-176">The offer will be live in 4-6 hours.</span></span>
5. <span data-ttu-id="f43f5-177">AppSource 'ta teklif listelemeyi görmek için, **teklif genel bakış** sayfasının alt kısmındaki **appsource** bağlantısını seçin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-177">To see your offer listing on AppSource, select the **AppSource** link at the bottom of the **Offer overview** page.</span></span>

    - <span data-ttu-id="f43f5-178">**Lisans etkin teklifler için**: teklifiniz bir lisans denetimi gerektiriyorsa, kullanıcılar bu kişilerle iletişim kurabilmesi Için yalnızca **benimle iletişim** kuracak bir müşteri adayı girebilecektir.</span><span class="sxs-lookup"><span data-stu-id="f43f5-178">**For license-enabled offers**: If your offer requires a license check, users will only be able to enter a lead by clicking **Contact Me**, so that you can communicate with them.</span></span>

    - <span data-ttu-id="f43f5-179">**Ücretsiz yükleme seçeneğiyle lisans etkin teklifler için**: teklifiniz bir lisans denetimi gerektirmiyorsa, yönetici kullanıcılar **bana başvurmaya** ek olarak **Şimdi bir şimdi al** düğmesine sahip olur.</span><span class="sxs-lookup"><span data-stu-id="f43f5-179">**For license-enabled offers with free installation option**: If your offer does not require a license check, admin users will see a **Get It Now** button in addition to **Contact Me**.</span></span> <span data-ttu-id="f43f5-180">Ücretsiz yükleme seçeneğinizi denemek isteyen kullanıcılar **Şimdi al**' a tıklamalıdır, bu, teklifi Power platform yönetim merkezine yüklemeye getirir.</span><span class="sxs-lookup"><span data-stu-id="f43f5-180">Users who want to try your free installation option should click **Get It Now**, which will bring them to install the offer on Power Platform Admin Center.</span></span> <span data-ttu-id="f43f5-181">Kullanıcılar, herhangi bir sorunuz varsa veya ücretli bir plana yükseltmek istediklerinde **benimle Iletişim kurma** 'yı kullanmaya devam edebilir.</span><span class="sxs-lookup"><span data-stu-id="f43f5-181">Users can still use **Contact Me** if they have any questions, or if they want to upgrade to a paid plan.</span></span>

## <a name="register-isv-connect-deal-in-dealreg"></a><span data-ttu-id="f43f5-182">Satıcılarla ilgili ISV bağlantısı anlaşmayı Kaydet</span><span class="sxs-lookup"><span data-stu-id="f43f5-182">Register ISV Connect deal in DealReg</span></span>

<span data-ttu-id="f43f5-183">Bir sonraki adım, anlaşmayı kaydetmenizi sağlar.</span><span class="sxs-lookup"><span data-stu-id="f43f5-183">The next step is to register your deal.</span></span> <span data-ttu-id="f43f5-184">Bunu yapmak için bkz. [anlaşmaları kaydetme](https://docs.microsoft.com/partner-center/register-deals).</span><span class="sxs-lookup"><span data-stu-id="f43f5-184">To do this, see [Register your deals](https://docs.microsoft.com/partner-center/register-deals).</span></span>

## <a name="invite-the-customer"></a><span data-ttu-id="f43f5-185">Müşteriyi davet etme</span><span class="sxs-lookup"><span data-stu-id="f43f5-185">Invite the customer</span></span>

<span data-ttu-id="f43f5-186">Müşteriyi bu başa katılmaya davet etmek için aşağıdaki yordamı kullanın.</span><span class="sxs-lookup"><span data-stu-id="f43f5-186">Use the following procedure to invite the customer to participate in this deal.</span></span>  

1. <span data-ttu-id="f43f5-187">[İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="f43f5-187">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="f43f5-188">Sol gezinti menüsünde **ticari Market/genel bakış**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-188">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="f43f5-189">**Gönderilen** anlaşmalar için filtre uygulayın, **devam eden** sekmesini seçin ve ardından istediğiniz anlaşmayı seçin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-189">Filter for **Submitted** deals, select the **In Progress** tab, and then select the deal you want.</span></span>
4. <span data-ttu-id="f43f5-190">Bu anlaşma için genel bakış sayfasında **Lisansları Yönet**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-190">On the overview page for this deal, select **Manage licenses**.</span></span>
5. <span data-ttu-id="f43f5-191">**Lisansları Yönet** penceresinde müşteri **ayrıntıları** açılır listesinden müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-191">In the **Manage licenses** window, select the customer from the **Customer details** dropdown list.</span></span> <span data-ttu-id="f43f5-192">Müşteri ilişkisi henüz yoksa, **+ Yeni müşteriyi onay olarak davet et**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-192">If the customer relationship does not exist yet, select **+Invite a new customer to consent**.</span></span>
6. <span data-ttu-id="f43f5-193">Görüntülenen bağlantıyı kopyalayın.</span><span class="sxs-lookup"><span data-stu-id="f43f5-193">Copy the link that is displayed.</span></span>
7. <span data-ttu-id="f43f5-194">Bu bağlantıyı, müşterinizin faturalandırma Yöneticisi veya genel yöneticisine e-posta ile gönderin ve bu bağlantıyı admin.microsoft.com erişmek ve oluşturduğunuz ilişkiyi kabul etmek ve yetkilendirmek için kullanın.</span><span class="sxs-lookup"><span data-stu-id="f43f5-194">Email this link to your customer’s billing admin or global admin, and have them use this link to access admin.microsoft.com and accept and authorize the relationship you’re establishing.</span></span>

    >[!NOTE]
    ><span data-ttu-id="f43f5-195">Müşteri bu adımı gerçekleştirene kadar ilişki kurulmayacak.</span><span class="sxs-lookup"><span data-stu-id="f43f5-195">The relationship will not be established until the customer performs this step.</span></span>

## <a name="activate-manage-and-remove-your-licenses"></a><span data-ttu-id="f43f5-196">Lisanslarınızı etkinleştirin, yönetin ve kaldırın</span><span class="sxs-lookup"><span data-stu-id="f43f5-196">Activate, manage, and remove your licenses</span></span>

<span data-ttu-id="f43f5-197">Müşteriniz kurulduktan sonra, teklifinizden planlar eklemeye başlayabilir ve her plana lisans atayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f43f5-197">Once your customer has been established, you can start adding plans from your offer and assigning licenses to each plan.</span></span>

1. <span data-ttu-id="f43f5-198">Bu anlaşma için Lisansları Yönet penceresinde **+ plan Ekle**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-198">In the Manage licenses window for this deal, select **+Add a plan**.</span></span>
2. <span data-ttu-id="f43f5-199">**Bu çözüm Için planları** ve lisans alanı **sayısını** tamamlayıp **Lisansları Güncelleştir**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-199">Complete the **Plans for this solution** and **Number of licenses** fields, and then select **Update licenses**.</span></span> <span data-ttu-id="f43f5-200">Lisanslar, müşteriler tarafından yönetilecek ve çalışanlara atanacak admin.microsoft.com adresinde kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="f43f5-200">The licenses will be available at admin.microsoft.com for customers to manage and assign to employees.</span></span>

    - <span data-ttu-id="f43f5-201">Mevcut bir planın lisans sayısını değiştirmek için, **Lisans sayısı** alanına yeni sayıyı girin ve ardından **Lisansları Güncelleştir**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-201">To change the number of licenses for an existing plan, enter the new number in the **Number of licenses** field and then select **Update licenses**.</span></span>

    - <span data-ttu-id="f43f5-202">Bir anlaşma için lisansları devre dışı bırakmak veya kaldırmak için, **Eylemler** alanındaki çöp kutusu simgesini seçin ve ardından **Lisansları Güncelleştir**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="f43f5-202">To deactivate or remove licenses for a deal, select the trash can icon in the **Actions** field and then select **Update licenses**.</span></span>