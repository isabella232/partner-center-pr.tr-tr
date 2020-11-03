---
title: Azure plan faturalandırma-fatura & keşfi dosyaları
ms.topic: article
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure planına yönelik faturalandırma ile ilgili fatura ve mutabakat dosya yapısına erişme ve bunları anlama hakkında bilgi edinin.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 5d8bb85357d796ae4917faf91c93db8fef4369c2
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/22/2020
ms.locfileid: "92531555"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="f8b8e-103">CSP 'de yeni ticaret deneyimi-Azure Faturalandırma</span><span class="sxs-lookup"><span data-stu-id="f8b8e-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="f8b8e-104">**Uygun roller:**</span><span class="sxs-lookup"><span data-stu-id="f8b8e-104">**Appropriate roles:**</span></span>

- <span data-ttu-id="f8b8e-105">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="f8b8e-105">Admin agent</span></span>
- <span data-ttu-id="f8b8e-106">Faturalama yöneticisi</span><span class="sxs-lookup"><span data-stu-id="f8b8e-106">Billing admin</span></span>
- <span data-ttu-id="f8b8e-107">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="f8b8e-107">Global admin</span></span>

<span data-ttu-id="f8b8e-108">Azure planı altında faturalandırma, hizalanmış bir tek faturalandırma tarihi ve takvim ay tabanlı fatura dönemi kullanan Basitleştirilmiş bir faturalandırma deneyimidir.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-108">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="f8b8e-109">Faturalandırma temelleri Özeti</span><span class="sxs-lookup"><span data-stu-id="f8b8e-109">Summary of billing essentials</span></span>

- <span data-ttu-id="f8b8e-110">**Fatura tarihi** : fatura ve mutabakat dosyası, 8 (gece yarısı UTC) tarafından iş ortağı merkezi panosunda/API 'de kullanıma sunulacaktır.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-110">**Invoice date** : Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="f8b8e-111">**Fatura fatura dönemi** : fatura fatura dönemi, takvim ayına hizalanır, örneğin, 10/1-10/31, 11/1-11/30.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-111">**Invoice billing period** : The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="f8b8e-112">**Ücret Servisi dönemleri** : ücretler takvim ayına hizalanır.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-112">**Charge service periods** : Charges will align to the calendar month.</span></span> <span data-ttu-id="f8b8e-113">Örneğin, faturalandırılan iş ortağı 10/15 tarihinde bir Azure planı aracılığıyla Azure hizmetleri eklerse ve müşteri Azure hizmetleri 'ni 10/15 ' de kullanmaya başlarsa, faturalandırılan servis dönemi 10/15-10/31 olan müşteri tüketimi için, faturalanan iş ortağı, 11/8 tarihinde fatura/keşfi alır.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-113">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="f8b8e-114">12/8 tarihinde oluşturulacak bir sonraki aya ait fatura, 11/1-11/31 servis dönemine yönelik tüm ücretleri içerir.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-114">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="f8b8e-115">**Fatura ödeme dönemi** : net 60 gün.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-115">**Invoice payment term** : Net 60 days.</span></span>

- <span data-ttu-id="f8b8e-116">**Fatura para birimi** : iş ortakları müşterinin countryatanmı para biriminde faturalandırılmaya devam edecektir.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-116">**Invoice currency** : Partners will continue to be billed in the customer's country's assigned currency.</span></span> <span data-ttu-id="f8b8e-117">Örneğin, faturalanmış iş ortağı UK, Norveç ve Almanya 'daki müşterilerle Irlanda 'da ise, faturalandırılan iş ortağı bir GBP, NOK ve Euro/keşfi EUR alır.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-117">For example, if the billed partner is in Ireland with customers in the UK, Norway, and Germany, then the billed partner will receive a GBP, NOK, and EUR invoice/recon.</span></span>

