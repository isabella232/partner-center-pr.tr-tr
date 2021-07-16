---
title: Analizler verileri için programlı erişim paradigması
description: Programlı analizler için API çağrı deseninin üst düzey akışını anlayın. Partner Insights Analytics raporlarına erişim API 'Leri de ele alınmıştır.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: dcdd54fcc744fdb1683259203188c309a3949eff
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376984"
---
# <a name="programmatic-access-paradigm"></a><span data-ttu-id="0d4b1-104">Programlı erişim paradigması</span><span class="sxs-lookup"><span data-stu-id="0d4b1-104">Programmatic access paradigm</span></span>

<span data-ttu-id="0d4b1-105">Bu diyagramda yeni bir rapor şablonu oluşturmak için kullanılan API çağrı deseninin yanı sıra özel rapor zamanlanır ve hata verileri alınır.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-105">This diagram shows the API call pattern used to create a new report template, schedule the custom report and retrieve failure data.</span></span>

:::image type="content" source="images/insights/prog-acc-paradigm.png" alt-text="Üst düzey akış":::
<span data-ttu-id="0d4b1-107">***Şekil 1: API çağrı deseninin yüksek düzey akışı***</span><span class="sxs-lookup"><span data-stu-id="0d4b1-107">***Figure 1: High level flow of the API call pattern***</span></span>

<span data-ttu-id="0d4b1-108">Bu liste Şekil 1 hakkında daha fazla ayrıntı sağlar.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-108">This list provides more details about Figure 1.</span></span>

