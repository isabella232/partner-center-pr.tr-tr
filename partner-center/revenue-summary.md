---
title: Iş Ortağı Merkezi panosundaki gelir Özeti
description: Gelir Özeti görünümünü gelir ve kazanç olarak kullanabilir ve herhangi bir uygun işlem hakkında verileri dışarı aktarabilirsiniz.
author: satinder37
ms.author: sabaja
ms.service: partner-dashboard
ms.topic: conceptual
ms.date: 10/04/2021
ms.custom: template-concept
customer intent: As an incentive user or incentive admin, I want to be able to read and export revenue data from Partner Center so I can see our earnings and learn why any transactions were reported ineligible.
ms.openlocfilehash: 9ec9d64127f537ac74615a8fbe17499ebb5872dd
ms.sourcegitcommit: cf8c78e0c8831371432007d5ab05f934f15a77b5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/05/2021
ms.locfileid: "129528662"
---
# <a name="revenue-summary"></a>Gelir Özeti

Azure hizmetlerinin müşteri tüketimine göre oluşturulan gelirin kazanç açısından nasıl katkıda bulunduğunu ve bazı gelirinin kazanç için ne şekilde saptanabilir olabileceğini anlamak için gelir özetini kullanabilirsiniz.

:::image type="content" source="images/revenue-summary/revenue-reporting-diagram.png" alt-text="Gelirin nasıl değerlendirildiğini ve Iş Ortağı Merkezi 'nde nasıl bildirildiğini gösteren diyagram":::

Gelir Özeti yalnızca işlemler hesaplandıktan sonra güncelleştirilir, bu nedenle Ekim ayında yer alan Azure tüketimi, Kasım 'a kadar gelir özetinde görünmez.

