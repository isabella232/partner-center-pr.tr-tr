---
title: Rapor sorguları API 'sini deneyin
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sorgunuzu test etmek ve Iş Ortağı Merkezi öngörülerinin sonuçlarını doğrulamak için bu API 'yi kullanın.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 13ad6fe385a4d31390b6806d863da3f647105b2c
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377411"
---
# <a name="try-report-queries-api"></a><span data-ttu-id="33366-103">Rapor sorguları API 'sini deneyin</span><span class="sxs-lookup"><span data-stu-id="33366-103">Try report queries API</span></span>

<span data-ttu-id="33366-104">Bu API bir rapor sorgu ekstresi yürütür.</span><span class="sxs-lookup"><span data-stu-id="33366-104">This API executes a Report query statement.</span></span> <span data-ttu-id="33366-105">API, verilerin beklediğiniz gibi olup olmadığını doğrulamak için yalnızca iş ortağı olarak kullandığınız 100 kaydı döndürür.</span><span class="sxs-lookup"><span data-stu-id="33366-105">The API returns only 100 records that you as a partner can use to verify if the data is as you expected.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="33366-106">Bu API, 100 saniyelik bir sorgu yürütme zaman aşımına uğradı.</span><span class="sxs-lookup"><span data-stu-id="33366-106">This API has a query execution timeout of 100 seconds.</span></span> <span data-ttu-id="33366-107">API 'nin 100 saniyeden daha fazla sürdüğünü fark ederseniz, sorgu sözdizimsel olarak yanlış olabilir veya 200 dışında bir hata kodu almış olursunuz.</span><span class="sxs-lookup"><span data-stu-id="33366-107">If you notice the API is taking more than 100 seconds, it is highly likely that the query is syntactically correct or else you would have received an error code other than 200.</span></span> <span data-ttu-id="33366-108">Sorgu söz dizimi doğruysa gerçek rapor oluşturma işlemi geçer.</span><span class="sxs-lookup"><span data-stu-id="33366-108">The actual report generation will pass if the query syntax is correct.</span></span>

<span data-ttu-id="33366-109">**İstek sözdizimi**</span><span class="sxs-lookup"><span data-stu-id="33366-109">**Request syntax**</span></span>

|    <span data-ttu-id="33366-110">Yöntem</span><span class="sxs-lookup"><span data-stu-id="33366-110">Method</span></span>    |    <span data-ttu-id="33366-111">İstek URI'si</span><span class="sxs-lookup"><span data-stu-id="33366-111">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="33366-112">GET</span><span class="sxs-lookup"><span data-stu-id="33366-112">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?<exportQuery={query text}|queryId={queryId}>`    |
|        |        |

<span data-ttu-id="33366-113">**İstek üst bilgisi**</span><span class="sxs-lookup"><span data-stu-id="33366-113">**Request header**</span></span>

