---
title: Azure plan faturalandırma-fatura & keşfi dosyaları
ms.topic: article
ms.date: 01/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure planına yönelik faturalandırma ile ilgili fatura ve mutabakat dosya yapısına erişme ve bunları anlama hakkında bilgi edinin.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 757383ee264e58e7b4dc8ffefafe213cb49acb79
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149800"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="ce076-103">CSP'de yeni ticari deneyim - Azure faturalama</span><span class="sxs-lookup"><span data-stu-id="ce076-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="ce076-104">**Uygun roller**: yönetici Aracısı | Faturalandırma Yöneticisi | Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="ce076-104">**Appropriate roles**: Admin agent | Billing admin | Global admin</span></span>

<span data-ttu-id="ce076-105">Bu makalede, Azure planına yönelik faturalandırma ile ilgili fatura ve mutabakat dosya yapısına nasıl erişebileceğiniz ve anlayabileceğiniz açıklanır.</span><span class="sxs-lookup"><span data-stu-id="ce076-105">This article explains how to access and understand the invoice and reconciliation file structure related to billing for the Azure plan.</span></span> <span data-ttu-id="ce076-106">Azure planı altında faturalandırma, hizalanmış bir tek faturalandırma tarihi ve takvim ay tabanlı fatura dönemi kullanan Basitleştirilmiş bir faturalandırma deneyimidir.</span><span class="sxs-lookup"><span data-stu-id="ce076-106">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="ce076-107">Faturalandırma temelleri Özeti</span><span class="sxs-lookup"><span data-stu-id="ce076-107">Summary of billing essentials</span></span>

- <span data-ttu-id="ce076-108">**Fatura tarihi**: fatura ve mutabakat dosyası, 8 (gece yarısı UTC) tarafından iş ortağı merkezi panosunda/API 'de kullanıma sunulacaktır.</span><span class="sxs-lookup"><span data-stu-id="ce076-108">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="ce076-109">**Fatura fatura dönemi**: fatura fatura dönemi, takvim ayına hizalanır, örneğin, 10/1-10/31, 11/1-11/30.</span><span class="sxs-lookup"><span data-stu-id="ce076-109">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="ce076-110">**Ücret Servisi dönemleri**: ücretler takvim ayına hizalanır.</span><span class="sxs-lookup"><span data-stu-id="ce076-110">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="ce076-111">Örneğin, faturalandırılan iş ortağı 10/15 tarihinde bir Azure planı aracılığıyla Azure hizmetleri eklerse ve müşteri Azure hizmetleri 'ni 10/15 ' de kullanmaya başlarsa, faturalandırılan servis dönemi 10/15-10/31 olan müşteri tüketimi için, faturalanan iş ortağı, 11/8 tarihinde fatura/keşfi alır.</span><span class="sxs-lookup"><span data-stu-id="ce076-111">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="ce076-112">12/8 tarihinde oluşturulacak bir sonraki aya ait fatura, 11/1-11/31 servis dönemine yönelik tüm ücretleri içerir.</span><span class="sxs-lookup"><span data-stu-id="ce076-112">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="ce076-113">**Fatura ödeme dönemi**: net 60 gün.</span><span class="sxs-lookup"><span data-stu-id="ce076-113">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="ce076-114">**Fatura para birimi**: 15 Ocak 2021 tarihinden ıtıbaren, AB/EFTA ve Birleşik Krallık bölgesindeki iş ortakları, yeni müşteriler ve mevcut CSP müşterileri, kiracıların 11 Mayıs 2020 ' den önce oluşturulduğu ilk kez yeni ticaret teklifleri satın alarak, iş ortağı konumu para birimi 'nde satın alma işlemleri için faturalandırılır.</span><span class="sxs-lookup"><span data-stu-id="ce076-114">**Invoice currency**: Starting January 28th 2021, partners in the EU/EFTA and UK region who have new customers and existing CSP customers purchasing new commerce offers for the first time whose tenants were created prior to 11 May 2020, will be billed for those purchases in partner location currency.</span></span> <span data-ttu-id="ce076-115">AB/EFTA ve UK bölgesinin dışında bulunan iş ortakları, iş ortağı konumu para birimiyle faturalandırılmaya devam edecektir.</span><span class="sxs-lookup"><span data-stu-id="ce076-115">Partners located outside of the EU/EFTA and UK region will continue to be billed in partner location currency.</span></span>

- <span data-ttu-id="ce076-116">**Partner teşvikleri**: fatura ayının sonundan itibaren ödenen 45 gün.</span><span class="sxs-lookup"><span data-stu-id="ce076-116">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="ce076-117">Faturanız ve mutabakat dosyalarınıza erişin</span><span class="sxs-lookup"><span data-stu-id="ce076-117">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="ce076-118">Bir fatura görüntülemeye hazırsanız şirketinizin genel yönetici veya faturalama yöneticisi bir e-posta alır.</span><span class="sxs-lookup"><span data-stu-id="ce076-118">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span>

<span data-ttu-id="ce076-119">Faturaya ve mutabakat dosyasına erişmek için:</span><span class="sxs-lookup"><span data-stu-id="ce076-119">To access the invoice and reconciliation file:</span></span>

1. <span data-ttu-id="ce076-120">İş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="ce076-120">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="ce076-121">Iş Ortağı Merkezi menüsünde **faturalandırma**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="ce076-121">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="ce076-122">**Yinelenen** ve **tek seferlik** ve ilgilendiğiniz para biriminin sekmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="ce076-122">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

   :::image type="content" source="images/azure/billing3.png" alt-text="ödeme":::

4. <span data-ttu-id="ce076-124">**Fatura** veya **Mutabakat dosyası** seçin.</span><span class="sxs-lookup"><span data-stu-id="ce076-124">Select **Invoice** or **Reconciliation file**.</span></span>  

   <span data-ttu-id="ce076-125">Geçmiş faturaları ve keşfi dosyalarını görüntülemek için, aşağıdaki faturalama geçmişi satırını genişletin.</span><span class="sxs-lookup"><span data-stu-id="ce076-125">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="understanding-usage-data"></a><span data-ttu-id="ce076-126">Kullanım verilerini anlama</span><span class="sxs-lookup"><span data-stu-id="ce076-126">Understanding usage data</span></span> 

1. <span data-ttu-id="ce076-127">Azure planı, kullanım için kök veya üst düzey kapsayıcıdır.</span><span class="sxs-lookup"><span data-stu-id="ce076-127">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="ce076-128">Tüm kullanımlar tek bir Azure planına geri bağlanır.</span><span class="sxs-lookup"><span data-stu-id="ce076-128">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="ce076-129">Bir plan içinde, bir veya daha fazla Azure aboneliği olacaktır.</span><span class="sxs-lookup"><span data-stu-id="ce076-129">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="ce076-130">Bunlar, kaynak yönetimi ve dağıtımı için kullanılan kapsayıcılardır.</span><span class="sxs-lookup"><span data-stu-id="ce076-130">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="ce076-131">Bir abonelik içinde, kaynak grupları grup kaynaklarına ekler.</span><span class="sxs-lookup"><span data-stu-id="ce076-131">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="ce076-132">Her kaynak bir kaynak grubuna dağıtılır.</span><span class="sxs-lookup"><span data-stu-id="ce076-132">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="ce076-133">Kaynak örnekleri, sanal makineler ve depolama hesapları içerir.</span><span class="sxs-lookup"><span data-stu-id="ce076-133">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="ce076-134">Kaynak yayma ölçümleri: ölçümler, bir kaynağın tüketim ölçümleridir ve bir kaynak birden fazla ölçüm için kullanım yayabilir.</span><span class="sxs-lookup"><span data-stu-id="ce076-134">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="ce076-135">Ölçümler, bir ProductID, SKUId ve kullanılabilirlik kimliği ile tanımlanır.</span><span class="sxs-lookup"><span data-stu-id="ce076-135">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="ce076-136">Abonelik kaynak grupları ve ölçüm hiyerarşisi</span><span class="sxs-lookup"><span data-stu-id="ce076-136">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="ce076-137">**Azure hesabı (kiracı)**</span><span class="sxs-lookup"><span data-stu-id="ce076-137">**Azure account (tenant)**</span></span>

