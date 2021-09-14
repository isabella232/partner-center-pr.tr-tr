---
title: Rapor sorguları API'si - Analizler al
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Rapor API'sinde kullanmak üzere tüm kullanılabilir sorguları almak için bu API'yi kullanın.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 5f65784ce93350c92e0ffe38849ce505f045e0b0
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248480"
---
# <a name="get-report-queries-api"></a>Rapor sorgularını al API'si

Rapor sorguları al API'si, raporlarda kullanılabilen tüm sorguları alır. Varsayılan olarak tüm sistem ve kullanıcı tanımlı sorguları alır.

**İstek söz dizimi**

|    Yöntem    |    İstek URI'si    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
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
|    Queryıd     |    dize     |    No    |    Yalnızca bağımsız değişkende verilen kimlikle sorguların ayrıntılarını almak için filtrele     |
|    queryName     |    dize     |    No    |    Yalnızca bağımsız değişkende verilen adla sorguların ayrıntılarını almak için filtrele     |
|    IncludeSystemQueries     |    boolean     |    No    |    Yanıta önceden tanımlanmış sistem sorgularını dahil etmek     |
|    IncludeOnlySystemQueries     |    boolean     |    No    |    Yanıta yalnızca sistem sorgularını dahil etmek     |
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
|    Queryıd     |    Sorgunun benzersiz UUID'i     |
|    Name     |    Sorgu oluşturma sırasında sorguya verilen ad     |
|    Description     |    Sorgunun oluşturulması sırasında verilen açıklama     |
|    Sorgu     |    Rapor sorgu dizesi     |
|    Tür     |    Önceden tanımlanmış sistem sorguları için kullanıcı tarafından oluşturulan sorgular ve sistem için userDefined olarak ayarlayın     |
|    Kullanıcı     |    Sorguyu oluşturan kullanıcı kimliği     |
|    CreatedTime     |    Sorgu oluşturma zamanı     |
|    TotalCount     |    Değer dizisinde veri kümesi sayısı     |
|    İleti     |    API'nin yürütülmesinden gelen durum iletisi     |
|    Statuscode     |    Sonuç Kodu. Olası değerler: 200, 400, 401, 403, 500     |
|        |        |
