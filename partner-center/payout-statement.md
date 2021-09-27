---
title: Ödeme deyimleri
description: Ödeme deyimleri ve özetler hakkında bilgi edinin ve Microsoft Iş Ortağı Merkezi 'nden ödeme verilerinizi nasıl görüntüleyip dışarı aktarabilirsiniz?
ms.subservice: partnercenter-payouts
ms.service: partner-dashboard
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 09/27/2021
ms.openlocfilehash: 6cc683609181ce58768a266ca6a323bbdd9e3486
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129074968"
---
# <a name="payout-statements"></a>Ödeme deyimleri

**Uygun roller**: Hesap Yöneticisi | Genel yönetici

**Ödeme beyanı** , ticari Market aracılığıyla satılan tekliflerden ödemalarınızın genel bir görünümünü sunar. Kazanlarınızın işlem geçmişini gösterir, bir sonraki ödemenizi tahmin eder ve ödeme eğilimlerini gösterir. Ayrıca, işlem geçmişi ve ödeme deyimlerini indirebilirsiniz. Bu makalede, ödeme deyiminize ve Iş Ortağı Merkezi 'nde size erişilebilen farklı ödeme sayfalarına ve indirmelere nasıl erişebileceğiniz açıklanır.

> [!NOTE]
> Yalnızca MPN kimlikleri ve sizinle ilişkilendirdiğiniz programlar için verileri görürsünüz. Ek verileri görmek isterseniz, izinler için hesap yöneticinizle birlikte çalışın. 

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

#### <a name="workspaces-view"></a>[Çalışma alanları görünümü](#tab/workspaces-view)

1. [Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard) oturum açın ve **ödemeler** kutucuğunu seçin.

2. Kullanılabilir özetlerin birini seçin:

    - Ödemelere genel bakış
    - İşlem geçmişi
    - Verileri dışarı aktarma

    :::image type="content" source="./images/payouts/payout-overview-workspaces.png" alt-text="Ödemeler çalışma alanına genel bakış gösteren ekran görüntüsü.":::

#### <a name="current-view"></a>[Geçerli görünüm](#tab/current-view)

[Iş Ortağı Merkezi](https://partner.microsoft.com/dashboard/home) ' nde oturum açın ve bu farklı özetlere erişmek için ekranın sağ üst köşesindeki ödeme simgesini seçin:

- İşlem geçmişi
- Ödemeler
- Verileri dışarı aktarma

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Iş Ortağı Merkezi portalının sağ üst köşesinde bulunan ödeme simgesini gösteren ekran görüntüsü.":::

* * *

Ayrıca, [Iş ortağı ödeme API](/rest/api/partner-center/partner-payouts) 'sini kullanarak doğrudan ödeme ve ödeme verilerini alabilir ve elde edebilirsiniz. [Ödeme HIZMETLERI API 'sini kullanarak ödemeleri yönetme](/partner-center/develop/manage-payouts)hakkında daha fazla bilgi edinin.

## <a name="transaction-history"></a>İşlem geçmişi

**İşlem geçmişi** sayfasında, son 36 aya göre kazanç, tahmini bir sonraki ödeme ve kazanç ve ödemeler eğilimi gösterilir. Ayrıca, bu bölümden işlem ayrıntılarını indirebilirsiniz.<br><br>Bu rapor, henüz gönderilmemiş ödemeler dahil olmak üzere, ödeme için uygun olan tüm gelirleri gösterir. Bir ISV, Iş Ortağı Merkezi 'ndeki tüm banka ve vergi bilgilerini tamamladıktan sonra kazanç $50 >, ISV hesabı etkin ve müşterinin faturalandırıldığı (EA işlemleri için) veya ödeme alındığı zaman (EA işlemleri için) ödemiştir.

- **Bu yıla gönderilen kazançlar** – ödenen ve gelecek ayda ödenen toplam kazanç ve döküm dökümü.
- **Tahmini ödeme ayı** – yaklaşan aylarda beklenen toplam kazanç.
- **Kazanç ve ödeme eğilimi** – son 36 aylar için aylık kazanç ve ödeme tutarları.
- **İndir** – işlem ayrıntılarını .csv veya. tsv biçiminde indirin.

