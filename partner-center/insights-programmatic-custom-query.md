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
# <a name="custom-query-specification"></a><span data-ttu-id="aaabb-103">Özel sorgu belirtimi</span><span class="sxs-lookup"><span data-stu-id="aaabb-103">Custom query specification</span></span>

<span data-ttu-id="aaabb-104">İş ortakları bu sorgu belirtimini, analiz tablolarından veri ayıklama için özel sorguları kolayca formülleştirmek için kullanabilir.</span><span class="sxs-lookup"><span data-stu-id="aaabb-104">Partners can use this query specification to easily formulate custom queries for extracting data from analytics tables.</span></span> <span data-ttu-id="aaabb-105">Sorgular yalnızca istenen sütunları ve belirli bir ölçütle eşleşen ölçümleri seçmek için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="aaabb-105">The queries can be used to select only the desired columns and metrics that match a certain criterion.</span></span> <span data-ttu-id="aaabb-106">Dil belirtiminin kalmasıyla, özel bir sorgunun yazılabileceği veri kümesi tanımıdır.</span><span class="sxs-lookup"><span data-stu-id="aaabb-106">At the heart of the language specification is the dataset definition on which a custom query can be written.</span></span>

## <a name="datasets"></a><span data-ttu-id="aaabb-107">Veri kümeleri</span><span class="sxs-lookup"><span data-stu-id="aaabb-107">Datasets</span></span>

<span data-ttu-id="aaabb-108">Tablo ve sütun içeren bir veritabanında bazı sorguların çalıştırıldığı şekilde, özel bir sorgu sütunları ve ölçümleri olan veri kümelerinde çalışır.</span><span class="sxs-lookup"><span data-stu-id="aaabb-108">In the same way that some queries are run against a database that has tables and columns, a custom query works on Datasets that have columns and metrics.</span></span> <span data-ttu-id="aaabb-109">Sorgu oluşturmak için kullanılabilir veri kümelerinin tam listesi, veri kümeleri API 'SI kullanılarak elde edilebilir.</span><span class="sxs-lookup"><span data-stu-id="aaabb-109">The full list of available datasets for formulating a query can be obtained by using the datasets API.</span></span>

<span data-ttu-id="aaabb-110">Bu bir JSON olarak gösterilen veri kümesi örneğidir:</span><span class="sxs-lookup"><span data-stu-id="aaabb-110">This is an example of a dataset shown as a JSON:</span></span>

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

## <a name="parts-of-a-dataset"></a><span data-ttu-id="aaabb-111">Veri kümesinin parçaları</span><span class="sxs-lookup"><span data-stu-id="aaabb-111">Parts of a dataset</span></span>

- <span data-ttu-id="aaabb-112">Veri kümesi adı, veritabanı tablosu adı gibidir.</span><span class="sxs-lookup"><span data-stu-id="aaabb-112">A dataset name is like a database table name.</span></span> <span data-ttu-id="aaabb-113">Örneğin, Officekullanımı.</span><span class="sxs-lookup"><span data-stu-id="aaabb-113">For example, OfficeUsage.</span></span> <span data-ttu-id="aaabb-114">Bir veri kümesinde, Customertenantıd gibi seçilebilirler bir sütun listesi bulunur.</span><span class="sxs-lookup"><span data-stu-id="aaabb-114">A dataset has a list of columns that can be selected, such as CustomerTenantId.</span></span>
- <span data-ttu-id="aaabb-115">Bir veri kümesinde ayrıca bir veritabanında toplama işlevleri gibi ölçümler de vardır.</span><span class="sxs-lookup"><span data-stu-id="aaabb-115">A dataset also has metrics, which are like aggregation functions in a database.</span></span> <span data-ttu-id="aaabb-116">Örneğin, TotalMonthlyActiveUsers.</span><span class="sxs-lookup"><span data-stu-id="aaabb-116">For example, TotalMonthlyActiveUsers.</span></span>
- <span data-ttu-id="aaabb-117">Verilerin verilebileceği sabit zaman yaymalar vardır.</span><span class="sxs-lookup"><span data-stu-id="aaabb-117">There are fixed time spans over which data can be exported.</span></span>

