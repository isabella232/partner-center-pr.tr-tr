---
title: Maksimum rezervasyon kullanımı için Azure VM boyutlandırması
description: Bir sanal makineyi (VM) müşteriler için rezervasyon satın alan müşterilerin bilgi işlem ihtiyaçlarına göre Microsoft Azure öğrenin.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 650618de7460f4667c60ac58cbe6716530db7f16
ms.sourcegitcommit: b55f63a029d88c73cd5190bbac2df1b5990e6e44
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/08/2021
ms.locfileid: "113510202"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="1ae8f-103">Maksimum ayırma kullanımı için Microsoft Azure VM boyutlandırması</span><span class="sxs-lookup"><span data-stu-id="1ae8f-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="1ae8f-104">**Uygun roller:** Yönetici aracısı | Satış aracısı</span><span class="sxs-lookup"><span data-stu-id="1ae8f-104">**Appropriate roles**: Admin agent | Sales agent</span></span>

<span data-ttu-id="1ae8f-105">Bu makalede, bir sanal makineyi (VM) müşteriler için rezervasyon satın alan müşterilerin bilgi işlem ihtiyaçlarına Microsoft Azure açıklanmıştır.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-105">This article explains how to size a virtual machine (VM) to your customers' computing needs when you buy Microsoft Azure reservations for them.</span></span>
 
> [!NOTE]
> <span data-ttu-id="1ae8f-106">Bu makale yalnızca Bulut Çözümü Sağlayıcısı (CSP) programı iş ortakları için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-106">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="1ae8f-107">Diğer abonelik türlerini (kullansanız öde, bireysel, Microsoft Müşteri Sözleşmesi veya Kurumsal Anlaşma abonelikler gibi) kullanan müşterilerin bu Azure rezervasyonları belgelerini [okuması gerekir.](/azure/cost-management-billing/reservations)</span><span class="sxs-lookup"><span data-stu-id="1ae8f-107">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="1ae8f-108">Müşterinin Azure rezervasyonu için VM boyutunu belirleme</span><span class="sxs-lookup"><span data-stu-id="1ae8f-108">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="1ae8f-109">Müşterileriniz adına Microsoft Azure rezervasyon satın alırken, müşterinin işlem ihtiyaçlarını karşılamak için boyutlandırıldı bir sanal makine (VM) seçmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-109">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="1ae8f-110">Bu bilgileri şu yöntemlerden birini kullanarak bulabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="1ae8f-110">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="1ae8f-111">Azure kullanım API'si</span><span class="sxs-lookup"><span data-stu-id="1ae8f-111">Azure utilization API</span></span>
- <span data-ttu-id="1ae8f-112">Azure portal</span><span class="sxs-lookup"><span data-stu-id="1ae8f-112">The Azure portal</span></span>
- <span data-ttu-id="1ae8f-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="1ae8f-113">Azure PowerShell</span></span>
- <span data-ttu-id="1ae8f-114">Azure Resource Manager (ARM) API'si</span><span class="sxs-lookup"><span data-stu-id="1ae8f-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="1ae8f-115">Bu yöntemlerin her birini kullanmaya ilişkin yönergeler aşağıda verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="1ae8f-116">Rezervasyon satın aldıktan sonra rezervasyon indirimi, rezervasyonun öznitelikleriyle ve miktarıyla eşleşen sanal makinelere otomatik olarak uygulanır.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="1ae8f-117">Rezervasyonu bir VM'ye atamanız gerek değildir.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-117">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="1ae8f-118">Rezervasyon indirimleri klasik veya promosyon amaçlı VM'ler için geçerli değildir.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-118">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="1ae8f-119">Müşteriniz adına satın alacak VM'nin türünü ve boyutunu doğru şekilde tanımlamak için, VM serisi türü, müşteri mutabakat dosyalarında doğru şekilde görüntülenmezken aşağıda açıklanan yöntemlerden birini İş Ortağı Merkezi gerekir.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="1ae8f-120">Azure kullanım API'sini kullanarak VM boyutlandırma bilgilerini edinin</span><span class="sxs-lookup"><span data-stu-id="1ae8f-120">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="1ae8f-121">Satın alacak VM boyutunu belirlemek için API yanıtta additionalInfo'dan ServiceType özniteliği değerini kullanın.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="1ae8f-122">Daha fazla bilgi için [api'sinde Azure için müşterinin](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) kullanım kayıtlarını [İş Ortağı Merkezi bakın.](/partner-center/develop/)</span><span class="sxs-lookup"><span data-stu-id="1ae8f-122">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="1ae8f-123">Microsoft Azure portalını kullanarak VM boyutlandırma bilgilerini alma</span><span class="sxs-lookup"><span data-stu-id="1ae8f-123">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="1ae8f-124">Bu İş Ortağı Merkezi Müşteriler **sayfanıza** gidin.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-124">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="1ae8f-125">Azure VM rezervasyonlarını satın almak isteyen müşteriyi bulun ve ardından aşağı oku seçerek müşterinin bilgilerini genişletin.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="1ae8f-126">**Microsoft Azure Yönetim Portalı'yi** seçerek müşterinin kaydını Azure portal.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-126">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="1ae8f-127">Portal **menüsünden** Sanal makineler'i ve ardından rezervasyon satın almak istediğiniz VM'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="1ae8f-128">VM'nin ayrıntı sayfasında, aşağıda gösterildiği gibi boyut ve bölge bilgilerini bulun ve bu bilgileri kullanarak rezervasyonu İş Ortağı Merkezi.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-128">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="Ayrıntı sayfasında boyut ve bölge bilgileri.":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="1ae8f-130">Vm boyutlandırma bilgilerini Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="1ae8f-130">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="1ae8f-131">Rezervasyon satın almak istediğiniz VM'nin konumunu ve boyutunu almak için aşağıdaki görüntüde yer alan bilgileri kullanın.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-131">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="VM konumu ve boyutu.":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="1ae8f-133">Azure Resource Manager (ARM) API'sini kullanarak VM boyutlandırma bilgilerini edinin</span><span class="sxs-lookup"><span data-stu-id="1ae8f-133">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="1ae8f-134">ARMClient veya ARM API'lerini kullanarak, rezervasyon satın almak istediğiniz VM için ARM istemcisini arayın.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-134">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. `/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01`

