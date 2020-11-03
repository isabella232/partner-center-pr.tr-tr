---
title: Dynamics 365 CRM Iş Ortağı Merkezi için ortak satış Bağlayıcısı
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Iş ortağı merkezindeki başvurularınızı Dynamics 365 CRM için ortak satış Bağlayıcınız ile senkronize edin. Satıcılar daha sonra CRM sistemlerinizden Microsoft ile ortak bir şekilde satıtabilecekleri.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 8ea803e675ce7c2d21d680491bbdaedf792e631f
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/14/2020
ms.locfileid: "92531895"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="01b35-104">Dynamics 365 CRM için ortak satış Bağlayıcısı – genel bakış</span><span class="sxs-lookup"><span data-stu-id="01b35-104">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="01b35-105">Uygun roller</span><span class="sxs-lookup"><span data-stu-id="01b35-105">Appropriate roles</span></span>

- <span data-ttu-id="01b35-106">Başvuru Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="01b35-106">Referrals admin</span></span>
- <span data-ttu-id="01b35-107">CRM 'de Sistem Yöneticisi veya sistem özelleştiricisi</span><span class="sxs-lookup"><span data-stu-id="01b35-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="01b35-108">İş Ortağı Merkezi ortak satış Bağlayıcısı, satıcılarınızın CRM sistemlerinizden Microsoft ile ortak satıtabmasını sağlar.</span><span class="sxs-lookup"><span data-stu-id="01b35-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="01b35-109">Ortak satış kurdukları anlaşmaları yönetmek için Iş Ortağı Merkezi 'ni kullanmaya eğitilmeleri gerekmez.</span><span class="sxs-lookup"><span data-stu-id="01b35-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="01b35-110">Ortak satış bağlayıcılarını kullanarak Microsoft satıcı 'ya yönelik yeni bir ortak satış başvurusu oluşturun, Microsoft satıcı 'dan başvurular alın, başvuruları kabul edin/reddedin, işlem değeri gibi işlem verilerini değiştirin ve kapanış tarihi.</span><span class="sxs-lookup"><span data-stu-id="01b35-110">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="01b35-111">Ayrıca, bu ortak satış konusunda Microsoft satıcılarından herhangi bir güncelleştirme de alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="01b35-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="01b35-112">Tüm başvurularınızın iş ortağı Merkezi yerine tercih ettiğiniz CRM 'de çalışmasını sağlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="01b35-112">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="01b35-113">Çözüm, Microsoft Power otomatikleştir çözümüne dayalıdır ve Iş Ortağı Merkezi API 'Lerini kullanır.</span><span class="sxs-lookup"><span data-stu-id="01b35-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="01b35-114">Yüklemeden önce önkoşulları</span><span class="sxs-lookup"><span data-stu-id="01b35-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="01b35-115">**Konu başlıkları**</span><span class="sxs-lookup"><span data-stu-id="01b35-115">**Topics**</span></span>   |<span data-ttu-id="01b35-116">**Ayrıntılar**</span><span class="sxs-lookup"><span data-stu-id="01b35-116">**Details**</span></span>   |<span data-ttu-id="01b35-117">**Bağlantılar**</span><span class="sxs-lookup"><span data-stu-id="01b35-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="01b35-118">Microsoft İş Ortağı Ağı KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="01b35-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="01b35-119">Geçerli bir MPN KIMLIĞI gerekir</span><span class="sxs-lookup"><span data-stu-id="01b35-119">You need a valid MPN ID</span></span>|<span data-ttu-id="01b35-120">[MPN](https://partner.microsoft.com/) 'ye katılması için</span><span class="sxs-lookup"><span data-stu-id="01b35-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="01b35-121">Cosatışı hazırlanıyor</span><span class="sxs-lookup"><span data-stu-id="01b35-121">Cosell ready</span></span>|<span data-ttu-id="01b35-122">IP/hizmet çözümünüz ortak satış için hazırlık olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="01b35-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="01b35-123">Microsoft ile satış</span><span class="sxs-lookup"><span data-stu-id="01b35-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="01b35-124">İş Ortağı Merkezi hesabı</span><span class="sxs-lookup"><span data-stu-id="01b35-124">Partner Center account</span></span>|<span data-ttu-id="01b35-125">Iş Ortağı Merkezi kiracısı ile ilişkili MPN KIMLIĞI, ortak satış çözümünüz ile ilişkili MPN KIMLIĞIYLE aynı olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="01b35-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="01b35-126">Bağlayıcıları dağıtmadan önce Iş Ortağı Merkezi portalındaki ortak satış başvurularınızı görebildiğinizi doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="01b35-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="01b35-127">Hesabınızı yönetme</span><span class="sxs-lookup"><span data-stu-id="01b35-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="01b35-128">İş Ortağı Merkezi Kullanıcı rolleri</span><span class="sxs-lookup"><span data-stu-id="01b35-128">Partner Center user roles</span></span>|<span data-ttu-id="01b35-129">Bağlayıcıları yükleyecek ve kullanacak çalışana bir başvuru Yöneticisi olmalıdır</span><span class="sxs-lookup"><span data-stu-id="01b35-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="01b35-130">Kullanıcı rollerini ve izinlerini atama</span><span class="sxs-lookup"><span data-stu-id="01b35-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="01b35-131">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="01b35-131">Dynamics 365 CRM</span></span>|<span data-ttu-id="01b35-132">CRM Kullanıcı rolü, Sistem Yöneticisi veya sistem özelleştiricisi</span><span class="sxs-lookup"><span data-stu-id="01b35-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="01b35-133">Dynamics 365 ' de rol atama</span><span class="sxs-lookup"><span data-stu-id="01b35-133">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="01b35-134">Güç otomatikleştirme akış hesabı</span><span class="sxs-lookup"><span data-stu-id="01b35-134">Power Automate Flow Account</span></span>|<span data-ttu-id="01b35-135">CRM Sistem Yöneticisi veya sistem özelleştirici için etkin bir [Güç otomatikleştirme](https://flow.microsoft.com) hesabı.</span><span class="sxs-lookup"><span data-stu-id="01b35-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="01b35-136">Bu kullanıcının, yüklemeden önce en az bir kez [Power otomatikleştirmek](https://flow.microsoft.com) için oturum açması gerekir.</span><span class="sxs-lookup"><span data-stu-id="01b35-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="01b35-137">Dynamics 365 için Iş Ortağı Merkezi başvuruları eşitlemesini (Power otomatikleştir çözümü) yükler</span><span class="sxs-lookup"><span data-stu-id="01b35-137">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="01b35-138">[Power otomatikleştirir](https://flow.microsoft.com) ' a gidin ve sağ üst köşedeki **ortamlar** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="01b35-138">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="01b35-139">Bu adımda, kullanılabilir CRM örnekleri gösterilir.</span><span class="sxs-lookup"><span data-stu-id="01b35-139">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="01b35-140">Sağ üst köşedeki açılan listeden uygun CRM örneğini seçin.</span><span class="sxs-lookup"><span data-stu-id="01b35-140">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="01b35-141">Sol gezinti çubuğunda **çözümler** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="01b35-141">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="01b35-142">Üstteki menüde **AppSource aç** bağlantısına tıklayın.</span><span class="sxs-lookup"><span data-stu-id="01b35-142">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource 'u aç":::

5. <span data-ttu-id="01b35-144">Açılır ekranda **Dynamics365 Için Iş Ortağı Merkezi başvuruları bağlayıcıları** aratın.</span><span class="sxs-lookup"><span data-stu-id="01b35-144">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="01b35-145">**Şimdi al** düğmesine tıklayın ve ardından **devam edin** .</span><span class="sxs-lookup"><span data-stu-id="01b35-145">Click the **Get it now** button and then **Continue** .</span></span>

7. <span data-ttu-id="01b35-146">Bu, uygulamayı yüklemek için CRM (Dynamics 365) ortamını seçebileceğiniz sayfayı açar.</span><span class="sxs-lookup"><span data-stu-id="01b35-146">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="01b35-147">Hüküm ve koşulları kabul edin.</span><span class="sxs-lookup"><span data-stu-id="01b35-147">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="01b35-148">Daha sonra **çözümlerinizi yönetme** sayfasına yönlendirilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="01b35-148">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="01b35-149">Sayfanın alt kısmındaki ok düğmelerini kullanarak "Iş Ortağı Merkezi başvuruları" na gidin.</span><span class="sxs-lookup"><span data-stu-id="01b35-149">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="01b35-150">**Yükleme zamanlandı** , Iş Ortağı Merkezi başvuruları çözümünün yanında görünmelidir.</span><span class="sxs-lookup"><span data-stu-id="01b35-150">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="01b35-151">Yükleme, 10-15 dakika sürer.</span><span class="sxs-lookup"><span data-stu-id="01b35-151">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="01b35-152">Yükleme tamamlandıktan sonra [Power otomatikleştirmeye](https://flow.microsoft.com) dönün ve sol gezinti alanından **çözümler** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="01b35-152">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="01b35-153">**Dynamics 365 Için Iş Ortağı Merkezi başvuruları** , çözümler listesinden kullanılabilir olduğuna dikkat edin.</span><span class="sxs-lookup"><span data-stu-id="01b35-153">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="01b35-154">**Dynamics 365 Için Iş Ortağı Merkezi başvuruları eşitlemesini** seçin.</span><span class="sxs-lookup"><span data-stu-id="01b35-154">Select **Partner Center Referrals Synchronization for Dynamics 365** .</span></span> <span data-ttu-id="01b35-155">Aşağıdaki güç otomatikleşme akışları ve varlıkları mevcuttur:</span><span class="sxs-lookup"><span data-stu-id="01b35-155">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Kullanılabilir CRMS 'ler":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="01b35-157">En iyi yöntem: canlı çalışmadan önce test edin</span><span class="sxs-lookup"><span data-stu-id="01b35-157">Best practice: test before you go live</span></span>

<span data-ttu-id="01b35-158">Üretim ortamında güç otomatikleştirme çözümünü yüklemeden, yapılandırmadan ve özelleştirebilmeniz için, çözümü bir hazırlama CRM örneğinde test ettiğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="01b35-158">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="01b35-159">Microsoft Power otomatikleştir çözümünü hazırlama ortamına/CRM örneğine yükler.</span><span class="sxs-lookup"><span data-stu-id="01b35-159">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="01b35-160">Çözümün bir kopyasını oluşturun ve yapılandırma ve Power otomatikleştir akış özelleştirmelerinizi hazırlama ortamında çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="01b35-160">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="01b35-161">Çözümü bir hazırlama/CRM örneğinde test edin.</span><span class="sxs-lookup"><span data-stu-id="01b35-161">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="01b35-162">Başarılı sayfasında, üretim örneğine yönetilen çözüm olarak içeri aktarın.</span><span class="sxs-lookup"><span data-stu-id="01b35-162">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="01b35-163">Çözümü yapılandırma</span><span class="sxs-lookup"><span data-stu-id="01b35-163">Configure the solution</span></span>

1. <span data-ttu-id="01b35-164">Çözümü CRM Örneğinizde yükledikten sonra [Power otomatikleştirmek](https://flow.microsoft.com/)' a geri gidin.</span><span class="sxs-lookup"><span data-stu-id="01b35-164">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="01b35-165">Sağ üst köşedeki **ortamlar** açılan penceresinden, Power otomatikleştir çözümünü yüklediğiniz CRM örneğini seçin.</span><span class="sxs-lookup"><span data-stu-id="01b35-165">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="01b35-166">Üç Kullanıcı hesabını ilişkilendiren bağlantılar oluşturmanız gerekir:</span><span class="sxs-lookup"><span data-stu-id="01b35-166">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="01b35-167">Ortak Merkezi Kullanıcı başvuruları yönetici kimlik bilgileri</span><span class="sxs-lookup"><span data-stu-id="01b35-167">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="01b35-168">İş Ortağı Merkezi Etkinlikleri</span><span class="sxs-lookup"><span data-stu-id="01b35-168">Partner Center Events</span></span>

   - <span data-ttu-id="01b35-169">Çözüm içindeki Power otomatikleştirmede CRM Yöneticisi.</span><span class="sxs-lookup"><span data-stu-id="01b35-169">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="01b35-170">Sol gezinti çubuğundan **Bağlantılar** ' ı seçin ve listeden "Iş Ortağı Merkezi başvuruları" çözümünü seçin.</span><span class="sxs-lookup"><span data-stu-id="01b35-170">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="01b35-171">**Bağlantı oluştur** ' a tıklayarak bir bağlantı oluşturun.</span><span class="sxs-lookup"><span data-stu-id="01b35-171">Create a connection by clicking **Create a connection** .</span></span>

         :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="Bağlantı oluşturma":::

      3. <span data-ttu-id="01b35-173">Sağ üst köşedeki arama çubuğunda **Iş Ortağı Merkezi başvurularını (Önizleme)** arayın.</span><span class="sxs-lookup"><span data-stu-id="01b35-173">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="01b35-174">Iş Ortağı Merkezi kullanıcılarınız için, başvuru yöneticisinin kimlik bilgileri rolüyle bir bağlantı oluşturun.</span><span class="sxs-lookup"><span data-stu-id="01b35-174">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="01b35-175">Daha sonra, Iş Ortağı Merkezi kullanıcılarınız için, referanslar yöneticisinin kimlik bilgileriyle bir Iş Ortağı Merkezi olaylar bağlantısı oluşturun.</span><span class="sxs-lookup"><span data-stu-id="01b35-175">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="01b35-176">CRM yönetici kullanıcısı için Common Data Service (geçerli ortam) bağlantısı oluşturun.</span><span class="sxs-lookup"><span data-stu-id="01b35-176">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="01b35-177">Power otomatikleştir akışlarını bağlantılarla ilişkilendirmek için, Common Data Service ve Iş Ortağı Merkezi başvurularına bağlanmak üzere her güç otomatikleştirme akışını düzenleyin.</span><span class="sxs-lookup"><span data-stu-id="01b35-177">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="01b35-178">Değişiklikleri kaydedin.</span><span class="sxs-lookup"><span data-stu-id="01b35-178">Save the changes.</span></span>

5. <span data-ttu-id="01b35-179">Power otomatikleştir akışlarını **açın** .</span><span class="sxs-lookup"><span data-stu-id="01b35-179">**Turn on** the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="01b35-180">Kaynak değişikliği olaylarına kaydolmak için Web kancası API 'Lerini kullanma</span><span class="sxs-lookup"><span data-stu-id="01b35-180">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="01b35-181">Iş Ortağı Merkezi Web kancası API 'Leri, kaynak değişiklik olaylarına kaydolmanızı sağlar.</span><span class="sxs-lookup"><span data-stu-id="01b35-181">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="01b35-182">Bu değişiklik olayları, URL 'nize HTTP gönderileri olarak gönderilir.</span><span class="sxs-lookup"><span data-stu-id="01b35-182">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="01b35-183">URL 'nizi kaydetmek için **Iş Ortağı Merkezi Web kancası kaydı (Insider Preview)** güç otomatikleştirme akışı ' nı seçin.</span><span class="sxs-lookup"><span data-stu-id="01b35-183">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="01b35-184">(A.) Iş Ortağı Merkezi kullanıcısına, aşağıdaki vurgulanmış şekilde, başvuru Yöneticisi kimlik bilgileri (b.) Iş Ortağı Merkezi etkinliklerine yönelik bağlantılar ekleyin</span><span class="sxs-lookup"><span data-stu-id="01b35-184">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Tetikleyici":::

3. <span data-ttu-id="01b35-186">Bu güncelleştirmeleri yaptığınızda şunu görürsünüz:</span><span class="sxs-lookup"><span data-stu-id="01b35-186">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Web Kancaları":::

4. <span data-ttu-id="01b35-188">Değişikliklerinizi kaydedin ve **Aç '** ı seçin.</span><span class="sxs-lookup"><span data-stu-id="01b35-188">Save your changes and select **Turn on** .</span></span>

   <span data-ttu-id="01b35-189">Iş Ortağı Merkezi Web kancalarını olay değişikliklerini dinleyecek şekilde etkinleştirmek için aşağıdaki adımları uygulayın:</span><span class="sxs-lookup"><span data-stu-id="01b35-189">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="01b35-190">**Iş Ortağı Merkezi 'Ni Dynamics 365 'e (Insider Preview)** seçin.</span><span class="sxs-lookup"><span data-stu-id="01b35-190">Select **Partner Center to Dynamics 365 (Insider Preview)** .</span></span>

6. <span data-ttu-id="01b35-191">**Düzenle** simgesini seçin ve **bir http isteği alındığında** öğesini seçin.</span><span class="sxs-lookup"><span data-stu-id="01b35-191">Select the **Edit** icon and select **When a HTTP request is received** .</span></span>

7. <span data-ttu-id="01b35-192">Belirtilen HTTP POST URL 'sini kopyalamak için **Kopyala** simgesini seçin.</span><span class="sxs-lookup"><span data-stu-id="01b35-192">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="URL'yi Kopyala":::

8. <span data-ttu-id="01b35-194">Şimdi "Iş Ortağı Merkezi Web kancası kaydı 'nı (Insider Preview)" Power otomatikleştirmeyi seçin ve **Çalıştır** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="01b35-194">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run** .</span></span>

9. <span data-ttu-id="01b35-195">Sağ bölmede "akış Çalıştır" penceresinin açık olduğundan emin olun ve **devam** ' a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="01b35-195">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue** .</span></span>

10. <span data-ttu-id="01b35-196">Şu ayrıntıları girin:</span><span class="sxs-lookup"><span data-stu-id="01b35-196">Enter the following details:</span></span>

    1. <span data-ttu-id="01b35-197">**Http tetikleyici uç noktası** : önceki adımdan kopyalanmış URL</span><span class="sxs-lookup"><span data-stu-id="01b35-197">**Http Trigger Endpoint** : URL copied from earlier step</span></span>

    2. <span data-ttu-id="01b35-198">**Kaydolmak Için olaylar** : "başvuru oluşturuldu" ve "başvuru-güncelleştirildi"</span><span class="sxs-lookup"><span data-stu-id="01b35-198">**Events to Register** : “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="01b35-199">Varsa **var olan tetikleyici uç noktalarının üzerine yaz** : Evet (Bu, mevcut tüm uç noktaların üzerine yazar.)</span><span class="sxs-lookup"><span data-stu-id="01b35-199">**Overwrite existing trigger endpoints if present** : Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="01b35-200">**Çalıştır** ' ı seçin ve **bitti** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="01b35-200">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="01b35-201">Web kancası artık olayları oluşturmak ve güncelleştirmek için dinleme yapabilir.</span><span class="sxs-lookup"><span data-stu-id="01b35-201">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="01b35-202">Eşitleme adımlarını özelleştirme</span><span class="sxs-lookup"><span data-stu-id="01b35-202">Customize synchronization steps</span></span>

<span data-ttu-id="01b35-203">Ortak satış başvuruları Iş ortağı merkezi ve CRM sisteminiz arasında eşitlendiğinde, Iş Ortağı Merkezi BILGISAYAR üzerinde eşitlenen alanlar burada listelenir.</span><span class="sxs-lookup"><span data-stu-id="01b35-203">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="01b35-204">Genellikle CRM sistemleri oldukça özelleştirilir.</span><span class="sxs-lookup"><span data-stu-id="01b35-204">Often CRM systems are highly customized.</span></span> <span data-ttu-id="01b35-205">Power otomatikleştir akışlarını özelleştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="01b35-205">You can customize the Power Automate flows.</span></span> <span data-ttu-id="01b35-206">Alan eşleme kılavuzunu izleyin ve gerekirse Power otomatikleştir akışlarının adımlarında uygun değişiklikleri yapın.</span><span class="sxs-lookup"><span data-stu-id="01b35-206">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="01b35-207">CRM eşlemelerine Microsoft Iş ortağı merkezleri sağlanır, ancak CRM ortamınıza göre alanları daha fazla özelleştirmeyi tercih edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="01b35-207">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="01b35-208">Her bir güç otomatikleştirme akışının birden çok adımı gereksinimlerinize göre özelleştirilebilir.</span><span class="sxs-lookup"><span data-stu-id="01b35-208">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="01b35-209">Aşağıdakiler kullanılabilir özelleştirmeler örneğidir:</span><span class="sxs-lookup"><span data-stu-id="01b35-209">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="01b35-210">Iş ortağı merkezindeki oluştur veya Güncelleştir olaylarının CRM başvuru eşitlemesine yönelik alanlarını özelleştirmek için:</span><span class="sxs-lookup"><span data-stu-id="01b35-210">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="01b35-211">a.</span><span class="sxs-lookup"><span data-stu-id="01b35-211">a.</span></span> <span data-ttu-id="01b35-212">Iş Ortağı Merkezi 'ni Dynamics 365 (Insider Preview) veya Iş Ortağı Merkezi ' ni (Insider Preview) seçin.</span><span class="sxs-lookup"><span data-stu-id="01b35-212">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="01b35-213">b.</span><span class="sxs-lookup"><span data-stu-id="01b35-213">b.</span></span> <span data-ttu-id="01b35-214">Power otomatikleştir akışını düzenlemek/özelleştirmek için **Düzenle** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="01b35-214">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="01b35-215">c.</span><span class="sxs-lookup"><span data-stu-id="01b35-215">c.</span></span> <span data-ttu-id="01b35-216">**Müşteri adayını veya fırsatı eşitlemeyi (kapsam)** seçin.</span><span class="sxs-lookup"><span data-stu-id="01b35-216">Select **(Scope) Synchronize the lead or opportunity** .</span></span>

2. <span data-ttu-id="01b35-217">Olay oluşturma için CRM alan eşlemelerini (alan eşlemeleri kılavuzuna göre) özelleştirmek için, **Yeni paylaşılan fırsat ' ı seçin ve ardından** .</span><span class="sxs-lookup"><span data-stu-id="01b35-217">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then** .</span></span> <span data-ttu-id="01b35-218">**Evet ise** alt adımı seçin ve ardından **CRM 'de yeni fırsat oluşturma** ' yı genişletin.</span><span class="sxs-lookup"><span data-stu-id="01b35-218">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM** .</span></span> <span data-ttu-id="01b35-219">Bu bölümdeki eşlemeleri alan eşleme kılavuzunu kullanarak düzenleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="01b35-219">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="01b35-220">d.</span><span class="sxs-lookup"><span data-stu-id="01b35-220">d.</span></span> <span data-ttu-id="01b35-221">Güncelleştirme olayları için CRM alan eşlemelerini özelleştirmek için (alan eşlemeleri kılavuzuna göre), "(kapsam) müşteri adayını veya fırsatı eşitlemeyi" adımına tıklayın.</span><span class="sxs-lookup"><span data-stu-id="01b35-221">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="01b35-222">e.</span><span class="sxs-lookup"><span data-stu-id="01b35-222">e.</span></span> <span data-ttu-id="01b35-223">Bir **fırsata yönelik güncelleştirme olup olmadığını seçin, sonra** .</span><span class="sxs-lookup"><span data-stu-id="01b35-223">Select **If it’s an update to an opportunity, then** .</span></span> <span data-ttu-id="01b35-224">**Evet ise** alt adımı seçin ve ardından **iş ortağı merkezi ve CRM 'deki fırsat nesneleri arasında fark olursa** öğesini genişletin.</span><span class="sxs-lookup"><span data-stu-id="01b35-224">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then** .</span></span>  

    <span data-ttu-id="01b35-225">f.</span><span class="sxs-lookup"><span data-stu-id="01b35-225">f.</span></span> <span data-ttu-id="01b35-226">**Mevcut fırsatı Güncelleştir** ' in ardından **Evet** ' i seçin</span><span class="sxs-lookup"><span data-stu-id="01b35-226">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="01b35-227">CRM için alanları güncelleştirme olayları için başvuru eşitlemesine göre özelleştirmek için:</span><span class="sxs-lookup"><span data-stu-id="01b35-227">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="01b35-228">a.</span><span class="sxs-lookup"><span data-stu-id="01b35-228">a.</span></span> <span data-ttu-id="01b35-229">Power otomatikleştir akışını düzenlemek/özelleştirmek için **Düzenle**  ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="01b35-229">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="01b35-230">b.</span><span class="sxs-lookup"><span data-stu-id="01b35-230">b.</span></span> <span data-ttu-id="01b35-231">**Fırsatı (kapsam) eşitlemeyi** seçin.</span><span class="sxs-lookup"><span data-stu-id="01b35-231">Select **(Scope) Synchronize the opportunity** .</span></span>

    <span data-ttu-id="01b35-232">c.</span><span class="sxs-lookup"><span data-stu-id="01b35-232">c.</span></span> <span data-ttu-id="01b35-233">Güncelleştirme olayları için CRM alan eşlemelerini özelleştirmek için, **Iş ortağı merkezi ve CRM 'deki lider nesneleri arasında fark olup olmadığını** seçin.</span><span class="sxs-lookup"><span data-stu-id="01b35-233">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then** .</span></span> 

    <span data-ttu-id="01b35-234">d.</span><span class="sxs-lookup"><span data-stu-id="01b35-234">d.</span></span> <span data-ttu-id="01b35-235">**Evet ise** alt adımı seçin ve ardından **fırsat verileriyle bir başvuruyu güncelleştir** adımını genişletin.</span><span class="sxs-lookup"><span data-stu-id="01b35-235">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data** .</span></span>

   <span data-ttu-id="01b35-236">Bu bölümdeki eşlemeleri alan eşleme kılavuzuna göre düzenleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="01b35-236">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="01b35-237">CRM için alanları, oluşturma olayları için bir BILGISAYAR başvurusu eşitlemesine göre özelleştirmek için?</span><span class="sxs-lookup"><span data-stu-id="01b35-237">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="01b35-238">a.</span><span class="sxs-lookup"><span data-stu-id="01b35-238">a.</span></span> <span data-ttu-id="01b35-239">Power otomatikleştir akışını düzenlemek/özelleştirmek için **Düzenle**  ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="01b35-239">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="01b35-240">b.</span><span class="sxs-lookup"><span data-stu-id="01b35-240">b.</span></span> <span data-ttu-id="01b35-241">**Başvuruları eşitleme (kapsam)** seçeneğini belirleyin.</span><span class="sxs-lookup"><span data-stu-id="01b35-241">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="01b35-242">c.</span><span class="sxs-lookup"><span data-stu-id="01b35-242">c.</span></span> <span data-ttu-id="01b35-243">Olay oluşturma için CRM alan eşlemelerini özelleştirmek için (alan eşlemeleri kılavuzuna göre) **Microsoft başvurusu oluştur** ' u seçin.</span><span class="sxs-lookup"><span data-stu-id="01b35-243">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral** .</span></span>

   <span data-ttu-id="01b35-244">Bu bölümdeki eşlemeleri alan eşleme kılavuzuna göre düzenleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="01b35-244">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="01b35-245">Uçtan uca iki yönlü ortak satış başvuru eşitlemesi</span><span class="sxs-lookup"><span data-stu-id="01b35-245">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="01b35-246">Power otomatikleştir çözümünü yükledikten, yapılandırdıktan ve özelleştirdikten sonra, Dynamics 365 ve Iş ortağı merkezi arasında ortak satış başvuruları eşitlemesini test edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="01b35-246">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="01b35-247">Ön koşullar</span><span class="sxs-lookup"><span data-stu-id="01b35-247">Pre-requisites</span></span>

<span data-ttu-id="01b35-248">Iş ortağı merkezi ve Dynamics 365 CRM arasındaki başvuruları eşleştirmek için, Power otomatikleştir çözümü, Microsoft 'a özgü başvuru alanlarını açıkça ortadan kaldırır.</span><span class="sxs-lookup"><span data-stu-id="01b35-248">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="01b35-249">Bu kimlik, satıcı ekiplerine ortak satış için Microsoft ile hangi referansları paylaşmak istediğini belirleme olanağı sağlar.</span><span class="sxs-lookup"><span data-stu-id="01b35-249">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="01b35-250">**Fırsat** varlığının bir parçası olarak bir dizi özel alan mevcuttur.</span><span class="sxs-lookup"><span data-stu-id="01b35-250">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="01b35-251">Bir CRM yönetici kullanıcısının **fırsat** özel alanlarıyla ayrı bir CRM bölümü oluşturması gerekir.</span><span class="sxs-lookup"><span data-stu-id="01b35-251">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="01b35-252">Aşağıdaki özel alanlar CRM bölümünün bir parçası olmalıdır:</span><span class="sxs-lookup"><span data-stu-id="01b35-252">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="01b35-253">**Iş Ortağı Merkezi Ile Eşitle** : fırsatın Microsoft Iş Ortağı Merkezi ile eşitlenmeyeceğini belirtir</span><span class="sxs-lookup"><span data-stu-id="01b35-253">**Sync with Partner Center** : Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="01b35-254">**Başvuru tanımlayıcısı** : Microsoft Iş Ortağı Merkezi başvurusu için salt okunurdur bir tanımlayıcı alanı</span><span class="sxs-lookup"><span data-stu-id="01b35-254">**Referral Identifier** : A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="01b35-255">**Başvuru bağlantısı** : Microsoft Iş Ortağı Merkezi 'nde başvuruya yönelik salt okunurdur bir bağlantı</span><span class="sxs-lookup"><span data-stu-id="01b35-255">**Referral Link** : A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="01b35-256">**Microsoft nasıl yardım edebilir?** : başvuru için Microsoft 'un gerekli olduğu yardım</span><span class="sxs-lookup"><span data-stu-id="01b35-256">**How can Microsoft help?** : Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="01b35-257">**Ürünler** : Bu fırsatla ilişkili ürünlerin listesi</span><span class="sxs-lookup"><span data-stu-id="01b35-257">**Products** : List of products associated with this opportunity</span></span>

- <span data-ttu-id="01b35-258">**Denetim** : Iş Ortağı Merkezi başvurularına eşitleme için salt okunurdur bir denetim izi</span><span class="sxs-lookup"><span data-stu-id="01b35-258">**Audit** : A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="01b35-259">LARLA</span><span class="sxs-lookup"><span data-stu-id="01b35-259">SCENARIOS:</span></span>

1. <span data-ttu-id="01b35-260">CRM 'de başvuru oluşturulduğunda veya güncelleştirilirken ve Iş Ortağı Merkezi 'nde eşitlendiğinde başvuru eşitlemesi:</span><span class="sxs-lookup"><span data-stu-id="01b35-260">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="01b35-261">Dynamics 365 CRM ortamınızda, CRM 'nin **fırsat** bölümünde görünürlük olan kullanıcıyla oturum açın.</span><span class="sxs-lookup"><span data-stu-id="01b35-261">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="01b35-262">Dynamics 365 ortamında "yeni fırsat" oluşturduğunuzda aşağıdaki bölümün mevcut olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="01b35-262">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Dynamics 365 ' de Microsoft Iş Ortağı Merkezi bilgilerini gösteren örnek fırsat bölümü.":::

   3. <span data-ttu-id="01b35-264">Bu fırsatı Microsoft Iş Ortağı Merkezi ile eşleştirmek için, kart görünümünde aşağıdaki alanları ayarlamış olduğunuzdan emin olun:</span><span class="sxs-lookup"><span data-stu-id="01b35-264">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="01b35-265">**Iş Ortağı Merkezi Ile Eşitle** : Evet</span><span class="sxs-lookup"><span data-stu-id="01b35-265">**Sync with Partner Center** : Yes</span></span>

      - <span data-ttu-id="01b35-266">**Microsoft nasıl yardım edebilir?** : aşağıdakilerden seçim yapın:</span><span class="sxs-lookup"><span data-stu-id="01b35-266">**How can Microsoft help?** : Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Dynamics 365 ' de, Microsoft 'un nasıl yardım edebilir adlı bir alanın yanında Microsoft Iş Ortağı Merkezi yardım seçeneklerini gösteren örnek fırsat bölümü.":::

      - <span data-ttu-id="01b35-268">**Ürünler** : ürünün çözüm kimlikleri</span><span class="sxs-lookup"><span data-stu-id="01b35-268">**Products** : Solution IDs of the product</span></span>

   4. <span data-ttu-id="01b35-269">Fırsat Dynamics 365 ' de **Iş Ortağı Merkezi Ile Eşitle** seçeneği **Evet** olarak ayarlandığında, 10 dakika bekleyin ve ardından iş ortağı Merkezi hesabınızda oturum açın.</span><span class="sxs-lookup"><span data-stu-id="01b35-269">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes** , wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="01b35-270">Başvurularınız Dynamics 365 ile eşitlenir.</span><span class="sxs-lookup"><span data-stu-id="01b35-270">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="01b35-271">Benzer şekilde, "Partner Center ile eşitleme" seçeneği "Evet" olarak ayarlanmış bir fırsat için, Dynamics 365 CRM 'de fırsatı güncelleştirirseniz değişiklikler Iş Ortağı Merkezi hesabınızda eşitlenir.</span><span class="sxs-lookup"><span data-stu-id="01b35-271">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="01b35-272">Iş Ortağı Merkezi ile başarıyla eşitlenen fırsatlar, Dynamics 365 ' de ✔ simgesiyle tanımlanır.</span><span class="sxs-lookup"><span data-stu-id="01b35-272">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="01b35-273">Microsoft Iş Ortağı Merkezi 'nde başvuru oluşturulduğunda veya güncelleştirilirken ve Dynamics 365 ortamında eşitlendiğinde başvuru eşitlemesi:</span><span class="sxs-lookup"><span data-stu-id="01b35-273">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="01b35-274">Iş Ortağı Merkezi [panonuzda](https://partner.microsoft.com/dashboard/home)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="01b35-274">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="01b35-275">Sol taraftaki menüden **referanslar** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="01b35-275">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="01b35-276">"Yeni anlaşma" seçeneğine tıklayarak Iş Ortağı Merkezi 'nden yeni bir ortak satış başvurusu oluşturun.</span><span class="sxs-lookup"><span data-stu-id="01b35-276">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="01b35-277">Dynamics 365 CRM ortamınızda oturum açın.</span><span class="sxs-lookup"><span data-stu-id="01b35-277">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="01b35-278">**Açık fırsatlara** gidin.</span><span class="sxs-lookup"><span data-stu-id="01b35-278">Navigate to **Open Opportunities** .</span></span> <span data-ttu-id="01b35-279">Microsoft Iş Ortağı Merkezi 'nde oluşturulan başvuru artık Dynamics 365 CRM 'de eşitlendi.</span><span class="sxs-lookup"><span data-stu-id="01b35-279">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="01b35-280">Eşitlenmiş bir başvuruyu seçtiğinizde, kart Görünümü ayrıntıları doldurulur.</span><span class="sxs-lookup"><span data-stu-id="01b35-280">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="01b35-281">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="01b35-281">Next steps</span></span>

- [<span data-ttu-id="01b35-282">Müşteri adaylarını yönetme</span><span class="sxs-lookup"><span data-stu-id="01b35-282">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="01b35-283">Ortak satış fırsatlarını yönetme</span><span class="sxs-lookup"><span data-stu-id="01b35-283">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="01b35-284">Microsoft Power otomatikleştir platformu hakkında daha fazla bilgi</span><span class="sxs-lookup"><span data-stu-id="01b35-284">More about Microsoft Power Automate platform?</span></span>](/power-automate/)

- [<span data-ttu-id="01b35-285">İş Ortağı Merkezi Web kancaları</span><span class="sxs-lookup"><span data-stu-id="01b35-285">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)