## <a name="formulating-a-query-on-a-dataset"></a><span data-ttu-id="aaabb-118">Bir veri kümesindeki sorguyu formülleyici</span><span class="sxs-lookup"><span data-stu-id="aaabb-118">Formulating a query on a dataset</span></span>

<span data-ttu-id="aaabb-119">Bunlar çeşitli veri türlerinin nasıl ayıklanacağını gösteren bazı örnek sorgulardır.</span><span class="sxs-lookup"><span data-stu-id="aaabb-119">These are some sample queries that show how to extract various types of data.</span></span>

|<span data-ttu-id="aaabb-120">Sorgu</span><span class="sxs-lookup"><span data-stu-id="aaabb-120">Query</span></span>|    <span data-ttu-id="aaabb-121">Açıklama</span><span class="sxs-lookup"><span data-stu-id="aaabb-121">Description</span></span>    |
|----|    ----    |
|<span data-ttu-id="aaabb-122">**Seç** Customertenantıd, Paidadvailableunits </span><span class="sxs-lookup"><span data-stu-id="aaabb-122">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span></span> <br><span data-ttu-id="aaabb-123">Officekullanım zaman **aralığı** LAST_MONTH</span><span class="sxs-lookup"><span data-stu-id="aaabb-123">OfficeUsage **TIMESPAN** LAST_MONTH</span></span>|    <span data-ttu-id="aaabb-124">Bu sorgu, son 1 ayda her Cusotmertenantıd ve karşılık gelen Paidavvailableunits 'ı alır.</span><span class="sxs-lookup"><span data-stu-id="aaabb-124">This query will get every CusotmerTenantID and its corresponding PaidAvailableUnits in the last 1 month.</span></span>    |
|<span data-ttu-id="aaabb-125">**Seç** Customertenantıd, Paidadvailableunits </span><span class="sxs-lookup"><span data-stu-id="aaabb-125">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span></span> <br><span data-ttu-id="aaabb-126">Paidadvailableunits tarafından Officekullanım **sırası** **sınırı** 10</span><span class="sxs-lookup"><span data-stu-id="aaabb-126">OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10</span></span>|    <span data-ttu-id="aaabb-127">Bu sorgu, ilk 10 müşteri kiracıyı, ücretli kullanılabilir birim sayısı azalan sırada alacak.</span><span class="sxs-lookup"><span data-stu-id="aaabb-127">This query will get the top 10 customer tenants in decreasing order of the number of paid available units.</span></span>     |
|<span data-ttu-id="aaabb-128">**Seç** Customertenantıd, Paidadvailableunits, monthlyactiveusers **kullanıcıları** ,  Monthlyactiveusers kullanıcı zaman aralığı **tarafından 100000 sıra** > LAST_6_MONTHS </span><span class="sxs-lookup"><span data-stu-id="aaabb-128">**SELECT** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS</span></span> |    <span data-ttu-id="aaabb-129">Bu sorgu, MonthlyActiveUsers 'ın 100.000 'den büyük olduğu tüm müşterilerin Paidadvailableunits ve MonthlyActiveUsers 'ı alır.</span><span class="sxs-lookup"><span data-stu-id="aaabb-129">This query will get the PaidAvailableUnits and MonthlyActiveUsers of all the Customers who have MonthlyActiveUsers greater than 100,000.</span></span>     |
|<span data-ttu-id="aaabb-130">**Seç** Customertenantıd, month, MonthlyActiveUsers </span><span class="sxs-lookup"><span data-stu-id="aaabb-130">**SELECT** CustomerTenantId, Month, MonthlyActiveUsers **FROM**</span></span> <br><span data-ttu-id="aaabb-131">' 2a31c234-1f4e-4c60-909e-76d234f93161 ', ' 80780748-3f9a-11eb-b378-0242ac130002 ' IÇINDE customertpıd 'nin **bulunduğu** officeusage</span><span class="sxs-lookup"><span data-stu-id="aaabb-131">OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002')</span></span> |    <span data-ttu-id="aaabb-132">Bu sorgu, her ay için Customertenantıd ve aylık etkin kullanıcıları iki Customertpıd değeriyle alacak: ' 2a31c234-1f4e-4c60-909e-76d234f93161 ' ve ' 80780748-3f9a-11eb-b378-0242ac130002 '.</span><span class="sxs-lookup"><span data-stu-id="aaabb-132">This query will get the CustomerTenantId and the monthly active users for every month by the two CustomerTpId values: '2a31c234-1f4e-4c60-909e-76d234f93161' and '80780748-3f9a-11eb-b378-0242ac130002'.</span></span>     |
|        |        |

