---
title: rapor apı 'si Analizler verileri al
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Iş Ortağı Merkezi öngörülerine tüm kullanılabilir rapor KIMLIKLERINI almak için bu API 'yi kullanın.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 174a2f60a36cb46b287b787b177dd32236cef4eb
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377418"
---
# <a name="get-report-api"></a><span data-ttu-id="eb2da-103">Rapor API 'SI al</span><span class="sxs-lookup"><span data-stu-id="eb2da-103">Get report API</span></span>

<span data-ttu-id="eb2da-104">Bu API, zamanlanmış tüm raporları alır.</span><span class="sxs-lookup"><span data-stu-id="eb2da-104">This API gets all the reports that have been scheduled.</span></span>

<span data-ttu-id="eb2da-105">**İstek sözdizimi**</span><span class="sxs-lookup"><span data-stu-id="eb2da-105">**Request syntax**</span></span>

|    <span data-ttu-id="eb2da-106">Yöntem</span><span class="sxs-lookup"><span data-stu-id="eb2da-106">Method</span></span>    |    <span data-ttu-id="eb2da-107">İstek URI'si</span><span class="sxs-lookup"><span data-stu-id="eb2da-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="eb2da-108">GET</span><span class="sxs-lookup"><span data-stu-id="eb2da-108">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport?reportId={Report ID}&reportName={Report Name}&queryId={Query ID}` |
|        |        |

<span data-ttu-id="eb2da-109">**İstek üst bilgisi**</span><span class="sxs-lookup"><span data-stu-id="eb2da-109">**Request header**</span></span>

|    <span data-ttu-id="eb2da-110">Üst bilgi</span><span class="sxs-lookup"><span data-stu-id="eb2da-110">Header</span></span>    |    <span data-ttu-id="eb2da-111">Tür</span><span class="sxs-lookup"><span data-stu-id="eb2da-111">Type</span></span>    |    <span data-ttu-id="eb2da-112">Açıklama</span><span class="sxs-lookup"><span data-stu-id="eb2da-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="eb2da-113">Yetkilendirme</span><span class="sxs-lookup"><span data-stu-id="eb2da-113">Authorization</span></span>    |    <span data-ttu-id="eb2da-114">string</span><span class="sxs-lookup"><span data-stu-id="eb2da-114">string</span></span>    |    <span data-ttu-id="eb2da-115">Gereklidir.</span><span class="sxs-lookup"><span data-stu-id="eb2da-115">Required.</span></span> <span data-ttu-id="eb2da-116">formdaki Azure Active Directory (AAD) erişim belirteci`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="eb2da-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="eb2da-117">İçerik Türü</span><span class="sxs-lookup"><span data-stu-id="eb2da-117">Content-Type</span></span>    |    <span data-ttu-id="eb2da-118">string</span><span class="sxs-lookup"><span data-stu-id="eb2da-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="eb2da-119">**Yol parametresi**</span><span class="sxs-lookup"><span data-stu-id="eb2da-119">**Path parameter**</span></span>

<span data-ttu-id="eb2da-120">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="eb2da-120">None</span></span>

<span data-ttu-id="eb2da-121">**Sorgu parametresi**</span><span class="sxs-lookup"><span data-stu-id="eb2da-121">**Query parameter**</span></span>

|    <span data-ttu-id="eb2da-122">Parametre Adı</span><span class="sxs-lookup"><span data-stu-id="eb2da-122">Parameter Name</span></span>    |    <span data-ttu-id="eb2da-123">Tür</span><span class="sxs-lookup"><span data-stu-id="eb2da-123">Type</span></span>    |    <span data-ttu-id="eb2da-124">Gerekli</span><span class="sxs-lookup"><span data-stu-id="eb2da-124">Required</span></span>    |    <span data-ttu-id="eb2da-125">Açıklama</span><span class="sxs-lookup"><span data-stu-id="eb2da-125">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="eb2da-126">reportId</span><span class="sxs-lookup"><span data-stu-id="eb2da-126">reportId</span></span>     |    <span data-ttu-id="eb2da-127">dize</span><span class="sxs-lookup"><span data-stu-id="eb2da-127">string</span></span>    |    <span data-ttu-id="eb2da-128">No</span><span class="sxs-lookup"><span data-stu-id="eb2da-128">No</span></span>    |    <span data-ttu-id="eb2da-129">Yalnızca bu bağımsız değişkende verilen REPORTID 'ye sahip raporların ayrıntılarını almak için filtrele</span><span class="sxs-lookup"><span data-stu-id="eb2da-129">Filter to get details of only reports with the reportId given in this argument</span></span>     |
|    <span data-ttu-id="eb2da-130">reportName</span><span class="sxs-lookup"><span data-stu-id="eb2da-130">reportName</span></span>     |    <span data-ttu-id="eb2da-131">dize</span><span class="sxs-lookup"><span data-stu-id="eb2da-131">string</span></span>    |    <span data-ttu-id="eb2da-132">No</span><span class="sxs-lookup"><span data-stu-id="eb2da-132">No</span></span>    |    <span data-ttu-id="eb2da-133">Yalnızca bu bağımsız değişkende verilen reportName 'e sahip raporların ayrıntılarını almak için filtrele</span><span class="sxs-lookup"><span data-stu-id="eb2da-133">Filter to get details of only reports with the reportName given in this argument</span></span>     |
|    <span data-ttu-id="eb2da-134">QueryId</span><span class="sxs-lookup"><span data-stu-id="eb2da-134">queryId</span></span>     |    <span data-ttu-id="eb2da-135">dize</span><span class="sxs-lookup"><span data-stu-id="eb2da-135">string</span></span>    |    <span data-ttu-id="eb2da-136">No</span><span class="sxs-lookup"><span data-stu-id="eb2da-136">No</span></span>    |    <span data-ttu-id="eb2da-137">Yalnızca bu bağımsız değişkende verilen QueryId 'ye sahip raporların ayrıntılarını almak için filtrele</span><span class="sxs-lookup"><span data-stu-id="eb2da-137">Filter to get details of only reports with the queryId given in this argument</span></span>     |
|        |        |        |        |


