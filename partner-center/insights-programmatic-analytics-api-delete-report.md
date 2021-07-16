---
title: rapor apı 'si Analizler verileri silme
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Iş Ortağı Merkezi öngörülerine ait herhangi bir raporu silmek için bu API 'yi kullanın.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e060104f8f09f69c213ab1b22d4be08d58babced
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377422"
---
# <a name="delete-report-api"></a><span data-ttu-id="ca30e-103">Rapor API 'sini Sil</span><span class="sxs-lookup"><span data-stu-id="ca30e-103">Delete report API</span></span>

<span data-ttu-id="ca30e-104">Bu API, yürütme sırasında tüm rapor ve rapor yürütme kayıtlarını siler.</span><span class="sxs-lookup"><span data-stu-id="ca30e-104">On execution, this API deletes all of the report and report execution records.</span></span>

<span data-ttu-id="ca30e-105">**İstek sözdizimi**</span><span class="sxs-lookup"><span data-stu-id="ca30e-105">**Request syntax**</span></span>

|    <span data-ttu-id="ca30e-106">Yöntem</span><span class="sxs-lookup"><span data-stu-id="ca30e-106">Method</span></span>    |    <span data-ttu-id="ca30e-107">İstek URI'si</span><span class="sxs-lookup"><span data-stu-id="ca30e-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="ca30e-108">DELETE</span><span class="sxs-lookup"><span data-stu-id="ca30e-108">DELETE</span></span>    |    ` https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

<span data-ttu-id="ca30e-109">**İstek üst bilgisi**</span><span class="sxs-lookup"><span data-stu-id="ca30e-109">**Request header**</span></span>

|    <span data-ttu-id="ca30e-110">Üst bilgi</span><span class="sxs-lookup"><span data-stu-id="ca30e-110">Header</span></span>    |    <span data-ttu-id="ca30e-111">Tür</span><span class="sxs-lookup"><span data-stu-id="ca30e-111">Type</span></span>    |    <span data-ttu-id="ca30e-112">Açıklama</span><span class="sxs-lookup"><span data-stu-id="ca30e-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="ca30e-113">Yetkilendirme</span><span class="sxs-lookup"><span data-stu-id="ca30e-113">Authorization</span></span>    |    <span data-ttu-id="ca30e-114">string</span><span class="sxs-lookup"><span data-stu-id="ca30e-114">string</span></span>    |    <span data-ttu-id="ca30e-115">Gereklidir.</span><span class="sxs-lookup"><span data-stu-id="ca30e-115">Required.</span></span> <span data-ttu-id="ca30e-116">formdaki Azure Active Directory (AAD) erişim belirteci`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="ca30e-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="ca30e-117">İçerik Türü</span><span class="sxs-lookup"><span data-stu-id="ca30e-117">Content-Type</span></span>    |    <span data-ttu-id="ca30e-118">string</span><span class="sxs-lookup"><span data-stu-id="ca30e-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="ca30e-119">**Yol parametresi**</span><span class="sxs-lookup"><span data-stu-id="ca30e-119">**Path parameter**</span></span>

|    <span data-ttu-id="ca30e-120">Parametre Adı</span><span class="sxs-lookup"><span data-stu-id="ca30e-120">Parameter Name</span></span>    |    <span data-ttu-id="ca30e-121">Tür</span><span class="sxs-lookup"><span data-stu-id="ca30e-121">Type</span></span>    |    <span data-ttu-id="ca30e-122">Gerekli</span><span class="sxs-lookup"><span data-stu-id="ca30e-122">Required</span></span>    |    <span data-ttu-id="ca30e-123">Açıklama</span><span class="sxs-lookup"><span data-stu-id="ca30e-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="ca30e-124">reportId</span><span class="sxs-lookup"><span data-stu-id="ca30e-124">reportId</span></span>     |    <span data-ttu-id="ca30e-125">dize</span><span class="sxs-lookup"><span data-stu-id="ca30e-125">string</span></span>    |    <span data-ttu-id="ca30e-126">No</span><span class="sxs-lookup"><span data-stu-id="ca30e-126">No</span></span>    |    <span data-ttu-id="ca30e-127">Silinen raporun KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="ca30e-127">ID of the report being deleted</span></span>    |
|        |        |        |        |

