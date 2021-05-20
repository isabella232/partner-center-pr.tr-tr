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
ms.openlocfilehash: 14d488091227e30909b3d41af0684494a8b55de7
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149460"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="e348e-103">Maksimum ayırma kullanımı için Microsoft Azure VM boyutlandırması</span><span class="sxs-lookup"><span data-stu-id="e348e-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="e348e-104">**Uygun roller:** Yönetici aracısı | Satış aracısı</span><span class="sxs-lookup"><span data-stu-id="e348e-104">**Appropriate roles**: Admin agent | Sales agent</span></span>

<span data-ttu-id="e348e-105">Bu makalede, bir sanal makineyi (VM) müşteriler için rezervasyon satın alan müşterilerin bilgi işlem ihtiyaçlarına Microsoft Azure açıklanmıştır.</span><span class="sxs-lookup"><span data-stu-id="e348e-105">This article explains how to size a virtual machine (VM) to your customers' computing needs when you buy Microsoft Azure reservations for them.</span></span>
 
> [!NOTE]
> <span data-ttu-id="e348e-106">Bu makale yalnızca Bulut Çözümü Sağlayıcısı (CSP) programı iş ortakları için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="e348e-106">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="e348e-107">Diğer abonelik türlerini (kullansanız öde, bireysel, Microsoft Müşteri Sözleşmesi veya Kurumsal Anlaşma abonelikler gibi) kullanan müşterilerin bu Azure rezervasyonları belgelerini [okuması gerekir.](/azure/cost-management-billing/reservations)</span><span class="sxs-lookup"><span data-stu-id="e348e-107">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="e348e-108">Müşterinin Azure rezervasyonu için VM boyutunu belirleme</span><span class="sxs-lookup"><span data-stu-id="e348e-108">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="e348e-109">Müşterileriniz adına Microsoft Azure rezervasyon satın alırken, müşterinin bilgi işlem ihtiyaçlarını karşılamak için boyutlandırıldı bir sanal makine (VM) seçmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="e348e-109">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="e348e-110">Bu bilgileri şu yöntemlerden birini kullanarak bulabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="e348e-110">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="e348e-111">Azure kullanım API'si</span><span class="sxs-lookup"><span data-stu-id="e348e-111">Azure utilization API</span></span>
- <span data-ttu-id="e348e-112">Azure portal</span><span class="sxs-lookup"><span data-stu-id="e348e-112">The Azure portal</span></span>
- <span data-ttu-id="e348e-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="e348e-113">Azure PowerShell</span></span>
- <span data-ttu-id="e348e-114">Azure Resource Manager (ARM) API'si</span><span class="sxs-lookup"><span data-stu-id="e348e-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="e348e-115">Bu yöntemlerin her birini kullanmaya ilişkin yönergeler aşağıda verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="e348e-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="e348e-116">Rezervasyon satın aldıktan sonra rezervasyon indirimi, rezervasyonun öznitelikleriyle ve miktarıyla eşleşen sanal makinelere otomatik olarak uygulanır.</span><span class="sxs-lookup"><span data-stu-id="e348e-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="e348e-117">Rezervasyonu bir VM'ye atamanız gerek değildir.</span><span class="sxs-lookup"><span data-stu-id="e348e-117">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="e348e-118">Rezervasyon indirimleri klasik veya promosyon amaçlı VM'ler için geçerli değildir.</span><span class="sxs-lookup"><span data-stu-id="e348e-118">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="e348e-119">Müşteriniz adına satın alacak VM'nin türünü ve boyutunu doğru şekilde tanımlamak için, VM serisi türü, müşteri mutabakat dosyalarında doğru şekilde görüntülenmezken aşağıda açıklanan yöntemlerden birini İş Ortağı Merkezi gerekir.</span><span class="sxs-lookup"><span data-stu-id="e348e-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="e348e-120">Azure kullanım API'sini kullanarak VM boyutlandırma bilgilerini edinin</span><span class="sxs-lookup"><span data-stu-id="e348e-120">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="e348e-121">Satın alacak VM boyutunu belirlemek için API yanıtta additionalInfo'dan ServiceType özniteliği değerini kullanın.</span><span class="sxs-lookup"><span data-stu-id="e348e-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="e348e-122">Daha fazla bilgi için [api'sinde Azure için müşterinin](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) kullanım kayıtlarını [İş Ortağı Merkezi bakın.](/partner-center/develop/)</span><span class="sxs-lookup"><span data-stu-id="e348e-122">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="e348e-123">Sanal makineyi kullanarak VM boyutlandırma bilgilerini Microsoft Azure portal</span><span class="sxs-lookup"><span data-stu-id="e348e-123">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="e348e-124">Bu İş Ortağı Merkezi Müşteriler **sayfanıza** gidin.</span><span class="sxs-lookup"><span data-stu-id="e348e-124">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="e348e-125">Azure VM ayırmaları satın almak isteyen müşteriyi bulun ve ardından müşterinin bilgilerini genişletmek için aşağı oku seçin.</span><span class="sxs-lookup"><span data-stu-id="e348e-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="e348e-126">**Microsoft Azure yönetim portalı** ' yi seçerek müşterinin kaydını Azure Portal açın.</span><span class="sxs-lookup"><span data-stu-id="e348e-126">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="e348e-127">Portal menüsünden **sanal makineler** ' i seçin ve ardından bir ayırma satın almak istediğiniz VM 'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="e348e-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="e348e-128">VM 'nin ayrıntı sayfasında, aşağıda gösterildiği gibi boyut ve bölge bilgilerini bulun ve bu bilgileri Iş Ortağı Merkezi 'nde ayırmayı satın almak için kullanın.</span><span class="sxs-lookup"><span data-stu-id="e348e-128">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="Ayrıntı sayfasında boyut ve bölge bilgileri":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="e348e-130">Microsoft Azure PowerShell kullanarak VM boyutlandırma bilgilerini al</span><span class="sxs-lookup"><span data-stu-id="e348e-130">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="e348e-131">Bir ayırma satın almak istediğiniz VM 'nin konumunu ve boyutunu almak için aşağıdaki görüntüdeki bilgileri kullanın.</span><span class="sxs-lookup"><span data-stu-id="e348e-131">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="VM konumu ve boyutu":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="e348e-133">Azure Resource Manager (ARM) API 'sini kullanarak VM boyutlandırma bilgilerini al</span><span class="sxs-lookup"><span data-stu-id="e348e-133">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="e348e-134">ARMClient veya ARM API 'Lerini kullanarak, bir ayırma satın almak istediğiniz VM için ARM istemcisini çağırın.</span><span class="sxs-lookup"><span data-stu-id="e348e-134">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="e348e-135">/Subscriptions/ <Subscription ID> /ResourceGroups/ <Resource group name> /providers/Microsoft.COMPUTE/virtualMachines/ <VM Instance Name> ? api-Version = 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="e348e-135">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="e348e-136">Çağrı, aşağıda gösterildiği gibi **VMSize** ve **konuma** ait değerleri döndürür.</span><span class="sxs-lookup"><span data-stu-id="e348e-136">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="vmSize değeri":::
    :::image type="content" source="images/usage4.png" alt-text="konum değeri":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="e348e-139">Azure VM kullanımını ve rezervasyon iskontosunu doğrulama</span><span class="sxs-lookup"><span data-stu-id="e348e-139">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="e348e-140">Bir müşteri adına bir Azure ayrılmış VM örneği satın aldıktan sonra, önce VM alanı için ödeme indirimi, müşteri rezervasyonunun öznitelikleriyle ve miktarıyla eşleşen sanal makinelere otomatik olarak uygulanır.</span><span class="sxs-lookup"><span data-stu-id="e348e-140">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="e348e-141">Aşağıdaki yöntemlerden birini kullanarak, müşterinin rezervasyon kullanımını doğrulayabilirsiniz ve rezervasyon iskontolarının hangi sanal makineleri uygulanacağını görebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="e348e-141">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="e348e-142">Azure portal</span><span class="sxs-lookup"><span data-stu-id="e348e-142">The Azure portal</span></span>
- <span data-ttu-id="e348e-143">Azure kullanım API 'SI</span><span class="sxs-lookup"><span data-stu-id="e348e-143">Azure utilization API</span></span>

<span data-ttu-id="e348e-144">Bu yöntemlerin her birini kullanmaya yönelik yönergeler aşağıda verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="e348e-144">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="e348e-145">Yalnızca Azure kullanım API 'SI, iskontonun hangi sanal makinede uygulanacağını gösterir.</span><span class="sxs-lookup"><span data-stu-id="e348e-145">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="e348e-146">Microsoft Azure portal müşterinin rezervasyon kullanımını doğrulayın</span><span class="sxs-lookup"><span data-stu-id="e348e-146">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="e348e-147">Iş Ortağı Merkezi 'nde **müşteriler** sayfanıza gidin.</span><span class="sxs-lookup"><span data-stu-id="e348e-147">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="e348e-148">Rezervasyon indirimi ve kullanımını doğrulamak istediğiniz müşteriyi bulun ve ardından müşterinin bilgilerini genişletmek için aşağı oku seçin.</span><span class="sxs-lookup"><span data-stu-id="e348e-148">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="e348e-149">**Microsoft Azure yönetim portalı** ' yi seçerek müşterinin kaydını Azure Portal açın.</span><span class="sxs-lookup"><span data-stu-id="e348e-149">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="e348e-150">Portal menüsünden **ayırmalar** ' ı seçin ve ardından kullanımı denetlemek istediğiniz ayırmayı seçin.</span><span class="sxs-lookup"><span data-stu-id="e348e-150">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="e348e-151">**Genel bakış** sayfasında, rezervasyonun sanal makinelere ne kadarının uygulandığını gösteren kullanım grafiğini kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="e348e-151">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="e348e-152">Kullanım verileri 8 saate kadar gecikebilir.</span><span class="sxs-lookup"><span data-stu-id="e348e-152">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="e348e-153">a.</span><span class="sxs-lookup"><span data-stu-id="e348e-153">a.</span></span> <span data-ttu-id="e348e-154">Rezervasyonun kullanımı %100 ise, müşteriniz, rezervasyon satın alma işlemi tarafından sağlanacak tüm olası tasarrufları elde edebilir.</span><span class="sxs-lookup"><span data-stu-id="e348e-154">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="e348e-155">b.</span><span class="sxs-lookup"><span data-stu-id="e348e-155">b.</span></span> <span data-ttu-id="e348e-156">Rezervasyonun kullanımı %0 ise, indirim herhangi bir sanal makineye uygulanmaz.</span><span class="sxs-lookup"><span data-stu-id="e348e-156">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="e348e-157">c.</span><span class="sxs-lookup"><span data-stu-id="e348e-157">c.</span></span> <span data-ttu-id="e348e-158">Rezervasyonun kullanımı %1 ile %99 arasındaysa, kullanılmayan avantajlar vardır.</span><span class="sxs-lookup"><span data-stu-id="e348e-158">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="e348e-159">Bu durumdan kaçınmak için, satın almayı yapmadan önce müşterinin bilgi işlem ihtiyaçlarını desteklemek üzere doğru boyut sanal makinesini saptayın.</span><span class="sxs-lookup"><span data-stu-id="e348e-159">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="e348e-160">Azure kullanım API 'SI ile müşterinin rezervasyon kullanımını doğrulama</span><span class="sxs-lookup"><span data-stu-id="e348e-160">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="e348e-161">Yalnızca Azure kullanım API 'SI, iskontonun hangi sanal makinede uygulanacağını gösterir.</span><span class="sxs-lookup"><span data-stu-id="e348e-161">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="e348e-162">Müşterinin rezervasyon iskontosunu aldığını doğrulamak ve iskontonun hangi VM 'Ler (sanal makineler) uygulanacağını öğrenmek için Azure kullanım API 'SI ile rezervasyon kullanım verilerini alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="e348e-162">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="e348e-163">Müşterinin ayırma kullanımını nasıl doğrulayabildiğini öğrenmek için örneğin, örnek B ile karşılaştırın.</span><span class="sxs-lookup"><span data-stu-id="e348e-163">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Ayırma kullanım örnekleri":::

- <span data-ttu-id="e348e-165">Rezervkimliği, iskontoyu VM 'ye uygulamak için kullanılan Azure ayırmasını tanımlar.</span><span class="sxs-lookup"><span data-stu-id="e348e-165">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="e348e-166">Tüketiytionmetre, rezervasyon iskontosunun uygulandığı VM için ölçüm kimliği.</span><span class="sxs-lookup"><span data-stu-id="e348e-166">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="e348e-167">Ayırma indirimi uygulandıktan sonra rezervde $0 maliyeti gösterilmektedir.</span><span class="sxs-lookup"><span data-stu-id="e348e-167">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="e348e-168">Daha fazla bilgi için bkz. [Iş ortağı MERKEZI API](/partner-center/develop/)'de [Azure için bir müşterinin kullanım kayıtlarını edinme](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) .</span><span class="sxs-lookup"><span data-stu-id="e348e-168">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="e348e-169">Microsoft Windows Server gibi yazılım maliyetleri, şu anda bir VM ayırma fiyatına dahil değildir ve sipariş kaydında ve faturanızda ayrı satır öğeleri olarak görünür.</span><span class="sxs-lookup"><span data-stu-id="e348e-169">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="e348e-170">Ancak, bir müşterinin Azure hibrit kullanım teklifi varsa, yazılım maliyetleri uygulanmaz.</span><span class="sxs-lookup"><span data-stu-id="e348e-170">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="e348e-171">Daha fazla bilgi için bkz. [Windows yazılım maliyetleri ayrılmış örneklere dahil değildir](/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="e348e-171">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="next-steps"></a><span data-ttu-id="e348e-172">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="e348e-172">Next steps</span></span>

|<span data-ttu-id="e348e-173">**Hakkında bilgi için**</span><span class="sxs-lookup"><span data-stu-id="e348e-173">**For information about**</span></span>   |<span data-ttu-id="e348e-174">**Bunu okuyun**</span><span class="sxs-lookup"><span data-stu-id="e348e-174">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="e348e-175">CSP 'de Azure ayırmaları genel bakış</span><span class="sxs-lookup"><span data-stu-id="e348e-175">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="e348e-176">Ayrılmış Microsoft Azure VM örnekleri satma</span><span class="sxs-lookup"><span data-stu-id="e348e-176">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="e348e-177">Iş Ortağı Merkezi 'nde müşterileriniz için Azure ayırmaları satın alma</span><span class="sxs-lookup"><span data-stu-id="e348e-177">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="e348e-178">Azure ayırmaları satın alma</span><span class="sxs-lookup"><span data-stu-id="e348e-178">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="e348e-179">Azure ayırmalarını Iş Ortağı Merkezi 'nde yönetme</span><span class="sxs-lookup"><span data-stu-id="e348e-179">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="e348e-180">Azure ayırmalarını Iş Ortağı Merkezi 'nde yönetme</span><span class="sxs-lookup"><span data-stu-id="e348e-180">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="e348e-181">Azure portal Azure ayırmaları satın alma</span><span class="sxs-lookup"><span data-stu-id="e348e-181">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="e348e-182">Azure yardım 'da [Azure ayrılmış VM örnekleri ile sanal makineler Için ön ödeme](/azure/virtual-machines/windows/prepay-reserved-vm-instances) yapın</span><span class="sxs-lookup"><span data-stu-id="e348e-182">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="e348e-183">Azure portal Azure ayırmalarını yönetme</span><span class="sxs-lookup"><span data-stu-id="e348e-183">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="e348e-184">Azure yardımında [ayrılmış VM örneklerini yönetme](/azure/billing/billing-manage-reserved-vm-instance)</span><span class="sxs-lookup"><span data-stu-id="e348e-184">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="e348e-185">Iş Ortağı Merkezi API 'sini kullanarak Azure ayırmaları satın alma</span><span class="sxs-lookup"><span data-stu-id="e348e-185">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="e348e-186">[Azure ayrılmış VM örneklerini](/partner-center/develop/purchase-azure-reservations) Iş Ortağı Merkezi geliştirici belgelerinde satın alma</span><span class="sxs-lookup"><span data-stu-id="e348e-186">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="e348e-187">Müşterilere satın almış olduğunuz bir abonelikten kendi Azure ayırmalarını satın alma izni verme.</span><span class="sxs-lookup"><span data-stu-id="e348e-187">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="e348e-188">Müşterilere kendi Azure ayırmalarını satın alma izni verin</span><span class="sxs-lookup"><span data-stu-id="e348e-188">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |