---
title: rapor sorguları al API-Analizler verileri
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Rapor API 'sinde kullanılmak üzere tüm kullanılabilir sorguları almak için bu API 'yi kullanın.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 3bf140576a19439990405cfef23190045e0a98be
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377419"
---
# <a name="get-report-queries-api"></a>Rapor sorguları al API 'SI

Rapor sorgularını al API 'SI, raporlarda kullanıma sunulan tüm sorguları alır. Tüm sistem ve Kullanıcı tanımlı sorguları varsayılan olarak alır.

**İstek sözdizimi**

|    Yöntem    |    İstek URI'si    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
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
|    QueryId     |    dize     |    No    |    Yalnızca bağımsız değişkende verilen KIMLIĞE sahip sorguların ayrıntılarını almak için filtrele     |
|    queryName     |    dize     |    No    |    Yalnızca bağımsız değişkende verilen ada sahip sorguların ayrıntılarını almak için filtrele     |
|    Includesystemqueries     |    boolean     |    Hayır    |    Yanıta önceden tanımlanmış sistem sorgularını dahil et     |
|    Includeonlysystemqueries     |    boolean     |    Hayır    |    Yanıta yalnızca sistem sorgularını dahil et     |
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

Bu tablo, yanıttaki anahtar öğeleri tanımlar:

|    Parametre    |    Açıklama    |
|    ----    |    ----    |
|    QueryId     |    Sorgunun benzersiz UUID 'SI     |
|    Name     |    Sorgu oluşturma sırasında sorguya verilen ad     |
|    Açıklama     |    Sorgunun oluşturulması sırasında verilen açıklama     |
|    Sorgu     |    Rapor sorgu dizesi     |
|    Tür     |    Önceden tanımlı sistem sorguları için Kullanıcı tarafından oluşturulan sorgular ve sistem için userDefined olarak ayarla     |
|    Kullanıcı     |    Sorguyu oluşturan kullanıcı KIMLIĞI     |
|    CreatedTime     |    Sorgu oluşturma zamanı     |
|    TotalCount     |    Değer dizisindeki veri kümesi sayısı     |
|    İleti     |    API 'nin yürütülmesindeki durum iletisi     |
|    Durum     |    Sonuç kodu. Olası değerler 200, 400, 401, 403, 500     |
|        |        |
