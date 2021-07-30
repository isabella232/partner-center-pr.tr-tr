---
title: Rapor yürütme API'sini duraklatma - Analizler verileri
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Bu API'yi kullanarak içgörüler için rapor yürütmeyi İş Ortağı Merkezi kullanın.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 798c5e87a3935923bd91d8e74716999fb8be4f54
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114836379"
---
# <a name="pause-report-executions-api"></a>Rapor yürütmeleri API'sini duraklatma

Yürütme sırasında bu API raporların zamanlanmış yürütülmesini duraklatıyor.

**İstek söz dizimi**

|    Yöntem    |    İstek URI'si    |
|    ----    |    ----    |
|    PUT    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/pause/{ReportID}`    |
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
|    ReportId     |    Duraklatılmış raporun evrensel benzersiz tanımlayıcısı (UUID)     |
|    Raporadı     |    Oluşturma sırasında rapora verilen ad     |
|    Description     |    Rapor oluşturma sırasında verilen açıklama     |
|    Queryıd     |    Sorgu kimliği raporun oluşturulma zamanında geçirildi     |
|    Sorgu     |    Bu rapor için yürütülecek sorgu metni     |
|    Kullanıcı     |    Raporu oluşturmak için kullanılan kullanıcı kimliği     |
|    CreatedTime     |    Raporun oluşturulma zamanı. Saat biçimi yyyy-MM-ddTHH:mm:ssZ'dir     |
|    ModifiedTime     |    Raporun en son değiştirilma zamanı. Saat biçimi yyyy-MM-ddTHH:mm:ssZ'dir     |
|    ExecuteNow     |    Raporun oluşturulma zamanında ayarlanmış ExecuteNow bayrağı     |
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
