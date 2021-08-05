---
title: Mart 2021 duyuruları
description: Yeni özellikler, promosyonlar, teklifler, pazarlar İş Ortağı Merkezi mevcut tekliflerde yapılan değişiklikler dahil olmak üzere Microsoft İş Ortağı Merkezi için Mart 2021 duyuruları.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-announcements
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: d03bbc6c48f7048dd111a7b83210d11c5c266977
ms.sourcegitcommit: 90bf27df911b428b1222f483c32ba6367870e7c5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/04/2021
ms.locfileid: "115100421"
---
# <a name="march-2021-announcements"></a>Mart 2021 duyuruları

Bu sayfa, Mart 2021 için Microsoft İş Ortağı Merkezi duyurularını sağlar.

## <a name="readiness-changes-to-the-cloud-solution-provider-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="19"></a>Hazır olma: Bulut Çözümü Sağlayıcısı (CSP) müşteri adresi doğrulama API'sinde yapılan değişiklikler Haziran ayında yayınlanacak; test özelliği artık kullanılabilir

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-30
- Hazır Olma

### <a name="summary"></a>Özet

İş ortaklarının ve müşterilerin işletmelerini güvene dayalı olarak çalıştırmalarına yardımcı olmak için, iş ortaklarını dünya genelindeki tüm ülkeler için Adresi Doğrula API'lerinde yapılan değişiklikleri test etmeye davet ediyoruz.

### <a name="impacted-audience"></a>Etkilene hedef kitle

CsP doğrudan fatura iş ortakları ve mevcut müşterilerin adres ayrıntılarını yeni veya güncelleştiren dolaylı sağlayıcılar.

### <a name="details"></a>Ayrıntılar

Microsoft güven üzerinde çalışır. CSP programında müşteri aboneliklerinin işlemesi için uyumlu, güvenli ve güvenli bir müşteri adresi doğrulama yöntemi sağlama konusunda kararlıyız. 31 Mart 2021'den baş olarak, Haziran 2021'de yapılan değişikliklerle birlikte canlı yayına devam etmek için iş ortaklarını test etmek için davet edilen Adresi Doğrula API'sinde değişikliklerini açıkladık.

Değişiklikler yalnızca Adresi Doğrula API'sini etkiler. Müşteri Oluşturma ve Faturalama Profili API'lerini güncelleştirme işlemi etkilenmez.

Yanıt aşağıdaki durum iletilerinden birini geri dönecektir:

| Durum     | Açıklama |    Döndürülen önerilen adres sayısı |
|-------|---------------|-------------------|
|Doğrulanmış gönderilebilir | Adres doğrulanır ve adresine gönderebilirsiniz. | Tek |
|Doğrulandı | Adres doğrulandı. | Tek |
|Etkileşim gerekiyor | Önerilen adres önemli ölçüde değiştirildi ve kullanıcı onayı gerekiyor. | Tek |
|Sokak kısmii | Adreste verilen sokak kısmidir ve daha fazla bilgiye ihtiyaç vardır. | Çoklu— en fazla üç |
|Kısmi şirket içi | Verilen şirket (bina numarası, paket numarası ve diğerleri) kısmidir ve daha fazla bilgiye ihtiyaç vardır. | Çoklu— en fazla üç |
|Birden çok | Adreste kısmi olan birden çok alan vardır (kısmi sokak ve kısmi şirket de dahil olmak üzere). | Çoklu— en fazla üç |
|Hiçbiri | Adres yanlış. | Hiçbiri |
|Doğrulanmamış | Adres doğrulama işlemi aracılığıyla gönderileemedi. | Hiçbiri |

ABD posta kodları ek 4 rakam + kısa çizgi (örneğin, 12345-6789) dönüşecek.

Adresi Doğrulama API'si aracılığıyla doğrulama için bir adres gönderildikten sonra aşağıdaki yanıt şeması döndürülür:

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

Bu örnek yanıta göz at. Posta kodu için yalnızca beş basamak girersiniz, ABD için yanıt posta kodu satırı için dört basamaklı ek bir sonek daha dönecektir.

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

- Güncelleştirme için hazırlanmaya başlayabilirsiniz. Bu nedenle, korumalı alan kiracı kimliğinizi test uçuşuna dahil edilecek konu uzmanı (AliSinki) ile paylaşın.

- Denetim masası satıcısı (CPV) çözümü kullanıyorsanız CPV'nize başvurun.

### <a name="questions"></a>Sorularınız mı var?

Microsoft ile olan işlemleriniz için de destek gerekirse, iş ortağı destek grubuyla Yammer olun.

### <a name="change-log"></a>Değişiklik günlüğü:

- 31 Mart 2020: Özgün yayın

- 30 Nisan 2021: Örnek yanıt ve Posta kodu ayrıntıları için güncelleştirmeler

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="18"></a>Yeni Exchange yönetim merkezi (EAC) deneyimi

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-29
- Özellikler

### <a name="summary"></a>Özet

27 Nisan 2021'den başlayarak Exchange yönetim merkezi (EAC) kullanıcılar için günlük verimliliği geliştirecek yeni bir deneyim sunuyor.

### <a name="impacted-audience"></a>Etkilene hedef kitle

Exchange üzerinden İş Ortağı Merkezi

### <a name="details"></a>Ayrıntılar

27 Nisan 2021'den başlayarak, Exchange aracılığıyla İş Ortağı Merkezi iş ortakları yeni EAC'ye yeniden yönlendirecek.

Bu yeni deneyim şu anda önizleme olarak sunulmaktadır ve yöneticiler klasik EAC'nin sağ üst köşesindeki iki durumlu düğmeyi seçerek bu deneyimi etkinleştirerek bu deneyimi etkinleştir kullanılabilir. Ayrıca tüm sayfalarda görüntülenen "Şimdi deneyin" başlığı seçerek yeni EAC'ye de gidebilirsiniz.

Yeni EAC'nin avantajları şunlardır:

- Posta akışıyla ilgili sorunlar için içgörüler, raporlar ve uyarı mekanizmaları eklendi. 

