---
title: Azure planı faturalaması - & mutabakat dosyaları
ms.topic: article
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Azure planının faturalaması ile ilgili fatura ve mutabakat dosyası yapısına erişmeyi ve bu yapıyı anlamayı öğrenin.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: ad04b7af67bb4cf664b2a552c94fc96fa25e5349
ms.sourcegitcommit: e1da62b36420d78bf44e3962358d0af65ebc3402
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129089275"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>CSP'de yeni ticari deneyim - Azure faturalama

**Uygun roller:** Yönetici aracısı | Faturalama yöneticisi | Genel yönetici

Bu makalede, Azure planının faturalaması ile ilgili fatura ve mutabakat dosyası yapısına erişme ve bu yapıyı anlama açıklanmıştır. Azure planı kapsamında faturalama, uyumlu bir tek faturalama tarihi ve takvim ayı tabanlı faturalama dönemi kullanılarak basitleştirilmiş bir faturalama deneyimidir.

## <a name="summary-of-billing-essentials"></a>Faturalama temellerinin özeti

- **Fatura tarihi:** Fatura ve mutabakat dosyası, İş Ortağı Merkezi (gece yarısı UTC) kadar panoda/API'de kullanılabilir.

- **Fatura faturalama dönemi:** Fatura faturalama dönemi takvim ayıyla hizalanır; örneğin, 10/1-10/31, 11/1-11/30.

- **Ücret hizmeti dönemleri:** Ücretler takvim ayıyla uyumlu olur. Örneğin, faturalandırmış iş ortağı azure hizmetlerini 10/15 tarihinde bir Azure planı aracılığıyla eklerse ve müşteri Azure hizmetlerinin tüketimini 10/15'te başlarsa, faturalandırmış iş ortağı 10/15 - 10/31 hizmet dönemi için müşteri tüketimi için 11/8'de fatura/mutabakat alır. 12/8 tarihinde oluşturulacak sonraki ayın faturası, 11/1- 11/31 hizmet dönemi için tüm ücretleri içerir.

- **Fatura ödeme dönemi:** Net 60 gün.

- **Fatura para** birimi: Ağustos 2021'den itibaren geçerli olacak şekilde, ürünleri sattığınız müşterinin konumu ne olursa olsun tüm iş ortakları iş ortağı konumu para birimi cinsinden faturalandırılacaktır.

- **İş ortağı teşvikleri:** Fatura ayı sonundan itibaren 45 gün boyunca ödeme.

## <a name="access-your-invoices-and-reconciliation-files"></a>Fatura ve mutabakat dosyalarınıza erişme

Fatura görüntülemeye hazır olduğunda, şirketinizin genel yöneticisi veya faturalama yöneticisi bir e-posta alır.

Fatura ve mutabakat dosyasına erişmek için:

> [!NOTE]
> Çalışma alanları arabirimi hakkında daha fazla bilgi edinmek için [bkz. İş Ortağı Merkezi.](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Çalışma alanları görünümü](#tab/workspaces-view)

1. Panodan [İş Ortağı Merkezi](https://partner.microsoft.com/dashboard/) **kutucuğunu** seçin.

2. Yinelenen ve Tek Sefer **sekmesini** **ve ilgilendiğinizi** para birimini seçin.

   :::image type="content" source="images/azure/billing-workspace-1.png" alt-text="Faturalama geçmişini gösteren ekran görüntüsü.":::

3. Fatura **veya Mutabakat** dosyasını **seçin.**

   Geçmiş faturaları ve mutabakat dosyalarını görüntülemek için aşağıdaki Faturalama geçmişi satırına bakın.

#### <a name="current-view"></a>[Geçerli görünüm](#tab/current-view)

1. Panodan [İş Ortağı Merkezi'ı](https://partner.microsoft.com/dashboard/) **seçin.**

2. Yinelenen ve Tek Sefer **sekmesini** **ve ilgilendiğinizi** para birimini seçin.

   :::image type="content" source="images/azure/billing3.png" alt-text="Fatura.":::

3. Fatura **veya Mutabakat** dosyasını **seçin.**

   Geçmiş faturaları ve mutabakat dosyalarını görüntülemek için aşağıdaki Faturalama geçmişi satırına bakın.

* * *

## <a name="about-usage-data"></a>Kullanım verileri hakkında

- Azure planı, kullanım için kök veya üst düzey kapsayıcıdır. Tüm kullanımlar tek bir Azure planına geri bağlanır.

- Bir plan içinde bir veya daha fazla Azure aboneliği olur. Bunlar kaynak yönetimi ve dağıtımı için kullanılan kapsayıcılardır.

- Bir abonelik içinde kaynak grupları, grup kaynaklarına ekler. Her kaynak bir kaynak grubuna dağıtılır.

- Kaynak örnekleri arasında sanal makineler ve depolama hesapları yer almaktadır.

- Kaynak yayma ölçümleri: Ölçümler, bir kaynağın tüketiminin ölçümleridir ve bir kaynak birden çok ölçüm için kullanım yayıyor olabilir. Metre bir ProductId, SKUId ve AvailabilityId ile tanımlanır.

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a>Abonelik kaynak grupları ve ölçüm hiyerarşisi

**Azure hesabı (kiracı)**

- Abonelik A
    - ResourceGroup 1
        - Sanal makine (kaynak)
            - İşlem ölçümü
        - Sanal ağ (kaynak)
            - Faturalama ölçümü yok

    - ResourceGroup 2
        - Sanal makine (kaynak)
            - Bilgisayar ölçümü
        - Premium SSD tarafından yönetilen disk (kaynak)
            - Depolama kapasitesi ölçümü
            - Depolama işlem ölçümü

- B Aboneliği -ResourceGroup 1 - Azure SQL (kaynak) - DTU ölçümü - VPN Gateway (kaynak) - VPN ağ geçidi ölçümü

    - ResourceGroup 2
        - Sanal Ağ Arabirimi (kaynak)
            - Faturalama ölçümü yok

## <a name="about-your-invoice"></a>Faturanız hakkında

- Fatura her ayın sekizlik günü kadar kullanılamaz.

- İş ortaklarının ödemelerini geri ödemesi için 60 günü olur.

- Faturalama dönemi, 10/1-10/31 gibi bir takvim ayı kapsar.

- Ücretler net ayarlamalardır ("Yönetilen hizmetler için iş ortağı tarafından kazanılan kredi" tutarıdır).

- Ek faturalama ayrıntıları için fatura mutabakat dosyasını ve günlük olarak derecelendirilmiş kullanım dosyasını gözden geçirme.

   :::image type="content" source="images/azure/invoice1.png" alt-text="Fatura.":::

## <a name="about-your-invoice-reconciliation-file"></a>Fatura mutabakat dosyanız hakkında

- Her Azure planı ve ölçüm bileşimi, mutabakat (mutabakat) dosyasında en fazla iki faturalama satırına sahip olabilir.

- Ölçüm, takvim ayı boyunca herhangi bir türde indirim veya krediye (katmanlı indirimler veya yönetilen hizmetler için İş ortağı tarafından kazanılan kredi gibi) uygunsa mutabakat dosyasında yalnızca bir faturalama satırı yer alır. **PriceAdjusmentDescription sütunu indirime** veya kazanılan krediye başvurur.

- İndirim veya iş ortağı tarafından kazanılan kredi için uygun olan belirli bir ölçüm için kaynak yoksa mutabakat dosyasında yalnızca bir faturalama satırı yer alır ve geçerli birim fiyat perakende fiyatı (birim fiyattır) olur.

- Ölçüm veya ölçümü yayan herhangi bir kaynak,  ayın bir parçası için yönetilen hizmetler için İş ortağı tarafından kazanılan kredi için uygunsa, mutabakat dosyasında iki faturalama satırı yer alacak. Bir satır ölçümün uygun olduğu günleri, ikinci satır ise ölçümün uygun olmadığının günlerini temsil edecek.

> [!NOTE]
> Azure tüketiminizi tek kullanımlık satın alma mutabakat dosyanıza uzlaştırabilirsiniz. Bunu yapmak için günlük olarak derecelendirilmiş kullanım mutabakat dosyanıza gidin ve SubscriptionID'nizi bulun. Bu, Azure plan kimliğinizle ilişkili tüm maliyetleri görüntüler. Azure SubscriptionID'niz EntitlementID olarak gösterilir.

## <a name="read-the-daily-usage-file"></a>Günlük kullanım dosyasını okuma

- Azure planı kapsamındaki abonelik sayaçları, günlük olarak derecelendirilmiş ve bir şekilde toplanıyor.

- **Yönetilen hizmetler için iş ortağı tarafından kazanılan** kredi, günlük olarak belirlenir ve uygulanır.

- Her abonelik ölçüm, tüketimin olduğu ayın her günü için bir satıra sahip olur.

- Aşağıdaki örnekte:

  - **1-7/3** arasında yönetilen hizmetler için İş ortağı tarafından kazanılan kredi için uygun ölçüm (geçerli birim fiyatın perakende fiyatı, iş ortağı tarafından kazanılan krediden daha düşük olduğunu unutmayın.

  - Ölçüm, **7/4** - 7/7 arasında yönetilen hizmetler için İş ortağı tarafından kazanılan kredi için uygun değildi (geçerli birim fiyatın perakende fiyatı olduğunu unutmayın).

  - **7/8** - 7/31 arasında yönetilen hizmetler için İş ortağı tarafından kazanılan kredi için uygun ölçüm (geçerli birim fiyatın perakende fiyatı daha az iş ortağı tarafından kazanılan kredi olduğunu unutmayın).

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2.":::

## <a name="invoice-in-partner-location-currency"></a>İş ortağı konumu para birimi cinsinden fatura

Azure planı aracılığıyla azure hizmetleri ABD doları olarak fiyatlandırılıyor ve iş ortağı ülkenin atanan para biriminde faturalandırılıyor. Faturalama para birimi USD olmayan bir değerse, kullanılan Döviz kuru (FX) faturanın son sayfasında gösterilir. FX fiyatları aylık olarak belirlenir ve aşağıdaki faturaya uygulanır. Ülke para birimlerinin tam listesi için lütfen yeni ticari teklifler ülke kullanılabilirliği ve iş ortağı [para birimi matrisini görüntüebilirsiniz.](https://go.microsoft.com/fwlink/?linkid=2112354)

Microsoft, her takvim ayı için satın alınan veya tüketilen Azure hizmetlerinin toplam ücretlerine varmak için temel USD fiyatlarına önceden belirlenen bir döviz kuru uygular. Aylık döviz kuru, Thomson Tümcesi (genellikle) tarafından önceki ay sonundan iki iş günü önce gmt'de saat 16:00'da yayımlanan orta fiyattır.

**Örneğin,** Microsoft'un Aralık döviz kuru, verili bir para birimi için 29 Kasım'da veya yaklaşık olarak Thomson Mid-rate olur. Bu oran, 1 Aralık ile 31 Aralık arasında bu para birimiyle yapılan tüm satın almalara uygulanır.

## <a name="azure-reservations"></a>Azure rezervasyonları

Bir [Azure planı aracılığıyla](azure-reservations.md) Azure rezervasyonları satın alırsanız, tek kullanımlık veya aylık faturalamayı seçebilirsiniz.

## <a name="azure-spending"></a>Azure harcaması

Mevcut Azure harcama deneyimi, azure'da yeni Azure planı faturalaması desteği İş Ortağı Merkezi. Bu, iş ortaklarının şunları sağlar:

- Müşteri düzeyinde ayarlanmış bütçe uyarılarını görüntüleme, yönetme ve alma

- Azure planında toplam tahmini harcamayı görüntüleme (kaynağa ve ölçüm düzeyine göre aşağı doğru)

Azure planı aracılığıyla Azure hizmetlerinin faturalama modeli ödeme sonrası tüketim olduğundan, beklenenden daha büyük bir faturayı önlemek için iş ortakları aylık bütçe uygulayabilir ve kullanım yüzdesini izleyebilir. Bütçe bir defada bir müşteriye veya birden çok müşteriye uygulanabilir.

:::image type="content" source="images/azure/azurespend.png" alt-text="Azure harcaması.":::

## <a name="next-steps"></a>Sonraki adımlar

- İş ortağı tarafından kazanılan kredinin (PEC) nasıl hesaplanmasına bakın. İş Ortağı Merkezi [panosunda oturum açın](https://partner.microsoft.com/dashboard/) ve fiyatlandırma listelerini **bulmak** için Fiyatlandırma kutucuğunu seçin.

- Azure planını [satın alma hakkında bilgi edinin](purchase-azure-plan.md)

- [CSP'de yeni ticaret deneyimi için fiyat listesine bakın](azure-plan-price-list.md)
