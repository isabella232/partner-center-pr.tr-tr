---
title: Nisan 2021 duyuruları
description: Yeni yetenekler, promosyonlar, teklifler, pazarlar veya mevcut tekliflerle ilgili değişiklikler dahil olmak üzere Microsoft Iş Ortağı Merkezi için Nisan 2021 duyuruları.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 04/29/2021
ms.openlocfilehash: 798dcb1570a0f6dfc94c7b45fc3c2e152f55cbe5
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702833"
---
# <a name="april-2021-announcements"></a>Nisan 2021 duyuruları

Bu sayfa, 2021 Nisan için Microsoft Iş Ortağı Merkezi duyuruları sağlar.

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a>Hazırlık: CSP müşteri adresi doğrulama API 'SI, Haziran ayında etkin olacak şekilde güncelleştirildi. test özelliği artık kullanılabilir

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-30
- Hazır Olma

### <a name="summary"></a>Özet

İş ortakları ve müşterilerin işletmelerini temel alarak işlerini çalıştırmasına yardımcı olmak için iş ortaklarını, dünyanın her yerindeki tüm ülkeler için doğrulama adresi API 'sine test etmek üzere davet edeceğiz.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

CSP doğrudan fatura ortakları ve yeni veya var olan müşterilerin adres ayrıntılarını güncelleştiren dolaylı sağlayıcılar

### <a name="details"></a>Ayrıntılar

Microsoft, güvende çalışır. CSP programındaki deneyimidir müşteri abonelikleri için uyumlu, güvenli ve güvenli bir müşteri adresi doğrulama yöntemi sağlamayı taahhüt ediyoruz. 31 Mart 2021 itibariyle, doğrulama adresi API 'sine değişiklikler ekledik. İş ortakları, Haziran 2021 ' nin sonunda, API 'yi test etmek üzere etkin olmaya başlamadan önce davet ediyoruz. 

Bu değişikliklerin yalnızca adresi doğrula API 'sini etkilediğini unutmayın. Müşteri oluşturma ve faturalandırma profilini güncelleştirme API 'Lerini etkilememektedir. Önerilen adresin Şu anda müşteri oluşturma API 'SI ile kullanılması gerekmese de, önemle önerilir.

Yanıt aşağıdaki durum iletilerinden birini döndürür:

| Durum     | Açıklama |    Döndürülen önerilen adreslerin sayısı |
|-------|---------------|-------------------|
|Doğrulanan sevk özellikli | Adres doğrulanır ve sevk edilebilir. | Tek |
|Doğrulanamayan | Adres doğrulandı. | Tek |
|Etkileşim gerekli | Önerilen adres önemli ölçüde değiştirildi ve kullanıcı onayı gerekiyor. | Tek |
|Cadde kısmi | Adreste verilen cadde kısmi ve daha fazla bilgi gerekiyor. | Birden çok — en fazla üç |
|Şirket içi kısmi | Verilen şirket içi (bina numarası, paket numarası ve diğerleri) kısmi ve daha fazla bilgi gerekiyor. | Birden çok — en fazla üç |
|Birden çok | Adreste kısmi olan birden çok alan vardır (büyük olasılıkla cadde kısmi ve şirket içi kısmı da dahil). | Birden çok — en fazla üç |
|Yok | Adres yanlış. | Yok |
|Doğrulanmamış | Adres, doğrulama işlemi aracılığıyla gönderilemedi. | Yok |

ABD Post kodları, dört basamaklı ek olarak dört basamak döndürür. Örneğin, 12345-6789.

### <a name="next-steps"></a>Sonraki adımlar

