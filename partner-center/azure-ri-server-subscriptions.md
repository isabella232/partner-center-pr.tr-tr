---
title: Azure ayırmaları & sunucu abonelikleri
ms.topic: article
ms.date: 11/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Müşteriler için Azure ayırmaları ve sunucu abonelikleri alma, sağlama ve yönetme ile ilgili bulut çözümü sağlayıcısı fırsatları hakkında bilgi edinin.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1d5386dd4b2b19e641cc9d731d4a3d0f44ab5ad6
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182503"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="70d5b-103">Azure ayrılmış VM örnekleri (RI) ve müşteriler için sunucu abonelikleri alma, sağlama, & yönetme</span><span class="sxs-lookup"><span data-stu-id="70d5b-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>


<span data-ttu-id="70d5b-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="70d5b-104">**Appropriate roles**</span></span>

- <span data-ttu-id="70d5b-105">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="70d5b-105">Admin agent</span></span>
- <span data-ttu-id="70d5b-106">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="70d5b-106">Global admin</span></span>
- <span data-ttu-id="70d5b-107">Yardım Masası Aracısı</span><span class="sxs-lookup"><span data-stu-id="70d5b-107">Helpdesk agent</span></span>
- <span data-ttu-id="70d5b-108">Satış Aracısı</span><span class="sxs-lookup"><span data-stu-id="70d5b-108">Sales agent</span></span>
- <span data-ttu-id="70d5b-109">Kullanıcı Yönetimi Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="70d5b-109">User management admin</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="70d5b-110">Azure Ayırmaları nedir?</span><span class="sxs-lookup"><span data-stu-id="70d5b-110">What are Azure Reservations?</span></span>

<span data-ttu-id="70d5b-111">Azure ayırmaları, bir yıllık veya üç yıllık sanal makine, SQL veritabanı işlem kapasitesi, Azure Cosmos DB üretilen iş veya diğer Azure kaynakları için ön ödeme yaparak para tasarrufu yapmanıza yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="70d5b-111">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="70d5b-112">Ön ödeme, kullandığınız kaynaklara ilişkin bir indirim elde etmenizi sağlar.</span><span class="sxs-lookup"><span data-stu-id="70d5b-112">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="70d5b-113">Ayırmalar, sanal makinenizi, SQL veritabanı işlem, Azure Cosmos DB ve diğer kaynak maliyetlerinizi, Kullandıkça Öde fiyatlarına kıyasla %72 ' e varan ölçüde azaltabilir.</span><span class="sxs-lookup"><span data-stu-id="70d5b-113">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="70d5b-114">Rezervasyonlar bir faturalandırma indirimi sağlar ve kaynaklarınızın çalışma zamanı durumunu etkilemez.</span><span class="sxs-lookup"><span data-stu-id="70d5b-114">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="70d5b-115">Daha fazla bilgi için bkz. [Azure rezervasyonları nelerdir?](/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="70d5b-115">For more information see [What are Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="70d5b-116">Müşteriler neden bir rezervasyon satın almalıdır?</span><span class="sxs-lookup"><span data-stu-id="70d5b-116">Why should customers buy a reservation?</span></span>

