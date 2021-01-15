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
ms.openlocfilehash: 244cb852728d47360cf8ecd1d1e9ccb641466b1d
ms.sourcegitcommit: 1a0c83e2089cb58221bdb24525127378f5197ea8
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/14/2021
ms.locfileid: "98215756"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="12f05-103">İş verilerinizi Microsoft için Partner Center Analytics uygulaması ile görüntüleyin Power BI</span><span class="sxs-lookup"><span data-stu-id="12f05-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="12f05-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="12f05-104">**Appropriate roles**</span></span>

- <span data-ttu-id="12f05-105">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="12f05-105">Global admin</span></span>
- <span data-ttu-id="12f05-106">Kullanıcı yöneticisi</span><span class="sxs-lookup"><span data-stu-id="12f05-106">User admin</span></span>
- <span data-ttu-id="12f05-107">Satış Aracısı</span><span class="sxs-lookup"><span data-stu-id="12f05-107">Sales agent</span></span>
- <span data-ttu-id="12f05-108">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="12f05-108">Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="12f05-109">İş verilerinizi görüntüleyin</span><span class="sxs-lookup"><span data-stu-id="12f05-109">View your business data</span></span>

<span data-ttu-id="12f05-110">Aşağıdakiler de dahil olmak üzere, Power BI için Partner Center Analytics uygulaması ile iş verilerinizin görsel bir temsilini alın:</span><span class="sxs-lookup"><span data-stu-id="12f05-110">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="12f05-111">Müşteri tabanınız, abonelikleriniz ve lisanslarınızın büyümesi</span><span class="sxs-lookup"><span data-stu-id="12f05-111">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="12f05-112">Office 365, Microsoft Dynamics ve Microsoft Azure ürünlerinin kullanımı</span><span class="sxs-lookup"><span data-stu-id="12f05-112">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="12f05-113">Son 60 güne ait her bir Azure aboneliğinde ölçülen her kaynak için günlük tüketim birimleri</span><span class="sxs-lookup"><span data-stu-id="12f05-113">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="12f05-114">Tahmini maliyet (en son fiyat kartına göre)</span><span class="sxs-lookup"><span data-stu-id="12f05-114">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="12f05-115">Veri kümelerini dışarı aktarma ve müşteri başına dahil özel raporlar oluşturma özelliği.</span><span class="sxs-lookup"><span data-stu-id="12f05-115">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="12f05-116">Iş ortağı merkezi analizi uygulama Önizleme sürümü hakkında</span><span class="sxs-lookup"><span data-stu-id="12f05-116">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="12f05-117">Bu uygulama yalnızca bulut çözüm sağlayıcısı programındaki doğrudan iş ortakları içindir.</span><span class="sxs-lookup"><span data-stu-id="12f05-117">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="12f05-118">CSP 'deki diğer iş ortakları (örneğin, dolaylı satıcılar) oturum açamaz.</span><span class="sxs-lookup"><span data-stu-id="12f05-118">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="12f05-119">Tüm tahmini maliyetler ön vergi faturalandırma/fatura verileri olduğundan, yasal olmayan bir şekilde bağlanmamalıdır.</span><span class="sxs-lookup"><span data-stu-id="12f05-119">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="12f05-120">Tahmini maliyetlerin yalnızca veri öngörüleri için kullanılması amaçlanmıştır.</span><span class="sxs-lookup"><span data-stu-id="12f05-120">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="12f05-121">Müşteri bilgileri, abonelikleri temel alır.</span><span class="sxs-lookup"><span data-stu-id="12f05-121">Customer information is based on subscriptions.</span></span> <span data-ttu-id="12f05-122">Son zamanlarda hesap oluşturduğunuz, ancak henüz abonelikleri olmayan müşteriler, sayımlar halinde dahil değildir.</span><span class="sxs-lookup"><span data-stu-id="12f05-122">Any customers that you've recently created accounts for, but who do not yet have subscriptions, are not included in counts.</span></span>

- <span data-ttu-id="12f05-123">Tahmini maliyet, CSP fiyatlandırmasını temel alan en son fiyat kartını temel alır.</span><span class="sxs-lookup"><span data-stu-id="12f05-123">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="12f05-124">Gün sayısı takvim gündür.</span><span class="sxs-lookup"><span data-stu-id="12f05-124">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="12f05-125">İş öngörüleri raporu</span><span class="sxs-lookup"><span data-stu-id="12f05-125">Business Insights report</span></span>