- Üretkenliği artırmak için kişiselleştirilmiş panolar.

Yeni deneyimde gezinmenize yardımcı olmak için yeni EAC **deneyiminin Eğitim &** Kılavuzu bölümünde videolar mevcuttur. Bunlar, yeni portalı en iyi şekilde nasıl kullanabileceğiniz hakkında genel bir bakış sağlar.

>[!NOTE]
>Bu değişiklikle, klasik EAC deneyimi kullanım dışı olmayacaktır. Herhangi bir değişiklik uygulanmadan önce size önceden bildirilecek.

### <a name="next-steps"></a>Sonraki adımlar

- Yeni [deneyimin ekran görüntülerini](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/)görüntüyebilirsiniz. Bu konu başlığıyla ilgili kaynaklara göz atabilirsiniz.

- Bu bilgileri, kuruluşta uygun proje katılımcıları ile paylaşın. 

### <a name="questions"></a>Sorularınız mı var?

Bu değişikliklerle ilgili sorularınız için ilgili toplulukları Yammer kontrol edin.

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="17"></a>Microsoft İşlemleri: Ürün lansman takvimini tanıtma

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-25
- Teklif | Modern Çalışma Alanı

### <a name="summary"></a>Özet

İş ortağı geri bildirimlerine yanıt olarak Microsoft İşlemleri, ürün lansmanları için iletişimi kolaylaştıracak.

### <a name="impacted-audience"></a>Etkilene hedef kitle

Bulut Çözümü Sağlayıcısı (CSP) iş ortakları

### <a name="details"></a>Ayrıntılar

Microsoft, iş ortağı deneyimlerini sürekli geliştirmeye kararlıdır. Microsoft'tan çok fazla iletişim aldığını ve ürün lansmanları için yinelenen duyurular da dahil olmak üzere geri bildirim aldık.

Geri bildiriminize yanıt olarak Microsoft, yeni ve mevcut teklifler için ürün lansmanlarına hazır olma deneyimini kolaylaştırdı.

Şimdi operasyon hazırlığı kaynak galerisinde yayımlanan ürün lansmanlarının tek bir aylık görünümünü sağlarız. Bu aylık [ürün lansman takvim görünümü,](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) İşlemler için hazır olma kaynak galerisinde ve uygulama duyurularında ürün İş Ortağı Merkezi yerini alacak.

