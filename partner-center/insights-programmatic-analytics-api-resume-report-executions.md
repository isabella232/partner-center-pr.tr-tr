---
title: Rapor yürütme API'sini sürdürme - Analizler yürütme
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Bu API'yi kullanarak herhangi bir duraklatılmış raporun içgörülerde yürütülmesini İş Ortağı Merkezi kullanın.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 1372823425f3aefd025ffc3441623c1ceee34e1e
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377415"
---
# <a name="resume-report-executions-api"></a><span data-ttu-id="25151-103">Rapor yürütme API'sini sürdürme</span><span class="sxs-lookup"><span data-stu-id="25151-103">Resume report executions API</span></span>

<span data-ttu-id="25151-104">Yürütme sırasında, bu API duraklatılmış bir raporun zamanlanmış yürütmesini sürdürür.</span><span class="sxs-lookup"><span data-stu-id="25151-104">On execution, this API resumes the scheduled execution of a paused report.</span></span>

<span data-ttu-id="25151-105">**İstek söz dizimi**</span><span class="sxs-lookup"><span data-stu-id="25151-105">**Request syntax**</span></span>

|    <span data-ttu-id="25151-106">Yöntem</span><span class="sxs-lookup"><span data-stu-id="25151-106">Method</span></span>    |    <span data-ttu-id="25151-107">İstek URI'si</span><span class="sxs-lookup"><span data-stu-id="25151-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="25151-108">PUT</span><span class="sxs-lookup"><span data-stu-id="25151-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/resume/{ReportID}`    |
|        |        |

<span data-ttu-id="25151-109">**İstek üst bilgisi**</span><span class="sxs-lookup"><span data-stu-id="25151-109">**Request header**</span></span>

|    <span data-ttu-id="25151-110">Üst bilgi</span><span class="sxs-lookup"><span data-stu-id="25151-110">Header</span></span>    |    <span data-ttu-id="25151-111">Tür</span><span class="sxs-lookup"><span data-stu-id="25151-111">Type</span></span>    |    <span data-ttu-id="25151-112">Açıklama</span><span class="sxs-lookup"><span data-stu-id="25151-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="25151-113">Yetkilendirme</span><span class="sxs-lookup"><span data-stu-id="25151-113">Authorization</span></span>    |    <span data-ttu-id="25151-114">string</span><span class="sxs-lookup"><span data-stu-id="25151-114">string</span></span>    |    <span data-ttu-id="25151-115">Gereklidir.</span><span class="sxs-lookup"><span data-stu-id="25151-115">Required.</span></span> <span data-ttu-id="25151-116">Formda Azure Active Directory (AAD) erişim belirteci`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="25151-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="25151-117">İçerik Türü</span><span class="sxs-lookup"><span data-stu-id="25151-117">Content-Type</span></span>    |    <span data-ttu-id="25151-118">string</span><span class="sxs-lookup"><span data-stu-id="25151-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="25151-119">**Yol parametresi**</span><span class="sxs-lookup"><span data-stu-id="25151-119">**Path parameter**</span></span>

|    <span data-ttu-id="25151-120">Parametre Adı</span><span class="sxs-lookup"><span data-stu-id="25151-120">Parameter Name</span></span>    |    <span data-ttu-id="25151-121">Tür</span><span class="sxs-lookup"><span data-stu-id="25151-121">Type</span></span>    |    <span data-ttu-id="25151-122">Gerekli</span><span class="sxs-lookup"><span data-stu-id="25151-122">Required</span></span>    |    <span data-ttu-id="25151-123">Açıklama</span><span class="sxs-lookup"><span data-stu-id="25151-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="25151-124">reportId</span><span class="sxs-lookup"><span data-stu-id="25151-124">reportId</span></span>     |    <span data-ttu-id="25151-125">dize</span><span class="sxs-lookup"><span data-stu-id="25151-125">string</span></span>    |    <span data-ttu-id="25151-126">No</span><span class="sxs-lookup"><span data-stu-id="25151-126">No</span></span>    |    <span data-ttu-id="25151-127">Değiştirilecek raporun kimliği</span><span class="sxs-lookup"><span data-stu-id="25151-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="25151-128">**Sorgu parametresi**</span><span class="sxs-lookup"><span data-stu-id="25151-128">**Query parameter**</span></span>