- <span data-ttu-id="ce076-138">Abonelik A</span><span class="sxs-lookup"><span data-stu-id="ce076-138">Subscription A</span></span>
    - <span data-ttu-id="ce076-139">ResourceGroup 1</span><span class="sxs-lookup"><span data-stu-id="ce076-139">ResourceGroup 1</span></span>
        - <span data-ttu-id="ce076-140">Sanal makine (kaynak)</span><span class="sxs-lookup"><span data-stu-id="ce076-140">Virtual machine (resource)</span></span>
            - <span data-ttu-id="ce076-141">İşlem ölçümü</span><span class="sxs-lookup"><span data-stu-id="ce076-141">Compute meter</span></span>
        - <span data-ttu-id="ce076-142">Sanal ağ (kaynak)</span><span class="sxs-lookup"><span data-stu-id="ce076-142">Virtual network (resource)</span></span>
            - <span data-ttu-id="ce076-143">Faturalama ölçümü yok</span><span class="sxs-lookup"><span data-stu-id="ce076-143">No billing meter</span></span>

    - <span data-ttu-id="ce076-144">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="ce076-144">ResourceGroup 2</span></span>
        - <span data-ttu-id="ce076-145">Sanal makine (kaynak)</span><span class="sxs-lookup"><span data-stu-id="ce076-145">Virtual machine (resource)</span></span>
            - <span data-ttu-id="ce076-146">Bilgisayar ölçümü</span><span class="sxs-lookup"><span data-stu-id="ce076-146">Computer meter</span></span>
        - <span data-ttu-id="ce076-147">Premium SSD yönetilen disk (kaynak)</span><span class="sxs-lookup"><span data-stu-id="ce076-147">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="ce076-148">Depolama kapasitesi ölçümü</span><span class="sxs-lookup"><span data-stu-id="ce076-148">Storage capacity meter</span></span>
            - <span data-ttu-id="ce076-149">Depolama işlemleri ölçümü</span><span class="sxs-lookup"><span data-stu-id="ce076-149">Storage operations meter</span></span>

- <span data-ttu-id="ce076-150">B Aboneliği -ResourceGroup 1 - Azure SQL (kaynak) - DTU ölçümü - VPN Gateway (kaynak) - VPN ağ geçidi ölçümü</span><span class="sxs-lookup"><span data-stu-id="ce076-150">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="ce076-151">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="ce076-151">ResourceGroup 2</span></span>
        - <span data-ttu-id="ce076-152">Sanal Ağ Arabirimi (kaynak)</span><span class="sxs-lookup"><span data-stu-id="ce076-152">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="ce076-153">Faturalama ölçümü yok</span><span class="sxs-lookup"><span data-stu-id="ce076-153">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="ce076-154">Faturayı okuma</span><span class="sxs-lookup"><span data-stu-id="ce076-154">Read the invoice</span></span>

1. <span data-ttu-id="ce076-155">Fatura her ayın sekizlik günü kadar kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="ce076-155">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="ce076-156">İş ortaklarının ödemelerini geri ödemesi için 60 günü olur.</span><span class="sxs-lookup"><span data-stu-id="ce076-156">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="ce076-157">Faturalama dönemi, 10/1-10/31 gibi bir takvim ayı kapsar.</span><span class="sxs-lookup"><span data-stu-id="ce076-157">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="ce076-158">Ücretler net ayarlamalardır (tutar net olarak "Yönetilen hizmetler için iş ortağı tarafından kazanılmış kredidir").</span><span class="sxs-lookup"><span data-stu-id="ce076-158">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="ce076-159">Ek faturalama ayrıntıları için fatura mutabakat dosyasını ve günlük olarak derecelendirilmiş kullanım dosyasını gözden geçirme.</span><span class="sxs-lookup"><span data-stu-id="ce076-159">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

   :::image type="content" source="images/azure/invoice1.png" alt-text="Fatura":::

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="ce076-161">Fatura mutabakat dosyasını okuma</span><span class="sxs-lookup"><span data-stu-id="ce076-161">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="ce076-162">Her Azure planı ve ölçüm bileşimi, mutabakat dosyasında en fazla iki faturalama satırına sahip olabilir.</span><span class="sxs-lookup"><span data-stu-id="ce076-162">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="ce076-163">Ölçüm, takvim ayı boyunca tüm takvim ayı boyunca herhangi bir türde indirim veya krediye (katmanlı indirimler veya yönetilen hizmetler için İş ortağı tarafından kazanılan kredi gibi) uygunsa mutabakat dosyasında yalnızca bir faturalama satırı vardır.</span><span class="sxs-lookup"><span data-stu-id="ce076-163">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="ce076-164">**PriceAdjusmentDescription sütunu indirime** veya kazanılan krediye başvurur.</span><span class="sxs-lookup"><span data-stu-id="ce076-164">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="ce076-165">İndirim veya iş ortağı tarafından kazanılan kredi için uygun olan belirli bir ölçüm için kaynak yoksa mutabakat dosyasında yalnızca bir faturalama satırı yer alır ve geçerli birim fiyat perakende fiyatı (birim fiyattır) olur.</span><span class="sxs-lookup"><span data-stu-id="ce076-165">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="ce076-166">Ölçüm veya ölçümü yayan herhangi bir kaynak,  ayın bir parçası için yönetilen hizmetler için İş ortağı tarafından kazanılan kredi için uygunsa, mutabakat dosyasında iki faturalama satırı yer alacak.</span><span class="sxs-lookup"><span data-stu-id="ce076-166">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="ce076-167">Bir satır ölçümün uygun olduğu günleri, ikinci satır ise ölçümün uygun olmadığının günlerini temsil edecek.</span><span class="sxs-lookup"><span data-stu-id="ce076-167">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span>

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="ce076-168">Günlük kullanım dosyasını okuma</span><span class="sxs-lookup"><span data-stu-id="ce076-168">Read the daily usage file</span></span>