Son 3, 6, 12 veya 36 ayı göstermek için sayfanın çıktısını filtrelemek üzere sayfanın sağ üst köşesindeki tarih aralığı seçimini kullanın. Ya da 36 aya kadar bir özel tarih aralığı seçin. Varsayılan tarih aralığı 12 aydır. Kayıt KIMLIĞI, program, ödeme KIMLIĞI, kazanç türü, MANI ve duruma göre de filtre uygulayabilirsiniz. Veriler geçerli mali yıl (1 Temmuz 30 Haziran) ve önceki iki mali yıl için kullanılabilir.

Bir atma hakkında daha fazla ayrıntı görmek için sayfanın sağ tarafındaki aşağı oku seçin. Bunun yapılması manı, gelir tutarını, ürünü ve müşteriyi görüntüler. Herhangi bir nedenle bu verilerden herhangi biri kullanılamıyorsa ama bu verilere erişmeye ihtiyacınız varsa dehaya başvurun. Kazanç, bir işlem değil düzeltmenin sonucu ise Product ve Customer alanları görüntülenmez.

### <a name="transaction-history-summary"></a>İşlem geçmişi özeti

Bu görünümde satılan üründen elde edilen kazançların kaynağı da dahil olmak üzere kazanç ayrıntıları, durum ve tahmini ödeme ayı yer aya ilişkin bilgiler yer amektedir.

:::image type="content" source="images/payouts/transaction-history.png" alt-text="İşlem geçmişi.":::

- **Kazanılan tarih:** Satın alma tarihi.
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

Kazanç hakkında daha fazla ayrıntı görmek için İndir'i **seçin.** Aşağıdaki tabloda, rapordaki her sütun açık bir şekilde açık bir şekilde açık bir şekilde ve açıklamadır.

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
| resellerId | Kurumsal bayi tanımlayıcısı | Teşvikleri-yalnızca bazı programlar |
| Reselleradı | Satıcı adı |  |
| SkuId | Yayımlama sırasında tanımlanan SKU KIMLIĞI. Bir teklifin birçok SKU 'su olabilir, ancak bir SKU yalnızca tek bir teklifle ilişkilendirilebilir. Teşvikleri-yalnızca bazı programlar |  |
| storeFee | Uygulama veya eklentiyi mağazada kullanılabilir hale getirmek için Microsoft tarafından bir ücret olarak tutulan miktar | marketlerinden |
| subscriptionEndDate | Abonelik bitiş tarihi | Teşvikleri-yalnızca bazı programlar |
| subscriptionId | Müşteriyle ilişkili abonelik tanımlayıcısı | Teşvikleri-yalnızca bazı programlar |
| subscriptionStartDate | Abonelik başlangıç tarihi | Teşvikleri-yalnızca bazı programlar |
| Vergilencity |  |  |
| taxCountry |  |  |
| Taxhavalemodeli | Vergi vergisinden sorumlu olan parti (satış, kullanım veya KDV/GST vergileri) | marketlerinden |
| Vergilenhavale edilmiş | Havale edilen vergi miktarı (satış, kullanım veya KDV/GST vergileri) | marketlerinden |
| taxState | Müşterinin durumu |  |
| taxZipCode | Müşterinin ZIP/posta kodu |  |
| tpan | Üçüncü taraf ad ağını belirtir | Pazar yalnızca reklamları yerleştir |
| Işlem miktarı | Orijinal işlem para biriminde, kazanıştan oluşan işleme göre işlem miktarı | Tümü |
| transactionAmountUSD | USD cinsinden işlem miktarı | Tümü |
| transactionCountryCode | İşlemin gerçekleştiği ülke/bölge kodu |  |
| Işlem para birimi | Orijinal müşteri işleminin gerçekleştiği para birimi (Bu iş ortağı konum para birimi değil) | Tümü |
| transactionDate | İşlemin tarihi. Birçok işlemin tek bir işleme katkıda bulunduğu programlar için yararlıdır | Tümü |
| transactionExchangeRate | karşılık gelen işlem USD tutarını göstermek için kullanılan Exchange hız tarihi | Tümü |
| TransactionId | İşlem için benzersiz tanımlayıcı | Tümü |
| transactionPaymentMethod | İşlem için kullanılan, kart, mobil taşıyıcı faturalandırma veya PayPal gibi müşteri ödeme gereci | marketlerinden |
| Işlem türü | Satın alma, iadesi, ters çevirme veya geri ödeme gibi işlem türü | marketlerinden |
| iş yükü | İş Yükü | Teşvikleri-yalnızca bazı programlar |
|

### <a name="transaction-adjustment-codes"></a>İşlem ayarlama kodları

Aşağıdaki tabloda, ayarlamalar ve açıklamaları için neden kodları listelenmektedir.

| Neden kodu   | Açıklama   |
|------------------|:-------------------------------------|
| AR uyumluluğu | Microsoft faturalarının iş ortağı tarafından zamanında ödenmeyen kazançlarını azaltan ayarlama. |
| Ortak işlem geçişi | Ortak op kazançlarını başka bir döneme aktaran veya ortak op kazançlarını indirimin olarak dönüştüren ayarlama. |
| Ops ayarlaması | Microsoft Sistem hesaplama hatalarını düzelten ayarlama. |
| Ops ayarlaması Microsoft yanlış hesaplama | Hatalı hesaplamaları düzelten ayarlama. |
| Ops ayarlaması Microsoft Hatalı kayıt | Kayıt ile ilgili hatalı hesaplamalar için ayarlama. |
| İş ortağı eşlemesi (abonelik) MCI/CSP | Aboneliğin hizalaması hatalı düzeltme. |
| İlke özel durumu | Bir program kuralını geçersiz kılan ayarlama.  |
| Önceki dönem gelirleri | Geçerli kazanç döneminin dışındaki kazançlar için ayarlama. |

## <a name="payments"></a>Ödemeler

**Ödemeler** sayfası, Microsoft ile kazandığınızı ayrıntılarıyla ayrıntılardır. Ayrıca ne zaman ve ne kadar ücret ödeeceğini gösterir.

> [!NOTE]
> Ödemenizin uygun olması için, devam eden $50 [ödeme eşiğine](payment-thresholds-methods-timeframes.md) ulaşmalıdır. daha fazla bilgi için [Microsoft Publisher sözleşmesine](/legal/marketplace/msft-publisher-agreement)bakın.

- **Toplam ödenen bu yıl** – tüm programlarınız için ABD Doları cinsinden bu yıla kadar ödenen toplam miktar.
- **Sonraki tahmini ödeme** : ABD Doları cinsinden size gelen tek bir sonraki ödeme (çok yakında geliyor olsa bile).
- **Son ödeme** : miktar (ABD Doları cinsinden), program adı ve en son ödemenizin programı.
- **Kaynağa göre ödeme** – son 12 aya göre, her program için ödeme miktarı (ABD Doları cinsinden).

### <a name="payments-list"></a>Ödemeler listesi

**Ödemeler tablosunun listesi** ücretli ve bekleyen ödemeleri gösterir. Hizmet ücreti vergi bilgilerini PDF biçiminde indirebilir ve belirli bir ödemenin kazanç ayrıntılarını görüntüleyebilirsiniz.

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="İşlem geçmişini dışarı aktarın.":::

- **Ücretli** – tüm ödemeler başarıyla gönderildi. Bu yıl içinde Yayınlanan ödemeleri filtrelemek için açılan menüdeki yılı seçin.
- **Bekleyen** – yaklaşan ödemeler.
- **Servis ücreti vergisi (PDF formu)** – ödemeler tabi for Service ücret vergisine göre kullanılabilir. Hizmet ücreti vergileri, **diğer vergilerle** gösterilir.
- **Görüntüle** : işlem geçmişine, ödemeye dahil edilen kazanç listesini kullanarak yeniden yönlendirir.

