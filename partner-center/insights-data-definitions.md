---
title: İçgörü verilerinin tanımları
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: belge, Analizler indirme raporu sayfasından indirebileceğiniz çeşitli raporlar ve veri tanımlarını listeler.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 92733f11713e8c16d607a51ef00efdcc25ddc855
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960874"
---
# <a name="export--data-definitions"></a>Dışarı aktarma – veri tanımları 

**Uygun roller**: rapor Görüntüleyici | Executive rapor Görüntüleyicisi

## <a name="introduction"></a>Giriş 

Analizler panosunda raporları indir merkezini kullanarak ham veri kümelerini dışarı aktarabilirsiniz. 

Veri tanımlarıyla birlikte indirebileceğiniz çeşitli raporlar aşağıdaki tablolarda listelenmiştir: 

### <a name="partner-profile-report"></a>**İş ortağı profili raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| Mpnıd | Microsoft İş Ortağı Ağı (MPN) KIMLIĞI| 
| PartnerName | Ortağın adı | 
| PGA_MPNId | Ortak küresel hesap MPN tanımlayıcısı | 
| PGA_PartnerName | Ortak genel hesap adı | 
| Şehir | Ortağın şehir konumu | 
| Ülke | Ortağın ülke konumu | 
| HierarchyLevel | Küresel bir MPN KIMLIĞI veya konum MPN KIMLIĞI olup olmadığını belirtir | 

### <a name="customer-details-report"></a>**Müşteri Ayrıntıları raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| Pgampnıd| Ortak küresel hesap MPN tanımlayıcısı|
| CustomerName| Müşterinin adı|
| CustomerTenantId| Müşteri kiracının tanımlayıcısı|
| Customertpıd| Müşteri üst üst öğesinin tanımlayıcısı|
| DUNSNumber|   Küresel veri evrensel sayı sistem tanımlayıcısı|
| CustomerSegment | Müşteri kesimi|
| TopSegment    | Müşterinin daha yüksek düzey segment sınıflandırması|
| CustomerMarket|   Müşterinin coğrafi pazarı|  
| CustomerStatus    | Müşteri durumu (etkin veya etkin değil)| 
| CustomerTenantName|   Müşteri kiracının adı|
| CustomerTenantCountry|    Müşteri kiracının ülkesi|
| Kiracıetkialanıadı| Müşteri kiracının etki alanı adı|
| Ürün|  mpn: O365, Dynamics 365, Enterprise Mobility + Security, Power BI veya Microsoft Azure tarafından müşteriye satılan ürün.|
| RawProductName|   Müşteriye satılan ayrıntılı ürün adı|
| SKU|  Ürün SKU 'SU|
| Ay|    Kullanım ve gelirin bildirildiği ay|
| Mpnıd|    Microsoft İş Ortağı Ağı tanımlayıcısı (MPN)|
| PartnerName|  Ortağın adı|
| PartnerLocation|  İş ortağının coğrafi konumu|
| PartnerAttributionType|   Ortağın atısyon türü| 
| SalesChannel| Satış kanalı|
| Iduplicaterowforpga| Tek PGA altında birden fazla iş ortağı tanımlayıcısı için, bu değer yalnızca bir MPNId için 0 olarak ayarlanır. Değer 1 olarak ayarlanırsa, yinelenen bir satırı gösterir|
| Availablekoltuk|   Kullanılabilir koltuk|
| BilledRevenueUSD| ABD Doları cinsinden faturalandırılan gelir|
| AzureConsumedRevenueUSD|  Azure tüketilen gelir ABD Doları|

### <a name="reseller-performance-report"></a>**Satıcı performans raporu**

> [!Note]
> Gelir ve Azure tüketilen gelir (ACR) verileri yalnızca Executive rapor izleyicileri olan kullanıcılar tarafından kullanılabilir.

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| Pgampnıd | Ortak küresel hesap MPN tanımlayıcısı |
| Resellermpnıd | Satıcı Microsoft İş Ortağı Ağı tanımlayıcısı | 
| ResellerName | Satıcı adı | 
| ResellerMarket | Market Bayi ülkesi | 
| Indirectprovidermpnıd | Dolaylı sağlayıcının tanımlayıcısı Microsoft İş Ortağı Ağı | 
| Indirectprovidername | Dolaylı sağlayıcı adı | 
| Ay | Kullanım ve gelirin bildirildiği ay | 
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
>Gelir ve ACR verileri yalnızca Yönetici rapor görüntüleyicisi olan kullanıcılar tarafından kullanılabilir.

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
|AvailableSeats | Ay içinde kullanılabilen yer farkı|
|BilledRevenueUSD | ABD doları olarak gelir|
|AzureConsumedRevenueUSD| Azure Tüketim Geliri ABD doları|

