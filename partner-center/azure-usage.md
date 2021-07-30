---
title: Maksimum rezervasyon kullanımı için Azure VM boyutlandırması
description: Bir sanal makineyi (VM) müşteriler için rezervasyon satın alan müşterilerin bilgi işlem ihtiyaçlarına göre Microsoft Azure öğrenin.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: dc9b9100e01191c24c03c76e9a9ff5a6ffe335d1
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114842193"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Maksimum ayırma kullanımı için Microsoft Azure VM boyutlandırması

**Uygun roller:** Yönetici aracısı | Satış aracısı

Bu makalede, bir sanal makineyi (VM) müşteriler için rezervasyon satın alan müşterilerin bilgi işlem ihtiyaçlarına Microsoft Azure açıklanmıştır.
 
> [!NOTE]
> Bu makale yalnızca Bulut Çözümü Sağlayıcısı (CSP) programı iş ortakları için geçerlidir. Diğer abonelik türlerini (kullansanız öde, bireysel, Microsoft Müşteri Sözleşmesi veya Kurumsal Anlaşma abonelikler gibi) kullanan müşterilerin bu Azure rezervasyonları belgelerini [okuması gerekir.](/azure/cost-management-billing/reservations)

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Müşterinin Azure rezervasyonu için VM boyutunu belirleme

Müşterileriniz adına Microsoft Azure rezervasyon satın alırken, müşterinin işlem ihtiyaçlarını karşılamak için boyutlandırıldı bir sanal makine (VM) seçmeniz gerekir. Bu bilgileri şu yöntemlerden birini kullanarak bulabilirsiniz:

- Azure kullanım API'si
- Azure portal
- Azure PowerShell
- Azure Resource Manager (ARM) API'si

Bu yöntemlerin her birini kullanmaya ilişkin yönergeler aşağıda verilmiştir. Rezervasyon satın aldıktan sonra rezervasyon indirimi, rezervasyonun öznitelikleriyle ve miktarıyla eşleşen sanal makinelere otomatik olarak uygulanır. Rezervasyonu bir VM'ye atamanız gerek değildir.

>[!NOTE]
>Rezervasyon indirimleri klasik veya promosyon amaçlı VM'ler için geçerli değildir.

>[!IMPORTANT]
>Müşteriniz adına satın alacak VM'nin türünü ve boyutunu doğru şekilde tanımlamak için, VM serisi türü, müşteri mutabakat dosyalarında doğru şekilde görüntülenmezken aşağıda açıklanan yöntemlerden birini İş Ortağı Merkezi gerekir.

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a>Azure kullanım API'sini kullanarak VM boyutlandırma bilgilerini edinin

1. Satın alacak VM boyutunu belirlemek için API yanıtta additionalInfo'dan ServiceType özniteliği değerini kullanın.

