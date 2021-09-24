---
title: Eylül 2021 duyuruları
description: Microsoft İş Ortağı Merkezi, promosyonlar, teklifler, pazarlar veya mevcut tekliflerde yapılan değişiklikler dahil olmak üzere Eylül 2021 duyuruları.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-announcements
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 09/20/2021
ms.openlocfilehash: 51706ec685519ea297e851cb4f2b862b96db3da1
ms.sourcegitcommit: fceaca54b0ec695cf214209c09b4516e1b40866a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/24/2021
ms.locfileid: "128373430"
---
# <a name="september-2021-announcements"></a>Eylül 2021 duyuruları

Bu sayfada Eylül 2021 için Microsoft İş Ortağı Merkezi duyuruları ve vermektedir.

________________

## <a name="product-keys-available-for-business-central-for-dual-use-rights"></a><a name="13"></a> Business Central'da çift kullanım hakları için kullanılabilen ürün anahtarları

### <a name="categories"></a>Kategoriler

- Tarih: 2021-09-23
- Özellikler

### <a name="summary"></a>Özet

23 Eylül 2021'den başlayarak, Business Central'ın şirket içi sürümü için çift kullanım hakları için ürün anahtarları müşterilere Microsoft 365 yönetim merkezi.

### <a name="impacted-audience"></a>Etkilene hedef kitle

CSP iş ortakları

### <a name="details"></a>Ayrıntılar

23 Eylül 2021'den başlayarak, business Central'ın çift kullanım hakları avantajı için şirket içi sürümü için ürün anahtarları artık İş Ortağı Kaynağı İş Merkezi'nde (PSBC) kullanılamaz. Müşteriler, kuruluşlarının ürün anahtarlarına kendi kendine hizmet vermek için Microsoft 365 yönetim merkezi.

Sipariş sürecinde veya ülke kodu değişikliği gerçekleştirme sürecinde değişiklik yoktur.

### <a name="next-steps"></a>Sonraki adımlar

- Bu konu başlığıyla ilgili kaynakları gözden geçirme ve kuruluşta uygun proje katılımcıları ile paylaşma.  
- Kuruluş ve müşteri kuruluşlarının bu değişiklik hakkında bilgi sahibi olduğundan emin olmak.
- Ürün anahtarlarını indirme hakkında bilginiz yoksa Kalıcı yazılım ve ürün lisans anahtarlarını [indirme'ye bakabilirsiniz.](/microsoft-365/admin/setup/download-software-licenses-csp?view=o365-worldwide)
- [Dynamics 365 Business Central](https://partner.microsoft.com/resources/collection/dynamics-365-business-central-dual-use-rights-resources#/)İkili Kullanım Hakları Kaynakları koleksiyonunda güncelleştirilmiş Dynamics çift kullanım hakları lisansını karşılama işlemini gözden geçirme.

### <a name="questions"></a>Sorularınız mı var?

Bu teklifler hakkında sorularınız için ilgili topluluklar için Yammer kontrol edin.

________________

## <a name="reminder-introducing-api-throttling-to-partners-calling-partner-center-apis"></a><a name="12"></a>Anımsatıcı: Api'leri çağıran iş ortaklarına API İş Ortağı Merkezi tanıtımı

### <a name="summary"></a>Özet

Ekim 2021'den başlayarak Microsoft, API'leri çağıran iş ortaklarına API İş Ortağı Merkezi uygulayacak.

### <a name="categories"></a>Kategoriler

- Tarih: 2021-09-21
- Özellikler

### <a name="impacted-audience"></a>Etkilene hedef kitle

Bulut Çözümü Sağlayıcısı programı aracılığıyla işlem Bulut Çözümü Sağlayıcısı iş ortakları  

### <a name="details"></a>Ayrıntılar

Ekim 2021'den başlayarak Microsoft, api'leri çağıran iş ortakları için bir zaman aralığı içinde daha tutarlı bir performans için API İş Ortağı Merkezi uygulayacak.Kaynakların fazla kullanımına engel olmak için azaltma, bir hizmete yönelik istek sayısını bir zaman aralığı içinde sınırlar.Bir azaltma eşiği aşılırsa, İş Ortağı Merkezi istemciden gelen diğer tüm istekleri bir süre için sınırlar.
  
#### <a name="partner-benefits"></a>İş ortağı avantajları

Bu İş Ortağı Merkezi yüksek hacimli istekleri işleyecek şekilde tasarlansa da, çok fazla sayıda istek oluşursa kısıtlama tüm iş ortakları için en iyi performansı ve güvenilirliği korumaya yardımcı olur.

Avantajları şunlardır:

- Azaltma minimum kapalı kalma süresi sağlar.
- Yüksek hacimli istekleri azaltarak tüm iş ortakları için tutarlı bir performans elde edilebilir.  

#### <a name="apis-to-be-throttled"></a>Kısıtlan API'ler

| İşlem | İş Ortağı Merkezi belgeleri |
| ----------- | ---------------------- |
| v1/customers/{customer_id}/users/{user_id}/lisansları alın | [Bir kullanıcıya atanan lisansları alma](/partner-center/develop/check-which-licenses-are-assigned-to-a-user) |
| Get /v1/customers/{customer_id}/subscribedskus | [Kullanılabilir lisansların bir listesini alma](/partner-center/develop/get-a-list-of-available-licenses) |
| /v1/customers/{customer_id}/yetkilendirmeleri alın | [Yetkilendirme koleksiyonu alma](/partner-center/develop/get-a-collection-of-entitlements) |
| Get /v1/customers/{customer_id}/artifacts/{artifact_type}<br>/groups/{group_id}/lineItems/{lineitem_id}<br>/resource/{resource_id} | [Yetkilendirme koleksiyonu alma](/partner-center/develop/get-a-collection-of-entitlements#retrieve-reservation-details-from-an-entitlement-by-using-sdk-v19) |
| Get /v1/customers/{customer_id}/users/{use<br>r_id}/directoryroles | [Müşteri için kullanıcı rolleri alma](/partner-center/develop/get-user-roles-for-a-customer) |

Daha fazla verimlilik ve azaltmayı önlemek için etkinlik günlüğü API'sini kullanmayı göz önünde bulundurabilirsiniz. Bu özellik hakkında daha fazla bilgi için buradaki ayrıntılara [bakın.](/partner-center/develop/api-throttling-guidance)  

### <a name="next-steps"></a>Sonraki adımlar

Bu [konu için](/partner-center/develop/api-throttling-guidance) kaynakları gözden geçirin ve gerekli adımları uygulayın.

### <a name="change-log"></a>Değişiklik günlüğü

- 21 Eylül: Yaklaşan değişiklikler için anımsatıcı
- 19 Temmuz: Özgün Duyuru

________________

## <a name="coming-soon-delegated-administrative-privileges-monitoring-and-self-service-removal"></a><a name="11"></a> Çok yakında: Yönetici ayrıcalıkları için temsilci izleme ve self servis kaldırma

### <a name="categories"></a>Kategoriler

- Tarih: 2021-14-10
- Özellikler

### <a name="summary"></a>Özet

Microsoft, iş ortaklarının kullanılmayan DAP bağlantılarını kapatması için etkin temsilcili yönetim ayrıcalıkları (DAP) bağlantılarını görüntülemek için yeni raporlama araçları başlatıyor.

### <a name="impacted-audience"></a>Etkilene hedef kitle

Doğrudan fatura iş ortakları, dolaylı sağlayıcılar ve dolaylı kurumsal bayiler Bulut Çözümü Sağlayıcısı işlem

### <a name="details"></a>Ayrıntılar

İş ortakları, müşterilerinin hizmetlerini yönetmek ve desteklemek için temsilcili yönetim ayrıcalıklarını (DAP) kullanabilir.

Microsoft, iş ortağı ve müşteri ekosistemi içinde güvenliği artırmak için, kullanım dışıyken DAP'ı kapatmayı öneriyor.

Microsoft, Ekim 2018'in sonundan itibaren iş ortaklarının yönetim aracılarının müşterileriyle DAP bağlantılarını denetlemesini sağlamak için yeni raporlama araçlarını başlatacak. Bu raporlama, iş ortağı aracılarının DAP aracılığıyla tüm kiracılar genelinde müşteri kiracısına nasıl erişeceklerini yakalar. İş ortakları daha sonra kullanımda olmayan DAP bağlantılarını gözden geçirip kaldırabilir.

Bu yeni raporlama özelliği hakkında daha fazla [](https://partner.microsoft.com/resources/detail/dap-monitoring-and-self-serve-removal-pdf) bilgi edinmek için, raporda bulunan çeşitli filtreleri ve alanları belgeletan bir kılavuz oluşturduk.

#### <a name="key-considerations"></a>Dikkat edilmesi gereken temel konular

- Müşteri için DAP erişimini kapatmak, müşteri kiracısı özelliklerini yönetmek için iş ortağının yönetici ayrıcalığını kapatacak.  
- İş ortaklarının işlemden geçiş yapmak, müşterileri adına siparişler yapmaya devam eder.
- İş ortağı aracıları artık müşterileri için Microsoft'a destek bileti yükseltemeyecek.  
- DAP'ı kapatma, abonelikte geçerli rol tabanlı erişim denetimi rollerini etkilemez ve iş ortağı tarafından kazanılan kredileri etkilemez.

### <a name="next-steps"></a>Sonraki adımlar

Bu konu [başlığıyla](https://partner.microsoft.com/resources/collection/delegated-administrative-privileges-dap#/) ilgili kaynakları gözden geçirme ve kuruluşta uygun proje katılımcıları ile paylaşma.

## <a name="september-cloud-solution-provider-community-update-and-reminders"></a><a name="10"></a>Eylül Bulut Çözümü Sağlayıcısı topluluk güncelleştirmeleri ve anımsatıcılar

### <a name="categories"></a>Kategoriler

- Tarih: 2021-9-10
- Community | Yetenek -lerini

### <a name="summary"></a>Özet

Aylık [Bulut Çözümü Sağlayıcısı (CSP)](https://partner.microsoft.com/resources/detail/csp-monthly-update-september-2021-global) güncelleştirme bülteninin yanı sıra temel program güncelleştirmelerini sağlayan [ek CSP](https://partner.microsoft.com/resources/collection/september-2021-csp-partner-community-content#/) topluluk kaynakları da mevcuttur.

### <a name="impacted-audience"></a>Etkilene hedef kitle

CSP doğrudan fatura iş ortakları ve dolaylı sağlayıcılar

### <a name="details"></a>Ayrıntılar

Bu ayın kaynakları aşağıdaki konuları ele alıyor:

#### <a name="launches"></a>Başlattı

- [CSP'de yeni ticaret deneyiminde Microsoft Dynamics 365, Microsoft 365, Microsoft Power Platform ve Windows 365](https://partner.microsoft.com/resources/detail/d365-m365-power-platform-w365-in-the-new-commerce-experience-in-csp-pdf)

#### <a name="clinics"></a>Klinik

- [İş ortakları için lisans desteğine giriş](https://partner.microsoft.com/resources/detail/introduction-to-licensing-support-for-partners-pdf)
- [İş ortakları için Ürün Koşulları sitesine kılavuz](https://partner.microsoft.com/resources/detail/product-terms-site-guide-for-partners-pdf)
- [Destek dolandırıcılığını bildirme](https://partner.microsoft.com/resources/detail/how-to-report-a-support-scam-pdf)
- [Enterprise için Microsoft 365 Uygulamaları Program öznitelik değişikliği](https://partner.microsoft.com/resources/detail/program-attribute-change-for-microsoft-365-apps-for-enterprise-pdf)

#### <a name="csp-community-qa-reminder"></a>CSP Community Q&bir anımsatıcı

Aylık CSP topluluk Q&bir oturum, daha fazla bilgi edinmek ve programı etkileyen değişiklikler hakkında sorular sormak için size bir fırsat sağlar. Bu ayın çağrısı, önceki bölümde ve daha birçok konuda listelenen konulara odaklanacaktır.

[Çağrıya katmak için buraya kaydolun](https://globalpbocomm.eventbuilder.com/GlobalCSP).

#### <a name="always-availablelaunch-content-on-demand"></a>Her zaman kullanılabilir — içeriği isteğe bağlı olarak başlatın

Aylık [CSP topluluk koleksiyonu](https://partner.microsoft.com/resources/collection/september-2021-csp-partner-community-content#/)içinde şunları bulabilirsiniz:

- En son CSP bildirilerini, güncelleştirmeleri, olayları ve anımsatıcıları kolay okunabilir bir belgede toplayan, indirilebilir [CSP aylık güncelleştirme Bülteni](https://partner.microsoft.com/resources/detail/csp-monthly-update-september-2021-global) .
- Programın etkilediği yaklaşan değişikliklerin zaman çizelgesi görünümünü sağlayan [CSP duyurusu takvimi](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-september-2021-pdf) .
- Yaklaşan ürünün başlatıldığı ve tekliflerinin görüntüleneceği **Yeni** [ürün başlatma takvimi](https://partner.microsoft.com/resources/detail/product-launch-calendar-september-pdf) .
- İş ortakları ve müşteriler tarafından sunulan son ve yaklaşan promosyonları kapsayan [genel promosyon hazırlığı Kılavuzu](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/) .
- CSP, anahtar işletimsel değişiklikler üzerinde kullanımı kolay içerik ile [güncelleştirme kaynaklarını başlatın](https://partner.microsoft.com/resources/collection/csp-launch-topics-collection#/) .
- Önemli CSP ile ilgili [Yenileiciler ve anımsatıcıları](https://partner.microsoft.com/resources/detail/csp-september-2021-refreshers-and-reminders-pdf) , ilgi ve sorguları alma konuları.

Lisanslama hazırlığı mi gerekiyor? [Aylık CSP servisleri web seminerleri](https://commercial_licensing.eventbuilder.com/YearToDate_ALL) , tüm iş ortakları için kullanılabilen en son CSP lisanslama bilgilerini kapsar.

### <a name="next-steps"></a>Sonraki adımlar

Topluluk kaynaklarını gözden geçirin ve soru-cevap&bir topluluk çağrısı için kaydolun.

### <a name="questions"></a>Sorularınız mı var?

Aylık CSP topluluk Q&bir çağrı, CSP programındaki işletimsel değişiklik hakkında sorular getirmek için en iyi yerdir. Çağrıdan önce 48 saate kadar [bir soru gönderebilirsiniz](https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbRzrhg6eBq-tPjJzqc4xPoxdUQU1WQklGNDZBNVJaRkMxUDVJVUxHSkNXWS4u) . Başlatma ile ilgili tüm sorulara çağrı ve/veya çağrıdan sonra yayımlanan bir belge&. Son ayın [topluluk koleksiyonunu](https://partner.microsoft.com/resources/collection/august-2021-csp-partner-community-content#/) ziyaret edebilir ve Ağustos olayından sonra yayımlanan bir belgeyi soru&gözden geçirebilirsiniz.

Diğer CSP konuları hakkında sorularınız mı var? [Iş ortağı merkezi desteği sayfasını](https://partner.microsoft.com/support/?stage=1)ziyaret edin.

_____________

## <a name="september-co-sell-with-microsoft-qa-community-call-reminder"></a><a name="9"></a> Eylül ortak satışı Microsoft Q&topluluk çağrısı anımsatıcısı

### <a name="categories"></a>Kategoriler

- Tarih: 2021-09-09
- Community | Davetlere ve anımsatıcıları

### <a name="summary"></a>Özet

Eylül Community oturumu için [Şimdi kaydolun](https://globalpbocomm.eventbuilder.com/GlobalCoSell) . Bu, Iş Ortağı Merkezi 'nde ticari Market ve başvuru modülleriyle ilgili en son başlatma ve geliştirmeleri vurgular.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

Bu oturum, aşağıdakileri yöneten Iş ortağı merkezine özgü kullanıcı rollerine ayrılmıştır:

- Teklif yayımlama yönetimi için ticari Market modülü.
- Müşteri adayları ve ortak satış fırsatı paylaşım yönetimi için başvurular modülü.

Diğer tüm Iş Ortağı Merkezi kullanıcıları, [Işlem hazırlık kaynağı galerisinde](https://partner.microsoft.com/resources/cloud-solution-provider-program)isteğe bağlı olarak içeriğe erişebilir.

### <a name="details"></a>Ayrıntılar

Bu aya ilişkin önemli makaleler şunlardır:

#### <a name="commercial-marketplace"></a>Ticari market

- [Çözüm Bulucu artık AppSource ile tümleştirildi](https://appsource.microsoft.com/blogs/now-live-on-microsoft-appsource-tap-into-the-unrivaled-microsoft-partner-ecosystem-to-accelerate-your-digital-transformation)
- [ticari market 'te teklif yayımlamak için gereken kılavuzluk ve izinler (PowerPoint sunusunu indirir)](https://assetsprod.microsoft.com/mpn/guidance-and-permissions-needed-to-publish-an-offer-and-co-sell-with-ms.pptm)

#### <a name="referral"></a>Başvuruyu

- [Ticari Market teklifi için ortak satışı yapılandırma](/azure/marketplace/co-sell-configure)
- [Gelen fırsatları yönlendirme kuralları oluşturma ve yönetme: Iş Ortağı Merkezi](../routing-rules.md)
- [Ortak satış fırsatlarını yönetin: Iş Ortağı Merkezi](../manage-co-sell-opportunities.md#accepted-stage)
- [anlaşma kayıt verileri artık başvuru Analizler dışarı aktarma için kullanılabilir](./2021-july.md#17)

#### <a name="refresh"></a>Yenile

- [Iş Ortağı Merkezi 'nde ortak satış deneyimi](/azure/marketplace/co-sell-configure#enter-your-contacts)
- [Iş Ortağı Merkezi 'nde başvuru yönetimi](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx)
- [Iş ortağı merkezi toplu işlemler özelliğini kullanarak ortak satış anlaşmaları ölçeğini ölçeklendirerek paylaşma](./2021-february.md#13)
- [İş ortağı LED ortak satış anlaşmaları ile daha fazla esneklik](./2021-february.md#11)
- [iş ortağı merkezi 'nde başvuru Analizler al](../referral-insights.md)

### <a name="next-steps"></a>Sonraki adımlar

[Topluluk kaynaklarını](https://partner.microsoft.com/resources/collection/september-2021-co-sell-partner-community-content#/)gözden geçirin ve soru&topluluk çağrısı için kaydolun.

### <a name="questions"></a>Sorularınız mı var?

Soru&topluluk çağrısı, işletimsel değişiklikler hakkında sorular getirmek için en iyi yerdir. Çağrıdan önce 48 saate kadar [bir soru gönderebilirsiniz](https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbRzrhg6eBq-tPjJzqc4xPoxdUQU1WQklGNDZBNVJaRkMxUDVJVUxHSkNXWS4u) . Başlatma ile ilgili tüm sorulara çağrı ve/veya çağrıdan sonra yayımlanan bir belge&.  

Diğer konularda sorularınız varsa, [Iş ortağı merkezi desteği sayfasını](https://partner.microsoft.com/support/?stage=1)ziyaret edin.

_____________

## <a name="new-validation-rules-for-company-name-and-email-address-on-september-22"></a><a name="8"></a>22 Eylül tarihinde Şirket adı ve e-posta adresi için yeni doğrulama kuralları

### <a name="categories"></a>Kategoriler

- Tarih: 2021-09-07
- Hazır Olma

### <a name="summary"></a>Özet

İş ortakları ve müşterilerin işletmelerini temel alarak işlerini çalıştırmasına yardımcı olmak için bir müşterinin Şirket adı ve e-posta adresi için doğrulama kurallarını güncelleştiriyoruz. Bu, hem yeni hem de mevcut müşteri ayrıntıları için geçerlidir. Gerekli bir API değişikliği yok.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

CSP doğrudan fatura ortakları ve dolaylı sağlayıcılar

### <a name="details"></a>Ayrıntılar

Microsoft, güvende çalışır. Müşteri şirket adı ve e-posta adresi bilgilerini doğrulamaya yönelik uyumlu, güvenli ve güvenli bir yöntem sağlamayı taahhüt ediyoruz. 22 Eylül 2021 itibariyle e-posta ve şirket adı doğrulamaları güncelleştirilecektir. Daha fazla bilgi için bkz. [yeni müşteri kaydı ekleme](../add-a-new-customer.md).

#### <a name="new-rules-for-company-name-and-email-address"></a>Şirket adı ve e-posta adresi için yeni kurallar

Eylül 22 2021 itibariyle aşağıdaki yeni doğrulama kuralları uygulanacaktır.

Şirket adı girerken aşağıdakilere izin verilmez:

- Yalnızca bir karakter kullanılıyor.
- Yalnızca &$ ^ # (bkz. [tablo](../add-a-new-customer.md#table-of-special-characters)) gibi özel karakterler kullanma.
- Yalnızca boşluklar ve/veya sekmeler kullanılıyor.
- Her tek başına kısaltmaların, LLC, Inc, vb. gibi kısıtlanmış listeden kullanılması (bkz. [tablo](../add-a-new-customer.md#table-of-abbreviations)).
- ". Com", ". org", ". edu", ". sinek" vb. gibi Internet Top-Level etki alanı (TDL) uzantılarına sahip adlar kullanma (bkz. [tablo](../add-a-new-customer.md#table-of-top-level-domain-extensions)).
- Üç veya daha fazla kez, 999 gibi başka karakterler olmadan yinelenen karakteri kullanma.
- Boşluk ve/veya sekmeleri 1 2 3 gibi tek karakterlerle karışık olarak kullanma.

Müşteri e-posta adresi girerken aşağıdakilere izin verilmez:
- E-posta adresi içeremez @microsoft.com .
- Müşteri e-posta adresi, iş ortağıyla aynı etki alanı adını içeremez. Örneğin, ABC adlı bir iş ortağı ile bir müşteri e-postası oluşturamaz @abc.com .

EAP Web semineri sırasında daha fazla ayrıntı bulabilirsiniz:
- Anda [https://www.yammer.com/cloudpartnercommunity/#/files/1094484746240](https://www.yammer.com/cloudpartnercommunity/#/files/1094484746240)

- Yapılmıyor [https://www.yammer.com/cloudpartnercommunity/#/files/1094484361216](https://www.yammer.com/cloudpartnercommunity/#/files/1094484361216)
 
#### <a name="partner-and-customer-impact"></a>İş ortağı ve müşteri etkisi

İş ortakları, Eylül 22nd ' deki Yukarıdaki kurallara uymadığı takdirde müşterileri oluşturamazlar.

_____________

## <a name="readiness-dual-mode-attestation-and-additional-reseller-declaration"></a><a name="7"></a>Hazırlık: çift modlu kanıtlama ve ek satıcı bildirimi

### <a name="summary"></a>Özet

İş ortakları ve müşterilerin işlerini güvenle çalıştırmasına yardımcı olmak için iş ortaklarının, işlem başına aynı kiracı KIMLIĞINI kullanırken doğrudan veya dolaylı iş ortakları olarak davrandıklarından emin olmak istiyoruz.

Ayrıca, AB/EFTA ülkelerinde yer alan tüm iş ortaklarının tüm ek satıcıları (en fazla 5 ' e kadar) bildirmek için de istekte bulunuyoruz.

### <a name="categories"></a>Kategoriler

- Tarih: 2021-09-07
- Aralık ayında bir dünya çapında pilot başlatma hazırlığı

### <a name="impacted-audience"></a>Etkilene hedef kitle

Hem doğrudan hem de dolaylı iş ortakları olan CSP dolaylı sağlayıcıları

AB/EFTA ülkelerinin dolaylı iş ortakları

### <a name="details"></a>Ayrıntılar

Microsoft güven üzerinde çalışır. CSP programında müşteri aboneliklerini işlemeye yardımcı olmak için uyumlu, güvenli ve güvenli bir yöntem sağlamayı taahhüt etmek istiyoruz.

7 Eylül 2021'den itibaren, iş ortaklarının Yeni onay gereksinimlerine ve Sepet Oluşturma, Sepeti Güncelleştirme ve Sipariş Oluşturma API'leri içinde oluşan ek kurumsal bayi (yalnızca EU/EFTA) değişikliklerine karşı test etme fırsatına sahip olması için bir pilot proje açeceğiz. Bu değişikliklerin bu API'ler için mevcut deneyimleri bozacak olduğunu lütfen unutmayın. Bu nedenle, iş ortaklarının Aralık ayındaki tam lansmandan önce pilota katılma fırsatına sahip olduğu önemle tavsiye edilir.

#### <a name="partner-and-customer-impact"></a>İş Ortağı ve Müşteri Etkisi

- YENI DEĞIŞIKLIK: Dolaylı iş ortakları, doğrudan veya dolaylı iş ortakları olarak davranacaklarını onaylayana kadar satın almaları tamamlayabilecektir
- EU/EFTA iş ortakları, işlemle ilgili ek kurumsal bayileri bildire ve dahil temliklerine uymazsa AB yönetmelikleri ile uyumlu olmaz
- EAP web sayfası sırasında daha fazla ayrıntı bulunabilir: 
- Güverte: [https://www.yammer.com/cloudpartnercommunity/#/files/1094484746240](https://www.yammer.com/cloudpartnercommunity/#/files/1094484746240)
- Kayıt: [https://www.yammer.com/cloudpartnercommunity/#/files/1094484361216](https://www.yammer.com/cloudpartnercommunity/#/files/1094484361216)

Aşağıdaki API'ler etkilenecektir ve ayrıntılar paylaşılır ve buna göre güncelleştirilir:

- [Müşteri siparişi oluşturma - İş Ortağı Merkezi geliştirici](/partner-center/develop/create-an-order)
- [Sepet oluşturma - İş Ortağı Merkezi uygulama geliştiricisi](/partner-center/develop/create-a-cart)
- [Sepeti güncelleştirme - İş Ortağı Merkezi geliştiricisi](/partner-center/develop/update-a-cart)

Ek kurumsal bayiler, aşağıdaki AB/EFTA ülkeleri üzerinde işlem yapılan iş ortaklarını etkiler:

| AB / EFTA Ülkeleri | &nbsp; | &nbsp; |
| --- | --- | --- |
| Andorra<br>Avusturya<br>Belçika<br>Bouvet Adası<br>Bulgaristan<br>Hırvatistan<br>Kıbrıs<br>Çekya<br>Danimarka<br>Estonya<br>Faroe Adaları<br>Finlandiya<br>Fransa<br>Almanya<br>Cebelitarık | Yunanistan<br>Grönland<br>Guernsey<br>See (City'nin kapsa olduğu Yer)<br>Macaristan<br>İzlanda<br>İrlanda<br>Man Adası<br>İtalya<br>Jersey<br>Letonya<br>Liechtenstein<br>Litvanya<br>Lüksemburg<br>Malta | Monako<br>Hollanda<br>Norveç<br>Polonya<br>Portekiz<br>Romanya<br>San Marino<br>Slovakya<br>Slovenya<br>İspanya<br>Svalbard ve Jan Mayen<br>İsveç<br>İsviçre<br>Birleşik Krallık: TBD |
|

Pilota katılmak için lütfen konu uzmanınıza (AliSinki) ulaşarak iş ortağı kiracı kimliğini girin ve uçuşa eklensin.

_____________

## <a name="perpetual-software-and-software-subscriptions-price-lists-republished-to-fix-price-increases-in-russia"></a><a name="6"></a>Kalıcı yazılım ve yazılım abonelikleri fiyat listeleri, Rusya'daki fiyat artışlarını düzeltmek için yeniden yayımlandı

### <a name="categories"></a>Kategoriler

- Tarih: 2021-09-03
- Teklifler/Pazarlar

### <a name="summary"></a>Özet

1 Eylül 2021'de yayımlanan kalıcı yazılım ve yazılım abonelikleri fiyat listeleri, Rusya'da bir fiyatlandırma sorunu düzeltmek için 3 Eylül'de yeniden yayımlandı.

### <a name="impacted-audience"></a>Etkilene hedef kitle

Dolaylı sağlayıcılar ve doğrudan fatura iş ortakları, Rusya'daki Bulut Çözümü Sağlayıcısı kalıcı yazılım ve yazılım aboneliklerini işlemektedir.

### <a name="details"></a>Ayrıntılar

1 Eylül'de yayımlanan kalıcı yazılım ve yazılım abonelikleri fiyat listeleri, tüm ürünler için yanlış %15,2 fiyat artışına sahipti.

%15,2'ye yakın fiyat artışı Eylül'de **değil, 1 Ekim 2021'de** yürürlüğe girecektir. Fiyat listeleri doğru fiyatlandırma bilgileriyle yeniden yayımlanmamıştır.

1 Eylül ile 3 Eylül arasında ürün satın alan iş ortakları, en son fiyat listelerinde yansıtilen düzeltilmiş fiyatlar üzerinden ücret tahsil edilecektir.

### <a name="next-steps"></a>Sonraki adımlar

- Rusya'da kalıcı yazılım ve yazılım abonelikleri yapan iş ortaklarının düzeltilen fiyatları görmek için en son fiyat listesini indirmesi gerekir.
- Ekim ayında gelecek fiyat artışları hakkında ayrıntılı bilgi için Microsoft'un Rusya'daki ticari müşteriler için [lisanslama programını ayarlaması makalesine bakın.](https://news.microsoft.com/ru-ru/licensing-changes-at-microsoft-russia-2021/)

_____________

## <a name="corrections-to-september-license-based-services-price-list-and-october-preview-for-microsoft-365-business-basic-usd"></a><a name="5"></a>Eylül lisans tabanlı hizmetler fiyat listesinde ve Ekim önizlemesinde düzeltmeler Microsoft 365 İş Temel (USD)

### <a name="summary"></a>Özet

Eylül fiyat listesi ve Ekim önizlemesinde, ABD doları olarak fiyat için Microsoft 365 İş Temel liste fiyatı vardı.

### <a name="categories"></a>Kategoriler

- Tarih: 2021-09-02
- Teklifler/Pazarlar

### <a name="impacted-audience"></a>Etkilene hedef kitle

Dolaylı sağlayıcılar ve doğrudan fatura iş ortakları, lisans tabanlı hizmetleri Bulut Çözümü Sağlayıcısı program.

### <a name="details"></a>Ayrıntılar

1 Eylül 2021'de yayınlanan lisans tabanlı hizmetler için Eylül fiyat listesi ve Ekim önizlemesi, 1 Eylül 2021'de Microsoft 365 İş Temel. Düzeltilmiş fiyat listeleri 2 Eylül 2021'de yayımlandı. Bu yalnızca USD'i etkiler.

Etkilene teklif şunları içerir:

- Teklif Adı: Microsoft 365 İş Temel
- Teklif Kimliği: bd938f12-058f-4927-bba3-ae36b1d2501c
- Önceki: Liste Fiyatı = 2
- Sonra: Liste Fiyatı = 4

### <a name="next-steps"></a>Sonraki adımlar

ABD doları olarak lisanslı hizmetlere işlem yapan iş ortakları, düzeltilen fiyatı görmek için en son fiyat listesini indirmeli.

________________
## <a name="nigeria-and-thailand-are-now-microsoft-managed-countries"></a><a name="4-5"></a>Avrupa ve Afrika artık Microsoft tarafından yönetilen ülkelerdir

### <a name="categories"></a>Kategoriler

- Tarih: 2021-09-01
- Özellikler

### <a name="summary"></a>Özet

Artık Avrupa ve Afrika, Microsoft tarafından yönetilen ülkelerdir.

### <a name="impacted-audience"></a>Etkilene hedef kitle

İş ortakları, Afrika ve Afrika'da işlemde bulunmaktadır.

### <a name="details"></a>Ayrıntılar

Ticari [market yayımcıları için vergi ayrıntılarına bakın.](../tax-details-marketplace.md)

### <a name="questions"></a>Sorular

Bu teklifler hakkında daha fazla soru için lütfen ilgili toplulukları Yammer kontrol edin.

________________
## <a name="announcing-intune-per-device-for-enterprise-for-csp-partners"></a><a name="4"></a>CSP iş ortakları için cihaz başına Enterprise Intune'un açıklanma

### <a name="categories"></a>Kategoriler

- Tarih: 2021-09-02
- Özellikler

### <a name="summary"></a>Özet

1 Eylül'den itibaren yeni bir Cihaz başına Intune teklifi sunuyoruz.

### <a name="impacted-audience"></a>Etkilene hedef kitle

Bulut Çözümü Sağlayıcısı (CSP) programında işlem yapılan iş ortakları.

### <a name="details"></a>Ayrıntılar

Microsoft Intune, hem fiziksel hem de sanal uç noktaları yönetmek ve güvenliğini sağlamak için kullanılan en kapsamlı birleşik uç nokta yönetim platformudur. Enterprise kuruluşlarının kimliği doğrulanmış bir kullanıcıya atanmış cihazları yönetmeye (örneğin, birden çok kimliği doğrulanmış kullanıcı tarafından kullanılmadığı) yardımcı olmak için yeni bir Intune cihaz başına teklifi sunuyoruz.

1 Eylül 2021'de kullanılabilen bu teklif, cihaz başına Intune'dan faydalanırken cihaz Azure Active Directory (Azure AD) ekler. Tamamen işlevsel ve hazır bir deneyimdir ve aşağıdaki hizmet planlarını içerir:

- Exchange Foundation
- Microsoft Intune
- Azure Active Directory için eğitim.

Microsoft iş ortaklarımızdan gelen geri bildirimlere dayanarak, cihaz başına Enterprise için Intune, cihaz başına satışa (cihaz + Windows + Intune) cihazın ömrünü kapsayan beş yıllık bir teklif olarak dahil edilecek şekilde oluşturulmuştur. Bu yeni teklif CSP'lere anlaşma yapılarını basitleştirme ve müşterilerine daha rekabetçi bir anlaşma sunması için yardımcı olacaktır.

Yeni Cihaz başına Intune teklifiyle ilgili dikkat gerekenler:

- Bu bir SaaS Enterprise teklifidir ve Small & Medium Business (SMB) müşterileri için tasarlanmamaktadır.
- Yalnızca CSP'ler için kullanılabilir ve Toplu Lisanslama veya Web Direct'te kullanılamaz.
- Beş yıllık abonelik için maliyet 150 ABD dolarıdır (USD/ERP).
- Teklif Kimliği: 5170ccfb-e95b-49a4-b7f3-31f631a356ba
- Tek bir kimliği doğrulanmış kullanıcıya atanmış Windows cihazlar için hazır şekilde çalışır.
- Teklif, Cihaz Tabanlı Koşullu Erişim'i içermez.  

### <a name="questions"></a>Sorular

Bu teklifler hakkında daha fazla soru için lütfen ilgili toplulukları Yammer kontrol edin.

_____________

## <a name="key-updates-for-the-new-commerce-experience-for-cloud-solution-provider-csp-seat-based-offers"></a><a name="3"></a>Bulut Çözümü Sağlayıcısı (CSP) tabanlı tekliflere yeni ticaret deneyimi için önemli güncelleştirmeler

### <a name="summary"></a>Özet

19 Ağustos 2021'den itibaren açıklanmasıyla birlikte, Microsoft'un CSP seat tabanlı tekliflere ilişkin yeni ticaret deneyimine ilişkin önemli güncelleştirmeleri vardır.

### <a name="categories"></a>Kategoriler

- Tarih: 2021-09-01
- Özellikler

### <a name="impacted-audience"></a>Etkilene hedef kitle

CSP doğrudan fatura iş ortakları ve dolaylı sağlayıcıları ve dolaylı sağlayıcıları aracılığıyla kurumsal bayiler

### <a name="details"></a>Ayrıntılar

19 Ağustos 2021'de [Microsoft,](https://partner.microsoft.com/resources/detail/new-commerce-for-csp-seat-based-offers-pdf) Ekim 2021'de yapılacak olan yeni Microsoft 365, Dynamics 365, Power Platform ve Windows 365 kişilik yer tabanlı teklifler için ticari deneyimi duyurdu. Bu duyurunun bir sonraki adımları için, kuruma bu dönüşüme hazırlanmanıza yardımcı olmak için aşağıdaki önemli güncelleştirmeler vardır:

- Tümleşik korumalı alan testi için yer tabanlı tekliflerin lansmanları
- Eylül ayında gelecek CSP Q&çağrıları için anımsatıcı
- Microsoft Ticari Teşvik programı

#### <a name="launch-of-seat-based-offers-for-integrated-sandbox-testing"></a>Tümleşik korumalı alan testi için yer tabanlı tekliflerin başlatılması

Microsoft, 1 Eylül 2021'den itibaren CSP programı için [](https://partner.microsoft.com/resources/detail/new-commerce-for-csp-seat-based-offers-pdf) yeni ticari deneyimde tümleşik korumalı alan testi için yer tabanlı teklifleri etkinleştirdi. [](/partner-center/develop/test-and-debug)

CSP'Microsoft 365 Dynamics 365, Power Platform ve Windows 365 tekliflerinin yeni ticaret deneyimine ek olarak, yeni ticaret yolculuğumuza önemli bir kilometre taşı daha eksildi. Microsoft, iş ortaklarının CSP gelirlerini artırarak müşterilere daha fazla seçenek sağlamalarını sağlayan yeni iş fırsatlarına, ürün yeniliklerine, daha iyi araçlara ve erişime yatırımlar sunmaktadır. Ticari platformumuz gelişiyor ve iş ortaklarının ve müşterilerin dijital dönüşümde başarılı olması için sipariş ve abonelik yönetimi süreçlerimizi geliştiriyoruz.

Korumalı alan test ortamına katılan iş ortakları, bu teklifler için önceden planlama, operasyonelleştirme ve teknik tümleştirmeye olanak sağlayan, yer tabanlı teklifler için yeni ticari deneyime erkenden görünürlük sağlayacaktır.

Korumalı alan ortamına katılma, kuruma şunları sağlar:

- Üretim ortamına dağıtmadan önce test ortamında API tümleştirmesi gerçekleştirme
- Lansmandan önce yeni ticaret deneyimini faaliyete geçirmek için yeterli zaman elde edin

Tabloda tümleşik korumalı alan test ortamında bulunan temel özelliklerin bir özeti yer alır:

| İş ortağı/müşteri yönetici ayrıcalıkları için temsilci ayarlama | Kısmi alt yükseltme–tam özellik |
| ----------- | ---------------|
| 1 katmanlı, 2 katmanlı modeller | Destek aracılığıyla kısmi abonelik yükseltmesi |
| Geçerli ve yeni deneyimi yan yana bulma | Yenilemede zamanlanmış değişiklikler  |
| Modern'i keşfetme ve satın alma (ürünleri seçme) | Askıya alma/sürdürme (destek yoluyla) |
| Aboneliği yönetme (otomatik yenileme iki durumlu düğme, yer ekleme, hareket iptal etme) | Ücretsiz denemeler (yalnızca MAC sunum) |
| Bağımsız eklentiler  | İş ortağı para birimi |
| Faturalama planları | Fiyat saydamlığı  |
| Abonelik yaşam döngüsü yönetimi (yetkisiz kullanım süresi) | Birden çok yıllık teklifler için yıllık faturalama planları  |
| Sahiplik kısıtlamaları | Askıya alma/sürdürme (self servis aracılığıyla)  |
| Fatura/mutabakat dosyaları | Tam miktar SKU geçişleri için otomatik olarak yeniden yer ataması |
| Orta vadeli tam miktar SKU yükseltmeleri | Ücretsiz deneme (tam sunum ile) |
| İptal ilkesi zorlaması: 30 gün sonra 30 günlük iptali engelle (genel kullanılabilirlik süresi 72 saat olarak değişir) |  |
|

#### <a name="reminder-for-upcoming-csp-qa-calls-in-september"></a>Eylül ayında gelecek CSP Q&çağrıları için anımsatıcı

Microsoft 365, Dynamics 365, Power Platform ve Windows 365 için yeni ticaret deneyimi hakkında bilgi edinmek ve ekim 2021'de gelecek geniş harekete ilişkin 365 kişilik yer tabanlı teklifler hakkında bilgi edinmek ve sorular sormak için 15 Eylül ve 16 Eylül'de gelecek [CSP Q&A](https://globalpbocomm.eventbuilder.com/GlobalCSP) Community Çağrılarına kaydolun. CSP Community Soru&A çağrıları, CSP doğrudan fatura ve dolaylı iş ortaklarına CSP başlatmaları ve yaklaşan değişikliklerle ilgili sorular konusunda yardımcı olmak için ayrılmıştır. Size kolaylık olması için topluluk koleksiyonları iş [](https://partner.microsoft.com/resources/assets/#/?prog=CSP%7CCSP-Direct%7CCSP-Indirect-Partner&type=collection&search=community%20collection%202021&sort=updated) ortağı hazırlığı galerisinde daha önce sağlanır ve burada Soru-Cevap çağrısında ele alınacak malzemeleri&edinebilirsiniz.

CSP TemelLeri çağrılarına katılmak ve/veya geçmiş kayıtları bulmak için [CSP temelleri kaydına bakın.](https://globalpbocomm.eventbuilder.com/CSPFundamentals)

#### <a name="microsoft-commerce-incentive-program"></a>Microsoft Ticari Teşvik programı

1 Eylül 2021'de Microsoft, iş ortağı teşvik programının ekim ayında kullanılabilir olması evrimi kapsamındaki sonraki adımlarla ilgili iş ortaklarını bilgilendirdi. Bu iletişimin iki temel bileşeni, FY22 teşvikleri kılavuzları ve bu kılavuzda geliştirilen gelişmiş teşvikler deneyimi hakkında bilgi İş Ortağı Merkezi.

- **Geliştirilmiş iş ortağı deneyimi**  İş ortaklarının kullanılabilirliği için Ekim 2018'in başlarında microsoft, iş ortaklarının satın alma hareketlerinde ve müşteri yaşam döngüsünün aşamalarında teşvik kazanmaları için merkezi bir hedef olacak İş Ortağı Merkezi'daki tek bir katılım ve etkinlik platformuna yatırım yapmakta.

- **Teşviklere yeni yaklaşım**  Yeni teşvik ve yatırım teklifleri, yeni Microsoft Commerce Incentives eklenecektir. Microsoft, iş ortağı deneyimini basitleştirme çabası kapsamında teşvik programı kılavuzlarını şirket içinde barındırılan tek bir belgede İş Ortağı Merkezi.

### <a name="next-steps"></a>Sonraki adımlar

#### <a name="launch-of-seat-based-offers-for-integrated-sandbox-testing"></a>Tümleşik korumalı alan testi için yer tabanlı tekliflerin başlatılması

- Kuruluşunuz tümleşik bir korumalı alan ortamı sağladıysa hiçbir işlem yapmanız gerekmez. Kuruluşunuzda tümleşik bir korumalı alan ortamı yoksa, bir tane oluşturmak için aşağıdaki [adımları](/partner-center/develop/indirect-provider-sandbox-capabilities) izleyin.
- özellikler, iş kuralları ve yayın için adım adım yönergeler hakkında daha fazla bilgi edinmek için yeni ticaret deneyiminde Microsoft 365, Dynamics 365, güç platformu ve Windows 365 [CSP işletim kılavuzunu](https://partner.microsoft.com/resources/detail/operating-guide-new-commerce-experience-for-csp-seat-based-offers-pdf) gözden geçirin. Düzenli aralıklarla güncelleştirilecektir, işletim kılavuzunu düzenli olarak denetleyin.
- [Hazırlık eşlemesinde](https://partner.microsoft.com/resources/detail/readiness-map-new-commerce-experienceseat-based-offers-pdf)özetlenen kaynakları gözden geçirin.
- [API belgeleri klasörünü](https://partner.microsoft.com/resources/collection/api-documentation#/)gözden geçirin.
- destek için bir destek bileti günlüğe kaydedin veya [iş ortağı merkezi SDK 'sı ve apı Yammer grubundaki](https://www.yammer.com/cloudpartnercommunity/#/threads/inGroup?type=in_group&feedId=6589502)konuşmalara gönderi gönderin. bu özellik, eylül-kılavuzlarına özelliğinin sunumlarının ve kayıtlarının eylül ayında nakledileceği her yerde gönderilir.

#### <a name="reminder-for-upcoming-csp-qa-calls-in-september"></a>Önümüzdeki CSP Q&Eylül ayının anımsatıcıları

- yakında çıkacak [CSP Q&](https://globalpbocomm.eventbuilder.com/GlobalCSP) , 15 eylül veya 16 eylül 'ta Community çağrılar için kaydolun.
- Bu başlatma için CSP bilgisayar [tabanlı teklifler için](https://partner.microsoft.com/resources/collection/new-commerce-experience-for-csp-seat-based-offers#/) yeni ticaret deneyimini gözden geçirin.
- CSP Q&bir Community çağrısı yapın ve kuruluşunuzun yukarı Microsoft 365, Dynamics 365, güç platformu ve Windows 365 özellikli yeni ticari deneyimle ilgili olan soruları, yukarı doğru hareket için bt tabanlı olarak öğrenin.

#### <a name="microsoft-commerce-incentive-program"></a>Microsoft ticaret teşvik programı

- [Microsoft Commerce teşvikleri kaynak koleksiyonundaki](https://partner.microsoft.com/asset/collection/microsoft-commerce-incentive-resources#/)yakında geliştirilmiş iş ortağı deneyimindeki iletişimi gözden geçirin.
- [Ortak teşvikleri portalındaki](https://microsoft.sharepoint.com/teams/PartnerIncentivesPortal)güncelleştirilmiş FY22 iş ortağı teşvik kılavuzlarını gözden geçirin.

### <a name="questions"></a>Sorularınız mı var?

bu teklifler hakkında daha fazla soru için ilgili Yammer topluluklarınızı kontrol edin.

_____________

## <a name="view-this-months-product-launches-and-offers"></a><a name="2"></a>Bu aya ait ürünün başlatılan ve tekliflerini görüntüleyin

### <a name="summary"></a>Özet

Eylül 2021 ürün başlatma takvimi artık yayımlandı.

### <a name="categories"></a>Kategoriler

- Tarih: 2021-09-01
- Işletmenizi büyütün

### <a name="impacted-audience"></a>Etkilenen hedef kitle

tüm iş ortakları Bulut Çözümü Sağlayıcısı (CSP) programı üzerinden deneyimidir

### <a name="details"></a>Ayrıntılar

Eylül 2021 [ürün başlatma takvimi](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) artık işlem hazırlık kaynağı galerisinde kullanılabilir. Yakında çıkacak ürünü görüntüleyin ve burada teklif edin.

### <a name="next-steps"></a>Sonraki adımlar

[Ürün başlatma takvimini](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)gözden geçirin ve bilgileri kuruluşunuzdaki uygun hissedarlarla paylaşabilirsiniz.  

### <a name="questions"></a>Sorularınız mı var?

bu teklifler hakkında daha fazla soru için ilgili Yammer topluluklarınızı kontrol edin.

_____________

## <a name="software-in-microsoft-china-cloud-solution-provider-program-mccl-csp-to-start-transactions-from-august-12"></a><a name="1"></a>12 ağustos 'tan işlem başlatmak için Microsoft çin Bulut Çözümü Sağlayıcısı program (mccl CSP) içindeki yazılım

### <a name="summary"></a>Özet

Ağustos 3 güncelleştirmemize yönelik bir izleme olarak, MCCL CSP 'deki yazılım, 12 Ağustos 2021 ' den başlatılan işlemleri başlatacak.

### <a name="categories"></a>Kategoriler

- Tarih: 2021-09-01
- Işletmenizi büyütün

### <a name="impacted-audience"></a>Etkilenen hedef kitle

MCCL CSP program iş ortakları

### <a name="details"></a>Ayrıntılar

#### <a name="mccl-csp-transaction-start"></a>MCCL CSP işlem başlangıcı

- 12 Ağustos 2021 ' de, MCCL CSP, Çin müşterileri için işlemler başlatacak.

- Müşteriler, 31 Aralık 2021 ' ye kadar açık lisans programındaki bir iş ortağı yardımıyla yazılım lisansları satın almaya devam edebilir. Kalıcı lisanslar, açık lisans programının kullanım dışı bırakılıncaya kadar hem MCCL CSP 'de hem de açık lisans programlarında kullanılabilir.

#### <a name="open-license-program-deprecation"></a>Lisans programını kullanımdan kaldırmayı aç

- Müşteriler, 1 Ocak 2022 ' den itibaren Microsoft açık lisans programı aracılığıyla yazılım lisanslarını satın alıp yenileyemez.

- Müşteriler, kullanımdan kalkdıktan sonra bile açık lisans programı aracılığıyla elde edilen tüm kalıcı yazılım lisanslarını tam haklara ve erişime sahip olmaya devam edebilir. Ayrıca, bu lisansları ve hizmetleri yönetmek için toplu lisanslama hizmet merkezine de erişebilirler.

#### <a name="software-assurance-sa-purchases"></a>Yazılım Güvencesi (SA) satın alma

- Açık lisansa sahip (L&SA) SA teklifleri açık değerde (OV) ve açık değer aboneliğinde (OVS) kullanılabilir olmaya devam edecektir. Ancak, bunu MCCL CSP 'de sunmak için bir plan olmadığından, MCL CSP programında ne SA ne de L&SA bulunmaz.

- Süre sonu 1 Ocak 2022 ' den sonra olsa da sa 'nın avantajları SA dönemi sona erene kadar devam edecektir.

- Microsoft OV programı, SA 'yı içeren gelecekte satın alma işlemleri için önerilir.

>[!NOTE]
>OV ve OVS programlarını değiştirme planı yoktur.

#### <a name="partner-change-management"></a>İş ortağı değişiklik yönetimi

- Mevcut Microsoft açık dağıtıcılarının eklendi as MCCL CSP dolaylı sağlayıcıları vardır.

- Dolaylı sağlayıcılar ve seçilen dolaylı satıcılar, işlem işlevini sağlamak için Ağustos ayında üretim ortamı testi yürütmek üzere davet edilir.

- Temmuz ayında kullanıma hazır olan dolaylı iş ortakları için hazırlık atölyeler ve Aralık 2021 ' a kadar devam edecektir.

### <a name="next-steps"></a>Sonraki adımlar

Aşağıdaki kaynaklar aracılığıyla bu değişikliğe hazırlanın:

- [Yeni ticaret nedir?](https://partner.microsoft.com/resources/detail/new-commerce-experience-introduction)
- [MCCL CSP dolaylı sağlayıcı PlayBook](https://microsoftapc.sharepoint.com/:b:/t/ChinaLicensingHome/EeWi5axiZ_RCkTbxa-brE-sBGYdLJ5idpnZvFt2MFiTLWw?e=6itfqY)
- [MCCL CSP dolaylı Bayi PlayBook](https://microsoftapc.sharepoint.com/:b:/t/ChinaLicensingHome/EY-csVS7lFdKpwkRqeJJ4hkBPGWv4qkfINictqVrwKVLxQ?e=9G6ZY1)

Bu değişikliklerin yalnızca MCCL CSP için uygulandığını ve 21 Vianet CSP üzerinde hiçbir etkisi olmadığını unutmayın.

### <a name="questions"></a>Sorularınız mı var?

Başka sorularınız varsa, yerel iş ortağı geliştirme yöneticinize konuşabilirsiniz.
