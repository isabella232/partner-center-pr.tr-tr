---
title: İş ortağı öngörülerine yönelik genel sorular programlama erişimi
description: API aracılığıyla partner Insights verilerine erişme hakkında sık sorulan soruların yanıtlarını alın.
ms.topic: troubleshooting
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 418af23ae50e1f8d9086b2eb6247ba964e4c1516
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114836974"
---
# <a name="programmatic-access-of-analytics-data-common-questions"></a>Analiz verilerine program aracılığıyla erişim hakkında sık sorulan sorular

Bu makalede, Iş Ortağı Merkezi 'nde iş ortağı öngörülerine programlı bir şekilde erişme hakkında sıkça sorulan sorular ele alınmaktadır.

## <a name="api-responses"></a>API yanıtları

200 (başarılı) dışında bir API yanıtı alabildiğim farklı senaryolar nelerdir?

Bu tablo, API yanıtlarını ve bunları alırsanız ne yapılacağını açıklar.

|    Hata açıklaması     |    Hata kodu     |    Sorun giderme     |
|    ----    |    ----    |    ----    |
|    Yetkisiz     |    401     |    Bu bir kimlik doğrulama istisnadır. Azure Active Directory (AAD) belirtecinin doğruluğunu denetleyin. AAD belirteci 60 dakika için geçerlidir, bu süre sonra AAD belirtecini yeniden oluşturmanız gerekir.     |
|    Geçersiz tablo adı     |    400     |    Veri kümesinin adı yanlış. "Tüm veri kümelerini al" API 'sini çağırarak veri kümesi adını yeniden denetleyin.     |
|    Sütun adı yanlış     |    400     |    Sorgudaki sütunun adı yanlış. "Tüm veri kümelerini al" API 'sini çağırarak sütun adını yeniden denetleyin veya veri tanımlarındaki sütun adlarına başvurun    |
|    Null veya eksik değer     |    400     |    API 'nin istek yükünün bir parçası olarak zorunlu parametreler eksik olabilir.     |
|    Geçersiz rapor parametreleri     |    400     |    Rapor parametrelerinin doğru olduğundan emin olun. Örneğin, Recurrenceınterval parametresi için 4 ' ten az bir değer vermiş olabilirsiniz.     |
|    Yinelenme aralığı 4 ile 2160 arasında olmalıdır     |    400     |    Recurrenceınterval istek parametresinin değerinin 4 ile 2160 arasında olduğundan emin olun.     |
|    Geçersiz QueryId     |    400     |    Oluşturulan QueryId 'yi yeniden denetleyin.     |
|    Oluşturma için geçersiz rapor parametreleri-raporun başlangıç zamanı, geçerli UTC zamanından en az 4 saat olmalıdır     |    400     |    İstek yükünün parçası olarak başlangıç zamanı parametresi geçmişte olmamalıdır. Raporun başlangıç saati, geçerli UTC zamanından en az 4 saat olmalıdır.     |
|    İstenen ' String ' değeri bulunamadı     |    400     |    İstek parametrelerini mi yoksa biçimini mi güncelleştirmeyeceğinizi denetleyin `callbackurl` .     |
|    Verilen filtrelere sahip öğe bulunamadı.     |    404     |    Rapor yürütmeleri API 'sinde kullanılan REPORTID parametresini denetleyin.     |
|    Belirtilen filtre koşulları için oluşmuş yürütmeler yok. REPORTID veya ExecutionID 'yi iki kez kontrol edin ve raporun zamanlanan yürütme zamanından sonra API 'yi yeniden deneyin     |    404     |    REPORTID 'nin doğru olduğundan emin olun. İstek yükünde belirtilen şekilde raporun zamanlanan yürütme zamanından sonra API 'yi yeniden deneyin.     |
|    Rapor oluşturulurken iç hatayla karşılaşıldı. Bağıntı KIMLIĞI <>     |    500     |    Alanlar için tarih biçiminin *StartTime*, *Querystarttime* ve *queryendtime* doğru olduğundan emin olun.     |
|    Hizmet kullanılamıyor    |    500     |    Sürekli olarak bir hizmet (5xx hatası) alırsanız bir destek bileti açın.    |
|        |        |        |

## <a name="no-records"></a>Kayıt yok

Raporu güvenli konumdan indirdiğimde API yanıtı 200 ' i alıyorum. Neden kayıt alıyorum?
Sorgudaki dizenin, sütun üst bilgisi için izin verilen değerlerden birine sahip olup olmadığını denetleyin. Örneğin, bu sorgu sıfır sonuç döndürür:

```sql
SELECT CustomerTenantId, CustomerTpId, WorkloadName, Month, MonthlyActiveUsers 
FROM OfficeUsage 
WHERE IsDuplicateRowForPGA = 'False' 
ORDER BY CustomerTenantId DESC
```

Bu örnekte, için izin verilen değerler `IsDuplicateRowForPGA` 0 veya 1 ' dir. Çeşitli sütunlarda tüm olası değerler için [veri tanımlarına](insights-data-definitions.md) bakın.