<span data-ttu-id="ca30e-128">**Sorgu parametresi**</span><span class="sxs-lookup"><span data-stu-id="ca30e-128">**Query parameter**</span></span>

<span data-ttu-id="ca30e-129">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="ca30e-129">None</span></span>

<span data-ttu-id="ca30e-130">**İstek yükü**</span><span class="sxs-lookup"><span data-stu-id="ca30e-130">**Request payload**</span></span>

<span data-ttu-id="ca30e-131">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="ca30e-131">None</span></span>

<span data-ttu-id="ca30e-132">**Sözlük**</span><span class="sxs-lookup"><span data-stu-id="ca30e-132">**Glossary**</span></span>

<span data-ttu-id="ca30e-133">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="ca30e-133">None</span></span>

<span data-ttu-id="ca30e-134">**Response**</span><span class="sxs-lookup"><span data-stu-id="ca30e-134">**Response**</span></span>

<span data-ttu-id="ca30e-135">Yanıt yükü aşağıdaki şekilde yapılandırılır:</span><span class="sxs-lookup"><span data-stu-id="ca30e-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="ca30e-136">Yanıt kodu: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="ca30e-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="ca30e-137">Yanıt yükü örneği:</span><span class="sxs-lookup"><span data-stu-id="ca30e-137">Response payload example:</span></span>

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

<span data-ttu-id="ca30e-138">**Sözlük**</span><span class="sxs-lookup"><span data-stu-id="ca30e-138">**Glossary**</span></span>

<span data-ttu-id="ca30e-139">Bu tablo, yanıttaki anahtar öğeleri tanımlar:</span><span class="sxs-lookup"><span data-stu-id="ca30e-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="ca30e-140">Parametre</span><span class="sxs-lookup"><span data-stu-id="ca30e-140">Parameter</span></span>    |    <span data-ttu-id="ca30e-141">Açıklama</span><span class="sxs-lookup"><span data-stu-id="ca30e-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="ca30e-142">REPORTID</span><span class="sxs-lookup"><span data-stu-id="ca30e-142">ReportId</span></span>     |    <span data-ttu-id="ca30e-143">Silinen raporun evrensel benzersiz tanımlayıcısı (UUID)</span><span class="sxs-lookup"><span data-stu-id="ca30e-143">Universally unique identifier (UUID) of the deleted report</span></span>     |
|    <span data-ttu-id="ca30e-144">ReportName</span><span class="sxs-lookup"><span data-stu-id="ca30e-144">ReportName</span></span>     |    <span data-ttu-id="ca30e-145">Oluşturma sırasında rapora verilen ad</span><span class="sxs-lookup"><span data-stu-id="ca30e-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="ca30e-146">Açıklama</span><span class="sxs-lookup"><span data-stu-id="ca30e-146">Description</span></span>     |    <span data-ttu-id="ca30e-147">Raporun oluşturulması sırasında verilen açıklama</span><span class="sxs-lookup"><span data-stu-id="ca30e-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="ca30e-148">QueryId</span><span class="sxs-lookup"><span data-stu-id="ca30e-148">QueryId</span></span>     |    <span data-ttu-id="ca30e-149">Rapor oluşturulduğu sırada geçirilen sorgu KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="ca30e-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="ca30e-150">Sorgu</span><span class="sxs-lookup"><span data-stu-id="ca30e-150">Query</span></span>     |    <span data-ttu-id="ca30e-151">Bu rapor için yürütülecek sorgu metni</span><span class="sxs-lookup"><span data-stu-id="ca30e-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="ca30e-152">Kullanıcı</span><span class="sxs-lookup"><span data-stu-id="ca30e-152">User</span></span>     |    <span data-ttu-id="ca30e-153">Raporu oluşturmak için kullanılan Kullanıcı KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="ca30e-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="ca30e-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="ca30e-154">CreatedTime</span></span>     |    <span data-ttu-id="ca30e-155">Raporun oluşturulduğu zaman.</span><span class="sxs-lookup"><span data-stu-id="ca30e-155">Time the report was created.</span></span> <span data-ttu-id="ca30e-156">Saat biçimi yyyy-MM-ddTHH: mm: ssZ şeklindedir</span><span class="sxs-lookup"><span data-stu-id="ca30e-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="ca30e-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="ca30e-157">ModifiedTime</span></span>     |    <span data-ttu-id="ca30e-158">Raporun son değiştirilme zamanı.</span><span class="sxs-lookup"><span data-stu-id="ca30e-158">Time the report was last modified.</span></span> <span data-ttu-id="ca30e-159">Saat biçimi yyyy-MM-ddTHH: mm: ssZ şeklindedir</span><span class="sxs-lookup"><span data-stu-id="ca30e-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="ca30e-160">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="ca30e-160">ExecuteNow</span></span>     |    <span data-ttu-id="ca30e-161">ExecuteNow bayrağı rapor oluşturulduğu sırada ayarlandı</span><span class="sxs-lookup"><span data-stu-id="ca30e-161">ExecuteNow flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="ca30e-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="ca30e-162">StartTime</span></span>     |    <span data-ttu-id="ca30e-163">Rapor yürütmenin başlayacağı zaman.</span><span class="sxs-lookup"><span data-stu-id="ca30e-163">Time the report execution will begin.</span></span> <span data-ttu-id="ca30e-164">Saat biçimi yyyy-MM-ddTHH: mm: ssZ şeklindedir</span><span class="sxs-lookup"><span data-stu-id="ca30e-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="ca30e-165">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="ca30e-165">ReportStatus</span></span>     |    <span data-ttu-id="ca30e-166">Rapor yürütmenin durumu.</span><span class="sxs-lookup"><span data-stu-id="ca30e-166">Status of the report execution.</span></span> <span data-ttu-id="ca30e-167">Olası değerler duraklatıldı, etkin ve etkin değildir.</span><span class="sxs-lookup"><span data-stu-id="ca30e-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="ca30e-168">Recurrenceınterval</span><span class="sxs-lookup"><span data-stu-id="ca30e-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="ca30e-169">Rapor oluşturma sırasında belirtilen yinelenme aralığı</span><span class="sxs-lookup"><span data-stu-id="ca30e-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="ca30e-170">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="ca30e-170">RecurrenceCount</span></span>     |    <span data-ttu-id="ca30e-171">Rapor oluşturma sırasında belirtilen yinelenme sayısı</span><span class="sxs-lookup"><span data-stu-id="ca30e-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="ca30e-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="ca30e-172">CallbackUrl</span></span>     |    <span data-ttu-id="ca30e-173">İstekte belirtilen geri çağırma URL 'SI</span><span class="sxs-lookup"><span data-stu-id="ca30e-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="ca30e-174">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="ca30e-174">CallbackMethod</span></span>    |    <span data-ttu-id="ca30e-175">İstekte belirtilen geri çağırma yöntemi</span><span class="sxs-lookup"><span data-stu-id="ca30e-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="ca30e-176">Biçimlendir</span><span class="sxs-lookup"><span data-stu-id="ca30e-176">Format</span></span>     |    <span data-ttu-id="ca30e-177">Rapor dosyalarının biçimi</span><span class="sxs-lookup"><span data-stu-id="ca30e-177">Format of the report files</span></span>     |
|    <span data-ttu-id="ca30e-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="ca30e-178">TotalCount</span></span>     |    <span data-ttu-id="ca30e-179">Değer dizisindeki veri kümesi sayısı</span><span class="sxs-lookup"><span data-stu-id="ca30e-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="ca30e-180">İleti</span><span class="sxs-lookup"><span data-stu-id="ca30e-180">Message</span></span>     |    <span data-ttu-id="ca30e-181">API 'nin yürütülmesindeki durum iletisi</span><span class="sxs-lookup"><span data-stu-id="ca30e-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="ca30e-182">Durum</span><span class="sxs-lookup"><span data-stu-id="ca30e-182">StatusCode</span></span>     |    <span data-ttu-id="ca30e-183">Sonuç kodu.</span><span class="sxs-lookup"><span data-stu-id="ca30e-183">Result Code.</span></span> <span data-ttu-id="ca30e-184">Olası değerler 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="ca30e-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
