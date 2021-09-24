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
ms.openlocfilehash: 674cc6f800edc540920d80bedd031fae959b973b
ms.sourcegitcommit: fceaca54b0ec695cf214209c09b4516e1b40866a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/24/2021
ms.locfileid: "128366141"
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

Rapor oluşturma API'si bir geri çağırma URL'si kabul eder. Bu URL, rapor oluşturma işlemi başarılı olduktan sonra çağrılacaktır. Geri çağırma URL 'SI genel olarak erişilebilir olmalıdır. URL 'ye ek olarak, bir geri çağırma yöntemi de verilebilir. Geri çağırma yöntemi yalnızca "GET" veya "POST" olabilir. Hiçbir değer geçirilmezse, varsayılan yöntem "POST" olacaktır. Oluşturmayı tamamlamış olan REPORTID, her zaman geri arama sırasında geri geçirilir.

Geri arama gönder: geçirilen URL Ise `https://www.contosso.com/callback` , çağrılan geri URL 'si `https://www.contosso.com/callback/<reportID>` 

Geri arama al: geçilen URL Ise `https://www.contosso.com/callback` , çağrılan geri URL 'si `https://www.contosso.com/callback?reportId=<reportID>` 

### <a name="executenow-reports"></a>ExecuteNow raporları

Zamanlama olmadan rapor oluşturmak için bir sağlama vardır. Rapor oluşturma API 'si yükü, `ExecuteNow` API çağrıldıktan hemen sonra raporun oluşturulmasını sıraya alacak bir parametreyi kabul edebilir. `ExecuteNow`True olarak ayarlandığında, `StartTime` `RecurrenceCount` `RecurrenceInterval` Bu raporlar zamanlanmadığından alanlar:, yok sayılır.

True olduğunda iki ek alan geçirilebilir `ExecuteNow` `QueryStartTime` ve `QueryEndTime` . Bu iki alan, `TIMESPAN` sorgudaki alanı geçersiz kılar. Bu alanlar, değişiklik olmayan sabit bir zaman dilimi için sürekli olarak oluşturulan veriler, zamanlanan raporlar için geçerli değildir.

### <a name="request-syntax"></a>İstek sözdizimi

|    Yöntem     |    İstek URI'si     |
|----- | -----|
|    POST     |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport` |

### <a name="request-header"></a>İstek üst bilgisi

|    Üst bilgi     |    Tür     |    Description     |
|-------|-----|------|
|    Yetkilendirme     |    string |Gereklidir. Azure Active Directory (Azure AD) erişim belirteci. Biçim  `Bearer <token>` .|
|    İçerik Türü     |string |`Application/JSON` |

### <a name="path-parameter"></a>Yol parametresi

Hiçbiri

### <a name="query-parameter"></a>Sorgu parametresi

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

İstek yükünde öğelerin temel tanımları aşağıda verilmiştir:

|    Parametre     |    Gerekli     |    Açıklama     |    İzin Verilen Değerler     |
|    ----    |    ----    |    ----    |    ----    |
|    ReportName     |    Yes     |    Rapora atanacak ad     |    string     |
|    Açıklama     |    Hayır     |    Oluşturulan raporun açıklaması     |    string     |
|    QueryId     |    Yes     |    Rapor sorgu KIMLIĞI     |    string     |
|    StartTime     |    Yes     |    Rapor oluşturmanın başlayacağı UTC zaman damgası. <br> Biçim şu şekilde olmalıdır: yyyy-MM-ddTHH: mm: ssZ       |    string     |
|    ExecuteNow     |    No     |    Bu parametre, yalnızca bir kez yürütülecek bir rapor oluşturmak için kullanılmalıdır. `StartTime`, `RecurrenceInterval` , ve `RecurrenceCount` true olarak ayarlanırsa yok sayılır. Rapor, anında zaman uyumsuz bir biçimde yürütülür     |    doğru/yanlış     |
|    QueryStartTime     |    No     |    İsteğe bağlı olarak, verileri ayıklayan sorgunun başlangıç saatini belirtir. Bu parametre yalnızca, true olarak ayarlanmış tek seferlik yürütme raporları için geçerlidir `ExecuteNow` . Sorguda verilen bu parametre geçersiz kılmaları ayarlanıyor `TIMESPAN` . Biçim yyyy-MM-ddTHH: mm: ssZ olmalıdır     |    Dize olarak zaman damgası     |
|    QueryEndTime     |    No     |    İsteğe bağlı olarak, verileri ayıklayan sorgunun bitiş saatini belirtir. Bu parametre yalnızca, true olarak ayarlanmış bir kerelik yürütme raporu için geçerlidir `ExecuteNow` . Sorguda verilen bu parametre geçersiz kılmaları ayarlanıyor `TIMESPAN` . Biçim yyyy-MM-ddTHH: mm: ssZ olmalıdır     |    Dize olarak zaman damgası     |
|    Recurrenceınterval     |    Yes     |    Raporun oluşturulması gereken saat sıklığı. <br> En küçük değer 4, en büyük değer 2160 ' dir.      |    tamsayı     |
|    RecurrenceCount     |    No     |    Oluşturulacak rapor sayısı.     |    tamsayı     |
|    Biçimlendir     |    No     |    İçe aktarılmış dosyanın dosya biçimi. <br> Varsayılan CSV 'dir.    |    "CSV"/"TSV"     |
|    CallbackUrl     |    No     |    İsteğe bağlı olarak, geri arama hedefi olarak yapılandırılabilen, genel olarak erişilebilen URL     |    Dize (http URL 'SI)     |
|    CallbackMethod     |    No     |    Geri arama için kullanılacak yöntem     |    AL/POSTALA     |
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
|    executionStatus    |    No    |    Dize/Enum    |    Yalnızca bu bağımsız değişkende verilen executionStatus raporlarının ayrıntılarını almak için filtreleyin. <br> Geçerli değerler şunlardır: `Pending` , `Running` , `Paused` , ve `Completed` . <br> `Completed` varsayılan değerdir. <br> Birden çok durum noktalı virgül ";" ile ayrılarak belirtilebilir.    |
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
- [İlk API çağrısını yapın] (insights-programmatic-first-api-call.md
