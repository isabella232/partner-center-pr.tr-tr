---
title: Azure plan faturalandırma-fatura & keşfi dosyaları
ms.topic: article
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure planına yönelik faturalandırma ile ilgili fatura ve mutabakat dosya yapısına erişme ve bunları anlama hakkında bilgi edinin.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: c7c06f5ed7b147625afb5020f63ead411ef58fa8
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551529"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="cc23d-103">CSP'de yeni ticari deneyim - Azure faturalama</span><span class="sxs-lookup"><span data-stu-id="cc23d-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="cc23d-104">**Uygun roller**: yönetici Aracısı | Faturalandırma Yöneticisi | Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="cc23d-104">**Appropriate roles**: Admin agent | Billing admin | Global admin</span></span>

<span data-ttu-id="cc23d-105">Bu makalede, Azure planına yönelik faturalandırma ile ilgili fatura ve mutabakat dosya yapısına nasıl erişebileceğiniz ve anlayabileceğiniz açıklanır.</span><span class="sxs-lookup"><span data-stu-id="cc23d-105">This article explains how to access and understand the invoice and reconciliation file structure related to billing for the Azure plan.</span></span> <span data-ttu-id="cc23d-106">Azure planı altında faturalandırma, hizalanmış bir tek faturalandırma tarihi ve takvim ay tabanlı fatura dönemi kullanan Basitleştirilmiş bir faturalandırma deneyimidir.</span><span class="sxs-lookup"><span data-stu-id="cc23d-106">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="cc23d-107">Faturalandırma temelleri Özeti</span><span class="sxs-lookup"><span data-stu-id="cc23d-107">Summary of billing essentials</span></span>

- <span data-ttu-id="cc23d-108">**Fatura tarihi**: fatura ve mutabakat dosyası, 8 (gece yarısı UTC) tarafından iş ortağı merkezi panosunda/API 'de kullanıma sunulacaktır.</span><span class="sxs-lookup"><span data-stu-id="cc23d-108">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="cc23d-109">**Fatura fatura dönemi**: fatura fatura dönemi, takvim ayına hizalanır, örneğin, 10/1-10/31, 11/1-11/30.</span><span class="sxs-lookup"><span data-stu-id="cc23d-109">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="cc23d-110">**Ücret Servisi dönemleri**: ücretler takvim ayına hizalanır.</span><span class="sxs-lookup"><span data-stu-id="cc23d-110">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="cc23d-111">Örneğin, faturalandırılan iş ortağı 10/15 tarihinde bir Azure planı aracılığıyla Azure hizmetleri eklerse ve müşteri Azure hizmetleri 'ni 10/15 ' de kullanmaya başlarsa, faturalandırılan servis dönemi 10/15-10/31 olan müşteri tüketimi için, faturalanan iş ortağı, 11/8 tarihinde fatura/keşfi alır.</span><span class="sxs-lookup"><span data-stu-id="cc23d-111">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="cc23d-112">12/8 tarihinde oluşturulacak bir sonraki aya ait fatura, 11/1-11/31 servis dönemine yönelik tüm ücretleri içerir.</span><span class="sxs-lookup"><span data-stu-id="cc23d-112">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="cc23d-113">**Fatura ödeme dönemi**: net 60 gün.</span><span class="sxs-lookup"><span data-stu-id="cc23d-113">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="cc23d-114">**Fatura para birimi**: 15 Ocak 2021 tarihinden ıtıbaren, AB/EFTA ve Birleşik Krallık bölgesindeki iş ortakları, yeni müşteriler ve mevcut CSP müşterileri, kiracıların 11 Mayıs 2020 ' den önce oluşturulduğu ilk kez yeni ticaret teklifleri satın alarak, iş ortağı konumu para birimi 'nde satın alma işlemleri için faturalandırılır.</span><span class="sxs-lookup"><span data-stu-id="cc23d-114">**Invoice currency**: Starting January 28th 2021, partners in the EU/EFTA and UK region who have new customers and existing CSP customers purchasing new commerce offers for the first time whose tenants were created prior to 11 May 2020, will be billed for those purchases in partner location currency.</span></span> <span data-ttu-id="cc23d-115">AB/EFTA ve UK bölgesinin dışında bulunan iş ortakları, iş ortağı konumu para birimiyle faturalandırılmaya devam edecektir.</span><span class="sxs-lookup"><span data-stu-id="cc23d-115">Partners located outside of the EU/EFTA and UK region will continue to be billed in partner location currency.</span></span>