- <span data-ttu-id="f8b8e-118">**Partner teşvikleri** : fatura ayının sonundan itibaren ödenen 45 gün.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-118">**Partner incentives** : Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="f8b8e-119">Faturanız ve mutabakat dosyalarınıza erişin</span><span class="sxs-lookup"><span data-stu-id="f8b8e-119">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="f8b8e-120">Bir fatura görüntülemeye hazırsanız şirketinizin genel yönetici veya faturalama yöneticisi bir e-posta alır.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-120">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span>

<span data-ttu-id="f8b8e-121">Faturaya ve mutabakat dosyasına erişmek için:</span><span class="sxs-lookup"><span data-stu-id="f8b8e-121">To access the invoice and reconciliation file:</span></span>

1. <span data-ttu-id="f8b8e-122">Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard/)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-122">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="f8b8e-123">Iş Ortağı Merkezi menüsünde **faturalandırma** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-123">From the Partner Center menu, select **Billing** .</span></span>

3. <span data-ttu-id="f8b8e-124">**Yinelenen** ve **tek seferlik** ve ilgilendiğiniz para biriminin sekmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-124">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

   :::image type="content" source="images/azure/billing3.png" alt-text="ödeme":::

4. <span data-ttu-id="f8b8e-126">**Fatura** veya **Mutabakat dosyası** seçin.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-126">Select **Invoice** or **Reconciliation file** .</span></span>  

   <span data-ttu-id="f8b8e-127">Geçmiş faturaları ve keşfi dosyalarını görüntülemek için, aşağıdaki faturalama geçmişi satırını genişletin.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-127">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="understanding-usage-data"></a><span data-ttu-id="f8b8e-128">Kullanım verilerini anlama</span><span class="sxs-lookup"><span data-stu-id="f8b8e-128">Understanding usage data</span></span> 

1. <span data-ttu-id="f8b8e-129">Azure planı, kullanım için kök veya üst düzey kapsayıcıdır.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-129">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="f8b8e-130">Tüm kullanımlar tek bir Azure planına geri bağlanır.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-130">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="f8b8e-131">Bir plan içinde, bir veya daha fazla Azure aboneliği olacaktır.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-131">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="f8b8e-132">Bunlar, kaynak yönetimi ve dağıtımı için kullanılan kapsayıcılardır.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-132">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="f8b8e-133">Bir abonelik içinde, kaynak grupları grup kaynaklarına ekler.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-133">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="f8b8e-134">Her kaynak bir kaynak grubuna dağıtılır.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-134">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="f8b8e-135">Kaynak örnekleri, sanal makineler ve depolama hesapları içerir.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-135">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="f8b8e-136">Kaynak yayma ölçümleri: ölçümler, bir kaynağın tüketim ölçümleridir ve bir kaynak birden fazla ölçüm için kullanım yayabilir.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-136">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="f8b8e-137">Ölçümler, bir ProductID, SKUId ve kullanılabilirlik kimliği ile tanımlanır.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-137">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="f8b8e-138">Abonelik kaynak grupları ve ölçüm hiyerarşisi</span><span class="sxs-lookup"><span data-stu-id="f8b8e-138">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="f8b8e-139">**Azure hesabı (kiracı)**</span><span class="sxs-lookup"><span data-stu-id="f8b8e-139">**Azure account (tenant)**</span></span>

