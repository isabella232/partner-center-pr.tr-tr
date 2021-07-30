---
title: Özel sorgu belirtimi
description: Analiz tablolarından veri ayıklamak için özel sorgular oluşturma hakkında bilgi edinin.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 636d2eba7d259ae5e4525100b8d26e25ff031f48
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114839728"
---
# <a name="custom-query-specification"></a>Özel sorgu belirtimi

İş ortakları, analiz tablolarından veri ayıklamak üzere özel sorguları kolayca formüle etmek için bu sorgu belirtimlerini kullanabilir. Sorgular yalnızca belirli bir ölçütle eşan istenen sütunları ve ölçümleri seçmek için kullanılabilir. Dil belirtimlerinin merkezinde özel bir sorgunun yazıldığı veri kümesi tanımı yer amektedir.

## <a name="datasets"></a>Veri kümeleri

Bazı sorguların tablo ve sütun içeren bir veritabanında çalıştırıla aynı şekilde, sütunları ve ölçümleri olan Veri Kümeleri üzerinde de özel bir sorgu çalışır. Sorguyu formüle etmek için kullanılabilen veri kümelerinin tam listesi, veri kümeleri API'si kullanılarak elde edilir.

Bu, JSON olarak gösterilen bir veri kümesi örneğidir:

```json
{ 
      "datasetName": "OfficeUsage", 
      "selectableColumns": [ 
        "CustomerTenantId", 
        "CustomerTpid", 
        "WorkloadName", 
        "Month", 
        "PaidAvailableUnits", 
        "MonthlyActiveUsers", 
        "CustomerName", 
        "CustomerMarket", 
        "CustomerSegment",  
        "MPNId", 
        "PartnerName", 
        "PartnerLocation", 
        "PartnerAttributionType", 
        "IsDuplicateRowForPGA" 
      ], 
      "availableMetrics": [ 
        "CustomerCount", 
        "CustomerTenantCount", 
        "TotalPaidAvailableUnits", 
        "TotalMonthlyActiveUsers" 
      ], 
      "availableDateRanges": [ 
        "LAST_MONTH", 
        "LAST_3_MONTHS", 
        "LAST_6_MONTHS", 
        "LAST_1_YEAR", 
        "LIFETIME" 
      ], 
      "minimumRecurrenceInterval": 24 
    },
```

## <a name="parts-of-a-dataset"></a>Veri kümesi bölümleri

- Veri kümesi adı, veritabanı tablo adı gibi bir addır. Örneğin, OfficeUsage. Veri kümesi, CustomerTenantId gibi seçilecek sütunların listesini içerir.
- Bir veri kümesinde, veritabanındaki toplama işlevlerine benzer ölçümler de vardır. Örneğin, TotalMonthlyActiveUsers.
- Verilerin dışarı aktarılamayacak sabit zaman aralıkları vardır.

## <a name="formulating-a-query-on-a-dataset"></a>Veri kümesi üzerinde sorguyu formüle etmek

Bunlar, çeşitli veri türlerini ayıklamayı göstermek için bazı örnek sorgulardır.

|Sorgu|    Description    |
|----|    ----    |
|**SELECT** CustomerTenantId, PaidAvailableUnits **FROM** <br>OfficeUsage **TIMESPAN** LAST_MONTH|    Bu sorgu, son 1 ay içinde her CusotmerTenantID ve buna karşılık gelen PaidAvailableUnits'i alır.    |
|**SELECT** CustomerTenantId, PaidAvailableUnits **FROM** <br>OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10|    Bu sorgu, ücretli kullanılabilir birim sayısını azaltarak ilk 10 müşteri kiracısına sahip olur.     |
|**SELECT** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 ORDER BYMonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS  |    Bu sorgu, 100.000'den büyük AylıkActiveUsers'a sahip tüm Müşterilerin PaidAvailableUnits ve MonthlyActiveUsers'larını alır.     |
|**SELECT** CustomerTenantId, Month, MonthlyActiveUsers **FROM** <br>OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002') |    Bu sorgu CustomerTenantId ve her ay için aylık etkin kullanıcıları iki CustomerTpId değeriyle elde eder: '2a31c234-1f4e-4c60-909e-76d234f93161' ve '80780748-3f9a-11eb-b378-0242ac130002'.     |
|        |        |

## <a name="query-specification"></a>Sorgu belirtimi

Bu bölüm sorgu tanımını ve yapısını açıklar.

## <a name="grammar-reference"></a>Dil bilgisi başvurusu

Bu tablo, sorgularda kullanılan sembolleri açıklar.

|    Sorgu    |    Description    |
|    ----    |    ----    |
|    `?`    |    İsteğe Bağlı    |
|    `*`    |    Sıfır veya daha fazla    |
|    `+`    |    Bir veya daha fazla    |
|    `\|`    |    Veya / Listelerden biri    |
|        |        |

## <a name="query-definition"></a>Sorgu tanımı

Sorgu deyimi şu yan tümcelerine sahiptir: SelectClause, FromClause, WhereClause, OrderClause, LimitClause ve TimeSpan.

- **Öğesini seçin:**`SELECT ColumOrMetricName (, ColumOrMetricName)*`
    - **ColumOrMetricName:** Veri Kümesi içinde tanımlanan sütunlar ve ölçümler
