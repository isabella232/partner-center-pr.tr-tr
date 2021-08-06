---
title: rapor sorgularını silme apı-Analizler verileri
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Iş Ortağı Merkezi öngörülerine Kullanıcı tanımlı sorguyu silmek için bu API 'yi kullanın.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 4714d523ff9942838e9666fe75f3df21aae69e043b6d9be1e1819cbd52dfb6ff
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115681663"
---
# <a name="delete-report-queries-api"></a>Rapor sorguları API 'sini Sil

Bu API Kullanıcı tanımlı sorguları siler.

**İstek sözdizimi**

|    Yöntem    |    İstek URI'si    |
|    ----    |    ----    |
|    DELETE    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
|        |        |

**İstek üst bilgisi**

|    Üst bilgi    |    Tür    |    Description    |
|    ----    |    ----    |    ----    |
|    Yetkilendirme    |    string    |    Gereklidir. formdaki Azure Active Directory (AAD) erişim belirteci`Bearer <token>`    |
|    İçerik Türü    |    string    |    `Application/JSON`    |
|        |        |        |

**Yol parametresi**

|    Parametre Adı    |    Tür    |    Gerekli    |    Açıklama    |
|    ----    |    ----    |    ----    |    ----    |
|    QueryId     |    dize     |    No    |    Yalnızca bağımsız değişkende verilen KIMLIĞE sahip sorguların ayrıntılarını almak için filtrele     |
|        |        |        |        |

**Sorgu parametresi**

Hiçbiri

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
|    QueryId     |    Silinen sorgunun benzersiz UUID 'SI    |
|    Name     |    Silinen sorgunun adı    |
|    Description     |    Silinen sorgunun açıklaması     |
|    Sorgu     |    Silinen sorgunun rapor sorgu dizesi    |
|    Tür     |    Kullanıcı tarafından oluşturulan sorgular için userDefined olarak ayarla     |
|    Kullanıcı     |    Sorguyu oluşturan kullanıcı KIMLIĞI     |
|    CreatedTime     |    Sorgu oluşturma zamanı     |
|    TotalCount     |    Değer dizisindeki veri kümesi sayısı     |
|    İleti     |    API 'nin yürütülmesindeki durum iletisi     |
|    Durum     |    Sonuç kodu. Olası değerler 200, 400, 401, 403, 500     |
|        |        |