- <span data-ttu-id="f8b8e-140">Abonelik A</span><span class="sxs-lookup"><span data-stu-id="f8b8e-140">Subscription A</span></span>
    - <span data-ttu-id="f8b8e-141">ResourceGroup 1</span><span class="sxs-lookup"><span data-stu-id="f8b8e-141">ResourceGroup 1</span></span>
        - <span data-ttu-id="f8b8e-142">Sanal makine (kaynak)</span><span class="sxs-lookup"><span data-stu-id="f8b8e-142">Virtual machine (resource)</span></span>
            - <span data-ttu-id="f8b8e-143">İşlem ölçümü</span><span class="sxs-lookup"><span data-stu-id="f8b8e-143">Compute meter</span></span>
        - <span data-ttu-id="f8b8e-144">Sanal ağ (kaynak)</span><span class="sxs-lookup"><span data-stu-id="f8b8e-144">Virtual network (resource)</span></span>
            - <span data-ttu-id="f8b8e-145">Faturalandırma ölçümü yok</span><span class="sxs-lookup"><span data-stu-id="f8b8e-145">No billing meter</span></span>

    - <span data-ttu-id="f8b8e-146">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="f8b8e-146">ResourceGroup 2</span></span>
        - <span data-ttu-id="f8b8e-147">Sanal makine (kaynak)</span><span class="sxs-lookup"><span data-stu-id="f8b8e-147">Virtual machine (resource)</span></span>
            - <span data-ttu-id="f8b8e-148">Bilgisayar ölçer</span><span class="sxs-lookup"><span data-stu-id="f8b8e-148">Computer meter</span></span>
        - <span data-ttu-id="f8b8e-149">Premium SSD yönetilen disk (kaynak)</span><span class="sxs-lookup"><span data-stu-id="f8b8e-149">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="f8b8e-150">Depolama kapasitesi ölçümü</span><span class="sxs-lookup"><span data-stu-id="f8b8e-150">Storage capacity meter</span></span>
            - <span data-ttu-id="f8b8e-151">Depolama işlemleri ölçümü</span><span class="sxs-lookup"><span data-stu-id="f8b8e-151">Storage operations meter</span></span>

- <span data-ttu-id="f8b8e-152">Abonelik B-ResourceGroup 1-Azure SQL (kaynak)-DTU ölçer-VPN Gateway (kaynak)-VPN ağ geçidi ölçer</span><span class="sxs-lookup"><span data-stu-id="f8b8e-152">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="f8b8e-153">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="f8b8e-153">ResourceGroup 2</span></span>
        - <span data-ttu-id="f8b8e-154">Sanal ağ arabirimi (kaynak)</span><span class="sxs-lookup"><span data-stu-id="f8b8e-154">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="f8b8e-155">Faturalandırma ölçümü yok</span><span class="sxs-lookup"><span data-stu-id="f8b8e-155">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="f8b8e-156">Faturayı okuyun</span><span class="sxs-lookup"><span data-stu-id="f8b8e-156">Read the invoice</span></span>

1. <span data-ttu-id="f8b8e-157">Fatura, her ayın sekizinci ' inden daha sonra kullanılabilir olacaktır.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-157">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="f8b8e-158">İş ortaklarının ödemeye havale etmek için 60 gün vardır.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-158">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="f8b8e-159">Fatura dönemi belirli bir takvim ayını kapsar. Örneğin, 10/1-10/31.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-159">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="f8b8e-160">Ücretler, ayarlamaların miktarıdır ("hizmet için Iş ortağı kazanılmış kredinin yüzdesi").</span><span class="sxs-lookup"><span data-stu-id="f8b8e-160">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="f8b8e-161">Fatura keşfi dosyasını ve günlük derecelendirmeli kullanım dosyasını, ek faturalandırma ayrıntıları için gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-161">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

   :::image type="content" source="images/azure/invoice1.png" alt-text="faturalayabilirsiniz":::

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="f8b8e-163">Fatura mutabakatı dosyasını okuyun</span><span class="sxs-lookup"><span data-stu-id="f8b8e-163">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="f8b8e-164">Her Azure planı ve ölçüm kombinasyonu, keşfi dosyasında en fazla iki faturalandırma satırı olabilir.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-164">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="f8b8e-165">Ölçüm, tüm takvim ayı boyunca herhangi bir indirim veya kredi türü (katmanlı iskontolar veya hizmet için Iş ortağı için kazanılan kredi gibi) için uygun değilse, keşfi dosyası yalnızca bir faturalandırma satırı içerir.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-165">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="f8b8e-166">**Priceayarlanmentdescription** sütunu, iskontoya veya kazanılan krediye başvurur.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-166">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="f8b8e-167">Belirli bir ölçüm için, indirimin veya iş ortağının kazanılmasını karşılayan bir kaynak yoksa, keşfi dosyası yalnızca bir faturalandırma satırı içerir ve geçerli birim fiyatı perakende fiyatı (birim fiyatı) olacaktır.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-167">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="f8b8e-168">Ölçüm veya bu ölçümü yayan herhangi bir kaynak, ayın bir parçası için **yönetilen hizmet Için Iş ortağı kazanılmış kredi** için uygun olan, keşfi dosyası iki faturalandırma satırı içerecektir.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-168">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="f8b8e-169">Tek bir satır, ölçüm 'in uygun olmadığı günleri temsil eder ve ikinci satır, ölçümün uygun olmadığı günleri temsil eder.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-169">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span>

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="f8b8e-170">Günlük kullanım dosyasını okuyun</span><span class="sxs-lookup"><span data-stu-id="f8b8e-170">Read the daily usage file</span></span>