3. <span data-ttu-id="1ae8f-135">Çağrı, aşağıda gösterildiği gibi **vmSize** ve **konum** değerlerini döndürür.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-135">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="vmSize değeri.":::
    :::image type="content" source="images/usage4.png" alt-text="konum değeri.":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="1ae8f-138">Azure VM kullanımını ve rezervasyon indirimi doğrulama</span><span class="sxs-lookup"><span data-stu-id="1ae8f-138">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="1ae8f-139">Müşteri adına bir Azure Ayrılmış VM Örneği satın aldığınız zaman, VM alanı için önceden ödemeye uygulanan indirim, müşterinin rezervasyon öznitelikleriyle ve miktarıyla eşan sanal makinelere otomatik olarak uygulanır.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-139">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="1ae8f-140">Aşağıdaki yöntemlerden birini kullanarak müşterinin rezervasyon kullanımını doğrular ve rezervasyon indirimlerinin hangi sanal makinelere uygulandığını kontrol edin:</span><span class="sxs-lookup"><span data-stu-id="1ae8f-140">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="1ae8f-141">Azure portal</span><span class="sxs-lookup"><span data-stu-id="1ae8f-141">The Azure portal</span></span>
- <span data-ttu-id="1ae8f-142">Azure kullanım API'si</span><span class="sxs-lookup"><span data-stu-id="1ae8f-142">Azure utilization API</span></span>

<span data-ttu-id="1ae8f-143">Bu yöntemlerin her birini kullanmaya ilişkin yönergeler aşağıda verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-143">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="1ae8f-144">Yalnızca Azure kullanım API'si indirimin uygulandığı sanal makineyi gösterir.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-144">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="1ae8f-145">Microsoft Azure portalında müşterinin rezervasyon kullanımını doğrulama</span><span class="sxs-lookup"><span data-stu-id="1ae8f-145">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="1ae8f-146">Bu İş Ortağı Merkezi Müşteriler **sayfanıza** gidin.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-146">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="1ae8f-147">Rezervasyon indirimi ve kullanımını doğrulamak istediğiniz müşteriyi bulun ve ardından aşağı oku seçerek müşterinin bilgilerini genişletin.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-147">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="1ae8f-148">**Microsoft Azure Yönetim Portalı'yi** seçerek müşterinin kaydını Azure portal.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-148">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="1ae8f-149">Portal **menüsünden** Rezervasyonlar'ı ve ardından kullanımı kontrol etmek istediğiniz rezervasyonu seçin.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-149">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="1ae8f-150">Genel **Bakış** sayfasında rezervasyonun sanal makinelere ne kadar uygulandığını gösteren rezervasyon kullanım grafiğini kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-150">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="1ae8f-151">Kullanım verileri 8 saate kadar geciktirebilir.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-151">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="1ae8f-152">a.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-152">a.</span></span> <span data-ttu-id="1ae8f-153">Rezervasyonun kullanımı %100 ise, müşteriniz rezervasyon satın alımının sağldırarak mümkün olan tüm tasarrufları elde edecektir.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-153">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="1ae8f-154">b.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-154">b.</span></span> <span data-ttu-id="1ae8f-155">Rezervasyonun kullanımı %0 ise indirim hiçbir sanal makineye uygulanmaz.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-155">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="1ae8f-156">c.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-156">c.</span></span> <span data-ttu-id="1ae8f-157">Rezervasyonun kullanımı %1 ile %99 arasında ise kullanılmayan avantajlar vardır.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-157">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="1ae8f-158">Bu durumdan kaçınmak için, satın alma işlemi öncesinde müşterinin bilgi işlem ihtiyaçlarını destekleyecek doğru boyutlu VM'yi belirleme.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-158">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="1ae8f-159">Azure kullanım API'si ile müşterinin rezervasyon kullanımını doğrulama</span><span class="sxs-lookup"><span data-stu-id="1ae8f-159">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="1ae8f-160">Yalnızca Azure kullanım API'si indirimin uygulandığı sanal makineyi gösterir.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-160">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="1ae8f-161">Müşterinin rezervasyon indirimi elde etmek ve indirimin uygulandığı VM'leri (sanal makineler) görmek için Azure kullanım API'si ile rezervasyon kullanım verilerini edinebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-161">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="1ae8f-162">Müşterinin rezervasyon kullanımını doğrulamayı görmek için Örnek A ile Örnek B'yi karşılaştırın.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-162">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Rezervasyon kullanım örnekleri.":::

