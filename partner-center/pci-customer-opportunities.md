---
title: İş Ortağı Merkezi öngörüleri-Cloudadscent eğilimini raporları
description: Iş Ortağı Merkezi 'nde Cloudadscent eğilimini raporları hakkında bilgi edinin. Microsoft ürünlerini satın almak için bir müşterinin eğilimini hakkında bilgiler içerir.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 430aea81964d1b75514b6e1377bd2ba1af41b538
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110153047"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a><span data-ttu-id="82ce4-104">Cloudadscent eğilimini raporları Iş Ortağı Merkezi panosundan kullanılabilir</span><span class="sxs-lookup"><span data-stu-id="82ce4-104">CloudAscent Propensity reports available from Partner Center dashboard</span></span>

<span data-ttu-id="82ce4-105">**Uygun roller**: Executive rapor Görüntüleyici | Rapor Görüntüleyicisi</span><span class="sxs-lookup"><span data-stu-id="82ce4-105">**Appropriate roles**: Executive report viewer | Report viewer</span></span>

<span data-ttu-id="82ce4-106">Iş Ortağı Merkezi panosu, Cloudadscent programından indirilebilir eğilimini verileri sağlar.</span><span class="sxs-lookup"><span data-stu-id="82ce4-106">The Partner Center dashboard provides downloadable propensity data from the CloudAscent program.</span></span> <span data-ttu-id="82ce4-107">Veriler, müşterilerin Microsoft ürünlerini satın alma olasılığını gösterir.</span><span class="sxs-lookup"><span data-stu-id="82ce4-107">The data shows the customers' likelihood to purchase Microsoft products.</span></span>  <span data-ttu-id="82ce4-108">Bu makalede bu verilerin dökümü, Puanlama kullanımı ve ne anlama geldiğini açıklanmaktadır.</span><span class="sxs-lookup"><span data-stu-id="82ce4-108">This article describes the breakdown of this data, how to use the scoring, and what it means.</span></span>

## <a name="summary-definitions"></a><span data-ttu-id="82ce4-109">Özet tanımları</span><span class="sxs-lookup"><span data-stu-id="82ce4-109">Summary definitions</span></span>

- <span data-ttu-id="82ce4-110">**SMC müşterileri**: Bu, eğilimini indirmelerinde bulunan toplam müşteri sayısıdır.</span><span class="sxs-lookup"><span data-stu-id="82ce4-110">**SMC Customers**– This is the total number of customers in the propensity downloads.</span></span>  <span data-ttu-id="82ce4-111">Müşteriler, kayıt ortağı tarafından tanımlanır.</span><span class="sxs-lookup"><span data-stu-id="82ce4-111">Customers are identified by partner of record.</span></span>
- <span data-ttu-id="82ce4-112">**Süresi dolan anlaşmalar**: geçerli mali yıl içinde, süresi dolan sözleşmelerin sayısını sağlıyoruz.</span><span class="sxs-lookup"><span data-stu-id="82ce4-112">**Expire Agreements**– Within the current fiscal year, we're providing the number of expiring agreements.</span></span>
- <span data-ttu-id="82ce4-113">**Süresi dolan gelir**: açık süresi dolan anlaşmalarla ilişkili gelir.</span><span class="sxs-lookup"><span data-stu-id="82ce4-113">**Open Expiring Revenue**– The revenue associated to the open expiring agreements.</span></span>

:::image type="content" source="images/pci/cust-oppor-11.png" alt-text="Müşteriler fırsatlar Özet Panosu ekran görüntüsü.":::

## <a name="cloudascent-smb-segmentation"></a><span data-ttu-id="82ce4-115">Cloudadtik SMB kesimlemesi</span><span class="sxs-lookup"><span data-stu-id="82ce4-115">CloudAscent SMB segmentation</span></span>

<span data-ttu-id="82ce4-116">Küçük ve orta ölçekli iş (SMB) segmenti üç farklı alt parçaya bölünür.</span><span class="sxs-lookup"><span data-stu-id="82ce4-116">The small to medium business (SMB) segment is divided into three distinct sub segments.</span></span>

