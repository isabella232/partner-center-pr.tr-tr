---
title: Microsoft AppSource'da özel planlar
description: Microsoft AppSource 'de (Azure Market) özel planlar ayarlama.
ms.service: marketplace-customer
ms.topic: how-to
author: Guyshu
ms.author: gushuchm
ms.date: 06/08/2021
robots: noindex
ms.openlocfilehash: a392859c1106c747e0e7c696927ef3b25262e411
ms.sourcegitcommit: a576c9606ade59cef7d0b2d5e1584016740d08eb
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/11/2021
ms.locfileid: "112008606"
---
# <a name="private-plans-in-microsoft-appsource"></a><span data-ttu-id="1bf3c-103">Microsoft AppSource'da özel planlar</span><span class="sxs-lookup"><span data-stu-id="1bf3c-103">Private plans in Microsoft AppSource</span></span>

<span data-ttu-id="1bf3c-104">Özel planlar, yayımcıların belirli müşterilere özel planlar sağlamalarıdır.</span><span class="sxs-lookup"><span data-stu-id="1bf3c-104">Private plans are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="1bf3c-105">Bu seçenek artık Microsoft AppSource.</span><span class="sxs-lookup"><span data-stu-id="1bf3c-105">This option is now available in Microsoft AppSource.</span></span> <span data-ttu-id="1bf3c-106">Özel planlar, Hemen al eylem çağrısıyla Hizmet olarak yazılım  (SaaS) teklifleri için AppSource'ta satılır.</span><span class="sxs-lookup"><span data-stu-id="1bf3c-106">Private plans can be sold on AppSource for software as a service (SaaS) offers with the **Get it now** call-to-action.</span></span>

## <a name="ask-your-isv-for-a-private-plan"></a><span data-ttu-id="1bf3c-107">ISV'nize özel plan sorma</span><span class="sxs-lookup"><span data-stu-id="1bf3c-107">Ask your ISV for a private plan</span></span>

<span data-ttu-id="1bf3c-108">AppSource'ta size özel bir plan için doğrudan ISV'ye başvurarak özel fiyat ve teknik belirtimler üzerinde anlaşmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="1bf3c-108">For a private plan to be available to you in AppSource, you need to contact the ISV directly and negotiate a custom price and technical specifications.</span></span> <span data-ttu-id="1bf3c-109">Özel planın koşulları kabul edildiktan sonra ISV sizin için bir plan oluşturabilir ve bunu, sağlamanız gereken kuruluş kiracı kimliğine atar.</span><span class="sxs-lookup"><span data-stu-id="1bf3c-109">Once the terms of the private plan are agreed to, the ISV will create a plan for you and assign it to your organization’s tenant ID, which you’ll need to provide.</span></span>

### <a name="finding-your-tenant-id"></a><span data-ttu-id="1bf3c-110">Kiracı kimliğinizi bulma</span><span class="sxs-lookup"><span data-stu-id="1bf3c-110">Finding your tenant ID</span></span>

1. <span data-ttu-id="1bf3c-111">AppSource'ta, sağ üst köşede hesap profili simgenizi ve ardından Kiracıyı **görüntüle'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="1bf3c-111">In AppSource, in the upper right corner, select your account profile icon and then **View tenant**.</span></span>
2. <span data-ttu-id="1bf3c-112">Kiracı kimliğini kopyalayın ve ISV'ye girin.</span><span class="sxs-lookup"><span data-stu-id="1bf3c-112">Copy the tenant ID and provide it to the ISV.</span></span>

    :::image type="content" source="media/private-offers/find-tenant-id.png" alt-text="Kiracı kimliğinizin nasıl bulun olduğunu gösterir.":::

## <a name="find-a-private-plan-in-appsource"></a><span data-ttu-id="1bf3c-114">AppSource'ta özel plan bulma</span><span class="sxs-lookup"><span data-stu-id="1bf3c-114">Find a private plan in AppSource</span></span>