- <span data-ttu-id="f8b8e-171">Bir Azure planı kapsamındaki abonelik ölçümleri derecelendirilir ve günlük olarak birikmiştir.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-171">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span>

- <span data-ttu-id="f8b8e-172">**Yönetilen hizmetler Için Iş ortağı kazanılmış kredisi** , günlük olarak belirlenir ve uygulanır.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-172">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="f8b8e-173">Her abonelik ölçünün, her ay için tüketimin olduğu her gün için bir satır olacaktır.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-173">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="f8b8e-174">Aşağıdaki örnekte:</span><span class="sxs-lookup"><span data-stu-id="f8b8e-174">In the example below:</span></span>

  - <span data-ttu-id="f8b8e-175">7/1-7/3 ' dan **yönetilen hizmetler Için Iş ortağı kazanılmış kredi** için uygun ölçüm (etkin birim fiyatının, perakende fiyatı daha az iş ortağı kazanılan kredisi olduğunu aklınızda bulunur.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-175">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="f8b8e-176">Ölçüm, 7/4-7/7 ' dan **yönetilen hizmetler Için Iş ortağı kazanılmış kredi** için uygun değil (geçerli birim fiyatı perakende fiyatı).</span><span class="sxs-lookup"><span data-stu-id="f8b8e-176">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="f8b8e-177">7/8-7/31 ' dan **yönetilen hizmetler Için Iş ortağı kazanılmış kredi** için uygun ölçüm (geçerli birim fiyatı, perakende fiyatı daha az iş ortağı kazanılan kredidir).</span><span class="sxs-lookup"><span data-stu-id="f8b8e-177">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="f8b8e-179">Müşteri para biriminde fatura</span><span class="sxs-lookup"><span data-stu-id="f8b8e-179">Invoice in customer currency</span></span>

<span data-ttu-id="f8b8e-180">Azure planı aracılığıyla Azure Hizmetleri, ABD Doları cinsinden fiyatlandırılır ve müşterinin ülke atanmış para birimiyle faturalandırılır.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-180">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="f8b8e-181">Faturalama para birimi ABD dışı ise, kullanılan yabancı Exchange (FX) ücreti faturanın son sayfasında gösterilir.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-181">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="f8b8e-182">FX ücretleri aylık olarak belirlenir ve aşağıdaki faturaya uygulanır.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-182">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="f8b8e-183">Ülke para birimlerinin tam listesi için lütfen [Yeni ticaret teklifleri ülke kullanılabilirliği ve müşteri para birimi matrisini](https://go.microsoft.com/fwlink/?linkid=2112354)görüntüleyin.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-183">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span>

<span data-ttu-id="f8b8e-184">Microsoft, fatura para birimi dönüştürmeye fiyatlandırma para birimini belirlemede kullanılan FX tarifelerinin belirlenmesi için Thomson Rebilgisayarları kullanır.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-184">Microsoft will use Thomson Reuters to determine the FX rates used to determine pricing currency to billing currency conversion.</span></span> <span data-ttu-id="f8b8e-185">FX ücretleri, uygulandıkları ayın ilk günü önce yenilenir ve kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-185">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