1. <span data-ttu-id="82ce4-117">**En Iyi yönetilmeyen** , Microsoft için en çok fırsat olan en büyük SMB müşterilerini içerir.</span><span class="sxs-lookup"><span data-stu-id="82ce4-117">**Top Unmanaged** includes the largest SMB customers with the most opportunity for Microsoft.</span></span> <span data-ttu-id="82ce4-118">Tipik En Iyi yönetilmeyen müşteriler benzer özellikleri, çok sayıda çalışan, büyük BT bütçeleri ve harcama ve Microsoft için büyük miktarda potansiyel gelir ile yönetilen hesaplara paylaşır.</span><span class="sxs-lookup"><span data-stu-id="82ce4-118">Typical Top Unmanaged customers share similar characteristics to Managed accounts, with large number of employees, large IT budgets and spend, and large amounts of potential revenue for Microsoft.</span></span>

   <span data-ttu-id="82ce4-119">En üst yönetilmeyen olarak iki şekilde tanımlanır:</span><span class="sxs-lookup"><span data-stu-id="82ce4-119">We define Top Unmanaged in two ways:</span></span>

   - <span data-ttu-id="82ce4-120">**Üst yönetilmeyen Kullanıcı tabanlı**– 300 veya daha fazla çalışan hesapları içerir.</span><span class="sxs-lookup"><span data-stu-id="82ce4-120">**Top Unmanaged User Based**– includes accounts with 300 or more employees.</span></span> <span data-ttu-id="82ce4-121">User-Based hesapları ilk kez satın alma veya Microsoft 365, Dynamics 365 veya Surface gibi kullanıcı tabanlı abonelik ürünlerinin genişletilmesi için harika hedeflerdir.</span><span class="sxs-lookup"><span data-stu-id="82ce4-121">User-Based accounts are great targets for first-time purchase, or expansion of user-based subscription products such as Microsoft 365, Dynamics 365, or Surface.</span></span>
   - <span data-ttu-id="82ce4-122">**En İyi Unmanaged Compute Based:** Azure potansiyeli 10 bin ABD dolarından büyük olan hesapları içerir.</span><span class="sxs-lookup"><span data-stu-id="82ce4-122">**Top Unmanaged Compute Based** – includes accounts with Azure potential greater than $10k.</span></span> <span data-ttu-id="82ce4-123">İşlem tabanlı hesaplar mevcut Azure'ları içerir.</span><span class="sxs-lookup"><span data-stu-id="82ce4-123">Compute based accounts include existing Azure.</span></span> <span data-ttu-id="82ce4-124">gelecek yıl için önemli bir potansiyele sahip olan hesaplar ve henüz Azure'a satın almamış ancak Azure için 10 bin DOlardan fazla potansiyele sahip olan hesaplar.</span><span class="sxs-lookup"><span data-stu-id="82ce4-124">accounts with significant future year potential and accounts who have yet to purchase Azure yet but have potential for Azure greater than $10k.</span></span>

2. <span data-ttu-id="82ce4-125">**Medium Business,** 25-300 çalışanı olan mevcut müşterileri ve potansiyel müşteri hesaplarını içerir.</span><span class="sxs-lookup"><span data-stu-id="82ce4-125">**Medium Business** includes existing customers and prospect accounts with 25 to 300 employees.</span></span>

3. <span data-ttu-id="82ce4-126">**Small Business,** 10-25 çalışanı olan işletmeler içerir.</span><span class="sxs-lookup"><span data-stu-id="82ce4-126">**Small Business** includes businesses with 10-25 employees.</span></span>

4. <span data-ttu-id="82ce4-127">**Çok Küçük İşletmeler,** 1-9 çalışanı olan işletmeler içerir.</span><span class="sxs-lookup"><span data-stu-id="82ce4-127">**Very Small Business** includes businesses with 1-9 employees.</span></span>

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="SMC türüne göre müşteri.":::

