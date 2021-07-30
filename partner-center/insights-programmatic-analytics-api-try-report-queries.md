---
title: Rapor sorguları API'sini deneme
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Sorguyu test etmek ve sonuçları içgörülere göre doğrulamak için İş Ortağı Merkezi kullanın.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: c83b56b7d52e0b9feb598597b4a8e1fdaec98a3b
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114845610"
---
# <a name="try-report-queries-api"></a>Rapor sorguları API'sini deneme

Bu API bir Rapor sorgusu deyimi yürütür. API, bir iş ortağı olarak verilerin beklendiği gibi olduğunu doğrulamak için kullanabileceğiniz yalnızca 100 kayıt döndürür.

> [!IMPORTANT]
> Bu API'nin 100 saniyelik bir sorgu yürütme zaman aşımı var. API'nin 100 saniyeden uzun sürüyor olduğunu fark ediyorsanız, sorgunun bozulmamış olması büyük olasılıkla doğrudur, yoksa 200 dışında bir hata kodu alırsınız. Sorgu söz dizimi doğruysa gerçek rapor oluşturma başarılı olur.

**İstek söz dizimi**

|    Yöntem    |    İstek URI'si    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?<exportQuery={query text}|queryId={queryId}>`    |
|        |        |

**İstek üst bilgisi**

|    Üst bilgi    |    Tür    |    Description    |
|    ----    |    ----    |    ----    |
|    Yetkilendirme    |    string    |    Gereklidir. Formda Azure Active Directory (AAD) erişim belirteci`Bearer <token>`    |
|    İçerik Türü    |    string    |    `Application/JSON`    |
|        |        |        |

**Yol parametresi**

Hiçbiri

**Sorgu parametresi**

|    Parametre Adı    |    Tür    |    Gerekli    |    Açıklama    |
|    ----    |    ----    |    ----    |    ----    |
|    exportQuery     |    dize    |    No    |    Yürütül olması gereken rapor sorgu dizesi     |
|    Queryıd     |    dize    |    No    |    Geçerli bir mevcut sorgu kimliği. exportQuery parametresinde belirtilen sorgu dizesiyle birbirini dışlar    |
|    startTime     |    dize    |    No    |    Verileri almak istediğiniz başlangıç zamanı. Sorguda belirtilen zaman zamanlarını geçersiz kılar    |
|    endTime     |    dize    |    No    |    Verileri almak istediğiniz bitiş zamanı. Sorguda belirtilen zaman zamanlarını geçersiz kılar    |
|        |        |        |        |

**İstek yükü**

Hiçbiri

**Sözlük**

Hiçbiri

**Response**

Yanıt yükü aşağıdaki gibi yapılandırılmıştır:

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

Bu tablo yanıtta önemli öğeleri tanımlar:

|    Parametre    |    Açıklama    |
|    ----    |    ----    |
|    TotalCount     |    Değer dizisinde veri kümesi sayısı     |
|    İleti     |    API'nin yürütülmesinden gelen durum iletisi     |
|    Statuscode     |    Sonuç Kodu. Olası değerler: 200, 400, 401, 403, 500     |
|        |        |