## <a name="query-specification"></a><span data-ttu-id="aaabb-133">Sorgu belirtimi</span><span class="sxs-lookup"><span data-stu-id="aaabb-133">Query specification</span></span>

<span data-ttu-id="aaabb-134">Bu bölümde sorgu tanımı ve yapısı açıklanmaktadır.</span><span class="sxs-lookup"><span data-stu-id="aaabb-134">This section describes the query definition and structure.</span></span>

## <a name="grammar-reference"></a><span data-ttu-id="aaabb-135">Dilbilgisi başvurusu</span><span class="sxs-lookup"><span data-stu-id="aaabb-135">Grammar reference</span></span>

<span data-ttu-id="aaabb-136">Bu tablo sorgularda kullanılan sembolleri açıklar.</span><span class="sxs-lookup"><span data-stu-id="aaabb-136">This table describes the symbols used in queries.</span></span>

|    <span data-ttu-id="aaabb-137">Sorgu</span><span class="sxs-lookup"><span data-stu-id="aaabb-137">Query</span></span>    |    <span data-ttu-id="aaabb-138">Açıklama</span><span class="sxs-lookup"><span data-stu-id="aaabb-138">Description</span></span>    |
|    ----    |    ----    |
|    `?`    |    <span data-ttu-id="aaabb-139">İsteğe Bağlı</span><span class="sxs-lookup"><span data-stu-id="aaabb-139">Optional</span></span>    |
|    `*`    |    <span data-ttu-id="aaabb-140">Sıfır veya daha fazla</span><span class="sxs-lookup"><span data-stu-id="aaabb-140">Zero or more</span></span>    |
|    `+`    |    <span data-ttu-id="aaabb-141">Bir veya daha fazla</span><span class="sxs-lookup"><span data-stu-id="aaabb-141">One or more</span></span>    |
|    `\|`    |    <span data-ttu-id="aaabb-142">Veya listelerden biri</span><span class="sxs-lookup"><span data-stu-id="aaabb-142">Or / One of the lists</span></span>    |
|        |        |

## <a name="query-definition"></a><span data-ttu-id="aaabb-143">Sorgu tanımı</span><span class="sxs-lookup"><span data-stu-id="aaabb-143">Query definition</span></span>

<span data-ttu-id="aaabb-144">Sorgu deyimi şu yan tümceleri içerir: SelectClause, FromClause, WhereClause, OrderClause, LimitClause ve TimeSpan.</span><span class="sxs-lookup"><span data-stu-id="aaabb-144">The query statement has the following clauses: SelectClause, FromClause, WhereClause, OrderClause, LimitClause, and TimeSpan.</span></span>

- <span data-ttu-id="aaabb-145">**Selectclause**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`</span><span class="sxs-lookup"><span data-stu-id="aaabb-145">**SelectClause**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`</span></span>
    - <span data-ttu-id="aaabb-146">**ColumOrMetricName**: veri kümesi içinde tanımlanan sütunlar ve ölçümler</span><span class="sxs-lookup"><span data-stu-id="aaabb-146">**ColumOrMetricName**: Columns and Metrics defined within the Dataset</span></span>
- <span data-ttu-id="aaabb-147">**FromClause**: `FROM DatasetName`</span><span class="sxs-lookup"><span data-stu-id="aaabb-147">**FromClause**: `FROM DatasetName`</span></span>
    - <span data-ttu-id="aaabb-148">**DataSetName**: veri kümesi içinde tanımlanan veri kümesi adı</span><span class="sxs-lookup"><span data-stu-id="aaabb-148">**DatasetName**: Dataset name defined within the Dataset</span></span>
