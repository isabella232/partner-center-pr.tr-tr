---
title: Müşteriler için Azure harcama bütçesi ayarlama
ms.topic: how-to
ms.date: 03/17/2021
description: Müşterileriniz için aylık Azure harcama bütçelerini ayarlamayı veya kaldırmayı ve ayrıca Azure harcama verilerini görüntülemeyi ve bütçeye ilişkin bildirimleri ayarlamayı öğrenin.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eaf54898d7a130ca38e5a2aaeba279fb722c9e66
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712758"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="80d35-103">Iş Ortağı Merkezi 'nde müşterilere yönelik aylık Azure harcama bütçelerini ayarlama, denetleme veya kaldırma</span><span class="sxs-lookup"><span data-stu-id="80d35-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="80d35-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="80d35-104">**Appropriate roles**</span></span>

- <span data-ttu-id="80d35-105">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="80d35-105">Admin agent</span></span>

<span data-ttu-id="80d35-106">Iş Ortağı Merkezi 'nde [müşterileriniz için aylık bir Azure harcama bütçesi ayarlayabilirsiniz](#set-azure-spending-budget) .</span><span class="sxs-lookup"><span data-stu-id="80d35-106">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="80d35-107">Bu, müşterilerinizin Azure harcamalarını yönetmesine yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="80d35-107">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="80d35-108">Bu seçenek, müşterilerinizin aylık dönemi boyunca Azure harcamalarınızı bütçenize göre karşılaştırmanızı sağlar.</span><span class="sxs-lookup"><span data-stu-id="80d35-108">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="80d35-109">Ayrıca, müşterilerinizin aylık faturanız düşünenden daha yüksek olmaması için Azure harcamalarını bütçelerinize de yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="80d35-109">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="80d35-110">Bu özellik korumalı alanda veya üretimde test (tıp) hesaplarında kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="80d35-110">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="80d35-111">Müşterilerinizin [Azure harcama bütçesini ayarladıktan](#set-azure-spending-budget)sonra, müşteri kullanımını aşağıdaki yollarla da gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="80d35-111">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="80d35-112">Bu seçenekler, yanlış yapılandırılmış Hizmetleri veya sahtekarlık önereceği olağan dışı eğilimleri belirlemenize yardımcı olabilir.</span><span class="sxs-lookup"><span data-stu-id="80d35-112">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="80d35-113">Bundan sonra, temel nedeni belirlemek ve maliyetleri yönetmek için müşteri (ler) i ile çalışabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="80d35-113">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="80d35-114">Gerekirse, [müşterinin bütçesini](#set-azure-spending-budget) daha yüksek bir tutara de değiştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="80d35-114">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="80d35-115">Geçerli Azure harcamayı denetle</span><span class="sxs-lookup"><span data-stu-id="80d35-115">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="80d35-116">Müşterinin harcama süresi Bütçe limitine yaklaştığı zaman için e-posta bildirimlerini aç</span><span class="sxs-lookup"><span data-stu-id="80d35-116">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="80d35-117">Kullanım tabanlı abonelikler için hizmete göre listelenen maliyetleri görüntüleme</span><span class="sxs-lookup"><span data-stu-id="80d35-117">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="80d35-118">Ayrıca, müşteriler için [bir Azure harcama bütçesini](#remove-azure-spending-budget) dilediğiniz zaman kaldırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="80d35-118">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="80d35-119">Azure harcama verileri</span><span class="sxs-lookup"><span data-stu-id="80d35-119">Azure spending data</span></span>

<span data-ttu-id="80d35-120">Azure harcama verileri bir *tahmindir* ve *gerçek faturalandırma miktarları farklılık* gösterebilir.</span><span class="sxs-lookup"><span data-stu-id="80d35-120">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="80d35-121">Verilerin değeri vergileri, kredilerin, ayarlamaların veya uygulayabilen diğer ücretleri *yansıtmaz* .</span><span class="sxs-lookup"><span data-stu-id="80d35-121">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="80d35-122">Harcama verileri *günde bir kez yenilenir*.</span><span class="sxs-lookup"><span data-stu-id="80d35-122">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="80d35-123">Müşterileriniz, Azure portal hesap ayarlarını değiştirmediğiniz müddetçe Azure hizmetleri ve kaynakları kullanmaya ve ücretlendirmeye devam edebilir.</span><span class="sxs-lookup"><span data-stu-id="80d35-123">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="80d35-124">Azure harcama bütçesini ayarlama</span><span class="sxs-lookup"><span data-stu-id="80d35-124">Set Azure spending budget</span></span>

<span data-ttu-id="80d35-125">Iş Ortağı Merkezi 'nde birden çok müşteri için *aylık bir Azure harcama bütçesi ayarlayabilirsiniz* :</span><span class="sxs-lookup"><span data-stu-id="80d35-125">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="80d35-126">[İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="80d35-126">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="80d35-127">**CSP** altındaki sol menüde **Azure harcama**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="80d35-127">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="80d35-128">**Azure harcama** sayfasında, **Microsoft Azure abonelikleri olan müşteriler** altında, bütçesini ayarlamak istediğiniz müşteri (ler) i seçin.</span><span class="sxs-lookup"><span data-stu-id="80d35-128">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="80d35-129">**Aylık bütçe** için bir değer girin.</span><span class="sxs-lookup"><span data-stu-id="80d35-129">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="80d35-130">Değişikliklerinizi kaydetmek için **Uygula** ' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="80d35-130">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="80d35-131">Ayrıca, abonelik ayarlarında *tek bir müşteri için bir bütçe ayarlayabilirsiniz* :</span><span class="sxs-lookup"><span data-stu-id="80d35-131">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="80d35-132">İş Ortağı Merkezi panosunda oturum açın.</span><span class="sxs-lookup"><span data-stu-id="80d35-132">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="80d35-133">**CSP** altındaki sol menüde **müşteriler**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="80d35-133">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="80d35-134">**Müşteriler** sayfasında, müşterinin **şirket adını** seçin.</span><span class="sxs-lookup"><span data-stu-id="80d35-134">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="80d35-135">Müşterinin **abonelikler** sayfasında, **Kullanım tabanlı abonelik**' ın altında, **bütçeyi Değiştir**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="80d35-135">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="80d35-136">Bütçe için bir değer girin.</span><span class="sxs-lookup"><span data-stu-id="80d35-136">Enter a value for the budget.</span></span>

6. <span data-ttu-id="80d35-137">Değişikliklerinizi kaydetmek için **Uygula** ' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="80d35-137">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="80d35-138">Azure harcama bütçesini kaldırma</span><span class="sxs-lookup"><span data-stu-id="80d35-138">Remove Azure spending budget</span></span>

<span data-ttu-id="80d35-139">Iş Ortağı Merkezi 'nde müşteri (ler) için *aylık bir Azure harcama bütçesini kaldırabilirsiniz* :</span><span class="sxs-lookup"><span data-stu-id="80d35-139">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="80d35-140">[İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="80d35-140">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="80d35-141">**CSP** altındaki sol menüde **Azure harcama**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="80d35-141">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="80d35-142">**Azure harcama** sayfasında, **Microsoft Azure abonelikleri olan müşteriler** altında, bütçesini kaldırmak istediğiniz müşteri (ler) i seçin.</span><span class="sxs-lookup"><span data-stu-id="80d35-142">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="80d35-143">**Bütçeyi Kaldır**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="80d35-143">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="80d35-144">Geçerli Azure harcamayı denetle</span><span class="sxs-lookup"><span data-stu-id="80d35-144">Check current Azure spending</span></span>

