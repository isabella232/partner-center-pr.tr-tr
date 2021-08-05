---
title: Nisan 2021 duyuruları
description: Yeni yetenekler, promosyonlar, teklifler, pazarlar veya mevcut tekliflerle ilgili değişiklikler dahil olmak üzere Microsoft Iş Ortağı Merkezi için Nisan 2021 duyuruları.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-announcements
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 04/29/2021
ms.openlocfilehash: 0756a67092cad6fc7750931a5a5f85f61ea7b56b
ms.sourcegitcommit: 90bf27df911b428b1222f483c32ba6367870e7c5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/04/2021
ms.locfileid: "115102499"
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
|Hiçbiri | Adres yanlış. | Hiçbiri |
|Doğrulanmamış | Adres, doğrulama işlemi aracılığıyla gönderilemedi. | Hiçbiri |

ABD Post kodları, dört basamaklı ek olarak dört basamak döndürür. Örneğin, 12345-6789.

### <a name="next-steps"></a>Sonraki adımlar

- Daha ayrıntılı rehberlik için, [adanmış iş ortağı koleksiyonundaki](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) teknik belgeleri ve sık sorulan soruları gözden geçirin.
- Iş Ortağı Merkezi API 'sini ve Web kullanıcısı deneyimini kullanarak değişiklikleri içerecek şekilde hazırlayın. 
- Güncelleştirme için hazırlamaya başlayabilmeniz için, korumalı alan kiracı KIMLIĞINIZI, test uçuşna dahil edilecek konu uzmanı (Ali Haki) ile paylaşabilirsiniz. 
- Bir denetim masası satıcısı (CPV) çözümü kullanıyorsanız, CPV 'nize başvurun.

### <a name="questions"></a>Sorularınız mı var?

Microsoft ile işlemlere yönelik desteğe ihtiyacınız varsa, iş ortağı destek Yammer grubuna ulaşın veya bir [hizmet isteği](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)açın.

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a>Iş Ortağı Merkezi API Swagger belgeleri için yeni konum

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-26
- Özellikler

### <a name="summary"></a>Özet

İş Ortağı Merkezi API Swagger belgeleri, [önceki Swagger belge sitesinden](https://apidocs.microsoft.com/services/partnercenter) [Yeni bir Swagger belge sitesine](/rest/api/partner-center-rest/)geçirildi.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

iş ortağı merkezi apı 'lerini kullanan Bulut Çözümü Sağlayıcısı (CSP) programa katılan doğrudan fatura ortakları ve dolaylı sağlayıcılar

### <a name="details"></a>Ayrıntılar

26 Nisan 2021 itibariyle, REST API içeriği de dahil olmak üzere Iş Ortağı Merkezi API Swagger belgeleri [Yeni bir sitede](/rest/api/partner-center-rest/)bulunuyor. Eski siteye birkaç hafta sonra erişilemeyecektir.

### <a name="benefits"></a>Avantajlar

Iş Ortağı Merkezi API Swagger belgeleri bir **TRY** işlevi sunacaktır. Bu işlevi kullanmak için, [Iş ortağı merkezi kimlik doğrulaması](/partner-center/develop/partner-center-authentication#app--user-authentication)' nda listelenen adımları izleyerek oluşturabileceğiniz bir taşıyıcı belirtecine sahip olmanız gerekir.

### <a name="next-steps"></a>Sonraki adımlar

Uygun ekibin süreçlerini gözden geçirebilmesi ve güncelleştirebilmesi için bu bilgileri kuruluşunuz dahilinde paylaşabilirsiniz.

### <a name="questions"></a>Sorularınız mı var?

bu tekliflerle ilgili sorular için ilgili Yammer topluluklarınızı kontrol edin.

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a>Bulut Çözümü Sağlayıcısı (CSP) yazılım dönüş dönemi ilkesi ve indirme bağlantısı süre sonu bildirimi

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

bu tekliflerle ilgili sorular için ilgili Yammer topluluklarınızı kontrol edin.

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a>lisanslama programını açın: satıcıları Bulut Çözümü Sağlayıcısı (CSP) programına geçiş

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-19
- İşletmenizi Büyüt

### <a name="summary"></a>Özet

Bu iletişim, yakında Open Licensing programına gelecek değişikliklere nasıl hazırlanacaklarını ayrıntılarıyla açıklayacak.

### <a name="impacted-audience"></a>Etkilene hedef kitle

CSP ve Açık Lisans iş ortakları

### <a name="details"></a>Ayrıntılar

2020'de [Microsoft,](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) kalıcı yazılım lisanslarının Bulut Çözümü Sağlayıcısı (CSP) programı aracılığıyla iş ortaklarının ve müşterilerin kullanımına açık olacağını duyurdu. İlk kilometre taşı, ticari kalıcı yazılım teklifleri kullanılabilir hale geldiğinde Ocak 2021'de ulaşıldı. Bir sonraki önemli kilometre taşı, kamu sektörü [](https://aka.ms/openlicensepublicsector) tekliflerini kullanılabilir hale geldiğinde Temmuz 2021'de gerçekleşecektir. Ayrıca, [](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) 1 Ocak 2022'den itibaren geçerli olan açık lisans programı aracılığıyla yeni yazılım lisansı satın Yazılım Güvencesi veya çevrimiçi hizmetler yenilemelerinin yapılamayacak olduğunu da ilettik.

Kalıcı yazılımların yeni ticaret deneyiminde CSP programına geçişi, iş ortaklarının çeşitli çözümler ve yönetilen hizmetler sunmak için fırsatları genişletmesini sağlar. Bu, müşterilerin buluta geçişlerini de hızlandırır.  Hem iş ortaklarımız hem de müşterilerimiz için sorunsuz bir geçiş sağlamaya yardımcı olmak için bu dijital dönüşümü hızlandırmak için bu ayarlamaları ve malzemeleri yaptık:

#### <a name="april-2021"></a>Nisan 2021

[Artık kullanılabilir:](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)Kurumsal bayiler için Lisans-CSP geçiş malzemelerini açma

#### <a name="july-2021"></a>Temmuz 2021

##### <a name="csp"></a>CSP

- 1 Temmuz: Kamu sektörü müşterileri tarafından kullanılabilen kalıcı yazılım lisansları

- 7 Temmuz: Visual Studio Pro ve Orijinal Windows Edinme Sözleşmesi kalıcı yazılım lisansları tüm segmentlerde kullanılabilir

##### <a name="open-value"></a>Değer Aç

- 1 Temmuz: Açık Lisans programına benzer teklifler sunan eğitim ve kar amacı gütmeyen kuruluşlara açık değer programında ek SKUS'lar sunulmaktadır

##### <a name="open-license"></a>Açık Lisans

- 1 Temmuz: Microsoft artık Açık Lisans programında yeni teklifleri başlatmayacak.

#### <a name="january-2022"></a>Ocak 2022

- 1 Ocak: Açık Lisans programı aracılığıyla yeni satın alma veya yenileme işlemi yapilemez

### <a name="next-steps"></a>Sonraki adımlar

#### <a name="csp-indirect-providers"></a>CSP dolaylı sağlayıcıları

Open License kurumsal bayileri, iş ortağı topluluğu etkinliklerine katılarak ve bayiler için Açık Lisans-CSP geçiş malzemelerini kullanarak CSP programına katılmalarına yardımcı olmak için önümüzdeki ayları kullanın:

- [Kurumsal bayiler için Lisanstan CSP'ye](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)geçiş malzemeleri :Kurumsal bayilerinizi büyük ölçekte benimsemenize yardımcı olmak için özelleştirilebilir genel bakış sunusu, e-posta şablonu, CSP dolaylı kurumsal bayi ekleme kılavuzu ve daha fazlasını açın.

- [CSP İş Community Microsoft](https://globalpbocomm.eventbuilder.com/GlobalCSP) İş Operasyonları tarafından barındırılan Olaylar.  CSP ile ilgili temel bilgileri (CSP Temel Bilgileri) öğrenmek veya güncel kalmak ve CSP'de Yazılım (Q&A Oturumları) ile ilgili sorular sormak için çeşitli oturumlara katılın.

- (Çok yakında) Microsoft Business Operations tarafından barındırılan CSP dolaylı kurumsal bayi odaklı eğitim oturumu.

#### <a name="open-license-resellers"></a>Açık Lisans kurumsal bayileri

- Kuruluş şu anda CSP programına kayıtlı değilse, nasıl başlatılacakları hakkında bilgi almak için dağıtımcınıza ulaşın. Bağlan sağlayıcıyla bağlantı [kurun.](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider)

- Organizasyonuz CSP programına zaten kayıtlı ise, burada CSP'de kalıcı yazılım hakkında daha fazla bilgi edinmek için buraya [bakabilirsiniz.](https://partner.microsoft.com/resources/collection/software-in-csp)

### <a name="questions"></a>Sorularınız mı var?

Bu teklifler hakkında daha fazla soru için ilgili toplulukları Yammer kontrol edin.

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

- [Community iş](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)ortağı çağrılarımız için destek malzemeleri içeren koleksiyonları ve yaklaşan değişiklikleri ve operasyonel ilgi alanlarına ilişkin zamanında konu başlıklarını vurgulayın.

- [CSP Aylık](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)Güncelleştirmesi gibi iş ortağı bültenleri

Aylık anımsatıcı olarak, genel promosyon hazırlığı kılavuzunun her İş Ortağı Merkezi yeni bir duyuru yayımlayız.

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

Aylık CSP Community Q&A çağrısı, CSP programı değişiklikleriyle ilgili sorular için en iyi yerdir. Her ay malzemeyi gözden geçirin ve oturumu sizin için en önemli konulara harcayacak şekilde önceden gönderin.

Daha fazla bilgi için Destek ile [iletişime geçin.](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)

________________
## <a name="final-reminder-deprecation-of-get-qualification-on-may-6-2021"></a><a name="4"></a>Son anımsatıcı: 6 Mayıs 2021'de GET niteliği kullanımdan kalkacak

### <a name="categories"></a>Kategoriler

- Tarih: 2021-05-04

- Özellikler

### <a name="impacted-audience"></a>Etkilene hedef kitle

İş Ortağı Merkezi API'sini kullanarak Bulut Çözümü Sağlayıcısı programı aracılığıyla Academic, Government Community Cloud Nonprofit ve GCC (GCC) teklifleri satan İş Ortağı Merkezi iş ortakları

### <a name="details"></a>Ayrıntılar

Bu duyuru, Aralık ayında yayımlanan İş Ortağı Merkezi [bir takiptir.](./2020-december.md#1) Bu yayının bir parçası olarak, yeni GET ve POST nitelikleri API 'Leri dağıtılır ve sonuç olarak, **mevcut Get niteliği 6 mayıs 2021 tarihinde kullanımdan** kaldırılacaktır. Bu süre içinde, yeni GÖNDERI Ortağı Merkezi API 'Lerini kullanmak için geçiş yapmanız gerekir. yeni gönderi apı 'leri, eğitim teklifleri satın almanızı sağlayacaktır, ancak yeni GET apı 'leri, önceden nitelikli kar ve GCC teklifleri satın almanızı sağlayacaktır.

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

Microsoft, Bulut Çözümü Sağlayıcısı (CSP) programında yeni ticaret PDF faturasına yönelik yeni bir biçim sunarak, fatura ayrıntılarını SKU açıklaması yerine ürün ayrıntısına göre görüntüler.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

CSP programı aracılığıyla iş ortakları deneyimidir

### <a name="details"></a>Ayrıntılar

Microsoft Mayıs 2021 ' den itibaren, Microsoft 'un fatura ayrıntılarını SKU açıklaması yerine ürün ayrıntısına göre görüntülemesi için CSP programındaki yeni ticaret PDF faturasına yönelik yeni bir biçim sunuyor. Bu yeni güncelleştirmeyle, her ürünü tek bir satırda görüntülerken, satır öğelerini ürün türüne göre toplamak için kullanılır.

İş ortakları, bu değişikliğin 1 Nisan 2021 ile 30 Nisan 2021 arasındaki fatura dönemi için faturalandırılmasına göre geçerli olduğunu fark eder. etkilenen teklifler Microsoft Azure ayrılmış örnek, azure abonelikleri (azure planı) ve market ' dir.

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

Microsoft iş ortağı web sitesinin [Işlem hazırlık kaynağı galerisinde](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) bu konuyla ilgili bilgileri gözden geçirin. Faturalandırma kaynakları, faturalar, CSP faturalandırma ve vergiler dahil faturalandırma ve vergi konuları hakkında daha fazla bilgi için Iş Ortağı Merkezi ' nde [faturalandırma bölümünü](../billing.md) ziyaret edin.

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a>Bulut Çözümü Sağlayıcısı (CSP) müşteri ekleme gereksinimlerinde yapılan değişiklikler

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

tüm iş ortakları Bulut Çözümü Sağlayıcısı (CSP) programı üzerinden deneyimidir

### <a name="details"></a>Ayrıntılar

Nisan 2021 [ürün başlatma takvimi](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) artık işlem hazırlık kaynağı galerisinde kullanılabilir. Yakında çıkacak ürünü görüntüleyin ve burada teklif edin.

### <a name="next-steps"></a>Sonraki adımlar

[Ürün başlatma takvimini](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)gözden geçirin ve bilgileri kuruluşunuzdaki uygun hissedarlarla paylaşabilirsiniz.  

### <a name="questions"></a>Sorularınız mı var?

bu teklifler hakkında daha fazla soru için ilgili Yammer topluluklarınızı kontrol edin.