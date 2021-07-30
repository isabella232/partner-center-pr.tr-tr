---
title: İçgörü verilerinin tanımları
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Belgede çeşitli raporlar ve bunların veri tanımları listelenmiş ve rapor indirme sayfasından Analizler indirebilirsiniz.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 92733f11713e8c16d607a51ef00efdcc25ddc855
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114843417"
---
# <a name="export--data-definitions"></a>Dışarı Aktarma – Veri tanımları 

**Uygun roller:** Rapor görüntüleyici | Yönetici raporu görüntüleyicisi

## <a name="introduction"></a>Giriş 

Panoda Raporları İndir hub'ını Analizler ham veri kümelerini dışarı aktarabilirsiniz. 

Veri tanımlarıyla birlikte indirebilirsiniz çeşitli raporlar aşağıdaki tablolarda listelenmiştir: 

### <a name="partner-profile-report"></a>**İş ortağı profili raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| MPNId | Microsoft İş Ortağı Ağı (MPN) Kimliği| 
| PartnerName | İş ortağının adı | 
| PGA_MPNId | İş ortağı genel hesabı MPN'lerinin tanımlayıcısı | 
| PGA_PartnerName | İş ortağı genel hesap adı | 
| Şehir | İş ortağının şehir konumu | 
| Ülke | İş ortağının ülke konumu | 
| HierarchyLevel | Genel MPN Kimliği mi yoksa konum MPN Kimliği mi olduğunu gösterir | 

### <a name="customer-details-report"></a>**Müşteri ayrıntıları raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| PGAMpnId| İş ortağı genel hesabı MPN'lerinin tanımlayıcısı|
| CustomerName| Müşterinin adı|
| CustomerTenantId| Müşteri kiracısı tanımlayıcısı|
| CustomerTpid| Müşterinin üst üst öğenin tanımlayıcısı|
| DUNSNumber|   Müşterinin Genel Veri Evrensel Sayı Sistem Tanımlayıcısı|
| CustomerSegment | Müşteri segmenti|
| TopSegment    | Müşterinin üst düzey segment sınıflandırması|
| CustomerMarket|   Müşterinin coğrafi pazar|  
| CustomerStatus    | Müşteri Durumu (Etkin veya Etkin Değil)| 
| CustomerTenantName|   Müşteri kiracısı adı|
| CustomerTenantCountry|    Müşteri kiracısı ülkesi|
| TenantDomainName| Müşteri kiracısı etki alanı adı|
| Ürün|  MÜŞTERIYE MPN tarafından satılan ürün: O365, Dynamics 365, Enterprise Mobility + Security, Power BI veya Microsoft Azure.|
| RawProductName|   Müşteriye satılan ayrıntılı ürün adı|
| SKU|  Ürün SKU'su|
| Ay|    Kullanım ve gelirin raporlandığı ay|
| MPNId|    Microsoft İş Ortağı Ağı (MPN) tanımlayıcısı|
| PartnerName|  İş ortağının adı|
| PartnerLocation|  İş ortağının coğrafi konumu|
| PartnerAttributionType|   İş ortağının atfı| 
| SalesChannel| Satış Kanalı|
| IsDuplicateRowForPGA| Tek bir PGA altındaki birden çok iş ortağı atıbetleri için bu değer yalnızca bir MPNId için 0 olarak ayarlanır. Değer 1 olarak ayarlanırsa yinelenen bir satır gösterir|
| AvailableSeats|   Kullanılabilir yer|
| BilledRevenueUSD| ABD doları olarak faturalandır edilen gelir|
| AzureConsumedRevenueUSD|  Azure Tüketim Geliri ABD doları|

### <a name="reseller-performance-report"></a>**Kurumsal bayi performans raporu**

> [!Note]
> Gelir ve Azure tüketilen gelir (ACR) verileri yalnızca Yönetici raporu görüntüleyicisi olan kullanıcılar tarafından kullanılabilir.

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| PGAMpnId | İş ortağı genel hesabı MPN'lerinin tanımlayıcısı |
| ResellerMPNid | Kurumsal Microsoft İş Ortağı Ağı tanımlayıcısı | 
| ResellerName | Satıcı adı | 
| ResellerMarket | Satıcı pazarı ülkesi | 
| IndirectProviderMPNId | Dolaylı sağlayıcı iş Microsoft İş Ortağı Ağı | 
| IndirectProviderName | Dolaylı sağlayıcı adı | 
| Ay | Kullanım ve gelirin raporlandığı ay | 
| Ürün | Ürün adı | 
| SubscriptionID | Aboneliğin tanımlayıcısı | 
| AvailableSeats | Kullanılabilir yer sayısı | 
| AssignedSeats | Atanan yer sayısı | 
| BilledRevenueUSD | ABD doları olarak faturalandır edilen gelir | 
| CustomerName | Müşterinin adı | 
| CustomerTPid | Müşterinin üst üst öğenin tanımlayıcısı | 
| CustomerSegment | Müşteri segmenti | 
| CustomerMarket | Müşterinin coğrafi pazar | 
| ResellerStatus | Kurumsal bayi durumu | 

### <a name="subscription-details-report"></a>**Abonelik ayrıntıları raporu**

>[!Note]
>Gelir ve ACR verileri yalnızca Yönetici raporu görüntüleyicisi olan kullanıcılar tarafından kullanılabilir.

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
|PGAMpnId| İş ortağı genel hesabı MPN'lerinin tanımlayıcısı |
|SubscriptionId | Aboneliğin GUID'si|
|SubscriptionStartDate | Aboneliğin başlangıç tarihi|
|SubscriptionEndDate | Aboneliğin bitiş tarihi|
|SubscriptionState | Aboneliğin durumu (Etkin veya Eskitildi)|
|Ay | Kullanım ve gelirin raporlandığı ay|
|IsAutoRenew | Aboneliğin otomatik yenileme olup olmadığını gösterir (Evet veya Hayır)|
|CustomerName | Müşterinin adı|
|CustomerTenantId | Müşterinin GUID'si|
|CustomerTpid | Müşteri üst üst tanımlayıcısı|
|DUNSNumber| Müşterinin Genel Veri Evrensel Sayı Sistem Tanımlayıcısı|
|CustomerSegment | Müşterinin pazar segmenti|
|TopSegment| Müşterinin üst düzey segment sınıflandırması|
|CustomerMarket | Müşterinin coğrafi pazar|
|ReportingProductName| Ayrıntılı ürün adı|
|Ürün | İş ortağı tarafından müşteriye satılan ürün|
|RawProductName| Müşteriye satılan ayrıntılı ürün adı|
|ProductPartNumber| Ürünün parça numarası|
|SKU | Ürünün SKU'su|
|RevSumDivisionName| Gelir raporlama ürün hiyerarşisi adı|
|SolutionArea| Ürünün iş uygulaması sınıflandırması|
|MPNId | Microsoft İş Ortağı Ağı ortağın kimlik numarası|
|PartnerName | İş ortağının adı|
|PartnerLocation | İş ortağının coğrafi konumu|
|PartnerAttributionType | Abonelik için asıf türü|
|SalesChannel | Satış kanalı - Doğrudan, CSP (Bulut Çözümü Sağlayıcısı) ve diğer|
|PricingLevel| Satışın fiyat noktası|
|EnrollmentNumber| Aboneliğin kayıt numarası|
|IsDuplicateRowForPGA| Tek bir PGA altındaki birden çok iş ortağı atıbetleri için bu değer yalnızca bir MPNId için 0 olarak ayarlanır. Değer 1 olarak ayarlanırsa yinelenen bir satır gösterir|
|SubscriptionStartMonth| Aboneliğin başlangıç ayı|
|ResellerID| Kurumsal bayinin kimliği|
|ResellerName| Satıcı adı|
|AvailableSeatsEOP| Dönem Sonuna Kadar Genel Kullanılabilir yer|
|AvailableSeats | Aya göre kullanılabilir yer farkı|
|BilledRevenueUSD | ABD doları olarak gelir|
|AzureConsumedRevenueUSD| Azure Tüketim Geliri ABD doları|