<span data-ttu-id="70d5b-117">Müşteriler, uzun süreler boyunca çalışan sanal makinelere, Azure Cosmos DB veya SQL veritabanlarına sahip olursa, bir ayırma satın almak onlara en uygun maliyetli seçeneği sunar.</span><span class="sxs-lookup"><span data-stu-id="70d5b-117">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="70d5b-118">Örneğin, bir müşteri sürekli olarak bir hizmetin dört örneğini bir rezervasyon olmadan çalıştırıyorsa, Kullandıkça Öde tarifesine göre ücretlendirilir.</span><span class="sxs-lookup"><span data-stu-id="70d5b-118">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="70d5b-119">Bu kaynaklar için bir rezervasyon satın aldıklarında, derhal rezervasyon indirimi alırlar.</span><span class="sxs-lookup"><span data-stu-id="70d5b-119">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="70d5b-120">Kaynaklar artık kullandıkça öde tarifelerine göre ücretlendirilmez.</span><span class="sxs-lookup"><span data-stu-id="70d5b-120">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="70d5b-121">CSP 'de etkileyici yeni Azure teklifi</span><span class="sxs-lookup"><span data-stu-id="70d5b-121">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="70d5b-122">Microsoft, Azure ayırmaları ve sunucu aboneliklerini CSP programına getirerek, iş ortaklarının yüksek düzeyde öngörülebilir ve kalıcı bulut iş yüklerini desteklemeye yönelik daha uygun maliyetli çözümler için hızlı büyümekte olan müşteri taleplerini ele aldığının daha iyi hale getirilmesi daha iyidir.</span><span class="sxs-lookup"><span data-stu-id="70d5b-122">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="70d5b-123">CSP programı, iş ortaklarının Microsoft Iş ortağı merkezi ve Azure portal aracılığıyla ticari müşteriler adına Azure ayırmaları ve sunucu abonelikleri almasına, sağlamasını ve yönetmesine olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="70d5b-123">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>
<span data-ttu-id="70d5b-124">Azure rezervasyonların nasıl satın alınabileceğine ilişkin CSP programımızda iş ortakları da sunuyoruz.</span><span class="sxs-lookup"><span data-stu-id="70d5b-124">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="70d5b-125">CSP iş ortakları, [müşteri adına Azure ayırmaları satın](azure-reservations-buying.md) alabilir veya müşterinin iş ortağının satın aldığı önceki bir Azure aboneliğinden [kendi ayırmalarını satın](give-customers-permission.md) almasını sağlayabilir.</span><span class="sxs-lookup"><span data-stu-id="70d5b-125">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="70d5b-126">Azure ayırmaları, müşterilere geliştirme ve test, uygulama çalıştırma ve veri merkezini genişletme gibi çok çeşitli bilgi işlem çözümleri için sanallaştırma esnekliği sunar.</span><span class="sxs-lookup"><span data-stu-id="70d5b-126">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="70d5b-127">[Azure ayrılmış sanal makine örnekleri](https://azure.microsoft.com/pricing/reserved-vm-instances/) ile, ticari müşteriler artık %72 ' e kadar ve Kullandıkça Öde Azure VM fiyatlandırmasına yalnızca 1 veya 3 yıllık bir dönem için sanal makine satın alabilir.</span><span class="sxs-lookup"><span data-stu-id="70d5b-127">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="70d5b-128">Yazılım Güvencesi kapsamındaki Azure Hibrit Avantajı olan Windows Server müşterileri, Kullandıkça Öde fiyatlandırmasına ve %80 ' e kadar tasarruf sağlayabilecektir.</span><span class="sxs-lookup"><span data-stu-id="70d5b-128">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="70d5b-129">İlgi çekici fiyatlandırma ve eşleşmeyen dağıtım esnekliğinden oluşan eşleşmeyen bir birleşimiyle, müşteriler Azure ayırmaları seçerken en iyi genel değeri görür.</span><span class="sxs-lookup"><span data-stu-id="70d5b-129">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations.</span></span>

- <span data-ttu-id="70d5b-130">Bkz. Azure portalında [satın alma ayırmaları](/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) .</span><span class="sxs-lookup"><span data-stu-id="70d5b-130">See [Purchase Reservations](/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) on the Azure Portal.</span></span>

- <span data-ttu-id="70d5b-131">Yazılım abonelikleri ve Linux ISV yıllık abonelikleri için Iş Ortağı Merkezi 'nde [fiyatlandırma ve teklifler](https://partner.microsoft.com/dashboard/sell/pricingandoffers) sayfasındaki **Microsoft Azure ayrılmış örnekler** KATEGORISI altındaki **Azure RI CSP ticari fiyat listesine** bakın.</span><span class="sxs-lookup"><span data-stu-id="70d5b-131">See the **Azure RI CSP Commercial Price List** under the **Microsoft Azure Reserved Instances** category on the [Pricing and Offers](https://partner.microsoft.com/dashboard/sell/pricingandoffers) page in Partner Center for software subscriptions and Linux ISV annual subscriptions.</span></span>


 
<span data-ttu-id="70d5b-132">**Linux ISV yıllık abonelikleri**</span><span class="sxs-lookup"><span data-stu-id="70d5b-132">**Linux ISV annual subscriptions**</span></span>

- <span data-ttu-id="70d5b-133">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="70d5b-133">SUSE Linux</span></span>
- <span data-ttu-id="70d5b-134">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="70d5b-134">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="70d5b-135">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="70d5b-135">Azure Red Hat OpenShift</span></span>

<span data-ttu-id="70d5b-136">**ISV yıllık abonelikleri**</span><span class="sxs-lookup"><span data-stu-id="70d5b-136">**ISV annual subscriptions**</span></span>

- <span data-ttu-id="70d5b-137">CloudSimple tarafından sunulan Azure VMware Çözümü</span><span class="sxs-lookup"><span data-stu-id="70d5b-137">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="70d5b-138">Başlarken</span><span class="sxs-lookup"><span data-stu-id="70d5b-138">Getting started</span></span>

<span data-ttu-id="70d5b-139">Azure ayırmalarını müşterilerinizle nasıl konumlandırabileceğinizi anlamak için, mümkün olduğunca hızlı bir şekilde çalışmaya başlayın ve en kısa sürede çalışır duruma getirmek için, hazırlık malzemelerini gözden geçirmek için aşağıdaki yaklaşımı öneririz:</span><span class="sxs-lookup"><span data-stu-id="70d5b-139">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="70d5b-140">[Iş Ortağı Merkezi yeni ticaret işlemleri kılavuzunu](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf)gözden geçirin ve anlayın.</span><span class="sxs-lookup"><span data-stu-id="70d5b-140">Review and understand the [Partner Center new commerce operations guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf).</span></span>

2. <span data-ttu-id="70d5b-141">[Iş Ortağı Merkezi API 'sindeki (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)Azure ayırmaları ve sunucu abonelikleri güncelleştirmelerini anlayın.</span><span class="sxs-lookup"><span data-stu-id="70d5b-141">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances).</span></span>


### <a name="sales-readiness"></a><span data-ttu-id="70d5b-142">Satış hazırlığı</span><span class="sxs-lookup"><span data-stu-id="70d5b-142">Sales readiness</span></span>

- [<span data-ttu-id="70d5b-143">Uzak Masaüstü Hizmetleri (RDS) Istemci erişim lisansı (CAL) (duyuru)</span><span class="sxs-lookup"><span data-stu-id="70d5b-143">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)

- [<span data-ttu-id="70d5b-144">Azure ayrılmış VM örnekleri (Azure portal)</span><span class="sxs-lookup"><span data-stu-id="70d5b-144">Azure Reserved VM Instances (Azure portal)</span></span>](/azure/virtual-machines/windows/prepay-reserved-vm-instances)

- [<span data-ttu-id="70d5b-145">Sunucu abonelikleri</span><span class="sxs-lookup"><span data-stu-id="70d5b-145">Server Subscriptions</span></span>](./csp-software-subscriptions.md)

- [<span data-ttu-id="70d5b-146">SQL DB ayırmaları (Azure portal)</span><span class="sxs-lookup"><span data-stu-id="70d5b-146">SQL DB Reservations (Azure portal)</span></span>](/azure/sql-database/sql-database-reserved-capacity)

- [<span data-ttu-id="70d5b-147">Azure Cosmos DB (Azure portal)</span><span class="sxs-lookup"><span data-stu-id="70d5b-147">Azure Cosmos DB (Azure portal)</span></span>](/azure/cosmos-db/cosmos-db-reserved-capacity)

- [<span data-ttu-id="70d5b-148">SQL yönetilen örneği (Azure portal)</span><span class="sxs-lookup"><span data-stu-id="70d5b-148">SQL Managed Instance (Azure portal)</span></span>](/azure/sql-database/sql-database-managed-instance)

- [<span data-ttu-id="70d5b-149">SUSE ve Red Hat Enterprise Linux (Azure portal)</span><span class="sxs-lookup"><span data-stu-id="70d5b-149">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](/azure/virtual-machines/linux/prepay-suse-software-charges)

- [<span data-ttu-id="70d5b-150">Azure 'da Red Hat Linux</span><span class="sxs-lookup"><span data-stu-id="70d5b-150">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)

- [<span data-ttu-id="70d5b-151">Azure 'da SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="70d5b-151">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)

- [<span data-ttu-id="70d5b-152">Azure’da Linux</span><span class="sxs-lookup"><span data-stu-id="70d5b-152">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)

- [<span data-ttu-id="70d5b-153">Azure fiyatlandırmasına genel bakış</span><span class="sxs-lookup"><span data-stu-id="70d5b-153">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)

- [<span data-ttu-id="70d5b-154">Azure Fiyatlandırma Hesaplayıcı</span><span class="sxs-lookup"><span data-stu-id="70d5b-154">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)

- [<span data-ttu-id="70d5b-155">Azure Databricks birim ayırmaları</span><span class="sxs-lookup"><span data-stu-id="70d5b-155">Azure Databricks unit reservations</span></span>](/azure/billing/billing-prepay-databricks-reserved-capacity)


## <a name="training"></a><span data-ttu-id="70d5b-156">Eğitim</span><span class="sxs-lookup"><span data-stu-id="70d5b-156">Training</span></span>

<span data-ttu-id="70d5b-157">[Ticari lisanslama hazırlığı web seminerlerini](https://commercial-licensing.eventbuilder.com/FY2019_ALL) ve isteğe bağlı olayları görüntülemek için kaydolun.</span><span class="sxs-lookup"><span data-stu-id="70d5b-157">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>
<span data-ttu-id="70d5b-158">Önceden kaydedilen lisanslama hazırlığı isteğe bağlı olayları aşağıdakiler gibi konuları içerir:</span><span class="sxs-lookup"><span data-stu-id="70d5b-158">Previously recorded Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="70d5b-159">CSP çevrimiçi Hizmetleri, CSP Azure ve Azure dahil genel lisanslama güncelleştirmeleri (Kasım 2018)</span><span class="sxs-lookup"><span data-stu-id="70d5b-159">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>

- <span data-ttu-id="70d5b-160">SQL DB ayrılmış kapasitesi & örnek boyutu esnekliği (Ağustos 2018)</span><span class="sxs-lookup"><span data-stu-id="70d5b-160">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>

- <span data-ttu-id="70d5b-161">CSP 'de sunucu abonelikleri (Temmuz 2018)</span><span class="sxs-lookup"><span data-stu-id="70d5b-161">Server Subscriptions in CSP (July 2018)</span></span>

- <span data-ttu-id="70d5b-162">CSP 'de Azure ayırmaları genel bakış (Mayıs 2018)</span><span class="sxs-lookup"><span data-stu-id="70d5b-162">Azure Reservations Overview in CSP (May 2018)</span></span>

## <a name="operations"></a><span data-ttu-id="70d5b-163">İşlemler</span><span class="sxs-lookup"><span data-stu-id="70d5b-163">Operations</span></span>

<span data-ttu-id="70d5b-164">[Iş Ortağı Merkezi yeni ticari işlemler Kılavuzu](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf): anlaşma, Iş Ortağı Merkezi, fatura, Fiyat Listesi ayrıntıları, teşvikleri, mutabakat dosyası, API/SDK, korumalı alan ve Azure Iş ortağı paylaşılan hizmetleri gibi önemli ilke ve operasyonel yönleri kapsayan kapsamlı kılavuz.</span><span class="sxs-lookup"><span data-stu-id="70d5b-164">[Partner Center new commerce operations guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf):  Comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="70d5b-165">Azure Hibrit Avantajı</span><span class="sxs-lookup"><span data-stu-id="70d5b-165">Azure Hybrid Benefit</span></span>

<span data-ttu-id="70d5b-166">[Azure hibrit avantajı](https://azure.microsoft.com/pricing/hybrid-benefit) , yazılım güvencesi olan lisanslarına sahip olan ve Azure 'a geçiş yaparken mevcut şirket Içi Windows Server ve/veya SQL Server lisans yatırımlarının en üst düzeye çıkmasına yardımcı olan müşterilere yönelik fiyatlandırma avantajıdır.</span><span class="sxs-lookup"><span data-stu-id="70d5b-166">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) is a pricing benefit for customers who have licenses with Software Assurance, which helps maximize the value of existing on-premises Windows Server and/or SQL Server license investments when migrating to Azure.</span></span> <span data-ttu-id="70d5b-167">Uygun müşteriler Azure sanal makinelerine (hizmet olarak altyapı veya IaaS) %40 ' e kadar tasarruf edebilir ve Azure SQL veritabanı 'nda (hizmet olarak platform veya Azure Hibrit Avantajı SQL Server PaaS) %55 ' e kadar tasarruf edebilir ve Azure ayrılmış örneklerle birleştirildiğinde %80 ' ye kadar artar.</span><span class="sxs-lookup"><span data-stu-id="70d5b-167">Eligible customers can save up to 40%\* on Azure Virtual Machines (infrastructure as a service, or IaaS), and save up to 55% on Azure SQL Database (platform as a service, or PaaS) and SQL Server on Azure Virtual Machines (IaaS) with Azure Hybrid Benefit, which increases to up to 80% when combined with Azure Reserved Instances.</span></span>

## <a name="next-steps"></a><span data-ttu-id="70d5b-168">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="70d5b-168">Next steps</span></span>

- [<span data-ttu-id="70d5b-169">Azure Hibrit Avantajı Hakkında SSS</span><span class="sxs-lookup"><span data-stu-id="70d5b-169">Azure Hybrid Benefit FAQ</span></span>](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)

<span data-ttu-id="70d5b-170">\* Gerçek tasarruf, bölgeye, örnek türüne veya kullanıma göre farklılık gösterebilir.</span><span class="sxs-lookup"><span data-stu-id="70d5b-170">\*Actual savings may vary based on region, instance type, or usage.</span></span>