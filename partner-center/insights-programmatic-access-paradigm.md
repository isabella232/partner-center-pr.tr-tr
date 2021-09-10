---
title: Öngörüler verileri için programlı erişim paradigması
description: Programlı analizler için API çağrı deseninin üst düzey akışını anlayın. Partner Insights Analytics raporlarına erişim API 'Leri de ele alınmıştır.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 1a06da353c8069d15d597faeaaf8700df5f62fd1
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960825"
---
# <a name="programmatic-access-paradigm"></a>Programlı erişim paradigması

Bu diyagramda yeni bir rapor şablonu oluşturmak için kullanılan API çağrı deseninin yanı sıra özel rapor zamanlanır ve hata verileri alınır.

:::image type="content" source="images/insights/prog-acc-paradigm.png" alt-text="Üst düzey akış":::
***Şekil 1: API çağrı deseninin yüksek düzey akışı***

Bu liste Şekil 1 hakkında daha fazla ayrıntı sağlar.

1. Istemci uygulaması, [rapor sorgusu oluştur API](#create-report-query-api)'sini çağırarak özel rapor şemasını/şablonunu tanımlayabilir. Alternatif olarak, burada listelenen rapor şablonu kitaplık örneklerinden bir rapor şablonu (QueryId) seçebilirsiniz [.](insights-programmatic-system-queries.md)
2. Başarılı olduğunda rapor sorgusu oluştur API 'SI QueryId döndürür.
3. Daha sonra istemci uygulamasının rapor başlangıç tarihi, yineleme aralığı, yinelenme ve isteğe bağlı bir geri çağırma URI 'SI ile birlikte QueryId kullanarak [rapor oluşturma API](#create-report-api) 'sini çağırması gerekir.
4. Başarı durumunda [rapor oluşturma API 'Si](#create-report-api) REPORTID ' yi döndürür.
5. İstemci uygulaması, rapor verileri indirilmeye uygun hale geldiğinde geri çağırma URL 'sinden bildirim alır.
6. İstemci uygulaması daha sonra rapor KIMLIĞI ve tarih aralığı ile raporun durumunu sorgulamak için [rapor yürütmeleri al API](#get-report-execution-api) 'sini kullanır.
7. Başarı durumunda, rapor indirme bağlantısı döndürülür ve uygulama verilerin indirilmesini başlatabilir.

## <a name="report-query-language-specification"></a>Rapor sorgusu dil belirtimi

Raporları oluşturmak için kullanabileceğiniz [Sistem sorguları](insights-programmatic-system-queries.md) sağlamamız sırasında, iş gereksinimlerinize göre kendi sorgularınızı de oluşturabilirsiniz. Özel sorgular hakkında daha fazla bilgi için bkz. [özel sorgu belirtimi](insights-programmatic-custom-query.md).

## <a name="create-report-query-api"></a>Rapor sorgu API 'SI oluştur

API, hangi sütunların ve ölçümlerin verilmesi gereken veri kümesini tanımlayan özel sorgular oluşturmaya yardımcı olur. API, iş gereksinimlerinize göre yeni bir raporlama şablonu oluşturma esnekliğini sağlar.  

Sağladığımız [sistem sorgularını](insights-programmatic-system-queries.md) da kullanabilirsiniz. Özel rapor şablonları gerekli olmadığında, sağlanmış sistem sorgularının QueryIds değerlerini kullanarak doğrudan [Create Report API](#create-report-api) çağırabilirsiniz.  

Aşağıdaki örnek, son ayın gelirine göre ilk 10 müşteriyi almak için özel bir sorgu oluşturmayı gösterir.

### <a name="request-syntax"></a>İstek sözdizimi

|    Yöntem     |    İstek URI'si     |
|----- | -----|
|    POST     |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries`|
|||

### <a name="request-header"></a>İstek üst bilgisi

|    Üst bilgi     |    Tür     |    Description     |
|-------|-----|------|
|    Yetkilendirme     |    string |Gereklidir. Azure Active Directory (Azure AD) erişim belirteci. Biçim  `Bearer <token>` .|
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

Bu tablo, istek yükünde öğelerin temel tanımlarını sağlar.

|Parametre|    Gerekli     |    Açıklama     |    İzin Verilen Değerler     |
|-----|    -----    |    -----    |    -----    |
|Name |    Yes     |    Sorgunun kolay adı     |    string     |
|    Açıklama     |    Hayır     |    Sorgunun döndürdüğü açıklama     |    string     |
|    Sorgu     |    Yes     |    Rapor sorgu dizesi     |    Veri türü: dize <br> İş gereksinimini temel alan [özel sorgu](insights-programmatic-custom-query.md) |
|        |        |        |        |

> [!Note]
> Özel sorgu örnekleri için bkz [. örnek sorgu örnekleri.](insights-programmatic-sample-queries.md)

### <a name="sample-response"></a>Örnek yanıt

Yanıt yükü aşağıdaki şekilde yapılandırılır:

Yanıt kodları: 200, 400, 401, 403, 500

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

Bu tablo, istek yükünde öğelerin temel tanımlarını sağlar.

|    Parametre     |    Açıklama     |
|    ----    |    ----    |
|    QueryId     |    Oluşturduğunuz sorgunun evrensel benzersiz tanımlayıcısı (UUID)     |
|    Name     |    İstek yükünde sorguya kolay ad verildi     |
|    Description     |    Sorgunun oluşturulması sırasında verilen açıklama     |
|    Sorgu     |    Sorgu oluşturma sırasında rapor sorgusu giriş olarak geçildi     |
|    Tür     |    Ayarla `userDefined`     |
|    Kullanıcı     |    Sorgu oluşturmak için kullanılan Kullanıcı KIMLIĞI     |
|    CreatedTime     |    Sorgunun oluşturulduğu UTC saati: yyyy-MM-ddTHH: mm: ssZ     |
|    TotalCount     |    Değer dizisindeki veri kümesi sayısı     |
|    Durum     |    Sonuç Kodu <br> Olası değerler 200, 400, 401, 403, 500     |
|    message     |    API 'nin yürütülmesindeki durum iletisi     |
|        |        |

## <a name="create-report-api"></a>Rapor API 'SI oluştur

Özel rapor şablonu oluşturma ve sorgu yanıtı [oluşturma](#create-report-query-api) ' nın bir parçası olarak QueryId alma sırasında, bu API, düzenli aralıklarla yürütülecek bir sorgu zamanlamak için çağrılabilir. Raporun teslim edileceği sıklığı ve zamanlamayı ayarlayabilirsiniz.
Sağladığımız sistem sorguları için, rapor oluşturma API 'SI de [QueryId](insights-programmatic-system-queries.md)ile çağrılabilir.

### <a name="callback-url"></a>Geri Çağırma URL’si

Rapor oluşturma API 'si bir geri çağırma URL 'sini kabul eder. Rapor oluşturma başarılı olduktan sonra bu URL çağrılır. Geri çağırma URL'si genel olarak erişilebilir olmalıdır. URL'ye ek olarak bir geri çağırma yöntemi de verilmiştir. Geri çağırma yöntemi yalnızca "GET" veya "POST" olabilir. Hiçbir değer geçirilse varsayılan yöntem "POST" olur. Oluşturmayı tamamlayan reportId her zaman geri çağırma sırasında geri geçiri.

POST geri çağırma: Geçirilen URL `https://www.contosso.com/callback` ise, geri çağrılır URL şu şekilde olur: `https://www.contosso.com/callback/<reportID>` 

GET geri çağırma: Geçirilen URL `https://www.contosso.com/callback` ise, geri çağrılır URL şu şekilde olur: `https://www.contosso.com/callback?reportId=<reportID>` 

### <a name="executenow-reports"></a>ExecuteNow raporları

Zamanlama olmadan rapor oluşturmak için bir sağlama vardır. Rapor oluşturma API yükü bir parametresini kabul eder. Bu parametre, API çağrılır oluşturulmaz rapor `ExecuteNow` oluşturulur. true olarak ayarlandığı zaman, şu raporlar zamanlanmaz çünkü , alanları `ExecuteNow` `StartTime` `RecurrenceCount` `RecurrenceInterval` yoksayılır.

true olduğunda ve olmak için `ExecuteNow` iki ek alan `QueryStartTime` `QueryEndTime` geçirebilirsiniz. Bu iki alan, `TIMESPAN` sorguda alanı geçersiz kılar. Veriler değişmeden sabit bir süre için sürekli olarak oluşturulacak olan zamanlanmış raporlar için bu alanlar geçerli değildir.

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
|    QueryStartTime     |    No     |    İsteğe bağlı olarak, verileri ayıklanan sorgunun başlangıç saati belirtir. Bu parametre yalnızca true olarak ayarlanmış bir kez yürütme `ExecuteNow` raporu için geçerlidir. Sorguda verilen bu parametre `TIMESPAN` geçersiz kılmalarını ayarlama. Biçim yyyy-MM-ddTHH:mm:ssZ olmalıdır     |    Dize olarak zaman damgası     |
|    QueryEndTime     |    No     |    İsteğe bağlı olarak, verileri ayıklanan sorgunun bitiş saati belirtir. Bu parametre yalnızca true olarak ayarlanmış bir kez yürütme `ExecuteNow` raporu için geçerlidir. Sorguda verilen bu parametre `TIMESPAN` geçersiz kılmalarını ayarlama. Biçim yyyy-MM-ddTHH:mm:ssZ olmalıdır     |    Dize olarak zaman damgası     |
|    RecurrenceInterval     |    Yes     |    Raporun oluşturulacak saat sıklığı. <br> En düşük değer 4, Maksimum değer ise 2160'tır.      |    tamsayı     |
|    RecurrenceCount     |    No     |    Oluşturulan rapor sayısı.     |    tamsayı     |
|    Biçimlendir     |    No     |    Dışarı aktaran dosyanın dosya biçimi. <br> Csv varsayılandır.    |    "CSV"/"TSV"     |
|    CallbackUrl     |    No     |    İsteğe bağlı olarak geri çağırma hedefi olarak yapılandırılan genel olarak erişilebilir URL     |    Dize (http URL'si)     |
|    CallbackMethod     |    No     |    Geri çağırma için kullanılacak yöntem     |    GET/POST     |
|        |        |        |        |

### <a name="sample-response"></a>Örnek yanıt

Yanıt yükü aşağıdaki şekilde yapılandırılır:

Yanıt kodları: 200, 400, 401, 403, 404, 500

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

Yanıttaki öğelerin temel tanımları aşağıda verilmiştir:

|    Parametre     |    Açıklama     |
|    ----    |    ----    |
|    REPORTID     |    Oluşturduğunuz raporun evrensel benzersiz tanımlayıcısı (UUID)     |
|    ReportName     |    İstek yükünde rapora verilen ad     |
|    Description     |    Raporun oluşturulması sırasında verilen açıklama     |
|    QueryId     |    Raporu oluşturduğunuz sırada geçirilen sorgu KIMLIĞI     |
|    Sorgu     |    Bu rapor için yürütülecek sorgu metni     |
|    Kullanıcı     |    Raporu oluşturmak için kullanılan Kullanıcı KIMLIĞI     |
|    CreatedTime     |    Raporun şu biçimde oluşturulduğu UTC saati: yyyy-MM-ddTHH: mm: ssZ     |
|    ModifiedTime     |    Raporun bu biçimde en son değiştirildiği UTC saati: yyyy-MM-ddTHH: mm: ssZ     |
|    ExecuteNow     |    `ExecuteNow` raporun oluşturulduğu sırada ayarlanan bayrak     |
|    StartTime     |    Rapor yürütmenin bu biçimde başlayacağı UTC saati: yyyy-MM-ddTHH: mm: ssZ     |
|    ReportStatus     |    Rapor yürütmenin durumu. Olası değerler şunlardır `Paused` , `Active` ve `Inactive`     |
|    Recurrenceınterval     |    Rapor oluşturma sırasında belirtilen yinelenme aralığı     |
|    RecurrenceCount     |    Rapor oluşturma sırasında yinelenme sayısı belirtildi.      |
|    CallbackUrl     |    İstekte belirtilen geri çağırma URL 'SI     |
|    CallbackMethod     |    İstekte belirtilen geri çağırma yöntemi     |
|    Biçimlendir     |    Rapor dosyalarının biçimi. Olası değerler veya ' `CSV` dir `TSV` .     |
|    TotalCount     |    Değer dizisindeki kayıt sayısı     |
|    Durum     |    Sonuç Kodu     |
|    message     |    Olası değerler 200, 400, 401, 403, 500 ' dir. API 'nin yürütülmesindeki durum iletisi     |
|        |        |

## <a name="get-report-execution-api"></a>Rapor yürütme API 'sini al

[Rapor oluşturma API](#create-report-api)'Sinden alınan REPORTID kullanarak rapor yürütmenin durumunu sorgulamak için bu yöntemi kullanabilirsiniz. Rapor indirmeye hazırsanız, yöntemi rapor indirme bağlantısını döndürür. Aksi takdirde, yöntemi durumu döndürür. Belirli bir rapor için gerçekleşen tüm yürütmeleri almak için bu API 'yi de kullanabilirsiniz.  

>[!IMPORTANT]
>Bu API, ve için ayarlanmış varsayılan sorgu parametrelerine sahiptir `executionStatus=Completed` `getLatestExecution=true` . Bu nedenle, raporun ilk başarılı yürütülmesi için önce API çağrılması 404 döndürür. Bekleyen yürütmeler, ayarıyla elde edilebilir `executionStatus=Pending` .

### <a name="request-syntax"></a>İstek sözdizimi

|    Yöntem     |    İstek URI'si     |
|----- | -----|
|    GET    |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/{reportId}?executionId={executionId}&executionStatus={executionStatus}&getLatestExecution={getLatestExecution}`  |

### <a name="request-header"></a>İstek üst bilgisi

|    Üst bilgi     |    Tür     |    Description     |
|-------|-----|------|
|    Yetkilendirme     |    string |Gereklidir. Azure Active Directory (Azure AD) erişim belirteci. Biçim  `Bearer <token>` .|
|    İçerik Türü     |string |`Application/JSON` |

### <a name="path-parameter"></a>Yol parametresi

|    Parametre Adı    |    Gerekli    |    Tür    |    Description    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId    |    Yes    |    string    |    Yalnızca bu bağımsız değişkende verilen REPORTID 'ye sahip raporların yürütme ayrıntılarını almak için filtreleyin. Birden çok Inceleme, noktalı virgül ";" ile ayrılarak belirtilebilir.    |
|        |        |        |        |

### <a name="query-parameter"></a>Sorgu parametresi

|    Parametre Adı    |    Gerekli    |    Tür    |    Description    |
|    ----    |    ----    |    ----    |    ----    |
|    Yürütme    |    No    |    string    |    Yalnızca bu bağımsız değişkende verilen ExecutionID 'ye sahip raporların ayrıntılarını almak için filtreleyin. Birden çok ExecutionID, noktalı virgül ";" ile ayrılarak belirtilebilir.    |
|    executionStatus    |    No    |    Dize/Enum    |    Yalnızca bu bağımsız değişkende verilen executionStatus raporlarının ayrıntılarını almak için filtreleyin. <br> Geçerli değerler şunlardır: `Pending` , `Running` , `Paused` ve `Completed` . <br> `Completed` varsayılan değerdir. <br> Birden çok durum noktalı virgül ";" ile ayrılarak belirtilebilir.    |
|    getLatestExecution    |    No    |    boolean    |    API, en son yürütmenin ayrıntılarını döndürür. Varsayılan olarak, bu parametre true olarak ayarlanır.<br> Bu parametrenin değerini false olarak geçirmeye seçerseniz, API son 90 gün yürütme örneğini döndürür.    |
|        |        |        |        |

### <a name="sample-request-payload"></a>Örnek Istek yükü

Hiçbiri

### <a name="sample-response"></a>Örnek Yanıt

Yanıt yükü aşağıdaki şekilde yapılandırılır:

Yanıt kodları: 200, 400, 401, 403, 404, 500

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

Rapor yürütme tamamlandıktan sonra, yürütme durumu `Completed` gösterilir. İçindeki URL 'YI seçerek raporu indirebilirsiniz `reportAccessSecureLink` .

### <a name="glossary"></a>Sözlük

Yanıttaki öğelerin anahtar tanımları.

|    Parametre    |    Açıklama    |
|    ----    |    ----    |
|    Yürütme    |    Yürütme örneğinin evrensel benzersiz tanımlayıcısı (UUID)    |
|    REPORTID    |    Yürütme örneğiyle ilişkili rapor KIMLIĞI    |
|    Recurrenceınterval    |    Rapor oluşturma sırasında belirtilen yinelenme aralığı    |
|    RecurrenceCount    |    Rapor oluşturma sırasında belirtilen yinelenme sayısı    |
|    CallbackUrl    |    Yürütme örneğiyle ilişkili geri çağırma URL 'SI    |
|    CallbackMethod    |    Yürütme örneğiyle ilişkili geri çağırma yöntemi    |
|    Biçimlendir    |    Yürütmenin sonunda oluşturulan dosyanın biçimi    |
|    ExecutionStatus    |    Rapor yürütme örneğinin durumu. <br> Geçerli değerler şunlardır: `Pending` , `Running` , `Paused` , ve `Completed`    |
|    ReportAccessSecureLink    |Rapora güvenli erişilebilen bağlantı        |
|    Reportexpiryıtime    |    Rapor bağlantısının süresinin dolmasına geçen UTC saati: yyyy-MM-ddTHH: mm: ssZ    |
|    ReportGeneratedTime    |    Raporun şu biçimde oluşturulduğu UTC saati: yyyy-MM-ddTHH: mm: ssZ    |
|    TotalCount    |    Değer dizisindeki veri kümesi sayısı    |
|    Durum    |    Sonuç Kodu <br> Olası değerler 200, 400, 401, 403, 404 ve 500    |
|    message    |    API 'nin yürütülmesindeki durum iletisi    |
|        |        |

## <a name="next-steps"></a>Sonraki adımlar

- [Swagger API URL 'si](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html) aracılığıyla API 'leri deneyin
- [İlk API çağrısını yapın](insights-programmatic-first-api-call.md)