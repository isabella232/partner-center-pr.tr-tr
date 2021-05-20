---
title: İçgörü verilerinin tanımları
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Belge, Öngörüler Indirme raporu sayfasından indirebileceğiniz çeşitli raporlar ve veri tanımlarını listeler.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 721caed2d8b0e24940e7adedeb90cc689a82d2e7
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152843"
---
# <a name="export--data-definitions"></a>Dışarı aktarma – veri tanımları 

**Uygun roller**: rapor Görüntüleyici | Executive rapor Görüntüleyicisi

## <a name="introduction"></a>Giriş 

Öngörüler panosunda rapor Indirme merkezini kullanarak ham veri kümelerini dışarı aktarabilirsiniz. 

Veri tanımlarıyla birlikte indirebileceğiniz çeşitli raporlar aşağıdaki tablolarda listelenmiştir: 

### <a name="partner-profile-report"></a>**İş ortağı profili raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| Mpnıd | Microsoft İş Ortağı Ağı tanımlayıcısı (MPN) | 
| PartnerName | Ortağın adı | 
| PGA_MPNId | Ortak küresel hesap MPN tanımlayıcısı | 
| PGA_PartnerName | Ortak genel hesap adı | 
| Şehir | Ortağın şehir konumu | 
| Ülke | Ortağın ülke konumu | 
| HierarchyLevel | Küresel bir MPN KIMLIĞI veya konum MPN KIMLIĞI olup olmadığını belirtir | 

### <a name="customer-details-report"></a>**Müşteri Ayrıntıları raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| CustomerName | Müşterinin adı | 
| CustomerTenantId | Müşteri kiracısı tanımlayıcısı | 
| CustomerTpid | Müşterinin üst üst öğenin tanımlayıcısı | 
| CustomerSegment | Müşteri segmenti | 
| CustomerMarket | Müşterinin coğrafi pazar | 
| CustomerStatus | Müşteri durumu (Etkin veya Etkin Değil) | 
| Ürün | MÜŞTERIYE MPN tarafından satılan ürün: O365, DYNAMICS 365, Enterprise Mobility + Security, Power BI veya Microsoft Azure | 
| SKU | Ürün SKU'su | 
| Ay | Kullanım ve gelirin raporlandığı ay | 
| MPNId | Kimlik Microsoft İş Ortağı Ağı | 
| PartnerName | İş ortağının adı | 
| PartnerLocation | İş ortağının coğrafi konumu | 
| PartnerAttributionType | İş ortağının atfı | 
| SalesChannel | Satış kanalı | 
| Availablekoltuk | Kullanılabilir koltuk | 
| RevenueUSD | ABD Doları cinsinden gelir | 

### <a name="reseller-performance-report"></a>**Satıcı performans raporu**

> [!Note]
> Gelir ve ACR verileri yalnızca Executive rapor izleyicileri olan kullanıcılar tarafından kullanılabilir.

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
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
| SubscriptionId | Aboneliğin GUID'si | 
| SubscriptionStartDate | Aboneliğin başlangıç tarihi | 
| SubscriptionEndDate | Aboneliğin bitiş tarihi | 
| SubscriptionState | Aboneliğin durumu (etkin veya uygulanmış) | 
| Ay | Kullanım ve gelirin bildirildiği ay | 
| IsAutoRenew | Aboneliğin autorenew olup olmadığını gösterir (Evet veya Hayır) | 
| CustomerName | Müşterinin adı | 
| CustomerTenantId | Müşterinin GUID 'SI | 
| Customertpıd | Müşteri üst üst öğe tanımlayıcısı | 
| CustomerSegment | Müşterinin pazar segmenti | 
| CustomerMarket | Müşterinin coğrafi pazarı | 
| Ürün | İş ortağı tarafından müşteriye satılan ürün | 
| SKU | Ürünün SKU 'SU | 
| Mpnıd | Ortağın Microsoft İş Ortağı Ağı KIMLIĞI | 
| PartnerName | İş ortağının adı | 
| PartnerLocation | İş ortağının coğrafi konumu | 
| PartnerAttributionType | Abonelik için asıf türü | 
| SalesChannel | Satış kanalı - Doğrudan, CSP (Bulut Çözümü Sağlayıcısı) ve diğer | 
| AvailableSeats | Mevcut kullanılabilir yer | 
| RevenueUSD | ABD doları geliri | 
| Kayıt Kimliği | Aboneliğin kayıt kimliği | 

### <a name="azure-usage-report"></a>**Azure kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| SubscriptionId | Aboneliğin GUID'si | 
| SubscriptionStartDate | Aboneliğin başlangıç tarihi | 
| SubscriptionEndDate | Aboneliğin bitiş tarihi | 
| SubscriptionState | Aboneliğin geçerli durumu (açık, kapalı, etkin veya yetkisiz kullanım süresi) | 
| Ay | Aya göre toplanan Tarih | 
| ServiceName | Azure hizmetinin adı | 
| MeterCategory | Ölçüm kategorisinin adı | 
| UsageUnits | Fatura çevrimi sırasında kullanılan birim sayısı | 
| CustomerName | Müşterinin adı | 
| CustomerTenantId | Müşterinin kiracı KIMLIĞI | 
| Customertpıd | Müşteri üst üst KIMLIĞI | 
| CustomerSegment | Müşterinin segmenti | 
| CustomerMarket | Müşterinin coğrafi pazarı | 
| Mpnıd | Microsoft İş Ortağı Ağı müşterinin KIMLIĞI | 
| PartnerName | Ortağın adı | 
| PartnerLocation | Ortağın coğrafi ülke konumu | 
| PartnerAttributionType | İş ortağının atfı | 
| SalesChannel | Satış kanalı (Doğrudan/CSP, Dolaylı/CSP, Doğrudan ve diğer) | 
| ACR_USD | ABD doları olarak Azure tarafından tüketilen gelir (ACR) | 
| Kayıt Kimliği | Azure aboneliğinin kayıt kimliği | 

