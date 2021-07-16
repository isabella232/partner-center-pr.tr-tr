---
title: rapor sorguları al API-Analizler verileri
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Rapor API 'sinde kullanılmak üzere tüm kullanılabilir sorguları almak için bu API 'yi kullanın.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 3bf140576a19439990405cfef23190045e0a98be
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377419"
---
# <a name="get-report-queries-api"></a><span data-ttu-id="cf6f5-103">Rapor sorguları al API 'SI</span><span class="sxs-lookup"><span data-stu-id="cf6f5-103">Get report queries API</span></span>

<span data-ttu-id="cf6f5-104">Rapor sorgularını al API 'SI, raporlarda kullanıma sunulan tüm sorguları alır.</span><span class="sxs-lookup"><span data-stu-id="cf6f5-104">The Get report queries API gets all the queries that are available for use in reports.</span></span> <span data-ttu-id="cf6f5-105">Tüm sistem ve Kullanıcı tanımlı sorguları varsayılan olarak alır.</span><span class="sxs-lookup"><span data-stu-id="cf6f5-105">It gets all the system and user-defined queries by default.</span></span>

<span data-ttu-id="cf6f5-106">**İstek sözdizimi**</span><span class="sxs-lookup"><span data-stu-id="cf6f5-106">**Request syntax**</span></span>

|    <span data-ttu-id="cf6f5-107">Yöntem</span><span class="sxs-lookup"><span data-stu-id="cf6f5-107">Method</span></span>    |    <span data-ttu-id="cf6f5-108">İstek URI'si</span><span class="sxs-lookup"><span data-stu-id="cf6f5-108">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="cf6f5-109">GET</span><span class="sxs-lookup"><span data-stu-id="cf6f5-109">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
|        |        |

<span data-ttu-id="cf6f5-110">**İstek üst bilgisi**</span><span class="sxs-lookup"><span data-stu-id="cf6f5-110">**Request header**</span></span>