<span data-ttu-id="82ce4-129">**En İyi Unmanaged** **ve Medium Business** alt kesimleri, Microsoft ve Microsoft İş Ortakları için yüksek yaşam süresi değeri (LTV) müşterilerini temsil eder.</span><span class="sxs-lookup"><span data-stu-id="82ce4-129">**Top Unmanaged** and **Medium Business** subsegments represent high life-time value (LTV) customers for Microsoft, and Microsoft Partners.</span></span> <span data-ttu-id="82ce4-130">Bu nedenle, bu segmentte büyümeyi devamtırma odak noktası bunlardır.</span><span class="sxs-lookup"><span data-stu-id="82ce4-130">Because of this, they're the lead areas of focus for driving growth in this segment.</span></span> <span data-ttu-id="82ce4-131">Bu iki alt abonelikte yuvayı Microsoft 365 ile almak, D365/Azure iş hattı (LOB) uygulamalarıyla daha fazla gelir elde etmek ve Microsoft için yüksek bir LTV gerçekleştirmek için daha iyi konumlara sahip oluruz.</span><span class="sxs-lookup"><span data-stu-id="82ce4-131">In these two subsegments, we're better positioned to acquire the socket with Microsoft 365, monetize further with D365/Azure line of business (LOB) apps, and realize a high LTV for Microsoft.</span></span>

<span data-ttu-id="82ce4-132">Bugün iki önemli fırsat alanımız vardır: 1.</span><span class="sxs-lookup"><span data-stu-id="82ce4-132">Today we have two key areas of opportunity – 1.</span></span> <span data-ttu-id="82ce4-133">müşterimiz büyümeye devam ediyor; 2.</span><span class="sxs-lookup"><span data-stu-id="82ce4-133">our customer adds growth; 2.</span></span> <span data-ttu-id="82ce4-134">Bulut yuvalarını en iyi şekilde Microsoft 365 dynamics 365 ve Azure'da büyük bir fırsatımız var.</span><span class="sxs-lookup"><span data-stu-id="82ce4-134">while we do well acquiring cloud sockets leading with Microsoft 365, we have a large opportunity in Dynamics 365 and Azure.</span></span>

<span data-ttu-id="82ce4-135">Aşağıdaki ekran görüntüsü dört SMB Altgegment'larını temsil eder.</span><span class="sxs-lookup"><span data-stu-id="82ce4-135">The following screenshot represents the four SMB Subsegments.</span></span> <span data-ttu-id="82ce4-136">CloudAscent, tüm En İyi Unmanaged ve Medium Business hesaplarının profil oluşturma, puanlama ve modelleme önceliklerini belirleme.</span><span class="sxs-lookup"><span data-stu-id="82ce4-136">CloudAscent prioritize the profiling, scoring, and modeling of all Top Unmanaged and Medium Business accounts.</span></span>

:::image type="content" source="images/pci/cust-oppor-32.png" alt-text="SMB alt ayrımlarının ekran görüntüsü.":::

## <a name="cloudascent-machine-learning"></a><span data-ttu-id="82ce4-138">CloudAscent Machine Learning</span><span class="sxs-lookup"><span data-stu-id="82ce4-138">CloudAscent Machine Learning</span></span>

<span data-ttu-id="82ce4-139">SMB, En İyi Unmanaged ve Medium Business segmentleri içinde satış ve pazarlama müşterisi tahminlerini sağlamak için makine öğrenmesi teknolojisini kullanır.</span><span class="sxs-lookup"><span data-stu-id="82ce4-139">SMB uses machine learning technology to drive sales and marketing customer predictions within the Top Unmanaged and Medium Business segments.</span></span> <span data-ttu-id="82ce4-140">Sinyaller nasıl toplanır ve yayma önerilerine nasıl dönüşer?</span><span class="sxs-lookup"><span data-stu-id="82ce4-140">How are signals collected and turned into propensity recommendations?</span></span>