1. <span data-ttu-id="0d4b1-109">Istemci uygulaması, [rapor sorgusu oluştur API](#create-report-query-api)'sini çağırarak özel rapor şemasını/şablonunu tanımlayabilir.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-109">The Client Application can define the custom report schema/template by calling the [Create Report Query API](#create-report-query-api).</span></span> <span data-ttu-id="0d4b1-110">Alternatif olarak, burada listelenen rapor şablonu kitaplık örneklerinden bir rapor şablonu (QueryId) seçebilirsiniz [.](insights-programmatic-system-queries.md)</span><span class="sxs-lookup"><span data-stu-id="0d4b1-110">Alternately, you can pick a report template (QueryId) from the report template library samples listed [here.](insights-programmatic-system-queries.md)</span></span>
2. <span data-ttu-id="0d4b1-111">Başarılı olduğunda rapor sorgusu oluştur API 'SI QueryId döndürür.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-111">On success, the Create Report Query API returns the QueryId.</span></span>
3. <span data-ttu-id="0d4b1-112">Daha sonra istemci uygulamasının rapor başlangıç tarihi, yineleme aralığı, yinelenme ve isteğe bağlı bir geri çağırma URI 'SI ile birlikte QueryId kullanarak [rapor oluşturma API](#create-report-api) 'sini çağırması gerekir.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-112">The client application then needs to call the [Create Report API](#create-report-api) using the QueryId along with the report start date, Repeat Interval, Recurrence, and an optional Callback URI.</span></span>
4. <span data-ttu-id="0d4b1-113">Başarı durumunda [rapor oluşturma API 'Si](#create-report-api) REPORTID ' yi döndürür.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-113">On Success, the [Create Report API](#create-report-api) returns the ReportId.</span></span>
5. <span data-ttu-id="0d4b1-114">İstemci uygulaması, rapor verileri indirilmeye uygun hale geldiğinde geri çağırma URL 'sinden bildirim alır.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-114">The client application gets notified at the callback URL as soon as the report data is ready for download.</span></span>
6. <span data-ttu-id="0d4b1-115">İstemci uygulaması daha sonra rapor KIMLIĞI ve tarih aralığı ile raporun durumunu sorgulamak için [rapor yürütmeleri al API](#get-report-execution-api) 'sini kullanır.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-115">The client application then uses the [Get Report Executions API](#get-report-execution-api) to query the status of the report with the Report ID and date range.</span></span>
7. <span data-ttu-id="0d4b1-116">Başarı durumunda, rapor indirme bağlantısı döndürülür ve uygulama verilerin indirilmesini başlatabilir.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-116">On success, the report download link is returned and the application can initiate download of the data.</span></span>

## <a name="report-query-language-specification"></a><span data-ttu-id="0d4b1-117">Rapor sorgusu dil belirtimi</span><span class="sxs-lookup"><span data-stu-id="0d4b1-117">Report query language specification</span></span>

<span data-ttu-id="0d4b1-118">Raporları oluşturmak için kullanabileceğiniz [Sistem sorguları](insights-programmatic-system-queries.md) sağlamamız sırasında, iş gereksinimlerinize göre kendi sorgularınızı de oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-118">While we do provide [system queries](insights-programmatic-system-queries.md) you can use to create reports, you can also create your own queries based on your business needs.</span></span> <span data-ttu-id="0d4b1-119">Özel sorgular hakkında daha fazla bilgi için bkz. [özel sorgu belirtimi](insights-programmatic-custom-query.md).</span><span class="sxs-lookup"><span data-stu-id="0d4b1-119">To learn more about custom queries, see [Custom Query Specification](insights-programmatic-custom-query.md).</span></span>

## <a name="create-report-query-api"></a><span data-ttu-id="0d4b1-120">Rapor sorgu API 'SI oluştur</span><span class="sxs-lookup"><span data-stu-id="0d4b1-120">Create report query API</span></span>

<span data-ttu-id="0d4b1-121">API, hangi sütunların ve ölçümlerin verilmesi gereken veri kümesini tanımlayan özel sorgular oluşturmaya yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-121">The API helps to create custom queries that define the dataset from which columns and metrics need to be exported.</span></span> <span data-ttu-id="0d4b1-122">API, iş gereksinimlerinize göre yeni bir raporlama şablonu oluşturma esnekliğini sağlar.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-122">The API provides the flexibility to create a new reporting template based on your business needs.</span></span>  

<span data-ttu-id="0d4b1-123">Sağladığımız [sistem sorgularını](insights-programmatic-system-queries.md) da kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-123">You can also use the [system queries](insights-programmatic-system-queries.md) we provide.</span></span> <span data-ttu-id="0d4b1-124">Özel rapor şablonları gerekli olmadığında, sağlanmış sistem sorgularının QueryIds değerlerini kullanarak doğrudan [Create Report API](#create-report-api) çağırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-124">When custom report templates are not needed, you can call [Create Report API](#create-report-api) directly using the QueryIds of the system queries that are provided.</span></span>  

<span data-ttu-id="0d4b1-125">Aşağıdaki örnek, son ayın gelirine göre ilk 10 müşteriyi almak için özel bir sorgu oluşturmayı gösterir.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-125">The following example shows how to create a custom query to get top 10 customers by revenue for last month.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="0d4b1-126">İstek sözdizimi</span><span class="sxs-lookup"><span data-stu-id="0d4b1-126">Request syntax</span></span>

|    <span data-ttu-id="0d4b1-127">Yöntem</span><span class="sxs-lookup"><span data-stu-id="0d4b1-127">Method</span></span>     |    <span data-ttu-id="0d4b1-128">İstek URI'si</span><span class="sxs-lookup"><span data-stu-id="0d4b1-128">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="0d4b1-129">POST</span><span class="sxs-lookup"><span data-stu-id="0d4b1-129">POST</span></span>     |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries`|
|||

### <a name="request-header"></a><span data-ttu-id="0d4b1-130">İstek üst bilgisi</span><span class="sxs-lookup"><span data-stu-id="0d4b1-130">Request header</span></span>

|    <span data-ttu-id="0d4b1-131">Üst bilgi</span><span class="sxs-lookup"><span data-stu-id="0d4b1-131">Header</span></span>     |    <span data-ttu-id="0d4b1-132">Tür</span><span class="sxs-lookup"><span data-stu-id="0d4b1-132">Type</span></span>     |    <span data-ttu-id="0d4b1-133">Açıklama</span><span class="sxs-lookup"><span data-stu-id="0d4b1-133">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="0d4b1-134">Yetkilendirme</span><span class="sxs-lookup"><span data-stu-id="0d4b1-134">Authorization</span></span>     |    <span data-ttu-id="0d4b1-135">string</span><span class="sxs-lookup"><span data-stu-id="0d4b1-135">string</span></span> |<span data-ttu-id="0d4b1-136">Gereklidir.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-136">Required.</span></span> <span data-ttu-id="0d4b1-137">Azure Active Directory (Azure AD) erişim belirteci.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-137">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="0d4b1-138">Biçim  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="0d4b1-138">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="0d4b1-139">İçerik Türü</span><span class="sxs-lookup"><span data-stu-id="0d4b1-139">Content-Type</span></span>     |<span data-ttu-id="0d4b1-140">string</span><span class="sxs-lookup"><span data-stu-id="0d4b1-140">string</span></span> |`Application/JSON` |
||||

### <a name="path-parameter"></a><span data-ttu-id="0d4b1-141">Yol parametresi</span><span class="sxs-lookup"><span data-stu-id="0d4b1-141">Path parameter</span></span>

<span data-ttu-id="0d4b1-142">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="0d4b1-142">None</span></span>

### <a name="query-parameter"></a><span data-ttu-id="0d4b1-143">Sorgu parametresi</span><span class="sxs-lookup"><span data-stu-id="0d4b1-143">Query parameter</span></span>

<span data-ttu-id="0d4b1-144">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="0d4b1-144">None</span></span>

### <a name="sample-request-payload"></a><span data-ttu-id="0d4b1-145">Örnek istek yükü</span><span class="sxs-lookup"><span data-stu-id="0d4b1-145">Sample request payload</span></span>

```json
{ 
  "Name": "CustomersRevenueQuery", 
  "Description": "Query to get top 10 customers by revenue for last month", 
  "Query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH" 
}
```

### <a name="glossary"></a><span data-ttu-id="0d4b1-146">Sözlük</span><span class="sxs-lookup"><span data-stu-id="0d4b1-146">Glossary</span></span>

<span data-ttu-id="0d4b1-147">Bu tablo, istek yükünde öğelerin temel tanımlarını sağlar.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-147">This table provides the key definitions of elements in the request payload.</span></span>

|<span data-ttu-id="0d4b1-148">Parametre</span><span class="sxs-lookup"><span data-stu-id="0d4b1-148">Parameter</span></span>|    <span data-ttu-id="0d4b1-149">Gerekli</span><span class="sxs-lookup"><span data-stu-id="0d4b1-149">Required</span></span>     |    <span data-ttu-id="0d4b1-150">Açıklama</span><span class="sxs-lookup"><span data-stu-id="0d4b1-150">Description</span></span>     |    <span data-ttu-id="0d4b1-151">İzin Verilen Değerler</span><span class="sxs-lookup"><span data-stu-id="0d4b1-151">Allowed Values</span></span>     |
|-----|    -----    |    -----    |    -----    |
|<span data-ttu-id="0d4b1-152">Name</span><span class="sxs-lookup"><span data-stu-id="0d4b1-152">Name</span></span> |    <span data-ttu-id="0d4b1-153">Yes</span><span class="sxs-lookup"><span data-stu-id="0d4b1-153">Yes</span></span>     |    <span data-ttu-id="0d4b1-154">Sorgunun kolay adı</span><span class="sxs-lookup"><span data-stu-id="0d4b1-154">Friendly name of the query</span></span>     |    <span data-ttu-id="0d4b1-155">string</span><span class="sxs-lookup"><span data-stu-id="0d4b1-155">string</span></span>     |
|    <span data-ttu-id="0d4b1-156">Açıklama</span><span class="sxs-lookup"><span data-stu-id="0d4b1-156">Description</span></span>     |    <span data-ttu-id="0d4b1-157">Hayır</span><span class="sxs-lookup"><span data-stu-id="0d4b1-157">No</span></span>     |    <span data-ttu-id="0d4b1-158">Sorgunun döndürdüğü açıklama</span><span class="sxs-lookup"><span data-stu-id="0d4b1-158">Description of what the query returns</span></span>     |    <span data-ttu-id="0d4b1-159">string</span><span class="sxs-lookup"><span data-stu-id="0d4b1-159">string</span></span>     |
|    <span data-ttu-id="0d4b1-160">Sorgu</span><span class="sxs-lookup"><span data-stu-id="0d4b1-160">Query</span></span>     |    <span data-ttu-id="0d4b1-161">Yes</span><span class="sxs-lookup"><span data-stu-id="0d4b1-161">Yes</span></span>     |    <span data-ttu-id="0d4b1-162">Rapor sorgu dizesi</span><span class="sxs-lookup"><span data-stu-id="0d4b1-162">Report query string</span></span>     |    <span data-ttu-id="0d4b1-163">Veri türü: dize</span><span class="sxs-lookup"><span data-stu-id="0d4b1-163">Data type: string</span></span> <br> <span data-ttu-id="0d4b1-164">İş gereksinimini temel alan [özel sorgu](insights-programmatic-custom-query.md)</span><span class="sxs-lookup"><span data-stu-id="0d4b1-164">[Custom query](insights-programmatic-custom-query.md) based on business need</span></span> |
|        |        |        |        |

> [!Note]
> <span data-ttu-id="0d4b1-165">Özel sorgu örnekleri için bkz [. örnek sorgu örnekleri.](insights-programmatic-sample-queries.md)</span><span class="sxs-lookup"><span data-stu-id="0d4b1-165">For custom query samples, see [Examples of sample queries.](insights-programmatic-sample-queries.md)</span></span>

### <a name="sample-response"></a><span data-ttu-id="0d4b1-166">Örnek yanıt</span><span class="sxs-lookup"><span data-stu-id="0d4b1-166">Sample response</span></span>

<span data-ttu-id="0d4b1-167">Yanıt yükü aşağıdaki şekilde yapılandırılır:</span><span class="sxs-lookup"><span data-stu-id="0d4b1-167">The response payload is structured as follows:</span></span>

<span data-ttu-id="0d4b1-168">Yanıt kodları: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="0d4b1-168">Response Codes: 200, 400, 401, 403, 500</span></span>

<span data-ttu-id="0d4b1-169">Yanıt yükü örneği:</span><span class="sxs-lookup"><span data-stu-id="0d4b1-169">Response payload example:</span></span>

```json
{ 
  "value": [ 
    { 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
      "name": "CustomersRevenueQuery",
      "description": "Query to get top 10 customers by revenue for last month",
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T12:52:39Z" 
    }
  ], 
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
} 
```

### <a name="glossary"></a><span data-ttu-id="0d4b1-170">Sözlük</span><span class="sxs-lookup"><span data-stu-id="0d4b1-170">Glossary</span></span>

<span data-ttu-id="0d4b1-171">Bu tablo, istek yükünde öğelerin temel tanımlarını sağlar.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-171">This table provides the key definitions of elements in the request payload.</span></span>

|    <span data-ttu-id="0d4b1-172">Parametre</span><span class="sxs-lookup"><span data-stu-id="0d4b1-172">Parameter</span></span>     |    <span data-ttu-id="0d4b1-173">Açıklama</span><span class="sxs-lookup"><span data-stu-id="0d4b1-173">Description</span></span>     |
|    ----    |    ----    |
|    <span data-ttu-id="0d4b1-174">QueryId</span><span class="sxs-lookup"><span data-stu-id="0d4b1-174">QueryId</span></span>     |    <span data-ttu-id="0d4b1-175">Oluşturduğunuz sorgunun evrensel benzersiz tanımlayıcısı (UUID)</span><span class="sxs-lookup"><span data-stu-id="0d4b1-175">Universally unique identifier (UUID) of the query you created</span></span>     |
|    <span data-ttu-id="0d4b1-176">Name</span><span class="sxs-lookup"><span data-stu-id="0d4b1-176">Name</span></span>     |    <span data-ttu-id="0d4b1-177">İstek yükünde sorguya kolay ad verildi</span><span class="sxs-lookup"><span data-stu-id="0d4b1-177">Friendly name given to the query in the request payload</span></span>     |
|    <span data-ttu-id="0d4b1-178">Açıklama</span><span class="sxs-lookup"><span data-stu-id="0d4b1-178">Description</span></span>     |    <span data-ttu-id="0d4b1-179">Sorgunun oluşturulması sırasında verilen açıklama</span><span class="sxs-lookup"><span data-stu-id="0d4b1-179">Description given during creation of the query</span></span>     |
|    <span data-ttu-id="0d4b1-180">Sorgu</span><span class="sxs-lookup"><span data-stu-id="0d4b1-180">Query</span></span>     |    <span data-ttu-id="0d4b1-181">Sorgu oluşturma sırasında rapor sorgusu giriş olarak geçildi</span><span class="sxs-lookup"><span data-stu-id="0d4b1-181">Report query passed as input during query creation</span></span>     |
|    <span data-ttu-id="0d4b1-182">Tür</span><span class="sxs-lookup"><span data-stu-id="0d4b1-182">Type</span></span>     |    <span data-ttu-id="0d4b1-183">Ayarla `userDefined`</span><span class="sxs-lookup"><span data-stu-id="0d4b1-183">Set to `userDefined`</span></span>     |
|    <span data-ttu-id="0d4b1-184">Kullanıcı</span><span class="sxs-lookup"><span data-stu-id="0d4b1-184">User</span></span>     |    <span data-ttu-id="0d4b1-185">Sorgu oluşturmak için kullanılan Kullanıcı KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="0d4b1-185">User ID used to create of the query</span></span>     |
|    <span data-ttu-id="0d4b1-186">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="0d4b1-186">CreatedTime</span></span>     |    <span data-ttu-id="0d4b1-187">Sorgunun oluşturulduğu UTC saati: yyyy-MM-ddTHH: mm: ssZ</span><span class="sxs-lookup"><span data-stu-id="0d4b1-187">UTC Time the query was created in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="0d4b1-188">TotalCount</span><span class="sxs-lookup"><span data-stu-id="0d4b1-188">TotalCount</span></span>     |    <span data-ttu-id="0d4b1-189">Değer dizisindeki veri kümesi sayısı</span><span class="sxs-lookup"><span data-stu-id="0d4b1-189">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="0d4b1-190">Durum</span><span class="sxs-lookup"><span data-stu-id="0d4b1-190">StatusCode</span></span>     |    <span data-ttu-id="0d4b1-191">Sonuç Kodu</span><span class="sxs-lookup"><span data-stu-id="0d4b1-191">Result Code</span></span> <br> <span data-ttu-id="0d4b1-192">Olası değerler 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="0d4b1-192">The possible values are 200, 400, 401, 403, 500</span></span>     |
|    <span data-ttu-id="0d4b1-193">message</span><span class="sxs-lookup"><span data-stu-id="0d4b1-193">message</span></span>     |    <span data-ttu-id="0d4b1-194">API 'nin yürütülmesindeki durum iletisi</span><span class="sxs-lookup"><span data-stu-id="0d4b1-194">Status message from the execution of the API</span></span>     |
|        |        |

## <a name="create-report-api"></a><span data-ttu-id="0d4b1-195">Rapor API 'SI oluştur</span><span class="sxs-lookup"><span data-stu-id="0d4b1-195">Create report API</span></span>

<span data-ttu-id="0d4b1-196">Özel rapor şablonu oluşturma ve sorgu yanıtı [oluşturma](#create-report-query-api) ' nın bir parçası olarak QueryId alma sırasında, bu API, düzenli aralıklarla yürütülecek bir sorgu zamanlamak için çağrılabilir.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-196">On creating a custom report template successfully and receiving the QueryID as part of [Create Report Query](#create-report-query-api) response, this API can be called to schedule a query to be executed at regular intervals.</span></span> <span data-ttu-id="0d4b1-197">Raporun teslim edileceği sıklığı ve zamanlamayı ayarlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-197">You can set a frequency and schedule for the report to be delivered.</span></span>
<span data-ttu-id="0d4b1-198">Sağladığımız sistem sorguları için, rapor oluşturma API 'SI de [QueryId](insights-programmatic-system-queries.md)ile çağrılabilir.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-198">For system queries we provide, the Create Report API can also be called with [QueryId](insights-programmatic-system-queries.md).</span></span>

### <a name="callback-url"></a><span data-ttu-id="0d4b1-199">Geri Çağırma URL’si</span><span class="sxs-lookup"><span data-stu-id="0d4b1-199">Callback URL</span></span>

<span data-ttu-id="0d4b1-200">Rapor oluşturma API 'si bir geri çağırma URL 'sini kabul eder.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-200">The create report API accepts a callback URL.</span></span> <span data-ttu-id="0d4b1-201">Rapor oluşturma başarılı olduktan sonra bu URL çağrılır.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-201">This URL will be called once the report generation is successful.</span></span> <span data-ttu-id="0d4b1-202">Geri çağırma URL'sinin genel olarak erişilebilir olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-202">The callback URL should be publicly reachable.</span></span> <span data-ttu-id="0d4b1-203">URL'ye ek olarak bir geri çağırma yöntemi de verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-203">In addition to the URL a callback method can also be given.</span></span> <span data-ttu-id="0d4b1-204">Geri çağırma yöntemi yalnızca "GET" veya "POST" olabilir.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-204">The callback method can only be "GET" or "POST".</span></span> <span data-ttu-id="0d4b1-205">Hiçbir değer geçirilse varsayılan yöntem "POST" olur.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-205">The default method if no value is passed will be "POST".</span></span> <span data-ttu-id="0d4b1-206">Oluşturmayı tamamlayan reportId her zaman geri çağırma sırasında geri geçiri.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-206">The reportId that has completed generation will always be passed back during the callback.</span></span>

<span data-ttu-id="0d4b1-207">POST geri çağırma: Geçirilen URL `https://www.contosso.com/callback` ise, geri çağrılır URL şu şekilde olur: `https://www.contosso.com/callback/<reportID>`</span><span class="sxs-lookup"><span data-stu-id="0d4b1-207">POST callback: If the URL passed was `https://www.contosso.com/callback`, then the called back URL will be `https://www.contosso.com/callback/<reportID>`</span></span> 

<span data-ttu-id="0d4b1-208">GET geri çağırma: Geçirilen URL `https://www.contosso.com/callback` ise, geri çağrılır URL şu şekilde olur: `https://www.contosso.com/callback?reportId=<reportID>`</span><span class="sxs-lookup"><span data-stu-id="0d4b1-208">GET callback: If the URL passed was `https://www.contosso.com/callback`, then the called back URL will be `https://www.contosso.com/callback?reportId=<reportID>`</span></span> 

### <a name="executenow-reports"></a><span data-ttu-id="0d4b1-209">ExecuteNow raporları</span><span class="sxs-lookup"><span data-stu-id="0d4b1-209">ExecuteNow reports</span></span>

<span data-ttu-id="0d4b1-210">Zamanlama olmadan rapor oluşturmak için bir sağlama vardır.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-210">There is a provision to generate a report without scheduling.</span></span> <span data-ttu-id="0d4b1-211">Rapor oluşturma API yükü bir parametresini kabul eder. Bu parametre, API çağrılır oluşturulmaz rapor `ExecuteNow` oluşturulur.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-211">The report create API payload can accept a parameter `ExecuteNow`, which will enqueue the report to be generated as soon as the API is called.</span></span> <span data-ttu-id="0d4b1-212">true olarak ayarlandığı zaman, şu raporlar zamanlanmaz çünkü , alanları `ExecuteNow` `StartTime` `RecurrenceCount` `RecurrenceInterval` yoksayılır.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-212">When `ExecuteNow` is set to true, the fields: `StartTime`, `RecurrenceCount`, `RecurrenceInterval` are ignored as these reports are not scheduled.</span></span>

<span data-ttu-id="0d4b1-213">true olduğunda ve olmak için `ExecuteNow` iki ek alan `QueryStartTime` `QueryEndTime` geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-213">Two additional fields can be passed when `ExecuteNow` is true, `QueryStartTime` and `QueryEndTime`.</span></span> <span data-ttu-id="0d4b1-214">Bu iki alan sorguda `TIMESPAN` alanı geçersiz kılar.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-214">These two fields will override the `TIMESPAN` field in the query.</span></span> <span data-ttu-id="0d4b1-215">Veriler değişmeden sabit bir süre için sürekli olarak oluşturulacak olan zamanlanmış raporlar için bu alanlar geçerli değildir.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-215">These fields are not applicable for scheduled reports as data will get continuously generated for a fixed time period that does not change.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="0d4b1-216">İstek söz dizimi</span><span class="sxs-lookup"><span data-stu-id="0d4b1-216">Request syntax</span></span>

|    <span data-ttu-id="0d4b1-217">Yöntem</span><span class="sxs-lookup"><span data-stu-id="0d4b1-217">Method</span></span>     |    <span data-ttu-id="0d4b1-218">İstek URI'si</span><span class="sxs-lookup"><span data-stu-id="0d4b1-218">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="0d4b1-219">POST</span><span class="sxs-lookup"><span data-stu-id="0d4b1-219">POST</span></span>     |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport` |

### <a name="request-header"></a><span data-ttu-id="0d4b1-220">İstek üst bilgisi</span><span class="sxs-lookup"><span data-stu-id="0d4b1-220">Request header</span></span>

|    <span data-ttu-id="0d4b1-221">Üst bilgi</span><span class="sxs-lookup"><span data-stu-id="0d4b1-221">Header</span></span>     |    <span data-ttu-id="0d4b1-222">Tür</span><span class="sxs-lookup"><span data-stu-id="0d4b1-222">Type</span></span>     |    <span data-ttu-id="0d4b1-223">Açıklama</span><span class="sxs-lookup"><span data-stu-id="0d4b1-223">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="0d4b1-224">Yetkilendirme</span><span class="sxs-lookup"><span data-stu-id="0d4b1-224">Authorization</span></span>     |    <span data-ttu-id="0d4b1-225">string</span><span class="sxs-lookup"><span data-stu-id="0d4b1-225">string</span></span> |<span data-ttu-id="0d4b1-226">Gereklidir.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-226">Required.</span></span> <span data-ttu-id="0d4b1-227">Azure Active Directory (Azure AD) erişim belirteci.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-227">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="0d4b1-228">Biçimi şu  `Bearer <token>` şekildedir: .</span><span class="sxs-lookup"><span data-stu-id="0d4b1-228">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="0d4b1-229">İçerik Türü</span><span class="sxs-lookup"><span data-stu-id="0d4b1-229">Content-Type</span></span>     |<span data-ttu-id="0d4b1-230">string</span><span class="sxs-lookup"><span data-stu-id="0d4b1-230">string</span></span> |`Application/JSON` |

### <a name="path-parameter"></a><span data-ttu-id="0d4b1-231">Yol Parametresi</span><span class="sxs-lookup"><span data-stu-id="0d4b1-231">Path Parameter</span></span>

<span data-ttu-id="0d4b1-232">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="0d4b1-232">None</span></span>

### <a name="query-parameter"></a><span data-ttu-id="0d4b1-233">Sorgu Parametresi</span><span class="sxs-lookup"><span data-stu-id="0d4b1-233">Query Parameter</span></span>

<span data-ttu-id="0d4b1-234">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="0d4b1-234">None</span></span>

### <a name="sample-request-payload"></a><span data-ttu-id="0d4b1-235">Örnek istek yükü</span><span class="sxs-lookup"><span data-stu-id="0d4b1-235">Sample request payload</span></span>

```json
{
  "ReportName": "Top10_CustomersReport",
  "Description": "Top 10 customers by revenue for last month",
  "QueryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
  "StartTime": "2021-03-31T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": null,
  "QueryEndTime": null,
  "RecurrenceInterval": 24,
  "RecurrenceCount": 100,
  "Format": "CSV",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}
```

### <a name="glossary"></a><span data-ttu-id="0d4b1-236">Sözlük</span><span class="sxs-lookup"><span data-stu-id="0d4b1-236">Glossary</span></span>

<span data-ttu-id="0d4b1-237">İstek yükünde öğelerin anahtar tanımları aşağıda açıklanmıştır:</span><span class="sxs-lookup"><span data-stu-id="0d4b1-237">Key definitions of elements in the request payload are articulated below:</span></span>

|    <span data-ttu-id="0d4b1-238">Parametre</span><span class="sxs-lookup"><span data-stu-id="0d4b1-238">Parameter</span></span>     |    <span data-ttu-id="0d4b1-239">Gerekli</span><span class="sxs-lookup"><span data-stu-id="0d4b1-239">Required</span></span>     |    <span data-ttu-id="0d4b1-240">Açıklama</span><span class="sxs-lookup"><span data-stu-id="0d4b1-240">Description</span></span>     |    <span data-ttu-id="0d4b1-241">İzin Verilen Değerler</span><span class="sxs-lookup"><span data-stu-id="0d4b1-241">Allowed Values</span></span>     |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="0d4b1-242">Raporadı</span><span class="sxs-lookup"><span data-stu-id="0d4b1-242">ReportName</span></span>     |    <span data-ttu-id="0d4b1-243">Yes</span><span class="sxs-lookup"><span data-stu-id="0d4b1-243">Yes</span></span>     |    <span data-ttu-id="0d4b1-244">Rapora atanacak ad</span><span class="sxs-lookup"><span data-stu-id="0d4b1-244">Name to be assigned to the report</span></span>     |    <span data-ttu-id="0d4b1-245">string</span><span class="sxs-lookup"><span data-stu-id="0d4b1-245">string</span></span>     |
|    <span data-ttu-id="0d4b1-246">Açıklama</span><span class="sxs-lookup"><span data-stu-id="0d4b1-246">Description</span></span>     |    <span data-ttu-id="0d4b1-247">Hayır</span><span class="sxs-lookup"><span data-stu-id="0d4b1-247">No</span></span>     |    <span data-ttu-id="0d4b1-248">Oluşturulan raporun açıklaması</span><span class="sxs-lookup"><span data-stu-id="0d4b1-248">Description of the created report</span></span>     |    <span data-ttu-id="0d4b1-249">string</span><span class="sxs-lookup"><span data-stu-id="0d4b1-249">string</span></span>     |
|    <span data-ttu-id="0d4b1-250">Queryıd</span><span class="sxs-lookup"><span data-stu-id="0d4b1-250">QueryId</span></span>     |    <span data-ttu-id="0d4b1-251">Yes</span><span class="sxs-lookup"><span data-stu-id="0d4b1-251">Yes</span></span>     |    <span data-ttu-id="0d4b1-252">Rapor sorgusu kimliği</span><span class="sxs-lookup"><span data-stu-id="0d4b1-252">Report query ID</span></span>     |    <span data-ttu-id="0d4b1-253">string</span><span class="sxs-lookup"><span data-stu-id="0d4b1-253">string</span></span>     |
|    <span data-ttu-id="0d4b1-254">StartTime</span><span class="sxs-lookup"><span data-stu-id="0d4b1-254">StartTime</span></span>     |    <span data-ttu-id="0d4b1-255">Yes</span><span class="sxs-lookup"><span data-stu-id="0d4b1-255">Yes</span></span>     |    <span data-ttu-id="0d4b1-256">Rapor oluşturmanın başlayacağı UTC Zaman Damgası.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-256">UTC Timestamp at which the report generation will begin.</span></span> <br> <span data-ttu-id="0d4b1-257">Biçim şu şekilde olmalıdır: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="0d4b1-257">The format should be: yyyy-MM-ddTHH:mm:ssZ</span></span>       |    <span data-ttu-id="0d4b1-258">string</span><span class="sxs-lookup"><span data-stu-id="0d4b1-258">string</span></span>     |
|    <span data-ttu-id="0d4b1-259">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="0d4b1-259">ExecuteNow</span></span>     |    <span data-ttu-id="0d4b1-260">Hayır</span><span class="sxs-lookup"><span data-stu-id="0d4b1-260">No</span></span>     |    <span data-ttu-id="0d4b1-261">Bu parametre, yalnızca bir kez yürütülecek bir rapor oluşturmak için kullanılmalıdır.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-261">This parameter should be used to create a report that will be executed only once.</span></span> <span data-ttu-id="0d4b1-262">`StartTime`, `RecurrenceInterval` ve , true olarak `RecurrenceCount` ayarlanırsa yoksayılır.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-262">`StartTime`, `RecurrenceInterval` and `RecurrenceCount` are ignored if this is set to true.</span></span> <span data-ttu-id="0d4b1-263">Rapor hemen zaman uyumsuz bir şekilde yürütülür</span><span class="sxs-lookup"><span data-stu-id="0d4b1-263">The report is executed immediately in an asynchronous fashion</span></span>     |    <span data-ttu-id="0d4b1-264">true/false</span><span class="sxs-lookup"><span data-stu-id="0d4b1-264">true/false</span></span>     |
|    <span data-ttu-id="0d4b1-265">QueryStartTime</span><span class="sxs-lookup"><span data-stu-id="0d4b1-265">QueryStartTime</span></span>     |    <span data-ttu-id="0d4b1-266">Hayır</span><span class="sxs-lookup"><span data-stu-id="0d4b1-266">No</span></span>     |    <span data-ttu-id="0d4b1-267">İsteğe bağlı olarak, verileri ayıklanan sorgunun başlangıç saati belirtir.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-267">Optionally specifies the start time for the query extracting the data.</span></span> <span data-ttu-id="0d4b1-268">Bu parametre yalnızca true olarak ayarlanmış bir kez yürütme `ExecuteNow` raporu için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-268">This parameter is applicable only for one time execution report that have `ExecuteNow` set to true.</span></span> <span data-ttu-id="0d4b1-269">Sorguda verilen bu parametre `TIMESPAN` geçersiz kılmalarını ayarlama.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-269">Setting this parameter overrides `TIMESPAN` given in the query.</span></span> <span data-ttu-id="0d4b1-270">Biçim yyyy-MM-ddTHH:mm:ssZ olmalıdır</span><span class="sxs-lookup"><span data-stu-id="0d4b1-270">The format should be yyyy-MM-ddTHH:mm:ssZ</span></span>     |    <span data-ttu-id="0d4b1-271">Dize olarak zaman damgası</span><span class="sxs-lookup"><span data-stu-id="0d4b1-271">Timestamp as string</span></span>     |
|    <span data-ttu-id="0d4b1-272">QueryEndTime</span><span class="sxs-lookup"><span data-stu-id="0d4b1-272">QueryEndTime</span></span>     |    <span data-ttu-id="0d4b1-273">Hayır</span><span class="sxs-lookup"><span data-stu-id="0d4b1-273">No</span></span>     |    <span data-ttu-id="0d4b1-274">İsteğe bağlı olarak, verileri ayıklanan sorgunun bitiş saati belirtir.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-274">Optionally specifies the end time for the query extracting the data.</span></span> <span data-ttu-id="0d4b1-275">Bu parametre yalnızca true olarak ayarlanmış bir kez yürütme `ExecuteNow` raporu için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-275">This parameter is applicable only for one time execution report that have `ExecuteNow` set to true.</span></span> <span data-ttu-id="0d4b1-276">Sorguda verilen bu parametre `TIMESPAN` geçersiz kılmalarını ayarlama.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-276">Setting this parameter overrides `TIMESPAN` given in the query.</span></span> <span data-ttu-id="0d4b1-277">Biçim yyyy-MM-ddTHH:mm:ssZ olmalıdır</span><span class="sxs-lookup"><span data-stu-id="0d4b1-277">The format should be yyyy-MM-ddTHH:mm:ssZ</span></span>     |    <span data-ttu-id="0d4b1-278">Dize olarak zaman damgası</span><span class="sxs-lookup"><span data-stu-id="0d4b1-278">Timestamp as string</span></span>     |
|    <span data-ttu-id="0d4b1-279">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="0d4b1-279">RecurrenceInterval</span></span>     |    <span data-ttu-id="0d4b1-280">Yes</span><span class="sxs-lookup"><span data-stu-id="0d4b1-280">Yes</span></span>     |    <span data-ttu-id="0d4b1-281">Raporun oluşturulacak saat sıklığı.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-281">Frequency in hours at which the report should be generated.</span></span> <br> <span data-ttu-id="0d4b1-282">En düşük değer 4, Maksimum değer ise 2160'tır.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-282">Minimum value is 4 and Maximum value is 2160.</span></span>      |    <span data-ttu-id="0d4b1-283">tamsayı</span><span class="sxs-lookup"><span data-stu-id="0d4b1-283">integer</span></span>     |
|    <span data-ttu-id="0d4b1-284">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="0d4b1-284">RecurrenceCount</span></span>     |    <span data-ttu-id="0d4b1-285">Hayır</span><span class="sxs-lookup"><span data-stu-id="0d4b1-285">No</span></span>     |    <span data-ttu-id="0d4b1-286">Oluşturulan rapor sayısı.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-286">Number of reports to be generated.</span></span>     |    <span data-ttu-id="0d4b1-287">tamsayı</span><span class="sxs-lookup"><span data-stu-id="0d4b1-287">integer</span></span>     |
|    <span data-ttu-id="0d4b1-288">Biçimlendir</span><span class="sxs-lookup"><span data-stu-id="0d4b1-288">Format</span></span>     |    <span data-ttu-id="0d4b1-289">Hayır</span><span class="sxs-lookup"><span data-stu-id="0d4b1-289">No</span></span>     |    <span data-ttu-id="0d4b1-290">Dışarı aktaran dosyanın dosya biçimi.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-290">File format of the exported file.</span></span> <br> <span data-ttu-id="0d4b1-291">Csv varsayılandır.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-291">Default is CSV.</span></span>    |    <span data-ttu-id="0d4b1-292">"CSV"/"TSV"</span><span class="sxs-lookup"><span data-stu-id="0d4b1-292">"CSV"/"TSV"</span></span>     |
|    <span data-ttu-id="0d4b1-293">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="0d4b1-293">CallbackUrl</span></span>     |    <span data-ttu-id="0d4b1-294">Hayır</span><span class="sxs-lookup"><span data-stu-id="0d4b1-294">No</span></span>     |    <span data-ttu-id="0d4b1-295">İsteğe bağlı olarak geri çağırma hedefi olarak yapılandırılan genel olarak erişilebilir URL</span><span class="sxs-lookup"><span data-stu-id="0d4b1-295">Publicly reachable URL that can be optionally configured as callback destination</span></span>     |    <span data-ttu-id="0d4b1-296">Dize (http URL'si)</span><span class="sxs-lookup"><span data-stu-id="0d4b1-296">String (http URL)</span></span>     |
|    <span data-ttu-id="0d4b1-297">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="0d4b1-297">CallbackMethod</span></span>     |    <span data-ttu-id="0d4b1-298">Hayır</span><span class="sxs-lookup"><span data-stu-id="0d4b1-298">No</span></span>     |    <span data-ttu-id="0d4b1-299">Geri çağırma için kullanılacak yöntem</span><span class="sxs-lookup"><span data-stu-id="0d4b1-299">The method to be used for callback</span></span>     |    <span data-ttu-id="0d4b1-300">GET/POST</span><span class="sxs-lookup"><span data-stu-id="0d4b1-300">GET/POST</span></span>     |
|        |        |        |        |

### <a name="sample-response"></a><span data-ttu-id="0d4b1-301">Örnek yanıt</span><span class="sxs-lookup"><span data-stu-id="0d4b1-301">Sample response</span></span>

<span data-ttu-id="0d4b1-302">Yanıt yükü aşağıdaki şekilde yapılandırılır:</span><span class="sxs-lookup"><span data-stu-id="0d4b1-302">The response payload is structured as follows:</span></span>

<span data-ttu-id="0d4b1-303">Yanıt kodları: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="0d4b1-303">Response Codes: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="0d4b1-304">Yanıt yükü örneği:</span><span class="sxs-lookup"><span data-stu-id="0d4b1-304">Response payload example:</span></span>

```json
{ 
  "value": [
    { 
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf", 
      "reportName": "Top10_CustomersReport", 
      "description": "Top 10 customers by revenue for last month", 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033", 
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH", 
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T13:11:58Z", 
      "modifiedTime": null, 
      "executeNow": false, 
      "startTime": "2021-03-31T18:41:00Z", 
      "reportStatus": "Active", 
      "recurrenceInterval": 24, 
      "recurrenceCount": 100, 
      "callbackUrl": "https://<SampleCallbackUrl>", 
      "callbackMethod": "GET", 
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

### <a name="glossary"></a><span data-ttu-id="0d4b1-305">Sözlük</span><span class="sxs-lookup"><span data-stu-id="0d4b1-305">Glossary</span></span>

<span data-ttu-id="0d4b1-306">Yanıttaki öğelerin temel tanımları aşağıda verilmiştir:</span><span class="sxs-lookup"><span data-stu-id="0d4b1-306">Key definitions of elements in the response are articulated below:</span></span>

|    <span data-ttu-id="0d4b1-307">Parametre</span><span class="sxs-lookup"><span data-stu-id="0d4b1-307">Parameter</span></span>     |    <span data-ttu-id="0d4b1-308">Açıklama</span><span class="sxs-lookup"><span data-stu-id="0d4b1-308">Description</span></span>     |
|    ----    |    ----    |
|    <span data-ttu-id="0d4b1-309">REPORTID</span><span class="sxs-lookup"><span data-stu-id="0d4b1-309">ReportId</span></span>     |    <span data-ttu-id="0d4b1-310">Oluşturduğunuz raporun evrensel benzersiz tanımlayıcısı (UUID)</span><span class="sxs-lookup"><span data-stu-id="0d4b1-310">Universally unique identifier (UUID) of the report you created</span></span>     |
|    <span data-ttu-id="0d4b1-311">ReportName</span><span class="sxs-lookup"><span data-stu-id="0d4b1-311">ReportName</span></span>     |    <span data-ttu-id="0d4b1-312">İstek yükünde rapora verilen ad</span><span class="sxs-lookup"><span data-stu-id="0d4b1-312">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="0d4b1-313">Açıklama</span><span class="sxs-lookup"><span data-stu-id="0d4b1-313">Description</span></span>     |    <span data-ttu-id="0d4b1-314">Raporun oluşturulması sırasında verilen açıklama</span><span class="sxs-lookup"><span data-stu-id="0d4b1-314">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="0d4b1-315">QueryId</span><span class="sxs-lookup"><span data-stu-id="0d4b1-315">QueryId</span></span>     |    <span data-ttu-id="0d4b1-316">Raporu oluşturduğunuz sırada geçirilen sorgu KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="0d4b1-316">Query ID passed at the time you created the report</span></span>     |
|    <span data-ttu-id="0d4b1-317">Sorgu</span><span class="sxs-lookup"><span data-stu-id="0d4b1-317">Query</span></span>     |    <span data-ttu-id="0d4b1-318">Bu rapor için yürütülecek sorgu metni</span><span class="sxs-lookup"><span data-stu-id="0d4b1-318">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="0d4b1-319">Kullanıcı</span><span class="sxs-lookup"><span data-stu-id="0d4b1-319">User</span></span>     |    <span data-ttu-id="0d4b1-320">Raporu oluşturmak için kullanılan Kullanıcı KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="0d4b1-320">User ID used to create the report</span></span>     |
|    <span data-ttu-id="0d4b1-321">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="0d4b1-321">CreatedTime</span></span>     |    <span data-ttu-id="0d4b1-322">Raporun şu biçimde oluşturulduğu UTC saati: yyyy-MM-ddTHH: mm: ssZ</span><span class="sxs-lookup"><span data-stu-id="0d4b1-322">UTC Time the report was created in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="0d4b1-323">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="0d4b1-323">ModifiedTime</span></span>     |    <span data-ttu-id="0d4b1-324">Raporun bu biçimde en son değiştirildiği UTC saati: yyyy-MM-ddTHH: mm: ssZ</span><span class="sxs-lookup"><span data-stu-id="0d4b1-324">UTC Time the report was last modified in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="0d4b1-325">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="0d4b1-325">ExecuteNow</span></span>     |    <span data-ttu-id="0d4b1-326">`ExecuteNow` raporun oluşturulduğu sırada ayarlanan bayrak</span><span class="sxs-lookup"><span data-stu-id="0d4b1-326">`ExecuteNow` flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="0d4b1-327">StartTime</span><span class="sxs-lookup"><span data-stu-id="0d4b1-327">StartTime</span></span>     |    <span data-ttu-id="0d4b1-328">Rapor yürütmenin bu biçimde başlayacağı UTC saati: yyyy-MM-ddTHH: mm: ssZ</span><span class="sxs-lookup"><span data-stu-id="0d4b1-328">UTC Time the report execution will begin in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="0d4b1-329">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="0d4b1-329">ReportStatus</span></span>     |    <span data-ttu-id="0d4b1-330">Rapor yürütmenin durumu.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-330">Status of the report execution.</span></span> <span data-ttu-id="0d4b1-331">Olası değerler şunlardır `Paused` , `Active` ve `Inactive`</span><span class="sxs-lookup"><span data-stu-id="0d4b1-331">The possible values are `Paused`, `Active`, and `Inactive`</span></span>     |
|    <span data-ttu-id="0d4b1-332">Recurrenceınterval</span><span class="sxs-lookup"><span data-stu-id="0d4b1-332">RecurrenceInterval</span></span>     |    <span data-ttu-id="0d4b1-333">Rapor oluşturma sırasında belirtilen yinelenme aralığı</span><span class="sxs-lookup"><span data-stu-id="0d4b1-333">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="0d4b1-334">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="0d4b1-334">RecurrenceCount</span></span>     |    <span data-ttu-id="0d4b1-335">Rapor oluşturma sırasında yinelenme sayısı belirtildi.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-335">Recurrence count provided during report creation.</span></span>      |
|    <span data-ttu-id="0d4b1-336">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="0d4b1-336">CallbackUrl</span></span>     |    <span data-ttu-id="0d4b1-337">İstekte belirtilen geri çağırma URL 'SI</span><span class="sxs-lookup"><span data-stu-id="0d4b1-337">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="0d4b1-338">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="0d4b1-338">CallbackMethod</span></span>     |    <span data-ttu-id="0d4b1-339">İstekte belirtilen geri çağırma yöntemi</span><span class="sxs-lookup"><span data-stu-id="0d4b1-339">Callback method provided in the request</span></span>     |
|    <span data-ttu-id="0d4b1-340">Biçimlendir</span><span class="sxs-lookup"><span data-stu-id="0d4b1-340">Format</span></span>     |    <span data-ttu-id="0d4b1-341">Rapor dosyalarının biçimi.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-341">Format of the report files.</span></span> <span data-ttu-id="0d4b1-342">Olası değerler veya ' `CSV` dir `TSV` .</span><span class="sxs-lookup"><span data-stu-id="0d4b1-342">The possible values are `CSV` or `TSV`.</span></span>     |
|    <span data-ttu-id="0d4b1-343">TotalCount</span><span class="sxs-lookup"><span data-stu-id="0d4b1-343">TotalCount</span></span>     |    <span data-ttu-id="0d4b1-344">Değer dizisindeki kayıt sayısı</span><span class="sxs-lookup"><span data-stu-id="0d4b1-344">Number of records in the Value array</span></span>     |
|    <span data-ttu-id="0d4b1-345">Durum</span><span class="sxs-lookup"><span data-stu-id="0d4b1-345">StatusCode</span></span>     |    <span data-ttu-id="0d4b1-346">Sonuç Kodu</span><span class="sxs-lookup"><span data-stu-id="0d4b1-346">Result Code</span></span>     |
|    <span data-ttu-id="0d4b1-347">message</span><span class="sxs-lookup"><span data-stu-id="0d4b1-347">message</span></span>     |    <span data-ttu-id="0d4b1-348">Olası değerler 200, 400, 401, 403, 500 ' dir.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-348">The possible values are 200, 400, 401, 403, 500.</span></span> <span data-ttu-id="0d4b1-349">API 'nin yürütülmesindeki durum iletisi</span><span class="sxs-lookup"><span data-stu-id="0d4b1-349">Status message from the execution of the API</span></span>     |
|        |        |

## <a name="get-report-execution-api"></a><span data-ttu-id="0d4b1-350">Rapor yürütme API 'sini al</span><span class="sxs-lookup"><span data-stu-id="0d4b1-350">Get report execution API</span></span>

<span data-ttu-id="0d4b1-351">[Rapor oluşturma API](#create-report-api)'Sinden alınan REPORTID kullanarak rapor yürütmenin durumunu sorgulamak için bu yöntemi kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-351">You can use this method to query the status of a report execution using the ReportId received from [Create Report API](#create-report-api).</span></span> <span data-ttu-id="0d4b1-352">Rapor indirmeye hazırsanız, yöntemi rapor indirme bağlantısını döndürür.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-352">The method returns the report download link if the report is ready for download.</span></span> <span data-ttu-id="0d4b1-353">Aksi takdirde, yöntemi durumu döndürür.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-353">Otherwise, the method returns the status.</span></span> <span data-ttu-id="0d4b1-354">Belirli bir rapor için gerçekleşen tüm yürütmeleri almak için bu API 'yi de kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-354">You can also use this API to get all the executions that have happened for a given report.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="0d4b1-355">Bu API, ve için ayarlanmış varsayılan sorgu parametrelerine sahiptir `executionStatus=Completed` `getLatestExecution=true` .</span><span class="sxs-lookup"><span data-stu-id="0d4b1-355">This API has default query parameters set for `executionStatus=Completed` and `getLatestExecution=true`.</span></span> <span data-ttu-id="0d4b1-356">Bu nedenle, raporun ilk başarılı yürütülmesi için önce API çağrılması 404 döndürür.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-356">Hence, calling the API before the first successful execution of the report will return 404.</span></span> <span data-ttu-id="0d4b1-357">Bekleyen yürütmeler, ayarıyla elde edilebilir `executionStatus=Pending` .</span><span class="sxs-lookup"><span data-stu-id="0d4b1-357">Pending executions can be obtained by setting `executionStatus=Pending`.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="0d4b1-358">İstek sözdizimi</span><span class="sxs-lookup"><span data-stu-id="0d4b1-358">Request syntax</span></span>

|    <span data-ttu-id="0d4b1-359">Yöntem</span><span class="sxs-lookup"><span data-stu-id="0d4b1-359">Method</span></span>     |    <span data-ttu-id="0d4b1-360">İstek URI'si</span><span class="sxs-lookup"><span data-stu-id="0d4b1-360">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="0d4b1-361">GET</span><span class="sxs-lookup"><span data-stu-id="0d4b1-361">GET</span></span>    |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/{reportId}?executionId={executionId}&executionStatus={executionStatus}&getLatestExecution={getLatestExecution}`  |

### <a name="request-header"></a><span data-ttu-id="0d4b1-362">İstek üst bilgisi</span><span class="sxs-lookup"><span data-stu-id="0d4b1-362">Request header</span></span>

|    <span data-ttu-id="0d4b1-363">Üst bilgi</span><span class="sxs-lookup"><span data-stu-id="0d4b1-363">Header</span></span>     |    <span data-ttu-id="0d4b1-364">Tür</span><span class="sxs-lookup"><span data-stu-id="0d4b1-364">Type</span></span>     |    <span data-ttu-id="0d4b1-365">Açıklama</span><span class="sxs-lookup"><span data-stu-id="0d4b1-365">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="0d4b1-366">Yetkilendirme</span><span class="sxs-lookup"><span data-stu-id="0d4b1-366">Authorization</span></span>     |    <span data-ttu-id="0d4b1-367">string</span><span class="sxs-lookup"><span data-stu-id="0d4b1-367">string</span></span> |<span data-ttu-id="0d4b1-368">Gereklidir.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-368">Required.</span></span> <span data-ttu-id="0d4b1-369">Azure Active Directory (Azure AD) erişim belirteci.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-369">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="0d4b1-370">Biçim  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="0d4b1-370">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="0d4b1-371">İçerik Türü</span><span class="sxs-lookup"><span data-stu-id="0d4b1-371">Content-Type</span></span>     |<span data-ttu-id="0d4b1-372">string</span><span class="sxs-lookup"><span data-stu-id="0d4b1-372">string</span></span> |`Application/JSON` |

### <a name="path-parameter"></a><span data-ttu-id="0d4b1-373">Yol parametresi</span><span class="sxs-lookup"><span data-stu-id="0d4b1-373">Path parameter</span></span>

|    <span data-ttu-id="0d4b1-374">Parametre Adı</span><span class="sxs-lookup"><span data-stu-id="0d4b1-374">Parameter Name</span></span>    |    <span data-ttu-id="0d4b1-375">Gerekli</span><span class="sxs-lookup"><span data-stu-id="0d4b1-375">Required</span></span>    |    <span data-ttu-id="0d4b1-376">Tür</span><span class="sxs-lookup"><span data-stu-id="0d4b1-376">Type</span></span>    |    <span data-ttu-id="0d4b1-377">Açıklama</span><span class="sxs-lookup"><span data-stu-id="0d4b1-377">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="0d4b1-378">reportId</span><span class="sxs-lookup"><span data-stu-id="0d4b1-378">reportId</span></span>    |    <span data-ttu-id="0d4b1-379">Yes</span><span class="sxs-lookup"><span data-stu-id="0d4b1-379">Yes</span></span>    |    <span data-ttu-id="0d4b1-380">string</span><span class="sxs-lookup"><span data-stu-id="0d4b1-380">string</span></span>    |    <span data-ttu-id="0d4b1-381">Yalnızca bu bağımsız değişkende verilen REPORTID 'ye sahip raporların yürütme ayrıntılarını almak için filtreleyin.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-381">Filter to get execution details of only reports with the reportId given in this argument.</span></span> <span data-ttu-id="0d4b1-382">Birden çok Inceleme, noktalı virgül ";" ile ayrılarak belirtilebilir.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-382">Multiple reportIds can be specified by separating them with a semicolon ";".</span></span>    |
|        |        |        |        |

### <a name="query-parameter"></a><span data-ttu-id="0d4b1-383">Sorgu parametresi</span><span class="sxs-lookup"><span data-stu-id="0d4b1-383">Query parameter</span></span>

|    <span data-ttu-id="0d4b1-384">Parametre Adı</span><span class="sxs-lookup"><span data-stu-id="0d4b1-384">Parameter Name</span></span>    |    <span data-ttu-id="0d4b1-385">Gerekli</span><span class="sxs-lookup"><span data-stu-id="0d4b1-385">Required</span></span>    |    <span data-ttu-id="0d4b1-386">Tür</span><span class="sxs-lookup"><span data-stu-id="0d4b1-386">Type</span></span>    |    <span data-ttu-id="0d4b1-387">Açıklama</span><span class="sxs-lookup"><span data-stu-id="0d4b1-387">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="0d4b1-388">Yürütme</span><span class="sxs-lookup"><span data-stu-id="0d4b1-388">executionId</span></span>    |    <span data-ttu-id="0d4b1-389">Hayır</span><span class="sxs-lookup"><span data-stu-id="0d4b1-389">No</span></span>    |    <span data-ttu-id="0d4b1-390">string</span><span class="sxs-lookup"><span data-stu-id="0d4b1-390">string</span></span>    |    <span data-ttu-id="0d4b1-391">Yalnızca bu bağımsız değişkende verilen ExecutionID 'ye sahip raporların ayrıntılarını almak için filtreleyin.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-391">Filter to get details of only reports with the executionId given in this argument.</span></span> <span data-ttu-id="0d4b1-392">Birden çok ExecutionID, noktalı virgül ";" ile ayrılarak belirtilebilir.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-392">Multiple executionIds can be specified by separating them with a semicolon ";".</span></span>    |
|    <span data-ttu-id="0d4b1-393">executionStatus</span><span class="sxs-lookup"><span data-stu-id="0d4b1-393">executionStatus</span></span>    |    <span data-ttu-id="0d4b1-394">Hayır</span><span class="sxs-lookup"><span data-stu-id="0d4b1-394">No</span></span>    |    <span data-ttu-id="0d4b1-395">Dize/Enum</span><span class="sxs-lookup"><span data-stu-id="0d4b1-395">String/enum</span></span>    |    <span data-ttu-id="0d4b1-396">Yalnızca bu bağımsız değişkende verilen executionStatus raporlarının ayrıntılarını almak için filtreleyin.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-396">Filter to get details of only reports with the executionStatus given in this argument.</span></span> <br> <span data-ttu-id="0d4b1-397">Geçerli değerler şunlardır: `Pending` , `Running` , `Paused` ve `Completed` .</span><span class="sxs-lookup"><span data-stu-id="0d4b1-397">Valid values are: `Pending`, `Running`, `Paused` and `Completed`.</span></span> <br> <span data-ttu-id="0d4b1-398">`Completed` varsayılan değerdir.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-398">The default value is `Completed`.</span></span> <br> <span data-ttu-id="0d4b1-399">Birden çok durum noktalı virgül ";" ile ayrılarak belirtilebilir.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-399">Multiple statuses can be specified by separating them with a semicolon ";".</span></span>    |
|    <span data-ttu-id="0d4b1-400">getLatestExecution</span><span class="sxs-lookup"><span data-stu-id="0d4b1-400">getLatestExecution</span></span>    |    <span data-ttu-id="0d4b1-401">Hayır</span><span class="sxs-lookup"><span data-stu-id="0d4b1-401">No</span></span>    |    <span data-ttu-id="0d4b1-402">boolean</span><span class="sxs-lookup"><span data-stu-id="0d4b1-402">boolean</span></span>    |    <span data-ttu-id="0d4b1-403">API, en son yürütmenin ayrıntılarını döndürür.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-403">The API will return details of the latest execution.</span></span> <span data-ttu-id="0d4b1-404">Varsayılan olarak, bu parametre true olarak ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-404">By default, this parameter is set to true.</span></span><br> <span data-ttu-id="0d4b1-405">Bu parametrenin değerini false olarak geçirmeye seçerseniz, API son 90 gün yürütme örneğini döndürür.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-405">If you choose to pass the value of this parameter as false, then the API will return the last 90 days execution instances.</span></span>    |
|        |        |        |        |

### <a name="sample-request-payload"></a><span data-ttu-id="0d4b1-406">Örnek Istek yükü</span><span class="sxs-lookup"><span data-stu-id="0d4b1-406">Sample Request Payload</span></span>

<span data-ttu-id="0d4b1-407">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="0d4b1-407">None</span></span>

### <a name="sample-response"></a><span data-ttu-id="0d4b1-408">Örnek Yanıt</span><span class="sxs-lookup"><span data-stu-id="0d4b1-408">Sample Response</span></span>

<span data-ttu-id="0d4b1-409">Yanıt yükü aşağıdaki şekilde yapılandırılır:</span><span class="sxs-lookup"><span data-stu-id="0d4b1-409">The response payload is structured as follows:</span></span>

<span data-ttu-id="0d4b1-410">Yanıt kodları: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="0d4b1-410">Response Codes: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="0d4b1-411">Yanıt yükü örneği:</span><span class="sxs-lookup"><span data-stu-id="0d4b1-411">Response payload example:</span></span>

```json
{
  "value": [
    {
      "executionId": "906931dc-4f2f-4195-bbb2-d7295c7550d3",
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf",
      "recurrenceInterval": 24,
      "recurrenceCount": 100,
      "callbackUrl": null,
      "callbackMethod": null,
      "format": "csv",
      "executionStatus": "Completed",
      "reportLocation": null,
      "reportAccessSecureLink": "https://<path to report for download>",
      "reportExpiryTime": null,
      "reportGeneratedTime": "2021-03-31T18:41:00Z"
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

<span data-ttu-id="0d4b1-412">Rapor yürütme tamamlandıktan sonra, yürütme durumu `Completed` gösterilir.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-412">Once report execution is complete, the execution status `Completed` is shown.</span></span> <span data-ttu-id="0d4b1-413">İçindeki URL 'YI seçerek raporu indirebilirsiniz `reportAccessSecureLink` .</span><span class="sxs-lookup"><span data-stu-id="0d4b1-413">You can download the report by selecting the URL in the `reportAccessSecureLink`.</span></span>

### <a name="glossary"></a><span data-ttu-id="0d4b1-414">Sözlük</span><span class="sxs-lookup"><span data-stu-id="0d4b1-414">Glossary</span></span>

<span data-ttu-id="0d4b1-415">Yanıttaki öğelerin anahtar tanımları.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-415">Key definitions of elements in the response.</span></span>

|    <span data-ttu-id="0d4b1-416">Parametre</span><span class="sxs-lookup"><span data-stu-id="0d4b1-416">Parameter</span></span>    |    <span data-ttu-id="0d4b1-417">Açıklama</span><span class="sxs-lookup"><span data-stu-id="0d4b1-417">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="0d4b1-418">Yürütme</span><span class="sxs-lookup"><span data-stu-id="0d4b1-418">ExecutionId</span></span>    |    <span data-ttu-id="0d4b1-419">Yürütme örneğinin evrensel benzersiz tanımlayıcısı (UUID)</span><span class="sxs-lookup"><span data-stu-id="0d4b1-419">Universally unique identifier (UUID) of the execution instance</span></span>    |
|    <span data-ttu-id="0d4b1-420">REPORTID</span><span class="sxs-lookup"><span data-stu-id="0d4b1-420">ReportId</span></span>    |    <span data-ttu-id="0d4b1-421">Yürütme örneğiyle ilişkili rapor KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="0d4b1-421">Report ID associated with the execution instance</span></span>    |
|    <span data-ttu-id="0d4b1-422">Recurrenceınterval</span><span class="sxs-lookup"><span data-stu-id="0d4b1-422">RecurrenceInterval</span></span>    |    <span data-ttu-id="0d4b1-423">Rapor oluşturma sırasında belirtilen yinelenme aralığı</span><span class="sxs-lookup"><span data-stu-id="0d4b1-423">Recurrence interval provided during report creation</span></span>    |
|    <span data-ttu-id="0d4b1-424">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="0d4b1-424">RecurrenceCount</span></span>    |    <span data-ttu-id="0d4b1-425">Rapor oluşturma sırasında belirtilen yinelenme sayısı</span><span class="sxs-lookup"><span data-stu-id="0d4b1-425">Recurrence count provided during report creation</span></span>    |
|    <span data-ttu-id="0d4b1-426">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="0d4b1-426">CallbackUrl</span></span>    |    <span data-ttu-id="0d4b1-427">Yürütme örneğiyle ilişkili geri çağırma URL 'SI</span><span class="sxs-lookup"><span data-stu-id="0d4b1-427">Callback URL associated with the execution instance</span></span>    |
|    <span data-ttu-id="0d4b1-428">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="0d4b1-428">CallbackMethod</span></span>    |    <span data-ttu-id="0d4b1-429">Yürütme örneğiyle ilişkili geri çağırma yöntemi</span><span class="sxs-lookup"><span data-stu-id="0d4b1-429">Callback method associated with the execution instance</span></span>    |
|    <span data-ttu-id="0d4b1-430">Biçimlendir</span><span class="sxs-lookup"><span data-stu-id="0d4b1-430">Format</span></span>    |    <span data-ttu-id="0d4b1-431">Yürütmenin sonunda oluşturulan dosyanın biçimi</span><span class="sxs-lookup"><span data-stu-id="0d4b1-431">Format of the generated file at the end of execution</span></span>    |
|    <span data-ttu-id="0d4b1-432">ExecutionStatus</span><span class="sxs-lookup"><span data-stu-id="0d4b1-432">ExecutionStatus</span></span>    |    <span data-ttu-id="0d4b1-433">Rapor yürütme örneğinin durumu.</span><span class="sxs-lookup"><span data-stu-id="0d4b1-433">Status of the report execution instance.</span></span> <br> <span data-ttu-id="0d4b1-434">Geçerli değerler şunlardır: `Pending` , `Running` , `Paused` , ve `Completed`</span><span class="sxs-lookup"><span data-stu-id="0d4b1-434">Valid values are: `Pending`, `Running`, `Paused`, and `Completed`</span></span>    |
|    <span data-ttu-id="0d4b1-435">ReportAccessSecureLink</span><span class="sxs-lookup"><span data-stu-id="0d4b1-435">ReportAccessSecureLink</span></span>    |<span data-ttu-id="0d4b1-436">Rapora güvenli erişilebilen bağlantı</span><span class="sxs-lookup"><span data-stu-id="0d4b1-436">Link through which the report can be accessed securely</span></span>        |
|    <span data-ttu-id="0d4b1-437">Reportexpiryıtime</span><span class="sxs-lookup"><span data-stu-id="0d4b1-437">ReportExpiryTime</span></span>    |    <span data-ttu-id="0d4b1-438">Rapor bağlantısının süresinin dolmasına geçen UTC saati: yyyy-MM-ddTHH: mm: ssZ</span><span class="sxs-lookup"><span data-stu-id="0d4b1-438">UTC Time after which the report link will expire in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>    |
|    <span data-ttu-id="0d4b1-439">ReportGeneratedTime</span><span class="sxs-lookup"><span data-stu-id="0d4b1-439">ReportGeneratedTime</span></span>    |    <span data-ttu-id="0d4b1-440">Raporun şu biçimde oluşturulduğu UTC saati: yyyy-MM-ddTHH: mm: ssZ</span><span class="sxs-lookup"><span data-stu-id="0d4b1-440">UTC Time at which the report was generated in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>    |
|    <span data-ttu-id="0d4b1-441">TotalCount</span><span class="sxs-lookup"><span data-stu-id="0d4b1-441">TotalCount</span></span>    |    <span data-ttu-id="0d4b1-442">Değer dizisindeki veri kümesi sayısı</span><span class="sxs-lookup"><span data-stu-id="0d4b1-442">Number of datasets in the Value array</span></span>    |
|    <span data-ttu-id="0d4b1-443">Durum</span><span class="sxs-lookup"><span data-stu-id="0d4b1-443">StatusCode</span></span>    |    <span data-ttu-id="0d4b1-444">Sonuç Kodu</span><span class="sxs-lookup"><span data-stu-id="0d4b1-444">Result Code</span></span> <br> <span data-ttu-id="0d4b1-445">Olası değerler 200, 400, 401, 403, 404 ve 500</span><span class="sxs-lookup"><span data-stu-id="0d4b1-445">The possible values are 200, 400, 401, 403, 404 and 500</span></span>    |
|    <span data-ttu-id="0d4b1-446">message</span><span class="sxs-lookup"><span data-stu-id="0d4b1-446">message</span></span>    |    <span data-ttu-id="0d4b1-447">API 'nin yürütülmesindeki durum iletisi</span><span class="sxs-lookup"><span data-stu-id="0d4b1-447">Status message from the execution of the API</span></span>    |
|        |        |

## <a name="next-steps"></a><span data-ttu-id="0d4b1-448">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="0d4b1-448">Next steps</span></span>

- <span data-ttu-id="0d4b1-449">[Swagger API URL 'si](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html) aracılığıyla API 'leri deneyin</span><span class="sxs-lookup"><span data-stu-id="0d4b1-449">Try out the APIs through the [swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span></span>
- [<span data-ttu-id="0d4b1-450">İlk API çağrısını yapın</span><span class="sxs-lookup"><span data-stu-id="0d4b1-450">Make your first API call</span></span>](insights-programmatic-first-api-call.md)