---
title: Yönetilen hizmetler için iş ortağı kazanılmış kredisi
ms.topic: article
ms.date: 11/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Yönetilen hizmetler için Microsoft iş ortağı kredisi (PEC) nasıl hesaplanacağını ve ödendiğini ve uygun şekilde nasıl emin olduğunuzu öğrenin.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 97af446c4021e9785833374131eee2f08431b5fe
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/01/2020
ms.locfileid: "96474317"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a><span data-ttu-id="068c2-103">İş ortağı kazanılmış kredisinin hesaplanması ve ödenmesi</span><span class="sxs-lookup"><span data-stu-id="068c2-103">How the partner earned credit is calculated and paid</span></span>

<span data-ttu-id="068c2-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="068c2-104">**Appropriate roles**</span></span>

- <span data-ttu-id="068c2-105">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="068c2-105">Global admin</span></span>
- <span data-ttu-id="068c2-106">Kullanıcı yöneticisi</span><span class="sxs-lookup"><span data-stu-id="068c2-106">User admin</span></span>
- <span data-ttu-id="068c2-107">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="068c2-107">Admin agent</span></span>
- <span data-ttu-id="068c2-108">Faturalama yöneticisi</span><span class="sxs-lookup"><span data-stu-id="068c2-108">Billing admin</span></span>
- <span data-ttu-id="068c2-109">Satış Aracısı</span><span class="sxs-lookup"><span data-stu-id="068c2-109">Sales agent</span></span>

<span data-ttu-id="068c2-110">Yönetilen hizmetler (PEC) için iş ortağı kazanılmış kredisi, müşterilerine 7/24 BT işletimsel denetim ve bunların bölümlerinin yönetimi ve müşterilerinin tüm Azure ortamı gibi iş ortaklarını tanır ve depolar.</span><span class="sxs-lookup"><span data-stu-id="068c2-110">Partner earned credit for managed services (PEC) recognizes and rewards partners that own the 24x7 IT operational control and management of parts of, or the entire, Azure environment of their customers.</span></span> <span data-ttu-id="068c2-111">Varsayılan olarak, CSP 'de iş ortaklarına, aboneliğin abonelik üzerinde 24 X 7 işlemsel yönetim ve denetim gerçekleştirmesine izin veren, müşterinin aboneliğine gerekli erişim hakları verilir.</span><span class="sxs-lookup"><span data-stu-id="068c2-111">By default, in CSP, partners are granted the necessary access rights to the customer's subscription allowing them to perform 24 X 7 operational management and control of the resources on the subscription.</span></span> <span data-ttu-id="068c2-112">Müşterinin deneyimidir iş ortağı için erişim sağlayabildiği diğer yollar aşağıdaki bölümde açıklanmıştır.</span><span class="sxs-lookup"><span data-stu-id="068c2-112">Additional ways in which customer can provision access for transacting partner is described in the following section.</span></span> <span data-ttu-id="068c2-113">Aylık fatura tutarı, iş ortağının kazandığı net kredi tutarıdır.</span><span class="sxs-lookup"><span data-stu-id="068c2-113">The monthly invoice amount is net of partner earned credit.</span></span> <span data-ttu-id="068c2-114">İş ortakları, aylık keşfi dosyasında PEC ayrıntılarını görebilir.</span><span class="sxs-lookup"><span data-stu-id="068c2-114">Partners can see the PEC details on their monthly recon file.</span></span> <span data-ttu-id="068c2-115">Müşterinin deneyimidir iş ortağı için erişim sağlayabildiği ek yollar için, [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)makalesini okuyun.</span><span class="sxs-lookup"><span data-stu-id="068c2-115">For additional ways in which a customer can provision access for the transacting partner, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="068c2-116">Ayrıca, [Azure CSP abonelikleri için yeniden devreye sokma yönetici ayrıcalıklarını](revoke-reinstate-csp.md) oku</span><span class="sxs-lookup"><span data-stu-id="068c2-116">Also read [Reinstate admin privileges for Azure CSP subscriptions](revoke-reinstate-csp.md)</span></span>

## <a name="important-eligibility-and-calculation-information"></a><span data-ttu-id="068c2-117">Önemli uygunluk ve hesaplama bilgileri</span><span class="sxs-lookup"><span data-stu-id="068c2-117">Important eligibility and calculation information</span></span>

