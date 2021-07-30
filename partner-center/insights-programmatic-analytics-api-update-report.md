---
title: Rapor API 'sini Güncelleştir
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Iş Ortağı Merkezi öngörülerinin rapor parametrelerini güncelleştirmek için bu API 'yi kullanın.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 64ef897dc3c883e4adfda4285183e441f27f3c7f
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114837042"
---
# <a name="update-report-api"></a>Rapor API 'sini Güncelleştir

Bu API, bir rapor parametresini değiştirmenize yardımcı olur.

**İstek sözdizimi**

|    Yöntem    |    İstek URI'si    |
|    ----    |    ----    |
|    PUT    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
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

Bu tabloda, yanıttaki öğelerin temel tanımları listelenmiştir.

|    Parametre    |    Gerekli    |    Açıklama    |    İzin Verilen Değerler    |
|    ----    |    ----    |    ----    |    ----    |
|    ReportName     |    Yes     |    Rapora atanacak ad     |    Dize     |
|    Açıklama     |    Hayır     |    Oluşturulan raporun açıklaması     |    Dize     |
|    StartTime     |    Yes    |    Rapor oluşturma işlemi başlamadan sonra zaman damgası     |    Dize     |
|    Recurrenceınterval     |    No     |    Raporun saat cinsinden oluşturulması gereken sıklık. En küçük değer 4 ' dir     |    Tamsayı     |
|    RecurrenceCount     |    No     |    Oluşturulacak rapor sayısı. Varsayılan değer sonsuzdir.     |    Tamsayı     |
|    Biçimlendir     |    No    |    İçe aktarılmış dosyanın dosya biçimi. Varsayılan CSV 'dir     |    CSV/TSV     |
|    CallbackURL     |    No     |    rapor oluşturma sırasında çağrılacak https geri çağırma URL 'SI     |    Dize     |
|    CallbackMethod    |    No    |    Geri arama için kullanılacak http yöntemi    |    AL/POSTALA    |
|        |        |        |        |


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
|    REPORTID     |    Güncelleştirilmekte olan raporun evrensel benzersiz tanımlayıcısı (UUID)     |
|    ReportName     |    İstek yükünde rapora verilen ad     |
|    Description     |    İstek yükünde rapora verilen açıklama     |
|    QueryId     |    Rapor oluşturulduğu sırada geçirilen sorgu KIMLIĞI     |
|    Sorgu     |    Bu rapor için yürütülecek sorgu metni     |
|    Kullanıcı     |    Raporu oluşturmak için kullanılan Kullanıcı KIMLIĞI     |
|    CreatedTime     |    Raporun oluşturulduğu zaman. Saat biçimi yyyy-MM-ddTHH: mm: ssZ şeklindedir     |
|    ModifiedTime     |    Raporun son değiştirilme zamanı. Saat biçimi yyyy-MM-ddTHH: mm: ssZ şeklindedir     |
|    ExecuteNow     |    ExecuteNow bayrağı rapor oluşturulduğu sırada ayarlandı    |
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