- <span data-ttu-id="82ce4-141">**Veri toplama**: web gezginleri şirket etki alanlarını ve blog yayınlarını izleyerek, yayınlar, sosyal akışlar ve teknik Forumlar ' e basarak milyarlarca müşteri sinyalleri tarar ve toplar.</span><span class="sxs-lookup"><span data-stu-id="82ce4-141">**Data Collection**: Web crawlers scan and collect billions of customer signals by pinging the company domains, and monitoring blog posts, press releases, social streams, and technical forums.</span></span>  <span data-ttu-id="82ce4-142">Toplanan sinyallere ek olarak, firmograf bilgileri, D&B, Microsoft Iç aboneliği ve işlem verileri gibi iç ve dış kaynaklardan toplanır.</span><span class="sxs-lookup"><span data-stu-id="82ce4-142">In addition to the collected signals, firmographics information is collected from both internal and external sources such as D&B, Microsoft Internal subscription and transactional data.</span></span>

- <span data-ttu-id="82ce4-143">**Machine Learning**: sinyaller, bulut ürünü ve kümesi tarafından her müşteri için yapılandırılmış veri satış ve pazarlama tahminleri kümesini veren makine öğrenimi modeline dağıtılır.</span><span class="sxs-lookup"><span data-stu-id="82ce4-143">**Machine Learning**: The signals are fed into the machine learning model that outputs a structured data set of Sales and Marketing predictions for each customer by cloud product and cluster.</span></span>  <span data-ttu-id="82ce4-144">Her müşteri, Microsoft 'un müşterinin sığdırmasını belirleyen ve müşterinin çevrimiçi davranışını tümleştiren makine öğrenimi algoritmalarının amaç olarak tanımladıkları, benzer bir model ile Microsoft 'un en üst SMB 'sini kullanarak puanlanır.</span><span class="sxs-lookup"><span data-stu-id="82ce4-144">Each customer is scored using a look alike model to Microsoft's top SMB that determines the customer's Fit, and machine learning algorithms that integrate the customer's online behavior define as Intent.</span></span> <span data-ttu-id="82ce4-145">Puanlama, Microsoft Bulut ürünlerini satın almak için müşterinin eğilimini gösteren kümeler halinde birleştirilir.</span><span class="sxs-lookup"><span data-stu-id="82ce4-145">The scoring is merged into clusters that show a customer's propensity to purchase Microsoft Cloud Products.</span></span>

- <span data-ttu-id="82ce4-146">**İyileştirme**: Machine Learning sistemi işlem verilerini aylık ve abonelik verilerini üç ayda bir tüketerek modelleri iyileştirir.</span><span class="sxs-lookup"><span data-stu-id="82ce4-146">**Optimization**: The Machine Learning system optimizes the models by consuming the transaction data monthly and the subscription data quarterly.</span></span>  <span data-ttu-id="82ce4-147">Win/kaybetme verilerini kullanarak, Machine Learning algoritmaları ayarlar ve küme önerilerini MSX bölümünde işlem yapılan fırsatlarla karşılaştırarak modellerin beklendiği gibi çalıştığını doğrular.</span><span class="sxs-lookup"><span data-stu-id="82ce4-147">Using the win/loss data, the Machine Learning adjusts the algorithms and validates that the models are working as expected by comparing cluster recommendations to opportunities acted upon in MSX.</span></span>

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="SMB Machine Learning 'in ekran görüntüsü.":::

## <a name="cloudascent-propensity"></a><span data-ttu-id="82ce4-149">Cloudadscent eğilimini</span><span class="sxs-lookup"><span data-stu-id="82ce4-149">CloudAscent Propensity</span></span>

<span data-ttu-id="82ce4-150">Eğilimini önerileri nasıl oluşturulur?</span><span class="sxs-lookup"><span data-stu-id="82ce4-150">How are propensity recommendations created?</span></span>

<span data-ttu-id="82ce4-151">Web gezginleri aracılığıyla toplanan sinyalleri ve çeşitli kaynaklardan gelen verileri kullanarak, firmograf verilerini ve müşterinin sosyal medya sinyallerini birleştirdik.</span><span class="sxs-lookup"><span data-stu-id="82ce4-151">Using signals collected via web crawlers and data provided from various sources, we consolidate the firmographics data and customer's social media signals.</span></span>  <span data-ttu-id="82ce4-152">Puanlama, bu sinyalleri ve verileri, amaç için uyum ve Puanlama modelleri için karşılaştırma modelleriyle kullanır.</span><span class="sxs-lookup"><span data-stu-id="82ce4-152">The scoring uses these signals and data in comparison models for fit and scoring models for Intent.</span></span>

