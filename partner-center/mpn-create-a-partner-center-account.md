---
title: İş Ortağı Merkezi hesabı oluşturma
ms.topic: article
ms.date: 02/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Microsoft İş Ortağı Ağı üyelerin ağ avantajlarını ve uzmanlarını yönetmek için bir Iş Ortağı Merkezi hesabı nasıl oluşturabileceğinizi öğrenin.
author: ParthP
ms.author: ParthP
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 129cdd337f9b475b37d14c4e68058736b473fe33
ms.sourcegitcommit: 5768f10cd122a20fe3df3062ea34e7096d99f639
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/09/2021
ms.locfileid: "100005947"
---
# <a name="create-a-partner-center-account-to-manage-network-benefits-and-competencies"></a><span data-ttu-id="3d438-103">Ağ avantajlarını ve uzmanlık alanı yönetimini yönetmek için bir Iş Ortağı Merkezi hesabı oluşturun</span><span class="sxs-lookup"><span data-stu-id="3d438-103">Create a Partner Center account to manage network benefits and competencies</span></span>


<span data-ttu-id="3d438-104">Microsoft İş Ortağı Ağı yeni başladıysanız ve MPN KIMLIĞI yoksa kayıt [yönergelerini](https://partner.microsoft.com/dashboard/account/v3/enrollment/introduction/partnership)izleyerek kaydınız başlatabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="3d438-104">If you are new to Microsoft Partner Network and don’t have an MPN ID, you can start your enrollment by following the [enrollment instructions](https://partner.microsoft.com/dashboard/account/v3/enrollment/introduction/partnership).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d438-105">Önkoşullar</span><span class="sxs-lookup"><span data-stu-id="3d438-105">Prerequisites</span></span> 

<span data-ttu-id="3d438-106">Iş Ortağı Merkezi 'nde bir hesap oluşturmaya hazır olduğunuzda, kullanmaya başlamak için aşağıdaki öğelerin elinizin altında olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="3d438-106">When you are ready to create an account on Partner Center, to get started you will need to have the following items on hand.</span></span>  <span data-ttu-id="3d438-107">Başlamadan önce bu öğelerin toplanması birkaç dakika geçmesi gerekebilir:</span><span class="sxs-lookup"><span data-stu-id="3d438-107">You may want to take a few minutes to gather these items before you get started:</span></span>

- <span data-ttu-id="3d438-108">Şirket iş e-postası veya Office 365 iş hesabı.</span><span class="sxs-lookup"><span data-stu-id="3d438-108">Company work email OR Office 365 work account.</span></span> <span data-ttu-id="3d438-109">Daha fazla bilgi edinmek için [şirketinizin iş hesabınızı ve Iş ortağı merkezini](azure-active-directory-tenants-and-partner-center.md) okuyun</span><span class="sxs-lookup"><span data-stu-id="3d438-109">Fore more information, read [Your company work account and Partner Center](azure-active-directory-tenants-and-partner-center.md)</span></span> 
 
- <span data-ttu-id="3d438-110">Şirketinizin yasal iş adı ve adresi.</span><span class="sxs-lookup"><span data-stu-id="3d438-110">Your company's legal business name and address.</span></span>

- <span data-ttu-id="3d438-111">Yasal sözleşmeleri imzalama yetkisi.</span><span class="sxs-lookup"><span data-stu-id="3d438-111">Authority to sign legal agreements.</span></span> <span data-ttu-id="3d438-112">Kayıt işlemi sırasında yapmanız istenecek şekilde, şirketinizin adına yasal sözleşmeleri imzalama yetkiniz olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="3d438-112">Ensure that you are authorized to sign legal agreements on your company's behalf as you'll be asked to do so during the enrollment process.</span></span>

- <span data-ttu-id="3d438-113">Birincil kişiniz olarak davranmak istediğiniz kişinin adı ve şirket e-postası.</span><span class="sxs-lookup"><span data-stu-id="3d438-113">Name and company email of the person you want to act as your primary contact.</span></span> <span data-ttu-id="3d438-114">Şirketinizin güvenliğinin ve gizliliğinin sağlanmasına yardımcı olmak üzere, e-posta adresini doğrulamak ve e-posta adresinin şirketinize ait olduğundan emin olmak için birincil kişinizi e-posta ile göndereceğiz.</span><span class="sxs-lookup"><span data-stu-id="3d438-114">To help ensure your company's security and privacy, we email your primary contact to verify the email address and to ensure that the email address belongs to your company.</span></span> <span data-ttu-id="3d438-115">Birincil iletişim e-posta adresini doğruladıktan sonra, belirtilen bilgileri gözden geçirmemiz için devam edeceğiz.</span><span class="sxs-lookup"><span data-stu-id="3d438-115">After the primary contact verifies the email address, we'll continue our review of the information provided.</span></span> <span data-ttu-id="3d438-116">Doğrulama genellikle 3-5 iş günü sürer.</span><span class="sxs-lookup"><span data-stu-id="3d438-116">Verification usually takes 3-5 business days.</span></span> 

- <span data-ttu-id="3d438-117">Doğrulama işlemi hakkında bilgi için bkz. [Hesap doğrulama](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="3d438-117">For information on the verification process, see [Account verification](verification-responses.md).</span></span>

>[!NOTE]
><span data-ttu-id="3d438-118">Microsoft İş Ortağı Ağı üyeliğiniz hala Iş ortağı üyelik merkeziyse (PMC), hesabınızı hemen Iş Ortağı Merkezi 'ne geçirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="3d438-118">If your Microsoft Partner Network membership is still in Partner Membership Center (PMC), you need to migrate your account immediately to Partner Center.</span></span> <span data-ttu-id="3d438-119">[Geçiş için adım adım Kılavuzu](https://assetsprod.microsoft.com/mpn/migrate-pmc-pc-mpa-guide.pptx)indirin.</span><span class="sxs-lookup"><span data-stu-id="3d438-119">Download the [step-by-step guide to migrate](https://assetsprod.microsoft.com/mpn/migrate-pmc-pc-mpa-guide.pptx).</span></span>

## <a name="get-started"></a><span data-ttu-id="3d438-120">başlarken</span><span class="sxs-lookup"><span data-stu-id="3d438-120">Get started</span></span>

1. <span data-ttu-id="3d438-121">Şirketiniz tarafından verilen iş e-postalarınız ile başlayın you@yourcompanyname.com .</span><span class="sxs-lookup"><span data-stu-id="3d438-121">Start with your work email given by your company like you@yourcompanyname.com.</span></span>
 
    <span data-ttu-id="3d438-122">a.</span><span class="sxs-lookup"><span data-stu-id="3d438-122">a.</span></span>  <span data-ttu-id="3d438-123">Devam etmek için bir doğrulama kodu gönderebilmemiz için e-posta adresinin geçerli ve erişilebilir olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="3d438-123">The email address must be valid and accessible to you as we will send a verification code to continue.</span></span>

    <span data-ttu-id="3d438-124">b.</span><span class="sxs-lookup"><span data-stu-id="3d438-124">b.</span></span>  <span data-ttu-id="3d438-125">E-posta adresi "bilgi", "Yönetici" gibi sözcükleri içermemelidir email@. . Ya da " marketing@.. ." desteklenmez.</span><span class="sxs-lookup"><span data-stu-id="3d438-125">Email address should not contain words like "info," "admin," "email@.." Or "marketing@..." as these are not supported.</span></span>

    <span data-ttu-id="3d438-126">c.</span><span class="sxs-lookup"><span data-stu-id="3d438-126">c.</span></span>  <span data-ttu-id="3d438-127">HARITALAR satın almak veya Uzmanlıklar yönetmek için, etki alanınızı doğrulayarak ve yönetici haline getirerek bu hesabı yükseltmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="3d438-127">To purchase MAPS or manage competencies, you will have to upgrade this account by verifying your domain and becoming admin.</span></span> 

2. <span data-ttu-id="3d438-128">Office 365 iş hesabınızla oturum açabilirsiniz, örneğin, you@contoso.onmicrosoft.com .</span><span class="sxs-lookup"><span data-stu-id="3d438-128">You can sign in with your Office 365 work account, for example, you@contoso.onmicrosoft.com.</span></span>

   >[!NOTE]
   > <span data-ttu-id="3d438-129">MPN 'ye kaydolmak için mevcut CSP hesabı kimlik bilgilerinizi kullanamazsınız.</span><span class="sxs-lookup"><span data-stu-id="3d438-129">You can’t use your existing CSP account credentials to enroll into MPN.</span></span>

3. <span data-ttu-id="3d438-130">Şirketinizin yasal iş ayrıntılarını sağlayın.</span><span class="sxs-lookup"><span data-stu-id="3d438-130">Provide your company's legal business details.</span></span>

<span data-ttu-id="3d438-131">Şirket Profilinizi arayabilir veya şirket bilgilerini el ile girebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="3d438-131">You can either look up your company profile or enter company information manually.</span></span> <span data-ttu-id="3d438-132">Şirketiniz [Dun & Bradstreet](https://partner.microsoft.com/marketing/usisvshowcase/dunandbrad)ile kayıtlıysa, şirketinizin bilgilerini aramak için Dlııd kimliğini kullanın.</span><span class="sxs-lookup"><span data-stu-id="3d438-132">If your company is registered with [Dun & Bradstreet](https://partner.microsoft.com/marketing/usisvshowcase/dunandbrad), use the DUNS Id to look up your company info.</span></span> <span data-ttu-id="3d438-133">Şirket ayrıntılarınızı kendiniz sağlamak istiyorsanız, **el ile**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="3d438-133">If you want to provide your company details yourself, select **Manual**.</span></span>

<span data-ttu-id="3d438-134">Şirket bilgilerini girdikten sonra, birincil iletişim bilgilerini girin ve **Şimdi kaydet**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="3d438-134">Once you have provided the company info, enter the primary contact information, and then select **Enroll now**.</span></span>
<span data-ttu-id="3d438-135">Birincil ilgili kişi, şirketinizde sizinle iletişim kurabildiğimiz kişi olmalıdır (Bu sizin veya şirketinizdeki başka bir kişi olabilir).</span><span class="sxs-lookup"><span data-stu-id="3d438-135">The primary contact should be the person in your company we can contact about your application (this can be you or another person in your company).</span></span>

>[!IMPORTANT]
><span data-ttu-id="3d438-136">Şirketinizin güvenliğinin ve gizliliğinin sağlanmasına yardımcı olmak üzere, e-posta adresini doğrulamak ve e-posta adresinin şirketinize ait olduğundan emin olmak için, birincil iletişim e-posta adresini doğruladıktan sonra, verdiğiniz bilgileri gözden geçirmemiz için devam edeceğiz.</span><span class="sxs-lookup"><span data-stu-id="3d438-136">To help ensure your company's security and privacy, we email your primary contact to verify the email address and ensure that the email address belongs to your company, After the primary contact verifies the email address, we'll continue our review of the information you provided.</span></span> <span data-ttu-id="3d438-137">Doğrulama genellikle 3-5 iş günü sürer.</span><span class="sxs-lookup"><span data-stu-id="3d438-137">Verification usually takes 3-5 business days.</span></span> 

## <a name="how-to-view-account-details-or-view-and-download-the-mpn-agreement"></a><span data-ttu-id="3d438-138">Hesap ayrıntılarını görüntüleme veya MPN sözleşmesini görüntüleme ve indirme</span><span class="sxs-lookup"><span data-stu-id="3d438-138">How to view account details or view and download the MPN agreement</span></span>

<span data-ttu-id="3d438-139">MPN kimlik bilgilerinizle Iş Ortağı Merkezi 'Nde oturum açın.</span><span class="sxs-lookup"><span data-stu-id="3d438-139">Sign into Partner Center with your MPN credentials.</span></span> <span data-ttu-id="3d438-140">Şirketinizin yasal ayrıntılarını, doğrulama durumunuzu, MPN kimliklerinizi görüntülemek ve gerekirse yeni MPN konumları oluşturmak için [**Iş ortağı profili**](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) ' ni seçin.</span><span class="sxs-lookup"><span data-stu-id="3d438-140">Select [**Partner profile**](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) to view your company’s legal details, your verification status, your MPN IDs and also create new MPN locations if needed.</span></span> 

<span data-ttu-id="3d438-141">Ayrıca, MPN kimlikleri gibi diğer önemli bilgileri görüntüleyebilir, MPN konumlarını yönetebilir ve aşağıdaki ekran görüntüsünde gösterildiği gibi sol menü bağlantılarını kullanarak Microsoft Iş ortağı sözleşmesi 'ni görüntüleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="3d438-141">You can also view other important information like MPN Ids, manage MPN locations, and view Microsoft Partner Agreement using the left menu links as show in the following screenshot.</span></span>

:::image type="content" source="images/mpn-new.png" alt-text="İş ortağı profili":::


## <a name="next-steps"></a><span data-ttu-id="3d438-143">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="3d438-143">Next steps</span></span>

-   [<span data-ttu-id="3d438-144">Hesap kullanıcılarını ekleme ve bunlara izin atama</span><span class="sxs-lookup"><span data-stu-id="3d438-144">Add account users and assign permissions to them</span></span>](create-user-accounts-and-set-permissions.md)

-   [<span data-ttu-id="3d438-145">Microsoft Eylem Paketi aboneliği satın alma veya yenileme</span><span class="sxs-lookup"><span data-stu-id="3d438-145">Purchase or renew a subscription to Microsoft Action Pack</span></span>](mpn-get-action-pack.md)

-   [<span data-ttu-id="3d438-146">Üyelik avantajlarınızı yönetin</span><span class="sxs-lookup"><span data-stu-id="3d438-146">Manage your membership benefits</span></span>](manage-your-partner-network-benefits.md)

-   [<span data-ttu-id="3d438-147">Altın ve gümüş üyelik için uzmanlığa yönelik gereksinimler hakkında bilgi edinin</span><span class="sxs-lookup"><span data-stu-id="3d438-147">Learn about competency requirements for Gold and Silver membership</span></span>](https://partner.microsoft.com/membership/competencies)

-   [<span data-ttu-id="3d438-148">Microsoft’tan müşteri adaylarını almak için iş profili oluşturma</span><span class="sxs-lookup"><span data-stu-id="3d438-148">Create a business profile to get sales leads from Microsoft</span></span>](create-a-marketing-profile.md)

-   [<span data-ttu-id="3d438-149">Microsoft 'tan satış fırsatlarını alın ve yönetin</span><span class="sxs-lookup"><span data-stu-id="3d438-149">Get and manage sales leads from Microsoft</span></span>](manage-leads.md)