- <span data-ttu-id="ce076-169">Azure planı kapsamındaki abonelik sayaçları, günlük olarak derecelendirilmiş ve bir şekilde toplanıyor.</span><span class="sxs-lookup"><span data-stu-id="ce076-169">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span>

- <span data-ttu-id="ce076-170">**Yönetilen hizmetler için iş ortağı tarafından kazanılan** kredi, günlük olarak belirlenir ve uygulanır.</span><span class="sxs-lookup"><span data-stu-id="ce076-170">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="ce076-171">Her abonelik ölçümde, tüketimin olduğu ayın her günü için bir satır vardır.</span><span class="sxs-lookup"><span data-stu-id="ce076-171">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="ce076-172">Aşağıdaki örnekte:</span><span class="sxs-lookup"><span data-stu-id="ce076-172">In the example below:</span></span>

  - <span data-ttu-id="ce076-173">**1-7/3** arasında yönetilen hizmetler için İş ortağı tarafından kazanılan kredi için uygun ölçüm (geçerli birim fiyatın perakende fiyatı, iş ortağı tarafından kazanılan krediden daha az olduğunu unutmayın.</span><span class="sxs-lookup"><span data-stu-id="ce076-173">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="ce076-174">Ölçüm, **7/4** - 7/7 arasında yönetilen hizmetler için İş ortağı tarafından kazanılan kredi için uygun değildi (geçerli birim fiyatın perakende fiyatı olduğunu unutmayın).</span><span class="sxs-lookup"><span data-stu-id="ce076-174">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="ce076-175">**7/8** - 7/31 arasında yönetilen hizmetler için İş ortağı tarafından kazanılan kredi için uygun ölçüm (geçerli birim fiyatın perakende fiyatı daha az iş ortağı tarafından kazanılan kredi olduğunu unutmayın).</span><span class="sxs-lookup"><span data-stu-id="ce076-175">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="ce076-177">Müşteri para birimi cinsinden fatura</span><span class="sxs-lookup"><span data-stu-id="ce076-177">Invoice in customer currency</span></span>

<span data-ttu-id="ce076-178">Azure planı aracılığıyla azure hizmetleri ABD doları olarak fiyatlandırılıyor ve müşterinin ülke tarafından atanan para birimi üzerinden faturalandırılıyor.</span><span class="sxs-lookup"><span data-stu-id="ce076-178">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="ce076-179">Faturalama para birimi USD olmayan bir değerse, kullanılan Döviz kuru (FX) oranı faturanın son sayfasında gösterilir.</span><span class="sxs-lookup"><span data-stu-id="ce076-179">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="ce076-180">FX fiyatları aylık olarak belirlenir ve aşağıdaki faturaya uygulanır.</span><span class="sxs-lookup"><span data-stu-id="ce076-180">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="ce076-181">Ülke para birimlerinin tam listesi için lütfen yeni ticari teklifler ülke kullanılabilirliği ve müşteri [para birimi matrisi'ne bakın.](https://go.microsoft.com/fwlink/?linkid=2112354)</span><span class="sxs-lookup"><span data-stu-id="ce076-181">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span>

<span data-ttu-id="ce076-182">Microsoft, dönüştürme için Londra Borsa'yı takip ediyor.</span><span class="sxs-lookup"><span data-stu-id="ce076-182">Microsoft follows the London Stock Exchange for conversion.</span></span> <span data-ttu-id="ce076-183">Londra Borsa'da ayın son iş gününde yakalanan döviz kuruna eşit olan döviz kurlarını kullanıyoruz.</span><span class="sxs-lookup"><span data-stu-id="ce076-183">We use the exchange rate, which is equal to the exchange rate captured on the last second of the last business day of the month on the London Stock Exchange.</span></span> <span data-ttu-id="ce076-184">FX fiyatları, geçerli olduğu ayın ilk gününden önceki gün yenilenir ve kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="ce076-184">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

## <a name="azure-reservations"></a><span data-ttu-id="ce076-185">Azure rezervasyonları</span><span class="sxs-lookup"><span data-stu-id="ce076-185">Azure reservations</span></span>


<span data-ttu-id="ce076-186">Bir [Azure planı aracılığıyla](azure-reservations.md) Azure rezervasyonları satın alırsanız, tek kullanımlık veya aylık faturalamayı seçebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ce076-186">If purchasing [Azure reservations](azure-reservations.md) through an Azure plan, you can choose either one-time or monthly billing.</span></span>


## <a name="azure-spending"></a><span data-ttu-id="ce076-187">Azure harcaması</span><span class="sxs-lookup"><span data-stu-id="ce076-187">Azure spending</span></span>

<span data-ttu-id="ce076-188">Mevcut Azure harcama deneyimi, azure'da yeni Azure planı faturalaması desteği İş Ortağı Merkezi.</span><span class="sxs-lookup"><span data-stu-id="ce076-188">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="ce076-189">Bu, iş ortaklarının şunları sağlar:</span><span class="sxs-lookup"><span data-stu-id="ce076-189">This enables partners to:</span></span>

- <span data-ttu-id="ce076-190">Müşteri düzeyinde ayarlanmış bütçe uyarılarını görüntüleme, yönetme ve alma</span><span class="sxs-lookup"><span data-stu-id="ce076-190">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="ce076-191">Azure planında toplam tahmini harcamayı görüntüleme (kaynağa ve ölçüm düzeyine göre aşağı doğru)</span><span class="sxs-lookup"><span data-stu-id="ce076-191">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="ce076-192">Azure planı aracılığıyla Azure hizmetlerinin faturalama modeli ödeme sonrası tüketim olduğundan, beklenenden daha büyük bir faturayı önlemek için iş ortakları aylık bütçe uygulayabilir ve kullanım yüzdesini izleyebilir.</span><span class="sxs-lookup"><span data-stu-id="ce076-192">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="ce076-193">Bütçe bir defada bir müşteriye veya birden çok müşteriye uygulanabilir.</span><span class="sxs-lookup"><span data-stu-id="ce076-193">A budget can be applied to one customer or multiple customers at one time.</span></span> 

:::image type="content" source="images/azure/azurespend.png" alt-text="Azure harcaması":::

## <a name="next-steps"></a><span data-ttu-id="ce076-195">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="ce076-195">Next steps</span></span>

- <span data-ttu-id="ce076-196">İş ortağı tarafından kazanılan kredinin (PEC) nasıl hesaplanmasına bakın.</span><span class="sxs-lookup"><span data-stu-id="ce076-196">See how the partner earned credit (PEC) is calculated.</span></span> <span data-ttu-id="ce076-197">İş Ortağı Merkezi [oturum](https://partner.microsoft.com/dashboard/) açın ve kullanılabilir fiyat listesini bulun.</span><span class="sxs-lookup"><span data-stu-id="ce076-197">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) and locate the price list available.</span></span>

- <span data-ttu-id="ce076-198">Azure planını [satın alma hakkında bilgi edinin](purchase-azure-plan.md)</span><span class="sxs-lookup"><span data-stu-id="ce076-198">Learn about [purchasing the Azure plan](purchase-azure-plan.md)</span></span>

- <span data-ttu-id="ce076-199">[CSP'de yeni ticaret deneyimi için fiyat listesine bakın](azure-plan-price-list.md)</span><span class="sxs-lookup"><span data-stu-id="ce076-199">See the [price list for the new commerce experience in CSP](azure-plan-price-list.md)</span></span>
