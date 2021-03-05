---
title: Iş Ortağı Merkezi hesabınıza kiracılar ekleyin
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Iş Ortağı Merkezi hesabınızda birden çok Azure AD kiracılarının nasıl ekleneceğini, birleştireceğinizi veya yönetileceğini öğrenin ve neden yapmak isteyebileceğiniz hakkında bilgi edinin.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124814"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="0d387-103">Iş Ortağı Merkezi hesabınızda birden çok kiracı ekleme ve yönetme</span><span class="sxs-lookup"><span data-stu-id="0d387-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="0d387-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="0d387-104">**Appropriate roles**</span></span>

- <span data-ttu-id="0d387-105">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="0d387-105">Global admin</span></span>
- <span data-ttu-id="0d387-106">Hesap yöneticisi</span><span class="sxs-lookup"><span data-stu-id="0d387-106">Account admin</span></span>

<span data-ttu-id="0d387-107">Bu makalede, şirketiniz için birden çok Azure Active Directory (Azure AD) kiracılarının nasıl birleştirilmesi ve ardından bunları Iş Ortağı Merkezi hesabınıza eklemek ve yönetmek açıklanır.</span><span class="sxs-lookup"><span data-stu-id="0d387-107">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="0d387-108">Bunu yapmanız pek çok neden vardır.</span><span class="sxs-lookup"><span data-stu-id="0d387-108">There are many reasons to do so.</span></span> <span data-ttu-id="0d387-109">Örnek:</span><span class="sxs-lookup"><span data-stu-id="0d387-109">For example:</span></span>

- <span data-ttu-id="0d387-110">Şirketinizin, contoso, başka bir şirket olan Fabrikam almış olduğunu varsayalım.</span><span class="sxs-lookup"><span data-stu-id="0d387-110">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="0d387-111">İki şirketin ayrı kalmasını istiyorsunuz, ancak yeni çalışanların Iş Ortağı Merkezi 'ni kullanmasını istiyorsunuz.</span><span class="sxs-lookup"><span data-stu-id="0d387-111">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="0d387-112">Bu durumda, yeni şirketin Azure AD kiracısını Iş ortağı küresel hesabınızla (PGA) ilişkilendirirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0d387-112">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="0d387-113">Bu ilişki, her iki şirketteki kullanıcıların iş ortağı merkezi 'nde çalışmasına olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="0d387-113">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="0d387-114">İşletmenizi birden fazla kiracı (örneğin, *contoso.com*, *contoso.uk* ve *contoso.in*) ile çalıştırırsanız, bunları aynı bilgisayar hesabında gruplamak için çoklu kiralama kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0d387-114">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="0d387-115">Birleşmeler ve alma yönergeleri her iki şirketteki kiracılar ile çalışmanız gerekiyorsa, hem *constoso.com* hem de *fabrikam.com* kiracılarını kullanırsınız.</span><span class="sxs-lookup"><span data-stu-id="0d387-115">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="0d387-116">Kiracıların herhangi birinin kullanıcılarının şunları yapabilmesi gerekir:</span><span class="sxs-lookup"><span data-stu-id="0d387-116">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="0d387-117">Eğitim, dijital indirmeler veya Microsoft Sertifikalı Profesyonel (MCP) ilişkisi için Iş Ortağı Merkezi 'Ne erişin.</span><span class="sxs-lookup"><span data-stu-id="0d387-117">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="0d387-118">Microsoft İş Ortağı Ağı (MPN) admin veya teşvikleri admin gibi Iş Ortağı Merkezi rolleri atanmalıdır.</span><span class="sxs-lookup"><span data-stu-id="0d387-118">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="0d387-119">Hesabınıza bir Azure AD kiracısı ekleyin</span><span class="sxs-lookup"><span data-stu-id="0d387-119">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="0d387-120">[Microsoft Iş Ortağı Merkezi](https://partner.microsoft.com/dashboard)'nde genel yönetici olarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="0d387-120">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="0d387-121">Sağ üst köşedeki **Ayarlar**' ı seçin, **Hesap ayarları**' nı seçin ve **kiracılar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="0d387-121">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Azure AD profili bölmesindeki Ilişkilendir düğmesinin ekran görüntüsü."::: 

1. <span data-ttu-id="0d387-123">**İlişkilendir**' i seçin ve ardından ilişkilendirmek istediğiniz kiracıyı belirtin.</span><span class="sxs-lookup"><span data-stu-id="0d387-123">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="0d387-124">Sorulduğunda, ilişkilendirmek istediğiniz kiracıya genel yönetici olarak oturum açın ve ardından **Onayla**' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="0d387-124">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Yeni Azure AD ilişkilendirmesini Onayla bölmesindeki Onayla düğmesinin ekran görüntüsü."::: 

   <span data-ttu-id="0d387-126">İlişkilendirmeyi onayladıktan sonra, **tüm küme** iletileri görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="0d387-126">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="0d387-127">Yeni eklenen kiracıyı görüntülemek için **kiracı yönetimine dön**' ü seçin.</span><span class="sxs-lookup"><span data-stu-id="0d387-127">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="0d387-128">Zaten başka bir Iş Ortağı Merkezi hesabıyla ilişkili ise, bir kiracıyı bir hesap ile ilişkilendiremezsiniz.</span><span class="sxs-lookup"><span data-stu-id="0d387-128">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="0d387-129">Bir kiracıyı hesabınızdan kaldırın</span><span class="sxs-lookup"><span data-stu-id="0d387-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="0d387-130">[Microsoft Iş Ortağı Merkezi](https://partner.microsoft.com/dashboard)'nde genel yönetici olarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="0d387-130">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="0d387-131">Sağ üst köşedeki **Ayarlar** simgesini seçin ve ardından **Hesap ayarları**' nı seçin.</span><span class="sxs-lookup"><span data-stu-id="0d387-131">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="0d387-132">Sol bölmede **kiracılar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="0d387-132">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="0d387-133">**Azure AD kiracılarını Yönet** altında **iş ortağı** sekmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="0d387-133">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="0d387-134">İlişkilendirmesini kaldırmak istediğiniz kiracının yanındaki **Kaldır** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="0d387-134">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="Geçerli kiracı ilişkilerinin ve bunların kaldırma bağlantılarının ekran görüntüsü.":::

   <span data-ttu-id="0d387-136">Önceki ekran görüntüsünde gösterildiği gibi, tüm ilişkili kiracılar için **kaldırma** bağlantıları etkinleştirilir, birincil kiracı ve şu anda oturum açtığınız kiracı hariç.</span><span class="sxs-lookup"><span data-stu-id="0d387-136">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="0d387-137">Bir kiracıyı kaldırdığınızda, bu Kiracıdaki kullanıcıların artık Iş Ortağı Merkezi hesabına erişimi olmaz ve kaldırma, uzmanlarınızın bir etkisi olabilir.</span><span class="sxs-lookup"><span data-stu-id="0d387-137">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="0d387-138">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="0d387-138">Next steps</span></span>

- [<span data-ttu-id="0d387-139">Kullanıcı hesapları oluşturma</span><span class="sxs-lookup"><span data-stu-id="0d387-139">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






