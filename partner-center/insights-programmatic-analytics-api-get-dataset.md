---
title: tüm veri kümelerini al API-Analizler verileri
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Iş Ortağı Merkezi öngörülerine tüm kullanılabilir veri kümelerinin ayrıntılarını almak için bu API 'yi kullanın.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 42ff7cc1f097e2423be5f1f7f9a7f62214d64949
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376960"
---
# <a name="get-all-datasets-api"></a><span data-ttu-id="80bc4-103">Tüm veri kümeleri API 'sini al</span><span class="sxs-lookup"><span data-stu-id="80bc4-103">Get all datasets API</span></span>

<span data-ttu-id="80bc4-104">Tüm veri kümelerini al API 'SI kullanılabilir tüm veri kümelerini alır.</span><span class="sxs-lookup"><span data-stu-id="80bc4-104">The Get all datasets API gets all the available datasets.</span></span> <span data-ttu-id="80bc4-105">Veri kümeleri tabloları, sütunları, ölçümleri ve zaman aralıklarını listeler.</span><span class="sxs-lookup"><span data-stu-id="80bc4-105">Datasets list the tables, columns, metrics, and time ranges.</span></span>

<span data-ttu-id="80bc4-106">**İstek sözdizimi**</span><span class="sxs-lookup"><span data-stu-id="80bc4-106">**Request syntax**</span></span>

|    <span data-ttu-id="80bc4-107">Yöntem</span><span class="sxs-lookup"><span data-stu-id="80bc4-107">Method</span></span>    |    <span data-ttu-id="80bc4-108">İstek URI'si</span><span class="sxs-lookup"><span data-stu-id="80bc4-108">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="80bc4-109">GET</span><span class="sxs-lookup"><span data-stu-id="80bc4-109">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset?datasetName={Dataset Name}`     |
|        |        |

<span data-ttu-id="80bc4-110">**İstek üst bilgisi**</span><span class="sxs-lookup"><span data-stu-id="80bc4-110">**Request header**</span></span>