### <a name="office-365-license-usage-report"></a>**Office 365 lisans kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| CustomerTenantId | Müşterinin kiracı kimliği | 
| CustomerTpid | Müşteri üst üst kimliği | 
| WorkloadName | Skype Kurumsal, Teams, Exchange Online | 
| Ay | Kullanımın raporlandığı ay | 
| PaidAvailableUnits | Ücretli kullanılabilir birimlerin sayısı | 
| MonthlyActiveUsers | Aylık etkin kullanıcı sayısı | 
| CustomerName | Müşterinin adı | 
| CustomerMarket | Müşterinin pazarına ait coğrafi ülke konumu | 
| CustomerSegment | Müşteri kesimi | 
| Mpnıd | Microsoft İş Ortağı Ağı tanımlayıcısı | 
| PartnerName | Ortağın adı | 
| PartnerLocation | Ortağın coğrafi konumu | 
| PartnerAttributionType | Ortağın atısyon türü | 

### <a name="enterprise-mobility-license-usage-report"></a>**Enterprise Mobility lisans kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| CustomerTenantId | Müşterinin kiracı KIMLIĞI | 
| Customertpıd | Müşteri üst üst KIMLIĞI | 
| WorkloadName | Enterprise Mobility + Security (EMS) iş yükünün adı | 
| Ay | Kullanımın bildirildiği ay | 
| PaidAvailableUnits | Ücretli kullanılabilir birimlerin sayısı | 
| MonthlyActiveUsers | Aylık etkin kullanıcı sayısı | 
| CustomerName | Müşterinin adı | 
| CustomerMarket | Müşterinin pazarının coğrafi ülke konumu | 
| CustomerSegment | Müşteri segmenti | 
| MPNId | Kimlik Microsoft İş Ortağı Ağı | 
| PartnerName | İş ortağının adı | 
| PartnerLocation | İş ortağının coğrafi konumu | 
| PartnerAttributionType | İş ortağının atfı | 

### <a name="dynamics-365-license-usage-report"></a>**Dynamics 365 lisans kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| SubscriptionId | Aboneliğin GUID'si | 
| SubscriptionStartDate | Aboneliğin başlangıç tarihi | 
| SubscriptionEndDate | Aboneliğin bitiş tarihi | 
| Abonelik durumu | Aboneliğin durumu | 
| Ay | Kullanımın bildirildiği ay | 
| RevSumDivisionName | Rev Sum bölümünün adı | 
| RevSumCategoryName | Rev Sum kategorisinin adı | 
| SKU | Ürünün SKU 'SU | 
| SkuId | Ürünün SKU KIMLIĞI | 
| Freevspaıdsku | Ücretsiz veya ücretli bir SKU olup olmadığını belirtir | 
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
| Availablekoltuk | Mevcut kullanılabilir bilgisayar | 
| AssignedSeats | Geçerli atanan bilgisayar | 
| Activekoltuk | Geçerli etkin koltuk | 
| DeploymentOpportunity | Geçerli dağıtım fırsatı | 
| ActiveUsagePercent | Geçerli etkin kullanım yüzdesi | 

### <a name="power-bi-license-usage-report"></a>**Power BI kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
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
| CustomerTenantId | Müşteri kiracının GUID 'SI | 
| Customertpıd | Müşteri üst üst öğesinin tanımlayıcısı | 
| CustomerSegment | Müşterinin pazar segmenti | 
| CustomerMarket | Müşterinin coğrafi pazarı | 
| Mpnıd | Microsoft İş Ortağı Ağı tanımlayıcısı | 
| PartnerName | Ortağın adı | 
| PartnerLocation | Ortağın coğrafi ülke konumu | 
| PartnerAttachType | Abonelik için attributıon türü | 
| Availablekoltuk | Mevcut kullanılabilir koltuk | 
| AssignedSeats | Geçerli atanan yer | 
| ActiveSeats | Geçerli etkin yer sayısı | 
| DeploymentOpportunity | Geçerli dağıtım fırsatı | 
| ActiveUsagePercent | Geçerli etkin kullanım yüzdesi | 

### <a name="teams-meetings-and-calls-report"></a>**Teams toplantı ve çağrı raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| CustomerTenantId | Müşterinin kiracı kimliği | 
| CustomerTpid | Müşterinin üst üst öğenin tanımlayıcısı | 
| Ay | Kullanımın raporlandığı ay | 
| Alt iş yükü | Kullanımın raporlandığı alt iş yükü (toplantılar, aramalar veya telefon sistemleri) | 
| Toplantı sayısı | Toplantı sayısı | 
| Toplantı süresi | Saat olarak toplam toplantı süresi | 