<span data-ttu-id="25151-129">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="25151-129">None</span></span>

<span data-ttu-id="25151-130">**İstek yükü**</span><span class="sxs-lookup"><span data-stu-id="25151-130">**Request payload**</span></span>

<span data-ttu-id="25151-131">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="25151-131">None</span></span>

<span data-ttu-id="25151-132">**Sözlük**</span><span class="sxs-lookup"><span data-stu-id="25151-132">**Glossary**</span></span>

<span data-ttu-id="25151-133">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="25151-133">None</span></span>

<span data-ttu-id="25151-134">**Response**</span><span class="sxs-lookup"><span data-stu-id="25151-134">**Response**</span></span>

<span data-ttu-id="25151-135">Yanıt yükü aşağıdaki gibi yapılandırılmıştır:</span><span class="sxs-lookup"><span data-stu-id="25151-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="25151-136">Yanıt kodu: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="25151-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="25151-137">Yanıt yükü örneği:</span><span class="sxs-lookup"><span data-stu-id="25151-137">Response payload example:</span></span>

```json
{ 
  "Value": [ 
    { 
      "ReportId": "string", 
      "ReportName": "string", 
      "Description": "string", 
      "QueryId": "string", 
      "Query": "string", 
      "User": "string", 
      "CreatedTime": "string", 
      "ModifiedTime": "string", 
      "ExecuteNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      "RecurrenceCount": 0, 
      "CallbackUrl": "string", 
      "CallbackMethod": "string", 
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="25151-138">**Sözlük**</span><span class="sxs-lookup"><span data-stu-id="25151-138">**Glossary**</span></span>

<span data-ttu-id="25151-139">Bu tablo yanıtta önemli öğeleri tanımlar:</span><span class="sxs-lookup"><span data-stu-id="25151-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="25151-140">Parametre</span><span class="sxs-lookup"><span data-stu-id="25151-140">Parameter</span></span>    |    <span data-ttu-id="25151-141">Açıklama</span><span class="sxs-lookup"><span data-stu-id="25151-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="25151-142">ReportId</span><span class="sxs-lookup"><span data-stu-id="25151-142">ReportId</span></span>     |    <span data-ttu-id="25151-143">Sürdürülen raporun evrensel olarak benzersiz tanımlayıcısı (UUID)</span><span class="sxs-lookup"><span data-stu-id="25151-143">Universally unique identifier (UUID) of the resumed report</span></span>     |
|    <span data-ttu-id="25151-144">Raporadı</span><span class="sxs-lookup"><span data-stu-id="25151-144">ReportName</span></span>     |    <span data-ttu-id="25151-145">Oluşturma sırasında rapora verilen ad</span><span class="sxs-lookup"><span data-stu-id="25151-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="25151-146">Açıklama</span><span class="sxs-lookup"><span data-stu-id="25151-146">Description</span></span>     |    <span data-ttu-id="25151-147">Rapor oluşturma sırasında verilen açıklama</span><span class="sxs-lookup"><span data-stu-id="25151-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="25151-148">Queryıd</span><span class="sxs-lookup"><span data-stu-id="25151-148">QueryId</span></span>     |    <span data-ttu-id="25151-149">Sorgu kimliği raporun oluşturulma zamanında geçirildi</span><span class="sxs-lookup"><span data-stu-id="25151-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="25151-150">Sorgu</span><span class="sxs-lookup"><span data-stu-id="25151-150">Query</span></span>     |    <span data-ttu-id="25151-151">Bu rapor için yürütülecek sorgu metni</span><span class="sxs-lookup"><span data-stu-id="25151-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="25151-152">Kullanıcı</span><span class="sxs-lookup"><span data-stu-id="25151-152">User</span></span>     |    <span data-ttu-id="25151-153">Raporu oluşturmak için kullanılan kullanıcı kimliği</span><span class="sxs-lookup"><span data-stu-id="25151-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="25151-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="25151-154">CreatedTime</span></span>     |    <span data-ttu-id="25151-155">Raporun oluşturulma zamanı.</span><span class="sxs-lookup"><span data-stu-id="25151-155">Time the report was created.</span></span> <span data-ttu-id="25151-156">Saat biçimi yyyy-MM-ddTHH:mm:ssZ'dir</span><span class="sxs-lookup"><span data-stu-id="25151-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="25151-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="25151-157">ModifiedTime</span></span>     |    <span data-ttu-id="25151-158">Raporun en son değiştirilma zamanı.</span><span class="sxs-lookup"><span data-stu-id="25151-158">Time the report was last modified.</span></span> <span data-ttu-id="25151-159">Saat biçimi yyyy-MM-ddTHH:mm:ssZ'dir</span><span class="sxs-lookup"><span data-stu-id="25151-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="25151-160">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="25151-160">ExecuteNow</span></span>     |    <span data-ttu-id="25151-161">Raporun oluşturulma zamanında ayarlanmış ExecuteNow bayrağı</span><span class="sxs-lookup"><span data-stu-id="25151-161">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="25151-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="25151-162">StartTime</span></span>     |    <span data-ttu-id="25151-163">Rapor yürütmenin başlayacağı zaman.</span><span class="sxs-lookup"><span data-stu-id="25151-163">Time the report execution will begin.</span></span> <span data-ttu-id="25151-164">Saat biçimi yyyy-MM-ddTHH:mm:ssZ'dir</span><span class="sxs-lookup"><span data-stu-id="25151-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="25151-165">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="25151-165">ReportStatus</span></span>     |    <span data-ttu-id="25151-166">Rapor yürütme durumu.</span><span class="sxs-lookup"><span data-stu-id="25151-166">Status of the report execution.</span></span> <span data-ttu-id="25151-167">Olası değerler Duraklatılmış, Etkin ve Devre Dışı'dır.</span><span class="sxs-lookup"><span data-stu-id="25151-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="25151-168">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="25151-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="25151-169">Rapor oluşturma sırasında sağlanan yinelenme aralığı</span><span class="sxs-lookup"><span data-stu-id="25151-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="25151-170">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="25151-170">RecurrenceCount</span></span>     |    <span data-ttu-id="25151-171">Rapor oluşturma sırasında sağlanan yinelenme sayısı</span><span class="sxs-lookup"><span data-stu-id="25151-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="25151-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="25151-172">CallbackUrl</span></span>     |    <span data-ttu-id="25151-173">İstekte sağlanan geri çağırma URL'si</span><span class="sxs-lookup"><span data-stu-id="25151-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="25151-174">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="25151-174">CallbackMethod</span></span>    |    <span data-ttu-id="25151-175">İstekte sağlanan geri çağırma yöntemi</span><span class="sxs-lookup"><span data-stu-id="25151-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="25151-176">Biçimlendir</span><span class="sxs-lookup"><span data-stu-id="25151-176">Format</span></span>     |    <span data-ttu-id="25151-177">Rapor dosyalarının biçimi</span><span class="sxs-lookup"><span data-stu-id="25151-177">Format of the report files</span></span>     |
|    <span data-ttu-id="25151-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="25151-178">TotalCount</span></span>     |    <span data-ttu-id="25151-179">Değer dizisinde veri kümesi sayısı</span><span class="sxs-lookup"><span data-stu-id="25151-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="25151-180">İleti</span><span class="sxs-lookup"><span data-stu-id="25151-180">Message</span></span>     |    <span data-ttu-id="25151-181">API'nin yürütülmesinden gelen durum iletisi</span><span class="sxs-lookup"><span data-stu-id="25151-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="25151-182">Statuscode</span><span class="sxs-lookup"><span data-stu-id="25151-182">StatusCode</span></span>     |    <span data-ttu-id="25151-183">Sonuç Kodu.</span><span class="sxs-lookup"><span data-stu-id="25151-183">Result Code.</span></span> <span data-ttu-id="25151-184">Olası değerler: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="25151-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
