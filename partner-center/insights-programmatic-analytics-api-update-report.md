---
title: Rapor API'sini güncelleştirme
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Veri içgörüleri'nin rapor parametrelerini güncelleştirmek için İş Ortağı Merkezi kullanın.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: c5ab1059e9be9b42918d268da6a6c1a3cbfe52af
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377410"
---
# <a name="update-report-api"></a><span data-ttu-id="5e72d-103">Rapor API'sini güncelleştirme</span><span class="sxs-lookup"><span data-stu-id="5e72d-103">Update report API</span></span>

<span data-ttu-id="5e72d-104">Bu API, bir rapor parametresini değiştirmenize yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="5e72d-104">This API helps you modify a report parameter.</span></span>

<span data-ttu-id="5e72d-105">**İstek söz dizimi**</span><span class="sxs-lookup"><span data-stu-id="5e72d-105">**Request syntax**</span></span>

|    <span data-ttu-id="5e72d-106">Yöntem</span><span class="sxs-lookup"><span data-stu-id="5e72d-106">Method</span></span>    |    <span data-ttu-id="5e72d-107">İstek URI'si</span><span class="sxs-lookup"><span data-stu-id="5e72d-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="5e72d-108">PUT</span><span class="sxs-lookup"><span data-stu-id="5e72d-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

<span data-ttu-id="5e72d-109">**İstek üst bilgisi**</span><span class="sxs-lookup"><span data-stu-id="5e72d-109">**Request header**</span></span>

|    <span data-ttu-id="5e72d-110">Üst bilgi</span><span class="sxs-lookup"><span data-stu-id="5e72d-110">Header</span></span>    |    <span data-ttu-id="5e72d-111">Tür</span><span class="sxs-lookup"><span data-stu-id="5e72d-111">Type</span></span>    |    <span data-ttu-id="5e72d-112">Açıklama</span><span class="sxs-lookup"><span data-stu-id="5e72d-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="5e72d-113">Yetkilendirme</span><span class="sxs-lookup"><span data-stu-id="5e72d-113">Authorization</span></span>    |    <span data-ttu-id="5e72d-114">string</span><span class="sxs-lookup"><span data-stu-id="5e72d-114">string</span></span>    |    <span data-ttu-id="5e72d-115">Gereklidir.</span><span class="sxs-lookup"><span data-stu-id="5e72d-115">Required.</span></span> <span data-ttu-id="5e72d-116">Formda Azure Active Directory (AAD) erişim belirteci`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="5e72d-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="5e72d-117">İçerik Türü</span><span class="sxs-lookup"><span data-stu-id="5e72d-117">Content-Type</span></span>    |    <span data-ttu-id="5e72d-118">string</span><span class="sxs-lookup"><span data-stu-id="5e72d-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="5e72d-119">**Yol parametresi**</span><span class="sxs-lookup"><span data-stu-id="5e72d-119">**Path parameter**</span></span>

|    <span data-ttu-id="5e72d-120">Parametre Adı</span><span class="sxs-lookup"><span data-stu-id="5e72d-120">Parameter Name</span></span>    |    <span data-ttu-id="5e72d-121">Tür</span><span class="sxs-lookup"><span data-stu-id="5e72d-121">Type</span></span>    |    <span data-ttu-id="5e72d-122">Gerekli</span><span class="sxs-lookup"><span data-stu-id="5e72d-122">Required</span></span>    |    <span data-ttu-id="5e72d-123">Açıklama</span><span class="sxs-lookup"><span data-stu-id="5e72d-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="5e72d-124">reportId</span><span class="sxs-lookup"><span data-stu-id="5e72d-124">reportId</span></span>     |    <span data-ttu-id="5e72d-125">dize</span><span class="sxs-lookup"><span data-stu-id="5e72d-125">string</span></span>    |    <span data-ttu-id="5e72d-126">No</span><span class="sxs-lookup"><span data-stu-id="5e72d-126">No</span></span>    |    <span data-ttu-id="5e72d-127">Değiştirilecek raporun kimliği</span><span class="sxs-lookup"><span data-stu-id="5e72d-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="5e72d-128">**Sorgu parametresi**</span><span class="sxs-lookup"><span data-stu-id="5e72d-128">**Query parameter**</span></span>

