---
title: Öngörüler veri tanımları
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Belge, Öngörüler Indirme raporu sayfasından indirilebilen çeşitli raporların ve her bir raporun veri tanımlarının listesini sağlar.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d4a805957fac7c7cff373d807347b7c6d0b13d6f
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2020
ms.locfileid: "97502134"
---
# <a name="export--data-definitions"></a>Dışarı aktarma – veri tanımları 

 **Uygun roller** 

- Rapor Görüntüleyicisi 
- Executive rapor Görüntüleyicisi 

## <a name="introduction"></a>Giriş 

Öngörüler panosundaki rapor Indirme Merkezi, ham veri kümelerini dışa aktarmaya olanak sağlar.  

Veri tanımıyla birlikte indirilebilen çeşitli raporlar aşağıda verilmiştir: 

**Iş ortağı profili**: profil raporunun çeşitli alanlarının veri tanımları şunlardır: 


| **Sütun adı** | **Veri açıklaması** |
|---------|:---------|
|Mpnıd|Microsoft İş Ortağı Ağı KIMLIĞI|
|PartnerName|Ortağın adı |
|PGA_MPNId|İş ortağı küresel hesap MPN KIMLIĞI|
|PGA_PartnerName|Ortak genel hesap adı|
|Şehir|Iş ortağının şehir konumu |
|Ülke|Iş ortağının ülke konumu |
|HierarchyLevel|Küresel bir MPN KIMLIĞI mi yoksa MPN KIMLIĞI mi olduğunu belirtir|

**Müşteri ayrıntıları**: müşteri ayrıntıları raporunun çeşitli alanlarının veri tanımları şunlardır:

| **Sütun adı** | **Veri açıklaması** |
|---------|:---------|
|CustomerName|Müşterinin adı |
|CustomerTenantId|Müşteri Kiracı Kimliği |
|Customertpıd|Müşteri üst üst öğe tanımlayıcısı |
|CustomerSegment|Müşteri kesimi |
|CustomerMarket|Müşterinin coğrafi pazarı  |
|CustomerStatus|Müşteri durumu (etkin/etkin değil) |
|Ürün|MPN tarafından müşteriye satılan ürün. Bu, O365, D365, Enterprise Mobility, Power BI, Microsoft Azure bir tane olacaktır.|
|SKU|   Ürün SKU 'SU|
|Ay| Kullanım ve gelirin bildirildiği ay|
|Mpnıd| Microsoft İş Ortağı Ağı KIMLIĞI|
|PartnerName|   Ortağın adı|
|PartnerLocation|   İş ortağının coğrafi konumu|
|PartnerAttributionType|    İş ortağının attributıon türü|
|SalesChannel|  Satış kanalı|
|Availablekoltuk|    Kullanılabilir koltuk| 
|RevenueUSD|    ABD Doları cinsinden gelir|

**Satıcı performansı**: satıcı performans raporlarının çeşitli alanlarının veri tanımları şunlardır:

> [!Note]
> Gelir ve ACR verileri yalnızca Executive rapor izleyicileri olan kullanıcılar tarafından kullanılabilir.

| **Sütun adı** | **Veri açıklaması** |
|---------|:---------|
|Resellermpnıd|Satıcı Microsoft İş Ortağı Ağı tanımlayıcısı| 
|ResellerName|Satıcı adı|
|ResellerMarket|Market Bayi ülkesi| 
|Indirectprovidermpnıd|Dolaylı sağlayıcı Microsoft İş Ortağı Ağı tanımlayıcısı|
|Indirectprovidername|Dolaylı sağlayıcı adı|
|Ay|Kullanım ve gelirin bildirildiği ay|
|Ürün|Ürün Adı|
|SubscriptionID|Abonelik tanımlayıcısı|
|Availablekoltuk|Kullanılabilir lisans sayısı|
|AssignedSeats|Atanan bilgisayar lisansı sayısı|
|BilledRevenueUSD|Faturalandırılan gelir ($ $)|
|CustomerName|Müşterinin adı| 
|Customertpıd|Müşteri üst üst öğe tanımlayıcısı| 
|CustomerSegment|Müşteri kesimi |
|CustomerMarket|Müşterinin coğrafi pazarı |
|ResellerStatus|Satıcı durumu| 

**Abonelik ayrıntıları**: abonelik ayrıntıları raporunun çeşitli alanlarının veri tanımları şunlardır:

>[!Note]
>Gelir ve ACR verileri yalnızca Executive rapor izleyicileri olan kullanıcılar için kullanılabilir

| **Sütun adı** | **Veri açıklaması** |
|---------|:---------|
|SubscriptionId|    Aboneliğin GUID 'SI|
|SubscriptionStartDate| Aboneliğin başlangıç tarihi|
|SubscriptionEndDate|   Aboneliğin bitiş tarihi|
|SubscriptionState| Aboneliğin durumu (etkin veya uygulanmış)|
|Ay| Kullanım ve gelirin bildirildiği ay|
|IsAutoRenew|   Aboneliğin otomatik olarak yenilenmesi veya oluşturulmayacağını belirtir (e/h)|
|CustomerName|  Müşteri Adı| 
|CustomerTenantId|  Müşteri GUID 'SI|
|Customertpıd|  Müşteri üst üst öğe tanımlayıcısı| 
|CustomerSegment|   Müşterinin pazar segmenti| 
|CustomerMarket|    Müşterinin coğrafi pazarı|
|Ürün|   Iş ortağı tarafından müşteriye satılan ürün| 
|SKU|   Ürünün SKU 'su |
|Mpnıd| Ortağın Microsoft İş Ortağı Ağı KIMLIĞI |
|PartnerName|   Ortağın adı |
|PartnerLocation|   Ortağın coğrafi konumu |
|PartnerAttributionType|    Abonelik için attributıon türü|
|SalesChannel|  Satışın kanalı (doğrudan/CSP vb.) |
|Availablekoltuk|    Mevcut kullanılabilir bilgisayar|
|RevenueUSD|    ABD Doları cinsinden gelir|
|Kayıt KIMLIĞI| Aboneliğin kayıt KIMLIĞI|

**Azure kullanımı**: Azure kullanım raporunun çeşitli alanlarının veri tanımları şunlardır:

| **Sütun adı** | **Veri açıklaması** |
|---------|:---------|
|SubscriptionId|    Aboneliğin GUID 'SI|
|SubscriptionStartDate| Aboneliğin başlangıç tarihi.|
|SubscriptionEndDate|   Aboneliğin bitiş tarihi.|
|SubscriptionState| Aboneliğin geçerli durumu (açık/kapalı/etkin/ınyetkisiz kullanım süresi)|
|Ay| Aya göre toplanan Tarih |
|ServiceName|   Azure hizmetinin adı|
|MeterCategory| Ölçüm kategorisinin adı|
|UsageUnits|    Fatura çevrimi sırasında kullanılan birim sayısı |
|CustomerName|  Müşterinin adı |
|CustomerTenantId|  Müşterinin kiracı KIMLIĞI |
|Customertpıd|  Müşteri üst üst KIMLIĞI |
|CustomerSegment|   Müşterinin segmenti |
|CustomerMarket|    Müşterinin coğrafi pazarı |
|Mpnıd  |Microsoft İş Ortağı Ağı müşterinin KIMLIĞI |
|PartnerName|   Ortağın adı |
|PartnerLocation    |Ortağın coğrafi ülke konumu |
|PartnerAttributionType |İş ortağının attributıon türü|
|SalesChannel|  Satışın kanalı (doğrudan/CSP dolaylı/CSP doğrudan vb.) |
|ACR_USD|   Azure tüketilen gelir ABD Doları|
|Kayıt KIMLIĞI| Azure aboneliğinin kayıt KIMLIĞI|

