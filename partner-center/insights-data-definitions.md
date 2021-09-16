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
ms.openlocfilehash: d1119152e601c0fa7f8bb080420181d1f52801db
ms.sourcegitcommit: 847ad384d44a5a673791cb2950af02225d8174c9
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/16/2021
ms.locfileid: "127876739"
---
# <a name="export--data-definitions"></a>Dışarı Aktarma – Veri tanımları 

**Uygun roller:** Rapor görüntüleyici | Yönetici raporu görüntüleyicisi

## <a name="introduction"></a>Giriş 

Panoda Raporları İndir hub'ını Analizler ham veri kümelerini dışarı aktarabilirsiniz. 

Veri tanımlarıyla birlikte indirebilirsiniz çeşitli raporlar aşağıdaki tablolarda listelenmiştir: 

### <a name="partner-profile-report"></a>**İş ortağı profili raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| MPNId | Microsoft İş Ortağı Ağı (MPN) Kimliği | 
| PartnerName | İş ortağının adı | 
| PGA_MPNId | İş ortağı genel hesabı MPN'lerinin tanımlayıcısı | 
| PGA_PartnerName | İş ortağı genel hesap adı | 
| Şehir | İş ortağının şehir konumu | 
| Ülke | İş ortağının ülke konumu | 
| HierarchyLevel | Bunun Genel MPN Kimliği mi yoksa konum MPN Kimliği mi olduğunu gösterir | 

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
| IndirectProviderMPNId | Dolaylı sağlayıcının kimliği Microsoft İş Ortağı Ağı | 
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
|kaynak grubundaki | Aboneliğin GUID'si|
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
|AvailableSeats | Ay içinde kullanılabilen yer farkı|
|BilledRevenueUSD | ABD doları olarak gelir|
|AzureConsumedRevenueUSD| Azure Tüketim Geliri ABD doları|

### <a name="azure-usage-report"></a>**Azure kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
|PGAMpnId| İş ortağı genel hesabı MPN'lerinin tanımlayıcısı|
|kaynak grubundaki| Aboneliğin GUID'si|
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
| PartnerAttributionType | İş ortağının atfı | 
| IsDuplicateRowForPGA | Tek bir PGA altındaki birden çok iş ortağı atıbetleri için bu değer yalnızca bir MPNId için 0 olarak ayarlanır. Değer 1 olarak ayarlanırsa yinelenen bir satır gösterir|

### <a name="enterprise-mobility-license-usage-report"></a>**Enterprise Mobility lisans kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| PGAMpnId| İş ortağı genel hesabı MPN'lerinin tanımlayıcısı| 
| kaynak grubundaki | Aboneliğin GUID'si| 
| SubscriptionStartDate | Aboneliğin başlangıç tarihi| 
| SubscriptionEndDate | Aboneliğin bitiş tarihi| 
| SubscriptionStatus| Aboneliğin geçerli durumu (Açık, Kapalı, Etkin veya Yetkisiz Kullanım Süresinde)| 
| Ay | Aya göre toplanan tarih| 
| SKU| Ürün SKU'su| 
| SKUId| Ürünün SKU Kimliği| 
| FreeVsPaidSKU| Ücretsiz veya Ücretli SKU'ya işaret| 
| SalesModel| Aboneliğin satışı için kullanılan satış kanalı| 
| DetailedSalesModel| Abonelik için ayrıntılı satış modeli| 
| CustomerName| Müşterinin adı| 
| CustomerTenantId | Müşterinin Kiracı Kimliği| 
| CustomerTpid | Müşteri üst üst kimliği| 
| CustomerSegment | Müşteri segmenti| 
| CustomerMarket | Müşterinin pazarının coğrafi ülke konumu| 
| MPNId | Microsoft İş Ortağı Ağı kimliği| 
| PartnerName | İş ortağının adı| 
| PartnerLocation | İş ortağının coğrafi konumu| 
| PartnerAttributionType | İş ortağının atfı türü| 
| PartnerHierarchy| İş ortağı hiyerarşisi (Sanal Kuruluş veya HeadQuarters veya Konum)| 
| PaidAvailableUnits | Ücretli kullanılabilir birimlerin sayısı| 
| MonthlyActiveUsers | Aylık etkin kullanıcı sayısı| 
| AATPActiveUsage| Azure Gelişmiş Tehdit Koruması (AATP) etkin kullanımı| 
| MCASActiveUsage| MCAS etkin kullanımı| 
| AADPPaidAvailableUnits| Azure Active Directory Premium (AADP) için ücretli kullanılabilir birim sayısı| 
| IntunePaidAvailableUnits| Intune için ücretli kullanılabilir birim sayısı| 
| AzipPaidAvailableUnits| Azip için ücretli kullanılabilir birim sayısı| 
| AADPMonthlyActiveUsers| Azure Active Directory Premium (AADP) için aylık etkin kullanıcı sayısı| 
| IntuneMonthlyActiveUsers| Intune için aylık etkin kullanıcı sayısı| 
| AzipMonthlyActiveUsers| Azip için aylık etkin kullanıcı sayısı| 
| MDM| MDM| 
| MAM| MAM| 
| SSPR| SSPR| 

