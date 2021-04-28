---
title: Iş Ortağı Merkezi 'nde MPN hesabı oluşturma
ms.topic: article
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Microsoft İş Ortağı Ağı üyelerin ağ avantajlarını ve uzmanlarını yönetmek için bir Iş Ortağı Merkezi hesabı nasıl oluşturabileceğinizi öğrenin.
author: ParthP
ms.author: ParthP
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 27cd00b5475914019963fad381b36b47a017dcf1
ms.sourcegitcommit: 078eac1456f68585ff1003b21e5e1fe777af314b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/28/2021
ms.locfileid: "108120809"
---
# <a name="create-an-mpn-account-in-partner-center-to-manage-network-benefits-and-competencies"></a><span data-ttu-id="29a9e-103">Ağ avantajlarını ve Uzmanlıklar yönetmek için Iş Ortağı Merkezi 'nde bir MPN hesabı oluşturun</span><span class="sxs-lookup"><span data-stu-id="29a9e-103">Create an MPN account in Partner Center to manage network benefits and competencies</span></span>

<span data-ttu-id="29a9e-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="29a9e-104">**Appropriate roles**</span></span>

- <span data-ttu-id="29a9e-105">MPN iş ortağı Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="29a9e-105">MPN partner admin</span></span>

<span data-ttu-id="29a9e-106">Microsoft İş Ortağı Ağı (MPN) ile yeni başladıysanız ve MPN KIMLIĞI yoksa kayıt [yönergelerini](https://partner.microsoft.com/dashboard/account/v3/enrollment/introduction/partnership)izleyerek kaydınız başlatabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="29a9e-106">If you are new to Microsoft Partner Network (MPN) and don’t have an MPN ID, you can start your enrollment by following the [enrollment instructions](https://partner.microsoft.com/dashboard/account/v3/enrollment/introduction/partnership).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29a9e-107">Önkoşullar</span><span class="sxs-lookup"><span data-stu-id="29a9e-107">Prerequisites</span></span> 

<span data-ttu-id="29a9e-108">Iş Ortağı Merkezi 'nde bir hesap oluşturmaya hazır olduğunuzda, aşağıdaki öğelerin elinizin altında olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="29a9e-108">When you are ready to create an account on Partner Center, you will need to have the following items on hand.</span></span>  <span data-ttu-id="29a9e-109">Başlamadan önce bu öğelerin toplanması birkaç dakika geçmesi gerekebilir:</span><span class="sxs-lookup"><span data-stu-id="29a9e-109">You may want to take a few minutes to gather these items before you get started:</span></span>

- <span data-ttu-id="29a9e-110">Şirket iş e-postası veya Office 365 iş hesabı.</span><span class="sxs-lookup"><span data-stu-id="29a9e-110">Company work email OR Office 365 work account.</span></span> <span data-ttu-id="29a9e-111">Çalışanlarınız için iş e-posta adresleri ayarlamanıza olanak sağlamak için şirketiniz bir e-posta etki alanı satın almanız gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="29a9e-111">Your company may need to purchase an email domain in order for you to set up work email addresses for your employees.</span></span> <span data-ttu-id="29a9e-112">Daha fazla bilgi için [şirketinizin iş hesabınızı ve Iş ortağı merkezini](azure-active-directory-tenants-and-partner-center.md)okuyun.</span><span class="sxs-lookup"><span data-stu-id="29a9e-112">For more information, read [Your company work account and Partner Center](azure-active-directory-tenants-and-partner-center.md).</span></span> 
 
- <span data-ttu-id="29a9e-113">Şirketinizin yasal iş adı ve adresi.</span><span class="sxs-lookup"><span data-stu-id="29a9e-113">Your company's legal business name and address.</span></span>

- <span data-ttu-id="29a9e-114">Yasal sözleşmeleri imzalama yetkisi.</span><span class="sxs-lookup"><span data-stu-id="29a9e-114">Authority to sign legal agreements.</span></span> <span data-ttu-id="29a9e-115">Kayıt işlemi sırasında yapmanız istenecek şekilde, şirketinizin adına yasal sözleşmeleri imzalama yetkiniz olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="29a9e-115">Ensure that you are authorized to sign legal agreements on your company's behalf as you'll be asked to do so during the enrollment process.</span></span>

- <span data-ttu-id="29a9e-116">Birincil kişiniz olarak davranmak istediğiniz kişinin adı ve şirket e-postası.</span><span class="sxs-lookup"><span data-stu-id="29a9e-116">Name and company email of the person you want to act as your primary contact.</span></span> <span data-ttu-id="29a9e-117">Şirketinizin güvenliğinin ve gizliliğinin sağlanmasına yardımcı olmak üzere, e-posta adresini doğrulamak ve e-posta adresinin şirketinize ait olduğundan emin olmak için birincil kişinizi e-posta ile göndereceğiz.</span><span class="sxs-lookup"><span data-stu-id="29a9e-117">To help ensure your company's security and privacy, we email your primary contact to verify the email address and to ensure that the email address belongs to your company.</span></span> <span data-ttu-id="29a9e-118">Birincil iletişim e-posta adresini doğruladıktan sonra, belirtilen bilgileri gözden geçirmemiz için devam edeceğiz.</span><span class="sxs-lookup"><span data-stu-id="29a9e-118">After the primary contact verifies the email address, we'll continue our review of the information provided.</span></span> <span data-ttu-id="29a9e-119">Doğrulama genellikle 3-5 iş günü sürer.</span><span class="sxs-lookup"><span data-stu-id="29a9e-119">Verification usually takes 3-5 business days.</span></span> 

- <span data-ttu-id="29a9e-120">Doğrulama işlemi hakkında bilgi için bkz. [Hesap doğrulama](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="29a9e-120">For information on the verification process, see [Account verification](verification-responses.md).</span></span>

>[!NOTE]
><span data-ttu-id="29a9e-121">Microsoft İş Ortağı Ağı üyeliğiniz hala Iş ortağı üyelik merkeziyse (PMC), hesabınızı hemen Iş Ortağı Merkezi 'ne geçirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="29a9e-121">If your Microsoft Partner Network membership is still in Partner Membership Center (PMC), you need to migrate your account immediately to Partner Center.</span></span> <span data-ttu-id="29a9e-122">[Geçiş için adım adım Kılavuzu](https://assetsprod.microsoft.com/mpn/migrate-pmc-pc-mpa-guide.pptx)indirin.</span><span class="sxs-lookup"><span data-stu-id="29a9e-122">Download the [step-by-step guide to migrate](https://assetsprod.microsoft.com/mpn/migrate-pmc-pc-mpa-guide.pptx).</span></span>

## <a name="get-started"></a><span data-ttu-id="29a9e-123">başlarken</span><span class="sxs-lookup"><span data-stu-id="29a9e-123">Get started</span></span>

1. <span data-ttu-id="29a9e-124">[**Başlarken**](https://partner.microsoft.com/dashboard/account/v3/enrollment/introduction/partnership) sayfasında şirketiniz tarafından size verilen iş e-postalarınızı (örneğin,) başlatın you@yourcompanyname.com .</span><span class="sxs-lookup"><span data-stu-id="29a9e-124">At the [**Get started**](https://partner.microsoft.com/dashboard/account/v3/enrollment/introduction/partnership) page, start with your work email given to you by your company, for example, you@yourcompanyname.com.</span></span>

 
    <span data-ttu-id="29a9e-125">a.</span><span class="sxs-lookup"><span data-stu-id="29a9e-125">a.</span></span>  <span data-ttu-id="29a9e-126">Bu e-postaya devam etmek için bir doğrulama kodu gönderebilmemiz için e-posta adresinin geçerli ve erişilebilir olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="29a9e-126">The email address must be valid and accessible to you because we will send a verification code to that email to continue.</span></span>

    <span data-ttu-id="29a9e-127">b.</span><span class="sxs-lookup"><span data-stu-id="29a9e-127">b.</span></span>  <span data-ttu-id="29a9e-128">E-posta adresi "bilgi", "Yönetici" gibi sözcükleri içermemelidir email@ .</span><span class="sxs-lookup"><span data-stu-id="29a9e-128">The email address should not contain words like "info," "admin," "email@."</span></span> <span data-ttu-id="29a9e-129">Veya " marketing@.. ."; Bu adres biçimleri desteklenmez.</span><span class="sxs-lookup"><span data-stu-id="29a9e-129">Or "marketing@..."; these address formats are not supported.</span></span>

    <span data-ttu-id="29a9e-130">c.</span><span class="sxs-lookup"><span data-stu-id="29a9e-130">c.</span></span>  <span data-ttu-id="29a9e-131">HARITALAR satın almak veya Uzmanlıklar yönetmek için, [etki alanınızı doğrulayarak](become-global-admin.md) ve yönetici haline getirerek bu hesabı yükseltmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="29a9e-131">To purchase MAPS or manage competencies, you will have to upgrade this account by [verifying your domain](become-global-admin.md) and becoming an admin.</span></span> 

2. <span data-ttu-id="29a9e-132">Office 365 iş hesabınızla oturum açabilirsiniz, örneğin, you@contoso.onmicrosoft.com .</span><span class="sxs-lookup"><span data-stu-id="29a9e-132">You can sign in with your Office 365 work account, for example, you@contoso.onmicrosoft.com.</span></span>

   >[!NOTE]
   > <span data-ttu-id="29a9e-133">MPN 'ye kaydolmak için mevcut CSP hesabı kimlik bilgilerinizi kullanamazsınız.</span><span class="sxs-lookup"><span data-stu-id="29a9e-133">You can’t use your existing CSP account credentials to enroll into MPN.</span></span>

3. <span data-ttu-id="29a9e-134">Şirketinizin yasal iş ayrıntılarını sağlayın.</span><span class="sxs-lookup"><span data-stu-id="29a9e-134">Provide your company's legal business details.</span></span>

<span data-ttu-id="29a9e-135">Şirket Profilinizi arayabilir veya şirket bilgilerini el ile girebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="29a9e-135">You can either look up your company profile or enter company information manually.</span></span> <span data-ttu-id="29a9e-136">Şirketiniz [Dun & Bradstreet](https://partner.microsoft.com/marketing/usisvshowcase/dunandbrad)ile kayıtlıysa, şirketinizin bilgilerini aramak için DLııD kimliğini kullanın.</span><span class="sxs-lookup"><span data-stu-id="29a9e-136">If your company is registered with [Dun & Bradstreet](https://partner.microsoft.com/marketing/usisvshowcase/dunandbrad), use the DUNS ID to look up your company info.</span></span> <span data-ttu-id="29a9e-137">Şirket ayrıntılarınızı kendiniz sağlamak istiyorsanız, **el ile**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="29a9e-137">If you want to provide your company details yourself, select **Manual**.</span></span>

<span data-ttu-id="29a9e-138">Şirketiniz **Ermenistan**, **Macaristan**, **Kırgızistan**, **Moldova**, **Özbekistan** veya **Rusya**'da bulunuyorsa ve adresinizi el ile girerseniz adresinizi sizin için doğrulayacağız.</span><span class="sxs-lookup"><span data-stu-id="29a9e-138">If your company is located in **Armenia**, **Hungary**, **Kyrgyzstan**, **Moldova**, **Uzbekistan**, or **Russia**, and you enter your address manually, we will validate your address for you.</span></span> <span data-ttu-id="29a9e-139">Girdiğiniz bir tane doğrulandıktan farklıysa, doğrulanan adresi kullanmanızı öneririz.</span><span class="sxs-lookup"><span data-stu-id="29a9e-139">If the one you enter differs from the validated one, we suggest you use the validated address.</span></span> <span data-ttu-id="29a9e-140">Bu, adresin öğelerinin, ülkenin posta yetkilisi tarafından tanımlanan, doğru şekilde biçimlendirilen ve sevkedilebilir şekilde standartlaştırılmış olmasını sağlar.</span><span class="sxs-lookup"><span data-stu-id="29a9e-140">This ensures that the elements of the address are standardized as defined by the country's postal authority, correctly formatted, and shippable.</span></span>  

<span data-ttu-id="29a9e-141">Şirket bilgilerini girdikten sonra, birincil iletişim bilgilerini girin.</span><span class="sxs-lookup"><span data-stu-id="29a9e-141">Once you have provided the company info, enter the primary contact information.</span></span> <span data-ttu-id="29a9e-142">Birincil iletişim, şirketinizde sizinle iletişim kurabildiğimiz kişi olmalıdır (Bu kişi sizin veya şirketinizdeki başka bir kişi olabilir).</span><span class="sxs-lookup"><span data-stu-id="29a9e-142">The primary contact should be the person in your company we can contact about your application (this contact can be you or another person in your company).</span></span>

4. <span data-ttu-id="29a9e-143">**Şimdi kaydet**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="29a9e-143">Select **Enroll now**.</span></span>

>[!IMPORTANT]
><span data-ttu-id="29a9e-144">Şirketinizin güvenliğinin ve gizliliğinin sağlanmasına yardımcı olmak üzere, e-posta adresini doğrulamak ve e-posta adresinin şirketinize ait olduğundan emin olmak için birincil kişinizi e-posta ile göndereceğiz.</span><span class="sxs-lookup"><span data-stu-id="29a9e-144">To help ensure your company's security and privacy, we email your primary contact to verify the email address and ensure that the email address belongs to your company.</span></span> <span data-ttu-id="29a9e-145">Birincil iletişim e-posta adresini doğruladıktan sonra, verdiğiniz bilgileri gözden geçirmemiz için devam edeceğiz.</span><span class="sxs-lookup"><span data-stu-id="29a9e-145">After the primary contact verifies the email address, we'll continue our review of the information you provided.</span></span> <span data-ttu-id="29a9e-146">Doğrulama genellikle 3-5 iş günü sürer.</span><span class="sxs-lookup"><span data-stu-id="29a9e-146">Verification usually takes 3-5 business days.</span></span> 

## <a name="how-to-view-account-details-or-view-and-download-the-mpn-agreement"></a><span data-ttu-id="29a9e-147">Hesap ayrıntılarını görüntüleme veya MPN sözleşmesini görüntüleme ve indirme</span><span class="sxs-lookup"><span data-stu-id="29a9e-147">How to view account details or view and download the MPN agreement</span></span>

<span data-ttu-id="29a9e-148">MPN kimlik bilgilerinizle Iş Ortağı Merkezi 'Nde oturum açın.</span><span class="sxs-lookup"><span data-stu-id="29a9e-148">Sign into Partner Center with your MPN credentials.</span></span> <span data-ttu-id="29a9e-149">Şirketinizin yasal ayrıntılarını, doğrulama durumunuzu, MPN kimliklerinizi görüntülemek ve gerekirse yeni MPN konumları oluşturmak için [**Iş ortağı profili**](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) ' ni seçin.</span><span class="sxs-lookup"><span data-stu-id="29a9e-149">Select [**Partner profile**](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) to view your company’s legal details, your verification status, your MPN IDs and also create new MPN locations if needed.</span></span> 

<span data-ttu-id="29a9e-150">Ayrıca, MPN kimlikleri gibi diğer önemli bilgileri görüntüleyebilir, MPN konumlarını yönetebilir ve aşağıdaki ekran görüntüsünde gösterildiği gibi sol menü bağlantılarını kullanarak Microsoft Iş ortağı sözleşmesi 'ni görüntüleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="29a9e-150">You can also view other important information like MPN Ids, manage MPN locations, and view Microsoft Partner Agreement using the left menu links as show in the following screenshot.</span></span>

:::image type="content" source="images/mpn-new.png" alt-text="İş ortağı profili":::


## <a name="next-steps"></a><span data-ttu-id="29a9e-152">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="29a9e-152">Next steps</span></span>

-  [<span data-ttu-id="29a9e-153">Hesap kullanıcılarını ekleme ve bunlara izin atama</span><span class="sxs-lookup"><span data-stu-id="29a9e-153">Add account users and assign permissions to them</span></span>](create-user-accounts-and-set-permissions.md)

-  [<span data-ttu-id="29a9e-154">Microsoft Eylem Paketi aboneliği satın alma veya yenileme</span><span class="sxs-lookup"><span data-stu-id="29a9e-154">Purchase or renew a subscription to Microsoft Action Pack</span></span>](mpn-get-action-pack.md)

-  [<span data-ttu-id="29a9e-155">Üyelik avantajlarınızı yönetin</span><span class="sxs-lookup"><span data-stu-id="29a9e-155">Manage your membership benefits</span></span>](manage-your-partner-network-benefits.md)

-  [<span data-ttu-id="29a9e-156">Altın ve gümüş üyelik için uzmanlığa yönelik gereksinimler hakkında bilgi edinin</span><span class="sxs-lookup"><span data-stu-id="29a9e-156">Learn about competency requirements for Gold and Silver membership</span></span>](https://partner.microsoft.com/membership/competencies)

-  [<span data-ttu-id="29a9e-157">Microsoft’tan müşteri adaylarını almak için iş profili oluşturma</span><span class="sxs-lookup"><span data-stu-id="29a9e-157">Create a business profile to get sales leads from Microsoft</span></span>](create-a-marketing-profile.md)

-  [<span data-ttu-id="29a9e-158">Microsoft 'tan satış fırsatlarını alın ve yönetin</span><span class="sxs-lookup"><span data-stu-id="29a9e-158">Get and manage sales leads from Microsoft</span></span>](manage-leads.md)