**Office 365-lisans kullanımı**: Office 365-lisans kullanım raporunun çeşitli alanlarının veri tanımları şunlardır:

| **Sütun adı** | **Veri açıklaması** |
|---------|:---------|
|CustomerTenantId|  Müşterinin kiracı KIMLIĞI| 
|Customertpıd|  Müşteri üst üst KIMLIĞI |
|WorkloadName|  SFB, takımlar, EXO |
|Ay| Kullanımın bildirildiği ay|
|Paidavvailableunits|    Ücretli kullanılabilir birim sayısı|
|MonthlyActiveUsers|    Aylık etkin kullanıcı sayısı|
|CustomerName|  Müşterinin adı|
|CustomerMarket|    Müşterinin pazarında coğrafi ülke konumu |
|CustomerSegment|   Müşteri kesimi |
|Mpnıd| Microsoft İş Ortağı Ağı KIMLIĞI|
|PartnerName|   Ortağın adı|
|PartnerLocation|   İş ortağının coğrafi konumu|
|PartnerAttributionType|    İş ortağının attributıon türü|

**Enterprise Mobility – lisans kullanımı**: EMS – lisans kullanım raporunun çeşitli alanlarının veri tanımı:

| **Sütun adı** | **Veri açıklaması** |
|---------|:---------|
|CustomerTenantId|  Müşterinin kiracı KIMLIĞI| 
|Customertpıd|  Müşteri üst üst KIMLIĞI |
|WorkloadName|  EMS iş yükünün adı |
|Ay| Kullanımın bildirildiği ay|
|Paidavvailableunits|    Ücretli kullanılabilir birim sayısı|
|MonthlyActiveUsers|    Aylık etkin kullanıcı sayısı|
|CustomerName|  Müşterinin adı|
|CustomerMarket|Müşterinin pazarında coğrafi ülke konumu |
|CustomerSegment|   Müşteri kesimi |
|Mpnıd| Microsoft İş Ortağı Ağı KIMLIĞI|
|PartnerName|   Ortağın adı|
|PartnerLocation|   İş ortağının coğrafi konumu|
|PartnerAttributionType|    İş ortağının attributıon türü|

**Dynamics 365 – lisans kullanımı**: Dynamics 365 – lisans kullanım raporunun çeşitli alanlarının veri tanımı:

| **Sütun adı** | **Veri açıklaması** |
|---------|:---------|
|SubscriptionId|Aboneliğin GUID 'SI|
|SubscriptionStartDate| Aboneliğin başlangıç tarihi|
|SubscriptionEndDate|   Aboneliğin bitiş tarihi|
|Abonelik durumu|    Aboneliğin durumu |
|Ay| Kullanımın bildirildiği ay|
|RevSumDivisionName|    Rev Sum bölümünün adı|
|RevSumCategoryName|    Rev Sum kategorisinin adı|
|SKU|   Ürünün SKU 'su |
|SkuId| Ürünün SKU KIMLIĞI |
|Freevspaıdsku| Ücretsiz veya ücretli SKU olup olmadığını belirtir |
|SalesModel|    Aboneliği satmakta kullanılan satış kanalı|
|DetailedSalesModel|    Abonelik için ayrıntılı satış modeli|
|CustomerName|  Müşteri Adı |
|CustomerTenantId|  Müşteri kiracı GUID 'SI |
|Customertpıd|  Müşteri üst üst öğe tanımlayıcısı |
|CustomerSegment|   Müşterinin pazar segmenti |
|CustomerMarket|    Müşterinin coğrafi pazarı |
|Mpnıd| Microsoft iş ortağı ağ KIMLIĞI |
|PartnerName|   Ortağın adı |
|PartnerLocation|   Ortağın coğrafi ülke konumu |
|PartnerAttachType| Abonelik için attributıon türü|
|Availablekoltuk|    Mevcut kullanılabilir bilgisayar|
|AssignedSeats| Geçerli atanan bilgisayar |
|Activekoltuk|   Geçerli etkin koltuk |
|DeploymentOpportunity| Geçerli dağıtım fırsatı|
|Activeusage yüzdesi|    Geçerli etkin kullanım yüzdesi|
 
**Power BI lisansı kullanımı**: Power BI – lisans kullanım raporunun çeşitli alanlarının veri tanımı:

| **Sütun adı** | **Veri açıklaması** |
|---------|:---------|
|SubscriptionId|    Aboneliğin GUID 'SI|
|SubscriptionStartDate| Aboneliğin başlangıç tarihi|
|SubscriptionEndDate|   Aboneliğin bitiş tarihi|
|Abonelik durumu|    Aboneliğin durumu (etkin veya In-Active veya yetkisiz kullanım süresi)|
|Ay| Aya göre toplanan Tarih |
|SKU|   Ürünün SKU 'su |
|SkuId| Ürünün SKU KIMLIĞI |
|Freevspaıdsku| Ücretsiz veya ücretli SKU Farklılama |
|SalesModel|    Aboneliği satmak için kullanılan satış modeli|
|DetailedSalesModel|    Abonelik için ayrıntılı satış modeli|
|CustomerName|  Müşteri Adı |
|CustomerTenantId|  Müşteri kiracı GUID 'SI |
|Customertpıd|  Müşteri üst üst öğe tanımlayıcısı| 
|CustomerSegment|   Müşterinin pazar segmenti |
|CustomerMarket|    Müşterinin coğrafi pazarı |
|Mpnıd| Microsoft İş Ortağı Ağı KIMLIĞI |
|PartnerName|   Ortağın adı |
|PartnerLocation|   Ortağın coğrafi ülke konumu |
|PartnerAttachType| Abonelik için attributıon türü|
|Availablekoltuk|    Mevcut kullanılabilir koltuk|
|AssignedSeats| Geçerli atanan koltuk|
|Activekoltuk|   Geçerli etkin koltuk|
|DeploymentOpportunity| Geçerli dağıtım fırsatı|
|Activeusage yüzdesi|    Geçerli etkin kullanım yüzdesi|

**Takımlar kullanımı – toplantılar ve çağrılar**: çeşitli alanların veri tanımları şunlardır:

| **Sütun adı** | **Veri açıklaması** |
|---------|:---------|
|CustomerTenantId|  Müşterinin kiracı KIMLIĞI |
|Customertpıd|  Müşteri üst üst KIMLIĞI |
|Ay| Kullanımın bildirildiği ay|
|Alt iş yükü|   Kullanım için bildirilen alt iş yükü (toplantılar, çağrılar, telefon sistemleri)|
|Toplantı sayısı| Toplantı sayısı|
|Toplantı süresi|  Toplam toplantı süresi (saat)|

**Takımlar-aylık kullanım ayrıntıları**: çeşitli alanların veri tanımları şunlardır:

