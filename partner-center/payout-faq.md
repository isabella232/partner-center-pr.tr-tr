---
title: Microsoft Commercial Market için ödeme hakkında SSS
description: Ticari Market 'teki ödemeler hakkında sık sorulan soruların yanıtlarını alın. Geliriniz beklenenden farklı olan yanıtları içerir.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: keferna
ms.author: keferna
ms.date: 09/11/2020
ms.openlocfilehash: 44bd7f488e3d4e79c45cb2746c7e2a6da449a310
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/19/2020
ms.locfileid: "92532067"
---
# <a name="common-questions-about-commercial-marketplace-payouts"></a>Ticari Market ödeimiyle ilgili sık sorulan sorular

Bu makalede, ticari Market 'teki ödemeler hakkında sık sorulan sorular yanıtlanmaktadır.

## <a name="earnings-incorrect-or-missing"></a>Kazanç yanlış veya eksik

#### <a name="why-are-my-earnings-missing"></a>Kazançlarım neden eksik?

- Müşteri siparişi henüz ödemeye uygun olmayabilir. Kurumsal olmayan müşteri siparişlerinde, yayımcı kazancının uygun duruma gelmesi için önce Microsoft'un müşteri ödemesini alması gerekir. Kurumsal müşteri siparişlerinde, Satın alma siparişi tarihinden sonraki 1-2 gün içinde kazançlarınız kullanılabilir duruma gelir. [Sipariş raporlarında](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order) Sipariş durumunu doğrulayın.
- Temmuz 2019'dan önceki işlemlerden elde edilen kazançlar işlem geçmişi raporunda gösterilmeyebilir. [Ödeme İndirmesi](https://partner.microsoft.com/dashboard/payouts/reports/incentiveexport) içinde Geçmiş Hesap Özetlerini denetleyin.
- [Ödeme döngüsünün zaman çerçevesini](payment-thresholds-methods-timeframes.md) denetleyin ve kullandıkça öde bildiriminde ne zaman görünebileceğini anlayın.

#### <a name="why-is-my-earnings-amount-different-than-what-i-expected"></a>Ne kadar kazanç miktarım, beklendiğim miktardan farklı midir?

- Sipariş müşteriniz tarafından kısmen ödenmişse, kazanç miktarı, ücret düşüldükten ve uygun vergi ile kısmen ödenen miktarı temel alır.
- Ülkeye göre vergi havale sorumluluğunu denetleyin. Vergiden Microsoft'un sorumlu olduğu ülkelerde, Microsoft vergiyi yayımcının kazançlarından toplar ve düşer. Hesap özetinde gösterilen işlem tutarı, vergi sonrası tutardır. [Vergi ayrıntıları](tax-details-marketplace.md) konusuna bakın.
- SaaS ve IaaS teklifleri Standart %20 ' nin yerine %10 oranında indirimli bir kurum ücretine sahiptir ve %90 kazanç oranını bırakır. Bu promosyon 30 Haziran 2021'e kadar geçerlidir.

**Daha fazla** bilgi: ticari Market [Yayımcı Sözleşmesi](https://go.microsoft.com/fwlink/p/?LinkID=699560), [ödeme ilkesi ayrıntıları](payout-policy-details.md), [ödeme eşiği, yöntem ve zaman dilimi](payment-thresholds-methods-timeframes.md), [ticari Market 'teki](marketplace-get-paid.md) [vergi ayrıntıları](tax-details-marketplace.md), [ödeme deyimleri](payout-statement.md), [ticari Market Analytics 'te siparişler panosu](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="earnings-reconciliation"></a>Kazanç mutabakatı
### <a name="how-do-i-reconcile-payout-statements-to-order-or-usage-reports-in-analytics"></a>Ödeme hesap özetleriyle analizdeki sipariş veya kullanım raporlarını nasıl mutabık kılabilirim?
Analitik siparişler ve kullanım raporları ile, ödeme işlem geçmişi raporunda görünen AssetID, OrderID ve Line Item ID kullanın. Bu eşlemeyi kullanın:

- Ödeme İşlem Geçmişi.AssetID = sipariş.OrderID
- Ödeme İşlem Geçmişi.OrderID ve LineItem = Kullanım.UsageReferenceID [OrderID:LineItemID]

### <a name="how-do-i-know-when-to-expect-payments-for-my-customer-orders"></a>Müşterimin siparişleri için ne zaman ödeme alabileceğimi nasıl öğrenirim?
- İlk olarak, assetID ' yi kullanarak [siparişler raporlarında](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order)müşteri siparişlerini kontrol edin.
- [Müşteriler raporunda](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/customer)müşteri aboneliğiniz için müşteri kanalını denetleyin.
- Kuruluş müşterileri için, yayımcı kazançları satınalma siparişi tarihinden sonraki 1-2 gün içinde görüntülenir.
- Kurumsal olmayan müşteriler için yayımcı kazançları, müşteri ödemesi alındıktan sonra 1-2 gün sonra görüntülenir.

**Daha fazla okuma** : [ödeme deyimleri](payout-statement.md), [ticari Market analizlerinde Pano panosu](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="payout-policies"></a>Ödeme ilkeleri

#### <a name="how-do-i-find-the-current-agency-fee-and-the-payout-rate"></a>Geçerli aracı ücretini ve ödeme oranını nasıl bulabilirim?

- Ticari market Yayımcı Sözleşmesini gözden geçirin. Standart aracı ücreti %20'dir. SaaS Co-Sell uygun işlemler %10 oranında indirimli ücretlidir. Promosyonlu aracı ücretlerine ilişkin duyuruları gözden geçirin.
- Ödeme deyiminizde, kazanç oranı belirli bir işlem için gerçek ödeme oranını belirtir.

#### <a name="when-can-i-expect-a-payment-from-microsoft-once-earnings-appear-on-my-statement"></a>Kazançlar hesap özetimde görüntülendikten sonra Microsoft'tan ne zaman ödeme almayı bekleyebilirim?
- Kazancınız işlenmedi durumuna geldikten sonra, kazançlarınızın ödemesinin işleneceği ay için vade tarihini denetleyebilirsiniz. Ödemenizin hazırlandığına göre kazanç durumunuz "işlendi" olarak değişir.  Microsoft vade ayının 15'inde ödemeleri serbest bırakır.
- Kredi kartıyla ödenen siparişlerde, Microsoft, kazanana kadar 30 gün boyunca tutar.

 **Daha fazla okuma** : [ticari Market Yayımcı Sözleşmesi](https://go.microsoft.com/fwlink/p/?LinkID=699560), [ödeme ilkesi ayrıntıları](payout-policy-details.md), [vergi ayrıntıları](tax-details-marketplace.md), [ödeme eşiği, yöntem ve zaman çerçevesi](payment-thresholds-methods-timeframes.md)

## <a name="payments-and-adjustments"></a>Ödemeler ve ayarlamalar

#### <a name="why-is-my-payment-missing"></a>Ödemem neden eksik?

- [Genel Bakış sayfasında](https://partner.microsoft.com/dashboard/commercial-marketplace/overview), ödeme durumunuzu ve vergi profili durumunuzu *geçerli* olarak gösterildiğinden emin olun.
- Ödeme için en düşük eşiğe ulaşamamış olabilirsiniz. Ödeme almak için kazançların en az 50 ABD Doları olması gerekir.


#### <a name="how-do-i-set-my-account-to-not-receive-payment"></a>Hesabımı ödeme almıyor Nasıl yaparım? mi?
Ödeme [profilinde](https://partner.microsoft.com/dashboard/commercial-marketplace/overview)ödemeleri tutabilirsiniz; yalnızca **tutmayı** kontrol edin. Microsoft, bekletme 'yi serbest bırakana kadar ödeme yapmak için ücret ödemenizi sağlar.

#### <a name="why-do-i-receive-in-a-different-currency-than-the-purchase-currency"></a>Neden satın alma para biriminden farklı bir para biriminde ödeme alıyorum?

Ödeme para birimi, ödeme profilinde seçtiğiniz para birimine dayanır. Satın alma para birimi müşterinin ödeme yaptığı para birimine dayanır.

#### <a name="how-do-i-reconcile-adjustments"></a>Düzeltmeleri nasıl mutabık kılabilirim?

Ödeme düzeltmeleri, sistem sorunları gibi telafi ayarlamalarını yapmaya yönelik düzeltmelerdir. Ödeme hesap özetinde ReasonCode, düzeltmenin nedenini belirtir. Bunlar doğrudan tek tek işlemlerin mutabakatına yönelik değildir.

**Daha fazla okuma** : [ticari Market Yayımcı Sözleşmesi](https://go.microsoft.com/fwlink/p/?LinkID=699560), [ödeme ilkesi ayrıntıları](payout-policy-details.md), [vergi ayrıntıları](tax-details-marketplace.md), [ödeme eşiği, yöntem ve zaman çerçevesi](payment-thresholds-methods-timeframes.md)

## <a name="taxes"></a>Vergiler

#### <a name="how-do-we-identify-tax-remit-responsibility-between-microsoft-or-publisher-in-the-payout-statement"></a>Ödeme hesap özetinde Microsoft veya Yayımcının Vergi Ödeme sorumluluğunu nasıl belirleriz?

İşlem geçmişi indirmesinde Vergi modeli sütununu bulun. Burada MS Tarafından Yönetilen veya ISS Tarafından Yönetilen gösterilir. [Vergi ayrıntıları](tax-details-marketplace.md) konusunda, ülkeye özgü vergi kurallarına ve ödemeye etkilerine bakın.

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Hizmet Ücreti Vergi formlarını nasıl indirebilirim?

**Ödeme** sayfasına ve sonra da **Ödeme Listesi** bölümüne gidin. Hizmet Ücreti Vergisi olan ödeme için Hizmet Ücreti vergi formunun bağlantısı görüntülenir.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>PDF biçiminde Stopaj vergisi formunu nasıl indirebilirim?

*Ödeme* sayfasına ve sonra da **Ödeme Listesi** bölümüne gidin. Ödemenin yanında stopaj vergisi formunun bağlantısı görüntülenir.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Yıl sonu vergi formlarını nerede bulabilirim?

Yıl sonu vergi formlarınızı görüntülemek için [Profil sayfasına](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) gidin.

#### <a name="how-do-i-find-withholding-tax-for-a-transaction"></a>Bir işlemin Stopaj vergisini nasıl bulabilirim?
Stopaj vergisi W-9 formu dolduran ABD'li yayımcılara uygulanır. Stopaj vergisi aylık ödeme temelinde hesaplanır.

**Daha fazla okuma** : [ticari Market Yayımcı Sözleşmesi](https://go.microsoft.com/fwlink/p/?LinkID=699560), [ödeme ilkesi ayrıntıları](payout-policy-details.md)

## <a name="payout-statement-access"></a>Ödeme bildirimine erişim

#### <a name="how-do-i-access-a-payout-statement"></a>Ödeme hesap özetine nasıl erişebilirim?

1. Rollerinizi kontrol edin. Ödeme hesap özetine erişmek için *finansal katkıda bulunan* veya *hesap sahibi* rolüne sahip olmalısınız.
2. Ödeme deyiminizi görüntülemek için sağ üst gezinti bölmesinde, **ödeme** simgesini seçin. **Işlem geçmişi** , **ödeme** ve **indirme** arasında seçim yapın.

**Daha fazla okuma** : [ödeme rolleri ve izinleri](payout-statement.md#roles-and-permissions), [ödeme deyimleri](payout-statement.md) 

## <a name="payout-statement-report"></a>Ödeme beyanı raporu

#### <a name="what-does-each-field-in-the-transaction-download-mean"></a>İşlem indirmesindeki alanlar ne anlama geliyor?

Özniteliklerin ayrıntılı listesi ve anlamları için bkz. [Payout deyimleri](payout-statement.md) .

#### <a name="what-is-earning-status"></a>Kazanç durumu nedir?

Bu, bedellerinizi işlenmemiş, işlenmiş veya gönderildi olarak gösterir.

- **İşlenmemiş** – kazanç, vade tarihine kadar bir emanet döneminde.
- **İşlendi** – kazanç, aylık bir ödemeye hazırlanır ve bu işlem için hazır. Ödemeler her ayın 15 ' i oranında serbest bırakılır.
- **Gönderildi** – ödeme, ödeme profilinize göre bankanızla başarıyla serbest bırakıldı.

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Hizmet Ücreti Vergi formlarını nasıl indirebilirim?

**Ödeme** sayfasına ve sonra da **Ödeme Listesi** bölümüne gidin. Hizmet Ücreti Vergisi olan ödeme için Hizmet Ücreti vergi formunun bağlantısı görüntülenir.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Bir stopaj vergisi formunu PDF 'ye Nasıl yaparım? indirmek mi?

**Ödeme** sayfasına ve sonra da **Ödeme Listesi** bölümüne gidin. Ödemenin yanında stopaj vergisi formunun bağlantısı görüntülenir.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Yıl sonu vergi formlarını nerede bulabilirim?

Yıl sonu vergi formlarınızı görüntülemek için [Profil sayfasına](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) gidin.

**Daha fazla okuma** : [ödeme deyimleri](payout-statement.md), [işlem geçmişi indirmesi](payout-statement.md#transaction-history-download)

## <a name="historical-statements"></a>Geçmiş deyimleri

#### <a name="how-do-i-view-historical-information"></a>Nasıl yaparım? geçmiş bilgileri görüntülensin mi?

Geçmiş hesap özetinde Ekim 2019 itibarıyla ödeme verilerinin anlık görüntüsü gösterilir. Ne yazık ki buradaki ödeme bilgileri yenilenmez. En son bilgileri almak için en son veriler için bir destek bileti gönderebilirsiniz.

**Daha fazla okuma** : [ödeme deyimleri](payout-statement.md), [işlem geçmişi indirmesi](payout-statement.md#transaction-history-download)

## <a name="payout-export-api"></a>Ödeme dışarı aktarma API 'SI

#### <a name="how-do-i-download-payout-data"></a>Ödeme verilerini nasıl indirebilirim?

[Iş ortağı ödeme API](https://apidocs.microsoft.com/services/partnerpayouts)'sini kullanın.

## <a name="next-steps"></a>Sonraki adımlar

- [Ticari markette ödeme alma](marketplace-get-paid.md)