|    <span data-ttu-id="80bc4-111">Üst bilgi</span><span class="sxs-lookup"><span data-stu-id="80bc4-111">Header</span></span>    |    <span data-ttu-id="80bc4-112">Tür</span><span class="sxs-lookup"><span data-stu-id="80bc4-112">Type</span></span>    |    <span data-ttu-id="80bc4-113">Açıklama</span><span class="sxs-lookup"><span data-stu-id="80bc4-113">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="80bc4-114">Yetkilendirme</span><span class="sxs-lookup"><span data-stu-id="80bc4-114">Authorization</span></span>    |    <span data-ttu-id="80bc4-115">string</span><span class="sxs-lookup"><span data-stu-id="80bc4-115">string</span></span>    |    <span data-ttu-id="80bc4-116">Gereklidir.</span><span class="sxs-lookup"><span data-stu-id="80bc4-116">Required.</span></span> <span data-ttu-id="80bc4-117">formdaki Azure Active Directory (AAD) erişim belirteci`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="80bc4-117">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="80bc4-118">İçerik Türü</span><span class="sxs-lookup"><span data-stu-id="80bc4-118">Content-Type</span></span>    |    <span data-ttu-id="80bc4-119">string</span><span class="sxs-lookup"><span data-stu-id="80bc4-119">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="80bc4-120">**Yol parametresi**</span><span class="sxs-lookup"><span data-stu-id="80bc4-120">**Path parameter**</span></span>

<span data-ttu-id="80bc4-121">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="80bc4-121">None</span></span>

<span data-ttu-id="80bc4-122">**Sorgu parametresi**</span><span class="sxs-lookup"><span data-stu-id="80bc4-122">**Query parameter**</span></span>

|    <span data-ttu-id="80bc4-123">Parametre Adı</span><span class="sxs-lookup"><span data-stu-id="80bc4-123">Parameter Name</span></span>    |    <span data-ttu-id="80bc4-124">Tür</span><span class="sxs-lookup"><span data-stu-id="80bc4-124">Type</span></span>    |    <span data-ttu-id="80bc4-125">Gerekli</span><span class="sxs-lookup"><span data-stu-id="80bc4-125">Required</span></span>    |    <span data-ttu-id="80bc4-126">Açıklama</span><span class="sxs-lookup"><span data-stu-id="80bc4-126">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="80bc4-127">datasetName</span><span class="sxs-lookup"><span data-stu-id="80bc4-127">datasetName</span></span>    |    <span data-ttu-id="80bc4-128">dize</span><span class="sxs-lookup"><span data-stu-id="80bc4-128">string</span></span>    |    <span data-ttu-id="80bc4-129">No</span><span class="sxs-lookup"><span data-stu-id="80bc4-129">No</span></span>    |    <span data-ttu-id="80bc4-130">Yalnızca bir veri kümesinin ayrıntılarını almak için filtrele</span><span class="sxs-lookup"><span data-stu-id="80bc4-130">Filter to get details of only one dataset</span></span>    |
|        |        |        |        |

<span data-ttu-id="80bc4-131">**İstek yükü**</span><span class="sxs-lookup"><span data-stu-id="80bc4-131">**Request payload**</span></span>

<span data-ttu-id="80bc4-132">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="80bc4-132">None</span></span>

<span data-ttu-id="80bc4-133">**Sözlük**</span><span class="sxs-lookup"><span data-stu-id="80bc4-133">**Glossary**</span></span>

<span data-ttu-id="80bc4-134">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="80bc4-134">None</span></span>

<span data-ttu-id="80bc4-135">**Response**</span><span class="sxs-lookup"><span data-stu-id="80bc4-135">**Response**</span></span>

<span data-ttu-id="80bc4-136">Yanıt yükü aşağıdaki şekilde yapılandırılır:</span><span class="sxs-lookup"><span data-stu-id="80bc4-136">The response payload is structured as follows:</span></span>

<span data-ttu-id="80bc4-137">Yanıt kodu: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="80bc4-137">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="80bc4-138">Yanıt yükü örneği:</span><span class="sxs-lookup"><span data-stu-id="80bc4-138">Response payload example:</span></span>

```json
{ 
   "Value":[ 
      { 
         "DatasetName ":"string", 
         "SelectableColumns":[ 
            "string" 
         ], 
         "AvailableMetrics":[ 
            "string" 
         ], 
         "AvailableDateRanges":[ 
            "string" 
         ], 
         "minimumRecurrenceInterval":0 
      } 
   ], 
   "TotalCount":0, 
   "Message":"<Error Message>", 
   "StatusCode": 0, 
} 
```

<span data-ttu-id="80bc4-139">**Sözlük**</span><span class="sxs-lookup"><span data-stu-id="80bc4-139">**Glossary**</span></span>

<span data-ttu-id="80bc4-140">Bu tablo, yanıttaki anahtar öğeleri tanımlar:</span><span class="sxs-lookup"><span data-stu-id="80bc4-140">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="80bc4-141">Parametre</span><span class="sxs-lookup"><span data-stu-id="80bc4-141">Parameter</span></span>    |    <span data-ttu-id="80bc4-142">Açıklama</span><span class="sxs-lookup"><span data-stu-id="80bc4-142">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="80bc4-143">DatasetName</span><span class="sxs-lookup"><span data-stu-id="80bc4-143">DatasetName</span></span>     |    <span data-ttu-id="80bc4-144">Bu dizi nesnesinin tanımladığı veri kümesinin adı</span><span class="sxs-lookup"><span data-stu-id="80bc4-144">Name of the dataset that this array object defines</span></span>     |
|    <span data-ttu-id="80bc4-145">SelectableColumns</span><span class="sxs-lookup"><span data-stu-id="80bc4-145">SelectableColumns</span></span>     |    <span data-ttu-id="80bc4-146">Seçme sütunlarında belirtilenebilir ham sütunlar</span><span class="sxs-lookup"><span data-stu-id="80bc4-146">Raw columns that can be specified in the select columns</span></span>     |
|    <span data-ttu-id="80bc4-147">Kullanılabilirlik Blemetrics</span><span class="sxs-lookup"><span data-stu-id="80bc4-147">AvailableMetrics</span></span>     |    <span data-ttu-id="80bc4-148">Seçme sütunlarında belirtilenebilir toplama/ölçüm sütun adları</span><span class="sxs-lookup"><span data-stu-id="80bc4-148">Aggregation/metric column names that can be specified in the select columns</span></span>     |
|    <span data-ttu-id="80bc4-149">Availableduteranges</span><span class="sxs-lookup"><span data-stu-id="80bc4-149">AvailableDateRanges</span></span>     |    <span data-ttu-id="80bc4-150">Veri kümesi için rapor sorgularında kullanılabilecek tarih aralığı</span><span class="sxs-lookup"><span data-stu-id="80bc4-150">Date range that can be used in report queries for the dataset</span></span>     |
|    <span data-ttu-id="80bc4-151">Minimumrecurrenceınterval</span><span class="sxs-lookup"><span data-stu-id="80bc4-151">minimumRecurrenceInterval</span></span>     |    <span data-ttu-id="80bc4-152">Yinelenme aralığının en düşük değeri</span><span class="sxs-lookup"><span data-stu-id="80bc4-152">Minimum value of Recurrence Interval</span></span>     |
|    <span data-ttu-id="80bc4-153">TotalCount</span><span class="sxs-lookup"><span data-stu-id="80bc4-153">TotalCount</span></span>     |    <span data-ttu-id="80bc4-154">Değer dizisindeki veri kümesi sayısı</span><span class="sxs-lookup"><span data-stu-id="80bc4-154">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="80bc4-155">İleti</span><span class="sxs-lookup"><span data-stu-id="80bc4-155">Message</span></span>     |    <span data-ttu-id="80bc4-156">API 'nin yürütülmesindeki durum iletisi</span><span class="sxs-lookup"><span data-stu-id="80bc4-156">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="80bc4-157">Durum</span><span class="sxs-lookup"><span data-stu-id="80bc4-157">StatusCode</span></span>     |    <span data-ttu-id="80bc4-158">Sonuç kodu.</span><span class="sxs-lookup"><span data-stu-id="80bc4-158">Result Code.</span></span> <span data-ttu-id="80bc4-159">Olası değerler 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="80bc4-159">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
