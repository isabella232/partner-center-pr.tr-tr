---
title: İş ortağı içgörüleri analiz verilerine erişmek için ilk API çağrınızı yapma
description: İş ortağı içgörüleri analiz verilerine erişmek için API'yi kullanmayı öğrenme örnekleri.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 76fb1b113a44e195114d67d79f192b3c2dce1071b7502f01af20387f69d62a8f
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115697474"
---
# <a name="make-your-first-api-call-to-access-partner-insights-analytics-data"></a>İş ortağı içgörüleri analiz verilerine erişmek için ilk API çağrınızı yapma

İş ortağı içgörüleri analiz verilerine erişmek için API'ler listesi için bkz. İş ortağı [içgörüleri analiz verilerine erişmek için API'ler.](insights-programmatic-analytics-available-api.md) İlk API çağrınızı yapmadan önce, İş [](insights-programmatic-prerequisites.md) Ortağına ve analiz verilerine program aracılığıyla erişmek için önkulları Analizler olun.

## <a name="token-generation"></a>Belirteç oluşturma

Yöntemlerden herhangi birini çağırmadan önce bir Azure Active Directory (AAD) erişim belirteci elde edin. Api'de her yöntemin Yetkilendirme üst bilgisinde Azure AD erişim belirteci geçmeniz gerekir. Erişim belirteci edindikten sonra, süresi dolmadan önce kullanmak için 60 dakika süreniz vardır. Belirteci süresi dolsa da belirteci yeniler ve API'ye yapılan diğer çağrılar için kullanmaya devam edersiniz.

Belirteç oluşturmak için aşağıdaki örnek isteğine bakın. Belirteci oluşturmak için gereken üç değer , `clientId` `clientSecret` ve `tenantId` değerleridir. Kaynak parametresi şu şekilde ayar olmalıdır: `https://api.partnercenter.microsoft.com`

#### <a name="request-example"></a>İstek örneği

```console
curl --location --request POST 'https://login.microsoftonline.com/<tenantId>/oauth2/token' \
--header 'return-client-request-id: true' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Cookie: fpc=Ar2GMei7JwdKg4Y4onHrMpvxqd4FAQAAAEhU_tcOAAAA; stsservicecookie=estsfd; x-ms-gateway-slice=estsfd' \
--data-urlencode 'resource= https://api.partnercenter.microsoft.com' \
--data-urlencode 'client_id= ' \
--data-urlencode 'client_secret= ' \
--data-urlencode 'grant_type=password' \
--data-urlencode 'scope=openid' \
--data-urlencode 'username= ' \
--data-urlencode 'password= '
```

#### <a name="response-example"></a>Yanıt örneği

```json
{
    "token_type": "Bearer",
    "expires_in": "3599",
    "ext_expires_in": "3599",
    "expires_on": "1612794445",
    "not_before": "1612790545",
    "resource": "https://api.partnercenter.microsoft.com",
    "access_token": {Token}
}
```