### <a name="azure-usage-report"></a>**Azure kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
|PGAMpnId| İş ortağı genel hesabı MPN'lerinin tanımlayıcısı|
|SubscriptionId| Aboneliğin GUID'si|
|SubscriptionStartDate| Aboneliğin başlangıç tarihi|
|SubscriptionEndDate| Aboneliğin bitiş tarihi|
|FirstUseDate| Azure hizmetlerinin ilk kez kullanılma tarihi|
|SubscriptionState| Aboneliğin Geçerli Durumu (Açık, Kapalı Etkin veya Yetkisiz Kullanım Süresinde)|
|Ay| Aya göre toplanan tarih|
|ServiceLevel1| Hizmet Düzeyi 1 – Kapsayıcılar, Veritabanları, Ağ gibi Hizmet Sütunlarına karşılık gelir.|
|ServiceLevel2| Hizmet Düzeyi 2 – Hizmet Sütunu için İş Yüküne Karşılık GelenLer|
|ServiceLevel3| Azure tekliflerini listelerken Azure.Microsoft.Com tarafından kullanılan hizmet adı|
|ServiceLevel4| Üst düzey özellik kümelerinin mantıksal gruplamaları hizmet içindeki farkları ayarlama. Sanal Genel Amaçlı, Bellek için İyileştirilmiş Sanal Makineler, Tek SQL Veritabanı, Elastik SQL Veritabanı vb. |
|ServiceGroup2| AI, Uygulama Geliştirme, IoT gibi Alan Geliri Sorumluluk (FRA) alanları |
|ServiceGroup3| IoT FRA için IoT Hub, Haritalar gibi FRA için ek ayrıntı|
|ServiceInfluencer| Service Fabric, Azure Databricks, AKS gibi altyapı kaynaklarının tüketimini Azure Databricks PaaS hizmetleri.|
|ComputeOS| İşlem için İşletim Sistemi|
|ComputeCoreSoftware| İşlem Çekirdeği Yazılımı|
|UsageUnits| Faturalama döngüsü sırasında kullanılan birim sayısı|
|Kullanım Miktarı| Kaynağın kullanım miktarı|
|CustomerName| Müşterinin adı|
|CustomerTenantId| Müşterinin Kiracı Kimliği|
|CustomerTpid| Müşteri üst üst kimliği|
|CustomerSegment| Müşterinin segmenti|
|CustomerMarket| Müşterinin coğrafi pazar|
|MPNId| Microsoft İş Ortağı Ağı kimliği|
|PartnerName| İş ortağının adı|
|PartnerLocation| İş ortağının coğrafi ülke konumu|
|PartnerAttributionType| İş ortağının atfı|
|SalesChannel| Satış kanalı (Doğrudan/CSP, Dolaylı/CSP, Doğrudan ve diğer)  |
|EnrollmentNumber| Aboneliğin kayıt numarası |
|IsACRDuplicateAtPGALevel| Tek bir PGA altındaki birden çok iş ortağı atıbetleri için bu değer yalnızca bir MPNId için 0 olarak ayarlanır. Değer 1 olarak ayarlanırsa yinelenen bir satır gösterir|
|ResellerID| Kurumsal bayinin kimliği|
|ResellerName| Satıcı adı|
|AdminType| İş Ortağı Atfı Türü "İş Ortağı Yönetici Bağlantısı (PAL)" olduğunda bu sütun müşterinin aboneliğinde atanan rolü gösterir.|
|Associationtype| İlişki türü|
|MonthlySubscriptionLevelACR| Aylık Abonelik Düzeyi ACR|
|ACR_USD| ABD doları olarak Azure tarafından tüketilen gelir (ACR)|

### <a name="office-365-license-usage-report"></a>**Office 365 kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| PGAMpnId | İş ortağı genel hesabı MPN'lerinin tanımlayıcısı | 
| CustomerTenantId | Müşterinin kiracı kimliği | 
| CustomerTpid | Müşteri üst üst kimliği | 
| WorkloadName | Skype Kurumsal, Teams, Exchange Online | 
| Ay | Kullanımın raporlandığı ay | 
| PaidAvailableUnits | Ücretli kullanılabilir birimlerin sayısı | 
| MonthlyActiveUsers | Aylık etkin kullanıcı sayısı | 
| CustomerName | Müşterinin adı | 
| CustomerMarket | Müşterinin pazarının coğrafi ülke konumu | 
| CustomerSegment | Müşteri segmenti | 
| MPNId | Microsoft İş Ortağı Ağı tanımlayıcısı | 
| PartnerName | İş ortağının adı | 
| PartnerLocation | İş ortağının coğrafi konumu | 
| PartnerAttributionType | İş ortağının atfı | 
| IsDuplicateRowForPGA | Tek bir PGA altındaki birden çok iş ortağı atıbetleri için bu değer yalnızca bir MPNId için 0 olarak ayarlanır. Değer 1 olarak ayarlanırsa yinelenen bir satır gösterir|