| **Sütun adı** | **Veri açıklaması** |
|---------|:---------|
|CustomerTenantId|  Müşterinin kiracı KIMLIĞI |
|Customertpıd|  Müşteri üst üst KIMLIĞI |
|Ay| Kullanımın bildirildiği ay|
|Alt iş yükü|   Kullanım için bildirilen alt iş yükü (toplantılar, çağrılar, telefon sistemleri)|
|Masaüstü kullanıcıları| Masaüstünde takımlar kullanan kullanıcı sayısı|
|Mobil Kullanıcılar|  Mobil üzerinde takımlar kullanan kullanıcı sayısı|
|Web kullanıcıları| Web üzerinde takımlar kullanan kullanıcı sayısı|
|Allupkatılımcıları| Aya ait farklı takımların Kullanıcı sayısı|

**Takımlar kullanımı – 3P uygulamalar**: çeşitli alanların veri tanımları şunlardır:

| **Sütun adı** | **Veri açıklaması** |
|---------|:---------|
|CustomerTenantId|  Müşterinin kiracı KIMLIĞI| 
|Customertpıd|  Müşteri üst üst KIMLIĞI |
|Ay| Kullanımın bildirildiği ay|
|3P uygulama adı|   Takımlar uygulamasının adı|
|Kullanıcı sayısı|    Uygulama için Kullanıcı sayısı|


**Eğitim ayrıntıları**: eğitim ayrıntıları raporundaki çeşitli alanların veri tanımları şunlardır:

| **Sütun adı** | **Veri açıklaması** |
|---------|:---------|
|Traıningactivityıd|    Eğitimin tanımlayıcısı |
|Traıningtitle| Eğitimin başlığı |
|Traıningtype|  Eğitim türü (sertifika/sınav)|
|Kişiselleştirsoyadı|   Müşterinin ilk adı| 
|Kişiselleştirallastname|    Müşterinin soyadı| 
|E-posta| Müşterinin kişisel e-posta KIMLIĞI|
|CorpEmail| Müşterinin ofis e-posta KIMLIĞI|
|Traıningcompletiondate|    Eğitimin tamamlanma tarihi |
|Ay| Verilerin bildirildiği ay|
|IMCP| Kullanıcının Microsoft sertifikalı bir profesyonel olup olmadığını belirtir|
|MCPID| Kullanıcının MCP KIMLIĞI|
|Mpnıd| Microsoft İş Ortağı Ağı KIMLIĞI |
|PartnerName|   Ortağın adı |
|PartnerCityLocation|   Ortağın coğrafi şehir konumu |
|PartnerCountryLocation|    Ortağın coğrafi ülke konumu |

**Microsoft Learn**: Microsoft Learn raporunun çeşitli alanlarının veri tanımları şunlardır:

| **Sütun adı** | **Veri açıklaması** |
|---------|:---------|
|UserName|Kullanıcının adı| 
|UserId|Kullanıcı GUID 'SI |
|Traıningname|Eğitimin adı |
|Traıningtype|Eğitim türü (modül/Learning yolu)|
|Ürünler|Öğrenme modülünün geçerli olduğu ürün|
|Roller|Eğitimin uygun rolleri |
|CompletionDate|Eğitimin tamamlanma tarihi |
|Mpnıd|Microsoft İş Ortağı Ağı KIMLIĞI |
|PartnerName|Ortağın adı |
|Ülke|Ortağın coğrafi ülke konumu |

**Uzmanlığa ilişkin özet ve geçmiş**: uzmanlık Özeti ve geçmiş raporunun çeşitli alanlarının veri tanımı:

| **Sütun adı** | **Veri açıklaması** |
|---------|:---------|
|Uzmanlık adı|Uzmanlığa ilişkin ad |
|Uzmanlık düzeyi|Uzmanlık düzeyi (Altın/Gümüş)|
|Uzmanlık durumu|Uzmanlığa ait geçerli durum (etkin/etkin olmayan/yetkisiz kullanım süresi)|
|Uzmanlık tarihi|Verilen uzmanlığa ait başlangıç tarihi| 
|Uzmandan bir yenne tarihi|Verilen uzmanlık bitiş tarihi |

**Uzmanlık performansı**: uzmanlığa göre performans raporunun çeşitli alanlarının veri tanımları şunlardır:

| **Sütun adı** | **Veri açıklaması** |
|---------|:---------|
|Uzmanlık adı|    Uzmanlığa ilişkin ad |
|Yıo Encyatlationmentoptionname|    Uzmanlığa erişme seçeneğinin adı|
|Ay| Ölçümlerin bildirildiği ay|
|MetricName|    Uzmanlığa uygun ölçüm adı|
|Metricmonthlykatkısı| Ölçümün aylık katkısı|
|TTMAggregate|  Sondaki 12 ay için toplanan ölçüm|
|Anniversarne Yearaggregate|  Geçerli yıldönümü yılı için toplanan ölçüm|
|GoldThreshold| Altın uzmanlığa uyması için performans gereksinimi|
|SilverThreshold|   Gümüş uzmanlığa uyması için performans gereksinimi|

**Cloud Ascent-M365 eğilimini**: Cloud Ascent-M365 eğilimini raporunun çeşitli alanlarının veri tanımları şunlardır:

| **Sütun adı** | **Veri açıklaması** |
|---------|:---------|
|MPN Kimliği|    Microsoft İş Ortağı Ağı KIMLIĞI|
|İş ortağı adı|  Ortağın adı|
|Müşteri Kimliği|   Müşteri tanımlayıcı numarası |
|DYENIDEN sayı|   Dun & Bradstreet, eğilimini için puanlanmış müşterinin numarası|
|Hesap Adı|  Hesap adı |
|Etki alanı|    Hesabın etki alanı|
|Kuruluş boyutu|  Kuruluşun boyutu|
|Sektör|  Sektör  |
|Dikey|  Microsoft ve diğer sektör standartları (D&B) tarafından tanımlandığı şekilde eğilimini için puanlanmakta olan müşterinin dikey|
|Alan|  Konumun coğrafi alanı|
|Yan Kuruluş|    Eğilimini için puanlanmakta olan müşterinin yan kuruluşu|
|Sales Territory|   Eğilimini için puanlanmakta olan müşterinin satış bölgesi|
|Şehir|  Coğrafi şehir konumu |
|Durum| Coğrafi durum konumu|
|Posta Kodu|   Posta Kodu|
|Ülke|   Coğrafi ülke konumu |
|Segment|   Pazar segmenti |
|Alt kesim|   Pazar alt segmenti |
|SMC tür Özeti|  SMC türü |
|En iyi yönetilmeyen Işlem tabanı|  En çok yönetilmeyen müşteriler – işlem|
|En çok yönetilmeyen-kullanıcı tabanı| En iyi yönetilmeyen müşteriler – Kullanıcı|
|Iskar dışı|   Kar dışı veya kar için (Evet/Hayır)|
|Uzak çalışma hedefi Exchange Online 'ı etkinleştir|   Etkin bir Exchange Online aboneliğine sahip olan müşteriler, M365 'e satış|
|CLAS eğilimini-+ 10 lisanslarıyla uzaktan çalışma-şirket içi alımı (geçerli sürüm) etkinleştirin|Mevcut şirket içi Office veya Win Client (yani, EOS ürünlerinden sonra olan sürümler) olan müşteriler. Müşterinin 10 veya daha fazla lisansı vardır. Eğilimini puanı olan müşteri. İş ortakları, M365 dönüştürmesi için hedeflemelidir.|
|CLAS eğilimini-<10 lisanslarıyla uzak Iş-şirket içi alımı (güncel sürüm) etkinleştirin|Mevcut şirket içi Office veya Win Client (yani, EOS ürünlerinden sonra olan sürümler) olan müşteriler. Müşterinin 10 ' dan az lisansı vardır. Eğilimini puanı olan müşteri. İş ortakları, M365 dönüştürmesi için hedeflemelidir.|
|CLAS eğilimini-+ 10 lisansı olmadan uzak Iş-şirket içi alımı (geçerli sürüm) etkinleştir| Mevcut şirket içi Office veya Win Client (yani, EOS ürünlerinden sonra olan sürümler) olan müşteriler. Müşterinin 10 veya daha fazla lisansı vardır. Müşterinin eğilimini puanı yok. İş ortakları, M365 dönüştürmesi için hedeflemelidir.|
|Eğilimini-<10 lisansı olmadan uzak Iş-şirket içi alımı (geçerli sürüm) etkinleştir| Mevcut şirket içi Office veya Win Client (yani, EOS ürünlerinden sonra olan sürümler) olan müşteriler. Müşterinin 10 ' dan az lisansı vardır. Müşterinin eğilimini puanı yok. İş ortakları, M365 dönüştürmesi için hedeflemelidir.|
|CLAS eğilimini-+ 10 lisanslarıyla uzaktan çalışma-şirket içi alımı (EOS) etkinleştirin|EOS şirket içi Office veya Win Client (diğer bir deyişle, EOS ürünleri dahil) olan müşteriler. Müşterinin 10 veya daha fazla lisansı vardır. Müşterinin bir eğilimini puanı vardır. İş ortakları, M365 dönüştürmesi için hedeflemelidir.|
|CLAS eğilimini-<10 lisanslarıyla uzak Iş-şirket içi alımı (EOS) etkinleştirin|EOS şirket içi Office veya Win Client (diğer bir deyişle, EOS ürünleri dahil) olan müşteriler. Müşterinin 10 ' dan az lisansı vardır. Müşterinin bir eğilimini puanı vardır. İş ortakları, M365 dönüştürmesi için hedeflemelidir.|
|CLAS eğilimini-+ 10 lisansı olmadan uzak Iş-şirket içi alımı (EOS) etkinleştir| Geçerli şirket içi Office veya Win Client (diğer bir deyişle, EOS ürünleriyle önceki ve dahil olan sürümler) içeren müşteri. Müşterinin 10 veya daha fazla lisansı vardır. Müşterinin eğilimini puanı yok. İş ortakları, M365 dönüştürmesi için hedeflemelidir.|
|Eğilimini-<10 lisansı olmadan uzak Iş-şirket içi alımı (EOS) etkinleştir| Geçerli şirket içi Office veya Win Client (diğer bir deyişle, EOS ürünleriyle önceki ve dahil olan sürümler) içeren müşteri. Müşterinin 10 ' dan az lisansı vardır. Müşterinin eğilimini puanı yok. İş ortakları, M365 dönüştürmesi için hedeflemelidir.|
|M365 için uzak Iş-yüksek eğilimini aday özelliğini etkinleştir (Şimdi davran/değerlendir)| M365 için yüksek eğilimini aday aday müşteri.|
|M365 ile uzak çalışma-rekabet (yakınlaştırma) özelliğini etkinleştirme| Zoom ve M365 ile müşteriler, takımlara dönüştürme hedefi|
|M365 olmadan uzak çalışma-rekabet (yakınlaştırma) özelliğini etkinleştir|  Yakınlaştırılmış olan müşteriler, takımlara dönüştürme hedefi|
|M365 E5 için hedeflenen maliyeti ve yönetimi-M365 E3 'i azaltma| M365 E3 ile mevcut müşteri, M365 E5 için hedef|
|M365 BP için hedeflenen maliyeti ve yönetimi-M365 BB ve BS müşterilerini azaltma|    Mevcut M365 BB ve BS müşterileri, bunları M365 BP için hedefleyin|
|Kuruluş üretkenliğini dönüştürme-Surface eğilimini|    Müşteri, yüzey için eğilimini gösteriyor.|
|M365Cluster|M365 satın almak için müşterinin eğilimini tanımlar.  Şimdi davran ve değerlendir, daha yüksek bir verim üretebilecekleri için hedeflenmelidir.  Daha önce yalnızca hedefleme ve müşterileri değerlendirme sonrasında hala kapasite olup olmadığını hedefleyen müşterileri yalnızca hedefleyerek hedeflemelidir.|
|M365Fit|   Firmografları tanımlayan iç ve dış veri noktaları. Kullanım Puanlama, müşterileri karşılaştırmak için en iyi SMB 'ye benzer bir model kullanır ve Microsoft Bulut ürünlere yönelik potansiyel bir uyum olup olmadığını görür. Skor, üç aylık olarak güncelleştirilir.|
|M365Intent|    Sosyal medya ve müşterinin çevrimiçi davranışı ile ilgili sinyaller amaç tanımlar. Amaç Puanlama, kümeleri tanımlamak için sığacak kadar yer alır. Amaç Puanlama aylık olarak güncelleştirilir.|
|SurfaceCluster|    Bu, bir kümeye sığdırma ve amaç önerilerini birleştirerek müşterinin yüzeyini satın almak için eğilimini belirler.  Şimdi davran ve değerlendir, daha yüksek bir verim üretebilecekleri için hedeflenmelidir.  Daha önce yalnızca hedefleme ve müşterileri değerlendirme sonrasında hala kapasite olup olmadığını hedefleyen müşterileri yalnızca hedefleyerek hedeflemelidir.|
|Surçok yönlü sığdırma|    Firmografları tanımlayan iç ve dış veri noktaları. Kullanım Puanlama, müşterileri karşılaştırmak için en iyi SMB 'ye benzer bir model kullanır ve Microsoft Bulut ürünlere yönelik potansiyel bir uyum olup olmadığını görür. Skor, üç aylık olarak güncelleştirilir.|
|Surçok yönlü amaç| Sosyal medya ve müşterinin çevrimiçi davranışı ile ilgili sinyaller amaç tanımlar. Amaç Puanlama, kümeleri tanımlamak için sığacak kadar yer alır. Amaç Puanlama aylık olarak güncelleştirilir.|
|O365Cluster|   Bu, O365 satın almak için müşterinin eğilimini belirler.  Şimdi davran ve değerlendir, daha yüksek bir verim üretebilecekleri için hedeflenmelidir.  Daha önce yalnızca hedefleme ve müşterileri değerlendirme sonrasında hala kapasite olup olmadığını hedefleyen müşterileri yalnızca hedefleyerek hedeflemelidir.|
|O365Fit|   Firmografları tanımlayan iç ve dış veri noktaları. Kullanım Puanlama, müşterileri karşılaştırmak için en iyi SMB 'ye benzer bir model kullanır ve Microsoft Bulut ürünlere yönelik potansiyel bir uyum olup olmadığını görür. Skor, üç aylık olarak güncelleştirilir.|
|O365Intent|    Sosyal medya ve müşterinin çevrimiçi davranışı ile ilgili sinyaller amaç tanımlar. Amaç Puanlama, kümeleri tanımlamak için sığacak kadar yer alır. Amaç Puanlama aylık olarak güncelleştirilir.|
|M365UpsellCustomer|    Bu, müşterinin M365 için upsateğilimini gösteriyor olup olmadığını belirler|
|Google 'a sahiptir|    Bu bayrak, bir müşterinin sahip olduğu Google ürünleri için rekabet sinyalleri göstermesini belirler|
|AWS 'ye sahip|   Bu bayrak, bir müşterinin sahip olduğu AWS ürünlerinin rekabet sinyallerini göstermesini belirler|
|EA 'ya sahiptir|    Bu, bir yenilemenin kurumsal anlaşma (EA) veya EA aboneliği olup olmadığını belirler|
|Açık|  Bu, bir yenilemenin açık veya açık değer anlaşması olduğunu belirler|

