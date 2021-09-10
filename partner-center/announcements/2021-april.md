---
title: Nisan 2021 duyuruları
description: Yeni özellikler, promosyonlar, teklifler, pazarlar veya mevcut tekliflerdeki değişiklikler dahil olmak üzere Microsoft İş Ortağı Merkezi için Nisan 2021 duyuruları.
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
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960695"
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
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a>İş Ortağı Merkezi API Swagger belgeleri için yeni konum

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-26
- Özellikler

### <a name="summary"></a>Özet

İş Ortağı Merkezi API Swagger belgeleri önceki [Swagger Belgeleri sitesinden](https://apidocs.microsoft.com/services/partnercenter) yeni bir [Swagger Belgeleri sitesine geçirildi.](/rest/api/partner-center-rest/)

### <a name="impacted-audience"></a>Etkilene hedef kitle

Doğrudan fatura iş ortakları ve Bulut Çözümü Sağlayıcısı API'lerini kullanan Bulut Çözümü Sağlayıcısı (CSP) programına İş Ortağı Merkezi Sağlayıcılar

### <a name="details"></a>Ayrıntılar

26 Nisan 2021'den itibaren Rest API içeriği dahil olmak İş Ortağı Merkezi API Swagger belgeleri yeni bir [sitede bulunur.](/rest/api/partner-center-rest/) Eski siteye birkaç hafta sonra erişilemez duruma gelecektir.

### <a name="benefits"></a>Avantajlar

Aşağıdaki İş Ortağı Merkezi API Swagger belgeleri bir **Try It işlevi** sağlar. Bu işlevi kullanmak için, Kimlik Doğrulaması altında listelenen adımları takip eden bir Taşıyıcı Belirtecin [İş Ortağı Merkezi gerekir.](/partner-center/develop/partner-center-authentication#app--user-authentication)

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
- Işletmenizi büyütün

### <a name="summary"></a>Özet

Bu iletişim, açık lisanslama programına yakında sunulacak değişiklikler için nasıl hazırlanacağına ilişkin ayrıntıları sağlar.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

CSP ve açık lisans iş ortakları

### <a name="details"></a>Ayrıntılar

2020 ' de, Microsoft kalıcı yazılım lisanslarının Bulut Çözümü Sağlayıcısı (CSP) programı aracılığıyla iş ortakları ve müşteriler için genel kullanıma sunulduğunu [duyurmuştur](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) . Ticari kalıcı yazılım teklifi kullanılabilir duruma geldiğinde, 2021 Ocak 'ta ilk kilometre taşına ulaşıldı. Bir sonraki anahtar kilometre taşı, [genel sektör](https://aka.ms/openlicensepublicsector) teklifleri kullanılabilir olduğunda 2021 Temmuz 'da gerçekleşecektir. [Ayrıca,](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) 1 Ocak 2022 ' den itibaren geçerli olan, yazılım güvencesi veya çevrimiçi hizmetler yeni yazılım lisansı satın alma veya yenileme Işlemleri açık lisans programı aracılığıyla yapılabilir.

Kalıcı yazılımın yeni ticaret deneyiminde CSP programına geçişi, iş ortaklarının farklı çözümler ve yönetilen hizmetler sunmak üzere fırsatları genişletmesine yardımcı olur. Bu, müşterilerin buluta geçişini de hızlandıracaktır.  Hem iş ortaklarımız hem de müşterilerimiz için sorunsuz bir geçişin sağlanmasına yardımcı olmak üzere bu düzeltmeleri ve malzemeleri bu dijital dönüştürmeyi hızlandırmak için yaptık:

#### <a name="april-2021"></a>2021 Nisan

[Artık kullanılabilir](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): satıcılar için LISANS-CSP geçiş malzemelerini açma

#### <a name="july-2021"></a>2021 Temmuz

##### <a name="csp"></a>CSP

- 1 Temmuz: kamu sektörü müşterileri için kullanılabilir kalıcı yazılım lisansları

- 7 temmuz: Visual Studio Pro ve Orijinal Windows Edinme sözleşmesi tüm kesimlerde kullanılabilir kalıcı yazılım lisansları

##### <a name="open-value"></a>Açık değer

- 1 Temmuz: eğitim ve kar amacı için açık değer programında bulunan ek SKU 'Lar, açık lisans programına benzer teklifler sağlar

##### <a name="open-license"></a>Açık Lisans

- 1 Temmuz: Microsoft, artık açık lisans programında yeni teklifleri başlatamaz.

#### <a name="january-2022"></a>Ocak 2022

- 1 Ocak: açık lisans programı aracılığıyla yeni satın alma veya yenileme yapılamaz

### <a name="next-steps"></a>Sonraki adımlar

#### <a name="csp-indirect-providers"></a>CSP dolaylı sağlayıcıları

Gelecek ayları kullanarak, iş ortağı topluluk olaylarına katılarak ve satıcıların açık lisans--CSP geçiş malzemelerini kullanarak, CSP programına yönlendiren lisans satıcıları hakkında yardım almak için önümüzdeki ayları kullanın:

- Satıcılar için [lisansdan CSP geçiş malzemelerini açın](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): özelleştirilebilir genel bakış sunumu, e-posta şablonu, CSP dolaylı Bayi ekleme Kılavuzu ve daha fazlası, satıcılarınızın ölçeğini ölçeklendirmenize yardımcı olur.

- [CSP iş ortağı Community](https://globalpbocomm.eventbuilder.com/GlobalCSP) Microsoft iş işlemleri tarafından barındırılan olaylar.  CSP temel bilgilerini (CSP temelleri) öğrenmek veya güncel kalmak ve CSP 'deki yazılımla ilgili sorular sormak (soru-cevap&) için çeşitli oturumlara katılarak.

- (Çok yakında) CSP dolaylı satıcısı – Microsoft Iş Işlemleri tarafından barındırılan odaklı eğitim oturumu.

#### <a name="open-license-resellers"></a>Açık Lisans satıcıları

- Kuruluşunuz Şu anda CSP programına kayıtlı değilse, kullanmaya başlama hakkında bilgi edinmek için dağıtıcıya başvurun. [burada](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider)dolaylı bir sağlayıcı ile Bağlan.

- Kuruluşunuz zaten CSP programına kaydedildiyse, [burada](https://partner.microsoft.com/resources/collection/software-in-csp)CSP 'de kalıcı yazılımlar hakkında daha fazla bilgi edinin.

### <a name="questions"></a>Sorularınız mı var?

bu teklifler hakkında daha fazla soru için ilgili Yammer topluluklarınızı denetleyin.

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a>Şimdi canlı: genel promosyon hazırlığı Kılavuzu

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-16
- Özellikler

### <a name="summary"></a>Özet

Başlatma hazırlığı, Işlem hazırlık kaynağı galerisinde yeni bir [genel promosyon hazırlığı Kılavuzu](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) yayımladı. Bu kılavuz, tüm etkin [küresel promosyonların](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/)birleştirilmiş bir görünümünü sağlar.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

tüm toplu lisanslama (VL), Dynamics fiyat listesi (dpl) ve Bulut Çözümü Sağlayıcısı (CSP) iş ortakları

### <a name="details"></a>Ayrıntılar

Microsoft iş ortakları, destekleyici ayrıntıların bulunduğu tüm küresel promosyonların birleştirilmiş bir görünümünü sağlama gereksinimiyle paylaşılır. Bu birleştirilmiş kılavuzun, tüm kullanılabilir bilgilerin merkezi ve uygun bir konumda erişilebilir olacağı güvenle birlikte yükseltmeleri kullanmanıza yardımcı olacak

Microsoft, 2021 Nisan 'dan itibaren bu kılavuzu aylık olarak güncelleştirecek ve Işlem hazırlık kaynağı galerisinde adanmış bir genel promosyon hazırlığı kılavuz koleksiyonunda kullanılabilir olacaktır.

Bu kılavuza bağlantılar da aşağıdaki koleksiyonlara dahil edilecek:

- Yaklaşan değişikliklerin merkezi bir görünümünü sağlayan ve başlatılan [Takvim koleksiyonunu başlatın](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/).

- aylık iş ortağı aramalarımız için destekleyici malzemeler içeren [Community koleksiyonlar](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), yaklaşan değişiklikleri ve işletimsel ilgi çekici konuları vurgular.

- CSP aylık güncelleştirmesi gibi [Iş ortağı bültenleri](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)

Aylık bir anımsatıcı olarak, genel promosyon hazırlığı Kılavuzu 'ndaki her yeni sorunla bir Iş Ortağı Merkezi duyurusu de yayımlayacağız.

### <a name="next-steps"></a>Sonraki adımlar

Her ayın başlangıcında, en son [genel promosyon hazırlığı kılavuzunu](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) , [işlem hazırlık kaynağı galerisinde](https://partner.microsoft.com/resources)bulabilirsiniz.

Bu bilgileri kuruluşlarınızın ilgili kişileri ile paylaşabilir ve "Bu sayfa yardımcı oldu mu?" kılavuzunun ne kadar faydalı olduğunu bize bildirmek için düğmesini her sayfanın sonundaki düğme.

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a>nisan Bulut Çözümü Sağlayıcısı (CSP) topluluk güncelleştirmesi ve anımsatıcıları

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-16
- Community | Davetlere ve anımsatıcıları

### <a name="summary"></a>Özet

CSP Community kaynakları isteğe bağlı olarak kullanılabilir ve CSP programında değişiklik için hazır ve hazırlanmaya hazırlıklı olmak üzere aylık olarak güncelleştirilir.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

CSP doğrudan fatura ortakları ve dolaylı sağlayıcılar

### <a name="details"></a>Ayrıntılar

Bu ay, kaynaklar aşağıdaki temel konuları içerir:

- [CSP program evrimi ve açık lisans programı değişikliklerinde Güncelleştir](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [Belirli bölgelerde CSP müşterisi ekleme gereksinimlerinde yapılan değişiklikler](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [CSP programındaki yeni ticaret PDF faturası için yeni biçim](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

[CSP topluluk koleksiyonu](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)içinde şunları bulabilirsiniz:

- En son CSP bildirilerini, güncelleştirmeleri, olayları ve anımsatıcıları kolay okunabilir bir belgede toplayan, indirilebilir [CSP aylık güncelleştirme Bülteni](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global).

- Programın etkilediği yaklaşan değişikliklerin zaman çizelgesi görünümünü sağlayan [CSP duyurusu takvimi](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021).

- Yaklaşan ürünün sunduğu ve tekliflerinin görüntüleneceği yeni [ürün başlatma takvimi](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf).

- CSP, anahtar işletimsel değişiklikler üzerinde kullanımı kolay içerik ile [güncelleştirme kaynaklarını başlatın](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) .

- Önemli CSP ile ilgili [Yenileiciler ve anımsatıcıları](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) , ilgi ve sorguları alma konuları.

#### <a name="csp-community-call-qas"></a>CSP Community&çağrı Q

Community Yaklaşan değişikliklerle ilgili sorularınız konusunda size yardımcı olmak için&soru-cevap ' i arayın. CSP için şimdi kaydolun Community nisan, mayıs ve haziran 'da gerçekleşen soru-cevap çağrısı&. Bunlar en son başlatmalar, önemli yenileiciler ve anımsatıcıları üzerine odaklanacaktır.

[Buraya kaydolun](https://globalpbocomm.eventbuilder.com/GlobalCSP).

### <a name="next-steps"></a>Sonraki adımlar

topluluk kaynaklarını gözden geçirin ve soru-cevap Community çağrısı A&kaydolun.

&soru-cevap Community çağrısından en iyi şekilde yararlantığınızdan emin olmak için, isteğe bağlı topluluk içeriğini gözden geçirin ve sorularınızı çağrıdan 48 saate kadar iletin.

### <a name="questions"></a>Sorularınız mı var?

Community aylık csp, csp programındaki değişikliklerle ilgili soruların en iyi yeri olan soru-cevap&çağrı. Her ay, sizin için en önemli olan konularda oturum harcayabilmeniz için malzemeleri gözden geçirin ve sorularınızı önceden gönderebilirsiniz.

Daha fazla bilgi için [desteğe](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)başvurun.

________________
## <a name="final-reminder-deprecation-of-get-qualification-on-may-6-2021"></a><a name="4"></a>Son anımsatıcı: 6 Mayıs 2021 ' de GET nitelemesini kullanımdan kaldırma

### <a name="categories"></a>Kategoriler

- Tarih: 2021-05-04

- Özellikler

### <a name="impacted-audience"></a>Etkilenen hedef kitle

ortaklık, kar amacı ve Government Community Cloud (GCC) satan iş ortakları, iş ortağı merkezi apı 'sini kullanarak Bulut Çözümü Sağlayıcısı programı aracılığıyla sunulur

### <a name="details"></a>Ayrıntılar

Bu duyuru, [Aralık ayında yayınlanan](./2020-december.md#1)Iş ortağı merkezi geliştirmeleri için bir izdir. Bu sürümün bir parçası olarak yeni GET ve POST Nitelik API'leri dağıtıldı ve sonuç olarak mevcut GET niteliği 6 Mayıs **2021'de kaldırılacaktır.** Bu süre boyunca yeni POST api'lerini kullanmaya İş Ortağı Merkezi gerekir. Yeni POST API'leri Eğitim tekliflerini satın alarken, yeni GET API'leri önceden nitelikli Kar Amacı Gütmeyen kuruluş ve GCC olanak sağlayacak.

### <a name="next-steps"></a>Sonraki adımlar

- **Başarılı ve zamanında geçiş için** yeni API'lere güncelleştirin.

- **Yeni İŞ ORTAĞı MERKEZI API değişikliklerini ve** İşlem hazırlığı kaynaklarında Kılavuz'İş Ortağı Merkezi [gözden geçirme: İş Ortağı Merkezi Eğitim müşteri doğrulama süreci geliştirmeleri.](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/)

- Bu bilgileri, bu değişikliklere hazırlanmalarına yardımcı olmak için kuruluş içindeki uygun ekiplerle ve kurumsal bayilerle paylaşın.

### <a name="questions"></a>Sorularınız mı var?

Bu bildirimle ilgili tüm sorular için destek için [İş Ortağı Merkezi başvurun.](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals)

### <a name="change-log"></a>Değişiklik günlüğü

- 4 Mayıs 2021: GET niteliğinin kullanımdan kalkacak olmasıyla ilgili son anımsatıcı

- 9 Nisan 2021: GET niteliğinin kullanımdan kalkacak olduğunu anımsatıcı 

- Şubat: GET ve PUT niteliklerinin kullanımdan & güncelleştirildi

- Ocak: GET ve PUT niteliklerinin gelecek kullanımdan & anımsatıcısı

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a>CSP'de yeni ticari PDF faturası için yeni biçim

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-05
- Özellikler

### <a name="summary"></a>Özet

Microsoft, fatura ayrıntılarını SKU açıklaması yerine ürün ayrıntılarına göre görüntülemek için Bulut Çözümü Sağlayıcısı (CSP) programında yeni ticari PDF faturası için yeni bir biçim sunuyor.

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

İş ortaklarına ve müşterilerin iş ortaklarına ve iş ortaklarına güvene dayalı olarak işlerini çalıştırmalarına yardımcı olmaya ilişkin taahhüdimizin bir parçası olarak, 25 Mart 2021'den itibaren geçerli olmak için ek müşteri bilgileri talep ediyoruz.

### <a name="impacted-audience"></a>Etkilene hedef kitle

CsP doğrudan fatura iş ortakları ve sonraki bölümde listelenen ülkelerde yeni veya mevcut müşterileri olan dolaylı sağlayıcılar

### <a name="details"></a>Ayrıntılar

Microsoft güven üzerinde çalışır. CSP programında müşteri aboneliklerini işlemeye yardımcı olmak için uyumlu, güvenli ve güvenli bir müşteri doğrulama yöntemi sağlamayı taahhüt etmek istiyoruz. 25 Mart 2021'de, aşağıdaki ölçütlerin her ikisini de karşıleyen iş ortaklarını etkileyecek İş Ortağı Merkezi API'si ve kullanıcı arabirimi (UI) geliştirmeleri tanıtacağız:

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

Ölçütlere uyan iş ortaklarının, bir sonraki müşteri için bir abonelik güncelleştirmesi veya oluşturması için müşterinin şirket kayıt kimliğini (müşterinin kuruluş INN'si olarak da bilinir) ve telefon numarasını göndermesi gerekir. Ayrıca bu iş ortakları müşteri için isteğe bağlı bir ikinci ad da girebilir.

Şirket kayıt kimliğinizi eklerken, müşterinin kişisel kimliğini değil, iş verginizi kullanmanız gerektiğini unutmayın.

Aşağıdaki ülkelerde yeni veya mevcut müşterilerle iş yapan iş ortakları, Kasım 2020'de önceki bir sürümle birlikte zaten ek açıklamaya alınmaktadır.

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
- Api ve web kullanıcı deneyimini İş Ortağı Merkezi değişiklikleri dahil etmek için hazırlanma. API/SDK'lar test için kullanılabilir.
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

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a>Bu ayın ürün lansmanlarını ve tekliflerini görüntüleme

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-01
- Özellikler
 
### <a name="summary"></a>Özet

Nisan 2021 ürün lansman takvimi yayımlandı.

### <a name="impacted-audience"></a>Etkilene hedef kitle

Bulut Çözümü Sağlayıcısı (CSP) programı aracılığıyla işlem yapılan tüm iş ortakları

### <a name="details"></a>Ayrıntılar

Nisan 2021 [ürün lansman takvimi](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) artık İşlemler için hazır olma kaynak galerisinde kullanılabilir. Yaklaşan ürün lansmanlarını ve tekliflerini burada görüntüle.

### <a name="next-steps"></a>Sonraki adımlar

Ürün [lansman takvimini](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)gözden geçirin ve bilgileri kuruluşta uygun proje katılımcıları ile paylaşın.  

### <a name="questions"></a>Sorularınız mı var?

Bu teklifler hakkında daha fazla soru için ilgili topluluklarınızı Yammer edin.