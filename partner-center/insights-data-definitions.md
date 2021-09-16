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
ms.sourcegitcommit: 986573bc4382b803bf4d641df6dd1e37c3af1955
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/16/2021
ms.locfileid: "127862298"
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
| Availablekoltuk | Kullanılabilir lisans sayısı | 
| AssignedSeats | Atanan bilgisayar lisansı sayısı | 
| BilledRevenueUSD | ABD Doları cinsinden faturalandırılan gelir | 
| CustomerName | Müşterinin adı | 
| Customertpıd | Müşteri üst üst öğesinin tanımlayıcısı | 
| CustomerSegment | Müşteri kesimi | 
| CustomerMarket | Müşterinin coğrafi pazarı | 
| ResellerStatus | Satıcı durumu | 

### <a name="subscription-details-report"></a>**Abonelik Ayrıntıları raporu**

>[!Note]
>Gelir ve ACR verileri yalnızca Executive rapor izleyicileri olan kullanıcılar tarafından kullanılabilir.

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
|Pgampnıd| Ortak küresel hesap MPN tanımlayıcısı |
|kaynak grubundaki | Aboneliğin GUID 'SI|
|SubscriptionStartDate | Aboneliğin başlangıç tarihi|
|SubscriptionEndDate | Aboneliğin bitiş tarihi|
|SubscriptionState | Aboneliğin durumu (etkin veya uygulanmış)|
|Ay | Kullanım ve gelirin bildirildiği ay|
|IsAutoRenew | Aboneliğin otomatik yenileme olup olmadığını gösterir (Evet veya Hayır)|
|CustomerName | Müşterinin adı|
|CustomerTenantId | Müşterinin GUID 'SI|
|Customertpıd | Müşteri üst üst öğe tanımlayıcısı|
|DUNSNumber| Küresel veri evrensel sayı sistem tanımlayıcısı|
|CustomerSegment | Müşterinin pazar segmenti|
|TopSegment| Müşterinin daha yüksek düzey segment sınıflandırması|
|CustomerMarket | Müşterinin coğrafi pazarı|
|ReportingProductName| Ayrıntılı ürün adı|
|Ürün | İş ortağı tarafından müşteriye satılan ürün|
|RawProductName| Müşteriye satılan ayrıntılı ürün adı|
|ProductPartNumber| Ürünün bölüm numarası|
|SKU | Ürünün SKU 'SU|
|RevSumDivisionName| Gelir raporlama ürün hiyerarşisi adı|
|SolutionArea| Ürünün iş uygulaması sınıflandırması|
|Mpnıd | Ortağın Microsoft İş Ortağı Ağı kimliği|
|PartnerName | Ortağın adı|
|PartnerLocation | Ortağın coğrafi konumu|
|PartnerAttributionType | Abonelik için attributıon türü|
|SalesChannel | sales-Direct, CSP (Bulut Çözümü Sağlayıcısı) vb. kanalı|
|PricingLevel| Satışın fiyat noktası|
|Kayıt numarası| Aboneliğin kayıt numarası|
|Iduplicaterowforpga| Tek PGA altında birden fazla iş ortağı tanımlayıcısı için, bu değer yalnızca bir MPNId için 0 olarak ayarlanır. Değer 1 olarak ayarlanırsa, yinelenen bir satırı gösterir|
|SubscriptionStartMonth| Aboneliğin başlangıç ayı|
|ResellerID| Satıcı kimliği|
|ResellerName| Satıcı adı|
|AvailableSeatsEOP| Dönemin sonuna kadar toplam kullanılabilir bilgisayar sayısı|
|Availablekoltuk | Aylık kullanılabilir koltuk farkı ayı|
|BilledRevenueUSD | ABD Doları cinsinden gelir|
|AzureConsumedRevenueUSD| Azure tüketilen gelir ABD Doları|

