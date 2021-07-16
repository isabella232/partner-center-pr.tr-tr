---
title: İş ortağı içgörüleri verilerine erişmek için API listesi
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: İş ortağı içgörüleri verilerine erişmek için API listesi.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 71d04b6927e27b1d7a8d72bbdaa56b41cb113625
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377407"
---
# <a name="available-apis-for-partner-insights-analytics"></a><span data-ttu-id="2635c-103">İş ortağı içgörüleri analizi için kullanılabilir API'ler</span><span class="sxs-lookup"><span data-stu-id="2635c-103">Available APIs for partner insights analytics</span></span>

<span data-ttu-id="2635c-104">Aşağıda iş ortağı içgörüleri analizine ve ilişkili işlevlerine yönelik API'ler listesi ve ardından yer alın.</span><span class="sxs-lookup"><span data-stu-id="2635c-104">Following are the list of APIs for partner insights analytics and their associated functionalities.</span></span>

## <a name="dataset-pull-apis"></a><span data-ttu-id="2635c-105">Veri kümesi çekme API'leri</span><span class="sxs-lookup"><span data-stu-id="2635c-105">Dataset pull APIs</span></span>

<span data-ttu-id="2635c-106">***Tablo 1: Veri kümesi çekme API'leri***</span><span class="sxs-lookup"><span data-stu-id="2635c-106">***Table 1: Dataset pull APIs***</span></span>

| <span data-ttu-id="2635c-107">**API**</span><span class="sxs-lookup"><span data-stu-id="2635c-107">**API**</span></span> | <span data-ttu-id="2635c-108">**İşlev**</span><span class="sxs-lookup"><span data-stu-id="2635c-108">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="2635c-109">Tüm veri kümelerini al</span><span class="sxs-lookup"><span data-stu-id="2635c-109">Get all datasets</span></span>](insights-programmatic-analytics-api-get-dataset.md) | <span data-ttu-id="2635c-110">Kullanılabilir tüm veri kümelerini alır.</span><span class="sxs-lookup"><span data-stu-id="2635c-110">Gets all the available datasets.</span></span> <span data-ttu-id="2635c-111">Veri kümeleri tabloları, sütunları, ölçümleri ve zaman aralıklarını listelemektedir.</span><span class="sxs-lookup"><span data-stu-id="2635c-111">Datasets list the tables, columns, metrics, and time ranges.</span></span> |
|||

## <a name="query-management-apis"></a><span data-ttu-id="2635c-112">Sorgu yönetimi API'leri</span><span class="sxs-lookup"><span data-stu-id="2635c-112">Query management APIs</span></span>

<span data-ttu-id="2635c-113">***Tablo 2: Sorgu yönetimi API'leri***</span><span class="sxs-lookup"><span data-stu-id="2635c-113">***Table 2: Query management APIs***</span></span>