### <a name="teams-monthly-usage-report"></a>**Takımlar aylık kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| CustomerTenantId | Müşterinin kiracı KIMLIĞI | 
| Customertpıd | Müşteri üst üst öğesinin tanımlayıcısı | 
| Ay | Kullanımın bildirildiği ay | 
| Alt iş yükü | Kullanım için raporlanan alt iş yükü (toplantılar, çağrılar veya telefon sistemleri) | 
| Masaüstü kullanıcıları | Masaüstünde takımlar kullanan kullanıcı sayısı | 
| Mobil Kullanıcılar | Mobil üzerinde takımlar kullanan kullanıcı sayısı | 
| Web kullanıcıları | Web üzerinde takımlar kullanan kullanıcı sayısı | 
| Allupkatılımcıları | Ay için ekiplerin benzersiz kullanıcı sayısı | 

### <a name="teams-usage-3p-apps-report"></a>**Takımlar kullanım 3P Apps raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| CustomerTenantId | Müşterinin kiracı KIMLIĞI | 
| Customertpıd | Müşteri üst üst KIMLIĞI | 
| Ay | Kullanımın raporlandığı ay | 
| 3P Uygulama Adı | Teams uygulamasının adı | 
| Kullanıcı sayısı | Uygulama için kullanıcı sayısı | 


### <a name="training-details-report"></a>**Eğitim ayrıntıları raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| TrainingActivityId | Eğitimin tanımlayıcısı | 
| TrainingTitle | Eğitimin başlığı | 
| TrainingType | Eğitim türü (sertifikasyon veya sınav) | 
| IndividualFirstName | Müşterinin adı | 
| IndividualLastName | Müşterinin soyadı | 
| E-posta | Müşterinin kişisel e-posta kimliği | 
| CorpEmail | Müşterinin office e-posta kimliği | 
| Traıningcompletiondate | Eğitimin tamamlanma tarihi | 
| Ay | Verilerin bildirildiği ay | 
| IMCP | Kullanıcının Microsoft sertifikalı bir profesyonel (MCP) olup olmadığını belirtir | 
| MCPID | Kullanıcının MCP KIMLIĞI | 
| Mpnıd | Microsoft İş Ortağı Ağı tanımlayıcısı | 
| PartnerName | Ortağın adı | 
| PartnerCityLocation | Ortağın coğrafi şehir konumu | 
| PartnerCountryLocation | Ortağın coğrafi ülke konumu | 

### <a name="microsoft-learn-report"></a>**Microsoft Learn raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| UserName | Kullanıcının adı | 
| UserId | Kullanıcının GUID 'SI | 
| Traıningname | Eğitimin adı | 
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

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**Bulut Yokent-Microsoft 365 eğilimini raporu**

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
| Alt Kesim | Pazar alt | 
| SMC Tür Özeti | SMC türü | 
| En İyi Unmanaged - İşlem Tabanı | En çok kontrol dışı olan müşteriler – işlem | 
| En İyi Unmanaged - Kullanıcı Tabanı | En iyi unmanaged customers – user | 
| IsNonProfit | Kuruluşun kar amacı gütmeyen kuruluş olup olmadığını gösterir (Evet veya Hayır) | 
| Uzaktan Çalışma Etkinleştir - Exchange Online'a hedefle | Etkin bir Exchange Online aboneliğine sahip olan müşteriler, Microsoft 365 | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi ile şirket içi alım (geçerli sürüm) - +10 lisans | Geçerli bir şirket içi Office veya Windows istemcisi olan müşteri. Başka bir ifadeyle, istemci sürümü yaşam sonu (EOL) sürümünden daha eskidir. Müşterinin 10 veya daha fazla lisansı vardır. Teklif puanına sahip olan müşteri. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi ile şirket içi alım (geçerli sürüm) - <10 lisans | Geçerli bir şirket içi Office veya Windows istemcisine sahip olan müşteri (yani, EOL 'tan sonraki bir sürüm). Müşterinin 10 ' dan az lisansı vardır. Eğilimini puanı olan müşteri. İş ortağı, Microsoft 365 dönüştürme için hedef almalıdır. | 
| Bulutu olmadan uzak Iş yerinde alımı (geçerli sürüm) etkinleştir eğilimini-+ 10 lisansı | Geçerli bir şirket içi Office veya Windows istemcisine sahip olan müşteri (yani, EOL 'tan sonraki bir sürüm). Müşterinin 10 veya daha fazla lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, Microsoft 365 dönüştürme için hedef almalıdır. | 
| Bulut olmadan uzak Iş-şirket içi alımı (geçerli sürüm) etkinleştir eğilimini-<10 lisans | Geçerli bir şirket içi Office veya Windows istemcisine sahip olan müşteri (yani, EOL 'tan sonraki bir sürüm). Müşterinin 10 ' dan az lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, Microsoft 365 dönüştürme için hedef almalıdır. | 
| Cloud Ascent eğilimini-+ 10 lisanslarıyla uzaktan Iş yerinde alımı (EOL sürümü) etkinleştirin | EOL şirket içi Office veya Windows istemcisine (yani, bir EOL sürümü veya daha eski) sahip olan müşteri. Müşterinin 10 veya daha fazla lisansı vardır. Müşterinin bir eğilimini puanı vardır. İş ortağı, Microsoft 365 dönüştürme için hedef almalıdır. | 
| Cloud Ascent eğilimini-<10 lisanslarıyla uzak Iş yerinde alımı (EOL sürümü) etkinleştirin | EOL şirket içi Office veya Windows istemcisi (yani, bir EOL sürümü veya daha önceki) olan müşteri. Müşterinin 10'dan az lisansı vardır. Müşterinin bir yayma puanı vardır. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi olmadan şirket içi alım (EOL sürümü) - +10 lisans | Geçerli bir şirket içi Office veya Windows istemcisine (yani EOL sürümüne veya daha önceki bir sürümüne) sahip olan müşteri. Müşterinin 10 veya daha fazla lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi olmadan şirket içi alım (EOL sürümü) - <10 lisans | Geçerli bir şirket içi Office veya Windows istemcisine (yani EOL sürümüne veya daha önceki bir sürümüne) sahip olan müşteri. Müşterinin 10'dan az lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştir - yüksek olasılık olasılığı Microsoft 365 (Act NowithEvaluate) | Müşteri adayları için yüksek Microsoft 365 | 
| Uzaktan Çalışma Etkinleştir - uzaktan çalışmayla rekabet Microsoft 365 | Yakınlaştırma ve yakınlaştırma özelliğine Microsoft 365, Teams'e dönüştürme hedefi | 
| Uzaktan Çalışma Etkinleştirme - uzaktan çalışma olmadan rekabet Microsoft 365 | Yakınlaştırmalı müşteri, Teams'e dönüştürme hedefi | 
| Microsoft 365 E5 için hedeflenen maliyet ve Manage-Microsoft 365 E3 'ı azaltma | Microsoft 365 E3 ile mevcut müşteri, Microsoft 365 E5 için hedef | 
| Microsoft 365 İş Premium için hedeflenen maliyet ve yönetim Microsoft 365 İş temel ve Iş standart müşterilerini azaltma | Mevcut Microsoft 365 İş temel ve Iş standart müşterileri, Microsoft 365 İş Premium için hedef | 
| Kuruluş üretkenliğini dönüştürme-Surface eğilimini | Müşteri, yüzey için bir eğilimini gösterir | 
| M365Cluster | Microsoft 365 satın almak için müşterinin eğilimini tanımlar. Hedef şimdi çalışır ve daha yüksek verim üretebilmeleri için kümeleri değerlendirir. Yalnızca Şimdi hareket eden ve müşterilerin hedeflediği bir kapasite varsa müşterileri Eğtir ve müşterileri eğitin. | 
| M365Fit | Firmografları tanımlayan iç ve dış veri noktaları. Kullanım Puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünlerine yönelik potansiyel bir uyum olup olmadığını görmek için en iyi küçük veya orta ölçekli işletmelere (SMB 'ler) bir gevmüike modeli kullanır. Skor, üç aylık olarak güncelleştirilir. | 
| M365Intent | Sosyal medya ve müşterinin çevrimiçi davranışı ile ilgili sinyaller amaç tanımlar. Amaç Puanlama, kümeleri tanımlamak için uygun şekilde yer alır. Amaç Puanlama aylık olarak güncelleştirilir. | 
| SurfaceCluster | Bir kümeye sığdırma ve amaç önerilerini birleştirerek bir müşterinin eğilimini ' i, yüzeyi satın almasını belirler. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir hedefle'den sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| SurfaceFit | Sıkı grafiği tanımlayan iç ve dış veri noktaları. Uygun puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünlerine potansiyel olarak uygun olup olmadığını görmek için en iyi SMB'lerimize benzer bir model kullanır. Fit puanlama üç aylık olarak güncelleştirilir. | 
| SurfaceIntent | Sosyal medya ve müşterinin çevrimiçi davranışıyla ilgili sinyaller Amacı tanımlar. Amaç puanlama, kümeleri tanımlamak için Sığdır'ın üzerine atlar. Amaç puanlama aylık olarak güncelleştirilir. | 
| O365Cluster | Müşterinin Office 365 satın alma eğilimini tanımlar. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir hedefle'den sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| O365Fit | Sıkı grafiği tanımlayan iç ve dış veri noktaları. Uygun puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünlerine potansiyel olarak uygun olup olmadığını görmek için en iyi SMB'lerimize benzer bir model kullanır. Fit puanlama üç aylık olarak güncelleştirilir. | 
| O365Intent | Sosyal medya ve müşterinin çevrimiçi davranışıyla ilgili sinyaller Amacı tanımlar. Amaç Puanlama, kümeleri tanımlamak için uygun şekilde yer alır. Amaç Puanlama aylık olarak güncelleştirilir. | 
| M365UpsellCustomer | Müşterinin Microsoft 365 için büyük satış eğilimini gösterilip gösterilmeyeceğini belirler | 
| Google 'a sahiptir | Müşterinin sahip olduğu Google ürünleri için rekabet sinyalleri gösterilip gösterilmeyeceğini belirler | 
| AWS 'ye sahip | Müşterinin sahip Amazon Web Services (AWS) ürünleri için rekabet sinyalleri gösterilip gösterilmeyeceğini belirler | 
| EA 'ya sahiptir | Bir yenilemenin bir kurumsal anlaşma (EA) veya EA aboneliği olup olmadığını belirler | 
| Açık | Bir yenilemenin açık veya açık bir değer anlaşması olup olmadığını belirler | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Bulut Yokent-Dynamics 365 eğilimini raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| MPN Kimliği | Microsoft İş Ortağı Ağı KIMLIĞI | 
| İş ortağı adı | Ortağın adı | 
| Müşteri Kimliği | Müşteri tanımlayıcı numarası | 
| DYENIDEN sayı | Dun & Bradstreet, eğilimini için puanlanmakta olan müşterinin numarası | 
| Hesap Adı | Hesabın adı | 
| Etki alanı | Hesabın etki alanı | 
| Kuruluş Boyutu | Kuruluşun boyutu | 
| Sektör | Kuruluşun ait olduğu sektör | 
| Dikey | Microsoft, D&B ve diğer sektör standartları tarafından tanımlanan, yayma puanı alan müşterinin dikeyi
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
| En İyi Unmanaged - Kullanıcı Tabanı | En çok yönetilmeyen müşteriler – kullanıcılar | 
| Iskar dışı | Kuruluşun kar dışı olup olmadığını gösterir (Evet veya Hayır) | 
| Dijital satışı etkinleştir-Microsoft 365 özellikli boyutu >= 25 bilgisayar (SalesPro eğilimini model) | Dynamics 365 içermeyen müşteri. Koltuk boyutu: 25 +. İş ortağı Dynamics 365 SalesPro 'nun çapraz satışı için hedeflemelidir. | 
| Dijital satışı etkinleştirin-Dynamics 365 SalesPro eğilimini (Şimdi davran veya değerlendir) | Dynamics 365 içermeyen yüksek eğilimini müşterileri. İş ortağı Dynamics 365 SalesPro için hedeflemelidir. | 
| Finans riskini yönetme & sahtekarlık-Dynamics şirket içi yüklemesi temel-Navision (Business Central eğilimini model) | Şirket içi Navision ile mevcut müşteri. İş ortağı Dynamics 365 Business Central için hedeflemelidir. | 
| Finans riskini yönetme & sahtekarlık-Dynamics şirket içi Install Base-Dynamics AX (Dynamics 365 finans + Operations eğilimini model) | Şirket içi AX ile mevcut müşteri. İş ortağı, Dynamics 365 finans + Işlemleri için hedeflemelidir. | 
| Finans riskini yönetme & sahtekarlık-Dynamics şirket içi yüklemesi temel-harika Plains (Business Central eğilimini model) | Şirket içi Great Plains 'e sahip mevcut müşteri. İş ortağı Dynamics 365 Business Central için hedeflemelidir. | 
| Finans riskini yönetme & sahtekarlık-Dynamics şirket içi yüklemesi temel-Solomon (Business Central eğilimini model) | Şirket içi Hizmet Merkezi olan mevcut müşteri. İş ortağıNın Dynamics 365 Business Central'a yönelik hedefi olması gerekir. | 
| Finansal Risk Yönetimi & Sahtekarlık - Dynamics şirket içi yükleme tabanı - Diğer (Business Central eğilimi modeli) | Daha önce listelenmiyor olan diğer şirket içi çözümlere sahip mevcut müşteri. İş ortağıNın Dynamics 365 Business Central'a yönelik hedefi olması gerekir. | 
| Çevik İş Süreçleri Oluşturma - Dynamics şirket içi yükleme tabanı - AX/GP/SL/NAV/Diğer (Dynamics 365 eğilimi modeli) | Çevik İş Süreçleri Oluşturma - Dynamics şirket içi yükleme tabanı - AX/GP/SL/NAV/Diğer (Dynamics 365 eğilimi modeli) | 
| Çevik İş Süreçleri Oluşturma - Dynamics rekabet tabanı - Mendix/OutSystems/Salesforce (Dynamics 365 eğilimi modeli) | Çevik iş süreçleri oluşturma - Dynamics rekabet tabanı - Mendix/OutSystems/Salesforce (Dynamics 365 eğilimi modeli) | 
| Çevik İş Süreçleri Oluşturma - Dynamics 365 Finance + Operations yükleme tabanı | Mevcut Dynamics 365 Finance + Operations müşterileri. İş ortağı hedef Power Apps. | 
| Çevik İş Süreçleri Oluşturma - Dynamics 365 Business Central yükleme tabanı | Mevcut Dynamics 365 Business Central müşterileri. İş ortağı hedef Power Apps. | 
| Çevik İş Süreçleri Oluşturma - Dynamics 365 Customer Engagement yükleme tabanı | Mevcut Dynamics 365 Customer Engagement müşterileri. İş ortağı hedef Power Apps. | 
| Bir Güçlü Tedarik Zinciri oluşturma - Windows ve Oracle olmayan veya SAP ERP (kurumsal kaynak planlama) müşterileri ile ilk Dynamics 365 iş yükünü Dynamics 365 Tedarik Zinciri Yönetimi olarak etkinleştirme | Dynamics 365 Tedarik Zinciri Yönetimi için hedef müşteriler | 
| Mevcut Dynamics 365 müşteri katılım müşterilerine dayanıklı bir tedarik zinciri oluşturun ve şirketler arası Dynamics 365 tedarik zinciri yönetimi ve/veya perakende veya ticaret | Mevcut Dynamics 365 müşteri katılımı müşterileri, şirketler arası Dynamics 365 tedarik zinciri yönetimi için hedeflenecek. | 
| Bir dayanıklı tedarik zinciri oluşturun-şirketler arası Dynamics 365 tedarik zinciri yönetimi ve/veya perakende veya ticaret, Dynamics 365 müşteri katılımı ve Oracle veya SAP 'a | Dynamics 365 tedarik zinciri yönetimi için hedeflemek üzere Oracle veya SAP ile mevcut Dynamics 365 müşteri katılımı müşterileri | 
| D365BCCluster | Dynamics 365 Business Central satın almak için müşterinin eğilimini tanımlar. Eğilimini for Business Central 'ı gösteren müşteriler orta ve küçük kategorilerde olacaktır. Hedef şimdi çalışır ve daha yüksek verim üretebilmeleri için kümeleri değerlendirir. Yalnızca Şimdi hareket ettikten ve müşterileri değerlendirdikten sonra hala kapasite varsa müşterileri Eğtir ve müşterileri eğitin. | 
| D365BCFit | Firmografları tanımlayan iç ve dış veri noktaları. Kullanım Puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünleri için olası bir uyum olup olmadığını görmek için en iyi SMB 'ye bir gevkalike modeli kullanır. Skor, üç aylık olarak güncelleştirilir. | 
| D365BCIntent | Sosyal medya ve müşterinin çevrimiçi davranışı ile ilgili sinyaller amaç tanımlar. Amaç Puanlama, kümeleri tanımlamak için uygun şekilde yer alır. Amaç Puanlama aylık olarak güncelleştirilir. | 
| D365FOCluster | Dynamics 365 finans ve Işlemlerini satın almak için müşterinin eğilimini tanımlar. Finans + Işlemlerine yönelik bir eğilimini gösteren müşteriler, en üstteki yönetilmeyen kategorilerde yer alacak. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| D365FOFit | Sıkı grafiği tanımlayan iç ve dış veri noktaları. Uygun puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünlerine potansiyel olarak uygun olup olmadığını görmek için en iyi SMB'mize benzer bir model kullanır. Fit puanlama üç aylık olarak güncelleştirilir. | 
| D365FOIntent | Sosyal medya ve müşterinin çevrimiçi davranışıyla ilgili sinyaller Amacı tanımlar. Amaç puanlama, kümeleri tanımlamak için Sığdır'ın üzerine atlar. Amaç puanlama aylık olarak güncelleştirilir. | 
| D365CECluster | Müşterinin Dynamics 365 Customer Engagement satın alma eğilimini tanımlar. Customer Engagement için bir teklifte yer alan müşteriler Orta ve Küçük kategorilerde yer atılır. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| D365CEFit | Dynamics 365 Customer Engagement için Uygun olduğunu gösterir | 
| D365CEIntent | Dynamics 365 Customer Engagement amacını gösterir | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Müşterinin Dynamics şirket içi AX veya CRM için açık yenileme olup olmadığını belirler | 
| M365UpsellCustomer | Müşterinin Microsoft 365 için büyük satış eğilimini gösterilip gösterilmeyeceğini belirler | 
| Google 'a sahiptir | Müşterinin sahip olduğu Google ürünleri için rekabet sinyalleri gösterilip gösterilmeyeceğini belirler | 
| AWS 'ye sahip | Müşterinin sahip olduğu AWS ürünleri için rekabet sinyalleri gösterilip gösterilmeyeceğini belirler | 
| EA 'ya sahiptir | Bir yenilemenin EA veya EA aboneliği olup olmadığını belirler | 
| Açık | Bir yenilemenin açık veya açık bir değer anlaşması olup olmadığını belirler | 

### <a name="cloud-ascent---azure-propensity-report"></a>**Bulut Yokent-Azure eğilimini raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| MPN Kimliği | Microsoft İş Ortağı Ağı KIMLIĞI | 
| İş ortağı adı | Ortağın adı | 
| Müşteri Kimliği | Müşteri tanımlayıcı numarası | 
| DYENIDEN sayı | Dun & Bradstreet, eğilimini için puanlanmakta olan müşterinin numarası | 
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
| SMC türü Özet | SMC türü | 
| En İyi Unmanaged - İşlem Tabanı | En çok kontrol dışı olan müşteriler – işlem | 
| En İyi Unmanaged - Kullanıcı Tabanı | En iyi unmanaged müşterileri – kullanıcılar | 
| IsNonProfit | Kuruluşun kar dışı olup olmadığını gösterir (Evet veya Hayır) | 
| Migrate-EOL Windows Server-EOL Windows Server ıB with Cloud Ascent eğilimini-5 + lisansları | Bir EOL şirket içi Windows Server (yani, bir EOL sürümü veya daha eski) olan müşteri. Müşterinin 5 veya daha fazla lisansı vardır. Eğilimini puanı olan müşteri. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Migrate-EOL Windows Server-EOL Windows Server ıB with Cloud Ascent eğilimini-<5 Lisansı | Bir EOL şirket içi Windows Server (yani, bir EOL sürümü veya daha eski) olan müşteri. Müşterinin 5 ' ten az lisansı vardır. Eğilimini puanı olan müşteri. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Migrate-EOL Windows Server-EOL Windows Server ıB, Cloud Ascent eğilimini-5 + lisanssız | Bir EOL şirket içi Windows Server (yani, bir EOL sürümü veya daha eski) olan müşteri. Müşterinin 5 ' ten fazla lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Migrate-EOL Windows Server-EOL Windows Server ıB, Cloud Ascent eğilimini-<5 Lisansı | Bir EOL şirket içi Windows Server (yani, bir EOL sürümü veya daha eski) olan müşteri. 5 ' ten az lisansa sahiptir. Müşterinin eğilimini puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL SQL - Bulut SQL Server ile EOL depolama IB - 5'ten fazla lisans | Şirket içi bir EOL sürümüne sahip SQL Server (yani, bir EOL sürümü veya daha önceki bir sürüm). Müşterinin 5'den fazla lisansı vardır. Müşterinin bir yayma puanı vardır. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL SQL - Bulut SQL Server ile EOL depolama IB - <5 lisans | Şirket içi bir EOL sürümüne sahip SQL Server (yani, bir EOL sürümü veya daha önceki bir sürüm). 5'ten az lisansa sahip. Teklif puanına sahip olan müşteri. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL SQL - Bulut SQL Server olmadan EOL depolama IB - 5'ten fazla lisans | Şirket içi bir EOL sürümüne sahip SQL Server (yani, bir EOL sürümü veya daha önceki bir sürüm). Müşterinin 5 veya daha fazla lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL SQL - Bulut SQL Server olmadan EOL SQL Server IB - <5 lisans | Şirket içi bir EOL sürümüne sahip SQL Server (yani, bir EOL sürümü veya daha önceki bir sürüm). Müşterinin 5'ten az lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Geçiş-şirket içi Windows Server-Cloud Ascent eğilimini-5 + lisanslarıyla geçerli Windows Server ıB | Geçerli bir şirket içi Windows Server (yani, EOL 'tan sonraki bir sürüm) olan müşteri. Müşterinin 5 ve lisansı vardır. Müşterinin bir eğilimini puanı vardır. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Geçiş geçişi-şirket içi Windows Server-bulut Yokent eğilimini-<5 lisanslarıyla geçerli Windows Server ıB | Geçerli bir şirket içi Windows Server (yani, EOL 'tan sonraki bir sürüm) olan müşteri. Müşterinin 5 ' ten az lisansı vardır. Müşterinin Azure için eğilimini puanı vardır. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Geçiş-şirket içi Windows Server-bulut yokuş eğilimini-5 ve lisans olmadan geçerli Windows Server ıB | Geçerli bir şirket içi Windows Server (yani, EOL 'tan sonraki bir sürüm) olan müşteri. Müşterinin 5 ve lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Geçiş-şirket içi Windows Server-bulut olmadan geçerli Windows Server ıB eğilimini-<5 lisans | Geçerli bir şirket içi Windows Server (yani, EOL 'tan sonraki bir sürüm) olan müşteri. Müşterinin 5 ' ten az lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Azure SQL veya SQL sanal makinelerine (VM) geçiş - Bulut SQL Server sahip geçerli sanal makine IB - 5'den fazla lisans | Geçerli şirket içi bulut hizmetine sahip olan SQL Server (başka bir ifadeyle, EOL'den sonraki bir sürüm). Müşterinin 5'den fazla lisansı vardır. Müşterinin bir yayma puanı vardır. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Azure SQL VEYA SQL VM'lere geçiş - bulut SQL Server eğilimi ile geçerli sanal <IB - <5 lisans | Geçerli şirket içi bulut hizmetine sahip olan SQL Server (başka bir ifadeyle, EOL'den sonraki bir sürüm). Müşterinin 5'ten az lisansı vardır. Müşterinin bir yayma puanı vardır. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Bulut Azure SQL SQL VM'lere geçiş - bulut SQL Server olmadan geçerli IB - 5'den fazla lisans | Geçerli şirket içi bulut hizmetine sahip olan SQL Server (başka bir ifadeyle, EOL'den sonraki bir sürüm). Müşterinin 5'den fazla lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Azure SQL VEYA SQL VM'lere geçiş - Bulut SQL Server eğilimi olmadan geçerli sanal <IB - <5 lisans | Geçerli şirket içi bulut hizmetine sahip olan SQL Server (başka bir ifadeyle, EOL'den sonraki bir sürüm). Müşterinin 5'ten az lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Migrate-OSS-açık kaynak Shakespeare (OSS) DB 'ye geçir | Aşağıdaki yarışmaya sahip ürünlerden birini içeren mevcut müşteri: PostgreSQL, MySQL, MariaDB. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Azure 'da-OSS-Linux geçirme | Linux ile mevcut müşteri. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Azure 'da geçiş-SAP-SAP | SAP ile mevcut müşteri. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Geçiş-Windows Sanal Masaüstü-Uzak Masaüstü Hizmetleri ıB | Etkin Windows Uzak Masaüstü Hizmetleri olan müşterileri tanımlar. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Geçirme-Windows sanal masaüstü-modern Işleri Azure 'a/WVD 'a çapraz satış | Microsoft 365 ile müşterileri tanımlar ve Azure 'a sahip değildir. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Geçiş-VMware ıB | Ürüne sahip mevcut müşteri: VMware. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Geçiş-Citrix ıB | Ürünü olan mevcut müşteri: Citrix Systems. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Yenilik - Analiz - Power BI Azure eğilimine sahip IB'ler | Power BI - Power BI Standalone Pro, Power BI - Azure Suites, Power BI - Office Paketleri, Power BI Paketleri - Microsoft 365 | 
| Etkinleştirme - GitHub ile DevOps - Visual Studio/MSDN IB | Etkin sürümlere sahip müşterileri Visual Studio tanımlar | 
| Windows Server Standard sürümü | Müşteri tarafından yapılan Windows Server Standard satın almalarının sürümünü görüntüler | 
| Windows Server Standard lisansı | Müşterinin Windows Server Standard satın almalarının lisans türünü görüntüler | 
| Windows Server Veri Merkezi sürümü | Müşteri tarafından yapılan Windows Veri Merkezi satın almalarının sürümünü görüntüler | 
| Windows Server Veri Merkezi Lisansı | Müşteri tarafından yapılan Windows Veri Merkezi satın almalarının lisans türünü görüntüler | 
| AzureFit | Sıkı grafiği tanımlayan iç ve dış veri noktaları. Uygun puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünlerine potansiyel olarak uygun olup olmadığını görmek için en iyi SMB'mize benzer bir model kullanır. Fit puanlama üç aylık olarak güncelleştirilir. | 
| AzureIntent | Sosyal medya ve müşterinin çevrimiçi davranışıyla ilgili sinyaller Amacı tanımlar. Amaç Puanlama, kümeleri tanımlamak için uygun şekilde yer alır. Amaç Puanlama aylık olarak güncelleştirilir. | 
| AzureCluster | Bir kümeye sığdırma ve amaç önerilerini birleştirerek müşterinin Azure satın alma eğilimini tanımlar. Hedef şimdi çalışır ve daha yüksek verim üretebilmeleri için kümeleri değerlendirir. Yalnızca Şimdi hareket ettikten ve müşterileri değerlendirdikten sonra hala kapasite varsa müşterileri Eğtir ve müşterileri eğitin. | 
| WindowsServerDataCenter_HasOpenRenewal | Müşterinin Windows Server Datacenter için açık yenileme olup olmadığını belirler | 
| WindowsServerStandard_HasOpenRenewal | Müşterinin Windows Server Standard için açık yenileme olup olmadığını belirler | 
| AzureUpsellCustomer | Müşterinin Azure için büyük satış eğilimini göstermeyeceğini belirler | 
| Google 'a sahiptir | Müşterinin sahip olduğu Google ürünleri için rekabet sinyalleri gösterilip gösterilmeyeceğini belirler | 
| AWS 'ye sahip | Müşterinin sahip olduğu AWS ürünleri için rekabet sinyalleri gösterilip gösterilmeyeceğini belirler | 
| EA 'ya sahiptir | Bir yenilemenin EA veya EA aboneliği olup olmadığını belirler | 
| Açık | Bir yenilemenin açık veya açık bir değer anlaşması olup olmadığını belirler | 

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
| Alt kesim | Pazar alt segmenti | 
| SMC tür Özeti | SMC türü | 
| En iyi yönetilmeyen Işlem tabanı | En çok yönetilmeyen müşteriler – işlem | 
| En çok yönetilmeyen-kullanıcı tabanı | En çok yönetilmeyen müşteriler – kullanıcılar | 
| Iskar dışı | Kuruluşun kar dışı olup olmadığını gösterir (Evet veya Hayır) | 
| Google 'a sahiptir | Müşterinin sahip olduğu AWS ürünleri için rekabet sinyalleri gösterilip gösterilmeyeceğini belirler | 
| AWS 'ye sahip | Müşterinin sahip olduğu AWS ürünleri için rekabet sinyalleri gösterilip gösterilmeyeceğini belirler | 
| Azure kümesi | Azure 'ı satın almak için müşterinin eğilimini tanımlar. Hedef şimdi çalışır ve daha yüksek verim üretebilmeleri için kümeleri değerlendirir. Yalnızca Şimdi hareket ettikten ve müşterileri değerlendirdikten sonra hala kapasite varsa müşterileri Eğtir ve müşterileri eğitin. | 
| D365 finans + Operations kümesi | Dynamics 365 finans ve Işlemlerini satın almak için müşterinin eğilimini tanımlar. Finance + Operations'a yönelik bir eğilimi olan müşteriler, en üst sırada yer alan ve en iyi tarafından kontrolsüz kategorilerde yer alan müşterilerdir. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| D365 CE Kümesi | Müşterinin Dynamics 365 Customer Engagement satın alma eğilimini tanımlar. Customer Engagement için bir teklifte yer alan müşteriler Orta ve Küçük kategorilerde yer atılır. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| D365 BC Kümesi | Müşterinin Dynamics 365 Business Central satın alma eğilimini tanımlar. Business Central için bir teklifte bulunan müşteriler Orta ve Küçük kategorilerde yer atılır. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| Microsoft 365 Kümesi | Müşterinin satın alma eğilimini Microsoft 365. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| Lisans Programı | Yenileme için lisans programı türünü tanımlar | 
| Sözleşme Kimliği | Sözleşmenin tanımlayıcısı | 
| Anlaşma bitiş tarihi | Sözleşmenin bitiş tarihi | 
| Sona erme türü | Süre sonu türü | 
| Süresi dolan gelir | Süresi dolan aboneliklerle ilişkili gelir | 
| EA 'ya sahiptir | Bir yenilemenin EA veya EA aboneliği olup olmadığını belirler | 
| Açık | Bir yenilemenin açık veya açık bir değer anlaşması olup olmadığını belirler | 
| Azure büyük satış müşterisi | Müşterinin Azure için büyük satış eğilimini göstermeyeceğini belirler | 
| Büyük satışı Microsoft 365 müşteri | Müşterinin Microsoft 365 için büyük satış eğilimini gösterilip gösterilmeyeceğini belirler | 
| RevSumDivisionName | Yenilemeye yönelik ürünü tanımlar | 

## <a name="next-steps"></a>Sonraki adımlar

Daha fazla bilgi için bkz. [raporları indirme](pci-download-reports.md).
