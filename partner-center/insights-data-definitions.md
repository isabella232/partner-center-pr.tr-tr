---
title: İçgörü verilerinin tanımları
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Belgede çeşitli raporlar ve bunların veri tanımları listelenmiş ve rapor indirme sayfasından Analizler indirebilirsiniz.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c77f5eb97771c4768f76b8d35c0d4493c5070ff2
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377434"
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
| CustomerName | Müşterinin adı | 
| CustomerTenantId | Müşteri kiracısı tanımlayıcısı | 
| CustomerTpid | Müşterinin üst üst öğenin tanımlayıcısı | 
| CustomerSegment | Müşteri segmenti | 
| CustomerMarket | Müşterinin coğrafi pazar | 
| CustomerStatus | Müşteri durumu (Etkin veya Etkin Değil) | 
| Ürün | Müşteriye MPN tarafından satılan ürün: Office 365, Dynamics 365, Enterprise Mobility and Security, Power BI veya Microsoft Azure | 
| SKU | Ürün SKU'su | 
| Ay | Kullanım ve gelirin raporlandığı ay | 
| MPNId | Kimlik Microsoft İş Ortağı Ağı | 
| PartnerName | İş ortağının adı | 
| PartnerLocation | İş ortağının coğrafi konumu | 
| PartnerAttributionType | İş ortağının atfı | 
| SalesChannel | Satış kanalı | 
| AvailableSeats | Kullanılabilir yer | 
| RevenueUSD | ABD doları geliri | 

### <a name="reseller-performance-report"></a>**Kurumsal bayi performans raporu**

> [!Note]
> Gelir ve Azure tüketilen gelir (ACR) verileri yalnızca Yönetici raporu görüntüleyicisi olan kullanıcılar tarafından kullanılabilir.

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
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
| SubscriptionId | Aboneliğin GUID'si | 
| SubscriptionStartDate | Aboneliğin başlangıç tarihi | 
| SubscriptionEndDate | Aboneliğin bitiş tarihi | 
| SubscriptionState | Aboneliğin durumu (Etkin veya Eskitildi) | 
| Ay | Kullanım ve gelirin raporlandığı ay | 
| IsAutoRenew | Aboneliğin otomatik olarak yenilenip yenil olmadığını gösterir (Evet veya Hayır) | 
| CustomerName | Müşterinin adı | 
| CustomerTenantId | Müşterinin GUID'si | 
| CustomerTpid | Müşteri üst üst tanımlayıcısı | 
| CustomerSegment | Müşterinin pazar segmenti | 
| CustomerMarket | Müşterinin coğrafi pazar | 
| Ürün | İş ortağı tarafından müşteriye satılan ürün | 
| SKU | Ürünün SKU'su | 
| MPNId | Microsoft İş Ortağı Ağı ortağın kimlik numarası | 
| PartnerName | İş ortağının adı | 
| PartnerLocation | İş ortağının coğrafi konumu | 
| PartnerAttributionType | Abonelik için asıf türü | 
| SalesChannel | Satış kanalı - Doğrudan, Bulut Çözümü Sağlayıcısı (CSP) ve diğer | 
| AvailableSeats | Mevcut kullanılabilir yer | 
| RevenueUSD | ABD doları geliri | 
| Kayıt Kimliği | Aboneliğin kayıt kimliği | 

### <a name="azure-usage-report"></a>**Azure kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| SubscriptionId | Aboneliğin GUID'si | 
| SubscriptionStartDate | Aboneliğin başlangıç tarihi | 
| SubscriptionEndDate | Aboneliğin bitiş tarihi | 
| SubscriptionState | Aboneliğin geçerli durumu (Açık, Kapalı, Etkin veya Yetkisiz Kullanım Süresinde) | 
| Ay | Aya göre toplanan tarih | 
| ServiceName | Azure hizmetinin adı | 
| MeterCategory | Ölçüm kategorisinin adı | 
| UsageUnits | Faturalama döngüsü sırasında kullanılan birim sayısı | 
| CustomerName | Müşterinin adı | 
| CustomerTenantId | Müşterinin kiracı kimliği | 
| CustomerTpid | Müşteri üst üst kimliği | 
| CustomerSegment | Müşterinin segmenti | 
| CustomerMarket | Müşterinin coğrafi pazar | 
| MPNId | Microsoft İş Ortağı Ağı kimliği | 
| PartnerName | İş ortağının adı | 
| PartnerLocation | İş ortağının coğrafi ülke konumu | 
| PartnerAttributionType | İş ortağının atfı | 
| SalesChannel | Satış kanalı (Doğrudan/CSP, Dolaylı/CSP, Doğrudan ve diğer) | 
| ACR_USD | ABD doları olarak Azure tarafından tüketilen gelir (ACR) | 
| Kayıt Kimliği | Azure aboneliğinin kayıt kimliği | 

### <a name="office-365-license-usage-report"></a>**Office 365 kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| CustomerTenantId | Müşterinin kiracı kimliği | 
| CustomerTpid | Müşteri üst üst kimliği | 
| WorkloadName | Skype Kurumsal, Teams, Exchange Online | 
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

### <a name="teams-meetings-and-calls-report"></a>**Teams toplantılar ve çağrılar raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| CustomerTenantId | Müşterinin kiracı KIMLIĞI | 
| Customertpıd | Müşteri üst üst öğesinin tanımlayıcısı | 
| Ay | Kullanımın bildirildiği ay | 
| Alt iş yükü | Kullanım için raporlanan alt iş yükü (toplantılar, çağrılar veya telefon sistemleri) | 
| Toplantı sayısı | Toplantı sayısı | 
| Toplantı süresi | Toplam toplantı süresi (saat) | 

### <a name="teams-monthly-usage-report"></a>**Teams aylık kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| CustomerTenantId | Müşterinin kiracı KIMLIĞI | 
| Customertpıd | Müşteri üst üst öğesinin tanımlayıcısı | 
| Ay | Kullanımın bildirildiği ay | 
| Alt iş yükü | Kullanım için raporlanan alt iş yükü (toplantılar, çağrılar veya telefon sistemleri) | 
| Masaüstü kullanıcıları | masaüstünde Teams kullanan kullanıcı sayısı | 
| Mobil Kullanıcılar | mobil üzerinde Teams kullanan kullanıcı sayısı | 
| Web kullanıcıları | web üzerinde Teams kullanan kullanıcı sayısı | 
| Allupkatılımcıları | ay için Teams benzersiz kullanıcı sayısı | 

### <a name="teams-usage-3p-apps-report"></a>**Teams kullanımı 3p apps raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| CustomerTenantId | Müşterinin kiracı KIMLIĞI | 
| Customertpıd | Müşteri üst üst KIMLIĞI | 
| Ay | Kullanımın bildirildiği ay | 
| 3P uygulama adı | Teams uygulamasının adı | 
| Kullanıcı sayısı | Uygulama için Kullanıcı sayısı | 


### <a name="training-details-report"></a>**Eğitim Ayrıntıları raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| Traıningactivityıd | Eğitimin tanımlayıcısı | 
| Traıningtitle | Eğitimin başlığı | 
| Traıningtype | Eğitim türü (sertifika veya sınava) | 
| Kişiselleştirsoyadı | Müşterinin ilk adı | 
| Kişiselleştirallastname | Müşterinin soyadı | 
| E-posta | Müşterinin kişisel e-posta KIMLIĞI | 
| CorpEmail | müşterinin Office e-posta kimliği | 
| Traıningcompletiondate | Eğitimin tamamlanma tarihi | 
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
| Uzaktan Çalışma Etkinleştirme - hedef Exchange Online | Etkin bir Exchange Online aboneliği olan müşteriler, Microsoft 365 | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi ile şirket içi alım (geçerli sürüm) - +10 lisans | Geçerli bir şirket içi müşterisi olan Office veya Windows. Başka bir ifadeyle, istemci sürümü yaşam sonu (EOL) sürümünden daha eskidir. Müşterinin 10 veya daha fazla lisansı vardır. Teklif puanına sahip olan müşteri. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi ile şirket içi alım (geçerli sürüm) - <10 lisans | Geçerli şirket içi istemciye sahip olan Office Windows (yani, EOL'den sonraki bir sürüm). Müşterinin 10'dan az lisansı vardır. Teklif puanına sahip olan müşteri. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi olmadan şirket içi alım (geçerli sürüm) - +10 lisans | Geçerli şirket içi istemciye sahip olan Office Windows (yani, EOL'den sonraki bir sürüm). Müşterinin 10 veya daha fazla lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağı, iş ortağının Microsoft 365. | 
| Uzaktan Çalışma Etkinleştirme - Bulut Ascent eğilimi olmadan şirket içi alım (geçerli sürüm) - <10 lisans | Geçerli şirket içi istemciye sahip olan Office Windows (yani, EOL'den sonraki bir sürüm). Müşterinin 10'dan az lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağı, iş ortağının Microsoft 365. | 
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
| DUNS Numarası | Dun &, yayma puanı alan müşterinin Bradstreet numarasını aldı | 
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
| SMC Tür Özeti | Bir müşterinin kategorilere ayırması: En fazla 300 çalışana sahip müşteriler, en fazla 300 çalışana sahip müşteriler, en üst düzeydeki verimsiz işlem tabanları Azure'da üç yıllık potansiyele sahip müşteriler, orta büyüklükteki işletmeler 25 veya daha fazla çalışana sahip müşteriler ve küçük işletmeler ise 25'ten az çalışanı olan müşterilerdir. | 
| En İyi Unmanaged - İşlem Tabanı | En çok kontrol dışı olan müşteriler – işlem | 
| En İyi Unmanaged - Kullanıcı Tabanı | En iyi unmanaged müşterileri – kullanıcılar | 
| IsNonProfit | Kuruluşun kar amacı gütmeyen bir kuruluş olup olmadığını gösterir (Evet veya Hayır) | 
| Dijital Satış Etkinleştirme - Microsoft 365 - lisans boyutu >= 25 lisans (SalesPro eğilimi modeli) | Dynamics 365 olmayan müşteri. Seat size: 25+. İş ortağıNın Dynamics 365 SalesPro çapraz satışını hedeflemesi gerekir. | 
| Dijital Satışı Etkinleştirme - Dynamics 365 SalesPro eğilimi (Şimdi Harekete Geç veya Değerlendir) | Dynamics 365 olmayan yüksek performanslı müşteriler. İş ortağıNın Dynamics 365 SalesPro'ya yönelik hedefi olması gerekir. | 
| Finansal Risk Yönetimi & Sahtekarlık - Dynamics şirket içi yükleme tabanı - Navision (Business Central eğilimi modeli) | Şirket içi Navision'a sahip mevcut müşteri. İş ortağıNın Dynamics 365 Business Central'a yönelik hedefi olması gerekir. | 
| Finansal Risk Yönetimi & Sahtekarlık - Dynamics şirket içi yükleme tabanı - Dynamics AX (Dynamics 365 Finance + Operations propensity model) | Şirket içi AX'e sahip mevcut müşteri. İş ortağıNın Dynamics 365 Finance + Operations'i hedeflemesi gerekir. | 
| Finansal Risk Yönetimi & Sahtekarlık - Dynamics şirket içi yükleme tabanı - Great Plains (Business Central eğilimi modeli) | Şirket içi Great Plains'e sahip mevcut müşteri. İş ortağıNın Dynamics 365 Business Central'a yönelik hedefi olması gerekir. | 
| Finansal Risk Yönetimi & Sahtekarlık - Dynamics şirket içi yükleme tabanı - Dynamics (Business Central eğilimi modeli) | Şirket içi Hizmet Merkezi olan mevcut müşteri. İş ortağıNın Dynamics 365 Business Central'a yönelik hedefi olması gerekir. | 
| Finansal Risk Yönetimi & Sahtekarlık - Dynamics şirket içi yükleme tabanı - Diğer (Business Central eğilimi modeli) | Diğer şirket içi çözümlere sahip mevcut müşteri daha önce listelenmemiş. İş ortağı Dynamics 365 Business Central için hedeflemelidir. | 
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
| Iskar dışı | Kuruluşun kar amacı gütmeyen bir kuruluş olup olmadığını gösterir (Evet veya Hayır) | 
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
| Azure Upsell müşterisi | Müşterinin Azure için satış eğilimi gösterip gösterip gösterir olmadığını tanımlar | 
| Microsoft 365 Müşteriye satış | Müşterinin sipariş için satış eğilimi gösterip Microsoft 365 | 
| RevSumDivisionName | Yenilemeye hazır olan ürünü tanımlar | 

## <a name="next-steps"></a>Sonraki adımlar

Daha fazla bilgi için bkz. [Raporları indirme.](insights-download-reports.md)
