---
title: Microsoft Müşteri sözleşmesinin müşteri kabul kabulü
description: Müşterinin adına Microsoft Müşteri sözleşmesinin kabul edilmesine ilişkin bir fikir sahibi olduğunu öğrenin.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/16/2020
ms.openlocfilehash: 921926ba44a592b8d2fb5da0a50697d62d9d95c7
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534786"
---
# <a name="attest-acceptance-of-the-microsoft-customer-agreement-on-behalf-of-your-customer"></a><span data-ttu-id="79f55-103">Müşterinizin adına Microsoft Müşteri sözleşmesinin onay onayı</span><span class="sxs-lookup"><span data-stu-id="79f55-103">Attest acceptance of the Microsoft Customer Agreement on behalf of your customer</span></span>


<span data-ttu-id="79f55-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="79f55-104">**Appropriate roles**</span></span>

- <span data-ttu-id="79f55-105">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="79f55-105">Global admin</span></span>
- <span data-ttu-id="79f55-106">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="79f55-106">Admin agent</span></span>
- <span data-ttu-id="79f55-107">Yardım Masası Aracısı</span><span class="sxs-lookup"><span data-stu-id="79f55-107">Helpdesk agent</span></span>

<span data-ttu-id="79f55-108">Bu makalede, müşterinin müşterinin adına Microsoft Müşteri Sözleşmesi kabulünü test etmeniz gerekebilecek bazı senaryolar açıklanır.</span><span class="sxs-lookup"><span data-stu-id="79f55-108">This article describes certain scenarios where you might need to attest a customer's acceptance of the Microsoft Customer Agreement on the customer's behalf.</span></span>

>[!NOTE]
><span data-ttu-id="79f55-109">Daha fazla bilgi edinmek için bkz. [Microsoft Müşteri sözleşmesinin müşteri kabulünü de onaylayın](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="79f55-109">To learn more, see also [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a><span data-ttu-id="79f55-110">Müşterinizin adına test etmeniz gereken iki senaryo</span><span class="sxs-lookup"><span data-stu-id="79f55-110">Two scenarios where you need to attest on behalf of your customer</span></span>

<span data-ttu-id="79f55-111">Müşterilerin, Microsoft Müşteri sözleşmesini Microsoft 365 Yönetim Merkezi 'nde doğrudan kabul edebilecekleri iki senaryo vardır.</span><span class="sxs-lookup"><span data-stu-id="79f55-111">There are currently two scenarios where customers may not be able to directly accept the Microsoft Customer Agreement within the Microsoft 365 Admin Center.</span></span>

<span data-ttu-id="79f55-112">**Senaryo 1**: mevcut bir müşteri, mevcut bir iş ortağı ilişkisi aracılığıyla aşağıdakilerden birini satın aldı: teklifler, yazılım veya yazılım abonelikleri, ayrılmış örnekler ve Azure planı.</span><span class="sxs-lookup"><span data-stu-id="79f55-112">**Scenario 1**: An existing customer has purchased any of the following through an existing partner relationship: offers, software or software subscriptions, Reserved Instances, and Azure Plan.</span></span> <span data-ttu-id="79f55-113">Müşteri artık yeni satın alma işlemi gerçekleştirmeye çalışıyor (otomatik yenileme hariç).</span><span class="sxs-lookup"><span data-stu-id="79f55-113">The customer is now attempting to make any new purchase (excluding auto renewal).</span></span> <span data-ttu-id="79f55-114">Bu müşteri URL 'YI tıklattığında, "Microsoft Müşteri anlaşmasını kabul etmek için lütfen Iş ortağınıza ulaşın" iletisini alırlar.</span><span class="sxs-lookup"><span data-stu-id="79f55-114">When that customer clicks the URL, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="79f55-115">**Çözümlemek için**: müşteri adına test etmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="79f55-115">**To resolve**: You must attest on behalf of the customer.</span></span>

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Microsoft Müşteri sözleşmesinin kabul edildiğini onaylamak için iş ortağınızla iletişime geçebilmeniz isteyen Microsoft 365 Yönetim Merkezi sayfasının ekran görüntüsü.":::

<span data-ttu-id="79f55-117">**Senaryo 2**: mevcut bir müşteri, aşağıdaki tekliflerden, yazılım ve yazılım aboneliklerinden, ayrılmış örneklerden ve Azure planından herhangi birini satın almış.</span><span class="sxs-lookup"><span data-stu-id="79f55-117">**Scenario 2**: An existing customer has purchased any of the following offers, software and software subscriptions, Reserved Instances, and Azure Plan.</span></span> <span data-ttu-id="79f55-118">Müşteri artık yeni bir iş ortağıyla yeni satın alma yapmaya çalışıyor.</span><span class="sxs-lookup"><span data-stu-id="79f55-118">The customer is now attempting to make any new purchase with a new partner.</span></span>

<span data-ttu-id="79f55-119">Müşteri, yeni iş ortağı ilişkisini ve sözleşmeyi kabul etmek üzere Yönetim Merkezi Microsoft 365 için URL 'YI tıkladığında, "lütfen Microsoft Müşteri sözleşmenizi kabul etmek için Iş ortağınıza ulaşın" iletisini alırlar.</span><span class="sxs-lookup"><span data-stu-id="79f55-119">When the customer clicks the URL to Microsoft 365 Admin Center to accept the new partner relationship and the agreement, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="79f55-120">**Çözümlemek için**: müşteri adına test etmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="79f55-120">**To resolve**: You must attest on behalf of the customer.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="79f55-121">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="79f55-121">Next steps</span></span>

- [<span data-ttu-id="79f55-122">Iş Ortağı Merkezi 'ne yeni bir müşteri kaydı ekleme</span><span class="sxs-lookup"><span data-stu-id="79f55-122">How to add a new customer record in Partner Center</span></span>](add-a-new-customer.md)
- [<span data-ttu-id="79f55-123">Giriş: Azure planı, iş ortaklarının müşteriler için Kullandıkça Öde tarifesine Azure satın almasını sağlar</span><span class="sxs-lookup"><span data-stu-id="79f55-123">Introduction: Azure plan lets partners buy Azure at pay-as-you-go-rates for customers</span></span>](azure-plan-lp.md)
