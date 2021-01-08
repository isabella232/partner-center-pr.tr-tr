---
title: İş Ortağı Merkezi hesabı oluşturma
ms.topic: article
ms.date: 01/07/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Microsoft İş Ortağı Ağı üyelerin ağ avantajlarını ve uzmanlarını yönetmek için bir Iş Ortağı Merkezi hesabı nasıl oluşturabileceğinizi öğrenin.
author: ParthP
ms.author: ParthP
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c7aa97760be9fdb2cc004ffd5612826f777c05c5
ms.sourcegitcommit: a78dd3c532860d01867d116bfb4e2c88b84bcd25
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/08/2021
ms.locfileid: "97979745"
---
# <a name="create-a-partner-center-account-to-manage-network-benefits-and-competencies"></a><span data-ttu-id="52563-103">Ağ avantajlarını ve uzmanlık alanı yönetimini yönetmek için bir Iş Ortağı Merkezi hesabı oluşturun</span><span class="sxs-lookup"><span data-stu-id="52563-103">Create a Partner Center account to manage network benefits and competencies</span></span>

<span data-ttu-id="52563-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="52563-104">**Appropriate roles**</span></span>

- <span data-ttu-id="52563-105">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="52563-105">Global admin</span></span>
- <span data-ttu-id="52563-106">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="52563-106">Admin agent</span></span>

