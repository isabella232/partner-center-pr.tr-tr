---
title: Iş Ortağı Merkezi 'nde ticari Market için ödeme beyanı
description: Ödeme deyimleri ve özetler hakkında bilgi edinin ve ticari Market için ödeme verilerinizi görüntüleme ve dışa aktarma
ms.subservice: partnercenter-marketplace-publisher
ms.service: marketplace
ms.topic: article
author: mingshen-ms
ms.author: mingshen
ms.date: 09/23/2020
ms.openlocfilehash: 460a7b1992d7db40e0f45d3aeb7e2236e9495e07
ms.sourcegitcommit: a84812b650ec8b6d0513c46c04840e4bbb0c8460
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/25/2020
ms.locfileid: "92531771"
---
# <a name="payout-statements"></a>Ödeme deyimleri

**Ödeme beyanı** , ticari Market aracılığıyla satılan tekliflerden ödemalarınızın genel bir görünümünü sunar. Kazanlarınızın işlem geçmişini gösterir, bir sonraki ödemenizi tahmin eder ve ödeme eğilimlerini gösterir. Ayrıca, işlem geçmişi ve ödeme deyimlerini indirebilirsiniz. Bu makalede, ödeme deyiminize ve Iş Ortağı Merkezi 'nde size erişilebilen farklı ödeme sayfalarına ve indirmelere nasıl erişebileceğiniz açıklanır.

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

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Iş Ortağı Merkezi portalının sağ üst köşesindeki ödeme simgesini gösterir":::