**Cloud Ascent-D365 eğilimini**: Cloud Ascent-D365 eğilimini raporunun çeşitli alanlarının veri tanımları şunlardır:

| **Sütun adı** | **Veri açıklaması** |
|---------|:---------|
|MPN Kimliği|    Microsoft İş Ortağı Ağı KIMLIĞI|
|İş ortağı adı|  Ortağın adı|
|Müşteri Kimliği|   Müşteri tanımlayıcı numarası |
|DYENIDEN sayı|   Dun & Bradstreet, eğilimini için puanlanmış müşterinin numarası|
|Hesap Adı|  Hesap adı |
|Etki alanı|    Hesabın etki alanı|
|Kuruluş boyutu|  Kuruluşun boyutu|
|Sektör|  Sektör  |
|Dikey|  Microsoft ve diğer sektör standartları (D&B) tarafından tanımlandığı şekilde eğilimini için puanlanmakta olan müşterinin dikey
|Alan|  Konumun coğrafi alanı|
|Yan Kuruluş|    Eğilimini için puanlanmakta olan müşterinin yan kuruluşu|
|Sales Territory|   Sales Territory|
|Şehir|  Coğrafi şehir konumu |
|Durum| Coğrafi durum konumu|
|Posta Kodu|   Posta Kodu|
|Ülke|   Coğrafi ülke konumu |
|Segment|   Pazar segmenti |
|Alt kesim|   Pazar alt segmenti |
|SMC tür Özeti|  Müşterinin kategorisi: En Iyi yönetilmeyen Kullanıcı temelleri 300 ' e kadar çalışan müşteriler, en fazla yönetilmeyen Işlem tabanı ise, Azure 3 yıllık potansiyel olarak $10.000 olan müşterilerimiz, orta ölçekli işletmeler ise 25 ' ten az çalışanı olan müşterilerimiz|
|En iyi yönetilmeyen Işlem tabanı   |En çok yönetilmeyen müşteriler – işlem|
|En çok yönetilmeyen-kullanıcı tabanı| En çok yönetilmeyen müşteriler – kullanıcılar|
|Iskar dışı|   Kar dışı veya kar için (Evet/Hayır)|
|Dijital satışı etkinleştir-M365-koltuk boyutu >= 25 koltuk (SalesPro eğilimini model)|   D365 olmadan müşteri. Koltuk boyutu: 25 +. İş ortakları D365 SalesPro 'nun çapraz satışı için hedeflemelidir|
|Dijital satışı etkinleştirin-D365 SalesPro eğilimini (Şimdi davran/değerlendir) |D365 olmayan yüksek eğilimini müşterileri.  İş ortakları D365 SalesPro için hedeflemelidir.|
|Finans riskini yönetme & sahtekarlık-Dynamics şirket içi Install Base-Navision (BC eğilimini model)|Onpreb Navision ile mevcut müşteri.  İş ortağı D365 BC için hedeflemelidir|
|Finans riskini yönetme & sahtekarlık-Dynamics on-Prem Install Base-AX (F&O eğilimini model)    |Onpreb AX 'e sahip mevcut müşteri.  İş ortağı D365 F&O için hedeflemelidir|
|Finans riskini yönetme & sahtekarlık-Dynamics on-The-Pre-Install Base-Great Plains (BC eğilimini model)|  Onpred Great Plains 'e sahip mevcut müşteri.  İş ortağı D365 BC için hedeflemelidir|
|Finans riskini yönetme & sahtekarlık-Dynamics şirket içi Install Base-Solomon (BC eğilimini model)|Onpred Solomon ile mevcut müşteri.  İş ortağı D365 BC için hedeflemelidir|
|Finans riskini yönetme & sahtekarlık-Dynamics şirket içi yüklemesi-diğerleri (BC eğilimini model) |Yukarıda listelenmeyen diğer Onpred çözümlerine sahip mevcut müşteri.  İş ortağı D365 BC için hedeflemelidir|
|Çevik Iş süreçleri oluşturma-Dynamics on-Prea Install Base-AX/GP/SL/NAV/diğer (D365 eğilimini model)|   Çevik Iş süreçleri oluşturma-Dynamics on-Prea Install Base-AX/GP/SL/NAV/diğer (D365 eğilimini model)|
|Çevik Iş süreçleri oluşturma-Dynamics rekabet tabanı-mendix/OutSystems/Salesforce (D365 eğilimini model)| Çevik Iş süreçleri oluşturma-Dynamics rekabet tabanı-mendix/OutSystems/Salesforce (D365 eğilimini model)|
|Çevik Iş süreçleri oluşturma-D365 F&O Install Base |Var olan D365 F&O müşterileri.  Hedef güç uygulamalarına yönelik iş ortağı.|
|Çevik Iş süreçleri oluşturma-D365 BC Install Base| Mevcut D365 BC müşterileri. Hedef güç uygulamalarına yönelik iş ortağı.|
|Çevik Iş süreçleri oluşturma-D365 CE Install Base| Mevcut D365 CE müşterileri. Hedef güç uygulamalarına yönelik iş ortağı.|
|Dayanıklı bir tedarik zinciri oluşturma-Oracle dışı/SAP ERP müşterileri ile Ilk D365 Iş yükünü D365 tedarik zinciri olarak Win ve etkinleştirin|  D365 tedarik zinciri için hedeflenen müşteriler.|
|Mevcut D365 CE müşterilerine dayanıklı bir tedarik zinciri ve çapraz satış D365 tedarik zinciri ve/veya perakende/ticaret oluşturun |Şirketler arası D365 tedarik zinciri için hedeflenecek mevcut D365 CE müşterileri|
|Dayanıklı bir tedarik zinciri oluşturun-çapraz satış D365 SUP oluşturun. D365 CE ve (Oracle veya SAP) zinciri ve/veya perakende/ticaret| D365 tedarik zinciri için hedeflemek üzere Oracle veya SAP ile mevcut D365 CE müşterileri|
|D365BCCluster| Bu, D365 Business Central satın almak için müşterinin eğilimini tanımlar.  BC için eğilimini gösteren müşteriler orta ve küçük kategorilerde olacaktır.  Şimdi davran ve değerlendir, daha yüksek bir verim üretebilecekleri için hedeflenmelidir.  Daha önce yalnızca hedefleme ve müşterileri değerlendirme sonrasında hala kapasite olup olmadığını hedefleyen müşterileri yalnızca hedefleyerek hedeflemelidir.|
|D365BCFit| Firmografları tanımlayan iç ve dış veri noktaları. Kullanım Puanlama, müşterileri karşılaştırmak için en iyi SMB 'ye benzer bir model kullanır ve Microsoft Bulut ürünlere yönelik potansiyel bir uyum olup olmadığını görür. Skor, üç aylık olarak güncelleştirilir.|
|D365BCIntent|  Sosyal medya ve müşterinin çevrimiçi davranışı ile ilgili sinyaller amaç tanımlar. Amaç Puanlama, kümeleri tanımlamak için sığacak kadar yer alır. Amaç Puanlama aylık olarak güncelleştirilir.|
|D365FOCluster| Bu, D365 finans ve Işlemlerini satın almak için müşterinin eğilimini belirler.  F&O için eğilimini gösteren müşteriler, en üstteki yönetilmeyen kategorilerde yer alacak. Şimdi davran ve değerlendir, daha yüksek bir verim üretebilecekleri için hedeflenmelidir.  Daha önce yalnızca hedefleme ve müşterileri değerlendirme sonrasında hala kapasite olup olmadığını hedefleyen müşterileri yalnızca hedefleyerek hedeflemelidir.|
|D365FOFit| Firmografları tanımlayan iç ve dış veri noktaları. Kullanım Puanlama, müşterileri karşılaştırmak için en iyi SMB 'ye benzer bir model kullanır ve Microsoft Bulut ürünlere yönelik potansiyel bir uyum olup olmadığını görür. Skor, üç aylık olarak güncelleştirilir.|
|D365FOIntent|  Sosyal medya ve müşterinin çevrimiçi davranışı ile ilgili sinyaller amaç tanımlar. Amaç Puanlama, kümeleri tanımlamak için sığacak kadar yer alır. Amaç Puanlama aylık olarak güncelleştirilir.|
|D365CECluster| Bu, D365 müşteri katılımı satın almak için müşterinin eğilimini belirler.  CE için eğilimini gösteren müşteriler orta ve küçük kategorilerde olacaktır.  Şimdi davran ve değerlendir, daha yüksek bir verim üretebilecekleri için hedeflenmelidir.  Daha önce yalnızca hedefleme ve müşterileri değerlendirme sonrasında hala kapasite olup olmadığını hedefleyen müşterileri yalnızca hedefleyerek hedeflemelidir.|
|D365CEFit| D365 CE 'ye Sığdır|
|D365CEIntent|  D365 CE için amaç|
|DynamicsOnPremAXorCRM_HasOpenRenewal|  Bu, bir müşterinin Dynamics şirket içi AX veya CRM için açık bir yenilemeye sahip olup olmadığını belirler.|
|M365UpsellCustomer|    Bu, müşterinin M365 için upsateğilimini gösteriyor olup olmadığını belirler|
|Google 'a sahiptir|    Bu bayrak, bir müşterinin sahip olduğu Google ürünleri için rekabet sinyalleri göstermesini belirler|
|AWS 'ye sahip|   Bu bayrak, bir müşterinin sahip olduğu AWS ürünlerinin rekabet sinyallerini göstermesini belirler|
|EA 'ya sahiptir |Bu, bir yenilemenin kurumsal anlaşma (EA) veya EA aboneliği olup olmadığını belirler|
|Açık|  Bu, bir yenilemenin açık veya açık değer anlaşması olduğunu belirler|

**Cloud Ascent-Azure eğilimini**: Cloud Ascent-Azure eğilimini raporunun çeşitli alanlarının veri tanımları şunlardır:

|**Sütun adı** |**Veri açıklaması** |
|---------|:---------|
|MPN Kimliği|    Microsoft İş Ortağı Ağı KIMLIĞI|
|İş ortağı adı|  Ortağın adı|
|Müşteri Kimliği|   Müşteri tanımlayıcı numarası |
|DYENIDEN sayı|   Dun & Bradstreet, eğilimini için puanlanmış müşterinin numarası|
|Hesap Adı|  Hesap adı |
|Etki alanı|    Hesabın etki alanı|
|Kuruluş boyutu|  Kuruluşun boyutu|
|Sektör|  Sektör  |
|Dikey|  Microsoft ve diğer sektör standartları (D&B) tarafından tanımlandığı şekilde eğilimini için puanlanmakta olan müşterinin dikey|
|Alan|  Konumun coğrafi alanı|
|Yan Kuruluş|    Eğilimini için puanlanmakta olan müşterinin yan kuruluşu|
|Sales Territory|   Sales Territory|
|Şehir|  Coğrafi şehir konumu |
|Durum| Coğrafi durum konumu|
|Posta Kodu|   Posta Kodu|
|Ülke|   Coğrafi ülke konumu |
|Segment|   Pazar segmenti |
|Alt kesim|   Pazar alt segmenti |
|SMC tür Özeti|  SMC türü |
|En iyi yönetilmeyen Işlem tabanı|  En çok yönetilmeyen müşteriler – işlem|
|En çok yönetilmeyen-kullanıcı tabanı| En çok yönetilmeyen müşteriler – kullanıcılar|
|Iskar dışı|   Kar dışı veya kar için (Evet/Hayır)|
|Migrate-EOS Win Server-EOS Windows Server ıB with CLAS eğilimini-5 + lisansları|   Şirket içi Win Server (diğer bir deyişle, EOS ürünleriyle önceki ve dahil olan sürümler) olan müşteri. Müşterinin 5 veya daha fazla lisansı vardır. Eğilimini puanı olan müşteri.  İş ortakları, bu müşterileri Azure 'a geçiş için hedeflemelidir.|
|Migrate-EOS Win Server-EOS Windows Server ıB, CLAS eğilimini-<5 lisanslarıyla|   EOS (hizmet sonu) Şirket içi Win Server (diğer bir deyişle, EOS ürünleriyle önceki ve dahil olan sürümler) olan müşteri. Müşterinin 5 ' ten az lisansı vardır. Eğilimini puanı olan müşteri.  İş ortakları, bu müşterileri Azure 'a geçiş için hedeflemelidir.|
|Migrate-EOS Win Server-EOS Windows Server ıB, CLAS eğilimini-5 + lisansı olmadan |Şirket içi Win Server (diğer bir deyişle, EOS ürünleriyle önceki ve dahil olan sürümler) olan müşteri. Müşterinin 5 ' ten fazla lisansı vardır. Müşterinin eğilimini puanı yok. İş ortakları, bu müşterileri Azure 'a geçiş için hedeflemelidir.|
|Migrate-EOS Win Server-EOS Windows Server ıB, CLAS eğilimini-<5 lisansı olmadan|    Şirket içi Win Server (diğer bir deyişle, EOS ürünleriyle önceki ve dahil olan sürümler) olan müşteri. 5 ' ten az lisansa sahiptir. Müşterinin eğilimini puanı yok. İş ortakları, bu müşterileri Azure 'a geçiş için hedeflemelidir.|
|CLAS eğilimini-5 + lisanslarıyla geçiş-EOS SQL-EOS SQL Server ıB|  Şirket içi SQL Server (diğer bir deyişle, EOS ürünleriyle önceki ve dahil olan sürümler) sahip olan müşteri. Müşterinin 5 ve lisansı vardır. Müşterinin bir eğilimini puanı vardır.  İş ortakları, bu müşterileri Azure 'a geçiş için hedeflemelidir.|
|CLAS eğilimini-<5 lisanslarıyla geçiş-EOS SQL-EOS SQL Server ıB|  Şirket içi SQL Server (diğer bir deyişle, EOS ürünleriyle önceki ve dahil olan sürümler) sahip olan müşteri. 5 ' ten az lisansa sahiptir. Eğilimini puanı olan müşteri. İş ortakları, bu müşterileri Azure 'a geçiş için hedeflemelidir.|
|CLAS eğilimini-5 + lisansı olmadan geçiş-EOS SQL-EOS SQL Server ıB|   Şirket içi SQL Server (diğer bir deyişle, EOS ürünleriyle önceki ve dahil olan sürümler) sahip olan müşteri. Müşterinin 5 veya daha fazla lisansı vardır. Müşterinin eğilimini puanı yok. İş ortakları, bu müşterileri Azure 'a geçiş için hedeflemelidir.|
|<eğilimini 5 lisansı olmadan geçiş-EOS SQL-EOS SQL Server ıB|   Şirket içi SQL Server (diğer bir deyişle, EOS ürünleriyle önceki ve dahil olan sürümler) sahip olan müşteri. Müşterinin 5 ' ten az lisansı vardır. Müşterinin eğilimini puanı yok. İş ortakları, bu müşterileri Azure 'a geçiş için hedeflemelidir.|
|Geçiş geçişi-şirket içi Win Server-geçerli Windows Server ıB with CLAS eğilimini-5 + lisansları|   Mevcut şirket içi Win Server (yani, EOS ürünlerinden sonra olan sürümler) olan müşteri. Müşterinin 5 ve lisansı vardır. Müşterinin bir eğilimini puanı vardır. İş ortakları, bu müşterileri Azure 'a geçiş için hedeflemelidir.|
|Geçirme-şirket içi Win Server-geçerli Windows Server ıB, CLAS eğilimini-<5 lisanslarıyla|   Mevcut şirket içi Win Server (yani, EOS ürünlerinden sonra olan sürümler) olan müşteri. Müşterinin 5 ' ten az lisansı vardır. Müşterinin Azure için eğilimini puanı vardır. İş ortakları, bu müşterileri Azure 'a geçiş için hedeflemelidir.|
|Geçiş geçişi-şirket içi Win Server-geçerli Windows Server ıB, CLAS eğilimini-5 ve lisans olmadan|    Mevcut şirket içi Win Server (yani, EOS ürünlerinden sonra olan sürümler) olan müşteri. Müşterinin 5 ve lisansı vardır. Müşterinin eğilimini puanı yok. İş ortakları, bu müşterileri Azure 'a geçiş için hedeflemelidir.|
|Geçirme-şirket içi Win Server-geçerli Windows Server ıB, CLAS eğilimini-<5 lisansı olmadan |Mevcut şirket içi Win Server (yani, EOS ürünlerinden sonra olan sürümler) olan müşteri. Müşterinin 5 ' ten az lisansı vardır. Müşterinin eğilimini puanı yok. İş ortakları, bu müşterileri Azure 'a geçiş için hedeflemelidir.|
|Geçiş-Azure SQL veya SQL VM 'lerine geçiş-geçerli SQL Server IB ile CLAS eğilimini-5 + lisansları|  Geçerli şirket içi SQL Server (yani, EOS ürünlerinden sonra olan sürümler) sahip olan müşteri. Müşterinin 5 ve lisansı vardır. Müşterinin bir eğilimini puanı vardır. İş ortakları, bu müşterileri Azure 'a geçiş için hedeflemelidir.|
|Geçiş-Azure SQL veya SQL VM 'lerine geçiş-geçerli SQL Server IB ile CLAS eğilimini-<5 Lisansı|  Geçerli şirket içi SQL Server (yani, EOS ürünlerinden sonra olan sürümler) sahip olan müşteri. Müşterinin 5 ' ten az lisansı vardır. Müşterinin bir eğilimini puanı vardır. İş ortakları, bu müşterileri Azure 'a geçiş için hedeflemelidir.|
|Geçiş-Azure SQL veya SQL VM 'lerine geçiş-geçerli SQL Server, CLAS eğilimini-5 ve lisans olmadan|   Geçerli şirket içi SQL Server (yani, EOS ürünlerinden sonra olan sürümler) sahip olan müşteri. Müşterinin 5 ve lisansı vardır. Müşterinin eğilimini puanı yok. İş ortakları, bu müşterileri Azure 'a geçiş için hedeflemelidir.|
|Geçiş-Azure SQL veya SQL VM 'lerine geçiş-geçerli SQL Server, CLAS eğilimini-<5 lisansı olmadan|   Geçerli şirket içi SQL Server (yani, EOS ürünlerinden sonra olan sürümler) sahip olan müşteri. Müşterinin 5 ' ten az lisansı vardır. Müşterinin eğilimini puanı yok. İş ortakları, bu müşterileri Azure 'a geçiş için hedeflemelidir.|
|Geçirme-OSS-OSS DB 'ye geçiş| Aşağıdaki yarışmaya sahip ürünlerden birini içeren mevcut müşteri: PostgreSQL, MySQL, MariaDB. İş ortakları, bu müşterileri Azure 'a geçiş için hedeflemelidir.|
|Azure 'da-OSS-Linux geçirme |Ürüne sahip mevcut müşteri: Linux. İş ortakları, bu müşterileri Azure 'a geçiş için hedeflemelidir.|
|Azure 'da geçiş-SAP-SAP|  Ürüne sahip mevcut müşteri: SAP. İş ortakları, bu müşterileri Azure 'a geçiş için hedeflemelidir.|
|Geçir-WVD-RDS ıB |Etkin Windows Uzak Masaüstü Hizmetleri olan müşterileri tanımlar. İş ortakları, bu müşterileri Azure 'a geçiş için hedeflemelidir.|
|Migrate-WVD-modern Işleri Azure 'a/WVD 'a çapraz satış|   M365 ile müşterileri tanımlar ve Azure 'a sahip değildir. İş ortakları, bu müşterileri Azure 'a geçiş için hedeflemelidir.|
|Geçiş-VMware ıB|   Ürüne sahip mevcut müşteri: VMware. İş ortakları, bu müşterileri Azure 'a geçiş için hedeflemelidir.|
|Geçiş-Citrix ıB|   Ürüne sahip mevcut müşteri: Citrix Systems. İş ortakları, bu müşterileri Azure 'a geçiş için hedeflemelidir.|
|Yenilik yapın-Analytics-Power BI ıB w/High Azure eğilimini|   Power BI abonelik içeren ve etkin olan müşteriler: Power BI-tek başına Pro, Power BI-Azure paketleri, Power BI-Office paketleri, Power BI paketleri-M365|
|GitHub ile DevOps 'u etkinleştirme-VisualStudio/MSDN ıB|    Etkin Visual Studios ile tanımlanmış müşteriler|
|Win Server standart sürümü|   Bu, müşteri tarafından Windows Server Standart satın alımlarınızın sürümünü gösterir|
|Win Server Standart lisansı|   Bu, müşteri tarafından Windows Server Standart satın alımlarınızın lisans türünü gösterir|
|Win Server veri merkezi sürümü|    Bu, müşteri tarafından Windows veri merkezi satın alımlarınızın sürümünü gösterir|
|Win Server veri merkezi lisansı| Bu, müşteri tarafından Windows veri merkezi satın alımlarınızın lisans türünü gösterir|
|AzureFit|  Firmografları tanımlayan iç ve dış veri noktaları. Kullanım Puanlama, müşterileri karşılaştırmak için en iyi SMB 'ye benzer bir model kullanır ve Microsoft Bulut ürünlere yönelik potansiyel bir uyum olup olmadığını görür. Skor, üç aylık olarak güncelleştirilir.|
|AzureIntent|   Sosyal medya ve müşterinin çevrimiçi davranışı ile ilgili sinyaller amaç tanımlar. Amaç Puanlama, kümeleri tanımlamak için sığacak kadar yer alır. Amaç Puanlama aylık olarak güncelleştirilir.|
|AzureCluster|  Bu, bir kümeye sığdırma ve amaç önerilerini birleştirerek müşterinin Azure satın alma eğilimini tanımlar.  Şimdi davran ve değerlendir, daha yüksek bir verim üretebilecekleri için hedeflenmelidir.  Daha önce yalnızca hedefleme ve müşterileri değerlendirme sonrasında hala kapasite olup olmadığını hedefleyen müşterileri yalnızca hedefleyerek hedeflemelidir.|
|WindowsServerDataCenter_HasOpenRenewal|    Bu, bir müşterinin Windows Server veri merkezi için açık bir yenilemeye sahip olup olmadığını belirler|
|WindowsServerStandard_HasOpenRenewal|  Bu, bir müşterinin Windows Server Standard için açık yenileme olup olmadığını belirler|
|AzureUpsellCustomer|   Bu, müşterinin Azure için upsateğilimini gösteriyor olup olmadığını belirler|
|Google 'a sahiptir|    Bu bayrak, bir müşterinin sahip olduğu Google ürünleri için rekabet sinyalleri göstermesini belirler|
|AWS 'ye sahip|   Bu bayrak, bir müşterinin sahip olduğu AWS ürünlerinin rekabet sinyallerini göstermesini belirler|
|EA 'ya sahiptir |Bu, bir yenilemenin kurumsal anlaşma (EA) veya EA aboneliği olup olmadığını belirler|
|Açık|  Bu, bir yenilemenin açık veya açık değer anlaşması olduğunu belirler|