- <span data-ttu-id="cc23d-116">**Partner teşvikleri**: fatura ayının sonundan itibaren ödenen 45 gün.</span><span class="sxs-lookup"><span data-stu-id="cc23d-116">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="cc23d-117">Faturanız ve mutabakat dosyalarınıza erişin</span><span class="sxs-lookup"><span data-stu-id="cc23d-117">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="cc23d-118">Bir fatura görüntülemeye hazırsanız şirketinizin genel yönetici veya faturalama yöneticisi bir e-posta alır.</span><span class="sxs-lookup"><span data-stu-id="cc23d-118">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span>

<span data-ttu-id="cc23d-119">Faturaya ve mutabakat dosyasına erişmek için:</span><span class="sxs-lookup"><span data-stu-id="cc23d-119">To access the invoice and reconciliation file:</span></span>

1. <span data-ttu-id="cc23d-120">İş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="cc23d-120">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="cc23d-121">Iş Ortağı Merkezi menüsünde **faturalandırma**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="cc23d-121">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="cc23d-122">**Yinelenen** ve **tek seferlik** ve ilgilendiğiniz para biriminin sekmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="cc23d-122">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

   :::image type="content" source="images/azure/billing3.png" alt-text="ödeme.":::

4. <span data-ttu-id="cc23d-124">**Fatura** veya **Mutabakat dosyası** seçin.</span><span class="sxs-lookup"><span data-stu-id="cc23d-124">Select **Invoice** or **Reconciliation file**.</span></span>  

   <span data-ttu-id="cc23d-125">Geçmiş faturaları ve keşfi dosyalarını görüntülemek için, aşağıdaki faturalama geçmişi satırını genişletin.</span><span class="sxs-lookup"><span data-stu-id="cc23d-125">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="understanding-usage-data"></a><span data-ttu-id="cc23d-126">Kullanım verilerini anlama</span><span class="sxs-lookup"><span data-stu-id="cc23d-126">Understanding usage data</span></span> 

1. <span data-ttu-id="cc23d-127">Azure planı, kullanım için kök veya üst düzey kapsayıcıdır.</span><span class="sxs-lookup"><span data-stu-id="cc23d-127">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="cc23d-128">Tüm kullanımlar tek bir Azure planına geri bağlanır.</span><span class="sxs-lookup"><span data-stu-id="cc23d-128">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="cc23d-129">Bir plan içinde, bir veya daha fazla Azure aboneliği olacaktır.</span><span class="sxs-lookup"><span data-stu-id="cc23d-129">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="cc23d-130">Bunlar, kaynak yönetimi ve dağıtımı için kullanılan kapsayıcılardır.</span><span class="sxs-lookup"><span data-stu-id="cc23d-130">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="cc23d-131">Bir abonelik içinde, kaynak grupları grup kaynaklarına ekler.</span><span class="sxs-lookup"><span data-stu-id="cc23d-131">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="cc23d-132">Her kaynak bir kaynak grubuna dağıtılır.</span><span class="sxs-lookup"><span data-stu-id="cc23d-132">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="cc23d-133">Kaynak örnekleri, sanal makineler ve depolama hesapları içerir.</span><span class="sxs-lookup"><span data-stu-id="cc23d-133">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="cc23d-134">Kaynak yayma ölçümleri: ölçümler, bir kaynağın tüketim ölçümleridir ve bir kaynak birden fazla ölçüm için kullanım yayabilir.</span><span class="sxs-lookup"><span data-stu-id="cc23d-134">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="cc23d-135">Ölçümler, bir ProductID, SKUId ve kullanılabilirlik kimliği ile tanımlanır.</span><span class="sxs-lookup"><span data-stu-id="cc23d-135">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="cc23d-136">Abonelik kaynak grupları ve ölçüm hiyerarşisi</span><span class="sxs-lookup"><span data-stu-id="cc23d-136">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="cc23d-137">**Azure hesabı (kiracı)**</span><span class="sxs-lookup"><span data-stu-id="cc23d-137">**Azure account (tenant)**</span></span>

