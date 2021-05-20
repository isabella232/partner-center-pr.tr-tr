---
title: Mart 2021 duyuruları
description: Yeni özellikler, promosyonlar, teklifler, pazarlar İş Ortağı Merkezi mevcut tekliflerde yapılan değişiklikler dahil olmak üzere Microsoft İş Ortağı Merkezi için Mart 2021 duyuruları.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: b503e928b1491d5c2c70ac52460080f9e1ba91b8
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150123"
---
# <a name="march-2021-announcements"></a>Mart 2021 duyuruları

Bu sayfa, Mart 2021 için Microsoft İş Ortağı Merkezi duyurularını sağlar.

## <a name="readiness-changes-to-the-cloud-solution-provider-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="18"></a>Hazır olma: Bulut Çözümü Sağlayıcısı (CSP) müşteri adresi doğrulama API'sinde yapılan değişiklikler Haziran ayında yayınlanacak; test özelliği artık kullanılabilir

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-30
- Hazır Olma

### <a name="summary"></a>Özet

İş ortaklarının ve müşterilerin işletmelerini güvene dayalı olarak çalıştırmalarına yardımcı olmak için, iş ortaklarını dünya genelindeki tüm ülkeler için Adresi Doğrula API'lerinde yapılan değişiklikleri test etmeye davet ediyoruz.

### <a name="impacted-audience"></a>Etkilene hedef kitle

CsP doğrudan fatura iş ortakları ve mevcut müşterilerin adres ayrıntılarını yeni veya güncelleştiren dolaylı sağlayıcılar.

### <a name="details"></a>Ayrıntılar

Microsoft güven üzerinde çalışır. CSP programında müşteri aboneliklerinin işlemesi için uyumlu, güvenli ve güvenli bir müşteri adresi doğrulama yöntemi sağlama konusunda kararlıyız. 31 Mart 2021'den baş olarak, Haziran 2021'de yapılan değişikliklerle canlı yayına devam etmek için iş ortaklarını test etmek için davet edilen Adresi Doğrula API'sinde değişikliklere yer verdik.

Değişiklikler yalnızca Adresi Doğrula API'sini etkiler. Müşteri Oluşturma ve Faturalama Profili API'lerini güncelleştirme işlemi etkilenmez.

Yanıt aşağıdaki durum iletilerinden birini geri dönecektir:

| Durum     | Açıklama |    Döndürülen önerilen adres sayısı |
|-------|---------------|-------------------|
|Doğrulanmış gönderilebilir | Adres doğrulanır ve adresine gönderebilirsiniz. | Tek |
|Doğrulandı | Adres doğrulandı. | Tek |
|Etkileşim gerekli | Önerilen adres önemli ölçüde değiştirildi ve kullanıcı onayı gerekiyor. | Tek |
|Cadde kısmi | Adreste verilen cadde kısmi ve daha fazla bilgi gerekiyor. | Birden çok — en fazla üç |
|Şirket içi kısmi | Verilen şirket içi (bina numarası, paket numarası ve diğerleri) kısmi ve daha fazla bilgi gerekiyor. | Birden çok — en fazla üç |
|Birden çok | Adreste kısmi olan birden çok alan vardır (büyük olasılıkla cadde kısmi ve şirket içi kısmı da dahil). | Birden çok — en fazla üç |
|Hiçbiri | Adres yanlış. | Hiçbiri |
|Doğrulanmamış | Adres, doğrulama işlemi aracılığıyla gönderilemedi. | Hiçbiri |

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

- 31 Mart 2020: Özgün yayın

- 30 Nisan 2021: Örnek yanıt ve Posta kodu ayrıntıları için güncelleştirmeler

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a>Yeni Exchange yönetim merkezi (EAC) deneyimi

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-29
- Özellikler

### <a name="summary"></a>Özet

27 Nisan 2021'den başlayarak, Exchange yönetim merkezi (EAC) kullanıcılar için günlük verimliliği geliştirecek yeni bir deneyim sunuyor.

### <a name="impacted-audience"></a>Etkilene hedef kitle

Exchange'e İş Ortağı Merkezi üzerinden erişen yönetici temsilcileri

### <a name="details"></a>Ayrıntılar

27 Nisan 2021'den başlayarak, İş Ortağı Merkezi aracılığıyla Exchange'e gelen iş ortakları yeni EAC'ye yeniden yönlendirecek.

Bu yeni deneyim şu anda önizleme olarak sunulmaktadır ve yöneticiler klasik EAC'nin sağ üst köşesindeki iki durumlu düğmeyi seçerek bu deneyimi etkinleştir kullanılabilir. Ayrıca tüm sayfalarda görüntülenen "Şimdi deneyin" başlığı seçerek yeni EAC'ye de gidebilirsiniz.

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

Bu değişikliklerle ilgili sorularınız için ilgili Yammer topluluklarınızı kontrol edin.

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

- Yeni müşteri ekleme veya mevcut müşteri ayrıntılarını değiştirme ile ilgili ek verileri gönderdiğinizden emin olun.

- Denetim masası satıcısı (CPV) çözümü kullanıyorsanız CPV'nize başvurun.

### <a name="questions"></a>Sorularınız mı var?

Yasal tanımlayıcıyla (INN veya TIN olarak da adlandırılan) ilgili sorularınız varsa vergi danışmanınıza veya yerel vergi ofisinize ulaşın. Microsoft, vergiler konusunda rehberlik sağamaz.

Microsoft ile işlemleriniz için de destek gerekirse [bir hizmet isteği açın.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a>1 Mart 2021 kalıcı yazılım fiyat listesinde yapılan düzeltmeler

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-23
- Teklifler/Pazarlar

### <a name="impacted-audience"></a>Etkilene hedef kitle

Dolaylı sağlayıcılar ve doğrudan fatura iş ortakları, Bulut Çözümü Sağlayıcısı programı 

### <a name="details"></a>Ayrıntılar

1 Mart 2021'de yayınlanan kalıcı yazılımların fiyat listesi, orada yer almamaları gereken pazarları da içerir. Kalıcı yazılım fiyat listesi, düzeltmelerle birlikte 17 Mart 2021'de güncelleştirildi. Bu düzeltmeler yalnızca şular için geçerlidir:

- Ürün Kimliği: DF77X4D43RKT 
- Ürün adı: Windows 10 Home İş için Pro Microsoft 365 Yükseltme
- Kaldırılan veya desteklenmeyen pazarlar: AE, AF, AL, AM, AO, BA, BB, BD,EŞ, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, NDE, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG , NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW

Bu değişiklikler yalnızca yukarıdaki ürün için geçerlidir. Diğer ürünlerin hiçbir düzeltmesi yoktu. 

### <a name="next-steps-and-resources"></a>Sonraki adımlar ve kaynaklar

- Kalıcı yazılım işlemi yapan iş ortakları en son kalıcı yazılım fiyat listesini indirmeli.
- İki [harfli kısaltmanın](/azure/marketplace/commercial-marketplace-co-sell-countries) ülkelerle kolay bir eşlemesi için bölge ülke kodlarına bakın.
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

- Katalog Değişiklikleri:

  - GET /products/{product-id}/skus/{sku-id}

- Satın Alma ve Yönetme:
  - GET /customers/{customerId}/subscriptions
  - GET /customers/{customerId}/subscriptions/{subscriptionId}
  - PATCH /customers/{customerId}/subscriptions/{subscriptionId}
  - GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities
  - GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions
  - POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions

### <a name="next-steps"></a>Sonraki Adımlar

- En son [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)
- [GitHub](https://github.com/Microsoft/Partner-Center-DotNet-Samples) örneklerini indirme ve gözden geçirme

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a>Uygun teklifler için CSP ticari market teklifi ve FY21 CSP teşvikleri

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-18
- Özellikler

### <a name="impacted-audience"></a>Etkilene hedef kitle

Bulut Çözümü Sağlayıcısı programında dolaylı sağlayıcılar ve doğrudan Bulut Çözümü Sağlayıcısı ortakları 

### <a name="details"></a>Ayrıntılar

Bulut Çözümü Sağlayıcısı programı kapsamındaki dolaylı sağlayıcılar ve doğrudan fatura iş ortakları üçüncü taraf teklifleri satıp İş Ortağı Merkezi veya Azure portal'da işlem yapılan her uygun üçüncü taraf teklifi için indirim teşviki Azure portal. Teşvik, uygun teklifler için faturalandırmış satışlara yönelik bir indirim şeklinde olacak ve **30 Haziran 2021'e** kadar kullanılabilir.  

Aşağıda bu CSP Ticari Market Teklifi teşvikini öğrenmeye devam edin ve müşterilerinizle iletişime geçerek başarılarının ve dijital dönüşümlerinin devam etmesini sağlamak için doğru teklifleri belirlemelerini sağlar.

En son IaaS ve SaaS çözümlerini Microsoft müşterilerine sunmak için Bağımsız Yazılım Satıcıları (ISV) ile birlikte çalışıyoruz. ISV yayımcıları, Microsoft iş ortağı kanalı aracılığıyla tekliflerinin satışlarını etkinleştirme seçeneğine sahip olur. Özendiğimiz tekliflerimiz iki kategoride yer almalıdır:

- Azure IP ortak satış incentivized durumu ile SaaS ve IaaS üçüncü taraf tekliflerini seçin. 

- Ekipler ile tümleştirilmiş SaaS uygulamaları veya PowerPoint, Word, Excel, Outlook veya SharePoint gibi en az iki Microsoft 365 üretkenlik uygulaması.

### <a name="next-steps-and-resources"></a>Sonraki adımlar ve kaynaklar

- Uygun Market uygulamaları satmaya uygun olan uygulamaları teşvik etmek için [Iş ortağı teşvikleri](https://partner.microsoft.com/membership/partner-incentives) hakkında bilgi edinin. Yeni teklifler aylık olarak eklenir.  
- [Bulut çözümü sağlayıcısı doğrudan fatura ortağı özendirme kaynakları](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [Bulut çözümü sağlayıcısı dolaylı sağlayıcı, kaynakları teşvik edin](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- Ticari market uygulamalarını satma hakkında daha fazla bilgi edinmek için bu [sunuyu](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) gözden geçirin. Ek kaynaklara [buradan](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/)göz atın. 
- [Iş Ortağı Merkezi](../csp-commercial-marketplace-discover.md) veya [Azure Portal](https://ms.portal.azure.com/#home) ticari Market kataloğunu keşfet
- Uygulamaları şirketinizin marketi ile bütünleştirmek için [API 'leri](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) kullanma
- İş yaparken ilgilendiğiniz ISV 'lere ulaşın
- Dolaylı sağlayıcıların, hangi uygulamaların satmaya yönelik API 'Leri ve kılavuz satıcılarını kullanarak tümleştirmeleri gerekir

### <a name="questions"></a>Sorularınız mı var?  

Iş Ortağı Merkezi 'nde ticari Market 'e genel bakış için [Bu makaleye](../csp-commercial-marketplace-overview.md) başvurun.

Daha fazla yardıma ihtiyacınız varsa, Iş Ortağı Merkezi 'nde bir destek isteği oluşturabilirsiniz. Daha fazla bilgi edinin [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a>Power BI Premium teklif adlandırma ve önkoşul güncelleştirme

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-18
- Özellikler

### <a name="summary"></a>Özet

1 Nisan 2021 son fiyat listesi, Kullanıcı başına Power BI Premium için adlandırma ve/veya önkoşul bilgilerine açıklık eklemek üzere güncelleştirilir.

### <a name="impacted-audience"></a>Etkilene hedef kitle

Bulut Çözümü Sağlayıcısı (CSP) doğrudan ve dolaylı iş ortakları

### <a name="details"></a>Ayrıntılar

1 Nisan 2021 son fiyat listesi, Kullanıcı Başına tekliflere ilişkin adlandırma ve/veya önkoşul bilgilerine açıklık Power BI Premium güncelleştirilecek.

Son fiyat listesi güncelleştirilene kadar doğru ürünün sipariş olduğundan emin olmak için bu bölümdeki bilgileri kullanın.

Aşağıdaki ayrıntılar etkilenen SKU ve önkoşul ayrıntılarını gösterir.

| Teklif görünen adı: 1 Mart fiyat listesi önizlemesi |  Teklif görünen adı 1 Nisan son fiyat listesinde güncelleştirildi| Teklif Kimliği |
| ------ | ----------- | ----------- |
| Power BI Premium Başına Add-On (Kar Amacı Gütmeyen Personel Fiyatlandırması)  |  Power BI Premium Başına Add-On **(Office)** (Kar Amacı Gütmeyen Personel Fiyatlandırması)   | 31c03289-47ab-4ab0-8df1-03742c127ac6   |

Müşterilerin bu teklifi satın almak için aşağıdaki önkoşullardan herhangi birinin olması gerekir:

| Teklif görünen adı | Teklif Kimliği |
| ------ | ----------- |
| Microsoft 365 E5 (Kar Amacı Gütmeyen Personel Fiyatlandırması)  |  31bedf01-9e57-4ece-a53a-d3656a563931   |
|   Microsoft 365 Konferanssız E5 (Kar Amacı Gütmeyen Personel Fiyatlandırması)|  b456810a-c414-4e07-98fc-ef74e8175a09|
|   Office 365 E5 (Kar Amacı Gütmeyen Personel Fiyatlandırması)| ce139fe5-8bd5-47ed-a5be-07c286f8b9e    |
|   Office 365 E5 (Kar Amacı Gütmeyen Personel Fiyatlandırması) Deneme Sürümü|  2f192efe-608a-4c9c-9d19-2b0b70b0962e|
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

| Teklif adı | Para Birimi | Teklif Kimliği | Malzeme Kimliği |
| ------ |----------- |----------- |----------- |
| Microsoft 365 F3 (ÖİP) | GBP | 57b722c2-c435-4bfb-9bc8-80509213a13a | AAD-11626 |
| Microsoft 365 F3 (Ticari) | EUR| 3451a3b0-8cda-44a7-bad7-c30be81c4aaa | AAA-89898 |
 
Mart ve Nisan önizleme lisans tabanı fiyat listeleri 16 Mart 17:00 Pasifik standart saatiyle güncelleştirildi.

### <a name="next-steps"></a>Sonraki adımlar

- İş ortaklarının geçerli lisans tabanlı fiyat listelerini (Mart ve Nisan önizlemesi) yeniden yüklemesi ve varsa bu fiyat düzeltmelerini de yüklemesi gerekir.  
- Microsoft, etkilenen işlemlerin düzeltilmesiyle ilgili sonraki adımları bildirmek için önümüzdeki haftalarda e-posta yoluyla etkilenen iş ortaklarıyla iletişim kuracak.

### <a name="questions"></a>Sorularınız mı var?

Diğer sorularınız için lütfen ilgili CSP Yammer topluluklarınızı kontrol edin.

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> Yasal şirket adını İş Ortağı Merkezi

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-16
- Sürücü Verimliliği & Ölçeklendirme

### <a name="summary"></a>Özet

Mart 2021'den başlayarak Microsoft İş Ortağı Ağı (MPN) iş ortakları ve Bulut Çözümü Sağlayıcısı (CSP) dolaylı kurumsal bayileri yasal şirket adını İş Ortağı Merkezi.

### <a name="impacted-audience"></a>Etkilene hedef kitle

MPN iş ortakları ve CSP dolaylı kurumsal bayileri (CSP doğrudan fatura iş ortakları için geçerli değildir)

### <a name="details"></a>Ayrıntılar

Mart 2021'den başlayarak MPN iş ortakları ve CSP dolaylı kurumsal bayileri, yasal şirket İş Ortağı Merkezi uyumlu ve self servis bir şekilde güncelleştirebilmektedir. Bu yeni özellik sayesinde iş ortaklarının şirket adını güncelleştirmek için İş Ortağı Merkezi destek bileti göndermesi gerekmeyecek. Bu, bu etkinlikleri gerçekleştirerek iş ortakları için önemli miktarda zaman tasarrufu sağlar. 

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

- 7 Temmuz 2021: Iki ticari teklif, orijinal Windows ve Visual Studio Professional edinme ve kamu sektörü teklifleri (kamu, eğitim ve kar amacı: [duyuru](./2020-december.md#9)), CSP kalıcı yazılım fiyat listesine eklenecektir.  Fiyat listesi, İş Ortağı Merkezi'daki [> Fiyatlandırma & Teklifleri](https://partnercenter.microsoft.com/pcv/sales) sayfasının Yazılım bölümünde bulunabilir ve bu tarihte yeniden yayımlanmaz.

CSP programı evrimi ve Açık Lisans programı değişiklikleriyle ilgili tüm ayrıntılar için lütfen aşağıdaki **Sonraki Adımlar'a** bakın.

### <a name="next-steps"></a>Sonraki Adımlar:

- CSP Programı evrimi: Program [hazırlığı malzemelerini Bulut Çözümü Sağlayıcısı Kalıcı yazılımı](https://partner.microsoft.com/resources/collection/software-in-csp#/) gözden geçirme. Rolünüz [için doğru bilgileri](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) hızla bulmak üzere bu hazır olma haritasını kullanın.

- Açık Lisans programı değişiklikleri: CSP programı [evrimini ve Açık Lisans programı değişikliklerinin hazırlık malzemelerini](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) gözden geçirme. Rolünüz [için doğru bilgileri](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) hızla bulmak üzere bu hazır olma haritasını kullanın.

### <a name="questions"></a>Sorular

Diğer sorularınız için lütfen ilgili CSP Yammer topluluklarınızı kontrol edin.

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a>Önceki duyuruya güncelleştirin: Uyumluluk Yöneticisi'ne bir eklenti olan Premium Değerlendirmeler

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

- [Microsoft 365 E5 güvenliği ve uyumluluğu](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [Microsoft Uyumluluk Yöneticisi'nde değerlendirmeleri oluşturma ve yönetme - Microsoft 365 Uyumluluğu](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a>Sonraki adımlar

Bu konu başlığıyla ilgili kaynakları gözden geçirme ve bu bilgileri kuruluşta uygun proje katılımcıları ile paylaşma.

### <a name="questions"></a>Sorularınız mı var?

Bu teklifler hakkında sorularınız için ilgili Yammer topluluklarınızı kontrol edin.

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> Çözümlerinizi Bir Ticari İş Ortağından (OCP) pazara satışa (GTM) Microsoft ticari markete geçirme

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

Sorularınız [varsa](https://partner.microsoft.com/support/?stage=1) veya daha fazla bilgiye ihtiyacınız varsa Destek ile iletişime geçin.

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a>Azure'dan Rusya'ya Bulut Çözümü Sağlayıcısı (CSP) programı kapsamındaki yeni ticaret deneyimini genişletme

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-10
- Özellikler

### <a name="impacted-audience"></a>Etkilene hedef kitle

Bulut Çözümü Sağlayıcısı (CSP) programı aracılığıyla işlem Bulut Çözümü Sağlayıcısı Rusya'daki tüm iş ortakları.

### <a name="details"></a>Ayrıntılar

10 Mart 2021'den başlayarak, Rusya'da Azure için CSP'de yeni ticaret deneyiminin **kullanılabilirliğini duyurmak için heyecanlanıyoruz.** Bu deneyim, müşterilerin Azure hizmetlerini satın alma ve tüketme yolunu kolaylaştıracak ve geliştirecektir. Ayrıca CSP programı iş ortaklarına satış hareketlerine göre Azure fiyatlandırmasını tutarlı bir şekilde görüntüleme, küresel tutarlılık için USD fiyatlandırması, faturalama tarihi hizalaması ve azure fiyatlandırması Azure Maliyet Yönetimi.

### <a name="next-steps"></a>Sonraki adımlar

Yeni Azure ticaret deneyimini tanıtan ve ek bilgiler sağlayan birçok kaynak vardır. CSP Program Güncelleştirmeleri Kaynak Galerisi'nde en son [SSS,](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/)desteler, video ve daha fazlasını bulabilirsiniz.

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a>İş Ortağı Merkezi lisans anahtarını yükleme ve yerine getirme

### <a name="categories"></a>Kategoriler

- Tarih: 2021-03-04
- Özellikler

### <a name="summary"></a>Özet

Yazılım İş Ortağı Merkezi ve lisans anahtarı yerine getirme özelliği yeniden getirildi.

### <a name="impacted-audience"></a>Etkilene hedef kitle

Tüm Bulut Çözümü Sağlayıcısı (CSP) iş ortakları, yazılım aracılığıyla kalıcı ve sunucu aboneliği yazılım siparişlerini İş Ortağı Merkezi

### <a name="details"></a>Ayrıntılar

İş ortağı geri bildirimlerine yanıt olarak, kalıcı ve İş Ortağı Merkezi abonelik yazılım siparişleri için yazılım ve lisans anahtarları alma olanağını yeniden hazırlarız. 19 Ocak 2021'de kaldırılmasından önceki durumuna geri yüklenecektir. (Duyuruya [bakın.)](2020-september.md#17)

Yazılım lisans anahtarları ve indirme bağlantılarının değerli ve son derece aranılan fikri mülkiyet varlıkları olduğunu unutmayın. Sızdırıldıklarında etkinleştirme sınırları hızla tükenebilir ve olumsuz müşteri ve iş ortağı deneyimine neden olabilir.

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

1 Nisan 2021'de Microsoft aşağıdaki yeni ürünleri ve teklifleri başlatacak:

- Power BI Premium Kullanıcı Başına
- Customer Voice and Marketing USL coğrafi ve segment genişletmesi

**Power BI Premium Kullanıcı Başına**

Microsoft, kullanıcı başına ilk kullanıcı başına Power BI Premium tanıtacak. Power BI Premium şu anda yalnızca bir kapasite yapısında satılıyor. Power BI Premium Kullanıcı Başına kurumsal iş zekası (BI) ve analiz özelliklerine erişim sağlar. Esnek bireysel lisanslama, küçük ve orta ölçekli işletmelere hitap ediyor.

Bu teklif [Power BI daha fazla bilgi](/power-platform-release-plan/2020wave2/power-bi/planned-features) edinmek için yayın ayrıntılarını gözden geçirme.


**Teklif ayrıntıları**

Teklif adının fiyat listesi önizlemeden biraz farklı olduğunu unutmayın.

| Teklif adı | Teklif Kimliği |
| ------ |----------- |
| Power BI Premium Kullanıcı Başına | 9c810018-9356-4903-95ab-eeb956289290 | 
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
| Fakülteler için Dynamics 365 müşteri sesi USL | 85162d70-9676-4cf6-a4bc-a0d6672f2657 |

Bu teklifler hakkında daha fazla bilgi için aşağıdaki sayfaları ziyaret edin:

- [Dynamics 365 Müşteri Hizmetleri Ses giriş sayfası](https://dynamics.microsoft.com/customer-voice/overview/)
- [Dynamics 365 Marketing giriş sayfası](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a>Sonraki adımlar

Bu konu başlığı altında yer alan kaynakları gözden geçirin ve bu bilgileri, kuruluşta uygun proje katılımcıları ile paylaşın.  

### <a name="questions"></a>Sorularınız mı var?

Bu teklifler hakkında sorularınız için ilgili Yammer topluluklarınızı kontrol edin. 

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

[Evrensel Yazdırma,](https://aka.ms/universalprint) şirket Microsoft 365 sunucularına olan ihtiyacı ortadan kaldıran ve Windows cihazlarının Azure'a kayıtlı yazıcılara yazdırmasını sağlayan bir yazdırma hizmetidir. 1 Mart 2021'den itibaren işlem için kullanılabilir olacak.

Çalışanlar sürücüsüz yazdırma, kolaylaştırılmış konum tabanlı yazıcı bulma ve öğrenme eğrisi olmayan sezgisel yazdırma deneyiminden faydalanıyor. Azure Active Directory (Azure AD) ile katılan cihazlar, mevcut Azure AD kimlik bilgilerini kullanarak güvenli bir şekilde yazdırılır. Yöneticiler, yazdırmayı yönetmek için Azure portal ve yazıcılara yerel destekle kolayca Evrensel Yazdırma. Evrensel Yazdırma yazılım kullanılarak uyumlu olmayan yazıcılarla Evrensel Yazdırma bağlayıcısı dağıtılabilir.

Evrensel Yazdırma Windows E3, A3, E5 ve A5'e ve Microsoft 365 BP, F3, E3, A3, E5 ve A5'e geri doldurulacak.  

**Teklif ayrıntıları**

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