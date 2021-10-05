---
title: Ödeme deyimleri
description: Ödeme deyimleri ve özetler hakkında bilgi edinin ve Microsoft Iş Ortağı Merkezi 'nden ödeme verilerinizi nasıl görüntüleyip dışarı aktarabilirsiniz?
ms.subservice: partnercenter-payouts
ms.service: partner-dashboard
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 09/27/2021
ms.openlocfilehash: fbc3b659bbb3dded386dfa970d815b27de48ebd5
ms.sourcegitcommit: cf8c78e0c8831371432007d5ab05f934f15a77b5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/05/2021
ms.locfileid: "129525329"
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

İşlem, ödeme uygunluğu ile buluşduktan sonra işleme işlemleri gösterilir. Neden eksik veya beklenmeyen kazanç olduğunu anlamak için bkz. [ticari Market ödemelerinin genel soruları](payout-faq.yml#why-are-my-earnings-missing-).

#### <a name="estimated-payment-month"></a>Tahmini ödeme ayı

Işlem geçmişi sayfası artık, önümüzdeki birkaç aya ait tahmini ödeme tutarlarınızı gösteren bir tablo içerir. Ayrıca, bu bilgileri Işlem geçmişi ve Özet raporu dışarı aktarmaları ' nde görüntüleyebilir ve indirebilirsiniz. Bu bilgiler mutabakatları ve ödeme projeksiyonlarını kolaylaştırır.

Tahmini ödeme ayı program yapılandırma kuralları ve zaman çizelgeleri temel alınarak hesaplanır ve sonraki/yaklaşan ödeme dönemi içinde işlenir.

Tahmini ödeme ayı, geçerli **değil** olarak görüntülenen ortak op hariç tüm kazanç türleri için kullanılabilir. 1 Temmuz 2020 tarihinden önceki kazançlar için tahmini ödeme ayı **kullanılamaz** olarak görünür.

Aşağıdaki tabloda tahmini bir ödeme ayı örneği gösterilmektedir.

| Ay | Miktar |
| ------ | :-----------: |
|  Eyl-2020 |  $7.273,99   |
|  Eki 2020 | $8.692,30  |
|  Kas-2020 | $107,89  |

Tahmini miktar, çeşitli nedenlerle gerçek miktardan farklı olabilir:

- Atık Sulama: kazançlar yeniden hesaplandıktan sonra gerçek miktar farklı olacaktır
- Ayarlamalar: gerçek miktar, gerçekleşen veya gönderilen ayarlamaların bağlı olarak değişir.
- Kurallar değişikliği: kurallarda yapılan değişiklik, ödenen gerçek miktardaki yeniden hesaplamayı yansıtabilir
- Borç: ödeme hatası oluşursa, gerçek tutar farklı olabilir

Ödemenizin yalnızca, programınızın eşiği ve ödeme uygunluk kuralları karşılanıyorsa öngörülen ay içinde yayınlandığını unutmayın. Bu kurallar aşağıdakileri içerir ancak aşağıdaki listeyle sınırlı değildir:

- Vergi profiliniz güncel olmalıdır
- Kazanmanız, program kılavuzumuza tanımlanan en düşük kazanç eşiğini karşılamalıdır veya aşmalıdır.
- Beklemeye ödeme: profil atama sayfasındaki "ödemi tut" seçeneğini belirlerseniz.
- Ödeme aracı kullanılamıyor: ödeme veya/ve vergi profili tamamlanmadı.

### <a name="transaction-history-download"></a>İşlem geçmişi indirmesi

Bir atma hakkında daha fazla ayrıntı görmek için **İndir**' i seçin. Aşağıdaki tabloda, rapordaki her bir sütun açıklanmaktadır.

| Sütun adı | Description | Teşvik için uygulanabilirlik programları/pazar yerleri |
| --- | --- | --- |
| agreementEndDate | Anlaşma bitiş tarihi | Teşvikleri-yalnızca bazı programlar |
| agreementNumber | Anlaşma numarası | Teşvikleri-yalnızca bazı programlar |
| agreementStartDate | Sözleşme başlangıç tarihi | Teşvikleri-yalnızca bazı programlar |
| calculationDate | Sistemin sistemde hesaplandığı Tarih | Tümü |
| Claimıd | Talep için benzersiz tanımlayıcı | Teşvikleri-yalnızca bazı programlar |
| customerCountry | Müşteri ülkesi/bölgesi | marketlerinden |
| customerEmail |  |  |
| customerName | Boş olabilir | Yalnızca programları teşvik edin (özel durum: OEM) ve pazar yerleri. CSP işlemleri için, Pazar yerleri CSP adını gösterir |
| Customertenantıd |  |  |
| distributorId | Dağıtıcı tanımlayıcısı | Teşvikleri-yalnızca bazı programlar |
| distributorName | Dağıtıcı adı | Teşvikleri-yalnızca bazı programlar |
| earningAmount | Orijinal işlem para birimindeki miktarı atma | Tümü |
| Earningamountınlastpaymentcurrency | Son ödeme para birimindeki miktarı atma (önceki ödemeler ödeniyorsa alan boş olacaktır) |  |
| earningAmountUSD | USD cinsinden miktar atma | Tümü |
| earningDate | Kazanlama tarihi | Tümü |
| earningExchangeRate | karşılık gelen USD tutarını göstermek için kullanılan Exchange oranı | Tümü |
| Eardokgıd | Her bir atma için benzersiz tanımlayıcı | Tümü |
| Eardokgrate | Teşvikleri oranı, bir kazanç oluşturmak için işlem tutarına uygulandı | Tümü |
| earningType | Ücret ödemesinin, indirimin, ortak işlem, satış ve benzeri olduğunu belirtir | Tümü |
| exchangeRateDate | Exchange oranını hesaplamak için kullanılan ücret tarihi USD | Tümü |
| Externalreferenceıd | Program için benzersiz tanımlayıcı | Doğrudan ödeme programları (teşvikleri ve pazar yerleri) |
| Externalreferenceıdlabel | Benzersiz tanımlayıcı etiketi | Doğrudan ödeme programları (teşvikleri ve pazar yerleri) |
| ınstantrebateamount |  |  |
| InvoiceDate |  |  |
| Faturanumarası | Fatura numarası (yalnızca kuruluş için geçerlidir) | Teşvikleri ve pazar yerleri-yalnızca bazı programlar |
| lastPaymentCurrency | Son ödeme para birimi (önceki ödeme ödenene kadar alan boştur) |  |
| düzeyi | Kazanç için iş kuralını gösterir | Tümü |
| LicensingProgramName | Lisanslama programının adı |  |
| Lineıtemıd | Müşterinin faturasında tek satırlık |  |
| Localprovidersatıcı | Yerel sağlayıcı/kayıt satıcı |  |
| Vade ayı | Tahmini ödeme ayı | Tümü |
| OrderId | Müşterinin faturasıyla ilişkili  | marketlerinden |
| Parentproductıd | Benzersiz üst ürün tanımlayıcısı. İşlem için bir üst ürün yoksa, üst ürün KIMLIĞI = ürün KIMLIĞI. | marketlerinden |
| parentProductName | Ana ürünün adı. İşlem için bir üst ürün yoksa, üst ürün adı = ürün adı. | marketlerinden |
| participantId | İş ortağının birincil kimliği program altında | Tümü |
| participantIdType | Pazar yerleri için programları ve satıcı için çoğunlukla program KIMLIĞI | Tümü |
| participantName | Kazanç ortağının adı | Tümü |
| partnerCountryCode | Kazanç ortağının konumu/ülkesi/bölgesi | Tümü |
| partNumber | Her zaman boş kalır | Bazı teşvik programları ve pazar yerleri |
| Paymentıd | Ödeme raporundaki belirli bir ödemeyle birlikte işlem raporundaki tüm işlemleri ilişkilendirmek için benzersiz tanımlayıcı | Tümü |
| paymentStatus | Ödeme durumu | Tümü |
| paymentStatusDescription | Ödeme durumunun kolay açıklaması | Tümü |
| productId | Benzersiz ürün tanımlayıcısı | marketlerinden |
| productName | İşlemle bağlantılı ürün adı | Tümü |
| productType | Uygulama, eklenti veya oyun gibi ürün türü | marketlerinden |
| Program kodu | Program adıyla Eşlenecek dize |  |
| Programadı | Program adını teşvik edin/depolayın | Tümü |
| purchaseOrderCoverageEndDate | Her zaman boş kalır | Teşvik programı-CRı |
| purchaseOrderCoverageStartDate | Her zaman boş kalır | Teşvik programı-CRı |
| purchaseOrderType | Her zaman boş kalır | Teşvik programı-CRı |
| purchaseTypeCode | Her zaman boş kalır | Teşvik programı-CRı |
| miktar | Programa göre farklılık gösterir. İşlem programlarının faturalandırılan miktarını gösterir | Tümü |
| reasonCode |  |  |
| Resellerülke |  |  |
| ResellerID | Satıcı tanımlayıcısı | Teşvikleri-yalnızca bazı programlar |
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

| Neden kodu   | Description   |
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
- **Hizmet ücreti vergisi (PDF formu)** – Hizmet ücreti vergisine tabi ödemeler için kullanılabilir. Hizmet ücreti vergileri Diğer **vergiler içinde gösterilir.**
- **Görünüm:** Ödemeye dahil edilen kazançların bir listesiyle işlem geçmişine yeniden yönlendirmeler.

Neden eksik veya beklenmeyen kazançlarınız olabileceğini anlamak için [bkz. Ticari market ödemeleri hakkında sık sorulan sorular.](payout-faq.yml#why-are-my-earnings-missing-)

### <a name="payment-status"></a>Ödeme durumu

Aşağıdaki tabloda farklı kazanç durumları açık açıklamalıdır.

| Kazanç durumu | Nedeni | İş ortağı eylemi gerekiyor mu? |
| --- | --- | --- |
| Işlenme -miş | Kazanç, ödeme için uygundur. Uygulamanın program kılavuzunda tanımlandığı gibi bir soğutma süresi boyunca bu Teşvikler programı. | No |
| Yaklaşan | Ödeme işlenmeden önce bekleyen iç incelemeler oluşturulan ödeme siparişi. | No |
| Bekleyen vergi faturası | Vergi faturanız eksik veya geçersiz. | Ödeme yapmak için vergi faturanızı güncelleştirmeniz gerekir |
| Gözden geçirme sırasında reddedildi | İnceleme sırasında ödeme reddedildi. | Ayrıntılar için Microsoft desteğine başvurun |
| Başarısız | Ödeme bir Microsoft sistem hatası nedeniyle başarısız oldu. | Ayrıntılar için Microsoft desteğine başvurun |
| Sürüyor | Ödeme devam ediyor. | No |
| Yanlış ödeme | Ödeme yeniden yalıtma devam ediyor. | No |
| Gönderilen | Ödeme bankanıza gönderildi. | No |
| Yeniden işleme | Ödeme bir Microsoft sistem hatasıyla karşılaştı ve yeniden işlenmeye devam ediyor. | No |
| Reversed | Ödeme, bankanız tarafından tersine çevrildi ve sonraki ödeme döngüsünde yeniden gönderilir. | No |
| Vergi faturası reddedildi | Vergi faturanız gözden geçirme sırasında reddedildi. Vergi faturası gözden geçirmesi tamamlandıktan sonra bekleyen tüm ödemeler beklemede olur. | Ayrıntılar için Microsoft desteğine başvurun |
| Gözden geçirilan vergi faturası | Vergi faturanız gözden geçirildi. Vergi faturası onaylandıktan sonra ödemeniz serbest bıraklanır. | No |
| Reddedildi | Ödeme bankanız tarafından reddedildi. | Ayrıntılar için bankanıza ulaşın. |
|

### <a name="payments-download"></a>Ödemeleri indirme

 Aşağıdaki tabloda, rapordaki her sütun açık bir şekilde açık bir şekilde açık bir şekilde ve açıklamadır. Ödemeniz hakkında daha fazla ayrıntı görmek için Ödemeler **sayfasının** üst kısmından İndir'i seçin.

| Sütun adı | Description |
| --- | --- |
| katılımcıKIMlikKimlik | Program kapsamında kazanç elde olan iş ortağının birincil kimliği |
| participantIDType | Teşvik programları için genellikle program kimliği ve Mağaza programları için Satıcı Kimliği |
| katılımcıAdı | Kazanç ortağının adı |
| programName | Teşvikler/mağaza programı adı |
| Kazan | Bu program/katılımcıki için Ödeme para biriminde kazanılan tutar |
| kazanılanUSD | Program/katılımcı kimliği için kazanılan tutar (ABD doları) |
| withheldTax | Program/katılımcıkikiki için Ödeme para biriminde yardım alan vergi tutarı |
| Satışvergisi | Program/katılımcıki için Ödeme para birimi cinsinden toplam satış vergisi tutarı (yalnızca teşvik programları için geçerlidir) |
| serviceFeeTax | Program/katılımcıKimliği için Ödeme para birimi cinsinden serviceFeeTax toplam tutarı (yalnızca mağaza programları ve Azure Market geçerlidir) |
| totalPayment | Stopaj vergisi hariç yerel para birimi cinsinden toplam ödeme ve program/katılımcıkininki için satış vergisini (varsa) dahil edin |
| currencyCode | Ödeme Para birimi kodu |
| paymentMethod | İş ortağına ödeme yapmak için kullanılan yöntem, örneğin elektronik banka aktarımı, kredi notu |
| paymentID | Ödeme için benzersiz tanımlayıcı. Bu sayı genellikle banka hesap hesaplarında görünür (yalnızca SAP ödemeleri için geçerlidir). |
| paymentStatus | Ödeme durumu |
| paymentStatusDescription | Ödeme durumunun kolay açıklaması |
| paymentDate | Ödemenin Microsoft'tan gönderildiği tarih |
|

## <a name="next-steps"></a>Sonraki adımlar

- [Gelir özeti](/partner-center/revenue-summary)
- [Yeni ödeme verileri dışarı aktarma sayfası](/partner-center/payouts-enhanced-exports)
- [İş Ortağı Ödemesi API'si](https://apidocs.microsoft.com/services/partnerpayouts)
- [Ödeme ilkesi ayrıntıları](payout-policy-details.md)
- Faturalama desteği için ticari market yayımcısı [desteğine başvurun.](https://partner.microsoft.com/support/v2/?stage=1)