<span data-ttu-id="1bf3c-115">ISV'nin yeni özel planı AppSource'ta göremeden önce yayımlaması 48 saat kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="1bf3c-115">It can take up to 48 hours after the ISV publishes the new private plan before you see it in AppSource.</span></span> <span data-ttu-id="1bf3c-116">Kiracı kimliğiniz ile ilişkili özel  planları bulmak için AppSource'ın sağ üst köşesindeki Özel planlar (Kilit simgesi) öğesini seçin.</span><span class="sxs-lookup"><span data-stu-id="1bf3c-116">To find private plans associated with your tenant ID, select **Private plans** (Lock icon) at the upper right of AppSource.</span></span>

:::image type="content" source="media/private-offers/lock-icon.png" alt-text="Üst araç çubuğundaki kilit simgesini (asma kilit) gösterir.":::

<span data-ttu-id="1bf3c-118">Oturum başlatmadıysanız, bunu yapmak için bir ileti istenir.</span><span class="sxs-lookup"><span data-stu-id="1bf3c-118">If you are not signed in, a message will prompt you to do so.</span></span> <span data-ttu-id="1bf3c-119">Ardından Planlar + fiyatlandırma sekmesinde kiracı kimliğinizle ilişkili özel **planları satın** alın.</span><span class="sxs-lookup"><span data-stu-id="1bf3c-119">You can then purchase the private plans associated with your tenant ID on the **Plans + pricing** tab.</span></span>

:::image type="content" source="media/private-offers/plan-pricing-tab.png" alt-text="Plan ve fiyatlandırma sekmesindeki özel teklifleri gösterir.":::

<span data-ttu-id="1bf3c-121">Kiracınız için özel planlar kullanılamıyorsa, özel planlarınız veya tekliflerinizi olmadığınız iletisiyle ifade edilir.</span><span class="sxs-lookup"><span data-stu-id="1bf3c-121">If private plans are not available for your tenant, a message will state that you don’t have any private plans or offers.</span></span>

## <a name="purchase-a-private-plan"></a><span data-ttu-id="1bf3c-122">Özel plan satın alma</span><span class="sxs-lookup"><span data-stu-id="1bf3c-122">Purchase a private plan</span></span>

<span data-ttu-id="1bf3c-123">ISV, teklif içinde bir veya daha fazla özel plan içerebilir.</span><span class="sxs-lookup"><span data-stu-id="1bf3c-123">An ISV can include one or more private plans within an offer.</span></span> <span data-ttu-id="1bf3c-124">Her teklif hem genel hem de özel planlara sahip olabilir, ancak özel planlar sayfanın sağ üst köşesindeki Özel teklifler simgesinden (asma kilit) erişilen ayrı bir teklif listeleme sayfasında görünür.</span><span class="sxs-lookup"><span data-stu-id="1bf3c-124">Each offer can have both public and private plans, but private plans appear under a separate offer listing page accessed from the Private offers icon (padlock) at the upper right of the page.</span></span>

<span data-ttu-id="1bf3c-125">Kullanılabilir özel planlar Planlar **+ fiyatlandırma sekmesinde** görüntülenir. Özel planların mavi rozetleri vardır.</span><span class="sxs-lookup"><span data-stu-id="1bf3c-125">Available private plans display on the **Plans + pricing** tab. Private plans have a distinctive blue badge.</span></span>

:::image type="content" source="media/private-offers/private-plans-badge.png" alt-text="Özel tekliflerin yanındaki mavi özel teklif rozetini gösterir.":::

<span data-ttu-id="1bf3c-127">Seçili planı satın almak için Şimdi **al'ı seçin** ve sağlanan adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="1bf3c-127">To purchase a selected plan, select **Get it now** and follow the steps provided.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1bf3c-128">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="1bf3c-128">Next steps</span></span>

- [<span data-ttu-id="1bf3c-129">Microsoft AppSource nedir?</span><span class="sxs-lookup"><span data-stu-id="1bf3c-129">What is Microsoft AppSource?</span></span>](appsource-overview.md)