- <span data-ttu-id="068c2-118">İş ortağı, yönettikleri Azure varlıklarının kazanıldığını alacak bir etkin MPN sözleşmesine ve geçerli RBAC rolüne sahip olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="068c2-118">Partner should have an active MPN agreement and valid RBAC role to receive earned credit for the Azure assets they manage.</span></span> 

- <span data-ttu-id="068c2-119">Dolaylı sağlayıcılar ve dolaylı satıcılarında, dolaylı sağlayıcı veya dolaylı satıcı ya da her ikisi de satıcının CSP 'deki Azure kaynaklarının 7/24 işletimsel denetim ve yönetimine sahip olan dolaylı sağlayıcı PEC 'e uygun olacaktır.</span><span class="sxs-lookup"><span data-stu-id="068c2-119">In the case of indirect providers and their indirect resellers, the indirect provider will be eligible for PEC if either the indirect provider, or the indirect reseller or both have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span>

- <span data-ttu-id="068c2-120">PEC, müşterinin iş ortağı tarafından yönetilen CSP 'de Azure 'un Azure 'da yaptığı Azure 'un faturalandırılma (Borçlandırılabilir) tüketimle ilişkilendirilir.</span><span class="sxs-lookup"><span data-stu-id="068c2-120">PEC is associated to billed (chargeable) consumption of customer's Azure estate in CSP managed by the partner.</span></span> <span data-ttu-id="068c2-121">PEC, yalnızca Microsoft tarafından faturalandırılan (dolaylı sağlayıcı ve doğrudan fatura ortağı) CSP 'deki iş ortakları için kullanılabilir hale getirilir.</span><span class="sxs-lookup"><span data-stu-id="068c2-121">PEC is made available only to partners in CSP billed by Microsoft (indirect provider and direct bill partner).</span></span> 

