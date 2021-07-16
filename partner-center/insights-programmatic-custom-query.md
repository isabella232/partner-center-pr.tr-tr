---
title: Özel sorgu belirtimi
description: Analiz tablolarından veri ayıklamak için özel sorgular oluşturmayı öğrenin.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 57f2109044e604dca21b0109b5be56f40170628e
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377405"
---
# <a name="custom-query-specification"></a>Özel sorgu belirtimi

İş ortakları bu sorgu belirtimini, analiz tablolarından veri ayıklama için özel sorguları kolayca formülleştirmek için kullanabilir. Sorgular yalnızca istenen sütunları ve belirli bir ölçütle eşleşen ölçümleri seçmek için kullanılabilir. Dil belirtiminin kalmasıyla, özel bir sorgunun yazılabileceği veri kümesi tanımıdır.

## <a name="datasets"></a>Veri kümeleri

Tablo ve sütun içeren bir veritabanında bazı sorguların çalıştırıldığı şekilde, özel bir sorgu sütunları ve ölçümleri olan veri kümelerinde çalışır. Sorgu oluşturmak için kullanılabilir veri kümelerinin tam listesi, veri kümeleri API 'SI kullanılarak elde edilebilir.

Bu bir JSON olarak gösterilen veri kümesi örneğidir:

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

## <a name="parts-of-a-dataset"></a>Veri kümesinin parçaları

- Veri kümesi adı, veritabanı tablosu adı gibidir. Örneğin, Officekullanımı. Bir veri kümesinde, Customertenantıd gibi seçilebilirler bir sütun listesi bulunur.
- Bir veri kümesinde ayrıca bir veritabanında toplama işlevleri gibi ölçümler de vardır. Örneğin, TotalMonthlyActiveUsers.
- Verilerin verilebileceği sabit zaman yaymalar vardır.

## <a name="formulating-a-query-on-a-dataset"></a>Bir veri kümesindeki sorguyu formülleyici

Bunlar çeşitli veri türlerinin nasıl ayıklanacağını gösteren bazı örnek sorgulardır.

|Sorgu|    Açıklama    |
|----|    ----    |
|**Seç** Customertenantıd, Paidadvailableunits  <br>Officekullanım zaman **aralığı** LAST_MONTH|    Bu sorgu, son 1 ayda her Cusotmertenantıd ve karşılık gelen Paidavvailableunits 'ı alır.    |
|**Seç** Customertenantıd, Paidadvailableunits  <br>Paidadvailableunits tarafından Officekullanım **sırası** **sınırı** 10|    Bu sorgu, ilk 10 müşteri kiracıyı, ücretli kullanılabilir birim sayısı azalan sırada alacak.     |
|**Seç** Customertenantıd, Paidadvailableunits, monthlyactiveusers **kullanıcıları** ,  Monthlyactiveusers kullanıcı zaman aralığı **tarafından 100000 sıra** > LAST_6_MONTHS  |    Bu sorgu, MonthlyActiveUsers 'ın 100.000 'den büyük olduğu tüm müşterilerin Paidadvailableunits ve MonthlyActiveUsers 'ı alır.     |
|**Seç** Customertenantıd, month, MonthlyActiveUsers  <br>' 2a31c234-1f4e-4c60-909e-76d234f93161 ', ' 80780748-3f9a-11eb-b378-0242ac130002 ' IÇINDE customertpıd 'nin **bulunduğu** officeusage |    Bu sorgu, her ay için Customertenantıd ve aylık etkin kullanıcıları iki Customertpıd değeriyle alacak: ' 2a31c234-1f4e-4c60-909e-76d234f93161 ' ve ' 80780748-3f9a-11eb-b378-0242ac130002 '.     |
|        |        |

## <a name="query-specification"></a>Sorgu belirtimi

Bu bölümde sorgu tanımı ve yapısı açıklanmaktadır.

## <a name="grammar-reference"></a>Dilbilgisi başvurusu

Bu tablo sorgularda kullanılan sembolleri açıklar.

|    Sorgu    |    Açıklama    |
|    ----    |    ----    |
|    `?`    |    İsteğe Bağlı    |
|    `*`    |    Sıfır veya daha fazla    |
|    `+`    |    Bir veya daha fazla    |
|    `\|`    |    Veya listelerden biri    |
|        |        |

## <a name="query-definition"></a>Sorgu tanımı

Sorgu deyimi şu yan tümceleri içerir: SelectClause, FromClause, WhereClause, OrderClause, LimitClause ve TimeSpan.

- **Selectclause**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`
    - **ColumOrMetricName**: veri kümesi içinde tanımlanan sütunlar ve ölçümler
- **FromClause**: `FROM DatasetName`
    - **DataSetName**: veri kümesi içinde tanımlanan veri kümesi adı
- **WhereClause**: `WHERE FilterCondition (AND FilterCondition)`
    - **FilterCondition**: ColumOrMetricName işleç değeri
        - **İşleç**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`
        - **Değer**: sayı | StringLiteral | MultiNumberList | MultiStringList
            - **Sayı**: `-? [0-9]+ (. [0-9] [0-9]*)?`
            - **Stringliteral**:  `' [a-zA-Z0-9_]*'`
            - **MultiNumberList**: `(Number (,Number)*)`
            - **Multistringlist**: `(StringLiteral (,StringLiteral)*)`
