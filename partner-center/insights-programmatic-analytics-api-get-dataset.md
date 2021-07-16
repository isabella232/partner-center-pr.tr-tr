---
title: tüm veri kümelerini al API-Analizler verileri
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Iş Ortağı Merkezi öngörülerine tüm kullanılabilir veri kümelerinin ayrıntılarını almak için bu API 'yi kullanın.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 42ff7cc1f097e2423be5f1f7f9a7f62214d64949
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376960"
---
# <a name="get-all-datasets-api"></a>Tüm veri kümeleri API 'sini al

Tüm veri kümelerini al API 'SI kullanılabilir tüm veri kümelerini alır. Veri kümeleri tabloları, sütunları, ölçümleri ve zaman aralıklarını listeler.

**İstek sözdizimi**

|    Yöntem    |    İstek URI'si    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset?datasetName={Dataset Name}`     |
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
|    datasetName    |    dize    |    No    |    Yalnızca bir veri kümesinin ayrıntılarını almak için filtrele    |
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
   "Value":[ 
      { 
         "DatasetName ":"string", 
         "SelectableColumns":[ 
            "string" 
         ], 
         "AvailableMetrics":[ 
            "string" 
         ], 
         "AvailableDateRanges":[ 
            "string" 
         ], 
         "minimumRecurrenceInterval":0 
      } 
   ], 
   "TotalCount":0, 
   "Message":"<Error Message>", 
   "StatusCode": 0, 
} 
```

**Sözlük**

Bu tablo, yanıttaki anahtar öğeleri tanımlar:

|    Parametre    |    Açıklama    |
|    ----    |    ----    |
|    DatasetName     |    Bu dizi nesnesinin tanımladığı veri kümesinin adı     |
|    SelectableColumns     |    Seçme sütunlarında belirtilenebilir ham sütunlar     |
|    Kullanılabilirlik Blemetrics     |    Seçme sütunlarında belirtilenebilir toplama/ölçüm sütun adları     |
|    Availableduteranges     |    Veri kümesi için rapor sorgularında kullanılabilecek tarih aralığı     |
|    Minimumrecurrenceınterval     |    Yinelenme aralığının en düşük değeri     |
|    TotalCount     |    Değer dizisindeki veri kümesi sayısı     |
|    İleti     |    API 'nin yürütülmesindeki durum iletisi     |
|    Durum     |    Sonuç kodu. Olası değerler 200, 400, 401, 403, 500     |
|        |        |
