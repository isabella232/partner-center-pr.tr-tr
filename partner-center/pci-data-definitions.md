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
ms.openlocfilehash: 23ca20fbb2febfd4b1ea92f72fbfda5ac83d7eb6
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565517"
---
# <a name="export--data-definitions"></a>Dışarı aktarma – veri tanımları 

**Uygun roller**: rapor Görüntüleyici | Executive rapor Görüntüleyicisi

## <a name="introduction"></a>Giriş 

Öngörüler panosunda rapor Indirme merkezini kullanarak ham veri kümelerini dışarı aktarabilirsiniz. 

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
| CustomerName | Müşterinin adı | 
| CustomerTenantId | Müşteri kiracının tanımlayıcısı | 
| Customertpıd | Müşteri üst üst öğesinin tanımlayıcısı | 
| CustomerSegment | Müşteri kesimi | 
| CustomerMarket | Müşterinin coğrafi pazarı | 
| CustomerStatus | Müşteri durumu (etkin veya etkin değil) | 
| Ürün | MPN: Office 365, Dynamics 365, Enterprise Mobility ve Security, Power BI veya Microsoft Azure tarafından müşteriye satılan ürün. | 
| SKU | Ürün SKU 'SU | 
| Ay | Kullanım ve gelirin bildirildiği ay | 
| Mpnıd | Microsoft İş Ortağı Ağı tanımlayıcısı | 
| PartnerName | Ortağın adı | 
| PartnerLocation | Ortağın coğrafi konumu | 
| PartnerAttributionType | Ortağın atısyon türü | 
| SalesChannel | Satış kanalı | 
| Availablekoltuk | Kullanılabilir koltuk | 
| RevenueUSD | ABD Doları cinsinden gelir | 

### <a name="reseller-performance-report"></a>**Satıcı performans raporu**

> [!Note]
> Gelir ve Azure tüketilen gelir (ACR) verileri yalnızca Executive rapor izleyicileri olan kullanıcılar tarafından kullanılabilir.

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
| SubscriptionId | Aboneliğin GUID 'SI | 
| SubscriptionStartDate | Aboneliğin başlangıç tarihi | 
| SubscriptionEndDate | Aboneliğin bitiş tarihi | 
| SubscriptionState | Aboneliğin durumu (etkin veya uygulanmış) | 
| Ay | Kullanım ve gelirin bildirildiği ay | 
| IsAutoRenew | Aboneliğin autorenewed olup olmadığını gösterir (Evet veya Hayır) | 
| CustomerName | Müşterinin adı | 
| CustomerTenantId | Müşterinin GUID 'SI | 
| Customertpıd | Müşteri üst üst öğe tanımlayıcısı | 
| CustomerSegment | Müşterinin pazar segmenti | 
| CustomerMarket | Müşterinin coğrafi pazarı | 
| Ürün | İş ortağı tarafından müşteriye satılan ürün | 
| SKU | Ürünün SKU 'SU | 
| Mpnıd | Ortağın Microsoft İş Ortağı Ağı KIMLIĞI | 
| PartnerName | Ortağın adı | 
| PartnerLocation | Ortağın coğrafi konumu | 
| PartnerAttributionType | Abonelik için attributıon türü | 
| SalesChannel | Satış-doğrudan, bulut çözümü sağlayıcısı (CSP) vb. kanalı | 
| Availablekoltuk | Mevcut kullanılabilir bilgisayar | 
| RevenueUSD | ABD Doları cinsinden gelir | 
| Kayıt KIMLIĞI | Aboneliğin kayıt KIMLIĞI | 

### <a name="azure-usage-report"></a>**Azure kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| SubscriptionId | Aboneliğin GUID 'SI | 
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
| PartnerAttributionType | Ortağın atısyon türü | 
| SalesChannel | Satışın kanalı (doğrudan/CSP, dolaylı/CSP, doğrudan, vb.) | 
| ACR_USD | Azure tüketilen gelir (ACR) ABD Doları cinsinden | 
| Kayıt KIMLIĞI | Azure aboneliğinin kayıt KIMLIĞI | 

