---
title: Mart 2021 duyuruları
description: Yeni yetenekler, promosyonlar, teklifler, pazarlar veya mevcut tekliflerle ilgili değişiklikler dahil olmak üzere Microsoft Iş Ortağı Merkezi için Mart 2021 duyuruları.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 17b8082b8a42050892ff434010952d5f91a39431
ms.sourcegitcommit: 6c20c3cc4a226cada70c56df295966696affcec8
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/30/2021
ms.locfileid: "108328075"
---
# <a name="march-2021-announcements"></a>Mart 2021 duyuruları

Bu sayfada Mart 2021 için Microsoft Iş Ortağı Merkezi duyuruları sağlanmaktadır.

## <a name="readiness-changes-to-the-cloud-solution-provider-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="18"></a>Hazırlık: bulut çözümü sağlayıcısı (CSP), Haziran ayında canlı olacak şekilde, müşteri adresi doğrulama API 'SI ile yapılan değişiklikler; test özelliği artık kullanılabilir

### <a name="categories"></a>Kategoriler

- Tarih: 2021-04-30
- Hazır Olma

### <a name="summary"></a>Özet

İş ortakları ve müşterilerin işletmelerini temel alarak işlerini çalıştırmasına yardımcı olmak için iş ortaklarını, dünyanın her yerindeki tüm ülkeler için doğrulama adresi API 'sine test etmek üzere davet edeceğiz.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

CSP doğrudan fatura ortakları ve yeni yeni veya mevcut müşterileri güncelleştiren dolaylı sağlayıcılar adres ayrıntıları.

### <a name="details"></a>Ayrıntılar

Microsoft, güvende çalışır. CSP programındaki deneyimidir müşteri abonelikleri için uyumlu, güvenli ve güvenli bir müşteri adresi doğrulama yöntemi sağlamayı taahhüt ediyoruz. 31 Mart 2021 itibariyle, Haziran 2021 ' deki değişikliklerle çalışmaya başlamadan önce iş ortaklarını test etmek üzere davet ettiğimiz doğrulama adresi API 'sine yönelik değişiklikler sunuyoruz.

Değişiklikler yalnızca adresi doğrula API 'sini etkiler. Müşteri oluşturma ve faturalandırma profilini güncelleştirme API 'Leri etkilenmemektedir.

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

ABD Post kodları, 4 basamaklı bir ve daha fazla tire döndürür. Örneğin, 12345-6789.

Adres doğrulama API 'SI aracılığıyla doğrulama için bir adres gönderildikten sonra, aşağıdaki yanıt şeması döndürülür:

```csharp

// <summary>
/// Object represents the address validation response.
/// </summary>

public class AddressValidationResponse
{
   /// <summary>
   /// Gets or sets the original address
   /// </summary>
   /// <value>
   /// Original Address
   /// </value>
   public Address OriginalAddress { get; set; }

   /// <summary>
   /// Gets or sets the suggested addresses
   /// </summary>
   /// <value>
   /// Suggested Addresses
   /// </value>
   public List<Address> SuggestedAddresses { get; set; }

   /// <summary>
   /// Gets or sets the validation status
   /// </summary>
   /// <value>
   /// Status
   /// </value>
   public string Status { get; set; }

   /// <summary>
   /// Gets or sets the validation message
   /// </summary>
   /// <value>
   /// Validation Message
   /// </value>
   public string ValidationMessage { get; set; }
   ```

Bu örnek yanıta göz atın. ABD için, posta kodu için yalnızca beş basamak girerseniz, yanıt posta kodu satırı için dört basamaklı ek bir sonek döndürdüğüne göz önünde koyun.

```csharp

"suggested_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Microsoft Way",
              "postal_Code": "98052-8300"
},
"original_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Micro Way",
              "postal_Code": "98052"
},
"status":  "InteractionRequired",
"validation_message": "Address field invalid for property: ‘Street’"
}
```

### <a name="next-steps"></a>Sonraki adımlar

- Güncelleştirme için hazırlamaya başlayabilmeniz için, korumalı alan kiracı KIMLIĞINIZI, test uçuşna dahil edilecek konu uzmanı (Ali Haki) ile paylaşabilirsiniz.

- Bir denetim masası satıcısı (CPV) çözümü kullanıyorsanız, CPV 'nize başvurun.

### <a name="questions"></a>Sorularınız mı var?

Microsoft ile işlemlere yönelik desteğe ihtiyacınız varsa iş ortağı destek Yammer grubunuza ulaşın.

### <a name="change-log"></a>Değişiklik günlüğü:

- 31 Mart 2020: özgün yayın

- 30 Nisan 2021: örnek yanıt ve ZIP kodu ayrıntıları için güncelleştirmeler

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a>Yeni Exchange Yönetim Merkezi (EAC) deneyimi

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-29
- Özellikler

### <a name="summary"></a>Özet

27 Nisan 2021 ' den itibaren, Exchange Yönetim Merkezi (EAC), kullanıcılar için günlük verimliliği artıran yeni bir deneyim çıkarır.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

Iş Ortağı Merkezi aracılığıyla Exchange 'e erişen yönetici temsilcileri

### <a name="details"></a>Ayrıntılar

27 Nisan 2021 ' den itibaren, Iş Ortağı Merkezi aracılığıyla Exchange 'e gitten iş ortakları yeni EAC 'ya yönlendirilir.

Bu yeni deneyim Şu anda önizleme olarak sunulmaktadır ve Yöneticiler, klasik EAC içinde sağ üst köşedeki geçişi seçerek bu deneyimi etkinleştirebilir. Ayrıca, tüm sayfalarda görüntülenen "Şimdi deneyin" başlığını seçerek yeni duyak 'e gidebilir.

Yeni EAC 'nin avantajları şunlardır:

- Posta akışı ile ilgili sorunlar için Öngörüler, raporlar ve uyarı mekanizmaları eklendi. 

- Üretkenliği artırmak için kişiselleştirilmiş panolar.

Yeni deneyimin içinde gezinmenize yardımcı olmak için, yeni EAC deneyiminde **eğitim & Kılavuzu** bölümünde videolar bulunur. Bu, size yeni portalı en iyi şekilde nasıl kullanabileceğinizi gösteren bir genel bakış sunar.

>[!NOTE]
>Bu değişiklik ile klasik EAC deneyimi kullanım dışı olmayacaktır. Herhangi bir değişiklik uygulanmadan önce iyi bir bildirim alırsınız.

### <a name="next-steps"></a>Sonraki adımlar

- Yeni deneyimin ekran görüntülerini görüntüleyebileceğiniz [Bu konuyla ilgili kaynaklara](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/)göz atın.

- Bu bilgileri, kuruluşunuzdaki uygun paydaşlarla paylaşabilirsiniz. 

### <a name="questions"></a>Sorularınız mı var?

Bu değişiklikler hakkında herhangi bir soru için ilgili Yammer topluluklarınızı kontrol edin.

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a>Microsoft Işlemleri: ürün başlatma takvimini tanıtma

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-25
- Teklifler | Modern çalışma alanı

### <a name="summary"></a>Özet

İş ortağı geri bildirimlerine yanıt olarak, Microsoft Işlemleri ürün başlatma ile ilgili iletişimleri kolaylaştıracaktır.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

Bulut çözümü sağlayıcısı (CSP) iş ortakları

### <a name="details"></a>Ayrıntılar

Microsoft, iş ortağı deneyimlerini sürekli olarak geliştirmeye kararlıdır. Microsoft 'tan çok fazla iletişim aldığınızı ve ürün başlatma için tekrarlanan Duyurular dahil ettiğimiz hakkında geri bildirimde bulunduk.

Microsoft, geri bildiriminiz doğrultusunda, yeni ve mevcut tekliflerle ilgili ürün için hazırlık deneyimini kolaylaştırmıştır.

Artık, Işlem hazırlık kaynağı galerisinde yayınlanan ürünün tek bir aylık görünümünü sunuyoruz. Bu aylık [ürün başlatma takvimi görünümü](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) , işlem hazırlık kaynağı galerisindeki ve Iş Ortağı Merkezi bildirilerinde tek tek ürün başlatma iletişimlerinin yerini alır.

Bu [ürün başlatma takvimine](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) [topluluk koleksiyonları](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [Takvim görünümleri](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated)ve [CSP bültenleri](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)' nden de erişebilirsiniz. Her ayın ürün başlatma takvimini, Işlem hazırlık kaynağı galerisinde bir duyuru ile yayımladığımızda sizi bilgilendireceğiz.

Fiyat listesi önizlemesi ve fiyat listesi değişiklik günlüklerinde ve ürün bloglarında, lisanslama kılavuzlarında ve ürün pazarlama sayfalarında yeni ve mevcut tekliflerle ilgili bilgiler bulabilirsiniz.

Değişiklik, aşağıdaki ürünler için başlatılır.

- Dynamics şirket içi
- Microsoft 365
- Microsoft Dynamics 365
- Windows
- Sunucu  
- Araçlar
- Takımlar ve Telco

Işlem hazırlığı ayrıntıları gerektiren ürün başlatma için özel duyurular gönderilmeye devam edeceğiz.

### <a name="next-steps"></a>Sonraki adımlar

Bu konuyla ilgili kaynakları gözden geçirin ve bu bilgileri kuruluşunuzdaki uygun hissedarlarla paylaşabilirsiniz.

### <a name="questions"></a>Sorularınız mı var?

Bu teklifler hakkında daha fazla soru için ilgili Yammer topluluklarınızı kontrol edin.

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a>CSP müşteri ekleme gereksinimlerinde yapılan değişiklikler

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-25
- Özellikler

### <a name="summary"></a>Özet

İş ortakları ve müşterilerin işlerini güvenle çalıştırmasına yardımcı olma çabamız kapsamında, 25 Mart 2021 ' den itibaren geçerli olan ek müşteri bilgileri isteyeceğiz.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

Bulut çözümü sağlayıcısı (CSP) doğrudan fatura ortakları ve sonraki bölümde listelenen ülkelerde yeni veya mevcut müşterileri olan dolaylı sağlayıcılar

### <a name="details"></a>Ayrıntılar

Microsoft, güvende çalışır. CSP programında deneyimidir müşteri abonelikleri için uyumlu, güvenli ve güvenli bir müşteri doğrulama yöntemi sağlamayı taahhüt ediyoruz. 25 Mart 2021 ' de, aşağıdaki ölçütlerin her ikisini de karşılayan iş ortaklarını etkileyecek Iş Ortağı Merkezi API 'SI ve Kullanıcı arabirimi (UI) geliştirmeleri sunacağız:

1. İş ortağı Microsoft ile doğrudan faturalandırma ilişkisine sahiptir (Bu, ortağın doğrudan bir fatura ortağı veya dolaylı bir sağlayıcı olduğu anlamına gelir).

2. İş ortağı aşağıdaki ülkelerde yeni veya mevcut müşteriler ile iş yapar:

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

Ölçütlere uyan iş ortaklarının, yeni müşterileri eklerken veya mevcut müşteri ayrıntılarını değiştirirken müşterinin **Şirket kayıt kimliği** 'ni (müşterinin **kuruluş** adı olarak da bilinir) ve **telefon numarasını** göndermesi gerekir. Ayrıca bu iş ortakları müşteri için isteğe bağlı bir **ikinci ad** da girebilir.

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

Dünyanın geri kalanında müşterilere sahip olan iş ortakları 25 Mart 2021 ' de, müşteriler için isteğe bağlı ayrıntılar olarak **Şirket kayıt kimliği**, **telefon numarası** ve **Orta adı** girme olanağına sahip olur.

### <a name="next-steps"></a>Sonraki adımlar

- Daha ayrıntılı rehberlik için, [adanmış iş ortağı koleksiyonundaki](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) teknik belgeleri ve sık sorulan soruları gözden geçirin.

- Iş Ortağı Merkezi API 'sini ve Web kullanıcısı deneyimini kullanarak değişiklikleri içerecek şekilde hazırlayın. API/SDK 'lar test için kullanılabilir olacak.

- Yeni müşterileri eklerken veya mevcut müşteri ayrıntılarını değiştirirken ek verileri gönderdiğinizden emin olun.

- Bir denetim masası satıcısı (CPV) çözümü kullanıyorsanız, CPV 'nize başvurun.

### <a name="questions"></a>Sorularınız mı var?

Yasal tanımlayıcıyla (ıNN veya tın olarak da bilinir) ilgili sorularınız varsa vergi danışmanınıza veya yerel vergi ofisine başvurun. Microsoft, vergi konusunda önemli yönergeler sağlayamaz.

Microsoft ile işlemlerinde desteğe ihtiyacınız varsa, [bir hizmet isteği açın](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a>1 Mart 2021 ' de yapılan düzeltmeler kalıcı yazılım fiyat listesi

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-23
- Teklifler/Pazarlar

### <a name="impacted-audience"></a>Etkilenen hedef kitle

Bulut çözüm sağlayıcısı programında dolaylı sağlayıcılar ve doğrudan fatura ortakları deneyimidir kalıcı yazılım 

### <a name="details"></a>Ayrıntılar

1 Mart 2021 ' de gönderilen kalıcı yazılım için fiyat listesi, orada olmaması gereken pazarlara dahil değildir. Kalıcı yazılım fiyat listesi, düzeltmeler ile 17 Mart 2021 ' de güncelleştirildi. Bu düzeltmeler yalnızca için geçerlidir:

- Ürün KIMLIĞI: DF77X4D43RKT 
- Ürün adı: Microsoft 365 İş için Windows 10 Home-Pro yükseltmesi
- Kaldırılan veya desteklenmeyen pazarlar: AE, AF, AL, har, AO, BA, BB, BD, BH, BM, mılyar TL, BO, BR, BS, siyah beyaz, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, çn, d, IN,, KN, KZ, LB, , Nı, NP, OM, PA, PE, PH, PK, PR, INER, QA, RS, RU, RW, SG, SN, ZF, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YS, ZM, ZW

Bu değişiklikler yalnızca yukarıdaki ürün için geçerlidir. Diğer ürünlerin bir düzeltme yoktur. 

### <a name="next-steps-and-resources"></a>Sonraki adımlar ve kaynaklar

- Transact kalıcı yazılım kullanan iş ortakları en son kalıcı yazılım fiyat listesini indirmelidir.
- Ülkelerinden oluşan iki harfli kısaltmayı kolay bir şekilde eşlemek için [bölge ülke kodlarına](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) başvurun.
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> .NET Standard SDK sürümü (v 1.17.0)

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-23

- Özellikler
 
### <a name="impacted-audience"></a>Etkilenen hedef kitle

Iş ortağı merkezi .NET SDK 'sını kullanan CSP programına katılan doğrudan fatura ortakları ve dolaylı sağlayıcılar.

### <a name="details"></a>Ayrıntılar

23 2020 Mart itibariyle Iş ortakları, [Microsoftpartnercenter. NETSDK (NuGet Galerisi |) sürümünü indirmeye başlayabilir. Microsoft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), güncelleştirilmiş ortak Iş ortağı MERKEZI SDK [GitHub örnekleri](https://github.com/Microsoft/Partner-Center-DotNet-Samples)ile birlikte. Bu sürüm aşağıdaki yöntemlerin güncelleştirmelerini içerir:

#### <a name="audit-updated-new-operation-types"></a>Denetim güncelleştirildi: yeni işlem türleri

Müşterinin ne zaman onayladığı ve sonlandırıldığı hakkında bilinmesi için yeni [işlem türleri](https://docs.microsoft.com/partner-center/develop/auditing-resources) eklendi.

- DapAdminRelationshipApproved

- Dapadminrelationshipsonlandırılan

#### <a name="audit-updated-new-resource-and-operation-types"></a>Denetim güncelleştirildi: yeni kaynak ve işlem türleri

Müşteri dizin rolü senaryosunu desteklemek için yeni [kaynak ve işlem türleri](https://docs.microsoft.com/partner-center/develop/auditing-resources) eklendi.

- Yeni kaynak türü "CustomerDirectoryRole"

- "AddUserMember" ve "RemoveUserMember" işlem türleri

#### <a name="sdk-updates-to-customer-accounts"></a>Müşteri hesaplarına SDK güncelleştirmeleri

- GET/customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus desteği

- /Customers/{Customer-Tenant-ID}/nitelikler al

- /Customers/{customer_id}/nitelikler SONRASı? Code = {validationCode}

#### <a name="additional-changes"></a>Ek değişiklikler

Aşağıdaki değişiklikler yeni ticaret 'nin bir parçası olarak sunulmuştur ve şu anda yalnızca M365/D365 yeni ticaret deneyimi Technical Preview 'ın parçası olan iş ortakları tarafından kullanılabilir. Yeni ticaret Technical Preview kapsamında olmayan iş ortakları, etkileri fark etmez ve geriye dönük olarak uyumlu olmalıdır.

- Katalog değişiklikleri:

  - /Products/{product-id}/SKUs/{SKU-id} al

- Satın alın ve yönetin:
  - /Customers/{CustomerID}/abonelikleri al
  - /Customers/{CustomerID}/Subscriptions/{SubscriptionID} al
  - PATCH/Customers/{CustomerID}/Subscriptions/{SubscriptionID}
  - /Customers/{CustomerID}/Subscriptions/{SubscriptionID}/geçişli tioneligılıklara al
  - /Customers/{CustomerID}/Subscriptions/{SubscriptionID}/geçişlerini al
  - POST/Customers/{CustomerID}/Subscriptions/{SubscriptionID}/geçişlerin

### <a name="next-steps"></a>Sonraki Adımlar

- En son [Microsoftpartnercenter. NETSDK sürümünü indirin (NuGet Galerisi | Microsoft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)
- [GitHub örneklerini](https://github.com/Microsoft/Partner-Center-DotNet-Samples) indirme ve gözden geçirme

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a>Uygun teklifler için CSP ticari Market teklifi ve FY21 CSP teşvikleri

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-18
- Özellikler

### <a name="impacted-audience"></a>Etkilenen hedef kitle

Bulut çözüm sağlayıcısı programındaki dolaylı sağlayıcılar ve doğrudan fatura ortakları 

### <a name="details"></a>Ayrıntılar

Bulut çözümü sağlayıcısı programındaki dolaylı sağlayıcılar ve doğrudan fatura ortakları, üçüncü taraf teklifler satmanıza ve Iş ortağı merkezi veya Azure portal işlenen her bir uygun üçüncü taraf teklifi için bir indirim teşvik elde edebilir. Bu öneriler, uygun tekliflerle ilgili olarak faturalandırılan satış hakkında indirim biçiminde olacaktır ve **30 haziran 2021 ' ye kadar kullanılabilir**.  

Aşağıdaki CSP ticari marketi teklifi hakkında bilgi edinmeye devam edin ve müşterilerin devam ettirme başarısını ve dijital dönüşümünü etkinleştirmeye yönelik doğru teklifleri belirlemek için müşterilerinizle iletişim kurun.

En son IaaS ve SaaS çözümlerini Microsoft müşterilerine pazarlamak için bağımsız yazılım satıcıları (ISV 'Ler) ile iş ortaklıyoruz. ISV yayımcıları, Microsoft iş ortağı kanalı aracılığıyla tekliflerinden satışları etkinleştirme seçeneğine sahiptir. Özendiğimiz tekliflerimiz iki kategoride yer almalıdır:

- Azure IP ortak satış incentivized durumu ile SaaS ve IaaS üçüncü taraf tekliflerini seçin. 

- Ekipler ile tümleştirilmiş SaaS uygulamaları veya PowerPoint, Word, Excel, Outlook veya SharePoint gibi en az iki Microsoft 365 üretkenlik uygulaması.

### <a name="next-steps-and-resources"></a>Sonraki adımlar ve kaynaklar

- Uygun Market uygulamaları satmaya uygun olan uygulamaları teşvik etmek için [Iş ortağı teşvikleri](https://partner.microsoft.com/membership/partner-incentives) hakkında bilgi edinin. Yeni teklifler aylık olarak eklenir.  
- [Bulut çözümü sağlayıcısı doğrudan fatura ortağı özendirme kaynakları](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [Bulut çözümü sağlayıcısı dolaylı sağlayıcı, kaynakları teşvik edin](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- Ticari market uygulamalarını satma hakkında daha fazla bilgi edinmek için bu [sunuyu](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) gözden geçirin. Ek kaynaklara [buradan](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/)göz atın. 
- [Iş Ortağı Merkezi](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) veya [Azure Portal](https://ms.portal.azure.com/#home) ticari Market kataloğunu keşfet
- Uygulamaları şirketinizin marketi ile bütünleştirmek için [API 'leri](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) kullanma
- İş yaparken ilgilendiğiniz ISV 'lere ulaşın
- Dolaylı sağlayıcıların, hangi uygulamaların satmaya yönelik API 'Leri ve kılavuz satıcılarını kullanarak tümleştirmeleri gerekir

### <a name="questions"></a>Sorularınız mı var?  

Iş Ortağı Merkezi 'nde ticari Market 'e genel bakış için [Bu makaleye](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) başvurun.

Daha fazla yardıma ihtiyacınız varsa, Iş Ortağı Merkezi 'nde bir destek isteği oluşturabilirsiniz. Daha fazla bilgi edinin [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a>Power BI Premium teklif adlandırma ve önkoşul güncelleştirme

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-18
- Özellikler

### <a name="summary"></a>Özet

1 Nisan 2021 son fiyat listesi, Kullanıcı başına Power BI Premium için adlandırma ve/veya önkoşul bilgilerine açıklık eklemek üzere güncelleştirilir.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

Bulut çözümü sağlayıcısı (CSP) doğrudan ve dolaylı iş ortakları

### <a name="details"></a>Ayrıntılar

1 Nisan 2021 son fiyat listesi, Kullanıcı başına Power BI Premium için adlandırma ve/veya önkoşul bilgilerine açıklık eklemek üzere güncelleştirilir.

Son fiyat listesi güncelleştirilene kadar, bu bölümdeki bilgileri kullanarak doğru ürünün düzenli olduğundan emin olun.

Aşağıdaki ayrıntılar etkilenen SKU ve önkoşul ayrıntılarını göstermektedir.

| 1 Mart 'ta bir görünen ad teklif listesi önizlemesi |  1 Nisan 'ın son fiyat listesindeki teklif görünen adı güncelleştirildi| Teklif Kimliği |
| ------ | ----------- | ----------- |
| Kullanıcı başına Power BI Premium Add-On (kar amacı gütmeyen personel fiyatlandırması)  |  Kullanıcı başına Power BI Premium Add-On **(Office)** (kar amacı gütmeyen personel fiyatlandırması)   | 31c03289-47AB-4AB0-8df1-03742c127ac6   |

Müşterilerin bu teklifi satın almak için aşağıdaki önkoşulların herhangi birine sahip olması gerekir:

| Teklif görünen adı | Teklif Kimliği |
| ------ | ----------- |
| Microsoft 365 E5 (kar amacı gütmeyen personel fiyatlandırması)  |  31bedf01-9e57-4ece-a53a-d3656a563931   |
|   Ses konferansı olmadan E5 Microsoft 365 (kar amacı gütmeyen personel fiyatlandırması)|  b456810a-c414-4e07-98fc-ef74e8175a09|
|   Office 365 E5 (kar amacı gütmeyen personel fiyatlandırması)| ce139fe5-8bd5-47ED-a5be-07c286f8b9e    |
|   Office 365 E5 (kar amacı gütmeyen personel fiyatlandırma) denemesi|  2f192efe-608a-4C9C-9d19-2b0b70b0962e|
|   Office 365 E5 ses konferansı olmadan (kar amacı gütmeyen personel fiyatlandırması)|  c3897426-9f49-4eaf-9b4d-7d9a1c72aef7|

Aşağıdaki Power BI Premium teklifi satın alma için gereken bir önkoşula sahiptir:

| Teklif görünen adı | Teklif Kimliği |
| ------ | ----------- |
|   Kullanıcı başına Power BI Premium Add-On (kar amacı gütmeyen personel fiyatlandırması)|  ef0b895b-681b-4026-a5b1-dda182a57d40 |

Müşterilerin bu teklifi satın alması için bu önkoşulu olması gerekir:

| Teklif görünen adı | Teklif Kimliği |
| ------ |----------|
| Power BI Pro (kar amacı gütmeyen personel fiyatlandırması)  |   cabdfc93-5786-4224-bfd3-35d58f833b35 |

### <a name="next-steps"></a>Sonraki adımlar

Bu konuyla ilgili kaynakları gözden geçirin ve bu bilgileri kuruluşunuzdaki uygun hissedarlarla paylaşabilirsiniz.  

### <a name="questions"></a>Sorularınız mı var?

Bu tekliflerle ilgili herhangi bir soru için ilgili Yammer topluluklarınızı kontrol edin. 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> Microsoft 365 F3 için Mart fiyat güncelleştirmeleri

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-16
- Teklifler/Pazarlar

### <a name="summary"></a>Özet

Microsoft 365 F3 Ingiliz Sterlini (GBP) ve Euro (EUR) için yanlış Mart 2021 fiyatlandırması düzeltildi.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

İş ortakları, 1 Mart 'ta Microsoft 365 F3 veya bulut çözümü sağlayıcısı (CSP) programı aracılığıyla 1 Mart 2021 arasında bir EUR Satın alma.

### <a name="details"></a>Ayrıntılar

Microsoft, Microsoft 365 F3 için yanlış fiyatlandırmayı çözümledi. Yanlış fiyatlar GBP ve EUR için ve yalnızca 1 Mart, 17 Mart 2021 arasında satın alınan tekliflere yöneliktir. Etkilenen teklifler ve para birimleri aşağıda listelenmiştir. 

| Teklif adı | Para Birimi | Teklif Kimliği | Malzeme KIMLIĞI |
| ------ |----------- |----------- |----------- |
| Microsoft 365 F3 (Hayır) | GBP | 57b722c2-c435-4bfb-9bc8-80509213a13a | AAD-11626 |
| Microsoft 365 F3 (ticari) | EUR| 3451a3b0-8cdav-44a7-bad7-c30be81c4aaa | AAA-89898 |
 
Mart ve Nisan Preview lisansı-temel fiyat listeleri, 16 Mart 5PM Pasifik standart saati ile güncelleştirildi.

### <a name="next-steps"></a>Sonraki adımlar

- İş ortakları, her ikisi de Mart ve Nisan önizlemesi olmak üzere geçerli lisans tabanlı fiyat listelerini, varsa bu fiyat düzeltmelerini yeniden indirmelidir.  
- Microsoft, etkilenen işlemleri düzeltme ile ilgili sonraki adımlar hakkında bilgi almak için, önümüzdeki haftalarda, gelecek haftalarda bulunan iş ortakları ile iletişim kuracaktır.

### <a name="questions"></a>Sorularınız mı var?

Diğer sorular için lütfen ilgili CSP Yammer topluluklarınızı denetleyin.

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> Iş Ortağı Merkezi aracılığıyla yasal şirket adını güncelleştirme

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-16
- Sürücü verimliliği & ölçeği

### <a name="summary"></a>Özet

2021 Mart 'tan başlayarak, Microsoft İş Ortağı Ağı (MPN) iş ortakları ve bulut çözümü sağlayıcısı (CSP) dolaylı satıcıları, Iş Ortağı Merkezi aracılığıyla yasal şirket adlarını güncelleştirebilir.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

MPN iş ortakları ve CSP dolaylı satıcıları (CSP doğrudan fatura ortakları için geçerli değildir)

### <a name="details"></a>Ayrıntılar

2021 Mart 'tan itibaren, MPN iş ortakları ve CSP dolaylı satıcıları, Iş Ortağı Merkezi aracılığıyla uyumlu ve kendi kendine bir şekilde yasal şirket adını güncelleştirebilir. Bu yeni özellik sayesinde, iş ortaklarının şirket adlarını güncelleştirmek için Iş ortağı merkezi destek bileti göndermesi artık gerekmez. Bu işlem, bu etkinlikleri gerçekleştirirken iş ortakları için önemli miktarda zaman kazandırır. 

Daha fazla bilgi için bkz. [yasal iş profilinizi güncelleştirme](../update-your-partner-profile.md#update-your-legal-business-profile).

>[!NOTE]
>Yasal iş profilinizde bulunan şirket adının yazım hatası ve kısaltmalarının olmadığından ve resmi şirket iş kaydı kayıtlarınızda tam olarak eşleştiğinden emin olun. Kuruluş profilinizi güncelleştirme hakkında daha fazla bilgi için bkz. [kuruluş profilinizi doğrulama](../update-your-partner-profile.md#update-your-legal-business-profile).

### <a name="next-steps"></a>Sonraki adımlar

Uygun ekibin süreçlerini gözden geçirebilmesi ve güncelleştirebilmesi için bu bilgileri kuruluşunuz dahilinde paylaşabilirsiniz.

### <a name="questions"></a>Sorularınız mı var?

Diğer sorular için lütfen ilgili CSP Yammer topluluklarınızı denetleyin.

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> Bulut çözümü sağlayıcısı (CSP) program evrimi ve açık lisans programı değişikliklerinde Güncelleştir

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-15
- Özellikler

### <a name="summary"></a>Özet

Yeni ticari ve kamu sektörü kalıcı yazılım teklifleri, açık lisanslama programındaki değişikliklerle birlikte bulut çözümü sağlayıcısı (CSP) programına geliyor.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

Açık lisans programı ile satılan ticari dağıtımcılar ve yönetilen satıcılar ve tüm CSP iş ortakları deneyimidir kalıcı yazılım

### <a name="details"></a>Ayrıntılar

Microsoft, Eylül 2020 ' de, iş ortakları için şirket içi yazılımın kullanılabilirliği de dahil olmak üzere, CSP programındaki iş ortaklarına yönelik fırsatları genişletmek için dijital dönüşümde yolculukta bir dizi adım [duyurmuştur](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) . Bu değişiklikler, iş ortaklarının, CSP 'deki yazılım lisanslarını kullanarak işlerini büyütmesine ve bunların erişimini genişletmesine imkan tanır. Ayrıca, müşterilerin buluta geçişini güçlendirin ve iş ortaklarına müşteri hibrit bulut ortamları için gereken esnekliği sunar.

Bu dijital dönüşüme devam eden aşağıdaki değişiklikleri duyuruyoruz:

- 1 Temmuz 2021: açık lisans programı fiyat listesine yeni SKU 'Lar, ürünler veya promosyonlar eklenmeyecektir.

- 7 Temmuz 2021: Iki ticari teklif, orijinal Windows ve Visual Studio Professional edinme ve kamu sektörü teklifleri (kamu, eğitim ve kar amacı: [duyuru](./2020-december.md#9)), CSP kalıcı yazılım fiyat listesine eklenecektir.  Fiyat listesi, Iş Ortağı Merkezi 'nde [satış > fiyatlandırma & teklifleri](https://partnercenter.microsoft.com/pcv/sales) sayfasının yazılımlar bölümünde bulunabilir ve bu tarihte yeniden yayımlanmak üzere olur.

CSP program evrimi ve açık lisans programı değişiklikleriyle ilgili tüm ayrıntılar için lütfen aşağıdaki **sonraki adımlara** bakın.

### <a name="next-steps"></a>Sonraki Adımlar:

- CSP program evrimi: [bulut çözümü sağlayıcısı program](https://partner.microsoft.com/resources/collection/software-in-csp#/) hazırlık malzemelerinden kalıcı yazılımı gözden geçirin. Rolünüzün doğru bilgilerini hızlı bir şekilde bulmak için bu [hazırlık haritasını](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) kullanın.

- Lisans programı değişikliklerini aç: [CSP program evrimini gözden geçirin ve açık lisans programı değişiklikleri](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) hazırlık malzemelerini inceleyin. Rolünüzün doğru bilgilerini hızlı bir şekilde bulmak için bu [hazırlık haritasını](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) kullanın.

### <a name="questions"></a>Sorular

Diğer sorular için lütfen ilgili CSP Yammer topluluklarınızı denetleyin.

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a>Önceki bir duyuruya güncelleştirme: Premium değerlendirmeler, uyumluluk Yöneticisi eklentisi

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-15
- İşlerinizi büyütme

### <a name="summary"></a>Özet

Deneme teklifleri fiyat listesinde listelenmemelidir ve kaldırılacak.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

Bulut çözüm sağlayıcısı aracılığıyla iş ortakları deneyimidir

### <a name="details"></a>Ayrıntılar

Deneme teklifleri fiyat listesine dahil edilmemelidir. Bunlar 1 Mayıs 2021 fiyat listesinden kaldırılacak.

Özgün duyuru [burada](./2021-february.md#4)bulunur.

### <a name="additional-resources"></a>Ek kaynaklar

- [Microsoft 365 E5 güvenlik ve uyumluluk](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [Microsoft Uyumluluk Yöneticisi-Microsoft 365 uyumluluğu 'nda değerlendirme oluşturma ve yönetme](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a>Sonraki adımlar

Bu konuyla ilgili kaynakları gözden geçirin ve bu bilgileri kuruluşunuzdaki uygun hissedarlarla paylaşabilirsiniz.

### <a name="questions"></a>Sorularınız mı var?

Bu tekliflerle ilgili sorular için ilgili Yammer topluluklarınızı kontrol edin.

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> Çözümlerinizi bir ticari Iş ortağından (OCP) Microsoft ticari Market 'e (GTM) taşıma

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-12
- Özellikler

### <a name="summary"></a>Özet

29 Mart 2021 ' den itibaren, sınırlı bir ticari Iş ortağı (OCP) go-to market (GTM) özelliği ile karşılaşırsınız. Çözümlerinizi Iş Ortağı Merkezi ' nde ticari Market 'e geçirmenizi öneririz.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

OCP GTM 'de çözümlerle ortak satış kurumları

### <a name="details"></a>Ayrıntılar

Aralık 2020 ' de, Microsoft OCP GTM aracından gelen yolculuğumuzu Iş Ortağı Merkezi 'nde Microsoft Commercial Market 'e başladık. Bu geçiş ticari Market 'in yeteneklerini genişleterek, çözümlerinizi milyonlarca müşteriye göre sergilemenize, diğer Microsoft ve iş ortağı satıcılarıyla fırsatları daha da paylaşabilir ve yenilikçi çözümleri ortaklaşa satabilirsiniz.

Geçişin sonraki kilometre taşı, 29 Mart 2021 ' de gerçekleşmeyecektir. Diğer bir deyişle, bazı alanlar salt okunurdur, sınırlı OCP GTM özelliklerine karşılaşmak için başlarsınız. Şu anda OCP GTM 'deki çözümlerle ortak satıyorsanız, kendi özelliklerinden faydalanmak ve yayımlama deneyiminizi basitleştirmek için çözümlerinizi ticari Market 'e geçirmenizi öneririz. 

Ticari Market 'e geçiş yapmak Iş Ortağı Merkezi 'ni ortak satış yayımlama deneyiminin birincil hedefine getirir. Çözümlerinizi, Microsoft ürünleri için kullandığımız aynı kanallar ve ürün içi deneyimler aracılığıyla paylaşılan müşterilerimiz ile bağlayarak işinizi büyütmeye devam edebilirsiniz. [Ticari Market hakkında daha fazla bilgi edinin](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).

### <a name="next-steps"></a>Sonraki adımlar

- Çözümlerinizi henüz taşıdıysanız, geçiş [kılavuzunda](/azure/marketplace/co-sell-solution-migration) açıklanan yönergeleri izleyin veya tüm geçiş etkinliklerini tamamlayıp, ticari markette çözümünüzü yayımlamaya başlamak için [adım adım video öğreticisini](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) görüntüleyin.

- OCP GTM 'deki sınırlı yetenek deneyimiyle ilgili sorularınız için, [Microsoft ticari Market SSS 'de yayımlanacak ortak satış gereksinimlerini](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf)görüntüleyin. (29 Mart 2021 ' i Başlatan "OCP GTM Limited yetenekler" bölümüne bakın.)

### <a name="questions"></a>Sorularınız mı var?

Sorularınız varsa veya daha fazla bilgiye ihtiyacınız varsa [desteğe](https://partner.microsoft.com/support/?stage=1) başvurun.

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a>Azure için bulut çözümü sağlayıcısı (CSP) programında yeni ticaret deneyimini Rusya 'ya genişletme

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-10
- Özellikler

### <a name="impacted-audience"></a>Etkilenen hedef kitle

Rusya 'daki tüm iş ortakları bulut çözümü sağlayıcısı (CSP) programı üzerinden deneyimidir.

### <a name="details"></a>Ayrıntılar

10 2021 Mart 'tan itibaren, **Rusya 'Da Azure IÇIN CSP 'de yeni ticaret deneyiminin** kullanılabilirliğini duyurmaktan mutluluk duyuyoruz. Bu deneyim, müşterilerin Azure hizmetlerini satın alıp tüketme yöntemini kolaylaştırır ve geliştirir. Ayrıca, CSP programındaki iş ortaklarına satış momalları genelinde Azure fiyatlandırması için tutarlı bir görünüm, genel tutarlılık için ABD Doları fiyatlandırması, faturalandırma tarihi hizalaması ve Azure maliyet yönetimine erişim hakkı verecektir.

### <a name="next-steps"></a>Sonraki adımlar

Yeni Azure ticari deneyimine giriş ve ek bilgi sağlama gibi birkaç kaynak mevcuttur. [CSP program güncelleştirmeleri kaynak galerisinde](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/)en son SSS, Decks, video ve daha fazlasını bulun.

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a>İş Ortağı Merkezi Yazılım lisans anahtarı ve indirme karşılama

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-04
- Özellikler

### <a name="summary"></a>Özet

Iş Ortağı Merkezi yazılım indirme ve lisans anahtarı karşılama özelliği yeniden belirtilmiştir.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

Tüm bulut çözümü sağlayıcısı (CSP) iş ortakları, kalıcı ve sunucu aboneliği yazılım siparişlerinin Iş Ortağı Merkezi aracılığıyla deneyimidir

### <a name="details"></a>Ayrıntılar

İş ortağı geri bildirimlerine yanıt olarak, kalıcı ve sunucu aboneliği yazılım siparişleri için yazılım ve lisans anahtarları almak üzere Iş Ortağı Merkezi 'ni karşılama özelliğini sunuyoruz. 19 Ocak 2021 ' de kaldırılmadan önce önceki durumuna geri yüklenecek. ( [Duyuruya](2020-september.md#17)bakın.)

Yazılım lisans anahtarlarının ve indirme bağlantılarının, fikri mülkiyet varlıklarından sonra değerli ve yüksek oranda aranan olduğunu unutmayın. Sızmış ise, etkinleştirme sınırlarının tükenmesine ve olumsuz bir müşteri ve iş ortağı deneyimine neden olabilir.

### <a name="next-steps"></a>Sonraki adımlar

Kullanım yönergeleri ve yazılım anahtarı dağıtımı hakkında önemli yönergeler için aşağıdaki kaynakları gözden geçirin:

- [CSP programı aracılığıyla şirket içi yazılım satma](../csp-on-premise-software.md)
- [Iş Ortağı Merkezi yeni ticaret Işlemleri Kılavuzu](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) ( **yazılım anahtarı dağıtımı hakkında rehberlik** bölümüne bakın.)

### <a name="questions"></a>Sorularınız mı var?

Bu bildirimde ilgili başka sorularınız varsa ilgili Yammer topluluklarınızı kontrol edin.

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a>Iş ortağı satış bağlantısı (PSC) üzerinden Iş Ortağı Merkezi 'ne anlaşmalar geçirin

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-04
- Özellikler

### <a name="summary"></a>Özet

İş ortağı satış bağlantısı (PSC), 31 Mart 2021 ' den itibaren salt okunurdur. bu nedenle, PSC 'lerden Iş ortağı merkezine geçişlerinizi geçirmeye başlamanızı başlıyoruz.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

PSC 'de anlaşmalar olan iş ortakları

### <a name="details"></a>Ayrıntılar

Paylaşılan büyüme taahhüdünün bir parçası olarak **Microsoft ile ortak satış** , keşfedilmesi için kullanabileceğiniz yoldur **, uzmanlığınızı sunun ve olumlu müşteri sonuçları için müşteri parmak izini genişletmenizi** sağlar. Normalden **3,5 kat daha hızlı** bir ortalama Işlem olan Iş Ortağı Merkezi 'nde ortak satış deneyiminizi yönetmek, doğrudan müşteri, iş ortağı ve Microsoft satıcı kanallarından satış yapmanıza ve tüm başvuru işlem hattınızı tek bir konumda yönetmenize olanak sağlar.

**PSC** , **31 Mart 2021**' den itibaren **salt okuma erişimine** geçer, bu nedenle iş ortağı merkezi 'ne taşıma ve bu özellik geliştirmelerini erişme hakkında bilgi alırız: 

- Microsoft ile paylaştığınız anlaşmalar, ihtiyacınız olan yardım türüne göre doğru satıcı için **daha doğru bir şekilde yönlendirilmenizi** sağlar.
- Mücadele için uygun çözümler ve ISV Connect program ölçütlerini karşılamak için, onay işlemini ve nihai yürütme (POE) kanıtlamayı basitleştirecek olan **ön ödemeli uygunluk doğrulaması** .
- Tüm ortak satış fırsatlarınızı ve satış nitelikli müşteri adaylarını tek bir yerde yönetmek için **sorunsuz Kullanıcı deneyimi** .

Ayrıca, taşınmasında yardımcı olması için Iş Ortağı Merkezi 'nde yeni özellikler ekledik:

- [Ortak satış fırsatları için toplu işlemler](../bulk-operations.md)
- [Geçiş özelliğini dağıt](../psc-to-pc.md) ( **PSC anlaşmalar geçiş** bölümüne bakın.)

Iş Ortağı Merkezi 'nde ortak satış deneyimini kullanarak, satış ekipleriniz, bu müşteri adaylarına ve fırsatlara odaklanmak, anlaşmaları kapatmak ve müşteri ilişkileri oluşturmak için daha fazla zaman alır.

### <a name="next-steps"></a>Sonraki adımlar

Iş Ortağı Merkezi [geçiş kılavuzunu](../psc-to-pc.md) kullanarak, PSC 'Lerden Iş ortağı merkezine anlaşmalar geçirme adımlarında size yol gösterir.

### <a name="questions"></a>Sorularınız mı var?

Daha fazla soru için [desteğe](https://partner.microsoft.com/support/?stage=1)başvurun.

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a>Yeni Microsoft Dynamics 365 ürünleri ve 1 Nisan 2021 ' de sunulan teklifler

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-04
- Özellikler

### <a name="summary"></a>Özet

Microsoft, 1 Nisan 2021 ' de, bulut çözümü sağlayıcısı (CSP) programı için birkaç yeni ürün ve teklif başlatacaktır.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

Tüm iş ortakları bulut çözümü sağlayıcısı (CSP) programı üzerinden deneyimidir

### <a name="details"></a>Ayrıntılar

Microsoft, 1 Nisan 2021 ' de aşağıdaki yeni ürünleri ve şunları sunuyor:

- Kullanıcı başına Power BI Premium
- Müşteri ses ve pazarlama USL coğrafi ve segment genişletme

**Kullanıcı başına Power BI Premium**

Microsoft, ilk Kullanıcı başına Power BI Premium tekliflerini tanıtacaktır. Power BI Premium Şu anda yalnızca bir kapasite yapısında satılabilir. Kullanıcı başına Power BI Premium kurumsal iş zekası (BI) ve analiz özelliklerine erişim sağlar. Esnek bireysel bilgisayar lisanslama, küçük ve orta ölçekli işletmeler için.

Bu teklif hakkında daha fazla bilgi edinmek için [Power BI sürüm ayrıntılarını](/power-platform-release-plan/2020wave2/power-bi/planned-features) gözden geçirin.


**Teklif Ayrıntıları**

Teklif adının fiyat listesi önizlemeden biraz farklı olduğunu unutmayın.

| Teklif adı | Teklif Kimliği |
| ------ |----------- |
| Kullanıcı başına Power BI Premium | 9c810018-9356-4903-95ab-eeb956289290 | 
| Fakülteler için Kullanıcı başına Power BI Premium | 3afc44f-f372-4ad5-8657-aadd9574fce0 | 
| Öğrenciler için Kullanıcı başına Power BI Premium | 657eea87-d0b0-4c89-8c8e-9b04395bd940 | 
| Kullanıcı başına Power BI Premium (kar personeli olmayan personel fiyatlandırması) | 7a0a856c-059f-45dd-9d26-ae27992e706a | 
| Kullanıcı başına Power BI Premium Add-On | 244ff87e-5925-44a0-BF31-gizlenir 189719b58 | 
| Fakülteler için Kullanıcı başına Power BI Premium Add-On | 5dad849bd-b8f7-4340-b4f4-3a9eaeb8987e | 
| Öğrenciler için Kullanıcı başına Add-On Power BI Premium | cf62d70d-5af5-422a-bda8-97936402ac8e | 
| Kullanıcı başına Power BI Premium Add-On (kar amacı gütmeyen personel fiyatlandırması) | 31c03289-47AB-4AB0-8df1-03742c127ac6 | 

**Müşteri ses ve pazarlama USL coğrafi ve segment genişletme**

Aralık 2020 başlatmaya yönelik bir izleme olarak Dynamics 365 müşteri Voice ve Marketing USL teklifleri, yeni ülkeler ve daha fazla kar ve eğitim SKU 'Ları eklemek üzere değiştirilmiştir.

| Teklif adı | Teklif Kimliği |
| ------ |----------- |
| Dynamics 365 müşteri sesi USL (kar amacı gütmeyen personel fiyatlandırması) | 7a8642a5-481e-4906-a642-b56dbeeb62a0 |
| Fakülteler için Dynamics 365 müşteri sesi USL | 85162d70-9676-4CF6-A4BC-a0d6672f2657 |

Bu teklifler hakkında daha fazla bilgi edinmek için aşağıdaki sayfaları ziyaret edin:

- [Dynamics 365 müşteri hizmeti sesli giriş sayfası](https://dynamics.microsoft.com/customer-voice/overview/)
- [Dynamics 365 pazarlama ana sayfası](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a>Sonraki adımlar

Bu konudaki kaynakları gözden geçirin ve bu bilgileri kuruluşunuzdaki uygun hissedarlarla paylaşabilirsiniz.  

### <a name="questions"></a>Sorularınız mı var?

Bu tekliflerle ilgili herhangi bir soru için ilgili Yammer topluluklarınızı kontrol edin. 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> Microsoft Evrensel Yazdırma artık bazı paketlerde kullanılabilir

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-33
- Özellikler

### <a name="summary"></a>Özet

Microsoft Evrensel Yazdırma, 1 Mart 2021 ' den bağımsız bir eklenti olarak, select Microsoft 365 paketleri ve tek başına eklenti olarak Transact tarafından kullanılabilir.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

Tüm iş ortakları bulut çözümü sağlayıcısı (CSP) programı üzerinden deneyimidir

### <a name="details"></a>Ayrıntılar

[Evrensel Yazdırma](https://aka.ms/universalprint) , şirket içi yazdırma sunucuları gereksinimini ortadan kaldıran ve Windows cihazlarının Azure 'a kayıtlı yazıcılara yazdırmasını sağlayan bir Microsoft 365 yazdırma hizmetidir. Bu, 1 Mart 2021 ' den itibaren Transact tarafından kullanılabilir olacaktır.

Çalışanlar, daha az yazdırma, kolay konum tabanlı yazıcı bulma ve öğrenme eğrisi olmadan sezgisel bir yazdırma deneyiminden yararlanır. Azure Active Directory (Azure AD) 'ye katılmış olan cihazlar, güvenli bir şekilde yazdırmak için mevcut Azure AD kimlik bilgilerini kullanır. Yöneticiler, Azure portal kullanarak yazdırmayı yönetir ve Evrensel Yazdırma için yerel destekle kolayca yazıcılara bağlanabilir. Evrensel Yazdırma, Evrensel Yazdırma Bağlayıcısı yazılımı kullanılarak uyumlu olmayan yazıcılarla dağıtılabilir.

Evrensel Yazdırma, Windows E3, a3, E5 ve A5, ve Microsoft 365 BP, F3, E3, a3, E5 ve a5 ' a başlayacak şekilde geri doldurulacak.  

**Teklif Ayrıntıları**

Teklif adının fiyat listesi önizlemeden biraz farklı olduğunu unutmayın.

| Teklif adı | Teklif Kimliği | Malzeme KIMLIĞI |
| ------ |----------- |----------- |  
| Evrensel yazdırma birimi eklentisi (500 iş)-Microsoft 365  | cb131356-45ee-4ae2-8537-873b706c8e75     | 9 Bı-00004   |
| Fakülteler için Evrensel yazdırma birimi eklentisi (500 işleri)-Microsoft 365   | 477bee81-9872-43d6-91d3-c72390bfcf49   | 9BK-00004   |
| Evrensel yazdırma birimi eklentisi (500 iş)-Windows    | d3ddc493-5741-4e0d-a02d-07edbb0bb72e   | 9 Bı-00002   |
| Fakülte için Evrensel yazdırma birimi eklentisi (500 işleri)-Windows   |  d0862f05-80f5-4fd4-8432-fe72dd893cc7  | 9BK-00002   |

### <a name="next-steps"></a>Sonraki adımlar

Fiyat listesi ve [evrensel yazdırmaya genel bakış hakkında bilgi](/universal-print/fundamentals/universal-print-whatis)edinin. Bu bilgileri kuruluşunuzdaki ilgili tüm kişilerle paylaşabilirsiniz.

### <a name="questions"></a>Sorularınız mı var?

Bu tekliflerle ilgili herhangi bir soru için ilgili Yammer topluluklarınızı kontrol edin.