- <span data-ttu-id="12f05-126">**Müşteri kiracılar**: abonelikleri satın almış olan müşterilerin farklı Azure AD kiracılarının sayısı</span><span class="sxs-lookup"><span data-stu-id="12f05-126">**Customer tenants**: Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="12f05-127">**Yeni (son 30 gün)**: son 30 gün içinde en az bir abonelik satın alan yeni müşteriler</span><span class="sxs-lookup"><span data-stu-id="12f05-127">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="12f05-128">**Karmaşıklık (son 30 gün)**: "etkin", "yetkisiz kullanım" veya "devre dışı" abonelikler olmadan müşteriler</span><span class="sxs-lookup"><span data-stu-id="12f05-128">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="12f05-129">**Yeni (son 24 saat)**: son 24 saat içinde en az bir abonelik satın alan yeni müşteriler</span><span class="sxs-lookup"><span data-stu-id="12f05-129">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="12f05-130">**Son 12 ay Içinde tahmini aylık maliyet**: aylık aylık, son 12 ay boyunca aylık olarak toplanan tahmini vergi öncesi fatura doları tutarının aylık eğilimi</span><span class="sxs-lookup"><span data-stu-id="12f05-130">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="12f05-131">**Son 12 ay içinde ürüne göre tahmini maliyet**: satılan ürünler, son 12 ay süresince toplanan tahmini vergi öncesi fatura doları tutarına göre sıralanır.</span><span class="sxs-lookup"><span data-stu-id="12f05-131">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="12f05-132">Bu durum, en fazla gelir getiren en popüler ürünleri gösterir.</span><span class="sxs-lookup"><span data-stu-id="12f05-132">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="12f05-133">**Son 12 ay Içindeki müşteriler**: aylık son 12 ay boyunca aylık olarak toplanan yeni müşteriler ve değişim müşterilerinin aylık ayı eğilimi</span><span class="sxs-lookup"><span data-stu-id="12f05-133">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="12f05-134">**Son 12 ay boyunca müşteriye göre tahmini maliyet**: müşteriler, son 12 ay süresince toplanan tahmini vergi öncesi fatura dolar tutarına göre sıralanır.</span><span class="sxs-lookup"><span data-stu-id="12f05-134">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="12f05-135">Bu durum, en çok gelir getiren popüler müşterileri gösterir.</span><span class="sxs-lookup"><span data-stu-id="12f05-135">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="12f05-136">**Ürüne göre müşteri sayısı**: satılan ürünler, ilişkili müşterilere göre sıralanır.</span><span class="sxs-lookup"><span data-stu-id="12f05-136">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="12f05-137">Bu durum, çoğu müşteriye satılan en popüler ürünleri gösterir.</span><span class="sxs-lookup"><span data-stu-id="12f05-137">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="12f05-138">Abonelik öngörüleri raporu</span><span class="sxs-lookup"><span data-stu-id="12f05-138">Subscription Insights report</span></span>

- <span data-ttu-id="12f05-139">**Abonelik durumu**:</span><span class="sxs-lookup"><span data-stu-id="12f05-139">**Subscription status**:</span></span>