<span data-ttu-id="5e72d-129">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="5e72d-129">None</span></span>

<span data-ttu-id="5e72d-130">**İstek yükü**</span><span class="sxs-lookup"><span data-stu-id="5e72d-130">**Request payload**</span></span>

```json
{ 
  "ReportName": "string", 
  "Description": "string", 
  "StartTime": "string", 
  "RecurrenceInterval": 0, 
  "RecurrenceCount": 0, 
  "Format": "string", 
  "CallbackUrl": "string",
 "CallbackMethod": "string"
}
```

<span data-ttu-id="5e72d-131">**Sözlük**</span><span class="sxs-lookup"><span data-stu-id="5e72d-131">**Glossary**</span></span>

<span data-ttu-id="5e72d-132">Bu tabloda yanıtta yer alan öğelerin anahtar tanımları liste edilmiştir.</span><span class="sxs-lookup"><span data-stu-id="5e72d-132">This table lists the key definitions of elements in the response.</span></span>

|    <span data-ttu-id="5e72d-133">Parametre</span><span class="sxs-lookup"><span data-stu-id="5e72d-133">Parameter</span></span>    |    <span data-ttu-id="5e72d-134">Gerekli</span><span class="sxs-lookup"><span data-stu-id="5e72d-134">Required</span></span>    |    <span data-ttu-id="5e72d-135">Açıklama</span><span class="sxs-lookup"><span data-stu-id="5e72d-135">Description</span></span>    |    <span data-ttu-id="5e72d-136">İzin Verilen Değerler</span><span class="sxs-lookup"><span data-stu-id="5e72d-136">Allowed Values</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="5e72d-137">Raporadı</span><span class="sxs-lookup"><span data-stu-id="5e72d-137">ReportName</span></span>     |    <span data-ttu-id="5e72d-138">Yes</span><span class="sxs-lookup"><span data-stu-id="5e72d-138">Yes</span></span>     |    <span data-ttu-id="5e72d-139">Rapora atanacak ad</span><span class="sxs-lookup"><span data-stu-id="5e72d-139">Name to be assigned to the report</span></span>     |    <span data-ttu-id="5e72d-140">Dize</span><span class="sxs-lookup"><span data-stu-id="5e72d-140">String</span></span>     |
|    <span data-ttu-id="5e72d-141">Açıklama</span><span class="sxs-lookup"><span data-stu-id="5e72d-141">Description</span></span>     |    <span data-ttu-id="5e72d-142">Hayır</span><span class="sxs-lookup"><span data-stu-id="5e72d-142">No</span></span>     |    <span data-ttu-id="5e72d-143">Oluşturulan raporun açıklaması</span><span class="sxs-lookup"><span data-stu-id="5e72d-143">Description of the created report</span></span>     |    <span data-ttu-id="5e72d-144">Dize</span><span class="sxs-lookup"><span data-stu-id="5e72d-144">String</span></span>     |
|    <span data-ttu-id="5e72d-145">StartTime</span><span class="sxs-lookup"><span data-stu-id="5e72d-145">StartTime</span></span>     |    <span data-ttu-id="5e72d-146">Yes</span><span class="sxs-lookup"><span data-stu-id="5e72d-146">Yes</span></span>    |    <span data-ttu-id="5e72d-147">Rapor oluşturmanın başlayacağı zaman damgası</span><span class="sxs-lookup"><span data-stu-id="5e72d-147">Timestamp after which the report generation will begin</span></span>     |    <span data-ttu-id="5e72d-148">Dize</span><span class="sxs-lookup"><span data-stu-id="5e72d-148">String</span></span>     |
|    <span data-ttu-id="5e72d-149">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="5e72d-149">RecurrenceInterval</span></span>     |    <span data-ttu-id="5e72d-150">Hayır</span><span class="sxs-lookup"><span data-stu-id="5e72d-150">No</span></span>     |    <span data-ttu-id="5e72d-151">Raporun saat olarak oluşturulma sıklığı.</span><span class="sxs-lookup"><span data-stu-id="5e72d-151">Frequency at which the report should be generated in hours.</span></span> <span data-ttu-id="5e72d-152">En düşük değer 4'tir</span><span class="sxs-lookup"><span data-stu-id="5e72d-152">Minimum value is 4</span></span>     |    <span data-ttu-id="5e72d-153">Tamsayı</span><span class="sxs-lookup"><span data-stu-id="5e72d-153">Integer</span></span>     |
|    <span data-ttu-id="5e72d-154">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="5e72d-154">RecurrenceCount</span></span>     |    <span data-ttu-id="5e72d-155">Hayır</span><span class="sxs-lookup"><span data-stu-id="5e72d-155">No</span></span>     |    <span data-ttu-id="5e72d-156">Oluşturulacağız rapor sayısı.</span><span class="sxs-lookup"><span data-stu-id="5e72d-156">Numbers of report to be generated.</span></span> <span data-ttu-id="5e72d-157">Varsayılan değer süresizdir.</span><span class="sxs-lookup"><span data-stu-id="5e72d-157">Default is indefinite.</span></span>     |    <span data-ttu-id="5e72d-158">Tamsayı</span><span class="sxs-lookup"><span data-stu-id="5e72d-158">Integer</span></span>     |
|    <span data-ttu-id="5e72d-159">Biçimlendir</span><span class="sxs-lookup"><span data-stu-id="5e72d-159">Format</span></span>     |    <span data-ttu-id="5e72d-160">Hayır</span><span class="sxs-lookup"><span data-stu-id="5e72d-160">No</span></span>    |    <span data-ttu-id="5e72d-161">Dışarı aktaran dosyanın dosya biçimi.</span><span class="sxs-lookup"><span data-stu-id="5e72d-161">File format of the exported file.</span></span> <span data-ttu-id="5e72d-162">Csv varsayılandır</span><span class="sxs-lookup"><span data-stu-id="5e72d-162">Default is CSV</span></span>     |    <span data-ttu-id="5e72d-163">CSV/TSV</span><span class="sxs-lookup"><span data-stu-id="5e72d-163">CSV/TSV</span></span>     |
|    <span data-ttu-id="5e72d-164">CallbackURL</span><span class="sxs-lookup"><span data-stu-id="5e72d-164">CallbackURL</span></span>     |    <span data-ttu-id="5e72d-165">Hayır</span><span class="sxs-lookup"><span data-stu-id="5e72d-165">No</span></span>     |    <span data-ttu-id="5e72d-166">rapor oluşturmada çağrıl olacak https geri çağırma URL'si</span><span class="sxs-lookup"><span data-stu-id="5e72d-166">https callback URL to be called on report generation</span></span>     |    <span data-ttu-id="5e72d-167">Dize</span><span class="sxs-lookup"><span data-stu-id="5e72d-167">String</span></span>     |
|    <span data-ttu-id="5e72d-168">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="5e72d-168">CallbackMethod</span></span>    |    <span data-ttu-id="5e72d-169">Hayır</span><span class="sxs-lookup"><span data-stu-id="5e72d-169">No</span></span>    |    <span data-ttu-id="5e72d-170">Geri çağırma için kullanılacak Http yöntemi</span><span class="sxs-lookup"><span data-stu-id="5e72d-170">Http method to be used for callback</span></span>    |    <span data-ttu-id="5e72d-171">GET/POST</span><span class="sxs-lookup"><span data-stu-id="5e72d-171">GET/POST</span></span>    |
|        |        |        |        |


