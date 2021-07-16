---
title: Rapor API'sini güncelleştirme
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Veri içgörüleri'nin rapor parametrelerini güncelleştirmek için İş Ortağı Merkezi kullanın.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: c5ab1059e9be9b42918d268da6a6c1a3cbfe52af
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377410"
---
# <a name="update-report-api"></a>Rapor API'sini güncelleştirme

Bu API, bir rapor parametresini değiştirmenize yardımcı olur.

**İstek söz dizimi**

|    Yöntem    |    İstek URI'si    |
|    ----    |    ----    |
|    PUT    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
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
|    reportId     |    dize    |    No    |    Değiştirilecek raporun kimliği     |
|        |        |        |        |

**Sorgu parametresi**

Hiçbiri

**İstek yükü**

```json
{ 
  "ReportName": "string", 
  "Description": "string", 
  "StartTime": "string", 
  "RecurrenceInterval": 0, 
  "RecurrenceCount": 0, 
  "Format": "string", 
  "CallbackUrl": "string",
 "CallbackMethod": "string"
}
```

**Sözlük**

Bu tabloda yanıtta yer alan öğelerin anahtar tanımları liste edilmiştir.

|    Parametre    |    Gerekli    |    Açıklama    |    İzin Verilen Değerler    |
|    ----    |    ----    |    ----    |    ----    |
|    Raporadı     |    Yes     |    Rapora atanacak ad     |    Dize     |
|    Açıklama     |    Hayır     |    Oluşturulan raporun açıklaması     |    Dize     |
|    StartTime     |    Yes    |    Rapor oluşturmanın başlayacağı zaman damgası     |    Dize     |
|    RecurrenceInterval     |    Hayır     |    Raporun saat olarak oluşturulma sıklığı. En düşük değer 4'tir     |    Tamsayı     |
|    RecurrenceCount     |    Hayır     |    Oluşturulacağız rapor sayısı. Varsayılan değer süresizdir.     |    Tamsayı     |
|    Biçimlendir     |    Hayır    |    Dışarı aktaran dosyanın dosya biçimi. Csv varsayılandır     |    CSV/TSV     |
|    CallbackURL     |    Hayır     |    rapor oluşturmada çağrıl olacak https geri çağırma URL'si     |    Dize     |
|    CallbackMethod    |    Hayır    |    Geri çağırma için kullanılacak Http yöntemi    |    GET/POST    |
|        |        |        |        |


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
|    ReportId     |    Güncelleştirilen raporun evrensel benzersiz tanımlayıcısı (UUID)     |
|    Raporadı     |    İstek yükünde rapora verilen ad     |
|    Açıklama     |    İstek yükünde rapora verilen açıklama     |
|    Queryıd     |    Sorgu kimliği raporun oluşturulma zamanında geçirildi     |
|    Sorgu     |    Bu rapor için yürütülecek sorgu metni     |
|    Kullanıcı     |    Raporu oluşturmak için kullanılan kullanıcı kimliği     |
|    CreatedTime     |    Raporun oluşturulma zamanı. Saat biçimi yyyy-MM-ddTHH:mm:ssZ'dir     |
|    ModifiedTime     |    Raporun en son değiştirilma zamanı. Saat biçimi yyyy-MM-ddTHH:mm:ssZ'dir     |
|    ExecuteNow     |    Raporun oluşturulma zamanında ayarlanmış ExecuteNow bayrağı    |
|    StartTime     |    Rapor yürütmenin başlayacağı zaman. Saat biçimi yyyy-MM-ddTHH: mm: ssZ şeklindedir     |
|    ReportStatus     |    Rapor yürütmenin durumu. Olası değerler duraklatıldı, etkin ve etkin değildir.     |
|    Recurrenceınterval     |    İstek yükünde belirtilen yinelenme aralığı     |
|    RecurrenceCount     |    İstek yükünde belirtilen yinelenme sayısı     |
|    CallbackUrl     |    İstekte belirtilen geri çağırma URL 'SI     |
|    CallbackMethod    |    İstekte belirtilen geri çağırma yöntemi    |
|    Biçimlendir     |    Rapor dosyalarının biçimi     |
|    TotalCount     |    Değer dizisindeki veri kümesi sayısı     |
|    İleti     |    API 'nin yürütülmesindeki durum iletisi     |
|    Durum     |    Sonuç kodu. Olası değerler 200, 400, 401, 403, 500     |
|        |        |