Uygulamanıza azure AD belirteci alma hakkında daha fazla bilgi için [bkz. Store hizmetlerini kullanarak analiz verilerine erişme.](/windows/uwp/monetize/access-analytics-data-using-windows-store-services#step-2-obtain-an-azure-ad-access-token)

## <a name="programmatic-api-call"></a>Programlı API çağrısı

Önceki bölümde açıklandığı gibi AAD Belirteci'ne sahip olduktan sonra, ilk programlı erişim raporlarınızı oluşturmak için aşağıdaki adımları izleyin.

Veriler aşağıdaki veri kümelerinden (datasetName) indirilebilir:

- CustomersAndTenants
- SeatsSubscriptionsAndRevenue
- AzureUsage
- MSLearn
- OfficeUsage
- Profil
- TrainingCompletions
- DynamicsUsage
- CompetencySummaryHistory
- PowerBIUsage
- EMSUsage
- CompetencyPeformanceRequirement
- ResellerPerformance
- CLASAgreementRenewalsPropensity
- CLASAzurePropensity
- CLASD365Propensity
- CLASM365Propensity
- TeamsUsage3PApps
- TeamsUsageWorkload
- TeamsUsageMeetingsAndCalls

Aşağıdaki bölümde, DynamicsUsage veri kümesinden program aracılığıyla nasıl `SubscriptionId` erişilene örnekler göreceğiz.

### <a name="step-1-make-a-rest-call-using-the-get-datasets-api"></a>1. Adım: Veri kümelerini al API'sini kullanarak REST çağrısı yapma

API yanıtı, raporu indirebilirsiniz veri kümesi adını sağlar. Api yanıtı, belirli bir veri kümesi için özel rapor şablonunuz için değiştirilebilir sütunların listesini de sağlar. Sütunların adlarını almak [için Veri](insights-data-definitions.md) Tanımları'ne de başvurabilirsiniz.

#### <a name="request-example"></a>İstek örneği

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset'\
--header 'Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a>Yanıt örneği

```json
{
  "value": [
    {
      "datasetName": "DynamicsUsage",
      "selectableColumns": [
        "PGAMpnId",
        "SubscriptionId",
        "SubscriptionStartDate",
        "SubscriptionEndDate",
        "SubscriptionStatus",
        "Month",
        "RevSumDivisionName",
        "RevSumCategoryName",
        "SKU",
        "SKUId",
        "FreeVsPaidSKU",
        "SalesModel",
        "DetailedSalesModel",
        "CustomerName",
        "CustomerTenantId",
        "CustomerTpid",
        "CustomerSegment",
        "CustomerMarket",
        "MPNId",
        "PartnerName",
        "PartnerLocation",
        "PartnerAttachType",
        "AvailableSeats",
        "AssignedSeats",
        "ActiveSeats",
        "DeploymentOpportunity",
        "ActiveUsagePercent"
      ],
      "availableMetrics": [
        "SubscriptionCount",
        "TotalAssignedSeats",
        "TotalSoldSeats",
        "TotalActiveSeats",
        "TotalRevenueAndACR",
        "CustomerCount",
        "CustomerTenantCount"
      ],
      "availableDateRanges": [
        "LAST_MONTH",
        "LAST_3_MONTHS",
        "LAST_6_MONTHS",
        "LAST_1_YEAR",
        "LIFETIME"
      ],
      "minimumRecurrenceInterval": 24
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Dataset fetched successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

### <a name="step-2-create-the-custom-query"></a>2. Adım: Özel Sorgu Oluşturma

Bu adımda, DynamicsUsage veri kümesinden SubscriptionId kullanarak istediğiniz rapor için özel bir sorgu oluşturuz. Sorguda belirtilmezse varsayılan zaman süresi 6 aydır.

#### <a name="request-example"></a>İstek örneği

```cli
curl 
--location 
--request POST 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries' \ 
--header ' Authorization: Bearer <AADToken>' \ 
--header 'Content-Type: application/json' \ 
--data-raw 
{
  "Name": "SubscriptionId Dynamics ",
  "Description": "List of Subscription Id from DynamicsUsage",
  "Query": "SELECT SubscriptionId from DynamicsUsage "
            }"
```

#### <a name="response-example"></a>Yanıt örneği

```json
{
  "value": [
    {
      "queryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
      "name": "SubscriptionId Dynamics",
      "description": "List of Subscription Id from DynamicsUsage",
      "query": "SELECT SubscriptionId from DynamicsUsage",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net",
      "createdTime": "2021-03-31T07:28:37Z"
    }
 ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

Sorgunun başarıyla yürütülmesi `queryId` sırasında, raporu oluşturmak için kullanılacak bir oluşturulur.

### <a name="step-3-execute-test-query-api"></a>3. Adım: Test sorgusu API'sini yürütme

Bu adımda, oluşturulan sorgu için ilk 100 satırı almak üzere test sorgusu API'sini kullanıyoruz.

#### <a name="request-example"></a>İstek örneği

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?queryId=7d19305c-56db-4edc-b776-428340e3a9c8' \
--header ' Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a>Yanıt örneği

```json
{
  "value": [
    {
      "SubscriptionId": "251DE3D4-8868-4032-B518-F142DA50522F"
    },
    {
      "SubscriptionId": "758A0647-790C-435B-BEAA-652DF47E327C"
    },
    {
      "SubscriptionId": "ACE5A84B-9794-4480-82C5-AF9462DE2589"
    },
    {
      "SubscriptionId": "C75163EE-A0CA-4822-8275-E29E2490FF1C"
    },
    {
      "SubscriptionId": "082A8A18-0834-4376-A9A4-3AA4ECD02826"
    },
    .
    .
    .
    {
      "SubscriptionId": "5E10B817-7FCB-43CE-9F32-9CB60CF14658"
    },
    {
      "SubscriptionId": "7578872A-18C1-4E6B-8F51-469555337389"
    },
    {
      "SubscriptionId": "00601E10-4C05-4BA2-B977-6578F5C81D69"
    },
    {
      "SubscriptionId": "7EBFC3A9-D502-4EA2-87E7-C42971639E8C"
    },
    {
      "SubscriptionId": "2AC30AE1-5934-48FB-A0E5-EF6985761138"
    }
  ],
  "nextLink": null,
  "totalCount": 100,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

### <a name="step-4-create-the-report"></a>4. Adım: Raporu oluşturma

Bu adımda, raporu oluşturmak için önceden oluşturulmuş QueryId'leri kullanıyoruz.

#### <a name="request-example"></a>İstek örneği

```cli
curl 
--location 
--request POST 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport'\
--header ' Authorization: Bearer <AADToken>' \ 
--header 'Content-Type: application/json' \ 
--data-raw 
'{
  "ReportName": "DynamicsUsage Subscription ID Report",
  "Description": "Report for getting list of Subscription Id for Dynamics Usage",
  "QueryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
  "StartTime": "2021-04-01T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": "2021-03-31T18:41:00Z",
  "QueryEndTime": "2021-06-30T18:41:00Z",
  "RecurrenceInterval": 48,
  "RecurrenceCount": 20,
  "Format": "csv",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}'
```

#### <a name="response-example"></a>Yanıt örneği

```json
{
  "value": [
    {
      "reportId": "cdc61cfe-d028-4333-a215-a1df51ccbfd4",
      "reportName": "DynamicsUsage Subscription ID Report",
      "description": "Report for getting list of Subscription Id for Dynamics Usage",
      "queryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
      "query": "SELECT SubscriptionId from DynamicsUsage",
      "user": "GAUser@PITEST2.ccsctp.net",
      "createdTime": "2021-03-31T08:15:15Z",
      "modifiedTime": null,
      "executeNow": false,
      "startTime": "2021-04-01T18:41:00Z",
      "reportStatus": "Active",
      "recurrenceInterval": 48,
      "recurrenceCount": 20,
      "callbackUrl": "https://<SampleCallbackUrl>",
      "CallbackMethod": "GET",
      "format": "csv"
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Report created successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

Başarılı bir `reportId` yürütmede, raporun indirilmlerini zamanlaması için kullanılacak bir oluşturulur.

### <a name="step-5-execute-report-executions-api"></a>5. Adım: Rapor Yürütme API'sini Yürütme

Bu adımda, raporun güvenli konumunu (URL) almak için Rapor YürütmeLERI API'sini kullanıyoruz.

#### <a name="request-example"></a>İstek örneği

```cli
Curl
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/ cdc61cfe-d028-4333-a215-a1df51ccbfd4?getLatestExecution=true'\
--header ' Authorization: Bearer <AADToken>' \
```

#### <a name="response-example"></a>Yanıt örneği

```json
{
  "value": [
    {
      "executionId": "315eb63e-e2b2-41a2-ad8e-790b040fdce3",
      "reportId": "cdc61cfe-d028-4333-a215-a1df51ccbfd4",
      "recurrenceInterval": 48,
      "recurrenceCount": 20,
      "callbackUrl": null,
      "CallbackMethod": null,
      "format": "csv",
      "executionStatus": "Pending",
      "reportLocation": null,
      "reportAccessSecureLink": null,
      "reportExpiryTime": null,
      "reportGeneratedTime": null
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

## <a name="next-steps"></a>Sonraki adımlar

- [Swagger API URL'si aracılığıyla API'leri deneyin](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)