- <span data-ttu-id="12f05-140">Etkin: "etkin" ya da "yetkisiz kullanım" durumuna ait abonelikler</span><span class="sxs-lookup"><span data-stu-id="12f05-140">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="12f05-141">Askıya alındı: "devre dışı" durumuna ait abonelikler</span><span class="sxs-lookup"><span data-stu-id="12f05-141">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="12f05-142">Serbest sağlanmış: "önceden sağlanmış" veya "süre sonu" durumuna ait abonelikler</span><span class="sxs-lookup"><span data-stu-id="12f05-142">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="12f05-143">**Süre sonu durumu**:</span><span class="sxs-lookup"><span data-stu-id="12f05-143">**Expiry status**:</span></span>

  - <span data-ttu-id="12f05-144">Süresi geçti: süresi zaten geçmiş abonelikler (abonelik bitiş tarihi geçmiş)</span><span class="sxs-lookup"><span data-stu-id="12f05-144">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="12f05-145">30 gün sonra süresi doluyor: 30 gün sonra süresi dolacak abonelikler (abonelik bitiş tarihi sonraki 30 gün sonra olduğunda)</span><span class="sxs-lookup"><span data-stu-id="12f05-145">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="12f05-146">30 gün içinde süresi doluyor: sonraki 30 gün içinde süresi dolacak abonelikler (abonelik bitiş tarihi bugün ve sonraki 30 gün arasındadır)</span><span class="sxs-lookup"><span data-stu-id="12f05-146">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="12f05-147">**Toplam abonelikler**: "etkin", "yetkisiz kullanım" veya "devre dışı" durumundaki abonelikler</span><span class="sxs-lookup"><span data-stu-id="12f05-147">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="12f05-148">**Yeni (son 30 gün)**: son 30 gün içinde müşteriler tarafından satın alınan yeni abonelikler</span><span class="sxs-lookup"><span data-stu-id="12f05-148">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="12f05-149">**Yeni (son 24 saat)**: son 24 saat içinde müşteriler tarafından satın alınan yeni abonelikler</span><span class="sxs-lookup"><span data-stu-id="12f05-149">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="12f05-150">**30 gün Içinde süresi doluyor**: sonraki 30 gün içinde süresi dolacak abonelikler</span><span class="sxs-lookup"><span data-stu-id="12f05-150">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="12f05-151">**Dalgalanma (son 30 gün)**: son 30 gün içinde zaten sağlanmış veya askıya alınmış (devre dışı) abonelikler</span><span class="sxs-lookup"><span data-stu-id="12f05-151">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="12f05-152">**Abonelik türlerine göre dağıtım**: Toplam aboneliklerin lisans tabanlı ve kullanım tabanlı abonelik türüne göre dağılımı</span><span class="sxs-lookup"><span data-stu-id="12f05-152">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="12f05-153">**Ürüne göre etkin abonelik sayısı**: satılan ürünler, etkin abonelik sayısına göre sıralanır</span><span class="sxs-lookup"><span data-stu-id="12f05-153">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="12f05-154">**Son** 12 aya ait abonelikler: son 12 ay boyunca aylık olarak toplanan yeni aboneliklerin ve değişim aboneliklerinin ayda ayı eğilimi</span><span class="sxs-lookup"><span data-stu-id="12f05-154">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="12f05-155">**Müşteri aboneliği ayrıntıları**: müşterilerin, aboneliklerin ve tekliflerin ayrıntılı görünümü</span><span class="sxs-lookup"><span data-stu-id="12f05-155">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="12f05-156">Lisans öngörüleri raporu:</span><span class="sxs-lookup"><span data-stu-id="12f05-156">License Insights report:</span></span>

- <span data-ttu-id="12f05-157">**Toplam** lisans sayısı: lisans tabanlı tüm abonelikler genelinde toplanan toplam lisans sayısı</span><span class="sxs-lookup"><span data-stu-id="12f05-157">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="12f05-158">**Yeni (son 30 gün)**: son 30 gün içinde lisans ekleme</span><span class="sxs-lookup"><span data-stu-id="12f05-158">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="12f05-159">**Karmaşıklık (son 30 gün)**: son 30 gün içinde lisans azaltma</span><span class="sxs-lookup"><span data-stu-id="12f05-159">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="12f05-160">**Yeni (son 24 saat)**: son 24 saat içinde lisans ekleme</span><span class="sxs-lookup"><span data-stu-id="12f05-160">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="12f05-161">**Son 90 gün Içindeki lisanslar**: son 90 günün süresi boyunca aylık olarak toplanan lisans eklemeleri ve indirimlerinin ayda ayı eğilimi</span><span class="sxs-lookup"><span data-stu-id="12f05-161">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="12f05-162">**Ürüne göre etkin lisans sayısı**: satılan ürünler, etkin lisans sayısına göre sıralanır</span><span class="sxs-lookup"><span data-stu-id="12f05-162">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="12f05-163">**Müşteriye göre etkin lisans sayısı**: müşteriler etkin lisans sayısına göre sıralanır</span><span class="sxs-lookup"><span data-stu-id="12f05-163">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="12f05-164">**Son 90 gün Içindeki müşteri lisans olay ayrıntıları**: olay tarihi, olay adı, miktar ve miktar değişikliği dahil olmak üzere müşteriler, abonelikler ve abonelik olaylarının ayrıntılı görünümü.</span><span class="sxs-lookup"><span data-stu-id="12f05-164">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="12f05-165">Lisans kullanım raporu:</span><span class="sxs-lookup"><span data-stu-id="12f05-165">Licenses Usage report:</span></span>