| <span data-ttu-id="2635c-114">**API**</span><span class="sxs-lookup"><span data-stu-id="2635c-114">**API**</span></span> | <span data-ttu-id="2635c-115">**İşlev**</span><span class="sxs-lookup"><span data-stu-id="2635c-115">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="2635c-116">Rapor Sorgusu Oluşturma</span><span class="sxs-lookup"><span data-stu-id="2635c-116">Create Report Query</span></span>](insights-programmatic-access-paradigm.md#create-report-query-api) | <span data-ttu-id="2635c-117">Sütunların ve ölçümlerin dışarı aktarması gereken veri kümelerini tanımlayan özel sorgular oluşturur.</span><span class="sxs-lookup"><span data-stu-id="2635c-117">Creates custom queries that define the dataset from which columns and metrics need to be exported.</span></span> |
| [<span data-ttu-id="2635c-118">GET Report Query</span><span class="sxs-lookup"><span data-stu-id="2635c-118">GET Report Query</span></span>](insights-programmatic-analytics-api-get-report-queries.md) | <span data-ttu-id="2635c-119">Raporlarda kullanılabilen tüm sorguları alır.</span><span class="sxs-lookup"><span data-stu-id="2635c-119">Gets all the queries available for use in reports.</span></span> <span data-ttu-id="2635c-120">Varsayılan olarak tüm sistem ve kullanıcı tanımlı sorguları alır.</span><span class="sxs-lookup"><span data-stu-id="2635c-120">Gets all the system and user-defined queries by default.</span></span> |
| [<span data-ttu-id="2635c-121">DELETE Report Query</span><span class="sxs-lookup"><span data-stu-id="2635c-121">DELETE Report Query</span></span>](insights-programmatic-analytics-api-delete-report-queries.md) | <span data-ttu-id="2635c-122">Kullanıcı tanımlı sorguları siler.</span><span class="sxs-lookup"><span data-stu-id="2635c-122">Deletes user-defined queries.</span></span> |
|||

## <a name="report-management-apis"></a><span data-ttu-id="2635c-123">Rapor yönetimi API'leri</span><span class="sxs-lookup"><span data-stu-id="2635c-123">Report management APIs</span></span>

<span data-ttu-id="2635c-124">***Tablo 3: Rapor yönetimi API'leri***</span><span class="sxs-lookup"><span data-stu-id="2635c-124">***Table 3: Report management APIs***</span></span>

| <span data-ttu-id="2635c-125">**API**</span><span class="sxs-lookup"><span data-stu-id="2635c-125">**API**</span></span> | <span data-ttu-id="2635c-126">**İşlev**</span><span class="sxs-lookup"><span data-stu-id="2635c-126">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="2635c-127">Rapor Oluşturma</span><span class="sxs-lookup"><span data-stu-id="2635c-127">Create Report</span></span>](insights-programmatic-access-paradigm.md#create-report-api) | <span data-ttu-id="2635c-128">Düzenli aralıklarla yürütülecek bir sorgu zamanlar.</span><span class="sxs-lookup"><span data-stu-id="2635c-128">Schedules a query to be executed at regular intervals.</span></span> |
| [<span data-ttu-id="2635c-129">TRY Report Query</span><span class="sxs-lookup"><span data-stu-id="2635c-129">TRY Report Query</span></span>](insights-programmatic-analytics-api-try-report-queries.md) | <span data-ttu-id="2635c-130">Bir Rapor sorgusu deyimi yürütür.</span><span class="sxs-lookup"><span data-stu-id="2635c-130">Executes a Report query statement.</span></span> <span data-ttu-id="2635c-131">Bir iş ortağının verilerin beklendiği gibi olup olduğunu doğrulamak için kullanabileceği yalnızca 10 kayıt döndürür.</span><span class="sxs-lookup"><span data-stu-id="2635c-131">Returns only 10 records that a partner can use to verify if the data is as expected.</span></span> |
| [<span data-ttu-id="2635c-132">Rapor Al</span><span class="sxs-lookup"><span data-stu-id="2635c-132">Get Report</span></span>](insights-programmatic-analytics-api-get-report.md) | <span data-ttu-id="2635c-133">Zamanlanmış olan tüm raporları al.</span><span class="sxs-lookup"><span data-stu-id="2635c-133">Get all the reports that have been scheduled.</span></span> |
| [<span data-ttu-id="2635c-134">Raporu Güncelleştirme</span><span class="sxs-lookup"><span data-stu-id="2635c-134">Update Report</span></span>](insights-programmatic-analytics-api-update-report.md) | <span data-ttu-id="2635c-135">Rapor parametresini değiştirme.</span><span class="sxs-lookup"><span data-stu-id="2635c-135">Modify a report parameter.</span></span> |
| [<span data-ttu-id="2635c-136">Raporu Sil</span><span class="sxs-lookup"><span data-stu-id="2635c-136">Delete Report</span></span>](insights-programmatic-analytics-api-delete-report.md) | <span data-ttu-id="2635c-137">Tüm raporu ve rapor yürütme kayıtlarını siler.</span><span class="sxs-lookup"><span data-stu-id="2635c-137">Deletes all the report and report execution records.</span></span> |
| [<span data-ttu-id="2635c-138">Rapor Yürütmelerini Duraklatma</span><span class="sxs-lookup"><span data-stu-id="2635c-138">Pause Report Executions</span></span>](insights-programmatic-analytics-api-pause-report-executions.md) | <span data-ttu-id="2635c-139">Raporların zamanlanmış yürütülmesini duraklatıyor.</span><span class="sxs-lookup"><span data-stu-id="2635c-139">Pauses the scheduled execution of reports.</span></span> |
| [<span data-ttu-id="2635c-140">Rapor Yürütmelerini Sürdürme</span><span class="sxs-lookup"><span data-stu-id="2635c-140">Resume Report Executions</span></span>](insights-programmatic-analytics-api-resume-report-executions.md) | <span data-ttu-id="2635c-141">Duraklatılmış bir raporun zamanlanmış yürütülmesini sürdürür.</span><span class="sxs-lookup"><span data-stu-id="2635c-141">Resumes the scheduled execution of a paused report.</span></span> |
|||

## <a name="report-execution-pull-apis"></a><span data-ttu-id="2635c-142">Rapor yürütme çekme API'leri</span><span class="sxs-lookup"><span data-stu-id="2635c-142">Report execution pull APIs</span></span>

<span data-ttu-id="2635c-143">***Tablo 4: Rapor yürütme çekme API'leri***</span><span class="sxs-lookup"><span data-stu-id="2635c-143">***Table 4: Report execution pull APIs***</span></span>

| <span data-ttu-id="2635c-144">**API**</span><span class="sxs-lookup"><span data-stu-id="2635c-144">**API**</span></span> | <span data-ttu-id="2635c-145">**İşlev**</span><span class="sxs-lookup"><span data-stu-id="2635c-145">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="2635c-146">Rapor Yürütmelerini Al</span><span class="sxs-lookup"><span data-stu-id="2635c-146">Get Report Executions</span></span>](insights-programmatic-access-paradigm.md#get-report-execution-api) | <span data-ttu-id="2635c-147">Verilen bir rapor için olan tüm yürütmeleri al.</span><span class="sxs-lookup"><span data-stu-id="2635c-147">Get all the executions that have happened for a given report.</span></span> |
|||

## <a name="next-steps"></a><span data-ttu-id="2635c-148">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="2635c-148">Next steps</span></span>

- <span data-ttu-id="2635c-149">API'leri [Swagger API URL'si aracılığıyla denemeniz gerekir.](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span><span class="sxs-lookup"><span data-stu-id="2635c-149">You can try out the APIs through the [Swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).</span></span>