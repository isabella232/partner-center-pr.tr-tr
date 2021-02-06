---
title: Yönetilen hizmetler için iş ortağı kazanılmış kredisi
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Yönetilen hizmetler için Microsoft iş ortağı kredisi (PEC) nasıl hesaplanacağını ve ödendiğini ve uygun şekilde nasıl emin olduğunuzu öğrenin.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 010f74164b0428a5cd6ffcde5000b52ac6a6993f
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624009"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a><span data-ttu-id="45ae0-103">İş ortağı kazanılmış kredisinin hesaplanması ve ödenmesi</span><span class="sxs-lookup"><span data-stu-id="45ae0-103">How the partner earned credit is calculated and paid</span></span>

<span data-ttu-id="45ae0-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="45ae0-104">**Appropriate roles**</span></span>

- <span data-ttu-id="45ae0-105">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="45ae0-105">Global admin</span></span>
- <span data-ttu-id="45ae0-106">Kullanıcı yöneticisi</span><span class="sxs-lookup"><span data-stu-id="45ae0-106">User admin</span></span>
- <span data-ttu-id="45ae0-107">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="45ae0-107">Admin agent</span></span>
- <span data-ttu-id="45ae0-108">Faturalama yöneticisi</span><span class="sxs-lookup"><span data-stu-id="45ae0-108">Billing admin</span></span>
- <span data-ttu-id="45ae0-109">Satış Aracısı</span><span class="sxs-lookup"><span data-stu-id="45ae0-109">Sales agent</span></span>

<span data-ttu-id="45ae0-110">Yönetilen hizmetler (PEC) için iş ortağı kazanılmış kredisi, müşterilerine 7/24 BT işletimsel denetim ve bunların bölümlerinin yönetimi ve müşterilerinin tüm Azure ortamı gibi iş ortaklarını tanır ve depolar.</span><span class="sxs-lookup"><span data-stu-id="45ae0-110">Partner earned credit for managed services (PEC) recognizes and rewards partners that own the 24x7 IT operational control and management of parts of, or the entire, Azure environment of their customers.</span></span> <span data-ttu-id="45ae0-111">Varsayılan olarak, CSP 'de iş ortaklarına, aboneliğin abonelik üzerinde 24 X 7 işlemsel yönetim ve denetim gerçekleştirmesine izin veren, müşterinin aboneliğine gerekli erişim hakları verilir.</span><span class="sxs-lookup"><span data-stu-id="45ae0-111">By default, in CSP, partners are granted the necessary access rights to the customer's subscription allowing them to perform 24 X 7 operational management and control of the resources on the subscription.</span></span> <span data-ttu-id="45ae0-112">Müşterinin deneyimidir iş ortağı için erişim sağlayabildiği diğer yollar aşağıdaki bölümde açıklanmıştır.</span><span class="sxs-lookup"><span data-stu-id="45ae0-112">Additional ways in which customer can provision access for transacting partner is described in the following section.</span></span> <span data-ttu-id="45ae0-113">Aylık fatura tutarı, iş ortağının kazandığı net kredi tutarıdır.</span><span class="sxs-lookup"><span data-stu-id="45ae0-113">The monthly invoice amount is net of partner earned credit.</span></span> <span data-ttu-id="45ae0-114">İş ortakları, aylık keşfi dosyasında PEC ayrıntılarını görebilir.</span><span class="sxs-lookup"><span data-stu-id="45ae0-114">Partners can see the PEC details on their monthly recon file.</span></span> <span data-ttu-id="45ae0-115">Müşterinin deneyimidir iş ortağı için erişim sağlayabildiği ek yollar için, [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)makalesini okuyun.</span><span class="sxs-lookup"><span data-stu-id="45ae0-115">For additional ways in which a customer can provision access for the transacting partner, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="45ae0-116">Ayrıca, [Azure CSP abonelikleri için yeniden devreye sokma yönetici ayrıcalıklarını](revoke-reinstate-csp.md) oku</span><span class="sxs-lookup"><span data-stu-id="45ae0-116">Also read [Reinstate admin privileges for Azure CSP subscriptions](revoke-reinstate-csp.md)</span></span>

## <a name="eligibility"></a><span data-ttu-id="45ae0-117">Önceliği</span><span class="sxs-lookup"><span data-stu-id="45ae0-117">Eligibility</span></span>

<span data-ttu-id="45ae0-118">İş ortağı kazanılmış kredisi (PEC) almak için aşağıdaki gereksinimler geçerlidir:</span><span class="sxs-lookup"><span data-stu-id="45ae0-118">In order to receive the partner earned credit (PEC), the following requirements apply:</span></span> 

- <span data-ttu-id="45ae0-119">Yönettiğiniz Azure varlıklarının kazanıldığını alacak bir etkin MPN anlaşmanız ve geçerli rol tabanlı erişim denetimi (RBAC) rolüne sahip olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="45ae0-119">You must have an active MPN agreement and valid role-based access control (RBAC) role to receive earned credit for the Azure assets you manage.</span></span>

- <span data-ttu-id="45ae0-120">CSP 'de müşterinin Azure kaynaklarını 7/24 işletimsel denetim ve yönetimine sahip olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="45ae0-120">You must have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span> <span data-ttu-id="45ae0-121">Bu, müşterinin Azure aboneliği, Azure Kaynak grubu, Azure kaynağı üzerinde yönetici ayrıcalıklarına sahip olmanız gerektiği anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="45ae0-121">This means you must have admin privileges on the customer’s Azure subscription, Azure resource group, Azure resource.</span></span> <span data-ttu-id="45ae0-122">Dolaylı sağlayıcılar ve dolaylı satıcıları söz konusu olduğunda, dolaylı sağlayıcı veya dolaylı satıcı ya da her ikisinin de bu işlemsel denetimi varsa, dolaylı sağlayıcı PEC 'e uygun olacaktır.</span><span class="sxs-lookup"><span data-stu-id="45ae0-122">In the case of indirect providers and their indirect resellers, the indirect provider will be eligible for PEC if either the indirect provider or the indirect reseller or both have this operational control.</span></span> <span data-ttu-id="45ae0-123">Bunun hakkında daha fazla bilgi edinmek için bkz. [Azure CSP abonelikleri için yeniden devreye alma yönetici ayrıcalıkları](./revoke-reinstate-csp.md).</span><span class="sxs-lookup"><span data-stu-id="45ae0-123">To learn more about this, see [Reinstate admin privileges for Azure CSP subscriptions](./revoke-reinstate-csp.md).</span></span>

- <span data-ttu-id="45ae0-124">PEC, yukarıdaki gereksinimlere ek olarak yalnızca Azure plan [fiyatlandırma](https://partner.microsoft.com/commerce/sales) sayfasından dışarı aktarmak için Azure plan tüketim fiyatlandırması 'nda listelenen hizmetlere uygulanabilir.</span><span class="sxs-lookup"><span data-stu-id="45ae0-124">In addition to the requirements above, PEC is only applicable to services listed in the Azure plan consumption pricing, which you can export from the [Azure plan pricing](https://partner.microsoft.com/commerce/sales) page.</span></span>

- <span data-ttu-id="45ae0-125">PEC, aşağıdaki hizmetler için geçerli **değildir** :</span><span class="sxs-lookup"><span data-stu-id="45ae0-125">PEC is **not** applicable to the following services:</span></span>
    - <span data-ttu-id="45ae0-126">Azure plan ayırmaları</span><span class="sxs-lookup"><span data-stu-id="45ae0-126">Azure Plan reservations</span></span>
    - <span data-ttu-id="45ae0-127">Azure plan tüketim fiyatının Etiketler sütununda üçüncü taraf olarak tanımlanan üçüncü taraf ürünleri</span><span class="sxs-lookup"><span data-stu-id="45ae0-127">Third-party products identified as Third Party in the Tags column of the Azure plan consumption price</span></span>
    - <span data-ttu-id="45ae0-128">Market fiyat listesindeki ürünler</span><span class="sxs-lookup"><span data-stu-id="45ae0-128">Products in the Marketplace price list</span></span>
    - [<span data-ttu-id="45ae0-129">Azure spot sanal makineleri</span><span class="sxs-lookup"><span data-stu-id="45ae0-129">Azure Spot Virtual Machines</span></span>](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- <span data-ttu-id="45ae0-130">PEC, Azure Kaynak düzeyine kadar kazanılmakta.</span><span class="sxs-lookup"><span data-stu-id="45ae0-130">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="45ae0-131">Abonelik veya kaynak grubu düzeyinde geçerli erişiminiz varsa, daha yüksek varlığa kaydolan her kaynak PEC 'e kazanacaktır.</span><span class="sxs-lookup"><span data-stu-id="45ae0-131">If you have valid access at either the subscription or resource group level, each resource that rolls up to the higher entity will earn PEC.</span></span>

- <span data-ttu-id="45ae0-132">PEC ile ilgili ayrıntılar için [Azure maliyet yönetimi](/azure/cost-management-billing/costs/get-started-partners) sayfasından da ulaşılabilir.</span><span class="sxs-lookup"><span data-stu-id="45ae0-132">Details on PEC are also available on the [Azure Cost management](/azure/cost-management-billing/costs/get-started-partners) page.</span></span>

### <a name="calculation"></a><span data-ttu-id="45ae0-133">Hesaplama</span><span class="sxs-lookup"><span data-stu-id="45ae0-133">Calculation</span></span>

<span data-ttu-id="45ae0-134">PEC günlük olarak hesaplanır ve günlük kullanım dosyasında ve aylık fatura keşfi dosyasında görüntülenebilir.</span><span class="sxs-lookup"><span data-stu-id="45ae0-134">PEC is calculated daily and can be viewed in the daily usage file and monthly invoice recon file.</span></span> <span data-ttu-id="45ae0-135">Bir iş ortağı (dolaylı sağlayıcı veya dolaylı satıcı), PEC kazanıdıklarından emin olmak için tüm gün (7/24) erişimi olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="45ae0-135">A partner (indirect provider or indirect reseller) must have access for the entire day (24x7) to ensure they earn PEC.</span></span> <span data-ttu-id="45ae0-136">PEC, yönetilen Azure varlıklarının her gün temelinde hesaplanır.</span><span class="sxs-lookup"><span data-stu-id="45ae0-136">PEC is calculated on a daily basis on the managed Azure assets.</span></span> <span data-ttu-id="45ae0-137">İş ortakları ayda kalıcı ayrıcalıklı erişimi (erişim kapsamı) ve tüm uygun kaynakların (erişim kapsamı) tam PEC kazanmasına sahip olur.</span><span class="sxs-lookup"><span data-stu-id="45ae0-137">Partners retaining persistent privileged access through the month (span of access) and for all the eligible resources (scope of access) will earn full PEC.</span></span> <span data-ttu-id="45ae0-138">Kapsam ve yayılma azaltma, ay için daha düşük PEC oranına neden olur.</span><span class="sxs-lookup"><span data-stu-id="45ae0-138">Scope and span reduction will result in lower PEC rate for the month.</span></span> <span data-ttu-id="45ae0-139">Günlük olarak derecelendirilen kullanım dosyası, PEC 'in uygulanıp uygulanmadığı bir Azure varlığı üzerinde günlük olarak gösterilir.</span><span class="sxs-lookup"><span data-stu-id="45ae0-139">Daily rated usage file shows on a daily basis on an Azure asset, whether PEC is applied or not.</span></span> <span data-ttu-id="45ae0-140">İş ortakları, kalıcı ayrıcalıklı erişimdeki değişiklikleri izlemek için uyarılara de kaydolabilir.</span><span class="sxs-lookup"><span data-stu-id="45ae0-140">Partners can also enroll in alerts to monitor changes to persistent privileged access.</span></span>

## <a name="azure-cost-management"></a><span data-ttu-id="45ae0-141">Azure Maliyet Yönetimi</span><span class="sxs-lookup"><span data-stu-id="45ae0-141">Azure Cost Management</span></span>

<span data-ttu-id="45ae0-142">Maliyet analizini kullanan Azure maliyet yönetimi (ACM), PEC 'in avantajını almış olan maliyetleri görüntülemek için bir iş ortağı olarak size olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="45ae0-142">Azure Cost Management (ACM) using Cost Analysis enables you as a partner to view the costs that have received the benefit of PEC.</span></span>  

1. <span data-ttu-id="45ae0-143">[Azure Portal](https://portal.azure.com), iş ortağı kiracınızda oturum açın ve **maliyet yönetimi + faturalandırma**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="45ae0-143">In the [Azure portal](https://portal.azure.com), sign into your partner tenant and select **Cost Management + Billing**.</span></span>

2. <span data-ttu-id="45ae0-144">**Maliyet yönetimi** Seç</span><span class="sxs-lookup"><span data-stu-id="45ae0-144">Select **Cost management**</span></span>

3. <span data-ttu-id="45ae0-145">**Maliyet analizini** seçin</span><span class="sxs-lookup"><span data-stu-id="45ae0-145">Select **Cost Analysis**</span></span>

   <span data-ttu-id="45ae0-146">Maliyet analizi görünümü, satın alınan ve Microsoft 'a ödediğiniz fiyatlarla tüketilen tüm hizmetler için faturalandırma hesabınızın maliyetlerini görüntüler.</span><span class="sxs-lookup"><span data-stu-id="45ae0-146">The Cost Analysis view will display the costs for your billing account, for all the services purchased and consumed at the prices that you pay Microsoft.</span></span>

4. <span data-ttu-id="45ae0-147">PEC 'in uygulandığı maliyetleri görmek için bir Özet grafiğinde açılan kutuda **Partnerearnedtappnda** ' u seçin.</span><span class="sxs-lookup"><span data-stu-id="45ae0-147">Select **PartnerEarnedCreditApplied** in the drop down on a pivot chart to see costs that have PEC applied.</span></span> <span data-ttu-id="45ae0-148">**Partnerearnedkredtappekonomi** özelliği true olduğunda, ilişkili maliyet iş ortağının kazanılan kredisi avantajına sahiptir.</span><span class="sxs-lookup"><span data-stu-id="45ae0-148">When **PartnerEarnedCreditApplied** property is True, the associated cost has the benefit of the partner earned credit.</span></span> 

   <span data-ttu-id="45ae0-149">Partnertatnedkredtappekonomi özelliği false olduğunda, ilişkili maliyet kredi için gereken uygunluğu karşılamıyor veya satın alınan hizmet, iş ortağı tarafından kazanılan kredi için uygun değil.</span><span class="sxs-lookup"><span data-stu-id="45ae0-149">When the PartnerEarnedCreditApplied property is False, the associated cost has not met the required eligibility for the credit or the service purchased is not eligible for partner earned credit.</span></span>

   >[!NOTE] 
   ><span data-ttu-id="45ae0-150">Genellikle, hizmetler için kullanım **Maliyet yönetiminde** 8-24 saat sürer ve Pec kredileri, Azure maliyet yönetimi 'nde erişim zamanından itibaren 48 saat içinde görünür.</span><span class="sxs-lookup"><span data-stu-id="45ae0-150">Typically, usage for services takes 8-24 hours to appear in **Cost Management** and the PEC credits will appear within 48 hours from time of access in Azure Cost Management.</span></span>

5. <span data-ttu-id="45ae0-151">Ayrıca, **Grup ölçütü** ' ne göre gruplandırma yapabilir ve filtreleme özellikleri **ekleyerek, PEC** 'e ve Pec uygulanmamış maliyetlere sahip olan maliyetlerde detaya gitme özelliği ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="45ae0-151">You can also group by, and filter by, the **PartnerEarnedCreditApplied** property using the **Group by and Add** filter features to drill into costs that have PEC and the costs that have no PEC applied.</span></span>

## <a name="next-steps"></a><span data-ttu-id="45ae0-152">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="45ae0-152">Next steps</span></span>

- [<span data-ttu-id="45ae0-153">İş ortağı kazanılmış kredi-genel bakış</span><span class="sxs-lookup"><span data-stu-id="45ae0-153">Partner earned credit - overview</span></span>](partner-earned-credit.md)

- <span data-ttu-id="45ae0-154">İş ortağı kazanılmış kredi hesaplamalarının ayrıntılı örnekleri, Iş Ortağı Merkezi panosu (oturum açma gerekir) aracılığıyla ulaşabileceğiniz fiyat listesinde bulunur.</span><span class="sxs-lookup"><span data-stu-id="45ae0-154">Detailed examples of partner earned credit calculations are located on the price list which you can reach through the Partner Center dashboard (sign-in required).</span></span>

- [<span data-ttu-id="45ae0-155">Azure planına taşıma-kullanmaya başlama</span><span class="sxs-lookup"><span data-stu-id="45ae0-155">Move to Azure plan - get started</span></span>](azure-plan-get-started.md)

- [<span data-ttu-id="45ae0-156">Azure planı kapsamındaki abonelikleri ve kaynakları yönetme</span><span class="sxs-lookup"><span data-stu-id="45ae0-156">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="45ae0-157">Azure CSP abonelikleri için yönetici ayrıcalıklarını iptal etme veya yeniden alma</span><span class="sxs-lookup"><span data-stu-id="45ae0-157">Revoke or re-instate admin privileges for Azure CSP subscriptions</span></span>](revoke-reinstate-csp.md)
