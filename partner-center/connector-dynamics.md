---
title: Dynamics 365 CRM Iş Ortağı Merkezi için ortak satış Bağlayıcısı
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ürün ortağı merkezindeki başvuruları, Dynamics 365 CRM için ortak satış Bağlayıcınız ile eşitler. Satıcılar daha sonra CRM sistemlerinizden Microsoft ile ortak bir şekilde satıtabilecekleri.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 18a54bf777cb987e8f486f85afcf277e04c1055c
ms.sourcegitcommit: 147813ba322653c989df5afe0b3bf0c252523a92
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/03/2020
ms.locfileid: "96556370"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="c99b2-104">Dynamics 365 CRM için ortak satış Bağlayıcısı – genel bakış</span><span class="sxs-lookup"><span data-stu-id="c99b2-104">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="c99b2-105">Uygun roller</span><span class="sxs-lookup"><span data-stu-id="c99b2-105">Appropriate roles</span></span>

- <span data-ttu-id="c99b2-106">Başvuru Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="c99b2-106">Referrals admin</span></span>
- <span data-ttu-id="c99b2-107">CRM 'de Sistem Yöneticisi veya sistem özelleştiricisi</span><span class="sxs-lookup"><span data-stu-id="c99b2-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="c99b2-108">İş Ortağı Merkezi ortak satış Bağlayıcısı, satıcılarınızın CRM sistemlerinizden Microsoft ile ortak satıtabmasını sağlar.</span><span class="sxs-lookup"><span data-stu-id="c99b2-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="c99b2-109">Ortak satış kurdukları anlaşmaları yönetmek için Iş Ortağı Merkezi 'ni kullanmaya eğitilmeleri gerekmez.</span><span class="sxs-lookup"><span data-stu-id="c99b2-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="c99b2-110">Ortak satış bağlayıcılarını kullanarak Microsoft satıcı 'ya yönelik yeni bir ortak satış başvurusu oluşturun, Microsoft satıcı 'dan başvurular alın, başvuruları kabul edin/reddedin, işlem değeri gibi işlem verilerini değiştirin ve kapanış tarihi.</span><span class="sxs-lookup"><span data-stu-id="c99b2-110">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="c99b2-111">Ayrıca, bu ortak satış konusunda Microsoft satıcılarından herhangi bir güncelleştirme de alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c99b2-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="c99b2-112">Tüm başvurularınızın iş ortağı Merkezi yerine tercih ettiğiniz CRM 'de çalışmasını sağlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c99b2-112">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="c99b2-113">Çözüm, Microsoft Power otomatikleştir çözümüne dayalıdır ve Iş Ortağı Merkezi API 'Lerini kullanır.</span><span class="sxs-lookup"><span data-stu-id="c99b2-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="c99b2-114">Yüklemeden önce önkoşulları</span><span class="sxs-lookup"><span data-stu-id="c99b2-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="c99b2-115">**Konu başlıkları**</span><span class="sxs-lookup"><span data-stu-id="c99b2-115">**Topics**</span></span>   |<span data-ttu-id="c99b2-116">**Ayrıntılar**</span><span class="sxs-lookup"><span data-stu-id="c99b2-116">**Details**</span></span>   |<span data-ttu-id="c99b2-117">**Bağlantılar**</span><span class="sxs-lookup"><span data-stu-id="c99b2-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="c99b2-118">Microsoft İş Ortağı Ağı KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="c99b2-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="c99b2-119">Geçerli bir MPN KIMLIĞI gerekir</span><span class="sxs-lookup"><span data-stu-id="c99b2-119">You need a valid MPN ID</span></span>|<span data-ttu-id="c99b2-120">[MPN](https://partner.microsoft.com/) 'ye katılması için</span><span class="sxs-lookup"><span data-stu-id="c99b2-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="c99b2-121">Cosatışı hazırlanıyor</span><span class="sxs-lookup"><span data-stu-id="c99b2-121">Cosell ready</span></span>|<span data-ttu-id="c99b2-122">IP/hizmet çözümünüz ortak satış için hazırlık olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="c99b2-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="c99b2-123">Microsoft ile satış</span><span class="sxs-lookup"><span data-stu-id="c99b2-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="c99b2-124">İş Ortağı Merkezi hesabı</span><span class="sxs-lookup"><span data-stu-id="c99b2-124">Partner Center account</span></span>|<span data-ttu-id="c99b2-125">Iş Ortağı Merkezi kiracısı ile ilişkili MPN KIMLIĞI, ortak satış çözümünüz ile ilişkili MPN KIMLIĞIYLE aynı olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="c99b2-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="c99b2-126">Bağlayıcıları dağıtmadan önce Iş Ortağı Merkezi portalındaki ortak satış başvurularınızı görebildiğinizi doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="c99b2-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="c99b2-127">Hesabınızı yönetme</span><span class="sxs-lookup"><span data-stu-id="c99b2-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="c99b2-128">İş Ortağı Merkezi Kullanıcı rolleri</span><span class="sxs-lookup"><span data-stu-id="c99b2-128">Partner Center user roles</span></span>|<span data-ttu-id="c99b2-129">Bağlayıcıları yükleyecek ve kullanacak çalışana bir başvuru Yöneticisi olmalıdır</span><span class="sxs-lookup"><span data-stu-id="c99b2-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="c99b2-130">Kullanıcı rollerini ve izinlerini atama</span><span class="sxs-lookup"><span data-stu-id="c99b2-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="c99b2-131">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="c99b2-131">Dynamics 365 CRM</span></span>|<span data-ttu-id="c99b2-132">CRM Kullanıcı rolü, Sistem Yöneticisi veya sistem özelleştiricisi</span><span class="sxs-lookup"><span data-stu-id="c99b2-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="c99b2-133">Dynamics 365 ' de rol atama</span><span class="sxs-lookup"><span data-stu-id="c99b2-133">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="c99b2-134">Güç otomatikleştirme akış hesabı</span><span class="sxs-lookup"><span data-stu-id="c99b2-134">Power Automate Flow Account</span></span>|<span data-ttu-id="c99b2-135">CRM Sistem Yöneticisi veya sistem özelleştirici için etkin bir [Güç otomatikleştirme](https://flow.microsoft.com) hesabı.</span><span class="sxs-lookup"><span data-stu-id="c99b2-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="c99b2-136">Bu kullanıcının, yüklemeden önce en az bir kez [Power otomatikleştirmek](https://flow.microsoft.com) için oturum açması gerekir.</span><span class="sxs-lookup"><span data-stu-id="c99b2-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="c99b2-137">Dynamics 365 için Iş Ortağı Merkezi başvuruları eşitlemesini (Power otomatikleştir çözümü) yükler</span><span class="sxs-lookup"><span data-stu-id="c99b2-137">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="c99b2-138">[Power otomatikleştirir](https://flow.microsoft.com) ' a gidin ve sağ üst köşedeki **ortamlar** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-138">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="c99b2-139">Bu adımda, kullanılabilir CRM örnekleri gösterilir.</span><span class="sxs-lookup"><span data-stu-id="c99b2-139">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="c99b2-140">Sağ üst köşedeki açılan listeden uygun CRM örneğini seçin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-140">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="c99b2-141">Sol gezinti çubuğunda **çözümler** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-141">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="c99b2-142">Üstteki menüde **AppSource aç** bağlantısına tıklayın.</span><span class="sxs-lookup"><span data-stu-id="c99b2-142">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource 'u aç":::

5. <span data-ttu-id="c99b2-144">Açılır ekranda **Dynamics365 Için Iş Ortağı Merkezi başvuruları bağlayıcıları** aratın.</span><span class="sxs-lookup"><span data-stu-id="c99b2-144">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="c99b2-145">**Şimdi al** düğmesine tıklayın ve ardından **devam edin**.</span><span class="sxs-lookup"><span data-stu-id="c99b2-145">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="c99b2-146">Bu, uygulamayı yüklemek için CRM (Dynamics 365) ortamını seçebileceğiniz sayfayı açar.</span><span class="sxs-lookup"><span data-stu-id="c99b2-146">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="c99b2-147">Hüküm ve koşulları kabul edin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-147">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="c99b2-148">Daha sonra **çözümlerinizi yönetme** sayfasına yönlendirilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c99b2-148">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="c99b2-149">Sayfanın alt kısmındaki ok düğmelerini kullanarak "Iş Ortağı Merkezi başvuruları" na gidin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-149">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="c99b2-150">**Yükleme zamanlandı** , Iş Ortağı Merkezi başvuruları çözümünün yanında görünmelidir.</span><span class="sxs-lookup"><span data-stu-id="c99b2-150">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="c99b2-151">Yükleme, 10-15 dakika sürer.</span><span class="sxs-lookup"><span data-stu-id="c99b2-151">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="c99b2-152">Yükleme tamamlandıktan sonra [Power otomatikleştirmeye](https://flow.microsoft.com) dönün ve sol gezinti alanından **çözümler** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-152">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="c99b2-153">**Dynamics 365 Için Iş Ortağı Merkezi başvuruları** , çözümler listesinden kullanılabilir olduğuna dikkat edin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-153">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="c99b2-154">**Dynamics 365 Için Iş Ortağı Merkezi başvuruları eşitlemesini** seçin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-154">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="c99b2-155">Aşağıdaki güç otomatikleşme akışları ve varlıkları mevcuttur:</span><span class="sxs-lookup"><span data-stu-id="c99b2-155">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Kullanılabilir CRMS 'ler":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="c99b2-157">En iyi yöntem: canlı çalışmadan önce test edin</span><span class="sxs-lookup"><span data-stu-id="c99b2-157">Best practice: test before you go live</span></span>

<span data-ttu-id="c99b2-158">Üretim ortamında güç otomatikleştirme çözümünü yüklemeden, yapılandırmadan ve özelleştirebilmeniz için, çözümü bir hazırlama CRM örneğinde test ettiğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="c99b2-158">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="c99b2-159">Microsoft Power otomatikleştir çözümünü hazırlama ortamına/CRM örneğine yükler.</span><span class="sxs-lookup"><span data-stu-id="c99b2-159">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="c99b2-160">Çözümün bir kopyasını oluşturun ve yapılandırma ve Power otomatikleştir akış özelleştirmelerinizi hazırlama ortamında çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="c99b2-160">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="c99b2-161">Çözümü bir hazırlama/CRM örneğinde test edin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-161">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="c99b2-162">Başarılı sayfasında, üretim örneğine yönetilen çözüm olarak içeri aktarın.</span><span class="sxs-lookup"><span data-stu-id="c99b2-162">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="c99b2-163">Çözümü yapılandırma</span><span class="sxs-lookup"><span data-stu-id="c99b2-163">Configure the solution</span></span>

1. <span data-ttu-id="c99b2-164">Çözümü CRM Örneğinizde yükledikten sonra [Power otomatikleştirmek](https://flow.microsoft.com/)' a geri gidin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-164">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>


2. <span data-ttu-id="c99b2-165">Sağ üst köşedeki **ortamlar** açılan penceresinden, Power otomatikleştir çözümünü yüklediğiniz CRM örneğini seçin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-165">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="c99b2-166">Üç Kullanıcı hesabını ilişkilendiren bağlantılar oluşturmanız gerekir:</span><span class="sxs-lookup"><span data-stu-id="c99b2-166">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="c99b2-167">Ortak Merkezi Kullanıcı başvuruları yönetici kimlik bilgileri</span><span class="sxs-lookup"><span data-stu-id="c99b2-167">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="c99b2-168">İş Ortağı Merkezi Etkinlikleri</span><span class="sxs-lookup"><span data-stu-id="c99b2-168">Partner Center Events</span></span>

   - <span data-ttu-id="c99b2-169">Çözüm içindeki Power otomatikleştirmede CRM Yöneticisi.</span><span class="sxs-lookup"><span data-stu-id="c99b2-169">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="c99b2-170">Sol gezinti çubuğundan **Bağlantılar** ' ı seçin ve listeden "Iş Ortağı Merkezi başvuruları" çözümünü seçin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-170">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="c99b2-171">**Bağlantı oluştur**' a tıklayarak bir bağlantı oluşturun.</span><span class="sxs-lookup"><span data-stu-id="c99b2-171">Create a connection by clicking **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/dynamics1.png" alt-text="Bağlantı oluşturma":::

      3. <span data-ttu-id="c99b2-173">Sağ üst köşedeki arama çubuğunda **Iş Ortağı Merkezi başvurularını (Önizleme)** arayın.</span><span class="sxs-lookup"><span data-stu-id="c99b2-173">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="c99b2-174">Iş Ortağı Merkezi kullanıcılarınız için, başvuru yöneticisinin kimlik bilgileri rolüyle bir bağlantı oluşturun.</span><span class="sxs-lookup"><span data-stu-id="c99b2-174">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="c99b2-175">Daha sonra, Iş Ortağı Merkezi kullanıcılarınız için, referanslar yöneticisinin kimlik bilgileriyle bir Iş Ortağı Merkezi olaylar bağlantısı oluşturun.</span><span class="sxs-lookup"><span data-stu-id="c99b2-175">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="c99b2-176">CRM yönetici kullanıcısı için Common Data Service (geçerli ortam) bağlantısı oluşturun.</span><span class="sxs-lookup"><span data-stu-id="c99b2-176">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>
       
     
      7. <span data-ttu-id="c99b2-177">Tüm bağlantılar eklendikten sonra ortamınızda aşağıdaki bağlantıları görmeniz gerekir:</span><span class="sxs-lookup"><span data-stu-id="c99b2-177">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

:::image type="content" source="images/cosellconnectors/dynamics2.png" alt-text="Bağlantılar":::
   
## <a name="edit-the-connections"></a><span data-ttu-id="c99b2-179">Bağlantıları düzenleme</span><span class="sxs-lookup"><span data-stu-id="c99b2-179">Edit the connections</span></span>

1. <span data-ttu-id="c99b2-180">**Çözümler** sayfasına dönün ve **Varsayılan çözüm**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-180">Return to the **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="c99b2-181">**Tüm**' a tıklayarak **Bağlantı başvurusunu (Önizleme)** seçin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-181">Select **Connection Reference (preview)** by clicking **All**.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics3.png" alt-text="Bağlan":::

2. <span data-ttu-id="c99b2-183">Üç nokta simgesini seçerek bağlantıların her birini tek tek düzenleyin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-183">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="c99b2-184">İlgili bağlantıları ekleyin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-184">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics4.png" alt-text="Listelenen bağlantılar"::: 

3.  <span data-ttu-id="c99b2-186">Akışları aşağıdaki sırada açın:</span><span class="sxs-lookup"><span data-stu-id="c99b2-186">Turn on the flows in the following sequence:</span></span>
- <span data-ttu-id="c99b2-187">İş Ortağı Merkezi Web kancası kaydı (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="c99b2-187">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="c99b2-188">Ortak satış başvurusu oluşturma – Dynamics 365-Iş Ortağı Merkezi (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="c99b2-188">Create Co-sell Referral – Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="c99b2-189">İş Ortağı Merkezi Microsoft ortak satış başvuruları Dynamics 365 'a (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="c99b2-189">Partner Center Microsoft Co-sell Referral Updates to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="c99b2-190">İş Ortağı Merkezi-Dynamics 365 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="c99b2-190">Partner Center to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="c99b2-191">Dynamics 365-Iş Ortağı Merkezi (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="c99b2-191">Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="c99b2-192">Dynamics 365 Iş Ortağı Merkezi (Insider Preview) fırsatı</span><span class="sxs-lookup"><span data-stu-id="c99b2-192">Dynamics 365 Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="c99b2-193">Dynamics 365 Microsoft Solutions for Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="c99b2-193">Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)</span></span>
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="c99b2-194">Kaynak değişikliği olaylarına kaydolmak için Web kancası API 'Lerini kullanma</span><span class="sxs-lookup"><span data-stu-id="c99b2-194">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="c99b2-195">Iş Ortağı Merkezi Web kancası API 'Leri, kaynak değişiklik olaylarına kaydolmanızı sağlar.</span><span class="sxs-lookup"><span data-stu-id="c99b2-195">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="c99b2-196">Bu değişiklik olayları, URL 'nize HTTP gönderileri olarak gönderilir.</span><span class="sxs-lookup"><span data-stu-id="c99b2-196">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="c99b2-197">URL 'nizi kaydetmek için **Iş Ortağı Merkezi Web kancası kaydı (Insider Preview)** güç otomatikleştirme akışı ' nı seçin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-197">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="c99b2-198">(A.) Iş Ortağı Merkezi kullanıcısına, aşağıdaki vurgulanmış şekilde, başvuru Yöneticisi kimlik bilgileri (b.) Iş Ortağı Merkezi etkinliklerine yönelik bağlantılar ekleyin</span><span class="sxs-lookup"><span data-stu-id="c99b2-198">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Tetikleyici":::

3. <span data-ttu-id="c99b2-200">Bu güncelleştirmeleri yaptığınızda şunu görürsünüz:</span><span class="sxs-lookup"><span data-stu-id="c99b2-200">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Web kancaları":::

4. <span data-ttu-id="c99b2-202">Değişikliklerinizi kaydedin ve **Aç '** ı seçin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-202">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="c99b2-203">Iş Ortağı Merkezi Web kancalarını olay değişikliklerini dinleyecek şekilde etkinleştirmek için aşağıdaki adımları uygulayın:</span><span class="sxs-lookup"><span data-stu-id="c99b2-203">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="c99b2-204">**Iş Ortağı Merkezi 'Ni Dynamics 365 'e (Insider Preview)** seçin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-204">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

6. <span data-ttu-id="c99b2-205">**Düzenle** simgesini seçin ve **bir http isteği alındığında** öğesini seçin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-205">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="c99b2-206">Belirtilen HTTP POST URL 'sini kopyalamak için **Kopyala** simgesini seçin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-206">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="URL'yi Kopyala":::

8. <span data-ttu-id="c99b2-208">Şimdi "Iş Ortağı Merkezi Web kancası kaydı 'nı (Insider Preview)" Power otomatikleştirmeyi seçin ve **Çalıştır**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-208">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="c99b2-209">Sağ bölmede "akış Çalıştır" penceresinin açık olduğundan emin olun ve **devam**' a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="c99b2-209">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="c99b2-210">Şu ayrıntıları girin:</span><span class="sxs-lookup"><span data-stu-id="c99b2-210">Enter the following details:</span></span>

    1. <span data-ttu-id="c99b2-211">**Http tetikleyici uç noktası**: önceki adımdan kopyalanmış URL</span><span class="sxs-lookup"><span data-stu-id="c99b2-211">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="c99b2-212">**Kaydolmak Için olaylar**: "başvuru oluşturuldu" ve "başvuru-güncelleştirildi"</span><span class="sxs-lookup"><span data-stu-id="c99b2-212">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="c99b2-213">Varsa **var olan tetikleyici uç noktalarının üzerine yaz**: Evet (Bu, mevcut tüm uç noktaların üzerine yazar.)</span><span class="sxs-lookup"><span data-stu-id="c99b2-213">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="c99b2-214">**Çalıştır** ' ı seçin ve **bitti** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-214">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="c99b2-215">Web kancası artık olayları oluşturmak ve güncelleştirmek için dinleme yapabilir.</span><span class="sxs-lookup"><span data-stu-id="c99b2-215">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="c99b2-216">Eşitleme adımlarını özelleştirme</span><span class="sxs-lookup"><span data-stu-id="c99b2-216">Customize synchronization steps</span></span>

<span data-ttu-id="c99b2-217">Ortak satış başvuruları Iş ortağı merkezi ve CRM sisteminiz arasında eşitlendiğinde, Iş Ortağı Merkezi BILGISAYAR üzerinde eşitlenen alanlar burada listelenir.</span><span class="sxs-lookup"><span data-stu-id="c99b2-217">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="c99b2-218">Genellikle CRM sistemleri oldukça özelleştirilir.</span><span class="sxs-lookup"><span data-stu-id="c99b2-218">Often CRM systems are highly customized.</span></span> <span data-ttu-id="c99b2-219">Power otomatikleştir akışlarını özelleştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c99b2-219">You can customize the Power Automate flows.</span></span> <span data-ttu-id="c99b2-220">Alan eşleme kılavuzunu izleyin ve gerekirse Power otomatikleştir akışlarının adımlarında uygun değişiklikleri yapın.</span><span class="sxs-lookup"><span data-stu-id="c99b2-220">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="c99b2-221">CRM eşlemelerine Microsoft Iş ortağı merkezleri sağlanır, ancak CRM ortamınıza göre alanları daha fazla özelleştirmeyi tercih edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c99b2-221">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="c99b2-222">Her bir güç otomatikleştirme akışının birden çok adımı gereksinimlerinize göre özelleştirilebilir.</span><span class="sxs-lookup"><span data-stu-id="c99b2-222">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="c99b2-223">Aşağıdakiler kullanılabilir özelleştirmeler örneğidir:</span><span class="sxs-lookup"><span data-stu-id="c99b2-223">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="c99b2-224">Iş ortağı merkezindeki oluştur veya Güncelleştir olaylarının CRM başvuru eşitlemesine yönelik alanlarını özelleştirmek için:</span><span class="sxs-lookup"><span data-stu-id="c99b2-224">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="c99b2-225">a.</span><span class="sxs-lookup"><span data-stu-id="c99b2-225">a.</span></span> <span data-ttu-id="c99b2-226">Iş Ortağı Merkezi 'ni Dynamics 365 (Insider Preview) veya Iş Ortağı Merkezi ' ni (Insider Preview) seçin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-226">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="c99b2-227">b.</span><span class="sxs-lookup"><span data-stu-id="c99b2-227">b.</span></span> <span data-ttu-id="c99b2-228">Power otomatikleştir akışını düzenlemek/özelleştirmek için **Düzenle** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-228">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="c99b2-229">c.</span><span class="sxs-lookup"><span data-stu-id="c99b2-229">c.</span></span> <span data-ttu-id="c99b2-230">**Müşteri adayını veya fırsatı eşitlemeyi (kapsam)** seçin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-230">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="c99b2-231">Olay oluşturma için CRM alan eşlemelerini (alan eşlemeleri kılavuzuna göre) özelleştirmek için, **Yeni paylaşılan fırsat ' ı seçin ve ardından**.</span><span class="sxs-lookup"><span data-stu-id="c99b2-231">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="c99b2-232">**Evet ise** alt adımı seçin ve ardından **CRM 'de yeni fırsat oluşturma**' yı genişletin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-232">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="c99b2-233">Bu bölümdeki eşlemeleri alan eşleme kılavuzunu kullanarak düzenleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c99b2-233">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="c99b2-234">d.</span><span class="sxs-lookup"><span data-stu-id="c99b2-234">d.</span></span> <span data-ttu-id="c99b2-235">Güncelleştirme olayları için CRM alan eşlemelerini özelleştirmek için (alan eşlemeleri kılavuzuna göre), "(kapsam) müşteri adayını veya fırsatı eşitlemeyi" adımına tıklayın.</span><span class="sxs-lookup"><span data-stu-id="c99b2-235">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="c99b2-236">e.</span><span class="sxs-lookup"><span data-stu-id="c99b2-236">e.</span></span> <span data-ttu-id="c99b2-237">Bir **fırsata yönelik güncelleştirme olup olmadığını seçin, sonra**.</span><span class="sxs-lookup"><span data-stu-id="c99b2-237">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="c99b2-238">**Evet ise** alt adımı seçin ve ardından **iş ortağı merkezi ve CRM 'deki fırsat nesneleri arasında fark olursa** öğesini genişletin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-238">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="c99b2-239">f.</span><span class="sxs-lookup"><span data-stu-id="c99b2-239">f.</span></span> <span data-ttu-id="c99b2-240">**Mevcut fırsatı Güncelleştir** ' in ardından **Evet** ' i seçin</span><span class="sxs-lookup"><span data-stu-id="c99b2-240">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="c99b2-241">CRM için alanları güncelleştirme olayları için başvuru eşitlemesine göre özelleştirmek için:</span><span class="sxs-lookup"><span data-stu-id="c99b2-241">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="c99b2-242">a.</span><span class="sxs-lookup"><span data-stu-id="c99b2-242">a.</span></span> <span data-ttu-id="c99b2-243">Power otomatikleştir akışını düzenlemek/özelleştirmek için **Düzenle**  ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-243">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="c99b2-244">b.</span><span class="sxs-lookup"><span data-stu-id="c99b2-244">b.</span></span> <span data-ttu-id="c99b2-245">**Fırsatı (kapsam) eşitlemeyi** seçin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-245">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="c99b2-246">c.</span><span class="sxs-lookup"><span data-stu-id="c99b2-246">c.</span></span> <span data-ttu-id="c99b2-247">Güncelleştirme olayları için CRM alan eşlemelerini özelleştirmek için, **Iş ortağı merkezi ve CRM 'deki lider nesneleri arasında fark olup olmadığını** seçin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-247">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="c99b2-248">d.</span><span class="sxs-lookup"><span data-stu-id="c99b2-248">d.</span></span> <span data-ttu-id="c99b2-249">**Evet ise** alt adımı seçin ve ardından **fırsat verileriyle bir başvuruyu güncelleştir** adımını genişletin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-249">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="c99b2-250">Bu bölümdeki eşlemeleri alan eşleme kılavuzuna göre düzenleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c99b2-250">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="c99b2-251">CRM için alanları, oluşturma olayları için bir BILGISAYAR başvurusu eşitlemesine göre özelleştirmek için?</span><span class="sxs-lookup"><span data-stu-id="c99b2-251">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="c99b2-252">a.</span><span class="sxs-lookup"><span data-stu-id="c99b2-252">a.</span></span> <span data-ttu-id="c99b2-253">Power otomatikleştir akışını düzenlemek/özelleştirmek için **Düzenle**  ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-253">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="c99b2-254">b.</span><span class="sxs-lookup"><span data-stu-id="c99b2-254">b.</span></span> <span data-ttu-id="c99b2-255">**Başvuruları eşitleme (kapsam)** seçeneğini belirleyin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-255">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="c99b2-256">c.</span><span class="sxs-lookup"><span data-stu-id="c99b2-256">c.</span></span> <span data-ttu-id="c99b2-257">Olay oluşturma için CRM alan eşlemelerini özelleştirmek için (alan eşlemeleri kılavuzuna göre) **Microsoft başvurusu oluştur**' u seçin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-257">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

   <span data-ttu-id="c99b2-258">Bu bölümdeki eşlemeleri alan eşleme kılavuzuna göre düzenleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c99b2-258">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

<span data-ttu-id="c99b2-259">Oluşturulan iki ortam değişkeni vardır:</span><span class="sxs-lookup"><span data-stu-id="c99b2-259">There are two environment variables created:</span></span>

- <span data-ttu-id="c99b2-260">Onay işareti: Iş ortağı merkezi ve Dynamics 365 CRM arasında çift yönlü olarak eşitlenen fırsatların yanı sıra onay işareti simgesi gerekip gerekmediğini belirtir.</span><span class="sxs-lookup"><span data-stu-id="c99b2-260">Checkmark: Signifies whether you would need a checkmark icon besides opportunities that are synchronized bi-directionally between Partner Center and Dynamics 365 CRM.</span></span>

- <span data-ttu-id="c99b2-261">Yalnızca ortak satış fırsatlarını eşitleyin: yalnızca ortak satış fırsatlarını eşitlemek isteyip istemediğinizi belirtir.</span><span class="sxs-lookup"><span data-stu-id="c99b2-261">Sync co-sell opportunities only: Signifies whether you want to synchronize only Co-sell opportunities.</span></span>

<span data-ttu-id="c99b2-262">Ortam değişkenleri için varsayılan değeri düzenlemeyi seçebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c99b2-262">You can choose to edit the default value for the environment variables.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics5.png" alt-text="Varsayılan değerler için düzenleme kutusu":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="c99b2-264">Uçtan uca iki yönlü ortak satış başvuru eşitlemesi</span><span class="sxs-lookup"><span data-stu-id="c99b2-264">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="c99b2-265">Power otomatikleştir çözümünü yükledikten, yapılandırdıktan ve özelleştirdikten sonra, Dynamics 365 ve Iş ortağı merkezi arasında ortak satış başvuruları eşitlemesini test edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c99b2-265">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="c99b2-266">Ön koşullar</span><span class="sxs-lookup"><span data-stu-id="c99b2-266">Pre-requisites</span></span>

<span data-ttu-id="c99b2-267">Iş ortağı merkezi ve Dynamics 365 CRM arasındaki başvuruları eşleştirmek için, Power otomatikleştir çözümü, Microsoft 'a özgü başvuru alanlarını açıkça ortadan kaldırır.</span><span class="sxs-lookup"><span data-stu-id="c99b2-267">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="c99b2-268">Bu kimlik, satıcı ekiplerine ortak satış için Microsoft ile hangi referansları paylaşmak istediğini belirleme olanağı sağlar.</span><span class="sxs-lookup"><span data-stu-id="c99b2-268">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="c99b2-269">**Fırsat** varlığının bir parçası olarak bir dizi özel alan mevcuttur.</span><span class="sxs-lookup"><span data-stu-id="c99b2-269">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="c99b2-270">Bir CRM yönetici kullanıcısının **fırsat** özel alanlarıyla ayrı bir CRM bölümü oluşturması gerekir.</span><span class="sxs-lookup"><span data-stu-id="c99b2-270">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="c99b2-271">Aşağıdaki özel alanlar CRM bölümünün bir parçası olmalıdır:</span><span class="sxs-lookup"><span data-stu-id="c99b2-271">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="c99b2-272">**Iş Ortağı Merkezi Ile Eşitle**: fırsatın Microsoft Iş Ortağı Merkezi ile eşitlenmeyeceğini belirtir</span><span class="sxs-lookup"><span data-stu-id="c99b2-272">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="c99b2-273">**Başvuru tanımlayıcısı**: Microsoft Iş Ortağı Merkezi başvurusu için salt okunurdur bir tanımlayıcı alanı</span><span class="sxs-lookup"><span data-stu-id="c99b2-273">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="c99b2-274">**Başvuru bağlantısı**: Microsoft Iş Ortağı Merkezi 'nde başvuruya yönelik salt okunurdur bir bağlantı</span><span class="sxs-lookup"><span data-stu-id="c99b2-274">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="c99b2-275">**Microsoft nasıl yardım edebilir?**: başvuru için Microsoft 'un gerekli olduğu yardım</span><span class="sxs-lookup"><span data-stu-id="c99b2-275">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="c99b2-276">**Ürünler**: Bu fırsatla ilişkili ürünlerin listesi</span><span class="sxs-lookup"><span data-stu-id="c99b2-276">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="c99b2-277">**Denetim**: Iş Ortağı Merkezi başvurularına eşitleme için salt okunurdur bir denetim izi</span><span class="sxs-lookup"><span data-stu-id="c99b2-277">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

<span data-ttu-id="c99b2-278">Dynamics 365 CRM 'deki fırsat formunu ürün çözümlerini içerecek şekilde güncelleştirin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-278">Update the opportunity form in Dynamics 365 CRM to include Solutions for Products field.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics6.png" alt-text="Fırsat formu":::

:::image type="content" source="images/cosellconnectors/dynamics7.png" alt-text="{alternatif-metin}":::

### <a name="scenarios"></a><span data-ttu-id="c99b2-281">LARLA</span><span class="sxs-lookup"><span data-stu-id="c99b2-281">SCENARIOS:</span></span>

1. <span data-ttu-id="c99b2-282">CRM 'de başvuru oluşturulduğunda veya güncelleştirilirken ve Iş Ortağı Merkezi 'nde eşitlendiğinde başvuru eşitlemesi:</span><span class="sxs-lookup"><span data-stu-id="c99b2-282">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="c99b2-283">Dynamics 365 CRM ortamınızda, CRM 'nin **fırsat** bölümünde görünürlük olan kullanıcıyla oturum açın.</span><span class="sxs-lookup"><span data-stu-id="c99b2-283">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="c99b2-284">Dynamics 365 ortamında "yeni fırsat" oluşturduğunuzda aşağıdaki bölümün mevcut olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="c99b2-284">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Dynamics 365 ' de Microsoft Iş Ortağı Merkezi bilgilerini gösteren örnek fırsat bölümü.":::

   3. <span data-ttu-id="c99b2-286">Bu fırsatı Microsoft Iş Ortağı Merkezi ile eşleştirmek için, kart görünümünde aşağıdaki alanları ayarlamış olduğunuzdan emin olun:</span><span class="sxs-lookup"><span data-stu-id="c99b2-286">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="c99b2-287">**Iş Ortağı Merkezi Ile Eşitle**: Evet</span><span class="sxs-lookup"><span data-stu-id="c99b2-287">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="c99b2-288">**Microsoft nasıl yardım edebilir?**: aşağıdakilerden seçim yapın:</span><span class="sxs-lookup"><span data-stu-id="c99b2-288">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Dynamics 365 ' de, Microsoft 'un nasıl yardım edebilir adlı bir alanın yanında Microsoft Iş Ortağı Merkezi yardım seçeneklerini gösteren örnek fırsat bölümü.":::

      - <span data-ttu-id="c99b2-290">**Ürünler**: ürünün çözüm kimlikleri</span><span class="sxs-lookup"><span data-stu-id="c99b2-290">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="c99b2-291">Fırsat Dynamics 365 ' de **Iş Ortağı Merkezi Ile Eşitle** seçeneği **Evet** olarak ayarlandığında, 10 dakika bekleyin ve ardından iş ortağı Merkezi hesabınızda oturum açın.</span><span class="sxs-lookup"><span data-stu-id="c99b2-291">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="c99b2-292">Başvurularınız Dynamics 365 ile eşitlenir.</span><span class="sxs-lookup"><span data-stu-id="c99b2-292">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="c99b2-293">Benzer şekilde, "Partner Center ile eşitleme" seçeneği "Evet" olarak ayarlanmış bir fırsat için, Dynamics 365 CRM 'de fırsatı güncelleştirirseniz değişiklikler Iş Ortağı Merkezi hesabınızda eşitlenir.</span><span class="sxs-lookup"><span data-stu-id="c99b2-293">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="c99b2-294">Iş Ortağı Merkezi ile başarıyla eşitlenen fırsatlar, Dynamics 365 ' de ✔ simgesiyle tanımlanır.</span><span class="sxs-lookup"><span data-stu-id="c99b2-294">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="c99b2-295">Microsoft Iş Ortağı Merkezi 'nde başvuru oluşturulduğunda veya güncelleştirilirken ve Dynamics 365 ortamında eşitlendiğinde başvuru eşitlemesi:</span><span class="sxs-lookup"><span data-stu-id="c99b2-295">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="c99b2-296">Iş Ortağı Merkezi [panonuzda](https://partner.microsoft.com/dashboard/home)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="c99b2-296">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="c99b2-297">Sol taraftaki menüden **referanslar** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-297">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="c99b2-298">"Yeni anlaşma" seçeneğine tıklayarak Iş Ortağı Merkezi 'nden yeni bir ortak satış başvurusu oluşturun.</span><span class="sxs-lookup"><span data-stu-id="c99b2-298">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="c99b2-299">Dynamics 365 CRM ortamınızda oturum açın.</span><span class="sxs-lookup"><span data-stu-id="c99b2-299">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="c99b2-300">**Açık fırsatlara** gidin.</span><span class="sxs-lookup"><span data-stu-id="c99b2-300">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="c99b2-301">Microsoft Iş Ortağı Merkezi 'nde oluşturulan başvuru artık Dynamics 365 CRM 'de eşitlendi.</span><span class="sxs-lookup"><span data-stu-id="c99b2-301">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="c99b2-302">Eşitlenmiş bir başvuruyu seçtiğinizde, kart Görünümü ayrıntıları doldurulur.</span><span class="sxs-lookup"><span data-stu-id="c99b2-302">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c99b2-303">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="c99b2-303">Next steps</span></span>

- [<span data-ttu-id="c99b2-304">Müşteri adaylarını yönetme</span><span class="sxs-lookup"><span data-stu-id="c99b2-304">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="c99b2-305">Ortak satış fırsatlarını yönetme</span><span class="sxs-lookup"><span data-stu-id="c99b2-305">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="c99b2-306">Microsoft Power otomatikleştir platformu hakkında daha fazla bilgi</span><span class="sxs-lookup"><span data-stu-id="c99b2-306">More about Microsoft Power Automate platform?</span></span>](/power-automate/)

- [<span data-ttu-id="c99b2-307">İş Ortağı Merkezi Web kancaları</span><span class="sxs-lookup"><span data-stu-id="c99b2-307">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)