### <a name="enterprise-mobility-license-usage-report"></a>**Enterprise Mobility lisans kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| PGAMpnId| İş ortağı genel hesabı MPN'lerinin tanımlayıcısı| 
| SubscriptionId | Aboneliğin GUID'si| 
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
| PartnerAttributionType | İş ortağının atfı| 
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
| SubscriptionId | Aboneliğin GUID'si | 
| SubscriptionStartDate | Aboneliğin başlangıç tarihi | 
| SubscriptionEndDate | Aboneliğin bitiş tarihi | 
| SubscriptionStatus | Aboneliğin durumu | 
| Ay | Kullanımın raporlandığı ay | 
| RevSumDivisionName | Rev sum bölümü adı | 
| RevSumCategoryName | Rev sum kategorisinin adı | 
| SKU | Ürünün SKU'su | 
| SKUId | Ürünün SKU kimliği | 
| FreeVsPaidSKU | Bunun ücretsiz mi yoksa ücretli bir SKU mu olduğunu gösterir | 
| SalesModel | Aboneliği satmakta kullanılan satış kanalı | 
| DetailedSalesModel | Abonelik için ayrıntılı satış modeli | 
| CustomerName | Müşterinin adı | 
| CustomerTenantId | Müşteri kiracının GUID 'SI | 
| Customertpıd | Müşteri üst üst öğe tanımlayıcısı | 
| CustomerSegment | Müşterinin pazar segmenti | 
| CustomerMarket | Müşterinin coğrafi pazarı | 
| Mpnıd | Microsoft İş Ortağı Ağı tanımlayıcısı | 
| PartnerName | Ortağın adı | 
| PartnerLocation | Ortağın coğrafi ülke konumu | 
| PartnerAttachType | Abonelik için attributıon türü | 
| Availablekoltuk |  Geçerli ücretli kullanılabilir koltuk|
| AssignedSeats |   Geçerli atanan koltuk|
| Activekoltuk | Geçerli etkin koltuk|
| DeploymentOpportunity |   Dağıtım fırsatı atanmamış lisans sayısıdır|
| Activeusage yüzdesi |  Kullanılabilir koltuk yüzdesi olarak geçerli etkin kullanım |

### <a name="power-bi-license-usage-report"></a>**Power BI lisansı kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| Pgampnıd | Ortak küresel hesap MPN tanımlayıcısı | 
| SubscriptionId | Aboneliğin GUID 'SI | 
| SubscriptionStartDate | Aboneliğin başlangıç tarihi | 
| SubscriptionEndDate | Aboneliğin bitiş tarihi | 
| Abonelik durumu | Aboneliğin durumu (etkin, etkin değil veya yetkisiz kullanım süresi) | 
| Ay | Aya göre toplanan Tarih | 
| SKU | Ürünün SKU 'SU | 
| SkuId | Ürünün SKU KIMLIĞI | 
| Freevspaıdsku | Ücretsiz veya ücretli SKU farklılama | 
| SalesModel | Aboneliği satmak için kullanılan satış modeli | 
| DetailedSalesModel | Abonelik için ayrıntılı satış modeli | 
| CustomerName | Müşterinin adı | 
| CustomerTenantId | Müşteri kiracının GUID 'SI | 
| Customertpıd | Müşteri üst üst öğesinin tanımlayıcısı | 
| CustomerSegment | Müşterinin pazar segmenti | 
| CustomerMarket | Müşterinin coğrafi pazarı | 
| Mpnıd | Microsoft İş Ortağı Ağı tanımlayıcısı | 
| PartnerName | Ortağın adı | 
| PartnerLocation | Ortağın coğrafi ülke konumu | 
| PartnerAttachType | Abonelik için attributıon türü | 
| İş ortağı hiyerarşisi |    İş ortağı hiyerarşisi (sanal kuruluş veya merkez veya konum)|
| Availablekoltuk |  Geçerli ücretli kullanılabilir koltuk|
| AssignedSeats |   Geçerli atanan koltuk|
| Activekoltuk | Geçerli etkin koltuk|
| DeploymentOpportunity |   Dağıtım fırsatı atanmamış lisans sayısıdır|
| Activeusage yüzdesi |  Kullanılabilir koltuk yüzdesi olarak geçerli etkin kullanım|

### <a name="teams-meetings-and-calls-report"></a>**Teams toplantılar ve çağrılar raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| Pgampnıd | Ortak küresel hesap MPN tanımlayıcısı | 
| CustomerTenantId | Müşterinin kiracı KIMLIĞI | 
| CustomerId | Müşteri üst üst öğesinin tanımlayıcısı | 
| DateKey | Kullanımın bildirildiği Tarih
| Alt iş yükü | Kullanım için raporlanan alt iş yükü (toplantılar, çağrılar veya telefon sistemleri) | 
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

### <a name="teams-usage-3p-apps-report"></a>**Teams kullanım 3P uygulamaları raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| PGAMpnId  | İş ortağı genel hesabı MPN'lerinin tanımlayıcısı |
| CustomerTenantId |    Müşterinin Kiracı Kimliği |
| CustomerId |  Müşteri üst üst kimliği |
| CustomerName |    Müşteri adı |
| CustomerCountry | Müşteri ülkesi |
| DateKey | Kullanımın raporlandığı tarih |
| Uygadı | Teams uygulamasının adı |
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
| MPNId | Microsoft İş Ortağı Ağı tanımlayıcısı | 
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
| MPNId | Kimlik Microsoft İş Ortağı Ağı | 
| PartnerName | İş ortağının adı | 
| Ülke | İş ortağının coğrafi ülke konumu | 

### <a name="competency-summary-and-history-report"></a>**Uzmanlık özeti ve geçmiş raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| CompetencyName | Uzmanlığın adı | 
| CompetencyLevel | Uzmanlık düzeyi (Altın veya Gümüş) | 
| CompetencyStatus | Uzmanlığın geçerli durumu (Etkin, Etkin Değil veya Yetkisiz Kullanım Süresinde) | 
| CompetencyStartDate | Uzmanlığın başlangıç tarihi | 
| CompetencyEndDate | Uzmanlığın bitiş tarihi | 

