---
title: Ödeme deyimleri
description: Ödeme deyimleri ve özetleri ve Ödeme verilerinizi Microsoft İş Ortağı Merkezi'dan görüntüleme ve dışarı aktarma hakkında bilgi İş Ortağı Merkezi
ms.subservice: partnercenter-marketplace-publisher
ms.service: marketplace
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 3/22/2021
ms.openlocfilehash: 4e9ab721fe356dbcdff7316a5ed5b52c81f2d4eb
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152605"
---
# <a name="payout-statements"></a>Ödeme deyimleri

**Uygun roller:** Hesap yöneticisi | Genel yönetici

Ödeme **deyimi, ticari** market aracılığıyla satılan tekliflerden yapılan ödemelere genel bir bakış sunar. Kazançlarınız için işlem geçmişini gösterir, sonraki ödemenizi tahmin eder ve ödeme eğilimlerini gösterir. ayrıca işlem geçmişini ve ödeme deyimlerini de indirebilirsiniz. Bu makalede, ödeme bildiriminize nasıl erişilip farklı ödeme sayfalarına ve indirmelere erişilme İş Ortağı Merkezi.

>[!NOTE]
>Yalnızca ilişkili olduğunu MPN kimlikleri ve programları için verileri göreceğiz. Ek veriler görmek için izinler için hesap yöneticinizle birlikte çalışabilirsiniz. 

## <a name="roles-and-permissions"></a>Roller ve izinler

Ödeme deyimine erişmek için Hesap sahibi veya Finansal katkıda **bulunan rolüne** **sahip olmak** gerekir.

| Raporlar/Sayfalar | Hesap sahibi | Yönetici | Geliştirici | İş katkıda bulunanı | Finans katkıda bulunanı | Pazarlamacı |
| --- | --- | --- | --- | --- | --- | --- |
| Edinme raporu (gerçek zamanlıya yakın veriler de dahil) | View ( View) | View ( View) | Erişim yok | Erişim yok | View ( View) | Erişim yok |
| Geri bildirim raporu/yanıtları | Geri bildirimi görüntüleme ve gönderme | Geri bildirimi görüntüleme ve gönderme | Geri bildirim görüntüleyebilir ve gönderebilir | Erişim yok | Erişim yok | Geri bildirim görüntüleyebilir ve gönderebilir |
| Sistem durumu raporu (neredeyse gerçek zamanlı veriler dahil) | Görüntüleyebilir | Görüntüleyebilir | Görüntüleyebilir | Görüntüleyebilir | Erişim yok | Erişim yok |
| Kullanım raporu | Görüntüleyebilir | Görüntüleyebilir | Görüntüleyebilir | Görüntüleyebilir | Erişim yok | Erişim yok |
| Ödeme hesabı | Güncelleştirebilir | Erişim yok | Erişim yok | Erişim yok | Güncelleştirebilir | Erişim yok |
| Vergi profili | Güncelleştirebilir | Erişim yok | Erişim yok | Erişim yok | Güncelleştirebilir | Erişim yok |
| Ödeme özeti | Görüntüleyebilir | Erişim yok | Erişim yok | Erişim yok | Görüntüleyebilir | Erişim yok |
|

## <a name="access-your-payout-statement"></a>Ödeme deyiminize erişme

