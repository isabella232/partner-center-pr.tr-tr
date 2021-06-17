---
title: Salesforce CRM Iş Ortağı Merkezi için ortak satış Bağlayıcısı
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Iş ortağı merkezindeki başvurularınızı Salesforce CRM 'niz ile eşitler. Satıcılar daha sonra CRM sistemlerinizden Microsoft ile ortak bir şekilde satıtabilecekleri.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 74894671966ac0409f6366f33c91ddadfae1ba4c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276986"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="b0e5d-104">Salesforce için ortak satış Bağlayıcısı CRM-genel bakış</span><span class="sxs-lookup"><span data-stu-id="b0e5d-104">Co-sell connector for Salesforce CRM - overview</span></span>

<span data-ttu-id="b0e5d-105">**Uygun roller**: başvuru Yöneticisi | CRM 'de Sistem Yöneticisi veya sistem özelleştiricisi</span><span class="sxs-lookup"><span data-stu-id="b0e5d-105">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

<span data-ttu-id="b0e5d-106">İş Ortağı Merkezi ortak satış Bağlayıcısı, satıcılarınızın CRM sistemlerinizden Microsoft ile ortak satıtabmasını sağlar.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-106">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="b0e5d-107">Ortak satış kurdukları anlaşmaları yönetmek için Iş Ortağı Merkezi 'ni kullanmaya eğitilmeleri gerekmez.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-107">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="b0e5d-108">Ortak satış bağlayıcılarını kullanarak, Microsoft satıcı 'ya yönelik yeni bir ortak satış başvurusu oluşturabilir, Microsoft satıcı ile başvuruları alabilir, başvuruları kabul edebilir/reddedebilir, anlaşma değeri gibi işlem verilerini değiştirebilir ve kapanış tarihi gibi işlemleri yapabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-108">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="b0e5d-109">Ayrıca, bu ortak satış konusunda Microsoft satıcılarından herhangi bir güncelleştirme de alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-109">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="b0e5d-110">İş Ortağı Merkezi yerine tercih ettiğiniz CRM 'de çalışırken tüm başvurularınızı yapabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-110">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="b0e5d-111">Çözüm, Microsoft Power otomatikleştir çözümüne dayalıdır ve Iş Ortağı Merkezi API 'Lerini kullanır.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-111">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="b0e5d-112">Yüklemeden önce önkoşulları</span><span class="sxs-lookup"><span data-stu-id="b0e5d-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="b0e5d-113">**Konu başlıkları**</span><span class="sxs-lookup"><span data-stu-id="b0e5d-113">**Topics**</span></span>   |<span data-ttu-id="b0e5d-114">**Ayrıntılar**</span><span class="sxs-lookup"><span data-stu-id="b0e5d-114">**Details**</span></span>   |<span data-ttu-id="b0e5d-115">**Bağlantılar**</span><span class="sxs-lookup"><span data-stu-id="b0e5d-115">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="b0e5d-116">Microsoft İş Ortağı Ağı KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="b0e5d-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="b0e5d-117">Geçerli bir MPN KIMLIĞI gerekir</span><span class="sxs-lookup"><span data-stu-id="b0e5d-117">You need a valid MPN ID</span></span>|<span data-ttu-id="b0e5d-118">[MPN](https://partner.microsoft.com/) 'ye katılması için</span><span class="sxs-lookup"><span data-stu-id="b0e5d-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="b0e5d-119">Ortak satış hazırlanıyor</span><span class="sxs-lookup"><span data-stu-id="b0e5d-119">Co-sell ready</span></span>|<span data-ttu-id="b0e5d-120">IP/hizmet çözümünüz ortak satış için hazırlık olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="b0e5d-121">Microsoft ile satış</span><span class="sxs-lookup"><span data-stu-id="b0e5d-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="b0e5d-122">İş Ortağı Merkezi hesabı</span><span class="sxs-lookup"><span data-stu-id="b0e5d-122">Partner Center account</span></span>|<span data-ttu-id="b0e5d-123">Iş Ortağı Merkezi kiracısı ile ilişkili MPN KIMLIĞI, ortak satış çözümünüz ile ilişkili MPN KIMLIĞIYLE aynı olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="b0e5d-124">Bağlayıcıları dağıtmadan önce Iş Ortağı Merkezi portalındaki ortak satış başvurularınızı görebildiğinizi doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-124">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="b0e5d-125">Hesabınızı yönetme</span><span class="sxs-lookup"><span data-stu-id="b0e5d-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="b0e5d-126">İş Ortağı Merkezi Kullanıcı rolleri</span><span class="sxs-lookup"><span data-stu-id="b0e5d-126">Partner Center user roles</span></span>|<span data-ttu-id="b0e5d-127">Bağlayıcıları yükleyecek ve kullanacak çalışana bir başvuru Yöneticisi olmalıdır</span><span class="sxs-lookup"><span data-stu-id="b0e5d-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="b0e5d-128">Kullanıcı rollerini ve izinlerini atama</span><span class="sxs-lookup"><span data-stu-id="b0e5d-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="b0e5d-129">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="b0e5d-129">Salesforce CRM</span></span>|<span data-ttu-id="b0e5d-130">CRM Kullanıcı rolü, Sistem Yöneticisi veya sistem özelleştiricisi</span><span class="sxs-lookup"><span data-stu-id="b0e5d-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="b0e5d-131">Salesforce CRM 'de rol atama</span><span class="sxs-lookup"><span data-stu-id="b0e5d-131">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="b0e5d-132">Güç otomatikleştirme akış hesabı</span><span class="sxs-lookup"><span data-stu-id="b0e5d-132">Power Automate Flow Account</span></span>|<span data-ttu-id="b0e5d-133">CRM Sistem Yöneticisi veya sistem özelleştirici için etkin bir [Güç otomatikleştirme](https://flow.microsoft.com) hesabı.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-133">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="b0e5d-134">Bu kullanıcının, yüklemeden önce en az bir kez [Power otomatikleştirmek](https://flow.microsoft.com) için oturum açması gerekir.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-134">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="b0e5d-135">Microsoft özel alanları için Salesforce paketi yüklemesi</span><span class="sxs-lookup"><span data-stu-id="b0e5d-135">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="b0e5d-136">Iş ortağı merkezi ve Salesforce CRM genelindeki başvuruları senkronize etmek için, Power otomatikleştir çözümünün Microsoft 'a özgü başvuru alanlarını açıkça tanımlaması gerekir.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-136">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft-specific referral fields.</span></span> <span data-ttu-id="b0e5d-137">Bu düzenleme, iş ortağı satıcı ekiplerine ortak satış için Microsoft ile hangi başvuruları paylaşacağına karar verme olanağı sunar.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-137">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="b0e5d-138">Salesforce 'ta **notları** etkinleştirin ve fırsatlar ilgili listesine ekleyin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-138">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="b0e5d-139">Başvuru</span><span class="sxs-lookup"><span data-stu-id="b0e5d-139">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="b0e5d-140">Aşağıdaki adımları izleyerek **fırsat ekiplerini** etkinleştirin:</span><span class="sxs-lookup"><span data-stu-id="b0e5d-140">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="b0e5d-141">Kurulum 'da, fırsat ekibi ayarlarını bulmak için **hızlı bul** kutusunu kullanın.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-141">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="b0e5d-142">Ayarları gerektiği gibi tanımlayın.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-142">Define the settings as needed.</span></span>
[<span data-ttu-id="b0e5d-143">Başvuru</span><span class="sxs-lookup"><span data-stu-id="b0e5d-143">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="b0e5d-144">Salesforce 'ta, [paket yükleyicisini](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV)kullanarak özel alanlar ve nesneler yükleme.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-144">In Salesforce, install custom fields and objects using the [package installer](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span></span> <span data-ttu-id="b0e5d-145">Paketi herhangi bir şirkete yüklemek için bunu kullanın.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-145">Use this to install the package into any company.</span></span>

>[!NOTE]
><span data-ttu-id="b0e5d-146">Bir korumalı alana yüklüyorsanız, URL 'nin başlangıçtaki bölümünü ile değiştirmelisiniz http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="b0e5d-146">If you are installing into a sandbox, you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="b0e5d-147">Salesforce. Microsoft çözümlerini **fırsatla** ilgili listeye ekleyin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-147">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="b0e5d-148">Eklendikten sonra, **wrancon** simgesini ve Update özelliklerini seçin</span><span class="sxs-lookup"><span data-stu-id="b0e5d-148">Once added, select the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="b0e5d-149">En iyi yöntem: canlı çalışmadan önce test edin</span><span class="sxs-lookup"><span data-stu-id="b0e5d-149">Best Practice: Test before you go live</span></span>

<span data-ttu-id="b0e5d-150">Üretim ortamında güç otomatikleştirme çözümünü yüklemeden, yapılandırmadan ve özelleştirebilmeniz için, çözümü bir hazırlama CRM örneğinde test ettiğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-150">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="b0e5d-151">Microsoft Power otomatikleştir çözümünü hazırlama ortamına/CRM örneğine yükler.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-151">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="b0e5d-152">Çözümün bir kopyasını oluşturun ve yapılandırma ve Power otomatikleştir akış özelleştirmelerinizi hazırlama ortamında çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-152">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="b0e5d-153">Çözümü bir hazırlama/CRM örneğinde test edin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-153">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="b0e5d-154">Başarı durumunda, üretim örneğine yönetilen bir çözüm olarak içeri aktarın.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-154">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="b0e5d-155">Salesforce CRM için Iş ortağı merkezi başvuru eşitlemesini yükler</span><span class="sxs-lookup"><span data-stu-id="b0e5d-155">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="b0e5d-156">[Power otomatikleştirir](https://flow.microsoft.com) ' a gidin ve sağ üst köşedeki **ortamlar** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-156">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="b0e5d-157">Bu, size kullanılabilir CRM örneklerini gösterir.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-157">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="b0e5d-158">Sağ üst köşedeki açılan listeden uygun CRM örneğini seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-158">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="b0e5d-159">Sol gezinti çubuğunda **çözümler** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-159">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="b0e5d-160">Üstteki menüde **AppSource 'U aç** bağlantısını seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-160">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource 'u açın.":::

5. <span data-ttu-id="b0e5d-162">Açılır ekranda **Salesforce Için Iş Ortağı Merkezi başvuruları bağlayıcıları** arayın.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-162">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Satış.":::

6. <span data-ttu-id="b0e5d-164">**Şimdi al** düğmesini seçin ve sonra **devam edin**.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-164">Select the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="b0e5d-165">Bu, uygulamayı yüklemek için Salesforce CRM ortamını seçebileceğiniz sayfayı açar.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-165">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="b0e5d-166">Hüküm ve koşulları kabul edin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-166">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Kullanılabilir CRMS 'ler.":::

8. <span data-ttu-id="b0e5d-168">Daha sonra **çözümlerinizi yönetme** sayfasına yönlendirilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-168">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="b0e5d-169">Sayfanın alt kısmındaki ok düğmelerini kullanarak "Iş Ortağı Merkezi başvuruları" na gidin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-169">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="b0e5d-170">**Yükleme zamanlandı** , Iş Ortağı Merkezi başvuruları çözümünün yanında görünmelidir.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-170">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="b0e5d-171">Yükleme, 10-15 dakika sürer.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-171">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="b0e5d-172">Yükleme tamamlandıktan sonra [Power otomatikleştirmeye](https://flow.microsoft.com) dönün ve sol gezinti alanından **çözümler** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-172">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="b0e5d-173">**Salesforce Için Iş Ortağı Merkezi başvuruları** , çözümler listesinden kullanılabilir olduğuna dikkat edin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-173">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="b0e5d-174">**Salesforce Için Iş Ortağı Merkezi başvuruları eşitlemesini** seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-174">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="b0e5d-175">Aşağıdaki güç otomatikleşme akışları ve varlıkları mevcuttur:</span><span class="sxs-lookup"><span data-stu-id="b0e5d-175">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce akışları.":::



## <a name="configure-the-solution"></a><span data-ttu-id="b0e5d-177">Çözümü yapılandırma</span><span class="sxs-lookup"><span data-stu-id="b0e5d-177">Configure the solution</span></span>

1. <span data-ttu-id="b0e5d-178">Çözümü CRM Örneğinizde yükledikten sonra [Power otomatikleştirmek](https://flow.microsoft.com/)' a geri gidin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-178">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="b0e5d-179">Sağ üst köşedeki **ortamlar** açılan penceresinden, Power otomatikleştir çözümünü yüklediğiniz CRM örneğini seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-179">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="b0e5d-180">Üç Kullanıcı hesabını ilişkilendiren bağlantılar oluşturmanız gerekir:</span><span class="sxs-lookup"><span data-stu-id="b0e5d-180">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="b0e5d-181">Ortak Merkezi Kullanıcı başvuruları yönetici kimlik bilgileri</span><span class="sxs-lookup"><span data-stu-id="b0e5d-181">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="b0e5d-182">İş Ortağı Merkezi Etkinlikleri</span><span class="sxs-lookup"><span data-stu-id="b0e5d-182">Partner Center Events</span></span>
    - <span data-ttu-id="b0e5d-183">Çözüm içindeki Power otomatikleştirmede CRM Yöneticisi.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-183">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="b0e5d-184">Sol gezinti çubuğundan **Bağlantılar** ' ı seçin ve listeden "Iş Ortağı Merkezi başvuruları" çözümünü seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-184">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="b0e5d-185">**Bağlantı oluştur**' a tıklayarak bir bağlantı oluşturun.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-185">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Bağlantı oluştur.":::

- <span data-ttu-id="b0e5d-187">Sağ üst köşedeki arama çubuğunda Iş Ortağı Merkezi başvurularını (Önizleme) arayın.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-187">Search for Partner Center Referrals (preview) in the search bar on the top-right corner.</span></span>

- <span data-ttu-id="b0e5d-188">Iş Ortağı Merkezi kullanıcılarınız için, başvuru yöneticisinin kimlik bilgileri rolüyle bir bağlantı oluşturun.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-188">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="b0e5d-189">Daha sonra, Iş Ortağı Merkezi kullanıcılarınız için, referanslar yöneticisinin kimlik bilgileriyle bir Iş Ortağı Merkezi olaylar bağlantısı oluşturun.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-189">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="b0e5d-190">CRM yönetici kullanıcısı için Salesforce bağlantısı oluşturun.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-190">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="b0e5d-191">Tüm bağlantılar eklendikten sonra ortamınızda aşağıdaki bağlantıları görmeniz gerekir:</span><span class="sxs-lookup"><span data-stu-id="b0e5d-191">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Bağlantıları gözlemleyin.":::

### <a name="edit-the-connections"></a><span data-ttu-id="b0e5d-193">Bağlantıları düzenleme</span><span class="sxs-lookup"><span data-stu-id="b0e5d-193">Edit the connections</span></span>

1. <span data-ttu-id="b0e5d-194">Çözümler sayfasına dönün ve **Varsayılan çözüm**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-194">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="b0e5d-195">**Tüm**' a tıklayarak **Bağlantı başvurusunu (Önizleme)** seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-195">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Bağlayıcı düzenlemeyi Başlat.":::

2. <span data-ttu-id="b0e5d-197">Üç nokta simgesini seçerek her bir bağlantıyı tek tek düzenleyin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-197">Edit each of the Connections individually by selecting the three dots icon.</span></span> <span data-ttu-id="b0e5d-198">İlgili bağlantıları ekleyin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-198">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Bağlayıcıları düzenleyin.":::

3. <span data-ttu-id="b0e5d-200">Akışları aşağıdaki sırada açın:</span><span class="sxs-lookup"><span data-stu-id="b0e5d-200">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="b0e5d-201">İş Ortağı Merkezi Web kancası kaydı (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b0e5d-201">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="b0e5d-202">Ortak satış başvurusu oluşturma-Salesforce 'a Iş Ortağı Merkezi 'ne (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b0e5d-202">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="b0e5d-203">İş Ortağı Merkezi Microsoft ortak-başvuru güncelleştirmelerini Salesforce 'a satma (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b0e5d-203">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="b0e5d-204">İş ortağı merkezini Salesforce 'a (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b0e5d-204">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="b0e5d-205">Salesforce-Iş Ortağı Merkezi (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b0e5d-205">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="b0e5d-206">Salesforce Iş Ortağı Merkezi (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b0e5d-206">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="b0e5d-207">Salesforce Microsoft çözümlerini Iş Ortağı Merkezi 'ne (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b0e5d-207">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="b0e5d-208">Kaynak değişikliği olaylarına kaydolmak için Web kancası API 'Lerini kullanma</span><span class="sxs-lookup"><span data-stu-id="b0e5d-208">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="b0e5d-209">Iş Ortağı Merkezi Web kancası API 'Leri, kaynak değişiklik olaylarına kaydolmanızı sağlar.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-209">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="b0e5d-210">Bu değişiklik olayları, URL 'nize HTTP gönderileri olarak gönderilir.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-210">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="b0e5d-211">URL 'nizi kaydetmek için **Iş Ortağı Merkezi Web kancası kaydı (Insider Preview)** güç otomatikleştirme akışı ' nı seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-211">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="b0e5d-212">(A.) Iş Ortağı Merkezi kullanıcısına, aşağıdaki vurgulanmış şekilde, başvuru Yöneticisi kimlik bilgileri (b.) Iş Ortağı Merkezi etkinliklerine yönelik bağlantılar ekleyin</span><span class="sxs-lookup"><span data-stu-id="b0e5d-212">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Tetikleyicinin.":::

3. <span data-ttu-id="b0e5d-214">Bu güncelleştirmeleri yaptığınızda şunu görürsünüz:</span><span class="sxs-lookup"><span data-stu-id="b0e5d-214">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Web kancaları.":::

4. <span data-ttu-id="b0e5d-216">Değişikliklerinizi kaydedin ve **Aç '** ı seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-216">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="b0e5d-217">Iş Ortağı Merkezi Web kancalarını olay değişikliklerini dinleyecek şekilde etkinleştirmek için aşağıdaki adımları uygulayın:</span><span class="sxs-lookup"><span data-stu-id="b0e5d-217">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="b0e5d-218">**Iş ortağı merkezini SALESFORCE CRM 'ye (Insider Preview)** seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-218">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="b0e5d-219">**Düzenle** simgesini seçin ve **bir http isteği alındığında** öğesini seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-219">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="b0e5d-220">Belirtilen HTTP POST URL 'sini kopyalamak için **Kopyala** simgesini seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-220">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="URL 'YI kopyalayın.":::

8. <span data-ttu-id="b0e5d-222">Şimdi "Iş Ortağı Merkezi Web kancası kaydı 'nı (Insider Preview)" Power otomatikleştirmeyi seçin ve **Çalıştır**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-222">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="b0e5d-223">Sağ bölmede "akış Çalıştır" penceresinin açık olduğundan emin olun ve **devam**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-223">Ensure that the "Run Flow" window opens on the right-hand pane and select **Continue**.</span></span>

10. <span data-ttu-id="b0e5d-224">Şu ayrıntıları girin:</span><span class="sxs-lookup"><span data-stu-id="b0e5d-224">Enter the following details:</span></span>

    1. <span data-ttu-id="b0e5d-225">**Http tetikleyici uç noktası**: önceki adımdan kopyalanmış URL</span><span class="sxs-lookup"><span data-stu-id="b0e5d-225">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="b0e5d-226">**Kaydolmak Için olaylar**: "başvuru oluşturuldu" ve "başvuru-güncelleştirildi"</span><span class="sxs-lookup"><span data-stu-id="b0e5d-226">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="b0e5d-227">Varsa **var olan tetikleyici uç noktalarının üzerine yaz**: Evet (Bu, mevcut tüm uç noktaların üzerine yazar.)</span><span class="sxs-lookup"><span data-stu-id="b0e5d-227">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="b0e5d-228">**Çalıştır** ' ı seçin ve **bitti** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-228">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="b0e5d-229">Web kancası artık olayları oluşturmak ve güncelleştirmek için dinleme yapabilir.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-229">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="b0e5d-230">Eşitleme adımlarını özelleştirme</span><span class="sxs-lookup"><span data-stu-id="b0e5d-230">Customize synchronization steps</span></span>

<span data-ttu-id="b0e5d-231">Ortak satış başvuruları Iş ortağı merkezi ve CRM sisteminiz arasında eşitlendiğinde, Iş Ortağı Merkezi BILGISAYAR üzerinde eşitlenen alanlar burada listelenir.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-231">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="b0e5d-232">Genellikle CRM sistemleri oldukça özelleştirilir.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-232">Often CRM systems are highly customized.</span></span> <span data-ttu-id="b0e5d-233">Power otomatikleştir akışlarını özelleştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-233">You can customize the Power Automate flows.</span></span> <span data-ttu-id="b0e5d-234">Alan eşleme kılavuzunu izleyin ve gerekirse Power otomatikleştir akışlarının adımlarında uygun değişiklikleri yapın.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-234">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="b0e5d-235">CRM eşlemelerine Microsoft Iş ortağı merkezleri sağlanır, ancak CRM ortamınıza göre alanları daha fazla özelleştirmeyi tercih edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-235">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="b0e5d-236">Her bir güç otomatikleştirme akışının birden çok adımı gereksinimlerinize göre özelleştirilebilir.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-236">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="b0e5d-237">Aşağıdakiler kullanılabilir özelleştirmeler örneğidir:</span><span class="sxs-lookup"><span data-stu-id="b0e5d-237">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="b0e5d-238">Iş ortağı merkezindeki oluştur veya Güncelleştir olaylarının CRM başvuru eşitlemesine yönelik alanlarını özelleştirmek için:</span><span class="sxs-lookup"><span data-stu-id="b0e5d-238">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="b0e5d-239">Iş ortağı merkezini Salesforce CRM 'ye (Insider Preview) seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-239">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="b0e5d-240">Power otomatikleştir akışını düzenlemek/özelleştirmek için **Düzenle** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-240">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="b0e5d-241">**Müşteri adayını veya fırsatı eşitlemeyi (kapsam)** seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-241">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="b0e5d-242">Olay oluşturma için CRM alan eşlemelerini özelleştirmek için, **Yeni paylaşılan fırsat ' ı seçin ve ardından**.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-242">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="b0e5d-243">**Evet ise** alt adımı seçin ve ardından **CRM 'de yeni fırsat oluşturma**' yı genişletin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-243">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="b0e5d-244">Bu bölümdeki eşlemeleri alan eşleme kılavuzunu kullanarak düzenleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-244">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="b0e5d-245">Güncelleştirme olayları için CRM alan eşlemelerini özelleştirmek için "(kapsam) müşteri adayını veya fırsatı eşitlemeyi" adımını seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-245">To customize CRM field mappings for update events, select the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="b0e5d-246">Bir **fırsata yönelik güncelleştirme olup olmadığını seçin, sonra**.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-246">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="b0e5d-247">**Evet ise** alt adımı seçin ve ardından **iş ortağı merkezi ve CRM 'deki fırsat nesneleri arasında fark olursa** öğesini genişletin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-247">Select the sub-step **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="b0e5d-248">**Mevcut fırsatı Güncelleştir** ' in ardından **Evet** ' i seçin</span><span class="sxs-lookup"><span data-stu-id="b0e5d-248">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="b0e5d-249">CRM için alanları güncelleştirme olayları için başvuru eşitlemesine göre özelleştirmek için:</span><span class="sxs-lookup"><span data-stu-id="b0e5d-249">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="b0e5d-250">Power otomatikleştir akışını düzenlemek/özelleştirmek için **Düzenle**  ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-250">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="b0e5d-251">**Fırsatı (kapsam) eşitlemeyi** seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-251">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="b0e5d-252">Güncelleştirme olayları için CRM alan eşlemelerini özelleştirmek için (alan eşlemeleri kılavuzuna göre), **Iş ortağı merkezi ve CRM 'deki lider nesneleri arasında fark olup olmadığını** seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-252">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="b0e5d-253">**Evet ise** alt adımı seçin ve ardından **fırsat verileriyle bir başvuruyu güncelleştir** adımını genişletin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-253">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="b0e5d-254">Bu bölümdeki eşlemeleri alan eşleme kılavuzuna göre düzenleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-254">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="b0e5d-255">CRM için alanları, oluşturma olayları için bir BILGISAYAR başvurusu eşitlemesine göre özelleştirmek için?</span><span class="sxs-lookup"><span data-stu-id="b0e5d-255">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="b0e5d-256">Power otomatikleştir akışını düzenlemek/özelleştirmek için **Düzenle**  ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-256">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="b0e5d-257">**Başvuruları eşitleme (kapsam)** seçeneğini belirleyin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-257">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="b0e5d-258">Olay oluşturma için CRM alan eşlemelerini özelleştirmek için (alan eşlemeleri kılavuzuna göre) **Microsoft başvurusu oluştur**' u seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-258">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="b0e5d-259">Bu bölümdeki eşlemeleri alan eşleme kılavuzuna göre düzenleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-259">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="b0e5d-260">Uçtan uca iki yönlü ortak satış başvuru eşitlemesi</span><span class="sxs-lookup"><span data-stu-id="b0e5d-260">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="b0e5d-261">Power otomatikleştir çözümünü yükledikten, yapılandırdıktan ve özelleştirdikten sonra Salesforce CRM ve Iş ortağı merkezi arasında ortak satış başvuruları eşitlemesini test edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-261">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="b0e5d-262">Ön koşullar</span><span class="sxs-lookup"><span data-stu-id="b0e5d-262">Pre-requisites</span></span>

<span data-ttu-id="b0e5d-263">Iş ortağı merkezi ve Salesforce CRM genelindeki başvuruları senkronize etmek için, Power otomatikleştir çözümünün Microsoft 'a özgü başvuru alanlarını açıkça ortadan kaldırma ihtiyacı vardır.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-263">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="b0e5d-264">Bu kimlik, satıcı ekiplerinizi, ortak satış için Microsoft ile hangi referansları paylaşmak istediğlerine karar vermenize olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-264">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="b0e5d-265">Bir dizi özel alan, Salesforce CRM çözümü **fırsat** varlığı Için Iş Ortağı Merkezi başvuruları eşitlemesinin bir parçası olarak kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-265">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="b0e5d-266">Bir CRM yönetici kullanıcısının **fırsat** özel alanlarıyla ayrı bir CRM bölümü oluşturması gerekir.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-266">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="b0e5d-267">Aşağıdaki özel alanlar CRM bölümünün bir parçası olmalıdır:</span><span class="sxs-lookup"><span data-stu-id="b0e5d-267">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="b0e5d-268">**Iş Ortağı Merkezi Ile Eşitle**: fırsatın Microsoft Iş Ortağı Merkezi ile eşitlenmeyeceğini belirtir</span><span class="sxs-lookup"><span data-stu-id="b0e5d-268">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="b0e5d-269">**Başvuru tanımlayıcısı**: Microsoft Iş Ortağı Merkezi başvurusu için salt okunurdur bir tanımlayıcı alanı</span><span class="sxs-lookup"><span data-stu-id="b0e5d-269">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="b0e5d-270">**Başvuru bağlantısı**: Microsoft Iş Ortağı Merkezi 'nde başvuruya yönelik salt okunurdur bir bağlantı</span><span class="sxs-lookup"><span data-stu-id="b0e5d-270">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="b0e5d-271">**Microsoft 'un yardımı**: başvuru için Microsoft 'un gerekli yardımı</span><span class="sxs-lookup"><span data-stu-id="b0e5d-271">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="b0e5d-272">**Ürünler**: Bu fırsatla ilişkili ürünlerin listesi</span><span class="sxs-lookup"><span data-stu-id="b0e5d-272">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="b0e5d-273">**Denetim**: Iş Ortağı Merkezi başvurularına eşitleme için salt okunurdur bir denetim izi</span><span class="sxs-lookup"><span data-stu-id="b0e5d-273">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="b0e5d-274">LARLA</span><span class="sxs-lookup"><span data-stu-id="b0e5d-274">SCENARIOS:</span></span>

1. <span data-ttu-id="b0e5d-275">CRM 'de başvuru oluşturulduğunda veya güncelleştirilirken ve Iş Ortağı Merkezi 'nde eşitlendiğinde başvuru eşitlemesi:</span><span class="sxs-lookup"><span data-stu-id="b0e5d-275">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="b0e5d-276">CRM 'nin **fırsat** bölümünde görünürlük olan KULLANıCıYLA Salesforce CRM ortamınızda oturum açın.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-276">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="b0e5d-277">Salesforce CRM ortamında "yeni fırsat" oluşturduğunuzda aşağıdaki bölümün mevcut olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-277">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce ortamı.":::

   3. <span data-ttu-id="b0e5d-279">Bu fırsatı Microsoft Iş Ortağı Merkezi ile eşleştirmek için, kart görünümünde aşağıdaki alanları ayarlamış olduğunuzdan emin olun:</span><span class="sxs-lookup"><span data-stu-id="b0e5d-279">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="b0e5d-280">"Iş Ortağı Merkezi ile Eşitle": Evet</span><span class="sxs-lookup"><span data-stu-id="b0e5d-280">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="b0e5d-281">"Microsoft nasıl yardım edebilir?": aşağıdaki seçeneklerden seçim yapın:</span><span class="sxs-lookup"><span data-stu-id="b0e5d-281">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="b0e5d-282">Ürünler: ürünün çözüm kimlikleri</span><span class="sxs-lookup"><span data-stu-id="b0e5d-282">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="b0e5d-283">**Iş Ortağı Merkezi ile fırsat eşitlemesi** seçeneğini **Evet** olarak ayarladıktan sonra 10 dakika bekleyin, iş ortağı Merkezi hesabınızda oturum açın.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-283">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="b0e5d-284">Başvurularınız Salesforce CRM ile eşitlenecek.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-284">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="b0e5d-285">"Iş Ortağı Merkezi ile Eşitle" seçeneği "Evet" olarak ayarlandığında, fırsatı Salesforce CRM 'de güncelleştirirseniz, değişiklikler Iş Ortağı Merkezi hesabınızla eşitlenir.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-285">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="b0e5d-286">Iş Ortağı Merkezi ile başarıyla eşitlenen fırsatlar, Salesforce CRM 'de ✔ simgesiyle tanımlanır.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-286">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="b0e5d-287">Microsoft Iş Ortağı Merkezi 'nde başvuru oluşturulduğunda veya güncelleştirilirken ve Salesforce CRM ortamında eşitlendiğinde başvuru eşitlemesi:</span><span class="sxs-lookup"><span data-stu-id="b0e5d-287">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="b0e5d-288">Iş Ortağı Merkezi [panonuzda](https://partner.microsoft.com/dashboard/home)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-288">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="b0e5d-289">Sol taraftaki menüden **referanslar** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-289">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="b0e5d-290">"Yeni anlaşma" seçeneğine tıklayarak Iş Ortağı Merkezi 'nden yeni bir ortak satış başvurusu oluşturun.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-290">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="b0e5d-291">Salesforce CRM ortamınızda oturum açın.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-291">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="b0e5d-292">**Açık fırsatlara** gidin.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-292">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="b0e5d-293">Microsoft Iş Ortağı Merkezi 'nde oluşturulan başvuru artık Salesforce CRM 'de eşitlendi.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-293">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce fırsat ekranı.":::

    6. <span data-ttu-id="b0e5d-295">Eşitlenmiş bir başvuruyu seçtiğinizde, kart Görünümü ayrıntıları doldurulur.</span><span class="sxs-lookup"><span data-stu-id="b0e5d-295">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b0e5d-296">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="b0e5d-296">Next steps</span></span>

- [<span data-ttu-id="b0e5d-297">Müşteri adaylarını yönetme</span><span class="sxs-lookup"><span data-stu-id="b0e5d-297">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="b0e5d-298">Ortak satış fırsatlarını yönetme</span><span class="sxs-lookup"><span data-stu-id="b0e5d-298">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="b0e5d-299">İş Ortağı Merkezi web kancaları</span><span class="sxs-lookup"><span data-stu-id="b0e5d-299">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
