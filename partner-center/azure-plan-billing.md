---
title: Azure plan faturalandırma-fatura & keşfi dosyaları
ms.topic: article
ms.date: 01/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure planına yönelik faturalandırma ile ilgili fatura ve mutabakat dosya yapısına erişme ve bunları anlama hakkında bilgi edinin.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 757383ee264e58e7b4dc8ffefafe213cb49acb79
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149800"
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

2. Iş Ortağı Merkezi menüsünde **faturalandırma**' i seçin.

3. **Yinelenen** ve **tek seferlik** ve ilgilendiğiniz para biriminin sekmesini seçin.

   :::image type="content" source="images/azure/billing3.png" alt-text="ödeme":::

4. **Fatura** veya **Mutabakat dosyası** seçin.  

   Geçmiş faturaları ve keşfi dosyalarını görüntülemek için, aşağıdaki faturalama geçmişi satırını genişletin.

## <a name="understanding-usage-data"></a>Kullanım verilerini anlama 

1. Azure planı, kullanım için kök veya üst düzey kapsayıcıdır. Tüm kullanımlar tek bir Azure planına geri bağlanır.

2. Bir plan içinde, bir veya daha fazla Azure aboneliği olacaktır. Bunlar, kaynak yönetimi ve dağıtımı için kullanılan kapsayıcılardır. 

3. Bir abonelik içinde, kaynak grupları grup kaynaklarına ekler. Her kaynak bir kaynak grubuna dağıtılır. 

4. Kaynak örnekleri, sanal makineler ve depolama hesapları içerir. 

5. Kaynak yayma ölçümleri: ölçümler, bir kaynağın tüketim ölçümleridir ve bir kaynak birden fazla ölçüm için kullanım yayabilir. Ölçümler, bir ProductID, SKUId ve kullanılabilirlik kimliği ile tanımlanır. 

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
        - Premium SSD yönetilen disk (kaynak)
            - Depolama kapasitesi ölçümü
            - Depolama işlemleri ölçümü

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

   :::image type="content" source="images/azure/invoice1.png" alt-text="Fatura":::

## <a name="read-the-invoice-reconciliation-file"></a>Fatura mutabakat dosyasını okuma

1. Her Azure planı ve ölçüm bileşimi, mutabakat dosyasında en fazla iki faturalama satırına sahip olabilir.

2. Ölçüm, takvim ayı boyunca tüm takvim ayı boyunca herhangi bir türde indirim veya krediye (katmanlı indirimler veya yönetilen hizmetler için İş ortağı tarafından kazanılan kredi gibi) uygunsa mutabakat dosyasında yalnızca bir faturalama satırı vardır. **PriceAdjusmentDescription sütunu indirime** veya kazanılan krediye başvurur.

3. İndirim veya iş ortağı tarafından kazanılan kredi için uygun olan belirli bir ölçüm için kaynak yoksa mutabakat dosyasında yalnızca bir faturalama satırı yer alır ve geçerli birim fiyat perakende fiyatı (birim fiyattır) olur.

4. Ölçüm veya ölçümü yayan herhangi bir kaynak,  ayın bir parçası için yönetilen hizmetler için İş ortağı tarafından kazanılan kredi için uygunsa, mutabakat dosyasında iki faturalama satırı yer alacak. Bir satır ölçümün uygun olduğu günleri, ikinci satır ise ölçümün uygun olmadığının günlerini temsil edecek.

## <a name="read-the-daily-usage-file"></a>Günlük kullanım dosyasını okuma

- Azure planı kapsamındaki abonelik sayaçları, günlük olarak derecelendirilmiş ve bir şekilde toplanıyor.

- **Yönetilen hizmetler için iş ortağı tarafından kazanılan** kredi, günlük olarak belirlenir ve uygulanır.

- Her abonelik ölçümde, tüketimin olduğu ayın her günü için bir satır vardır.

- Aşağıdaki örnekte:

  - **1-7/3** arasında yönetilen hizmetler için İş ortağı tarafından kazanılan kredi için uygun ölçüm (geçerli birim fiyatın perakende fiyatı, iş ortağı tarafından kazanılan krediden daha az olduğunu unutmayın.

  - Ölçüm, **7/4** - 7/7 arasında yönetilen hizmetler için İş ortağı tarafından kazanılan kredi için uygun değildi (geçerli birim fiyatın perakende fiyatı olduğunu unutmayın).

  - **7/8** - 7/31 arasında yönetilen hizmetler için İş ortağı tarafından kazanılan kredi için uygun ölçüm (geçerli birim fiyatın perakende fiyatı daha az iş ortağı tarafından kazanılan kredi olduğunu unutmayın).

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a>Müşteri para birimi cinsinden fatura

Azure planı aracılığıyla azure hizmetleri ABD doları olarak fiyatlandırılıyor ve müşterinin ülke tarafından atanan para birimi üzerinden faturalandırılıyor. Faturalama para birimi USD olmayan bir değerse, kullanılan Döviz kuru (FX) oranı faturanın son sayfasında gösterilir. FX fiyatları aylık olarak belirlenir ve aşağıdaki faturaya uygulanır. Ülke para birimlerinin tam listesi için lütfen yeni ticari teklifler ülke kullanılabilirliği ve müşteri [para birimi matrisi'ne bakın.](https://go.microsoft.com/fwlink/?linkid=2112354)

Microsoft, dönüştürme için Londra Borsa'yı takip ediyor. Londra Borsa'da ayın son iş gününde yakalanan döviz kuruna eşit olan döviz kurlarını kullanıyoruz. FX fiyatları, geçerli olduğu ayın ilk gününden önceki gün yenilenir ve kullanılabilir.

## <a name="azure-reservations"></a>Azure rezervasyonları


Bir [Azure planı aracılığıyla](azure-reservations.md) Azure rezervasyonları satın alırsanız, tek kullanımlık veya aylık faturalamayı seçebilirsiniz.


## <a name="azure-spending"></a>Azure harcaması

Mevcut Azure harcama deneyimi, azure'da yeni Azure planı faturalaması desteği İş Ortağı Merkezi. Bu, iş ortaklarının şunları sağlar:

- Müşteri düzeyinde ayarlanmış bütçe uyarılarını görüntüleme, yönetme ve alma 

- Azure planında toplam tahmini harcamayı görüntüleme (kaynağa ve ölçüm düzeyine göre aşağı doğru)

Azure planı aracılığıyla Azure hizmetlerinin faturalama modeli ödeme sonrası tüketim olduğundan, beklenenden daha büyük bir faturayı önlemek için iş ortakları aylık bütçe uygulayabilir ve kullanım yüzdesini izleyebilir. Bütçe bir defada bir müşteriye veya birden çok müşteriye uygulanabilir. 

:::image type="content" source="images/azure/azurespend.png" alt-text="Azure harcaması":::

## <a name="next-steps"></a>Sonraki adımlar

- İş ortağı tarafından kazanılan kredinin (PEC) nasıl hesaplanmasına bakın. İş Ortağı Merkezi [oturum](https://partner.microsoft.com/dashboard/) açın ve kullanılabilir fiyat listesini bulun.

- Azure planını [satın alma hakkında bilgi edinin](purchase-azure-plan.md)

- [CSP'de yeni ticaret deneyimi için fiyat listesine bakın](azure-plan-price-list.md)
