---
title: Örnek sorgu listesi
description: İş ortağı öngörüleri analiz verilerine programlı bir şekilde erişmek için örnek sorguları kullanın.
ms.topic: reference
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: e25784585a1ac505db99e58265939a8851edcbad
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376941"
---
# <a name="sample-queries-for-partner-center-insights-report"></a><span data-ttu-id="7b4ce-103">Iş Ortağı Merkezi Öngörüler için örnek sorgular raporu</span><span class="sxs-lookup"><span data-stu-id="7b4ce-103">Sample queries for Partner Center insights report</span></span>

<span data-ttu-id="7b4ce-104">bu makalede, iş ortağı Analizler raporları için örnek sorgular sağlanmaktadır.</span><span class="sxs-lookup"><span data-stu-id="7b4ce-104">This article provides sample queries for the Partner Insights reports.</span></span> <span data-ttu-id="7b4ce-105">Bu sorguları rapor sorgusu oluştur API uç noktasını çağırarak kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7b4ce-105">You can use these queries by calling the Create Report Query API endpoint.</span></span> <span data-ttu-id="7b4ce-106">Gerekirse, daha fazla sütun eklemek, hesaplama dönemini ayarlamak ve filtre koşulları eklemek için [rapor sorgusu oluştur API](insights-programmatic-access-paradigm.md#create-report-query-api) çağrısı değiştirilebilir.</span><span class="sxs-lookup"><span data-stu-id="7b4ce-106">If necessary, the [Create Report Query API](insights-programmatic-access-paradigm.md#create-report-query-api) call can be modified to add more columns, adjust the computation period, and add filter conditions.</span></span>

<span data-ttu-id="7b4ce-107">Sütun adları, öznitelikler ve açıklamalar hakkındaki ayrıntılar için [veri tanımlarına](insights-data-definitions.md)bakın.</span><span class="sxs-lookup"><span data-stu-id="7b4ce-107">For details about the column names, attributes, and descriptions, refer to the [Data Definitions](insights-data-definitions.md).</span></span>

## <a name="customer-details"></a><span data-ttu-id="7b4ce-108">Müşteri ayrıntıları</span><span class="sxs-lookup"><span data-stu-id="7b4ce-108">Customer details</span></span>

<span data-ttu-id="7b4ce-109">Bu örnek sorgular, müşteriler Ayrıntılar raporu için geçerlidir:</span><span class="sxs-lookup"><span data-stu-id="7b4ce-109">These sample queries apply to the customers details report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="7b4ce-110">Coğrafya tarafından</span><span class="sxs-lookup"><span data-stu-id="7b4ce-110">By geography</span></span>

<span data-ttu-id="7b4ce-111">Geçen ay içindeki belirli bir Coğrafya ait müşterilerin listesi.</span><span class="sxs-lookup"><span data-stu-id="7b4ce-111">List of customers from a specific geography in last month.</span></span>

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a><span data-ttu-id="7b4ce-112">SKU ve faturalandırılan gelire göre</span><span class="sxs-lookup"><span data-stu-id="7b4ce-112">By SKU and billed revenue</span></span>

<span data-ttu-id="7b4ce-113">Belirli SKU ve faturalandırılan gelir kullanan müşterilerin listesi, son 6 ay içinde 20.000 ' den fazla</span><span class="sxs-lookup"><span data-stu-id="7b4ce-113">List of customers using specific SKU and Billed Revenue is more than 20,000 in the last 6 months</span></span>

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a><span data-ttu-id="7b4ce-114">Kullanılabilir koltuk</span><span class="sxs-lookup"><span data-stu-id="7b4ce-114">By available seats</span></span>

<span data-ttu-id="7b4ce-115">Son aydaki mevcut bilgisayarlara göre ilk 10 müşteri</span><span class="sxs-lookup"><span data-stu-id="7b4ce-115">Top 10 customers based on Available seats in last month</span></span>

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a><span data-ttu-id="7b4ce-116">İş ortağı profili</span><span class="sxs-lookup"><span data-stu-id="7b4ce-116">Partner Profile</span></span>

<span data-ttu-id="7b4ce-117">Bu örnek sorgular iş ortağı profili raporuna uygulanır:</span><span class="sxs-lookup"><span data-stu-id="7b4ce-117">These sample queries apply to the partner profile report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="7b4ce-118">Coğrafya tarafından</span><span class="sxs-lookup"><span data-stu-id="7b4ce-118">By geography</span></span>

<span data-ttu-id="7b4ce-119">Belirli bir Coğrafya iş ortaklarının listesi.</span><span class="sxs-lookup"><span data-stu-id="7b4ce-119">List of partners from a specific geography.</span></span>

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a><span data-ttu-id="7b4ce-120">MPN iş ortağı tarafından</span><span class="sxs-lookup"><span data-stu-id="7b4ce-120">By MPN partner</span></span>

<span data-ttu-id="7b4ce-121">Aynı PGA MPN Iş ortağı kapsamındaki iş ortaklarının listesi</span><span class="sxs-lookup"><span data-stu-id="7b4ce-121">List of partners under same PGA MPN Partner</span></span>

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a><span data-ttu-id="7b4ce-122">Satıcı performansı</span><span class="sxs-lookup"><span data-stu-id="7b4ce-122">Reseller Performance</span></span>