### <a name="competency-performance-report"></a>**Uzmanlık performans raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| CompetencyName | Uzmanlığın adı | 
| CompetencyAttainmentOptionName | Yetkinlik elde etme seçeneğinin adı | 
| Ay | Ölçümlerin raporlandığı ay | 
| MetricName | Uzmanlıkla ilgili ölçümün adı | 
| MetricMonthlyContribution | Ölçümün aylık katkısı | 
| TTMAggregate | Sonda 12 ay için toplu ölçüm | 
| AnniversaryYearAggregate | Geçerli yıl dönümü için toplu ölçüm | 
| GoldThreshold | Gold uzmanlığını karşılamak için performans gereksinimi | 
| SilverThreshold | Silver yetkinliğine uygun performans gereksinimi | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**Bulut Ascent - Microsoft 365 raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| MPN Kimliği | Microsoft İş Ortağı Ağı kimliği | 
| İş Ortağı Adı | İş ortağının adı | 
| Müşteri Kimliği | Müşterinin tanımlayıcı numarası | 
| DUNS Numarası | Dun & Bradstreet (D&B) sayısı | 
| Hesap Adı | Hesabın adı | 
| Etki alanı | Hesabın etki alanı | 
| Kuruluş Boyutu | Kuruluşun boyutu | 
| Sektör | Kuruluşun ait olduğu sektör | 
| Dikey | Microsoft, D&B ve diğer sektör standartları tarafından tanımlanan, yayma puanı alan müşterinin dikeyi | 
| Alan | Konumun coğrafi alanı | 
| Yan Kuruluş | Teklif puanı alan müşterinin yan kuruluşu | 
| Sales Territory | Yayma puanı alan müşterinin satış bölgesi | 
| Şehir | Kuruluşun coğrafi şehir konumu | 
| Durum | Kuruluşun coğrafi durum konumu | 
| Posta Kodu | Kuruluşun posta kodu | 
| Ülke | Kuruluşun coğrafi ülke konumu | 
| Segment | Pazar segmenti | 
| Alt Kesim | Pazar alt | 
| SMC Tür Özeti | SMC türü | 
| En İyi Unmanaged - İşlem Tabanı | En çok kontrol dışı olan müşteriler – işlem | 
| En İyi Unmanaged - Kullanıcı Tabanı | En iyi unmanaged customers – user | 
| IsNonProfit | Kuruluşun kar amacı gütmeyen kuruluş olup olmadığını gösterir (Evet veya Hayır) | 
| Uzaktan Çalışma Etkinleştirme - hedef Exchange Online | Etkin bir Exchange Online olan müşteriler, Microsoft 365'a Microsoft 365 | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi ile şirket içi alım (geçerli sürüm) - +10 lisans | Geçerli bir şirket içi müşterisi veya Office Windows müşteri. Başka bir ifadeyle, istemci sürümü bir yaşam sonu (EOL) sürümünden daha eskidir. Müşterinin 10 veya daha fazla lisansı vardır. Teklif puanına sahip olan müşteri. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi ile şirket içi alım (geçerli sürüm) - <10 lisans | Geçerli bir şirket içi istemciye sahip olan Office Windows (yani, EOL'den sonraki bir sürüm). Müşterinin 10'dan az lisansı vardır. Teklif puanına sahip olan müşteri. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi olmadan şirket içi alım (geçerli sürüm) - +10 lisans | Geçerli bir şirket içi istemciye sahip olan Office Windows (yani, EOL'den sonraki bir sürüm). Müşterinin 10 veya daha fazla lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi olmadan şirket içi alım (geçerli sürüm) - <10 lisans | Geçerli bir şirket içi istemciye sahip olan Office Windows (yani, EOL'den sonraki bir sürüm). Müşterinin 10'dan az lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi ile şirket içi alım (EOL sürümü) - +10 lisans | Şirket içi bir EOL veya Office Windows (yani, bir EOL sürümü veya daha önceki) olan müşteri. Müşterinin 10 veya daha fazla lisansı vardır. Müşterinin bir yayma puanı vardır. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi ile şirket içi alım (EOL sürümü) - <10 lisans | Şirket içi bir EOL veya Office Windows (yani, bir EOL sürümü veya daha önceki) olan müşteri. Müşterinin 10'dan az lisansı vardır. Müşterinin bir yayma puanı vardır. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi olmadan şirket içi alım (EOL sürümü) - +10 lisans | Geçerli bir şirket içi istemciye sahip olan Office Windows (yani, bir EOL sürümü veya daha önceki bir sürümü). Müşterinin 10 veya daha fazla lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi olmadan şirket içi alım (EOL sürümü) - <10 lisans | Geçerli bir şirket içi istemciye sahip olan Office Windows (yani, bir EOL sürümü veya daha önceki bir sürümü). Müşterinin 10'dan az lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştir - yüksek olasılık olasılığı Microsoft 365 (Act NowithEvaluate) | Müşteri adayları için yüksek Microsoft 365 | 
| Uzaktan Çalışma Etkinleştir - uzaktan çalışmayla rekabet Microsoft 365 | Yakınlaştırma ve yakınlaştırma özelliğine Microsoft 365 müşteri, hedef olarak Teams | 
| Uzaktan Çalışma Etkinleştirme - uzaktan çalışma olmadan rekabet Microsoft 365 | Yakınlaştırmalı müşteri, hedef hedef Teams | 
| Maliyet ve Yönetimi Azaltma - Microsoft 365 E3 için Microsoft 365 E5 | Mevcut müşteri Microsoft 365 E3, hedef Microsoft 365 E5 | 
| Maliyetleri ve Yönetimi Azaltma - Microsoft 365 İş Temel ve İş Standardı müşterileri Microsoft 365 İş Ekstra | Mevcut Microsoft 365 İş Temel ve İş Standardı müşterileri, Microsoft 365 İş Ekstra | 
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
| AWS'ye sahip | Müşterinin sahip olduğu ürünler (AWS) için rekabet Amazon Web Services gösterip gösterir | 
| EA'ya sahip | Yenilemenin kurumsal anlaşma (EA) veya EA aboneliği olup olmadığını tanımlar | 
| Açık | Yenilemenin Açık veya Açık Değer sözleşmesi olup olmadığını tanımlar | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Bulut Ascent - Dynamics 365 eğilimi raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| MPN Kimliği | Microsoft İş Ortağı Ağı (MPN) Kimliği | 
| İş Ortağı Adı | İş ortağının adı | 
| Müşteri Kimliği | Müşteri tanımlayıcı numarası | 
| DUNS Numarası | Dun &, yayma puanı alan müşterinin Bradstreet numarasını aldı | 
| Hesap Adı | Hesabın adı | 
| Etki alanı | Hesabın etki alanı | 
| Kuruluş Boyutu | Kuruluşun boyutu | 
| Sektör | Kuruluşun ait olduğu sektör | 
| Dikey | Microsoft, D&B ve diğer sektör standartları tarafından belirlenerek, yayma puanı alan müşterinin dikeyi
| Alan | Konumun coğrafi alanı | 
| Yan Kuruluş | Teklif puanı alan müşterinin yan kuruluşu | 
| Sales Territory | Yayma puanı alan müşterinin satış bölgesi | 
| Şehir | Coğrafi şehir konumu | 
| Durum | Coğrafi durum konumu | 
| Posta Kodu | Kuruluşun posta kodu | 
| Ülke | Coğrafi ülke konumu | 
| Segment | Pazar segmenti | 
| Alt Kesim | Pazar alt | 
| SMC Tür Özeti | Müşterinin kategorilere ayırması: En üst düzeydeki kullanıcı tabanı 300'den fazla çalışana sahip müşteriler, en iyi unmanaged işlem tabanı üç yıllık Azure'da 10.000 ABD doları potansiyele sahip müşteriler, orta ölçekli işletmeler 25 veya daha fazla çalışanı olan müşteriler ve küçük işletmeler ise 25'ten az çalışanı olan müşterilerdir. | 
| En İyi Unmanaged - İşlem Tabanı | En çok kontrol dışı olan müşteriler – işlem | 
| En İyi Unmanaged - Kullanıcı Tabanı | En çok kontrol dışı müşteriler – kullanıcılar | 
| IsNonProfit | Kuruluşun kar amacı gütmeyen bir kuruluş olup olmadığını gösterir (Evet veya Hayır) | 
| Dijital Satış etkinleştirme - Microsoft 365 - lisans boyutu >= 25 lisans (SalesPro eğilimi modeli) | Dynamics 365 olmayan müşteri. Seat size: 25+. İş ortağıNın Dynamics 365 SalesPro çapraz satışını hedeflemesi gerekir. | 
| Dijital Satışı Etkinleştirme - Dynamics 365 SalesPro eğilimi (Şimdi Harekete Geç veya Değerlendir) | Dynamics 365 olmayan yüksek performanslı müşteriler. İş ortağıNın Dynamics 365 SalesPro'ya yönelik hedefi olması gerekir. | 
| Finansal Risk Yönetimi & Sahtekarlık - Dynamics şirket içi yükleme tabanı - Navision (Business Central eğilimi modeli) | Şirket içi Navision'a sahip mevcut müşteri. İş ortağıNın Dynamics 365 Business Central'a yönelik hedefi olması gerekir. | 
| Finansal Risk Yönetimi & Sahtekarlık - Dynamics şirket içi yükleme tabanı - Dynamics AX (Dynamics 365 Finance + Operations propensity model) | Şirket içi AX'e sahip mevcut müşteri. İş ortağıNın Dynamics 365 Finance + Operations'i hedeflemesi gerekir. | 
| Finansal Risk Yönetimi & Sahtekarlık - Dynamics şirket içi yükleme tabanı - Great Plains (Business Central eğilimi modeli) | Şirket içi Great Plains'e sahip mevcut müşteri. İş ortağıNın Dynamics 365 Business Central'a yönelik hedefi olması gerekir. | 
| Finansal Risk Yönetimi & Sahtekarlık - Dynamics şirket içi yükleme tabanı - Dynamics (Business Central eğilimi modeli) | Şirket içi Hizmet Merkezi olan mevcut müşteri. İş ortağıNın Dynamics 365 Business Central'a yönelik hedefi olması gerekir. | 
| Finansal Risk Yönetimi & Sahtekarlık - Dynamics şirket içi yükleme tabanı - Diğer (Business Central eğilimi modeli) | Daha önce listelenmiyor olan diğer şirket içi çözümlere sahip mevcut müşteri. İş ortağıNın Dynamics 365 Business Central'a yönelik hedefi olması gerekir. | 
| Çevik İş Süreçleri Oluşturma - Dynamics şirket içi yükleme tabanı - AX/GP/SL/NAV/Diğer (Dynamics 365 eğilimi modeli) | Çevik İş Süreçleri Oluşturma - Dynamics şirket içi yükleme tabanı - AX/GP/SL/NAV/Diğer (Dynamics 365 eğilimi modeli) | 
| Çevik İş Süreçleri Oluşturma - Dynamics rekabet tabanı - Mendix/OutSystems/Salesforce (Dynamics 365 eğilimi modeli) | Çevik iş süreçleri oluşturma - Dynamics rekabet tabanı - Mendix/OutSystems/Salesforce (Dynamics 365 eğilimi modeli) | 
| Çevik İş Süreçleri Oluşturma - Dynamics 365 Finance + Operations yükleme tabanı | Mevcut Dynamics 365 Finance + Operations müşterileri. İş ortağı, hedef Power Apps. | 
| Çevik İş Süreçleri Oluşturma - Dynamics 365 Business Central yükleme tabanı | Mevcut Dynamics 365 Business Central müşterileri. İş ortağı, hedef Power Apps. | 
| Çevik İş Süreçleri Oluşturma - Dynamics 365 Customer Engagement yükleme tabanı | Mevcut Dynamics 365 Customer Engagement müşterileri. İş ortağı, hedef Power Apps. | 
| Oracle olmayan veya SAP ERP (kurumsal kaynak planlama) Windows Dynamics 365 Tedarik Zinciri Yönetimi olarak ilk Dynamics 365 iş yükünü etkinleştirme ve etkinleştirme | Dynamics 365 Tedarik Zinciri Yönetimi için hedef müşteriler | 
| Bir Resilient Tedarik Zinciri oluşturma - Dynamics 365 Tedarik Zinciri Yönetimi ve/veya Perakende veya Ticaret'i mevcut Dynamics 365 Customer Engagement müşterilerine çapraz satış | Dynamics 365 Tedarik Zinciri Yönetimi'nin çapraz satışlarını hedeflemek için mevcut Dynamics 365 Customer Engagement müşterileri. | 
| Bir Resilient Tedarik Zinciri Oluşturma - Dynamics 365 Tedarik Zinciri Yönetimi ve/veya Perakende veya Ticaret'i Dynamics 365 Customer Engagement ve Oracle veya SAP'ye çapraz satış | Dynamics 365 Tedarik Zinciri Yönetimini hedeflemek için Oracle veya SAP'ye sahip mevcut Dynamics 365 Customer Engagement müşterileri | 
| D365BCCluster | Müşterinin Dynamics 365 Business Central satın alma eğilimini tanımlar. Business Central için bir teklifte bulunan müşteriler Orta ve Küçük kategorilerde yer atılır. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| D365BCFit | Sıkı grafiği tanımlayan iç ve dış veri noktaları. Uygun puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünlerine potansiyel olarak uygun olup olmadığını görmek için en iyi SMB'mize benzer bir model kullanır. Fit puanlama üç aylık olarak güncelleştirilir. | 
| D365BCIntent | Sosyal medya ve müşterinin çevrimiçi davranışıyla ilgili sinyaller Amacı tanımlar. Amaç puanlama, kümeleri tanımlamak için Sığdır'ın üzerine atlar. Amaç puanlama aylık olarak güncelleştirilir. | 
| D365FOCluster | Müşterinin Dynamics 365 Finance and Operations satın alma eğilimini tanımlar. Finance + Operations için bir eğilimini göstermekte olan müşteriler, en üstteki unmanaged kategorilerde yer alamaktadır. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| D365FOFit | Sıkı grafiği tanımlayan iç ve dış veri noktaları. Uygun puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünlerine potansiyel olarak uygun olup olmadığını görmek için en iyi SMB'mize benzer bir model kullanır. Fit puanlama üç aylık olarak güncelleştirilir. | 
| D365FOIntent | Sosyal medya ve müşterinin çevrimiçi davranışıyla ilgili sinyaller Amacı tanımlar. Amaç puanlama, kümeleri tanımlamak için Sığdır'ın üzerine atlar. Amaç puanlama aylık olarak güncelleştirilir. | 
| D365CECluster | Müşterinin Dynamics 365 Customer Engagement satın alma eğilimini tanımlar. Customer Engagement için bir teklifte yer alan müşteriler Orta ve Küçük kategorilerde yer atılır. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| D365CEFit | Dynamics 365 Customer Engagement için Uygun olduğunu gösterir | 
| D365CEIntent | Dynamics 365 Customer Engagement amacını gösterir | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Müşterinin Dynamics şirket içi AX veya CRM için açık yenilemeye sahip olup olmadığını tanımlar | 
| M365UpsellCustomer | Müşterinin sipariş için satış eğilimi gösterip Microsoft 365 | 
| Google'a sahip | Müşterinin Google ürünlerine sahip olmak için rekabet sinyalleri gösterip gösterip gösterir olmadığını tanımlar | 
| AWS'ye sahip | Müşterinin AWS ürünlerine sahip olan müşterilere yönelik rekabet sinyalleri gösterip gösterip gösterir | 
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
| En İyi Unmanaged - Kullanıcı Tabanı | En çok kontrol dışı müşteriler – kullanıcılar | 
| IsNonProfit | Kuruluşun kar amacı gütmeyen bir kuruluş olup olmadığını gösterir (Evet veya Hayır) | 
| Geçiş - EOL Windows Sunucusu - EOL Windows Bulut Ascent eğilimine sahip Sunucu IB -5+ lisans | Şirket içi bir EOL Windows Sunucusuna (yani, bir EOL sürümü veya daha önceki) sahip olan müşteri. Müşterinin 5 veya daha fazla lisansı vardır. Teklif puanına sahip olan müşteri. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL Windows Sunucusu - EOL Windows Bulut Ascent eğilimine sahip Sunucu IB 'leri - <5 lisans | Şirket içi bir EOL Windows Sunucusuna (yani, bir EOL sürümü veya daha önceki) sahip olan müşteri. Müşterinin 5'ten az lisansı vardır. Teklif puanına sahip olan müşteri. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL Windows Sunucusu - EOL Windows Bulut Ascent eğilimi olmadan Sunucu IB -5+ lisans | Şirket içi bir EOL Windows Sunucusuna (yani, bir EOL sürümü veya daha önceki) sahip olan müşteri. Müşterinin 5'in üzerinde lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL Windows Sunucusu - EOL Windows Bulut Ascent eğilimi olmadan Sunucu IB -<5 lisans | Şirket içi bir EOL Windows Sunucusuna (yani, bir EOL sürümü veya daha önceki) sahip olan müşteri. 5'ten az lisansa sahip. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL SQL - EOL SQL Server BulutAslılık ile IB-5+ lisans | Şirket içi bir EOL sürümüne sahip SQL Server (yani, bir EOL sürümü veya önceki bir sürüm). Müşterinin 5'den fazla lisansı vardır. Müşterinin bir yayma puanı vardır. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL SQL - Bulut SQL Server eğilimi olan EOL <IB - <5 lisans | Şirket içi bir EOL sürümüne sahip SQL Server (yani, bir EOL sürümü veya önceki bir sürüm). 5'ten az lisansa sahip. Teklif puanına sahip olan müşteri. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL SQL - EOL SQL Server BulutAslılıksız IB - 5+ lisans | Şirket içi bir EOL sürümüne sahip SQL Server (yani, bir EOL sürümü veya daha önceki bir sürüm). Müşterinin 5 veya daha fazla lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL SQL - Bulut SQL Server eğilimi olmadan EOL <IB - <5 lisans | Şirket içi bir EOL sürümüne sahip SQL Server (yani, bir EOL sürümü veya daha önceki bir sürüm). Müşterinin 5'ten az lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçirme - Şirket içi Windows Sunucusunu geçirme - geçerli Windows Bulut Ascent eğilimi ile Sunucu IB - 5' den fazla lisans | Geçerli şirket içi sunucu sunucusuna sahip Windows (yani, EOL'den sonraki bir sürüm). Müşterinin 5'den fazla lisansı vardır. Müşterinin bir yayma puanı vardır. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçirme - Şirket içi Windows Sunucusunu geçirme - geçerli Windows Bulut Ascent eğilimi ile Sunucu IB - <5 lisans | Geçerli şirket içi sunucu sunucusuna sahip Windows (yani, EOL'den sonraki bir sürüm). Müşterinin 5'ten az lisansı vardır. Müşterinin Azure için bir teklif puanı vardır. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçirme - Şirket içi Windows Sunucusunu geçirme - geçerli Windows Bulut Ascent eğilimi olmadan Sunucu IB 'leri - 5'den fazla lisans | Geçerli şirket içi sunucu sunucusuna sahip Windows (yani, EOL'den sonraki bir sürüm). Müşterinin 5'den fazla lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçirme - Şirket içi Windows Sunucusunu geçirme - geçerli Windows Bulut Ascent eğilimi olmadan Sunucu IB 'leri - <5 lisans | Geçerli şirket içi sunucu sunucusuna sahip Windows (yani, EOL'den sonraki bir sürüm). Müşterinin 5'ten az lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Azure SQL veya SQL sanal makinelere (VM) geçiş - bulut SQL Server sahip geçerli sanal makine IB - 5'den fazla lisans | Geçerli şirket içi bulut hizmetine sahip olan SQL Server (başka bir ifadeyle, EOL'den sonraki bir sürüm). Müşterinin 5'den fazla lisansı vardır. Müşterinin bir yayma puanı vardır. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Azure SQL veya SQL VM'lere geçiş - Bulut SQL Server eğilimi ile geçerli SQL Server IB - <5 lisans | Geçerli şirket içi bulut hizmetine sahip olan SQL Server (başka bir ifadeyle, EOL'den sonraki bir sürüm). Müşterinin 5'ten az lisansı vardır. Müşterinin bir yayma puanı vardır. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Azure SQL veya SQL VM'lere geçiş - bulut SQL Server buluta geçiş eğilimi olmadan geçerli SQL Server IB - 5'den fazla lisans | Geçerli şirket içi bulut hizmetine sahip olan SQL Server (başka bir ifadeyle, EOL'den sonraki bir sürüm). Müşterinin 5'den fazla lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Azure SQL veya SQL VM'lere geçiş - Bulut SQL Server eğilimi olmadan geçerli SQL Server IB - <5 lisans | Geçerli şirket içi bulut hizmetine sahip olan SQL Server (başka bir ifadeyle, EOL'den sonraki bir sürüm). Müşterinin 5'ten az lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - OSS - Açık Kaynak Kod (OSS) DB'ye Geçiş | Şu ürünlerden herhangi birini alan mevcut müşteri: PostgreSQL, MySQL, MariaDB. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - OSS - Azure'da Linux | Linux'a sahip mevcut müşteri. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçirme - SAP - Azure üzerinde SAP | SAP ile mevcut müşteri. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Windows Sanal Masaüstü - Uzak Masaüstü Hizmetleri IB | Etkin verilerle müşterileri Windows Uzak Masaüstü Hizmetleri. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Windows Sanal Masaüstü - Modern Çalışmaları Azure'a Çapraz Satış/WVD | Azure'Microsoft 365 sahip olmayan müşterileri tanımlar. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - VMware IB | Ürüne sahip mevcut müşteri: VMware. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçirme - Citrix IB | Ürünü olan mevcut müşteri: Citrix Systems. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Yenilik - Analiz - Power BI Azure eğilimine sahip IB'ler | Ve Etkin Power BI aboneliğine sahip müşteriler: Power BI - Tek başına Pro, Power BI - Azure Paketleri, Power BI - Office Paketleri, Power BI Paketleri - Microsoft 365 | 
| Etkinleştirme - DevOps ile GitHub - Visual Studio/MSDN IB | Etkin sürümlere sahip müşterileri Visual Studio tanımlar | 
| Windows Sunucu Standart sürümü | Müşteri tarafından Windows Server Standard satın almalarının sürümünü görüntüler | 
| Windows Sunucu Standart lisansı | Müşterinin Windows Server Standard satın almalarının lisans türünü görüntüler | 
| Windows Sunucu Veri Merkezi sürümü | Müşteri tarafından Windows Veri Merkezi satın almalarının sürümünü görüntüler | 
| Windows Sunucu Veri Merkezi Lisansı | Müşterinin Veri Merkezi Windows lisans türünü görüntüler | 
| AzureFit | Sıkı grafiği tanımlayan iç ve dış veri noktaları. Uygun puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünlerine potansiyel olarak uygun olup olmadığını görmek için en iyi SMB'mize benzer bir model kullanır. Fit puanlama üç aylık olarak güncelleştirilir. | 
| AzureIntent | Sosyal medya ve müşterinin çevrimiçi davranışıyla ilgili sinyaller Amacı tanımlar. Amaç puanlama, kümeleri tanımlamak için Sığdır'ın üzerine atlar. Amaç puanlama aylık olarak güncelleştirilir. | 
| AzureCluster | Fit ve Intent önerilerini bir kümede bir arada kullanarak müşterinin Azure satın alma eğilimini tanımlar. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| WindowsServerDataCenter_HasOpenRenewal | Müşterinin Windows Server Datacenter için açık yenilemeye sahip olup olmadığını tanımlar | 
| WindowsServerStandard_HasOpenRenewal | Müşterinin Windows Server Standard için açık yenilemesi olup olmadığını tanımlar | 
| AzureUpsellCustomer | Müşterinin Azure için satış eğilimi gösterip gösterip gösterir olmadığını tanımlar | 
| Google'a sahip | Müşterinin Google ürünlerine sahip olmak için rekabet sinyalleri gösterip gösterip gösterir olmadığını tanımlar | 
| AWS'ye sahip | Müşterinin AWS ürünlerine sahip olan müşterilere yönelik rekabet sinyalleri gösterip gösterip gösterir | 
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
| SMC Tür Özeti | SMC türü | 
| En İyi Unmanaged - İşlem Tabanı | En çok kontrol dışı olan müşteriler – işlem | 
| En İyi Unmanaged - Kullanıcı Tabanı | En çok kontrol dışı müşteriler – kullanıcılar | 
| IsNonProfit | Kuruluşun kar amacı gütmeyen bir kuruluş olup olmadığını gösterir (Evet veya Hayır) | 
| Google'a sahip | Müşterinin AWS ürünlerine sahip olan müşterilere yönelik rekabet sinyalleri gösterip gösterip gösterir | 
| AWS'ye sahip | Müşterinin AWS ürünlerine sahip olan müşterilere yönelik rekabet sinyalleri gösterip gösterip gösterir | 
| Azure Kümesi | Müşterinin Azure satın alma eğilimini tanımlar. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| D365 Finance + Operations Cluster | Müşterinin Dynamics 365 Finance and Operations satın alma eğilimini tanımlar. Finance + Operations'a yönelik bir eğilimi olan müşteriler, en üst sırada yer alan ve en iyi tarafından kontrolsüz kategorilerde yer alan müşterilerdir. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
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
| Azure Upsell müşterisi | Müşterinin Azure için satış eğilimi gösterip gösterip gösterir olmadığını tanımlar | 
| Microsoft 365 Müşteriye satış | Müşterinin sipariş için satış eğilimi gösterip Microsoft 365 | 
| RevSumDivisionName | Yenilemeye hazır olan ürünü tanımlar | 

## <a name="next-steps"></a>Sonraki adımlar

Daha fazla bilgi için bkz. [Raporları indirme.](insights-download-reports.md)
