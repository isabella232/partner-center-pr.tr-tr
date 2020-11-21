---
title: Aktarım uygunluğu – bir aboneliği faturalandırma hesapları, Azure Marketi arasında aktarmaya yönelik yönergeler
description: Azure portal faturalandırma hesapları arasında abonelik aktarmadan önce ticari denetimleri için yönergeler.
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: a6a3c8954643ea982ae5107ae417a900ed51e77d
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007600"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a><span data-ttu-id="1d5fc-103">Faturalama hesapları arasında bir abonelik için aktarım uygunluğu</span><span class="sxs-lookup"><span data-stu-id="1d5fc-103">Transfer eligibility for a subscription between billing accounts</span></span>

<span data-ttu-id="1d5fc-104">Azure portal Faturalandırma bölümünde bir faturalandırma hesabından diğerine [abonelik aktarabilirsiniz](/azure/cost-management-billing/understand/subscription-transfer) .</span><span class="sxs-lookup"><span data-stu-id="1d5fc-104">You can [transfer a subscription](/azure/cost-management-billing/understand/subscription-transfer) from one billing account to another in the billing section of the Azure portal.</span></span> <span data-ttu-id="1d5fc-105">Bir aktarımdan önce abonelik, üçüncü taraf ürünleri için taranır.</span><span class="sxs-lookup"><span data-stu-id="1d5fc-105">Prior to a transfer, the subscription is scanned for third-party products.</span></span> <span data-ttu-id="1d5fc-106">Aktarıma yalnızca *Tüm* ürünler aktarım için silinirse izin verilir (aşağıdaki [ölçütlere](#criteria-for-transfer-approval-or-denial) bakın).</span><span class="sxs-lookup"><span data-stu-id="1d5fc-106">The transfer is permitted only if *all* products are cleared for transfer (see the [criteria](#criteria-for-transfer-approval-or-denial) below).</span></span> <span data-ttu-id="1d5fc-107">Sistem, sonraki adımları belirlemenize yardımcı olmak için temizlendirilemez uygulamalar için ilgili hata iletileri oluşturur.</span><span class="sxs-lookup"><span data-stu-id="1d5fc-107">The system will generate relevant error messages for the apps that failed to clear to help you determine next steps.</span></span>

> [!NOTE]
> <span data-ttu-id="1d5fc-108">SaaS kaynakları bir aboneliğe değil bir kiracıya eklendiğinden, bu makale SaaS teklifleri için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="1d5fc-108">This article does not apply to SaaS offers because SaaS resources are attached to a tenant, not a subscription.</span></span> <span data-ttu-id="1d5fc-109">SaaS kaynakları bir faturalandırma hesabından diğerine aktarılabilir, ancak bu, kaynak başına ve destek talebi olarak Azure desteği tarafından yapılır.</span><span class="sxs-lookup"><span data-stu-id="1d5fc-109">SaaS resources are transferable from one billing account to another, but this is done per resource and by Azure support as a support request.</span></span>

## <a name="criteria-for-transfer-approval-or-denial"></a><span data-ttu-id="1d5fc-110">Aktarım onayı veya reddetme ölçütü</span><span class="sxs-lookup"><span data-stu-id="1d5fc-110">Criteria for transfer approval or denial</span></span>

<span data-ttu-id="1d5fc-111">Üçüncü taraf uygulamalarından herhangi biri aşağıdaki ölçütlerden herhangi birini karşılıyorsa aboneliği aktaramazsınız:</span><span class="sxs-lookup"><span data-stu-id="1d5fc-111">You cannot transfer a subscription if any of its third-party apps meet any of the following criteria:</span></span>

- <span data-ttu-id="1d5fc-112">Hedef hesap ticari ve uygulama iş ortakları aracılığıyla satılacak şekilde kabul edilir.</span><span class="sxs-lookup"><span data-stu-id="1d5fc-112">The target account is commercial and the app is opt-out to be sold via partners.</span></span>
- <span data-ttu-id="1d5fc-113">Uygulama, seçilen iş ortakları için kabul ediyor ve hedef hesap izin verilenler listesinde değil.</span><span class="sxs-lookup"><span data-stu-id="1d5fc-113">The app is opt-in for selected partners and the target account is not in the allow list.</span></span>
- <span data-ttu-id="1d5fc-114">Teklif, geçmişte seçili abonelikler için bir önizleme teklifiydi veya özel bir teklifdi ve abonelik artık izin verilenler listesinde değil.</span><span class="sxs-lookup"><span data-stu-id="1d5fc-114">The offer was a preview offer in the past for selected subscriptions or was a private offer and the subscription is no longer in the allow list.</span></span>
- <span data-ttu-id="1d5fc-115">Yeni faturalandırma hesabı, teklifin satışında farklı olan ve teklifin bu bölgede satılmama yeri dışında bir bölgedir.</span><span class="sxs-lookup"><span data-stu-id="1d5fc-115">The new billing account is in a region different from where the offer is sold AND the offer is not to be sold in that region.</span></span>

<span data-ttu-id="1d5fc-116">Engellenen bir aktarım, kaynağı abonelikten kaldırana kadar etkin kalır, sonra aktarmayı yeniden deneyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1d5fc-116">A blocked transfer remains in effect until you remove the resource from the subscription, after which you can try the transfer again.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1d5fc-117">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="1d5fc-117">Next steps</span></span>

[<span data-ttu-id="1d5fc-118">Microsoft AppSource ve Azure Marketi için destek alın</span><span class="sxs-lookup"><span data-stu-id="1d5fc-118">Get support for Microsoft AppSource and Azure Marketplace</span></span>](get-support.md)

