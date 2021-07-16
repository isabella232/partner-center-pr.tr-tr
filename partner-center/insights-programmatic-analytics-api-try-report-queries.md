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
# <a name="try-report-queries-api"></a>Rapor sorguları API 'sini deneyin

Bu API bir rapor sorgu ekstresi yürütür. API, verilerin beklediğiniz gibi olup olmadığını doğrulamak için yalnızca iş ortağı olarak kullandığınız 100 kaydı döndürür.

> [!IMPORTANT]
> Bu API, 100 saniyelik bir sorgu yürütme zaman aşımına uğradı. API 'nin 100 saniyeden daha fazla sürdüğünü fark ederseniz, sorgu sözdizimsel olarak yanlış olabilir veya 200 dışında bir hata kodu almış olursunuz. Sorgu söz dizimi doğruysa gerçek rapor oluşturma işlemi geçer.

**İstek sözdizimi**

|    Yöntem    |    İstek URI'si    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?<exportQuery={query text}|queryId={queryId}>`    |
|        |        |

**İstek üst bilgisi**

|    Üst bilgi    |    Tür    |    Açıklama    |
|    ----    |    ----    |    ----    |
|    Yetkilendirme    |    string    |    Gereklidir. formdaki Azure Active Directory (AAD) erişim belirteci`Bearer <token>`    |
|    İçerik Türü    |    string    |    `Application/JSON`    |
|        |        |        |

**Yol parametresi**

Hiçbiri

**Sorgu parametresi**

|    Parametre Adı    |    Tür    |    Gerekli    |    Açıklama    |
|    ----    |    ----    |    ----    |    ----    |
|    exportQuery     |    dize    |    No    |    Yürütülmesi gereken rapor sorgu dizesi     |
|    QueryId     |    dize    |    No    |    Geçerli bir var olan sorgu KIMLIĞI. ExportQuery parametresinde belirtilen sorgu dizesiyle birbirini dışlayan dışlamalı    |
|    startTime     |    dize    |    No    |    Verilerin olmasını istediğimiz başlangıç zamanı. Sorguda belirtilen TimeSpan 'yi geçersiz kılar    |
|    endTime     |    dize    |    No    |    Verilerin ne kadar süre istediğini belirten bitiş zamanı. Sorguda belirtilen TimeSpan 'yi geçersiz kılar    |
|        |        |        |        |

**İstek yükü**

Hiçbiri

**Sözlük**

Hiçbiri

**Response**

Yanıt yükü aşağıdaki şekilde yapılandırılır:

Yanıt kodu: 200, 400, 401, 403, 404, 500

Yanıt yükü örneği:

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

**Sözlük**

Bu tablo, yanıttaki anahtar öğeleri tanımlar:

|    Parametre    |    Açıklama    |
|    ----    |    ----    |
|    TotalCount     |    Değer dizisindeki veri kümesi sayısı     |
|    İleti     |    API 'nin yürütülmesindeki durum iletisi     |
|    Durum     |    Sonuç kodu. Olası değerler 200, 400, 401, 403, 500     |
|        |        |