- <span data-ttu-id="12f05-166">**Ürüne göre atanan lisanslar**: lisans atama sayısına göre sıralanan ürünler</span><span class="sxs-lookup"><span data-stu-id="12f05-166">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="12f05-167">**Ürün tarafından kullanılan lisanslar**: lisans kullanım sayısına göre sıralanan ürünler</span><span class="sxs-lookup"><span data-stu-id="12f05-167">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="12f05-168">**Atanan lisansların müşteri dağılımı**:% %20 ' nin %20 ' si için lisans ataması ile toplam müşterilerin dağılımı</span><span class="sxs-lookup"><span data-stu-id="12f05-168">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="12f05-169">**Kullanımdaki lisansların müşteri dağılımı**: %20 ' nin lisans kullanımına göre %20 aralığında bozuk toplam müşterilerin dağılımı%</span><span class="sxs-lookup"><span data-stu-id="12f05-169">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="12f05-170">**Müşteri tarafından atanan lisanslar**: satılan lisansların ayrıntılı görünümü ve müşteriler ve ürünler tarafından atanan lisanslar</span><span class="sxs-lookup"><span data-stu-id="12f05-170">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="12f05-171">**Müşteri tarafından kullanılan lisanslar**: müşteriler ve ürünler tarafından kullanılan lisansların ve lisansların ayrıntılı görünümü</span><span class="sxs-lookup"><span data-stu-id="12f05-171">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="12f05-172">Azure Insights raporu:</span><span class="sxs-lookup"><span data-stu-id="12f05-172">Azure Insights report:</span></span>

- <span data-ttu-id="12f05-173">**Son 12 ay Içinde kullanım tabanlı müşteriler**: son 12 ay boyunca aylık olarak toplanan yeni kullanım tabanlı müşterilerin aylık ayı eğilimi ve tek başına kullanılan kullanım tabanlı müşteriler</span><span class="sxs-lookup"><span data-stu-id="12f05-173">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="12f05-174">**Son 12 aya göre kullanım tabanlı abonelikler**: son 12 ay boyunca aylık olarak toplanan yeni kullanım tabanlı aboneliklerin ve tek başına kullanılan kullanım tabanlı aboneliklerin aya göre ayı eğilimi</span><span class="sxs-lookup"><span data-stu-id="12f05-174">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="12f05-175">**Son 60 gün içinde müşterinin tahmin edilen kullanım maliyeti**: Kullanım tabanlı müşteriler, son 60 günün dönemi boyunca toplanan tahmini vergi öncesi fatura doları tutarına göre sıralanır.</span><span class="sxs-lookup"><span data-stu-id="12f05-175">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="12f05-176">Bu durum, en çok geliri getiren en popüler kullanım tabanlı müşterileri gösterir</span><span class="sxs-lookup"><span data-stu-id="12f05-176">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="12f05-177">**Son 60 gün içinde kategoriye göre tahmini kullanım maliyeti**: Kullanım tabanlı aboneliklerin ölçüm kategorileri, son 60 günün dönemi boyunca toplanan tahmini vergi öncesi fatura dolar tutarına göre sıralanır.</span><span class="sxs-lookup"><span data-stu-id="12f05-177">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="12f05-178">**Son 60 gün içinde abonelik tarafından tahmini kullanım maliyeti**: son 60 günün dönemi boyunca toplanan tahmini vergi öncesi fatura doları tutarına göre kullanım tabanlı abonelikler.</span><span class="sxs-lookup"><span data-stu-id="12f05-178">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="12f05-179">**Bütçe harcamasına göre müşterinin tahmini kullanım maliyeti**: müşteriler, geçerli kullanım harcama bütçesi yüzdesine göre sıralanır (%100%).</span><span class="sxs-lookup"><span data-stu-id="12f05-179">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="12f05-180">Azure Kaynak kullanımı raporu:</span><span class="sxs-lookup"><span data-stu-id="12f05-180">Azure Resource Usage report:</span></span>

- <span data-ttu-id="12f05-181">**Seçili dönem için güne göre Azure kaynakları kullanımı**: son 60 gün içindeki seçili dönem için her bir kullanım tabanlı abonelikte her bir ölçülen kaynak için günlük tüketim birimleri.</span><span class="sxs-lookup"><span data-stu-id="12f05-181">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="12f05-182">**Seçili dönem Için Azure kaynaklarının tahmini kullanım maliyeti**: son 60 gün içindeki seçili dönem için her bir kullanım tabanlı abonelikte her bir ölçülen kaynak için en son fiyat kartına göre tahmini maliyet.</span><span class="sxs-lookup"><span data-stu-id="12f05-182">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="12f05-183">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="12f05-183">Next steps</span></span>

- [<span data-ttu-id="12f05-184">Power BI uygulamasına genel bakış için iş ortağı merkezi analizi</span><span class="sxs-lookup"><span data-stu-id="12f05-184">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="12f05-185">Microsoft Power BI için İş Ortağı Merkezi Analizi uygulamasını yükleme ve önizleme</span><span class="sxs-lookup"><span data-stu-id="12f05-185">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