2. Daha fazla bilgi için [api'sinde Azure için müşterinin](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) kullanım kayıtlarını [İş Ortağı Merkezi bakın.](/partner-center/develop/)

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a>Microsoft Azure portalını kullanarak VM boyutlandırma bilgilerini alma

1. Bu İş Ortağı Merkezi Müşteriler **sayfanıza** gidin.

2. Azure VM rezervasyonlarını satın almak isteyen müşteriyi bulun ve ardından aşağı oku seçerek müşterinin bilgilerini genişletin. **Microsoft Azure Yönetim Portalı'yi** seçerek müşterinin kaydını Azure portal.

3. Portal **menüsünden** Sanal makineler'i ve ardından rezervasyon satın almak istediğiniz VM'yi seçin.

4. VM'nin ayrıntı sayfasında, aşağıda gösterildiği gibi boyut ve bölge bilgilerini bulun ve bu bilgileri kullanarak rezervasyonu İş Ortağı Merkezi.  

   :::image type="content" source="images/usage1.png" alt-text="Ayrıntı sayfasında boyut ve bölge bilgileri.":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a>Vm boyutlandırma bilgilerini Microsoft Azure PowerShell

Rezervasyon satın almak istediğiniz VM'nin konumunu ve boyutunu almak için aşağıdaki görüntüde yer alan bilgileri kullanın. 

:::image type="content" source="images/usage2.png" alt-text="VM konumu ve boyutu.":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a>Azure Resource Manager (ARM) API'sini kullanarak VM boyutlandırma bilgilerini edinin

1. ARMClient veya ARM API'lerini kullanarak, rezervasyon satın almak istediğiniz VM için ARM istemcisini arayın.

2. `/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01`

3. Çağrı, aşağıda gösterildiği gibi **vmSize** ve **konum** değerlerini döndürür.

    :::image type="content" source="images/usage3.png" alt-text="vmSize değeri.":::
    :::image type="content" source="images/usage4.png" alt-text="konum değeri.":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Azure VM kullanımını ve rezervasyon indirimi doğrulama

Müşteri adına bir Azure Ayrılmış VM Örneği satın aldıktan sonra, VM alanı için önceden ödemeye uygulanan indirim, müşterinin rezervasyon öznitelikleriyle ve miktarıyla eşan sanal makinelere otomatik olarak uygulanır.

Müşterinin rezervasyon kullanımını doğrular ve aşağıdaki yöntemlerden birini kullanarak rezervasyon indirimlerinin hangi sanal makinelere uygulandığını kontrol edin:

- Azure portal
- Azure kullanım API'si

Bu yöntemlerin her birini kullanmaya ilişkin yönergeler aşağıda verilmiştir.

>[!NOTE]
>Yalnızca Azure kullanım API'si indirimin uygulandığı sanal makineyi gösterir.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Microsoft Azure portalında müşterinin rezervasyon kullanımını doğrulama

1. Bu İş Ortağı Merkezi Müşteriler **sayfanıza** gidin.

2. Rezervasyon indirimi ve kullanımını doğrulamak istediğiniz müşteriyi bulun ve ardından aşağı oku seçerek müşterinin bilgilerini genişletin. **Microsoft Azure Yönetim Portalı'yi** seçerek müşterinin kaydını Azure portal.
3. Portal **menüsünden** Rezervasyonlar'ı ve ardından kullanımı kontrol etmek istediğiniz rezervasyonu seçin.
4. Genel **Bakış** sayfasında rezervasyonun sanal makinelere ne kadar uygulandığını gösteren rezervasyon kullanım grafiğini kontrol edin.

    >[!NOTE]
    >Kullanım verileri 8 saate kadar geciktirebilir.

    a. Rezervasyonun kullanımı %100 ise, müşteriniz rezervasyon satın alımının sağldırarak mümkün olan tüm tasarrufları elde edecektir.
    b. Rezervasyonun kullanımı %0 ise indirim hiçbir sanal makineye uygulanmaz.
    c. Rezervasyonun kullanımı %1 ile %99 arasında ise kullanılmayan avantajlar vardır.

5. Bu durumdan kaçınmak için, satın alma işlemi öncesinde müşterinin bilgi işlem ihtiyaçlarını destekleyecek doğru boyutlu VM'yi belirleme.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Azure kullanım API'si ile müşterinin rezervasyon kullanımını doğrulama

>[!NOTE]
>Yalnızca Azure kullanım API'si indirimin uygulandığı sanal makineyi gösterir.  

Müşterinin rezervasyon indirimi elde etmek ve indirimin uygulandığı VM'leri (sanal makineler) görmek için Azure kullanım API'si ile rezervasyon kullanım verilerini edinebilirsiniz. Müşterinin rezervasyon kullanımını doğrulamayı görmek için Örnek A ile Örnek B'yi karşılaştırın.

:::image type="content" source="images/usage5.png" alt-text="Rezervasyon kullanım örnekleri.":::

- reservationId, indirimi VM'ye uygulamak için kullanılan Azure rezervasyonlarını tanımlar.
- consumptionMeter, rezervasyon indirimi uygulanmış vm'nin MeterId'dir.
- Rezervasyon indirimi uygulandığından ReservationMeter 0 ABD doları maliyet gösterir.

Daha fazla bilgi için [api'sinde Azure için müşterinin](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) kullanım kayıtlarını [İş Ortağı Merkezi bakın.](/partner-center/develop/)

>[!IMPORTANT]
>Microsoft Windows Server gibi yazılım maliyetleri şu anda VM rezervasyonu fiyatına dahil değildir ve sipariş kaydında ve faturada ayrı satır öğeleri olarak görünür. Ancak, bir müşterinin Azure Hibrit Kullanım Avantajı varsa yazılım maliyetleri uygulanmaz. Daha fazla bilgi için [bkz. Windows ayrılmış örneklerde yer alan yazılım maliyetleri.](/azure/billing/billing-reserved-instance-windows-software-costs)  

## <a name="next-steps"></a>Sonraki adımlar

|**Hakkında bilgi için**   |**Bunu okuyun**    |
|:-----------------------------|:-----------------|
|CSP'de Azure rezervasyonları genel bakış  | [Ayrılmış Microsoft Azure Örnekleri satma](azure-reservations.md)
|İş Ortağı Merkezi'de müşterileriniz için Azure rezervasyonları satın İş Ortağı Merkezi   | [Azure rezervasyonları satın alma](azure-reservations-buying.md)
|Azure rezervasyonlarını İş Ortağı Merkezi | [Azure rezervasyonlarını İş Ortağı Merkezi](azure-reservations-manage.md)
|Azure rezervasyonlarını Azure portal | [Azure Yardımı'Azure Ayrılmış VM Örnekleri sanal makineler](/azure/virtual-machines/windows/prepay-reserved-vm-instances) için ön ödeme |
|Azure rezervasyonlarını Azure portal   | Azure [Yardım'da ayrılmış VM](/azure/billing/billing-manage-reserved-vm-instance) örneklerini yönetme  |
|İş Ortağı Merkezi API'sini kullanarak Azure rezervasyonları satın alma | [Geliştirici Azure Ayrılmış VM Örnekleri](/partner-center/develop/purchase-azure-reservations) belgelerinde İş Ortağı Merkezi satın alma   |
|Müşterilere, satın aldığınız abonelikten kendi Azure rezervasyonlarını satın alma izni verme. | [Müşterilere kendi Azure rezervasyonlarını satın alma izni verme](give-customers-permission.md)   |