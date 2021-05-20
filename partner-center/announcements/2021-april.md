---
title: Nisan 2021 duyuruları
description: Microsoft İş Ortağı Merkezi, promosyonlar, teklifler, pazarlar veya mevcut tekliflerde yapılan değişiklikler dahil olmak üzere Nisan 2021 duyuruları.
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
ms.openlocfilehash: 13b8ec9ddd82b38a265606809b8c39c07436e548
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150140"
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
|Doğrulanmış gönderilebilir | Adres doğrulanır ve adresine gönderebilirsiniz. | Tek |
|Doğrulanamayan | Adres doğrulandı. | Tek |
|Etkileşim gerekli | Önerilen adres önemli ölçüde değiştirildi ve kullanıcı onayı gerekiyor. | Tek |
|Cadde kısmi | Adreste verilen cadde kısmi ve daha fazla bilgi gerekiyor. | Birden çok — en fazla üç |
|Şirket içi kısmi | Verilen şirket içi (bina numarası, paket numarası ve diğerleri) kısmi ve daha fazla bilgi gerekiyor. | Birden çok — en fazla üç |
|Birden çok | Adreste kısmi olan birden çok alan vardır (büyük olasılıkla cadde kısmi ve şirket içi kısmı da dahil). | Birden çok — en fazla üç |
|Hiçbiri | Adres yanlış. | Hiçbiri |
|Doğrulanmamış | Adres, doğrulama işlemi aracılığıyla gönderilemedi. | Hiçbiri |

ABD Post kodları, dört basamaklı ek olarak dört basamak döndürür. Örneğin, 12345-6789.

### <a name="next-steps"></a>Sonraki adımlar

- Daha ayrıntılı rehberlik için, [adanmış iş ortağı koleksiyonundaki](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) teknik belgeleri ve sık sorulan soruları gözden geçirin.
- Iş Ortağı Merkezi API 'sini ve Web kullanıcısı deneyimini kullanarak değişiklikleri içerecek şekilde hazırlayın. 
- Güncelleştirme için hazırlamaya başlayabilmeniz için, korumalı alan kiracı KIMLIĞINIZI, test uçuşna dahil edilecek konu uzmanı (Ali Haki) ile paylaşabilirsiniz. 
- Bir denetim masası satıcısı (CPV) çözümü kullanıyorsanız, CPV 'nize başvurun.

### <a name="questions"></a>Sorularınız mı var?

Microsoft ile işlemlere yönelik desteğe ihtiyacınız varsa iş ortağı destek Yammer grubuna ulaşın veya bir [hizmet isteği](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)açın.

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

26 Nisan 2021'den itibaren Rest API içeriği dahil olmak İş Ortağı Merkezi API Swagger belgeleri yeni bir [sitede bulunur.](/rest/api/partner-center-rest/) Eski siteye birkaç hafta sonra erişilemez duruma gelecektir.

### <a name="benefits"></a>Avantajlar

Aşağıdaki İş Ortağı Merkezi API Swagger belgeleri bir **Try It işlevi** sağlar. Bu işlevi kullanmak için, Kimlik Doğrulaması altında listelenen adımları takip edin ve oluşturabilirsiniz bir Taşıyıcı Belirtec [İş Ortağı Merkezi gerekir.](/partner-center/develop/partner-center-authentication#app--user-authentication)

### <a name="next-steps"></a>Sonraki adımlar

Uygun ekibin işlemlerini gözden geçire incelemesi ve güncelleştirmesi için bu bilgileri kuruluş içinde paylaşın.

### <a name="questions"></a>Sorularınız mı var?

Bu teklifler hakkında sorularınız için ilgili Yammer topluluklarınızı kontrol edin.

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

- 30 günlük iade döneminde döndürülen kalıcı yazılım lisansları, ücretli satın alma fiyatının tam kredisi alır.

- 30 günlük iade süresi içinde döndürülen tüm yazılım aboneliği ürünleri, ücretli satın alma fiyatının protratılmış kredisi alır.

Bu ileti, dönüş dönemi ve MPA'daki diğer güncelleştirmeler ile ilgili olarak Aralık 2020 ve Nisan 2021'de tüm CSP iş ortaklarına gönderilen e-posta iletişimlerimizin bir izlemesidir. MPA'yı etkileyen değişikliklerle ilgili tüm ayrıntılar için bu bildirimlere bakın.

#### <a name="software-download-link-expiry"></a>Yazılım indirme bağlantısı süre sonu

3 Haziran 2021'den itibaren, İş Ortağı Merkezi üzerinden kalıcı yazılım ve yazılım aboneliği ürün satın alımları için yazılım indirme bağlantıları, ilk indirmeden itibaren beş günlük bir sona erme tarihine sahip olacak. Süre sonu, 3 Haziran 2021'den önceki ve 3 Haziran 2021'den sonra yapılan tüm satın almalar için geçerlidir.

### <a name="next-steps"></a>Sonraki adımlar

[CSP dönüş dönemi ve indirme bağlantısı süre sonu hakkında SSS](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf)bölümünü gözden geçirin ve bu değişikliklerle ilgili olarak kuruluş içindeki tüm uygun ekipleri bilgilendirin:

### <a name="questions"></a>Sorularınız mı var?

Bu teklifler hakkında sorularınız için ilgili Yammer topluluklarınızı kontrol edin.

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

2020'de [Microsoft,](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) kalıcı yazılım lisanslarının Bulut Çözümü Sağlayıcısı (CSP) programı aracılığıyla iş ortaklarının ve müşterilerin kullanımına açık olacağını duyurdu. İlk kilometre taşı, ticari kalıcı yazılım teklifleri kullanılabilir hale geldiğinde Ocak 2021'de ulaşıldı. Bir sonraki önemli kilometre taşı, kamu sektörü [](https://aka.ms/openlicensepublicsector) tekliflerini kullanılabilir hale geldiğinde Temmuz 2021'de gerçekleşecektir. Ayrıca, [](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) 1 Ocak 2022'den itibaren geçerli olan açık lisans programı aracılığıyla yeni yazılım lisansı satın Yazılım Güvencesi veya çevrimiçi hizmetler yenilemelerinin yapılamayacak olduğunu da ilettik.

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

#### <a name="open-license-resellers"></a>Açık Lisans kurumsal bayileri

- Kuruluş şu anda CSP programına kayıtlı değilse, nasıl başlatılacakları hakkında bilgi almak için dağıtımcınıza ulaşın. Burada dolaylı bir sağlayıcıyla [bağlantı kurun.](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider)

- Organizasyonuz CSP programına zaten kayıtlı ise, burada CSP'de kalıcı yazılım hakkında daha fazla bilgi edinmek için buraya [bakabilirsiniz.](https://partner.microsoft.com/resources/collection/software-in-csp)

### <a name="questions"></a>Sorularınız mı var?

Bu teklifler hakkında daha fazla soru için ilgili Yammer topluluklarınızı kontrol edin.

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

- [Aylık iş ortağı](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)çağrılarımız için destek malzemeleri içeren topluluk koleksiyonları, yaklaşan değişiklikleri ve operasyonel ilgi alanlarına ilişkin zamanında konu başlıklarını vurgular.

- [CSP Aylık](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)Güncelleştirmesi gibi iş ortağı bültenleri

Aylık anımsatıcı olarak, genel promosyon hazırlığı kılavuzunun her İş Ortağı Merkezi yeni bir duyuru yayımlayız.

### <a name="next-steps"></a>Sonraki adımlar

Her ayın başında, operasyon hazırlığı [](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) kaynak galerisinde en son genel promosyon hazırlığı [kılavuzunu bulabilirsiniz.](https://partner.microsoft.com/resources)

Bu bilgileri kuruluşlarınıza uygun kişilerle paylaşın ve "Bu sayfa yararlı oldu mu?" sayfasından kılavuzun ne kadar yararlı olduğunu bize haber ver düğmesini seçin.

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a>Nisan Bulut Çözümü Sağlayıcısı (CSP) topluluk güncelleştirmeleri ve anımsatıcılar

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-16
- Topluluk | Davetler ve anımsatıcılar

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

- [İlgi ve sorgu alan önemli](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) CSP konu başlıklarına ilişkin yenilemeler ve anımsatıcılar.

#### <a name="csp-community-call-qas"></a>CSP Community Call Q&As

Topluluk Çağrısı&As, yaklaşan değişikliklerle ilgili sorularda size yardımcı olabilir. CSP topluluk çağrısı soru-cevap&Nisan, Mayıs ve Haziran 'da gerçekleşirken hemen kaydolun. Bunlar en son başlatmalar, önemli yenileiciler ve anımsatıcıları üzerine odaklanacaktır.

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

Bu duyuru, [Aralık ayında yayınlanan](./2020-december.md#1)Iş ortağı merkezi geliştirmeleri için bir izdir. Bu yayının bir parçası olarak, yeni GET ve POST nitelikleri API 'Leri dağıtılır ve sonuç olarak, **mevcut Get niteliği 6 mayıs 2021 tarihinde kullanımdan** kaldırılacaktır. Bu süre içinde, yeni GÖNDERI Ortağı Merkezi API 'Lerini kullanmak için geçiş yapmanız gerekir. Yeni GÖNDERI API 'Leri, eğitim teklifleri satın almanızı sağlayacaktır, ancak yeni GET API 'Leri, önceden nitelikli kar ve GCC teklifleri satın almanızı sağlayacaktır.

### <a name="next-steps"></a>Sonraki adımlar

- Başarılı ve zamanında geçiş için **yeni API 'Lere güncelleştirin** .

- Işlem hazırlık kaynaklarında **Yeni Iş Ortağı Merkezi API 'si değişikliklerini ve kılavuzunu gözden geçirin** : [Partner Center eğitim müşteri doğrulama işlemi geliştirmeleri](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).

- Bu bilgileri kuruluşunuzdaki uygun ekiplerle ve bu değişikliklere hazırlanmalarına yardımcı olmak için satıcılarla birlikte paylaşabilirsiniz.

### <a name="questions"></a>Sorularınız mı var?

Bu bildirimle ilgili sorularınız için [Iş ortağı merkezi desteği](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals)'ne başvurun.

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

Microsoft, fatura ayrıntılarını SKU açıklaması yerine ürün ayrıntılarına göre görüntülemek için Bulut Çözümü Sağlayıcısı (CSP) programında yeni ticari PDF faturası için yeni bir biçim sunuyor.

### <a name="impacted-audience"></a>Etkilene hedef kitle

CSP programı aracılığıyla işlem yapılan iş ortakları

### <a name="details"></a>Ayrıntılar

Mayıs 2021'den başlayarak, Microsoft CSP programında yeni ticari PDF faturası için SKU açıklaması yerine ürün ayrıntılarına göre faturalama ayrıntılarını görüntülemek için yeni bir biçim sunuyor. Bu yeni güncelleştirmeyle, her ürünü tek bir satırda görüntülerken satır öğelerini ürün türüne göre toplamamız gerekir.

İş ortakları bu değişikliğin 1 Nisan 2021 ile 30 Nisan 2021 arasındaki faturalama dönemi için Mayıs faturalarında yürürlüğe gir olduğunu fark eder. Etkilenen teklifler Ayrılmış Microsoft Azure, Azure abonelikleri (Azure planı) ve Market'tir.

Fatura biçimi güncelleştirildikten sonra yapılan kredi yeniden ödeme istekleri yeni biçimde oluşturulur.

#### <a name="partner-benefits"></a>İş ortağı avantajları

Bu güncelleştirme, iş ortakları için faturalama deneyiminde aşağıdaki geliştirmeleri sunar:

- Kritik verileri korurken fatura boyutu azaltıldı

- Sıkıştırılmış ve kullanıcı dostu faturalar için biçimin sektör standartlarına uygun olması 

Aşağıdaki öğeler etkilenmez:

- Fatura PDF'leri sayfasındaki faturalama özeti sayfası

- Mevcut faturalandırma API 'Leri

- Karşılaştırma dosyaları (keşfi dosyaları, parçalı verileri almak için kullanılabilir.) 

- Kullanım ve lisans tabanlı ücretler faturaları

### <a name="next-steps"></a>Sonraki adımlar

Microsoft iş ortağı web sitesinin [Işlem hazırlık kaynağı galerisinde](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) bu konuyla ilgili bilgileri gözden geçirin. Faturalandırma kaynakları, faturalar, CSP faturalandırma ve vergiler dahil faturalandırma ve vergi konuları hakkında daha fazla bilgi için Iş Ortağı Merkezi ' nde [faturalandırma bölümünü](../billing.md) ziyaret edin.

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

Dünyanın geri kalanındaki müşterilerle iş ortakları, Mart 2021'in sonunda isteğe bağlı ayrıntılar olarak müşterilerin şirket kayıt kimliğini, telefon numarasını ve ara adını girme olanağına sahip olacak.

### <a name="next-steps"></a>Sonraki adımlar

- Daha ayrıntılı rehberlik için ayrılmış iş ortağı koleksiyonunda teknik belgeleri [ve sık](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) sorulan soruları gözden geçirme.
- Api ve web kullanıcı deneyimini İş Ortağı Merkezi değişiklikleri dahil etmek için hazırlanma. API/SDK'lar test için kullanılabilir.
- Yeni müşteri ekleme veya mevcut müşteri ayrıntılarını değiştirme ile ilgili ek verileri gönderdiğinizden emin olun.
- Denetim masası satıcısı (CPV) çözümü kullanıyorsanız CPV'nize başvurun.

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

Bu teklifler hakkında daha fazla soru için ilgili Yammer topluluklarınızı kontrol edin.