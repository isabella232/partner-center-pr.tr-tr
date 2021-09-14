---
title: rapor yürütme apı 'si Analizler verileri sürdürür
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Bu API 'yi kullanarak, Iş Ortağı Merkezi öngörülerine duraklatılan herhangi bir raporu yürütmeyi sürdürebilirsiniz.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 1019e9e6f679084ca0a388d685b5239ecc2e09e2
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248478"
---
# <a name="resume-report-executions-api"></a>Rapor yürütmeleri API 'sini sürdürür

Bu API, yürütme sırasında, duraklatılmış bir raporun zamanlanan yürütmesini sürdürür.

**İstek sözdizimi**

|    Yöntem    |    İstek URI'si    |
|    ----    |    ----    |
|    PUT    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/resume/{ReportID}`    |
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
|    reportId     |    dize    |    No    |    Değiştirilen raporun KIMLIĞI     |
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
|    REPORTID     |    Devam eden raporun evrensel benzersiz tanımlayıcısı (UUID)     |
|    ReportName     |    Oluşturma sırasında rapora verilen ad     |
|    Description     |    Raporun oluşturulması sırasında verilen açıklama     |
|    QueryId     |    Rapor oluşturulduğu sırada geçirilen sorgu KIMLIĞI     |
|    Sorgu     |    Bu rapor için yürütülecek sorgu metni     |
|    Kullanıcı     |    Raporu oluşturmak için kullanılan Kullanıcı KIMLIĞI     |
|    CreatedTime     |    Raporun oluşturulduğu zaman. Saat biçimi yyyy-MM-ddTHH: mm: ssZ şeklindedir     |
|    ModifiedTime     |    Raporun son değiştirilme zamanı. Saat biçimi yyyy-MM-ddTHH: mm: ssZ şeklindedir     |
|    ExecuteNow     |    ExecuteNow bayrağı rapor oluşturulduğu sırada ayarlandı    |
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