### <a name="azure-usage-report"></a>**Azure kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
|PGAMpnId| İş ortağı genel hesabı MPN'lerinin tanımlayıcısı|
|SubscriptionId| Aboneliğin GUID'si|
|SubscriptionStartDate| Aboneliğin başlangıç tarihi|
|SubscriptionEndDate| Aboneliğin bitiş tarihi|
|Firijklmnosedate| Önce Azure hizmetlerinin kullanıldığı Tarih|
|SubscriptionState| Aboneliğin geçerli durumu (açık, kapalı etkin veya yetkisiz kullanım süresi)|
|Ay| Aya göre toplanan Tarih|
|ServiceLevel1| Hizmet düzeyi 1 – kapsayıcılar, veritabanları, ağ vb. gibi hizmet pilleriyle eşleşir.|
|ServiceLevel2| Hizmet düzeyi 2 – hizmet pillerinin Iş yüküne karşılık gelir|
|ServiceLevel3| Azure tekliflerini listelerken Azure.Microsoft.Com tarafından kullanılan hizmet adı|
|ServiceLevel4| Hizmet içindeki yüksek düzey özellik kümesi farklılıkları mantıksal gruplandırmaları. Genel Amaçlı sanal makineler, bellek için iyileştirilmiş sanal makineler, tek SQL Veritabanı, elastik SQL Veritabanı vb. |
|ServiceGroup2| AI, uygulama geliştirme, IoT vb. alan gelir sorumluluğu (FRA) alanları |
|ServiceGroup3| IoT Hub gibi FRA için ek ayrıntılar, ıot FRA için Haritalar|
|Serviceetkileyen Şifreleyici| Service Fabric, Azure Databricks, aks vb. gibi ınfra kaynaklarının tüketimini sağlayan paas hizmetleri.|
|ComputeOS| Işlem için işletim sistemi|
|ComputeCoreSoftware| İşlem çekirdek yazılımı|
|UsageUnits| Fatura çevrimi sırasında kullanılan birim sayısı|
|UsageQuantity| Kaynağın kullanım miktarı|
|CustomerName| Müşterinin adı|
|CustomerTenantId| Müşterinin Kiracı kimliği|
|Customertpıd| Müşteri üst üst kimliği|
|CustomerSegment| Müşterinin segmenti|
|CustomerMarket| Müşterinin coğrafi pazarı|
|Mpnıd| Microsoft İş Ortağı Ağı müşterinin kimliği|
|PartnerName| Ortağın adı|
|PartnerLocation| Ortağın coğrafi ülke konumu|
|PartnerAttributionType| Ortağın atısyon türü|
|SalesChannel| Satışın kanalı (doğrudan/CSP, dolaylı/CSP, doğrudan vb.)  |
|Kayıt numarası| Aboneliğin kayıt numarası |
|IsACRDuplicateAtPGALevel| Tek PGA altında birden fazla iş ortağı tanımlayıcısı için, bu değer yalnızca bir MPNId için 0 olarak ayarlanır. Değer 1 olarak ayarlanırsa, yinelenen bir satırı gösterir|
|ResellerID| Satıcı kimliği|
|ResellerName| Satıcı adı|
|AdminType| Iş ortağı Attributıon türü "Iş ortağı yönetici bağlantısı (PAL)" olduğunda, bu sütun müşterinin aboneliğindeki atanmış rolü gösterir.|
|AssociationType| Ilişki türü|
|MonthlySubscriptionLevelACR| Aylık abonelik düzeyi ACR|
|ACR_USD| Azure tüketilen gelir (ACR) ABD Doları cinsinden|

### <a name="office-365-license-usage-report"></a>**Office 365 lisansı kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| Pgampnıd | Ortak küresel hesap MPN tanımlayıcısı | 
| CustomerTenantId | Müşterinin kiracı KIMLIĞI | 
| Customertpıd | Müşteri üst üst KIMLIĞI | 
| WorkloadName | Skype Kurumsal, Teams, Exchange Online | 
| Ay | Kullanımın bildirildiği ay | 
| Paidavvailableunits | Ücretli kullanılabilir birim sayısı | 
| MonthlyActiveUsers | Aylık etkin kullanıcı sayısı | 
| CustomerName | Müşterinin adı | 
| CustomerMarket | Müşterinin pazarına ait coğrafi ülke konumu | 
| CustomerSegment | Müşteri kesimi | 
| Mpnıd | Microsoft İş Ortağı Ağı tanımlayıcısı | 
| PartnerName | Ortağın adı | 
| PartnerLocation | Ortağın coğrafi konumu | 
| PartnerAttributionType | Ortağın atısyon türü | 
| Iduplicaterowforpga | Tek PGA altında birden fazla iş ortağı tanımlayıcısı için, bu değer yalnızca bir MPNId için 0 olarak ayarlanır. Değer 1 olarak ayarlanırsa, yinelenen bir satırı gösterir|

### <a name="enterprise-mobility-license-usage-report"></a>**Enterprise Mobility Lisansı kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| Pgampnıd| Ortak küresel hesap MPN tanımlayıcısı| 
| SubscriptionId | Aboneliğin GUID 'SI| 
| SubscriptionStartDate | Aboneliğin başlangıç tarihi| 
| SubscriptionEndDate | Aboneliğin bitiş tarihi| 
| Abonelik durumu| Aboneliğin geçerli durumu (açık, kapalı, etkin veya yetkisiz kullanım süresi)| 
| Ay | Aya göre toplanan Tarih| 
| SKU| Ürün SKU 'SU| 
| SkuId| Ürünün SKU kimliği| 
| Freevspaıdsku| Ücretsiz veya ücretli SKU 'YU gösterir| 
| SalesModel| Aboneliği satmakta kullanılan satış kanalı| 
| DetailedSalesModel| Abonelik için ayrıntılı satış modeli| 
| CustomerName| Müşterinin adı| 
| CustomerTenantId | Müşterinin Kiracı kimliği| 
| Customertpıd | Müşteri üst üst kimliği| 
| CustomerSegment | Müşteri kesimi| 
| CustomerMarket | Müşterinin pazarında coğrafi ülke konumu| 
| Mpnıd | Microsoft İş Ortağı Ağı KIMLIĞI| 
| PartnerName | Ortağın adı| 
| PartnerLocation | İş ortağının coğrafi konumu| 
| PartnerAttributionType | İş ortağının attributıon türü| 
| İş ortağı hiyerarşisi| İş ortağı hiyerarşisi (sanal kuruluş veya merkez veya konum)| 
| Paidavvailableunits | Ücretli kullanılabilir birim sayısı| 
| MonthlyActiveUsers | Aylık etkin kullanıcı sayısı| 
| AATPActiveUsage| Azure Gelişmiş tehdit koruması (AATP) etkin kullanımı| 
| MCASActiveUsage| MCAS etkin kullanımı| 
| Aadppaidavvailableunits| Azure Active Directory Premium için ücretli kullanılabilir birim sayısı (aadp)| 
| Intunepaidavailableunits| Intune için ücretli kullanılabilir birim sayısı| 
| Azippaidavvailableunits| Azıp için ücretli kullanılabilir birim sayısı| 
| AADPMonthlyActiveUsers| Azure Active Directory Premium için aylık etkin kullanıcı sayısı (aadp)| 
| Intunemonthlyactiveusers| Intune için aylık etkin kullanıcı sayısı| 
| AzipMonthlyActiveUsers| Azıp için aylık etkin kullanıcı sayısı| 
| MDM| MDM| 
| MAM| MAM| 
| SSPR| SSPR| 