- <span data-ttu-id="aaabb-149">**WhereClause**: `WHERE FilterCondition (AND FilterCondition)`</span><span class="sxs-lookup"><span data-stu-id="aaabb-149">**WhereClause**: `WHERE FilterCondition (AND FilterCondition)`</span></span>
    - <span data-ttu-id="aaabb-150">**FilterCondition**: ColumOrMetricName işleç değeri</span><span class="sxs-lookup"><span data-stu-id="aaabb-150">**FilterCondition**: ColumOrMetricName Operator Value</span></span>
        - <span data-ttu-id="aaabb-151">**İşleç**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`</span><span class="sxs-lookup"><span data-stu-id="aaabb-151">**Operator**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`</span></span>
        - <span data-ttu-id="aaabb-152">**Değer**: sayı | StringLiteral | MultiNumberList | MultiStringList</span><span class="sxs-lookup"><span data-stu-id="aaabb-152">**Value**: Number | StringLiteral | MultiNumberList | MultiStringList</span></span>
            - <span data-ttu-id="aaabb-153">**Sayı**: `-? [0-9]+ (. [0-9] [0-9]*)?`</span><span class="sxs-lookup"><span data-stu-id="aaabb-153">**Number**: `-? [0-9]+ (. [0-9] [0-9]*)?`</span></span>
            - <span data-ttu-id="aaabb-154">**Stringliteral**:  `' [a-zA-Z0-9_]*'`</span><span class="sxs-lookup"><span data-stu-id="aaabb-154">**StringLiteral**:  `' [a-zA-Z0-9_]*'`</span></span>
            - <span data-ttu-id="aaabb-155">**MultiNumberList**: `(Number (,Number)*)`</span><span class="sxs-lookup"><span data-stu-id="aaabb-155">**MultiNumberList**: `(Number (,Number)*)`</span></span>
            - <span data-ttu-id="aaabb-156">**Multistringlist**: `(StringLiteral (,StringLiteral)*)`</span><span class="sxs-lookup"><span data-stu-id="aaabb-156">**MultiStringList**: `(StringLiteral (,StringLiteral)*)`</span></span>
- <span data-ttu-id="aaabb-157">**Orderclause**: `ORDER BY OrderCondition (,OrderCondition)`</span><span class="sxs-lookup"><span data-stu-id="aaabb-157">**OrderClause**: `ORDER BY OrderCondition (,OrderCondition)`</span></span>
    - <span data-ttu-id="aaabb-158">**Ordercondition**: `ColumOrMetricName (ASC | DESC)*`</span><span class="sxs-lookup"><span data-stu-id="aaabb-158">**OrderCondition**: `ColumOrMetricName (ASC | DESC)*`</span></span>
- <span data-ttu-id="aaabb-159">**Limitclause**: `LIMIT [0-9]+`</span><span class="sxs-lookup"><span data-stu-id="aaabb-159">**LimitClause**: `LIMIT [0-9]+`</span></span>
- <span data-ttu-id="aaabb-160">**TimeSpan**: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`</span><span class="sxs-lookup"><span data-stu-id="aaabb-160">**TimeSpan**: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`</span></span>

## <a name="query-structure"></a><span data-ttu-id="aaabb-161">Sorgu yapısı</span><span class="sxs-lookup"><span data-stu-id="aaabb-161">Query Structure</span></span>

<span data-ttu-id="aaabb-162">Rapor sorgusu birden çok bölümden oluşur:</span><span class="sxs-lookup"><span data-stu-id="aaabb-162">A Report query is made up of multiple parts:</span></span>
- `SELECT`
- `FROM`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `TIMESPAN`

<span data-ttu-id="aaabb-163">Her bölüm aşağıda açıklanmıştır.</span><span class="sxs-lookup"><span data-stu-id="aaabb-163">Each part is described below.</span></span>

### `SELECT`

<span data-ttu-id="aaabb-164">Sorgunun bu bölümü, verilecek sütunları belirtir.</span><span class="sxs-lookup"><span data-stu-id="aaabb-164">This part of the query specifies the columns that will get exported.</span></span> <span data-ttu-id="aaabb-165">Seçilebilir sütunlar, bir veri kümesinin *Selectablecolumns* ve *kullanılabilirlik* bölümlerinde listelenen alanlardır.</span><span class="sxs-lookup"><span data-stu-id="aaabb-165">The columns that can be selected are the fields listed in *selectableColumns* and *availableMetrics* sections of a dataset.</span></span>