- <span data-ttu-id="1ae8f-164">reservationId, indirimi VM'ye uygulamak için kullanılan Azure rezervasyonlarını tanımlar.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-164">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="1ae8f-165">consumptionMeter, rezervasyon indirimi uygulanmış vm'nin MeterId'dir.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-165">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="1ae8f-166">Rezervasyon indirimi uygulandığından ReservationMeter 0 ABD doları maliyet gösterir.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-166">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="1ae8f-167">Daha fazla bilgi için [api'sinde Azure için müşterinin](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) kullanım kayıtlarını [İş Ortağı Merkezi bakın.](/partner-center/develop/)</span><span class="sxs-lookup"><span data-stu-id="1ae8f-167">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="1ae8f-168">Microsoft Windows Server gibi yazılım maliyetleri şu anda VM rezervasyonu fiyatına dahil değildir ve sipariş kaydında ve faturada ayrı satır öğeleri olarak görünür.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-168">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="1ae8f-169">Ancak, bir müşterinin Azure Hibrit Kullanım Avantajı varsa yazılım maliyetleri uygulanmaz.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-169">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="1ae8f-170">Daha fazla bilgi için [bkz. Windows ayrılmış örneklerde yer alan yazılım maliyetleri.](/azure/billing/billing-reserved-instance-windows-software-costs)</span><span class="sxs-lookup"><span data-stu-id="1ae8f-170">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="next-steps"></a><span data-ttu-id="1ae8f-171">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="1ae8f-171">Next steps</span></span>

|<span data-ttu-id="1ae8f-172">**Hakkında bilgi için**</span><span class="sxs-lookup"><span data-stu-id="1ae8f-172">**For information about**</span></span>   |<span data-ttu-id="1ae8f-173">**Bunu okuyun**</span><span class="sxs-lookup"><span data-stu-id="1ae8f-173">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="1ae8f-174">CSP'de Azure rezervasyonları genel bakış</span><span class="sxs-lookup"><span data-stu-id="1ae8f-174">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="1ae8f-175">Ayrılmış Microsoft Azure Örnekleri satma</span><span class="sxs-lookup"><span data-stu-id="1ae8f-175">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="1ae8f-176">İş Ortağı Merkezi'de müşterileriniz için Azure rezervasyonları satın İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="1ae8f-176">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="1ae8f-177">Azure rezervasyonları satın alma</span><span class="sxs-lookup"><span data-stu-id="1ae8f-177">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="1ae8f-178">Azure rezervasyonlarını İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="1ae8f-178">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="1ae8f-179">Azure rezervasyonlarını İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="1ae8f-179">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="1ae8f-180">Azure rezervasyonlarını Azure portal</span><span class="sxs-lookup"><span data-stu-id="1ae8f-180">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="1ae8f-181">[Azure Yardımı'Azure Ayrılmış VM Örnekleri sanal makineler](/azure/virtual-machines/windows/prepay-reserved-vm-instances) için ön ödeme</span><span class="sxs-lookup"><span data-stu-id="1ae8f-181">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="1ae8f-182">Azure rezervasyonlarını Azure portal</span><span class="sxs-lookup"><span data-stu-id="1ae8f-182">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="1ae8f-183">Azure [Yardım'da ayrılmış VM](/azure/billing/billing-manage-reserved-vm-instance) örneklerini yönetme</span><span class="sxs-lookup"><span data-stu-id="1ae8f-183">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="1ae8f-184">İş Ortağı Merkezi API'sini kullanarak Azure rezervasyonları satın alma</span><span class="sxs-lookup"><span data-stu-id="1ae8f-184">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="1ae8f-185">[Geliştirici Azure Ayrılmış VM Örnekleri](/partner-center/develop/purchase-azure-reservations) belgelerinde İş Ortağı Merkezi satın alma</span><span class="sxs-lookup"><span data-stu-id="1ae8f-185">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="1ae8f-186">Müşterilere, satın aldığınız abonelikten kendi Azure rezervasyonlarını satın alma izni verme.</span><span class="sxs-lookup"><span data-stu-id="1ae8f-186">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="1ae8f-187">Müşterilere kendi Azure rezervasyonlarını satın alma izni verme</span><span class="sxs-lookup"><span data-stu-id="1ae8f-187">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |