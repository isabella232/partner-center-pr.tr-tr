---
title: Öngörü verileri için programlı erişim paradigması
description: Programlı analiz için API çağrı deseninin üst düzey akışını anlama. İş ortağı içgörüleri analiz raporlarına erişmek için API'ler de ele alındır.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 304607b5d79b0ad8a07c3efe690ccb7feef83331
ms.sourcegitcommit: 8d5c2463fc0f0c03972a6f89d01605421288daea
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/19/2021
ms.locfileid: "128001692"
---
# <a name="programmatic-access-paradigm"></a>Programlı erişim paradigması

Bu diyagramda, yeni bir rapor şablonu oluşturmak, özel raporu zamanlamayı ve hata verilerini almak için kullanılan API çağrı deseni gösterir.

:::image type="content" source="images/insights/prog-acc-paradigm.png" alt-text="Üst düzey akış":::
***Şekil 1: API çağrı deseninin üst düzey akışı***

Bu liste Şekil 1 hakkında daha fazla ayrıntı sağlar.

1. İstemci Uygulaması, Rapor Sorgusu OLUŞTURMA API'sini çağırarak özel rapor [şemasını/şablonunu tanımlayabilir.](#create-report-query-api) Alternatif olarak, iş ortağı içgörüleri programlı erişimi için sistem sorguları listesi'nde yer alan rapor şablonu kitaplığı örneklerinden bir rapor şablonu (QueryId) [seçebilirsiniz.](insights-programmatic-system-queries.md)
2. Başarılı olduğu zaman Rapor Sorgusu OLUŞTURMA API'si QueryId döndürür.
3. İstemci uygulamasının daha sonra [](#create-report-api) QueryId ile birlikte rapor başlangıç tarihi, Yineleme Aralığı, Yinelenme ve isteğe bağlı bir Geri Çağırma URI'si kullanarak Rapor Oluşturma API'sini çağırması gerekir.
4. Başarılı olduğu zaman Rapor [Oluşturma API'si](#create-report-api) ReportId döndürür.
5. Rapor verileri indirmeye hazır olduğunda istemci uygulaması geri çağırma URL'sinde bilgi alır.
6. İstemci uygulaması daha sonra Rapor [Yürütmeleri Al](#get-report-execution-api) API'sini kullanarak rapor durumunu Rapor Kimliği ve tarih aralığıyla sorgular.
7. Başarılı olduğu zaman, rapor indirme bağlantısı döndürülür ve uygulama verileri indirmeyi başlatabilirsiniz.

## <a name="report-query-language-specification"></a>Rapor sorgu dili belirtimi

Rapor oluşturmak için [kullanabileceğiniz sistem](insights-programmatic-system-queries.md) sorguları sağlarken, iş ihtiyaçlarına göre kendi sorgularınızı da oluşturabilirsiniz. Özel sorgular hakkında daha fazla bilgi edinmek için bkz. [Özel Sorgu Belirtimi.](insights-programmatic-custom-query.md)

## <a name="create-report-query-api"></a>Rapor sorgusu API'si oluşturma

API, sütunların ve ölçümlerin dışarı aktarıldıklarından veri kümelerini tanımlayan özel sorgular oluşturmanıza yardımcı olur. API, iş ihtiyaçlarınıza göre yeni bir raporlama şablonu oluşturma esnekliği sağlar.  

Ayrıca, bizim [sağlaymız sistem sorgularını](insights-programmatic-system-queries.md) da kullanabilirsiniz. Özel rapor şablonları gerekli değilken, sağlanan sistem sorgularının QueryId'lerini kullanarak rapor [oluşturma API'sini](#create-report-api) doğrudan çağırabilirsiniz.  

Aşağıdaki örnekte, geçen aya göre gelire göre ilk 10 müşteriyi almak için özel bir sorgunun nasıl oluşturulacakları gösterir.

### <a name="request-syntax"></a>İstek söz dizimi

|    Yöntem     |    İstek URI'si     |
|----- | -----|
|    POST     |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries`|
|||

### <a name="request-header"></a>İstek üst bilgisi

|    Üst bilgi     |    Tür     |    Description     |
|-------|-----|------|
|    Yetkilendirme     |    string |Gereklidir. Azure Active Directory (Azure AD) erişim belirteci. Biçimi şu  `Bearer <token>` şekildedir: .|
|    İçerik Türü     |string |`Application/JSON` |
||||

### <a name="path-parameter"></a>Yol parametresi

Hiçbiri

### <a name="query-parameter"></a>Sorgu parametresi

Hiçbiri

### <a name="sample-request-payload"></a>Örnek istek yükü

```json
{ 
  "Name": "CustomersRevenueQuery", 
  "Description": "Query to get top 10 customers by revenue for last month", 
  "Query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH" 
}
```

### <a name="glossary"></a>Sözlük

Bu tablo, istek yükünde öğelerin anahtar tanımlarını sağlar.

|Parametre|    Gerekli     |    Açıklama     |    İzin Verilen Değerler     |
|-----|    -----    |    -----    |    -----    |
|Name |    Yes     |    Sorgunun kolay adı     |    string     |
|    Açıklama     |    Hayır     |    Sorgunun döndürenlerin açıklaması     |    string     |
|    Sorgu     |    Yes     |    Rapor sorgu dizesi     |    Veri türü: dize <br> [İş ihtiyaçlarına](insights-programmatic-custom-query.md) göre özel sorgu |
|        |        |        |        |

> [!Note]
> Özel sorgu örnekleri için [bkz. Örnek sorgu örnekleri.](insights-programmatic-sample-queries.md)

### <a name="sample-response"></a>Örnek yanıt

Yanıt yükü aşağıdaki gibi yapılandırılmıştır:

Yanıt Kodları: 200, 400, 401, 403, 500

Yanıt yükü örneği:

```json
{ 
  "value": [ 
    { 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
      "name": "CustomersRevenueQuery",
      "description": "Query to get top 10 customers by revenue for last month",
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T12:52:39Z" 
    }
  ], 
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
} 
```

### <a name="glossary"></a>Sözlük

Bu tablo, istek yükünde öğelerin anahtar tanımlarını sağlar.

|    Parametre     |    Açıklama     |
|    ----    |    ----    |
|    Queryıd     |    Oluşturduğunuz sorgunun evrensel olarak benzersiz tanımlayıcısı (UUID)     |
|    Name     |    İstek yükünde sorguya kolay ad verilir     |
|    Description     |    Sorgunun oluşturulması sırasında verilen açıklama     |
|    Sorgu     |    Sorgu oluşturma sırasında giriş olarak geçirilen rapor sorgusu     |
|    Tür     |    Olarak ayarlayın `userDefined`     |
|    Kullanıcı     |    Sorguyu oluşturmak için kullanılan kullanıcı kimliği     |
|    CreatedTime     |    UTC Sorgunun şu biçimde oluşturulma zamanı: yyyy-MM-ddTHH:mm:ssZ     |
|    TotalCount     |    Değer dizisinde veri kümesi sayısı     |
|    Statuscode     |    Sonuç Kodu <br> Olası değerler: 200, 400, 401, 403, 500     |
|    message     |    API'nin yürütülmesinden gelen durum iletisi     |
|        |        |

## <a name="create-report-api"></a>Rapor API'si oluşturma

Özel bir rapor şablonu başarıyla oluşturulurken ve [](#create-report-query-api) Rapor Sorgusu Oluştur yanıtının bir parçası olarak QueryID alınarak, düzenli aralıklarla yürütülecek bir sorgu zamanlaması için bu API çağrılabilirsiniz. Raporun teslimi için bir sıklık ve zamanlama ayarlayın.
Sistem sorguları için, Rapor Oluşturma API'si QueryId ile de [çağrılabilirsiniz.](insights-programmatic-system-queries.md)

### <a name="callback-url"></a>Geri Çağırma URL’si

Rapor oluşturma API'si bir geri çağırma URL'si kabul eder. Rapor oluşturma başarılı olduktan sonra bu URL çağrılır. Geri çağırma URL'sinin genel olarak erişilebilir olması gerekir. URL'ye ek olarak bir geri çağırma yöntemi de verilmiştir. Geri çağırma yöntemi yalnızca "GET" veya "POST" olabilir. Hiçbir değer geçirilse varsayılan yöntem "POST" olur. Oluşturmayı tamamlayan reportId her zaman geri çağırma sırasında geri geçiri.

POST geri çağırma: Geçirilen URL `https://www.contosso.com/callback` ise, geri çağrılır URL şu şekilde olur: `https://www.contosso.com/callback/<reportID>` 

GET geri çağırma: Geçirilen URL `https://www.contosso.com/callback` ise, geri çağrılır URL şu şekilde olur: `https://www.contosso.com/callback?reportId=<reportID>` 

### <a name="executenow-reports"></a>ExecuteNow raporları

Zamanlama olmadan rapor oluşturmak için bir sağlama vardır. Rapor oluşturma API yükü bir parametresini kabul eder. Bu parametre, API çağrılır oluşturulmaz rapor `ExecuteNow` oluşturulur. True olarak ayarlandığı zaman, şu raporlar zamanlanmaz çünkü , alanları `ExecuteNow` `StartTime` `RecurrenceCount` `RecurrenceInterval` yoksayılır.

true olduğunda ve olmak için `ExecuteNow` iki ek alan `QueryStartTime` `QueryEndTime` geçirebilirsiniz. Bu iki alan sorguda `TIMESPAN` alanı geçersiz kılar. Veriler değişmeden sabit bir süre için sürekli olarak oluşturulacak olan zamanlanmış raporlar için bu alanlar geçerli değildir.

### <a name="request-syntax"></a>İstek söz dizimi

|    Yöntem     |    İstek URI'si     |
|----- | -----|
|    POST     |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport` |

### <a name="request-header"></a>İstek üst bilgisi

|    Üst bilgi     |    Tür     |    Description     |
|-------|-----|------|
|    Yetkilendirme     |    string |Gereklidir. Azure Active Directory (Azure AD) erişim belirteci. Biçimi şu  `Bearer <token>` şekildedir: .|
|    İçerik Türü     |string |`Application/JSON` |

### <a name="path-parameter"></a>Yol Parametresi

Hiçbiri

### <a name="query-parameter"></a>Sorgu Parametresi

Hiçbiri

### <a name="sample-request-payload"></a>Örnek istek yükü

```json
{
  "ReportName": "Top10_CustomersReport",
  "Description": "Top 10 customers by revenue for last month",
  "QueryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
  "StartTime": "2021-03-31T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": null,
  "QueryEndTime": null,
  "RecurrenceInterval": 24,
  "RecurrenceCount": 100,
  "Format": "CSV",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}
```

### <a name="glossary"></a>Sözlük

İstek yükünde öğelerin anahtar tanımları aşağıda açıklanmıştır:

|    Parametre     |    Gerekli     |    Açıklama     |    İzin Verilen Değerler     |
|    ----    |    ----    |    ----    |    ----    |
|    Raporadı     |    Yes     |    Rapora atanacak ad     |    string     |
|    Açıklama     |    Hayır     |    Oluşturulan raporun açıklaması     |    string     |
|    Queryıd     |    Yes     |    Rapor sorgusu kimliği     |    string     |
|    StartTime     |    Yes     |    Rapor oluşturmanın başlayacağı UTC Zaman Damgası. <br> Biçim şu şekilde olmalıdır: yyyy-MM-ddTHH:mm:ssZ       |    string     |
|    ExecuteNow     |    No     |    Bu parametre, yalnızca bir kez yürütülecek bir rapor oluşturmak için kullanılmalıdır. `StartTime`, `RecurrenceInterval` ve , true olarak `RecurrenceCount` ayarlanırsa yoksayılır. Rapor hemen zaman uyumsuz bir şekilde yürütülür     |    true/false     |
|    QueryStartTime     |    No     |    İsteğe bağlı olarak, verileri ayıklanan sorgunun başlangıç saati belirtir. Bu parametre yalnızca true olarak ayarlanmış tek bir kez yürütme `ExecuteNow` raporları için geçerlidir. Sorguda verilen bu parametre `TIMESPAN` geçersiz kılmalarını ayarlama. Biçim yyyy-MM-ddTHH:mm:ssZ olmalıdır     |    Dize olarak zaman damgası     |
|    QueryEndTime     |    No     |    İsteğe bağlı olarak, verileri ayıklanan sorgunun bitiş saati belirtir. Bu parametre yalnızca true olarak ayarlanmış bir kez yürütme `ExecuteNow` raporu için geçerlidir. Sorguda verilen bu parametre `TIMESPAN` geçersiz kılmalarını ayarlama. Biçim yyyy-MM-ddTHH:mm:ssZ olmalıdır     |    Dize olarak zaman damgası     |
|    RecurrenceInterval     |    Yes     |    Raporun oluşturulacak saat sıklığı. <br> En düşük değer 4, Maksimum değer ise 2160'tır.      |    tamsayı     |
|    RecurrenceCount     |    No     |    Oluşturulan rapor sayısı.     |    tamsayı     |
|    Biçimlendir     |    No     |    Dışarı aktaran dosyanın dosya biçimi. <br> Csv varsayılandır.    |    "CSV"/"TSV"     |
|    CallbackUrl     |    No     |    İsteğe bağlı olarak geri arama hedefi olarak yapılandırılan genel olarak erişilebilir URL     |    Dize (http URL'si)     |
|    CallbackMethod     |    No     |    Geri çağırma için kullanılacak yöntem     |    GET/POST     |
|        |        |        |        |

### <a name="sample-response"></a>Örnek yanıt

Yanıt yükü aşağıdaki gibi yapılandırılmıştır:

Yanıt Kodları: 200, 400, 401, 403, 404, 500

Yanıt yükü örneği:

```json
{ 
  "value": [
    { 
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf", 
      "reportName": "Top10_CustomersReport", 
      "description": "Top 10 customers by revenue for last month", 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033", 
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH", 
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T13:11:58Z", 
      "modifiedTime": null, 
      "executeNow": false, 
      "startTime": "2021-03-31T18:41:00Z", 
      "reportStatus": "Active", 
      "recurrenceInterval": 24, 
      "recurrenceCount": 100, 
      "callbackUrl": "https://<SampleCallbackUrl>", 
      "callbackMethod": "GET", 
      "format": "csv"
    } 
  ], 
  "nextLink": null, 
  "totalCount": 1, 
  "message": "Report created successfully", 
  "statusCode": 200, 
  "dataRedacted": false 
}
```

### <a name="glossary"></a>Sözlük

Yanıtta yer alan öğelerin anahtar tanımları aşağıda açıklanmıştır:

|    Parametre     |    Açıklama     |
|    ----    |    ----    |
|    ReportId     |    Oluşturduğunuz raporun evrensel olarak benzersiz tanımlayıcısı (UUID)     |
|    Raporadı     |    İstek yükünde rapora verilen ad     |
|    Description     |    Rapor oluşturma sırasında verilen açıklama     |
|    Queryıd     |    Raporu oluşturduğunuz sırada geçirilen sorgu kimliği     |
|    Sorgu     |    Bu rapor için yürütülecek sorgu metni     |
|    Kullanıcı     |    Raporu oluşturmak için kullanılan kullanıcı kimliği     |
|    CreatedTime     |    UTC Raporun şu biçimde oluşturulma zamanı: yyyy-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    UTC Raporun son değiştirilma zamanı: yyyy-MM-ddTHH:mm:ssZ     |
|    ExecuteNow     |    `ExecuteNow` raporun oluşturulma zamanında ayarlanmış bayrağı     |
|    StartTime     |    UTC Saati Rapor yürütme şu biçimde başlar: yyyy-MM-ddTHH:mm:ssZ     |
|    ReportStatus     |    Rapor yürütme durumu. Olası değerler `Paused` , `Active` ve değerleridir `Inactive`     |
|    RecurrenceInterval     |    Rapor oluşturma sırasında sağlanan yinelenme aralığı     |
|    RecurrenceCount     |    Rapor oluşturma sırasında sağlanan yineleme sayısı.      |
|    CallbackUrl     |    İstekte sağlanan geri çağırma URL'si     |
|    CallbackMethod     |    İstekte sağlanan geri çağırma yöntemi     |
|    Biçimlendir     |    Rapor dosyalarının biçimi. Olası değerler veya `CSV` `TSV` değerleridir.     |
|    TotalCount     |    Değer dizisinde kayıt sayısı     |
|    Statuscode     |    Sonuç Kodu     |
|    message     |    Olası değerler: 200, 400, 401, 403, 500. API'nin yürütülmesinden gelen durum iletisi     |
|        |        |

## <a name="get-report-execution-api"></a>Rapor yürütme API'sini al

Rapor Oluşturma API'sinde alınan ReportId'yi kullanarak rapor yürütme durumunu sorgulamak için [bu yöntemi kullanabilirsiniz.](#create-report-api) Yöntem, rapor indirme için hazırsa rapor indirme bağlantısını döndürür. Aksi takdirde yöntem durumu döndürür. Ayrıca, bu API'yi kullanarak bir rapor için olan tüm yürütmeleri elde edin.  

>[!IMPORTANT]
>Bu API' de ve için varsayılan sorgu parametreleri `executionStatus=Completed` `getLatestExecution=true` ayarlanmıştır. Bu nedenle, raporun ilk başarılı yürütülmesi öncesinde API'nin çağrılsı 404'ü sonuç olarak gösterir. Bekleyen yürütmeler ayarıyla elde `executionStatus=Pending` edilir.

### <a name="request-syntax"></a>İstek söz dizimi

|    Yöntem     |    İstek URI'si     |
|----- | -----|
|    GET    |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/{reportId}?executionId={executionId}&executionStatus={executionStatus}&getLatestExecution={getLatestExecution}`  |

### <a name="request-header"></a>İstek üst bilgisi

|    Üst bilgi     |    Tür     |    Description     |
|-------|-----|------|
|    Yetkilendirme     |    string |Gereklidir. Azure Active Directory (Azure AD) erişim belirteci. Biçimi şu  `Bearer <token>` şekildedir: .|
|    İçerik Türü     |string |`Application/JSON` |

### <a name="path-parameter"></a>Yol parametresi

|    Parametre Adı    |    Gerekli    |    Tür    |    Description    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId    |    Yes    |    string    |    Yalnızca bu bağımsız değişkende verilen reportId değerine sahip raporların yürütme ayrıntılarını almak için filtreyi seçin. Birden çok reportId, noktalı virgül ";" ile ayrılarak belirtilebilir.    |
|        |        |        |        |

### <a name="query-parameter"></a>Sorgu parametresi

|    Parametre Adı    |    Gerekli    |    Tür    |    Description    |
|    ----    |    ----    |    ----    |    ----    |
|    Executionıd    |    No    |    string    |    Yalnızca bu bağımsız değişkende verilen executionId değerine sahip raporların ayrıntılarını almak için filtreyi seçin. Birden çok executionId, noktalı virgül ";" ile ayrılarak belirtilebilir.    |
|    executionStatus    |    No    |    Dize/enum    |    Yalnızca bu bağımsız değişkende verilen executionStatus değerine sahip raporların ayrıntılarını almak için filtrele. <br> Geçerli değerler: `Pending` , , ve `Running` `Paused` `Completed` . <br> `Completed` varsayılan değerdir. <br> Birden çok durum, noktalı virgül ";" ile ayrılarak belirtilebilir.    |
|    getLatestExecution    |    No    |    boolean    |    API en son yürütmenin ayrıntılarını dönecektir. Varsayılan olarak, bu parametre true olarak ayarlanır.<br> Bu parametrenin değerini false olarak geçmeyi seçerseniz, API son 90 günlük yürütme örneklerini döndürür.    |
|        |        |        |        |

### <a name="sample-request-payload"></a>Örnek İstek Yükü

Hiçbiri

### <a name="sample-response"></a>Örnek Yanıt

Yanıt yükü aşağıdaki gibi yapılandırılmıştır:

Yanıt Kodları: 200, 400, 401, 403, 404, 500

Yanıt yükü örneği:

```json
{
  "value": [
    {
      "executionId": "906931dc-4f2f-4195-bbb2-d7295c7550d3",
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf",
      "recurrenceInterval": 24,
      "recurrenceCount": 100,
      "callbackUrl": null,
      "callbackMethod": null,
      "format": "csv",
      "executionStatus": "Completed",
      "reportLocation": null,
      "reportAccessSecureLink": "https://<path to report for download>",
      "reportExpiryTime": null,
      "reportGeneratedTime": "2021-03-31T18:41:00Z"
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

Rapor yürütme tamamlandıktan sonra yürütme `Completed` durumu gösterilir. içinde URL'yi seçerek raporu `reportAccessSecureLink` indirebilirsiniz.

### <a name="glossary"></a>Sözlük

Yanıtta öğelerin anahtar tanımları.

|    Parametre    |    Açıklama    |
|    ----    |    ----    |
|    Executionıd    |    Yürütme örneğinin evrensel olarak benzersiz tanımlayıcısı (UUID)    |
|    ReportId    |    Yürütme örneğiyle ilişkili rapor kimliği    |
|    RecurrenceInterval    |    Rapor oluşturma sırasında sağlanan yinelenme aralığı    |
|    RecurrenceCount    |    Rapor oluşturma sırasında sağlanan yinelenme sayısı    |
|    CallbackUrl    |    Yürütme örneğiyle ilişkili geri çağırma URL'si    |
|    CallbackMethod    |    Yürütme örneğiyle ilişkili geri çağırma yöntemi    |
|    Biçimlendir    |    Yürütmenin sonunda oluşturulan dosyanın biçimi    |
|    ExecutionStatus    |    Rapor yürütme örneğinin durumu. <br> Geçerli değerler: `Pending` , `Running` , `Paused` ve `Completed`    |
|    ReportAccessSecureLink    |Rapora güvenli bir şekilde erişilebilen bağlantı        |
|    ReportExpiryTime    |    Utc Saati: Rapor bağlantısının süresi şu biçimde dolacak: yyyy-MM-ddTHH:mm:ssZ    |
|    ReportGeneratedTime    |    Raporun şu biçimde üret alındığı UTC Saati: yyyy-MM-ddTHH:mm:ssZ    |
|    TotalCount    |    Değer dizisinde veri kümesi sayısı    |
|    Statuscode    |    Sonuç Kodu <br> Olası değerler: 200, 400, 401, 403, 404 ve 500    |
|    message    |    API'nin yürütülmesinden gelen durum iletisi    |
|        |        |

## <a name="next-steps"></a>Sonraki adımlar

- [Swagger API URL'si aracılığıyla API'leri deneyin](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)
- [İlk API çağrınızı yapma] (insights-programmatic-first-api-call.md