- <span data-ttu-id="cc23d-138">Abonelik A</span><span class="sxs-lookup"><span data-stu-id="cc23d-138">Subscription A</span></span>
    - <span data-ttu-id="cc23d-139">ResourceGroup 1</span><span class="sxs-lookup"><span data-stu-id="cc23d-139">ResourceGroup 1</span></span>
        - <span data-ttu-id="cc23d-140">Sanal makine (kaynak)</span><span class="sxs-lookup"><span data-stu-id="cc23d-140">Virtual machine (resource)</span></span>
            - <span data-ttu-id="cc23d-141">İşlem ölçümü</span><span class="sxs-lookup"><span data-stu-id="cc23d-141">Compute meter</span></span>
        - <span data-ttu-id="cc23d-142">Sanal ağ (kaynak)</span><span class="sxs-lookup"><span data-stu-id="cc23d-142">Virtual network (resource)</span></span>
            - <span data-ttu-id="cc23d-143">Faturalandırma ölçümü yok</span><span class="sxs-lookup"><span data-stu-id="cc23d-143">No billing meter</span></span>

    - <span data-ttu-id="cc23d-144">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="cc23d-144">ResourceGroup 2</span></span>
        - <span data-ttu-id="cc23d-145">Sanal makine (kaynak)</span><span class="sxs-lookup"><span data-stu-id="cc23d-145">Virtual machine (resource)</span></span>
            - <span data-ttu-id="cc23d-146">Bilgisayar ölçer</span><span class="sxs-lookup"><span data-stu-id="cc23d-146">Computer meter</span></span>
        - <span data-ttu-id="cc23d-147">Premium SSD yönetilen disk (kaynak)</span><span class="sxs-lookup"><span data-stu-id="cc23d-147">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="cc23d-148">Depolama kapasitesi ölçümü</span><span class="sxs-lookup"><span data-stu-id="cc23d-148">Storage capacity meter</span></span>
            - <span data-ttu-id="cc23d-149">Depolama işlemleri ölçümü</span><span class="sxs-lookup"><span data-stu-id="cc23d-149">Storage operations meter</span></span>

- <span data-ttu-id="cc23d-150">Abonelik B-ResourceGroup 1-Azure SQL (kaynak)-DTU ölçer-VPN Gateway (kaynak)-VPN ağ geçidi ölçer</span><span class="sxs-lookup"><span data-stu-id="cc23d-150">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="cc23d-151">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="cc23d-151">ResourceGroup 2</span></span>
        - <span data-ttu-id="cc23d-152">Sanal ağ arabirimi (kaynak)</span><span class="sxs-lookup"><span data-stu-id="cc23d-152">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="cc23d-153">Faturalandırma ölçümü yok</span><span class="sxs-lookup"><span data-stu-id="cc23d-153">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="cc23d-154">Faturayı okuyun</span><span class="sxs-lookup"><span data-stu-id="cc23d-154">Read the invoice</span></span>