|    <span data-ttu-id="33366-114">Üst bilgi</span><span class="sxs-lookup"><span data-stu-id="33366-114">Header</span></span>    |    <span data-ttu-id="33366-115">Tür</span><span class="sxs-lookup"><span data-stu-id="33366-115">Type</span></span>    |    <span data-ttu-id="33366-116">Açıklama</span><span class="sxs-lookup"><span data-stu-id="33366-116">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="33366-117">Yetkilendirme</span><span class="sxs-lookup"><span data-stu-id="33366-117">Authorization</span></span>    |    <span data-ttu-id="33366-118">string</span><span class="sxs-lookup"><span data-stu-id="33366-118">string</span></span>    |    <span data-ttu-id="33366-119">Gereklidir.</span><span class="sxs-lookup"><span data-stu-id="33366-119">Required.</span></span> <span data-ttu-id="33366-120">formdaki Azure Active Directory (AAD) erişim belirteci`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="33366-120">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="33366-121">İçerik Türü</span><span class="sxs-lookup"><span data-stu-id="33366-121">Content-Type</span></span>    |    <span data-ttu-id="33366-122">string</span><span class="sxs-lookup"><span data-stu-id="33366-122">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="33366-123">**Yol parametresi**</span><span class="sxs-lookup"><span data-stu-id="33366-123">**Path parameter**</span></span>

<span data-ttu-id="33366-124">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="33366-124">None</span></span>

<span data-ttu-id="33366-125">**Sorgu parametresi**</span><span class="sxs-lookup"><span data-stu-id="33366-125">**Query parameter**</span></span>

|    <span data-ttu-id="33366-126">Parametre Adı</span><span class="sxs-lookup"><span data-stu-id="33366-126">Parameter Name</span></span>    |    <span data-ttu-id="33366-127">Tür</span><span class="sxs-lookup"><span data-stu-id="33366-127">Type</span></span>    |    <span data-ttu-id="33366-128">Gerekli</span><span class="sxs-lookup"><span data-stu-id="33366-128">Required</span></span>    |    <span data-ttu-id="33366-129">Açıklama</span><span class="sxs-lookup"><span data-stu-id="33366-129">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="33366-130">exportQuery</span><span class="sxs-lookup"><span data-stu-id="33366-130">exportQuery</span></span>     |    <span data-ttu-id="33366-131">dize</span><span class="sxs-lookup"><span data-stu-id="33366-131">string</span></span>    |    <span data-ttu-id="33366-132">No</span><span class="sxs-lookup"><span data-stu-id="33366-132">No</span></span>    |    <span data-ttu-id="33366-133">Yürütülmesi gereken rapor sorgu dizesi</span><span class="sxs-lookup"><span data-stu-id="33366-133">Report query string that needs to be executed</span></span>     |
|    <span data-ttu-id="33366-134">QueryId</span><span class="sxs-lookup"><span data-stu-id="33366-134">queryId</span></span>     |    <span data-ttu-id="33366-135">dize</span><span class="sxs-lookup"><span data-stu-id="33366-135">string</span></span>    |    <span data-ttu-id="33366-136">No</span><span class="sxs-lookup"><span data-stu-id="33366-136">No</span></span>    |    <span data-ttu-id="33366-137">Geçerli bir var olan sorgu KIMLIĞI.</span><span class="sxs-lookup"><span data-stu-id="33366-137">A valid existing query ID.</span></span> <span data-ttu-id="33366-138">ExportQuery parametresinde belirtilen sorgu dizesiyle birbirini dışlayan dışlamalı</span><span class="sxs-lookup"><span data-stu-id="33366-138">Mutually exclusive with query string specified in exportQuery parameter</span></span>    |
|    <span data-ttu-id="33366-139">startTime</span><span class="sxs-lookup"><span data-stu-id="33366-139">startTime</span></span>     |    <span data-ttu-id="33366-140">dize</span><span class="sxs-lookup"><span data-stu-id="33366-140">string</span></span>    |    <span data-ttu-id="33366-141">No</span><span class="sxs-lookup"><span data-stu-id="33366-141">No</span></span>    |    <span data-ttu-id="33366-142">Verilerin olmasını istediğimiz başlangıç zamanı.</span><span class="sxs-lookup"><span data-stu-id="33366-142">Start time from which we want the data.</span></span> <span data-ttu-id="33366-143">Sorguda belirtilen TimeSpan 'yi geçersiz kılar</span><span class="sxs-lookup"><span data-stu-id="33366-143">It overrides timespan specified in the query</span></span>    |
|    <span data-ttu-id="33366-144">endTime</span><span class="sxs-lookup"><span data-stu-id="33366-144">endTime</span></span>     |    <span data-ttu-id="33366-145">dize</span><span class="sxs-lookup"><span data-stu-id="33366-145">string</span></span>    |    <span data-ttu-id="33366-146">No</span><span class="sxs-lookup"><span data-stu-id="33366-146">No</span></span>    |    <span data-ttu-id="33366-147">Verilerin ne kadar süre istediğini belirten bitiş zamanı.</span><span class="sxs-lookup"><span data-stu-id="33366-147">End time till which we want the data.</span></span> <span data-ttu-id="33366-148">Sorguda belirtilen TimeSpan 'yi geçersiz kılar</span><span class="sxs-lookup"><span data-stu-id="33366-148">It overrides timespan specified in the query</span></span>    |
|        |        |        |        |

<span data-ttu-id="33366-149">**İstek yükü**</span><span class="sxs-lookup"><span data-stu-id="33366-149">**Request payload**</span></span>

<span data-ttu-id="33366-150">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="33366-150">None</span></span>

<span data-ttu-id="33366-151">**Sözlük**</span><span class="sxs-lookup"><span data-stu-id="33366-151">**Glossary**</span></span>

<span data-ttu-id="33366-152">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="33366-152">None</span></span>

<span data-ttu-id="33366-153">**Response**</span><span class="sxs-lookup"><span data-stu-id="33366-153">**Response**</span></span>

<span data-ttu-id="33366-154">Yanıt yükü aşağıdaki şekilde yapılandırılır:</span><span class="sxs-lookup"><span data-stu-id="33366-154">The response payload is structured as follows:</span></span>

<span data-ttu-id="33366-155">Yanıt kodu: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="33366-155">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="33366-156">Yanıt yükü örneği:</span><span class="sxs-lookup"><span data-stu-id="33366-156">Response payload example:</span></span>

```json
Top 100 rows of query execution 
{ 
  "Value": [ 
    { 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="33366-157">**Sözlük**</span><span class="sxs-lookup"><span data-stu-id="33366-157">**Glossary**</span></span>

<span data-ttu-id="33366-158">Bu tablo, yanıttaki anahtar öğeleri tanımlar:</span><span class="sxs-lookup"><span data-stu-id="33366-158">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="33366-159">Parametre</span><span class="sxs-lookup"><span data-stu-id="33366-159">Parameter</span></span>    |    <span data-ttu-id="33366-160">Açıklama</span><span class="sxs-lookup"><span data-stu-id="33366-160">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="33366-161">TotalCount</span><span class="sxs-lookup"><span data-stu-id="33366-161">TotalCount</span></span>     |    <span data-ttu-id="33366-162">Değer dizisindeki veri kümesi sayısı</span><span class="sxs-lookup"><span data-stu-id="33366-162">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="33366-163">İleti</span><span class="sxs-lookup"><span data-stu-id="33366-163">Message</span></span>     |    <span data-ttu-id="33366-164">API 'nin yürütülmesindeki durum iletisi</span><span class="sxs-lookup"><span data-stu-id="33366-164">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="33366-165">Durum</span><span class="sxs-lookup"><span data-stu-id="33366-165">StatusCode</span></span>     |    <span data-ttu-id="33366-166">Sonuç kodu.</span><span class="sxs-lookup"><span data-stu-id="33366-166">Result Code.</span></span> <span data-ttu-id="33366-167">Olası değerler 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="33366-167">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