<span data-ttu-id="80d35-145">*Müşterilerinizin geçerli Azure harcamalarını ve aylık bütçelerinin* dilediğiniz zaman izlenmesini sağlayabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="80d35-145">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="80d35-146">[İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="80d35-146">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="80d35-147">**CSP** altındaki sol menüde **Azure harcama**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="80d35-147">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="80d35-148">**Azure harcama** sayfasında, **Microsoft Azure abonelikleri olan müşteriler** altında müşterilerin aylık bütçeleri, geçerli harcama tahminleri ve kullanılan bütçenin yüzdesi hakkında bir genel bakış görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="80d35-148">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="80d35-149">Bütçe limitlerinin bildirimleri</span><span class="sxs-lookup"><span data-stu-id="80d35-149">Notifications for budget limits</span></span>

<span data-ttu-id="80d35-150">Müşterinizin aylık harcama süresi Bütçe limitine yaklaştığı zaman için *e-posta bildirimlerini açabilirsiniz* .</span><span class="sxs-lookup"><span data-stu-id="80d35-150">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="80d35-151">Bu seçeneği etkinleştirdiğinizde, müşteriler aylık bütçesinden %80 veya daha fazlasını kullandıklarında bildirim alırsınız.</span><span class="sxs-lookup"><span data-stu-id="80d35-151">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="80d35-152">Bu seçenek, Azure faturanızda bir göz kalmanıza yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="80d35-152">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="80d35-153">E-posta bildirimlerini yapılandırmak için:</span><span class="sxs-lookup"><span data-stu-id="80d35-153">To configure email notifications:</span></span>

1. <span data-ttu-id="80d35-154">İş Ortağı Merkezi'nde oturum açın.</span><span class="sxs-lookup"><span data-stu-id="80d35-154">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="80d35-155">**Ayarlar**' a gidin.</span><span class="sxs-lookup"><span data-stu-id="80d35-155">Go to **Settings**.</span></span>

3. <span data-ttu-id="80d35-156">**Tercihlerimi** seçin.</span><span class="sxs-lookup"><span data-stu-id="80d35-156">Select **My preferences**.</span></span>

4. <span data-ttu-id="80d35-157">Yapmadıysanız tercih edilen e-posta adresini yapılandırın.</span><span class="sxs-lookup"><span data-stu-id="80d35-157">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="80d35-158">Bildirim için tercih edilen dili yapılandırın.</span><span class="sxs-lookup"><span data-stu-id="80d35-158">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="80d35-159">**Bildirim tercihleri** bölümünde **CSP** sekmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="80d35-159">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="80d35-160">**Azure harcama** bildirimi Için e-posta seçeneğini Işaretleyin ve **kaydedin**.</span><span class="sxs-lookup"><span data-stu-id="80d35-160">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="80d35-161">Hizmete göre listelenen maliyetler</span><span class="sxs-lookup"><span data-stu-id="80d35-161">Itemized costs by service</span></span>

<span data-ttu-id="80d35-162">*Kullanım tabanlı abonelikler için, hizmete göre listelenen maliyeti (ve tahmini kullanımı)* görebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="80d35-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="80d35-163">İş Ortağı Merkezi'nde oturum açın.</span><span class="sxs-lookup"><span data-stu-id="80d35-163">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="80d35-164">**CSP** altındaki sol menüde **müşteriler**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="80d35-164">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="80d35-165">**Müşteriler** sayfasında, müşterinin **şirket adını** seçin.</span><span class="sxs-lookup"><span data-stu-id="80d35-165">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="80d35-166">Müşterinin **abonelikler** sayfasında, **Kullanım tabanlı abonelikler**' in altında, **aboneliğin** adını seçin.</span><span class="sxs-lookup"><span data-stu-id="80d35-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="80d35-167">Aboneliğin sayfasında, hizmete göre **listelenen maliyeti** ve geçerli ay için **Tahmini kullanımı** gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="80d35-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="80d35-168">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="80d35-168">Next steps</span></span>

- [<span data-ttu-id="80d35-169">CSP'de yeni ticari deneyim - Azure faturalama</span><span class="sxs-lookup"><span data-stu-id="80d35-169">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
