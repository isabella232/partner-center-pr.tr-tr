---
title: Rapor yürütme API'sini duraklatma - Analizler verileri
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Bu API'yi kullanarak içgörüler için rapor yürütmeyi İş Ortağı Merkezi kullanın.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 1e490a6d5120d729f0ea4979a201e9a80ba2991c
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377417"
---
# <a name="pause-report-executions-api"></a><span data-ttu-id="c05d3-103">Rapor yürütmeleri API'sini duraklatma</span><span class="sxs-lookup"><span data-stu-id="c05d3-103">Pause report executions API</span></span>

<span data-ttu-id="c05d3-104">Yürütme sırasında bu API raporların zamanlanmış yürütülmesini duraklatıyor.</span><span class="sxs-lookup"><span data-stu-id="c05d3-104">On execution, this API pauses the scheduled execution of reports.</span></span>

<span data-ttu-id="c05d3-105">**İstek söz dizimi**</span><span class="sxs-lookup"><span data-stu-id="c05d3-105">**Request syntax**</span></span>

|    <span data-ttu-id="c05d3-106">Yöntem</span><span class="sxs-lookup"><span data-stu-id="c05d3-106">Method</span></span>    |    <span data-ttu-id="c05d3-107">İstek URI'si</span><span class="sxs-lookup"><span data-stu-id="c05d3-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="c05d3-108">PUT</span><span class="sxs-lookup"><span data-stu-id="c05d3-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/pause/{ReportID}`    |
|        |        |

<span data-ttu-id="c05d3-109">**İstek üst bilgisi**</span><span class="sxs-lookup"><span data-stu-id="c05d3-109">**Request header**</span></span>

|    <span data-ttu-id="c05d3-110">Üst bilgi</span><span class="sxs-lookup"><span data-stu-id="c05d3-110">Header</span></span>    |    <span data-ttu-id="c05d3-111">Tür</span><span class="sxs-lookup"><span data-stu-id="c05d3-111">Type</span></span>    |    <span data-ttu-id="c05d3-112">Açıklama</span><span class="sxs-lookup"><span data-stu-id="c05d3-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="c05d3-113">Yetkilendirme</span><span class="sxs-lookup"><span data-stu-id="c05d3-113">Authorization</span></span>    |    <span data-ttu-id="c05d3-114">string</span><span class="sxs-lookup"><span data-stu-id="c05d3-114">string</span></span>    |    <span data-ttu-id="c05d3-115">Gereklidir.</span><span class="sxs-lookup"><span data-stu-id="c05d3-115">Required.</span></span> <span data-ttu-id="c05d3-116">Formda Azure Active Directory (AAD) erişim belirteci`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="c05d3-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="c05d3-117">İçerik Türü</span><span class="sxs-lookup"><span data-stu-id="c05d3-117">Content-Type</span></span>    |    <span data-ttu-id="c05d3-118">string</span><span class="sxs-lookup"><span data-stu-id="c05d3-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="c05d3-119">**Yol parametresi**</span><span class="sxs-lookup"><span data-stu-id="c05d3-119">**Path parameter**</span></span>

|    <span data-ttu-id="c05d3-120">Parametre Adı</span><span class="sxs-lookup"><span data-stu-id="c05d3-120">Parameter Name</span></span>    |    <span data-ttu-id="c05d3-121">Tür</span><span class="sxs-lookup"><span data-stu-id="c05d3-121">Type</span></span>    |    <span data-ttu-id="c05d3-122">Gerekli</span><span class="sxs-lookup"><span data-stu-id="c05d3-122">Required</span></span>    |    <span data-ttu-id="c05d3-123">Açıklama</span><span class="sxs-lookup"><span data-stu-id="c05d3-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="c05d3-124">reportId</span><span class="sxs-lookup"><span data-stu-id="c05d3-124">reportId</span></span>     |    <span data-ttu-id="c05d3-125">dize</span><span class="sxs-lookup"><span data-stu-id="c05d3-125">string</span></span>    |    <span data-ttu-id="c05d3-126">No</span><span class="sxs-lookup"><span data-stu-id="c05d3-126">No</span></span>    |    <span data-ttu-id="c05d3-127">Değiştirilecek raporun kimliği</span><span class="sxs-lookup"><span data-stu-id="c05d3-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="c05d3-128">**Sorgu parametresi**</span><span class="sxs-lookup"><span data-stu-id="c05d3-128">**Query parameter**</span></span>

