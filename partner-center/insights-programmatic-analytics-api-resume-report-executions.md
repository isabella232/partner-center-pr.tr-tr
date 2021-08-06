---
title: Rapor yürütme API'sini sürdürme - Analizler yürütme
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Bu API'yi kullanarak herhangi bir duraklatılmış raporun içgörülerde yürütülmesini İş Ortağı Merkezi kullanın.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 8c429913e269b88a42216ca99c4a4afbc545eb599b6dcfeb1d5fb79af5fdd50c
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115697049"
---
# <a name="resume-report-executions-api"></a>Rapor yürütme API'sini sürdürme

Yürütme sırasında, bu API duraklatılmış bir raporun zamanlanmış yürütmesini sürdürür.

**İstek söz dizimi**

|    Yöntem    |    İstek URI'si    |
|    ----    |    ----    |
|    PUT    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/resume/{ReportID}`    |
|        |        |

**İstek üst bilgisi**

|    Üst bilgi    |    Tür    |    Description    |
|    ----    |    ----    |    ----    |
|    Yetkilendirme    |    string    |    Gereklidir. Formda Azure Active Directory (AAD) erişim belirteci`Bearer <token>`    |
|    İçerik Türü    |    string    |    `Application/JSON`    |
|        |        |        |

**Yol parametresi**

|    Parametre Adı    |    Tür    |    Gerekli    |    Açıklama    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId     |    dize    |    No    |    Değiştirilecek raporun kimliği     |
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

Bu tablo yanıtta önemli öğeleri tanımlar:

|    Parametre    |    Açıklama    |
|    ----    |    ----    |
|    ReportId     |    Sürdürülen raporun evrensel olarak benzersiz tanımlayıcısı (UUID)     |
|    Raporadı     |    Oluşturma sırasında rapora verilen ad     |
|    Description     |    Rapor oluşturma sırasında verilen açıklama     |
|    Queryıd     |    Sorgu kimliği raporun oluşturulma zamanında geçirildi     |
|    Sorgu     |    Bu rapor için yürütülecek sorgu metni     |
|    Kullanıcı     |    Raporu oluşturmak için kullanılan kullanıcı kimliği     |
|    CreatedTime     |    Raporun oluşturulma zamanı. Saat biçimi yyyy-MM-ddTHH:mm:ssZ'dir     |
|    ModifiedTime     |    Raporun en son değiştirilma zamanı. Saat biçimi yyyy-MM-ddTHH:mm:ssZ'dir     |
|    ExecuteNow     |    Raporun oluşturulma zamanında ayarlanmış ExecuteNow bayrağı    |
|    StartTime     |    Rapor yürütmenin başlayacağı zaman. Saat biçimi yyyy-MM-ddTHH:mm:ssZ'dir     |
|    ReportStatus     |    Rapor yürütme durumu. Olası değerler Duraklatılmış, Etkin ve Devre Dışı'dır.     |
|    RecurrenceInterval     |    Rapor oluşturma sırasında sağlanan yinelenme aralığı     |
|    RecurrenceCount     |    Rapor oluşturma sırasında sağlanan yinelenme sayısı     |
|    CallbackUrl     |    İstekte sağlanan geri çağırma URL'si     |
|    CallbackMethod    |    İstekte sağlanan geri çağırma yöntemi    |
|    Biçimlendir     |    Rapor dosyalarının biçimi     |
|    TotalCount     |    Değer dizisinde veri kümesi sayısı     |
|    İleti     |    API'nin yürütülmesinden gelen durum iletisi     |
|    Statuscode     |    Sonuç Kodu. Olası değerler: 200, 400, 401, 403, 500     |
|        |        |