**Bulut Ascent-Agreement yenilemeleri eğilimini**: bulut yokuş-anlaşma yenilemeler eğilimini raporunun çeşitli alanlarının veri tanımları şunlardır:

|**Sütun adı** |**Veri açıklaması** |
|---------|:---------|
|MPN Kimliği|    Microsoft İş Ortağı Ağı KIMLIĞI|
|İş ortağı adı|  Ortağın adı|
|Müşteri Kimliği|   Müşteri tanımlayıcı numarası |
|DYENIDEN sayı|   Dun & Bradstreet, eğilimini için puanlanmış müşterinin numarası|
|Hesap Adı|  Hesap adı |
|Etki alanı|    Hesabın etki alanı|
|Kuruluş boyutu|  Kuruluşun boyutu|
|Sektör|  Sektör  |
|Dikey|  Microsoft ve diğer sektör standartları (D&B) tarafından tanımlandığı şekilde eğilimini için puanlanmakta olan müşterinin dikey|
|Alan|  Konumun coğrafi alanı|
|Yan Kuruluş|    Eğilimini için puanlanmakta olan müşterinin yan kuruluşu|
|Sales Territory|   Sales Territory|
|Şehir|  Coğrafi şehir konumu |
|Durum| Coğrafi durum konumu|
|Posta Kodu|   Posta Kodu|
|Ülke|   Coğrafi ülke konumu |
|Segment|   Pazar segmenti |
|Alt kesim|   Pazar alt segmenti |
|SMC tür Özeti|  SMC türü |
|En iyi yönetilmeyen Işlem tabanı|  En çok yönetilmeyen müşteriler – işlem|
|En çok yönetilmeyen-kullanıcı tabanı| En çok yönetilmeyen müşteriler – kullanıcılar|
|Iskar dışı|Kar dışı veya kar için (Evet/Hayır)|
|Google 'a sahiptir|Bu bayrak, bir müşterinin sahip olduğu AWS ürünlerinin rekabet sinyallerini göstermesini belirler|
|AWS 'ye sahip|Bu bayrak, bir müşterinin sahip olduğu AWS ürünlerinin rekabet sinyallerini göstermesini belirler|
|Azure kümesi|Bu, Azure 'ı satın almak için müşterinin eğilimini tanımlar.  Şimdi davran ve değerlendir, daha yüksek bir verim üretebilecekleri için hedeflenmelidir.  Daha önce yalnızca hedefleme ve müşterileri değerlendirme sonrasında hala kapasite olup olmadığını hedefleyen müşterileri yalnızca hedefleyerek hedeflemelidir.|
|D365 F&O kümesi|  Bu, D365 finans ve Işlemlerini satın almak için müşterinin eğilimini belirler.  F&O için eğilimini gösteren müşteriler, en üstteki yönetilmeyen kategorilerde yer alacak.  Şimdi davran ve değerlendir, daha yüksek bir verim üretebilecekleri için hedeflenmelidir.  Daha önce yalnızca hedefleme ve müşterileri değerlendirme sonrasında hala kapasite olup olmadığını hedefleyen müşterileri yalnızca hedefleyerek hedeflemelidir.|
|D365 CE kümesi|   Bu, D365 müşteri katılımı satın almak için müşterinin eğilimini belirler.  CE için eğilimini gösteren müşteriler orta ve küçük kategorilerde olacaktır.  Şimdi davran ve değerlendir, daha yüksek bir verim üretebilecekleri için hedeflenmelidir.  Daha önce yalnızca hedefleme ve müşterileri değerlendirme sonrasında hala kapasite olup olmadığını hedefleyen müşterileri yalnızca hedefleyerek hedeflemelidir.|
|D365 BC kümesi|   Bu, D365 Business Central satın almak için müşterinin eğilimini tanımlar.  BC için eğilimini gösteren müşteriler orta ve küçük kategorilerde olacaktır.  Şimdi davran ve değerlendir, daha yüksek bir verim üretebilecekleri için hedeflenmelidir.  Daha önce yalnızca hedefleme ve müşterileri değerlendirme sonrasında hala kapasite olup olmadığını hedefleyen müşterileri yalnızca hedefleyerek hedeflemelidir.|
|M365 kümesi|  Bu, M365 satın almak için müşterinin eğilimini tanımlar.  Şimdi davran ve değerlendir, daha yüksek bir verim üretebilecekleri için hedeflenmelidir.  Daha önce yalnızca hedefleme ve müşterileri değerlendirme sonrasında hala kapasite olup olmadığını hedefleyen müşterileri yalnızca hedefleyerek hedeflemelidir.|
|Lisans programı|   Bu, yenileme için lisans programı türünü tanımlar|
|Anlaşma KIMLIĞI|  Anlaşma tanımlayıcısı|
|Anlaşma bitiş tarihi|    Anlaşma bitiş tarihi |
|Sona erme türü|   Süre sonu türü|
|Süresi dolan gelir|  Süresi dolan aboneliklerle ilişkili gelir|
|EA 'ya sahiptir|    Bu, bir yenilemenin kurumsal anlaşma (EA) veya EA aboneliği olup olmadığını belirler|
|Açık|  Bu, bir yenilemenin açık veya açık değer anlaşması olduğunu belirler|
|Azure büyük satış müşterisi| Bu, müşterinin Azure için upsateğilimini gösteriyor olup olmadığını belirler|
|M365 Upsata müşterisi|  Bu, müşterinin M365 için upsateğilimini gösteriyor olup olmadığını belirler|
|RevSumDivisionName|    Bu, yenilemeye yönelik ürünü tanımlar|

## <a name="next-steps"></a>Sonraki adımlar

Raporlar için bkz. [raporları indirme](pci-download-reports.md).
