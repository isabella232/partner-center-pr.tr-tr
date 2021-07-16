---
title: rapor apı 'si Analizler verileri silme
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Iş Ortağı Merkezi öngörülerine ait herhangi bir raporu silmek için bu API 'yi kullanın.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e060104f8f09f69c213ab1b22d4be08d58babced
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377422"
---
# <a name="delete-report-api"></a>Rapor API 'sini Sil

Bu API, yürütme sırasında tüm rapor ve rapor yürütme kayıtlarını siler.

**İstek sözdizimi**

|    Yöntem    |    İstek URI'si    |
|    ----    |    ----    |
|    DELETE    |    ` https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

**İstek üst bilgisi**

|    Üst bilgi    |    Tür    |    Açıklama    |
|    ----    |    ----    |    ----    |
|    Yetkilendirme    |    string    |    Gereklidir. formdaki Azure Active Directory (AAD) erişim belirteci`Bearer <token>`    |
|    İçerik Türü    |    string    |    `Application/JSON`    |
|        |        |        |

**Yol parametresi**

|    Parametre Adı    |    Tür    |    Gerekli    |    Açıklama    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId     |    dize    |    No    |    Silinen raporun KIMLIĞI    |
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
      "ReportId": "string", 
      "ReportName": "string", 
      "Description": "string", 
      "QueryId": "string", 
      "Query": "string", 
      "User": "string", 
      "CreatedTime": "string", 
      "ModifiedTime": "string", 
      "ExecuteNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      "RecurrenceCount": 0, 
      "CallbackUrl": "string",
      "CallbackMethod": "string",
      "Format": "string" 
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
|    REPORTID     |    Silinen raporun evrensel benzersiz tanımlayıcısı (UUID)     |
|    ReportName     |    Oluşturma sırasında rapora verilen ad     |
|    Açıklama     |    Raporun oluşturulması sırasında verilen açıklama     |
|    QueryId     |    Rapor oluşturulduğu sırada geçirilen sorgu KIMLIĞI     |
|    Sorgu     |    Bu rapor için yürütülecek sorgu metni     |
|    Kullanıcı     |    Raporu oluşturmak için kullanılan Kullanıcı KIMLIĞI     |
|    CreatedTime     |    Raporun oluşturulduğu zaman. Saat biçimi yyyy-MM-ddTHH: mm: ssZ şeklindedir     |
|    ModifiedTime     |    Raporun son değiştirilme zamanı. Saat biçimi yyyy-MM-ddTHH: mm: ssZ şeklindedir     |
|    ExecuteNow     |    ExecuteNow bayrağı rapor oluşturulduğu sırada ayarlandı     |
|    StartTime     |    Rapor yürütmenin başlayacağı zaman. Saat biçimi yyyy-MM-ddTHH: mm: ssZ şeklindedir     |
|    ReportStatus     |    Rapor yürütmenin durumu. Olası değerler duraklatıldı, etkin ve etkin değildir.     |
|    Recurrenceınterval     |    Rapor oluşturma sırasında belirtilen yinelenme aralığı     |
|    RecurrenceCount     |    Rapor oluşturma sırasında belirtilen yinelenme sayısı     |
|    CallbackUrl     |    İstekte belirtilen geri çağırma URL 'SI     |
|    CallbackMethod    |    İstekte belirtilen geri çağırma yöntemi    |
|    Biçimlendir     |    Rapor dosyalarının biçimi     |
|    TotalCount     |    Değer dizisindeki veri kümesi sayısı     |
|    İleti     |    API 'nin yürütülmesindeki durum iletisi     |
|    Durum     |    Sonuç kodu. Olası değerler 200, 400, 401, 403, 500     |
|        |        |
