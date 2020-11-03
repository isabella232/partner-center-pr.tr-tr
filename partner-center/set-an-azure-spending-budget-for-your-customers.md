---
title: Müşteriler için bir Azure harcama bütçesi ayarlama
ms.topic: how-to
ms.date: 06/03/2020
description: Müşterileriniz için aylık Azure harcama bütçelerini ayarlamayı veya kaldırmayı ve ayrıca Azure harcama verilerini görüntülemeyi ve bütçeye ilişkin bildirimleri ayarlamayı öğrenin.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 982d4ed310415349acde3d260afce04eb0d55ac5
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2020
ms.locfileid: "92531214"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="de66d-103">Iş Ortağı Merkezi 'nde müşterilere yönelik aylık Azure harcama bütçelerini ayarlama, denetleme veya kaldırma</span><span class="sxs-lookup"><span data-stu-id="de66d-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="de66d-104">Aşağıdakiler cihazlar için geçerlidir:</span><span class="sxs-lookup"><span data-stu-id="de66d-104">Applies to:</span></span>

- <span data-ttu-id="de66d-105">İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="de66d-105">Partner Center</span></span>
- <span data-ttu-id="de66d-106">ABD kamu için Microsoft Bulut iş ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="de66d-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="de66d-107">Iş Ortağı Merkezi 'nde [müşterileriniz için aylık bir Azure harcama bütçesi ayarlayabilirsiniz](#set-azure-spending-budget) .</span><span class="sxs-lookup"><span data-stu-id="de66d-107">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="de66d-108">Bu, müşterilerinizin Azure harcamalarını yönetmesine yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="de66d-108">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="de66d-109">Bu seçenek, müşterilerinizin aylık dönemi boyunca Azure harcamalarınızı bütçenize göre karşılaştırmanızı sağlar.</span><span class="sxs-lookup"><span data-stu-id="de66d-109">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="de66d-110">Ayrıca, müşterilerinizin aylık faturanız düşünenden daha yüksek olmaması için Azure harcamalarını bütçelerinize de yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="de66d-110">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="de66d-111">Bu özellik korumalı alanda veya üretimde test (tıp) hesaplarında kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="de66d-111">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="de66d-112">Müşterilerinizin [Azure harcama bütçesini ayarladıktan](#set-azure-spending-budget)sonra, müşteri kullanımını aşağıdaki yollarla da gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="de66d-112">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="de66d-113">Bu seçenekler, yanlış yapılandırılmış Hizmetleri veya sahtekarlık önereceği olağan dışı eğilimleri belirlemenize yardımcı olabilir.</span><span class="sxs-lookup"><span data-stu-id="de66d-113">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="de66d-114">Bundan sonra, temel nedeni belirlemek ve maliyetleri yönetmek için müşteri (ler) i ile çalışabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="de66d-114">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="de66d-115">Gerekirse, [müşterinin bütçesini](#set-azure-spending-budget) daha yüksek bir tutara de değiştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="de66d-115">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="de66d-116">Geçerli Azure harcamayı denetle</span><span class="sxs-lookup"><span data-stu-id="de66d-116">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="de66d-117">Müşterinin harcama süresi Bütçe limitine yaklaştığı zaman için e-posta bildirimlerini aç</span><span class="sxs-lookup"><span data-stu-id="de66d-117">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="de66d-118">Kullanım tabanlı abonelikler için hizmete göre listelenen maliyetleri görüntüleme</span><span class="sxs-lookup"><span data-stu-id="de66d-118">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="de66d-119">Ayrıca, müşteriler için [bir Azure harcama bütçesini](#remove-azure-spending-budget) dilediğiniz zaman kaldırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="de66d-119">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="de66d-120">Azure harcama verileri</span><span class="sxs-lookup"><span data-stu-id="de66d-120">Azure spending data</span></span>

<span data-ttu-id="de66d-121">Azure harcama verileri bir *tahmindir* ve *gerçek faturalandırma miktarları farklılık* gösterebilir.</span><span class="sxs-lookup"><span data-stu-id="de66d-121">The Azure spending data is an *estimate* and *actual billing amounts may vary* .</span></span> <span data-ttu-id="de66d-122">Verilerin değeri vergileri, kredilerin, ayarlamaların veya uygulayabilen diğer ücretleri *yansıtmaz* .</span><span class="sxs-lookup"><span data-stu-id="de66d-122">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="de66d-123">Harcama verileri *günde bir kez yenilenir* .</span><span class="sxs-lookup"><span data-stu-id="de66d-123">The spending data is *refreshed once per day* .</span></span> <span data-ttu-id="de66d-124">Müşterileriniz, Azure portal hesap ayarlarını değiştirmediğiniz müddetçe Azure hizmetleri ve kaynakları kullanmaya ve ücretlendirmeye devam edebilir.</span><span class="sxs-lookup"><span data-stu-id="de66d-124">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="de66d-125">Azure harcama bütçesini ayarlama</span><span class="sxs-lookup"><span data-stu-id="de66d-125">Set Azure spending budget</span></span>

