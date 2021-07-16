---
title: Rapor sorguları API'sini silme - Analizler silme
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Bu API'yi kullanarak içgörüler için kullanıcı İş Ortağı Merkezi silin.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e608068613edad1fca277ba5886c9c4bc962ffd2
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376977"
---
# <a name="delete-report-queries-api"></a><span data-ttu-id="7425d-103">Rapor sorguları API'sini silme</span><span class="sxs-lookup"><span data-stu-id="7425d-103">Delete report queries API</span></span>

<span data-ttu-id="7425d-104">Bu API, kullanıcı tanımlı sorguları siler.</span><span class="sxs-lookup"><span data-stu-id="7425d-104">This API deletes user-defined queries.</span></span>

<span data-ttu-id="7425d-105">**İstek söz dizimi**</span><span class="sxs-lookup"><span data-stu-id="7425d-105">**Request syntax**</span></span>

|    <span data-ttu-id="7425d-106">Yöntem</span><span class="sxs-lookup"><span data-stu-id="7425d-106">Method</span></span>    |    <span data-ttu-id="7425d-107">İstek URI'si</span><span class="sxs-lookup"><span data-stu-id="7425d-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="7425d-108">DELETE</span><span class="sxs-lookup"><span data-stu-id="7425d-108">DELETE</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
|        |        |

<span data-ttu-id="7425d-109">**İstek üst bilgisi**</span><span class="sxs-lookup"><span data-stu-id="7425d-109">**Request header**</span></span>

|    <span data-ttu-id="7425d-110">Üst bilgi</span><span class="sxs-lookup"><span data-stu-id="7425d-110">Header</span></span>    |    <span data-ttu-id="7425d-111">Tür</span><span class="sxs-lookup"><span data-stu-id="7425d-111">Type</span></span>    |    <span data-ttu-id="7425d-112">Açıklama</span><span class="sxs-lookup"><span data-stu-id="7425d-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="7425d-113">Yetkilendirme</span><span class="sxs-lookup"><span data-stu-id="7425d-113">Authorization</span></span>    |    <span data-ttu-id="7425d-114">string</span><span class="sxs-lookup"><span data-stu-id="7425d-114">string</span></span>    |    <span data-ttu-id="7425d-115">Gereklidir.</span><span class="sxs-lookup"><span data-stu-id="7425d-115">Required.</span></span> <span data-ttu-id="7425d-116">Formda Azure Active Directory (AAD) erişim belirteci`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="7425d-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="7425d-117">İçerik Türü</span><span class="sxs-lookup"><span data-stu-id="7425d-117">Content-Type</span></span>    |    <span data-ttu-id="7425d-118">string</span><span class="sxs-lookup"><span data-stu-id="7425d-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="7425d-119">**Yol parametresi**</span><span class="sxs-lookup"><span data-stu-id="7425d-119">**Path parameter**</span></span>

|    <span data-ttu-id="7425d-120">Parametre Adı</span><span class="sxs-lookup"><span data-stu-id="7425d-120">Parameter Name</span></span>    |    <span data-ttu-id="7425d-121">Tür</span><span class="sxs-lookup"><span data-stu-id="7425d-121">Type</span></span>    |    <span data-ttu-id="7425d-122">Gerekli</span><span class="sxs-lookup"><span data-stu-id="7425d-122">Required</span></span>    |    <span data-ttu-id="7425d-123">Açıklama</span><span class="sxs-lookup"><span data-stu-id="7425d-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="7425d-124">Queryıd</span><span class="sxs-lookup"><span data-stu-id="7425d-124">queryId</span></span>     |    <span data-ttu-id="7425d-125">dize</span><span class="sxs-lookup"><span data-stu-id="7425d-125">string</span></span>     |    <span data-ttu-id="7425d-126">No</span><span class="sxs-lookup"><span data-stu-id="7425d-126">No</span></span>    |    <span data-ttu-id="7425d-127">Yalnızca bağımsız değişkende verilen kimlikle sorguların ayrıntılarını almak için filtrele</span><span class="sxs-lookup"><span data-stu-id="7425d-127">Filter to get details of only queries with the ID given in the argument</span></span>     |
|        |        |        |        |

<span data-ttu-id="7425d-128">**Sorgu parametresi**</span><span class="sxs-lookup"><span data-stu-id="7425d-128">**Query parameter**</span></span>

<span data-ttu-id="7425d-129">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="7425d-129">None</span></span>

<span data-ttu-id="7425d-130">**İstek yükü**</span><span class="sxs-lookup"><span data-stu-id="7425d-130">**Request payload**</span></span>

<span data-ttu-id="7425d-131">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="7425d-131">None</span></span>

<span data-ttu-id="7425d-132">**Sözlük**</span><span class="sxs-lookup"><span data-stu-id="7425d-132">**Glossary**</span></span>

<span data-ttu-id="7425d-133">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="7425d-133">None</span></span>

<span data-ttu-id="7425d-134">**Response**</span><span class="sxs-lookup"><span data-stu-id="7425d-134">**Response**</span></span>

<span data-ttu-id="7425d-135">Yanıt yükü aşağıdaki gibi yapılandırılmıştır:</span><span class="sxs-lookup"><span data-stu-id="7425d-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="7425d-136">Yanıt kodu: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="7425d-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="7425d-137">Yanıt yükü örneği:</span><span class="sxs-lookup"><span data-stu-id="7425d-137">Response payload example:</span></span>

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

<span data-ttu-id="7425d-138">**Sözlük**</span><span class="sxs-lookup"><span data-stu-id="7425d-138">**Glossary**</span></span>

<span data-ttu-id="7425d-139">Bu tablo yanıtta önemli öğeleri tanımlar:</span><span class="sxs-lookup"><span data-stu-id="7425d-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="7425d-140">Parametre</span><span class="sxs-lookup"><span data-stu-id="7425d-140">Parameter</span></span>    |    <span data-ttu-id="7425d-141">Açıklama</span><span class="sxs-lookup"><span data-stu-id="7425d-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="7425d-142">Queryıd</span><span class="sxs-lookup"><span data-stu-id="7425d-142">QueryId</span></span>     |    <span data-ttu-id="7425d-143">Silinen sorgunun benzersiz UUID'i</span><span class="sxs-lookup"><span data-stu-id="7425d-143">Unique UUID of the query that was deleted</span></span>    |
|    <span data-ttu-id="7425d-144">Name</span><span class="sxs-lookup"><span data-stu-id="7425d-144">Name</span></span>     |    <span data-ttu-id="7425d-145">Silinen sorgunun adı</span><span class="sxs-lookup"><span data-stu-id="7425d-145">Name of the query that was deleted</span></span>    |
|    <span data-ttu-id="7425d-146">Açıklama</span><span class="sxs-lookup"><span data-stu-id="7425d-146">Description</span></span>     |    <span data-ttu-id="7425d-147">Silinen sorgunun açıklaması</span><span class="sxs-lookup"><span data-stu-id="7425d-147">Description of the deleted query</span></span>     |
|    <span data-ttu-id="7425d-148">Sorgu</span><span class="sxs-lookup"><span data-stu-id="7425d-148">Query</span></span>     |    <span data-ttu-id="7425d-149">Silinen sorgunun rapor sorgu dizesi</span><span class="sxs-lookup"><span data-stu-id="7425d-149">Report query string of the deleted query</span></span>    |
|    <span data-ttu-id="7425d-150">Tür</span><span class="sxs-lookup"><span data-stu-id="7425d-150">Type</span></span>     |    <span data-ttu-id="7425d-151">Kullanıcı tarafından oluşturulan sorgular için userDefined olarak ayarlayın</span><span class="sxs-lookup"><span data-stu-id="7425d-151">Set to userDefined for user created queries</span></span>     |
|    <span data-ttu-id="7425d-152">Kullanıcı</span><span class="sxs-lookup"><span data-stu-id="7425d-152">User</span></span>     |    <span data-ttu-id="7425d-153">Sorguyu oluşturan kullanıcı kimliği</span><span class="sxs-lookup"><span data-stu-id="7425d-153">User ID who created the query</span></span>     |
|    <span data-ttu-id="7425d-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="7425d-154">CreatedTime</span></span>     |    <span data-ttu-id="7425d-155">Sorgu oluşturma zamanı</span><span class="sxs-lookup"><span data-stu-id="7425d-155">Time of creation of query</span></span>     |
|    <span data-ttu-id="7425d-156">TotalCount</span><span class="sxs-lookup"><span data-stu-id="7425d-156">TotalCount</span></span>     |    <span data-ttu-id="7425d-157">Değer dizisinde veri kümesi sayısı</span><span class="sxs-lookup"><span data-stu-id="7425d-157">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="7425d-158">İleti</span><span class="sxs-lookup"><span data-stu-id="7425d-158">Message</span></span>     |    <span data-ttu-id="7425d-159">API'nin yürütülmesinden gelen durum iletisi</span><span class="sxs-lookup"><span data-stu-id="7425d-159">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="7425d-160">Statuscode</span><span class="sxs-lookup"><span data-stu-id="7425d-160">StatusCode</span></span>     |    <span data-ttu-id="7425d-161">Sonuç Kodu.</span><span class="sxs-lookup"><span data-stu-id="7425d-161">Result Code.</span></span> <span data-ttu-id="7425d-162">Olası değerler: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="7425d-162">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