Oturum [İş Ortağı Merkezi](https://partner.microsoft.com/dashboard/home) ve ekranın sağ üst köşesindeki ödeme simgesini seçerek bu farklı özetlere erişin:

- İşlem geçmişi
- Ödemeler
- Verileri dışarı aktarma

:::image type="content" source="images/payouts/payout-overview.png" alt-text="İş Ortağı Merkezi portalının sağ üst köşesindeki Ödeme simgesini gösterir":::

Ayrıca, doğrudan ödeme işlemi [ve ödeme verilerine bağlanmak](https://apidocs.microsoft.com/services/partnerpayouts) ve almak için İş Ortağı Ödeme API'sini de kullanabilirsiniz.


## <a name="transaction-history"></a>İşlem geçmişi

İşlem **geçmişi sayfasında,** son 36 aya göre kazançlarınız, tahmini sonraki ödemeniz ve kazançlarınız ile ödeme eğiliminiz özetini gösterir. İşlem ayrıntılarını bu bölümden de indirebilirsiniz.<br><br>Bu rapor, henüz gönderilmemiş ödemeler de dahil olmak üzere ödeme için uygun olan tüm kazançları gösterir. IsV, İş Ortağı Merkezi'daki tüm banka ve vergi bilgilerini tamamlamış >, 50 ABD doları kazanmış, ISV hesabı etkin olduğunda ve müşteri faturalandırılmış (EA işlemleri için) veya ödeme (EA dışı işlemler için) alınmıştır.

:::image type="content" source="images/payouts/transaction-overview.png" alt-text="İşlemlere genel bakış.":::

- **Bu yıl gönderilen kazançlar** : Toplam kazançlar ve ödenen ve gelecek ay içinde ödenecek olan kazançların dökümü.
- **Tahmini ödeme ayı:** Önümüzdeki aylarda beklenen toplam kazançlar.
- **Kazançlar ve ödeme eğilimi:** Son 36 aya göre aylık kazanç ve ödeme tutarları.
- **İndir** – İşlem ayrıntılarını .csv veya .tsv biçiminde indirin.

Sayfanın çıkışını son 3, 6, 12 veya 36 ay gösterecek şekilde filtrelemek için sayfanın sağ üst köşesindeki tarih aralığı seçimini kullanın. 36 aya kadar olan özel bir tarih aralığı da seçin. Varsayılan tarih aralığı 12 aydır. Ayrıca Kayıt Kimliği, Program, Ödeme Kimliği, Kazanç türü, Kaldıraç ve Durum'a göre de filtreleyin. Veriler geçerli mali yıl (1 Temmuz - 30 Haziran) ve önceki iki mali yıl için kullanılabilir.

:::image type="content" source="images/payouts/search-filter.png" alt-text="Sayfanın sağ üst kısmındaki arama filtresi.":::

Bir atma hakkında daha fazla ayrıntı görmek için sayfanın sağ tarafındaki aşağı oku seçin. Bunun yapılması manı, gelir tutarını, ürünü ve müşteriyi görüntüler. Herhangi bir nedenden dolayı bu verilerden herhangi biri kullanılamaz, ancak ona erişmeniz gerekiyorsa, desteğe başvurun. Kazanım, bir işlem değil, bir ayarlamanın sonucu ise, ürün ve müşteri alanları gösterilmez.

### <a name="transaction-history-summary"></a>İşlem geçmişi Özeti

Bu görünüm, ürün ve tahmini ödeme ayından oluşan ürünün kazanç kaynağı dahil olmak üzere kazanç ayrıntılarını gösterir.

:::image type="content" source="images/payouts/transaction-history.png" alt-text="İşlem geçmişi.":::

- **Kazanılan tarih** : satın alma tarihi.
- **Kazanç türü** : satış, Indirim veya ortak işlem gibi kazanç türü.
- **Toplam tutar** – net kazanç miktarı. Ticari Market 'te, bu, standart Market ücreti düşüldükten sonraki anlamına gelir.
- **Durum** – üç seçeneğe sahiptir:
    - **Yaklaşan** – kazanç, bekleyen soğutma döneminde.
    - **İşlenmiş** – kazanç, bir sonraki ödeme için hazırlanır.
    - **Gönderilen** – kazanç ödenmiştir.
- **Tahmini ödeme ayı** : kazancının ödenmesi beklenen ay. Daha fazla bilgi için [sonraki bölüme](#estimated-payment-month) bakın.

İşlem, ödeme uygunluğu ile buluşduktan sonra işleme işlemleri gösterilir. Neden eksik veya beklenmeyen kazanç olduğunu anlamak için bkz. [ticari Market ödemelerinin genel soruları](payout-faq.md#why-are-my-earnings-missing).

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

Ödemenizin yalnızca program eşiğine ve ödeme uygunluk kurallarına uyulması şartıyla, bu ayda serbest bırakılmıştır. Bu kurallar aşağıdakileri içerir ancak aşağıdaki listeyle sınırlı değildir:

- Vergi profiliniz güncel olmalıdır
- Kazanmanız, program kılavuzumuza tanımlanan en düşük kazanç eşiğini karşılamalıdır veya aşmalıdır.
- Beklemeye ödeme: profil atama sayfasındaki "ödemi tut" seçeneğini belirlerseniz.
- Ödeme aracı kullanılamıyor: ödeme veya/ve vergi profili tamamlanmadı.

### <a name="transaction-history-download"></a>İşlem geçmişi indirmesi

Bir atma hakkında daha fazla ayrıntı görmek için sayfanın en üstünde **İndir** ' i seçin. Aşağıdaki tabloda, rapordaki her bir sütun açıklanmaktadır.

>[!NOTE]
>Işlem geçmişi indirmesi dışarı aktarma, Ağustos 2020 itibariyle iki yeni alana sahiptir:
>
>- **Lastpaymentcurrency**  En son ödemenin alındığı, o anda oturum açmış olan iş ortağının erişebileceği para birimi. Ödeme alınmaz, son ödeme para birimi ABD Doları olacaktır.
>- **Earningamountınlastpaymentcurrency**  Son ödeme para biriminde kazanç miktarı.

| Sütun adı | Description | Teşvik için uygulanabilirlik programları/pazar yerleri |
| --- | --- | --- |
| agreementEndDate | Anlaşma bitiş tarihi | Teşvikleri-yalnızca bazı programlar |
| agreementNumber | Anlaşma numarası | Teşvikleri-yalnızca bazı programlar |
| agreementStartDate | Sözleşme başlangıç tarihi | Teşvikler - yalnızca bazı programlar |
| calculationDate | Kazançların sistemde hesaplanma tarihi | Tümü |
| claimId | Talep için benzersiz tanımlayıcı | Teşvikler - yalnızca bazı programlar |
| customerCountry | Müşteri ülkesi/bölgesi | Pazaryerleri |
| customerEmail |  |  |
| Müşteriadı | Boş olabilir | Yalnızca teşvik programları (özel durum: OEM) ve marketler. CSP işlemleri için marketler CSP'nin adını gösterir |
| customerTenantId |  |  |
| distributorId | Dağıtımcı tanımlayıcısı | Teşvikler - yalnızca bazı programlar |
| distributorName | Dağıtıcı adı | Teşvikleri-yalnızca bazı programlar |
| earningAmount | Orijinal işlem para birimindeki miktarı atma | Tümü |
| Earningamountınlastpaymentcurrency | Son ödeme para birimindeki miktarı atma (önceki ödemeler ödeniyorsa alan boş olacaktır) |  |
| earningAmountUSD | USD cinsinden miktar atma | Tümü |
| earningDate | Kazanlama tarihi | Tümü |
| earningExchangeRate | Karşılık gelen USD tutarını göstermek için kullanılan döviz kuru | Tümü |
| Eardokgıd | Her bir atma için benzersiz tanımlayıcı | Tümü |
| Eardokgrate | Teşvikleri oranı, bir kazanç oluşturmak için işlem tutarına uygulandı | Tümü |
| earningType | Ücret ödemesinin, indirimin, ortak işlem, satış ve benzeri olduğunu belirtir | Tümü |
| exchangeRateDate | EarningAmount USD 'yi hesaplamak için kullanılan döviz kuru tarihi | Tümü |
| Externalreferenceıd | Programın benzersiz tanımlayıcısı | Doğrudan Ödeme programları (teşvikler ve marketler) |
| externalReferenceIdLabel | Benzersiz tanımlayıcı etiketi | Doğrudan Ödeme programları (teşvikler ve marketler) |
| instantRebateAmount |  |  |
| invoiceDate |  |  |
| invoiceNumber | Fatura numarası (yalnızca kuruluş için geçerlidir) | Teşvikler ve marketler - yalnızca bazı programlar |
| lastPaymentCurrency | Son ödeme para birimi (önceden ödeme yapılan bir ödeme yoksa alan boş olur) |  |
| Kolu | Kazanç için iş kuralını gösterir | Tümü |
| LicensingProgramName | Lisanslama programının adı |  |
| LineItemId | Müşterinin faturasında tek satır |  |
| localProviderSeller | Yerel sağlayıcı/kayıt satıcısı |  |
| Vade ayı | Tahmini ödeme ayı | Tümü |
| OrderId | Müşterinin faturasıyla ilişkili  | marketlerinden |
| Parentproductıd | Benzersiz üst ürün tanımlayıcısı. İşlem için bir üst ürün yoksa, üst ürün KIMLIĞI = ürün KIMLIĞI. | marketlerinden |
| parentProductName | Ana ürünün adı. İşlem için bir üst ürün yoksa, üst ürün adı = ürün adı. | marketlerinden |
| participantId | İş ortağının birincil kimliği program altında | Tümü |
| participantIdType | Pazar yerleri için programları ve satıcı için çoğunlukla program KIMLIĞI | Tümü |
| participantName | Kazanç ortağının adı | Tümü |
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
| purchaseOrderCoverageStartDate | Her zaman boş kalır | Teşvik programı-CRı |
| purchaseOrderType | Her zaman boş kalır | Teşvik programı-CRı |
| purchaseTypeCode | Her zaman boş kalır | Teşvik programı-CRı |
| miktar | Programa göre farklılık gösterir. İşlem programlarının faturalandırılan miktarını gösterir | Tümü |
| reasonCode |  |  |
| Resellerülke |  |  |
| ResellerID | Satıcı tanımlayıcısı | Teşvikleri-yalnızca bazı programlar |
| Reselleradı | Satıcı adı |  |
| SkuId | Yayımlama sırasında tanımlanan SKU KIMLIĞI. Bir teklifin birçok SKU 'su olabilir, ancak bir SKU yalnızca tek bir teklifle ilişkilendirilebilir. Teşvikler - yalnızca bazı programlar |  |
| storeFee | Uygulamayı veya eklentiyi Mağaza'da kullanılabilir yapma ücreti olarak Microsoft tarafından eldeki tutar | Pazaryerleri |
| subscriptionEndDate | Abonelik bitiş tarihi | Teşvikler - yalnızca bazı programlar |
| subscriptionId | Müşteriyle ilişkili abonelik tanımlayıcısı | Teşvikler - yalnızca bazı programlar |
| subscriptionStartDate | Abonelik başlangıç tarihi | Teşvikler - yalnızca bazı programlar |
| taxCity |  |  |
| taxCountry |  |  |
| taxRemitModel | Vergileri (satış, kullanım veya KDV/GST vergileri) sorumlu taraf | Pazaryerleri |
| taxRemitted | Atlanmış vergi tutarı (satış, kullanım veya KDV/GST vergileri) | Pazaryerleri |
| taxState | Müşterinin durumu |  |
| taxZipCode | Müşterinin ZIP/posta kodu |  |
| tpan | Üçüncü taraf ad ağını belirtir | Pazar yalnızca reklamları yerleştir |
| Işlem miktarı | Orijinal işlem para biriminde, kazanıştan oluşan işleme göre işlem miktarı | Tümü |
| transactionAmountUSD | USD cinsinden işlem miktarı | Tümü |
| transactionCountryCode | İşlemin gerçekleştiği ülke/bölge kodu |  |
| Işlem para birimi | Orijinal müşteri işleminin gerçekleştiği para birimi (Bu iş ortağı konum para birimi değil) | Tümü |
| transactionDate | İşlemin tarihi. Birçok işlemin tek bir işleme katkıda bulunduğu programlar için yararlıdır | Tümü |
| transactionExchangeRate | Karşılık gelen işlem USD tutarını göstermek için kullanılan döviz kuru tarihi | Tümü |
| Transactionıd | İşlem için benzersiz tanımlayıcı | Tümü |
| transactionPaymentMethod | İşlem için kullanılan Kart, Mobil Operatör Faturalaması veya PayPal gibi müşteri ödeme aracı | Pazaryerleri |
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
| İşlem Ayarlaması Microsoft yanlış hesaplaması | Yanlış hesaplamaları düzelten ayarlama. |
| Ops ayarlaması Microsoft Hatalı kayıt | Kayıt ile ilgili hatalı hesaplamalar için ayarlama. |
| İş ortağı eşlemesi (abonelik) MCI/CSP | Aboneliğin hizalaması hatalı düzeltme. |
| İlke özel durumu | Bir program kuralını geçersiz kılan ayarlama.  |
| Önceki dönem gelirleri | Geçerli kazanç döneminin dışındaki kazançlar için ayarlama. |

## <a name="payments"></a>Ödemeler

**Ödemeler** sayfası, Microsoft ile kazandığınızı ayrıntılarıyla ayrıntılardır. Ayrıca ne zaman ve ne kadar ücret ödeeceğini gösterir.

>[!Note]
> Ödemenizin uygun olması için, devam eden $50 [ödeme eşiğine](payment-thresholds-methods-timeframes.md) ulaşmalıdır. Daha fazla bilgi için bkz. [Microsoft Publisher sözleşmesi](/legal/marketplace/msft-publisher-agreement).

:::image type="content" source="images/payouts/payments-overview.png" alt-text="Ödemeler genel bakış ekranı.":::

- **Toplam ödenen bu yıl** – tüm programlarınız için ABD Doları cinsinden bu yıla kadar ödenen toplam miktar.
- **Sonraki tahmini ödeme** : ABD Doları cinsinden size gelen tek bir sonraki ödeme (çok yakında geliyor olsa bile).
- **Son ödeme** : miktar (ABD Doları cinsinden), program adı ve en son ödemenizin programı.
- **Kaynağa göre ödeme** – son 12 aya göre, her program için ödeme miktarı (ABD Doları cinsinden).

### <a name="payments-list"></a>Ödemeler listesi

**Ödemeler tablosunun listesi** ücretli ve bekleyen ödemeleri gösterir. Hizmet ücreti vergi bilgilerini PDF biçiminde indirebilir ve belirli bir ödemenin kazanç ayrıntılarını görüntüleyebilirsiniz.

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="İşlem geçmişini dışarı aktarma":::

- **Paid:** Başarıyla gönderilen tüm ödemeler. Açılan menüden yıl'ı seçecek ve bu yıl yayımlanan ödemeleri filtrele.
- **Beklemede:** Yaklaşan ödemeler.
- **Hizmet ücreti vergisi (PDF formu)** – Hizmet ücreti vergisine tabi ödemeler için kullanılabilir. Hizmet ücreti vergileri Diğer **vergiler içinde gösterilir.**
- **Görünüm:** Ödemeye dahil edilen kazançların listesiyle işlem geçmişine yeniden yönlendirmeler.

Neden eksik veya beklenmeyen kazançlarınız olabileceğini anlamak için [bkz. Ticari market ödemeleri hakkında sık sorulan sorular.](payout-faq.md#why-are-my-earnings-missing)

### <a name="payment-status"></a>Ödeme durumu

Aşağıdaki tabloda farklı kazanç durumları açık açıklamalıdır.

| Kazanç durumu | Nedeni | İş ortağı eylemi gerekiyor mu? |
| --- | --- | --- |
| Işlenme -miş | Kazanç, ödeme için uygundur. Uygulamanın program kılavuzunda tanımlandığı gibi bir soğutma süresi boyunca bu Teşvikler programı. | No |
| Yaklaşan | Ödeme işlenmeden önce bekleyen iç incelemeler oluşturulan ödeme siparişi. | No |
| Bekleyen vergi faturası | Vergi faturanız eksik veya geçersiz. | Ödeme yapmak için vergi faturanızı güncelleştirmeniz gerekir |
| Gözden geçirme sırasında reddedildi | Ödeme, gözden geçirme sırasında reddedildi. | Ayrıntılar için Microsoft destek 'e başvurun |
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

### <a name="payments-download"></a>Ödemeleri indirme

 Aşağıdaki tabloda, rapordaki her sütun açık bir şekilde açık bir şekilde ve açıklamadır. Ödemeniz hakkında daha fazla ayrıntı görmek için Ödemeler **sayfasının** üst kısmından İndir'i seçin.

| Sütun adı | Description |
| --- | --- |
| katılımcıKIMlikKimlik | Program kapsamında kazanç elde olan iş ortağının birincil kimliği |
| participantIDType | Teşvik programları için genellikle program kimliği ve Mağaza programları için Satıcı Kimliği |
| katılımcıAdı | Kazanç ortağının adı |
| programName | Teşvikler/mağaza programı adı |
| Kazan | Bu program/katılımcıki için Ödeme para biriminde kazanılan tutar |
| kazanılanUSD | Program/katılımcı kimliği için kazanılan tutar (ABD doları) |
| withheldTax | Program/katılımcıkikiki için Ödeme para biriminde yardım alan vergi tutarı |
| Satışvergisi | Program/katılımcıkikiki için Ödeme para birimi cinsinden toplam satış vergisi tutarı (yalnızca teşvik programları için geçerlidir) |
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

Örnek ödemeleri dışarı aktarma örneği:

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="Ödemeler raporunu dışarı aktarın.":::

### <a name="historical-statements"></a>Geçmiş deyimleri

Verileri **dışarı aktar** özeti, geçmiş deyimlerine de erişim sağlar.

> [!NOTE]
> Geçmiş deyimi bir anlık görüntüdir ve yenilenmez. Lütfen [destekle iletişime](https://partner.microsoft.com/support/v2/?stage=1) geçin ve gerekirse en son verileri talep edin.

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="Geçmiş deyimlerini dışarı aktarma.":::

- 1 Temmuz 2019'dan önceki işlem geçmişi ayrı olarak işlendi ve sonraki geçmiş raporlarından farklı alanlar kullanıyor.
- Eski işlem geçmişi, modern tarihteki "Kazançlar" sütununa karşılık gelen "Ayrılmış" adlı bir sütuna sahip ancak durumu "Payment Sent" ile eşit olan tüm kazançları dışlar.
- 3M, 6M veya 12M gibi filtreler Geçmiş deyimleri bölümüne uygulanmayacak.

### <a name="historical-statement-downloads"></a>Geçmiş deyim indirmeleri

Aşağıdaki tabloda, geçmiş deyiminde yer alan her sütun açık bir şekilde açık bir şekilde ele alır.

| Alan adı | Description |
| --- | --- |
| Gelir Kaynağı | Microsoft Store, Windows Phone Store, Windows Mağazası 8 veya reklam gibi işlemlerin nerede meydana geldiğine bağlı olarak gelir kaynağı |
| Sipariş kimliği | Benzersiz sipariş tanımlayıcısı. Bu kimlik, satın alma işlemlerini para iadeleri veya geri ödeme gibi ilgili satın alma dışı işlemleriyle tanımlamanıza olanak sağlar. Her ikisi de aynı Sipariş Kimliğine sahip olacak. Ayrıca, tek bir satın alma için birden çok ödeme yönteminin kullanılmış olduğu bir bölme ücreti varsa, satın alma işlemlerini bağlamaya olanak sağlar. |
| İşlem kimliği | Benzersiz işlem tanımlayıcısı. |
| İşlem Tarihi Saati | İşlemin gerçekleştiği tarih ve saat (UTC). |
| Üst ürün KIMLIĞI | Benzersiz üst ürün tanımlayıcısı. İşlem için bir üst ürün yoksa, üst ürün KIMLIĞI = ürün KIMLIĞI. |
| Ürün Kimliği | Benzersiz ürün tanımlayıcısı. |
| Ana ürün adı | Ana ürünün adı. İşlem için bir üst ürün yoksa, üst ürün adı = ürün adı. |
| Ürün Adı | Ürünün adı |
| Ürün Türü | Uygulama, eklenti veya oyun gibi ürün türü |
| Miktar | Gelir kaynağı Iş için Microsoft Store, miktar satın alınan lisansların sayısını temsil eder. Diğer tüm gelir kaynakları için miktar her zaman 1 olur. İki farklı ödeme yöntemi kullanıldığından, tek bir işlem iki satır öğesine bölündüğünde bile, her satır öğesi 1 miktarını gösterir. |
| İşlem Türü | Satın alma, iadesi, ters çevirme veya geri ödeme gibi işlem türü |
| Ödeme yöntemi | İşlem için kullanılan, kart, mobil taşıyıcı faturalandırma veya PayPal gibi müşteri ödeme aracı |
| Ülke/bölge | İşlemin gerçekleştiği ülke/bölge |
| Yerel sağlayıcı/satıcı | Yerel sağlayıcı/kayıt satıcı |
| İşlem Para Birimi | İşlem para birimi |
| İşlem Tutarı | İşlem tutarı |
| Vergi Atlandı | Atlanmış vergi tutarı (satış, kullanım veya KDV/GST vergileri) |
| Net Makbuzlar | İşlem tutarı daha az vergi atlandı |
| Mağaza Ücreti | Uygulamayı veya eklentiyi Mağaza'da kullanılabilir yapma ücreti olarak Microsoft tarafından elde edilen Net Makbuzların yüzdesi |
| Uygulama Devam Ediyor | Net makbuzlar eksi Mağaza Ücreti |
| Vergiler Için Yardım | Elde edilen gelir vergisi tutarı (Ayrılmış **CSV** dosyasına dahildir) |
| Payment | Uygulama Devam Eder, geçerli gelir vergisi stopajı (İşlem Para Birimi cinsinden gösterilen tutar) daha azdır. Ayrılmış CSV **dosyasına** dahil değildir. |
| FX Oranı | İşlem Para Birimini Ödeme Para Birimine dönüştürmek için kullanılan döviz kuru |
| Ödeme Para Birimi | Ödemenizin yapıldı olduğu para birimi |
| Dönüştürülen Ödeme | FX Rate kullanılarak ödeme para birimine dönüştürülen ödeme tutarı |
| Vergi havale modeli | Vergi vergisinden sorumlu olan parti (satış, kullanım veya KDV/GST vergileri) |
| Uygunluk tarihi saati | İşlemin devam eden ödeme için uygun hale geldiği tarih ve saat (UTC). Bir ödeme oluşturulduğunda, bu işlem, ödeme oluşturma tarihinden (yalnızca **ayrılmış** CSV dosyasına dahil) önce uygunluk tarihi ile devam eder. |
| Ücretler | Işlem tutarı sütununda toplanan tüm ücret ayrıntılarının dökümünü gösterir (yalnızca Azure Marketi 'ne dahildir; **ayrılmış** CSV dosyasına dahil değildir). |
|||

## <a name="next-steps"></a>Sonraki adımlar

- [İş Ortağı Ödemesi API'si](https://apidocs.microsoft.com/services/partnerpayouts)
- [Ödeme ilkesi ayrıntıları](payout-policy-details.md)
- Faturalandırma desteği için ticari Market [Yayımcı desteği](https://partner.microsoft.com/support/v2/?stage=1)'ne başvurun.