1. <span data-ttu-id="cc23d-155">Fatura, her ayın sekizinci ' inden daha sonra kullanılabilir olacaktır.</span><span class="sxs-lookup"><span data-stu-id="cc23d-155">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="cc23d-156">İş ortaklarının ödemeye havale etmek için 60 gün vardır.</span><span class="sxs-lookup"><span data-stu-id="cc23d-156">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="cc23d-157">Fatura dönemi belirli bir takvim ayını kapsar. Örneğin, 10/1-10/31.</span><span class="sxs-lookup"><span data-stu-id="cc23d-157">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="cc23d-158">Ücretler, ayarlamaların miktarıdır ("hizmet için Iş ortağı kazanılmış kredinin yüzdesi").</span><span class="sxs-lookup"><span data-stu-id="cc23d-158">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="cc23d-159">Fatura keşfi dosyasını ve günlük derecelendirmeli kullanım dosyasını, ek faturalandırma ayrıntıları için gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="cc23d-159">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

   :::image type="content" source="images/azure/invoice1.png" alt-text="faturalayabilirsiniz.":::

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="cc23d-161">Fatura mutabakatı dosyasını okuyun</span><span class="sxs-lookup"><span data-stu-id="cc23d-161">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="cc23d-162">Her Azure planı ve ölçüm kombinasyonu, keşfi dosyasında en fazla iki faturalandırma satırı olabilir.</span><span class="sxs-lookup"><span data-stu-id="cc23d-162">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="cc23d-163">Ölçüm, tüm takvim ayı boyunca herhangi bir indirim veya kredi türü (katmanlı iskontolar veya hizmet için Iş ortağı için kazanılan kredi gibi) için uygun değilse, keşfi dosyası yalnızca bir faturalandırma satırı içerir.</span><span class="sxs-lookup"><span data-stu-id="cc23d-163">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="cc23d-164">**Priceayarlanmentdescription** sütunu, iskontoya veya kazanılan krediye başvurur.</span><span class="sxs-lookup"><span data-stu-id="cc23d-164">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="cc23d-165">Belirli bir ölçüm için, indirimin veya iş ortağının kazanılmasını karşılayan bir kaynak yoksa, keşfi dosyası yalnızca bir faturalandırma satırı içerir ve geçerli birim fiyatı perakende fiyatı (birim fiyatı) olacaktır.</span><span class="sxs-lookup"><span data-stu-id="cc23d-165">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="cc23d-166">Ölçüm veya bu ölçümü yayan herhangi bir kaynak, ayın bir parçası için **yönetilen hizmet Için Iş ortağı kazanılmış kredi** için uygun olan, keşfi dosyası iki faturalandırma satırı içerecektir.</span><span class="sxs-lookup"><span data-stu-id="cc23d-166">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="cc23d-167">Tek bir satır, ölçüm 'in uygun olmadığı günleri temsil eder ve ikinci satır, ölçümün uygun olmadığı günleri temsil eder.</span><span class="sxs-lookup"><span data-stu-id="cc23d-167">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span>

>[!NOTE]
><span data-ttu-id="cc23d-168">Azure tüketiminizi tek seferlik satın alma keşfi dosyanızda mutabık hale getirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cc23d-168">You can reconcile your Azure consumption in your one-time purchase recon file.</span></span> <span data-ttu-id="cc23d-169">Bunu yapmak için, günlük derecelendirdiğiniz kullanım keşfi dosyasına gidin ve SubscriptionID 'nizi arayın.</span><span class="sxs-lookup"><span data-stu-id="cc23d-169">To do this, go to your daily-rated usage recon file and search for your SubscriptionID.</span></span> <span data-ttu-id="cc23d-170">Bu, Azure plan KIMLIĞINIZLE ilişkili tüm maliyetleri görüntüler.</span><span class="sxs-lookup"><span data-stu-id="cc23d-170">This will display all costs associated with your Azure Plan ID.</span></span> <span data-ttu-id="cc23d-171">Azure SubscriptionID 'niz EntitlementID olarak gösterilir.</span><span class="sxs-lookup"><span data-stu-id="cc23d-171">Your Azure SubscriptionID is shown as the EntitlementID.</span></span>

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="cc23d-172">Günlük kullanım dosyasını okuyun</span><span class="sxs-lookup"><span data-stu-id="cc23d-172">Read the daily usage file</span></span>

- <span data-ttu-id="cc23d-173">Bir Azure planı kapsamındaki abonelik ölçümleri derecelendirilir ve günlük olarak birikmiştir.</span><span class="sxs-lookup"><span data-stu-id="cc23d-173">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span>

