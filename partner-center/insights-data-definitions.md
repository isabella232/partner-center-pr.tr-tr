---
title: İçgörü verilerinin tanımları
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Belgede çeşitli raporlar ve bunların veri tanımları listelenmiş ve bu raporları Analizler sayfasından indirebilirsiniz.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eac173fa84625d39d828fa104c461fc52d873176
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129073252"
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
| kaynak grubundaki | Aboneliğin GUID 'SI | 
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
| MPNId | Microsoft İş Ortağı Ağı | 
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
| CompetencyAttainmentOptionName | Uzmanlık elde etme seçeneğinin adı | 
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
| IsNonProfit | Kuruluşun kar amacı gütmeyen bir kuruluş olup olmadığını gösterir (Evet veya Hayır) | 
| Uzaktan Çalışma Etkinleştirme - hedef Exchange Online | Etkin bir Exchange Online olan müşteriler, Microsoft 365'a Microsoft 365 | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi ile şirket içi alım (geçerli sürüm) - +10 lisans | Geçerli bir şirket içi müşterisi veya Office müşterisi Windows müşteri. Başka bir ifadeyle, istemci sürümü bir yaşam sonu (EOL) sürümünden daha eskidir. Müşterinin 10 veya daha fazla lisansı vardır. Teklif puanına sahip olan müşteri. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi ile şirket içi alım (geçerli sürüm) - <10 lisans | Geçerli bir şirket içi istemciye sahip olan Office Windows (yani, EOL'den sonraki bir sürüm). Müşterinin 10'dan az lisansı vardır. Teklif puanına sahip olan müşteri. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi olmadan şirket içi alım (geçerli sürüm) - +10 lisans | Geçerli bir şirket içi istemciye sahip olan Office Windows (yani, EOL'den sonraki bir sürüm). Müşterinin 10 veya daha fazla lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi olmadan şirket içi alım (geçerli sürüm) - <10 lisans | Geçerli bir şirket içi istemciye sahip olan Office Windows (yani, EOL'den sonraki bir sürüm). Müşterinin 10'dan az lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi ile şirket içi alım (EOL sürümü) - +10 lisans | Şirket içi EOL veya Office Windows (yani, bir EOL sürümü veya önceki) olan müşteri. Müşterinin 10 veya daha fazla lisansı vardır. Müşterinin bir yayma puanı vardır. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi ile şirket içi alım (EOL sürümü) - <10 lisans | Şirket içi EOL veya Office Windows (yani, bir EOL sürümü veya önceki) olan müşteri. Müşterinin 10'dan az lisansı vardır. Müşterinin bir yayma puanı vardır. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi olmadan şirket içi alım (EOL sürümü) - +10 lisans | Geçerli bir şirket içi hizmet Office veya Windows (EOL sürümü veya önceki bir sürüm) olan müşteri. Müşterinin 10 veya daha fazla lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi olmadan şirket içi alım (EOL sürümü) - <10 lisans | Geçerli bir şirket içi hizmet Office veya Windows (EOL sürümü veya önceki bir sürüm) olan müşteri. Müşterinin 10'dan az lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştir - yüksek olasılık olasılığı Microsoft 365 (Act NowithEvaluate) | Müşteri adayları için yüksek Microsoft 365 | 
| Uzaktan Çalışma Etkinleştir - uzaktan çalışmayla rekabet Microsoft 365 | Yakınlaştırma ve yakınlaştırma özelliğine Microsoft 365 müşteri, hedef olarak Teams | 
| Uzaktan Çalışma Özelliğini Etkinleştirme - uzaktan çalışma olmadan rekabet Microsoft 365 | Yakınlaştırmalı müşteri, hedef hedef Teams | 
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
| DUNS Numarası | Dun & Bradstreet sayısı, yayma puanı alan müşterinin sayısıdır | 
| Hesap Adı | Hesabın adı | 
| Etki alanı | Hesabın etki alanı | 
| Kuruluş Boyutu | Kuruluşun boyutu | 
| Sektör | Sektör | 
| Dikey | Microsoft, D&B ve diğer sektör standartları tarafından belirlenen, yayma puanı alan müşterinin dikeyi | 
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
| IsNonProfit | Kuruluşun kar amacı gütmeyen bir kuruluş olup olmadığını gösterir (Evet veya Hayır) | 
| Geçiş - EOL Windows Sunucusu - EOL Windows Bulut Tabanlı Sunucu IB - 5+ lisans | Şirket içi bir EOL sunucusuna sahip Windows (yani, bir EOL sürümü veya daha önceki bir sürüm). Müşterinin 5 veya daha fazla lisansı vardır. Teklif puanına sahip olan müşteri. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL Windows Sunucusu - EOL Windows Bulut Ascent eğilimi ile Sunucu IB - <5 lisans | Şirket içi bir EOL sunucusuna sahip Windows (yani, bir EOL sürümü veya daha önceki bir sürüm). Müşterinin 5'ten az lisansı vardır. Teklif puanına sahip olan müşteri. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL Windows Sunucusu - EOL Windows Bulut Ascent eğilimi olmadan Sunucu IB -5+ lisans | Şirket içi bir EOL sunucusuna sahip Windows (yani, bir EOL sürümü veya daha önceki bir sürüm). Müşterinin 5'in üzerinde lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL Windows Sunucusu - EOL Windows Bulut Ascent eğilimi olmadan Sunucu IB - <5 lisans | Şirket içi bir EOL sunucusuna sahip Windows (yani, bir EOL sürümü veya daha önceki bir sürüm). 5'ten az lisansa sahip. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL SQL - Bulut SQL Server ile EOL bulut tabanlı IB - 5+ lisans | Şirket içi bir EOL sürümüne sahip SQL Server (yani, bir EOL sürümü veya önceki bir sürüm). Müşterinin 5'den fazla lisansı vardır. Müşterinin bir yayma puanı vardır. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL SQL - Bulut SQL Server ile EOL <IB - <5 lisans | Şirket içi bir EOL sürümüne sahip SQL Server (yani, bir EOL sürümü veya önceki bir sürüm). 5'ten az lisansa sahip. Teklif puanına sahip olan müşteri. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL SQL - EOL SQL Server BulutAslılıksız IB - 5+ lisans | Şirket içi bir EOL sürümüne sahip SQL Server (yani, bir EOL sürümü veya daha önceki bir sürüm). Müşterinin 5 veya daha fazla lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL SQL - Bulut SQL Server eğilimi olmadan EOL <IB - <5 lisans | Şirket içi bir EOL sürümüne sahip SQL Server (yani, bir EOL sürümü veya daha önceki bir sürüm). Müşterinin 5'ten az lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçirme - Şirket içi Windows Sunucusunu geçirme - geçerli Windows Bulut Ascent eğilimi ile Sunucu IB - 5' den fazla lisans | Geçerli şirket içi sunucu sunucusuna sahip Windows (yani, EOL'den sonraki bir sürüm). Müşterinin 5'den fazla lisansı vardır. Müşterinin bir yayma puanı vardır. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçirme - Şirket içi Windows Sunucusunu geçirme - geçerli Windows Bulut Ascent eğilimi ile Sunucu IB - <5 lisans | Geçerli şirket içi sunucu sunucusuna sahip Windows (yani, EOL'den sonraki bir sürüm). Müşterinin 5'ten az lisansı vardır. Müşterinin Azure için bir teklif puanı vardır. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçirme - Şirket içi Windows Sunucusunu geçirme - geçerli Windows Bulut Ascent eğilimi olmadan Sunucu IB - 5' den fazla lisans | Geçerli şirket içi sunucu sunucusuna sahip Windows (yani, EOL'den sonraki bir sürüm). Müşterinin 5'den fazla lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçirme - Şirket içi Windows Sunucusunu geçirme - geçerli Windows Bulut Windows eğilimi olmadan Sunucu IB 'leri - <5 lisans | Geçerli şirket içi sunucu sunucusuna sahip Windows (yani, EOL'den sonraki bir sürüm). Müşterinin 5'ten az lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Azure SQL veya SQL sanal makinelere (VM) geçiş - Bulut SQL Server sahip geçerli sanal makine - 5'den fazla lisans | Geçerli şirket içi bulut hizmetine sahip olan SQL Server (başka bir ifadeyle, EOL'den sonraki bir sürüm). Müşterinin 5'den fazla lisansı vardır. Müşterinin bir yayma puanı vardır. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçirme - Azure SQL veya SQL VM'lere geçiş - Bulut SQL Server eğilimine sahip geçerli sanal <IB - <5 lisans | Geçerli şirket içi bulut hizmetine sahip olan SQL Server (başka bir ifadeyle, EOL'den sonraki bir sürüm). Müşterinin 5'ten az lisansı vardır. Müşterinin bir yayma puanı vardır. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Azure SQL veya SQL VM'lere geçiş - Bulut SQL Server olmadan geçerli sanal SQL Server IB - 5'den fazla lisans | Geçerli şirket içi bulut hizmetine sahip olan SQL Server (başka bir ifadeyle, EOL'den sonraki bir sürüm). Müşterinin 5'den fazla lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Azure SQL veya SQL VM'lere geçiş - Bulut SQL Server eğilimi olmadan geçerli SQL Server IB - <5 lisans | Geçerli şirket içi bulut hizmetine sahip olan SQL Server (başka bir ifadeyle, EOL'den sonraki bir sürüm). Müşterinin 5'ten az lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - OSS - Açık Kaynak (OSS) DB'ye Geçiş | Şu ürünlerden herhangi birini alan mevcut müşteri: PostgreSQL, MySQL, MariaDB. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
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
