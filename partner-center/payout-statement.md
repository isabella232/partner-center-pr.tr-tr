---
title: Ödeme deyimleri
description: Ödeme deyimleri ve özetler hakkında bilgi edinin ve Microsoft Iş Ortağı Merkezi 'nden ödeme verilerinizi nasıl görüntüleyip dışarı aktarabilirsiniz?
ms.subservice: partnercenter-payouts
ms.service: partner-dashboard
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 3/22/2021
ms.openlocfilehash: d95927db27d7dfd05b8f29a6536658c3210f9b05
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248669"
---
# <a name="payout-statements"></a>Ödeme deyimleri

**Uygun roller**: Hesap Yöneticisi | Genel yönetici

**Ödeme beyanı** , ticari Market aracılığıyla satılan tekliflerden ödemalarınızın genel bir görünümünü sunar. Kazanlarınızın işlem geçmişini gösterir, bir sonraki ödemenizi tahmin eder ve ödeme eğilimlerini gösterir. Ayrıca, işlem geçmişi ve ödeme deyimlerini indirebilirsiniz. Bu makalede, ödeme deyiminize ve Iş Ortağı Merkezi 'nde size erişilebilen farklı ödeme sayfalarına ve indirmelere nasıl erişebileceğiniz açıklanır.

>[!NOTE]
>Yalnızca MPN kimlikleri ve sizinle ilişkilendirdiğiniz programlar için verileri görürsünüz. Ek verileri görmek isterseniz, izinler için hesap yöneticinizle birlikte çalışın. 

## <a name="roles-and-permissions"></a>Roller ve izinler

Bir ödeme bildirimine erişmek için **hesap sahibi** veya **mali katkıda bulunan** rolü atanması gerekir.

| Raporlar/sayfalar | Hesap sahibi | Yönetici | Geliştirici | İş Katılımcısı | Finans Katılımcısı | Pazarlamacısıdır |
| --- | --- | --- | --- | --- | --- | --- |
| Alım raporu (neredeyse gerçek zamanlı veriler dahil) | Görüntüleyebilir | Görüntüleyebilir | Erişim yok | Erişim yok | Görüntüleyebilir | Erişim yok |
| Geri bildirim raporu/yanıtları | Geri bildirim görüntüleyebilir ve gönderebilir | Geri bildirim görüntüleyebilir ve gönderebilir | Geri bildirim görüntüleyebilir ve gönderebilir | Erişim yok | Erişim yok | Geri bildirim görüntüleyebilir ve gönderebilir |
| Sistem durumu raporu (neredeyse gerçek zamanlı veriler dahil) | Görüntüleyebilir | Görüntüleyebilir | Görüntüleyebilir | Görüntüleyebilir | Erişim yok | Erişim yok |
| Kullanım raporu | Görüntüleyebilir | Görüntüleyebilir | Görüntüleyebilir | Görüntüleyebilir | Erişim yok | Erişim yok |
| Ödeme hesabı | Güncelleştirebilir | Erişim yok | Erişim yok | Erişim yok | Güncelleştirebilir | Erişim yok |
| Vergi profili | Güncelleştirebilir | Erişim yok | Erişim yok | Erişim yok | Güncelleştirebilir | Erişim yok |
| Ödeme özeti | Görüntüleyebilir | Erişim yok | Erişim yok | Erişim yok | Görüntüleyebilir | Erişim yok |
|

## <a name="access-your-payout-statement"></a>Ödeme deyiminize erişin

[Iş Ortağı Merkezi](https://partner.microsoft.com/dashboard/home) ' nde oturum açın ve bu farklı özetlere erişmek için ekranın sağ üst köşesindeki ödeme simgesini seçin:

- İşlem geçmişi
- Ödemeler
- Verileri dışarı aktarma

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Iş Ortağı Merkezi portalının sağ üst köşesindeki ödeme simgesini gösterir.":::

Ayrıca, [Iş ortağı ödeme API](/rest/api/partner-center/partner-payouts) 'sini kullanarak doğrudan ödeme ve ödeme verilerini alabilir ve elde edebilirsiniz. [Ödeme HIZMETLERI API 'sini kullanarak ödemeleri yönetme](/partner-center/develop/manage-payouts)hakkında daha fazla bilgi edinin.