<span data-ttu-id="aaabb-166">İsteğe bağlı olarak, `DISTINCT` anahtar sözcük daha sonra belirtilebilir `SELECT` .</span><span class="sxs-lookup"><span data-stu-id="aaabb-166">Optionally, `DISTINCT` keyword can be specified after `SELECT`.</span></span> <span data-ttu-id="aaabb-167">`DISTINCT`Belirtilmişse, son içe aktarılmış satırlar her zaman Seçili sütunların ayrı değerlerini içerecektir.</span><span class="sxs-lookup"><span data-stu-id="aaabb-167">If `DISTINCT` is specified, then the final exported rows will always contain distinct values of the selected columns.</span></span> <span data-ttu-id="aaabb-168">Ölçümler Seçili sütunların her farklı birleşimi için hesaplanacak, bu nedenle `DISTINCT` sütun Seç listesine bir ölçüm sütunu dahil edildiğinde anahtar sözcüğü gerekli değildir.</span><span class="sxs-lookup"><span data-stu-id="aaabb-168">Metrics will be calculated for every distinct combination of the selected columns, hence `DISTINCT` keyword is not required when a metric column is included in the select column list.</span></span>

<span data-ttu-id="aaabb-169">**Örnek:**</span><span class="sxs-lookup"><span data-stu-id="aaabb-169">**Example:**</span></span>

```sql
SELECT CustomerTenantId, PaidAvailableUnits; 
SELECT DISTINCT CustomerTenantId
```

### `FROM`

<span data-ttu-id="aaabb-170">Sorgunun bu bölümü, verilerin verilmesi gereken veri kümesini gösterir.</span><span class="sxs-lookup"><span data-stu-id="aaabb-170">This part of the query indicates the dataset from which data needs to be exported.</span></span> <span data-ttu-id="aaabb-171">Burada verilen veri kümesi adının, veri kümeleri API 'SI tarafından döndürülen geçerli bir veri kümesi adı olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="aaabb-171">The dataset name given here needs to be a valid dataset name returned by the datasets API.</span></span>

<span data-ttu-id="aaabb-172">**Örnek:**</span><span class="sxs-lookup"><span data-stu-id="aaabb-172">**Example:**</span></span>

- `FROM  OfficeUsage`
- `FROM  AzureUsage`

### `WHERE`

<span data-ttu-id="aaabb-173">Sorgunun bu bölümü, veri kümesindeki Filtre koşullarını belirtmek için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="aaabb-173">This part of the query is used to specify filter conditions on the dataset.</span></span> <span data-ttu-id="aaabb-174">Yalnızca bu yan tümce içinde listelenen tüm koşullara uyan satırlar, son verilen dosyada mevcut olacaktır.</span><span class="sxs-lookup"><span data-stu-id="aaabb-174">Only rows matching all the conditions listed in this clause will be present in the final exported file.</span></span> <span data-ttu-id="aaabb-175">Filtre koşulu *Selectablecolumns* ve *kullanılabilirliği Blemetrics*' da listelenen sütunlardan herhangi birinde olabilir.</span><span class="sxs-lookup"><span data-stu-id="aaabb-175">The filter condition can be on any of the columns listed in *selectableColumns* and *availableMetrics*.</span></span> <span data-ttu-id="aaabb-176">Filtre koşulunda belirtilen değerler, yalnızca işleci veya olduğunda bir dize listesi veya dizeler listesi olabilir `IN` `NOT IN` .</span><span class="sxs-lookup"><span data-stu-id="aaabb-176">The values specified in the filter condition can be a list of numbers or a list of strings only when the operator is `IN` or `NOT IN`.</span></span> <span data-ttu-id="aaabb-177">Değerler her zaman sabit bir dize olarak verilebilir ve bunlar yerel sütun türlerine dönüştürülecektir.</span><span class="sxs-lookup"><span data-stu-id="aaabb-177">The values can always be given as a literal string and they will be converted to the native types of columns.</span></span> <span data-ttu-id="aaabb-178">Birden çok filtre koşullarının bir ve işlemiyle ayrılması gerekir.</span><span class="sxs-lookup"><span data-stu-id="aaabb-178">Multiple filter conditions need to be separated with an AND operation.</span></span>

<span data-ttu-id="aaabb-179">**Örnek:**</span><span class="sxs-lookup"><span data-stu-id="aaabb-179">**Example:**</span></span>