- Daha ayrıntılı rehberlik için, [adanmış iş ortağı koleksiyonundaki](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) teknik belgeleri ve sık sorulan soruları gözden geçirin.
- Iş Ortağı Merkezi API 'sini ve Web kullanıcısı deneyimini kullanarak değişiklikleri içerecek şekilde hazırlayın. 
- Güncelleştirme için hazırlamaya başlayabilmeniz için, korumalı alan kiracı KIMLIĞINIZI, test uçuşna dahil edilecek konu uzmanı (Ali Haki) ile paylaşabilirsiniz. 
- Bir denetim masası satıcısı (CPV) çözümü kullanıyorsanız, CPV 'nize başvurun.

### <a name="questions"></a>Sorularınız mı var?

Microsoft ile işlemlere yönelik desteğe ihtiyacınız varsa iş ortağı destek Yammer grubuna ulaşın veya bir [hizmet isteği](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)açın.

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a>Iş Ortağı Merkezi API Swagger belgeleri için yeni konum

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-26
- Özellikler

### <a name="summary"></a>Özet

İş Ortağı Merkezi API Swagger belgeleri, [önceki Swagger belge sitesinden](https://apidocs.microsoft.com/services/partnercenter) [Yeni bir Swagger belge sitesine](https://docs.microsoft.com/rest/api/partner-center-rest/)geçirildi.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

Iş Ortağı Merkezi API 'Lerini kullanan bulut çözümü sağlayıcısı (CSP) programına katılan doğrudan fatura ortakları ve dolaylı sağlayıcılar

### <a name="details"></a>Ayrıntılar

26 Nisan 2021 itibariyle, REST API içeriği de dahil olmak üzere Iş Ortağı Merkezi API Swagger belgeleri [Yeni bir sitede](https://docs.microsoft.com/rest/api/partner-center-rest/)bulunuyor. Eski siteye birkaç hafta sonra erişilemeyecektir.

### <a name="benefits"></a>Avantajlar

Iş Ortağı Merkezi API Swagger belgeleri bir **TRY** işlevi sunacaktır. Bu işlevi kullanmak için, [Iş ortağı merkezi kimlik doğrulaması](https://docs.microsoft.com/partner-center/develop/partner-center-authentication#app--user-authentication)' nda listelenen adımları izleyerek oluşturabileceğiniz bir taşıyıcı belirtecine sahip olmanız gerekir.

### <a name="next-steps"></a>Sonraki adımlar

Uygun ekibin süreçlerini gözden geçirebilmesi ve güncelleştirebilmesi için bu bilgileri kuruluşunuz dahilinde paylaşabilirsiniz.

### <a name="questions"></a>Sorularınız mı var?

Bu tekliflerle ilgili sorular için ilgili Yammer topluluklarınızı kontrol edin.

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a>Bulut çözümü sağlayıcısı (CSP) yazılım dönüş dönemi ilkesi ve indirme bağlantısı süre sonu bildirimi

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-21
- Özellikler

### <a name="summary"></a>Özet

CSP yazılım dönüş dönemi ilkesinde değişiklikler ve indirme bağlantısı süre sonu bulunur.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

CSP 'de deneyimidir iş ortakları kalıcı yazılım veya yazılım aboneliği tekliflerini

### <a name="details"></a>Ayrıntılar

Kalıcı yazılım ve yazılım aboneliği satın alımları ile ilgili aşağıdaki önemli bildirimlere Iş Ortağı Merkezi aracılığıyla dikkat edin:

#### <a name="software-return-period-policy"></a>Yazılım dönüş dönemi ilkesi

1 Haziran 2021 ' den itibaren, Microsoft Iş ortağı sözleşmesi 'nde (MPA) belirtilen CSP 'deki yazılım teklifleri için dönüş süresi, sipariş tarihinden itibaren Tarih ile 30 gün arasında 60 değişir.

Yazılım teklifinin bir siparişi gönderildikten sonra, iş ortaklarının bu sırada herhangi bir düzeltme göndermesi için sipariş tarihinden 30 gün daha sahip olur:

- 30 günlük iade dönemi içinde döndürülen herhangi bir kalıcı yazılım lisansı, ücretli satın alma fiyatının tam kredisini alacaktır.

- 30 günlük iade dönemi içinde döndürülen tüm yazılım aboneliği ürünleri, ücretli satın alma fiyatının eşit oranda dağıtılmış bir kredisi alır.

Bu ileti, 2020 Aralık tarihinde gönderilen e-posta iletişimimizi takip eden bir izleme ve MPA 'nın geri dönüş dönemi ve diğer güncelleştirmeleriyle ilgili tüm CSP iş ortakları için 2021 Nisan. MPA 'nın etkilediği değişikliklerle ilgili tam Ayrıntılar için bu bildirimlere bakın.

#### <a name="software-download-link-expiry"></a>Yazılım indirme bağlantısı süre sonu

3 Haziran 2021 ' den, kalıcı yazılım ve yazılım aboneliği satın alma işlemleri için Iş Ortağı Merkezi aracılığıyla yapılan yazılım indirme bağlantılarının ilk indirmesinden beş gün sona erme tarihi olacaktır. Süre sonu dönemi 3 Haziran 2021 ' den önceki tüm satın alımlar için, 3 Haziran 2021 ' de veya sonrasında geçerlidir.

### <a name="next-steps"></a>Sonraki adımlar

[CSP dönüş dönemini gözden geçirin ve bağlantı süre sonu hakkında SSS 'yi indirin](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf)ve bu değişiklikleri kuruluşunuzdaki tüm uygun takımları bilgilendirin:

### <a name="questions"></a>Sorularınız mı var?

Bu tekliflerle ilgili sorular için ilgili Yammer topluluklarınızı kontrol edin.

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a>Lisanslama programını açın: satıcıları bulut çözümü sağlayıcısı (CSP) programına geçiş

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-19
- Işletmenizi büyütün

### <a name="summary"></a>Özet

Bu iletişim, açık lisanslama programına yakında sunulacak değişiklikler için nasıl hazırlanacağına ilişkin ayrıntıları sağlar.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

CSP ve açık lisans iş ortakları

### <a name="details"></a>Ayrıntılar

2020 ' de, Microsoft kalıcı yazılım lisanslarının bulut çözümü sağlayıcısı (CSP) programı aracılığıyla iş ortakları ve müşteriler için genel kullanıma sunulduğunu [duyurmuştur](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) . Ticari kalıcı yazılım teklifi kullanılabilir duruma geldiğinde, 2021 Ocak 'ta ilk kilometre taşına ulaşıldı. Bir sonraki anahtar kilometre taşı, [genel sektör](https://aka.ms/openlicensepublicsector) teklifleri kullanılabilir olduğunda 2021 Temmuz 'da gerçekleşecektir. [Ayrıca,](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) 1 Ocak 2022 ' den itibaren geçerli olan, yazılım güvencesi veya çevrimiçi hizmetler yeni yazılım lisansı satın alma veya yenileme Işlemleri açık lisans programı aracılığıyla yapılabilir.

Kalıcı yazılımın yeni ticaret deneyiminde CSP programına geçişi, iş ortaklarının farklı çözümler ve yönetilen hizmetler sunmak üzere fırsatları genişletmesine yardımcı olur. Bu, müşterilerin buluta geçişini de hızlandıracaktır.  Hem iş ortaklarımız hem de müşterilerimiz için sorunsuz bir geçişin sağlanmasına yardımcı olmak üzere bu düzeltmeleri ve malzemeleri bu dijital dönüştürmeyi hızlandırmak için yaptık:

#### <a name="april-2021"></a>2021 Nisan

[Artık kullanılabilir](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): satıcılar için LISANS-CSP geçiş malzemelerini açma

#### <a name="july-2021"></a>2021 Temmuz

##### <a name="csp"></a>CSP

- 1 Temmuz: kamu sektörü müşterileri için kullanılabilir kalıcı yazılım lisansları

- 7 Temmuz: Visual Studio Pro ve tüm kesimlerde kullanılabilen orijinal Windows sözleşmesi kalıcı yazılım lisanslarını al

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

- Microsoft Iş Işlemleri tarafından barındırılan [CSP Iş ortağı topluluk olayları](https://globalpbocomm.eventbuilder.com/GlobalCSP) .  CSP temel bilgilerini (CSP temelleri) öğrenmek veya güncel kalmak ve CSP 'deki yazılımla ilgili sorular sormak (soru-cevap&) için çeşitli oturumlara katılarak.

- (Çok yakında) CSP dolaylı satıcısı – Microsoft Iş Işlemleri tarafından barındırılan odaklı eğitim oturumu.

#### <a name="open-license-resellers"></a>Açık Lisans satıcıları

- Kuruluşunuz Şu anda CSP programına kayıtlı değilse, kullanmaya başlama hakkında bilgi edinmek için dağıtıcıya başvurun. Dolaylı bir sağlayıcıya [buradan](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider)bağlanın.

- Kuruluşunuz zaten CSP programına kaydedildiyse, [burada](https://partner.microsoft.com/resources/collection/software-in-csp)CSP 'de kalıcı yazılımlar hakkında daha fazla bilgi edinin.

### <a name="questions"></a>Sorularınız mı var?

Bu teklifler hakkında daha fazla soru için ilgili Yammer topluluklarınızı kontrol edin.

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a>Şimdi canlı: genel promosyon hazırlığı Kılavuzu

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-16
- Özellikler

### <a name="summary"></a>Özet

Başlatma hazırlığı, Işlem hazırlık kaynağı galerisinde yeni bir [genel promosyon hazırlığı Kılavuzu](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) yayımladı. Bu kılavuz, tüm etkin [küresel promosyonların](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/)birleştirilmiş bir görünümünü sağlar.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

Tüm toplu lisanslama (VL), Dynamics fiyat listesi (DPL) ve bulut çözümü sağlayıcısı (CSP) iş ortakları

### <a name="details"></a>Ayrıntılar

Microsoft iş ortakları, destekleyici ayrıntıların bulunduğu tüm küresel promosyonların birleştirilmiş bir görünümünü sağlama gereksinimiyle paylaşılır. Bu birleştirilmiş kılavuzun, tüm kullanılabilir bilgilerin merkezi ve uygun bir konumda erişilebilir olacağı güvenle birlikte yükseltmeleri kullanmanıza yardımcı olacak

Microsoft, 2021 Nisan 'dan itibaren bu kılavuzu aylık olarak güncelleştirecek ve Işlem hazırlık kaynağı galerisinde adanmış bir genel promosyon hazırlığı kılavuz koleksiyonunda kullanılabilir olacaktır.

Bu kılavuza bağlantılar da aşağıdaki koleksiyonlara dahil edilecek:

- Yaklaşan değişikliklerin merkezi bir görünümünü sağlayan ve başlatılan [Takvim koleksiyonunu başlatın](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/).

- Aylık iş ortağı aramalarımıza yönelik destekleyici malzemeler içeren [topluluk koleksiyonları](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), yaklaşan değişiklikleri ve işletimsel ilgi çekici konuları vurgular.

- CSP aylık güncelleştirmesi gibi [Iş ortağı bültenleri](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)

Aylık bir anımsatıcı olarak, genel promosyon hazırlığı Kılavuzu 'ndaki her yeni sorunla bir Iş Ortağı Merkezi duyurusu de yayımlayacağız.

### <a name="next-steps"></a>Sonraki adımlar

Her ayın başlangıcında, en son [genel promosyon hazırlığı kılavuzunu](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) , [işlem hazırlık kaynağı galerisinde](https://partner.microsoft.com/resources)bulabilirsiniz.

Bu bilgileri kuruluşlarınızın ilgili kişileri ile paylaşabilir ve "Bu sayfa yardımcı oldu mu?" kılavuzunun ne kadar faydalı olduğunu bize bildirmek için düğmesini her sayfanın sonundaki düğme.

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a>Nisan bulut çözümü sağlayıcısı (CSP) topluluk güncelleştirmesi ve anımsatıcıları

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-16
- Topluluk | Davetlere ve anımsatıcıları

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

#### <a name="csp-community-call-qas"></a>CSP topluluk çağrısı soru-cevap&

Topluluk çağrısı soru-cevap, yaklaşan değişikliklerle ilgili sorularınız konusunda size yardımcı olacak şekilde&. CSP topluluk çağrısı soru-cevap&Nisan, Mayıs ve Haziran 'da gerçekleşirken hemen kaydolun. Bunlar en son başlatmalar, önemli yenileiciler ve anımsatıcıları üzerine odaklanacaktır.

[Buraya kaydolun](https://globalpbocomm.eventbuilder.com/GlobalCSP).

### <a name="next-steps"></a>Sonraki adımlar

Topluluk kaynaklarını gözden geçirin ve topluluk çağrısı Q&A için kaydolun.

Soru-cevap&topluluk çağrısından en iyi şekilde yararlantığınızdan emin olmak için, isteğe bağlı topluluk içeriğini gözden geçirin ve sorularınızı çağrıdan önce 48 saate kadar iletin.

### <a name="questions"></a>Sorularınız mı var?

Aylık CSP topluluk çağrısı Q&A, CSP programındaki değişikliklerle ilgili soruların en iyi yerdir. Her ay, sizin için en önemli olan konularda oturum harcayabilmeniz için malzemeleri gözden geçirin ve sorularınızı önceden gönderebilirsiniz.

Daha fazla bilgi için [desteğe](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)başvurun.

________________
## <a name="final-reminder-deprecation-of-get-qualification-on-may-6-2021"></a><a name="4"></a>Son anımsatıcı: 6 Mayıs 2021 ' de GET nitelemesini kullanımdan kaldırma

### <a name="categories"></a>Kategoriler

- Tarih: 2021-05-04

- Özellikler

### <a name="impacted-audience"></a>Etkilenen hedef kitle

Iş Ortağı Merkezi API 'sini kullanarak bulut çözümü sağlayıcısı programı aracılığıyla akademik, kar amacı gütmeyen ve kamu Community bulutu (GCC) satan iş ortakları

### <a name="details"></a>Ayrıntılar

Bu duyuru, [Aralık ayında yayınlanan](https://docs.microsoft.com/partner-center/announcements/2020-december#1)Iş ortağı merkezi geliştirmeleri için bir izdir. Bu yayının bir parçası olarak, yeni GET ve POST nitelikleri API 'Leri dağıtılır ve sonuç olarak, **mevcut Get niteliği 6 mayıs 2021 tarihinde kullanımdan** kaldırılacaktır. Bu süre içinde, yeni GÖNDERI Ortağı Merkezi API 'Lerini kullanmak için geçiş yapmanız gerekir. Yeni GÖNDERI API 'Leri, eğitim teklifleri satın almanızı sağlayacaktır, ancak yeni GET API 'Leri, önceden nitelikli kar ve GCC teklifleri satın almanızı sağlayacaktır.

### <a name="next-steps"></a>Sonraki adımlar

- Başarılı ve zamanında geçiş için **yeni API 'Lere güncelleştirin** .

- Işlem hazırlık kaynaklarında **Yeni Iş Ortağı Merkezi API 'si değişikliklerini ve kılavuzunu gözden geçirin** : [Partner Center eğitim müşteri doğrulama işlemi geliştirmeleri](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).

- Bu bilgileri kuruluşunuzdaki uygun ekiplerle ve bu değişikliklere hazırlanmalarına yardımcı olmak için satıcılarla birlikte paylaşabilirsiniz.

### <a name="questions"></a>Sorularınız mı var?

Bu bildirimle ilgili sorularınız için [Iş ortağı merkezi desteği](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals)'ne başvurun.

### <a name="change-log"></a>Değişiklik günlüğü

- 4 Mayıs 2021: son kullanım dışı bırakma için son anımsatıcı

- 9 Nisan 2021: kullanım dışı bırakma niteliği kullanım dışı bırakma anımsatıcısı 

- Şubat: GET & PUT nitelikleri 'nin kullanımdan kaldırılması için zaman çizelgeleri güncelleştirildi

- Ocak: GET & PUT nitelikleri için yaklaşan kullanım dışı bırakın

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a>CSP 'de yeni ticaret PDF faturası için yeni biçim

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-05
- Özellikler

### <a name="summary"></a>Özet

Microsoft, bulut çözümü sağlayıcısı (CSP) programındaki yeni ticaret PDF faturasına yönelik yeni bir biçim sunarak, fatura ayrıntılarını SKU açıklaması yerine ürün ayrıntısına göre görüntüler.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

CSP programı aracılığıyla iş ortakları deneyimidir

### <a name="details"></a>Ayrıntılar

Microsoft Mayıs 2021 ' den itibaren, Microsoft 'un fatura ayrıntılarını SKU açıklaması yerine ürün ayrıntısına göre görüntülemesi için CSP programındaki yeni ticaret PDF faturasına yönelik yeni bir biçim sunuyor. Bu yeni güncelleştirmeyle, her ürünü tek bir satırda görüntülerken, satır öğelerini ürün türüne göre toplamak için kullanılır.

İş ortakları, bu değişikliğin 1 Nisan 2021 ile 30 Nisan 2021 arasındaki fatura dönemi için faturalandırılmasına göre geçerli olduğunu fark eder. Etkilenen teklifler Microsoft Azure ayrılmış örnek, Azure abonelikleri (Azure planı) ve Market ' dir.

Fatura biçimi güncelleştirildikten sonra yapılan tüm kredi faturaları istekleri yeni biçimde oluşturulur.

#### <a name="partner-benefits"></a>İş ortağı avantajları

Bu güncelleştirme, iş ortakları için faturalandırma deneyiminde aşağıdaki geliştirmeleri sunar:

- Kritik verileri korurken fatura boyutu azaltıldı

- Sıkıştırma ve Kullanıcı dostu faturalar için, biçimin sektör standartlarına göre hizalaması 

Aşağıdaki öğeler etkilenmeyecektir:

- Fatura PDF 'sinde Faturalandırma Özeti sayfası

- Mevcut faturalandırma API 'Leri

- Karşılaştırma dosyaları (keşfi dosyaları, parçalı verileri almak için kullanılabilir.) 

- Kullanım ve lisans tabanlı ücretler faturaları

### <a name="next-steps"></a>Sonraki adımlar

Microsoft iş ortağı web sitesinin [Işlem hazırlık kaynağı galerisinde](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) bu konuyla ilgili bilgileri gözden geçirin. Faturalandırma kaynakları, faturalar, CSP faturalandırma ve vergiler dahil faturalandırma ve vergi konuları hakkında daha fazla bilgi için Iş Ortağı Merkezi ' nde [faturalandırma bölümünü](https://docs.microsoft.com/partner-center/billing) ziyaret edin.

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a>Bulut çözümü sağlayıcısı (CSP) müşteri ekleme gereksinimleriyle yapılan değişiklikler

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-02
- Teklifler/Pazarlar

### <a name="summary"></a>Özet

İş ortakları ve müşterilerin işlerini güvenle çalıştırmasına yardımcı olma çabamız kapsamında, 25 Mart 2021 ' den itibaren geçerli olan ek müşteri bilgileri isteyeceğiz.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

CSP doğrudan fatura ortakları ve sonraki bölümde listelenen ülkelerde yeni veya mevcut müşteriler bulunan dolaylı sağlayıcılar

### <a name="details"></a>Ayrıntılar

Microsoft, güvende çalışır. CSP programında deneyimidir müşteri abonelikleri için uyumlu, güvenli ve güvenli bir müşteri doğrulama yöntemi sağlamayı taahhüt ediyoruz. 25 Mart 2021 ' de, aşağıdaki ölçütlerin her ikisini de karşılayan iş ortaklarını etkileyecek Iş Ortağı Merkezi API 'SI ve Kullanıcı arabirimi (UI) geliştirmeleri sunacağız:

- İş ortağı Microsoft ile doğrudan faturalandırma ilişkisine sahiptir (Bu, ortağın doğrudan bir fatura ortağı veya dolaylı bir sağlayıcı olduğu anlamına gelir).

- İş ortağı aşağıdaki ülkelerde yeni veya mevcut müşteriler ile iş yapar:

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

Ölçütlere uyan iş ortaklarının bir müşterinin Şirket kayıt KIMLIĞINI (müşterinin kuruluş adı olarak da bilinir) ve telefon numarasını bir sonraki güncelleştirdiklerinde ve bu müşteri için bir abonelik oluştururken göndermesi gerekecektir. Ayrıca bu iş ortakları müşteri için isteğe bağlı bir ikinci ad da girebilir.

Şirket kayıt KIMLIĞINIZI eklediğinizde müşterinin kişisel KIMLIĞINI değil iş vergi KIMLIĞINIZI kullanmanız gerektiğini unutmayın.

Aşağıdaki ülkelerde yeni veya mevcut müşteriler ile iş yapan iş ortakları, Kasım 2020 ' de daha önceki bir sürüm ile zaten eklendi.

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

Dünyanın geri kalanında müşterilere sahip iş ortakları, 2021 Mart 'ın sonunda, müşteriler için isteğe bağlı ayrıntılar olarak şirket kayıt KIMLIĞI, telefon numarası ve orta adı girme yeteneğine sahip olacaktır.

### <a name="next-steps"></a>Sonraki adımlar

- Daha ayrıntılı rehberlik için, adanmış [iş ortağı koleksiyonundaki](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) teknik belgeleri ve sık sorulan soruları gözden geçirin.
- Iş Ortağı Merkezi API 'sini ve Web kullanıcısı deneyimini kullanarak değişiklikleri dahil etmek için hazırlanın. API/SDK 'lar test için kullanılabilir olacak.
- Yeni müşterileri eklerken veya mevcut müşteri ayrıntılarını değiştirirken ek verileri gönderdiğinizden emin olun.
- Bir denetim masası satıcısı (CPV) çözümü kullanıyorsanız, CPV 'nize başvurun.

### <a name="questions"></a>Sorularınız mı var?

Şirket kayıt KIMLIĞI (ıNN veya tın olarak da bilinir) ile ilgili sorularınız varsa vergi danışmanınıza veya yerel vergi ofisine başvurun. Microsoft, vergi konusunda önemli yönergeler sağlayamaz.

Microsoft ile işlemlerinizi desteklemek için bir [hizmet isteği](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)açın.

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a>Bu aya ait ürünün başlatılan ve tekliflerini görüntüleyin

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-01
- Özellikler
 
### <a name="summary"></a>Özet

Nisan 2021 ürün başlatma takvimi artık yayımlandı.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

Tüm iş ortakları bulut çözümü sağlayıcısı (CSP) programı üzerinden deneyimidir

### <a name="details"></a>Ayrıntılar

Nisan 2021 [ürün başlatma takvimi](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) artık işlem hazırlık kaynağı galerisinde kullanılabilir. Yakında çıkacak ürünü görüntüleyin ve burada teklif edin.

### <a name="next-steps"></a>Sonraki adımlar

[Ürün başlatma takvimini](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)gözden geçirin ve bilgileri kuruluşunuzdaki uygun hissedarlarla paylaşabilirsiniz.  

### <a name="questions"></a>Sorularınız mı var?

Bu teklifler hakkında daha fazla soru için ilgili Yammer topluluklarınızı kontrol edin.