Gelir Özeti, ödeme çalışma alanında, [işlem geçmişi](https://partner.microsoft.com/dashboard/payouts/reports/transactionhistory) ve [ödemeler sayfasıyla](https://partner.microsoft.com/dashboard/payouts/reports/incentivepayments)birlikte bulunur.

## <a name="using-the-revenue-summary"></a>Gelir özetini kullanma

Gelir özetini kullanarak şunları yapabilirsiniz:

- Müşteri veya aboneliğe göre uygun geliri ve elde edilen kazanç miktarını bulun.
- Temel alınan gelir miktarları hakkındaki öngörülerle [işlem geçmişinden](https://partner.microsoft.com/dashboard/payouts/reports/transactionhistory)  öğrendiklerinizi destekleyebilirsiniz.
- Uygun olmayan geliri bulun ve gelirin neden sınıflandırıldığına ilişkin nedeni öğrenin.
- Bu işlemlerin neden teşvikleri kazanmadığına yardımcı olan [ineligibility nedenler](#ineligibility-reasons) ve [öznitelikler](#exported-data-attributes)de dahil olmak üzere uygun olmayan işlemler hakkında verileri dışa aktarın.

## <a name="access-roles-and-permissions"></a>Rollere ve izinlere erişim

Kullanıcıları teşvik edin ve Yöneticiler, gelir özetine erişebilir.
Özette bulunan bilgiler, kullanıcıların ve yöneticilerin erişimi olan programa ve Microsoft İş Ortağı Ağı (MPN) birleşimlerine (yalnızca Işlem geçmişi ve ödemeler sayfalarında olduğu gibi) bağlıdır. (Kullanıcıların roller ve parolalarla kurulumunu alma hakkında daha fazla bilgi edinmek için bkz. [rolleri ve Izinleri atama](permissions-overview.md) .)

## <a name="when-data-is-available"></a>Veriler kullanılabilir olduğunda

Azure tüketim verileri genellikle hareketlerin oluştuğu aydan birkaç hafta sonra değerlendirilir. Gelir özeti bilgileri yalnızca değerlendirme tamamlandığında güncelleştirilir. Bu, işlemlerin oluşma ve bildirilme işlemleri arasında gecikmeye neden olur, bu nedenle gelir özetinde geçerli ay için tüketimi göremezsiniz. Örnek olarak, Mart için veriler genellikle Nisan 'un üçüncü haftasında değerlendirilir ve gelir Özet bilgileri genellikle kısa bir süre sonra güncelleştirilir.

## <a name="customer-summary-view"></a>Müşteri Özeti Görünümü

Müşteri Özeti Görünümü müşteri adına ve programa/görevlendirmeye göre toplanmış geliri gösterir.

Müşteri Özeti öngörüleri şunları içerir:

- **Uygun gelire göre ilk 10** , en fazla uygun gelire katkıda bulunan ilk 10 müşteriyi gösterir.
- Uygun olmayan **gelire göre ilk 10** müşteri, en fazla sayıda gelirin katkısından en iyi 10 müşteriyi gösterir.
- **Kazanca göre ilk 10** , maksimum kazanç için katkıda bulunan ilk 10 müşteriyi gösterir.

Yalnızca ilk 10 ' a değil, müşteri özetinde herhangi bir müşteri hakkında bilgi için arama yapabilirsiniz.

## <a name="eligible-transactions"></a>Uygun işlemler

*Uygun işlemler* , kazanç ödemeleri için uygun olan geliri üreten işlemlerdir.

Müşteri KIMLIĞINE veya abonelik KIMLIĞINE göre uygun işlemler hakkında bilgi için arama yapabilirsiniz. Ancak uygun işlemler hakkında verileri dışarı aktarabilirsiniz.

## <a name="ineligible-transactions"></a>Kaçınak işlemler

Uygun olmayan *işlemler* , kazanç ödemeleri için uygun olmayan işlemlerdir.

- Tüm işlemlerin kazanç için uygun olmadığı düşünülme nedenleri, bu makalenin [Ineligibility nedenleri](#ineligibility-reasons) bölümünde listelenmiştir.
- Herhangi bir türlü uygun olmayan işlem hakkında verileri arayabilir ve  [dışarı aktarabilirsiniz](#exporting-data) . bu nedenle, hiç kazanılan teşvikleri.
- Gelir Özeti her zaman en son gelir sınıflandırmasını görüntüler (Bu nedenle bir işlemin bir ay önce nasıl sınıflandırıldığını göremezsiniz). Bir ay daha okunaklı olarak işaretlenmiş bir işlem sonraki ay uygun olarak işaretlenebilir.

Gelir özetinde listelenen uygun olmayan işlemler şunlar dahil olmak üzere özniteliklere sahiptir:

- ürün
- uygun olmayan gelir
- [ineligibility nedeni](#ineligibility-reasons)
- abonelik kimliği
- Müşteri adı (genellikle bir abonelik ilk kez faturalandıktan sonra kullanılabilir)

Müşteri adına ve abonelik KIMLIĞINE göre uygun olmayan işlemlere arama yapabilirsiniz. (Görüntülenecek kayıt sayısı 10 ile sınırlıdır.) Bulduğunuz bilgiler sorularınızı yanıtlamadıysanız yardım için desteğe başvurun.

## <a name="ineligibility-reasons"></a>Ineligibility nedenler

Aşağıdaki tablolarda *Ineligibility nedenler* , gelirin kazanç için neden uygun şekilde sınıflandırıldığını gösterir. Tablolardaki her satırda Ayrıca, uygun olmayan kazanç içeren bir ortağın kazanç için yeniden kullanılabilir olup olmadığı hakkında bir açıklama bulunur.

Bu tablolardaki bazı ineligibility nedenleri belirli bir katılım için geçerli olmayabilir.

Üç ineligibility kategorisi vardır:

- [Uygun olmayan müşteri](#ineligible-customer)
- [Uygun olmayan iş ortağı](#ineligible-partner)
- [Uygun olmayan işlem](#ineligible-transaction)

### <a name="ineligible-customer"></a>Uygun olmayan müşteri

|Ineligibility nedeni|İş ortağı eylemi gerekli mi?|Yeniden nasıl uygun hale getirilir|
|---------|---------|---------|
|Müşteri genel sektör|Evet, müşteri Birleşik Devletler, Porto Riko veya Hindistan 'da ise|Bir yürütme kanıtı (POE) isteği için yanıt verdiyseniz ve reddedilirse, tekrar uygun hale gelmemeniz gerekir. (Bir POE reddedildiğinde, nedenini açıklayan e-posta gönderilir.)<br><br>İşlem/kazanç tarihindeki 90 gün içinde başka bir POE isteyebilirsiniz. (Bu, geldiğinde, POE e-postası alındığını onaylamanız emin olun.) Ayrıca, ineligibility nedeni, abonelik ve müşteri bilgileri ve itiraz nedeni ile desteğe başvurarak 90 gün içinde ineligibility de sorumlu olabilirsiniz.|
|Çin geliri Çin olmayan iş ortağına ait olmamalıdır|No|İş ortağı ilke tarafından yeniden uygun hale gelbırakılamaz.|

### <a name="ineligible-partner"></a>Uygun olmayan iş ortağı

|Ineligibility nedeni|İş ortağı eylemi gerekli|Yeniden nasıl uygun hale getirilir|
|---------|---------|---------|
|Gelişmiş özelleşme gereksinimi karşılanmadı|Yes|[Gelişmiş specialmeler hakkında bilgi edinin](advanced-specializations.md)|
|Uzmanlık durumu karşılanmadı veya zaman aşımına uğradı|Yes|Uzmanlıklar için uzmanlık durumunuzu görüntüleyin [.](https://partner.microsoft.com/pcv/partnership/competencies) [Teşvikleri görevlendirmelerde](https://partner.microsoft.com/dashboard/incentives/engagements/ux) , katılımlarınız için gerekli olan uzmanlılığı görüntüleyin|
|MPA sözleşmesinin son kullanma veya imzalı değil|Yes|[CSP program iş ortakları Için Microsoft Iş ortağı sözleşmesi](microsoft-partner-agreement.md) ' ne KıLAVUZLUK ederek MPa sözleşmesini doğrulayın ve imzalayın|
|Ortak satış uygunluk durumu geçildi veya kurulmadı|Yes|Bkz. [Microsoft satış ekipleriyle ortak satış ve iş ortaklarına genel bakış](/azure/marketplace/co-sell-overview)|
|İş ortağı konumu teşvikleri için uygun değil|No|İş ortağı ilke tarafından yeniden uygun hale gelbırakılamaz|
|MPN KIMLIĞI, görevlendirmeye katılmak için uygun değil|No|İş ortağı ilke tarafından yeniden uygun hale gelbırakılamaz|

### <a name="ineligible-transaction"></a>Uygun olmayan işlem

|Ineligibility nedeni|İş ortağı eylemi gerekli mi?|Yeniden nasıl uygun hale getirilir|
|---------|---------|---------|
|Yürütmenin kanıtı onaylanmadı|Evet, Microsoft 'tan bir dijital kayıt iş ortağı (DPOR) yürütme gerekli (POE) e-postası yanıtı verdiyseniz|Yürütme isteğinin kanıtı yalnızca genel sektör veya DPOR için geçerlidir. 1 Ekim 2021 DPVEYA artık Azure için incentivized, bu nedenle POE istekleri gönderilmez.<br><br>E-postaya "yürütme kanıtı gereklidir" konusunu kullanarak yanıt verdiyseniz ve yanıtınız reddedildiyse, tekrar uygun hale gelmemeniz gerekir.|

## <a name="exporting-data"></a>Verileri dışarı aktarma

Gelir özetinde, sınırsız işlem (uygun olmayan işlemler) hakkında bilgi indirebilirsiniz.

:::image type="content" source="images/revenue-summary/export-data-page.png" alt-text="Iş Ortağı Merkezi 'nde verileri dışarı aktar sayfasının ekran görüntüsü":::

### <a name="exported-data-attributes"></a>Aktarılmış veri öznitelikleri

Uygun olmayan işlem öznitelikleri şunlardır:

|Öznitelik adı  |Description  |
|---------|---------|
|agreementNumber|Anlaşma numarası (yalnızca uygun olarak kullanılabilir)|
|customerId|Abonelik/kaynakla ilişkili müşterinin kimliği. (Azure tüketimi için, ilk fatura oluşturulmadığı takdirde bu bilgiler yeni bir aboneliğin ilk 30 ila 45 gün boyunca kullanılamaz.)|
|Customerıdtype|TPıD veya MCAPı KIMLIĞI|
|customerName|Müşterinin adı|
|Faturanumarası|Fatura numarası (yalnızca iş ortakları için kullanılabilir, alan-LED ve müşteri-LED)|
|partnerCountryCode|Kayıtlı MPN konumu|
|iş ortağı kimliği|Kayıtlı ortağın MPN KIMLIĞI|
|partnerName|Ortağın adı|
|productId|Ticari ürün adı|
|productFamily|Ürün ailesi|
|reason|İneligibility nedeni|
|subscriptionId|Abonelik Kimliği|
|transactionAmountUSD|ABD Doları cinsinden tüketim tutarı|
|transactionDate|Tüketim veya faturalandırma tarihi
|Karşılanmadı|Destek sorgusu oluşturmanıza yardımcı olabilecek benzersiz tanımlayıcı|
|iş yükü|Hizmet adı veya iş yükü adı|

## <a name="next-steps"></a>Sonraki adımlar

İşlemler, gelir, kazançlar ve ödemeler hakkında daha fazla bilgi edinmek için aşağıdaki makaleleri görüntüleyin.

- Karşılık gelen ödeme durumuyla tüm programlarınızda kazanç ve ilişkili işlem ayrıntılarını görüntülemek için [işlem geçmişi](https://partner.microsoft.com/dashboard/payouts/reports/transactionhistory) sayfasını görüntüleyin.
- Tüm programlarınız için tamamlanan ve bekleyen ödemeleri görüntülemek üzere [ödemeler sayfasını](https://partner.microsoft.com/dashboard/payouts/reports/incentivepayments) görüntüleyin.
- Ticari Market aracılığıyla satılan tekliflerden ödemalarınızın genel bir görünümünü almak için [ödeme deyimleri](payout-statement.md) sayfasını görüntüleyin.
