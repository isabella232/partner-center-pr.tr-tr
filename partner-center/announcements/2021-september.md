---
title: Eylül 2021 duyuruları
description: Yeni yetenekler, promosyonlar, teklifler, pazarlar veya mevcut tekliflerle ilgili değişiklikler dahil olmak üzere Microsoft Iş Ortağı Merkezi için Eylül 2021 duyuruları.
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
ms.lasthandoff: 09/23/2021
ms.locfileid: "128322464"
---
# <a name="september-2021-announcements"></a>Eylül 2021 duyuruları

Bu sayfada, Eylül 2021 için Microsoft Iş Ortağı Merkezi duyuruları sağlanmaktadır.

________________

## <a name="product-keys-available-for-business-central-for-dual-use-rights"></a><a name="13"></a> Ürün anahtarları, Çift kullanım hakları için Iş Merkezi 'nde kullanılabilir

### <a name="categories"></a>Kategoriler

- Tarih: 2021-09-23
- Özellikler

### <a name="summary"></a>Özet

23 eylül 2021 ' ten itibaren, çift kullanım hakları için iş merkezi 'nin şirket içi sürümü için ürün anahtarları Microsoft 365 yönetim merkezi aracılığıyla müşteriler tarafından kullanılabilir.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

CSP iş ortakları

### <a name="details"></a>Ayrıntılar

23 Eylül 2021 ' ten itibaren, Çift kullanım hakları için Iş Merkezi 'nin şirket içi sürümüne yönelik ürün anahtarları artık iş ortağı kaynağı Iş merkezinde (PSBC) kullanılamaz. müşteriler, Microsoft 365 yönetim merkezi aracılığıyla kuruluşun ürün anahtarlarını self servis sunabilir.

Sıralama işleminde veya ülke kodu değişikliği karşılama işleminde değişiklik yapılmaz.

### <a name="next-steps"></a>Sonraki adımlar

- Bu konuyla ilgili kaynakları gözden geçirin ve kuruluşunuzdaki uygun hissedarlarla paylaşabilirsiniz.  
- Kuruluşunuzun ve müşteri kurumlarınızın bu değişikliği öğrendiğinden emin olun.
- Ürün anahtarlarının nasıl indirileceği hakkında bilgi sahibi değilseniz, [kalıcı yazılım ve ürün lisans anahtarlarını indirin](/microsoft-365/admin/setup/download-software-licenses-csp?view=o365-worldwide)' ı gözden geçirin.
- [Dynamics 365 Iş Merkezi çift kullanım hakları kaynakları koleksiyonundaki](https://partner.microsoft.com/resources/collection/dynamics-365-business-central-dual-use-rights-resources#/)güncelleştirilmiş Dynamics ikili kullanım hakları Lisans işlemini gözden geçirin.

### <a name="questions"></a>Sorularınız mı var?

bu tekliflerle ilgili herhangi bir soru için ilgili Yammer topluluklarınızı kontrol edin.

________________

## <a name="reminder-introducing-api-throttling-to-partners-calling-partner-center-apis"></a><a name="12"></a>Anımsatıcı: Iş Ortağı Merkezi API 'Lerini çağıran iş ortaklarına API azaltma ile tanışın

### <a name="summary"></a>Özet

Microsoft, 2021 Ekim 'den başlayarak Iş Ortağı Merkezi API 'Lerini çağıran iş ortaklarına API daraltma uygular.

### <a name="categories"></a>Kategoriler

- Tarih: 2021-09-21
- Özellikler

### <a name="impacted-audience"></a>Etkilenen hedef kitle

Bulut Çözümü Sağlayıcısı programı aracılığıyla iş ortakları deneyimidir  

### <a name="details"></a>Ayrıntılar

Microsoft, 2021 Ekim 'den itibaren Iş Ortağı Merkezi API 'Lerini çağıran iş ortakları için zaman dilimi içinde daha tutarlı bir performans için API daraltma uygulamayı uygulamaya yöneliktir.Kaynakların aşırı kullanımını engellemek için, azaltma, bir zaman aralığında bir hizmete yönelik istek sayısını sınırlar.Bir azaltma eşiği aşıldığında, Iş ortağı merkezi bir süre için o istemciden gelen diğer istekleri sınırlandırır.
  
#### <a name="partner-benefits"></a>İş ortağı avantajları

Iş Ortağı Merkezi, yüksek hacimli istekleri işleyecek şekilde tasarlandığından, çok sayıda istek oluşursa, azaltma işlemi tüm iş ortakları için en iyi performansı ve güvenilirliği korumanıza yardımcı olur.

Avantajları şunlardır:

- Azaltma, en az kapalı kalma süresini sağlar.
- Yüksek hacimli istekleri azaltarak tüm iş ortakları için tutarlı bir performans sağlayabilirsiniz.  

#### <a name="apis-to-be-throttled"></a>Kısıtlanacak API 'Ler

| İşlem | İş Ortağı Merkezi belgeleri |
| ----------- | ---------------------- |
| V1/Customers/{customer_id}/Users/{user_id}/lisansları alın | [Bir kullanıcıya atanan lisansları alma](/partner-center/develop/check-which-licenses-are-assigned-to-a-user) |
| /V1/Customers/{customer_id}/subscribedskus al | [Kullanılabilir lisansların bir listesini alma](/partner-center/develop/get-a-list-of-available-licenses) |
| /V1/Customers/{customer_id}/yetkilendirmelerini al | [Yetkilendirme koleksiyonu alma](/partner-center/develop/get-a-collection-of-entitlements) |
| /V1/Customers/{customer_id}/Artifacts/{artifact_type} al<br>/Groups/{group_id}/LineItem/{lineitem_id}<br>/Resource/{resource_id} | [Yetkilendirme koleksiyonu alma](/partner-center/develop/get-a-collection-of-entitlements#retrieve-reservation-details-from-an-entitlement-by-using-sdk-v19) |
| /V1/Customers/{customer_id}/Users/{use komutunu alın<br>r_id}/directoryroles | [Müşteri için kullanıcı rolleri alma](/partner-center/develop/get-user-roles-for-a-customer) |

Daha verimlilik sağlamak ve azaltmayı önlemek için etkinlik günlüğü API 'sini kullanmayı düşünmenizi öneririz. Bu özellik hakkında daha fazla bilgi için [buradaki](/partner-center/develop/api-throttling-guidance)ayrıntılara bakın.  

### <a name="next-steps"></a>Sonraki adımlar

Bu konunun [kaynaklarını](/partner-center/develop/api-throttling-guidance) gözden geçirin ve gerekli adımları uygulayın.

### <a name="change-log"></a>Değişiklik günlüğü

- 21 Eylül: yaklaşan değişiklikler için anımsatıcı
- 19 Temmuz: özgün duyuru

________________

## <a name="coming-soon-delegated-administrative-privileges-monitoring-and-self-service-removal"></a><a name="11"></a> Yakında: yönetici ayrıcalıkları izleme ve self servis kaldırma temsilcisi

### <a name="categories"></a>Kategoriler

- Tarih: 2021-14-10
- Özellikler

### <a name="summary"></a>Özet

Microsoft, etkin temsil edilen yönetim ayrıcalıkları (DAP) bağlantılarını görüntüleyen ve iş ortaklarının kullanılmayan DAP bağlantılarını kapamaları için yeni raporlama araçları başlatıyor.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

Bulut Çözümü Sağlayıcısı programı aracılığıyla doğrudan fatura ortakları, dolaylı sağlayıcılar ve dolaylı satıcılar deneyimidir

### <a name="details"></a>Ayrıntılar

İş ortakları, müşterilerinin hizmetlerini yönetmek ve desteklemek için yetkilendirilmiş yönetim ayrıcalıkları (DAP) kullanabilir.

İş ortağı ve müşteri ekosistemi içindeki güvenliği artırmak için, Microsoft, kullanımda olmadığında DAP 'i kapatmayı öneriyor.

En geç Ekim 'den itibaren, Microsoft yeni raporlama araçları 'nı başlatarak iş ortaklarının yönetim aracılarının müşterileri ile DAP bağlantılarını denetleyebilir. Bu raporlama, iş ortağı aracılarının tüm kiracılar genelinde müşteri kiracılarına DAP aracılığıyla nasıl eriştiğini yakalar. İş ortakları daha sonra kullanımda olmayan DAP bağlantılarını gözden geçirebilir ve kaldırabilir.

Bu yeni raporlama özelliği hakkında daha fazla bilgi edinmek için, raporda bulunan çeşitli filtre ve alanları belgeleyen bir [kılavuz](https://partner.microsoft.com/resources/detail/dap-monitoring-and-self-serve-removal-pdf) oluşturduk.

#### <a name="key-considerations"></a>Dikkat edilmesi gereken temel konular

- Bir müşteri için DAP erişiminin kapatılması, müşterinin kiracısındaki özellikleri yönetmek üzere ortağın yönetici ayrıcalığını devre dışı bırakır.  
- Deneyimidir iş ortakları, müşteri adına sipariş yerleştirmeyi devam edebilir.
- İş ortağı aracıları artık müşterileri için Microsoft 'a destek bileti oluşturmaz.  
- DAP 'in kapatılması, bir abonelikte geçerli rol tabanlı erişim denetimi rollerini etkilemez ve iş ortağının kazanılma kredilerini etkilemez.

### <a name="next-steps"></a>Sonraki adımlar

Bu konuyla ilgili [kaynakları](https://partner.microsoft.com/resources/collection/delegated-administrative-privileges-dap#/) gözden geçirin ve kuruluşunuzdaki uygun hissedarlarla paylaşabilirsiniz.

## <a name="september-cloud-solution-provider-community-update-and-reminders"></a><a name="10"></a>eylül Bulut Çözümü Sağlayıcısı topluluk güncelleştirmesi ve anımsatıcıları

### <a name="categories"></a>Kategoriler

- Tarih: 2021-9-10
- Community | Yetenek

### <a name="summary"></a>Özet

[Bulut Çözümü Sağlayıcısı (CSP) aylık güncelleştirme bülteni](https://partner.microsoft.com/resources/detail/csp-monthly-update-september-2021-global) artık size temel program güncelleştirmeleri sağlayan ek [CSP topluluk kaynaklarıyla](https://partner.microsoft.com/resources/collection/september-2021-csp-partner-community-content#/) birlikte kullanılabilir.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

CSP doğrudan fatura ortakları ve dolaylı sağlayıcılar

### <a name="details"></a>Ayrıntılar

Bu ayın kaynakları aşağıdaki konuları kapsar:

#### <a name="launches"></a>Yapılandırma

- [CSP 'de yeni ticaret deneyiminde microsoft Dynamics 365, Microsoft 365, microsoft Power Platform ve Windows 365](https://partner.microsoft.com/resources/detail/d365-m365-power-platform-w365-in-the-new-commerce-experience-in-csp-pdf)

#### <a name="clinics"></a>Klinikler

- [İş ortakları için lisans desteğine giriş](https://partner.microsoft.com/resources/detail/introduction-to-licensing-support-for-partners-pdf)
- [İş ortakları için ürün koşulları sitesi Kılavuzu](https://partner.microsoft.com/resources/detail/product-terms-site-guide-for-partners-pdf)
- [Destek raporunu bildirme](https://partner.microsoft.com/resources/detail/how-to-report-a-support-scam-pdf)
- [Enterprise için Microsoft 365 Uygulamaları özniteliği değişikliği](https://partner.microsoft.com/resources/detail/program-attribute-change-for-microsoft-365-apps-for-enterprise-pdf)

#### <a name="csp-community-qa-reminder"></a>CSP Community Q&anımsatıcı

Aylık CSP topluluğu&Oturum, daha fazla bilgi edinmek ve programı etkileyen değişiklikler hakkında sorular sormak için size bir fırsat sağlar. Bu ayın çağrısı önceki bölümde listelenen konulara ve daha birçok konuya odaklanacak.

[çağrısına katılmak için buraya kaydolmanız gerekir.](https://globalpbocomm.eventbuilder.com/GlobalCSP)

#### <a name="always-availablelaunch-content-on-demand"></a>Her zaman kullanılabilir—İçeriği isteğe bağlı olarak başlatma

Aylık [CSP topluluk koleksiyonu içinde](https://partner.microsoft.com/resources/collection/september-2021-csp-partner-community-content#/)şunları bulabilirsiniz:

- Son [CSP duyurularını,](https://partner.microsoft.com/resources/detail/csp-monthly-update-september-2021-global) güncelleştirmelerini, olaylarını ve anımsatıcıları kolay okunur bir belgede toplanmış indirilebilir CSP Aylık Güncelleştirme bülteni.
- Programı etkileyen yaklaşan değişikliklerin zaman çizelgesi görünümünü sağlayan [CSP](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-september-2021-pdf) Duyuru Takvimi.
- Yaklaşan **ürün** [lansmanlarını](https://partner.microsoft.com/resources/detail/product-launch-calendar-september-pdf) ve tekliflerini görüntüyebilirsiniz yeni ürün lansman takvimi.
- İş [ortakları ve müşteriler için kullanılabilir](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/) olan son ve yaklaşan promosyonları harmanlar Küresel Promosyon Hazırlığı Kılavuzu.
- [CSP, önemli işlem değişikliklerinde](https://partner.microsoft.com/resources/collection/csp-launch-topics-collection#/) kullanımı kolay içerikle güncelleştirme kaynaklarını başlatacak.
- [İlgi ve sorgu alan önemli](https://partner.microsoft.com/resources/detail/csp-september-2021-refreshers-and-reminders-pdf) CSP konularına ilişkin yenilemeler ve anımsatıcılar.

Lisans hazırlığı mı gerekiyor? Aylık [CSP spotlight web seminerleri,](https://commercial_licensing.eventbuilder.com/YearToDate_ALL) tüm iş ortakları için kullanılabilen en son CSP lisans bilgilerini içerir.

### <a name="next-steps"></a>Sonraki adımlar

Topluluk kaynaklarını gözden geçirme ve Soru-Cevap topluluk&kaydolma.

### <a name="questions"></a>Sorularınız mı var?

Aylık CSP topluluğu Q&A çağrısı, CSP programında operasyonel değişiklikle ilgili sorular getirmek için en iyi yerdir. Aramadan [48](https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbRzrhg6eBq-tPjJzqc4xPoxdUQU1WQklGNDZBNVJaRkMxUDVJVUxHSkNXWS4u) saat önceye kadar bir soru gönderesiniz. Başlatmayla ilgili tüm sorular çağrısında ve/veya çağrıdan sonra yayımlanan&A belgesinde yanıtlanır. Geçen ayın topluluk koleksiyonunu ziyaret [edecek ve](https://partner.microsoft.com/resources/collection/august-2021-csp-partner-community-content#/) Ağustos&yayımlanan Q&belgesini gözden geçirebilirsiniz.

Başka bir CSP konusuyla ilgili sorularınız mı var? İş Ortağı Merkezi [sayfasını ziyaret edin.](https://partner.microsoft.com/support/?stage=1)

_____________

## <a name="september-co-sell-with-microsoft-qa-community-call-reminder"></a><a name="9"></a> Microsoft Q ve A topluluk&anımsatıcı ile Eylül ayında ortak satış

### <a name="categories"></a>Kategoriler

- Tarih: 2021-09-09
- Community | Davetler ve anımsatıcılar

### <a name="summary"></a>Özet

[Ticari markette](https://globalpbocomm.eventbuilder.com/GlobalCoSell) yapılan en son lansmanları ve geliştirmeleri ve bu modüllerde referans modüllerini vurgulayan Eylül topluluk oturumuna İş Ortağı Merkezi.

### <a name="impacted-audience"></a>Etkilene hedef kitle

Bu oturum, aşağıdaki İş Ortağı Merkezi belirli kullanıcı rollerine ayrılmıştır:

- Teklif yayımlama yönetimi için ticari market modülü.
- Müşteri adayları ve ortak satış fırsat paylaşımı yönetimi için referanslar modülü.

Diğer tüm İş Ortağı Merkezi kullanıcılar, İşlem hazırlığı kaynak galerisinde isteğe [bağlı olarak içeriğe erişebilirsiniz.](https://partner.microsoft.com/resources/cloud-solution-provider-program)

### <a name="details"></a>Ayrıntılar

Bu ayın önemli makaleleri şunlardır:

#### <a name="commercial-marketplace"></a>Ticari market

- [Çözüm bulici artık AppSource ile tümleştirildi](https://appsource.microsoft.com/blogs/now-live-on-microsoft-appsource-tap-into-the-unrivaled-microsoft-partner-ecosystem-to-accelerate-your-digital-transformation)
- [Ticari markette teklif yayımlamak için gereken rehberlik ve izinler (PowerPoint indirmeleri)](https://assetsprod.microsoft.com/mpn/guidance-and-permissions-needed-to-publish-an-offer-and-co-sell-with-ms.pptm)

#### <a name="referral"></a>Tavsiye

- [Ticari market teklifi için ortak satış yapılandırma](/azure/marketplace/co-sell-configure)
- [Gelen fırsatları yönlendirme kurallarını oluşturma ve yönetme: İş Ortağı Merkezi](../routing-rules.md)
- [Ortak satış fırsatlarını yönetme: İş Ortağı Merkezi](../manage-co-sell-opportunities.md#accepted-stage)
- [Satış anlaşması kayıt verileri artık Referans Veri Kaynağı'Analizler](./2021-july.md#17)

#### <a name="refresh"></a>Yenile

- [İş Ortağı Merkezi'da ortak satış deneyimi](/azure/marketplace/co-sell-configure#enter-your-contacts)
- [İş Ortağı Merkezi'de referans yönetimi](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx)
- [Toplu işlem özelliğini kullanarak ortak satış anlaşmalarını İş Ortağı Merkezi paylaşın](./2021-february.md#13)
- [İş ortağı tarafından ortak satış anlaşmaları ile daha fazla esneklik](./2021-february.md#11)
- [İş Ortağı Merkezi'Analizler Referans İş Ortağı Merkezi](../referral-insights.md)

### <a name="next-steps"></a>Sonraki adımlar

Topluluk kaynaklarını [gözden geçirme](https://partner.microsoft.com/resources/collection/september-2021-co-sell-partner-community-content#/)ve Soru-Cevap topluluk&kaydolma.

### <a name="questions"></a>Sorularınız mı var?

Soru-&topluluk çağrısı, operasyonel değişikliklerle ilgili sorular getirmek için en iyi yerdir. Çağrıdan [48](https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbRzrhg6eBq-tPjJzqc4xPoxdUQU1WQklGNDZBNVJaRkMxUDVJVUxHSkNXWS4u) saat önceye kadar bir soru gönderesiniz. Başlatmayla ilgili tüm sorular çağrısında ve/veya çağrıdan sonra yayımlanan&A belgesinde yanıtlanır.  

Diğer konularla ilgili sorularınız varsa destek [sayfasından İş Ortağı Merkezi ziyaret edin.](https://partner.microsoft.com/support/?stage=1)

_____________

## <a name="new-validation-rules-for-company-name-and-email-address-on-september-22"></a><a name="8"></a>22 Eylül'de şirket adı ve e-posta adresi için yeni doğrulama kuralları

### <a name="categories"></a>Kategoriler

- Tarih: 2021-09-07
- Hazır Olma

### <a name="summary"></a>Özet

İş ortaklarının ve müşterilerin işletmelerini güvene göre çalıştırmalarına yardımcı olmak için müşterinin şirket adı ve e-posta adresi için doğrulama kurallarını güncelleştiriyoruz. Bu, hem yeni hem de mevcut müşteri ayrıntıları için geçerlidir. Gerekli API değişikliği yoktur.

### <a name="impacted-audience"></a>Etkilene hedef kitle

CSP doğrudan fatura iş ortakları ve dolaylı sağlayıcılar

### <a name="details"></a>Ayrıntılar

Microsoft güven üzerinde çalışır. Müşteri şirket adı ve e-posta adresi bilgilerini doğrulamaya ilişkin uyumlu, güvenli ve güvenli bir yöntem sağlamayı taahhüt etmek istiyoruz. 22 Eylül 2021'den itibaren e-posta ve şirket adı doğrulamalarını güncelleştireceksiniz. Daha fazla bilgi için [bkz. Yeni müşteri kaydı ekleme.](../add-a-new-customer.md)

#### <a name="new-rules-for-company-name-and-email-address"></a>Şirket adı ve e-posta adresi için yeni kurallar

22 Eylül 2021'den itibaren aşağıdaki yeni doğrulama kuralları geçerli olacaktır.

Bir şirket adı girerken aşağıdakilere izin verilmez:

- Yalnızca bir karakter kullanma.
- Yalnızca $^# gibi özel &kullanma (tabloya [bakın).](../add-a-new-customer.md#table-of-special-characters)
- Yalnızca boşlukları ve/veya sekmeleri kullanma.
- LLC, Inc vb. gibi kısıtlı listeden bağımsız kısaltmaları kullanma (tabloya [bakın).](../add-a-new-customer.md#table-of-abbreviations)
- ".com", ".org", ".edu", ".club" gibi internet Top-Level Etki Alanı (TDL) uzantılarıyla adları kullanma (tabloya [bakın).](../add-a-new-customer.md#table-of-top-level-domain-extensions)
- Aynı karakterin, 999 gibi başka bir karakterle üç veya daha fazla kez tekrarlanan bir karakter kullanma.
- 1 2 3 gibi tek tek karakterlerle karışık boşluklar ve/veya sekmeler kullanma.

Müşteri e-posta adresi girerken aşağıdakilere izin verilmez:
- E-posta adresi @microsoft.com içermez.
- Müşteri e-posta adresi, iş ortağıyla aynı etki alanı adını içere değildir. Örneğin ABC adlı bir iş ortağı ile müşteri e-postası oluşturamayabilirsiniz. @abc.com

EAP web sayfası sırasında daha fazla ayrıntı bulunabilir:
- Güverte: [https://www.yammer.com/cloudpartnercommunity/#/files/1094484746240](https://www.yammer.com/cloudpartnercommunity/#/files/1094484746240)

- Kayıt: [https://www.yammer.com/cloudpartnercommunity/#/files/1094484361216](https://www.yammer.com/cloudpartnercommunity/#/files/1094484361216)
 
#### <a name="partner-and-customer-impact"></a>İş Ortağı ve Müşteri Etkisi

İş ortakları, 22 Eylül'den itibaren yukarıdaki kurallara uymadıkça müşteri oluşturabilecektir.

_____________

## <a name="readiness-dual-mode-attestation-and-additional-reseller-declaration"></a><a name="7"></a>Hazır olma: Çift modlu uygunluk ve ek kurumsal bayi bildirimi

### <a name="summary"></a>Özet

İş ortaklarının ve müşterilerin işletmelerini güvene dayalı olarak çalıştırmalarına yardımcı olmak için, iş ortaklarının işlem başına aynı kiracı kimliğini kullanırken doğrudan veya dolaylı iş ortakları olarak davranacaklarını doğrulamaları gerekir.

Ayrıca, EU/EFTA ülkelerde işlem yapmakta olan tüm iş ortaklarından, işlemde yer alan ek kurumsal bayileri (en fazla 5 adede kadar) bildirerek talepte bulunabilirsiniz.

### <a name="categories"></a>Kategoriler

- Tarih: 2021-09-07
- Aralık ayında yapılan WW fırlatma için pilot hazırlığı

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

ABD Doları içindeki lisanslı Hizmetleri Transact iş ortakları, düzeltilen fiyatı görmek için en son fiyat listesini indirmelidir.

________________
## <a name="nigeria-and-thailand-are-now-microsoft-managed-countries"></a><a name="4-5"></a>Nijerya ve Tayland artık Microsoft tarafından yönetilen ülkelerle

### <a name="categories"></a>Kategoriler

- Tarih: 2021-09-01
- Özellikler

### <a name="summary"></a>Özet

Nijerya ve Tayland artık Microsoft tarafından yönetilen ülkelerle.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

Nijerya ve Tayland 'daki iş ortakları deneyimidir.

### <a name="details"></a>Ayrıntılar

[Ticari Market yayımcıları Için vergi ayrıntılarına](../tax-details-marketplace.md)bakın.

### <a name="questions"></a>Sorular

bu teklifler hakkında daha fazla soru için lütfen ilgili Yammer topluluklarınızı kontrol edin.

________________
## <a name="announcing-intune-per-device-for-enterprise-for-csp-partners"></a><a name="4"></a>CSP iş ortakları için Enterprise ıntune cihaz başına duyurusu

### <a name="categories"></a>Kategoriler

- Tarih: 2021-09-02
- Özellikler

### <a name="summary"></a>Özet

1 Eylül itibariyle sunulan yeni bir Intune cihaz başına teklif duyuruyoruz.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

Bulut Çözümü Sağlayıcısı (CSP) programında iş ortakları deneyimidir.

### <a name="details"></a>Ayrıntılar

Microsoft Intune, kuruluşunuzda hem fiziksel hem de sanal uç noktaların yönetilmesi ve güvenliğini sağlamak için en kapsamlı birleşik uç nokta yönetimi platformudur. Enterprise kuruluşların, kimliği doğrulanmış bir kullanıcıya atanan cihazları (yani birden çok kimliği doğrulanmış kullanıcı tarafından kullanılmayan) yönetmesine yardımcı olmak için yeni bir ıntune cihaz başına teklif duyuruyoruz.

1 Eylül 2021 ' de kullanılabilir olan bu teklif, Azure Active Directory (Azure AD) eklenirken cihaz başına Intune 'dan yararlanır. Bu, tamamen işlevsel bir deneyimdir ve aşağıdaki hizmet planlarını içerir:

- Exchange Kuruluşu
- Microsoft Intune
- eğitim için Azure Active Directory.

Microsoft iş ortaklarımızın geri bildirimlerine bağlı olarak, cihazın ömrünü kapsayacak beş yıllık bir teklif olarak cihaz başına bir satışa (cihaz + Windows + ıntune) dahil edilecek Enterprise için ıntune cihaz başına, oluşturulmuştur. Bu yeni teklif, CSP 'Lerin anlaşma yapılarını basitleştirmesine yardımcı olur ve müşterilerine daha rekabet sağlayan bir işlem sağlar.

Yeni Intune cihaz başına teklifi hakkında notuna yönelik öğeler:

- bu bir SaaS Enterprise tekliftir ve küçük & orta ölçekli işletme (SMB) müşterileri için tasarlanmamıştır.
- Yalnızca CSP 'Ler için kullanılabilir ve toplu lisanslama veya Web doğrudan için kullanılabilir değildir.
- Beş yıllık bir abonelik için maliyet $150 (USD/ERP).
- Teklif KIMLIĞI: 5170ccfb-e95b-49a4-b7f3-31f631a356ba
- tek kimliği doğrulanmış bir kullanıcıya atanan Windows cihazların kullanıma hazır olarak çalışır.
- Teklif, cihaz tabanlı koşullu erişim içermez.  

### <a name="questions"></a>Sorular

bu teklifler hakkında daha fazla soru için lütfen ilgili Yammer topluluklarınızı kontrol edin.

_____________

## <a name="key-updates-for-the-new-commerce-experience-for-cloud-solution-provider-csp-seat-based-offers"></a><a name="3"></a>Bulut Çözümü Sağlayıcısı (CSP) için yeni ticari deneyim, bilgisayar tabanlı tekliflere yönelik temel güncelleştirmeler

### <a name="summary"></a>Özet

Microsoft, 19 Ağustos 2021 ' e varan bir adım olarak, CSP bilgisayar tabanlı tekliflere yönelik yeni ticari deneyim için önemli güncelleştirmeler içerir.

### <a name="categories"></a>Kategoriler

- Tarih: 2021-09-01
- Özellikler

### <a name="impacted-audience"></a>Etkilenen hedef kitle

CSP doğrudan fatura ortakları ve dolaylı sağlayıcılar ve dolaylı sağlayıcılar aracılığıyla satıcılar

### <a name="details"></a>Ayrıntılar

[Microsoft,](https://partner.microsoft.com/resources/detail/new-commerce-for-csp-seat-based-offers-pdf) 19 ağustos 2021 ' de Microsoft 365, Dynamics 365, güç platformu ve Windows 365 için yeni ticaret deneyimi elde etdiğinin yanı sıra 2021 ekim 'e göre Bu duyuruya bir izleme olarak, kuruluşunuzun bu dönüştürmeye hazırlanmasına yardımcı olmak için aşağıdaki önemli güncelleştirmeleri sunuyoruz:

- Tümleşik korumalı alan testi için bilgisayar tabanlı teklifleri başlatma
- Önümüzdeki CSP Q&Eylül ayının anımsatıcıları
- Microsoft ticaret teşvik programı

#### <a name="launch-of-seat-based-offers-for-integrated-sandbox-testing"></a>Tümleşik korumalı alan testleri için bilgisayar tabanlı tekliflerin başlatılması

1 Eylül 2021 ' de geçerli olan Microsoft, CSP programı için [Yeni ticaret deneyiminde](https://partner.microsoft.com/resources/detail/new-commerce-for-csp-seat-based-offers-pdf) [Tümleşik korumalı alan](/partner-center/develop/test-and-debug) testi için bilgisayar tabanlı teklifleri etkinleştirdi.

CSP 'de Microsoft 365, Dynamics 365, güç platformu ve Windows 365 tekliflerinin eklenmesi, yeni ticaret yolculuğumuza yönelik başka bir büyük kilometre taşdır. Microsoft, ürün yenilikleri, daha iyi araçlar ve iş ortaklarının CSP gelirini büyütmesini ve müşterilere daha fazla seçenek sağlamasını sağlayan yeni iş fırsatlarına erişim sağlar. İş ortaklarının ve müşterilerin dijital dönüşümle başarılı olmasını sağlamak için ticari platformumuzu geliştirdik ve sıralamayı ve abonelik yönetim süreçlerini kolaylaştırıyoruz.

Sandbox test ortamında yer alan iş ortakları, bu tekliflere yönelik daha fazla planlama, işlem yapma ve teknik tümleştirme sağlayan, bilgisayar tabanlı tekliflere yönelik yeni ticaret deneyiminden erken görünürlük sahibi olacaktır.

Korumalı alan ortamına katılmak, kuruluşunuzun şunları yapmasını sağlar:

- Üretimde dağıtım yapmadan önce bir test ortamında API Tümleştirmesi gerçekleştirme
- Başlamadan önce yeni ticaret deneyimini gerçekleştirmek için yeterli zaman vardır

Tablo, tümleşik korumalı alan test ortamında kullanılabilen temel özelliklerin bir özetini sağlar:

| İş ortağı/müşteri tarafından atanan yönetici ayrıcalıkları ayarı | Kısmi alt yükseltme – tam Özellik |
| ----------- | ---------------|
| 1 katmanlı, 2 katmanlı modeller | Destek aracılığıyla kısmi abonelik yükseltmesi |
| Geçerli ve yeni deneyimin yan yana keşfi | Yenileme sırasında zamanlanan değişiklikler  |
| Modern bulma ve satın alma (ürünleri seçme) | Askıya al/özgeçmişi (Destek aracılığıyla) |
| Aboneliği Yönet (otomatik yenileme geçiş, bilgisayar ekleme, hareketi iptal etme) | Ücretsiz Denemeler (yalnızca MAC presentment) |
| Bağımsız eklentiler  | İş ortağı para birimi |
| Faturalandırma planları | Fiyat saydamlığı  |
| Abonelik yaşam döngüsü yönetimi (yetkisiz kullanım süresi) | Multi-Year teklifleri için yıllık faturalandırma planları  |
| Sahiplik kısıtlamaları | Askıya al/özgeçmişi (kendi kendine servis aracılığıyla)  |
| Fatura/keşfi dosyaları | Tam miktar SKU geçişleri için otomatik yeniden atama |
| Orta dönem tam miktar SKU yükseltmeleri | Ücretsiz deneme (tam presentment ile) |
| İptal İlkesi zorlaması: 30 günlük blok 30 gün sonra iptal (genel kullanıma yönelik olarak 72 saat olarak değişir) |  |
|

#### <a name="reminder-for-upcoming-csp-qa-calls-in-september"></a>Önümüzdeki CSP Q&Eylül ayının anımsatıcıları

yakında sunulan [CSP Q Community&](https://globalpbocomm.eventbuilder.com/GlobalCSP) için kaydolun ve Microsoft 365, Dynamics 365, güç platformu ve Windows 365 ' 2021 de yeni ticaret deneyimi hakkında bilgi edinmek ve adım adım ' de yer alan hareket için. csp Community Q&bir çağrı csp doğrudan fatura ve dolaylı iş ortakları csp tarafından başlatılan ve yaklaşan değişikliklerle ilgili soruları içeren bir çağrı için ayrılmıştır. Size kolaylık olması için, topluluk koleksiyonları [iş ortağı hazırlık galerisinde](https://partner.microsoft.com/resources/assets/#/?prog=CSP%7CCSP-Direct%7CCSP-Indirect-Partner&type=collection&search=community%20collection%202021&sort=updated) kullanıma sunulmuştur. bu noktada, soru&bir çağrıda ele alınacaktır.

CSP temel çağrılarının geçmiş kayıtlarını bulmak ve/veya daha fazla bilgi almak istiyorsanız, [CSP temelleri kaydına](https://globalpbocomm.eventbuilder.com/CSPFundamentals)bakın.

#### <a name="microsoft-commerce-incentive-program"></a>Microsoft ticaret teşvik programı

Microsoft, 1 Eylül 2021 ' de, iş ortağı teşvik programının gelişiminde Ekim ayında kullanılabilmesi için bir sonraki adım iş ortakları olduğunu bildirdi. Bu iletişimin iki birincil bileşeni, FY22 teşvikleri kılavuzlar ve Iş Ortağı Merkezi 'nde geliştirilen Gelişmiş teşvikleri deneyimiyle ilgili bilgiler olacaktır.

- **Geliştirilmiş iş ortağı deneyimi**  Microsoft, iş ortakları için kullanıma hazır kullanım için hedefleyerek iş ortağı merkezi 'nde tek bir katılım ve etkinlik platformunda müşteri yaşam döngüsünün satın alınması ve aşamaları boyunca teşvikleri kazanmak için merkezi bir hedef sağlar.

- **Teşvikleri Için yeni yaklaşım**  Yeni teşvik ve yatırım teklifleri, Microsoft Commerce teşvikleri programına eklenmeye devam edecektir. İş ortağı deneyimini basitleştirecek çabayla birlikte, Microsoft, teşvik programı kılavuzlarını Iş Ortağı Merkezi 'nde barındırılan tek bir belge halinde birleştirecek.

### <a name="next-steps"></a>Sonraki adımlar

#### <a name="launch-of-seat-based-offers-for-integrated-sandbox-testing"></a>Tümleşik korumalı alan testleri için bilgisayar tabanlı tekliflerin başlatılması

- Kuruluş tümleşik bir korumalı alan ortamı sağlamamışsa herhangi bir işlem gerekmez. Kurumda tümleşik korumalı alan ortamı yoksa, oluşturmak için [bu](/partner-center/develop/indirect-provider-sandbox-capabilities) adımları izleyin.
- Yeni ticaret deneyiminde Microsoft 365, Dynamics 365, Power Platform ve Windows 365 için [CSP](https://partner.microsoft.com/resources/detail/operating-guide-new-commerce-experience-for-csp-seat-based-offers-pdf) çalışma kılavuzunu gözden geçirerek sürüme ilişkin özellikler, iş kuralları ve adım adım yönergeler hakkında daha fazla bilgi edinin. Düzenli aralıklarla güncelleştirilecek olan çalışma kılavuzunu düzenli olarak kontrol edin.
- Hazırlık haritasında özetlenen [kaynakları gözden geçirme.](https://partner.microsoft.com/resources/detail/readiness-map-new-commerce-experienceseat-based-offers-pdf)
- API belgeleri [klasörünü gözden geçirme.](https://partner.microsoft.com/resources/collection/api-documentation#/)
- Destek için, İş Ortağı Merkezi SDK'sı ve [API Yammer](https://www.yammer.com/cloudpartnercommunity/#/threads/inGroup?type=in_group&feedId=6589502)grubunda konuşmalara bir destek bileti veya gönderi kaydederek özellik adım adımlarının sunumlarının ve kayıtlarının Eylül ayı boyunca paylaşılacak olması.

#### <a name="reminder-for-upcoming-csp-qa-calls-in-september"></a>Eylül ayında gelecek CSP Q&çağrıları için anımsatıcı

- 15 Eylül veya 16 [Eylül'de&CSP Q](https://globalpbocomm.eventbuilder.com/GlobalCSP) Community Çağrılar'a kaydolacaksınız.
- Bu lansman için CSP seat-based offers koleksiyonuna [yönelik yeni ticari](https://partner.microsoft.com/resources/collection/new-commerce-experience-for-csp-seat-based-offers#/) deneyimi gözden geçirme.
- CSP Q&Community Çağrısı'na katılarak, kuruluşta hareket için yeni Microsoft 365, Dynamics 365, Power Platform ve Windows 365 kişilik alan tabanlı ticari deneyimle ilgili sorular sorabilirsiniz.

#### <a name="microsoft-commerce-incentive-program"></a>Microsoft Ticari Teşvik programı

- Kaynak koleksiyonunda gelecek gelişmiş iş ortağı deneyiminde iletişimi [Microsoft Commerce Incentives gözden geçirme.](https://partner.microsoft.com/asset/collection/microsoft-commerce-incentive-resources#/)
- İş Ortağı Teşvikleri portalında güncelleştirilmiş FY22 iş [ortağı teşvik kılavuzlarını gözden geçirebilirsiniz.](https://microsoft.sharepoint.com/teams/PartnerIncentivesPortal)

### <a name="questions"></a>Sorularınız mı var?

Bu teklifler hakkında daha fazla soru için ilgili topluluklarınızı Yammer kontrol edin.

_____________

## <a name="view-this-months-product-launches-and-offers"></a><a name="2"></a>Bu ayın ürün lansmanlarını ve tekliflerini görüntüleme

### <a name="summary"></a>Özet

Eylül 2021 ürün lansman takvimi yayımlandı.

### <a name="categories"></a>Kategoriler

- Tarih: 2021-09-01
- İşletmenizi Büyüt

### <a name="impacted-audience"></a>Etkilene hedef kitle

Bulut Çözümü Sağlayıcısı (CSP) programı aracılığıyla işlem yapılan tüm iş ortakları

### <a name="details"></a>Ayrıntılar

Eylül 2021 [ürün lansman takvimi](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) artık İşlemler için hazır olma kaynak galerisinde kullanılabilir. Yaklaşan ürün lansmanlarını ve tekliflerini burada görüntüle.

### <a name="next-steps"></a>Sonraki adımlar

Ürün [lansman takvimini](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)gözden geçirin ve bilgileri kuruluşta uygun proje katılımcıları ile paylaşın.  

### <a name="questions"></a>Sorularınız mı var?

Bu teklifler hakkında daha fazla soru için ilgili topluluklarınızı Yammer kontrol edin.

_____________

## <a name="software-in-microsoft-china-cloud-solution-provider-program-mccl-csp-to-start-transactions-from-august-12"></a><a name="1"></a>Microsoft Çin'de yazılım Bulut Çözümü Sağlayıcısı (MCCL CSP) ile 12 Ağustos'tan itibaren işlemleri başlatabilirsiniz

### <a name="summary"></a>Özet

3 Ağustos güncelleştirmemize bir takip olarak, MCCL CSP'de yazılım 12 Ağustos 2021'den itibaren işlemleri başlatacak.

### <a name="categories"></a>Kategoriler

- Tarih: 2021-09-01
- İşletmenizi Büyüt

### <a name="impacted-audience"></a>Etkilene hedef kitle

MCCL CSP programı iş ortakları

### <a name="details"></a>Ayrıntılar

#### <a name="mccl-csp-transaction-start"></a>MCCL CSP işlem başlatma

- MCCL CSP, 12 Ağustos 2021'de Çin müşterileri için işlemleri başlatacak.

- Müşteriler, 31 Aralık 2021'e kadar Açık Lisans programında bir iş ortağının yardımıyla yazılım lisansları satın almaya devam edebilir. Kalıcı lisanslar, Açık Lisans programı kullanımdan kaldırana kadar hem MCCL CSP hem de Açık Lisans programlarında kullanılabilir.

#### <a name="open-license-program-deprecation"></a>Açık Lisans programı kullanımdan silindi

- 1 Ocak 2022'den itibaren müşteriler artık Microsoft Open License programı aracılığıyla yazılım lisansları satın alamaz veya yenileyemeyecek.

- Müşteriler kullanım dışı bırakıldıktan sonra bile Açık Lisans programı aracılığıyla edinilen tüm kalıcı yazılım lisanslarına tam haklara ve erişime sahip olmaya devam edebilir. Bu lisansları ve hizmetleri yönetmek için Toplu Lisanslama Hizmet Merkezi'ne de erişmeye devam ediyor.

#### <a name="software-assurance-sa-purchases"></a>Yazılım Güvencesi (SA) satın almaları

- Açık Lisans (L veya SA)&SA teklifleri, Açık Değer (OV) ve Açık Değer Aboneliği (OVS) içinde kullanılabilir olmaya devam edecektir. Ancak, MCCL CSP'de bunu sunmak için bir plan mevcut olduğundan, NE SA ne de L&SA MCCL CSP programında kullanılabilir.

- SA avantajları, süre sonu 1 Ocak 2022'den sonra olsa bile SA süresi dolana kadar devam eder.

- Microsoft OV programı, SA içeren gelecekteki satın almalar için önerilir.

>[!NOTE]
>OV ve OVS programlarını değiştirmeye plan yoktur.

#### <a name="partner-change-management"></a>İş ortağı değişiklik yönetimi

- Mevcut Microsoft Open dağıtımcıları MCCL CSP dolaylı sağlayıcıları olarak ekli.

- Dolaylı sağlayıcılar ve seçilen dolaylı kurumsal bayiler, işlem işlevinin düzgün olduğundan emin olmak için Ağustos ayında üretim ortamı testi yapmak üzere davet edildi.

- Dolaylı iş ortakları için hazırlık atölyeleri Temmuz ayında başladı ve Aralık 2021'e kadar devam edecek.

### <a name="next-steps"></a>Sonraki adımlar

Aşağıdaki kaynaklar aracılığıyla bu değişiklik için hazır olun:

- [Yeni ticaret nedir?](https://partner.microsoft.com/resources/detail/new-commerce-experience-introduction)
- [MCCL CSP dolaylı sağlayıcı playbook'u](https://microsoftapc.sharepoint.com/:b:/t/ChinaLicensingHome/EeWi5axiZ_RCkTbxa-brE-sBGYdLJ5idpnZvFt2MFiTLWw?e=6itfqY)
- [MCCL CSP dolaylı kurumsal bayi playbook'u](https://microsoftapc.sharepoint.com/:b:/t/ChinaLicensingHome/EY-csVS7lFdKpwkRqeJJ4hkBPGWv4qkfINictqVrwKVLxQ?e=9G6ZY1)

Bu değişikliklerin yalnızca MCCL CSP için geçerli olduğunu ve 21 Vianet CSP üzerinde hiçbir etkisi olmadığını unutmayın.

### <a name="questions"></a>Sorularınız mı var?

Başka sorularınız varsa yerel iş ortağı geliştirme yöneticinizle konuşun.