## <a name="transaction-history"></a>İşlem geçmişi

**İşlem geçmişi** sayfasında, son 36 aya göre kazanç, tahmini bir sonraki ödeme ve kazanç ve ödemeler eğilimi gösterilir. Ayrıca, bu bölümden işlem ayrıntılarını indirebilirsiniz.<br><br>Bu rapor, henüz gönderilmemiş ödemeler dahil olmak üzere, ödeme için uygun olan tüm gelirleri gösterir. Bir ISV, Iş Ortağı Merkezi 'ndeki tüm banka ve vergi bilgilerini tamamladıktan sonra kazanç $50 >, ISV hesabı etkin ve müşterinin faturalandırıldığı (EA işlemleri için) veya ödeme alındığı zaman (EA işlemleri için) ödemiştir.

:::image type="content" source="images/payouts/transaction-overview.png" alt-text="İşleme genel bakış.":::

- **Bu yıla gönderilen kazançlar** – ödenen ve gelecek ayda ödenen toplam kazanç ve döküm dökümü.
- **Tahmini ödeme ayı** – yaklaşan aylarda beklenen toplam kazanç.
- **Kazanç ve ödeme eğilimi** – son 36 aylar için aylık kazanç ve ödeme tutarları.
- **İndir** – işlem ayrıntılarını .csv veya. tsv biçiminde indirin.

Son 3, 6, 12 veya 36 ayı göstermek için sayfanın çıktısını filtrelemek üzere sayfanın sağ üst köşesindeki tarih aralığı seçimini kullanın. Ya da 36 aya kadar bir özel tarih aralığı seçin. Varsayılan tarih aralığı 12 aydır. Kayıt KIMLIĞI, program, ödeme KIMLIĞI, kazanç türü, MANI ve duruma göre de filtre uygulayabilirsiniz. Veriler geçerli mali yıl (1 Temmuz 30 Haziran) ve önceki iki mali yıl için kullanılabilir.

:::image type="content" source="images/payouts/search-filter.png" alt-text="Sayfanın sağ üst kısmındaki arama filtresi.":::

Bir atma hakkında daha fazla ayrıntı görmek için sayfanın sağ tarafındaki aşağı oku seçin. Bunun yapılması manı, gelir tutarını, ürünü ve müşteriyi görüntüler. Herhangi bir nedenden dolayı bu verilerden herhangi biri kullanılamaz, ancak ona erişmeniz gerekiyorsa, desteğe başvurun. Kazanım, bir işlem değil, bir ayarlamanın sonucu ise, ürün ve müşteri alanları gösterilmez.

### <a name="transaction-history-summary"></a>İşlem geçmişi Özeti

Bu görünüm, ürün ve tahmini ödeme ayından oluşan ürünün kazanç kaynağı dahil olmak üzere kazanç ayrıntılarını gösterir.

:::image type="content" source="images/payouts/transaction-history.png" alt-text="İşlem geçmişi.":::

- **Kazanılan tarih** : satın alma tarihi.
- **Kazanç türü:** Satış, İndirim veya Ortak satış gibi kazanç türü.
- **Toplam tutar:** Net kazanç tutarı. Ticari markette bu, standart market ücretinin düşüldüğü anlamına gelir.
- **Durum–** Üç seçenek vardır:
    - **Yaklaşan –** Kazançlar beklemede soğutma süresinde.
    - **İşlendi:** Kazançlar sonraki ödeme için hazırlanır.
    - **Sent:** Kazançlar ödendi.