### <a name="office-365-license-usage-report"></a>**Office 365 lisans kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| CustomerTenantId | Müşterinin kiracı KIMLIĞI | 
| Customertpıd | Müşteri üst üst KIMLIĞI | 
| WorkloadName | Skype Kurumsal, takımlar, Exchange Online | 
| Ay | Kullanımın bildirildiği ay | 
| Paidavvailableunits | Ücretli kullanılabilir birim sayısı | 
| MonthlyActiveUsers | Aylık etkin kullanıcı sayısı | 
| CustomerName | Müşterinin adı | 
| CustomerMarket | Müşterinin pazarının coğrafi ülke konumu | 
| CustomerSegment | Müşteri segmenti | 
| MPNId | Kimlik Microsoft İş Ortağı Ağı | 
| PartnerName | İş ortağının adı | 
| PartnerLocation | İş ortağının coğrafi konumu | 
| PartnerAttributionType | İş ortağının atfı | 

### <a name="enterprise-mobility-license-usage-report"></a>**Enterprise Mobility lisans kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| CustomerTenantId | Müşterinin kiracı kimliği | 
| CustomerTpid | Müşteri üst üst kimliği | 
| WorkloadName | Enterprise Mobility + Security (EMS) iş yükünün adı | 
| Ay | Kullanımın raporlandığı ay | 
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
| MPNId | Kimlik Microsoft İş Ortağı Ağı | 
| PartnerName | İş ortağının adı | 
| PartnerLocation | İş ortağının coğrafi ülke konumu | 
| PartnerAttachType | Abonelik için asıf türü | 
| AvailableSeats | Mevcut kullanılabilir yer | 
| AssignedSeats | Geçerli atanan yer | 
| ActiveSeats | Geçerli etkin yer sayısı | 
| DeploymentOpportunity | Geçerli dağıtım fırsatı | 
| ActiveUsagePercent | Geçerli etkin kullanım yüzdesi | 

### <a name="power-bi-license-usage-report"></a>**Power BI kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
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
| Availablekoltuk | Mevcut kullanılabilir koltuk | 
| AssignedSeats | Geçerli atanan koltuk | 
| Activekoltuk | Geçerli etkin koltuk | 
| DeploymentOpportunity | Geçerli dağıtım fırsatı | 
| Activeusage yüzdesi | Geçerli etkin kullanım yüzdesi | 

### <a name="teams-meetings-and-calls-report"></a>**Takımlar toplantıları ve çağrı raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| CustomerTenantId | Müşterinin kiracı KIMLIĞI | 
| Customertpıd | Müşteri üst üst öğesinin tanımlayıcısı | 
| Ay | Kullanımın bildirildiği ay | 
| Alt iş yükü | Kullanım için raporlanan alt iş yükü (toplantılar, çağrılar veya telefon sistemleri) | 
| Toplantı sayısı | Toplantı sayısı | 
| Toplantı süresi | Toplam toplantı süresi (saat) | 

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
| Ay | Kullanımın bildirildiği ay | 
| 3P uygulama adı | Takımlar uygulamasının adı | 
| Kullanıcı sayısı | Uygulama için Kullanıcı sayısı | 


### <a name="training-details-report"></a>**Eğitim Ayrıntıları raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| Traıningactivityıd | Eğitimin tanımlayıcısı | 
| TrainingTitle | Eğitimin başlığı | 
| TrainingType | Eğitim türü (sertifikasyon veya sınav) | 
| IndividualFirstName | Müşterinin adı | 
| IndividualLastName | Müşterinin soyadı | 
| E-posta | Müşterinin kişisel e-posta kimliği | 
| CorpEmail | Müşterinin office e-posta kimliği | 
| TrainingCompletionDate | Eğitimin tamamlanma tarihi | 
| Ay | Verilerin raporlandığı ay | 
| IcMCP | Kullanıcının Bir Microsoft Sertifikalı Profesyonel (MCP) olup olmadığını gösterir | 
| MCPID | Kullanıcının MCP kimliği | 
| MPNId | Kimlik Microsoft İş Ortağı Ağı | 
| PartnerName | İş ortağının adı | 
| PartnerCityLocation | İş ortağının coğrafi şehir konumu | 
| PartnerCountryLocation | İş ortağının coğrafi ülke konumu | 

### <a name="microsoft-learn-report"></a>**Microsoft Learn raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
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
| Uzak çalışma hedefi Exchange Online 'ı etkinleştir | Etkin bir Exchange Online aboneliğine sahip olan müşteriler, Microsoft 365 için büyük satış | 
| Cloud Ascent eğilimini-+ 10 lisanslarıyla uzak Iş yerinde alımı (geçerli sürüm) etkinleştirin | Geçerli bir şirket içi Office veya Windows istemcisine sahip olan müşteri. Diğer bir deyişle, istemci sürümü yaşam sonu (EOL) sürümünden daha sonraki bir sürümdür. Müşterinin 10 veya daha fazla lisansı vardır. Eğilimini puanı olan müşteri. İş ortağı, Microsoft 365 dönüştürme için hedef almalıdır. | 
| Cloud Ascent eğilimini-<10 lisanslarıyla uzak Iş yerinde alımı (geçerli sürüm) etkinleştirin | Geçerli bir şirket içi Office veya Windows istemcisine sahip olan müşteri (yani, EOL 'tan sonraki bir sürüm). Müşterinin 10 ' dan az lisansı vardır. Eğilimini puanı olan müşteri. İş ortağı, Microsoft 365 dönüştürme için hedef almalıdır. | 
| Bulutu olmadan uzak Iş yerinde alımı (geçerli sürüm) etkinleştir eğilimini-+ 10 lisansı | Geçerli bir şirket içi Office veya Windows istemcisine sahip olan müşteri (yani, EOL 'tan sonraki bir sürüm). Müşterinin 10 veya daha fazla lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, Microsoft 365 dönüştürme için hedef almalıdır. | 
| Bulut olmadan uzak Iş-şirket içi alımı (geçerli sürüm) etkinleştir eğilimini-<10 lisans | Geçerli bir şirket içi Office veya Windows istemcisine sahip olan müşteri (yani, EOL 'tan sonraki bir sürüm). Müşterinin 10 ' dan az lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, Microsoft 365 dönüştürme için hedef almalıdır. | 
| Cloud Ascent eğilimini-+ 10 lisanslarıyla uzaktan Iş yerinde alımı (EOL sürümü) etkinleştirin | EOL şirket içi Office veya Windows istemcisine (yani, bir EOL sürümü veya daha eski) sahip olan müşteri. Müşterinin 10 veya daha fazla lisansı vardır. Müşterinin bir eğilimini puanı vardır. İş ortağı, Microsoft 365 dönüştürme için hedef almalıdır. | 
| Cloud Ascent eğilimini-<10 lisanslarıyla uzak Iş yerinde alımı (EOL sürümü) etkinleştirin | EOL şirket içi Office veya Windows istemcisine (yani, bir EOL sürümü veya daha eski) sahip olan müşteri. Müşterinin 10 ' dan az lisansı vardır. Müşterinin bir eğilimini puanı vardır. İş ortağı, Microsoft 365 dönüştürme için hedef almalıdır. | 
| Cloud Ascent eğilimini-+ 10 lisansı olmadan uzak Iş yerinde alımı (EOL sürümü) etkinleştir | Geçerli bir şirket içi Office veya Windows istemcisine sahip olan müşteri (yani, bir EOL sürümü veya daha eski). Müşterinin 10 veya daha fazla lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, Microsoft 365 dönüştürme için hedef almalıdır. | 
| Buluttan uzak Iş-şirket içi alımı (EOL sürümü) etkinleştir eğilimini-<10 lisans | Geçerli bir şirket içi Office veya Windows istemcisine sahip olan müşteri (yani, bir EOL sürümü veya daha eski). Müşterinin 10 ' dan az lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, Microsoft 365 dönüştürme için hedef almalıdır. | 
| Microsoft 365 için uzak çalışmayı etkinleştirme-yüksek-eğilimini aday (sahne NowithEvaluate) | Microsoft 365 için yüksek eğilimini aday aday müşteri | 
| Microsoft 365 ile uzak çalışmayı etkinleştirin (yakınlaştırma) | Yakınlaştırma ve Microsoft 365 olan müşteri, takımlara dönüştürme hedefi | 
| Microsoft 365 olmadan uzak çalışmayı (yakınlaştırma) etkinleştir | Yakınlaştırmalı müşteri, takımlara dönüştürme hedefi | 
| Microsoft 365 E5 için hedeflenen maliyet ve Manage-Microsoft 365 E3 'ı azaltma | Microsoft 365 E3 ile mevcut müşteri, Microsoft 365 E5 için hedef | 
| Microsoft 365 İş Premium için hedeflenen maliyet ve yönetim Microsoft 365 İş temel ve Iş standart müşterilerini azaltma | Mevcut Microsoft 365 İş temel ve Iş standart müşterileri, Microsoft 365 İş Premium için hedef | 
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
| Dijital satışı etkinleştir-Microsoft 365 özellikli boyutu >= 25 bilgisayar (SalesPro eğilimini model) | Dynamics 365 içermeyen müşteri. Koltuk boyutu: 25 +. İş ortağı Dynamics 365 SalesPro 'nun çapraz satışı için hedeflemelidir. | 
| Dijital satışı etkinleştirin-Dynamics 365 SalesPro eğilimini (Şimdi davran veya değerlendir) | Dynamics 365 içermeyen yüksek eğilimini müşterileri. İş ortağı Dynamics 365 SalesPro için hedeflemelidir. | 
| Finans riskini yönetme & sahtekarlık-Dynamics şirket içi yüklemesi temel-Navision (Business Central eğilimini model) | Şirket içi Navision ile mevcut müşteri. İş ortağı Dynamics 365 Business Central için hedeflemelidir. | 
| Finans riskini yönetme & sahtekarlık-Dynamics şirket içi Install Base-Dynamics AX (Dynamics 365 finans + Operations eğilimini model) | Şirket içi AX ile mevcut müşteri. İş ortağı, Dynamics 365 finans + Işlemleri için hedeflemelidir. | 
| Finans riskini yönetme & sahtekarlık-Dynamics şirket içi yüklemesi temel-harika Plains (Business Central eğilimini model) | Şirket içi Great Plains 'e sahip mevcut müşteri. İş ortağı Dynamics 365 Business Central için hedeflemelidir. | 
| Finans riskini yönetme & sahtekarlık-Dynamics şirket içi yüklemesi temel-Solomon (Business Central eğilimini model) | Şirket içi Solomon ile mevcut müşteri. İş ortağı Dynamics 365 Business Central için hedeflemelidir. | 
| Finans riskini yönetme & sahtekarlık-Dynamics şirket içi yüklemesi-diğerleri (Business Central eğilimini model) | Daha önce listelenmiyor olan diğer şirket içi çözümlere sahip mevcut müşteri. İş ortağıNın Dynamics 365 Business Central'a yönelik hedefi olması gerekir. | 
| Çevik İş Süreçleri Oluşturma - Dynamics şirket içi yükleme tabanı - AX/GP/SL/NAV/Diğer (Dynamics 365 eğilimi modeli) | Çevik İş Süreçleri Oluşturma - Dynamics şirket içi yükleme tabanı - AX/GP/SL/NAV/Diğer (Dynamics 365 eğilimi modeli) | 
| Çevik İş Süreçleri Oluşturma - Dynamics rekabet tabanı - Mendix/OutSystems/Salesforce (Dynamics 365 eğilimi modeli) | Çevik iş süreçleri oluşturma - Dynamics rekabet tabanı - Mendix/OutSystems/Salesforce (Dynamics 365 eğilimi modeli) | 
| Çevik İş Süreçleri Oluşturma - Dynamics 365 Finance + Operations yükleme tabanı | Mevcut Dynamics 365 Finance + Operations müşterileri. İş ortağı hedef Power Apps. | 
| Çevik İş Süreçleri Oluşturma - Dynamics 365 Business Central yükleme tabanı | Mevcut Dynamics 365 Business Central müşterileri. İş ortağı hedef Power Apps. | 
| Çevik İş Süreçleri Oluşturma - Dynamics 365 Customer Engagement yükleme tabanı | Mevcut Dynamics 365 Customer Engagement müşterileri. İş ortağı hedef Power Apps. | 
| Bir Güçlü Tedarik Zinciri oluşturma - Windows ve Oracle olmayan veya SAP ERP (kurumsal kaynak planlama) müşterileri ile ilk Dynamics 365 iş yükünü Dynamics 365 Tedarik Zinciri Yönetimi olarak etkinleştirme | Dynamics 365 Tedarik Zinciri Yönetimi için hedef müşteriler | 
| Bir Resilient Tedarik Zinciri oluşturma - Dynamics 365 Tedarik Zinciri Yönetimi ve/veya Perakende veya Ticaret'i mevcut Dynamics 365 Customer Engagement müşterilerine çapraz satış | Dynamics 365 Tedarik Zinciri Yönetimi'nin çapraz satışlarını hedeflemek için mevcut Dynamics 365 Customer Engagement müşterileri. | 
| Bir Resilient Tedarik Zinciri oluşturma - Dynamics 365 Tedarik Zinciri Yönetimi ve/veya Perakende veya Ticaret'i Dynamics 365 Customer Engagement ve Oracle veya SAP'ye çapraz satış | Dynamics 365 Tedarik Zinciri Yönetimini hedeflemek için Oracle veya SAP'ye sahip mevcut Dynamics 365 Customer Engagement müşterileri | 
| D365BCCluster | Müşterinin Dynamics 365 Business Central satın alma eğilimini tanımlar. Business Central için bir teklifte bulunan müşteriler Orta ve Küçük kategorilerde yer atılır. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| D365BCFit | Sıkı grafiği tanımlayan iç ve dış veri noktaları. Uygun puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünlerine potansiyel olarak uygun olup olmadığını görmek için en iyi SMB'mize benzer bir model kullanır. Fit puanlama üç aylık olarak güncelleştirilir. | 
| D365BCIntent | Sosyal medya ve müşterinin çevrimiçi davranışıyla ilgili sinyaller Amacı tanımlar. Amaç puanlama, kümeleri tanımlamak için Sığdır'ın üzerine atlar. Amaç puanlama aylık olarak güncelleştirilir. | 
| D365FOCluster | Müşterinin Dynamics 365 Finance and Operations satın alma eğilimini tanımlar. Finance + Operations'a yönelik bir eğilimi olan müşteriler, en üst sırada yer alan ve en iyi tarafından kontrolsüz kategorilerde yer alan müşterilerdir. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| D365FOFit | Sıkı grafiği tanımlayan iç ve dış veri noktaları. Uygun puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünlerine potansiyel olarak uygun olup olmadığını görmek için en iyi SMB'mize benzer bir model kullanır. Fit puanlama üç aylık olarak güncelleştirilir. | 
| D365FOIntent | Sosyal medya ve müşterinin çevrimiçi davranışıyla ilgili sinyaller Amacı tanımlar. Amaç puanlama, kümeleri tanımlamak için Sığdır'ın üzerine atlar. Amaç puanlama aylık olarak güncelleştirilir. | 
| D365CECluster | Müşterinin Dynamics 365 Customer Engagement satın alma eğilimini tanımlar. Customer Engagement için bir teklifte yer alan müşteriler Orta ve Küçük kategorilerde yer atılır. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| D365CEFit | Dynamics 365 Customer Engagement için Uygun olduğunu gösterir | 
| D365CEIntent | Dynamics 365 Customer Engagement amacını gösterir | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Müşterinin Dynamics şirket içi AX veya CRM için açık yenilemeye sahip olup olmadığını tanımlar | 
| M365UpsellCustomer | Müşterinin müşteriler için satış eğilimi gösterip Microsoft 365 | 
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
| Migrate-EOL Windows Server-EOL Windows Server ıB with Cloud Ascent eğilimini-5 + lisansları | Bir EOL şirket içi Windows Server (yani, bir EOL sürümü veya daha eski) olan müşteri. Müşterinin 5 veya daha fazla lisansı vardır. Eğilimini puanı olan müşteri. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Migrate-EOL Windows Server-EOL Windows Server ıB with Cloud Ascent eğilimini-<5 Lisansı | Bir EOL şirket içi Windows Server (yani, bir EOL sürümü veya daha eski) olan müşteri. Müşterinin 5 ' ten az lisansı vardır. Eğilimini puanı olan müşteri. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Migrate-EOL Windows Server-EOL Windows Server ıB, Cloud Ascent eğilimini-5 + lisanssız | Bir EOL şirket içi Windows Server (yani, bir EOL sürümü veya daha eski) olan müşteri. Müşterinin 5 ' ten fazla lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Migrate-EOL Windows Server-EOL Windows Server ıB, Cloud Ascent eğilimini-<5 Lisansı | Bir EOL şirket içi Windows Server (yani, bir EOL sürümü veya daha eski) olan müşteri. 5 ' ten az lisansa sahiptir. Müşterinin eğilimini puanı yok. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Cloud Ascent eğilimini-5 + lisanslarıyla geçiş-EOL SQL-EOL SQL Server ıB | Bir EOL şirket içi SQL Server (yani, bir EOL sürümü veya daha eski) olan müşteri. Müşterinin 5 ve lisansı vardır. Müşterinin bir eğilimini puanı vardır. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Cloud Ascent eğilimini-<5 lisanslarıyla geçiş-EOL SQL-EOL SQL Server ıB | Bir EOL şirket içi SQL Server (yani, bir EOL sürümü veya daha eski) olan müşteri. 5 ' ten az lisansa sahiptir. Eğilimini puanı olan müşteri. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Cloud Ascent eğilimini-5 + lisansı olmadan Migrate-EOL SQL-EOL SQL Server ıB | Bir EOL şirket içi SQL Server (yani, bir EOL sürümü veya daha eski) olan müşteri. Müşterinin 5 veya daha fazla lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Buluta geçiş-EOL SQL-EOL SQL Server ıB, bulut Yokent eğilimini-<5 Lisansı | Bir EOL şirket içi SQL Server (yani, bir EOL sürümü veya daha eski) olan müşteri. Müşterinin 5 ' ten az lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Geçiş-şirket içi Windows Server-Cloud Ascent eğilimini-5 + lisanslarıyla geçerli Windows Server ıB | Geçerli bir şirket içi Windows Server (yani, EOL 'tan sonraki bir sürüm) olan müşteri. Müşterinin 5 ve lisansı vardır. Müşterinin bir eğilimini puanı vardır. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Geçiş geçişi-şirket içi Windows Server-bulut Yokent eğilimini-<5 lisanslarıyla geçerli Windows Server ıB | Geçerli bir şirket içi Windows Server (yani, EOL 'tan sonraki bir sürüm) olan müşteri. Müşterinin 5 ' ten az lisansı vardır. Müşterinin Azure için eğilimini puanı vardır. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Geçiş-şirket içi Windows Server-bulut yokuş eğilimini-5 ve lisans olmadan geçerli Windows Server ıB | Geçerli bir şirket içi Windows Server (yani, EOL 'tan sonraki bir sürüm) olan müşteri. Müşterinin 5 ve lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Geçiş-şirket içi Windows Server-bulut olmadan geçerli Windows Server ıB eğilimini-<5 lisans | Geçerli bir şirket içi Windows Server (yani, EOL 'tan sonraki bir sürüm) olan müşteri. Müşterinin 5 ' ten az lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Geçiş-Azure SQL 'e veya SQL sanal makinelerine (VM) geçiş-Cloud Ascent eğilimini-5 + lisanslarıyla güncel SQL Server IB | Geçerli bir şirket içi SQL Server (yani, EOL 'tan sonraki bir sürüm) olan müşteri. Müşterinin 5 ve lisansı vardır. Müşterinin bir eğilimini puanı vardır. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Geçiş-Azure SQL veya SQL VM 'lerine geçiş-Cloud Ascent eğilimini-<5 lisanslarıyla geçerli SQL Server IB | Geçerli bir şirket içi SQL Server (yani, EOL 'tan sonraki bir sürüm) olan müşteri. Müşterinin 5 ' ten az lisansı vardır. Müşterinin bir eğilimini puanı vardır. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Geçiş-Azure SQL veya SQL VM 'lerine geçiş-bulut Yokent eğilimini-5 ve lisans olmadan geçerli SQL Server IB | Geçerli bir şirket içi SQL Server (yani, EOL 'tan sonraki bir sürüm) olan müşteri. Müşterinin 5 ve lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Geçiş-Azure SQL veya SQL VM 'lerine geçiş-bulut Yokent eğilimini-<5 lisansı olmadan geçerli SQL Server IB | Geçerli bir şirket içi SQL Server (yani, EOL 'tan sonraki bir sürüm) olan müşteri. Müşterinin 5 ' ten az lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Migrate-OSS-açık kaynak Shakespeare (OSS) DB 'ye geçir | Aşağıdaki yarışmaya sahip ürünlerden birini içeren mevcut müşteri: PostgreSQL, MySQL, MariaDB. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Azure 'da-OSS-Linux geçirme | Linux ile mevcut müşteri. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçirme - SAP - Azure üzerinde SAP | SAP ile mevcut müşteri. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Windows Sanal Masaüstü - Uzak Masaüstü Hizmetleri IB | Etkin Windows hesabı olan Uzak Masaüstü Hizmetleri. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Windows Sanal Masaüstü - Modern Çalışmaları Azure'a Çapraz Satış/WVD | Azure'Microsoft 365 sahip olmayan müşterileri tanımlar. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - VMware IB | Ürüne sahip mevcut müşteri: VMware. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçirme - Citrix IB | Ürünü olan mevcut müşteri: Citrix Systems. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Yenilik - Analiz - Power BI Azure eğilimine sahip IB'ler | Power BI - Power BI Standalone Pro, Power BI - Azure Paketleri, Power BI - Office Paketleri, Power BI Paketleri - Microsoft 365 | 
| Etkinleştirme - GitHub ile DevOps - Visual Studio/MSDN IB | Etkin sürümlere sahip müşterileri Visual Studio tanımlar | 
| Windows Server Standard sürümü | Müşteri tarafından yapılan Windows Server Standard satın almalarının sürümünü görüntüler | 
| Windows Server Standard lisansı | Müşterinin Windows Server Standard satın almalarının lisans türünü görüntüler | 
| Windows Server Veri Merkezi sürümü | Müşteri tarafından yapılan Windows Veri Merkezi satın almalarının sürümünü görüntüler | 
| Windows Server Veri Merkezi Lisansı | Müşteri tarafından yapılan Windows Veri Merkezi satın almalarının lisans türünü görüntüler | 
| AzureFit | Sıkı grafiği tanımlayan iç ve dış veri noktaları. Uygun puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünlerine potansiyel olarak uygun olup olmadığını görmek için en iyi SMB'mize benzer bir model kullanır. Fit puanlama üç aylık olarak güncelleştirilir. | 
| AzureIntent | Sosyal medya ve müşterinin çevrimiçi davranışıyla ilgili sinyaller Amacı tanımlar. Amaç puanlama, kümeleri tanımlamak için Sığdır'ın üzerine atlar. Amaç puanlama aylık olarak güncelleştirilir. | 
| AzureCluster | Fit ve Intent önerilerini bir kümede bir arada kullanarak müşterinin Azure satın alma eğilimini tanımlar. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| WindowsServerDataCenter_HasOpenRenewal | Müşterinin Windows Server Datacenter için açık yenilemesi olup olmadığını tanımlar | 
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
| En İyi Unmanaged - Kullanıcı Tabanı | En çok kontrol dışı müşteriler – kullanıcılar | 
| IsNonProfit | Kuruluşun kar amacı gütmeyen kuruluş olup olmadığını gösterir (Evet veya Hayır) | 
| Google'a sahip | Müşterinin AWS ürünlerine sahip olan müşterilere yönelik rekabet sinyalleri gösterip gösterip gösterir | 
| AWS'ye sahip | Müşterinin AWS ürünlerine sahip olan müşterilere yönelik rekabet sinyalleri gösterip gösterip gösterir | 
| Azure Kümesi | Müşterinin Azure satın alma eğilimini tanımlar. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| D365 Finance + Operations Cluster | Müşterinin Dynamics 365 Finance and Operations satın alma eğilimini tanımlar. Finance + Operations'a yönelik bir eğilimi olan müşteriler, en üst sırada yer alan ve en iyi tarafından kontrolsüz kategorilerde yer alan müşterilerdir. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| D365 CE Kümesi | Müşterinin Dynamics 365 Customer Engagement satın alma eğilimini tanımlar. Customer Engagement için bir teklifte yer alan müşteriler Orta ve Küçük kategorilerde yer atılır. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| D365 BC Kümesi | Müşterinin Dynamics 365 Business Central satın alma eğilimini tanımlar. Business Central için bir teklifte bulunan müşteriler Orta ve Küçük kategorilerde yer atılır. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| Microsoft 365 Kümesi | Müşterinin satın alma eğilimini Microsoft 365. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| Lisans Programı | Yenileme için lisans programı türünü tanımlar | 
| Sözleşme Kimliği | Sözleşmenin tanımlayıcısı | 
| Sözleşme Bitiş Tarihi | Sözleşmenin bitiş tarihi | 
| Süre Sonu Türü | Süre sonu türü | 
| Süresi Dolan Gelir | Süresi dolan aboneliklerle ilişkili gelir | 
| EA'ya sahip | Yenilemenin EA aboneliği mi yoksa EA aboneliği mi olduğunu tanımlar | 
| Açık | Yenilemenin Açık veya Açık Değer sözleşmesi olup olmadığını tanımlar | 
| Azure Upsell müşterisi | Müşterinin Azure için satış eğilimi gösterip gösterip gösterir olmadığını tanımlar | 
| Microsoft 365 Upsell müşterisi | Müşterinin müşteriler için satış eğilimi gösterip Microsoft 365 | 
| RevSumDivisionName | Yenilemeye hazır olan ürünü tanımlar | 

## <a name="next-steps"></a>Sonraki adımlar

Daha fazla bilgi için bkz. [Raporları indirme.](pci-download-reports.md)