Bu ürün lansman [takvimine topluluk](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) [koleksiyonlarından, takvim görünümlerinden](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) [ve](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated) [CSP bültenlerinden de erişebilirsiniz.](https://partner.microsoft.com/resources/collection/csp-monthly-update#/) Her ayın ürün lansman takvimini, İşlemler için hazır olma kaynak galerisinde bir duyuru ile yayımlayacaz.

Yeni ve mevcut tekliflere ilişkin bilgileri fiyat listesi önizleme ve fiyat listesi değişiklik günlüklerinde, ayrıca ürün bloglarında, lisanslama kılavuzlarında ve ürün pazarlama sayfalarında bulabilirsiniz.

Bu değişiklik, aşağıdaki ürünler için lansmanlar için geçerli olacaktır:

- Dynamics şirket içi
- Microsoft 365
- Microsoft Dynamics 365
- Windows
- Sunucu  
- Araçlar
- Teams ve telco

Işlem hazırlığı ayrıntıları gerektiren ürün başlatma için özel duyurular gönderilmeye devam edeceğiz.

### <a name="next-steps"></a>Sonraki adımlar

Bu konuyla ilgili kaynakları gözden geçirin ve bu bilgileri kuruluşunuzdaki uygun hissedarlarla paylaşabilirsiniz.

### <a name="questions"></a>Sorularınız mı var?

bu teklifler hakkında daha fazla soru için ilgili Yammer topluluklarınızı kontrol edin.

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="16"></a>CSP müşteri ekleme gereksinimlerinde yapılan değişiklikler

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-25
- Özellikler

### <a name="summary"></a>Özet

İş ortakları ve müşterilerin işlerini güvenle çalıştırmasına yardımcı olma çabamız kapsamında, 25 Mart 2021 ' den itibaren geçerli olan ek müşteri bilgileri isteyeceğiz.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

Bulut Çözümü Sağlayıcısı (CSP) doğrudan fatura ortakları ve sonraki bölümde listelenen ülkelerde yeni veya mevcut müşteriler bulunan dolaylı sağlayıcılar

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
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="15"></a>1 Mart 2021 ' de yapılan düzeltmeler kalıcı yazılım fiyat listesi

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-23
- Teklifler/Pazarlar

### <a name="impacted-audience"></a>Etkilenen hedef kitle

Bulut Çözümü Sağlayıcısı programında dolaylı sağlayıcılar ve doğrudan fatura ortakları deneyimidir kalıcı yazılım 

### <a name="details"></a>Ayrıntılar

1 Mart 2021 ' de gönderilen kalıcı yazılım için fiyat listesi, orada olmaması gereken pazarlara dahil değildir. Kalıcı yazılım fiyat listesi, düzeltmeler ile 17 Mart 2021 ' de güncelleştirildi. Bu düzeltmeler yalnızca için geçerlidir:

- Ürün KIMLIĞI: DF77X4D43RKT 
- ürün adı: Microsoft 365 işletme için Pro yükseltmeye Windows 10 Home
- Kaldırılan veya desteklenmeyen pazarlar: AE, AF, AL, har, AO, BA, BB, BD, BH, BM, mılyar TL, BO, BR, BS, beyaz,,,, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, , MN, MO, MU, NA, NG, Nı, NP, OM, PA, PE, PH, PK, PR, INER, QA, RS, RU, RW, SG, SN, ZF, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YS, ZM, ZW

Bu değişiklikler yalnızca yukarıdaki ürün için geçerlidir. Diğer ürünlerin bir düzeltme yoktur. 

### <a name="next-steps-and-resources"></a>Sonraki adımlar ve kaynaklar

- Transact kalıcı yazılım kullanan iş ortakları en son kalıcı yazılım fiyat listesini indirmelidir.
- Ülkelerinden oluşan iki harfli kısaltmayı kolay bir şekilde eşlemek için [bölge ülke kodlarına](/azure/marketplace/commercial-marketplace-co-sell-countries) başvurun.
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="14"></a> .NET Standard SDK sürümü (v 1.17.0)

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-23

- Özellikler
 
### <a name="impacted-audience"></a>Etkilenen hedef kitle

Iş ortağı merkezi .NET SDK 'sını kullanan CSP programına katılan doğrudan fatura ortakları ve dolaylı sağlayıcılar.

### <a name="details"></a>Ayrıntılar

23 2020 mart itibariyle iş ortakları, [microsoftpartnercenter. netsdk 'nın (NuGet galerisi) sürümünü indirmeye başlayabilir | Microsoft. Store. partnercenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), güncelleştirilmiş ortak iş ortağı merkezi SDK [GitHub örneklerle](https://github.com/Microsoft/Partner-Center-DotNet-Samples)birlikte. Bu sürüm aşağıdaki yöntemlerin güncelleştirmelerini içerir:

#### <a name="audit-updated-new-operation-types"></a>Denetim güncelleştirildi: yeni işlem türleri

Müşterinin ne zaman onayladığı ve sonlandırıldığı hakkında bilinmesi için yeni [işlem türleri](/partner-center/develop/auditing-resources) eklendi.

- DapAdminRelationshipApproved

- Dapadminrelationshipsonlandırılan

#### <a name="audit-updated-new-resource-and-operation-types"></a>Denetim güncelleştirildi: yeni kaynak ve işlem türleri

Müşteri dizin rolü senaryosunu desteklemek için yeni [kaynak ve işlem türleri](/partner-center/develop/auditing-resources) eklendi.

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

- en son [microsoftpartnercenter. netsdk sürümünü indirin (NuGet galerisi | Microsoft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)
- [GitHub örnekleri](https://github.com/Microsoft/Partner-Center-DotNet-Samples) indirin ve gözden geçirin

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="13"></a>Uygun teklifler için CSP ticari Market teklifi ve FY21 CSP teşvikleri

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-18
- Özellikler

### <a name="impacted-audience"></a>Etkilenen hedef kitle

Bulut Çözümü Sağlayıcısı programdaki dolaylı sağlayıcılar ve doğrudan fatura ortakları 

### <a name="details"></a>Ayrıntılar

Bulut Çözümü Sağlayıcısı programdaki dolaylı sağlayıcılar ve doğrudan fatura ortakları, üçüncü taraf teklifleri satmakta ve iş ortağı merkezinde veya Azure portal işlenen her bir uygun üçüncü taraf teklifi için bir indirim teşvik elde edebilir. Bu öneriler, uygun tekliflerle ilgili olarak faturalandırılan satış hakkında indirim biçiminde olacaktır ve **30 haziran 2021 ' ye kadar kullanılabilir**.  

Aşağıdaki CSP ticari marketi teklifi hakkında bilgi edinmeye devam edin ve müşterilerin devam ettirme başarısını ve dijital dönüşümünü etkinleştirmeye yönelik doğru teklifleri belirlemek için müşterilerinizle iletişim kurun.

En son IaaS ve SaaS çözümlerini Microsoft müşterilerine pazarlamak için bağımsız yazılım satıcıları (ISV 'Ler) ile iş ortaklıyoruz. ISV yayımcıları, Microsoft iş ortağı kanalı aracılığıyla tekliflerinden satışları etkinleştirme seçeneğine sahiptir. Özendiğimiz tekliflerimiz iki kategoride yer almalıdır:

- Azure IP ortak satış incentivized durumu ile SaaS ve IaaS üçüncü taraf tekliflerini seçin. 

- Teams veya PowerPoint, sözcük, Excel, Outlook veya SharePoint gibi en az iki Microsoft 365 üretkenlik uygulaması ile tümleştirilmiş SaaS uygulamaları.

### <a name="next-steps-and-resources"></a>Sonraki adımlar ve kaynaklar

- Uygun Market uygulamaları satmaya uygun olan uygulamaları teşvik etmek için [Iş ortağı teşvikleri](https://partner.microsoft.com/membership/partner-incentives) hakkında bilgi edinin. Yeni teklifler aylık olarak eklenir.  
- [Bulut Çözümü Sağlayıcısı doğrudan fatura ortağı özendirme kaynakları](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [Bulut Çözümü Sağlayıcısı dolaylı sağlayıcı özendirme kaynakları](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- Ticari market uygulamalarını satma hakkında daha fazla bilgi edinmek için bu [sunuyu](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) gözden geçirin. Ek kaynaklara [buradan](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/)göz atın. 
- [Iş Ortağı Merkezi](../csp-commercial-marketplace-discover.md) veya [Azure Portal](https://ms.portal.azure.com/#home) ticari Market kataloğunu keşfet
- Uygulamaları şirketinizin marketi ile bütünleştirmek için [API 'leri](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) kullanma
- İş yaparken ilgilendiğiniz ISV 'lere ulaşın
- Dolaylı sağlayıcıların, hangi uygulamaların satmaya yönelik API 'Leri ve kılavuz satıcılarını kullanarak tümleştirmeleri gerekir

### <a name="questions"></a>Sorularınız mı var?  

Iş Ortağı Merkezi 'nde ticari Market 'e genel bakış için [Bu makaleye](../csp-commercial-marketplace-overview.md) başvurun.

Daha fazla yardıma ihtiyacınız varsa, Iş Ortağı Merkezi 'nde bir destek isteği oluşturabilirsiniz. Daha fazla bilgi edinin [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="12"></a>Power BI Premium teklif adlandırma ve önkoşul güncelleştirme

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-18
- Özellikler

### <a name="summary"></a>Özet

1 nisan 2021 son fiyat listesi, kullanıcı başına Power BI Premium için adlandırma ve/veya önkoşul bilgilerine açıklık eklemek üzere güncelleştirilir.

### <a name="impacted-audience"></a>Etkilenen hedef kitle

Bulut Çözümü Sağlayıcısı (CSP) doğrudan ve dolaylı iş ortakları

### <a name="details"></a>Ayrıntılar

1 nisan 2021 son fiyat listesi, kullanıcı başına Power BI Premium için adlandırma ve/veya önkoşul bilgilerine açıklık eklemek üzere güncelleştirilir.

Son fiyat listesi güncelleştirilene kadar, bu bölümdeki bilgileri kullanarak doğru ürünün düzenli olduğundan emin olun.

Aşağıdaki ayrıntılar etkilenen SKU ve önkoşul ayrıntılarını göstermektedir.

| 1 Mart 'ta bir görünen ad teklif listesi önizlemesi |  1 Nisan 'ın son fiyat listesindeki teklif görünen adı güncelleştirildi| Teklif Kimliği |
| ------ | ----------- | ----------- |
| Power BI Premium Kullanıcı başına Add-On (kar amacı gütmeyen personel fiyatlandırması)  |  Power BI Premium kullanıcı başına Add-On **(Office)** (kar amacı gütmeyen personel fiyatlandırması)   | 31c03289-47AB-4AB0-8df1-03742c127ac6   |

Müşterilerin bu teklifi satın almak için aşağıdaki önkoşulların herhangi birine sahip olması gerekir:

| Teklif görünen adı | Teklif Kimliği |
| ------ | ----------- |
| Microsoft 365 E5 (kar amacı gütmeyen personel fiyatlandırması)  |  31bedf01-9e57-4ece-a53a-d3656a563931   |
|   ses konferansı olmadan Microsoft 365 E5 (kar amacı gütmeyen personel fiyatlandırması)|  b456810a-c414-4e07-98fc-ef74e8175a09|
|   Office 365 E5 (kar amacı gütmeyen personel fiyatlandırması)| ce139fe5-8bd5-47ED-a5be-07c286f8b9e    |
|   Office 365 E5 (kar amacı gütmeyen personel fiyatlandırma) denemesi|  2f192efe-608a-4C9C-9d19-2b0b70b0962e|
|   ses konferansı olmadan Office 365 E5 (kar amacı gütmeyen personel fiyatlandırması)|  c3897426-9f49-4eaf-9b4d-7d9a1c72aef7|

aşağıdaki Power BI Premium teklifi satın alma için gereken bir önkoşula sahiptir:

| Teklif görünen adı | Teklif Kimliği |
| ------ | ----------- |
|   Power BI Premium Kullanıcı başına Add-On (kar amacı gütmeyen personel fiyatlandırması)|  ef0b895b-681b-4026-a5b1-dda182a57d40 |

Müşterilerin bu teklifi satın alması için bu önkoşulu olması gerekir:

| Teklif görünen adı | Teklif Kimliği |
| ------ |----------|
| Power BI Pro (kar amacı gütmeyen personel fiyatlandırması)  |   cabdfc93-5786-4224-bfd3-35d58f833b35 |

### <a name="next-steps"></a>Sonraki adımlar

Bu konuyla ilgili kaynakları gözden geçirin ve bu bilgileri kuruluşunuzdaki uygun hissedarlarla paylaşabilirsiniz.  

### <a name="questions"></a>Sorularınız mı var?

bu tekliflerle ilgili herhangi bir soru için ilgili Yammer topluluklarınızı kontrol edin. 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="11"></a>Microsoft 365 F3 için Mart fiyat güncelleştirmeleri

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-16
- Teklifler/Pazarlar

### <a name="summary"></a>Özet

Microsoft 365 F3 ingiliz sterlini (gbp) ve Euro (EUR) için 2021 mart fiyatlandırması yanlış düzeltildi.

### <a name="impacted-audience"></a>Etkilene hedef kitle

İş ortakları Microsoft 365 F3 (CSP) programı aracılığıyla 1 Mart ile 17 Mart 2021 Bulut Çözümü Sağlayıcısı GBP veya EUR olarak satın almaları.

### <a name="details"></a>Ayrıntılar

Microsoft, Microsoft 365 F3 için yanlış fiyatlandırmayı Microsoft 365 F3. Hatalı fiyatlar GBP ve EUR için ve yalnızca 1 Mart ile 17 Mart 2021 arasında satın alınan teklifler içindi. Etkilenmiş teklifler ve para birimleri aşağıda listelenmiştir. 

| Teklif adı | Para Birimi | Teklif Kimliği | Malzeme Kimliği |
| ------ |----------- |----------- |----------- |
| Microsoft 365 F3 (Yer) | GBP | 57b722c2-c435-4bfb-9bc8-80509213a13a | AAD-11626 |
| Microsoft 365 F3 (Ticari) | EUR| 3451a3b0-8cda-44a7-bad7-c30be81c4aaa | AAA-89898 |
 
Mart ve Nisan önizleme lisans tabanı fiyat listeleri 16 Mart 17:00 Pasifik standart saatiyle güncelleştirildi.

### <a name="next-steps"></a>Sonraki adımlar

- İş ortaklarının geçerli lisans tabanlı fiyat listelerini (Mart ve Nisan önizlemesi) yeniden yüklemesi ve varsa bu fiyat düzeltmelerini de yüklemesi gerekir.  
- Microsoft, etkilenen işlemlerin düzeltilmesiyle ilgili sonraki adımları bildirmek için önümüzdeki haftalarda e-posta yoluyla etkilenen iş ortaklarıyla iletişim kuracak.

### <a name="questions"></a>Sorularınız mı var?

Diğer sorularınız için lütfen ilgili CSP Yammer kontrol edin.

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="10"></a> Yasal şirket adını şirket İş Ortağı Merkezi

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-16
- Sürücü Verimliliği & Ölçeklendirme

### <a name="summary"></a>Özet

Mart 2021'den başlayarak Microsoft İş Ortağı Ağı (MPN) iş ortakları ve Bulut Çözümü Sağlayıcısı (CSP) dolaylı kurumsal bayileri, yasal şirket adını İş Ortağı Merkezi.

### <a name="impacted-audience"></a>Etkilene hedef kitle

MPN iş ortakları ve CSP dolaylı kurumsal bayileri (CSP doğrudan fatura iş ortakları için geçerli değildir)

### <a name="details"></a>Ayrıntılar

Mart 2021'den başlayarak MPN iş ortakları ve CSP dolaylı kurumsal bayileri, yasal şirket İş Ortağı Merkezi uyumlu ve self servis bir şekilde güncelleştirebilmektedir. Bu yeni özellik sayesinde iş ortaklarının şirket adını güncelleştirmek için İş Ortağı Merkezi destek bileti göndermesi gerekmeyecek. Bu, bu etkinlikleri gerçekleştirerek iş ortakları için önemli ölçüde zaman tasarrufu sağlar. 

Daha fazla bilgi edinmek için [bkz. Yasal iş profilinizi güncelleştirme.](../update-your-partner-profile.md#update-your-legal-business-profile)

>[!NOTE]
>Yasal iş profilinizde şirket adının yazım hataları ve kısaltmaları olduğundan ve resmi şirket iş kaydı kayıtlarınıza tam olarak uygun olduğundan emin olun. Kuruluş profilinizi güncelleştirme hakkında daha fazla bilgi için bkz. [Kuruluş profilinizi doğrulama.](../update-your-partner-profile.md#update-your-legal-business-profile)

### <a name="next-steps"></a>Sonraki adımlar

Uygun ekibin işlemlerini gözden geçire incelemesi ve güncelleştirmesi için bu bilgileri kuruluş içinde paylaşın.

### <a name="questions"></a>Sorularınız mı var?

Diğer sorularınız için lütfen ilgili CSP Yammer kontrol edin.

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="9"></a>Güncelleştirme: Bulut Çözümü Sağlayıcısı (CSP) programı evrimi ve Açık Lisans programı değişiklikleri

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-15
- Özellikler

### <a name="summary"></a>Özet

Açık Lisanslama programında yapılan değişikliklerle birlikte Bulut Çözümü Sağlayıcısı (CSP) programına yeni ticari ve kamu sektörü kalıcı yazılım teklifleri geliyor.

### <a name="impacted-audience"></a>Etkilene hedef kitle

Açık Lisans programı aracılığıyla satış yapan ticari dağıtımcılar ve yönetilen kurumsal bayilerin yanı sıra kalıcı yazılım işlem yapan tüm CSP iş ortakları

### <a name="details"></a>Ayrıntılar

[Eylül](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) 2020'de Microsoft, iş ortakları için şirket içi yazılımların kullanılabilirliği dahil olmak üzere CSP programı kapsamındaki iş ortaklarına fırsatları genişletmek için dijital dönüşüm yolculuğumuza bir dizi adımı duyurdu. Bu değişiklikler, iş ortaklarının CSP'de yazılım lisanslarından yararlanarak işletmelerini büyüterek ve günümüzün buluta ilk dünyasında başarıya ulaşacak şekilde konumlandırmalarına olanak sağlar. Ayrıca müşterilerin buluta geçişlerini güçlendirerek iş ortaklarına müşteri hibrit bulut ortamları için gereken esnekliği sunar.

Bu dijital dönüşümün devamında aşağıdaki değişiklikleri açıklarız:

- 1 Temmuz 2021: Açık Lisans programı fiyat listesine yeni SKU' lar, ürünler veya promosyonlar eklenmez.

- 7 Temmuz 2021: CSP kalıcı yazılım fiyat listesine Orijinal Windows Edinme ve Visual Studio Professional ve kamu sektörü teklifleri (kamu, eğitim ve kar amacı gütmeyen kuruluş – duyuruya [bakın)](./2020-december.md#9)olmak için iki ticari teklif eklenecektir.  Fiyat listesi, İş Ortağı Merkezi'daki [> Fiyatlandırma & Teklifleri](https://partnercenter.microsoft.com/pcv/sales) sayfasının Yazılım bölümünde bulunabilir ve bu tarihte yeniden yayımlanmaz.

CSP programı evrimi ve Açık Lisans programı değişiklikleriyle ilgili tüm ayrıntılar için lütfen aşağıdaki **Sonraki Adımlar'a** bakın.

### <a name="next-steps"></a>Sonraki Adımlar:

- CSP Programı evrimi: Program [hazırlığı malzemelerini Bulut Çözümü Sağlayıcısı Kalıcı](https://partner.microsoft.com/resources/collection/software-in-csp#/) yazılımı gözden geçirme. Rolünüz [için doğru bilgileri](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) hızla bulmak üzere bu hazır olma haritasını kullanın.

- Açık Lisans programı değişiklikleri: CSP programı [evrimini ve Açık Lisans programı değişikliklerinin hazırlık malzemelerini](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) gözden geçirme. Rolünüz [için doğru bilgileri](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) hızla bulmak üzere bu hazır olma haritasını kullanın.

### <a name="questions"></a>Sorular

Diğer sorularınız için lütfen ilgili CSP Yammer kontrol edin.

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="8"></a>Önceki bir duyuruya güncelleştirin: Premium Değerlendirmeleri, Uyumluluk Yöneticisi'ne bir eklenti

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-15
- İşlerinizi büyütme

### <a name="summary"></a>Özet

Deneme teklifleri fiyat listesinde listelenmiyor olmalı ve kaldırılacaktır.

### <a name="impacted-audience"></a>Etkilene hedef kitle

İş ortakları Bulut Çözümü Sağlayıcısı

### <a name="details"></a>Ayrıntılar

Deneme teklifleri fiyat listesine dahil etmene gerek yok. Bunlar 1 Mayıs 2021 fiyat listesinden kaldırılacaktır.

İlk duyuru [buradadır.](./2021-february.md#4)

### <a name="additional-resources"></a>Ek kaynaklar

- [Microsoft 365 E5 ve uyumluluk](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [Microsoft Uyumluluk Yöneticisi'nde değerlendirmeleri oluşturma ve yönetme - Microsoft 365 Uyumluluğu](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a>Sonraki adımlar

Bu konu başlığıyla ilgili kaynakları gözden geçirme ve bu bilgileri kuruluşta uygun proje katılımcıları ile paylaşma.

### <a name="questions"></a>Sorularınız mı var?

Bu teklifler hakkında sorular için ilgili topluluklar için Yammer kontrol edin.

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="7"></a> Çözümlerinizi Bir Ticari İş Ortağından (OCP) pazara satışa (GTM) Microsoft ticari markete geçirme

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-12
- Özellikler

### <a name="summary"></a>Özet

29 Mart 2021'den itibaren sınırlı Bir Ticari İş Ortağı (OCP) pazara satış (GTM) özellikleriyle deneyim edineceksiniz. Çözümlerinizi İş Ortağı Merkezi'da ticari markete geçirmenizi İş Ortağı Merkezi.

### <a name="impacted-audience"></a>Etkilene hedef kitle

Kuruluşlar OCP GTM'de çözümlerle ortak satışlar

### <a name="details"></a>Ayrıntılar

Aralık 2020'de, Microsoft OCP GTM aracından microsoft'ta Microsoft ticari marketi ile İş Ortağı Merkezi. Bu geçiş, çözümlerinizi milyonlarca müşteriyle gösterip diğer Microsoft ve iş ortağı satıcılarla çift yönlü olarak fırsat paylaşıp yenilikçi çözümler satarak ticari marketin özelliklerini genişletir.

Geçişte bir sonraki kilometre taşı 29 Mart 2021'de gerçekleşecek. İşte bu zaman sınırlı OCP GTM özellikleriyle, bazı alanlar salt okunur hale geldi. Şu anda OCP GTM'de çözümlerle ortak satışlar sunuyorsanız, özelliklerini yararlanmak ve yayımlama deneyiminizi basitleştirmek için çözümlerinizi ticari markete geçirmenizi teşvik ediyoruz.

Ticari markete taşıma, ortak İş Ortağı Merkezi yayımlama deneyimi için birincil hedef haline gelmektedir. Microsoft ürünleri için aynı kanallar ve ürün içinde deneyimler aracılığıyla çözümlerinizi paylaşılan müşterilerimize bağlayarak işlerinizi büyümeye devam edersiniz. [Ticari market hakkında daha fazla bilgi alın.](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/)

### <a name="next-steps"></a>Sonraki adımlar

- Çözümlerinizi henüz taşımadıysanız, geçiş kılavuzunda [](/azure/marketplace/co-sell-solution-migration) ayrıntılı yönergeleri izleyin veya tüm geçiş etkinliklerini tamamlamak ve çözümlerinizi ticari markette yayımlamaya başlamak için adım adım [video öğreticiyi](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) izleyin.

- OCP GTM'de sınırlı yetenek deneyimiyle ilgili sorular için Ortak satış gereksinimlerini Microsoft ticari market [SSS'de yayımlayın.](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf) ("29 Mart 2021'den başlayarak OCP GTM sınırlı özellikleri" bölümüne bakın.)

### <a name="questions"></a>Sorularınız mı var?

Sorularınız [varsa](https://partner.microsoft.com/support/?stage=1) veya daha fazla bilgiye ihtiyacınız varsa De destekle iletişime geçin.

________________
## <a name="programmatic-access-to-commercial-marketplace-analytics"></a><a name="6"></a>Ticari market analizine programlı erişim

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-10
- Özellikler

### <a name="summary"></a>Özet

İş ortakları artık satışları izlemek, performansı değerlendirmek ve ticari markette teklifleri iyileştirmek için analiz raporlarına program aracılığıyla erişebilir.

### <a name="impacted-audience"></a>Etkilene hedef kitle

Ticari markette tekliflerle iş ortakları.

### <a name="details"></a>Ayrıntılar

Ticari market raporlarına erişim API'si, analiz verilerinizin özel raporlarını zaman uyumsuz olarak zamanlamanıza olanak sağlar.

Bu özellik, ihtiyaçlarınıza göre raporlama sorguları ve şablonları tanımlamanızı, bir zamanlama ayarlamanızı ve zamanlanan aralıklarla zamanında ve güvenilir raporlar amanızı sağlar.

### <a name="next-steps"></a>Sonraki adımlar

Daha fazla bilgi edinmek için [bkz. Kullanmaya başlayın programlı erişimi olan uygulama.](/azure/marketplace/analytics-get-started)

### <a name="questions"></a>Sorularınız mı var?

Başka [sorularınız](https://go.microsoft.com/fwlink/?linkid=2165533) varsa De destekle iletişime geçin.

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a>Azure'dan Rusya'ya Bulut Çözümü Sağlayıcısı (CSP) programı kapsamındaki yeni ticaret deneyimini genişletme

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-10
- Özellikler

### <a name="impacted-audience"></a>Etkilene hedef kitle

Rusya'daki tüm iş ortakları Bulut Çözümü Sağlayıcısı (CSP) programı aracılığıyla işlem yaptı.

### <a name="details"></a>Ayrıntılar

10 Mart 2021'den başlayarak, Rusya'da Azure için CSP'de yeni ticaret deneyiminin **kullanılabilirliğini duyurmak için heyecanlanıyoruz.** Bu deneyim, müşterilerin Azure hizmetlerini satın alma ve tüketme yolunu kolaylaştıracak ve geliştirecektir. Ayrıca CSP programı iş ortaklarına satış hareketlerine göre Azure fiyatlandırmasını tutarlı bir şekilde görüntüleme, küresel tutarlılık için USD fiyatlandırması, faturalama tarihi hizalaması ve azure fiyatlandırması Azure Maliyet Yönetimi.

### <a name="next-steps"></a>Sonraki adımlar

Yeni Azure ticaret deneyimini tanıtan ve ek bilgiler sağlayan birçok kaynak vardır. CSP Program Güncelleştirmeleri Kaynak Galerisi'nde en son [SSS,](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/)desteler, video ve daha fazlasını bulabilirsiniz.

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a>İş Ortağı Merkezi lisans anahtarını indirme ve gerçekleştirmeyi indirme

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-04
- Özellikler

### <a name="summary"></a>Özet

Yazılım İş Ortağı Merkezi ve lisans anahtarı yerine getirme özelliği yeniden getirildi.

### <a name="impacted-audience"></a>Etkilene hedef kitle

Tüm Bulut Çözümü Sağlayıcısı (CSP) iş ortakları, sürekli ve sunucu aboneliği yazılım siparişlerini İş Ortağı Merkezi

### <a name="details"></a>Ayrıntılar

İş ortağı geri bildirimlerine yanıt olarak, kalıcı ve İş Ortağı Merkezi abonelik yazılım siparişleri için yazılım ve lisans anahtarları alma olanağını yeniden hazırlarız. 19 Ocak 2021'de kaldırılmasından önceki durumuna geri yüklenecektir. (Duyuruya [bakın.)](2020-september.md#17)

Yazılım lisans anahtarları ve indirme bağlantılarının değerli ve son derece aranılan fikri mülkiyet varlıkları olduğunu unutmayın. Sızdırıldıklarında etkinleştirme sınırları hızla tükenebilir ve olumsuz müşteri ve iş ortağı deneyimine neden olabilir.

### <a name="next-steps"></a>Sonraki adımlar

Kullanım yönergeleri ve yazılım anahtarı dağıtımıyla ilgili önemli yönergeler için aşağıdaki kaynakları gözden geçirme:

- [CSP programı aracılığıyla şirket içi yazılım satma](../csp-on-premise-software.md)
- [İş Ortağı Merkezi Ticaret İşlemleri Kılavuzu (Yazılım](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) Anahtarı **Dağıtımı Kılavuzu bölümüne** bakın.)

### <a name="questions"></a>Sorularınız mı var?

Bu bildirimle ilgili başka sorularınız varsa, ilgili topluluklar için Yammer kontrol edin.

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a>Anlaşmalarınızı İş Ortağı Satışları Bağlan (PSC) İş Ortağı Merkezi

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-04
- Özellikler

### <a name="summary"></a>Özet

İş Ortağı Bağlan (PSC), 31 Mart 2021'den başlayarak salt okunur erişime taşınacak, bu nedenle anlaşmalarınızı PSC'den İş Ortağı Merkezi.

### <a name="impacted-audience"></a>Etkilene hedef kitle

PSC'de anlaşmaları olan iş ortakları

### <a name="details"></a>Ayrıntılar

Ortak büyüme taahhüdü kapsamında **Microsoft** ile ortak satış yapmak, keşfedilecek, uzmanlığınızı sunacak ve olumlu müşteri sonuçları elde etmek için müşteri ayak izinizi genişletecek olan yoldur.  Ortalama satış fiyatı **normalden 3,5** kat daha hızlı olduğu için İş Ortağı Merkezi'de ortak satış deneyiminizi yönetmek doğrudan müşteri, iş ortağı ve Microsoft satıcı kanalları arasında satış ve referans işlem hattınızı tek bir konumda yönetmenizi sağlar.

**PSC,** 31 Mart **2021'den** itibaren salt okunur erişime taşınacak. Bu nedenle, İş Ortağı Merkezi ve bu özellik geliştirmelerine erişmenizi istiyoruz:  

- **Microsoft ile** paylaştığın satış anlaşmalarının, ihtiyacınız olan yardım türüne göre doğru satıcıya yönlendiren daha doğru yönlendirme.
- **Teşvike uygun çözümler için** ön anlaşma uygunluk doğrulaması ve ISV Bağlan programı ölçütlerini karşılamak, onay sürecini ve son yürütme kanıtı (POE) kanıtını basitleştirir.
- **Tüm ortak satış** fırsatlarınızı ve satış nitelikli müşteri adaylarınızı tek bir yerde yönetmek için sorunsuz kullanıcı deneyimi.

Ayrıca taşımanıza yardımcı olmak için İş Ortağı Merkezi yeni özellikler ekledik:

- [Ortak satış fırsatları için toplu işlemler](../bulk-operations.md)
- [Anlaşma geçişi özelliği](../psc-to-pc.md) **(PSC Anlaşmaları geçiş bölümüne** bakın.)

Satış ekipleriniz İş Ortağı Merkezi satış deneyimini kullanarak müşteri adaylarını ve fırsatları beslemeye, satış anlaşmalarını kapatmaya ve müşteri ilişkileri oluşturmaya daha fazla zaman sahip olacak.

### <a name="next-steps"></a>Sonraki adımlar

Anlaşmalarınızı PSC İş Ortağı Merkezi den İş Ortağı Merkezi'a geçirme adımları için İş Ortağı Merkezi. [](../psc-to-pc.md)

### <a name="questions"></a>Sorularınız mı var?

Daha fazla soru için Destek ile iletişime [geçin.](https://partner.microsoft.com/support/?stage=1)

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a>1 Nisan 2021'de yeni Microsoft Dynamics 365 ürünleri ve teklifleri

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-04
- Özellikler

### <a name="summary"></a>Özet

1 Nisan 2021'de Microsoft, Bulut Çözümü Sağlayıcısı (CSP) programı için birçok yeni ürün ve teklif başlatacak.

### <a name="impacted-audience"></a>Etkilene hedef kitle

Bulut Çözümü Sağlayıcısı (CSP) programı aracılığıyla işlem yapılan tüm iş ortakları

### <a name="details"></a>Ayrıntılar

Microsoft, 1 Nisan 2021'de aşağıdaki yeni ürünleri ve teklifleri başlatacak:

- Power BI Premium Kullanıcı Başına
- Customer Voice and Marketing USL coğrafi ve segment genişletmesi

**Power BI Premium Kullanıcı Başına**

Microsoft, kullanıcı başına ilk kullanıcı başına Power BI Premium tanıtacak. Power BI Premium şu anda yalnızca bir kapasite yapısında satılıyor. Power BI Premium Kullanıcı Başına kurumsal iş zekası (BI) ve analiz özelliklerine erişim sağlar. Esnek bireysel lisanslama, küçük ve orta ölçekli işletmelere hitap ediyor.

Bu teklif [Power BI daha fazla bilgi](/power-platform-release-plan/2020wave2/power-bi/planned-features) edinmek için yayın ayrıntılarını gözden geçirebilirsiniz.


**Teklif ayrıntıları**

Teklif adının fiyat listesi önizlemeden biraz farklı olduğunu unutmayın.

| Teklif adı | Teklif Kimliği |
| ------ |----------- |
| Power BI Premium Kullanıcı Başına | 9c810018-9356-4903-95ab-eeb956289290 | 
| Power BI Premium Fakülteler için Kullanıcı Başına | 3affc44f-f372-4ad5-8657-aadd9574fce0 | 
| Power BI Premium Öğrenciler için Kullanıcı Başına | 657eea87-d0b0-4c89-8c8e-9b04395bd940 | 
| Power BI Premium Kullanıcı Başına (Kar Amacı Gütmeyen Personel Fiyatlandırması) | 7a0a856c-059f-45dd-9d26-ae27992e706a | 
| Power BI Premium Kullanıcı Başına Add-On | 244ff87e-5925-44a0-bf31-cea189719b58 | 
| Power BI Premium Fakülteler Add-On Kullanıcı Başına | 5da849bd-b8f7-4340-b4f4-3a9eaeb8987e | 
| Power BI Premium Öğrenciler için kullanıcı Add-On başına | cf62d70d-5af5-422a-bda8-97936402ac8e | 
| Power BI Premium Kullanıcı Başına Add-On (Kar Amacı Gütmeyen Personel Fiyatlandırması) | 31c03289-47ab-4ab0-8df1-03742c127ac6 | 

**Customer Voice and Marketing USL coğrafi ve segment genişletmesi**

Aralık 2020 lansmanını takip etmek için Dynamics 365 Customer Voice and Marketing USL teklifleri yeni ülkeler ve daha fazla kar amacı gütmeyen ve eğitim amaçlı SKUS eklemek için değiştirilmiştir.

| Teklif adı | Teklif Kimliği |
| ------ |----------- |
| Dynamics 365 Customer Voice USL (Kar Amacı Gütmeyen Personel Fiyatlandırması) | 7a8642a5-481e-4906-a642-b56dbeeb62a0 |
| Fakülteler için Dynamics 365 Customer Voice USL | 85162d70-9676-4cf6-a4bc-a0d6672f2657 |

Bu teklifler hakkında daha fazla bilgi için aşağıdaki sayfaları ziyaret edin:

- [Dynamics 365 Müşteri Hizmetleri Ses giriş sayfası](https://dynamics.microsoft.com/customer-voice/overview/)
- [Dynamics 365 Marketing giriş sayfası](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a>Sonraki adımlar

Bu konu başlığı altında yer alan kaynakları gözden geçirin ve bu bilgileri, kuruluşta uygun proje katılımcıları ile paylaşın.  

### <a name="questions"></a>Sorularınız mı var?

Bu teklifler hakkında sorularınız varsa ilgili topluluklar için Yammer kontrol edin. 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> Microsoft Evrensel Yazdırma artık bazı paketlerin içinde kullanılabilir

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-03
- Özellikler

### <a name="summary"></a>Özet

Microsoft Evrensel Yazdırma, 1 Mart 2021'den itibaren Microsoft 365 paketleri ve tek başına eklenti olarak işlem yapmak için kullanılabilir.

### <a name="impacted-audience"></a>Etkilene hedef kitle

Bulut Çözümü Sağlayıcısı (CSP) programı aracılığıyla işlem yapılan tüm iş ortakları

### <a name="details"></a>Ayrıntılar

[Evrensel Yazdırma](https://aka.ms/universalprint) şirket Microsoft 365 sunucularına olan ihtiyacı ortadan kaldıran ve Windows cihazların Azure'a kayıtlı yazıcılara yazdırmasını sağlayan bir yazdırma hizmetidir. 1 Mart 2021'den itibaren işlem için kullanılabilir olacak.

Çalışanlar sürücüsüz yazdırma, kolaylaştırılmış konum tabanlı yazıcı bulma ve öğrenme eğrisi olmayan sezgisel yazdırma deneyiminden faydalanıyor. Azure Active Directory 'a (Azure AD) katılan cihazlar, mevcut Azure AD kimlik bilgilerini kullanarak güvenli bir şekilde yazdırılır. Yöneticiler, yazdırmayı yönetmek için Azure portal ve yazıcılara yerel destekle kolayca Evrensel Yazdırma. Evrensel Yazdırma yazılım kullanılarak uyumlu olmayan yazıcılarla Evrensel Yazdırma bağlayıcısı dağıtılabilir.

Evrensel Yazdırma, Windows E3, A3, E5 ve A5'e ve Microsoft 365 BP, F3, E3, A3, E5 ve A5'e geri doldurulacak.  

**Teklif ayrıntıları**

Teklif adının fiyat listesi önizlemeden biraz farklı olduğunu unutmayın.

| Teklif adı | Teklif Kimliği | Malzeme Kimliği |
| ------ |----------- |----------- |  
| Evrensel Yazdırma birim eklenti (500 iş) - Microsoft 365  | cb131356-45ee-4ae2-8537-873b706c8e75     | 9BI-00004   |
| Evrensel Yazdırma için toplu eklenti (500 iş) - Microsoft 365   | 477 sini81-9872-43d6-91d3-c72390bfcf49   | 9BK-00004   |
| Evrensel Yazdırma birim eklenti (500 iş) - Windows    | d3ddc493-5741-4e0d-a02d-07edbb0bb72e   | 9BI-00002   |
| Evrensel Yazdırma için toplu eklenti (500 iş) - Windows   |  d0862f05-80f5-4fd4-8432-fe72dd893cc7  | 9BK-00002   |

### <a name="next-steps"></a>Sonraki adımlar

Fiyat listesi ve genel bakış hakkında bilgi [Evrensel Yazdırma edinebilirsiniz.](/universal-print/fundamentals/universal-print-whatis) Bu bilgileri, kuruluşta tüm uygun kişiler ile paylaşın.

### <a name="questions"></a>Sorularınız mı var?

Bu teklifler hakkında sorularınız varsa ilgili topluluklar için Yammer kontrol edin.