<span data-ttu-id="52563-107">Iş Ortağı Merkezi 'nde bir hesap oluşturabilmeniz için şirketinizin Microsoft İş Ortağı Ağı bir üyesi olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="52563-107">Before you can create an account on Partner Center, your company must be a member of the Microsoft Partner Network.</span></span> <span data-ttu-id="52563-108">Zaten ağın bir üyesi değilseniz, [Şimdi katılabilir](https://partner.microsoft.com/commercial#).</span><span class="sxs-lookup"><span data-stu-id="52563-108">If you're not already a member of the network, you can [join now](https://partner.microsoft.com/commercial#).</span></span> <span data-ttu-id="52563-109">Bir Iş Ortağı Merkezi hesabı oluşturduktan sonra, [panonuzu öğrenin](https://vimeo.com/290338211)ve bu kısa videoyu izleyin.</span><span class="sxs-lookup"><span data-stu-id="52563-109">After you create a Partner Center account, watch this short video [Discover your dashboard](https://vimeo.com/290338211).</span></span>

## <a name="get-a-work-email-address-before-setting-up-a-partner-center-account"></a><span data-ttu-id="52563-110">İş Ortağı Merkezi hesabı ayarlamadan önce bir iş e-posta adresi alın</span><span class="sxs-lookup"><span data-stu-id="52563-110">Get a work email address before setting up a Partner Center account</span></span>

<span data-ttu-id="52563-111">Çalışanlarınız için iş e-posta adreslerini ayarlayabilmeniz için şirketiniz bir e-posta etki alanı satın almanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="52563-111">Your company needs to purchase an email domain in order for you to be able to set up work email addresses for your employees.</span></span> <span data-ttu-id="52563-112">Bu teknik bir işlem olduğundan, bir e-posta etki alanı satın almak için BT departmanınızla birlikte çalışın.</span><span class="sxs-lookup"><span data-stu-id="52563-112">Work with your IT department to buy an email domain since this is a technical process.</span></span> <span data-ttu-id="52563-113">Yeni e-postayı kullanarak Azure AD kiracınızı ve Iş Ortağı Merkezi hesabınızı ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="52563-113">Use the new email to set up your Azure AD tenant and your Partner Center account.</span></span>

## <a name="get-started"></a><span data-ttu-id="52563-114">başlarken</span><span class="sxs-lookup"><span data-stu-id="52563-114">Get started</span></span>

<span data-ttu-id="52563-115">Iş Ortağı Merkezi 'nde bir hesap oluşturmak için aşağıdaki bilgileri kullanmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="52563-115">To create an account on Partner Center, you'll need to have on hand the following information.</span></span> <span data-ttu-id="52563-116">Başlamadan önce bu öğelerin toplanması birkaç dakika geçmesi gerekebilir:</span><span class="sxs-lookup"><span data-stu-id="52563-116">You may want to take a few minutes to gather these items before you get started:</span></span>

- <span data-ttu-id="52563-117">Genel yönetici iş e-postası.</span><span class="sxs-lookup"><span data-stu-id="52563-117">Global administrator work email.</span></span>

- <span data-ttu-id="52563-118">Şirketinizin iş hesabının ne olduğundan emin değilseniz şirketinizin iş hesabı [ve Iş ortağı merkezinizde](azure-active-directory-tenants-and-partner-center.md) , şirketinizin iş hesabı yoksa hesap oluşturma işlemi sırasında bir tane oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="52563-118">If you're not sure what your company's work account is, see [Your company work account and Partner Center](azure-active-directory-tenants-and-partner-center.md) If your company doesn't have a work account, you can create one during the account creation process.</span></span> 

- <span data-ttu-id="52563-119">Şirketinizin yasal iş adı ve adresi.</span><span class="sxs-lookup"><span data-stu-id="52563-119">Your company's legal business name and address.</span></span>  

- <span data-ttu-id="52563-120">Yasal sözleşmeleri imzalama yetkisi.</span><span class="sxs-lookup"><span data-stu-id="52563-120">Authority to sign legal agreements.</span></span> <span data-ttu-id="52563-121">Kayıt işlemi sırasında yapmanız istenecek şekilde, şirketinizin adına yasal sözleşmeleri imzalama yetkiniz olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="52563-121">Ensure that you are authorized to sign legal agreements on your company's behalf as you'll be asked to do so during the enrollment process.</span></span>

- <span data-ttu-id="52563-122">Birincil kişiniz olarak davranmak istediğiniz kişinin adı ve şirket e-postası.</span><span class="sxs-lookup"><span data-stu-id="52563-122">Name and company email of the person you want to act as your primary contact.</span></span> <span data-ttu-id="52563-123">Şirketinizin güvenliğinin ve gizliliğinin sağlanmasına yardımcı olmak için birincil kişinize e-posta ile bir Iş Ortağı Merkezi hesabına kaydolup (1), bu e-posta adresinin şirketinize ait olduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="52563-123">To help ensure your company's security and privacy, we'll email your primary contact to verify that (1) he or she signed up for a Partner Center account, and that (2) this email address belongs to your company.</span></span> <span data-ttu-id="52563-124">Birincil iletişim e-posta adresini doğruladıktan sonra, verdiğiniz bilgileri gözden geçirmemiz için devam edeceğiz.</span><span class="sxs-lookup"><span data-stu-id="52563-124">After the primary contact verifies his or her email address, we'll continue our review of the information you provided.</span></span>

<span data-ttu-id="52563-125">Bu bilgileri, hesap oluşturma işlemi sırasında doğrulayacağız.</span><span class="sxs-lookup"><span data-stu-id="52563-125">We'll verify this information during the account creation process.</span></span> <span data-ttu-id="52563-126">Doğrulama süreci hakkında bilgi için bkz. [Hesap doğrulama](verification-responses.md)</span><span class="sxs-lookup"><span data-stu-id="52563-126">For information on the verification process, see [Account verification](verification-responses.md)</span></span>
 
## <a name="create-a-partner-center-account"></a><span data-ttu-id="52563-127">İş Ortağı Merkezi hesabı oluşturma</span><span class="sxs-lookup"><span data-stu-id="52563-127">Create a Partner Center account</span></span>

1.  <span data-ttu-id="52563-128">**Hoş geldiniz** sayfasındaki bilgileri gözden geçirin ve ardından **İleri**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="52563-128">Review the information on the **Welcome** page and then select **Next**.</span></span>

2.  <span data-ttu-id="52563-129">Şirketinizin iş hesabına genel yönetici olarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="52563-129">Sign in as a global admin to your company's work account.</span></span> <span data-ttu-id="52563-130">Şirketinizin iş hesabının ne olduğundan emin değilseniz, [şirketinizin iş hesabı ve Iş Ortağı Merkezi](azure-active-directory-tenants-and-partner-center.md)' ne bakın.</span><span class="sxs-lookup"><span data-stu-id="52563-130">If you're not sure what your company's work account   is, see [Your company work account and Partner Center](azure-active-directory-tenants-and-partner-center.md).</span></span>

    <span data-ttu-id="52563-131">Şirketinizin bir iş e-posta hesabı olduğunu biliyorsanız **oturum aç '** ı seçin.</span><span class="sxs-lookup"><span data-stu-id="52563-131">Select **Sign in** if you know your company has a work email account.</span></span> <span data-ttu-id="52563-132">Bir sonraki sayfada, şirketinizin iş hesabı için genel yönetici kimlik bilgilerini girin.</span><span class="sxs-lookup"><span data-stu-id="52563-132">On the next page, enter global admin credentials for your company's work account.</span></span> 

    <span data-ttu-id="52563-133">Şirketiniz bir iş hesabına sahip değilse, şimdi bir tane ayarlamak için **Oluştur** ' u seçin.</span><span class="sxs-lookup"><span data-stu-id="52563-133">If your company doesn't have a work account, select **Create one** to set one up now.</span></span> <span data-ttu-id="52563-134">Bir iş hesabı oluşturduktan sonra, az önce oluşturduğunuz iş hesabı için genel yönetici kimlik bilgilerinizi kullanarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="52563-134">After creating a work account, sign in using your global admin credentials for the work account you just created.</span></span>

3.  <span data-ttu-id="52563-135">Şirketinizin yasal iş profilini sağlayın veya güncelleştirin.</span><span class="sxs-lookup"><span data-stu-id="52563-135">Provide or update your company's legal business profile.</span></span>

    <span data-ttu-id="52563-136">Şirket Profilinizi araması yapabilir veya şirket bilgilerini el ile girebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="52563-136">You can either lookup your company profile or enter company information manually.</span></span> <span data-ttu-id="52563-137">Şirketiniz [Dun & Bradstreet](https://partner.microsoft.com/marketing/usisvshowcase/dunandbrad)ile kayıtlıysa, şirketinizin bilgilerini aramak için Dlııd kimliğini kullanın.</span><span class="sxs-lookup"><span data-stu-id="52563-137">If your company is registered with [Dun & Bradstreet](https://partner.microsoft.com/marketing/usisvshowcase/dunandbrad), use the DUNS Id to look up your company info.</span></span> <span data-ttu-id="52563-138">Şirket ayrıntılarınızı kendiniz sağlamak istiyorsanız, **el ile**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="52563-138">If you want to provide your company details yourself, select **Manual**.</span></span>

4. <span data-ttu-id="52563-139">Şirket bilgilerini girdikten sonra, birincil iletişim bilgilerini girip **Şimdi kaydet**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="52563-139">Once you have provided the company info, enter the primary contact information and then select **Enroll now**.</span></span>

    <span data-ttu-id="52563-140">Birincil ilgili kişi, şirketinizde sizinle iletişim kurabildiğimiz kişi olmalıdır (Bu sizin veya şirketinizdeki başka bir kişi olabilir).</span><span class="sxs-lookup"><span data-stu-id="52563-140">The primary contact should be the person in your company we can contact about your application (this can be you or another person in your company).</span></span> <span data-ttu-id="52563-141">Bu bilgileri ayrıca, bu kişinin şirketinizde çalıştığını ve bir Iş Ortağı Merkezi hesabına kaydolmadığını doğrulamak için de kullanacağız.</span><span class="sxs-lookup"><span data-stu-id="52563-141">We'll also use this information to verify that this person works at your company and has signed up for a Partner Center account.</span></span>

    > [!IMPORTANT]  
    > <span data-ttu-id="52563-142">Şirketinizin güvenliğinin ve gizliliğinin sağlanmasına yardımcı olmak için, birincil kişinize e-posta ile bir Iş Ortağı Merkezi hesabına kaydolup (1), bu e-posta adresinin şirketinize ait olduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="52563-142">To help ensure your company's security and privacy, we'll email your primary contact to verify that (1) he or she signed up for a Partner Center account, and (2) that this email address belongs to your company.</span></span> <span data-ttu-id="52563-143">Birincil iletişim e-posta adresini doğruladıktan sonra, verdiğiniz bilgileri gözden geçirmemiz için devam edeceğiz.</span><span class="sxs-lookup"><span data-stu-id="52563-143">After the primary contact verifies his or her email address, we'll continue our review of the information you provided.</span></span>

5.  <span data-ttu-id="52563-144">Microsoft İş Ortağı Ağı sözleşmesindeki hüküm ve koşulları okuyun ve kabul edin.</span><span class="sxs-lookup"><span data-stu-id="52563-144">Read and accept the terms and conditions in the Microsoft Partner Network agreement.</span></span> 

6.  <span data-ttu-id="52563-145">Yönetim Aracısı grubuna eklendiğinizi doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="52563-145">Verify that you've been added to the admin agent group.</span></span> <span data-ttu-id="52563-146">Diğer kullanıcıları ekleme dahil olmak üzere hesabınızı ayarlamayı tamamlaması için yönetici Aracısı izinlerinizin olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="52563-146">To finish setting up your account, including adding other users, you must have admin agent permissions.</span></span> <span data-ttu-id="52563-147">İzinlerinizi görüntülemek veya güncelleştirmek için şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="52563-147">Follow these steps to view or update your permissions:</span></span>

    <span data-ttu-id="52563-148">a.</span><span class="sxs-lookup"><span data-stu-id="52563-148">a.</span></span> <span data-ttu-id="52563-149">Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard/home**), **Ayarlar** simgesini seçin ve ardından **Kullanıcı yönetimi**' ni seçin.</span><span class="sxs-lookup"><span data-stu-id="52563-149">From the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home**), select the **Settings** icon and then select **User management**.</span></span>  

    <span data-ttu-id="52563-150">b.</span><span class="sxs-lookup"><span data-stu-id="52563-150">b.</span></span> <span data-ttu-id="52563-151">Kullanıcılar listesinden adınızı seçin ve daha önce seçilmemişse **yönetici Aracısı** ' nı seçin.</span><span class="sxs-lookup"><span data-stu-id="52563-151">Select your name from the users list and then select **Admin agent** if it's not already selected.</span></span> <span data-ttu-id="52563-152">**Güncelleştir**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="52563-152">Select **Update**.</span></span>  

## <a name="view-mpn-account-details"></a><span data-ttu-id="52563-153">MPN hesabı ayrıntılarını görüntüle</span><span class="sxs-lookup"><span data-stu-id="52563-153">View MPN account details</span></span>

<span data-ttu-id="52563-154">Bir Iş Ortağı Merkezi hesabı oluşturduktan sonra çeşitli hesap ayrıntılarını görmek için Iş Ortağı Merkezi 'ne dönebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="52563-154">Once you create a Partner Center account, you can return to Partner Center to see various account details.</span></span> <span data-ttu-id="52563-155">Bunların birçoğu Iş Ortağı Merkezi [panonuzdaki](https://partner.microsoft.com/dashboard) **iş ortağı profili** sayfasında görünürler.</span><span class="sxs-lookup"><span data-stu-id="52563-155">Many of these appear on the **Partner profile** page in your Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

<span data-ttu-id="52563-156">Bu tür Ayrıntılar şunları içerir:</span><span class="sxs-lookup"><span data-stu-id="52563-156">Such details include:</span></span>

- <span data-ttu-id="52563-157">Şirketinizin yasal iş profili</span><span class="sxs-lookup"><span data-stu-id="52563-157">Your company's legal business profile</span></span>

- <span data-ttu-id="52563-158">MPN KIMLIĞINIZ hakkında bilgi</span><span class="sxs-lookup"><span data-stu-id="52563-158">Information about your MPN ID</span></span>

- <span data-ttu-id="52563-159">Kayıtlı Microsoft programlarınızla ilişkili geçerli sözleşmelerin bağlantıları</span><span class="sxs-lookup"><span data-stu-id="52563-159">Links to current agreements associated with your enrolled Microsoft program</span></span>

  <span data-ttu-id="52563-160">Örneğin, MPN programına kaydolduysanız geçerli Microsoft İş Ortağı Ağı sözleşmesinin bağlantısını görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="52563-160">For example, if you are enrolled in the MPN program, you'll see a link to the current Microsoft Partner Network agreement.</span></span> <span data-ttu-id="52563-161">Bulut çözümü sağlayıcısı (CSP) programı gibi diğer iş ortağı programlarına kaydolduysanız, Microsoft Iş ortağı sözleşmesi gibi diğer sözleşmelerin bağlantılarını da görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="52563-161">If you're enrolled in other partner programs, like the Cloud Solution Provider (CSP) program, you may also see links to other agreements, such as the Microsoft Partner Agreement.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="52563-162">Bir sözleşmeyi gözden geçirmek, erişmek veya indirmek ya da imzalandığı tarihi denetlemek istediğinizde bu bağlantı türlerini görmek yararlı olabilir.</span><span class="sxs-lookup"><span data-stu-id="52563-162">Seeing these types of links may be useful if you ever want to review, access, or download an agreement, or, check the date it was signed.</span></span>

### <a name="how-to-view-account-details-or-view-and-download-the-mpn-agreement"></a><span data-ttu-id="52563-163">Hesap ayrıntılarını görüntüleme veya MPN sözleşmesini görüntüleme ve indirme</span><span class="sxs-lookup"><span data-stu-id="52563-163">How to view account details or view and download the MPN agreement</span></span>

<span data-ttu-id="52563-164">Hesap ayrıntılarını görüntülemek veya MPN sözleşmesini görüntülemek ve indirmek için şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="52563-164">Follow these steps to view account details or view and download the MPN agreement:</span></span>

1. <span data-ttu-id="52563-165">İş hesabı kullanıcı adınızı ve parolanızı kullanarak iş ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="52563-165">Using your work account username and password, sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="52563-166">Genel Bakış sayfası görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="52563-166">An Overview page appears.</span></span> <span data-ttu-id="52563-167">(Genel bakış sayfasını görmüyorsanız, sol gezinti menüsünden **genel bakış** ' ı seçin.)</span><span class="sxs-lookup"><span data-stu-id="52563-167">(If you do not see the Overview page, select **Overview** from the left-navigation menu.)</span></span>

3. <span data-ttu-id="52563-168">Panonun sağ üst köşesindeki dişli simgesini seçin ve ardından **Iş ortağı ayarları**' nı seçin.</span><span class="sxs-lookup"><span data-stu-id="52563-168">Select the Gear icon in the top-right corner of the dashboard, then select **Partner settings**.</span></span> <span data-ttu-id="52563-169">Bu sizi Iş ortağı profili sayfasına götürür.</span><span class="sxs-lookup"><span data-stu-id="52563-169">This takes you to the Partner profile page.</span></span>

4. <span data-ttu-id="52563-170">Iş ortağı profili sayfasında, farklı alan görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="52563-170">From the Partner profile page, you'll see different areas.</span></span> <span data-ttu-id="52563-171">Bunlar yasal bir **iş profili** alanı ve bir **Program bilgi** alanı içerir.</span><span class="sxs-lookup"><span data-stu-id="52563-171">These include a **Legal business profile** area and a **Program info** area.</span></span>

5. <span data-ttu-id="52563-172">**Program bilgileri** altında **MPN program durumu** alanını bulun.</span><span class="sxs-lookup"><span data-stu-id="52563-172">Under **Program info**, locate the **MPN program status** field.</span></span> <span data-ttu-id="52563-173">Bu, Microsoft İş Ortağı Ağı anlaşmanıza bir bağlantı gösterir.</span><span class="sxs-lookup"><span data-stu-id="52563-173">This displays a link to your Microsoft Partner Network agreement.</span></span> <span data-ttu-id="52563-174">Ayrıca, programda geçerli durumunuzu da açıklar.</span><span class="sxs-lookup"><span data-stu-id="52563-174">It also describes your current status in the program.</span></span>


   :::image type="content" source="images/accountsettings/mpn-program-info-download-mpn-agreement.png" alt-text="Iş ortağı profili sayfasındaki program bilgileri alanını, bu alandaki MPN program durumu alanını, Microsoft İş Ortağı Ağı sözleşmesinin ilişkili bağlantısıyla birlikte vurgulama kutusuyla gösteren resim.":::

6. <span data-ttu-id="52563-176">Bu Sözleşmeyi görüntülemek veya indirmek için **Microsoft iş ortağı ağı sözleşmesi**' ni seçin.</span><span class="sxs-lookup"><span data-stu-id="52563-176">To view or download this agreement, select **Microsoft Partner Network agreement**.</span></span>  

> [!NOTE]
> <span data-ttu-id="52563-177">Ayrıca, bulut çözümü sağlayıcısı (CSP) programına kaydolmanız durumunda Microsoft Iş ortağı sözleşmesi gibi diğer kayıtlı programlar için diğer sözleşmeleri görüntülemek veya indirmek üzere yukarıdaki adımları da kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="52563-177">You can also use the above steps to view or download other agreements for other, enrolled programs, such as the Microsoft Partner Agreement if you happen to be enrolled in the Cloud Solution Provider (CSP) program.</span></span>

## <a name="next-steps"></a><span data-ttu-id="52563-178">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="52563-178">Next steps</span></span>

-   [<span data-ttu-id="52563-179">Hesap kullanıcılarını ekleme ve bunlara izin atama</span><span class="sxs-lookup"><span data-stu-id="52563-179">Add account users and assign permissions to them</span></span>](create-user-accounts-and-set-permissions.md)

-   [<span data-ttu-id="52563-180">Microsoft Eylem Paketi aboneliği satın alma veya yenileme</span><span class="sxs-lookup"><span data-stu-id="52563-180">Purchase or renew a subscription to Microsoft Action Pack</span></span>](mpn-get-action-pack.md)

-   [<span data-ttu-id="52563-181">Üyelik avantajlarınızı yönetin</span><span class="sxs-lookup"><span data-stu-id="52563-181">Manage your membership benefits</span></span>](manage-your-partner-network-benefits.md)

-   [<span data-ttu-id="52563-182">Altın ve gümüş üyelik için uzmanlığa yönelik gereksinimler hakkında bilgi edinin</span><span class="sxs-lookup"><span data-stu-id="52563-182">Learn about competency requirements for Gold and Silver membership</span></span>](https://partner.microsoft.com/membership/competencies)

-   [<span data-ttu-id="52563-183">Microsoft’tan müşteri adaylarını almak için iş profili oluşturma</span><span class="sxs-lookup"><span data-stu-id="52563-183">Create a business profile to get sales leads from Microsoft</span></span>](create-a-marketing-profile.md)

-   [<span data-ttu-id="52563-184">Microsoft 'tan satış fırsatlarını alın ve yönetin</span><span class="sxs-lookup"><span data-stu-id="52563-184">Get and manage sales leads from Microsoft</span></span>](manage-leads.md)