- **Orderclause**: `ORDER BY OrderCondition (,OrderCondition)`
    - **Ordercondition**: `ColumOrMetricName (ASC | DESC)*`
- **Limitclause**: `LIMIT [0-9]+`
- **TimeSpan**: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`

## <a name="query-structure"></a>Sorgu yapısı

Rapor sorgusu birden çok bölümden oluşur:
- `SELECT`
- `FROM`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `TIMESPAN`

Her bölüm aşağıda açıklanmıştır.

### `SELECT`

Sorgunun bu bölümü, verilecek sütunları belirtir. Seçilebilir sütunlar, bir veri kümesinin *Selectablecolumns* ve *kullanılabilirlik* bölümlerinde listelenen alanlardır.

İsteğe bağlı olarak, `DISTINCT` anahtar sözcük daha sonra belirtilebilir `SELECT` . `DISTINCT`Belirtilmişse, son içe aktarılmış satırlar her zaman Seçili sütunların ayrı değerlerini içerecektir. Ölçümler Seçili sütunların her farklı birleşimi için hesaplanacak, bu nedenle `DISTINCT` sütun Seç listesine bir ölçüm sütunu dahil edildiğinde anahtar sözcüğü gerekli değildir.

**Örnek:**

```sql
SELECT CustomerTenantId, PaidAvailableUnits; 
SELECT DISTINCT CustomerTenantId
```

### `FROM`

Sorgunun bu bölümü, verilerin verilmesi gereken veri kümesini gösterir. Burada verilen veri kümesi adının, veri kümeleri API 'SI tarafından döndürülen geçerli bir veri kümesi adı olması gerekir.

**Örnek:**

- `FROM  OfficeUsage`
- `FROM  AzureUsage`

### `WHERE`

Sorgunun bu bölümü, veri kümesindeki Filtre koşullarını belirtmek için kullanılır. Yalnızca bu yan tümce içinde listelenen tüm koşullara uyan satırlar, son verilen dosyada mevcut olacaktır. Filtre koşulu *Selectablecolumns* ve *kullanılabilirliği Blemetrics*' da listelenen sütunlardan herhangi birinde olabilir. Filtre koşulunda belirtilen değerler, yalnızca işleci veya olduğunda bir dize listesi veya dizeler listesi olabilir `IN` `NOT IN` . Değerler her zaman sabit bir dize olarak verilebilir ve bunlar yerel sütun türlerine dönüştürülecektir. Birden çok filtre koşullarının bir ve işlemiyle ayrılması gerekir.

**Örnek:**

- `CustomerTenantId= '868368da-957d-4959-8992-3c12dc7e6260'`
- `CustomerName LIKE '%Contoso%'`
- `CustomerId NOT IN (1000, 1001, 1002)`
- `OrderQuantity=100`
- `CustomerTenantId='7b487ac0-ce12-b732-dcd6-91a1e4e74a50' AND CustomerTpId=' 0f8b7fa0-eb83-a183-1225-ca153ef807aa'`

### `ORDER BY`

Sorgunun bu kısmı, aktarılmış satırlar için sıralama ölçütlerini belirtir. Sıralamanın tanımlanbileceği sütunların, veri kümesinin *Selectablecolumns* ve *kullanılabilirlik Blemetrics* öğesinden olması gerekir. Sıralama yönü belirtilmemişse, sütunda varsayılan değer DESC olarak ayarlanır. Sıralama, ölçütü virgülle ayırarak birden çok sütunda tanımlanabilir.

**Örnek:**

- `ORDER BY  MonthlyActiveUsers ASC,  Month DESC`
- `ORDER BY CustomerName ASC,  Month`

### `LIMIT`

Sorgunun bu bölümü, verilecek satır sayısını belirtir. Belirttiğiniz sayının pozitif sıfır dışında bir tamsayı olması gerekir.

### `TIMESPAN`

Sorgunun bu bölümü, verilerin verilmesi gereken süreyi belirtir. Olası değerler veri kümesi tanımındaki *Availabledateranges* alanından olmalıdır.

### <a name="case-sensitivity-in-query-specification"></a>Sorgu belirtiminde büyük/küçük harf duyarlılığı

Belirtim tamamen büyük/küçük harfe duyarlıdır. Önceden tanımlanmış anahtar sözcükler, sütun adları ve değerler büyük veya küçük harf kullanılarak belirtilebilir.

## <a name="next-steps"></a>Sonraki adımlar

- [Sistem sorgularının listesi](insights-programmatic-system-queries.md)
- [Örnek sorgu listesi](insights-programmatic-sample-queries.md)