<span data-ttu-id="de66d-126">Iş Ortağı Merkezi 'nde birden çok müşteri için *aylık bir Azure harcama bütçesi ayarlayabilirsiniz* :</span><span class="sxs-lookup"><span data-stu-id="de66d-126">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="de66d-127">[Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="de66d-127">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="de66d-128">**CSP** altındaki sol menüde **Azure harcama** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="de66d-128">In the left-hand menu under **CSP** , choose **Azure spending** .</span></span>

3. <span data-ttu-id="de66d-129">**Azure harcama** sayfasında, **Microsoft Azure abonelikleri olan müşteriler** altında, bütçesini ayarlamak istediğiniz müşteri (ler) i seçin.</span><span class="sxs-lookup"><span data-stu-id="de66d-129">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions** , select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="de66d-130">**Aylık bütçe** için bir değer girin.</span><span class="sxs-lookup"><span data-stu-id="de66d-130">Enter a value for **Monthly budget** .</span></span>

5. <span data-ttu-id="de66d-131">Değişikliklerinizi kaydetmek için **Uygula** ' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="de66d-131">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="de66d-132">Ayrıca, abonelik ayarlarında *tek bir müşteri için bir bütçe ayarlayabilirsiniz* :</span><span class="sxs-lookup"><span data-stu-id="de66d-132">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="de66d-133">Iş Ortağı Merkezi panosunda oturum açın.</span><span class="sxs-lookup"><span data-stu-id="de66d-133">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="de66d-134">**CSP** altındaki sol menüde **müşteriler** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="de66d-134">In the left-hand menu under **CSP** , choose **Customers** .</span></span>

3. <span data-ttu-id="de66d-135">**Müşteriler** sayfasında, müşterinin **şirket adını** seçin.</span><span class="sxs-lookup"><span data-stu-id="de66d-135">On the **Customers** page, select the customer's **Company name** .</span></span>

4. <span data-ttu-id="de66d-136">Müşterinin **abonelikler** sayfasında, **Kullanım tabanlı abonelik** ' ın altında, **bütçeyi Değiştir** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="de66d-136">On the customer's **Subscriptions** page, under **Usage-based subscription** , choose **Change budget** .</span></span>

5. <span data-ttu-id="de66d-137">Bütçe için bir değer girin.</span><span class="sxs-lookup"><span data-stu-id="de66d-137">Enter a value for the budget.</span></span>

6. <span data-ttu-id="de66d-138">Değişikliklerinizi kaydetmek için **Uygula** ' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="de66d-138">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="de66d-139">Azure harcama bütçesini kaldırma</span><span class="sxs-lookup"><span data-stu-id="de66d-139">Remove Azure spending budget</span></span>

<span data-ttu-id="de66d-140">Iş Ortağı Merkezi 'nde müşteri (ler) için *aylık bir Azure harcama bütçesini kaldırabilirsiniz* :</span><span class="sxs-lookup"><span data-stu-id="de66d-140">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="de66d-141">[Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="de66d-141">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="de66d-142">**CSP** altındaki sol menüde **Azure harcama** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="de66d-142">In the left-hand menu under **CSP** , choose **Azure spending** .</span></span>

3. <span data-ttu-id="de66d-143">**Azure harcama** sayfasında, **Microsoft Azure abonelikleri olan müşteriler** altında, bütçesini kaldırmak istediğiniz müşteri (ler) i seçin.</span><span class="sxs-lookup"><span data-stu-id="de66d-143">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions** , select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="de66d-144">**Bütçeyi Kaldır** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="de66d-144">Choose **Remove budget** .</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="de66d-145">Geçerli Azure harcamayı denetle</span><span class="sxs-lookup"><span data-stu-id="de66d-145">Check current Azure spending</span></span>