### <a name="dynamics-365-license-usage-report"></a>**Dynamics 365 lisans kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| Pgampnıd | Ortak küresel hesap MPN tanımlayıcısı | 
| SubscriptionId | Aboneliğin GUID 'SI | 
| SubscriptionStartDate | Aboneliğin başlangıç tarihi | 
| SubscriptionEndDate | Aboneliğin bitiş tarihi | 
| Abonelik durumu | Aboneliğin durumu | 
| Ay | Kullanımın bildirildiği ay | 
| RevSumDivisionName | Rev Sum bölümünün adı | 
| RevSumCategoryName | Rev Sum kategorisinin adı | 
| SKU | Ürünün SKU 'SU | 
| SkuId | Ürünün SKU KIMLIĞI | 
| Freevspaıdsku | Ücretsiz veya ücretli bir SKU olup olmadığını belirtir | 
| SalesModel | Aboneliğin satışı için kullanılan satış kanalı | 
| DetailedSalesModel | Abonelik için ayrıntılı satış modeli | 
| CustomerName | Müşterinin adı | 
| CustomerTenantId | Müşteri kiracısı GUID'si | 
| CustomerTpid | Müşteri üst üst tanımlayıcısı | 
| CustomerSegment | Müşterinin pazar segmenti | 
| CustomerMarket | Müşterinin coğrafi pazar | 
| MPNId | Kimlik Microsoft İş Ortağı Ağı | 
| PartnerName | İş ortağının adı | 
| PartnerLocation | İş ortağının coğrafi ülke konumu | 
| PartnerAttachType | Abonelik için asıf türü | 
| AvailableSeats |  Geçerli ücretli kullanılabilir yer|
| AssignedSeats |   Geçerli atanan yer|
| ActiveSeats | Geçerli etkin yer sayısı|
| DeploymentOpportunity |   Dağıtım fırsatı, atanmamış olan yer sayısıdır|
| ActiveUsagePercent |  Kullanılabilir yerlerin yüzdesi olarak geçerli etkin kullanım |

### <a name="power-bi-license-usage-report"></a>**Power BI kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| PGAMpnId | İş ortağı genel hesabı MPN'lerinin tanımlayıcısı | 
| SubscriptionId | Aboneliğin GUID'si | 
| SubscriptionStartDate | Aboneliğin başlangıç tarihi | 
| SubscriptionEndDate | Aboneliğin bitiş tarihi | 
| SubscriptionStatus | Aboneliğin durumu (Etkin, Etkin Değil veya Yetkisiz Kullanım Süresi) | 
| Ay | Aya göre toplanan tarih | 
| SKU | Ürünün SKU'su | 
| SKUId | Ürünün SKU kimliği | 
| FreeVsPaidSKU | Ücretsiz veya ücretli SKU farklılaştırıcısı | 
| SalesModel | Aboneliği satmak için kullanılan satış modeli | 
| DetailedSalesModel | Abonelik için ayrıntılı satış modeli | 
| CustomerName | Müşterinin adı | 
| CustomerTenantId | Müşteri kiracısı GUID'si | 
| CustomerTpid | Müşterinin üst üst öğenin tanımlayıcısı | 
| CustomerSegment | Müşterinin pazar segmenti | 
| CustomerMarket | Müşterinin coğrafi pazar | 
| MPNId | Kimlik Microsoft İş Ortağı Ağı | 
| PartnerName | İş ortağının adı | 
| PartnerLocation | İş ortağının coğrafi ülke konumu | 
| PartnerAttachType | Abonelik için asıf türü | 
| PartnerHierarchy |    İş ortağı hiyerarşisi (Sanal Kuruluş veya HeadQuarters veya Konum)|
| AvailableSeats |  Geçerli ücretli kullanılabilir yer|
| AssignedSeats |   Geçerli atanan yer|
| ActiveSeats | Geçerli etkin yer sayısı|
| DeploymentOpportunity |   Dağıtım fırsatı, atanmamış olan yer sayısıdır|
| ActiveUsagePercent |  Kullanılabilir yerlerin yüzdesi olarak geçerli etkin kullanım|

### <a name="teams-meetings-and-calls-report"></a>**Teams ve çağrıları raporla**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| PGAMpnId | İş ortağı genel hesabı MPN'lerinin tanımlayıcısı | 
| CustomerTenantId | Müşterinin kiracı kimliği | 
| CustomerId | Müşterinin üst üst öğenin tanımlayıcısı | 
| DateKey | Kullanımın raporlandığı tarih
| Alt iş yükü | Kullanımın raporlandığı alt iş yükü (toplantılar, aramalar veya telefon sistemleri) | 
| Toplantı sayısı | Toplantı sayısı | 
| Toplantı süresi | Toplam toplantı süresi (saat) | 

### <a name="teams-monthly-usage-report"></a>**Teams aylık kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| Pgampnıd |    Ortak küresel hesap MPN tanımlayıcısı |
| CustomerTenantId |    Müşterinin Kiracı kimliği|
| CustomerId |  Müşteri üst üst öğesinin tanımlayıcısı|
| MonthKey |    Kullanımın bildirildiği ay|
| Alt Iş yükü | Kullanım için raporlanan alt iş yükü (toplantılar, çağrılar veya telefon sistemleri)|
| DesktopUsers |    masaüstünde Teams kullanan kullanıcı sayısı|
| MobileUsers | mobil üzerinde Teams kullanan kullanıcı sayısı|
| WebUsers |    web üzerinde Teams kullanan kullanıcı sayısı|
| Allupkatılımcıları |   ay için Teams benzersiz kullanıcı sayısı|

### <a name="teams-usage-3p-apps-report"></a>**Teams kullanımı 3p apps raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| Pgampnıd  | Ortak küresel hesap MPN tanımlayıcısı |
| CustomerTenantId |    Müşterinin Kiracı kimliği |
| CustomerId |  Müşteri üst üst kimliği |
| CustomerName |    Müşteri adı |
| CustomerCountry | Müşteri ülkesi |
| DateKey | Kullanımın bildirildiği Tarih |
| AppName | Teams uygulamasının adı |
| UserCount |   Uygulama için Kullanıcı sayısı |

