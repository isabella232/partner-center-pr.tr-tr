---
title: Maksimum rezervasyon kullanımı için Azure VM boyutlandırması
description: bir sanal makineyi (VM), müşteriler için Microsoft Azure ayırmaları satın aldığınızda müşterilerinizin bilgi işlem ihtiyaçlarına göre nasıl boyutlandırdığını öğrenin.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: dc9b9100e01191c24c03c76e9a9ff5a6ffe335d1
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123959985"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Maksimum ayırma kullanımı için Microsoft Azure VM boyutlandırması

**Uygun roller**: yönetici Aracısı | Satış Aracısı

bu makalede, bir sanal makinenin (VM) müşterilere bilgi işlem gereksinimlerine göre nasıl boyutlandırılacağını ve bunlara yönelik Microsoft Azure ayırmaları satın almanız açıklanmaktadır.
 
> [!NOTE]
> bu makale yalnızca Bulut Çözümü Sağlayıcısı (CSP) programındaki iş ortakları için geçerlidir. diğer abonelik türleri (örneğin, kullandıkça öde, bireysel, Microsoft müşteri sözleşmesi veya Kurumsal Anlaşma abonelikleri) kullanan müşteriler [bu Azure ayırmaları belgelerini](/azure/cost-management-billing/reservations)okumalı olmalıdır.

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Müşterinin Azure ayırması için VM boyutunu belirleme

müşterileriniz adına Microsoft Azure ayırmaları satın alırken müşterinin bilgi işlem ihtiyaçlarını karşılamak için boyutlandırılmış bir sanal makine (VM) seçmeniz gerekir. Aşağıdaki yöntemlerden birini kullanarak bu bilgileri bulabilirsiniz:

- Azure kullanım API 'SI
- Azure portal
- Azure PowerShell
- Azure Resource Manager (ARM) API 'SI

Bu yöntemlerin her birini kullanmaya yönelik yönergeler aşağıda verilmiştir. Bir rezervasyon satın aldıktan sonra, rezervasyon iskontosu, rezervasyonun öznitelikleriyle ve miktarıyla eşleşen sanal makinelere otomatik olarak uygulanır. Ayırmayı bir VM 'ye atamanız gerekmez.

>[!NOTE]
>Rezervasyon iskontoları, klasik veya promosyon VM 'lerine uygulanmaz.

>[!IMPORTANT]
>Müşterinizin adına satın alacağınız VM 'nin türünü ve boyutunu doğru şekilde belirlemek için, VM Serisi türü Iş Ortağı Merkezi mutabakatı dosyalarında doğru görüntülenmediğinden aşağıda açıklanan yöntemlerden birini kullanmanız gerekir.

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a>Azure kullanım API 'sini kullanarak VM boyutlandırma bilgilerini alın

1. Satın alınan VM boyutunu belirlemek için API yanıtında AdditionalInfo öğesinden ServiceType özniteliği için değeri kullanın.

2. Daha fazla bilgi için bkz. [Iş ortağı MERKEZI API](/partner-center/develop/)'de [Azure için bir müşterinin kullanım kayıtlarını edinme](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) .

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a>Microsoft Azure portalını kullanarak VM boyutlandırma bilgilerini al

1. Iş Ortağı Merkezi 'nde **müşteriler** sayfanıza gidin.

2. Azure VM ayırmaları satın almak isteyen müşteriyi bulun ve ardından müşterinin bilgilerini genişletmek için aşağı oku seçin. müşterinin kaydını Azure portal açmak için **Microsoft Azure Yönetim Portalı** seçin.

3. Portal menüsünden **sanal makineler** ' i seçin ve ardından bir ayırma satın almak istediğiniz VM 'yi seçin.

4. VM 'nin ayrıntı sayfasında, aşağıda gösterildiği gibi boyut ve bölge bilgilerini bulun ve bu bilgileri Iş Ortağı Merkezi 'nde ayırmayı satın almak için kullanın.  

   :::image type="content" source="images/usage1.png" alt-text="Ayrıntı sayfasında boyut ve bölge bilgileri.":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a>Microsoft Azure PowerShell kullanarak VM boyutlandırma bilgilerini al

Bir ayırma satın almak istediğiniz VM 'nin konumunu ve boyutunu almak için aşağıdaki görüntüdeki bilgileri kullanın. 

:::image type="content" source="images/usage2.png" alt-text="VM konumu ve boyutu.":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a>Azure Resource Manager (ARM) API 'sini kullanarak VM boyutlandırma bilgilerini al

1. ARMClient veya ARM API 'Lerini kullanarak, bir ayırma satın almak istediğiniz VM için ARM istemcisini çağırın.

2. `/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01`

3. Çağrı, aşağıda gösterildiği gibi **VMSize** ve **konuma** ait değerleri döndürür.

    :::image type="content" source="images/usage3.png" alt-text="vmSize değeri.":::
    :::image type="content" source="images/usage4.png" alt-text="konum değeri.":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Azure VM kullanımını ve rezervasyon iskontosunu doğrulama

Bir müşteri adına bir Azure ayrılmış VM örneği satın aldıktan sonra, önce VM alanı için ödeme indirimi, müşteri rezervasyonunun öznitelikleriyle ve miktarıyla eşleşen sanal makinelere otomatik olarak uygulanır.

