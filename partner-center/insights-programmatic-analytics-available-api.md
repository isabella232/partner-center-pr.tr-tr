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
# <a name="available-apis-for-partner-insights-analytics"></a>İş ortağı içgörüleri analizi için kullanılabilir API'ler

Aşağıda iş ortağı içgörüleri analizine ve ilişkili işlevlerine yönelik API'ler listesi ve ardından yer alın.

## <a name="dataset-pull-apis"></a>Veri kümesi çekme API'leri

***Tablo 1: Veri kümesi çekme API'leri***

| **API** | **İşlev** |
| --- | --- |
| [Tüm veri kümelerini al](insights-programmatic-analytics-api-get-dataset.md) | Kullanılabilir tüm veri kümelerini alır. Veri kümeleri tabloları, sütunları, ölçümleri ve zaman aralıklarını listelemektedir. |
|||

## <a name="query-management-apis"></a>Sorgu yönetimi API'leri

***Tablo 2: Sorgu yönetimi API'leri***

| **API** | **İşlev** |
| --- | --- |
| [Rapor Sorgusu Oluşturma](insights-programmatic-access-paradigm.md#create-report-query-api) | Sütunların ve ölçümlerin dışarı aktarması gereken veri kümelerini tanımlayan özel sorgular oluşturur. |
| [GET Report Query](insights-programmatic-analytics-api-get-report-queries.md) | Raporlarda kullanılabilen tüm sorguları alır. Varsayılan olarak tüm sistem ve kullanıcı tanımlı sorguları alır. |
| [DELETE Report Query](insights-programmatic-analytics-api-delete-report-queries.md) | Kullanıcı tanımlı sorguları siler. |
|||

## <a name="report-management-apis"></a>Rapor yönetimi API'leri

***Tablo 3: Rapor yönetimi API'leri***

| **API** | **İşlev** |
| --- | --- |
| [Rapor Oluşturma](insights-programmatic-access-paradigm.md#create-report-api) | Düzenli aralıklarla yürütülecek bir sorgu zamanlar. |
| [TRY Report Query](insights-programmatic-analytics-api-try-report-queries.md) | Bir Rapor sorgusu deyimi yürütür. Bir iş ortağının verilerin beklendiği gibi olup olduğunu doğrulamak için kullanabileceği yalnızca 10 kayıt döndürür. |
| [Rapor Al](insights-programmatic-analytics-api-get-report.md) | Zamanlanmış olan tüm raporları al. |
| [Raporu Güncelleştirme](insights-programmatic-analytics-api-update-report.md) | Rapor parametresini değiştirme. |
| [Raporu Sil](insights-programmatic-analytics-api-delete-report.md) | Tüm raporu ve rapor yürütme kayıtlarını siler. |
| [Rapor Yürütmelerini Duraklatma](insights-programmatic-analytics-api-pause-report-executions.md) | Raporların zamanlanmış yürütülmesini duraklatıyor. |
| [Rapor Yürütmelerini Sürdürme](insights-programmatic-analytics-api-resume-report-executions.md) | Duraklatılmış bir raporun zamanlanmış yürütülmesini sürdürür. |
|||

## <a name="report-execution-pull-apis"></a>Rapor yürütme çekme API'leri

***Tablo 4: Rapor yürütme çekme API'leri***

| **API** | **İşlev** |
| --- | --- |
| [Rapor Yürütmelerini Al](insights-programmatic-access-paradigm.md#get-report-execution-api) | Verilen bir rapor için olan tüm yürütmeleri al. |
|||

## <a name="next-steps"></a>Sonraki adımlar

- API'leri [Swagger API URL'si aracılığıyla denemeniz gerekir.](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)