### <a name="azure-usage-report"></a>**Azure kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
|Pgampnıd| Ortak küresel hesap MPN tanımlayıcısı|
|kaynak grubundaki| Aboneliğin GUID 'SI|
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
|ServiceGroup3| IoT FRA için IoT Hub, Haritalar fra için ek ayrıntı|
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
| MPNId | Microsoft İş Ortağı Ağı | 
| PartnerName | İş ortağının adı | 
| PartnerLocation | İş ortağının coğrafi konumu | 
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
| DYENIDEN sayı | Dun &, yayma puanı alan müşterinin Bradstreet numarasını aldı | 
| Hesap Adı | Hesabın adı | 
| Etki alanı | Hesabın etki alanı | 
| Kuruluş Boyutu | Kuruluşun boyutu | 
| Sektör | Kuruluşun ait olduğu sektör | 
| Dikey | Microsoft, D&B ve diğer sektör standartları tarafından belirlenen, yayma puanı alan müşterinin dikeyi
| Alan | Konumun coğrafi alanı | 
| Yan Kuruluş | Teklif puanı alan müşterinin yan kuruluşu | 
| Sales Territory | Yayma puanı alan müşterinin satış bölgesi | 
| Şehir | Coğrafi şehir konumu | 
| Durum | Coğrafi durum konumu | 
| Posta Kodu | Kuruluşun posta kodu | 
| Ülke | Coğrafi ülke konumu | 
| Segment | Pazar segmenti | 
| Alt Kesim | Pazar alt | 
| SMC Tür Özeti | Bir müşterinin kategorilere ayırması: En fazla 300 çalışana sahip müşteriler, en fazla 10.000 ABD doları Azure'da üç yıllık potansiyele sahip müşteriler, orta ölçekli işletmeler 25 veya daha fazla çalışana sahip müşteriler ve küçük işletmeler ise 25'ten az çalışanı olan müşterilerdir. | 
| En İyi Unmanaged - İşlem Tabanı | En çok kontrol dışı olan müşteriler – işlem | 
| En İyi Unmanaged - Kullanıcı Tabanı | En iyi unmanaged müşterileri – kullanıcılar | 
| IsNonProfit | Kuruluşun kar amacı gütmeyen bir kuruluş olup olmadığını gösterir (Evet veya Hayır) | 
| Dijital Satış etkinleştirme - Microsoft 365 - lisans boyutu >= 25 lisans (SalesPro eğilimi modeli) | Dynamics 365 olmayan müşteri. Seat size: 25+. İş ortağıNın Dynamics 365 SalesPro çapraz satışını hedeflemesi gerekir. | 
| Dijital Satışı Etkinleştirme - Dynamics 365 SalesPro eğilimi (Şimdi Harekete Geç veya Değerlendir) | Dynamics 365 olmayan yüksek performanslı müşteriler. İş ortağıNın Dynamics 365 SalesPro'ya yönelik hedefi olması gerekir. | 
| Finansal Risk Yönetimi & Sahtekarlık - Dynamics şirket içi yükleme tabanı - Navision (Business Central eğilimi modeli) | Şirket içi Navision'a sahip mevcut müşteri. İş ortağıNın Dynamics 365 Business Central'a yönelik hedefi olması gerekir. | 
| Finansal Risk Yönetimi & Sahtekarlık - Dynamics şirket içi yükleme tabanı - Dynamics AX (Dynamics 365 Finance + Operations propensity model) | Şirket içi AX'e sahip mevcut müşteri. İş ortağıNın Dynamics 365 Finance + Operations'i hedeflemesi gerekir. | 
| Finansal Risk Yönetimi & Sahtekarlık - Dynamics şirket içi yükleme tabanı - Great Plains (Business Central eğilimi modeli) | Şirket içi Great Plains'e sahip mevcut müşteri. İş ortağıNın Dynamics 365 Business Central'a yönelik hedefi olması gerekir. | 
| Finansal Risk Yönetimi & Sahtekarlık - Dynamics şirket içi yükleme tabanı - Dynamics (Business Central eğilimi modeli) | Şirket içi Hizmet Merkezi olan mevcut müşteri. İş ortağıNın Dynamics 365 Business Central'a yönelik hedefi olması gerekir. | 
| Finansal Risk Yönetimi & Sahtekarlık - Dynamics şirket içi yükleme tabanı - Diğerleri (Business Central eğilimi modeli) | Daha önce listelenmiyor olan diğer şirket içi çözümlere sahip mevcut müşteri. İş ortağıNın Dynamics 365 Business Central'a yönelik hedefi olması gerekir. | 
| Çevik İş Süreçleri Oluşturma - Dynamics şirket içi yükleme tabanı - AX/GP/SL/NAV/Diğer (Dynamics 365 eğilimi modeli) | Çevik İş Süreçleri Oluşturma - Dynamics şirket içi yükleme tabanı - AX/GP/SL/NAV/Diğer (Dynamics 365 eğilimi modeli) | 
| Çevik İş Süreçleri Oluşturma - Dynamics rekabet tabanı - Mendix/OutSystems/Salesforce (Dynamics 365 eğilimi modeli) | Çevik iş süreçleri oluşturma - Dynamics rekabet tabanı - Mendix/OutSystems/Salesforce (Dynamics 365 eğilimi modeli) | 
| Çevik İş Süreçleri Oluşturma - Dynamics 365 Finance + Operations yükleme tabanı | Mevcut Dynamics 365 Finance + Operations müşterileri. İş ortağı hedef Power Apps. | 
| Çevik İş Süreçleri Oluşturma - Dynamics 365 Business Central yükleme tabanı | Mevcut Dynamics 365 Business Central müşterileri. İş ortağı hedef Power Apps. | 
| Çevik İş Süreçleri Oluşturma - Dynamics 365 Customer Engagement yükleme tabanı | Mevcut Dynamics 365 Customer Engagement müşterileri. İş ortağı hedef Power Apps. | 
| Oracle olmayan veya SAP ERP (kurumsal kaynak planlama) Windows Dynamics 365 Tedarik Zinciri Yönetimi olarak ilk Dynamics 365 iş yükünü etkinleştirme ve etkinleştirme | Dynamics 365 Tedarik Zinciri Yönetimi için hedef müşteriler | 
| Bir Resilient Tedarik Zinciri oluşturma - Dynamics 365 Tedarik Zinciri Yönetimi ve/veya Perakende veya Ticaret'i mevcut Dynamics 365 Customer Engagement müşterilerine çapraz satış | Dynamics 365 Tedarik Zinciri Yönetimi'nin çapraz satışlarını hedeflemek için mevcut Dynamics 365 Customer Engagement müşterileri. | 
| Bir Resilient Tedarik Zinciri Oluşturma - Dynamics 365 Tedarik Zinciri Yönetimi ve/veya Perakende veya Ticaret'i Dynamics 365 Customer Engagement ve Oracle veya SAP'ye çapraz satış | Dynamics 365 Tedarik Zinciri Yönetimini hedeflemek için Oracle veya SAP ile mevcut Dynamics 365 Müşteri Katılımı müşterileri | 
| D365BCCluster | Müşterinin Dynamics 365 Business Central satın alma eğilimini tanımlar. Business Central için bir teklifte bulunan müşteriler Orta ve Küçük kategorilerde yer atılır. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| D365BCFit | Sıkı grafiği tanımlayan iç ve dış veri noktaları. Uygun puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünlerine potansiyel olarak uygun olup olmadığını görmek için en iyi SMB'mize benzer bir model kullanır. Fit puanlama üç aylık olarak güncelleştirilir. | 
| D365BCIntent | Sosyal medya ve müşterinin çevrimiçi davranışıyla ilgili sinyaller Amacı tanımlar. Amaç puanlama, kümeleri tanımlamak için Sığdır'ın üzerine atlar. Amaç puanlama aylık olarak güncelleştirilir. | 
| D365FOCluster | Müşterinin Dynamics 365 Finance and Operations satın alma eğilimini tanımlar. Finance + Operations için bir eğilimini göstermekte olan müşteriler, en üstteki unmanaged kategorilerde yer alamaktadır. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| D365FOFit | Sıkı grafiği tanımlayan iç ve dış veri noktaları. Uygun puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünlerine potansiyel olarak uygun olup olmadığını görmek için en iyi SMB'mize benzer bir model kullanır. Fit puanlama üç aylık olarak güncelleştirilir. | 
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
| Migrate-eol SQL-eol SQL Server ıb, Cloud ascent eğilimini-<5 lisanslarıyla | bir eol şirket içi SQL Server (yani, bir eol sürümü veya daha eski) olan müşteri. 5 ' ten az lisansa sahiptir. Teklif puanına sahip olan müşteri. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
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
| WindowsServerStandard_HasOpenRenewal | Müşterinin Windows Server Standard için açık yenilemesi olup olmadığını tanımlar | 
| AzureUpsellCustomer | Müşterinin Azure için satış eğilimi gösterip gösterip gösterir olmadığını tanımlar | 
| Google'a sahip | Müşterinin Google ürünlerine sahip olmak için rekabet sinyalleri gösterip gösterip gösterir olmadığını tanımlar | 
| AWS'ye sahip | Müşterinin sahip olduğu AWS ürünleri için rekabet sinyalleri gösterip gösterip gösterir | 
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
| En İyi Unmanaged - Kullanıcı Tabanı | En iyi unmanaged müşterileri – kullanıcılar | 
| IsNonProfit | Kuruluşun kar amacı gütmeyen kuruluş olup olmadığını gösterir (Evet veya Hayır) | 
| Google'a sahip | Müşterinin sahip olduğu AWS ürünleri için rekabet sinyalleri gösterip gösterip gösterir | 
| AWS'ye sahip | Müşterinin sahip olduğu AWS ürünleri için rekabet sinyalleri gösterip gösterip gösterir | 
| Azure Kümesi | Müşterinin Azure satın alma eğilimini tanımlar. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| D365 Finance + Operations Cluster | Müşterinin Dynamics 365 Finance and Operations satın alma eğilimini tanımlar. Finance + Operations için bir eğilimini göstermekte olan müşteriler, en üstteki unmanaged kategorilerde yer alamaktadır. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
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
| Microsoft 365 Müşteriye satış | Müşterinin müşteriler için satış eğilimi gösterip Microsoft 365 | 
| RevSumDivisionName | Yenilemeye hazır olan ürünü tanımlar | 

### <a name="cpor-m365usage-report"></a>**CPOR-M365Usage raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| CustomerTenantId | Müşterinin Kiracı Kimliği | 
| CustomerName | Müşterinin adı | 
| WorkloadName | İş yükünün adı | 
| MonthlyActiveUsers | MAU (aylık etkin kullanıcılar) | 
| PaidAvailableUnits | PAU (ücretli kullanılabilir birimler) | 
| ClaimId | İş yükünün talep kimliği | 
| MpnId | Microsoft İş Ortağı Ağı (MPN) Kimliği | 
| DateAssociated | İş yükünün iş ortağıyla ilişkilendirilen tarihi | 
| PartnerAttributionType | İş Ortağı Atfı Türü (CPOR) | 
| Tarih | Verilerin dışarı aktarıldı olduğu tarih (ayın ve yılın ilki) | 

## <a name="next-steps"></a>Sonraki adımlar

Daha fazla bilgi için bkz. [Raporları indirme.](insights-download-reports.md)
