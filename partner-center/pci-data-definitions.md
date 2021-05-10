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
ms.openlocfilehash: 21be5b22c453174fcb66e9409d6e26dad8e25c6b
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686356"
---
# <a name="export--data-definitions"></a>Dışarı aktarma – veri tanımları 

**Uygun roller** 

- Rapor Görüntüleyicisi
- Executive rapor Görüntüleyicisi

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

### <a name="customer-details-report"></a>**Müşteri ayrıntıları raporu**

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
| AvailableSeats | Kullanılabilir yer | 
| RevenueUSD | ABD doları geliri | 

### <a name="reseller-performance-report"></a>**Kurumsal bayi performans raporu**

> [!Note]
> Gelir ve ACR verileri yalnızca Yönetici raporu görüntüleyicisi olan kullanıcılar tarafından kullanılabilir.

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
| SubscriptionId | Aboneliğin GUID'si | 
| SubscriptionStartDate | Aboneliğin başlangıç tarihi | 
| SubscriptionEndDate | Aboneliğin bitiş tarihi | 
| SubscriptionState | Aboneliğin durumu (Etkin veya Eskitildi) | 
| Ay | Kullanım ve gelirin raporlandığı ay | 
| IsAutoRenew | Aboneliğin otomatik olarak yenilenin (Evet veya Hayır) olup olmadığını gösterir | 
| CustomerName | Müşterinin adı | 
| CustomerTenantId | Müşterinin GUID'si | 
| CustomerTpid | Müşteri üst üst tanımlayıcısı | 
| CustomerSegment | Müşterinin pazar segmenti | 
| CustomerMarket | Müşterinin coğrafi pazar | 
| Ürün | İş ortağı tarafından müşteriye satılan ürün | 
| SKU | Ürünün SKU'su | 
| Mpnıd | Ortağın Microsoft İş Ortağı Ağı KIMLIĞI | 
| PartnerName | Ortağın adı | 
| PartnerLocation | Ortağın coğrafi konumu | 
| PartnerAttributionType | Abonelik için attributıon türü | 
| SalesChannel | Sales-Direct, CSP (bulut çözümü sağlayıcısı) vb. kanalı | 
| Availablekoltuk | Mevcut kullanılabilir bilgisayar | 
| RevenueUSD | ABD Doları cinsinden gelir | 
| Kayıt KIMLIĞI | Aboneliğin kayıt KIMLIĞI | 

### <a name="azure-usage-report"></a>**Azure kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| SubscriptionId | Aboneliğin GUID 'SI | 
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
| Paidavvailableunits | Ücretli kullanılabilir birim sayısı | 
| MonthlyActiveUsers | Aylık etkin kullanıcı sayısı | 
| CustomerName | Müşterinin adı | 
| CustomerMarket | Müşterinin pazarına ait coğrafi ülke konumu | 
| CustomerSegment | Müşteri kesimi | 
| Mpnıd | Microsoft İş Ortağı Ağı tanımlayıcısı | 
| PartnerName | Ortağın adı | 
| PartnerLocation | Ortağın coğrafi konumu | 
| PartnerAttributionType | Ortağın atısyon türü | 

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
| Activeusage yüzdesi | Geçerli etkin kullanım yüzdesi | 

### <a name="power-bi-license-usage-report"></a>**Power BI Lisansı kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| SubscriptionId | Aboneliğin GUID 'SI | 
| SubscriptionStartDate | Aboneliğin başlangıç tarihi | 
| SubscriptionEndDate | Aboneliğin bitiş tarihi | 
| Abonelik durumu | Aboneliğin durumu (etkin, etkin değil veya yetkisiz kullanım süresi) | 
| Ay | Aya göre toplanan Tarih | 
| SKU | Ürünün SKU 'SU | 
| SkuId | Ürünün SKU KIMLIĞI | 
| Freevspaıdsku | Ücretsiz veya ücretli SKU farklılaştırıcısı | 
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
| Toplantı süresi | Saat olarak toplam toplantı süresi | 

### <a name="teams-monthly-usage-report"></a>**Teams aylık kullanım raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| CustomerTenantId | Müşterinin kiracı kimliği | 
| CustomerTpid | Müşterinin üst üst öğenin tanımlayıcısı | 
| Ay | Kullanımın raporlandığı ay | 
| Alt iş yükü | Kullanımın raporlandığı alt iş yükü (toplantılar, aramalar veya telefon sistemleri) | 
| Masaüstü Kullanıcıları | Masaüstünde Teams kullanan kullanıcı sayısı | 
| Mobil Kullanıcılar | Mobil cihazlarda Teams kullanan kullanıcı sayısı | 
| Web Kullanıcıları | Web'de Teams kullanan kullanıcı sayısı | 
| AllUpParticipants | Ay için Teams'in benzersiz kullanıcı sayısı | 

### <a name="teams-usage-3p-apps-report"></a>**Teams kullanım 3P uygulamaları raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| CustomerTenantId | Müşterinin kiracı kimliği | 
| Customertpıd | Müşteri üst üst KIMLIĞI | 
| Ay | Kullanımın bildirildiği ay | 
| 3P uygulama adı | Takımlar uygulamasının adı | 
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
| Uzaktan Çalışma Özelliğini Etkinleştirme - uzaktan çalışma olmadan rekabet Microsoft 365 | Yakınlaştırmalı müşteri, Teams'e dönüştürme hedefi | 
| Maliyeti Azaltma ve Yönetme - Microsoft 365 E5 için hedeflenen E3 Microsoft 365 | Microsoft 365 E5 Microsoft 365 E3'e sahip mevcut müşteri | 
| Maliyeti ve Yönetimi Azaltma - Microsoft 365 İş Ekstra için hedeflenen İş Temel ve İş Standardı Microsoft 365 müşteriler | mevcut Microsoft 365 Business Basic ve Business Standard müşterileri, Microsoft 365 Premium için hedeftir | 
| Kuruluş Üretkenliğini Dönüştürme - Yüzey eğilimi | Müşteri Surface için bir eğilimi gösteriyor | 
| M365Cluster | Müşterinin satın alma eğilimini Microsoft 365. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir hedefle'den sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| M365Fit | Sıkı grafiği tanımlayan iç ve dış veri noktaları. Uygun puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünleri için potansiyel olarak uygun olup olmadığını görmek için en küçük veya orta ölçekli işletmelere (SMB) benzer bir model kullanır. Fit puanlama üç aylık olarak güncelleştirilir. | 
| M365Intent | Sosyal medya ve müşterinin çevrimiçi davranışıyla ilgili sinyaller Amacı tanımlar. Amaç puanlama, kümeleri tanımlamak için Sığdır'ın üzerine atlar. Amaç puanlama aylık olarak güncelleştirilir. | 
| SurfaceCluster | Bir kümeye sığdırma ve amaç önerilerini birleştirerek bir müşterinin eğilimini ' i, yüzeyi satın almasını belirler. Hedef şimdi çalışır ve daha yüksek verim üretebilmeleri için kümeleri değerlendirir. Yalnızca Şimdi hareket eden ve müşterilerin hedeflediği bir kapasite varsa müşterileri Eğtir ve müşterileri eğitin. | 
| Surçok yönlü sığdırma | Firmografları tanımlayan iç ve dış veri noktaları. Kullanım Puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünleri için olası bir uyum olup olmadığını görmek için en iyi SMB kuruluşlarımızda bir gevmüike modeli kullanır. Skor, üç aylık olarak güncelleştirilir. | 
| Surçok yönlü amaç | Sosyal medya ve müşterinin çevrimiçi davranışı ile ilgili sinyaller amaç tanımlar. Amaç Puanlama, kümeleri tanımlamak için uygun şekilde yer alır. Amaç Puanlama aylık olarak güncelleştirilir. | 
| O365Cluster | Office 365 satın almak için müşterinin eğilimini tanımlar. Hedef şimdi çalışır ve daha yüksek verim üretebilmeleri için kümeleri değerlendirir. Yalnızca Şimdi hareket eden ve müşterilerin hedeflediği bir kapasite varsa müşterileri Eğtir ve müşterileri eğitin. | 
| O365Fit | Firmografları tanımlayan iç ve dış veri noktaları. Kullanım Puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünleri için olası bir uyum olup olmadığını görmek için en iyi SMB kuruluşlarımızda bir gevmüike modeli kullanır. Skor, üç aylık olarak güncelleştirilir. | 
| O365Intent | Sosyal medya ve müşterinin çevrimiçi davranışıyla ilgili sinyaller Amacı tanımlar. Amaç puanlama, kümeleri tanımlamak için Sığdır'ın üzerine atlar. Amaç puanlama aylık olarak güncelleştirilir. | 
| M365UpsellCustomer | Müşterinin müşteriler için satış eğilimi gösterip Microsoft 365 | 
| Google'a sahip | Müşterinin Google ürünlerine sahip olmak için rekabet sinyalleri gösterip gösterip gösterir olmadığını tanımlar | 
| AWS'ye sahip | Müşterinin kendi (AWS) ürünlerine sahip olmak için Amazon Web Services sinyalleri gösterip gösterip gösterir | 
| EA'ya sahip | Yenilemenin kurumsal anlaşma (EA) veya EA aboneliği olup olmadığını tanımlar | 
| Açık | Yenilemenin Açık veya Açık Değer sözleşmesi olup olmadığını tanımlar | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Bulut Ascent - Dynamics 365 eğilimi raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| MPN Kimliği | Microsoft İş Ortağı Ağı kimliği | 
| İş Ortağı Adı | İş ortağının adı | 
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
| En iyi yönetilmeyen Işlem tabanı | En çok kontrol dışı olan müşteriler – işlem | 
| En İyi Unmanaged - Kullanıcı Tabanı | En iyi unmanaged müşterileri – kullanıcılar | 
| IsNonProfit | Kuruluşun kar amacı gütmeyen kuruluş olup olmadığını gösterir (Evet veya Hayır) | 
| Dijital Satış etkinleştirme - Microsoft 365 - lisans boyutu >= 25 lisans (SalesPro eğilimi modeli) | Dynamics 365 olmayan müşteri. Seat size: 25+. İş ortağının Dynamics 365 SalesPro çapraz satışını hedeflemesi gerekir. | 
| Dijital Satışı Etkinleştirme - Dynamics 365 SalesPro eğilimi (Şimdi Harekete Geç veya Değerlendir) | Dynamics 365 olmayan yüksek performanslı müşteriler. İş ortağıNın Dynamics 365 SalesPro'ya yönelik hedefi olması gerekir. | 
| Finansal Risk Yönetimi & Sahtekarlık - Dynamics şirket içi yükleme tabanı - Navision (Business Central eğilimi modeli) | Şirket içi Navision'a sahip mevcut müşteri. İş ortağıNın Dynamics 365 Business Central'a yönelik hedefi olması gerekir. | 
| Finansal Risk Yönetimi & Sahtekarlık - Dynamics şirket içi yükleme tabanı - Dynamics AX (Dynamics 365 Finance + Operations propensity model) | Şirket içi AX'e sahip mevcut müşteri. İş ortağıNın Dynamics 365 Finance + Operations'i hedeflemesi gerekir. | 
| Finansal Risk Yönetimi & Sahtekarlık - Dynamics şirket içi yükleme tabanı - Great Plains (Business Central eğilimi modeli) | Şirket içi Great Plains'e sahip mevcut müşteri. İş ortağı Dynamics 365 Business Central için hedeflemelidir. | 
| Finans riskini yönetme & sahtekarlık-Dynamics şirket içi yüklemesi temel-Solomon (Business Central eğilimini model) | Şirket içi Solomon ile mevcut müşteri. İş ortağı Dynamics 365 Business Central için hedeflemelidir. | 
| Finans riskini yönetme & sahtekarlık-Dynamics şirket içi yüklemesi-diğerleri (Business Central eğilimini model) | Diğer şirket içi çözümlere sahip mevcut müşteri daha önce listelenmemiş. İş ortağı Dynamics 365 Business Central için hedeflemelidir. | 
| Çevik Iş süreçleri oluşturma-Dynamics şirket içi yüklemesi temel-AX/GP/SL/NAV/diğer (Dynamics 365 eğilimini model) | Çevik Iş süreçleri oluşturma-Dynamics şirket içi yüklemesi temel-AX/GP/SL/NAV/diğer (Dynamics 365 eğilimini model) | 
| Çevik Iş süreçleri oluşturma-Dynamics rekabet tabanı-mendix/OutSystems/Salesforce (Dynamics 365 eğilimini model) | Çevik iş süreçleri oluşturma-Dynamics rekabet tabanı-mendix/OutSystems/Salesforce (Dynamics 365 eğilimini model) | 
| Çevik Iş süreçleri oluşturma-Dynamics 365 finans + Operations Install Base | Mevcut Dynamics 365 finans + Operations müşterileri. Hedef güç uygulamalarına yönelik iş ortağı. | 
| Çevik Iş süreçleri oluşturma-Dynamics 365 Iş Merkezi yüklemesi temeli | Mevcut Dynamics 365 Iş merkezi müşterileri. Hedef güç uygulamalarına yönelik iş ortağı. | 
| Çevik Iş süreçleri oluşturma-Dynamics 365 müşteri katılımı yüklemesi temeli | Mevcut Dynamics 365 müşteri katılımı müşterileri. Hedef güç uygulamalarına yönelik iş ortağı. | 
| Oracle olmayan veya SAP ERP (kurumsal kaynak planlama) müşterileri ile bir Resilient Tedarik Zinciri - Windows oluşturma ve ilk Dynamics 365 iş yükünü Dynamics 365 Tedarik Zinciri Yönetimi olarak etkinleştirme | Dynamics 365 Tedarik Zinciri Yönetimi için hedef müşteriler | 
| Bir Resilient Tedarik Zinciri oluşturma - Dynamics 365 Tedarik Zinciri Yönetimi ve/veya Perakende veya Ticaret'i mevcut Dynamics 365 Customer Engagement müşterilerine çapraz satış | Dynamics 365 Tedarik Zinciri Yönetimi'nin çapraz satışlarını hedeflemek için mevcut Dynamics 365 Customer Engagement müşterileri. | 
| Bir Resilient Tedarik Zinciri Oluşturma - Dynamics 365 Tedarik Zinciri Yönetimi ve/veya Perakende veya Ticaret'i Dynamics 365 Customer Engagement ve Oracle veya SAP'ye çapraz satış | Dynamics 365 Tedarik Zinciri Yönetimini hedeflemek için Oracle veya SAP ile mevcut Dynamics 365 Müşteri Katılımı müşterileri | 
| D365BCCluster | Müşterinin Dynamics 365 Business Central satın alma eğilimini tanımlar. Business Central için bir teklifte bulunan müşteriler Orta ve Küçük kategorilerde yer atılır. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| D365BCFit | Sıkı grafiği tanımlayan iç ve dış veri noktaları. Uygun puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünlerine potansiyel olarak uygun olup olmadığını görmek için en iyi SMB'mize benzer bir model kullanır. Fit puanlama üç aylık olarak güncelleştirilir. | 
| D365BCIntent | Sosyal medya ve müşterinin çevrimiçi davranışıyla ilgili sinyaller Amacı tanımlar. Amaç puanlama, kümeleri tanımlamak için Sığdır'ın üzerine atlar. Amaç puanlama aylık olarak güncelleştirilir. | 
| D365FOCluster | Dynamics 365 finans ve Işlemlerini satın almak için müşterinin eğilimini tanımlar. Finans + Işlemlerine yönelik bir eğilimini gösteren müşteriler, en üstteki yönetilmeyen kategorilerde yer alacak. Hedef şimdi çalışır ve daha yüksek verim üretebilmeleri için kümeleri değerlendirir. Yalnızca Şimdi hareket ettikten ve müşterileri değerlendirdikten sonra hala kapasite varsa müşterileri Eğtir ve müşterileri eğitin. | 
| D365FOFit | Firmografları tanımlayan iç ve dış veri noktaları. Kullanım Puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünleri için olası bir uyum olup olmadığını görmek için en iyi SMB 'ye bir gevkalike modeli kullanır. Skor, üç aylık olarak güncelleştirilir. | 
| D365FOIntent | Sosyal medya ve müşterinin çevrimiçi davranışı ile ilgili sinyaller amaç tanımlar. Amaç Puanlama, kümeleri tanımlamak için uygun şekilde yer alır. Amaç Puanlama aylık olarak güncelleştirilir. | 
| D365CECluster | Dynamics 365 müşteri katılımı satın almak için müşterinin eğilimini tanımlar. Müşteri katılımı için bir eğilimini gösteren müşteriler orta ve küçük kategorilerde olacaktır. Hedef şimdi çalışır ve daha yüksek verim üretebilmeleri için kümeleri değerlendirir. Yalnızca Şimdi hareket ettikten ve müşterileri değerlendirdikten sonra hala kapasite varsa müşterileri Eğtir ve müşterileri eğitin. | 
| D365CEFit | Dynamics 365 müşteri katılımı için uygun olduğunu belirtir | 
| D365CEIntent | Dynamics 365 Customer Engagement amacını gösterir | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Müşterinin Dynamics şirket içi AX veya CRM için açık yenilemeye sahip olup olmadığını tanımlar | 
| M365UpsellCustomer | Müşterinin müşteriler için satış eğilimi gösterip Microsoft 365 | 
| Google'a sahip | Müşterinin Google ürünlerine sahip olmak için rekabet sinyalleri gösterip gösterip gösterir olmadığını tanımlar | 
| AWS'ye sahip | Müşterinin aws ürünlerine sahip olan müşteriler için rekabet sinyalleri gösterip gösterip gösterip gösterir | 
| EA'ya sahip | Yenilemenin EA aboneliği mi yoksa EA aboneliği mi olduğunu tanımlar | 
| Açık | Yenilemenin Açık veya Açık Değer sözleşmesi olup olmadığını tanımlar | 

### <a name="cloud-ascent---azure-propensity-report"></a>**Bulut Ascent - Azure eğilimi raporu**

| Sütun adı | Veri açıklaması | 
| :--------- | :--------- | 
| MPN Kimliği | Microsoft İş Ortağı Ağı kimliği | 
| İş Ortağı Adı | İş ortağının adı | 
| Müşteri Kimliği | Müşteri tanımlayıcı numarası | 
| DUNS Numarası | Dun & Bradstreet, eğilimini için puanlanmakta olan müşterinin numarası | 
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
| En çok yönetilmeyen-kullanıcı tabanı | En iyi unmanaged müşterileri – kullanıcılar | 
| IsNonProfit | Kuruluşun kar amacı gütmeyen kuruluş olup olmadığını gösterir (Evet veya Hayır) | 
| Geçiş - EOL Windows Server - Bulut Ascent eğilimine sahip EOL Windows Server IB - 5+ lisans | EOL şirket içi Windows Server'a (yani, bir EOL sürümü veya daha önceki) sahip olan müşteri. Müşterinin 5 veya daha fazla lisansı vardır. Teklif puanına sahip olan müşteri. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL Windows Server - Bulut Ascent eğilimine sahip EOL Windows Server IB - <5 lisans | EOL şirket içi Windows Server'a (yani, bir EOL sürümü veya daha önceki) sahip olan müşteri. Müşterinin 5'ten az lisansı vardır. Teklif puanına sahip olan müşteri. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL Windows Server - Bulut Ascent eğilimi olmadan EOL Windows Server IB - 5+ lisans | EOL şirket içi Windows Server'a (yani, bir EOL sürümü veya daha önceki) sahip olan müşteri. Müşterinin 5'in üzerinde lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - EOL Windows Server - Bulut Ascent eğilimi olmadan EOL Windows Server IB - <5 lisans | EOL şirket içi Windows Server'a (yani, bir EOL sürümü veya daha önceki) sahip olan müşteri. 5 ' ten az lisansa sahiptir. Müşterinin eğilimini puanı yok. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Cloud Ascent eğilimini-5 + lisanslarıyla geçiş-EOL SQL-EOL SQL Server ıB | Bir EOL şirket içi SQL Server (yani, bir EOL sürümü veya daha eski) olan müşteri. Müşterinin 5 ve lisansı vardır. Müşterinin bir eğilimini puanı vardır. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Cloud Ascent eğilimini-<5 lisanslarıyla geçiş-EOL SQL-EOL SQL Server ıB | Bir EOL şirket içi SQL Server (yani, bir EOL sürümü veya daha eski) olan müşteri. 5 ' ten az lisansa sahiptir. Eğilimini puanı olan müşteri. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Cloud Ascent eğilimini-5 + lisansı olmadan Migrate-EOL SQL-EOL SQL Server ıB | Bir EOL şirket içi SQL Server (yani, bir EOL sürümü veya daha eski) olan müşteri. Müşterinin 5 veya daha fazla lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Buluta geçiş-EOL SQL-EOL SQL Server ıB, bulut Yokent eğilimini-<5 Lisansı | Bir EOL şirket içi SQL Server (yani, bir EOL sürümü veya daha eski) olan müşteri. Müşterinin 5'ten az lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Şirket içi Windows Server'ı geçirme - Bulut Ascent eğilimi ile geçerli Windows Server IB - 5'den fazla lisans | Geçerli bir şirket içi Windows Server'a (yani EOL'den sonraki bir sürüm) sahip olan müşteri. Müşterinin 5'den fazla lisansı vardır. Müşterinin bir yayma puanı vardır. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Şirket içi Windows Server'ı geçirme - Bulut Ascent eğilimi ile geçerli Windows Server IB - <5 lisans | Geçerli bir şirket içi Windows Server'a (yani EOL'den sonraki bir sürüm) sahip olan müşteri. Müşterinin 5'ten az lisansı vardır. Müşterinin Azure için bir teklif puanı vardır. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Şirket içi Windows Server'ı geçirme - Bulut Ascent eğilimi olmadan geçerli Windows Server IB - 5'den fazla lisans | Geçerli bir şirket içi Windows Server'a (yani EOL'den sonraki bir sürüm) sahip olan müşteri. Müşterinin 5'den fazla lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçirme - Şirket içi Windows Server'ı geçirme - Bulut Ascent eğilimi olmadan geçerli Windows Server IB - <5 lisans | Geçerli bir şirket içi Windows Server'a (yani EOL'den sonraki bir sürüm) sahip olan müşteri. Müşterinin 5 ' ten az lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Geçiş-Azure SQL 'e veya SQL sanal makinelerine (VM) geçiş-Cloud Ascent eğilimini-5 + lisanslarıyla güncel SQL Server IB | Geçerli bir şirket içi SQL Server (yani, EOL 'tan sonraki bir sürüm) olan müşteri. Müşterinin 5 ve lisansı vardır. Müşterinin bir eğilimini puanı vardır. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Geçiş-Azure SQL veya SQL VM 'lerine geçiş-Cloud Ascent eğilimini-<5 lisanslarıyla geçerli SQL Server IB | Geçerli bir şirket içi SQL Server (yani, EOL 'tan sonraki bir sürüm) olan müşteri. Müşterinin 5 ' ten az lisansı vardır. Müşterinin bir eğilimini puanı vardır. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Geçiş-Azure SQL veya SQL VM 'lerine geçiş-bulut Yokent eğilimini-5 ve lisans olmadan geçerli SQL Server IB | Geçerli bir şirket içi SQL Server (yani, EOL 'tan sonraki bir sürüm) olan müşteri. Müşterinin 5 ve lisansı vardır. Müşterinin eğilimini puanı yok. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Geçiş-Azure SQL veya SQL VM 'lerine geçiş-bulut Yokent eğilimini-<5 lisansı olmadan geçerli SQL Server IB | Geçerli bir şirket içi SQL Server (yani, EOL 'tan sonraki bir sürüm) olan müşteri. Müşterinin 5'ten az lisansı vardır. Müşterinin bir yayma puanı yok. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - OSS - Açık Kaynak Kod (OSS) DB'ye Geçiş | Şu ürünlerden herhangi birini alan mevcut müşteri: PostgreSQL, MySQL, MariaDB. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - OSS - Azure'da Linux | Linux'a sahip mevcut müşteri. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçirme - SAP - Azure üzerinde SAP | SAP ile mevcut müşteri. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Windows Sanal Masaüstü - Uzak Masaüstü Hizmetleri IB | Etkin Windows hesabı olan Uzak Masaüstü Hizmetleri. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - Windows Sanal Masaüstü - Modern Çalışmaları Azure'a Çapraz Satış/WVD | Azure'Microsoft 365 sahip olmayan müşterileri tanımlar. İş ortağının Azure'a geçiş için bu müşteriyi hedeflemesi gerekir. | 
| Geçiş - VMware IB | Ürüne sahip mevcut müşteri: VMware. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Geçiş-Citrix ıB | Ürüne sahip mevcut müşteri: Citrix Systems. İş ortağı, bu müşteriyi Azure 'a geçirmek için hedeflemelidir. | 
| Yenilik yapın-Analytics-Power BI ıB with High Azure eğilimini | Power BI abonelik içeren ve etkin olan müşteriler: Power BI-tek başına Pro, Power BI-Azure paketleri, Power BI-Office paketleri, Power BI paketleri-Microsoft 365 | 
| GitHub ile etkinleştirme-DevOps-Visual Studio/MSDN ıB | Etkin Visual Studio sürümleriyle müşterileri tanımlar | 
| Windows Server Standard sürümü | Müşteri tarafından Windows Server Standart satın alımlarınızın sürümünü görüntüler | 
| Windows Server Standart lisansı | Müşteri tarafından Windows Server Standart satın alımlarınızın lisans türünü görüntüler | 
| Windows Server veri merkezi sürümü | Müşterinin Windows veri merkezi satın alımlarınızın sürümünü görüntüler | 
| Windows Server veri merkezi lisansı | Müşteri tarafından Windows veri merkezi satın alımlarınızın lisans türünü görüntüler | 
| AzureFit | Firmografları tanımlayan iç ve dış veri noktaları. Kullanım Puanlama, müşterileri karşılaştırmak ve Microsoft bulut ürünleri için olası bir uyum olup olmadığını görmek için en iyi SMB 'ye bir gevkalike modeli kullanır. Skor, üç aylık olarak güncelleştirilir. | 
| AzureIntent | Sosyal medya ve müşterinin çevrimiçi davranışıyla ilgili sinyaller Amacı tanımlar. Amaç puanlama, kümeleri tanımlamak için Sığdır'ın üzerine atlar. Amaç puanlama aylık olarak güncelleştirilir. | 
| AzureCluster | Fit ve Intent önerilerini bir kümede bir arada kullanarak müşterinin Azure satın alma eğilimini tanımlar. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| WindowsServerDataCenter_HasOpenRenewal | Müşterinin Windows Server Datacenter için açık yenilemesi olup olmadığını tanımlar | 
| WindowsServerStandard_HasOpenRenewal | Müşterinin Windows Server Standard için açık yenilemesi olup olmadığını tanımlar | 
| AzureUpsellCustomer | Müşterinin Azure için satış eğilimi gösterip gösterip gösterir olmadığını tanımlar | 
| Google'a sahip | Müşterinin Google ürünlerine sahip olmak için rekabet sinyalleri gösterip gösterip gösterir olmadığını tanımlar | 
| AWS'ye sahip | Müşterinin AWS ürünlerine sahip olan müşterilere yönelik rekabet sinyalleri gösterip gösterip gösterir | 
| EA'ya sahip | Yenilemenin EA aboneliği mi yoksa EA aboneliği mi olduğunu tanımlar | 
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
| Alt Kesim | Pazar alt | 
| SMC Tür Özeti | SMC türü | 
| En İyi Unmanaged - İşlem Tabanı | En çok kontrol dışı olan müşteriler – işlem | 
| En İyi Unmanaged - Kullanıcı Tabanı | En iyi unmanaged müşterileri – kullanıcılar | 
| IsNonProfit | Kuruluşun kar amacı gütmeyen kuruluş olup olmadığını gösterir (Evet veya Hayır) | 
| Google'a sahip | Müşterinin AWS ürünlerine sahip olan müşterilere yönelik rekabet sinyalleri gösterip gösterip gösterir | 
| AWS'ye sahip | Müşterinin AWS ürünlerine sahip olan müşterilere yönelik rekabet sinyalleri gösterip gösterip gösterir | 
| Azure Kümesi | Müşterinin Azure satın alma eğilimini tanımlar. Daha yüksek verim üretecekleri için Şimdi Harekete Geç ve Kümeleri Değerlendir'i hedefle. Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedefledikten sonra hala kapasite varsa Müşterileri Hedefleme ve Eğitme. | 
| D365 finans + Operations kümesi | Dynamics 365 finans ve Işlemlerini satın almak için müşterinin eğilimini tanımlar. Finans + Işlemlerine yönelik bir eğilimini gösteren müşteriler, en üstteki yönetilmeyen kategorilerde yer alacak. Hedef şimdi çalışır ve daha yüksek verim üretebilmeleri için kümeleri değerlendirir. Yalnızca Şimdi hareket ettikten ve müşterileri değerlendirdikten sonra hala kapasite varsa müşterileri Eğtir ve müşterileri eğitin. | 
| D365 CE kümesi | Dynamics 365 müşteri katılımı satın almak için müşterinin eğilimini tanımlar. Müşteri katılımı için bir eğilimini gösteren müşteriler orta ve küçük kategorilerde olacaktır. Hedef şimdi çalışır ve daha yüksek verim üretebilmeleri için kümeleri değerlendirir. Yalnızca Şimdi hareket ettikten ve müşterileri değerlendirdikten sonra hala kapasite varsa müşterileri Eğtir ve müşterileri eğitin. | 
| D365 BC kümesi | Dynamics 365 Business Central satın almak için müşterinin eğilimini tanımlar. Eğilimini for Business Central 'ı gösteren müşteriler orta ve küçük kategorilerde olacaktır. Hedef şimdi çalışır ve daha yüksek verim üretebilmeleri için kümeleri değerlendirir. Yalnızca Şimdi hareket ettikten ve müşterileri değerlendirdikten sonra hala kapasite varsa müşterileri Eğtir ve müşterileri eğitin. | 
| Microsoft 365 kümesi | Microsoft 365 satın almak için müşterinin eğilimini tanımlar. Hedef şimdi çalışır ve daha yüksek verim üretebilmeleri için kümeleri değerlendirir. Yalnızca Şimdi hareket ettikten ve müşterileri değerlendirdikten sonra hala kapasite varsa müşterileri Eğtir ve müşterileri eğitin. | 
| Lisans programı | Yenileme için lisans programı türünü tanımlar | 
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