<span data-ttu-id="c05d3-129">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="c05d3-129">None</span></span>

<span data-ttu-id="c05d3-130">**İstek yükü**</span><span class="sxs-lookup"><span data-stu-id="c05d3-130">**Request payload**</span></span>

<span data-ttu-id="c05d3-131">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="c05d3-131">None</span></span>

<span data-ttu-id="c05d3-132">**Sözlük**</span><span class="sxs-lookup"><span data-stu-id="c05d3-132">**Glossary**</span></span>

<span data-ttu-id="c05d3-133">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="c05d3-133">None</span></span>

<span data-ttu-id="c05d3-134">**Response**</span><span class="sxs-lookup"><span data-stu-id="c05d3-134">**Response**</span></span>

<span data-ttu-id="c05d3-135">Yanıt yükü aşağıdaki gibi yapılandırılmıştır:</span><span class="sxs-lookup"><span data-stu-id="c05d3-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="c05d3-136">Yanıt kodu: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="c05d3-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="c05d3-137">Yanıt yükü örneği:</span><span class="sxs-lookup"><span data-stu-id="c05d3-137">Response payload example:</span></span>

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

<span data-ttu-id="c05d3-138">**Sözlük**</span><span class="sxs-lookup"><span data-stu-id="c05d3-138">**Glossary**</span></span>