1. <span data-ttu-id="82ce4-153">Müşteri hesabına Sığdır</span><span class="sxs-lookup"><span data-stu-id="82ce4-153">Customer Account Fit</span></span>

   - <span data-ttu-id="82ce4-154">Firmografları tanımlayan iç ve dış veri noktaları.</span><span class="sxs-lookup"><span data-stu-id="82ce4-154">Internal and External data points that define firmographics.</span></span>

   - <span data-ttu-id="82ce4-155">Kullanım Puanlama, müşterileri karşılaştırmak için en iyi SMB 'ye benzer bir model kullanır ve Microsoft Bulut ürünlere yönelik potansiyel bir uyum olup olmadığını görür.</span><span class="sxs-lookup"><span data-stu-id="82ce4-155">Fit scoring uses a look alike model to our best SMB to compare customers and see if they're a potential  fit for Microsoft Cloud Products.</span></span>

   - <span data-ttu-id="82ce4-156">Puanlama Sığdır üç ayda bir güncelleştirilir</span><span class="sxs-lookup"><span data-stu-id="82ce4-156">Fit scoring is updated quarterly</span></span>

2. <span data-ttu-id="82ce4-157">Müşteri hesabı hedefi</span><span class="sxs-lookup"><span data-stu-id="82ce4-157">Customer Account Intent</span></span>

   - <span data-ttu-id="82ce4-158">Sosyal medya ve müşterinin çevrimiçi davranışı ile ilgili sinyaller amaç tanımlar.</span><span class="sxs-lookup"><span data-stu-id="82ce4-158">Signals related to Social media and a customer's online behavior define Intent.</span></span>

   - <span data-ttu-id="82ce4-159">Amaç puanlama, kümeleri tanımlamak için uygun olan üst düzeye atlar.</span><span class="sxs-lookup"><span data-stu-id="82ce4-159">Intent scoring is overlaid on top of fit to define the clusters.</span></span>

   - <span data-ttu-id="82ce4-160">Amaç puanlama aylık olarak güncelleştirilir.</span><span class="sxs-lookup"><span data-stu-id="82ce4-160">Intent scoring is updated monthly.</span></span>

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="CloudAscent SMB tahmine dayalı modelleri.":::