<span data-ttu-id="f8b8e-186">**Örnek** : 1 Ağustos 'ta hizmet dönemi için kullanım ücretleri 31 Temmuz TARIHINDE yayınlanan FX ücreti kullanılarak faturalandırılır.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-186">**Example** :  Usage charges for the service period August 1 - August 31 will be billed using the FX rate published on July 31.</span></span> <span data-ttu-id="f8b8e-187">Bu ücretler, Eylül faturasında görüntülenir ve fatura son sayfasında FX fiyatı belirtilir.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-187">These charges will appear on the September invoice and the FX rate will be noted on the last page of the invoice.</span></span>

## <a name="azure-reservations"></a><span data-ttu-id="f8b8e-188">Azure rezervasyonları</span><span class="sxs-lookup"><span data-stu-id="f8b8e-188">Azure reservations</span></span>


<span data-ttu-id="f8b8e-189">Azure [ayırmaları](azure-reservations.md) bir Azure planıyla satın alıyorsa, tek seferlik veya aylık faturalandırma seçeneklerinden birini belirleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-189">If purchasing [Azure reservations](azure-reservations.md) through an Azure plan, you can choose either one-time or monthly billing.</span></span>


## <a name="azure-spending"></a><span data-ttu-id="f8b8e-190">Azure harcaması</span><span class="sxs-lookup"><span data-stu-id="f8b8e-190">Azure spending</span></span>

<span data-ttu-id="f8b8e-191">Mevcut Azure harcama deneyimi, Iş Ortağı Merkezi 'nde yeni Azure planı faturalandırmasını destekleyecek şekilde güncelleştirildi.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-191">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="f8b8e-192">Bu, iş ortaklarının şunları yapmasına olanak sağlar:</span><span class="sxs-lookup"><span data-stu-id="f8b8e-192">This enables partners to:</span></span>

- <span data-ttu-id="f8b8e-193">Müşteri düzeyinde bütçe kümesi için uyarıları görüntüleyin, yönetin ve alın</span><span class="sxs-lookup"><span data-stu-id="f8b8e-193">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="f8b8e-194">Bir Azure planında toplam tahmini harcama (kaynak ve ölçüm düzeyine göre ayrılmış) görüntüleyin</span><span class="sxs-lookup"><span data-stu-id="f8b8e-194">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="f8b8e-195">Azure planı aracılığıyla Azure hizmetleri için faturalandırma modeli, daha büyük bir faturanız beklenenden daha büyük bir fatura olduğundan, iş ortakları aylık bir bütçe uygulayabilir ve kullanım yüzdesini izleyebilir.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-195">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="f8b8e-196">Bir bütçe, bir kerede bir müşteriye veya birden çok müşteriye uygulanabilir.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-196">A budget can be applied to one customer or multiple customers at one time.</span></span> 

:::image type="content" source="images/azure/azurespend.png" alt-text="Azure harcaması":::

## <a name="next-steps"></a><span data-ttu-id="f8b8e-198">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="f8b8e-198">Next steps</span></span>

- <span data-ttu-id="f8b8e-199">Ortağın kazanılan kredisi (PEC) nasıl hesaplanacağını görün.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-199">See how the partner earned credit (PEC) is calculated.</span></span> <span data-ttu-id="f8b8e-200">Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard/) oturum açın ve kullanılabilir fiyat listesini bulun.</span><span class="sxs-lookup"><span data-stu-id="f8b8e-200">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) and locate the price list available.</span></span>

- <span data-ttu-id="f8b8e-201">[Azure planını satın alma](purchase-azure-plan.md) hakkında bilgi edinin</span><span class="sxs-lookup"><span data-stu-id="f8b8e-201">Learn about [purchasing the Azure plan](purchase-azure-plan.md)</span></span>

- <span data-ttu-id="f8b8e-202">[CSP 'de yeni ticaret deneyimi için fiyat listesine](azure-plan-price-list.md) bakın</span><span class="sxs-lookup"><span data-stu-id="f8b8e-202">See the [price list for the new commerce experience in CSP](azure-plan-price-list.md)</span></span>