- **Tahmini ödeme ayı:** Kazançların ödeneceği ay. Daha fazla [bilgi için sonraki](#estimated-payment-month) bölüme bakın.

Kazanç işlemleri, işlem ödeme uygunluğunu karşılarken gösterilir. Neden eksik veya beklenmeyen kazançlarınız olabileceğini anlamak için [bkz. Ticari market ödemeleri hakkında sık sorulan sorular.](payout-faq.yml#why-are-my-earnings-missing-)

#### <a name="estimated-payment-month"></a>Tahmini ödeme ayı

İşlem Geçmişi sayfası artık sonraki birkaç ay için tahmini ödeme tutarlarınızı gösteren bir tablo içerir. Ayrıca bu bilgileri İşlem geçmişi ve Özet raporu dışarı aktarmalarında da indirebilirsiniz. Bu bilgiler mutabakatları ve ödeme tahminlerini kolaylaştırır.

Tahmini ödeme ayı, program yapılandırma kurallarına ve zaman çizelgelerine göre hesaplanır ve sonraki/sonraki ödeme döngüsünde işlenir.

Tahmini ödeme ayı şu anda ortak çalışma dışındaki tüm kazanç türlerinde kullanılabilir ve geçerli değil **olarak görüntülenir.** 1 Temmuz 2020'den önceki kazançlar için Tahmini ödeme ayı Kullanılabilir değil **olarak görünür.**

Aşağıdaki tabloda tahmini ödeme ayı örneği yer alır.

| Ay | Miktar |
| ------ | :-----------: |
|  Eylül 2020 |  7.273,99 ABD doları   |
|  Ekim 2020 | 8.692,30 ABD doları  |
|  Nov-2020 | 107,89 ABD doları  |

Tahmini miktar, çeşitli nedenlerle gerçek tutardan farklı olabilir:

- Kazanç yeniden ifadesi: Kazançlar yeniden hesaplanırsa gerçek tutar farklı olur
- Ayarlamalar: Gerçek tutar, yapılan veya gönderilen düzeltmelere bağlı olarak değişir.
- Kuralların Değişmesi: Kurallarda yapılan bir değişiklik, ödenen gerçek tutarda yeniden hesaplamayı yansıt olabilir
- Ödeme: Ödeme hatası oluşursa gerçek tutar farklı olabilir

Ödemenizin yalnızca program eşiğine ve ödeme uygunluk kurallarına uyulması şartıyla, proje ay içinde serbest bırakılmıştır. Bu kurallar arasında aşağıdakiler yer almaktadır ancak bunlarla sınırlı değildir:

- Vergi profilinizin güncel olması gerekir
- Kazançlarınız program kılavuzunda tanımlanan minimum kazanç eşiğini karşılamalı veya aşmalı.
- Ödeme tutmada: Profil atama sayfasında "Ödememi tut" seçeneğini belirtin.
- Ödeme aracı kullanılamıyor: Ödeme veya/ve Vergi profili tamamlanmadı.

### <a name="transaction-history-download"></a>İşlem geçmişi indirme

Kazanç hakkında daha fazla ayrıntı görmek için sayfanın **üst kısmından** İndir'i seçin. Aşağıdaki tabloda, rapordaki her sütun açık bir şekilde açık bir şekilde açık bir şekilde ve açıklamadır.

>[!NOTE]
>İşlem geçmişi indirme dışarı aktarma işlemi Ağustos 2020'den itibaren iki yeni alan içerir:
>
>- **lastPaymentCurrency**  Oturum açmış olan iş ortağının erişimi olan tüm MPN'lerde en son ödemenin alın aldığı para birimi. Ödeme alınmayacaksa son ödeme para birimi ABD doları olur.
>- **earningAmountInLastPaymentCurrency**  Son ödeme para birimi cinsinden kazanç tutarı.

| Sütun adı | Description | Teşvik programları/marketler için uygulanabilirlik |
| --- | --- | --- |
| agreementEndDate | Sözleşme bitiş tarihi | Teşvikler - yalnızca bazı programlar |
| agreementNumber | Anlaşma numarası | Teşvikler - yalnızca bazı programlar |
| agreementStartDate | Sözleşme başlangıç tarihi | Teşvikler - yalnızca bazı programlar |
| calculationDate | Kazançların sistemde hesaplanma tarihi | Tümü |
| claimId | Talep için benzersiz tanımlayıcı | Teşvikler - yalnızca bazı programlar |
| customerCountry | Müşteri ülkesi/bölgesi | Pazaryerleri |
| customerEmail |  |  |
| Müşteriadı | Boş olabilir | Yalnızca teşvik programları (özel durum: OEM) ve marketler. CSP işlemleri için marketler CSP'nin adını gösterir |
| customerTenantId |  |  |
| distributorId | Dağıtımcı tanımlayıcısı | Teşvikler - yalnızca bazı programlar |
| distributorName | Dağıtımcı adı | Teşvikler - yalnızca bazı programlar |
| earningAmount | Özgün işlem para birimi cinsinden Kazanç Tutarı | Tümü |
| earningAmountInLastPaymentCurrency | Son ödeme para birimi cinsinden kazanç tutarı (önceden ödeme yapılan bir ödeme yoksa alan boş olur) |  |
| earningAmountUSD | USD Olarak Kazanç Tutarı | Tümü |
| earningDate | Kazanç tarihi | Tümü |
| earningExchangeRate | Exchange ABD doları tutarını göstermek için kullanılan fiyat | Tümü |
| earningId | Her kazanç için benzersiz tanımlayıcı | Tümü |
| earningRate | Kazanç elde etmek için işlem tutarına uygulanan teşvik oranı | Tümü |
| earningType | Bunun ücret, indirim, ortak çalışma, satış gibi bir şey olup olduğunu gösterir | Tümü |
| exchangeRateDate | Exchange USD değerini hesaplamak için kullanılan fiyat tarihi | Tümü |
| externalReferenceId | Programın benzersiz tanımlayıcısı | Doğrudan Ödeme programları (teşvikler ve marketler) |
| externalReferenceIdLabel | Benzersiz tanımlayıcı etiketi | Doğrudan Ödeme programları (teşvikler ve marketler) |
| instantRebateAmount |  |  |
| invoiceDate |  |  |
| invoiceNumber | Fatura numarası (yalnızca kuruluş için geçerlidir) | Teşvikler ve marketler - yalnızca bazı programlar |
| lastPaymentCurrency | Son ödeme para birimi (önceden ödeme yapılan bir ödeme yoksa alan boş olur) |  |
| Kolu | Kazanç için iş kuralını gösterir | Tümü |
| LicensingProgramName | Lisanslama programının adı |  |
| LineItemId | Müşterinin faturalarında tek satır |  |
| localProviderSeller | Yerel sağlayıcı/kayıt satıcısı |  |
| Vade ayı | Tahmini ödeme ayı | Tümü |
| OrderId | Müşterinin faturasıyla ilgilidir  | Pazaryerleri |
| parentProductId | Benzersiz üst ürün tanımlayıcısı. İşlem için bir üst ürün yoksa Üst Ürün Kimliği = Ürün Kimliği. | Pazaryerleri |
| parentProductName | Üst ürünün adı. İşlem için bir üst ürün yoksa, Üst Ürün Adı = Ürün Adı. | Pazaryerleri |
| participantId | Program kapsamında kazanç elde olan iş ortağının birincil kimliği | Tümü |
| participantIdType | Teşvik programları için çoğunlukla program kimliği ve marketler için Satıcı IF | Tümü |
| katılımcıAdı | Kazanç ortağının adı | Tümü |
| partnerCountryCode | Kazanç ortağının konumu/ülkesi/bölgesi | Tümü |
| partNumber | Her zaman boş olur | Bazı teşvik programları ve marketler |
| paymentId | İşlem raporuna dahil olan tüm işlemleri ödeme raporunda belirli bir ödemeyle ilişkili olarak eşlemek için benzersiz tanımlayıcı | Tümü |
| paymentStatus | Ödeme durumu | Tümü |
| paymentStatusDescription | Ödeme durumunun kolay açıklaması | Tümü |
| productId | Benzersiz ürün tanımlayıcısı | Pazaryerleri |
| Productname | İşlemle bağlantılı ürün adı | Tümü |
| productType | Uygulama, Eklenti veya Oyun gibi ürün türü | Pazaryerleri |
| Program Kodu | Program adıyla eşlentirilen dize |  |
| programName | Teşvik/mağaza programı adı | Tümü |
| purchaseOrderCoverageEndDate | Her zaman boş olur | Teşvik programı - CRI |
| purchaseOrderCoverageStartDate | Her zaman boş olur | Teşvik programı - CRI |
| purchaseOrderType | Her zaman boş olur | Teşvik programı - CRI |
| purchaseTypeCode | Her zaman boş olur | Teşvik programı - CRI |
| miktar | Programa göre değişir. İşlem programları için faturalandır edilen miktarı gösterir | Tümü |
| reasonCode |  |  |
| resellerCountry |  |  |
| resellerId | Kurumsal bayi tanımlayıcısı | Teşvikler - yalnızca bazı programlar |
| resellerName | Satıcı adı |  |
| SkuId | Yayımlama sırasında tanımlandığı gibi SKU Kimliği. Bir teklifte çok sayıda SKU olabilir, ancak SKU yalnızca tek bir teklifle ilişkilendirilir. Teşvikler - yalnızca bazı programlar |  |
| storeFee | Uygulamayı veya eklentiyi Mağaza'da kullanılabilir yapma ücreti olarak Microsoft tarafından eldeki tutar | Pazaryerleri |
| subscriptionEndDate | Abonelik bitiş tarihi | Teşvikler - yalnızca bazı programlar |
| subscriptionId | Müşteriyle ilişkili abonelik tanımlayıcısı | Teşvikler - yalnızca bazı programlar |
| subscriptionStartDate | Abonelik başlangıç tarihi | Teşvikler - yalnızca bazı programlar |
| taxCity |  |  |
| taxCountry |  |  |
| taxRemitModel | Vergileri (satış, kullanım veya KDV/GST vergileri) sorumlu taraf | Pazaryerleri |
| taxRemitted | Atlanmış vergi tutarı (satış, kullanım veya KDV/GST vergileri) | Pazaryerleri |
| taxState | Müşterinin durumu |  |
| taxZipCode | Müşterinin posta kodu |  |
| tpan | Üçüncü taraf reklam ağına işaret | yalnızca marketplaces Ads |
| transactionAmount | Kazanç oluşturulana göre özgün işlem para birimi cinsinden işlem tutarı | Tümü |
| transactionAmountUSD | ABD doları olarak işlem tutarı | Tümü |
| transactionCountryCode | İşlem gerçekleşti ülke/bölge kodu |  |
| transactionCurrency | Özgün müşteri işlemlerinin meydana geldiği para birimi (bu iş ortağı konumu para birimi değildir) | Tümü |
| transactionDate | İşlem tarihi. Birçok işlemi tek bir kazanç için katkıda bulunan programlar için yararlıdır | Tümü |
| transactionExchangeRate | Exchange abd doları tutarını göstermek için kullanılan fiyat tarihi | Tümü |
| Transactionıd | İşlem için benzersiz tanımlayıcı | Tümü |
| transactionPaymentMethod | İşlem için kullanılan Kart, Mobil Operatör Faturalaması veya Mobil Operatör Faturalaması gibi müşteri PayPal | Pazaryerleri |
| Transactiontype | Satın alma, para iadesi, geri alma veya geri ödeme gibi işlem türü | Pazaryerleri |
| iş yükü | İş Yükü | Teşvikler - yalnızca bazı programlar |
|

### <a name="transaction-adjustment-codes"></a>İşlem ayarlama kodları

Aşağıdaki tabloda düzeltmeler için neden kodları ve açıklamaları liste almaktadır.

|**Neden kodu**   |**Açıklama**   |
|------------------|:-------------------------------------|
| AR Uyumluluğu | microsoft faturaları iş ortağı tarafından zamanında ödenmemiş olduğunda kazançları azaltan düzeltme. |
| Ortak çalışma rollover | Ortak kazançları başka bir döneme aktaran veya ortak kazançları indirime dönüştüren düzeltme. |
| İşlem Ayarlaması | Microsoft sistem hesaplama hatalarını düzelten ayarlama. |
| İşlem AyarlamaSı Microsoft yanlış hesaplaması | Yanlış hesaplamaları düzelten ayarlama. |
| İşlem AyarlamaSı Microsoft hatalı kayıt | Kayıtla ilgili yanlış hesaplamalar için ayarlama. |
| İş ortağı eşlemesi (abonelik) MCI/CSP | Abonelik yanlış hizasını düzelten düzeltme. |
| İlke Özel Durumu | Program kuralını geçersiz kılmak için ayarlama.  |
| Önceki dönem kazançları | Geçerli kazanç dönemi dışındaki kazançlar için düzeltme. |

## <a name="payments"></a>Ödemeler

Ödemeler **sayfasında,** Microsoft ile kazandığınız paraların ayrıntıları yer almaktadır. Ayrıca ne zaman ve ne kadar ödenmiş olacağını gösterir.

>[!Note]
> Ödemeye uygun olmak için gelirlerinizi 50 [ABD doları olan ödeme](payment-thresholds-methods-timeframes.md) eşiğine ulaşmanız gerekir. Daha fazla bilgi için [bkz. Microsoft Publisher Sözleşmesi.](/legal/marketplace/msft-publisher-agreement)

:::image type="content" source="images/payouts/payments-overview.png" alt-text="Ödemelere genel bakış ekranı.":::

- **Bu yılın toplam** ödemesi: Tüm programlarınız için bu yıl ABD doları olarak size ödenen birleşik toplam.
- **Sonraki tahmini ödeme:** Abd doları olarak size gelecek tek bir sonraki ödeme (yakında başka ödeme de olsa) gelir.
- **Son ödeme:** Tutarı (ABD doları), program adı ve en son ödemenizin programı.
- **Kaynak tarafından ödeme** – Son 12 ay içinde program başına yapılan ödeme miktarı (ABD doları).

### <a name="payments-list"></a>Ödemeler listesi

Ödeme **Listesi tablosu,** ücretli ve bekleyen ödemeleri gösterir. Hizmet ücreti vergi bilgilerini PDF biçiminde indirebilir ve verilen ödemenin kazanç ayrıntılarını görüntüebilirsiniz.

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="İşlem geçmişini dışarı aktarma.":::

- **Paid:** Başarıyla gönderilen tüm ödemeler. Açılan menüden yıl'ı seçecek ve bu yıl yayımlanan ödemeleri filtrele.
- **Beklemede:** Yaklaşan ödemeler.
- **Hizmet ücreti vergisi (PDF formu)** – Hizmet ücreti vergisine tabi ödemeler için kullanılabilir. Hizmet ücreti vergileri, **diğer vergilerle** gösterilir.
- **Görüntüle** : işlem geçmişine, ödemeye dahil edilen kazanç listesini kullanarak yeniden yönlendirir.

Neden eksik veya beklenmeyen kazanç olduğunu anlamak için bkz. [ticari Market ödemelerinin genel soruları](payout-faq.yml#why-are-my-earnings-missing-).

### <a name="payment-status"></a>Ödeme durumu

Aşağıdaki tabloda farklı kazanç durumları açıklanmaktadır.

| Kazanç durumu | Nedeni | İş ortağı eylemi gerekli mi? |
| --- | --- | --- |
| İşlenmemiş | Kazanç ödeme için uygun. Teşvikleri programı program kılavuzunda tanımlanan bir soğutma dönemi için bu durumda kalır. | No |
| İlerideki | Ödeme siparişi, ödeme işlenmeden önce bekleyen dahili incelemeler için üretildi. | No |
| Bekleyen vergi faturası | Vergi faturanızda eksik veya geçersiz. | Ödeme yapabilmeniz için vergi faturanızı güncelleştirmeniz gerekir |
| İnceleme sırasında reddedildi | Ödeme, gözden geçirme sırasında reddedildi. | Ayrıntılar için Microsoft destek 'e başvurun |
| Başarısız | Ödeme, bir Microsoft Sistem hatası nedeniyle başarısız oldu. | Ayrıntılar için Microsoft destek 'e başvurun |
| Sürüyor | Ödeme devam ediyor. | No |
| Yanlış ödeme | Ödeme kurtarma devam ediyor. | No |
| Gönderilen | Ödeme, bankanızla gönderilmiştir. | No |
| Yeniden işleme | Ödeme bir Microsoft sistem hatasıyla karşılaştı ve yeniden işleniyor. | No |
| Reversed | Ödeme, bankanızla ters çevrildi ve bir sonraki ödeme aşamasında yeniden gönderilecek. | No |
| Vergi faturası reddedildi | Vergi faturanızda gözden geçirme sırasında reddedildi. Tüm bekleyen ödemeler, vergi faturası incelemesi tamamlanana kadar beklemeye alınacaktır. | Ayrıntılar için Microsoft destek 'e başvurun |
| Gözden geçirme kapsamında vergi faturası | Vergi faturanızda İnceleme uygulanıyor. Vergi faturası onaylandıktan sonra ödeme serbest bırakılır. | No |
| Reddedildi | Ödeme, bankanızla reddedildi. | Ayrıntılar için bankanızla görüşün. |
|

### <a name="payments-download"></a>Ödemeler indirilir

 Aşağıdaki tabloda, rapordaki her bir sütun açıklanmaktadır. Ödemeler hakkında daha fazla ayrıntı görmek için ödemeler sayfasının en üstünde **İndir** ' i seçin.

| Sütun adı | Description |
| --- | --- |
| participantID | İş ortağının birincil kimliği program altında |
| participantIDType | Genellikle teşvikleri programları ve mağaza programları için satıcı KIMLIĞI için program KIMLIĞI |
| participantName | Kazanç ortağının adı |
| Programadı | Teşvikleri/mağaza programı adı |
| sıfatını | Bu program/participantID için ödeme para birimi cinsinden kazanılan miktar |
| earnedUSD | Program/katılımcı KIMLIĞI için kazanılan miktar (USD) |
| withheldTax | Program/participantID için ödeme para birimi cinsinden stopaj uygulanan vergi miktarı |
| salesTax | Program/participantID için ödeme para birimi cinsinden toplam satış vergisi miktarı (yalnızca teşvikleri programları için geçerlidir) |
| serviceFeeTax | Program/participantID (yalnızca mağaza programları ve Azure Market için geçerlidir) için para birimine ödenen serviceFeeTax toplam miktarı |
| Toplam ödeme | Program/participantID için vergi stopajı hariç ve satış vergisini (varsa) dahil olmak üzere yerel para birimindeki toplam ödeme |
| currencyCode | Para birimi koduna ödeme |
| paymentMethod | İş ortağını ödemek için kullanılan yöntem, örneğin elektronik banka aktarımı, Kredi dekontu |
| Paymentıd | Ödeme için benzersiz tanımlayıcı. Bu sayı genellikle banka deyiminizde görünür (yalnızca SAP ödemeleri için geçerlidir). |
| paymentStatus | Ödeme durumu |
| paymentStatusDescription | Ödeme durumunun kolay açıklaması |
| paymentDate | Microsoft 'tan Tarih ödeme gönderildi |
|

## <a name="export-data"></a>Verileri dışarı aktarma

**Verileri dışarı aktar** sayfası kendi başına yenilemez. En son verileri görmek için sayfayı el ile yenilemeniz gerekebilir. **İşlem geçmişi**, **ödemeler**, **işlem Özeti** veya **Geçmiş ekstresini** dışarı aktarmak için üç sekmeden birini seçin.

Filtreniz **veri kullanılabilir** hatasıyla sonuçlanabilir. Bu, varsayılan zaman dilimini üç ayda bir kez sola bıraktıysanız ve daha sonra söz konusu dönemin dışında kalan bir ödeme KIMLIĞI seçtiyseniz meydana gelir. Bu durumda, zaman döneminizin kapsamını genişletip yeniden deneyin.

Örnek ödemeler dışarı aktarma işlemi aşağıda verilmiştir:

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="Ödemeler raporunu dışarı aktarın.":::

### <a name="historical-statements"></a>Geçmiş deyimleri

**Dışarı aktarma verisi** Özeti Ayrıca geçmiş deyimlerine erişim sağlar.

> [!NOTE]
> Geçmiş bir ifade bir anlık görüntüdür ve yenilenmez. Lütfen [desteğe](https://partner.microsoft.com/support/v2/?stage=1) başvurun ve gerekirse en son verileri isteyin.

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="Geçmiş deyimlerini dışarı aktarın.":::

- 1 Temmuz 2019 tarihinden önceki işlem geçmişi ayrı olarak işlenir ve sonraki geçmiş raporlarından farklı alanlar kullanır.
- Eski işlem geçmişi, "ayrılmış" adlı, modern geçmişteki "kazanç" sütununa karşılık gelen ve "ödeme gönderildi" durumuna eşit olan tüm kazançları hariç saklayan bir sütun içerir.
- 3K, 6k veya 12D gibi filtreler geçmiş deyimler bölümüne uygulanmaz.

### <a name="historical-statement-downloads"></a>Geçmiş ekstresi İndirmeleri

Aşağıdaki tabloda bir geçmiş deyimindeki her bir sütun açıklanmaktadır.

| Alan adı | Description |
| --- | --- |
| Gelir kaynağı | Microsoft Store, Windows Phone deposu, Windows deposu 8 veya reklam gibi işlemin gerçekleştiği yere göre gelirinin kaynağı |
| Sipariş kimliği | Benzersiz sipariş tanımlayıcısı. Bu KIMLIK, satın alma veya geri ödeme gibi satın alma işlemleri olmayan işlemlerle Satınalma işlemlerini tanımlamanızı sağlar. Her ikisinin de aynı sıra KIMLIĞI olur. Ayrıca, tek bir satın alma işlemi için birden çok ödeme yönteminin kullanıldığı bir bölünmüş ücret varsa, satın alma işlemlerini bağlayabilmeniz sağlanır. |
| İşlem kimliği | Benzersiz işlem tanımlayıcısı. |
| İşlem tarihi saati | İşlemin gerçekleştiği tarih ve saat (UTC). |
| Üst ürün KIMLIĞI | Benzersiz üst ürün tanımlayıcısı. İşlem için bir üst ürün yoksa, üst ürün KIMLIĞI = ürün KIMLIĞI. |
| Ürün Kimliği | Benzersiz ürün tanımlayıcısı. |
| Ana ürün adı | Ana ürünün adı. İşlem için bir üst ürün yoksa, üst ürün adı = ürün adı. |
| Ürün Adı | Ürünün adı |
| Ürün Türü | Uygulama, eklenti veya oyun gibi ürün türü |
| Miktar | gelir kaynağı İş İçin Microsoft Store, miktar satın alınan lisansların sayısını temsil eder. Diğer tüm gelir kaynakları için miktar her zaman 1 olur. İki farklı ödeme yöntemi kullanıldığından, tek bir işlem iki satır öğesine bölündüğünde bile, her satır öğesi 1 miktarını gösterir. |
| İşlem Türü | Satın alma, iadesi, ters çevirme veya geri ödeme gibi işlem türü |
| Ödeme yöntemi | İşlem için kullanılan, kart, mobil taşıyıcı faturalandırma veya PayPal gibi müşteri ödeme gereci |
| Ülke/bölge | İşlemin gerçekleştiği ülke/bölge |
| Yerel sağlayıcı/satıcı | Yerel sağlayıcı/kayıt satıcı |
| İşlem para birimi | İşlemin para birimi |
| İşlem miktarı | İşlem miktarı |
| Havale edilen vergi | Havale edilen vergi miktarı (satış, kullanım veya KDV/GST vergileri) |
| NET alındılar | Daha az vergi havale edilen işlem miktarı |
| Mağaza ücreti | Uygulamanın veya eklentinin depoda kullanılabilmesini sağlama ücreti olarak Microsoft tarafından korunan net alındıları yüzdesi |
| Uygulama devam eder | NET alındılar mağaza ücreti eksi |
| Stopaj uygulanan vergiler | Stopaj uygulanan gelir vergisi miktarı ( **ayrılmış** CSV dosyasına dahil) |
| Payment | Uygulama, geçerli gelir Vergi stopajını (Işlem para birimi cinsinden gösterilen tutar) daha az sürer. **Ayrılmış** CSV dosyasına dahil değildir. |
| FX oranı | Işlem para birimini ödeme para birimine dönüştürmek için kullanılan yabancı değişim oranı |
| Ödeme Para Birimi | Ödemenizin yapıldığı para birimi |
| Dönüştürülen ödeme | FX Rate kullanılarak ödeme para birimine dönüştürülen ödeme tutarı |
| Vergi havale modeli | Vergi vergisinden sorumlu olan parti (satış, kullanım veya KDV/GST vergileri) |
| Uygunluk tarihi saati | İşlemin devam eden ödeme için uygun hale geldiği tarih ve saat (UTC). Bir ödeme oluşturulduğunda, bu işlem, ödeme oluşturma tarihinden (yalnızca **ayrılmış** CSV dosyasına dahil) önce uygunluk tarihi ile devam eder. |
| Ücretler | Işlem tutarı sütununda toplanan tüm ücret ayrıntılarının dökümünü gösterir (yalnızca Azure Marketi 'ne dahildir; **ayrılmış** CSV dosyasına dahil değildir). |
|||

## <a name="next-steps"></a>Sonraki adımlar

- [İş Ortağı Ödemesi API'si](https://apidocs.microsoft.com/services/partnerpayouts)
- [Ödeme ilkesi ayrıntıları](payout-policy-details.md)
- Faturalandırma desteği için ticari Market [Yayımcı desteği](https://partner.microsoft.com/support/v2/?stage=1)'ne başvurun.
