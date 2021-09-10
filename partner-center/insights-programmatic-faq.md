---
title: İş ortağı içgörülerine programlı erişim için sık sorulan sorular
description: API aracılığıyla iş ortağı içgörüleri verilerine erişme hakkında sık sorulan soruların yanıtlarını alın.
ms.topic: troubleshooting
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 418af23ae50e1f8d9086b2eb6247ba964e4c1516
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961395"
---
# <a name="programmatic-access-of-analytics-data-common-questions"></a>Analiz verilerine program aracılığıyla erişim hakkında sık sorulan sorular

Bu makalede, iş ortağı içgörüleri verilerine program aracılığıyla erişme hakkında sık sorulan sorular İş Ortağı Merkezi.

## <a name="api-responses"></a>API yanıtları

200 (Başarılı) dışında hangi senaryolarda API yanıtı aliyorum?

Bu tablo API yanıtlarını ve bunları alırsanız ne yapacaklarını açıklar.

|    Hata açıklaması     |    Hata kodu     |    Sorun giderme     |
|    ----    |    ----    |    ----    |
|    Yetkisiz     |    401     |    Bu bir kimlik doğrulaması özel durumudur. Azure Active Directory (AAD) belirtecin doğru olup olmadığını denetleyin. AAD belirteci 60 dakika geçerlidir ve bu sürenin ardından AAD belirteci yeniden oluşturma gerekir.     |
|    Geçersiz tablo adı     |    400     |    Veri kümesi adı yanlış. "Tüm Veri Kümelerini Al" API'sini çağırarak veri kümesi adını yeniden kontrol edin.     |
|    Yanlış sütun adı     |    400     |    Sorgudaki sütunun adı yanlış. "Tüm Veri Kümelerini Al" API'sini çağırarak sütun adını yeniden işaretleyin veya Veri Tanımları'nın sütun adlarında yer alan sütun adlara bakın    |
|    Null veya eksik değer     |    400     |    API'nin istek yükünün bir parçası olarak zorunlu parametreler eksik olabilir.     |
|    Geçersiz rapor parametreleri     |    400     |    Rapor parametrelerinin doğru olduğundan emin olun. Örneğin RecurrenceInterval parametresi için 4'den küçük bir değer veriyor olabilirsiniz.     |
|    Yinelenme Aralığı 4 ile 2160 arasında olmalıdır     |    400     |    RecurrenceInterval istek parametresinin değerinin 4 ile 2160 arasında olduğundan emin olun.     |
|    Geçersiz QueryId     |    400     |    Oluşturulan QueryId'i yeniden işaretleyin.     |
|    Oluşturma için geçersiz rapor parametreleri - Raporun başlangıç saati geçerli UTC saatine en az 4 saat olmalıdır     |    400     |    İstek yükünün bir parçası olarak Başlangıç Zamanı parametresi geçmişte olmaması gerekir. Raporun başlangıç saati, geçerli UTC saati ile en az 4 saat arasında olabilir.     |
|    İstenen 'string' değeri bulunamadı     |    400     |    İstek parametrelerini mi yoksa biçimini mi `callbackurl` güncelleştirilmiş olduğunu kontrol edin.     |
|    Verilen filtrelerle öğe bulunamadı.     |    404     |    Get Report Executions API'sinde kullanılan reportID parametresini kontrol edin.     |
|    Verilen filtre koşulları için herhangi bir yürütme yoktur. reportId veya executionId'yi bir kez daha kontrol edin ve raporun zamanlanmış yürütme zamanından sonra API'yi yeniden deneyin     |    404     |    reportId'nin doğru olduğundan emin olun. İSTEK yükünde belirtilen raporun zamanlanmış yürütme zamanından sonra API'yi yeniden deneyin.     |
|    Rapor oluşturulurken iç hatayla karşılaşıldı. Bağıntı kimliği <>     |    500     |    *StartTime,* *QueryStartTime* ve *QueryEndTime* alanlarının tarih biçiminin doğru olduğundan emin olun.     |
|    Hizmet kullanılamıyor    |    500     |    Sürekli olarak kullanılamayan bir hizmet alırsanız (5xx hatası) bir destek bileti açın.    |
|        |        |        |

## <a name="no-records"></a>Kayıt yok

Raporu güvenli konumdan indirirken API yanıtı 200'leri alırsınız. Neden hiç kayıt al değilim?
Sorgudaki dizenin sütun üst bilgisi için izin verilebilir değerlerden biri olup olmadığını kontrol edin. Örneğin, bu sorgu sıfır sonuç verir:

```sql
SELECT CustomerTenantId, CustomerTpId, WorkloadName, Month, MonthlyActiveUsers 
FROM OfficeUsage 
WHERE IsDuplicateRowForPGA = 'False' 
ORDER BY CustomerTenantId DESC
```

Bu örnekte, için izin verilebilir değerler `IsDuplicateRowForPGA` 0 veya 1'tir. Çeşitli sütunlar [için tüm olası](insights-data-definitions.md) değerler için Veri Tanımları'ne bakın.