<span data-ttu-id="c05d3-139">Bu tablo yanıtta önemli öğeleri tanımlar:</span><span class="sxs-lookup"><span data-stu-id="c05d3-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="c05d3-140">Parametre</span><span class="sxs-lookup"><span data-stu-id="c05d3-140">Parameter</span></span>    |    <span data-ttu-id="c05d3-141">Açıklama</span><span class="sxs-lookup"><span data-stu-id="c05d3-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="c05d3-142">ReportId</span><span class="sxs-lookup"><span data-stu-id="c05d3-142">ReportId</span></span>     |    <span data-ttu-id="c05d3-143">Duraklatılmış raporun evrensel benzersiz tanımlayıcısı (UUID)</span><span class="sxs-lookup"><span data-stu-id="c05d3-143">Universally unique identifier (UUID) of the paused report</span></span>     |
|    <span data-ttu-id="c05d3-144">Raporadı</span><span class="sxs-lookup"><span data-stu-id="c05d3-144">ReportName</span></span>     |    <span data-ttu-id="c05d3-145">Oluşturma sırasında rapora verilen ad</span><span class="sxs-lookup"><span data-stu-id="c05d3-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="c05d3-146">Açıklama</span><span class="sxs-lookup"><span data-stu-id="c05d3-146">Description</span></span>     |    <span data-ttu-id="c05d3-147">Rapor oluşturma sırasında verilen açıklama</span><span class="sxs-lookup"><span data-stu-id="c05d3-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="c05d3-148">Queryıd</span><span class="sxs-lookup"><span data-stu-id="c05d3-148">QueryId</span></span>     |    <span data-ttu-id="c05d3-149">Sorgu kimliği raporun oluşturulma zamanında geçirildi</span><span class="sxs-lookup"><span data-stu-id="c05d3-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="c05d3-150">Sorgu</span><span class="sxs-lookup"><span data-stu-id="c05d3-150">Query</span></span>     |    <span data-ttu-id="c05d3-151">Bu rapor için yürütülecek sorgu metni</span><span class="sxs-lookup"><span data-stu-id="c05d3-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="c05d3-152">Kullanıcı</span><span class="sxs-lookup"><span data-stu-id="c05d3-152">User</span></span>     |    <span data-ttu-id="c05d3-153">Raporu oluşturmak için kullanılan kullanıcı kimliği</span><span class="sxs-lookup"><span data-stu-id="c05d3-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="c05d3-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="c05d3-154">CreatedTime</span></span>     |    <span data-ttu-id="c05d3-155">Raporun oluşturulma zamanı.</span><span class="sxs-lookup"><span data-stu-id="c05d3-155">Time the report was created.</span></span> <span data-ttu-id="c05d3-156">Saat biçimi yyyy-MM-ddTHH:mm:ssZ'dir</span><span class="sxs-lookup"><span data-stu-id="c05d3-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="c05d3-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="c05d3-157">ModifiedTime</span></span>     |    <span data-ttu-id="c05d3-158">Raporun en son değiştirilma zamanı.</span><span class="sxs-lookup"><span data-stu-id="c05d3-158">Time the report was last modified.</span></span> <span data-ttu-id="c05d3-159">Saat biçimi yyyy-MM-ddTHH:mm:ssZ'dir</span><span class="sxs-lookup"><span data-stu-id="c05d3-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="c05d3-160">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="c05d3-160">ExecuteNow</span></span>     |    <span data-ttu-id="c05d3-161">Raporun oluşturulma zamanında ayarlanmış ExecuteNow bayrağı</span><span class="sxs-lookup"><span data-stu-id="c05d3-161">ExecuteNow flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="c05d3-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="c05d3-162">StartTime</span></span>     |    <span data-ttu-id="c05d3-163">Rapor yürütmenin başlayacağı zaman.</span><span class="sxs-lookup"><span data-stu-id="c05d3-163">Time the report execution will begin.</span></span> <span data-ttu-id="c05d3-164">Saat biçimi yyyy-MM-ddTHH:mm:ssZ'dir</span><span class="sxs-lookup"><span data-stu-id="c05d3-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="c05d3-165">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="c05d3-165">ReportStatus</span></span>     |    <span data-ttu-id="c05d3-166">Rapor yürütme durumu.</span><span class="sxs-lookup"><span data-stu-id="c05d3-166">Status of the report execution.</span></span> <span data-ttu-id="c05d3-167">Olası değerler Duraklatılmış, Etkin ve Devre Dışı'dır.</span><span class="sxs-lookup"><span data-stu-id="c05d3-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="c05d3-168">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="c05d3-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="c05d3-169">Rapor oluşturma sırasında sağlanan yinelenme aralığı</span><span class="sxs-lookup"><span data-stu-id="c05d3-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="c05d3-170">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="c05d3-170">RecurrenceCount</span></span>     |    <span data-ttu-id="c05d3-171">Rapor oluşturma sırasında sağlanan yinelenme sayısı</span><span class="sxs-lookup"><span data-stu-id="c05d3-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="c05d3-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="c05d3-172">CallbackUrl</span></span>     |    <span data-ttu-id="c05d3-173">İstekte sağlanan geri çağırma URL'si</span><span class="sxs-lookup"><span data-stu-id="c05d3-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="c05d3-174">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="c05d3-174">CallbackMethod</span></span>    |    <span data-ttu-id="c05d3-175">İstekte sağlanan geri çağırma yöntemi</span><span class="sxs-lookup"><span data-stu-id="c05d3-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="c05d3-176">Biçimlendir</span><span class="sxs-lookup"><span data-stu-id="c05d3-176">Format</span></span>     |    <span data-ttu-id="c05d3-177">Rapor dosyalarının biçimi</span><span class="sxs-lookup"><span data-stu-id="c05d3-177">Format of the report files</span></span>     |
|    <span data-ttu-id="c05d3-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="c05d3-178">TotalCount</span></span>     |    <span data-ttu-id="c05d3-179">Değer dizisinde veri kümesi sayısı</span><span class="sxs-lookup"><span data-stu-id="c05d3-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="c05d3-180">İleti</span><span class="sxs-lookup"><span data-stu-id="c05d3-180">Message</span></span>     |    <span data-ttu-id="c05d3-181">API'nin yürütülmesinden gelen durum iletisi</span><span class="sxs-lookup"><span data-stu-id="c05d3-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="c05d3-182">Statuscode</span><span class="sxs-lookup"><span data-stu-id="c05d3-182">StatusCode</span></span>     |    <span data-ttu-id="c05d3-183">Sonuç Kodu.</span><span class="sxs-lookup"><span data-stu-id="c05d3-183">Result Code.</span></span> <span data-ttu-id="c05d3-184">Olası değerler: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="c05d3-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
