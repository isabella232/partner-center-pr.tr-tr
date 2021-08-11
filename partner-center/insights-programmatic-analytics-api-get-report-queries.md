---
title: rapor sorguları al API-Analizler verileri
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Rapor API 'sinde kullanılmak üzere tüm kullanılabilir sorguları almak için bu API 'yi kullanın.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 943eea26a08f1072b6ddcaf8136b7f9f757d52b8c0170f03519b8787c1877bd3
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115695195"
---
# <a name="get-report-queries-api"></a>Rapor sorguları al API 'SI

Rapor sorgularını al API 'SI, raporlarda kullanıma sunulan tüm sorguları alır. Tüm sistem ve Kullanıcı tanımlı sorguları varsayılan olarak alır.

**İstek sözdizimi**

|    Yöntem    |    İstek URI'si    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
|        |        |

**İstek üst bilgisi**

|    Üst bilgi    |    Tür    |    Description    |
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
|    Includesystemqueries     |    boolean     |    No    |    Yanıta önceden tanımlanmış sistem sorgularını dahil et     |
|    Includeonlysystemqueries     |    boolean     |    No    |    Yanıta yalnızca sistem sorgularını dahil et     |
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
|    Description     |    Sorgunun oluşturulması sırasında verilen açıklama     |
|    Sorgu     |    Rapor sorgu dizesi     |
|    Tür     |    Önceden tanımlı sistem sorguları için Kullanıcı tarafından oluşturulan sorgular ve sistem için userDefined olarak ayarla     |
|    Kullanıcı     |    Sorguyu oluşturan kullanıcı KIMLIĞI     |
|    CreatedTime     |    Sorgu oluşturma zamanı     |
|    TotalCount     |    Değer dizisindeki veri kümesi sayısı     |
|    İleti     |    API 'nin yürütülmesindeki durum iletisi     |
|    Durum     |    Sonuç kodu. Olası değerler 200, 400, 401, 403, 500     |
|        |        |