3. <span data-ttu-id="82ce4-162">Kümeleme</span><span class="sxs-lookup"><span data-stu-id="82ce4-162">Clustering</span></span>

   <span data-ttu-id="82ce4-163">Fit ve amaç sinyalleri bir kümeleme puanında birleştirilmiştir.</span><span class="sxs-lookup"><span data-stu-id="82ce4-163">The Signals for fit and intent are consolidated into a clustering score.</span></span> <span data-ttu-id="82ce4-164">CloudAscent dört kümeye sahip:</span><span class="sxs-lookup"><span data-stu-id="82ce4-164">CloudAscent has four clusters:</span></span>

      - <span data-ttu-id="82ce4-165">Hemen Harekete Geç - satışa hazır müşteriler</span><span class="sxs-lookup"><span data-stu-id="82ce4-165">Act Now - sales ready customers</span></span>
      - <span data-ttu-id="82ce4-166">Değerlendirme - pazarlamaya hazır müşteriler</span><span class="sxs-lookup"><span data-stu-id="82ce4-166">Evaluate - marketing ready customers</span></span>
      - <span data-ttu-id="82ce4-167">Besleme - farkındalık kampanyalarını artırma</span><span class="sxs-lookup"><span data-stu-id="82ce4-167">Nurture - drive awareness campaigns</span></span>
      - <span data-ttu-id="82ce4-168">Eğitin - amaç için eğitin ve izleme</span><span class="sxs-lookup"><span data-stu-id="82ce4-168">Educate - educate and monitor for intent</span></span>

   <span data-ttu-id="82ce4-169">Kümeleme, kullanıcıların segment faktörlerine (örneğin ürün, coğrafi, sektör ve dikey) göre satış ve pazarlama girişimleri için belirli müşterileri hedeflemelerine olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="82ce4-169">The clustering allows users to target specific customers for sales and marketing initiatives based on segment factors, for example: product, geo, industry and vertical.</span></span>

   <span data-ttu-id="82ce4-170">CloudAscent Workbooks'daki Yayma modeli sekmesi, eğilimi ve tahmini boşluk gelirini paylaşıyor. </span><span class="sxs-lookup"><span data-stu-id="82ce4-170">The **Propensity model** tab in the CloudAscent Workbooks shares the propensity and the estimated whitespace revenue.</span></span> <span data-ttu-id="82ce4-171">Fit ve Intent kümelelerini tanımlamak için aşağıdaki adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="82ce4-171">To define the clustering of Fit and Intent, we go through the following steps:</span></span>

      1. <span data-ttu-id="82ce4-172">ML Modellerini kullanarak önce 100 ölçeğinde Customer Fit Score ve intent Score hesaplarız.</span><span class="sxs-lookup"><span data-stu-id="82ce4-172">Using ML Models, we first calculate Customer Fit Score and intent Score on a scale of 100.</span></span>  <span data-ttu-id="82ce4-173">Tam Puanlar ML Modellerine göre farklılık gösterir.</span><span class="sxs-lookup"><span data-stu-id="82ce4-173">Exact Scores will vary based on ML Models.</span></span>  <span data-ttu-id="82ce4-174">Aşağıdaki Örnek Puanlar:</span><span class="sxs-lookup"><span data-stu-id="82ce4-174">Example Scores Below:</span></span>

         |<span data-ttu-id="82ce4-175">**Sınıflandırma**</span><span class="sxs-lookup"><span data-stu-id="82ce4-175">**Classification**</span></span>|<span data-ttu-id="82ce4-176">**Puan**</span><span class="sxs-lookup"><span data-stu-id="82ce4-176">**Score**</span></span>|
         |---------|:---------|
         |<span data-ttu-id="82ce4-177">Yüksek</span><span class="sxs-lookup"><span data-stu-id="82ce4-177">High</span></span>|<span data-ttu-id="82ce4-178">75 - 100</span><span class="sxs-lookup"><span data-stu-id="82ce4-178">75 - 100</span></span>|
         |<span data-ttu-id="82ce4-179">Orta</span><span class="sxs-lookup"><span data-stu-id="82ce4-179">Medium</span></span>|<span data-ttu-id="82ce4-180">55 - 74</span><span class="sxs-lookup"><span data-stu-id="82ce4-180">55 - 74</span></span>|
         |<span data-ttu-id="82ce4-181">Düşük</span><span class="sxs-lookup"><span data-stu-id="82ce4-181">Low</span></span>|<span data-ttu-id="82ce4-182">30 - 54</span><span class="sxs-lookup"><span data-stu-id="82ce4-182">30 - 54</span></span>|
         |<span data-ttu-id="82ce4-183">Çok Düşük</span><span class="sxs-lookup"><span data-stu-id="82ce4-183">Very Low</span></span>|<span data-ttu-id="82ce4-184">0 - 29</span><span class="sxs-lookup"><span data-stu-id="82ce4-184">0 - 29</span></span>|

      2. <span data-ttu-id="82ce4-185">Yukarıdaki kuralı kullanarak, şirketlerin hem müşteri hem de amaç sinyallerine göre yüksek, orta, düşük ve çok düşük olmasını sağladık.</span><span class="sxs-lookup"><span data-stu-id="82ce4-185">Using the rule above, we classify companies to be High, Medium, Low, and Very Low across both Customer Fit and Intent Signals.</span></span>

      3. <span data-ttu-id="82ce4-186">Eğilimini temsil eden her kesişmeyle, bir 2B matriste müşterinin sığdırmasını ve amaç sinyallerini çiztik.</span><span class="sxs-lookup"><span data-stu-id="82ce4-186">We plot customer fit and intent signals on a 2D matrix with each intersection representing the propensity.</span></span> <span data-ttu-id="82ce4-187">Örneğin, en yüksek eğilimini temsil eden üst düzey + yüksek amaç = a1.</span><span class="sxs-lookup"><span data-stu-id="82ce4-187">For Example, High Fit + High Intent = A1, representing the highest propensity.</span></span>

      4. <span data-ttu-id="82ce4-188">Son olarak, bu segmentler grupları kümeler halinde oluşturur.</span><span class="sxs-lookup"><span data-stu-id="82ce4-188">Finally, these segments group to form clusters.</span></span>  <span data-ttu-id="82ce4-189">Örneğin, a1, a2, a3, A4, şimdi davran kümesi.</span><span class="sxs-lookup"><span data-stu-id="82ce4-189">For Example, A1, A2, A3, A4 form the Act Now cluster.</span></span>

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="Cloudadscent modelleri.":::

   <span data-ttu-id="82ce4-191">Bu müşteriler için, şimdi davran 'ın hedeflenmesini ve müşterileri değerlendirmesini öneririz.</span><span class="sxs-lookup"><span data-stu-id="82ce4-191">For these customers, we recommend targeting Act Now and Evaluate customers.</span></span>