<span data-ttu-id="5e72d-172">**Response**</span><span class="sxs-lookup"><span data-stu-id="5e72d-172">**Response**</span></span>

<span data-ttu-id="5e72d-173">Yanıt yükü aşağıdaki gibi yapılandırılmıştır:</span><span class="sxs-lookup"><span data-stu-id="5e72d-173">The response payload is structured as follows:</span></span>

<span data-ttu-id="5e72d-174">Yanıt kodu: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="5e72d-174">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="5e72d-175">Yanıt yükü örneği:</span><span class="sxs-lookup"><span data-stu-id="5e72d-175">Response payload example:</span></span>

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

<span data-ttu-id="5e72d-176">**Sözlük**</span><span class="sxs-lookup"><span data-stu-id="5e72d-176">**Glossary**</span></span>

<span data-ttu-id="5e72d-177">Bu tablo yanıtta önemli öğeleri tanımlar:</span><span class="sxs-lookup"><span data-stu-id="5e72d-177">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="5e72d-178">Parametre</span><span class="sxs-lookup"><span data-stu-id="5e72d-178">Parameter</span></span>    |    <span data-ttu-id="5e72d-179">Açıklama</span><span class="sxs-lookup"><span data-stu-id="5e72d-179">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="5e72d-180">ReportId</span><span class="sxs-lookup"><span data-stu-id="5e72d-180">ReportId</span></span>     |    <span data-ttu-id="5e72d-181">Güncelleştirilen raporun evrensel benzersiz tanımlayıcısı (UUID)</span><span class="sxs-lookup"><span data-stu-id="5e72d-181">Universally unique identifier (UUID) of the report being updated</span></span>     |
|    <span data-ttu-id="5e72d-182">Raporadı</span><span class="sxs-lookup"><span data-stu-id="5e72d-182">ReportName</span></span>     |    <span data-ttu-id="5e72d-183">İstek yükünde rapora verilen ad</span><span class="sxs-lookup"><span data-stu-id="5e72d-183">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="5e72d-184">Açıklama</span><span class="sxs-lookup"><span data-stu-id="5e72d-184">Description</span></span>     |    <span data-ttu-id="5e72d-185">İstek yükünde rapora verilen açıklama</span><span class="sxs-lookup"><span data-stu-id="5e72d-185">Description given to the report in the request payload</span></span>     |
|    <span data-ttu-id="5e72d-186">Queryıd</span><span class="sxs-lookup"><span data-stu-id="5e72d-186">QueryId</span></span>     |    <span data-ttu-id="5e72d-187">Sorgu kimliği raporun oluşturulma zamanında geçirildi</span><span class="sxs-lookup"><span data-stu-id="5e72d-187">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="5e72d-188">Sorgu</span><span class="sxs-lookup"><span data-stu-id="5e72d-188">Query</span></span>     |    <span data-ttu-id="5e72d-189">Bu rapor için yürütülecek sorgu metni</span><span class="sxs-lookup"><span data-stu-id="5e72d-189">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="5e72d-190">Kullanıcı</span><span class="sxs-lookup"><span data-stu-id="5e72d-190">User</span></span>     |    <span data-ttu-id="5e72d-191">Raporu oluşturmak için kullanılan kullanıcı kimliği</span><span class="sxs-lookup"><span data-stu-id="5e72d-191">User ID used to create the report</span></span>     |
|    <span data-ttu-id="5e72d-192">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="5e72d-192">CreatedTime</span></span>     |    <span data-ttu-id="5e72d-193">Raporun oluşturulma zamanı.</span><span class="sxs-lookup"><span data-stu-id="5e72d-193">Time the report was created.</span></span> <span data-ttu-id="5e72d-194">Saat biçimi yyyy-MM-ddTHH:mm:ssZ'dir</span><span class="sxs-lookup"><span data-stu-id="5e72d-194">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="5e72d-195">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="5e72d-195">ModifiedTime</span></span>     |    <span data-ttu-id="5e72d-196">Raporun en son değiştirilma zamanı.</span><span class="sxs-lookup"><span data-stu-id="5e72d-196">Time the report was last modified.</span></span> <span data-ttu-id="5e72d-197">Saat biçimi yyyy-MM-ddTHH:mm:ssZ'dir</span><span class="sxs-lookup"><span data-stu-id="5e72d-197">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="5e72d-198">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="5e72d-198">ExecuteNow</span></span>     |    <span data-ttu-id="5e72d-199">Raporun oluşturulma zamanında ayarlanmış ExecuteNow bayrağı</span><span class="sxs-lookup"><span data-stu-id="5e72d-199">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="5e72d-200">StartTime</span><span class="sxs-lookup"><span data-stu-id="5e72d-200">StartTime</span></span>     |    <span data-ttu-id="5e72d-201">Rapor yürütmenin başlayacağı zaman.</span><span class="sxs-lookup"><span data-stu-id="5e72d-201">Time the report execution will begin.</span></span> <span data-ttu-id="5e72d-202">Saat biçimi yyyy-MM-ddTHH: mm: ssZ şeklindedir</span><span class="sxs-lookup"><span data-stu-id="5e72d-202">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="5e72d-203">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="5e72d-203">ReportStatus</span></span>     |    <span data-ttu-id="5e72d-204">Rapor yürütmenin durumu.</span><span class="sxs-lookup"><span data-stu-id="5e72d-204">Status of the report execution.</span></span> <span data-ttu-id="5e72d-205">Olası değerler duraklatıldı, etkin ve etkin değildir.</span><span class="sxs-lookup"><span data-stu-id="5e72d-205">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="5e72d-206">Recurrenceınterval</span><span class="sxs-lookup"><span data-stu-id="5e72d-206">RecurrenceInterval</span></span>     |    <span data-ttu-id="5e72d-207">İstek yükünde belirtilen yinelenme aralığı</span><span class="sxs-lookup"><span data-stu-id="5e72d-207">Recurrence interval provided in the request payload</span></span>     |
|    <span data-ttu-id="5e72d-208">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="5e72d-208">RecurrenceCount</span></span>     |    <span data-ttu-id="5e72d-209">İstek yükünde belirtilen yinelenme sayısı</span><span class="sxs-lookup"><span data-stu-id="5e72d-209">Recurrence count provided in the request payload</span></span>     |
|    <span data-ttu-id="5e72d-210">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="5e72d-210">CallbackUrl</span></span>     |    <span data-ttu-id="5e72d-211">İstekte belirtilen geri çağırma URL 'SI</span><span class="sxs-lookup"><span data-stu-id="5e72d-211">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="5e72d-212">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="5e72d-212">CallbackMethod</span></span>    |    <span data-ttu-id="5e72d-213">İstekte belirtilen geri çağırma yöntemi</span><span class="sxs-lookup"><span data-stu-id="5e72d-213">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="5e72d-214">Biçimlendir</span><span class="sxs-lookup"><span data-stu-id="5e72d-214">Format</span></span>     |    <span data-ttu-id="5e72d-215">Rapor dosyalarının biçimi</span><span class="sxs-lookup"><span data-stu-id="5e72d-215">Format of the report files</span></span>     |
|    <span data-ttu-id="5e72d-216">TotalCount</span><span class="sxs-lookup"><span data-stu-id="5e72d-216">TotalCount</span></span>     |    <span data-ttu-id="5e72d-217">Değer dizisindeki veri kümesi sayısı</span><span class="sxs-lookup"><span data-stu-id="5e72d-217">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="5e72d-218">İleti</span><span class="sxs-lookup"><span data-stu-id="5e72d-218">Message</span></span>     |    <span data-ttu-id="5e72d-219">API 'nin yürütülmesindeki durum iletisi</span><span class="sxs-lookup"><span data-stu-id="5e72d-219">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="5e72d-220">Durum</span><span class="sxs-lookup"><span data-stu-id="5e72d-220">StatusCode</span></span>     |    <span data-ttu-id="5e72d-221">Sonuç kodu.</span><span class="sxs-lookup"><span data-stu-id="5e72d-221">Result Code.</span></span> <span data-ttu-id="5e72d-222">Olası değerler 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="5e72d-222">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |