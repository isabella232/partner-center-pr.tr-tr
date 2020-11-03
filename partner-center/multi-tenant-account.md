---
title: Iş Ortağı Merkezi hesabınıza ek kiracılar ekleyin
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Iş Ortağı Merkezi hesabınızda birden çok Azure AD kiracılarının nasıl ekleneceğini, birleştireceğinizi veya yönetileceğini öğrenin. Bunu yapmak isteyebileceğiniz bazı nedenler hakkında bilgi edinin.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b9379ce6b27a8ef6e5d6894a0630745794e04e04
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/19/2020
ms.locfileid: "92532027"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="ed0ee-104">Iş Ortağı Merkezi hesabınızda birden çok kiracı ekleme ve yönetme</span><span class="sxs-lookup"><span data-stu-id="ed0ee-104">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="ed0ee-105">**Uygulama hedefi**</span><span class="sxs-lookup"><span data-stu-id="ed0ee-105">**Applies to**</span></span>

- <span data-ttu-id="ed0ee-106">İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="ed0ee-106">Partner Center</span></span>

<span data-ttu-id="ed0ee-107">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="ed0ee-107">**Appropriate roles**</span></span>

- <span data-ttu-id="ed0ee-108">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="ed0ee-108">Global admin</span></span>

<span data-ttu-id="ed0ee-109">Bu özellik şirketiniz için birden çok kiracıyı yönetmenizi ve bunları İş Ortağı Merkezi hesabında birleştirmenizi sağlar.</span><span class="sxs-lookup"><span data-stu-id="ed0ee-109">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="ed0ee-110">Iş Ortağı Merkezi hesabınızda birden çok Azure AD kiracıyı yönetmeniz gerekebileceği birçok neden vardır.</span><span class="sxs-lookup"><span data-stu-id="ed0ee-110">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="ed0ee-111">Örneğin:</span><span class="sxs-lookup"><span data-stu-id="ed0ee-111">For example:</span></span>

- <span data-ttu-id="ed0ee-112">Şirketiniz başka bir şirket satın alabilir ve yeni şirketteki çalışanların Iş ortağı merkezini kullanmasını istiyorsunuz.</span><span class="sxs-lookup"><span data-stu-id="ed0ee-112">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="ed0ee-113">Ancak, iki şirketin ayrı kalmasını istersiniz.</span><span class="sxs-lookup"><span data-stu-id="ed0ee-113">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="ed0ee-114">Bu durumda, yeni şirketin Azure AD kiracısını Iş ortağı küresel hesabınızla (PGA) ilişkilendirirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ed0ee-114">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="ed0ee-115">Bu ilişki, her iki şirketteki kullanıcıların iş ortağı merkezi 'nde çalışmasını sağlar.</span><span class="sxs-lookup"><span data-stu-id="ed0ee-115">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="ed0ee-116">İşletmenizi çalıştırmak için birden fazla kiracınız varsa (örn. contoso.com, contoso.uk, contoso.in), aynı bılgısayar hesabı altına bağlamak için çok kiracılı bir şekilde kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ed0ee-116">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="ed0ee-117">Birleşmeler ve alımlar birden fazla kiracı ile çalışmanız gerekir (örn. contoso fabrikam 'ı edindiğinde, hem Constoso.com hem de Fabrikam.com ilgili kiracılar kullanabilmek gerekir).</span><span class="sxs-lookup"><span data-stu-id="ed0ee-117">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="ed0ee-118">Kiracıların herhangi birinden kullanıcıların şunları yapabilmesi gerekir:</span><span class="sxs-lookup"><span data-stu-id="ed0ee-118">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="ed0ee-119">Eğitim, dijital indirmeler, MCP ilişkilendirmesi için Iş Ortağı Merkezi 'Ne erişin</span><span class="sxs-lookup"><span data-stu-id="ed0ee-119">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="ed0ee-120">MPN admin, teşvikleri admin vb. gibi Iş Ortağı Merkezi rolleri atanmalıdır.</span><span class="sxs-lookup"><span data-stu-id="ed0ee-120">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="ed0ee-121">Hesabınıza başka bir Azure AD kiracısı ekleyin</span><span class="sxs-lookup"><span data-stu-id="ed0ee-121">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="ed0ee-122">Genel yönetici olarak, Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="ed0ee-122">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="ed0ee-123">**Ayarlar** simgesinden **Hesap ayarları** ' nı seçin ve **kiracılar** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="ed0ee-123">From the **Settings** icon, select **Account settings** and then select **Tenants** .</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Kiracılar ilişkilendir"::: 

3. <span data-ttu-id="ed0ee-125">**Başka BIR ad kiracısını ilişkilendir** ' i seçin ve ilişkilendirmek istediğiniz kiracıyı belirtin.</span><span class="sxs-lookup"><span data-stu-id="ed0ee-125">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="ed0ee-126">Genel yönetici olarak, ilişkilendirmek istediğiniz kiracıda oturum açın ve ilişkilendirmeyi onaylayın.</span><span class="sxs-lookup"><span data-stu-id="ed0ee-126">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Kiracılar ilişkilendirmeyi Onayla"::: 

5. <span data-ttu-id="ed0ee-128">' Yi doğruladıktan sonra, bir **küme** bildirimi görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="ed0ee-128">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="ed0ee-129">**Kiracı yönetimine dön** ' ü seçin ve yeni eklenen kiracıyı listelenmiş olarak görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="ed0ee-129">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="ed0ee-130">Bir kiracıyı zaten başka bir Iş Ortağı Merkezi hesabıyla ilişkili ise bir firmayla ilişkilendiremezsiniz.</span><span class="sxs-lookup"><span data-stu-id="ed0ee-130">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>

 
## <a name="next-steps"></a><span data-ttu-id="ed0ee-131">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="ed0ee-131">Next steps</span></span>

- [<span data-ttu-id="ed0ee-132">Kullanıcı ekle</span><span class="sxs-lookup"><span data-stu-id="ed0ee-132">Add users</span></span>](create-user-accounts-and-set-permissions.md)
