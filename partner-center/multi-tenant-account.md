---
title: Iş Ortağı Merkezi hesabınıza ek kiracılar ekleyin
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Iş Ortağı Merkezi hesabınızda birden çok Azure AD kiracılarının nasıl ekleneceğini, birleştireceğinizi veya yönetileceğini öğrenin. Bunu yapmak isteyebileceğiniz bazı nedenler hakkında bilgi edinin.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f9852b4e1c3997b82f744555db25fe64e1afc8ad
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182447"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="d84c1-104">Iş Ortağı Merkezi hesabınızda birden çok kiracı ekleme ve yönetme</span><span class="sxs-lookup"><span data-stu-id="d84c1-104">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="d84c1-105">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="d84c1-105">**Appropriate roles**</span></span>

- <span data-ttu-id="d84c1-106">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="d84c1-106">Global admin</span></span>
- <span data-ttu-id="d84c1-107">Hesap yöneticisi</span><span class="sxs-lookup"><span data-stu-id="d84c1-107">Account admin</span></span>

<span data-ttu-id="d84c1-108">Bu özellik şirketiniz için birden çok kiracıyı yönetmenizi ve bunları İş Ortağı Merkezi hesabında birleştirmenizi sağlar.</span><span class="sxs-lookup"><span data-stu-id="d84c1-108">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="d84c1-109">Iş Ortağı Merkezi hesabınızda birden çok Azure AD kiracıyı yönetmeniz gerekebileceği birçok neden vardır.</span><span class="sxs-lookup"><span data-stu-id="d84c1-109">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="d84c1-110">Örnek:</span><span class="sxs-lookup"><span data-stu-id="d84c1-110">For example:</span></span>

- <span data-ttu-id="d84c1-111">Şirketiniz başka bir şirket satın alabilir ve yeni şirketteki çalışanların Iş ortağı merkezini kullanmasını istiyorsunuz.</span><span class="sxs-lookup"><span data-stu-id="d84c1-111">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="d84c1-112">Ancak, iki şirketin ayrı kalmasını istersiniz.</span><span class="sxs-lookup"><span data-stu-id="d84c1-112">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="d84c1-113">Bu durumda, yeni şirketin Azure AD kiracısını Iş ortağı küresel hesabınızla (PGA) ilişkilendirirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d84c1-113">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="d84c1-114">Bu ilişki, her iki şirketteki kullanıcıların iş ortağı merkezi 'nde çalışmasını sağlar.</span><span class="sxs-lookup"><span data-stu-id="d84c1-114">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="d84c1-115">İşletmenizi çalıştırmak için birden fazla kiracınız varsa (örn. contoso.com, contoso.uk, contoso.in), aynı bılgısayar hesabı altına bağlamak için çok kiracılı bir şekilde kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d84c1-115">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="d84c1-116">Birleşmeler ve alımlar birden fazla kiracı ile çalışmanız gerekir (örn. contoso fabrikam 'ı edindiğinde, hem Constoso.com hem de Fabrikam.com ilgili kiracılar kullanabilmek gerekir).</span><span class="sxs-lookup"><span data-stu-id="d84c1-116">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="d84c1-117">Kiracıların herhangi birinden kullanıcıların şunları yapabilmesi gerekir:</span><span class="sxs-lookup"><span data-stu-id="d84c1-117">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="d84c1-118">Eğitim, dijital indirmeler, MCP ilişkilendirmesi için Iş Ortağı Merkezi 'Ne erişin</span><span class="sxs-lookup"><span data-stu-id="d84c1-118">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="d84c1-119">MPN admin, teşvikleri admin vb. gibi Iş Ortağı Merkezi rolleri atanmalıdır.</span><span class="sxs-lookup"><span data-stu-id="d84c1-119">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="d84c1-120">Hesabınıza başka bir Azure AD kiracısı ekleyin</span><span class="sxs-lookup"><span data-stu-id="d84c1-120">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="d84c1-121">Genel yönetici olarak, Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="d84c1-121">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="d84c1-122">**Ayarlar** simgesinden **Hesap ayarları** ' nı seçin ve **kiracılar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="d84c1-122">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Kiracılar ilişkilendir"::: 

3. <span data-ttu-id="d84c1-124">**Başka BIR ad kiracısını ilişkilendir** ' i seçin ve ilişkilendirmek istediğiniz kiracıyı belirtin.</span><span class="sxs-lookup"><span data-stu-id="d84c1-124">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="d84c1-125">Genel yönetici olarak, ilişkilendirmek istediğiniz kiracıda oturum açın ve ilişkilendirmeyi onaylayın.</span><span class="sxs-lookup"><span data-stu-id="d84c1-125">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Kiracılar ilişkilendirmeyi Onayla"::: 

5. <span data-ttu-id="d84c1-127">' Yi doğruladıktan sonra, bir **küme** bildirimi görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="d84c1-127">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="d84c1-128">**Kiracı yönetimine dön** ' ü seçin ve yeni eklenen kiracıyı listelendiğini görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="d84c1-128">Select **Return to tenant management** and you'll see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="d84c1-129">Bir kiracıyı zaten başka bir Iş Ortağı Merkezi hesabıyla ilişkili ise bir firmayla ilişkilendiremezsiniz.</span><span class="sxs-lookup"><span data-stu-id="d84c1-129">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="d84c1-130">Bir kiracıyı hesabınızdan kaldırın</span><span class="sxs-lookup"><span data-stu-id="d84c1-130">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="d84c1-131">Genel yönetici olarak, Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="d84c1-131">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="d84c1-132">**Ayarlar** simgesinden **Hesap ayarları** -kiracılar > seçin ve **iş ortağı** sekmesine tıklayın.</span><span class="sxs-lookup"><span data-stu-id="d84c1-132">From the **Settings** icon, select **Account settings** -> Tenants and click on the **Partner** tab.</span></span>
 
3. <span data-ttu-id="d84c1-133">İlişkilendirmesini **kaldırmak** istediğiniz kiracı için Kaldır ' a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="d84c1-133">Click **Remove** for the tenant you want to dissociate.</span></span>

4. <span data-ttu-id="d84c1-134">Bir kiracının ilişkilendirmesini kaldırmak, söz konusu Kiracıdaki kullanıcıların artık Iş Ortağı Merkezi hesabına erişemeyeceği anlamına gelir ve bu, uzmanlarınızın bir etkisi olabilir.</span><span class="sxs-lookup"><span data-stu-id="d84c1-134">Dissociating a tenant means that the users on that tenant will no longer have access to the Partner Center account, and this could have an impact on your competencies.</span></span> 

<span data-ttu-id="d84c1-135">Birincil kiracı ve şu anda oturum açtığınız Kiracı dışında, ilişkili tüm kiracılar için **Kaldır** düğmesi etkinleştirilir.</span><span class="sxs-lookup"><span data-stu-id="d84c1-135">The **Remove** button is enabled for all associated tenants, except the primary tenant and the tenant which you are currently signed into.</span></span>

:::image type="content" source="images/disassociate.png" alt-text="Kaldır düğmesi olan kiracılar":::
 

## <a name="next-steps"></a><span data-ttu-id="d84c1-137">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="d84c1-137">Next steps</span></span>

- [<span data-ttu-id="d84c1-138">Kullanıcı ekle</span><span class="sxs-lookup"><span data-stu-id="d84c1-138">Add users</span></span>](create-user-accounts-and-set-permissions.md)