- `CustomerTenantId= '868368da-957d-4959-8992-3c12dc7e6260'`
- `CustomerName LIKE '%Contoso%'`
- `CustomerId NOT IN (1000, 1001, 1002)`
- `OrderQuantity=100`
- `CustomerTenantId='7b487ac0-ce12-b732-dcd6-91a1e4e74a50' AND CustomerTpId=' 0f8b7fa0-eb83-a183-1225-ca153ef807aa'`

### `ORDER BY`

<span data-ttu-id="aaabb-180">Sorgunun bu kısmı, aktarılmış satırlar için sıralama ölçütlerini belirtir.</span><span class="sxs-lookup"><span data-stu-id="aaabb-180">This part of the query specifies the ordering criteria for the exported rows.</span></span> <span data-ttu-id="aaabb-181">Sıralamanın tanımlanbileceği sütunların, veri kümesinin *Selectablecolumns* ve *kullanılabilirlik Blemetrics* öğesinden olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="aaabb-181">The columns on which ordering can be defined need to be from the *selectableColumns* and *availableMetrics* of the dataset.</span></span> <span data-ttu-id="aaabb-182">Sıralama yönü belirtilmemişse, sütunda varsayılan değer DESC olarak ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="aaabb-182">If there is no ordering direction specified, it will be defaulted to DESC on the column.</span></span> <span data-ttu-id="aaabb-183">Sıralama, ölçütü virgülle ayırarak birden çok sütunda tanımlanabilir.</span><span class="sxs-lookup"><span data-stu-id="aaabb-183">Ordering can be defined on multiple columns by separating the criteria with a comma.</span></span>

<span data-ttu-id="aaabb-184">**Örnek:**</span><span class="sxs-lookup"><span data-stu-id="aaabb-184">**Example:**</span></span>

- `ORDER BY  MonthlyActiveUsers ASC,  Month DESC`
- `ORDER BY CustomerName ASC,  Month`

### `LIMIT`

<span data-ttu-id="aaabb-185">Sorgunun bu bölümü, verilecek satır sayısını belirtir.</span><span class="sxs-lookup"><span data-stu-id="aaabb-185">This part of the query specifies the number of rows that will be exported.</span></span> <span data-ttu-id="aaabb-186">Belirttiğiniz sayının pozitif sıfır dışında bir tamsayı olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="aaabb-186">The number you specify needs to be a positive nonzero integer.</span></span>

### `TIMESPAN`

<span data-ttu-id="aaabb-187">Sorgunun bu bölümü, verilerin verilmesi gereken süreyi belirtir.</span><span class="sxs-lookup"><span data-stu-id="aaabb-187">This part of the query specifies the time duration for which the data needs to be exported.</span></span> <span data-ttu-id="aaabb-188">Olası değerler veri kümesi tanımındaki *Availabledateranges* alanından olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="aaabb-188">The possible values should be from the *availableDateRanges* field in the dataset definition.</span></span>

### <a name="case-sensitivity-in-query-specification"></a><span data-ttu-id="aaabb-189">Sorgu belirtiminde büyük/küçük harf duyarlılığı</span><span class="sxs-lookup"><span data-stu-id="aaabb-189">Case sensitivity in query specification</span></span>

<span data-ttu-id="aaabb-190">Belirtim tamamen büyük/küçük harfe duyarlıdır.</span><span class="sxs-lookup"><span data-stu-id="aaabb-190">The specification is completely case insensitive.</span></span> <span data-ttu-id="aaabb-191">Önceden tanımlanmış anahtar sözcükler, sütun adları ve değerler büyük veya küçük harf kullanılarak belirtilebilir.</span><span class="sxs-lookup"><span data-stu-id="aaabb-191">Predefined keywords, column names and values can be specified using upper or lower case.</span></span>

## <a name="next-steps"></a><span data-ttu-id="aaabb-192">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="aaabb-192">Next steps</span></span>

- [<span data-ttu-id="aaabb-193">Sistem sorgularının listesi</span><span class="sxs-lookup"><span data-stu-id="aaabb-193">List of system queries</span></span>](insights-programmatic-system-queries.md)
- [<span data-ttu-id="aaabb-194">Örnek sorgu listesi</span><span class="sxs-lookup"><span data-stu-id="aaabb-194">List of sample queries</span></span>](insights-programmatic-sample-queries.md)