<span data-ttu-id="eb2da-138">**İstek yükü**</span><span class="sxs-lookup"><span data-stu-id="eb2da-138">**Request payload**</span></span>

<span data-ttu-id="eb2da-139">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="eb2da-139">None</span></span>

<span data-ttu-id="eb2da-140">**Sözlük**</span><span class="sxs-lookup"><span data-stu-id="eb2da-140">**Glossary**</span></span>

<span data-ttu-id="eb2da-141">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="eb2da-141">None</span></span>

<span data-ttu-id="eb2da-142">**Response**</span><span class="sxs-lookup"><span data-stu-id="eb2da-142">**Response**</span></span>

<span data-ttu-id="eb2da-143">Yanıt yükü aşağıdaki şekilde yapılandırılır:</span><span class="sxs-lookup"><span data-stu-id="eb2da-143">The response payload is structured as follows:</span></span>

<span data-ttu-id="eb2da-144">Yanıt kodu: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="eb2da-144">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="eb2da-145">Yanıt yükü örneği:</span><span class="sxs-lookup"><span data-stu-id="eb2da-145">Response payload example:</span></span>

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
      "executeNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      " RecurrenceCount": 0, 
      "CallbackUrl": "string",
      "CallbackMethod": null,
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0 
}
```

<span data-ttu-id="eb2da-146">**Sözlük**</span><span class="sxs-lookup"><span data-stu-id="eb2da-146">**Glossary**</span></span>

<span data-ttu-id="eb2da-147">Bu tablo, yanıttaki anahtar öğeleri tanımlar:</span><span class="sxs-lookup"><span data-stu-id="eb2da-147">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="eb2da-148">Parametre</span><span class="sxs-lookup"><span data-stu-id="eb2da-148">Parameter</span></span>    |    <span data-ttu-id="eb2da-149">Açıklama</span><span class="sxs-lookup"><span data-stu-id="eb2da-149">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="eb2da-150">REPORTID</span><span class="sxs-lookup"><span data-stu-id="eb2da-150">ReportId</span></span>     |    <span data-ttu-id="eb2da-151">Oluşturulan raporun benzersiz UUID 'SI</span><span class="sxs-lookup"><span data-stu-id="eb2da-151">Unique UUID of the report that was created</span></span>     |
|    <span data-ttu-id="eb2da-152">ReportName</span><span class="sxs-lookup"><span data-stu-id="eb2da-152">ReportName</span></span>     |    <span data-ttu-id="eb2da-153">İstek yükünde rapora verilen ad</span><span class="sxs-lookup"><span data-stu-id="eb2da-153">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="eb2da-154">Açıklama</span><span class="sxs-lookup"><span data-stu-id="eb2da-154">Description</span></span>     |    <span data-ttu-id="eb2da-155">Rapor oluşturulduğunda verilen açıklama</span><span class="sxs-lookup"><span data-stu-id="eb2da-155">Description given when the report was created</span></span>     |
|    <span data-ttu-id="eb2da-156">QueryId</span><span class="sxs-lookup"><span data-stu-id="eb2da-156">QueryId</span></span>     |    <span data-ttu-id="eb2da-157">Rapor oluşturulduğu sırada geçirilen sorgu KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="eb2da-157">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="eb2da-158">Sorgu</span><span class="sxs-lookup"><span data-stu-id="eb2da-158">Query</span></span>     |    <span data-ttu-id="eb2da-159">Bu rapor için yürütülecek sorgu metni</span><span class="sxs-lookup"><span data-stu-id="eb2da-159">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="eb2da-160">Kullanıcı</span><span class="sxs-lookup"><span data-stu-id="eb2da-160">User</span></span>     |    <span data-ttu-id="eb2da-161">Raporu oluşturmak için kullanılan Kullanıcı KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="eb2da-161">User ID used to create the report</span></span>     |
|    <span data-ttu-id="eb2da-162">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="eb2da-162">CreatedTime</span></span>     |    <span data-ttu-id="eb2da-163">Raporun oluşturulduğu zaman.</span><span class="sxs-lookup"><span data-stu-id="eb2da-163">Time the report was created.</span></span> <span data-ttu-id="eb2da-164">Saat biçimi yyyy-MM-ddTHH: mm: ssZ şeklindedir</span><span class="sxs-lookup"><span data-stu-id="eb2da-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="eb2da-165">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="eb2da-165">ModifiedTime</span></span>     |    <span data-ttu-id="eb2da-166">Raporun son değiştirilme zamanı.</span><span class="sxs-lookup"><span data-stu-id="eb2da-166">Time the report was last modified.</span></span> <span data-ttu-id="eb2da-167">Saat biçimi yyyy-MM-ddTHH: mm: ssZ şeklindedir</span><span class="sxs-lookup"><span data-stu-id="eb2da-167">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="eb2da-168">executeNow</span><span class="sxs-lookup"><span data-stu-id="eb2da-168">executeNow</span></span>     |    <span data-ttu-id="eb2da-169">ExecuteNow bayrağı rapor oluşturulduğu sırada ayarlandı</span><span class="sxs-lookup"><span data-stu-id="eb2da-169">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="eb2da-170">StartTime</span><span class="sxs-lookup"><span data-stu-id="eb2da-170">StartTime</span></span>     |    <span data-ttu-id="eb2da-171">Yürütmenin başlayacağı zaman.</span><span class="sxs-lookup"><span data-stu-id="eb2da-171">Time execution will begin.</span></span> <span data-ttu-id="eb2da-172">Saat biçimi yyyy-MM-ddTHH: mm: ssZ şeklindedir</span><span class="sxs-lookup"><span data-stu-id="eb2da-172">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="eb2da-173">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="eb2da-173">ReportStatus</span></span>     |    <span data-ttu-id="eb2da-174">Rapor yürütmenin durumu.</span><span class="sxs-lookup"><span data-stu-id="eb2da-174">Status of the report execution.</span></span> <span data-ttu-id="eb2da-175">Olası değerler duraklatıldı, etkin ve etkin değildir.</span><span class="sxs-lookup"><span data-stu-id="eb2da-175">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="eb2da-176">Recurrenceınterval</span><span class="sxs-lookup"><span data-stu-id="eb2da-176">RecurrenceInterval</span></span>     |    <span data-ttu-id="eb2da-177">Rapor oluşturma sırasında belirtilen yinelenme aralığı</span><span class="sxs-lookup"><span data-stu-id="eb2da-177">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="eb2da-178">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="eb2da-178">RecurrenceCount</span></span>     |    <span data-ttu-id="eb2da-179">Rapor oluşturma sırasında belirtilen yinelenme sayısı</span><span class="sxs-lookup"><span data-stu-id="eb2da-179">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="eb2da-180">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="eb2da-180">CallbackUrl</span></span>     |    <span data-ttu-id="eb2da-181">İstekte belirtilen geri çağırma URL 'SI</span><span class="sxs-lookup"><span data-stu-id="eb2da-181">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="eb2da-182">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="eb2da-182">CallbackMethod</span></span>    |    <span data-ttu-id="eb2da-183">İstekte belirtilen geri çağırma yöntemi</span><span class="sxs-lookup"><span data-stu-id="eb2da-183">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="eb2da-184">Biçimlendir</span><span class="sxs-lookup"><span data-stu-id="eb2da-184">Format</span></span>     |    <span data-ttu-id="eb2da-185">Rapor dosyalarının biçimi</span><span class="sxs-lookup"><span data-stu-id="eb2da-185">Format of the report files</span></span>     |
|    <span data-ttu-id="eb2da-186">TotalCount</span><span class="sxs-lookup"><span data-stu-id="eb2da-186">TotalCount</span></span>     |    <span data-ttu-id="eb2da-187">Değer dizisindeki veri kümesi sayısı</span><span class="sxs-lookup"><span data-stu-id="eb2da-187">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="eb2da-188">İleti</span><span class="sxs-lookup"><span data-stu-id="eb2da-188">Message</span></span>     |    <span data-ttu-id="eb2da-189">API 'nin yürütülmesindeki durum iletisi</span><span class="sxs-lookup"><span data-stu-id="eb2da-189">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="eb2da-190">Durum</span><span class="sxs-lookup"><span data-stu-id="eb2da-190">StatusCode</span></span>     |    <span data-ttu-id="eb2da-191">Sonuç kodu.</span><span class="sxs-lookup"><span data-stu-id="eb2da-191">Result Code.</span></span> <span data-ttu-id="eb2da-192">Olası değerler 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="eb2da-192">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |