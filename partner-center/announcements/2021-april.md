---
title: Nisan 2021 duyuruları
description: Yeni özellikler, promosyonlar, teklifler, pazarlar İş Ortağı Merkezi mevcut tekliflerde yapılan değişiklikler dahil olmak üzere Microsoft İş Ortağı Merkezi için Nisan 2021 duyuruları.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-announcements
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 09/01/2021
ms.openlocfilehash: 2b81cf61b8fff5be82a41c4dcc46f24404fa6cf4
ms.sourcegitcommit: 14a1cc0c679a84f9ee6d2eec814528415195162c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/02/2021
ms.locfileid: "123396128"
---
# <a name="april-2021-announcements"></a>Nisan 2021 duyuruları

Bu sayfa, Nisan 2021 için Microsoft İş Ortağı Merkezi duyurularını sağlar.

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a>Hazır olma: CSP müşteri adresi doğrulama API'si Haziran ayında canlı olarak güncelleştirildi; test özelliği artık kullanılabilir

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-30
- Hazır Olma

### <a name="summary"></a>Özet

İş ortaklarının ve müşterilerin işletmelerini güvene dayalı olarak çalıştırmalarına yardımcı olmak için, iş ortaklarını dünya genelindeki tüm ülkeler için Adresi Doğrula API'lerinde yapılan değişiklikleri test etmeye davet ediyoruz.

### <a name="impacted-audience"></a>Etkilene hedef kitle

CsP doğrudan fatura iş ortakları ve mevcut müşterilerin adres ayrıntılarını yeni veya güncelleştiren dolaylı sağlayıcılar

### <a name="details"></a>Ayrıntılar

Microsoft güven üzerinde çalışır. CSP programında müşteri aboneliklerinin işlemesi için uyumlu, güvenli ve güvenli bir müşteri adresi doğrulama yöntemi sağlama konusunda kararlıyız. 31 Mart 2021'den başlanmasıyla birlikte Adresi Doğrula API'sinde değişikliklere yer ve daha fazla bilgi ve uygulama tanıtıldı. İş ortaklarını Haziran 2021'in sonunda canlı yayından önce API'yi test etmelerini davet ediyoruz. 

Bu değişikliklerin yalnızca Adresi Doğrula API'sini etkilediğini unutmayın. Müşteri Oluşturma ve Faturalama Profili API'lerini güncelleştirme işlemi bundan etkilenmez. Önerilen adresin şu anda Müşteri Oluşturma API'si ile kullanılması gerekse de, kesinlikle önerilir.

Yanıt aşağıdaki durum iletilerinden birini geri dönecektir:

| Durum     | Açıklama |    Döndürülen önerilen adres sayısı |
|-------|---------------|-------------------|
|Doğrulanabilir | Adres doğrulanır ve adresine gönderebilirsiniz. | Tek |
|Doğrulandı | Adres doğrulandı. | Tek |
|Etkileşim gerekiyor | Önerilen adres önemli ölçüde değiştirildi ve kullanıcı onayı gerekiyor. | Tek |
|Sokak kısmii | Adreste verilen sokak kısmidir ve daha fazla bilgiye ihtiyaç vardır. | Çoklu— en fazla üç |
|Kısmi şirket içi | Verilen şirket (bina numarası, paket numarası ve diğerleri) kısmidir ve daha fazla bilgiye ihtiyaç vardır. | Çoklu— en fazla üç |
|Birden çok | Adreste kısmi olan birden çok alan vardır (kısmi sokak ve kısmi şirket de dahil olmak üzere). | Çoklu— en fazla üç |
|Hiçbiri | Adres yanlış. | Hiçbiri |
|Doğrulanmamış | Adres doğrulama işlemi aracılığıyla gönderileemedi. | Hiçbiri |

ABD posta kodları ek dört basamaklı + kısa çizgi (örneğin, 12345-6789) dönüşecek.

### <a name="next-steps"></a>Sonraki adımlar

- Daha ayrıntılı rehberlik için ayrılmış iş ortağı koleksiyonunda teknik [belgeleri ve sık](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) sorulan soruları gözden geçirme.
- İş Ortağı Merkezi API'sini ve web kullanıcı deneyimini kullanarak değişiklikleri dahil etmek için hazırlanma. 
- Güncelleştirmeye hazırlanmaya başlayabilirsiniz. Korumalı alan kiracı kimliğini test uçuşuna dahil edilecek konu uzmanı (AliSinki) ile paylaşın. 
- Denetim masası satıcısı (CPV) çözümü kullanıyorsanız CPV'nize başvurun.

### <a name="questions"></a>Sorularınız mı var?

Microsoft ile olan işlemleriniz için de destek gerekirse, iş ortağı destek grubuyla Yammer veya bir hizmet [isteği açın.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a>Api Swagger İş Ortağı Merkezi için yeni konum

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-26
- Özellikler

### <a name="summary"></a>Özet

İş Ortağı Merkezi API Swagger belgeleri önceki [Swagger Belgeleri sitesinden](https://apidocs.microsoft.com/services/partnercenter) yeni bir [Swagger Belgeleri sitesine geçirildi.](/rest/api/partner-center-rest/)

### <a name="impacted-audience"></a>Etkilene hedef kitle

Doğrudan fatura iş ortakları ve Bulut Çözümü Sağlayıcısı API'lerini kullanan Bulut Çözümü Sağlayıcısı (CSP) programına İş Ortağı Merkezi Sağlayıcılar

### <a name="details"></a>Ayrıntılar

26 Nisan 2021'den itibaren Rest API içeriği dahil olmak üzere İş Ortağı Merkezi API Swagger belgeleri yeni bir [sitede bulunur.](/rest/api/partner-center-rest/) Eski siteye birkaç hafta sonra erişilemez duruma gelecektir.

### <a name="benefits"></a>Avantajlar

Aşağıdaki İş Ortağı Merkezi API Swagger belgeleri bir **Try It işlevi** sağlar. Bu işlevi kullanmak için, Kimlik Doğrulaması altında listelenen adımları takip edin ve oluşturabilirsiniz bir Taşıyıcı Belirtec [İş Ortağı Merkezi gerekir.](/partner-center/develop/partner-center-authentication#app--user-authentication)

### <a name="next-steps"></a>Sonraki adımlar

Uygun ekibin işlemlerini gözden geçire incelemesi ve güncelleştirmesi için bu bilgileri kuruluş içinde paylaşın.

### <a name="questions"></a>Sorularınız mı var?

Bu teklifler hakkında sorular için ilgili toplulukları Yammer kontrol edin.

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a>Bulut Çözümü Sağlayıcısı (CSP) yazılım iade dönemi ilkesi ve indirme bağlantısı süre sonu bildirimi

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-21
- Özellikler

### <a name="summary"></a>Özet

CSP yazılımı dönüş dönemi ilkesinde ve indirme bağlantısının süre sonunda değişiklikler vardır.

### <a name="impacted-audience"></a>Etkilene hedef kitle

CSP'de kalıcı yazılım veya yazılım aboneliği tekliflerini işlemden alan iş ortakları

### <a name="details"></a>Ayrıntılar

Kalıcı yazılım ve yazılım aboneliği satın almaları ile ilgili olarak aşağıdaki önemli bildirimleri İş Ortağı Merkezi:

#### <a name="software-return-period-policy"></a>Yazılım iade dönemi ilkesi

1 Haziran 2021'den itibaren, Microsoft İş Ortağı Sözleşmesi (MPA) içinde belirtildiği gibi CSP'de yazılım teklifleri için iade süresi, sipariş tarihinden 60 gün ile sipariş tarihi arasında 30 gün olarak değişecektir.

Bir yazılım teklifi için sipariş gönderildikten sonra, iş ortaklarının bu siparişe düzeltme göndermeleri için sipariş tarihten itibaren 30 günü vardır:

- 30 günlük iade süresi içinde döndürülen kalıcı yazılım lisansları, ücretli satın alma fiyatının tam kredisi alır.

- 30 günlük iade süresi içinde döndürülen tüm yazılım aboneliği ürünleri, ücretli satın alma fiyatının protratılmış kredisi alır.

Bu ileti, dönüş dönemi ve MPA'daki diğer güncelleştirmeler ile ilgili olarak Aralık 2020 ve Nisan 2021'de tüm CSP iş ortaklarına gönderilen e-posta iletişimlerimizin bir izlemesidir. MPA'yı etkileyen değişikliklerle ilgili tüm ayrıntılar için bu bildirimlere bakın.

#### <a name="software-download-link-expiry"></a>Yazılım indirme bağlantısı süre sonu

3 Haziran 2021'den itibaren, İş Ortağı Merkezi aracılığıyla yapılan kalıcı yazılım ve yazılım aboneliği ürün satın alımları için yazılım indirme bağlantıları, ilk indirmeden itibaren beş günlük bir sona erme tarihine sahip olacak. Süre sonu, 3 Haziran 2021'den önceki ve 3 Haziran 2021'den sonra yapılan tüm satın almalar için geçerlidir.

### <a name="next-steps"></a>Sonraki adımlar

[CSP dönüş dönemi ve indirme bağlantısı süre sonu hakkında SSS bölümünü gözden](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf)geçirin ve bu değişikliklerle ilgili olarak kuruluş içindeki tüm uygun ekipleri bilgilendirin:

### <a name="questions"></a>Sorularınız mı var?

Bu teklifler hakkında sorular için ilgili toplulukları Yammer kontrol edin.

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a>Açık Lisans programı: Kurumsal bayileri Bulut Çözümü Sağlayıcısı (CSP) programına geçiş

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-19
- İşletmenizi Büyüt

### <a name="summary"></a>Özet

Bu iletişim, yakında Open Licensing programına gelecek değişikliklere nasıl hazırlanacaklarını ayrıntılarıyla açıklayacak.

### <a name="impacted-audience"></a>Etkilene hedef kitle

CSP ve Açık Lisans iş ortakları

### <a name="details"></a>Ayrıntılar

2020'de [Microsoft,](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) kalıcı yazılım lisanslarının Bulut Çözümü Sağlayıcısı (CSP) programı aracılığıyla iş ortaklarının ve müşterilerin kullanımına açık olacağını duyurdu. İlk kilometre taşı, ticari kalıcı yazılım teklifleri kullanılabilir hale geldiğinde Ocak 2021'de ulaşıldı. Bir sonraki önemli kilometre taşı, kamu sektörü [](https://aka.ms/openlicensepublicsector) tekliflerini kullanılabilir hale geldiğinde Temmuz 2021'de gerçekleşecektir. Ayrıca 1 [Ocak](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) 2022'den itibaren geçerli olacak şekilde, Açık Lisans programı aracılığıyla Yazılım Güvencesi veya çevrimiçi hizmetler yeni yazılım lisansı satın almalarının veya yenilemelerinin yapılamayacaklarını da ilettik.

Kalıcı yazılımların yeni ticaret deneyiminde CSP programına geçişi, iş ortaklarının çeşitli çözümler ve yönetilen hizmetler sunma fırsatlarını genişletmelerini sağlar. Bu, müşterilerin buluta geçişlerini de hızlandırır.  Hem iş ortaklarımız hem de müşterilerimiz için sorunsuz bir geçiş sağlamaya yardımcı olmak için bu dijital dönüşümü hızlandırmak için bu ayarlamaları ve malzemeleri yaptık:

#### <a name="april-2021"></a>Nisan 2021

[Artık kullanılabilir:](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)Kurumsal bayiler için Lisans-CSP geçiş malzemelerini açma

#### <a name="july-2021"></a>Temmuz 2021

##### <a name="csp"></a>CSP

- 1 Temmuz: Kamu sektörü müşterileri tarafından kullanılabilen kalıcı yazılım lisansları

- 7 Temmuz: Visual Studio Pro ve Orijinal Windows Edinme Sözleşmesi kalıcı yazılım lisansları tüm segmentlerde kullanılabilir

##### <a name="open-value"></a>Değer Aç

- 1 Temmuz: Açık Lisans programına benzer teklifler sunan eğitim ve kar amacı gütmeyen kuruluşlara açık değer programında ek SKUS'lar sunulmaktadır

##### <a name="open-license"></a>Açık Lisans

- 1 Temmuz: Microsoft artık Open License programında yeni teklifleri başlatmayacak.

#### <a name="january-2022"></a>Ocak 2022

- 1 Ocak: Açık Lisans programı aracılığıyla yeni satın alma veya yenileme işlemi yapilemez

### <a name="next-steps"></a>Sonraki adımlar

#### <a name="csp-indirect-providers"></a>CSP dolaylı sağlayıcıları

Open License kurumsal bayileri, iş ortağı topluluğu etkinliklerine katılarak ve bayiler için Open License-to-CSP geçiş malzemelerini kullanarak CSP programına katılmalarına yardımcı olmak için önümüzdeki ayları kullanın:

- [Kurumsal bayiler için Lisanstan CSP'ye](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)geçiş malzemeleri :Kurumsal bayilerinizi büyük ölçekte benimsemenize yardımcı olmak için özelleştirilebilir genel bakış sunusu, e-posta şablonu, CSP dolaylı kurumsal bayi ekleme kılavuzu ve daha fazlasını açın.

- [CSP İş Community Microsoft İş](https://globalpbocomm.eventbuilder.com/GlobalCSP) Operasyonları tarafından barındırılan Olaylar.  CSP ile ilgili temel bilgileri (CSP Temel Bilgileri) öğrenmek veya güncel kalmak ve CSP'de Yazılım (Q&A Oturumları) ile ilgili sorular sormak için çeşitli oturumlara katılın.

- (Çok yakında) Microsoft Business Operations tarafından barındırılan CSP dolaylı kurumsal bayi odaklı eğitim oturumu.

#### <a name="open-license-resellers"></a>Açık Lisans kurumsal bayileri

- Kuruluş şu anda CSP programına kayıtlı değilse, nasıl başlatılacakları hakkında bilgi almak için dağıtımcınıza ulaşın. Bağlan sağlayıcı ile bağlantı [kurun.](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider)

- Kuruluş CSP programına zaten kayıtlı ise, burada CSP'de kalıcı yazılım hakkında daha fazla bilgi edinmek için buraya [bakabilirsiniz.](https://partner.microsoft.com/resources/collection/software-in-csp)

### <a name="questions"></a>Sorularınız mı var?

Bu teklifler hakkında daha fazla soru için ilgili topluluklarınızı Yammer kontrol edin.

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a>Artık canlı: Küresel promosyon için hazır olma kılavuzu

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-16
- Özellikler

### <a name="summary"></a>Özet

Launch Readiness, Operations Readiness kaynak [galerisinde yeni bir](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) genel promosyon hazırlığı kılavuzu yayımladı. Bu kılavuz tüm etkin genel promosyonların [birleştirilmiş bir görünümünü sağlar.](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/)

### <a name="impacted-audience"></a>Etkilene hedef kitle

Tüm Toplu Lisanslama (VL), Dynamics Fiyat Listesi (DPL) ve Bulut Çözümü Sağlayıcısı (CSP) iş ortakları

### <a name="details"></a>Ayrıntılar

Microsoft iş ortakları, destek ayrıntılarıyla birlikte tüm genel promosyonların birleştirilmiş bir görünümünü sağlama ihtiyacıyla bizimle paylaştı. Bu birleştirilmiş kılavuzun, tüm kullanılabilir bilgilere merkezi ve kullanışlı bir konumdan kolayca erişil hazır olacağının güveni ile promosyonları kullanmanıza yardımcı olmak istediniz.

Nisan 2021'den itibaren, Microsoft bu kılavuzu aylık olarak güncelleştirecek ve Operasyon hazırlığı kaynak galerisinde ayrılmış bir Küresel Promosyon Hazırlığı Kılavuzu koleksiyonunda kullanılabilir olacak.

Bu kılavuzun bağlantıları aşağıdaki koleksiyonlara da dahil edilir:

- [Yaklaşan değişikliklerin ve](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/)fırlatmaların merkezi bir görünümünü sağlayan takvim koleksiyonunu başlatma.

- [Community iş](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)ortağı çağrılarımız için destek malzemeleri içeren koleksiyonlar, yaklaşan değişiklikleri ve operasyonel ilgiyle ilgili zamanında konu başlıklarını vurgular.

- [CSP Aylık](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)Güncelleştirmesi gibi iş ortağı bültenleri

Aylık anımsatıcı olarak, genel promosyon hazırlığı İş Ortağı Merkezi her yeni sorunuyla birlikte yeni bir duyuru yayımlayabilirsiniz.

### <a name="next-steps"></a>Sonraki adımlar

Her ayın başında, operasyon hazırlığı [](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) kaynak galerisinde en son genel promosyon hazırlığı [kılavuzunu bulabilirsiniz.](https://partner.microsoft.com/resources)

Bu bilgileri kuruluşlarınıza uygun kişilerle paylaşın ve "Bu sayfa yararlı oldu mu?" sayfasından kılavuzun ne kadar yararlı olduğunu bize haber ver düğmesini seçin.

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a>Nisan Bulut Çözümü Sağlayıcısı (CSP) topluluğu güncelleştirmeleri ve anımsatıcılar

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-16
- Community | Davetler ve anımsatıcılar

### <a name="summary"></a>Özet

CSP topluluk kaynakları isteğe bağlı olarak kullanılabilir ve CSP programında değişiklik yapmak için sizi bilgilendirip hazırlıklı olmak için aylık olarak güncelleştirilir.

### <a name="impacted-audience"></a>Etkilene hedef kitle

CSP doğrudan fatura iş ortakları ve dolaylı sağlayıcılar

### <a name="details"></a>Ayrıntılar

Bu ay kaynaklar aşağıdaki önemli konuları içerir:

- [CSP programı evrimi ve Açık Lisans programı değişikliklerine güncelleştirme](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [Belirli bölgelerde CSP müşteri ekleme gereksinimlerinde yapılan değişiklikler](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [CSP programında yeni ticari PDF faturası için yeni biçim](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

[CSP topluluk koleksiyonunda](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)şunları bulabilirsiniz:

- Son [CSP duyurularını,](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global)güncelleştirmelerini, olayları ve anımsatıcıları kolay okunur bir belgede toplanmış indirilebilir CSP Aylık Güncelleştirme bülteni.

- Programı etkileyen yaklaşan değişikliklerin zaman çizelgesi görünümünü sağlayan [CSP](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021)Duyuru Takvimi.

- Yaklaşan [ürün lansmanlarını](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf)ve tekliflerini görüntüyebilirsiniz yeni ürün lansman takvimi.

- [CSP, önemli işlem değişikliklerinde](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) kullanımı kolay içerikle güncelleştirme kaynaklarını başlatacak.

- [İlgi ve sorgu alan önemli](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) CSP konularına ilişkin yenilemeler ve anımsatıcılar.

#### <a name="csp-community-call-qas"></a>CSP Community Q&Olarak Çağırma

Community Yaklaşan değişikliklerle&yardımcı olmak için Q&As çağrısı yapın. Nisan, Mayıs Community Haziran'&Q&CSP'ye hemen kaydol. Bunlar en son başlatmalara, önemli yenilemelere ve anımsatıcılara odaklanır.

[Buraya kayıt olun.](https://globalpbocomm.eventbuilder.com/GlobalCSP)

### <a name="next-steps"></a>Sonraki adımlar

Topluluk kaynaklarını gözden geçirme ve soru-cevap Community için&.

Soru-Cevap'ı Community en iyi şekilde&için isteğe bağlı topluluk içeriğini gözden geçirin ve aramadan 48 saat önceye kadar sorularınıza yanıt gönderin.

### <a name="questions"></a>Sorularınız mı var?

Aylık CSP Community Q&A, CSP programında yapılan değişikliklerle ilgili sorular için en iyi yerdir. Her ay malzemeyi gözden geçirin ve oturumu sizin için en önemli konulara harcayacak şekilde önceden gönderin.

Daha fazla bilgi için Destek ile [iletişime geçin.](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)

________________
## <a name="final-reminder-deprecation-of-get-qualification-on-may-6-2021"></a><a name="4"></a>Son anımsatıcı: 6 Mayıs 2021'de GET niteliği kullanımdan kalkacak

### <a name="categories"></a>Kategoriler

- Tarih: 2021-05-04

- Özellikler

### <a name="impacted-audience"></a>Etkilene hedef kitle

İş Ortağı Merkezi API'sini kullanarak Bulut Çözümü Sağlayıcısı programı aracılığıyla Academic, Nonprofit ve Government Community Cloud (GCC) teklifleri satan İş Ortağı Merkezi iş ortakları

### <a name="details"></a>Ayrıntılar

Bu duyuru, Aralık ayında yayımlanan İş Ortağı Merkezi [bir takiptir.](./2020-december.md#1) Bu sürümün bir parçası olarak yeni GET ve POST Nitelik API'leri dağıtıldı ve sonuç olarak mevcut GET niteliği 6 Mayıs **2021'de kaldırılacaktır.** Bu süre boyunca yeni POST api'lerini kullanmaya İş Ortağı Merkezi gerekir. Yeni POST API'leri Eğitim tekliflerini satın alarken yeni GET API'leri önceden nitelikli Kar Amacı Gütmeyen kuruluş ve GCC sunar.

### <a name="next-steps"></a>Sonraki adımlar

- **Başarılı ve zamanında geçiş için** yeni API'lere güncelleştirin.

- **Yeni API değişikliklerini İş Ortağı Merkezi** Operations Readiness kaynaklarında Kılavuzu gözden geçirme: [İş Ortağı Merkezi Eğitim müşteri doğrulama süreci geliştirmeleri.](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/)

- Bu bilgileri, bu değişikliklere hazırlanmalarına yardımcı olmak için kuruluş içindeki uygun ekiplerle ve kurumsal bayilerle paylaşın.

### <a name="questions"></a>Sorularınız mı var?

Bu bildirimle ilgili tüm sorular için destek için [İş Ortağı Merkezi başvurun.](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals)

### <a name="change-log"></a>Değişiklik günlüğü

- 4 Mayıs 2021: GET niteliğinin kullanımdan kalkacak olmasıyla ilgili son anımsatıcı

- 9 Nisan 2021: GET niteliğinin kullanımdan kalkacak olduğunu anımsatmak 

- Şubat: GET ve PUT niteliklerinin kullanımdan & güncelleştirildi

- Ocak: GET ve PUT niteliklerinin gelecek kullanımdan & anımsatıcısı

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a>CSP'de yeni ticari PDF faturası için yeni biçim

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-05
- Özellikler

### <a name="summary"></a>Özet

Microsoft, SKU açıklaması yerine ürün ayrıntılarına göre faturalama ayrıntılarını görüntülemek için Bulut Çözümü Sağlayıcısı (CSP) programında yeni ticari PDF faturası için yeni bir biçim sunuyor.

### <a name="impacted-audience"></a>Etkilene hedef kitle

CSP programı aracılığıyla işlem yapılan iş ortakları

### <a name="details"></a>Ayrıntılar

Mayıs 2021'den başlayarak, Microsoft CSP programında yeni ticari PDF faturası için SKU açıklaması yerine ürün ayrıntılarına göre faturalama ayrıntılarını görüntülemek için yeni bir biçim sunuyor. Bu yeni güncelleştirmeyle, her ürünü tek bir satırda görüntülerken satır öğelerini ürün türüne göre toplamamız gerekir.

İş ortakları, bu değişikliğin 1 Nisan 2021 ile 30 Nisan 2021 arasındaki faturalama dönemi için Mayıs faturalarında yürürlüğe gireceklerini fark eder. Etkilenen teklifler Ayrılmış Microsoft Azure, Azure abonelikleri (Azure planı) ve Market'tir.

Fatura biçimi güncelleştirildikten sonra yapılan kredi yeniden ödeme istekleri yeni biçimde oluşturulur.

#### <a name="partner-benefits"></a>İş ortağı avantajları

Bu güncelleştirme, iş ortakları için faturalama deneyiminde aşağıdaki geliştirmeleri sunar:

- Kritik verileri korurken fatura boyutu azaltıldı

- Sıkıştırılmış ve kullanıcı dostu faturalar için biçimin sektör standartlarına uygun olması 

Aşağıdaki öğeler etkilenmez:

- Fatura PDF'leri sayfasındaki faturalama özeti sayfası

- Mevcut faturalama API'leri

- Mutabakat dosyaları (Ayrıntılı verileri almak için Mutabakat dosyaları kullanılabilir.) 

- Kullanım ve lisans tabanlı ücretler faturaları

### <a name="next-steps"></a>Sonraki adımlar

Microsoft iş ortağı web sitesinin İşlem hazırlığı kaynak [galerisinde bu konu](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) hakkında bilgileri gözden geçirebilirsiniz. Faturalama kaynakları, faturalar, CSP faturalaması ve vergiler gibi faturalama [](../billing.md) ve vergi konuları hakkında daha fazla bilgi için, İş Ortağı Merkezi.

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a>Bulut Çözümü Sağlayıcısı (CSP) müşteri ekleme gereksinimlerinde yapılan değişiklikler

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-02
- Teklifler/Pazarlar

### <a name="summary"></a>Özet

İş ortaklarına ve müşterilerin iş ortaklarına ve iş ortaklarına güvene dayalı olarak işlerini çalıştırmalarına yardımcı olmaya ilişkin taahhüdüm kapsamında, 25 Mart 2021'den itibaren geçerli olacak şekilde ek müşteri bilgileri talep ediyoruz.

### <a name="impacted-audience"></a>Etkilene hedef kitle

CsP doğrudan fatura iş ortakları ve sonraki bölümde listelenen ülkelerde yeni veya mevcut müşterileri olan dolaylı sağlayıcılar

### <a name="details"></a>Ayrıntılar

Microsoft güven üzerinde çalışır. CSP programında müşteri aboneliklerini işlemeye yardımcı olmak için uyumlu, güvenli ve güvenli bir müşteri doğrulama yöntemi sağlamayı taahhüt etmek istiyoruz. 25 Mart 2021'de, aşağıdaki ölçütlerin her ikisini de karşıleyen iş ortaklarını etkileyecek İş Ortağı Merkezi API ve kullanıcı arabirimi (UI) geliştirmeleri tanıtacağız:

- İş ortağının Microsoft ile doğrudan faturalama ilişkisi vardır (bu da iş ortağının doğrudan fatura iş ortağı veya dolaylı sağlayıcı olduğu anlamına gelir).

- İş ortağı, aşağıdaki ülkelerdeki yeni veya mevcut müşterilerle iş yapar:

    - Tayland
    - Vietnam
    - Türkiye
    - Polonya
    - Güney Afrika
    - Hindistan
    - Brezilya
    - Irak
    - Myanmar
    - Güney Sudan
    - Suudi Arabistan
    - Birleşik Arap Emirlikleri
    - Venezuela

Ölçütlere uyan iş ortaklarının, müşterinin şirket kayıt kimliğini (müşterinin kuruluş INN'si olarak da bilinir) ve bu müşteri için bir sonraki güncelleştirme veya abonelik oluşturma işlemi sırasında telefon numarasını göndermesi gerekir. Ayrıca bu iş ortakları müşteri için isteğe bağlı bir ikinci ad da girebilir.

Şirket kayıt kimliğinizi eklerken, müşterinin kişisel kimliğini değil, iş verginizi kullanmanız gerektiğini unutmayın.

Aşağıdaki ülkelerde yeni veya mevcut müşterilerle iş yapan iş ortakları, Kasım 2020'de önceki bir sürümle birlikte zaten ekli.

- Ermenistan
- Azerbaycan
- Belarus
- Macaristan
- Kazakistan
- Kırgızistan
- Moldova
- Rusya
- Tacikistan
- Ukrayna
- Özbekistan

Dünyanın geri kalanındaki müşterilerle iş ortakları, Mart 2021'in sonunda isteğe bağlı ayrıntılar olarak müşterilerin şirket kayıt kimliğini, telefon numarasını ve ara adını girme olanağına sahip olacak.

### <a name="next-steps"></a>Sonraki adımlar

- Daha ayrıntılı rehberlik için ayrılmış iş ortağı koleksiyonunda teknik belgeleri [ve sık](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) sorulan soruları gözden geçirme.
- Api'yi ve web kullanıcı İş Ortağı Merkezi kullanarak değişiklikleri dahil etmek için hazırlanma. API/SDK'lar test için kullanılabilir.
- Yeni müşteri ekleme veya mevcut müşteri ayrıntılarını değiştirme ile ilgili ek verileri gönderdiğinizden emin olun.
- Denetim masası satıcısı (CPV) çözümü kullanıyorsanız CPV'nize başvurun.

>[!NOTE]
>CSP işlemi işlene değilse, kiracı doğrulanmaz. Bu durumda müşterinin Microsoft Yönetim Portalı'dan bir deneme teklifi satın alması gerekir.
>
>#### <a name="purchase-a-trial-offer"></a>Deneme teklifi satın alma
>
>1. Microsoft [Yönetim Merkezi portalını açın.](https://admin.microsoft.com/)
>
>2. Sol gezinti menüsünde Faturalama'ya ve **ardından** Hizmetleri satın **alın'a tıklayın.**
>
>3. Planı ve ardından **Checkout 'ı seçin.**
>
>Kiracı doğrulanmasına ve CSP işlemlerine izin vermeye hazırdır.

### <a name="questions"></a>Sorularınız mı var?

Şirket kayıt kimliğiyle (INN veya TIN olarak da adlandırılan) ilgili sorularınız varsa vergi danışmanınıza veya yerel vergi ofisinize ulaşın. Microsoft, vergiler konusunda rehberlik sağamaz.

Microsoft ile işlemleriniz için de destek gerekirse bir hizmet [isteği açın.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a>Bu aya ait ürünün başlatılan ve tekliflerini görüntüleyin

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-01
- Özellikler
 
### <a name="summary"></a>Özet

Nisan 2021 ürün başlatma takvimi artık yayımlandı.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

tüm iş ortakları Bulut Çözümü Sağlayıcısı (CSP) programı üzerinden deneyimidir

### <a name="details"></a>Ayrıntılar

Nisan 2021 [ürün başlatma takvimi](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) artık işlem hazırlık kaynağı galerisinde kullanılabilir. Yakında çıkacak ürünü görüntüleyin ve burada teklif edin.

### <a name="next-steps"></a>Sonraki adımlar

[Ürün başlatma takvimini](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)gözden geçirin ve bilgileri kuruluşunuzdaki uygun hissedarlarla paylaşabilirsiniz.  

### <a name="questions"></a>Sorularınız mı var?

bu teklifler hakkında daha fazla soru için ilgili Yammer topluluklarınızı kontrol edin.