### <a name="dynamics-365-license-usage-report"></a>**Dynamics 365 lisans kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| PGAMpnId | İş ortağı genel hesabı MPN'lerinin tanımlayıcısı | 
| kaynak grubundaki | Aboneliğin GUID'si | 
| SubscriptionStartDate | Aboneliğin başlangıç tarihi | 
| SubscriptionEndDate | Aboneliğin bitiş tarihi | 
| SubscriptionStatus | Aboneliğin durumu | 
| Ay | Kullanımın raporlandığı ay | 
| RevSumDivisionName | Rev sum bölümü adı | 
| RevSumCategoryName | Rev sum kategorisinin adı | 
| SKU | Ürünün SKU'su | 
| SKUId | Ürünün SKU kimliği | 
| FreeVsPaidSKU | Bunun ücretsiz mi yoksa ücretli bir SKU mu olduğunu gösterir | 
| SalesModel | Aboneliğin satışı için kullanılan satış kanalı | 
| DetailedSalesModel | Abonelik için ayrıntılı satış modeli | 
| CustomerName | Müşterinin adı | 
| CustomerTenantId | Müşteri kiracısı GUID'si | 
| CustomerTpid | Müşteri üst üst tanımlayıcısı | 
| CustomerSegment | Müşterinin pazar segmenti | 
| CustomerMarket | Müşterinin coğrafi pazar | 
| MPNId | Microsoft İş Ortağı Ağı | 
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
| kaynak grubundaki | Aboneliğin GUID'si | 
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
| MPNId | Microsoft İş Ortağı Ağı | 
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
| Toplantı süresi | Saat olarak toplam toplantı süresi | 

### <a name="teams-monthly-usage-report"></a>**Teams kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| PGAMpnId |    İş ortağı genel hesabı MPN'lerinin tanımlayıcısı |
| CustomerTenantId |    Müşterinin Kiracı Kimliği|
| CustomerId |  Müşterinin üst üst öğenin tanımlayıcısı|
| MonthKey |    Kullanımın raporlandığı ay|
| SubWorkload | Kullanımın raporlandığı alt iş yükü (Toplantılar, aramalar veya telefon sistemleri)|
| MasaüstüKullanıcıları |    Masaüstünde kullanıcı Teams sayısı|
| MobileUsers | Mobil cihazlarda Teams kullanıcı sayısı|
| WebUsers |    Web'de Teams kullanıcı sayısı|
| AllUpParticipants |   Ayın benzersiz kullanıcı Teams sayısı|

### <a name="teams-usage-3p-apps-report"></a>**Teams 3P uygulamaları raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| PGAMpnId  | İş ortağı genel hesabı MPN'lerinin tanımlayıcısı |
| CustomerTenantId |    Müşterinin Kiracı Kimliği |
| CustomerId |  Müşteri üst üst kimliği |
| CustomerName |    Müşteri adı |
| CustomerCountry | Müşteri ülkesi |
| DateKey | Kullanımın raporlandığı tarih |
| Uygadı | Teams adı |
| Kullanıcı Sayısı |   Uygulama için kullanıcı sayısı |