- <span data-ttu-id="068c2-122">Uygun hizmetler: Iş ortağı kazanılmış kredisi, Azure plan [fiyatlandırma](https://partner.microsoft.com/commerce/sales) sayfasından iş ortaklarının dışarı aktarılacağı **Azure plan tüketim fiyatlandırması** 'nda listelenen hizmetler için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="068c2-122">Eligible services: Partner earned credit is applicable to services listed in the **Azure plan consumption pricing** which partners can export from the [Azure plan pricing](https://partner.microsoft.com/commerce/sales) page.</span></span> 

- <span data-ttu-id="068c2-123">Uygun olmayan hizmetler: Iş ortağı kazanılmış kredisi \**_değil_*, şunlar için geçerlidir:</span><span class="sxs-lookup"><span data-stu-id="068c2-123">Ineligible services: Partner earned credit is \**_not_* _ applicable to the following:</span></span>
    - <span data-ttu-id="068c2-124">Azure plan ayırmaları</span><span class="sxs-lookup"><span data-stu-id="068c2-124">Azure Plan reservations</span></span>
    - <span data-ttu-id="068c2-125">Azure plan tüketim fiyatının **Etiketler sütununda** _ *üçüncü taraf*\* olarak tanımlanan üçüncü taraf ürünleri</span><span class="sxs-lookup"><span data-stu-id="068c2-125">Third-party products identified as _ *Third Party*\* in the **Tags column** of the Azure plan consumption price</span></span>    
    - <span data-ttu-id="068c2-126">Market fiyat listesindeki ürünler</span><span class="sxs-lookup"><span data-stu-id="068c2-126">Products in the Marketplace price list</span></span>
   - [<span data-ttu-id="068c2-127">Azure spot sanal makineleri</span><span class="sxs-lookup"><span data-stu-id="068c2-127">Azure Spot Virtual Machines</span></span>](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- <span data-ttu-id="068c2-128">PEC günlük olarak hesaplanır ve günlük kullanım dosyasında ve aylık fatura keşfi dosyasında görüntülenebilir.</span><span class="sxs-lookup"><span data-stu-id="068c2-128">PEC is calculated daily and can be viewed in the daily usage file and monthly invoice recon file.</span></span> <span data-ttu-id="068c2-129">Bir iş ortağı (dolaylı sağlayıcı veya dolaylı satıcı), PEC kazanıdıklarından emin olmak için tüm gün (7/24) erişimi olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="068c2-129">A partner (indirect provider or indirect reseller) must have access for the entire day (24x7) to ensure they earn PEC.</span></span> <span data-ttu-id="068c2-130">PEC, yönetilen Azure varlıkları için günlük olarak hesaplanır.</span><span class="sxs-lookup"><span data-stu-id="068c2-130">PEC is calculated on daily basis on the managed Azure assets.</span></span> <span data-ttu-id="068c2-131">Belirli bir fatura dönemi için maksimum PEC (ay) %15 ' tir.</span><span class="sxs-lookup"><span data-stu-id="068c2-131">The maximum PEC for a given billing period (Month) is 15%.</span></span> <span data-ttu-id="068c2-132">İş ortakları ay (erişim kapsamı) ile kalıcı ayrıcalıklı erişimi korur ve tüm uygun kaynaklar (erişim kapsamı) için tam PEC %15 kazanacaktır.</span><span class="sxs-lookup"><span data-stu-id="068c2-132">Partners retaining persistent privileged access through the month(span of access) and for all the eligible resources (scope of access) will earn full PEC of 15%.</span></span> <span data-ttu-id="068c2-133">Kapsam ve yayılma azaltma, ay için daha düşük PEC oranına neden olur.</span><span class="sxs-lookup"><span data-stu-id="068c2-133">Scope and span reduction will result in lower PEC rate for the month.</span></span> <span data-ttu-id="068c2-134">Günlük derecelendirildi kullanım dosyası, PEC 'in uygulanıp uygulanmadığı bir Azure varlığı üzerinde günlük olarak gösterilir.</span><span class="sxs-lookup"><span data-stu-id="068c2-134">Daily rated usage file shows on daily basis on an Azure asset whether PEC is applied or not.</span></span> <span data-ttu-id="068c2-135">Ayrıca iş ortakları, kalıcı ayrıcalıklı erişim değişiklikleri olup olmadığını algılamak için uyarılara de kaydolabilir.</span><span class="sxs-lookup"><span data-stu-id="068c2-135">Partners can also enroll in alerts to detect if there are changes to persistent privileged access.</span></span>

- <span data-ttu-id="068c2-136">PEC, Azure Kaynak düzeyine kadar kazanılmakta.</span><span class="sxs-lookup"><span data-stu-id="068c2-136">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="068c2-137">İş ortağı abonelikte veya kaynak grubu düzeyinde geçerli erişime sahipse, daha yüksek varlığa kadar olan her bir kaynak PEC kazanıcaktır.</span><span class="sxs-lookup"><span data-stu-id="068c2-137">If the partner has valid access at the subscription, or resource group level, each resource that roles up to the higher entity will earn PEC.</span></span>  

- <span data-ttu-id="068c2-138">PEC ayrıntıları [Azure maliyet yönetimi](/azure/cost-management-billing/costs/get-started-partners) 'nde de kullanılabilir olacaktır</span><span class="sxs-lookup"><span data-stu-id="068c2-138">PEC details will also be available on [Azure Cost management](/azure/cost-management-billing/costs/get-started-partners)</span></span>

## <a name="azure-cost-management"></a><span data-ttu-id="068c2-139">Azure Maliyet Yönetimi</span><span class="sxs-lookup"><span data-stu-id="068c2-139">Azure Cost Management</span></span>

<span data-ttu-id="068c2-140">Maliyet analizini kullanan Azure maliyet yönetimi (ACM), PEC 'in avantajını almış olan maliyetleri görüntülemek için bir iş ortağı olarak size olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="068c2-140">Azure Cost Management (ACM) using Cost Analysis enables you as a partner to view the costs that have received the benefit of PEC.</span></span>  

1. <span data-ttu-id="068c2-141">[Azure Portal](https://portal.azure.com), iş ortağı kiracınızda oturum açın ve **maliyet yönetimi + faturalandırma**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="068c2-141">In the [Azure portal](https://portal.azure.com), sign into your partner tenant and select **Cost Management + Billing**.</span></span>

2. <span data-ttu-id="068c2-142">**Maliyet yönetimi** Seç</span><span class="sxs-lookup"><span data-stu-id="068c2-142">Select **Cost management**</span></span>

3. <span data-ttu-id="068c2-143">**Maliyet analizini** seçin</span><span class="sxs-lookup"><span data-stu-id="068c2-143">Select **Cost Analysis**</span></span>

   <span data-ttu-id="068c2-144">Maliyet analizi görünümü, satın alınan ve Microsoft 'a ödediğiniz fiyatlarla tüketilen tüm hizmetler için faturalandırma hesabınızın maliyetlerini görüntüler.</span><span class="sxs-lookup"><span data-stu-id="068c2-144">The Cost Analysis view will display the costs for your billing account, for all the services purchased and consumed at the prices that you pay Microsoft.</span></span>

4. <span data-ttu-id="068c2-145">PEC 'in uygulandığı maliyetleri görmek için bir Özet grafiğinde açılan kutuda **Partnerearnedtappnda** ' u seçin.</span><span class="sxs-lookup"><span data-stu-id="068c2-145">Select **PartnerEarnedCreditApplied** in the drop down on a pivot chart to see costs that have PEC applied.</span></span> <span data-ttu-id="068c2-146">**Partnerearnedkredtappekonomi** özelliği true olduğunda, ilişkili maliyet iş ortağının kazanılan kredisi avantajına sahiptir.</span><span class="sxs-lookup"><span data-stu-id="068c2-146">When **PartnerEarnedCreditApplied** property is True, the associated cost has the benefit of the partner earned credit.</span></span> 

<span data-ttu-id="068c2-147">Partnertatnedkredtappekonomi özelliği false olduğunda, ilişkili maliyet kredi için gereken uygunluğu karşılamıyor veya satın alınan hizmet, iş ortağı tarafından kazanılan kredi için uygun değil.</span><span class="sxs-lookup"><span data-stu-id="068c2-147">When the PartnerEarnedCreditApplied property is False, the associated cost has not met the required eligibility for the credit or the service purchased is not eligible for partner earned credit.</span></span>

>[!NOTE] 
><span data-ttu-id="068c2-148">Genellikle, hizmetler için kullanım **Maliyet yönetiminde** 8-24 saat sürer ve Pec kredileri, Azure maliyet yönetimi 'nde erişim zamanından itibaren 48 saat içinde görünür.</span><span class="sxs-lookup"><span data-stu-id="068c2-148">Typically, usage for services takes 8-24 hours to appear in **Cost Management** and the PEC credits will appear within 48 hours from time of access in Azure Cost Management.</span></span>

5. <span data-ttu-id="068c2-149">Ayrıca, **Grup ölçütü** ' ne göre gruplandırma yapabilir ve filtreleme özellikleri **ekleyerek, PEC** 'e ve Pec uygulanmamış maliyetlere sahip olan maliyetlerde detaya gitme özelliği ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="068c2-149">You can also group by, and filter by, the **PartnerEarnedCreditApplied** property using the **Group by and Add** filter features to drill into costs that have PEC and the costs that have no PEC applied.</span></span>

## <a name="next-steps"></a><span data-ttu-id="068c2-150">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="068c2-150">Next steps</span></span>

- [<span data-ttu-id="068c2-151">İş ortağı kazanılmış kredi-genel bakış</span><span class="sxs-lookup"><span data-stu-id="068c2-151">Partner earned credit - overview</span></span>](partner-earned-credit.md)

- <span data-ttu-id="068c2-152">İş ortağı kazanılmış kredi hesaplamalarının ayrıntılı örnekleri, Iş Ortağı Merkezi panosu (oturum açma gerekir) aracılığıyla ulaşabileceğiniz fiyat listesinde bulunur.</span><span class="sxs-lookup"><span data-stu-id="068c2-152">Detailed examples of partner earned credit calculations are located on the price list which you can reach through the Partner Center dashboard (sign-in required).</span></span>

- [<span data-ttu-id="068c2-153">Azure planına taşıma-kullanmaya başlama</span><span class="sxs-lookup"><span data-stu-id="068c2-153">Move to Azure plan - get started</span></span>](azure-plan-get-started.md)

- [<span data-ttu-id="068c2-154">Azure planı kapsamındaki abonelikleri ve kaynakları yönetme</span><span class="sxs-lookup"><span data-stu-id="068c2-154">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="068c2-155">Azure CSP abonelikleri için yönetici ayrıcalıklarını iptal etme veya yeniden alma</span><span class="sxs-lookup"><span data-stu-id="068c2-155">Revoke or re-instate admin privileges for Azure CSP subscriptions</span></span>](revoke-reinstate-csp.md)