|    <span data-ttu-id="cf6f5-111">Üst bilgi</span><span class="sxs-lookup"><span data-stu-id="cf6f5-111">Header</span></span>    |    <span data-ttu-id="cf6f5-112">Tür</span><span class="sxs-lookup"><span data-stu-id="cf6f5-112">Type</span></span>    |    <span data-ttu-id="cf6f5-113">Açıklama</span><span class="sxs-lookup"><span data-stu-id="cf6f5-113">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="cf6f5-114">Yetkilendirme</span><span class="sxs-lookup"><span data-stu-id="cf6f5-114">Authorization</span></span>    |    <span data-ttu-id="cf6f5-115">string</span><span class="sxs-lookup"><span data-stu-id="cf6f5-115">string</span></span>    |    <span data-ttu-id="cf6f5-116">Gereklidir.</span><span class="sxs-lookup"><span data-stu-id="cf6f5-116">Required.</span></span> <span data-ttu-id="cf6f5-117">formdaki Azure Active Directory (AAD) erişim belirteci`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="cf6f5-117">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="cf6f5-118">İçerik Türü</span><span class="sxs-lookup"><span data-stu-id="cf6f5-118">Content-Type</span></span>    |    <span data-ttu-id="cf6f5-119">string</span><span class="sxs-lookup"><span data-stu-id="cf6f5-119">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="cf6f5-120">**Yol parametresi**</span><span class="sxs-lookup"><span data-stu-id="cf6f5-120">**Path parameter**</span></span>

<span data-ttu-id="cf6f5-121">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="cf6f5-121">None</span></span>

<span data-ttu-id="cf6f5-122">**Sorgu parametresi**</span><span class="sxs-lookup"><span data-stu-id="cf6f5-122">**Query parameter**</span></span>

|    <span data-ttu-id="cf6f5-123">Parametre Adı</span><span class="sxs-lookup"><span data-stu-id="cf6f5-123">Parameter Name</span></span>    |    <span data-ttu-id="cf6f5-124">Tür</span><span class="sxs-lookup"><span data-stu-id="cf6f5-124">Type</span></span>    |    <span data-ttu-id="cf6f5-125">Gerekli</span><span class="sxs-lookup"><span data-stu-id="cf6f5-125">Required</span></span>    |    <span data-ttu-id="cf6f5-126">Açıklama</span><span class="sxs-lookup"><span data-stu-id="cf6f5-126">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="cf6f5-127">QueryId</span><span class="sxs-lookup"><span data-stu-id="cf6f5-127">queryId</span></span>     |    <span data-ttu-id="cf6f5-128">dize</span><span class="sxs-lookup"><span data-stu-id="cf6f5-128">string</span></span>     |    <span data-ttu-id="cf6f5-129">No</span><span class="sxs-lookup"><span data-stu-id="cf6f5-129">No</span></span>    |    <span data-ttu-id="cf6f5-130">Yalnızca bağımsız değişkende verilen KIMLIĞE sahip sorguların ayrıntılarını almak için filtrele</span><span class="sxs-lookup"><span data-stu-id="cf6f5-130">Filter to get details of only queries with the ID given in the argument</span></span>     |
|    <span data-ttu-id="cf6f5-131">queryName</span><span class="sxs-lookup"><span data-stu-id="cf6f5-131">queryName</span></span>     |    <span data-ttu-id="cf6f5-132">dize</span><span class="sxs-lookup"><span data-stu-id="cf6f5-132">string</span></span>     |    <span data-ttu-id="cf6f5-133">No</span><span class="sxs-lookup"><span data-stu-id="cf6f5-133">No</span></span>    |    <span data-ttu-id="cf6f5-134">Yalnızca bağımsız değişkende verilen ada sahip sorguların ayrıntılarını almak için filtrele</span><span class="sxs-lookup"><span data-stu-id="cf6f5-134">Filter to get details of only queries with the name given in the argument</span></span>     |
|    <span data-ttu-id="cf6f5-135">Includesystemqueries</span><span class="sxs-lookup"><span data-stu-id="cf6f5-135">IncludeSystemQueries</span></span>     |    <span data-ttu-id="cf6f5-136">boolean</span><span class="sxs-lookup"><span data-stu-id="cf6f5-136">boolean</span></span>     |    <span data-ttu-id="cf6f5-137">Hayır</span><span class="sxs-lookup"><span data-stu-id="cf6f5-137">No</span></span>    |    <span data-ttu-id="cf6f5-138">Yanıta önceden tanımlanmış sistem sorgularını dahil et</span><span class="sxs-lookup"><span data-stu-id="cf6f5-138">Include predefined system queries in the response</span></span>     |
|    <span data-ttu-id="cf6f5-139">Includeonlysystemqueries</span><span class="sxs-lookup"><span data-stu-id="cf6f5-139">IncludeOnlySystemQueries</span></span>     |    <span data-ttu-id="cf6f5-140">boolean</span><span class="sxs-lookup"><span data-stu-id="cf6f5-140">boolean</span></span>     |    <span data-ttu-id="cf6f5-141">Hayır</span><span class="sxs-lookup"><span data-stu-id="cf6f5-141">No</span></span>    |    <span data-ttu-id="cf6f5-142">Yanıta yalnızca sistem sorgularını dahil et</span><span class="sxs-lookup"><span data-stu-id="cf6f5-142">Include only system queries in the response</span></span>     |
|        |        |        |        |


<span data-ttu-id="cf6f5-143">**İstek yükü**</span><span class="sxs-lookup"><span data-stu-id="cf6f5-143">**Request payload**</span></span>

<span data-ttu-id="cf6f5-144">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="cf6f5-144">None</span></span>

<span data-ttu-id="cf6f5-145">**Sözlük**</span><span class="sxs-lookup"><span data-stu-id="cf6f5-145">**Glossary**</span></span>

<span data-ttu-id="cf6f5-146">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="cf6f5-146">None</span></span>

<span data-ttu-id="cf6f5-147">**Response**</span><span class="sxs-lookup"><span data-stu-id="cf6f5-147">**Response**</span></span>

<span data-ttu-id="cf6f5-148">Yanıt yükü aşağıdaki şekilde yapılandırılır:</span><span class="sxs-lookup"><span data-stu-id="cf6f5-148">The response payload is structured as follows:</span></span>

<span data-ttu-id="cf6f5-149">Yanıt kodu: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="cf6f5-149">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="cf6f5-150">Yanıt yükü örneği:</span><span class="sxs-lookup"><span data-stu-id="cf6f5-150">Response payload example:</span></span>

```json
{ 
  "Value": [ 
    { 
      "QueryId": "string", 
      "Name": "string", 
      "Description": "string", 
      "Query": "string", 
      "Type": "string", 
      "User": "string", 
      "CreatedTime": "string", 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="cf6f5-151">**Sözlük**</span><span class="sxs-lookup"><span data-stu-id="cf6f5-151">**Glossary**</span></span>

<span data-ttu-id="cf6f5-152">Bu tablo, yanıttaki anahtar öğeleri tanımlar:</span><span class="sxs-lookup"><span data-stu-id="cf6f5-152">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="cf6f5-153">Parametre</span><span class="sxs-lookup"><span data-stu-id="cf6f5-153">Parameter</span></span>    |    <span data-ttu-id="cf6f5-154">Açıklama</span><span class="sxs-lookup"><span data-stu-id="cf6f5-154">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="cf6f5-155">QueryId</span><span class="sxs-lookup"><span data-stu-id="cf6f5-155">QueryId</span></span>     |    <span data-ttu-id="cf6f5-156">Sorgunun benzersiz UUID 'SI</span><span class="sxs-lookup"><span data-stu-id="cf6f5-156">Unique UUID of the query</span></span>     |
|    <span data-ttu-id="cf6f5-157">Name</span><span class="sxs-lookup"><span data-stu-id="cf6f5-157">Name</span></span>     |    <span data-ttu-id="cf6f5-158">Sorgu oluşturma sırasında sorguya verilen ad</span><span class="sxs-lookup"><span data-stu-id="cf6f5-158">Name given to the query at the time of query creation</span></span>     |
|    <span data-ttu-id="cf6f5-159">Açıklama</span><span class="sxs-lookup"><span data-stu-id="cf6f5-159">Description</span></span>     |    <span data-ttu-id="cf6f5-160">Sorgunun oluşturulması sırasında verilen açıklama</span><span class="sxs-lookup"><span data-stu-id="cf6f5-160">Description given during creation of the query</span></span>     |
|    <span data-ttu-id="cf6f5-161">Sorgu</span><span class="sxs-lookup"><span data-stu-id="cf6f5-161">Query</span></span>     |    <span data-ttu-id="cf6f5-162">Rapor sorgu dizesi</span><span class="sxs-lookup"><span data-stu-id="cf6f5-162">Report query string</span></span>     |
|    <span data-ttu-id="cf6f5-163">Tür</span><span class="sxs-lookup"><span data-stu-id="cf6f5-163">Type</span></span>     |    <span data-ttu-id="cf6f5-164">Önceden tanımlı sistem sorguları için Kullanıcı tarafından oluşturulan sorgular ve sistem için userDefined olarak ayarla</span><span class="sxs-lookup"><span data-stu-id="cf6f5-164">Set to userDefined for user created queries and system for predefined system queries</span></span>     |
|    <span data-ttu-id="cf6f5-165">Kullanıcı</span><span class="sxs-lookup"><span data-stu-id="cf6f5-165">User</span></span>     |    <span data-ttu-id="cf6f5-166">Sorguyu oluşturan kullanıcı KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="cf6f5-166">User ID who created the query</span></span>     |
|    <span data-ttu-id="cf6f5-167">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="cf6f5-167">CreatedTime</span></span>     |    <span data-ttu-id="cf6f5-168">Sorgu oluşturma zamanı</span><span class="sxs-lookup"><span data-stu-id="cf6f5-168">Time of creation of query</span></span>     |
|    <span data-ttu-id="cf6f5-169">TotalCount</span><span class="sxs-lookup"><span data-stu-id="cf6f5-169">TotalCount</span></span>     |    <span data-ttu-id="cf6f5-170">Değer dizisindeki veri kümesi sayısı</span><span class="sxs-lookup"><span data-stu-id="cf6f5-170">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="cf6f5-171">İleti</span><span class="sxs-lookup"><span data-stu-id="cf6f5-171">Message</span></span>     |    <span data-ttu-id="cf6f5-172">API 'nin yürütülmesindeki durum iletisi</span><span class="sxs-lookup"><span data-stu-id="cf6f5-172">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="cf6f5-173">Durum</span><span class="sxs-lookup"><span data-stu-id="cf6f5-173">StatusCode</span></span>     |    <span data-ttu-id="cf6f5-174">Sonuç kodu.</span><span class="sxs-lookup"><span data-stu-id="cf6f5-174">Result Code.</span></span> <span data-ttu-id="cf6f5-175">Olası değerler 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="cf6f5-175">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