Ayrıca, [Iş ortağı ödeme API](https://apidocs.microsoft.com/services/partnerpayouts) 'sini kullanarak doğrudan ödeme ve ödeme verilerini alabilir ve elde edebilirsiniz.


## <a name="transaction-history"></a>İşlem geçmişi

**İşlem geçmişi** sayfasında, son 36 aya göre kazanç, tahmini bir sonraki ödeme ve kazanç ve ödemeler eğilimi gösterilir. Ayrıca, bu bölümden işlem ayrıntılarını indirebilirsiniz.

:::image type="content" source="images/payouts/transaction-overview.png" alt-text="Iş Ortağı Merkezi portalının sağ üst köşesindeki ödeme simgesini gösterir":::

- **Bu yıla gönderilen kazançlar** – ödenen ve gelecek ayda ödenen toplam kazanç ve döküm dökümü.
- **Tahmini ödeme ayı** – yaklaşan aylarda beklenen toplam kazanç.
- **Kazanç ve ödeme eğilimi** – son 36 aylar için aylık kazanç ve ödeme tutarları.
- **İndir** – işlem ayrıntılarını. csv veya. tsv biçiminde indirin.

Son 3, 6, 12 veya 36 ayı göstermek için sayfanın çıktısını filtrelemek üzere sayfanın sağ üst köşesindeki tarih aralığı seçimini kullanın. Ya da 36 aya kadar bir özel tarih aralığı seçin. Varsayılan tarih aralığı 12 aydır.

:::image type="content" source="images/payouts/search-filter.png" alt-text="Iş Ortağı Merkezi portalının sağ üst köşesindeki ödeme simgesini gösterir":::

### <a name="transaction-history-summary"></a>İşlem geçmişi Özeti

Bu, ürünün sunduğu ve tahmin edilen tarihleri, durumu ve tahmini ödeme ayını kazanmanın kaynağı dahil olmak üzere, ayrıntıları gösterir.

:::image type="content" source="images/payouts/transaction-history.png" alt-text="Iş Ortağı Merkezi portalının sağ üst köşesindeki ödeme simgesini gösterir":::

- **Kazanılan tarih** : satın alma tarihi.
- **Kazanç türü** : satış, Indirim veya ortak işlem gibi kazanç türü.
- **Toplam tutar** – net kazanç miktarı. Ticari Market 'te, bu, standart Market ücreti düşüldükten sonraki anlamına gelir.
- **Durum** – üç seçeneğe sahiptir:
    - **Yaklaşan** – kazanç, bekleyen soğutma döneminde.
    - **İşlenmiş** – kazanç, bir sonraki ödeme için hazırlanır.
    - **Gönderilen** – kazanç ödenmiştir.
- **Tahmini ödeme ayı** : kazancının ödenmesi beklenen ay.

İşlem, ödeme uygunluğu ile buluşduktan sonra işleme işlemleri gösterilir. Neden eksik veya beklenmeyen kazanç olduğunu anlamak için bkz. [ticari Market ödemelerinin genel soruları](payout-faq.md#why-are-my-earnings-missing).

### <a name="transaction-history-download"></a>İşlem geçmişi indirmesi

Bir atma hakkında daha fazla ayrıntı görmek için sayfanın en üstünde **İndir** ' i seçin. Aşağıdaki tabloda, rapordaki her bir sütun açıklanmaktadır.

| Sütun adı | Açıklama | Teşvik için uygulanabilirlik programları/pazar yerleri |
| --- | --- | --- |
| agreementEndDate | Anlaşma bitiş tarihi | Teşvikleri-yalnızca bazı programlar |
| agreementNumber | Anlaşma numarası | Teşvikleri-yalnızca bazı programlar |
| agreementStartDate | Sözleşme başlangıç tarihi | Teşvikleri-yalnızca bazı programlar |
| calculationDate | Sistemin sistemde hesaplandığı Tarih | Tümü |
| Claimıd | Talep için benzersiz tanımlayıcı | Teşvikleri-yalnızca bazı programlar |
| customerCountry | Müşteri ülkesi/bölgesi | marketlerinden |
| customerEmail |  |  |
| customerName | Her zaman boş kalır | Yalnızca programları teşvik edin (özel durum: OEM) ve pazar yerleri |
| Customertenantıd |  |  |
| distributorId | Dağıtıcı tanımlayıcısı | Teşvikleri-yalnızca bazı programlar |
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
| Paymentıd | Ödeme için benzersiz tanımlayıcı. Bu sayı genellikle banka deyiminizde görünür | Yalnızca SAP ödemeleri |
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
| transactionExchangeRate | Karşılık gelen işlem USD tutarını göstermek için kullanılan döviz kuru tarihi | Tümü |
| TransactionId | İşlem için benzersiz tanımlayıcı | Tümü |
| transactionPaymentMethod | İşlem için kullanılan, kart, mobil taşıyıcı faturalandırma veya PayPal gibi müşteri ödeme aracı | marketlerinden |
| Işlem türü | Satın alma, iadesi, ters çevirme veya geri ödeme gibi işlem türü | marketlerinden |
| iş yükü | İş Yükü | Teşvikleri-yalnızca bazı programlar |
|

## <a name="payments"></a>Ödemeler

**Ödemeler** sayfası, Microsoft ile kazandığınızı ayrıntılarıyla ayrıntılardır. Ayrıca ne zaman ve ne kadar ücret ödeeceğini gösterir.

>[!Note]
> Ödemenizin uygun olması için, devam eden $50 [ödeme eşiğine](payment-thresholds-methods-timeframes.md) ulaşmalıdır. Daha fazla bilgi için bkz. [Microsoft Publisher sözleşmesi](https://go.microsoft.com/fwlink/?LinkID=699560).

:::image type="content" source="images/payouts/payments-overview.png" alt-text="Iş Ortağı Merkezi portalının sağ üst köşesindeki ödeme simgesini gösterir":::

- **Toplam ödenen bu yıl** – tüm programlarınız için ABD Doları cinsinden bu yıla kadar ödenen toplam miktar.
- **Sonraki tahmini ödeme** : ABD Doları cinsinden size gelen tek bir sonraki ödeme (çok yakında geliyor olsa bile).
- **Son ödeme** : miktar (ABD Doları cinsinden), program adı ve en son ödemenizin programı.
- **Kaynağa göre ödeme** – son 12 aya göre, her program için ödeme miktarı (ABD Doları cinsinden).

### <a name="payments-list"></a>Ödemeler listesi

**Ödemeler tablosunun listesi** ücretli ve bekleyen ödemeleri gösterir. Hizmet ücreti vergi bilgilerini PDF biçiminde indirebilir ve belirli bir ödemenin kazanç ayrıntılarını görüntüleyebilirsiniz.

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="Iş Ortağı Merkezi portalının sağ üst köşesindeki ödeme simgesini gösterir":::

- **Ücretli** – tüm ödemeler başarıyla gönderildi. Bu yıl içinde Yayınlanan ödemeleri filtrelemek için açılan menüdeki yılı seçin.
- **Bekleyen** – yaklaşan ödemeler.
- **Servis ücreti vergisi (PDF formu)** – ödemeler tabi for Service ücret vergisine göre kullanılabilir. Hizmet ücreti vergileri, **diğer vergilerle** gösterilir.
- **Görüntüle** : işlem geçmişine, ödemeye dahil edilen kazanç listesini kullanarak yeniden yönlendirir.

Neden eksik veya beklenmeyen kazanç olduğunu anlamak için bkz. [ticari Market ödemelerinin genel soruları](payout-faq.md#why-are-my-earnings-missing).

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

Ödemeler hakkında daha fazla ayrıntı görmek için sayfanın en üstünde **İndir** ' i seçin. Aşağıdaki tabloda, rapordaki her bir sütun açıklanmaktadır.

| Sütun adı | Açıklama |
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

**Verileri dışarı aktar** sayfası kendi başına yenilemez. En son verileri görmek için sayfayı el ile yenilemeniz gerekebilir. **İşlem geçmişi** , **ödemeler** , **işlem Özeti** veya **Geçmiş ekstresini** dışarı aktarmak için üç sekmeden birini seçin.

Filtreniz **veri kullanılabilir** hatasıyla sonuçlanabilir. Bu, varsayılan zaman dilimini üç ayda bir kez sola bıraktıysanız ve daha sonra söz konusu dönemin dışında kalan bir ödeme KIMLIĞI seçtiyseniz meydana gelir. Bu durumda, zaman döneminizin kapsamını genişletip yeniden deneyin.

Örnek ödemeler dışarı aktarma işlemi aşağıda verilmiştir:

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="Iş Ortağı Merkezi portalının sağ üst köşesindeki ödeme simgesini gösterir":::

### <a name="historical-statements"></a>Geçmiş deyimleri

**Dışarı aktarma verisi** Özeti Ayrıca geçmiş deyimlerine erişim sağlar.

> [!NOTE]
> Geçmiş bir ifade bir anlık görüntüdür ve yenilenmez. Lütfen [desteğe](https://partner.microsoft.com/support/v2/?stage=1) başvurun ve gerekirse en son verileri isteyin.

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="Iş Ortağı Merkezi portalının sağ üst köşesindeki ödeme simgesini gösterir" durumuna eşit olan tüm kazançları hariç saklayan bir sütun içerir.
- 3K, 6k veya 12D gibi filtreler geçmiş deyimler bölümüne uygulanmaz.

### <a name="historical-statement-downloads"></a>Geçmiş ekstresi İndirmeleri

Aşağıdaki tabloda bir geçmiş deyimindeki her bir sütun açıklanmaktadır.

| Alan adı | Açıklama |
| --- | --- |
| Gelir kaynağı | Microsoft Store, Windows Phone Mağazası, Windows Mağazası 8 veya reklam gibi işlem gerçekleştiği yere göre gelirinin kaynağı |
| Sipariş kimliği | Benzersiz sipariş tanımlayıcısı. Bu KIMLIK, satın alma veya geri ödeme gibi satın alma işlemleri olmayan işlemlerle Satınalma işlemlerini tanımlamanızı sağlar. Her ikisinin de aynı sıra KIMLIĞI olur. Ayrıca, tek bir satın alma işlemi için birden çok ödeme yönteminin kullanıldığı bir bölünmüş ücret varsa, satın alma işlemlerini bağlayabilmeniz sağlanır. |
| İşlem kimliği | Benzersiz işlem tanımlayıcısı. |
| İşlem tarihi saati | İşlemin gerçekleştiği tarih ve saat (UTC). |
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