### <a name="training-details-report"></a>**Eğitim Ayrıntıları raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| Pgampnıd  | Ortak küresel hesap MPN tanımlayıcısı |
| Traıningactivityıd | Eğitimin tanımlayıcısı | 
| Traıningtitle | Eğitimin başlığı | 
| Traıningtype | Eğitim türü (sertifika veya sınava) | 
| Kişiselleştirsoyadı | Müşterinin ilk adı | 
| Kişiselleştirallastname | Müşterinin soyadı | 
| E-posta | Müşterinin kişisel e-posta KIMLIĞI | 
| CorpEmail | müşterinin Office e-posta kimliği | 
| Traıningcompletiondate | Eğitimin tamamlanma tarihi | 
| ExpirationDate |  Sertifikanın sona erme tarihi|
| ActivationStatus |    Sertifika durumu|
| Ay | Verilerin bildirildiği ay | 
| IMCP | kullanıcının Microsoft sertifikalı Professional (MCP) olup olmadığını belirtir | 
| MCPID | Kullanıcının MCP KIMLIĞI | 
| Mpnıd | Microsoft İş Ortağı Ağı tanımlayıcısı | 
| PartnerName | Ortağın adı | 
| PartnerCityLocation | Ortağın coğrafi şehir konumu | 
| PartnerCountryLocation | Ortağın coğrafi ülke konumu | 

### <a name="microsoft-learn-report"></a>**Microsoft Learn raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| Pgampnıd  | Ortak küresel hesap MPN tanımlayıcısı |
| UserName | Kullanıcının adı | 
| UserId | Kullanıcının GUID 'SI | 
| Traıningname | Eğitimin adı | 
| Traıningtype | Eğitim türü (modül veya öğrenme yolu) | 
| Ürünler | Öğrenme modülünün geçerli olduğu ürün | 
| Roller | Eğitimin uygun rolleri | 
| CompletionDate | Eğitimin tamamlanma tarihi | 
| Mpnıd | Microsoft İş Ortağı Ağı tanımlayıcısı | 
| PartnerName | Ortağın adı | 
| Ülke | Ortağın coğrafi ülke konumu | 

### <a name="competency-summary-and-history-report"></a>**Uzmanlık Özeti ve geçmiş raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| Uzmanlık adı | Uzmanlığa ilişkin ad | 
| Uzmanlık düzeyi | Uzmanlık düzeyi (altın veya gümüş) | 
| Uzmanlık durumu | Uzmanlığa ait geçerli durum (etkin, etkin değil veya yetkisiz kullanım süresi) | 
| Uzmanlık tarihi | Uzmanlığa ait başlangıç tarihi | 
| Uzmandan bir yenne tarihi | Uzmanlığa ilişkin bitiş tarihi | 