<span data-ttu-id="7b4ce-123">Bu örnek sorgular, satıcı performans raporu için geçerlidir:</span><span class="sxs-lookup"><span data-stu-id="7b4ce-123">These sample queries apply to the reseller performance report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="7b4ce-124">Coğrafya tarafından</span><span class="sxs-lookup"><span data-stu-id="7b4ce-124">By geography</span></span>

<span data-ttu-id="7b4ce-125">Geçen ay içindeki belirli bir coğrafya için satıcıların listesi.</span><span class="sxs-lookup"><span data-stu-id="7b4ce-125">List of resellers from a specific geography in last month.</span></span>

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a><span data-ttu-id="7b4ce-126">Satıcıya göre</span><span class="sxs-lookup"><span data-stu-id="7b4ce-126">By reseller</span></span>

<span data-ttu-id="7b4ce-127">Müşteri sayısı, abonelik sayısı, kullanılabilir toplam bilgisayar, toplam atanan koltuk, belirli bir Bayi için toplam gelir.</span><span class="sxs-lookup"><span data-stu-id="7b4ce-127">Customer count, subscription count, total available seats, total assigned seats, total revenue for a specific reseller.</span></span>

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a><span data-ttu-id="7b4ce-128">Gelire göre ilk 10</span><span class="sxs-lookup"><span data-stu-id="7b4ce-128">Top 10 by revenue</span></span>

<span data-ttu-id="7b4ce-129">Son aydaki toplam geliri temel alan ilk 10 satıcıdır.</span><span class="sxs-lookup"><span data-stu-id="7b4ce-129">Top 10 resellers based on total revenue in last month.</span></span>

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a><span data-ttu-id="7b4ce-130">Abonelik Ayrıntıları</span><span class="sxs-lookup"><span data-stu-id="7b4ce-130">Subscription Details</span></span>

<span data-ttu-id="7b4ce-131">Bu örnek sorgular Abonelik Ayrıntıları raporu için geçerlidir:</span><span class="sxs-lookup"><span data-stu-id="7b4ce-131">These sample queries apply to the subscription details report:</span></span>

### <a name="by-renewal-eligibility"></a><span data-ttu-id="7b4ce-132">Yenilemeye uygunluk ölçütü</span><span class="sxs-lookup"><span data-stu-id="7b4ce-132">By renewal eligibility</span></span>

<span data-ttu-id="7b4ce-133">Son ay içinde otomatik yenilemeye uygun olmayan aboneliklerin listesi.</span><span class="sxs-lookup"><span data-stu-id="7b4ce-133">List of subscriptions who are not eligible for auto renewal in last month.</span></span>

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a><span data-ttu-id="7b4ce-134">Abonelik durumuna göre</span><span class="sxs-lookup"><span data-stu-id="7b4ce-134">By subscription state</span></span>

<span data-ttu-id="7b4ce-135">Son aydaki devre dışı durumunda olan aboneliklerin listesi.</span><span class="sxs-lookup"><span data-stu-id="7b4ce-135">List of subscriptions who are in Disable state in last month.</span></span>

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a><span data-ttu-id="7b4ce-136">Altı ay sayısı</span><span class="sxs-lookup"><span data-stu-id="7b4ce-136">Counts for six months</span></span>

<span data-ttu-id="7b4ce-137">Abonelik sayısı, toplam satılan lisans sayısı, son altı ayda belirli bir iş ortağı için müşteri sayısı.</span><span class="sxs-lookup"><span data-stu-id="7b4ce-137">Subscription count, total sold seats, customer count for a specific partner in last six months.</span></span>

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a><span data-ttu-id="7b4ce-138">Azure kullanımı</span><span class="sxs-lookup"><span data-stu-id="7b4ce-138">Azure Usage</span></span>

<span data-ttu-id="7b4ce-139">Bu örnek sorgular, Azure kullanım raporu için geçerlidir:</span><span class="sxs-lookup"><span data-stu-id="7b4ce-139">These sample queries apply to the Azure usage report:</span></span>

### <a name="by-meter-category"></a><span data-ttu-id="7b4ce-140">Ölçüm kategorisine göre</span><span class="sxs-lookup"><span data-stu-id="7b4ce-140">By meter category</span></span>

<span data-ttu-id="7b4ce-141">Son altı ay içindeki belirli ölçüm kategorisi için kullanım birimleri ve ACR ile Azure kullanım aboneliklerinin listesi.</span><span class="sxs-lookup"><span data-stu-id="7b4ce-141">List of Azure usage subscriptions with usage units and ACR for specific meter category in last six months.</span></span>

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a><span data-ttu-id="7b4ce-142">Toplam ACR 'ye göre</span><span class="sxs-lookup"><span data-stu-id="7b4ce-142">By total ACR</span></span>

<span data-ttu-id="7b4ce-143">Toplam ACR 'nin son altı ayda 20.000 ' den büyük olduğu Azure kullanım aboneliklerinin listesi</span><span class="sxs-lookup"><span data-stu-id="7b4ce-143">List of Azure usage subscriptions where total ACR is greater than 20,000 in last six months</span></span>

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a><span data-ttu-id="7b4ce-144">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="7b4ce-144">Next steps</span></span>

- [<span data-ttu-id="7b4ce-145">Partner Insights Analytics verilerine erişim için API 'Ler</span><span class="sxs-lookup"><span data-stu-id="7b4ce-145">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)