Aşağıdaki yöntemlerden birini kullanarak, müşterinin rezervasyon kullanımını doğrulayabilirsiniz ve rezervasyon iskontolarının hangi sanal makineleri uygulanacağını görebilirsiniz:

- Azure portal
- Azure kullanım API 'SI

Bu yöntemlerin her birini kullanmaya yönelik yönergeler aşağıda verilmiştir.

>[!NOTE]
>Yalnızca Azure kullanım API 'SI, iskontonun hangi sanal makinede uygulanacağını gösterir.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Microsoft Azure portalında müşterinin rezervasyon kullanımını doğrulama

1. Iş Ortağı Merkezi 'nde **müşteriler** sayfanıza gidin.

2. Rezervasyon indirimi ve kullanımını doğrulamak istediğiniz müşteriyi bulun ve ardından müşterinin bilgilerini genişletmek için aşağı oku seçin. müşterinin kaydını Azure portal açmak için **Microsoft Azure Yönetim Portalı** seçin.
3. Portal menüsünden **ayırmalar** ' ı seçin ve ardından kullanımı denetlemek istediğiniz ayırmayı seçin.
4. **Genel bakış** sayfasında, rezervasyonun sanal makinelere ne kadarının uygulandığını gösteren kullanım grafiğini kontrol edin.

    >[!NOTE]
    >Kullanım verileri 8 saate kadar gecikebilir.

    a. Rezervasyonun kullanımı %100 ise, müşteriniz, rezervasyon satın alma işlemi tarafından sağlanacak tüm olası tasarrufları elde edebilir.
    b. Rezervasyonun kullanımı %0 ise, indirim herhangi bir sanal makineye uygulanmaz.
    c. Rezervasyonun kullanımı %1 ile %99 arasındaysa, kullanılmayan avantajlar vardır.

5. Bu durumdan kaçınmak için, satın almayı yapmadan önce müşterinin bilgi işlem ihtiyaçlarını desteklemek üzere doğru boyut sanal makinesini saptayın.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Azure kullanım API 'SI ile müşterinin rezervasyon kullanımını doğrulama

>[!NOTE]
>Yalnızca Azure kullanım API 'SI, iskontonun hangi sanal makinede uygulanacağını gösterir.  

Müşterinin rezervasyon iskontosunu aldığını doğrulamak ve iskontonun hangi VM 'Ler (sanal makineler) uygulanacağını öğrenmek için Azure kullanım API 'SI ile rezervasyon kullanım verilerini alabilirsiniz. Müşterinin ayırma kullanımını nasıl doğrulayabildiğini öğrenmek için örneğin, örnek B ile karşılaştırın.

:::image type="content" source="images/usage5.png" alt-text="Ayırma kullanım örnekleri.":::

- Rezervkimliği, iskontoyu VM 'ye uygulamak için kullanılan Azure ayırmasını tanımlar.
- Tüketiytionmetre, rezervasyon iskontosunun uygulandığı VM için ölçüm kimliği.
- Ayırma indirimi uygulandıktan sonra rezervde $0 maliyeti gösterilmektedir.

Daha fazla bilgi için bkz. [Iş ortağı MERKEZI API](/partner-center/develop/)'de [Azure için bir müşterinin kullanım kayıtlarını edinme](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) .

>[!IMPORTANT]
>Microsoft Windows Server gibi yazılım maliyetleri, şu anda bir VM ayırma fiyatına dahil edilmez ve sipariş kaydında ve faturanızda ayrı satır öğeleri olarak görünür. Ancak, bir müşterinin Azure hibrit kullanım teklifi varsa, yazılım maliyetleri uygulanmaz. daha fazla bilgi için bkz. [Windows yazılım maliyetleri ayrılmış örneklere dahil değildir](/azure/billing/billing-reserved-instance-windows-software-costs).  

## <a name="next-steps"></a>Sonraki adımlar

|**Hakkında bilgi için**   |**Bunu okuyun**    |
|:-----------------------------|:-----------------|
|CSP 'de Azure ayırmaları genel bakış  | [ayrılmış Microsoft Azure VM örnekleri satma](azure-reservations.md)
|Iş Ortağı Merkezi 'nde müşterileriniz için Azure ayırmaları satın alma   | [Azure ayırmaları satın alma](azure-reservations-buying.md)
|Azure ayırmalarını Iş Ortağı Merkezi 'nde yönetme | [Azure ayırmalarını Iş Ortağı Merkezi 'nde yönetme](azure-reservations-manage.md)
|Azure portal Azure ayırmaları satın alma | Azure yardım 'da [Azure ayrılmış VM örnekleri ile sanal makineler Için ön ödeme](/azure/virtual-machines/windows/prepay-reserved-vm-instances) yapın |
|Azure portal Azure ayırmalarını yönetme   | Azure yardımında [ayrılmış VM örneklerini yönetme](/azure/billing/billing-manage-reserved-vm-instance)  |
|Iş Ortağı Merkezi API 'sini kullanarak Azure ayırmaları satın alma | [Azure ayrılmış VM örneklerini](/partner-center/develop/purchase-azure-reservations) Iş Ortağı Merkezi geliştirici belgelerinde satın alma   |
|Müşterilere satın almış olduğunuz bir abonelikten kendi Azure ayırmalarını satın alma izni verme. | [Müşterilere kendi Azure ayırmalarını satın alma izni verin](give-customers-permission.md)   |