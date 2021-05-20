---
title: Azure plan faturalandırma-fatura & keşfi dosyaları
ms.topic: article
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure planına yönelik faturalandırma ile ilgili fatura ve mutabakat dosya yapısına erişme ve bunları anlama hakkında bilgi edinin.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 5ab086a4d15d16f094e33d19b81f1c93711916dc
ms.sourcegitcommit: e0444145d7720df948b9d02ae2469206db48dba5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110201434"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>CSP'de yeni ticari deneyim - Azure faturalama 

**Uygun roller**: yönetici Aracısı | Faturalandırma Yöneticisi | Genel yönetici

Bu makalede, Azure planına yönelik faturalandırma ile ilgili fatura ve mutabakat dosya yapısına nasıl erişebileceğiniz ve anlayabileceğiniz açıklanır. Azure planı altında faturalandırma, hizalanmış bir tek faturalandırma tarihi ve takvim ay tabanlı fatura dönemi kullanan Basitleştirilmiş bir faturalandırma deneyimidir.

## <a name="summary-of-billing-essentials"></a>Faturalandırma temelleri Özeti

- **Fatura tarihi**: fatura ve mutabakat dosyası, 8 (gece yarısı UTC) tarafından iş ortağı merkezi panosunda/API 'de kullanıma sunulacaktır.

- **Fatura fatura dönemi**: fatura fatura dönemi, takvim ayına hizalanır, örneğin, 10/1-10/31, 11/1-11/30.

- **Ücret Servisi dönemleri**: ücretler takvim ayına hizalanır. Örneğin, faturalandırılan iş ortağı 10/15 tarihinde bir Azure planı aracılığıyla Azure hizmetleri eklerse ve müşteri Azure hizmetleri 'ni 10/15 ' de kullanmaya başlarsa, faturalandırılan servis dönemi 10/15-10/31 olan müşteri tüketimi için, faturalanan iş ortağı, 11/8 tarihinde fatura/keşfi alır. 12/8 tarihinde oluşturulacak bir sonraki aya ait fatura, 11/1-11/31 servis dönemine yönelik tüm ücretleri içerir.

- **Fatura ödeme dönemi**: net 60 gün.

- **Fatura para birimi**: 15 Ocak 2021 tarihinden ıtıbaren, AB/EFTA ve Birleşik Krallık bölgesindeki iş ortakları, yeni müşteriler ve mevcut CSP müşterileri, kiracıların 11 Mayıs 2020 ' den önce oluşturulduğu ilk kez yeni ticaret teklifleri satın alarak, iş ortağı konumu para birimi 'nde satın alma işlemleri için faturalandırılır. AB/EFTA ve UK bölgesinin dışında bulunan iş ortakları, iş ortağı konumu para birimiyle faturalandırılmaya devam edecektir.

- **Partner teşvikleri**: fatura ayının sonundan itibaren ödenen 45 gün.

## <a name="access-your-invoices-and-reconciliation-files"></a>Faturanız ve mutabakat dosyalarınıza erişin

Bir fatura görüntülemeye hazırsanız şirketinizin genel yönetici veya faturalama yöneticisi bir e-posta alır.

Faturaya ve mutabakat dosyasına erişmek için:

1. İş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard/) oturum açın.

2. Fatura menüsünden İş Ortağı Merkezi'yi **seçin.**

3. Yinelenen ve Tek Sefer **sekmesini** **ve ilgilendiğinizi** para birimini seçin.

   :::image type="content" source="images/azure/billing3.png" alt-text="Fatura":::

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
            - Faturalandırma ölçümü yok

    - ResourceGroup 2
        - Sanal makine (kaynak)
            - Bilgisayar ölçer
        - Premium SSD yönetilen disk (kaynak)
            - Depolama kapasitesi ölçümü
            - Depolama işlemleri ölçümü

- Abonelik B-ResourceGroup 1-Azure SQL (kaynak)-DTU ölçer-VPN Gateway (kaynak)-VPN ağ geçidi ölçer

    - ResourceGroup 2
        - Sanal ağ arabirimi (kaynak)
            - Faturalandırma ölçümü yok

## <a name="read-the-invoice"></a>Faturayı okuyun

1. Fatura, her ayın sekizinci ' inden daha sonra kullanılabilir olacaktır.

2. İş ortaklarının ödemeye havale etmek için 60 gün vardır.

3. Fatura dönemi belirli bir takvim ayını kapsar. Örneğin, 10/1-10/31.

4. Ücretler, ayarlamaların miktarıdır ("hizmet için Iş ortağı kazanılmış kredinin yüzdesi").

5. Fatura keşfi dosyasını ve günlük derecelendirmeli kullanım dosyasını, ek faturalandırma ayrıntıları için gözden geçirin.

   :::image type="content" source="images/azure/invoice1.png" alt-text="faturalayabilirsiniz":::

## <a name="read-the-invoice-reconciliation-file"></a>Fatura mutabakat dosyasını okuma

1. Her Azure planı ve ölçüm bileşimi, mutabakat dosyasında en fazla iki faturalama satırına sahip olabilir.

2. Ölçüm, takvim ayı boyunca tüm takvim ayı boyunca herhangi bir türde indirim veya krediye (katmanlı indirimler veya yönetilen hizmetler için İş ortağı tarafından kazanılan kredi gibi) uygunsa mutabakat dosyasında yalnızca bir faturalama satırı vardır. **PriceAdjusmentDescription sütunu indirime** veya kazanılan krediye başvurur.