### <a name="training-details-report"></a>**Eğitim ayrıntıları raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| PGAMpnId  | İş ortağı genel hesabı MPN'lerinin tanımlayıcısı |
| TrainingActivityId | Eğitimin tanımlayıcısı | 
| TrainingTitle | Eğitimin başlığı | 
| TrainingType | Eğitim türü (sertifikasyon veya sınav) | 
| IndividualFirstName | Müşterinin adı | 
| IndividualLastName | Müşterinin soyadı | 
| E-posta | Müşterinin kişisel e-posta kimliği | 
| CorpEmail | Office e-posta kimliğini girin | 
| TrainingCompletionDate | Eğitimin tamamlanma tarihi | 
| ExpirationDate |  Sertifikasyon son kullanma tarihi|
| ActivationStatus |    Sertifikasyon durumu|
| Ay | Verilerin raporlandığı ay | 
| IcMCP | Kullanıcının Bir Microsoft Certified Professional (MCP) olup olmadığını gösterir | 
| MCPID | Kullanıcının MCP kimliği | 
| MPNId | Microsoft İş Ortağı Ağı | 
| PartnerName | İş ortağının adı | 
| PartnerCityLocation | İş ortağının coğrafi şehir konumu | 
| PartnerCountryLocation | İş ortağının coğrafi ülke konumu | 