- <span data-ttu-id="cc23d-174">**Yönetilen hizmetler Için Iş ortağı kazanılmış kredisi** , günlük olarak belirlenir ve uygulanır.</span><span class="sxs-lookup"><span data-stu-id="cc23d-174">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="cc23d-175">Her abonelik ölçünün, her ay için tüketimin olduğu her gün için bir satır olacaktır.</span><span class="sxs-lookup"><span data-stu-id="cc23d-175">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="cc23d-176">Aşağıdaki örnekte:</span><span class="sxs-lookup"><span data-stu-id="cc23d-176">In the example below:</span></span>

  - <span data-ttu-id="cc23d-177">7/1-7/3 ' dan **yönetilen hizmetler Için Iş ortağı kazanılmış kredi** için uygun ölçüm (etkin birim fiyatının, perakende fiyatı daha az iş ortağı kazanılan kredisi olduğunu aklınızda bulunur.</span><span class="sxs-lookup"><span data-stu-id="cc23d-177">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="cc23d-178">Ölçüm, 7/4-7/7 ' dan **yönetilen hizmetler Için Iş ortağı kazanılmış kredi** için uygun değil (geçerli birim fiyatı perakende fiyatı).</span><span class="sxs-lookup"><span data-stu-id="cc23d-178">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="cc23d-179">7/8-7/31 ' dan **yönetilen hizmetler Için Iş ortağı kazanılmış kredi** için uygun ölçüm (geçerli birim fiyatı, perakende fiyatı daha az iş ortağı kazanılan kredidir).</span><span class="sxs-lookup"><span data-stu-id="cc23d-179">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2.":::

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="cc23d-181">Müşteri para biriminde fatura</span><span class="sxs-lookup"><span data-stu-id="cc23d-181">Invoice in customer currency</span></span>

