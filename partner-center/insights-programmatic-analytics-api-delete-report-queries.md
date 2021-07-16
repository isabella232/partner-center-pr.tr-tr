---
title: Rapor sorguları API'sini silme - Analizler silme
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Bu API'yi kullanarak içgörüler için kullanıcı İş Ortağı Merkezi silin.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e608068613edad1fca277ba5886c9c4bc962ffd2
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376977"
---
# <a name="delete-report-queries-api"></a>Rapor sorguları API'sini silme

Bu API, kullanıcı tanımlı sorguları siler.

**İstek söz dizimi**

|    Yöntem    |    İstek URI'si    |
|    ----    |    ----    |
|    DELETE    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
|        |        |

**İstek üst bilgisi**

|    Üst bilgi    |    Tür    |    Açıklama    |
|    ----    |    ----    |    ----    |
|    Yetkilendirme    |    string    |    Gereklidir. Formda Azure Active Directory (AAD) erişim belirteci`Bearer <token>`    |
|    İçerik Türü    |    string    |    `Application/JSON`    |
|        |        |        |

**Yol parametresi**

|    Parametre Adı    |    Tür    |    Gerekli    |    Açıklama    |
|    ----    |    ----    |    ----    |    ----    |
|    Queryıd     |    dize     |    No    |    Yalnızca bağımsız değişkende verilen kimlikle sorguların ayrıntılarını almak için filtrele     |
|        |        |        |        |

**Sorgu parametresi**

Hiçbiri

**İstek yükü**

Hiçbiri

**Sözlük**

Hiçbiri

**Response**

Yanıt yükü aşağıdaki gibi yapılandırılmıştır:

Yanıt kodu: 200, 400, 401, 403, 404, 500

Yanıt yükü örneği:

```json
{ 
  "Value": [ 
    { 
      "QueryId": "string", 
      "Name": "string", 
      "Description": "string", 
      "Query": "string", 
      "Type": "string", 
      "User": "string", 
      "CreatedTime": "string", 
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
|    Queryıd     |    Silinen sorgunun benzersiz UUID'i    |
|    Name     |    Silinen sorgunun adı    |
|    Açıklama     |    Silinen sorgunun açıklaması     |
|    Sorgu     |    Silinen sorgunun rapor sorgu dizesi    |
|    Tür     |    Kullanıcı tarafından oluşturulan sorgular için userDefined olarak ayarlayın     |
|    Kullanıcı     |    Sorguyu oluşturan kullanıcı kimliği     |
|    CreatedTime     |    Sorgu oluşturma zamanı     |
|    TotalCount     |    Değer dizisinde veri kümesi sayısı     |
|    İleti     |    API'nin yürütülmesinden gelen durum iletisi     |
|    Statuscode     |    Sonuç Kodu. Olası değerler: 200, 400, 401, 403, 500     |
|        |        |