### <a name="microsoft-learn-report"></a>**Microsoft Learn raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| PGAMpnId  | İş ortağı genel hesabı MPN'lerinin tanımlayıcısı |
| UserName | Kullanıcının adı | 
| UserId | Kullanıcının GUID'si | 
| TrainingName | Eğitimin adı | 
| TrainingType | Eğitim türü (modül veya öğrenme yolu) | 
| Ürünler | Öğrenme modülünün geçerli olduğu ürün | 
| Roller | Eğitimin geçerli rolleri | 
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
| Cloud Ascent eğilimini-<10 lisanslarıyla uzak Iş yerinde alımı (geçerli sürüm) etkinleştirin | geçerli bir şirket içi Office veya Windows istemcisine sahip olan müşteri (yani, eol 'tan sonraki bir sürüm). Müşterinin 10 ' dan az lisansı vardır. Eğilimini puanı olan müşteri. İş ortağı, Microsoft 365 dönüştürme için hedef almalıdır. | 
| Bulutu olmadan uzak Iş yerinde alımı (geçerli sürüm) etkinleştir eğilimini-+ 10 lisansı | geçerli bir şirket içi Office veya Windows istemcisine sahip olan müşteri (yani, eol 'tan sonraki bir sürüm). Müşterinin 10 veya daha fazla lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, Microsoft 365 dönüştürme için hedef almalıdır. | 
| Bulut olmadan uzak Iş-şirket içi alımı (geçerli sürüm) etkinleştir eğilimini-<10 lisans | geçerli bir şirket içi Office veya Windows istemcisine sahip olan müşteri (yani, eol 'tan sonraki bir sürüm). Müşterinin 10 ' dan az lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, Microsoft 365 dönüştürme için hedef almalıdır. | 
| Cloud Ascent eğilimini-+ 10 lisanslarıyla uzaktan Iş yerinde alımı (EOL sürümü) etkinleştirin | bir eol şirket içi Office veya Windows istemcisi (yani, bir eol sürümü veya daha eski) olan müşteri. Müşterinin 10 veya daha fazla lisansı vardır. Müşterinin bir eğilimini puanı vardır. İş ortağı, Microsoft 365 dönüştürme için hedef almalıdır. | 
| Cloud Ascent eğilimini-<10 lisanslarıyla uzak Iş yerinde alımı (EOL sürümü) etkinleştirin | bir eol şirket içi Office veya Windows istemcisi (yani, bir eol sürümü veya daha eski) olan müşteri. Müşterinin 10 ' dan az lisansı vardır. Müşterinin bir eğilimini puanı vardır. İş ortağı, Microsoft 365 dönüştürme için hedef almalıdır. | 
| Cloud Ascent eğilimini-+ 10 lisansı olmadan uzak Iş yerinde alımı (EOL sürümü) etkinleştir | geçerli bir şirket içi Office veya Windows istemcisine (yani, bir eol sürümü veya daha eski) sahip olan müşteri. Müşterinin 10 veya daha fazla lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, Microsoft 365 dönüştürme için hedef almalıdır. | 
| Buluttan uzak Iş-şirket içi alımı (EOL sürümü) etkinleştir eğilimini-<10 lisans | geçerli bir şirket içi Office veya Windows istemcisine (yani, bir eol sürümü veya daha eski) sahip olan müşteri. Müşterinin 10 ' dan az lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, Microsoft 365 dönüştürme için hedef almalıdır. | 
| Microsoft 365 için uzak çalışmayı etkinleştirme-yüksek-eğilimini aday (sahne NowithEvaluate) | Microsoft 365 için yüksek eğilimini aday aday müşteri | 
| Microsoft 365 ile uzak çalışmayı etkinleştirin (yakınlaştırma) | yakınlaştırma ve Microsoft 365 olan müşteri, Teams dönüştürme hedefi | 
| Microsoft 365 olmadan uzak çalışmayı (yakınlaştırma) etkinleştir | Yakınlaştırma özellikli müşteri, Teams dönüştürme hedefi | 
| Microsoft 365 E5 için hedeflenen maliyeti ve yönetimi Microsoft 365 E3 azaltma | Microsoft 365 E3, Microsoft 365 E5 hedefi olan mevcut müşteri | 
| Microsoft 365 İş Ekstra için hedeflenen maliyet ve yönetim Microsoft 365 İş Temel ve iş standart müşterilerini azaltma | mevcut Microsoft 365 İş Temel ve iş standart müşterileri, Microsoft 365 İş Ekstra için hedef | 
| Kuruluş üretkenliğini dönüştürme-Surface eğilimini | Müşteri, yüzey için bir eğilimini gösterir | 
| M365Cluster | Microsoft 365 satın almak için müşterinin eğilimini tanımlar. Hedef şimdi çalışır ve daha yüksek verim üretebilmeleri için kümeleri değerlendirir. Yalnızca Şimdi hareket eden ve müşterilerin hedeflediği bir kapasite varsa müşterileri Eğtir ve müşterileri eğitin. | 
| M365Fit | Firmografları tanımlayan iç ve dış veri noktaları. Kullanım Puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünlerine yönelik potansiyel bir uyum olup olmadığını görmek için en iyi küçük veya orta ölçekli işletmelere (SMB 'ler) bir gevmüike modeli kullanır. Skor, üç aylık olarak güncelleştirilir. | 
| M365Intent | Sosyal medya ve müşterinin çevrimiçi davranışı ile ilgili sinyaller amaç tanımlar. Amaç Puanlama, kümeleri tanımlamak için uygun şekilde yer alır. Amaç Puanlama aylık olarak güncelleştirilir. | 
| SurfaceCluster | Bir kümeye sığdırma ve amaç önerilerini birleştirerek bir müşterinin eğilimini ' i, yüzeyi satın almasını belirler. Hedef şimdi çalışır ve daha yüksek verim üretebilmeleri için kümeleri değerlendirir. Yalnızca Şimdi hareket eden ve müşterilerin hedeflediği bir kapasite varsa müşterileri Eğtir ve müşterileri eğitin. | 
| Surçok yönlü sığdırma | Firmografları tanımlayan iç ve dış veri noktaları. Kullanım Puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünleri için olası bir uyum olup olmadığını görmek için en iyi SMB kuruluşlarımızda bir gevmüike modeli kullanır. Skor, üç aylık olarak güncelleştirilir. | 
| Surçok yönlü amaç | Sosyal medya ve müşterinin çevrimiçi davranışı ile ilgili sinyaller amaç tanımlar. Amaç Puanlama, kümeleri tanımlamak için uygun şekilde yer alır. Amaç Puanlama aylık olarak güncelleştirilir. | 
| O365Cluster | Office 365 satın almak için müşterinin eğilimini tanımlar. Hedef şimdi çalışır ve daha yüksek verim üretebilmeleri için kümeleri değerlendirir. Yalnızca Şimdi hareket eden ve müşterilerin hedeflediği bir kapasite varsa müşterileri Eğtir ve müşterileri eğitin. | 
| O365Fit | Firmografları tanımlayan iç ve dış veri noktaları. Kullanım Puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünleri için olası bir uyum olup olmadığını görmek için en iyi SMB kuruluşlarımızda bir gevmüike modeli kullanır. Skor, üç aylık olarak güncelleştirilir. | 
| O365Intent | Sosyal medya ve müşterinin çevrimiçi davranışı ile ilgili sinyaller amaç tanımlar. Amaç Puanlama, kümeleri tanımlamak için uygun şekilde yer alır. Amaç Puanlama aylık olarak güncelleştirilir. | 
| M365UpsellCustomer | Müşterinin Microsoft 365 için büyük satış eğilimini gösterilip gösterilmeyeceğini belirler | 
| Google 'a sahiptir | Müşterinin sahip olduğu Google ürünleri için rekabet sinyalleri gösterilip gösterilmeyeceğini belirler | 
| AWS 'ye sahip | Müşterinin sahip Amazon Web Services (AWS) ürünleri için rekabet sinyalleri gösterilip gösterilmeyeceğini belirler | 
| EA 'ya sahiptir | Bir yenilemenin bir kurumsal anlaşma (EA) veya EA aboneliği olup olmadığını belirler | 
| Açık | Bir yenilemenin açık veya açık bir değer anlaşması olup olmadığını belirler | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Bulut Yokent-Dynamics 365 eğilimini raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| MPN Kimliği | Microsoft İş Ortağı Ağı (MPN) KIMLIĞI | 
| İş ortağı adı | Ortağın adı | 
| Müşteri Kimliği | Müşteri tanımlayıcı numarası | 
| DYENIDEN sayı | Dun & Bradstreet, eğilimini için puanlanmakta olan müşterinin numarası | 
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
| D365FOIntent | Sosyal medya ve müşterinin çevrimiçi davranışıyla ilgili sinyaller Amacı tanımlar. Amaç puanlama, kümeleri tanımlamak için Sığdır'ın üzerine atlar. Amaç puanlama aylık olarak güncelleştirilir. | 
| D365CECluster | Müşterinin Dynamics 365 Customer Engagement satın alma eğilimini tanımlar. Customer Engagement için bir teklifte yer alan müşteriler Orta ve Küçük kategorilerde yer atılır. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| D365CEFit | Dynamics 365 Customer Engagement için Uygun olduğunu gösterir | 
| D365CEIntent | Dynamics 365 Müşteri Etkileşimi amacını gösterir | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Müşterinin Dynamics şirket içi AX veya CRM için açık yenilemeye sahip olup olmadığını tanımlar | 
| M365UpsellCustomer | Müşterinin sipariş için satış eğilimi gösterip Microsoft 365 | 
| Google'a sahip | Müşterinin Google ürünlerine sahip olmak için rekabet sinyalleri gösterip gösterip gösterir olmadığını tanımlar | 
| AWS'ye sahip | Müşterinin sahip olduğu AWS ürünleri için rekabet sinyalleri gösterip gösterip gösterir | 
| EA'ya sahip | Yenilemenin EA aboneliği mi yoksa EA aboneliği mi olduğunu tanımlar | 
| Açık | Yenilemenin Açık veya Açık Değer sözleşmesi olup olmadığını tanımlar | 

### <a name="cloud-ascent---azure-propensity-report"></a>**Bulut Ascent - Azure eğilimi raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| MPN Kimliği | Microsoft İş Ortağı Ağı (MPN) Kimliği | 
| İş Ortağı Adı | İş ortağının adı | 
| Müşteri Kimliği | Müşteri tanımlayıcı numarası | 
| DUNS Numarası | Dun &, yayma puanı alan müşterinin Bradstreet numarasını aldı | 
| Hesap Adı | Hesabın adı | 
| Etki alanı | Hesabın etki alanı | 
| Kuruluş Boyutu | Kuruluşun boyutu | 
| Sektör | Sektör | 
| Dikey | Microsoft, D&B ve diğer sektör standartları tarafından belirlenerek, yayma puanı alan müşterinin dikeyi | 
| Alan | Konumun coğrafi alanı | 
| Yan Kuruluş | Teklif puanı alan müşterinin yan kuruluşu | 
| Sales Territory | Yayma puanı alan müşterinin satış bölgesi | 
| Şehir | Coğrafi şehir konumu | 
| Durum | Coğrafi durum konumu | 
| Posta Kodu | Kuruluşun posta kodu | 
| Ülke | Coğrafi ülke konumu | 
| Segment | Pazar segmenti | 
| Alt Kesim | Pazar alt | 
| SMC türü Özet | SMC türü | 
| En İyi Unmanaged - İşlem Tabanı | En çok kontrol dışı olan müşteriler – işlem | 
| En İyi Unmanaged - Kullanıcı Tabanı | En iyi unmanaged müşterileri – kullanıcılar | 
| IsNonProfit | Kuruluşun kar amacı gütmeyen kuruluş olup olmadığını gösterir (Evet veya Hayır) | 
| Geçiş - EOL Windows Sunucusu - EOL Windows Bulut Ascent eğilimine sahip Sunucu IB -5+ lisans | Şirket içi bir EOL sunucusuna sahip Windows (yani, bir EOL sürümü veya daha önceki bir sürüm). Müşterinin 5 veya daha fazla lisansı vardır. Teklif puanına sahip olan müşteri. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL Windows Sunucusu - EOL Windows Bulut Ascent eğilimine sahip Sunucu IB'leri - <5 lisans | Şirket içi bir EOL sunucusuna sahip Windows (yani, bir EOL sürümü veya daha önceki bir sürüm). Müşterinin 5'ten az lisansı vardır. Teklif puanına sahip olan müşteri. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL Windows Sunucusu - EOL Windows Bulut Ascent eğilimi olmadan Sunucu IB 'leri - 5+ lisans | Şirket içi bir EOL sunucusuna sahip Windows (yani, bir EOL sürümü veya daha önceki bir sürüm). Müşterinin 5'in üzerinde lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL Windows Sunucusu - EOL Windows Bulut Ascent eğilimi olmadan Sunucu IB -<5 lisans | Şirket içi bir EOL sunucusuna sahip Windows (yani, bir EOL sürümü veya daha önceki bir sürüm). 5'ten az lisansa sahip. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL SQL - Bulut SQL Server ile EOL depolama IB - 5'ten fazla lisans | Şirket içi bir EOL sürümüne sahip olan SQL Server (yani, bir EOL sürümü veya daha önceki bir sürüm). Müşterinin 5'den fazla lisansı vardır. Müşterinin bir yayma puanı vardır. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL SQL - Bulut SQL Server eğilimi olan EOL <IB - <5 lisans | Şirket içi bir EOL sürümüne sahip olan SQL Server (yani, bir EOL sürümü veya daha önceki bir sürüm). 5'ten az lisansa sahip. Teklif puanına sahip olan müşteri. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL SQL - Bulut SQL Server olmadan EOL SQL Server IB - 5'ten fazla lisans | Şirket içi bir EOL sürümüne sahip olan SQL Server (yani, bir EOL sürümü veya daha önceki bir sürüm). Müşterinin 5 veya daha fazla lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL SQL - Bulut SQL Server eğilimi olmadan EOL SQL Server IB - <5 lisans | Şirket içi bir EOL sürümüne sahip olan SQL Server (yani, bir EOL sürümü veya daha önceki bir sürüm). Müşterinin 5'ten az lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçirme - Şirket içi Windows Sunucusunu geçirme - geçerli Windows Bulut Tabanlı Sunucu IB - 5'den fazla lisans | Geçerli şirket içi sunucu sunucusuna sahip Windows (yani, EOL'den sonraki bir sürüm). Müşterinin 5'den fazla lisansı vardır. Müşterinin bir yayma puanı vardır. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Şirket içi Windows Sunucusunu geçirme - geçerli Windows Bulut Ascent eğilimi ile Sunucu IB - <5 lisans | Geçerli şirket içi sunucu sunucusuna sahip Windows (yani, EOL'den sonraki bir sürüm). Müşterinin 5'ten az lisansı vardır. Müşterinin Azure için bir teklif puanı vardır. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçirme - Şirket içi Windows Sunucusunu geçirme - geçerli Windows Bulut Ascent eğilimi olmadan Sunucu IB - 5'den fazla lisans | Geçerli şirket içi sunucu sunucusuna sahip Windows (yani, EOL'den sonraki bir sürüm). Müşterinin 5'den fazla lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Şirket içi Windows Sunucusunu geçirme - geçerli Windows Bulut Ascent eğilimi olmadan Sunucu IB - <5 lisans | Geçerli şirket içi sunucu sunucusuna sahip Windows (yani, EOL'den sonraki bir sürüm). Müşterinin 5'ten az lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Azure SQL veya SQL sanal makinelere (VM) geçiş - Bulut SQL Server sahip geçerli sanal makine IB - 5'den fazla lisans | Geçerli bir şirket içi bulut hizmetine sahip SQL Server (başka bir ifadeyle, EOL'den sonraki bir sürüm). Müşterinin 5'den fazla lisansı vardır. Müşterinin bir yayma puanı vardır. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Azure SQL veya SQL VM'lere geçiş - Bulut SQL Server eğilimi ile geçerli SQL Server IB - <5 lisans | Geçerli bir şirket içi bulut hizmetine sahip SQL Server (başka bir ifadeyle, EOL'den sonraki bir sürüm). Müşterinin 5'ten az lisansı vardır. Müşterinin bir yayma puanı vardır. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Azure SQL veya SQL VM'lere geçiş - Bulut SQL Server olmadan geçerli sanal SQL Server IB - 5'den fazla lisans | Geçerli bir şirket içi bulut hizmetine sahip SQL Server (başka bir ifadeyle, EOL'den sonraki bir sürüm). Müşterinin 5'den fazla lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Azure SQL veya SQL VM'lere geçiş - Bulut SQL Server eğilimi olmadan geçerli <IB - <5 lisans | Geçerli bir şirket içi bulut hizmetine sahip SQL Server (başka bir ifadeyle, EOL'den sonraki bir sürüm). Müşterinin 5'ten az lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - OSS - Açık Kaynak (OSS) DB'ye Geçiş | Şu ürünlerden herhangi birini alan mevcut müşteri: PostgreSQL, MySQL, MariaDB. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - OSS - Azure'da Linux | Linux'a sahip mevcut müşteri. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçirme - SAP - Azure üzerinde SAP | SAP ile mevcut müşteri. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Windows Sanal Masaüstü - Uzak Masaüstü Hizmetleri IB | Etkin verilerle müşterileri Windows Uzak Masaüstü Hizmetleri. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Windows Sanal Masaüstü - Modern Çalışmaları Azure'a Çapraz Satış/WVD | Azure'Microsoft 365 sahip olmayan müşterileri tanımlar. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - VMware IB | Ürüne sahip mevcut müşteri: VMware. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçirme - Citrix IB | Ürünü olan mevcut müşteri: Citrix Systems. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Yenilik - Analiz - Power BI Azure eğilimine sahip IB'ler | Ve Etkin Power BI aboneliğine sahip müşteriler: Power BI - Tek başına Pro, Power BI - Azure Paketleri, Power BI - Office Paketleri, Power BI Paketleri - Microsoft 365 | 
| Etkinleştirme - DevOps ile GitHub - Visual Studio/MSDN IB | Etkin sürümlere sahip Visual Studio tanımlar | 
| Windows Sunucu Standart sürümü | Müşteri tarafından Windows Server Standard satın almalarının sürümünü görüntüler | 
| Windows Sunucu Standart lisansı | Müşterinin Windows Server Standard satın almalarının lisans türünü görüntüler | 
| Windows Sunucu Veri Merkezi sürümü | Müşteri tarafından Windows Veri Merkezi satın almalarının sürümünü görüntüler | 
| Windows Sunucu Veri Merkezi Lisansı | Müşterinin Veri Merkezi Windows lisans türünü görüntüler | 
| AzureFit | Sıkı grafiği tanımlayan iç ve dış veri noktaları. Uygun puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünlerine potansiyel olarak uygun olup olmadığını görmek için en iyi SMB'mize benzer bir model kullanır. Fit puanlama üç aylık olarak güncelleştirilir. | 
| AzureIntent | Sosyal medya ve müşterinin çevrimiçi davranışıyla ilgili sinyaller Amacı tanımlar. Amaç puanlama, kümeleri tanımlamak için Sığdır'ın üzerine atlar. Amaç puanlama aylık olarak güncelleştirilir. | 
| AzureCluster | Fit ve Intent önerilerini bir kümede bir arada kullanarak müşterinin Azure satın alma eğilimini tanımlar. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| WindowsServerDataCenter_HasOpenRenewal | Müşterinin Windows Server Datacenter için açık yenilemeye sahip olup olmadığını tanımlar | 
| WindowsServerStandard_HasOpenRenewal | müşterinin Windows Server Standard için açık yenileme olup olmadığını belirler | 
| AzureUpsellCustomer | Müşterinin Azure için büyük satış eğilimini göstermeyeceğini belirler | 
| Google 'a sahiptir | Müşterinin sahip olduğu Google ürünleri için rekabet sinyalleri gösterilip gösterilmeyeceğini belirler | 
| AWS 'ye sahip | Müşterinin sahip olduğu AWS ürünleri için rekabet sinyalleri gösterilip gösterilmeyeceğini belirler | 
| EA 'ya sahiptir | Bir yenilemenin EA veya EA aboneliği olup olmadığını belirler | 
| Açık | Bir yenilemenin açık veya açık bir değer anlaşması olup olmadığını belirler | 

### <a name="cloud-ascent---agreement-renewal-propensity-report"></a>**Bulut yokuş-anlaşma yenileme eğilimini raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| MPN Kimliği | Microsoft İş Ortağı Ağı KIMLIĞI | 
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
| Google 'a sahiptir | Müşterinin sahip olduğu AWS ürünleri için rekabet sinyalleri gösterilip gösterilmeyeceğini belirler | 
| AWS 'ye sahip | Müşterinin sahip olduğu AWS ürünleri için rekabet sinyalleri gösterilip gösterilmeyeceğini belirler | 
| Azure kümesi | Azure 'ı satın almak için müşterinin eğilimini tanımlar. Hedef şimdi çalışır ve daha yüksek verim üretebilmeleri için kümeleri değerlendirir. Yalnızca Şimdi hareket ettikten ve müşterileri değerlendirdikten sonra hala kapasite varsa müşterileri Eğtir ve müşterileri eğitin. | 
| D365 finans + Operations kümesi | Dynamics 365 finans ve Işlemlerini satın almak için müşterinin eğilimini tanımlar. Finans + Işlemlerine yönelik bir eğilimini gösteren müşteriler, en üstteki yönetilmeyen kategorilerde yer alacak. Hedef şimdi çalışır ve daha yüksek verim üretebilmeleri için kümeleri değerlendirir. Yalnızca Şimdi hareket ettikten ve müşterileri değerlendirdikten sonra hala kapasite varsa müşterileri Eğtir ve müşterileri eğitin. | 
| D365 CE kümesi | Dynamics 365 müşteri katılımı satın almak için müşterinin eğilimini tanımlar. Müşteri katılımı için bir eğilimini gösteren müşteriler orta ve küçük kategorilerde olacaktır. Hedef şimdi çalışır ve daha yüksek verim üretebilmeleri için kümeleri değerlendirir. Yalnızca Şimdi hareket ettikten ve müşterileri değerlendirdikten sonra hala kapasite varsa müşterileri Eğtir ve müşterileri eğitin. | 
| D365 BC kümesi | Dynamics 365 Business Central satın almak için müşterinin eğilimini tanımlar. Eğilimini for Business Central 'ı gösteren müşteriler orta ve küçük kategorilerde olacaktır. Hedef şimdi çalışır ve daha yüksek verim üretebilmeleri için kümeleri değerlendirir. Yalnızca Şimdi hareket ettikten ve müşterileri değerlendirdikten sonra hala kapasite varsa müşterileri Eğtir ve müşterileri eğitin. | 
| Microsoft 365 İçi | Microsoft 365 satın almak için müşterinin eğilimini tanımlar. Hedef şimdi çalışır ve daha yüksek verim üretebilmeleri için kümeleri değerlendirir. Yalnızca Şimdi hareket ettikten ve müşterileri değerlendirdikten sonra hala kapasite varsa müşterileri Eğtir ve müşterileri eğitin. | 
| Lisans programı | Yenileme için lisans programı türünü tanımlar | 
| Anlaşma KIMLIĞI | Sözleşmenin tanımlayıcısı | 
| Anlaşma bitiş tarihi | Sözleşmenin bitiş tarihi | 
| Sona erme türü | Süre sonu türü | 
| Süresi dolan gelir | Süresi dolan aboneliklerle ilişkili gelir | 
| EA 'ya sahiptir | Bir yenilemenin EA veya EA aboneliği olup olmadığını belirler | 
| Açık | Bir yenilemenin açık veya açık bir değer anlaşması olup olmadığını belirler | 
| Azure büyük satış müşterisi | Müşterinin Azure için büyük satış eğilimini göstermeyeceğini belirler | 
| Microsoft 365 Büyük satış müşterisi | Müşterinin Microsoft 365 için büyük satış eğilimini gösterilip gösterilmeyeceğini belirler | 
| RevSumDivisionName | Yenilemeye yönelik ürünü tanımlar | 

### <a name="cpor-m365usage-report"></a>**CPOR-M365Usage raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| CustomerTenantId | Müşterinin Kiracı kimliği | 
| CustomerName | Müşterinin adı | 
| WorkloadName | İş yükünün adı | 
| MonthlyActiveUsers | MAU (aylık etkin kullanıcılar) | 
| Paidavvailableunits | PAU (ücretli kullanılabilir birimler) | 
| Claimıd | İş yükünün talep KIMLIĞI | 
| Mpnıd | Microsoft İş Ortağı Ağı (MPN) KIMLIĞI | 
| Dateiliþkilendirilmiþ | Ortak iş yükünün ilişkili tarihi | 
| PartnerAttributionType | İş ortağı Attributıon türü (CPOR) | 
| Tarih | Verilerin verildiği tarih (ilk ay ve yıl) | 

## <a name="next-steps"></a>Sonraki adımlar

Daha fazla bilgi için bkz. [raporları indirme](insights-download-reports.md).