3. İndirim veya iş ortağı tarafından kazanılan kredi için uygun olan belirli bir ölçüm için kaynak yoksa mutabakat dosyasında yalnızca bir faturalama satırı yer alır ve geçerli birim fiyat perakende fiyatı (birim fiyattır) olur.

4. Ölçüm veya ölçümü yayan herhangi bir kaynak,  ayın bir parçası için yönetilen hizmetler için İş ortağı tarafından kazanılan kredi için uygunsa, mutabakat dosyasında iki faturalama satırı yer alacak. Bir satır ölçümün uygun olduğu günleri, ikinci satır ise ölçümün uygun olmadığının günlerini temsil edecek.

>[!NOTE]
>Azure tüketiminizi tek kullanımlık satın alma mutabakat dosyanıza uzlaştırabilirsiniz. Bunu yapmak için günlük olarak derecelendirilmiş kullanım mutabakat dosyanıza gidin ve SubscriptionID'nizi bulun. Bu, Azure Plan Kimliğiniz ile ilişkili tüm maliyetleri görüntüler. Azure SubscriptionID'niz EntitlementID olarak gösterilir.

## <a name="read-the-daily-usage-file"></a>Günlük kullanım dosyasını okuma

- Azure planı kapsamındaki abonelik sayaçları, günlük olarak derecelendirilmiş ve bir şekilde toplanıyor.

- **Yönetilen hizmetler için iş ortağı tarafından kazanılan** kredi, günlük olarak belirlenir ve uygulanır.

- Her abonelik ölçümde, tüketimin olduğu ayın her günü için bir satır vardır.

- Aşağıdaki örnekte:

  - **1-7/3** arasında yönetilen hizmetler için İş ortağı tarafından kazanılan kredi için uygun ölçüm (geçerli birim fiyatın perakende fiyatı, iş ortağı tarafından kazanılan krediden daha az olduğunu unutmayın.

  - Ölçüm, **7/4** - 7/7 arasında yönetilen hizmetler için İş ortağı tarafından kazanılan kredi için uygun değildi (geçerli birim fiyatın perakende fiyatı olduğunu unutmayın).

  - 7/8-7/31 ' dan **yönetilen hizmetler Için Iş ortağı kazanılmış kredi** için uygun ölçüm (geçerli birim fiyatı, perakende fiyatı daha az iş ortağı kazanılan kredidir).

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a>Müşteri para biriminde fatura

Azure planı aracılığıyla Azure Hizmetleri, ABD Doları cinsinden fiyatlandırılır ve müşterinin ülke atanmış para birimiyle faturalandırılır. Faturalama para birimi ABD dışı ise, kullanılan yabancı Exchange (FX) ücreti faturanın son sayfasında gösterilir. FX ücretleri aylık olarak belirlenir ve aşağıdaki faturaya uygulanır. Ülke para birimlerinin tam listesi için lütfen [Yeni ticaret teklifleri ülke kullanılabilirliği ve müşteri para birimi matrisini](https://go.microsoft.com/fwlink/?linkid=2112354)görüntüleyin.

Microsoft, dönüştürme için Londra hisse senedi alışverişini izler. Londra 'daki ayın son gününde yakalanan Döviz oranına eşit olan döviz ücretini kullanırız. Bu değer, ayın son günü olan günün son gününde yakalanan Döviz ücretini kullanır. FX ücretleri, uygulandıkları ayın ilk günü önce yenilenir ve kullanılabilir.

## <a name="azure-reservations"></a>Azure rezervasyonları


Azure [ayırmaları](azure-reservations.md) bir Azure planıyla satın alıyorsa, tek seferlik veya aylık faturalandırma seçeneklerinden birini belirleyebilirsiniz.


## <a name="azure-spending"></a>Azure harcaması

Mevcut Azure harcama deneyimi, Iş Ortağı Merkezi 'nde yeni Azure planı faturalandırmasını destekleyecek şekilde güncelleştirildi. Bu, iş ortaklarının şunları yapmasına olanak sağlar:

- Müşteri düzeyinde bütçe kümesi için uyarıları görüntüleyin, yönetin ve alın 

- Bir Azure planında toplam tahmini harcama (kaynak ve ölçüm düzeyine göre ayrılmış) görüntüleyin

Azure planı aracılığıyla Azure hizmetleri için faturalandırma modeli, daha büyük bir faturanız beklenenden daha büyük bir fatura olduğundan, iş ortakları aylık bir bütçe uygulayabilir ve kullanım yüzdesini izleyebilir. Bir bütçe, bir kerede bir müşteriye veya birden çok müşteriye uygulanabilir. 

:::image type="content" source="images/azure/azurespend.png" alt-text="Azure harcaması":::

## <a name="next-steps"></a>Sonraki adımlar

- Ortağın kazanılan kredisi (PEC) nasıl hesaplanacağını görün. Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard/) oturum açın ve kullanılabilir fiyat listesini bulun.

- [Azure planını satın alma](purchase-azure-plan.md) hakkında bilgi edinin

- [CSP'de yeni ticaret deneyimi için fiyat listesine bakın](azure-plan-price-list.md)
