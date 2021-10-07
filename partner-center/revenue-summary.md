---
title: İş Ortağı Merkezi panosunda gelir özeti
description: Azure hizmetlerinin müşteri tüketimi tarafından oluşturulan gelirin kazançlarınız için ne kadar katkı sağlayacağını ve bazı gelirlerin kazançlar için neden uygun olmayan olarak belirlenebilir olduğunu anlamak için Gelir özetini kullanabilirsiniz.
author: satinder37
ms.author: sabaja
ms.service: partner-dashboard
ms.topic: conceptual
ms.date: 10/04/2021
ms.custom: template-concept
customer intent: As an incentive user or incentive admin, I want to be able to read and export revenue data from Partner Center so I can see our earnings and learn why any transactions were reported ineligible.
ms.openlocfilehash: 11e58324adf38e92fc892ec5dd62933e6372f2cb
ms.sourcegitcommit: 76a7dac540d129ae15cd4c251a4ff43d768370da
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/06/2021
ms.locfileid: "129593353"
---
# <a name="revenue-summary"></a>Gelir özeti

Azure hizmetlerinin müşteri tüketimi tarafından oluşturulan gelirin kazançlarınız için ne kadar katkı sağlayacağını ve bazı gelirlerin kazançlar için neden uygun olmayan olarak belirlenebilir olduğunu anlamak için Gelir özetini kullanabilirsiniz.

:::image type="content" source="images/revenue-summary/revenue-reporting-diagram.png" alt-text="Gelirin değerlendirme ve rapor durumunun İş Ortağı Merkezi":::

Gelir özeti yalnızca işlemler değerlendirildikten sonra güncelleştirilir. Bu nedenle Ekim ayında yapılan Azure tüketimi, Örneğin, Kasım ayına kadar Gelir özette görünmez.

Gelir özeti, İşlem geçmişi ve Ödemeler sayfasıyla [birlikte Ödemeler](https://partner.microsoft.com/dashboard/payouts/reports/transactionhistory) [çalışma alanındadır.](https://partner.microsoft.com/dashboard/payouts/reports/incentivepayments)

## <a name="using-the-revenue-summary"></a>Gelir özetini kullanma

Gelir özetini kullanarak şunları da s işin:

- Müşteriye veya aboneliğe göre uygun geliri ve elde edilen kazanç miktarını öğrenin.
- İşlem geçmişinden elde edilen bilgileri [temel alınan gelir](https://partner.microsoft.com/dashboard/payouts/reports/transactionhistory)  tutarları hakkında içgörülerle destekle.
- Uygun olmayan gelirleri öğrenin ve bu gelirin uygun olmayan olarak sınıflandırılma nedenini öğrenin.
- Uygun olmayan nedenler ve öznitelikler [](#ineligibility-reasons) de dahil olmak [](#exported-data-attributes)üzere, önemsiz işlemlerle ilgili verileri dışarı aktarın. Bu, bu işlemlerin neden teşvik kazanmadı, anlamanıza yardımcı olur.

## <a name="access-roles-and-permissions"></a>Rollere ve izinlere erişme

Teşvik kullanıcıları ve teşvik yöneticileriNin Gelir özetine erişimi vardır.
Özette yer alan bilgiler programa ve bu Microsoft İş Ortağı Ağı yöneticilerin (İşlem geçmişi ve Ödemeler sayfalarında olduğu gibi) erişime sahip olduğu tüm (MPN) birleşimlerine bağlıdır. (Kullanıcıları [roller ve parolalarla ayarlama](permissions-overview.md) hakkında daha fazla bilgi edinmek için bkz. Rol ve izin atama.)

## <a name="when-data-is-available"></a>Veriler kullanılabilir olduğunda

Azure tüketim verileri genellikle işlemlerin oluştuğu aydan birkaç hafta sonra değerlendirilir. Gelir özeti bilgileri yalnızca değerlendirme tamamlandığında güncelleştirilir. Bu da işlemlerin ne zaman oluştuğu ve ne zaman raporlandığı arasında bir gecikmeye neden olur. Bu nedenle Gelir özetine göre geçerli aya göre tüketimi göremeysiniz. Örneğin Mart verileri genellikle Nisan 2018'in üçüncü haftasında değerlendirilecek ve Gelir özeti bilgileri genellikle kısa bir süre sonra güncelleştirilecektir.

## <a name="customer-summary-view"></a>Müşteri özeti görünümü

Müşteri özeti görünümü, müşteri adına ve programa/katılıma göre toplanan geliri gösterir.

Müşteri özeti içgörüleri şunları içerir:

- **Uygun gelire göre ilk 10 müşteri,** en yüksek uygun gelire katkıda bulunan ilk 10 müşteriyi gösterir.
- **Uygun olmayan gelire göre ilk 10 ürün,** en yüksek gelire katkıda bulunan ilk 10 müşteriyi gösterir.
- **Kazançlara göre ilk 10'da** en fazla kazanç sağlayan ilk 10 müşteri yer aldı.

Yalnızca ilk 10'a değil, müşteri özet kısmında herhangi bir müşteri hakkında bilgi arayabilirsiniz.

## <a name="eligible-transactions"></a>Uygun işlemler

*Uygun işlemler,* kazanç ödemeleri için uygun gelir üreten işlemlerdir.

Müşteri kimliğine veya abonelik kimliğine göre uygun işlemler hakkında bilgi arayabilirsiniz. Ancak uygun işlemlerle ilgili verileri dışarı aktaramazsiniz.

## <a name="ineligible-transactions"></a>Önemsiz işlemler

*Önemsiz işlemler,* kazanç ödemeleri için uygun olmayan işlemlerdir.

- Kazançlar için herhangi bir işlemi önemsiz olarak kabul edilen nedenler bu makalenin Uygun olmayan [nedenler](#ineligibility-reasons) bölümünde listelenmiştir.
- MCI teşvikleri  [kazanmama](#exporting-data) nedenlerini bulmanıza yardımcı olmak için, uygun olmayan işlemlerle ilgili verileri arayabilir ve dışarı aktarabilirsiniz.
- Gelir özeti her zaman en son gelir sınıflandırmalarını görüntüler (bu nedenle, bir işlemi bir ay önce nasıl sınıflandırmış olduğunu göresiniz). Bir ay uygun olmayan olarak işaretlenen bir işlem, sonraki ay uygun olarak işaretlenir.

Gelir özetsinde listelenen uygun olmayan işlemlerin öznitelikleri şunlardır:

- ürün
- uygun olmayan gelir
- [uygun olmayan nedeni](#ineligibility-reasons)
- abonelik kimliği
- müşteri adı (genellikle bir abonelik ilk kez faturalandıktan sonra kullanılabilir)

Uygun olmayan işlemleri müşteri adına ve abonelik kimliğine göre arayabilirsiniz. (Görüntülenen kayıt sayısı 10 ile sınırlıdır.) Bu bilgiler sorularınıza yanıt vermiyorsa yardım için de destekle iletişime geçin.

## <a name="ineligibility-reasons"></a>Önemsizlik nedenleri

*Aşağıdaki tablolarda yer alan* önemsiz nedenler gelirin kazançlar için neden uygun olmadığını gösteriyor. Tablolarda yer alan her satırın, uygun olmayan kazançlara sahip bir iş ortağının kazançlar için yeniden uygun olup olmadığı ve nasıl uygun hale geldi hakkında bir açıklaması da vardır.

Bu tablolarda bazı önemsiz nedenler belirli bir etkileşim için geçerli olabilir.

Üç önemsizlik kategorisi vardır:

- [Uygun olmayan müşteri](#ineligible-customer)
- [Uygun olmayan iş ortağı](#ineligible-partner)
- [Uygun olmayan işlem](#ineligible-transaction)

### <a name="ineligible-customer"></a>Uygun olmayan müşteri

|Önemsizlik nedeni|İş ortağı eylemi gerekiyor mu?|Yeniden uygun olma|
|---------|---------|---------|
|Müşteri kamu sektörüdür|Evet, müşteri Birleşik Devletler, Porto Riko veya Hindistan'da|Yürütme kanıtı (POE) isteğine yanıt verdiy ve reddedildi ise yeniden uygun kabul edilemezsiniz. (PoE reddedilirse, neden olduğunu açıklayan bir e-posta gönderilir.)<br><br>İşlem/kazanç tarihini takip edinen 90 gün içinde başka bir POE talepte bulundurarak. (PoE e-postası geldiğinde e-postanın alınarak alınanı onaylayın.) Ayrıca, uygun olmayan neden, abonelik ve müşteri bilgileri ve uyuşmazlık nedeni ile de destekle iletişime geçerek 90 gün içinde önemsizliğe itiraz edebilirsiniz.|
|Çin geliri Çin dışı iş ortağına ait değildir|No|İş ortağı, ilke tarafından yeniden uygun hale kullanılamaz.|

### <a name="ineligible-partner"></a>Uygun olmayan iş ortağı

|Önemsizlik nedeni|İş ortağı eylemi gerekiyor|Yeniden uygun olma|
|---------|---------|---------|
|Gelişmiş özelleştirme gereksinimi karşılanmaz|Yes|[Gelişmiş uzmanlıklar hakkında bilgi](advanced-specializations.md)|
|Uzmanlık durumu karşılanmaz veya süresi dolmaz|Yes|Yetkinlikler'de yetkinlik durumunu [görüntüleme.](https://partner.microsoft.com/pcv/partnership/competencies) Teşvikler Katılımları'nda katılımınız için [gerekli yetkinlikleri görüntüleme](https://partner.microsoft.com/dashboard/incentives/engagements/ux)|
|MPA anlaşmasının süresi doldu veya imzalanmaz|Yes|CSP programı iş ortakları için Microsoft İş Ortağı Sözleşmesi [MPA anlaşmasını doğrulama ve imzalama](microsoft-partner-agreement.md)|
|Ortak satış uygunluğunun süresi doldu veya kurulmadı|Yes|Bkz. [Microsoft satış ekipleri ve iş ortaklarıyla ortak satışa genel bakış](/azure/marketplace/co-sell-overview)|
|İş ortağı konumu teşvikler için uygun değil|No|İş ortağı ilke tarafından yeniden uygun hale olamaz|
|MPN Kimliği katılım için uygun değil|No|İş ortağı ilke tarafından yeniden uygun hale olamaz|

### <a name="ineligible-transaction"></a>Uygun olmayan işlem

|Önemsizlik nedeni|İş ortağı eylemi gerekiyor mu?|Yeniden uygun olma|
|---------|---------|---------|
|Yürütme kanıtı onaylanmadı|Evet, Microsoft'tan dijital bir kayıt iş ortağı (DPOR) yürütme kanıtı gerekli (POE) e-postası yanıtlamadıysanız|Yürütme kanıtı isteği yalnızca kamu sektörü veya DPOR için geçerlidir. 1 Ekim 2021'den itibaren geçerli olmak üzere DPOR artık Azure için hazırlanmaz, dolayısıyla POE istekleri gönderilmez.<br><br>E-postaya "Yürütme kanıtı gerekiyor" konusuyla yanıt verdiy ve yanıtınız reddedildi ise, yeniden uygun kabul edilemezsiniz.|

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