### <a name="competency-performance-report"></a>**Uzmanlığa yönelik performans raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| Uzmanlık adı | Uzmanlığa ilişkin ad | 
| Yıo Encyatlationmentoptionname | Uzmanlığa erişme seçeneğinin adı | 
| Ay | Ölçümlerin bildirildiği ay | 
| MetricName | Uzmanlığa uygun ölçüm adı | 
| Metricmonthlykatkısı | Ölçümün aylık katkısı | 
| TTMAggregate | Sondaki 12 ay için toplanan ölçüm | 
| Anniversarne Yearaggregate | Geçerli yıldönümü yılı için toplanan ölçüm | 
| GoldThreshold | Altın uzmanlığa uyması için performans gereksinimi | 
| SilverThreshold | Gümüş uzmanlığa uyması için performans gereksinimi | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**bulut yokent-Microsoft 365 eğilimini raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| MPN Kimliği | Microsoft İş Ortağı Ağı KIMLIĞI | 
| İş ortağı adı | Ortağın adı | 
| Müşteri Kimliği | Müşterinin tanımlayıcı numarası | 
| DYENIDEN sayı | Eğilimini için puanlanmakta olan müşterinin Dun & Bradstreet (D&B) numarası | 
| Hesap Adı | Hesabın adı | 
| Etki alanı | Hesabın etki alanı | 
| Kuruluş boyutu | Kuruluşun boyutu | 
| Sektör | Kuruluşun ait olduğu sektör | 
| Dikey | Microsoft, D&B ve diğer sektör standartları tarafından tanımlanan eğilimini için puanlanmakta olan müşterinin dikey | 
| Alan | Konumun coğrafi alanı | 
| Yan Kuruluş | Eğilimini için puanlanmakta olan müşterinin yan kuruluşu | 
| Sales Territory | Eğilimini için puanlanmakta olan müşterinin satış bölgesi | 
| Şehir | Kuruluşun coğrafi şehir konumu | 
| Durum | Kuruluşun coğrafi durum konumu | 
| Posta Kodu | Kuruluşun posta kodu | 
| Ülke | Kuruluşun coğrafi ülke konumu | 
| Segment | Pazar segmenti | 
| Alt kesim | Pazar alt segmenti | 
| SMC tür Özeti | SMC türü | 
| En iyi yönetilmeyen Işlem tabanı | En çok yönetilmeyen müşteriler – işlem | 
| En çok yönetilmeyen-kullanıcı tabanı | En iyi yönetilmeyen müşteriler – Kullanıcı | 
| Iskar dışı | Kuruluşun kar dışı olup olmadığını gösterir (Evet veya Hayır) | 
| Uzak Iş-hedef Exchange Online etkinleştir | etkin bir Exchange Online aboneliğine sahip olan müşteriler, Microsoft 365 yukarı satış | 
| Cloud Ascent eğilimini-+ 10 lisanslarıyla uzak Iş yerinde alımı (geçerli sürüm) etkinleştirin | geçerli bir şirket içi Office veya Windows istemcisi olan müşteri. Diğer bir deyişle, istemci sürümü yaşam sonu (EOL) sürümünden daha sonraki bir sürümdür. Müşterinin 10 veya daha fazla lisansı vardır. Eğilimini puanı olan müşteri. İş ortağı, Microsoft 365 dönüştürme için hedef almalıdır. | 
| Cloud Ascent eğilimini-<10 lisanslarıyla uzak Iş yerinde alımı (geçerli sürüm) etkinleştirin | geçerli bir şirket içi Office veya Windows istemcisine sahip olan müşteri (yani, eol 'tan sonraki bir sürüm). Müşterinin 10 ' dan az lisansı vardır. Teklif puanına sahip olan müşteri. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi olmadan şirket içi alım (geçerli sürüm) - +10 lisans | Geçerli bir şirket içi istemciye sahip olan Office Windows (yani, EOL'den sonraki bir sürüm). Müşterinin 10 veya daha fazla lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi olmadan şirket içi alım (geçerli sürüm) - <10 lisans | Geçerli bir şirket içi istemciye sahip olan Office Windows (yani, EOL'den sonraki bir sürüm). Müşterinin 10'dan az lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi ile şirket içi alım (EOL sürümü) - +10 lisans | Şirket içi bir EOL veya Office Windows (yani, bir EOL sürümü veya önceki) olan müşteri. Müşterinin 10 veya daha fazla lisansı vardır. Müşterinin bir yayma puanı vardır. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi ile şirket içi alım (EOL sürümü) - <10 lisans | Şirket içi bir EOL veya Office Windows (yani, bir EOL sürümü veya önceki) olan müşteri. Müşterinin 10'dan az lisansı vardır. Müşterinin bir yayma puanı vardır. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi olmadan şirket içi alım (EOL sürümü) - +10 lisans | Geçerli bir şirket içi istemciye sahip olan Office Windows (yani, bir EOL sürümü veya önceki bir sürümü). Müşterinin 10 veya daha fazla lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi olmadan şirket içi alım (EOL sürümü) - <10 lisans | Geçerli bir şirket içi istemciye sahip olan Office Windows (yani, bir EOL sürümü veya önceki bir sürümü). Müşterinin 10'dan az lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştir - yüksek olasılık olasılığı Microsoft 365 (Act NowithEvaluate) | Müşteri adayları için yüksek Microsoft 365 | 
| Uzaktan Çalışma Etkinleştir - uzaktan çalışmayla rekabet Microsoft 365 | Yakınlaştırma ve yakınlaştırma özelliğine Microsoft 365 müşteri, hedef olarak Teams | 
| Uzaktan Çalışma Özelliğini Etkinleştirme - uzaktan çalışmadan rekabet Microsoft 365 | Yakınlaştırmalı müşteri, hedef hedef Teams | 
| Maliyet ve Yönetimi Azaltma - Microsoft 365 E3 hedefli Microsoft 365 E5 | Mevcut müşteri Microsoft 365 E3, hedef Microsoft 365 E5 | 
| Maliyet ve Yönetimi Azaltma - Microsoft 365 İş Temel ve İş Standardı müşterileri Microsoft 365 İş Ekstra | Mevcut Microsoft 365 İş Temel ve İş Standardı müşterileri, Microsoft 365 İş Ekstra | 
| Kuruluş Üretkenliğini Dönüştürme - Yüzey eğilimi | Müşteri Surface için bir eğilimi gösteriyor | 
| M365Cluster | Müşterinin satın alma eğilimini Microsoft 365. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir hedefle'den sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| M365Fit | Sıkı grafiği tanımlayan iç ve dış veri noktaları. Uygun puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünleri için potansiyel olarak uygun olup olmadığını görmek için en küçük veya orta ölçekli işletmelere (SMB) benzer bir model kullanır. Fit puanlama üç aylık olarak güncelleştirilir. | 
| M365Intent | Sosyal medya ve müşterinin çevrimiçi davranışıyla ilgili sinyaller Amacı tanımlar. Amaç puanlama, kümeleri tanımlamak için Sığdır'ın üzerine atlar. Amaç puanlama aylık olarak güncelleştirilir. | 
| SurfaceCluster | Fit ve Intent önerilerini bir kümede bir arada kullanarak bir müşterinin Surface satın alma eğilimini tanımlar. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir hedefle'den sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| SurfaceFit | Sıkı grafiği tanımlayan iç ve dış veri noktaları. Uygun puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünlerine potansiyel olarak uygun olup olmadığını görmek için en iyi SMB'lerimize benzer bir model kullanır. Fit puanlama üç aylık olarak güncelleştirilir. | 
| SurfaceIntent | Sosyal medya ve müşterinin çevrimiçi davranışıyla ilgili sinyaller Amacı tanımlar. Amaç puanlama, kümeleri tanımlamak için Sığdır'ın üzerine atlar. Amaç puanlama aylık olarak güncelleştirilir. | 
| O365Cluster | Müşterinin satın alma eğilimini Office 365. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir hedefle'den sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| O365Fit | Sıkı grafiği tanımlayan iç ve dış veri noktaları. Uygun puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünlerine potansiyel olarak uygun olup olmadığını görmek için en iyi SMB'lerimize benzer bir model kullanır. Fit puanlama üç aylık olarak güncelleştirilir. | 
| O365Intent | Sosyal medya ve müşterinin çevrimiçi davranışıyla ilgili sinyaller Amacı tanımlar. Amaç puanlama, kümeleri tanımlamak için Sığdır'ın üzerine atlar. Amaç puanlama aylık olarak güncelleştirilir. | 
| M365UpsellCustomer | Müşterinin sipariş için satış eğilimi gösterip Microsoft 365 | 
| Google'a sahip | Müşterinin Google ürünlerine sahip olmak için rekabet sinyalleri gösterip gösterip gösterir olmadığını tanımlar | 
| AWS'ye sahip | Müşterinin kendi (AWS) ürünlerine sahip olmak için Amazon Web Services sinyalleri gösterip gösterip gösterir | 
| EA'ya sahip | Yenilemenin kurumsal anlaşma (EA) veya EA aboneliği olup olmadığını tanımlar | 
| Açık | Yenilemenin Açık veya Açık Değer sözleşmesi olup olmadığını tanımlar | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Bulut Ascent - Dynamics 365 eğilimi raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| MPN Kimliği | Microsoft İş Ortağı Ağı (MPN) Kimliği | 
| İş Ortağı Adı | İş ortağının adı | 
| Müşteri Kimliği | Müşteri tanımlayıcı numarası | 
| DUNS Numarası | Dun & Bradstreet, eğilimini için puanlanmakta olan müşterinin numarası | 
| Hesap Adı | Hesabın adı | 
| Etki alanı | Hesabın etki alanı | 
| Kuruluş boyutu | Kuruluşun boyutu | 
| Sektör | Kuruluşun ait olduğu sektör | 
| Dikey | Microsoft, D&B ve diğer sektör standartları tarafından tanımlanan eğilimini için puanlanmakta olan müşterinin dikey
| Alan | Konumun coğrafi alanı | 
| Yan Kuruluş | Eğilimini için puanlanmakta olan müşterinin yan kuruluşu | 
| Sales Territory | Eğilimini için puanlanmakta olan müşterinin satış bölgesi | 
| Şehir | Coğrafi şehir konumu | 
| Durum | Coğrafi durum konumu | 
| Posta Kodu | Kuruluşun posta kodu | 
| Ülke | Coğrafi ülke konumu | 
| Segment | Pazar segmenti | 
| Alt kesim | Pazar alt segmenti | 
| SMC tür Özeti | Müşterinin kategorisi: en popüler yönetilmeyen Kullanıcı temelleri, 300 ' e kadar çalışan müşteriler, en fazla yönetilmeyen işlem esasları ise müşterilerin üç yıllık potansiyel olarak USD10, orta ölçekli çalışanlar ise 25 ' ten az çalışanı olan müşterilerimiz ve küçük işletmeler için 25 ' ten az çalışan müşteriler. | 
| En iyi yönetilmeyen Işlem tabanı | En çok yönetilmeyen müşteriler – işlem | 
| En çok yönetilmeyen-kullanıcı tabanı | En çok yönetilmeyen müşteriler – kullanıcılar | 
| Iskar dışı | Kuruluşun kar dışı olup olmadığını gösterir (Evet veya Hayır) | 
| dijital satışı etkinleştir-Microsoft 365 özellikli boyutu >= 25 bilgisayar (salespro eğilimini model) | Dynamics 365 içermeyen müşteri. Koltuk boyutu: 25 +. İş ortağı Dynamics 365 SalesPro 'nun çapraz satışı için hedeflemelidir. | 
| Dijital satışı etkinleştirin-Dynamics 365 SalesPro eğilimini (Şimdi davran veya değerlendir) | Dynamics 365 içermeyen yüksek eğilimini müşterileri. İş ortağı Dynamics 365 SalesPro için hedeflemelidir. | 
| Finans riskini yönetme & sahtekarlık-Dynamics şirket içi yüklemesi temel-Navision (Business Central eğilimini model) | Şirket içi Navision ile mevcut müşteri. İş ortağı Dynamics 365 Business Central için hedeflemelidir. | 
| Finans riskini yönetme & sahtekarlık-Dynamics şirket içi Install Base-Dynamics AX (Dynamics 365 finans + Operations eğilimini model) | Şirket içi AX ile mevcut müşteri. İş ortağı, Dynamics 365 finans + Işlemleri için hedeflemelidir. | 
| Finans riskini yönetme & sahtekarlık-Dynamics şirket içi yüklemesi temel-harika Plains (Business Central eğilimini model) | Şirket içi Great Plains 'e sahip mevcut müşteri. İş ortağı Dynamics 365 Business Central için hedeflemelidir. | 
| Finans riskini yönetme & sahtekarlık-Dynamics şirket içi yüklemesi temel-Solomon (Business Central eğilimini model) | Şirket içi Solomon ile mevcut müşteri. İş ortağı Dynamics 365 Business Central için hedeflemelidir. | 
| Finans riskini yönetme & sahtekarlık-Dynamics şirket içi yüklemesi-diğerleri (Business Central eğilimini model) | Diğer şirket içi çözümlere sahip mevcut müşteri daha önce listelenmemiş. İş ortağı Dynamics 365 Business Central için hedeflemelidir. | 
| Çevik Iş süreçleri oluşturma-Dynamics şirket içi yüklemesi temel-AX/GP/SL/NAV/diğer (Dynamics 365 eğilimini model) | Çevik Iş süreçleri oluşturma-Dynamics şirket içi yüklemesi temel-AX/GP/SL/NAV/diğer (Dynamics 365 eğilimini model) | 
| Çevik Iş süreçleri oluşturma-Dynamics rekabet tabanı-mendix/OutSystems/Salesforce (Dynamics 365 eğilimini model) | Çevik iş süreçleri oluşturma-Dynamics rekabet tabanı-mendix/OutSystems/Salesforce (Dynamics 365 eğilimini model) | 
| Çevik Iş süreçleri oluşturma-Dynamics 365 finans + Operations Install Base | Mevcut Dynamics 365 finans + Operations müşterileri. Hedef iş ortağı Power Apps. | 
| Çevik Iş süreçleri oluşturma-Dynamics 365 Iş Merkezi yüklemesi temeli | Mevcut Dynamics 365 Iş merkezi müşterileri. Hedef iş ortağı Power Apps. | 
| Çevik Iş süreçleri oluşturma-Dynamics 365 müşteri katılımı yüklemesi temeli | Mevcut Dynamics 365 müşteri katılımı müşterileri. Hedef iş ortağı Power Apps. | 
| esnek tedarik zinciri oluşturma-Windows ve ilk dynamics 365 iş yükünü Oracle olmayan veya SAP ERP (kurumsal kaynak planlama) müşterileri ile dynamics 365 tedarik zinciri yönetimi olarak etkinleştirin | Dynamics 365 tedarik zinciri yönetimi için hedef müşteriler | 
| Mevcut Dynamics 365 müşteri katılım müşterilerine dayanıklı bir tedarik zinciri oluşturun ve şirketler arası Dynamics 365 tedarik zinciri yönetimi ve/veya perakende veya ticaret | Mevcut Dynamics 365 müşteri katılımı müşterileri, şirketler arası Dynamics 365 tedarik zinciri yönetimi için hedeflenecek. | 
| Bir dayanıklı tedarik zinciri oluşturun-şirketler arası Dynamics 365 tedarik zinciri yönetimi ve/veya perakende veya ticaret, Dynamics 365 müşteri katılımı ve Oracle veya SAP 'a | Dynamics 365 tedarik zinciri yönetimi için hedeflemek üzere Oracle veya SAP ile mevcut Dynamics 365 müşteri katılımı müşterileri | 
| D365BCCluster | Dynamics 365 Business Central satın almak için müşterinin eğilimini tanımlar. Eğilimini for Business Central 'ı gösteren müşteriler orta ve küçük kategorilerde olacaktır. Hedef şimdi çalışır ve daha yüksek verim üretebilmeleri için kümeleri değerlendirir. Yalnızca Şimdi hareket ettikten ve müşterileri değerlendirdikten sonra hala kapasite varsa müşterileri Eğtir ve müşterileri eğitin. | 
| D365BCFit | Firmografları tanımlayan iç ve dış veri noktaları. Kullanım Puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünleri için olası bir uyum olup olmadığını görmek için en iyi SMB 'ye bir gevkalike modeli kullanır. Skor, üç aylık olarak güncelleştirilir. | 
| D365BCIntent | Sosyal medya ve müşterinin çevrimiçi davranışı ile ilgili sinyaller amaç tanımlar. Amaç Puanlama, kümeleri tanımlamak için uygun şekilde yer alır. Amaç Puanlama aylık olarak güncelleştirilir. | 
| D365FOCluster | Dynamics 365 finans ve Işlemlerini satın almak için müşterinin eğilimini tanımlar. Finans + Işlemlerine yönelik bir eğilimini gösteren müşteriler, en üstteki yönetilmeyen kategorilerde yer alacak. Hedef şimdi çalışır ve daha yüksek verim üretebilmeleri için kümeleri değerlendirir. Yalnızca Şimdi hareket ettikten ve müşterileri değerlendirdikten sonra hala kapasite varsa müşterileri Eğtir ve müşterileri eğitin. | 
| D365FOFit | Firmografları tanımlayan iç ve dış veri noktaları. Kullanım Puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünleri için olası bir uyum olup olmadığını görmek için en iyi SMB 'ye bir gevkalike modeli kullanır. Skor, üç aylık olarak güncelleştirilir. | 
| D365FOIntent | Sosyal medya ve müşterinin çevrimiçi davranışı ile ilgili sinyaller amaç tanımlar. Amaç Puanlama, kümeleri tanımlamak için uygun şekilde yer alır. Amaç Puanlama aylık olarak güncelleştirilir. | 
| D365CECluster | Dynamics 365 müşteri katılımı satın almak için müşterinin eğilimini tanımlar. Müşteri katılımı için bir eğilimini gösteren müşteriler orta ve küçük kategorilerde olacaktır. Hedef şimdi çalışır ve daha yüksek verim üretebilmeleri için kümeleri değerlendirir. Yalnızca Şimdi hareket ettikten ve müşterileri değerlendirdikten sonra hala kapasite varsa müşterileri Eğtir ve müşterileri eğitin. | 
| D365CEFit | Dynamics 365 müşteri katılımı için uygun olduğunu belirtir | 
| D365CEIntent | Dynamics 365 müşteri katılımı için amacı gösterir | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Müşterinin Dynamics şirket içi AX veya CRM için açık yenileme olup olmadığını belirler | 
| M365UpsellCustomer | Müşterinin Microsoft 365 için büyük satış eğilimini gösterilip gösterilmeyeceğini belirler | 
| Google 'a sahiptir | Müşterinin sahip olduğu Google ürünleri için rekabet sinyalleri gösterilip gösterilmeyeceğini belirler | 
| AWS 'ye sahip | Müşterinin sahip olduğu AWS ürünleri için rekabet sinyalleri gösterilip gösterilmeyeceğini belirler | 
| EA 'ya sahiptir | Bir yenilemenin EA veya EA aboneliği olup olmadığını belirler | 
| Açık | Bir yenilemenin açık veya açık bir değer anlaşması olup olmadığını belirler | 

### <a name="cloud-ascent---azure-propensity-report"></a>**Bulut Yokent-Azure eğilimini raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| MPN Kimliği | Microsoft İş Ortağı Ağı (MPN) KIMLIĞI | 
| İş ortağı adı | Ortağın adı | 
| Müşteri Kimliği | Müşteri tanımlayıcı numarası | 
| DYENIDEN sayı | Dun & Bradstreet, eğilimini için puanlanmakta olan müşterinin numarası | 
| Hesap Adı | Hesabın adı | 
| Etki alanı | Hesabın etki alanı | 
| Kuruluş boyutu | Kuruluşun boyutu | 
| Sektör | Sektör | 
| Dikey | Microsoft, D&B ve diğer sektör standartları tarafından tanımlanan eğilimini için puanlanmakta olan müşterinin dikey | 
| Alan | Konumun coğrafi alanı | 
| Yan Kuruluş | Eğilimini için puanlanmakta olan müşterinin yan kuruluşu | 
| Sales Territory | Eğilimini için puanlanmakta olan müşterinin satış bölgesi | 
| Şehir | Coğrafi şehir konumu | 
| Durum | Coğrafi durum konumu | 
| Posta Kodu | Kuruluşun posta kodu | 
| Ülke | Coğrafi ülke konumu | 
| Segment | Pazar segmenti | 
| Alt kesim | Pazar alt segmenti | 
| SMC tür Özeti | SMC türü | 
| En iyi yönetilmeyen Işlem tabanı | En çok yönetilmeyen müşteriler – işlem | 
| En çok yönetilmeyen-kullanıcı tabanı | En çok yönetilmeyen müşteriler – kullanıcılar | 
| Iskar dışı | Kuruluşun kar dışı olup olmadığını gösterir (Evet veya Hayır) | 
| Migrate-eol Windows server-eol Windows server ıb, Cloud ascent eğilimini-5 + lisanslarıyla | bir eol şirket içi Windows sunucusuna sahip olan müşteri (yani, bir eol sürümü veya daha eski). Müşterinin 5 veya daha fazla lisansı vardır. Eğilimini puanı olan müşteri. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Migrate-eol Windows server-eol Windows server ıb, Cloud ascent eğilimini-<5 lisanslarına sahip | bir eol şirket içi Windows sunucusuna sahip olan müşteri (yani, bir eol sürümü veya daha eski). Müşterinin 5 ' ten az lisansı vardır. Eğilimini puanı olan müşteri. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Migrate-eol Windows server-eol Windows server ıb, Cloud ascent eğilimini-5 + lisansı olmadan | bir eol şirket içi Windows sunucusuna sahip olan müşteri (yani, bir eol sürümü veya daha eski). Müşterinin 5 ' ten fazla lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Migrate-eol Windows server-eol Windows server ıb olmadan eğilimini-<5 lisansı | bir eol şirket içi Windows sunucusuna sahip olan müşteri (yani, bir eol sürümü veya daha eski). 5 ' ten az lisansa sahiptir. Müşterinin eğilimini puanı yok. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Cloud ascent eğilimini-5 + lisanslarıyla geçiş-eol SQL-eol SQL Server IB | bir eol şirket içi SQL Server (yani, bir eol sürümü veya daha eski) olan müşteri. Müşterinin 5 ve lisansı vardır. Müşterinin bir eğilimini puanı vardır. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Migrate-eol SQL-eol SQL Server ıb, Cloud ascent eğilimini-<5 lisanslarıyla | bir eol şirket içi SQL Server (yani, bir eol sürümü veya daha eski) olan müşteri. 5 ' ten az lisansa sahiptir. Eğilimini puanı olan müşteri. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| -eol SQL-eol SQL Server ıb, Cloud ascent eğilimini-5 + lisansı olmadan | bir eol şirket içi SQL Server (yani, bir eol sürümü veya daha eski) olan müşteri. Müşterinin 5 veya daha fazla lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Migrate-eol SQL-eol SQL Server ıb, Cloud ascent eğilimini-<5 lisansı olmadan | bir eol şirket içi SQL Server (yani, bir eol sürümü veya daha eski) olan müşteri. Müşterinin 5 ' ten az lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| geçiş-şirket içi Windows sunucusu-bulut ascent eğilimini-5 + lisanslarıyla geçerli Windows sunucusu ıb | geçerli bir şirket içi Windows sunucusuna (yani, eol 'tan sonraki bir sürüm) sahip olan müşteri. Müşterinin 5 ve lisansı vardır. Müşterinin bir eğilimini puanı vardır. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| geçiş-şirket içi Windows sunucusu-bulut ascent eğilimini-<5 lisanslarıyla geçerli Windows sunucusu ıb | geçerli bir şirket içi Windows sunucusuna (yani, eol 'tan sonraki bir sürüm) sahip olan müşteri. Müşterinin 5 ' ten az lisansı vardır. Müşterinin Azure için eğilimini puanı vardır. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| geçiş-şirket içi Windows sunucusu-geçerli Windows sunucusu, Cloud ascent eğilimini-5 ' i içermeyen lisans | geçerli bir şirket içi Windows sunucusuna (yani, eol 'tan sonraki bir sürüm) sahip olan müşteri. Müşterinin 5 ve lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| geçiş-şirket içi Windows sunucusu-bulut yokeğilimini-<5 lisansı olmadan geçerli Windows sunucusu ıb | geçerli bir şirket içi Windows sunucusuna (yani, eol 'tan sonraki bir sürüm) sahip olan müşteri. Müşterinin 5 ' ten az lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| geçiş-Azure SQL veya SQL sanal makinelere (vm) geçiş-Cloud ascent eğilimini-5 + lisanslarıyla güncel SQL Server IB | geçerli bir şirket içi SQL Server (yani, eol 'tan sonraki bir sürüm) olan müşteri. Müşterinin 5 ve lisansı vardır. Müşterinin bir eğilimini puanı vardır. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| geçiş-Azure SQL veya SQL vm 'lere geçiş-Cloud ascent eğilimini-<5 lisanslarıyla güncel SQL Server IB | geçerli bir şirket içi SQL Server (yani, eol 'tan sonraki bir sürüm) olan müşteri. Müşterinin 5 ' ten az lisansı vardır. Müşterinin bir eğilimini puanı vardır. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| geçiş-Azure SQL veya SQL vm 'lere geçiş-Cloud ascent eğilimini-5 + lisansı olmadan geçerli SQL Server IB | geçerli bir şirket içi SQL Server (yani, eol 'tan sonraki bir sürüm) olan müşteri. Müşterinin 5 ve lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| geçiş-Azure SQL veya SQL vm 'lere geçiş-Cloud ascent eğilimini-<5 lisansı olmadan güncel SQL Server IB | geçerli bir şirket içi SQL Server (yani, eol 'tan sonraki bir sürüm) olan müşteri. Müşterinin 5 ' ten az lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Migrate-OSS-açık kaynak Shakespeare (OSS) DB 'ye geçir | Aşağıdaki yarışmaya sahip ürünlerden birini içeren mevcut müşteri: PostgreSQL, MySQL, MariaDB. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Azure 'da-OSS-Linux geçirme | Linux ile mevcut müşteri. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Azure 'da geçiş-SAP-SAP | SAP ile mevcut müşteri. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| geçiş-Windows sanal masaüstü-Uzak Masaüstü Hizmetleri ıb | etkin Windows Uzak Masaüstü Hizmetleri olan müşterileri tanımlar. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| geçiş-Windows sanal masaüstü-Modern işleri Azure 'a/wvd 'e çapraz satış | Microsoft 365 ile müşterileri tanımlar ve Azure 'a sahip değildir. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Geçiş-VMware ıB | Ürüne sahip mevcut müşteri: VMware. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Geçiş-Citrix ıB | Ürüne sahip mevcut müşteri: Citrix Systems. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| yenilik yapın-Analytics-Power BI ıb with high Azure eğilimini | Power BI abonelik içeren ve etkin olan müşteriler: Power BI-tek başına Pro, Power BI-Azure paketleri, Power BI Office paketleri, Power BI paketleri-Microsoft 365 | 
| GitHub DevOps etkinleştirme-Visual Studio/msdn ıb | etkin Visual Studio sürümleriyle müşterileri tanımlar | 
| Windows Sunucu standart sürümü | müşteri tarafından Windows sunucusu standart satın alımlarınızın sürümünü görüntüler | 
| Windows Sunucu standart lisansı | müşteri tarafından Windows sunucusu standart satın alımlarınızın lisans türünü görüntüler | 
| Windows Sunucu veri merkezi sürümü | müşteriye göre Windows veri merkezi satın alımlarınızın sürümünü görüntüler | 
| Windows Sunucu veri merkezi lisansı | müşteriye göre Windows veri merkezi satın alımlarınızın lisans türünü görüntüler | 
| AzureFit | Firmografları tanımlayan iç ve dış veri noktaları. Kullanım Puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünleri için olası bir uyum olup olmadığını görmek için en iyi SMB 'ye bir gevkalike modeli kullanır. Skor, üç aylık olarak güncelleştirilir. | 
| AzureIntent | Sosyal medya ve müşterinin çevrimiçi davranışı ile ilgili sinyaller amaç tanımlar. Amaç Puanlama, kümeleri tanımlamak için uygun şekilde yer alır. Amaç Puanlama aylık olarak güncelleştirilir. | 
| AzureCluster | Bir kümeye sığdırma ve amaç önerilerini birleştirerek müşterinin Azure satın alma eğilimini tanımlar. Hedef şimdi çalışır ve daha yüksek verim üretebilmeleri için kümeleri değerlendirir. Yalnızca Şimdi hareket ettikten ve müşterileri değerlendirdikten sonra hala kapasite varsa müşterileri Eğtir ve müşterileri eğitin. | 
| WindowsServerDataCenter_HasOpenRenewal | müşterinin Windows Server veri merkezi için açık yenileme olup olmadığını belirler | 
| WindowsServerStandard_HasOpenRenewal | Müşterinin Windows Server Standard için açık yenilemeye sahip olup olmadığını tanımlar | 
| AzureUpsellCustomer | Müşterinin Azure için satış eğilimi gösterip gösterip gösterir olmadığını tanımlar | 
| Google'a sahip | Müşterinin Google ürünlerine sahip olmak için rekabet sinyalleri gösterip gösterip gösterir olmadığını tanımlar | 
| AWS'ye sahip | Müşterinin aws ürünlerine sahip olan müşteriler için rekabet sinyalleri gösterip gösterip gösterip gösterir | 
| EA'ya sahip | Yenilemenin EA aboneliği mi yoksa EA aboneliği mi olduğunu tanımlar | 
| Açık | Yenilemenin Açık veya Açık Değer sözleşmesi olup olmadığını tanımlar | 

### <a name="cloud-ascent---agreement-renewal-propensity-report"></a>**Bulut Ascent - sözleşme yenileme eğilimi raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| MPN Kimliği | Microsoft İş Ortağı Ağı kimliği | 
| İş Ortağı Adı | İş ortağının adı | 
| Müşteri Kimliği | Müşteri tanımlayıcı numarası | 
| DUNS Numarası | Dun &, yayma puanı alan müşterinin Bradstreet numarasını aldı | 
| Hesap Adı | Hesabın adı | 
| Etki alanı | Hesabın etki alanı | 
| Kuruluş Boyutu | Kuruluşun boyutu | 
| Sektör | Sektör | 
| Dikey | Microsoft, D&B ve diğer sektör standartları tarafından tanımlanan, yayma puanı alan müşterinin dikeyi | 
| Alan | Konumun coğrafi alanı | 
| Yan Kuruluş | Teklif puanı alan müşterinin yan kuruluşu | 
| Sales Territory | Yayma puanı alan müşterinin satış bölgesi | 
| Şehir | Coğrafi şehir konumu | 
| Durum | Coğrafi durum konumu | 
| Posta Kodu | Kuruluşun posta kodu | 
| Ülke | Coğrafi ülke konumu | 
| Segment | Pazar segmenti | 
| Alt Kesim | Pazar alt | 
| SMC Tür Özeti | SMC türü | 
| En İyi Unmanaged - İşlem Tabanı | En çok kontrol dışı olan müşteriler – işlem | 
| En İyi Unmanaged - Kullanıcı Tabanı | En iyi unmanaged müşterileri – kullanıcılar | 
| IsNonProfit | Kuruluşun kar amacı gütmeyen bir kuruluş olup olmadığını gösterir (Evet veya Hayır) | 
| Google'a sahip | Müşterinin aws ürünlerine sahip olan müşteriler için rekabet sinyalleri gösterip gösterip gösterip gösterir | 
| AWS'ye sahip | Müşterinin aws ürünlerine sahip olan müşteriler için rekabet sinyalleri gösterip gösterip gösterip gösterir | 
| Azure Kümesi | Müşterinin Azure satın alma eğilimini tanımlar. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| D365 Finance + Operations Cluster | Müşterinin Dynamics 365 Finance and Operations satın alma eğilimini tanımlar. Finance + Operations için bir eğilimini göstermekte olan müşteriler, en üst sırada yer alan, en üst sırada yer alan ve olmayan kategorilere ayrılır. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| D365 CE Kümesi | Müşterinin Dynamics 365 Customer Engagement satın alma eğilimini tanımlar. Customer Engagement için bir teklifte yer alan müşteriler Orta ve Küçük kategorilerde yer atılır. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| D365 BC Kümesi | Müşterinin Dynamics 365 Business Central satın alma eğilimini tanımlar. Business Central için bir teklifte bulunan müşteriler Orta ve Küçük kategorilerde yer atılır. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| Microsoft 365 Küme | Müşterinin satın alma eğilimini Microsoft 365. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| Lisans Programı | Yenileme için lisans programı türünü tanımlar | 
| Sözleşme Kimliği | Sözleşmenin tanımlayıcısı | 
| Sözleşme Bitiş Tarihi | Sözleşmenin bitiş tarihi | 
| Süre Sonu Türü | Süre sonu türü | 
| Süresi Dolan Gelir | Süresi dolan aboneliklerle ilişkili gelir | 
| EA'ya sahip | Yenilemenin EA aboneliği mi yoksa EA aboneliği mi olduğunu tanımlar | 
| Açık | Yenilemenin Açık veya Açık Değer sözleşmesi olup olmadığını tanımlar | 
| Azure Upsell müşterisi | Müşterinin Azure için büyük satış eğilimini göstermeyeceğini belirler | 
| Microsoft 365 Büyük satış müşterisi | Müşterinin Microsoft 365 için büyük satış eğilimini gösterilip gösterilmeyeceğini belirler | 
| RevSumDivisionName | Yenilemeye yönelik ürünü tanımlar | 

## <a name="next-steps"></a>Sonraki adımlar

Daha fazla bilgi için bkz. [raporları indirme](insights-download-reports.md).
