---
title: Azure plan faturalandırma-fatura & keşfi dosyaları
ms.topic: article
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Azure planına yönelik faturalandırma ile ilgili fatura ve mutabakat dosya yapısına erişme ve bunları anlama hakkında bilgi edinin.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: a5942cf0fb69dc94cb45184a2abb9e8f6068073b
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129074217"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>CSP'de yeni ticari deneyim - Azure faturalama

**Uygun roller**: yönetici Aracısı | Faturalandırma Yöneticisi | Genel yönetici

Bu makalede, Azure planına yönelik faturalandırma ile ilgili fatura ve mutabakat dosya yapısına nasıl erişebileceğiniz ve anlayabileceğiniz açıklanır. Azure planı altında faturalandırma, hizalanmış bir tek faturalandırma tarihi ve takvim ay tabanlı fatura dönemi kullanan Basitleştirilmiş bir faturalandırma deneyimidir.

## <a name="summary-of-billing-essentials"></a>Faturalandırma temelleri Özeti

- **Fatura tarihi**: fatura ve mutabakat dosyası, 8 (gece yarısı UTC) tarafından iş ortağı merkezi panosunda/API 'de kullanıma sunulacaktır.

- **Fatura fatura dönemi**: fatura fatura dönemi, takvim ayına hizalanır, örneğin, 10/1-10/31, 11/1-11/30.

- **Ücret Servisi dönemleri**: ücretler takvim ayına hizalanır. Örneğin, faturalandırılan iş ortağı 10/15 tarihinde bir Azure planı aracılığıyla Azure hizmetleri eklerse ve müşteri Azure hizmetleri 'ni 10/15 ' de kullanmaya başlarsa, faturalandırılan servis dönemi 10/15-10/31 olan müşteri tüketimi için, faturalanan iş ortağı, 11/8 tarihinde fatura/keşfi alır. 12/8 tarihinde oluşturulacak bir sonraki aya ait fatura, 11/1-11/31 servis dönemine yönelik tüm ücretleri içerir.

- **Fatura ödeme dönemi**: net 60 gün.

- **Fatura para birimi**: geçerli Ağustos 2021, tüm iş ortakları, ürünü satdığınız müşterinin konumundan bağımsız olarak iş ortağı konumu para birimiyle faturalandırılır.

- **Partner teşvikleri**: fatura ayının sonundan itibaren ödenen 45 gün.

## <a name="access-your-invoices-and-reconciliation-files"></a>Faturanız ve mutabakat dosyalarınıza erişin

Bir fatura görüntülemeye hazırsanız şirketinizin genel yönetici veya faturalama yöneticisi bir e-posta alır.

Faturaya ve mutabakat dosyasına erişmek için:

> [!NOTE]
> Iş Ortağı Merkezi önizleme arabirimi, mantıksal olarak gruplanmış çalışma alanları aracılığıyla daha verimli ve üretken bir kullanıcı deneyimi sağlar. Çalışma alanları arabirimi ve nasıl kullanılacağı hakkında daha fazla bilgi edinmek için bkz. [Iş ortağı merkezini alma](get-around-partner-center.md#turn-workspaces-on-and-off).

#### <a name="workspaces-view"></a>[Çalışma alanları görünümü](#tab/workspaces-view)

1. [Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) **faturalandırma** kutucuğunu seçin.

2. **Yinelenen** ve **tek seferlik** ve ilgilendiğiniz para biriminin sekmesini seçin.

   :::image type="content" source="images/azure/billing-workspace-1.png" alt-text="Faturalama geçmişini gösteren ekran görüntüsü.":::

3. **Fatura** veya **Mutabakat dosyası** seçin.

   Geçmiş faturaları ve mutabakatı dosyalarını görüntülemek için, aşağıdaki faturalama geçmişi satırını genişletin.

#### <a name="current-view"></a>[Geçerli görünüm](#tab/current-view)

1. [Iş Ortağı Merkezi panosundan](https://partner.microsoft.com/dashboard/) **faturalandırma**' i seçin.

2. **Yinelenen** ve **tek seferlik** ve ilgilendiğiniz para biriminin sekmesini seçin.

   :::image type="content" source="images/azure/billing3.png" alt-text="ödeme.":::

3. **Fatura** veya **Mutabakat dosyası** seçin.

   Geçmiş faturaları ve mutabakatı dosyalarını görüntülemek için, aşağıdaki faturalama geçmişi satırını genişletin.

* * *

## <a name="about-usage-data"></a>Kullanım verileri hakkında

- Azure planı, kullanım için kök veya üst düzey kapsayıcıdır. Tüm kullanımlar tek bir Azure planına geri bağlanır.

- Bir plan içinde, bir veya daha fazla Azure aboneliği olacaktır. Bunlar, kaynak yönetimi ve dağıtımı için kullanılan kapsayıcılardır.

- Bir abonelik içinde, kaynak grupları grup kaynaklarına ekler. Her kaynak bir kaynak grubuna dağıtılır.

- Kaynak örnekleri, sanal makineler ve depolama hesapları içerir.

- Kaynak yayma ölçümleri: ölçümler, bir kaynağın tüketim ölçümleridir ve bir kaynak birden fazla ölçüm için kullanım yayabilir. Ölçümler, bir ProductID, SKUId ve kullanılabilirlik kimliği ile tanımlanır.

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a>Abonelik kaynak grupları ve ölçüm hiyerarşisi

**Azure hesabı (kiracı)**

- Abonelik A
    - ResourceGroup 1
        - Sanal makine (kaynak)
            - İşlem ölçümü
        - Sanal ağ (kaynak)
            - Faturalandırma ölçümü yok

    - ResourceGroup 2
        - Sanal makine (kaynak)
            - Bilgisayar ölçer
        - Premium SSD tarafından yönetilen disk (kaynak)
            - Depolama kapasite ölçümü
            - Depolama işlemler ölçümü

- abonelik B-ResourceGroup 1-Azure SQL (kaynak)-DTU ölçer-VPN Gateway (kaynak)-VPN ağ geçidi ölçer

    - ResourceGroup 2
        - Sanal ağ arabirimi (kaynak)
            - Faturalandırma ölçümü yok

## <a name="about-your-invoice"></a>Faturanızda

- Fatura, her ayın sekizinci ' inden daha sonra kullanılabilir olacaktır.

- İş ortaklarının ödemeye havale etmek için 60 gün vardır.

- Fatura dönemi belirli bir takvim ayını kapsar. Örneğin, 10/1-10/31.

- Ücretler, ayarlamaların miktarıdır ("hizmet için Iş ortağı kazanılmış kredinin yüzdesi").

- Fatura keşfi dosyasını ve günlük derecelendirmeli kullanım dosyasını, ek faturalandırma ayrıntıları için gözden geçirin.

   :::image type="content" source="images/azure/invoice1.png" alt-text="faturalayabilirsiniz.":::

## <a name="about-your-invoice-reconciliation-file"></a>Fatura mutabakat dosyanız hakkında

- Her Azure planı ve ölçüm kombinasyonu, mutabakat (keşfi) dosyasında en fazla iki faturalandırma satırı olabilir.

- Ölçüm, tüm takvim ayı boyunca herhangi bir indirim veya kredi türü (katmanlı iskontolar veya hizmet için Iş ortağı için kazanılan kredi gibi) için uygun değilse, keşfi dosyası yalnızca bir faturalandırma satırı içerir. **Priceayarlanmentdescription** sütunu, iskontoya veya kazanılan krediye başvurur.

- Belirli bir ölçüm için, indirimin veya iş ortağının kazanılmasını karşılayan bir kaynak yoksa, keşfi dosyası yalnızca bir faturalandırma satırı içerir ve geçerli birim fiyatı perakende fiyatı (birim fiyatı) olacaktır.

- Ölçüm veya bu ölçümü yayan herhangi bir kaynak, ayın bir parçası için **yönetilen hizmet Için Iş ortağı kazanılmış kredi** için uygun olan, keşfi dosyası iki faturalandırma satırı içerecektir. Tek bir satır, ölçüm 'in uygun olmadığı günleri temsil eder ve ikinci satır, ölçümün uygun olmadığı günleri temsil eder.

> [!NOTE]
> Azure tüketiminizi tek seferlik satın alma keşfi dosyanızda mutabık hale getirebilirsiniz. Bunu yapmak için, günlük derecelendirdiğiniz kullanım keşfi dosyasına gidin ve SubscriptionID 'nizi arayın. Bu, Azure plan KIMLIĞINIZLE ilişkili tüm maliyetleri görüntüler. Azure SubscriptionID 'niz EntitlementID olarak gösterilir.

## <a name="read-the-daily-usage-file"></a>Günlük kullanım dosyasını okuyun

- Bir Azure planı kapsamındaki abonelik ölçümleri derecelendirilir ve günlük olarak birikmiştir.

- **Yönetilen hizmetler Için Iş ortağı kazanılmış kredisi** , günlük olarak belirlenir ve uygulanır.

- Her abonelik ölçünün, her ay için tüketimin olduğu her gün için bir satır olacaktır.

- Aşağıdaki örnekte:

  - 7/1-7/3 ' dan **yönetilen hizmetler Için Iş ortağı kazanılmış kredi** için uygun ölçüm (etkin birim fiyatının, perakende fiyatı daha az iş ortağı kazanılan kredisi olduğunu aklınızda bulunur.

  - Ölçüm, 7/4-7/7 ' dan **yönetilen hizmetler Için Iş ortağı kazanılmış kredi** için uygun değil (geçerli birim fiyatı perakende fiyatı).

  - 7/8-7/31 ' dan **yönetilen hizmetler Için Iş ortağı kazanılmış kredi** için uygun ölçüm (geçerli birim fiyatı, perakende fiyatı daha az iş ortağı kazanılan kredidir).

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2.":::

## <a name="invoice-in-partner-location-currency"></a>İş ortağı konumunda fatura para birimi

Azure planı aracılığıyla Azure Hizmetleri, ABD Doları cinsinden fiyatlandırılır ve iş ortağı ülkenin atandığı para birimiyle faturalandırılır. Faturalama para birimi ABD dışı ise, kullanılan yabancı Exchange (FX) ücreti faturanın son sayfasında gösterilir. FX ücretleri aylık olarak belirlenir ve aşağıdaki faturaya uygulanır. Ülke para birimlerinin tam listesi için lütfen [Yeni ticaret teklifleri ülke kullanılabilirliği ve iş ortağı para birimi matrisini](https://go.microsoft.com/fwlink/?linkid=2112354)görüntüleyin.

Microsoft, her takvim ayında satın alınan veya tüketilen Azure hizmetleri için tahakkuk eden toplam ücretlere ulaşmak üzere ABD Doları fiyatlarını temel alan önceden tanımlı bir döviz kuru uygular. Aylık Döviz Kuru, Thomson depolarında (genellikle), önceki aya ait 4:00 PM GMT 'den önce iki iş günü tarafından yayımlanan orta orandır.

**Örneğin,** Microsoft 'un Aralık değişimi oranı, belirli bir para birimi için, 29 Kasım veya bu yana ABD 'de veya sonrasında Tomson yeniden başlatılıyor. Bu oran, 1 Aralık 'tan 31 Aralık 'a kadar bu para birimindeki tüm satınalmalara uygulanır.

## <a name="azure-reservations"></a>Azure rezervasyonları

Azure [ayırmaları](azure-reservations.md) bir Azure planıyla satın alıyorsa, tek seferlik veya aylık faturalandırma seçeneklerinden birini belirleyebilirsiniz.

## <a name="azure-spending"></a>Azure harcaması

Mevcut Azure harcama deneyimi, Iş Ortağı Merkezi 'nde yeni Azure planı faturalandırmasını destekleyecek şekilde güncelleştirildi. Bu, iş ortaklarının şunları yapmasına olanak sağlar:

- Müşteri düzeyinde bütçe kümesi için uyarıları görüntüleyin, yönetin ve alın

- Bir Azure planında toplam tahmini harcama (kaynak ve ölçüm düzeyine göre ayrılmış) görüntüleyin

Azure planı aracılığıyla Azure hizmetleri için faturalandırma modeli, daha büyük bir faturanız beklenenden daha büyük bir fatura olduğundan, iş ortakları aylık bir bütçe uygulayabilir ve kullanım yüzdesini izleyebilir. Bir bütçe, bir kerede bir müşteriye veya birden çok müşteriye uygulanabilir.

:::image type="content" source="images/azure/azurespend.png" alt-text="Azure harcama.":::

## <a name="next-steps"></a>Sonraki adımlar

- Ortağın kazanılan kredisi (PEC) nasıl hesaplanacağını görün. [Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın ve kullanılabilir fiyatlandırma listelerini bulmak için **fiyatlandırma** kutucuğunu seçin.

- [Azure planını satın alma](purchase-azure-plan.md) hakkında bilgi edinin

- [CSP 'de yeni ticaret deneyimi için fiyat listesine](azure-plan-price-list.md) bakın