## <a name="cloudascent-products--models"></a><span data-ttu-id="82ce4-192">Clouduscent ürünleri & modelleri</span><span class="sxs-lookup"><span data-stu-id="82ce4-192">CloudAscent Products & Models</span></span>

<span data-ttu-id="82ce4-193">Aşağıdaki grafik, Clouthscent içindeki her eğilimini modelinin bir görünümünü sağlar:</span><span class="sxs-lookup"><span data-stu-id="82ce4-193">The following graphic provides a view of each propensity model within CloudAscent:</span></span>

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="Cloudadscent eğilimini modeli.":::

<span data-ttu-id="82ce4-195">Boşluk modelleri, bir ürünün olmadığı ve/veya net yeni aday müşteriler müşterileri olmayan mevcut Microsoft müşterilerinin tahminlerden oluşur.</span><span class="sxs-lookup"><span data-stu-id="82ce4-195">Whitespace models are composed of predictions for existing Microsoft customers where they don't have a product and/or are net new prospect customers.</span></span>

<span data-ttu-id="82ce4-196">Büyük satış modelleri, Azure ve Microsoft 365 SKU 'Larında büyük satış potansiyelini tahmin etmek için işlem verilerini kullanır.</span><span class="sxs-lookup"><span data-stu-id="82ce4-196">Upsell models use transaction data to predict the potential for upsell in Azure and Microsoft 365 SKUs.</span></span>

<span data-ttu-id="82ce4-197">Bu müşterilerin hem Azure hem de Microsoft 365 sahip olacağı ve büyük satış modeli, mevcut SKU 'sunun daha fazlasını satın aldıklarından emin olur.</span><span class="sxs-lookup"><span data-stu-id="82ce4-197">These customers will already have both Azure or Microsoft 365 and the upsell model shows that they’re likely to purchase more of their existing SKU.</span></span>

<span data-ttu-id="82ce4-198">EOS, Win 7, Office 2010, SQL Server ve Windows Server için hizmet sonu (EOS) müşterilerini paylaşır.</span><span class="sxs-lookup"><span data-stu-id="82ce4-198">EOS shares the end of service (EOS) customers for Win 7, Office 2010, SQL Server, and Windows Server.</span></span> <span data-ttu-id="82ce4-199">EOS verileri MS Sales 'ten çekilir ve kullanılabilir olduğunda CloudAscent eğilimini modellemesiyle yer alýr.</span><span class="sxs-lookup"><span data-stu-id="82ce4-199">The EOS data is pulled from MS Sales and overlaid with the CloudAscent propensity modeling where available.</span></span> <span data-ttu-id="82ce4-200">EOS verileri, modern Iş ve Azure satış oynatılırken yaşar.</span><span class="sxs-lookup"><span data-stu-id="82ce4-200">EOS data lives in the Modern Work and Azure Sales plays.</span></span>
