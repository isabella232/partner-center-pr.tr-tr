---
title: İş ortağı öngörüleri verilerine erişmek için API listesi
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: İş ortağı öngörüleri verilerine erişmek için API listesi.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: cbd9f7fd08dfc4cfd247a0ed07a2c12845c5514c
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248477"
---
# <a name="available-apis-for-partner-insights-analytics"></a>Partner Insights Analytics için kullanılabilir API 'Ler

Ortak Öngörüler analizine ve bunlarla ilişkili işlevlere yönelik API 'lerin listesi aşağıda verilmiştir.

## <a name="dataset-pull-apis"></a>Veri kümesi çekme API 'Leri

***Tablo 1: veri kümesi çekme API 'Leri***

| **API** | **İşlev** |
| --- | --- |
| [Tüm veri kümelerini al](insights-programmatic-analytics-api-get-dataset.md) | Tüm kullanılabilir veri kümelerini alır. Veri kümeleri tabloları, sütunları, ölçümleri ve zaman aralıklarını listeler. |
|||

## <a name="query-management-apis"></a>Sorgu yönetimi API 'Leri

***Tablo 2: sorgu yönetimi API 'Leri***

| **API** | **İşlev** |
| --- | --- |
| [Rapor sorgusu oluştur](insights-programmatic-access-paradigm.md#create-report-query-api) | Sütunların ve ölçümlerin verilmesi gereken veri kümesini tanımlayan özel sorgular oluşturur. |
| [Rapor sorgusu al](insights-programmatic-analytics-api-get-report-queries.md) | Raporlarda kullanıma sunulan tüm sorguları alır. Tüm sistem ve Kullanıcı tanımlı sorguları varsayılan olarak alır. |
| [Rapor sorgusunu SIL](insights-programmatic-analytics-api-delete-report-queries.md) | Kullanıcı tanımlı sorguları siler. |
|||

## <a name="report-management-apis"></a>Rapor yönetimi API 'Leri

***Tablo 3: rapor yönetim API 'Leri***

| **API** | **İşlev** |
| --- | --- |
| [Rapor Oluştur](insights-programmatic-access-paradigm.md#create-report-api) | Düzenli aralıklarla yürütülecek bir sorgu zamanlar. |
| [Rapor sorgusunu dene](insights-programmatic-analytics-api-try-report-queries.md) | Bir rapor sorgu ekstresi yürütür. Yalnızca bir ortağın, verilerin beklendiğini doğrulamak için kullanabileceği 10 kayıt döndürür. |
| [Rapor Al](insights-programmatic-analytics-api-get-report.md) | Zamanlanan tüm raporları alın. |
| [Raporu Güncelleştir](insights-programmatic-analytics-api-update-report.md) | Rapor parametresini değiştirme. |
| [Raporu Sil](insights-programmatic-analytics-api-delete-report.md) | Tüm rapor ve rapor yürütme kayıtlarını siler. |
| [Rapor yürütmelerini Duraklat](insights-programmatic-analytics-api-pause-report-executions.md) | Raporların zamanlanan yürütmesini duraklatır. |
| [Rapor yürütmelerini sürdürür](insights-programmatic-analytics-api-resume-report-executions.md) | Duraklatılmış bir raporun zamanlanan yürütmesini sürdürür. |
|||

## <a name="report-execution-pull-apis"></a>Rapor yürütme çekme API 'Leri

***Tablo 4: rapor yürütme çekme API 'Leri***

| **API** | **İşlev** |
| --- | --- |
| [Rapor yürütmelerini al](insights-programmatic-access-paradigm.md#get-report-execution-api) | Belirli bir rapor için gerçekleşen tüm yürütmeleri alın. |
|||

## <a name="next-steps"></a>Sonraki adımlar

- [Swagger API URL 'si](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)aracılığıyla API 'leri deneyebilirsiniz.