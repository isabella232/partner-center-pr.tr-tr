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
ms.openlocfilehash: caea2002b5edc2958c0af316762408e309bcf14a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151211"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="f59bd-103">Iş Ortağı Merkezi hesabınızda birden çok kiracı ekleme ve yönetme</span><span class="sxs-lookup"><span data-stu-id="f59bd-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="f59bd-104">**Uygun roller**: genel yönetici | Hesap Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="f59bd-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="f59bd-105">Bu makalede, şirketiniz için birden çok Azure Active Directory (Azure AD) kiracılarının nasıl birleştirilmesi ve ardından bunları Iş Ortağı Merkezi hesabınıza eklemek ve yönetmek açıklanır.</span><span class="sxs-lookup"><span data-stu-id="f59bd-105">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="f59bd-106">Bunu yapmanız pek çok neden vardır.</span><span class="sxs-lookup"><span data-stu-id="f59bd-106">There are many reasons to do so.</span></span> <span data-ttu-id="f59bd-107">Örnek:</span><span class="sxs-lookup"><span data-stu-id="f59bd-107">For example:</span></span>

- <span data-ttu-id="f59bd-108">Şirketinizin, contoso, başka bir şirket olan Fabrikam almış olduğunu varsayalım.</span><span class="sxs-lookup"><span data-stu-id="f59bd-108">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="f59bd-109">İki şirketin ayrı kalmasını istiyorsunuz, ancak yeni çalışanların Iş Ortağı Merkezi 'ni kullanmasını istiyorsunuz.</span><span class="sxs-lookup"><span data-stu-id="f59bd-109">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="f59bd-110">Bu durumda, yeni şirketin Azure AD kiracısını Iş ortağı küresel hesabınızla (PGA) ilişkilendirirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f59bd-110">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="f59bd-111">Bu ilişki, her iki şirketteki kullanıcıların iş ortağı merkezi 'nde çalışmasına olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="f59bd-111">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="f59bd-112">İşletmenizi birden fazla kiracı (örneğin, *contoso.com*, *contoso.uk* ve *contoso.in*) ile çalıştırırsanız, bunları aynı bilgisayar hesabında gruplamak için çoklu kiralama kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f59bd-112">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="f59bd-113">Birleşmeler ve alma yönergeleri her iki şirketteki kiracılar ile çalışmanız gerekiyorsa, hem *constoso.com* hem de *fabrikam.com* kiracılarını kullanırsınız.</span><span class="sxs-lookup"><span data-stu-id="f59bd-113">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="f59bd-114">Kiracıların herhangi birinin kullanıcılarının şunları yapabilmesi gerekir:</span><span class="sxs-lookup"><span data-stu-id="f59bd-114">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="f59bd-115">Eğitim, dijital indirmeler veya Microsoft Sertifikalı Profesyonel (MCP) ilişkisi için Iş Ortağı Merkezi 'Ne erişin.</span><span class="sxs-lookup"><span data-stu-id="f59bd-115">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="f59bd-116">Microsoft İş Ortağı Ağı (MPN) admin veya teşvikleri admin gibi Iş Ortağı Merkezi rolleri atanmalıdır.</span><span class="sxs-lookup"><span data-stu-id="f59bd-116">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="f59bd-117">Hesabınıza bir Azure AD kiracısı ekleyin</span><span class="sxs-lookup"><span data-stu-id="f59bd-117">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="f59bd-118">[Microsoft Iş Ortağı Merkezi](https://partner.microsoft.com/dashboard)'nde genel yönetici olarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="f59bd-118">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="f59bd-119">Sağ üst köşedeki **Ayarlar**' ı seçin, **Hesap ayarları**' nı seçin ve **kiracılar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="f59bd-119">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Azure AD profili bölmesindeki Ilişkilendir düğmesinin ekran görüntüsü."::: 

1. <span data-ttu-id="f59bd-121">**İlişkilendir**' i seçin ve ardından ilişkilendirmek istediğiniz kiracıyı belirtin.</span><span class="sxs-lookup"><span data-stu-id="f59bd-121">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="f59bd-122">İstendiğinde, ilişkilendirmek istediğiniz kiracıda genel yönetici olarak oturum açın ve Onayla'ya **seçin.**</span><span class="sxs-lookup"><span data-stu-id="f59bd-122">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Yeni Azure AD ilişkilendirmesi onaylayın bölmesindeki Onayla düğmesinin ekran görüntüsü."::: 

   <span data-ttu-id="f59bd-124">İlişkiyi onaylandıktan sonra Tüm **ayarlamalar iletisi** görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="f59bd-124">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="f59bd-125">Yeni eklenen kiracıyı görüntülemek için Kiracı yönetimine **geri dön seçeneğini seçin.**</span><span class="sxs-lookup"><span data-stu-id="f59bd-125">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="f59bd-126">Zaten başka bir kiracı hesabıyla ilişkilendirilmişse kiracıyı bir hesapla İş Ortağı Merkezi.</span><span class="sxs-lookup"><span data-stu-id="f59bd-126">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="f59bd-127">Bir kiracıyı hesabınızdan kaldırma</span><span class="sxs-lookup"><span data-stu-id="f59bd-127">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="f59bd-128">Microsoft'ta genel yönetici olarak [oturum İş Ortağı Merkezi.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="f59bd-128">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="f59bd-129">Sağ üst kısımda Ayarlar simgesini **ve** ardından Hesap **ayarları'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="f59bd-129">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="f59bd-130">Sol bölmede **Kiracılar'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="f59bd-130">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="f59bd-131">**Azure AD kiracılarını yönet altında** İş ortağı **sekmesini** seçin.</span><span class="sxs-lookup"><span data-stu-id="f59bd-131">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="f59bd-132">**İlişkilerini** kaldırmak istediğiniz kiracının yanındaki Kaldır'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="f59bd-132">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="Geçerli kiracı ilişkilendirmelerinin ve bunların Kaldır bağlantılarının ekran görüntüsü.":::

   <span data-ttu-id="f59bd-134">Önceki ekran görüntüsünde gösterildiği  gibi, Birincil kiracı ve o anda oturum asanız kiracı dışında tüm ilişkili kiracılar için Kaldır bağlantıları etkinleştirilir.</span><span class="sxs-lookup"><span data-stu-id="f59bd-134">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="f59bd-135">Bir kiracıyı kaldırsanız, kiracı üzerindeki kullanıcılar artık İş Ortağı Merkezi hesabı erişimine sahip olmaz ve kaldırmanın yetkinliklerinizi etkilemesi olabilir.</span><span class="sxs-lookup"><span data-stu-id="f59bd-135">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="f59bd-136">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="f59bd-136">Next steps</span></span>

- [<span data-ttu-id="f59bd-137">Kullanıcı hesapları oluşturma</span><span class="sxs-lookup"><span data-stu-id="f59bd-137">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






