---
title: Power BI için Iş Ortağı Merkezi analizlerini kullanma
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Power BI için Partner Center Analytics uygulamasını kullanarak iş verilerinizi görüntülemeyi öğrenin (CSP 'deki doğrudan iş ortakları için).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 248527fdbc536c552f7b2d00f208838b4ef19085
ms.sourcegitcommit: 0a6b1e6d845391539f54213efff00af4d23f028c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/14/2020
ms.locfileid: "92530956"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="6fe55-103">İş verilerinizi Microsoft için Partner Center Analytics uygulaması ile görüntüleyin Power BI</span><span class="sxs-lookup"><span data-stu-id="6fe55-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>

<span data-ttu-id="6fe55-104">**Uygulama hedefi**</span><span class="sxs-lookup"><span data-stu-id="6fe55-104">**Applies to**</span></span>

- <span data-ttu-id="6fe55-105">İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="6fe55-105">Partner Center</span></span>

<span data-ttu-id="6fe55-106">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="6fe55-106">**Appropriate roles**</span></span>

- <span data-ttu-id="6fe55-107">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="6fe55-107">Global admin</span></span>
- <span data-ttu-id="6fe55-108">Kullanıcı yöneticisi</span><span class="sxs-lookup"><span data-stu-id="6fe55-108">User admin</span></span>
- <span data-ttu-id="6fe55-109">Satış Aracısı</span><span class="sxs-lookup"><span data-stu-id="6fe55-109">Sales agent</span></span>
- <span data-ttu-id="6fe55-110">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="6fe55-110">Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="6fe55-111">İş verilerinizi görüntüleyin</span><span class="sxs-lookup"><span data-stu-id="6fe55-111">View your business data</span></span>

<span data-ttu-id="6fe55-112">Aşağıdakiler de dahil olmak üzere, Power BI için Partner Center Analytics uygulaması ile iş verilerinizin görsel bir temsilini alın:</span><span class="sxs-lookup"><span data-stu-id="6fe55-112">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="6fe55-113">Müşteri tabanınız, abonelikleriniz ve lisanslarınızın büyümesi</span><span class="sxs-lookup"><span data-stu-id="6fe55-113">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="6fe55-114">Office 365, Microsoft Dynamics ve Microsoft Azure ürünlerinin kullanımı</span><span class="sxs-lookup"><span data-stu-id="6fe55-114">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="6fe55-115">Son 60 güne ait her bir Azure aboneliğinde ölçülen her kaynak için günlük tüketim birimleri</span><span class="sxs-lookup"><span data-stu-id="6fe55-115">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="6fe55-116">Tahmini maliyet (en son fiyat kartına göre)</span><span class="sxs-lookup"><span data-stu-id="6fe55-116">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="6fe55-117">Veri kümelerini dışarı aktarma ve müşteri başına dahil özel raporlar oluşturma özelliği.</span><span class="sxs-lookup"><span data-stu-id="6fe55-117">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="6fe55-118">Iş ortağı merkezi analizi uygulama Önizleme sürümü hakkında</span><span class="sxs-lookup"><span data-stu-id="6fe55-118">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="6fe55-119">Bu uygulama yalnızca bulut çözüm sağlayıcısı programındaki doğrudan iş ortakları içindir.</span><span class="sxs-lookup"><span data-stu-id="6fe55-119">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="6fe55-120">CSP 'deki diğer iş ortakları (örneğin, dolaylı satıcılar) oturum açamaz.</span><span class="sxs-lookup"><span data-stu-id="6fe55-120">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="6fe55-121">Tüm tahmini maliyetler ön vergi faturalandırma/fatura verileri olduğundan, yasal olmayan bir şekilde bağlanmamalıdır.</span><span class="sxs-lookup"><span data-stu-id="6fe55-121">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="6fe55-122">Tahmini maliyetlerin yalnızca veri öngörüleri için kullanılması amaçlanmıştır.</span><span class="sxs-lookup"><span data-stu-id="6fe55-122">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="6fe55-123">Müşteri bilgileri, abonelikleri temel alır.</span><span class="sxs-lookup"><span data-stu-id="6fe55-123">Customer information is based on subscriptions.</span></span> <span data-ttu-id="6fe55-124">Son zamanlarda hesap oluşturduğunuz, ancak henüz abonelikleri olmayan müşteriler, sayımlar halinde dahil değildir.</span><span class="sxs-lookup"><span data-stu-id="6fe55-124">Any customers that you've recently created accounts for, but who do not yet have subscriptions, are not included in counts.</span></span>

- <span data-ttu-id="6fe55-125">Tahmini maliyet, CSP fiyatlandırmasını temel alan en son fiyat kartını temel alır.</span><span class="sxs-lookup"><span data-stu-id="6fe55-125">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="6fe55-126">Gün sayısı takvim gündür.</span><span class="sxs-lookup"><span data-stu-id="6fe55-126">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="6fe55-127">İş öngörüleri raporu</span><span class="sxs-lookup"><span data-stu-id="6fe55-127">Business Insights report</span></span>

- <span data-ttu-id="6fe55-128">**Müşteri kiracılar** : abonelikleri satın almış olan müşterilerin farklı Azure AD kiracılarının sayısı</span><span class="sxs-lookup"><span data-stu-id="6fe55-128">**Customer tenants** : Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="6fe55-129">**Yeni (son 30 gün)** : son 30 gün içinde en az bir abonelik satın alan yeni müşteriler</span><span class="sxs-lookup"><span data-stu-id="6fe55-129">**New (last 30 days)** : New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="6fe55-130">**Karmaşıklık (son 30 gün)** : "etkin", "yetkisiz kullanım" veya "devre dışı" abonelikler olmadan müşteriler</span><span class="sxs-lookup"><span data-stu-id="6fe55-130">**Churn (last 30 days)** : Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="6fe55-131">**Yeni (son 24 saat)** : son 24 saat içinde en az bir abonelik satın alan yeni müşteriler</span><span class="sxs-lookup"><span data-stu-id="6fe55-131">**New (last 24 hours)** : New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="6fe55-132">**Son 12 ay Içinde tahmini aylık maliyet** : aylık aylık, son 12 ay boyunca aylık olarak toplanan tahmini vergi öncesi fatura doları tutarının aylık eğilimi</span><span class="sxs-lookup"><span data-stu-id="6fe55-132">**Estimated monthly cost over last 12 months** : Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="6fe55-133">**Son 12 ay içinde ürüne göre tahmini maliyet** : satılan ürünler, son 12 ay süresince toplanan tahmini vergi öncesi fatura doları tutarına göre sıralanır.</span><span class="sxs-lookup"><span data-stu-id="6fe55-133">**Estimated cost by product over last 12 months** : Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="6fe55-134">Bu durum, en fazla gelir getiren en popüler ürünleri gösterir.</span><span class="sxs-lookup"><span data-stu-id="6fe55-134">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="6fe55-135">**Son 12 ay Içindeki müşteriler** : aylık son 12 ay boyunca aylık olarak toplanan yeni müşteriler ve değişim müşterilerinin aylık ayı eğilimi</span><span class="sxs-lookup"><span data-stu-id="6fe55-135">**Customers over last 12 months** : Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="6fe55-136">**Son 12 ay boyunca müşteriye göre tahmini maliyet** : müşteriler, son 12 ay süresince toplanan tahmini vergi öncesi fatura dolar tutarına göre sıralanır.</span><span class="sxs-lookup"><span data-stu-id="6fe55-136">**Estimated cost by customer over last 12 months** : Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="6fe55-137">Bu durum, en çok gelir getiren popüler müşterileri gösterir.</span><span class="sxs-lookup"><span data-stu-id="6fe55-137">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="6fe55-138">**Ürüne göre müşteri sayısı** : satılan ürünler, ilişkili müşterilere göre sıralanır.</span><span class="sxs-lookup"><span data-stu-id="6fe55-138">**Customer count by product** : Products sold sorted by associated customers.</span></span> <span data-ttu-id="6fe55-139">Bu durum, çoğu müşteriye satılan en popüler ürünleri gösterir.</span><span class="sxs-lookup"><span data-stu-id="6fe55-139">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="6fe55-140">Abonelik öngörüleri raporu</span><span class="sxs-lookup"><span data-stu-id="6fe55-140">Subscription Insights report</span></span>

- <span data-ttu-id="6fe55-141">**Abonelik durumu** :</span><span class="sxs-lookup"><span data-stu-id="6fe55-141">**Subscription status** :</span></span>

- <span data-ttu-id="6fe55-142">Etkin: "etkin" ya da "yetkisiz kullanım" durumuna ait abonelikler</span><span class="sxs-lookup"><span data-stu-id="6fe55-142">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="6fe55-143">Askıya alındı: "devre dışı" durumuna ait abonelikler</span><span class="sxs-lookup"><span data-stu-id="6fe55-143">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="6fe55-144">Serbest sağlanmış: "önceden sağlanmış" veya "süre sonu" durumuna ait abonelikler</span><span class="sxs-lookup"><span data-stu-id="6fe55-144">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="6fe55-145">**Süre sonu durumu** :</span><span class="sxs-lookup"><span data-stu-id="6fe55-145">**Expiry status** :</span></span>

  - <span data-ttu-id="6fe55-146">Süresi geçti: süresi zaten geçmiş abonelikler (abonelik bitiş tarihi geçmiş)</span><span class="sxs-lookup"><span data-stu-id="6fe55-146">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="6fe55-147">30 gün sonra süresi doluyor: 30 gün sonra süresi dolacak abonelikler (abonelik bitiş tarihi sonraki 30 gün sonra olduğunda)</span><span class="sxs-lookup"><span data-stu-id="6fe55-147">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="6fe55-148">30 gün içinde süresi doluyor: sonraki 30 gün içinde süresi dolacak abonelikler (abonelik bitiş tarihi bugün ve sonraki 30 gün arasındadır)</span><span class="sxs-lookup"><span data-stu-id="6fe55-148">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="6fe55-149">**Toplam abonelikler** : "etkin", "yetkisiz kullanım" veya "devre dışı" durumundaki abonelikler</span><span class="sxs-lookup"><span data-stu-id="6fe55-149">**Total subscriptions** : Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="6fe55-150">**Yeni (son 30 gün)** : son 30 gün içinde müşteriler tarafından satın alınan yeni abonelikler</span><span class="sxs-lookup"><span data-stu-id="6fe55-150">**New (last 30 days)** : New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="6fe55-151">**Yeni (son 24 saat)** : son 24 saat içinde müşteriler tarafından satın alınan yeni abonelikler</span><span class="sxs-lookup"><span data-stu-id="6fe55-151">**New (last 24 hours)** : New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="6fe55-152">**30 gün Içinde süresi doluyor** : sonraki 30 gün içinde süresi dolacak abonelikler</span><span class="sxs-lookup"><span data-stu-id="6fe55-152">**Expiring in 30 days** : Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="6fe55-153">**Dalgalanma (son 30 gün)** : son 30 gün içinde zaten sağlanmış veya askıya alınmış (devre dışı) abonelikler</span><span class="sxs-lookup"><span data-stu-id="6fe55-153">**Churn (last 30 days)** : Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="6fe55-154">**Abonelik türlerine göre dağıtım** : Toplam aboneliklerin lisans tabanlı ve kullanım tabanlı abonelik türüne göre dağılımı</span><span class="sxs-lookup"><span data-stu-id="6fe55-154">**Distribution by subscription types** : % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="6fe55-155">**Ürüne göre etkin abonelik sayısı** : satılan ürünler, etkin abonelik sayısına göre sıralanır</span><span class="sxs-lookup"><span data-stu-id="6fe55-155">**Active subscription count by product** : Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="6fe55-156">**Son** 12 aya ait abonelikler: son 12 ay boyunca aylık olarak toplanan yeni aboneliklerin ve değişim aboneliklerinin ayda ayı eğilimi</span><span class="sxs-lookup"><span data-stu-id="6fe55-156">**Subscriptions over last 12 months** : Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="6fe55-157">**Müşteri aboneliği ayrıntıları** : müşterilerin, aboneliklerin ve tekliflerin ayrıntılı görünümü</span><span class="sxs-lookup"><span data-stu-id="6fe55-157">**Customer subscription details** : Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="6fe55-158">Lisans öngörüleri raporu:</span><span class="sxs-lookup"><span data-stu-id="6fe55-158">License Insights report:</span></span>

- <span data-ttu-id="6fe55-159">**Toplam** lisans sayısı: lisans tabanlı tüm abonelikler genelinde toplanan toplam lisans sayısı</span><span class="sxs-lookup"><span data-stu-id="6fe55-159">**Total licenses** : Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="6fe55-160">**Yeni (son 30 gün)** : son 30 gün içinde lisans ekleme</span><span class="sxs-lookup"><span data-stu-id="6fe55-160">**New (last 30 days)** : License addition within last 30 days</span></span>

- <span data-ttu-id="6fe55-161">**Karmaşıklık (son 30 gün)** : son 30 gün içinde lisans azaltma</span><span class="sxs-lookup"><span data-stu-id="6fe55-161">**Churn (last 30 days)** : License reduction within last 30 days</span></span>

- <span data-ttu-id="6fe55-162">**Yeni (son 24 saat)** : son 24 saat içinde lisans ekleme</span><span class="sxs-lookup"><span data-stu-id="6fe55-162">**New (last 24 hours)** : License addition within last 24 hours</span></span>

- <span data-ttu-id="6fe55-163">**Son 90 gün Içindeki lisanslar** : son 90 günün süresi boyunca aylık olarak toplanan lisans eklemeleri ve indirimlerinin ayda ayı eğilimi</span><span class="sxs-lookup"><span data-stu-id="6fe55-163">**Licenses over last 90 days** : Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="6fe55-164">**Ürüne göre etkin lisans sayısı** : satılan ürünler, etkin lisans sayısına göre sıralanır</span><span class="sxs-lookup"><span data-stu-id="6fe55-164">**Active license count by product** : Products sold sorted by active license count</span></span>

- <span data-ttu-id="6fe55-165">**Müşteriye göre etkin lisans sayısı** : müşteriler etkin lisans sayısına göre sıralanır</span><span class="sxs-lookup"><span data-stu-id="6fe55-165">**Active license count by customer** : Customers sorted by active license count</span></span>

- <span data-ttu-id="6fe55-166">**Son 90 gün Içindeki müşteri lisans olay ayrıntıları** : olay tarihi, olay adı, miktar ve miktar değişikliği dahil olmak üzere müşteriler, abonelikler ve abonelik olaylarının ayrıntılı görünümü.</span><span class="sxs-lookup"><span data-stu-id="6fe55-166">**Customer license event details over last 90 days** : Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="6fe55-167">Lisans kullanım raporu:</span><span class="sxs-lookup"><span data-stu-id="6fe55-167">Licenses Usage report:</span></span>

- <span data-ttu-id="6fe55-168">**Ürüne göre atanan lisanslar** : lisans atama sayısına göre sıralanan ürünler</span><span class="sxs-lookup"><span data-stu-id="6fe55-168">**Licenses assigned by product** : Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="6fe55-169">**Ürün tarafından kullanılan lisanslar** : lisans kullanım sayısına göre sıralanan ürünler</span><span class="sxs-lookup"><span data-stu-id="6fe55-169">**Licenses in use by product** : Products sold sorted by license usage count</span></span>

- <span data-ttu-id="6fe55-170">**Atanan lisansların müşteri dağılımı** :% %20 ' nin %20 ' si için lisans ataması ile toplam müşterilerin dağılımı</span><span class="sxs-lookup"><span data-stu-id="6fe55-170">**Customer distribution of licenses assigned** : % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="6fe55-171">**Kullanımdaki lisansların müşteri dağılımı** : %20 ' nin lisans kullanımına göre %20 aralığında bozuk toplam müşterilerin dağılımı%</span><span class="sxs-lookup"><span data-stu-id="6fe55-171">**Customer distribution of licenses in use** : % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="6fe55-172">**Müşteri tarafından atanan lisanslar** : satılan lisansların ayrıntılı görünümü ve müşteriler ve ürünler tarafından atanan lisanslar</span><span class="sxs-lookup"><span data-stu-id="6fe55-172">**Licenses assigned by customer** : Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="6fe55-173">**Müşteri tarafından kullanılan lisanslar** : müşteriler ve ürünler tarafından kullanılan lisansların ve lisansların ayrıntılı görünümü</span><span class="sxs-lookup"><span data-stu-id="6fe55-173">**Licenses in use by customer** : Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="6fe55-174">Azure Insights raporu:</span><span class="sxs-lookup"><span data-stu-id="6fe55-174">Azure Insights report:</span></span>

- <span data-ttu-id="6fe55-175">**Son 12 ay Içinde kullanım tabanlı müşteriler** : son 12 ay boyunca aylık olarak toplanan yeni kullanım tabanlı müşterilerin aylık ayı eğilimi ve tek başına kullanılan kullanım tabanlı müşteriler</span><span class="sxs-lookup"><span data-stu-id="6fe55-175">**Usage-based customers over last 12 months** : Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="6fe55-176">**Son 12 aya göre kullanım tabanlı abonelikler** : son 12 ay boyunca aylık olarak toplanan yeni kullanım tabanlı aboneliklerin ve tek başına kullanılan kullanım tabanlı aboneliklerin aya göre ayı eğilimi</span><span class="sxs-lookup"><span data-stu-id="6fe55-176">**Usage-based subscriptions over last 12 months** : Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="6fe55-177">**Son 60 gün içinde müşterinin tahmin edilen kullanım maliyeti** : Kullanım tabanlı müşteriler, son 60 günün dönemi boyunca toplanan tahmini vergi öncesi fatura doları tutarına göre sıralanır.</span><span class="sxs-lookup"><span data-stu-id="6fe55-177">**Estimated cost of usage by customer over last 60 days** : Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="6fe55-178">Bu durum, en çok geliri getiren en popüler kullanım tabanlı müşterileri gösterir</span><span class="sxs-lookup"><span data-stu-id="6fe55-178">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="6fe55-179">**Son 60 gün içinde kategoriye göre tahmini kullanım maliyeti** : Kullanım tabanlı aboneliklerin ölçüm kategorileri, son 60 günün dönemi boyunca toplanan tahmini vergi öncesi fatura dolar tutarına göre sıralanır.</span><span class="sxs-lookup"><span data-stu-id="6fe55-179">**Estimated cost of usage by category over last 60 days** : Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="6fe55-180">**Son 60 gün içinde abonelik tarafından tahmini kullanım maliyeti** : son 60 günün dönemi boyunca toplanan tahmini vergi öncesi fatura doları tutarına göre kullanım tabanlı abonelikler.</span><span class="sxs-lookup"><span data-stu-id="6fe55-180">**Estimated cost of usage by subscription over last 60 days** : Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="6fe55-181">**Bütçe harcamasına göre müşterinin tahmini kullanım maliyeti** : müşteriler, geçerli kullanım harcama bütçesi yüzdesine göre sıralanır (%100%).</span><span class="sxs-lookup"><span data-stu-id="6fe55-181">**Customer estimated usage cost by spending budget** : Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="6fe55-182">Azure Kaynak kullanımı raporu:</span><span class="sxs-lookup"><span data-stu-id="6fe55-182">Azure Resource Usage report:</span></span>

- <span data-ttu-id="6fe55-183">**Seçili dönem için güne göre Azure kaynakları kullanımı** : son 60 gün içindeki seçili dönem için her bir kullanım tabanlı abonelikte her bir ölçülen kaynak için günlük tüketim birimleri.</span><span class="sxs-lookup"><span data-stu-id="6fe55-183">**Usage of Azure resources by day for selected period** : Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="6fe55-184">**Seçili dönem Için Azure kaynaklarının tahmini kullanım maliyeti** : son 60 gün içindeki seçili dönem için her bir kullanım tabanlı abonelikte her bir ölçülen kaynak için en son fiyat kartına göre tahmini maliyet.</span><span class="sxs-lookup"><span data-stu-id="6fe55-184">**Estimated usage cost of Azure resources for selected period** : Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="6fe55-185">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="6fe55-185">Next steps</span></span>

- [<span data-ttu-id="6fe55-186">Power BI uygulamasına genel bakış için iş ortağı merkezi analizi</span><span class="sxs-lookup"><span data-stu-id="6fe55-186">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="6fe55-187">Microsoft Power BI için İş Ortağı Merkezi Analizi uygulamasını yükleme ve önizleme</span><span class="sxs-lookup"><span data-stu-id="6fe55-187">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
