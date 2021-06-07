---
title: Azure Market 'te özel teklifler
description: Azure Marketi 'ndeki özel teklifler hakkında bilgi edinin.
ms.service: marketplace-customer
ms.topic: article
author: Guyshu
ms.author: gushuchm
ms.date: 06/03/2021
ms.openlocfilehash: 55d0716b183e9e8905e631447e547396d6f55404
ms.sourcegitcommit: 9cb6bc9df20540f812b7932f88e520976c1aa85a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/06/2021
ms.locfileid: "111534166"
---
# <a name="private-plans-in-azure-marketplace"></a><span data-ttu-id="f0aed-103">Azure Marketi 'nde özel planlar</span><span class="sxs-lookup"><span data-stu-id="f0aed-103">Private plans in Azure Marketplace</span></span>

<span data-ttu-id="f0aed-104">Özel planlar, yayımcıların belirli müşterilere özel planlar sağlamalarına göre yapılır.</span><span class="sxs-lookup"><span data-stu-id="f0aed-104">Private plans are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="f0aed-105">Özel planlar yalnızca satın alınabilecek ve Azure portal doğrudan yüklenebilen ücretli tekliflerle kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="f0aed-105">Private plans are only available for paid offers that can be purchased and directly installed from the Azure portal.</span></span> <span data-ttu-id="f0aed-106">Yayımcılar, Portal 'dan yüklenip yüklenemediğine bakılmaksızın danışmanlık hizmetleri için bir eylem çağrısı veya ücretsiz **hizmeti olan herhangi** bir hizmet için özel planlar oluşturamaz.</span><span class="sxs-lookup"><span data-stu-id="f0aed-106">Publishers cannot create private plans for consulting services, any service that has **Contact me** as a call-to-action, or any free service, regardless of whether it can be installed from the portal or not.</span></span>

## <a name="find-private-plans-in-the-azure-portal"></a><span data-ttu-id="f0aed-107">Azure portal özel planlar bulun</span><span class="sxs-lookup"><span data-stu-id="f0aed-107">Find private plans in the Azure portal</span></span>

<span data-ttu-id="f0aed-108">Bir iş ortağı özel bir plan yayımladığında, yalnızca Azure portal **Market** bölümündeki uygun kullanıcılar tarafından görülebilir.</span><span class="sxs-lookup"><span data-stu-id="f0aed-108">When a partner publishes a private plan, it is visible only to eligible users in the **Marketplace** section of the Azure portal.</span></span> <span data-ttu-id="f0aed-109">Bu kullanıcılar, teklif türüne bağlı olarak abonelik KIMLIĞI veya kiracı KIMLIĞI tarafından tanımlanır.</span><span class="sxs-lookup"><span data-stu-id="f0aed-109">These users are defined by subscription ID or tenant ID, depending on the offer type.</span></span> <span data-ttu-id="f0aed-110">Özel planlara uygunsanız, bunları portalda bulmanın iki yolu vardır.</span><span class="sxs-lookup"><span data-stu-id="f0aed-110">If you are eligible for private plans, there are two ways to find them in the portal.</span></span>

> [!NOTE]
> <span data-ttu-id="f0aed-111">Özel planlar Azure portal aranabilir ancak filtrelenebilir değil (kategoriye göre).</span><span class="sxs-lookup"><span data-stu-id="f0aed-111">Private plans are searchable but not filterable (by category) in the Azure portal.</span></span>

<span data-ttu-id="f0aed-112">Azure portal, **Market** sayfasına gitmek için **+ kaynak oluştur** ' u seçin veya "Market" araması yapın.</span><span class="sxs-lookup"><span data-stu-id="f0aed-112">In the Azure portal, select **+ Create a resource** or search for “marketplace” to go to the **Marketplace** page.</span></span> <span data-ttu-id="f0aed-113">Özel planlara uygunsanız, sayfanın üst kısmında **özel planlar kullanılabilir başlık olduğunu** görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="f0aed-113">If you are eligible for private plans, you will see the **You have private plans available** banner on the top of the page.</span></span> <span data-ttu-id="f0aed-114">Özel planlar sayfanıza gitmek için **özel teklifleri görüntüle + planlar** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="f0aed-114">Select **View private offers + plans** to go to your private plans page.</span></span>

:::image type="content" source="media/private-offers/private-offers-banner.png" alt-text="Özel planlarınız varsa görüntülenen başlık.":::

## <a name="review-private-plans"></a><span data-ttu-id="f0aed-116">Özel planları gözden geçirme</span><span class="sxs-lookup"><span data-stu-id="f0aed-116">Review private plans</span></span>

<span data-ttu-id="f0aed-117">Özel bir plan, bir teklifte çeşitli planların bir parçasıdır.</span><span class="sxs-lookup"><span data-stu-id="f0aed-117">A private plan is part of several plans in an offer.</span></span> <span data-ttu-id="f0aed-118">Her teklifin hem genel hem de özel birden çok planı olabilir, ancak özel planlar genel planlardan ayrı bir liste altında gösterilir.</span><span class="sxs-lookup"><span data-stu-id="f0aed-118">Each offer can have multiple plans, both public and private, but private plans are shown under a separate listing from public plans.</span></span>

<span data-ttu-id="f0aed-119">Kullanılabilir özel planları, farklı bir **özel** rozet Ile işaretlenmiş **planlar** sekmesinde görebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="f0aed-119">You can see the available private plans under the **Plans** tab, marked with a distinctive **Private** badge:</span></span>

:::image type="content" source="media/private-offers/private-badge.png" alt-text="Özel olarak işaretlenen planların bir sayfası.":::

<span data-ttu-id="f0aed-121">Birden fazla aboneliğiniz varsa tüm abonelikleriniz için kullanılabilir olan tüm özel planları görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="f0aed-121">If you have more than one subscription, you will see all private plans available for all your subscriptions.</span></span> <span data-ttu-id="f0aed-122">**Oluştur**' u seçtiğinizde, kaynağı yapılandırmaya başlamak için kaynak oluşturma sayfasına yönlendirilir.</span><span class="sxs-lookup"><span data-stu-id="f0aed-122">When you select **Create**, you are routed to the resource creation page to start configuring your resource.</span></span>

<span data-ttu-id="f0aed-123">**Oluştur** ve birden çok abonelik varsa, ancak bunların tümü özel plana eklendiyse, varsayılan aboneliğiniz bu özel plana uygun abonelik olmayabilir.</span><span class="sxs-lookup"><span data-stu-id="f0aed-123">If you select **Create** and have multiple subscriptions, but not all of them are added to the private plan, your default subscription may not be the subscription eligible for this private plan.</span></span> <span data-ttu-id="f0aed-124">Bu durumda, doğru aboneliği seçin.</span><span class="sxs-lookup"><span data-stu-id="f0aed-124">In this case, select the correct subscription.</span></span>

:::image type="content" source="media/private-offers/select-correct-subscription.png" alt-text="Daha fazla özel plan olduğunu gösteren bağlantı.":::

## <a name="next-steps"></a><span data-ttu-id="f0aed-126">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="f0aed-126">Next steps</span></span>

- [<span data-ttu-id="f0aed-127">Azure Market nedir?</span><span class="sxs-lookup"><span data-stu-id="f0aed-127">What is Azure Marketplace?</span></span>](azure-marketplace-overview.md)
