---
title: İş ortağı içgörüleri programlı erişimi için sistem sorgularının listesi
description: İş ortağı içgörüleri analiz verilerine erişmek için kullanabileceğiniz sistem sorguları hakkında daha fazla bilgi edinin.
ms.topic: reference
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 4b0bd5411d02463b015cf812cde78e34ef853814
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376918"
---
# <a name="list-of-system-queries-for-partner-insights-programmatic-access"></a>İş ortağı içgörüleri programlı erişimi için sistem sorgularının listesi

Aşağıdaki sistem sorguları doğrudan QueryId ile [Rapor Oluşturma API'sinde](insights-programmatic-access-paradigm.md#create-report-api) kullanılabilir. Sistem sorguları, altı aylık (6 milyon) İş Ortağı Merkezi raporları dışarı aktarma raporlarına benzer.

Sütun adları, öznitelikler ve açıklama hakkında daha fazla bilgi için lütfen Veri [Tanımları'na bakın](insights-data-definitions.md)

Aşağıdaki bölümlerde çeşitli raporlar için rapor sorguları sağlanmıştır.

## <a name="customers"></a>Müşteriler

Son altı aya göre Müşteriler raporu

Sorgu Kimliği: `6664daf3-c161-423a-92a1-0ea6db2c0384`

### <a name="report-query"></a>Rapor sorgusu
```sql
SELECT PGAMpnId,MpnId,PartnerName,CustomerName,CustomerTpid,DUNSNumber,CustomerSegment,TopSegment,
CustomerMarket,CustomerStatus,CustomerTenantId,CustomerTenantName,CustomerTenantCountry,TenantDomainName,
Product,RawProductName,ProductPartNumber,SKU,Month,PartnerLocation,PartnerAttributionType,SalesChannel,
IsDuplicateRowForPGA,AvailableSeats,BilledRevenueUSD,AzureConsumedRevenueUSD 
FROM CustomersAndTenants TIMESPAN LAST_6_MONTHS
```

## <a name="seats-subscriptions-and-revenue"></a>Seats Subscriptions and Revenue

Son altı ay için yer, abonelik ve gelir raporu

Sorgu Kimliği: `c9fc1c79-4408-49ff-97f9-e1aa3f155804`

### <a name="report-query"></a>Rapor sorgusu

```sql
SELECT PGAMpnId,MpnId,SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,SubscriptionState,month,
IsAutoRenew,CustomerName,CustomerTenantId,CustomerTpid,DUNSNumber,CustomerSegment,TopSegment,CustomerMarket,
ProductFamily,ReportingProductName,Product,RawProductName,ProductPartNumber,SKU,RevSumDivisionName,PartnerName,
SolutionArea,PartnerLocation,PartnerAttributionType,SalesChannel,PricingLevel,EnrollmentNumber,
IsDuplicateRowForPGA,SubscriptionStartMonth,TotalSoldSeats,TotalAssignedSeats,BilledRevenueUSD,
AzureConsumedRevenueUSD FROM SeatsSubscriptionsAndRevenue TIMESPAN LAST_6_MONTHS
```

## <a name="partner-profile"></a>İş Ortağı Profili

Profil verileri

Sorgu Kimliği: `e65f3a4f-fb99-4319-97ff-59e57566a871`

### <a name="report-query"></a>Rapor sorgusu

```sql
SELECT MPNId,PartnerName,PGA_MPNId,PGA_PartnerName,City,Country,HierarchyLevel 
FROM Profile
```

## <a name="azure-usage"></a>Azure Kullanımı

Son altı ay için AzureUsage raporu

Sorgu Kimliği: `d1a4d75e-5ca8-4847-845f-ee0a9be6f07b`

### <a name="report-query"></a>Rapor sorgusu

```sql
SELECT PGAMpnId,SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,FirstUseDate,SubscriptionState,Month,
ServiceName,MeterCategory,UsageUnits,UsageQuantity,CustomerName,CustomerTenantId,CustomerTpid,CustomerSegment,
CustomerMarket,MpnId,PartnerName,PartnerLocation,PartnerAttributionType,SalesChannel,EnrollmentNumber,
IsACRDuplicateAtPGALevel,ResellerID,ResellerName,MonthlySubscriptionLevelACR,TotalACR 
FROM AzureUsage TIMESPAN LAST_6_MONTHS
```

## <a name="office-usage"></a>Office Kullanım

Son altı ay için OfficeUsage raporu

Sorgu Kimliği: `d8349f7b-a7d1-467e-b26d-434d4a50f26a`

### <a name="report-query"></a>Rapor sorgusu

```sql
SELECT CustomerTenantId,CustomerTpid,WorkloadName,Month,PaidAvailableUnits,MonthlyActiveUsers,CustomerName,
CustomerMarket,CustomerSegment,MPNId,PartnerName,PartnerLocation,PartnerAttributionType,IsDuplicateRowForPGA
FROM OfficeUsage TIMESPAN LAST_6_MONTHS
```

## <a name="dynamics-usage"></a>Dynamics Kullanımı

DynamicsUsage raporu altı ay boyunca

Sorgu Kimliği: `6209a8fd-93af-442e-8b3f-3df0f77e8463`

### <a name="report-query"></a>Rapor sorgusu

```sql
SELECT SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,SubscriptionStatus,Month,RevSumDivisionName,
RevSumCategoryName,SKU,SKUId,FreeVsPaidSKU,SalesModel,DetailedSalesModel,CustomerName,CustomerTenantId,
CustomerTpid,CustomerSegment,CustomerMarket,MPNId,PartnerName,PartnerLocation,PartnerAttachType,AvailableSeats,
AssignedSeats,ActiveSeats,DeploymentOpportunity,ActiveUsagePercent 
FROM DynamicsUsage TIMESPAN LAST_6_MONTHS
```

## <a name="power-bi-usage"></a>Power BI kullanımı

Altı ay boyunca PowerBIUsage raporu

Sorgu Kimliği: `40ebfe2f-7183-4427-a911-5c9b45b6df15`

### <a name="report-query"></a>Rapor sorgusu

```sql
SELECT SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,SubscriptionStatus,Month,SKU,SKUId,
FreeVsPaidSKU,SalesModel,DetailedSalesModel,CustomerName,CustomerTenantId,CustomerTpid,CustomerSegment,
CustomerMarket,MPNId,PartnerName,PartnerLocation,PartnerAttachType,PartnerHierarchy,AvailableSeats,
AssignedSeats,ActiveSeats,DeploymentOpportunity,ActiveUsagePercent 
FROM PowerBIUsage TIMESPAN LAST_6_MONTHS
```

## <a name="ems-usage"></a>EMS Kullanımı

ALTı ay boyunca EMSUsage raporu

Sorgu Kimliği: `d7f20ea4-8751-4d6b-b1d7-821c316acd6a`

### <a name="report-query"></a>Rapor sorgusu

```sql
SELECT SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,SubscriptionStatus,Month,SKU,SKUId,
FreeVsPaidSKU,SalesModel,DetailedSalesModel,CustomerName,CustomerTenantId,CustomerTpid,CustomerSegment,
CustomerMarket,MPNId,PartnerName,PartnerLocation,PartnerAttachType,PartnerHierarchy,PaidAvailableUnits,
MonthlyActiveUsers,AADPPaidAvailableUnits,IntunePaidAvailableUnits,AzipPaidAvailableUnits,
AADPMonthlyActiveUsers,IntuneMonthlyActiveUsers,AzipMonthlyActiveUsers FROM EMSUsage TIMESPAN LAST_6_MONTHS
```

## <a name="competency-performance-requirement-report"></a>Uzmanlık Performansı gereksinim raporu

CompetencyPeformanceRequirement raporu altı ay boyunca

Sorgu Kimliği: `3a0e1adc-f5c1-42ac-9422-8e944bf81ae5`

### <a name="report-query"></a>Rapor sorgusu

```sql
SELECT CompetencyName,CompetencyAttainmentOptionName,Month,MetricName,MetricMonthlyContribution,TTMAggregate,
AnniversaryYearAggregate,GoldThreshold,SilverThreshold 
FROM CompetencyPeformanceRequirement 
TIMESPAN LAST_6_MONTHS
```

## <a name="cloud-products-reseller-performance"></a>Bulut ürünleri kurumsal bayi performansı

### <a name="report-description"></a>Rapor açıklaması

Altı ay boyunca CloudProductsResellerPerformance raporu

Sorgu Kimliği: `c09c2eda-861b-4664-8ee8-48a14745a26a`

### <a name="report-query"></a>Rapor sorgusu

```sql
SELECT ResellerMpnid,ResellerName,ResellerMarket,IndirectProviderMPNId,IndirectProviderName,Month,Product,
SubscriptionID,AvailableSeats,AssignedSeats,BilledRevenueUSD,CustomerName,CustomerTPid,CustomerSegment,
CustomerMarket,ResellerStatus 
FROM CloudProductsResellerPerformance TIMESPAN LAST_6_MONTHS
```

## <a name="clas-agreement-renewal-propensity"></a>CLAS Sözleşmesi Yenileme eğilimi

CLASAgreementRenewalsPropensity raporu altı ay boyunca

Sorgu Kimliği: `c4fc87ac-4cca-44cd-bf4d-835ac513f9ee`

### <a name="report-query"></a>Rapor sorgusu

```sql
SELECT MPNID,PartnerName,CustomerID,DUNSNumber,AccountName,Domain,OrgSize,Industry,Vertical,Area,Subsidiary,
SalesTerritory,City,State,PostalCode,Country,Segment,SubSegment,SMCTypeSummary,TopUnmanagedComputeBase,
TopUnmanagedUserBase,IsNonProfit,HasGoogle,HasAWS,AzureCluster,D365FOCluster,D365CECluster,D365BCCluster,
M365Cluster,LicenseProgram,AgreementID,AgreementEndDate,ExpirationType,ExpiringRevenue,HasEA,HasOpen,
AzureUpsellCustomer,M365UpsellCustomer,RevSumDivisionName 
FROM CLASAgreementRenewalsPropensity
```

## <a name="clas-azure-propensity"></a>CLAS Azure eğilimi

ALTı ay boyunca CLASAzurePropensity raporu

Sorgu Kimliği: `9a18bd70-8f90-4bd2-8266-5f6e453e3ee7`

### <a name="report-query"></a>Rapor sorgusu

```sql
SELECT MPNID,PartnerName,CustomerID,DUNSNumber,AccountName,Domain,OrgSize,Industry,Vertical,Area,Subsidiary,
SalesTerritory,City,State,PostalCode,Country,Segment,SubSegment,SMCTypeSummary,TopUnmanagedComputeBase,
TopUnmanagedUserBase,IsNonProfit,MigrateEOSWinServerWithCLASPropensityAbove5Licenses,
MigrateEOSWinServerWithCLASPropensityBelow5Licenses,
MigrateEOSWinServerWithoutCLASPropensityAbove5Licenses,
MigrateEOSWinServerWithoutCLASPropensityBelow5Licenses,MigrateEOSSQLWithCLASPropensityAbove5Licenses,
MigrateEOSSQLWithCLASPropensityBelow5Licenses,MigrateEOSSQLWithoutCLASPropensityAbove5Licenses,
MigrateEOSSQLWithoutCLASPropensityBelow5Licenses,
MigrateOnPremWinServerCurrentWindowsServerWithCLASPropensityAbove5Licenses,
MigrateOnPremWinServerCurrentWindowsServerWithCLASPropensityBelow5Licenses,
MigrateOnPremWinServerCurrentWindowsServerWithoutCLASPropensityAbove5Licenses,
MigrateOnPremWinServerCurrentWindowsServerIBWithoutCLASPropensityBelow5Licenses,
MigrateToAzureSQLOrSQLVMsCurrentSQLServerWithCLASPropensityAbove5Licenses,
MigrateToAzureSQLOrSQLVMsCurrentSQLServerWithCLASPropensityBelow5Licenses,
MigrateToAzureSQLOrSQLVMsCurrentSQLServerWithoutCLASPropensityAbove5Licenses,
MigrateToAzureSQLOrSQLVMsCurrentSQLServerWithoutCLASPropensityBelow5Licenses,MigrateOSSMigrateToOSSDB,
MigrateOSSLinuxOnAzure,MigrateSAPOnAzure,MigrateWVDRDSIB,MigrateWVDCrossSellModernWorkToAzureWVD,
MigrateVMWareIB,MigrateCitrixIB,InnovateAnalyticsPowerBIIBWithHighAzurepropensity,
EnableDevOpsWithGitHubVisualStudioMSDNIB,WinServerStandardVersion,WinServerStandardLicense,
WinServerDataCenterVersion,WinServerDataCenterLicense,AzureFit,AzureIntent,AzureCluster,
WindowsServerDataCenter_HasOpenRenewal,WindowsServerStandard_HasOpenRenewal,AzureUpsellCustomer,HasGoogle,
HasAWS,HasEA,HasOpen 
FROM CLASAzurePropensity
```

## <a name="clas-d365-propensity"></a>CLAS D365 eğilimi

ALTı ay boyunca CLASD365Propensity raporu

Sorgu Kimliği: `258fdcac-6e9c-4072-af27-b1b3d97be16c`

### <a name="report-query"></a>Rapor sorgusu

```sql
SELECT MPNID,PartnerName,CustomerID,DUNSNumber,AccountName,Domain,OrgSize,Industry,Vertical,Area,Subsidiary,
SalesTerritory,City,State,PostalCode,Country,Segment,SubSegment,SMCTypeSummary,TopUnmanagedComputeBase,
TopUnmanagedUserBase,IsNonProfit,ActivateDigitalSellingM365SeatSizeAbove25SeatsSalesProPropensityModel,
ActivateDigitalSellingD365SalesProPropensityActNowOrEvaluate,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseNavisionBCPropensityModel,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseAXFAndOPropensityModel,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseGreatPlainsBCPropensityModel,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseSolomonBCPropensityModel,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseOthersBCPropensityModel,
ManagingFinancialRiskAndFraudNewCustomerAcquisitionFAndOPropensityModel,
ManagingFinancialRiskAndFraudNewCustomerAcquisitionBCPropensityModel,
BuildAgileBusinessProcessesDynamicsOnPremInstallBaseAXGPSLNAVOtherD365PropensityModel,
BuildAgileBusinessProcessesDynamicsCompeteBaseMendixOutsystemsSalesforceD365PropensityModel,
BuildAgileBusinessProcessesD365FAndOInstallBase,BuildAgileBusinessProcessesD365BCInstallBase,
BuildAgileBusinessProcessesD365CEInstallBase,
BuildaResilientSupplyChainWinandActivateFirstD365WorkloadasD365SupplyChainwithNonOracleSAPERPCustomers,
BuildaResilientSupplyChainCrossSellD365SupplyChainANDORRetailCommercetoExistingD365CECustomers,
BuildaResilientSupplyChainCrossSellD365SupChainANDORRetailCommercetoD365CEANDOracleORSAP,D365BCCluster,
D365BCFit,D365BCIntent,D365FOCluster,D365FOFit,D365FOIntent,D365CECluster,D365CEFit,D365CEIntent,
DynamicsOnPremAXorCRM_HasOpenRenewal,M365UpsellCustomer,HasGoogle,HasAWS,HasEA,HasOpen 
FROM CLASD365Propensity
```

## <a name="clas-m365-propensity"></a>CLAS M365 eğilimi

CLASM365Propensity raporu altı ay boyunca

Sorgu Kimliği: `fbe00e32-fdde-4465-b3e4-41bbd021a130`

### <a name="report-query"></a>Rapor sorgusu

```sql
SELECT MPNID,PartnerName,CustomerID,DUNSNumber,AccountName,Domain,OrgSize,Industry,Vertical,Area,Subsidiary,
SalesTerritory,City,State,PostalCode,Country,Segment,SubSegment,SMCTypeSummary,TopUnmanagedComputeBase,
TopUnmanagedUserBase,IsNonProfit,EnableRemoteWorkTargetExchangeOnline,
EnableRemoteWorkOnPremAcquisitionCurrentVersionwithCLASPropensityAbove10Licenses,
EnableRemoteWorkOnPremAcquisitionCurrentVersionwithCLASPropensityBelow10Licenses,
EnableRemoteWorkOnPremAcquisitionCurrentVersionwithoutCLASPropensityAbove10Licenses,
EnableRemoteWorkOnPremAcquisitionCurrentVersionwithoutCLASPropensityBelow10Licenses,
EnableRemoteWorkOnPremAcquisitionEOSwithCLASPropensityAbove10Licenses,
EnableRemoteWorkOnPremAcquisitionEOSwithCLASPropensityBelow10Licenses,
EnableRemoteWorkOnPremAcquisitionEOSwithoutCLASPropensityAbove10Licenses,
EnableRemoteWorkOnPremAcquisitionEOSwithoutCLASPropensityBelow10Licenses,
EnableRemoteWorkHighPropensityProspectforM365ActNowEvaluate,EnableRemoteWorkCompeteZoomwithM365,
EnableRemoteWorkCompeteZoomwithoutM365,ReduceCostandManageM365E3targetedforM365E5,
ReduceCostandManageM365BBandBScustomerstargetedforM365BP,TransformOrganizationalProductivitySurfacePropensity,
M365Cluster,M365Fit,M365Intent,SurfaceCluster,SurfaceFit,SurfaceIntent,O365Cluster,O365Fit,O365Intent,
M365UpsellCustomer,HasGoogle,HasAWS,HasEA,HasOpen 
FROM CLASM365Propensity
```

## <a name="teams-usage-3p-apps"></a>Teams Kullanım 3P Uygulamaları

TeamsUsage3PApps raporu altı ay boyunca

Sorgu Kimliği: `42d287be-cc76-4109-a066-f3140ad97fe2`

### <a name="report-query"></a>Rapor sorgusu

```sql
SELECT CustomerId,CustomerTenantId,CustomerName,CustomerCountry,DateKey,AppName,UserCount 
FROM TeamsUsage3PApps TIMESPAN LAST_6_MONTHS
```

## <a name="teams-usage-workload"></a>Teams iş yükü kullanma

TeamsUsageWorkload raporu altı ay boyunca

Sorgu Kimliği: `817fe875-acb0-4c45-9201-b7a35a60235a`

### <a name="report-query"></a>Rapor sorgusu

```sql
SELECT CustomerId,CustomerTenantId,MonthKey,SubWorkload,DesktopUsers,WebUsers,MobileUsers,AllUpPartiticipants
FROM TeamsUsageWorkload TIMESPAN LAST_6_MONTHS
```

## <a name="teams-usage-meetings-and-calls"></a>Teams toplantılarını ve çağrıları kullanma

TeamsUsageMeetingsAndCalls raporu altı ay boyunca

Sorgu Kimliği: `b7bd73a8-47e8-4c57-b915-445708cfd7bf`

### <a name="report-query"></a>Rapor sorgusu

```sql
SELECT CustomerId,CustomerTenantId,DateKey,SubWorkload,MeetingCount,MeetingDuration 
FROM TeamsUsageMeetingsAndCalls TIMESPAN LAST_6_MONTHS
```

## <a name="competency-summary-history"></a>Uzmanlık özeti geçmişi

CompetencySummaryHistory raporu altı ay boyunca

Sorgu Kimliği: `fddab2aa-523d-47f6-90fe-588557306db4`

### <a name="report-query"></a>Rapor sorgusu

```sql
SELECT CompetencyName,CompetencyLevel,CompetencyStatus,CompetencyStartDate,CompetencyEndDate 
FROM CompetencySummaryHistory TIMESPAN LAST_6_MONTHS
```

## <a name="training-completion"></a>Eğitimin tamamlanması

Altı ay boyunca Eğitim Tamamlamaları raporu

Sorgu Kimliği: `20f5da57-3c2a-481b-b6a0-ec34d6db14e2`

### <a name="report-query"></a>Rapor sorgusu

```sql
SELECT TrainingActivityId,TrainingTitle,TrainingType,AADUserId,TrainingCompletionDate,Month,IcMCP,MCPID,MPNId,
PartnerName,PartnerCityLocation,PartnerCountryLocation 
FROM TrainingCompletions TIMESPAN LAST_6_MONTHS
```

## <a name="microsoft-learn"></a>Microsoft Learn

Microsoft Learn altı aya göre rapor

Sorgu Kimliği: `0e06c7c3-75ab-4cd5-8178-8cf1a2de49cc`

### <a name="report-query"></a>Rapor sorgusu

```sql
SELECT UserName,UserId,TrainingName,TrainingType,Products,Roles,CompletionDate,MPNId,PartnerName,CustomerMarket 
FROM MSLearn TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a>Sonraki adımlar

- [İş ortağı içgörüleri analiz verilerine erişmek için API'ler](insights-programmatic-analytics-available-api.md)
- [İş ortağı içgörüleri analiz verilerine erişmek için örnek uygulama](insights-programmatic-sample-application.md)