Neden eksik veya beklenmeyen kazanç olduğunu anlamak için bkz. [ticari Market ödemelerinin genel soruları](payout-faq.yml#why-are-my-earnings-missing-).

### <a name="payment-status"></a>Ödeme durumu

Aşağıdaki tabloda farklı kazanç durumları açıklanmaktadır.

| Kazanç durumu | Nedeni | İş ortağı eylemi gerekli mi? |
| --- | --- | --- |
| İşlenmemiş | Kazanç ödeme için uygun. Teşvikleri programı program kılavuzunda tanımlanan bir soğutma dönemi için bu durumda kalır. | Hayır |
| İlerideki | Ödeme siparişi, ödeme işlenmeden önce bekleyen dahili incelemeler için üretildi. | Hayır |
| Bekleyen vergi faturası | Vergi faturanızda eksik veya geçersiz. | Ödeme yapabilmeniz için vergi faturanızı güncelleştirmeniz gerekir |
| İnceleme sırasında reddedildi | Ödeme, gözden geçirme sırasında reddedildi. | Ayrıntılar için Microsoft destek 'e başvurun |
| Başarısız | Ödeme, bir Microsoft Sistem hatası nedeniyle başarısız oldu. | Ayrıntılar için Microsoft destek 'e başvurun |
| Sürüyor | Ödeme devam ediyor. | Hayır |
| Yanlış ödeme | Ödeme kurtarma devam ediyor. | Hayır |
| Gönderilen | Ödeme, bankanızla gönderilmiştir. | Hayır |
| Yeniden işleme | Ödeme bir Microsoft sistem hatasıyla karşılaştı ve yeniden işleniyor. | Hayır |
| Reversed | Ödeme, bankanızla ters çevrildi ve bir sonraki ödeme aşamasında yeniden gönderilecek. | Hayır |
| Vergi faturası reddedildi | Vergi faturanızda gözden geçirme sırasında reddedildi. Tüm bekleyen ödemeler, vergi faturası incelemesi tamamlanana kadar beklemeye alınacaktır. | Ayrıntılar için Microsoft destek 'e başvurun |
| Gözden geçirme kapsamında vergi faturası | Vergi faturanızda İnceleme uygulanıyor. Vergi faturası onaylandıktan sonra ödeme serbest bırakılır. | Hayır |
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
> Geçmiş deyimi bir anlık görüntüdir ve yenilenmez. Lütfen [destekle iletişime](https://partner.microsoft.com/support/v2/?stage=1) geçin ve gerekirse en son verileri talep edin.

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="Geçmiş deyimlerini dışarı aktarın.":::

- 1 Temmuz 2019'dan önceki işlem geçmişi ayrı olarak işlendi ve sonraki geçmiş raporlarından farklı alanlar kullanıyor.
- Eski işlem geçmişinde, modern tarihteki "Kazançlar" sütununa karşılık gelen "Ayrılmış" adlı bir sütun vardır ancak durumu "Payment Sent" ile eşit olan tüm kazançları dışlar.
- 3M, 6M veya 12M gibi filtreler Geçmiş deyimleri bölümüne uygulanmayacak.

### <a name="historical-statement-downloads"></a>Geçmiş deyim indirmeleri

Aşağıdaki tabloda, geçmiş deyiminde yer alan her sütun açık bir şekilde açık bir şekilde ele alır.

| Alan adı | Açıklama |
| --- | --- |
| Gelir Kaynağı | Microsoft Store, Windows Phone Store, Windows Store 8 veya reklam gibi işlemlerin nerede Windows gelir kaynağı |
| Sipariş kimliği | Benzersiz sipariş tanımlayıcısı. Bu kimlik, satın alma işlemlerini para iadeleri veya geri ödeme gibi ilgili satın alma dışı işlemleriyle tanımlamanıza olanak sağlar. Her ikisi de aynı Sipariş Kimliğine sahip olacak. Ayrıca, tek bir satın alma için birden çok ödeme yönteminin kullanılmış olduğu bir bölme ücreti varsa, satın alma işlemlerini bağlamanız olanaklı olur. |
| İşlem kimliği | Benzersiz işlem tanımlayıcısı. |
| İşlem Tarihi Saati | İşlemin meydana geldiği tarih ve saat (UTC). |
| Üst Ürün Kimliği | Benzersiz üst ürün tanımlayıcısı. İşlem için bir üst ürün yoksa Üst Ürün Kimliği = Ürün Kimliği. |
| Ürün Kimliği | Benzersiz ürün tanımlayıcısı. |
| Üst Ürün Adı | Üst ürünün adı. İşlem için bir üst ürün yoksa, Üst Ürün Adı = Ürün Adı. |
| Ürün Adı | Ürünün adı |
| Ürün Türü | Uygulama, Eklenti veya Oyun gibi ürün türü |
| Miktar | Revenue Source İş İçin Microsoft Store, Quantity değeri satın alınan lisans sayısını temsil eder. Diğer tüm Gelir Kaynakları için Miktar her zaman 1 olur. İki farklı ödeme yöntemi kullanılırken tek bir işlem iki satır öğeye bölünse bile her satır öğesi 1 Miktarı gösterir. |
| İşlem Türü | Satın alma, para iadesi, geri alma veya geri ödeme gibi işlem türü |
| Ödeme Yöntemi | İşlem için kullanılan Kart, Mobil Operatör Faturalaması gibi müşteri ödeme aracı PayPal |
| Ülke /Bölge | İşlemin meydana geldiği ülke/bölge |
| Yerel Sağlayıcı /Satıcı | Yerel sağlayıcı/kayıt satıcısı |
| İşlem Para Birimi | İşlem para birimi |
| İşlem Tutarı | İşlem tutarı |
| Vergi Atlandı | Atlanmış vergi tutarı (satış, kullanım veya KDV/GST vergileri) |
| Net Makbuzlar | İşlem tutarı daha az vergi atlandı |
| Mağaza Ücreti | Uygulamayı veya eklentiyi Mağaza'da kullanılabilir yapma ücreti olarak Microsoft tarafından elde edilen Net Makbuzların yüzdesi |
| Uygulama Devam Ediyor | Net makbuzlar eksi Mağaza Ücreti |
| Vergiler Için Yardım | Elde edilen gelir vergisi tutarı (Ayrılmış CSV dosyasına **dahildir)** |
| Payment | Uygulama Devam Eder, geçerli gelir vergisi stopajı (İşlem Para Birimi cinsinden gösterilen tutar) daha azdır. Ayrılmış CSV **dosyasına** dahil değildir. |
| FX Oranı | İşlem Para Birimini Ödeme Para Birimine dönüştürmek için kullanılan döviz kuru |
| Ödeme Para Birimi | Ödemenizin yapıldı olduğu para birimi |
| Dönüştürülen Ödeme | FX Oranı kullanılarak Ödeme Para Birimine dönüştürülen ödeme tutarı |
| Vergi Havale Modeli | Vergileri (satış, kullanım veya KDV/GST vergileri) sorumlu taraf |
| Uygunluk Tarih Saati | İşlem devam eder tarih ve saat ödeme için uygun hale gelir (UTC). Bir ödeme oluşturulduğunda, işlem ödeme oluşturma tarihinden önce Uygunluk Tarih Saati ile devam eder (yalnızca Ayrılmış **CSV** dosyasına dahil edilir). |
| Ücretler | Transaction Amount sütununda toplanan tüm ücret ayrıntılarının dökümünü gösterir (yalnızca ayrılmış Azure Market dahil edilir; **Ayrılmış** CSV dosyasına dahil değildir). |

## <a name="next-steps"></a>Sonraki adımlar

- [İş Ortağı Ödemesi API'si](https://apidocs.microsoft.com/services/partnerpayouts)
- [Ödeme ilkesi ayrıntıları](payout-policy-details.md)
- Faturalama desteği için ticari market yayımcısı [desteğine başvurun.](https://partner.microsoft.com/support/v2/?stage=1)
