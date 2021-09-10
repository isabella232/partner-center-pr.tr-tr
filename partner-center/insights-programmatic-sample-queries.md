---
title: Örnek sorgu listesi
description: İş ortağı öngörüleri analiz verilerine programlı bir şekilde erişmek için örnek sorguları kullanın.
ms.topic: reference
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 36da8a59548142bf09daf42dbc936fba15d46d1e
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960855"
---
# <a name="sample-queries-for-partner-center-insights-report"></a>Iş Ortağı Merkezi Öngörüler için örnek sorgular raporu

bu makalede, iş ortağı Analizler raporları için örnek sorgular sağlanmaktadır. Bu sorguları rapor sorgusu oluştur API uç noktasını çağırarak kullanabilirsiniz. Gerekirse, daha fazla sütun eklemek, hesaplama dönemini ayarlamak ve filtre koşulları eklemek için [rapor sorgusu oluştur API](insights-programmatic-access-paradigm.md#create-report-query-api) çağrısı değiştirilebilir.

Sütun adları, öznitelikler ve açıklamalar hakkındaki ayrıntılar için [veri tanımlarına](insights-data-definitions.md)bakın.

## <a name="customer-details"></a>Müşteri ayrıntıları

Bu örnek sorgular, müşteriler Ayrıntılar raporu için geçerlidir:

### <a name="by-geography"></a>Coğrafya tarafından

Geçen ay içindeki belirli bir Coğrafya ait müşterilerin listesi.

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a>SKU ve faturalandırılan gelire göre

Belirli SKU ve faturalandırılan gelir kullanan müşterilerin listesi, son 6 ay içinde 20.000 ' den fazla

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a>Kullanılabilir koltuk

Son aydaki mevcut bilgisayarlara göre ilk 10 müşteri

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a>İş ortağı profili

Bu örnek sorgular iş ortağı profili raporuna uygulanır:

### <a name="by-geography"></a>Coğrafya tarafından

Belirli bir Coğrafya iş ortaklarının listesi.

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a>MPN iş ortağı tarafından

Aynı PGA MPN Iş ortağı kapsamındaki iş ortaklarının listesi

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a>Satıcı performansı

Bu örnek sorgular, satıcı performans raporu için geçerlidir:

### <a name="by-geography"></a>Coğrafya tarafından

Geçen ay içindeki belirli bir coğrafya için satıcıların listesi.

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a>Satıcıya göre

Müşteri sayısı, abonelik sayısı, kullanılabilir toplam bilgisayar, toplam atanan koltuk, belirli bir Bayi için toplam gelir.

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a>Gelire göre ilk 10

Son aydaki toplam geliri temel alan ilk 10 satıcıdır.

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a>Abonelik Ayrıntıları

Bu örnek sorgular Abonelik Ayrıntıları raporu için geçerlidir:

### <a name="by-renewal-eligibility"></a>Yenilemeye uygunluk ölçütü

Son ay içinde otomatik yenilemeye uygun olmayan aboneliklerin listesi.

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a>Abonelik durumuna göre

Son aydaki devre dışı durumunda olan aboneliklerin listesi.

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a>Altı ay sayısı

Abonelik sayısı, toplam satılan lisans sayısı, son altı ayda belirli bir iş ortağı için müşteri sayısı.

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a>Azure kullanımı

Bu örnek sorgular, Azure kullanım raporu için geçerlidir:

### <a name="by-meter-category"></a>Ölçüm kategorisine göre

Son altı ay içindeki belirli ölçüm kategorisi için kullanım birimleri ve ACR ile Azure kullanım aboneliklerinin listesi.

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a>Toplam ACR 'ye göre

Toplam ACR 'nin son altı ayda 20.000 ' den büyük olduğu Azure kullanım aboneliklerinin listesi

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a>Sonraki adımlar

- [Partner Insights Analytics verilerine erişim için API 'Ler](insights-programmatic-analytics-available-api.md)