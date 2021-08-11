---
title: Azure planı faturalaması - & mutabakat dosyaları
ms.topic: article
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Azure planının faturalaması ile ilgili fatura ve mutabakat dosyası yapısına erişmeyi ve bu yapıyı anlamayı öğrenin.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 7e2abdc7536521e72265d99369f165eb7c13d7ae8c258e5db6f84fd774877c19
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115691327"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>CSP'de yeni ticari deneyim - Azure faturalama 

**Uygun roller:** Yönetici aracısı | Faturalama yöneticisi | Genel yönetici

Bu makalede, Azure planının faturalaması ile ilgili fatura ve mutabakat dosyası yapısına erişme ve bu yapıyı anlama açıklanmıştır. Azure planı kapsamında faturalama, uyumlu bir tek faturalama tarihi ve takvim ayı tabanlı faturalama dönemi kullanılarak basitleştirilmiş bir faturalama deneyimidir.

## <a name="summary-of-billing-essentials"></a>Faturalama temellerinin özeti

- **Fatura tarihi:** Fatura ve mutabakat dosyası, 8 İş Ortağı Merkezi (gece yarısı UTC) kadar panoda/API'de kullanılabilir.

- **Fatura faturalama dönemi:** Fatura faturalama dönemi takvim ayıyla hizalanır; örneğin, 10/1-10/31, 11/1-11/30.

- **Ücret hizmeti dönemleri:** Ücretler takvim ayıyla aynı olur. Örneğin, faturalandırmış iş ortağı azure hizmetlerini 10/15 tarihinde bir Azure planı aracılığıyla eklerse ve müşteri Azure hizmetlerinin tüketimini 10/15'te başlarsa, faturalandırmış iş ortağı 10/15 - 10/31 hizmet dönemi için müşteri tüketimi için 11/8'de fatura/mutabakat alır. 12/8 tarihinde oluşturulacak sonraki ayın faturası, 11/1- 11/31 hizmet dönemi için tüm ücretleri içerir.

- **Fatura ödeme dönemi:** Net 60 gün.

- **Fatura para** birimi: 28 Ocak 2021'den başlayarak, AB/EFTA ve Birleşik Krallık bölgesinde yeni müşterileri olan iş ortakları ve kiracıları 11 Mayıs 2020'den önce oluşturulmuş olan yeni ticaret tekliflerini ilk kez satın alan mevcut CSP müşterileri, bu satın almalar için iş ortağı konumu para birimi cinsinden faturalanacak. EU/EFTA ve Birleşik Krallık bölgesi dışında bulunan iş ortakları, iş ortağı konumu para birimiyle faturalandır olmaya devam edecektir.

- **İş ortağı teşvikleri:** Fatura ayı sonundan itibaren 45 gün boyunca ödeme.

## <a name="access-your-invoices-and-reconciliation-files"></a>Fatura ve mutabakat dosyalarınıza erişme

Bir fatura görüntülemeye hazır olduğunda, şirketinizin genel yöneticisi veya faturalama yöneticisi bir e-posta alır.

Fatura ve mutabakat dosyasına erişmek için:

1. İş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard/) oturum açın.

2. Fatura menüsünden İş Ortağı Merkezi'yi **seçin.**

3. Yinelenen ve Tek Sefer **sekmesini** **ve ilgilendiğinizi** para birimini seçin.

   :::image type="content" source="images/azure/billing3.png" alt-text="Fatura.":::

4. Fatura **veya Mutabakat** dosyasını **seçin.**  

   Geçmiş faturaları ve mutabakat dosyalarını görüntülemek için aşağıdaki Faturalama geçmişi satırına bakın.

## <a name="understanding-usage-data"></a>Kullanım verilerini anlama 

1. Azure planı, kullanım için kök veya üst düzey kapsayıcıdır. Tüm kullanımlar tek bir Azure planına geri bağlanır.

2. Bir plan içinde bir veya daha fazla Azure aboneliği olur. Bunlar kaynak yönetimi ve dağıtımı için kullanılan kapsayıcılardır. 

3. Bir abonelik içinde kaynak grupları, grup kaynaklarına ekler. Her kaynak bir kaynak grubuna dağıtılır. 

4. Kaynak örnekleri arasında sanal makineler ve depolama hesapları yer almaktadır. 

5. Kaynak yayma ölçümleri: Ölçümler, bir kaynağın tüketiminin ölçümleridir ve bir kaynak birden çok ölçüm için kullanım yayıyor olabilir. Metre bir ProductId, SKUId ve AvailabilityId ile tanımlanır. 

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

## <a name="read-the-invoice"></a>Faturayı okuma

1. Fatura her ayın sekizlik günü kadar kullanılamaz.

2. İş ortaklarının ödemelerini geri ödemesi için 60 günü olur.

3. Faturalama dönemi, 10/1-10/31 gibi bir takvim ayı kapsar.

4. Ücretler net ayarlamalardır (tutar net olarak "Yönetilen hizmetler için iş ortağı tarafından kazanılmış kredidir").

5. Ek faturalama ayrıntıları için fatura mutabakat dosyasını ve günlük olarak derecelendirilmiş kullanım dosyasını gözden geçirme.

   :::image type="content" source="images/azure/invoice1.png" alt-text="Fatura.":::

## <a name="read-the-invoice-reconciliation-file"></a>Fatura mutabakat dosyasını okuma

1. Her Azure planı ve ölçüm bileşimi, mutabakat dosyasında en fazla iki faturalama satırına sahip olabilir.

2. Ölçüm, takvim ayı boyunca tüm takvim ayı boyunca herhangi bir türde indirim veya krediye (katmanlı indirimler veya yönetilen hizmetler için İş ortağı tarafından kazanılan kredi gibi) uygunsa mutabakat dosyasında yalnızca bir faturalama satırı vardır. **PriceAdjusmentDescription sütunu indirime** veya kazanılan krediye başvurur.

3. İndirim veya iş ortağı tarafından kazanılan kredi için uygun olan belirli bir ölçüm için kaynak yoksa mutabakat dosyasında yalnızca bir faturalama satırı ve geçerli birim fiyat perakende fiyatı (birim fiyat) olur.

4. Ölçüm veya ölçümü yayan herhangi bir kaynak,  ayın bir parçası için yönetilen hizmetler için İş ortağı tarafından kazanılan kredi için uygunsa, mutabakat dosyasında iki faturalama satırı yer alacak. Bir satır ölçümün uygun olduğu günleri, ikinci satır ise ölçümün uygun olduğu günleri temsil edecek.

>[!NOTE]
>Azure tüketiminizi tek kullanımlık satın alma mutabakat dosyanıza uzlaştırabilirsiniz. Bunu yapmak için günlük olarak derecelendirilmiş kullanım mutabakat dosyanıza gidin ve SubscriptionID'nizi bulun. Bu, Azure plan kimliğinizle ilişkili tüm maliyetleri görüntüler. Azure SubscriptionID'niz EntitlementID olarak gösterilir.

## <a name="read-the-daily-usage-file"></a>Günlük kullanım dosyasını okuma

- Azure planı kapsamındaki abonelik sayaçları, günlük olarak derecelendirilmiş ve bir şekilde toplanıyor.

- **Yönetilen hizmetler için iş ortağı tarafından kazanılan** kredi, günlük olarak belirlenir ve uygulanır.

- Her abonelik ölçümde, tüketimin olduğu ayın her günü için bir satır vardır.

- Aşağıdaki örnekte:

  - **1-7/3** arasında yönetilen hizmetler için İş ortağı tarafından kazanılan kredi için uygun ölçüm (geçerli birim fiyatın perakende fiyatı, iş ortağı tarafından kazanılan krediden daha düşük olduğunu unutmayın.

  - Ölçüm, **7/4** - 7/7 arasında yönetilen hizmetler için İş ortağı tarafından kazanılan kredi için uygun değildi (geçerli birim fiyatın perakende fiyatı olduğunu unutmayın).

  - **7/8** - 7/31 arasında yönetilen hizmetler için İş ortağı tarafından kazanılan kredi için uygun ölçüm (geçerli birim fiyatın perakende fiyatı daha az iş ortağı tarafından kazanılan kredi olduğunu unutmayın).

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2.":::

## <a name="invoice-in-customer-currency"></a>Müşteri para birimi cinsinden fatura

Azure planı aracılığıyla azure hizmetleri ABD doları olarak fiyatlandırılıyor ve müşterinin ülke tarafından atanan para biriminde faturalandırılıyor. Faturalama para birimi USD olmayan bir değerse, kullanılan Döviz kuru (FX) oranı faturanın son sayfasında gösterilir. FX fiyatları aylık olarak belirlenir ve aşağıdaki faturaya uygulanır. Ülke para birimlerinin tam listesi için lütfen yeni ticari teklifler ülke kullanılabilirliği ve müşteri [para birimi matrisi'ne bakın.](https://go.microsoft.com/fwlink/?linkid=2112354)

Microsoft, her takvim ayı için satın alınan veya tüketilen Azure hizmetlerinin toplam ücretlerine varmak için temel USD fiyatlarına önceden belirlenen bir döviz kuru uygular. Aylık döviz kuru, Thomson Tümcesi (genellikle) tarafından önceki ay sonundan iki gün önce gmt'de saat 16:00'da yayımlanan orta fiyattır. 

**Örneğin,** Microsoft'un Aralık döviz kuru, verili bir para birimi için 29 Kasım'da veya yaklaşık olarak Thomson Mid-rate olur. Bu oran, 1 Aralık ile 31 Aralık arasında bu para birimiyle yapılan tüm satın almalara uygulanır. 

## <a name="azure-reservations"></a>Azure rezervasyonları


Bir [Azure planı aracılığıyla](azure-reservations.md) Azure rezervasyonları satın alırsanız, tek kullanımlık veya aylık faturalamayı seçebilirsiniz.


## <a name="azure-spending"></a>Azure harcaması

Mevcut Azure harcama deneyimi, azure'da yeni Azure planı faturalaması desteği İş Ortağı Merkezi. Bu, iş ortaklarının şunları sağlar:

- Müşteri düzeyinde ayarlanmış bütçe uyarılarını görüntüleme, yönetme ve alma 

- Azure planında toplam tahmini harcamayı görüntüleme (kaynağa ve ölçüm düzeyine göre)

Azure planı aracılığıyla Azure hizmetlerinin faturalama modeli ödeme sonrası tüketim olduğundan, beklenenden daha büyük bir faturayı önlemek için iş ortakları aylık bütçe uygulayabilir ve kullanım yüzdesini izleyebilir. Bütçe bir defada bir müşteriye veya birden çok müşteriye uygulanabilir. 

:::image type="content" source="images/azure/azurespend.png" alt-text="Azure harcaması.":::

## <a name="next-steps"></a>Sonraki adımlar

- İş ortağı tarafından kazanılan kredinin (PEC) nasıl hesaplanmasına bakın. İş Ortağı Merkezi [oturum](https://partner.microsoft.com/dashboard/) açın ve kullanılabilir fiyat listesini bulun.

- Azure planını [satın alma hakkında bilgi edinin](purchase-azure-plan.md)

- [CSP'de yeni ticaret deneyimi için fiyat listesine bakın](azure-plan-price-list.md)