<span data-ttu-id="cc23d-182">Azure planı aracılığıyla Azure Hizmetleri, ABD Doları cinsinden fiyatlandırılır ve müşterinin ülke atanmış para birimiyle faturalandırılır.</span><span class="sxs-lookup"><span data-stu-id="cc23d-182">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="cc23d-183">Faturalama para birimi ABD dışı ise, kullanılan yabancı Exchange (FX) ücreti faturanın son sayfasında gösterilir.</span><span class="sxs-lookup"><span data-stu-id="cc23d-183">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="cc23d-184">FX ücretleri aylık olarak belirlenir ve aşağıdaki faturaya uygulanır.</span><span class="sxs-lookup"><span data-stu-id="cc23d-184">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="cc23d-185">Ülke para birimlerinin tam listesi için lütfen [Yeni ticaret teklifleri ülke kullanılabilirliği ve müşteri para birimi matrisini](https://go.microsoft.com/fwlink/?linkid=2112354)görüntüleyin.</span><span class="sxs-lookup"><span data-stu-id="cc23d-185">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span>

<span data-ttu-id="cc23d-186">Microsoft, her takvim ayında satın alınan veya tüketilen Azure hizmetleri için tahakkuk eden toplam ücretlere ulaşmak üzere ABD Doları fiyatlarını temel alan önceden tanımlı bir döviz kuru uygular.</span><span class="sxs-lookup"><span data-stu-id="cc23d-186">Microsoft applies a predetermined exchange rate to base USD prices to arrive at total charges incurred for Azure services purchased or consumed each calendar month.</span></span> <span data-ttu-id="cc23d-187">Aylık Döviz Kuru, Thomson depolarında (genellikle), önceki aya ait 4:00 PM GMT 'den önce iki iş günü tarafından yayımlanan orta orandır.</span><span class="sxs-lookup"><span data-stu-id="cc23d-187">The monthly exchange rate is the mid-rate published by Thomson Reuters (typically) two business days prior to the preceding month-end at 4:00 pm GMT.</span></span> 

<span data-ttu-id="cc23d-188">**Örneğin,** Microsoft 'un Aralık değişimi oranı, belirli bir para birimi için, 29 Kasım veya bu yana ABD 'de veya sonrasında Tomson yeniden başlatılıyor.</span><span class="sxs-lookup"><span data-stu-id="cc23d-188">**For example,** Microsoft’s December exchange rate would be the Thomson Reuters mid-rate on or around November 29 for a given currency.</span></span> <span data-ttu-id="cc23d-189">Bu oran, 1 Aralık 'tan 31 Aralık 'a kadar bu para birimindeki tüm satınalmalara uygulanır.</span><span class="sxs-lookup"><span data-stu-id="cc23d-189">That rate will be applied to all purchases in that currency from December 1 to December 31.</span></span> 

## <a name="azure-reservations"></a><span data-ttu-id="cc23d-190">Azure rezervasyonları</span><span class="sxs-lookup"><span data-stu-id="cc23d-190">Azure reservations</span></span>


<span data-ttu-id="cc23d-191">Azure [ayırmaları](azure-reservations.md) bir Azure planıyla satın alıyorsa, tek seferlik veya aylık faturalandırma seçeneklerinden birini belirleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cc23d-191">If purchasing [Azure reservations](azure-reservations.md) through an Azure plan, you can choose either one-time or monthly billing.</span></span>


## <a name="azure-spending"></a><span data-ttu-id="cc23d-192">Azure harcaması</span><span class="sxs-lookup"><span data-stu-id="cc23d-192">Azure spending</span></span>

<span data-ttu-id="cc23d-193">Mevcut Azure harcama deneyimi, Iş Ortağı Merkezi 'nde yeni Azure planı faturalandırmasını destekleyecek şekilde güncelleştirildi.</span><span class="sxs-lookup"><span data-stu-id="cc23d-193">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="cc23d-194">Bu, iş ortaklarının şunları yapmasına olanak sağlar:</span><span class="sxs-lookup"><span data-stu-id="cc23d-194">This enables partners to:</span></span>

- <span data-ttu-id="cc23d-195">Müşteri düzeyinde bütçe kümesi için uyarıları görüntüleyin, yönetin ve alın</span><span class="sxs-lookup"><span data-stu-id="cc23d-195">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="cc23d-196">Bir Azure planında toplam tahmini harcama (kaynak ve ölçüm düzeyine göre ayrılmış) görüntüleyin</span><span class="sxs-lookup"><span data-stu-id="cc23d-196">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="cc23d-197">Azure planı aracılığıyla Azure hizmetleri için faturalandırma modeli, daha büyük bir faturanız beklenenden daha büyük bir fatura olduğundan, iş ortakları aylık bir bütçe uygulayabilir ve kullanım yüzdesini izleyebilir.</span><span class="sxs-lookup"><span data-stu-id="cc23d-197">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="cc23d-198">Bir bütçe, bir kerede bir müşteriye veya birden çok müşteriye uygulanabilir.</span><span class="sxs-lookup"><span data-stu-id="cc23d-198">A budget can be applied to one customer or multiple customers at one time.</span></span> 

:::image type="content" source="images/azure/azurespend.png" alt-text="Azure harcama.":::

## <a name="next-steps"></a><span data-ttu-id="cc23d-200">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="cc23d-200">Next steps</span></span>

- <span data-ttu-id="cc23d-201">İş ortağı tarafından kazanılan kredinin (PEC) nasıl hesaplanmasına bakın.</span><span class="sxs-lookup"><span data-stu-id="cc23d-201">See how the partner earned credit (PEC) is calculated.</span></span> <span data-ttu-id="cc23d-202">Panoda oturum İş Ortağı Merkezi [ve](https://partner.microsoft.com/dashboard/) kullanılabilir fiyat listesini bulun.</span><span class="sxs-lookup"><span data-stu-id="cc23d-202">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) and locate the price list available.</span></span>

- <span data-ttu-id="cc23d-203">Azure planını [satın alma hakkında bilgi edinin](purchase-azure-plan.md)</span><span class="sxs-lookup"><span data-stu-id="cc23d-203">Learn about [purchasing the Azure plan](purchase-azure-plan.md)</span></span>

- <span data-ttu-id="cc23d-204">[CSP'de yeni ticaret deneyimi için fiyat listesine bakın](azure-plan-price-list.md)</span><span class="sxs-lookup"><span data-stu-id="cc23d-204">See the [price list for the new commerce experience in CSP](azure-plan-price-list.md)</span></span>