- **FromClause:**`FROM DatasetName`
    - **DatasetName**: Veri Kümesi içinde tanımlanan veri kümesi adı
- **WhereClause:**`WHERE FilterCondition (AND FilterCondition)`
    - **FilterCondition:** ColumOrMetricName İşleci Değeri
        - **İşleci:**`=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`
        - **Değer:** Sayı | StringLiteral | MultiNumberList | MultiStringList
            - **Sayı:**`-? [0-9]+ (. [0-9] [0-9]*)?`
            - **StringLiteral:**`' [a-zA-Z0-9_]*'`
            - **MultiNumberList:**`(Number (,Number)*)`
            - **MultiStringList:**`(StringLiteral (,StringLiteral)*)`
- **OrderClause:**`ORDER BY OrderCondition (,OrderCondition)`
    - **OrderCondition:**`ColumOrMetricName (ASC | DESC)*`
- **LimitClause:**`LIMIT [0-9]+`
- **TimeSpan:**`TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`

## <a name="query-structure"></a>Sorgu Yapısı

Rapor sorgusu birden çok parçadan oluşur:
- `SELECT`
- `FROM`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `TIMESPAN`

Her bölüm aşağıda açıklanmıştır.

### `SELECT`

Sorgunun bu bölümü dışarı aktaracak sütunları belirtir. Seçilebilir sütunlar, bir veri kümesinde *selectableColumns* ve *availableMetrics* bölümlerinde listelenen alanlardır.

İsteğe bağlı olarak, `DISTINCT` anahtar sözcük sonra `SELECT` belirtilebilir. `DISTINCT`belirtilirse, dışarı aktaran son satırlar her zaman seçili sütunların ayrı değerlerini içerir. Ölçümler, seçilen sütunların her ayrı birleşimi için hesaplanır; bu nedenle, bir ölçüm sütunu seçili sütun listesine ekli olduğunda `DISTINCT` anahtar sözcük gerekli değildir.

**Örnek:**

```sql
SELECT CustomerTenantId, PaidAvailableUnits; 
SELECT DISTINCT CustomerTenantId
```

### `FROM`

Sorgunun bu bölümü, verilerin dışarı aktar yapılması gereken veri kümesine işaret etmek için kullanılır. Burada verilen veri kümesi adının, veri kümeleri API'si tarafından döndürülen geçerli bir veri kümesi adı olması gerekir.

**Örnek:**

- `FROM  OfficeUsage`
- `FROM  AzureUsage`

### `WHERE`

Sorgunun bu bölümü, veri kümesi üzerinde filtre koşullarını belirtmek için kullanılır. Yalnızca bu yan tümcesinde listelenen tüm koşullarla eşleşen satırlar dışarı aktarıldı son dosyasında yer atılır. Filtre koşulu *selectableColumns ve availableMetrics içinde listelenen sütunlardan* *herhangi biri üzerinde olabilir.* Filtre koşulunda belirtilen değerler, yalnızca işleç veya olduğunda sayı listesi veya dize listesi `IN` `NOT IN` olabilir. Değerler her zaman değişmez değer dizesi olarak verilmiştir ve yerel sütun türlerine dönüştürülür. And işlemiyle birden çok filtre koşullarının ayrılması gerekir.

**Örnek:**

- `CustomerTenantId= '868368da-957d-4959-8992-3c12dc7e6260'`
- `CustomerName LIKE '%Contoso%'`
- `CustomerId NOT IN (1000, 1001, 1002)`
- `OrderQuantity=100`
- `CustomerTenantId='7b487ac0-ce12-b732-dcd6-91a1e4e74a50' AND CustomerTpId=' 0f8b7fa0-eb83-a183-1225-ca153ef807aa'`

### `ORDER BY`

Sorgunun bu bölümü, dışarı aktaran satırlar için sıralama ölçütlerini belirtir. Sıralamanın tanımlandığı sütunların *selectableColumns* ve *availableMetrics veri kümesinden* olması gerekir. Belirtilen bir sıralama yönü yoksa, sütunda varsayılan olarak DESC kullanılır. Sıralama, ölçütleri virgülle ayırarak birden çok sütunda tanımlanabilir.

**Örnek:**

- `ORDER BY  MonthlyActiveUsers ASC,  Month DESC`
- `ORDER BY CustomerName ASC,  Month`

### `LIMIT`

Sorgunun bu bölümü, dışarı aktaracak satır sayısını belirtir. Belirttiğiniz sayanın sıfır olmayan pozitif bir tamsayı olması gerekir.

### `TIMESPAN`

Sorgunun bu bölümü, verilerin dışarı aktarnma süresini belirtir. Olası değerler, veri kümesi *tanımında availableDateRanges* alanından olması gerekir.

### <a name="case-sensitivity-in-query-specification"></a>Sorgu belirtimsinde büyük/küçük harf duyarlılığı

Belirtim büyük/büyük/büyük harfe duyarlı değildir. Önceden tanımlanmış anahtar sözcükler, sütun adları ve değerler büyük veya küçük harf kullanılarak belirtilebilir.

## <a name="next-steps"></a>Sonraki adımlar

- [Sistem sorgularının listesi](insights-programmatic-system-queries.md)
- [Örnek sorguların listesi](insights-programmatic-sample-queries.md)