---
title: Müşteriler için Azure harcama bütçesi ayarlama
ms.topic: how-to
ms.date: 03/17/2021
description: Müşterileriniz için aylık Azure harcama bütçeleri ayarlamayı veya kaldırmayı ve ayrıca Azure harcama verilerini görüntülemeyi ve bütçeyle ilgili bildirimleri ayarlamayı öğrenin.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14e901f51841e58b28a3cbbb1b7a19ce89d7c324
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855361"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="6e65c-103">Azure'daki müşteriler için aylık Azure harcama bütçelerini ayarlama, denetleme veya İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="6e65c-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="6e65c-104">**Uygun roller:** Yönetici aracısı</span><span class="sxs-lookup"><span data-stu-id="6e65c-104">**Appropriate roles**: Admin agent</span></span>

<span data-ttu-id="6e65c-105">[Azure'da müşterileriniz için aylık Bir Azure harcama bütçesi](#set-azure-spending-budget) İş Ortağı Merkezi.</span><span class="sxs-lookup"><span data-stu-id="6e65c-105">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="6e65c-106">Bu, müşterilerinize Azure harcamalarını yönetmeye yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="6e65c-106">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="6e65c-107">Bu seçenek, müşterinizin Azure harcamalarını ay boyunca bütçeyle karşılaştırmanızı sağlar.</span><span class="sxs-lookup"><span data-stu-id="6e65c-107">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="6e65c-108">Ayrıca, müşterilerin aylık faturalarının beklenenden yüksek olması için Azure harcamaları için bütçelerini düzenlemelerine de yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="6e65c-108">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="6e65c-109">Bu özellik korumalı alan veya Üretimde Test (TIP) hesaplarında kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="6e65c-109">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="6e65c-110">Müşteriniz [için bir Azure harcama bütçesi ayardikten](#set-azure-spending-budget)sonra, aşağıdaki yollarla müşteri kullanımını da gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6e65c-110">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="6e65c-111">Bu seçenekler yanlış yapılandırılmış hizmetleri veya sahtekarlık öneren olağan dışı eğilimleri tespit etmeye yardımcı olabilir.</span><span class="sxs-lookup"><span data-stu-id="6e65c-111">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="6e65c-112">Daha sonra kök nedeni belirlemek ve maliyetleri yönetmek için müşterileriyle çalışabileceksiniz.</span><span class="sxs-lookup"><span data-stu-id="6e65c-112">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="6e65c-113">Gerekirse müşterinin bütçesini [daha yüksek bir miktarla](#set-azure-spending-budget) da değiştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6e65c-113">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="6e65c-114">Geçerli Azure harcamalarını denetleme</span><span class="sxs-lookup"><span data-stu-id="6e65c-114">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="6e65c-115">Müşterinin harcaması bütçe sınırına yaklaşıyorsa e-posta bildirimlerini açma</span><span class="sxs-lookup"><span data-stu-id="6e65c-115">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="6e65c-116">Kullanım tabanlı abonelikler için hizmete göre maddeleştirilmiş maliyetleri görüntüleme</span><span class="sxs-lookup"><span data-stu-id="6e65c-116">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="6e65c-117">Ayrıca, [müşteriler için azure harcama](#remove-azure-spending-budget) bütçesini istediğiniz zaman kaldırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6e65c-117">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="6e65c-118">Azure harcama verileri</span><span class="sxs-lookup"><span data-stu-id="6e65c-118">Azure spending data</span></span>

<span data-ttu-id="6e65c-119">Azure harcama verileri bir *tahmindir ve* *gerçek faturalama tutarları değişiklik gösterebilir.*</span><span class="sxs-lookup"><span data-stu-id="6e65c-119">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="6e65c-120">Verilerin değeri *vergileri, kredileri,* düzeltmeleri veya uygulanabilecek diğer ücretleri yansıtmaz.</span><span class="sxs-lookup"><span data-stu-id="6e65c-120">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="6e65c-121">Harcama verileri günde *bir kez yenilenir.*</span><span class="sxs-lookup"><span data-stu-id="6e65c-121">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="6e65c-122">Müşterileriniz, Azure portal hesap ayarlarını değiştirmediğiniz müddetçe Azure hizmetleri ve kaynakları kullanmaya ve ücretlendirmeye devam edebilir.</span><span class="sxs-lookup"><span data-stu-id="6e65c-122">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="6e65c-123">Azure harcama bütçesini ayarlama</span><span class="sxs-lookup"><span data-stu-id="6e65c-123">Set Azure spending budget</span></span>

<span data-ttu-id="6e65c-124">Iş Ortağı Merkezi 'nde birden çok müşteri için *aylık bir Azure harcama bütçesi ayarlayabilirsiniz* :</span><span class="sxs-lookup"><span data-stu-id="6e65c-124">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="6e65c-125">[İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="6e65c-125">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="6e65c-126">**CSP** altındaki sol menüde **Azure harcama**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="6e65c-126">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="6e65c-127">**Azure harcama** sayfasında, **Microsoft Azure abonelikleri olan müşteriler** altında, bütçesini ayarlamak istediğiniz müşteri (ler) i seçin.</span><span class="sxs-lookup"><span data-stu-id="6e65c-127">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="6e65c-128">**Aylık bütçe** için bir değer girin.</span><span class="sxs-lookup"><span data-stu-id="6e65c-128">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="6e65c-129">Değişikliklerinizi kaydetmek için **Uygula** ' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="6e65c-129">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="6e65c-130">Ayrıca, abonelik ayarlarında *tek bir müşteri için bir bütçe ayarlayabilirsiniz* :</span><span class="sxs-lookup"><span data-stu-id="6e65c-130">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="6e65c-131">İş Ortağı Merkezi panosunda oturum açın.</span><span class="sxs-lookup"><span data-stu-id="6e65c-131">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="6e65c-132">**CSP** altındaki sol menüde **müşteriler**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="6e65c-132">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="6e65c-133">**Müşteriler** sayfasında, müşterinin **şirket adını** seçin.</span><span class="sxs-lookup"><span data-stu-id="6e65c-133">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="6e65c-134">Müşterinin **abonelikler** sayfasında, **Kullanım tabanlı abonelik**' ın altında, **bütçeyi Değiştir**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="6e65c-134">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="6e65c-135">Bütçe için bir değer girin.</span><span class="sxs-lookup"><span data-stu-id="6e65c-135">Enter a value for the budget.</span></span>

6. <span data-ttu-id="6e65c-136">Değişikliklerinizi kaydetmek için **Uygula** ' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="6e65c-136">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="6e65c-137">Azure harcama bütçesini kaldırma</span><span class="sxs-lookup"><span data-stu-id="6e65c-137">Remove Azure spending budget</span></span>

<span data-ttu-id="6e65c-138">Iş Ortağı Merkezi 'nde müşteri (ler) için *aylık bir Azure harcama bütçesini kaldırabilirsiniz* :</span><span class="sxs-lookup"><span data-stu-id="6e65c-138">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="6e65c-139">[İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="6e65c-139">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="6e65c-140">**CSP** altındaki sol menüde **Azure harcama**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="6e65c-140">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="6e65c-141">**Azure harcama** sayfasında, **Microsoft Azure abonelikleri olan müşteriler** altında, bütçesini kaldırmak istediğiniz müşteri (ler) i seçin.</span><span class="sxs-lookup"><span data-stu-id="6e65c-141">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="6e65c-142">**Bütçeyi Kaldır**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="6e65c-142">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="6e65c-143">Geçerli Azure harcamayı denetle</span><span class="sxs-lookup"><span data-stu-id="6e65c-143">Check current Azure spending</span></span>

<span data-ttu-id="6e65c-144">*Müşterilerinizin geçerli Azure harcamalarını ve aylık bütçelerinin* dilediğiniz zaman izlenmesini sağlayabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="6e65c-144">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="6e65c-145">[İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="6e65c-145">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="6e65c-146">**CSP'nin** altındaki sol menüde **Azure harcaması'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="6e65c-146">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="6e65c-147">Azure **harcaması sayfasındaki** Microsoft Azure abonelikleri olan müşteriler altında müşterilerin aylık bütçelerine, geçerli harcama tahminlerine ve kullanılan bütçe yüzdesine genel bir bakış görebilirsiniz. </span><span class="sxs-lookup"><span data-stu-id="6e65c-147">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="6e65c-148">Bütçe sınırları için bildirimler</span><span class="sxs-lookup"><span data-stu-id="6e65c-148">Notifications for budget limits</span></span>

<span data-ttu-id="6e65c-149">Müşterinizin *aylık harcaması bütçe* sınırına yaklaşacaksa e-posta bildirimlerini açabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6e65c-149">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="6e65c-150">Bu seçeneği açsanız, müşteriler aylık bütçelerinin %80'ini veya daha fazlasını kullanıyorsa size bildirilecek.</span><span class="sxs-lookup"><span data-stu-id="6e65c-150">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="6e65c-151">Bu seçenek, Azure faturanızı takip etmek için size yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="6e65c-151">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="6e65c-152">E-posta bildirimlerini yapılandırmak için:</span><span class="sxs-lookup"><span data-stu-id="6e65c-152">To configure email notifications:</span></span>

1. <span data-ttu-id="6e65c-153">İş Ortağı Merkezi'nde oturum açın.</span><span class="sxs-lookup"><span data-stu-id="6e65c-153">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="6e65c-154">**Ayarlar'a gidin.**</span><span class="sxs-lookup"><span data-stu-id="6e65c-154">Go to **Settings**.</span></span>

3. <span data-ttu-id="6e65c-155">**Tercihlerim'i seçin.**</span><span class="sxs-lookup"><span data-stu-id="6e65c-155">Select **My preferences**.</span></span>

4. <span data-ttu-id="6e65c-156">Tercih edilen bir e-posta adresi yapılandırmadısanız.</span><span class="sxs-lookup"><span data-stu-id="6e65c-156">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="6e65c-157">Bildirim için tercih edilen dili yapılandırma.</span><span class="sxs-lookup"><span data-stu-id="6e65c-157">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="6e65c-158">Bildirim **tercihleri bölümünde CSP** **sekmesini** seçin.</span><span class="sxs-lookup"><span data-stu-id="6e65c-158">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="6e65c-159">Azure Harcama bildirimi için **E-posta seçeneğini işaretleyin** ve **Kaydet'i seçin.**</span><span class="sxs-lookup"><span data-stu-id="6e65c-159">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="6e65c-160">Hizmete göre maddeleştirilmiş maliyetler</span><span class="sxs-lookup"><span data-stu-id="6e65c-160">Itemized costs by service</span></span>

<span data-ttu-id="6e65c-161">Kullanım tabanlı *abonelikler için hizmete göre maddeleştirilmiş maliyetleri (ve tahmini kullanımı) görüntüebilirsiniz:*</span><span class="sxs-lookup"><span data-stu-id="6e65c-161">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="6e65c-162">İş Ortağı Merkezi'nde oturum açın.</span><span class="sxs-lookup"><span data-stu-id="6e65c-162">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="6e65c-163">**CSP'nin** altındaki sol menüde Müşteriler'i **seçin.**</span><span class="sxs-lookup"><span data-stu-id="6e65c-163">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="6e65c-164">Müşteriler **sayfasında** müşterinin Şirket adını **seçin.**</span><span class="sxs-lookup"><span data-stu-id="6e65c-164">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="6e65c-165">Müşterinin Abonelikler **sayfasındaki** Kullanım **tabanlı abonelikler** altında Aboneliğin adını **seçin.**</span><span class="sxs-lookup"><span data-stu-id="6e65c-165">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="6e65c-166">Aboneliğin sayfasında Hizmete göre maddeleştirilmiş maliyetleri **ve** geçerli aya yönelik **tahmini kullanımı** gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6e65c-166">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="6e65c-167">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="6e65c-167">Next steps</span></span>

- [<span data-ttu-id="6e65c-168">CSP'de yeni ticari deneyim - Azure faturalama</span><span class="sxs-lookup"><span data-stu-id="6e65c-168">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