<span data-ttu-id="de66d-146">*Müşterilerinizin geçerli Azure harcamalarını ve aylık bütçelerinin* dilediğiniz zaman izlenmesini sağlayabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="de66d-146">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="de66d-147">[Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="de66d-147">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="de66d-148">**CSP** altındaki sol menüde **Azure harcama** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="de66d-148">In the left-hand menu under **CSP** , choose **Azure spending** .</span></span>

3. <span data-ttu-id="de66d-149">**Azure harcama** sayfasında, **Microsoft Azure abonelikleri olan müşteriler** altında müşterilerin aylık bütçeleri, geçerli harcama tahminleri ve kullanılan bütçenin yüzdesi hakkında bir genel bakış görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="de66d-149">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions** , you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="de66d-150">Bütçe limitlerinin bildirimleri</span><span class="sxs-lookup"><span data-stu-id="de66d-150">Notifications for budget limits</span></span>

<span data-ttu-id="de66d-151">Müşterinizin aylık harcama süresi Bütçe limitine yaklaştığı zaman için *e-posta bildirimlerini açabilirsiniz* .</span><span class="sxs-lookup"><span data-stu-id="de66d-151">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="de66d-152">Bu seçeneği etkinleştirdiğinizde, müşteriler aylık bütçesinden %80 veya daha fazlasını kullandıklarında bildirim alırsınız.</span><span class="sxs-lookup"><span data-stu-id="de66d-152">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="de66d-153">Bu seçenek, Azure faturanızda bir göz kalmanıza yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="de66d-153">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="de66d-154">E-posta bildirimlerini yapılandırmak için:</span><span class="sxs-lookup"><span data-stu-id="de66d-154">To configure email notifications:</span></span>

1. <span data-ttu-id="de66d-155">İş Ortağı Merkezi'nde oturum açın.</span><span class="sxs-lookup"><span data-stu-id="de66d-155">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="de66d-156">**CSP** altındaki sol menüde **Azure harcama** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="de66d-156">In the left-hand menu under **CSP** , choose **Azure spending** .</span></span>

3. <span data-ttu-id="de66d-157">**Azure harcama** sayfasında, **e-posta bildirimleri** ' nin altında, e **-postaları al** ayarını **Açık** olarak değiştirin.</span><span class="sxs-lookup"><span data-stu-id="de66d-157">On the **Azure spending** page, under **Email notifications** , toggle the **Get emails** setting to **On** .</span></span>

4. <span data-ttu-id="de66d-158">Bildirimlerin e-posta adresini görmek için **e-posta adresini değiştir** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="de66d-158">Choose **Change email address** to see the email address for notifications.</span></span>

5. <span data-ttu-id="de66d-159">E-posta adresi *doğru değilse* , doğru e-posta adresini girip **Güncelleştir** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="de66d-159">If the email address *isn't correct* , enter the correct email address and choose **Update** .</span></span> <span data-ttu-id="de66d-160">E-posta adresi *doğruysa* **iptal** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="de66d-160">If the email address *is correct* , choose **Cancel** .</span></span>

## <a name="itemized-costs-by-service"></a><span data-ttu-id="de66d-161">Hizmete göre listelenen maliyetler</span><span class="sxs-lookup"><span data-stu-id="de66d-161">Itemized costs by service</span></span>

<span data-ttu-id="de66d-162">*Kullanım tabanlı abonelikler için, hizmete göre listelenen maliyeti (ve tahmini kullanımı)* görebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="de66d-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions* :</span></span>

1. <span data-ttu-id="de66d-163">İş Ortağı Merkezi'nde oturum açın.</span><span class="sxs-lookup"><span data-stu-id="de66d-163">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="de66d-164">**CSP** altındaki sol menüde **müşteriler** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="de66d-164">In the left-hand menu under **CSP** , choose **Customers** .</span></span>

3. <span data-ttu-id="de66d-165">**Müşteriler** sayfasında, müşterinin **şirket adını** seçin.</span><span class="sxs-lookup"><span data-stu-id="de66d-165">On the **Customers** page, select the customer's **Company name** .</span></span>

4. <span data-ttu-id="de66d-166">Müşterinin **abonelikler** sayfasında, **Kullanım tabanlı abonelikler** ' in altında, **aboneliğin** adını seçin.</span><span class="sxs-lookup"><span data-stu-id="de66d-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions** , select the name of the **Subscription** .</span></span>

5. <span data-ttu-id="de66d-167">Aboneliğin sayfasında, hizmete göre **listelenen maliyeti** ve geçerli ay için **Tahmini kullanımı** gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="de66d-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>
