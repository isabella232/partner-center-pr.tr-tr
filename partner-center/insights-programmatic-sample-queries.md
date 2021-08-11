---
title: Örnek sorguların listesi
description: İş ortağı içgörüleri analiz verilerine program aracılığıyla erişmek için örnek sorguları kullanın.
ms.topic: reference
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: fff74f7bf6c58f5845c491d23a1f71c3da177e0c126e863205f0fb18eb07b7c9
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115693291"
---
# <a name="sample-queries-for-partner-center-insights-report"></a>İş Ortağı Merkezi içgörüleri raporu için örnek sorgular

Bu makalede İş Ortağı raporları için örnek sorgular Analizler ve sağlar. Rapor Sorgusu API'si oluşturma uç noktasını çağırarak bu sorguları kullanabilirsiniz. Gerekirse Rapor Sorgusu [API'si](insights-programmatic-access-paradigm.md#create-report-query-api) oluşturma çağrısı daha fazla sütun eklemek, hesaplama dönemini ayarlamak ve filtre koşulları eklemek için değiştirilebilir.

Sütun adları, öznitelikler ve açıklamalar hakkında ayrıntılı bilgi için Veri [Tanımları'na bakın.](insights-data-definitions.md)

## <a name="customer-details"></a>Müşteri ayrıntıları

Bu örnek sorgular, müşterilere ilişkin ayrıntılar raporu için geçerlidir:

### <a name="by-geography"></a>Coğrafyaya göre

Geçen ay belirli bir coğrafyadan gelen müşterilerin listesi.

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a>SKU'ya ve faturalandırmış gelire göre

Belirli SKU ve Faturalı Gelir kullanan müşterilerin listesi son 6 ay içinde 20.000'den fazladır

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a>Kullanılabilir yerlere göre

Geçen ayki Kullanılabilir boş alanlara göre ilk 10 müşteri

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a>İş Ortağı Profili

Bu örnek sorgular iş ortağı profili raporu için geçerlidir:

### <a name="by-geography"></a>Coğrafyaya göre

Belirli bir coğrafyadan iş ortaklarının listesi.

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a>MPN iş ortağına göre

Aynı PGA MPN İş Ortağı altındaki iş ortakları listesi

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a>Kurumsal Bayi Performansı

Bu örnek sorgular kurumsal bayi performans raporu için geçerlidir:

### <a name="by-geography"></a>Coğrafyaya göre

Geçen ay belirli bir coğrafyada yer alan kurumsal bayilerin listesi.

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a>Kurumsal bayiye göre

Müşteri sayısı, abonelik sayısı, toplam kullanılabilir lisans sayısı, toplam atanan lisans sayısı, belirli bir kurumsal bayinin toplam geliri.

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a>Gelire göre ilk 10

Geçen ayki toplam gelire göre ilk 10 kurumsal bayi.

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a>Abonelik Ayrıntıları

Bu örnek sorgular abonelik ayrıntıları raporu için geçerlidir:

### <a name="by-renewal-eligibility"></a>Yenileme uygunluğuna göre

Geçen ay otomatik yenileme için uygun olan aboneliklerin listesi.

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a>Abonelik durumuna göre

Geçen ay Devre Dışı Bırak durumuna sahip aboneliklerin listesi.

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a>Altı ay için sayımlar

Abonelik sayısı, toplam satılan yer sayısı, son altı ay içinde belirli bir iş ortağı için müşteri sayısı.

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a>Azure Kullanımı

Bu örnek sorgular Azure kullanım raporu için geçerlidir:

### <a name="by-meter-category"></a>Ölçüm kategorisine göre

Son altı ay içinde kullanım birimleri ve belirli ölçüm kategorisi için ACR'ye sahip Azure kullanım aboneliklerinin listesi.

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a>Toplam ACR'ye göre

Toplam ACR'nin son altı ay içinde 20.000'den fazla olduğu Azure kullanım aboneliklerinin listesi

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a>Sonraki adımlar

- [İş ortağı içgörüleri analiz verilerine erişmek için API'ler](insights-programmatic-analytics-available-api.md)