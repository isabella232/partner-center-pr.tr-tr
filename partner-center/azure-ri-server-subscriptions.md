---
title: Azure ayırmaları & sunucu abonelikleri
ms.topic: article
ms.date: 08/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Müşteriler için Azure ayırmaları ve sunucu abonelikleri alma, sağlama ve yönetme ile ilgili bulut çözümü sağlayıcısı fırsatları hakkında bilgi edinin.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3c08e897a8f5d7c11b36627b0c24ad2da3f92329
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/22/2020
ms.locfileid: "92531626"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="f00fd-103">Azure ayrılmış VM örnekleri (RI) ve müşteriler için sunucu abonelikleri alma, sağlama, & yönetme</span><span class="sxs-lookup"><span data-stu-id="f00fd-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>

<span data-ttu-id="f00fd-104">Aşağıdakiler cihazlar için geçerlidir:</span><span class="sxs-lookup"><span data-stu-id="f00fd-104">Applies to:</span></span>

- <span data-ttu-id="f00fd-105">İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="f00fd-105">Partner Center</span></span>

<span data-ttu-id="f00fd-106">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="f00fd-106">**Appropriate roles**</span></span>

- <span data-ttu-id="f00fd-107">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="f00fd-107">Admin agent</span></span>
- <span data-ttu-id="f00fd-108">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="f00fd-108">Global admin</span></span>
- <span data-ttu-id="f00fd-109">Yardım Masası Aracısı</span><span class="sxs-lookup"><span data-stu-id="f00fd-109">Helpdesk agent</span></span>
- <span data-ttu-id="f00fd-110">Satış Aracısı</span><span class="sxs-lookup"><span data-stu-id="f00fd-110">Sales agent</span></span>
- <span data-ttu-id="f00fd-111">Kullanıcı Yönetimi Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="f00fd-111">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="f00fd-112">Bu makale yalnızca bulut çözümü sağlayıcısı (CSP) programındaki iş ortakları için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="f00fd-112">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="f00fd-113">Diğer abonelik türleri (örneğin, Kullandıkça öde, bireysel, Microsoft Müşteri Sözleşmesi veya Kurumsal Anlaşma abonelikleri) kullanan müşteriler [Bu Azure ayırmaları belgelerini](/azure/cost-management-billing/reservations)okumalı olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="f00fd-113">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="f00fd-114">Azure Ayırmaları nedir?</span><span class="sxs-lookup"><span data-stu-id="f00fd-114">What are Azure Reservations?</span></span>

<span data-ttu-id="f00fd-115">Azure ayırmaları, bir yıllık veya üç yıllık sanal makine, SQL veritabanı işlem kapasitesi, Azure Cosmos DB üretilen iş veya diğer Azure kaynakları için ön ödeme yaparak para tasarrufu yapmanıza yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="f00fd-115">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="f00fd-116">Ön ödeme, kullandığınız kaynaklara ilişkin bir indirim elde etmenizi sağlar.</span><span class="sxs-lookup"><span data-stu-id="f00fd-116">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="f00fd-117">Ayırmalar, sanal makinenizi, SQL veritabanı işlem, Azure Cosmos DB ve diğer kaynak maliyetlerinizi, Kullandıkça Öde fiyatlarına kıyasla %72 ' e varan ölçüde azaltabilir.</span><span class="sxs-lookup"><span data-stu-id="f00fd-117">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="f00fd-118">Rezervasyonlar bir faturalandırma indirimi sağlar ve kaynaklarınızın çalışma zamanı durumunu etkilemez.</span><span class="sxs-lookup"><span data-stu-id="f00fd-118">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="f00fd-119">Daha fazla bilgi için bkz. [Azure rezervasyonları nelerdir?](/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="f00fd-119">For more information see [What are Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="f00fd-120">Müşteriler neden bir rezervasyon satın almalıdır?</span><span class="sxs-lookup"><span data-stu-id="f00fd-120">Why should customers buy a reservation?</span></span>

<span data-ttu-id="f00fd-121">Müşteriler, uzun süreler boyunca çalışan sanal makinelere, Azure Cosmos DB veya SQL veritabanlarına sahip olursa, bir ayırma satın almak onlara en uygun maliyetli seçeneği sunar.</span><span class="sxs-lookup"><span data-stu-id="f00fd-121">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="f00fd-122">Örneğin, bir müşteri sürekli olarak bir hizmetin dört örneğini bir rezervasyon olmadan çalıştırıyorsa, Kullandıkça Öde tarifesine göre ücretlendirilir.</span><span class="sxs-lookup"><span data-stu-id="f00fd-122">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="f00fd-123">Bu kaynaklar için bir rezervasyon satın aldıklarında, derhal rezervasyon indirimi alırlar.</span><span class="sxs-lookup"><span data-stu-id="f00fd-123">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="f00fd-124">Kaynaklar artık kullandıkça öde tarifelerine göre ücretlendirilmez.</span><span class="sxs-lookup"><span data-stu-id="f00fd-124">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="f00fd-125">CSP 'de etkileyici yeni Azure teklifi</span><span class="sxs-lookup"><span data-stu-id="f00fd-125">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="f00fd-126">Microsoft, Azure ayırmaları ve sunucu aboneliklerini CSP programına getirerek, iş ortaklarının yüksek düzeyde öngörülebilir ve kalıcı bulut iş yüklerini desteklemeye yönelik daha uygun maliyetli çözümler için hızlı büyümekte olan müşteri taleplerini ele aldığının daha iyi hale getirilmesi daha iyidir.</span><span class="sxs-lookup"><span data-stu-id="f00fd-126">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="f00fd-127">CSP programı, iş ortaklarının Microsoft Iş ortağı merkezi ve Azure portal aracılığıyla ticari müşteriler adına Azure ayırmaları ve sunucu abonelikleri almasına, sağlamasını ve yönetmesine olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="f00fd-127">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>

<span data-ttu-id="f00fd-128">Azure rezervasyonların nasıl satın alınabileceğine ilişkin CSP programımızda iş ortakları da sunuyoruz.</span><span class="sxs-lookup"><span data-stu-id="f00fd-128">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="f00fd-129">CSP iş ortakları, [müşteri adına Azure ayırmaları satın](azure-reservations-buying.md) alabilir veya müşterinin iş ortağının satın aldığı önceki bir Azure aboneliğinden [kendi ayırmalarını satın](give-customers-permission.md) almasını sağlayabilir.</span><span class="sxs-lookup"><span data-stu-id="f00fd-129">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="f00fd-130">Azure ayırmaları, müşterilere geliştirme ve test, uygulama çalıştırma ve veri merkezini genişletme gibi çok çeşitli bilgi işlem çözümleri için sanallaştırma esnekliği sunar.</span><span class="sxs-lookup"><span data-stu-id="f00fd-130">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="f00fd-131">[Azure ayrılmış sanal makine örnekleri](https://azure.microsoft.com/pricing/reserved-vm-instances/) ile, ticari müşteriler artık %72 ' e kadar ve Kullandıkça Öde Azure VM fiyatlandırmasına yalnızca 1 veya 3 yıllık bir dönem için sanal makine satın alabilir.</span><span class="sxs-lookup"><span data-stu-id="f00fd-131">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="f00fd-132">Yazılım Güvencesi kapsamındaki Azure Hibrit Avantajı olan Windows Server müşterileri, Kullandıkça Öde fiyatlandırmasına ve %80 ' e kadar tasarruf sağlayabilecektir.</span><span class="sxs-lookup"><span data-stu-id="f00fd-132">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="f00fd-133">İlgi çekici fiyatlandırma ve eşleşmeyen dağıtım esnekliğinden oluşan eşleşmeyen bir birleşimiyle, müşteriler Azure ayırmaları seçerken en iyi genel değeri görür:</span><span class="sxs-lookup"><span data-stu-id="f00fd-133">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="f00fd-134">Azure rezervasyonları</span><span class="sxs-lookup"><span data-stu-id="f00fd-134">Azure reservations</span></span>

- <span data-ttu-id="f00fd-135">Azure ayrılmış VM örnekleri</span><span class="sxs-lookup"><span data-stu-id="f00fd-135">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="f00fd-136">SQL DB ayırmaları</span><span class="sxs-lookup"><span data-stu-id="f00fd-136">SQL DB Reservations</span></span>
- <span data-ttu-id="f00fd-137">SQL Yönetilen Örnek</span><span class="sxs-lookup"><span data-stu-id="f00fd-137">SQL Managed Instance</span></span>
- <span data-ttu-id="f00fd-138">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f00fd-138">Azure Cosmos DB</span></span>
- <span data-ttu-id="f00fd-139">Azure SQL Veri Ambarı</span><span class="sxs-lookup"><span data-stu-id="f00fd-139">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="f00fd-140">Uygulama Hizmetleri</span><span class="sxs-lookup"><span data-stu-id="f00fd-140">App Services</span></span>
- <span data-ttu-id="f00fd-141">Azure Databricks birim ayırmaları</span><span class="sxs-lookup"><span data-stu-id="f00fd-141">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="f00fd-142">Yönetilen Disk</span><span class="sxs-lookup"><span data-stu-id="f00fd-142">Managed Disk</span></span>
- <span data-ttu-id="f00fd-143">Blok blobu</span><span class="sxs-lookup"><span data-stu-id="f00fd-143">Block blob</span></span>
- <span data-ttu-id="f00fd-144">MySQL</span><span class="sxs-lookup"><span data-stu-id="f00fd-144">MySQL</span></span>
- <span data-ttu-id="f00fd-145">Azure Veri Gezgini</span><span class="sxs-lookup"><span data-stu-id="f00fd-145">Azure Data explorer</span></span>
- <span data-ttu-id="f00fd-146">MariaDB</span><span class="sxs-lookup"><span data-stu-id="f00fd-146">MariaDB</span></span>
- <span data-ttu-id="f00fd-147">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="f00fd-147">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="f00fd-148">Sunucu abonelikleri</span><span class="sxs-lookup"><span data-stu-id="f00fd-148">Server subscriptions</span></span>

- <span data-ttu-id="f00fd-149">Windows Server</span><span class="sxs-lookup"><span data-stu-id="f00fd-149">Windows Server</span></span>
- <span data-ttu-id="f00fd-150">Uzak Masaüstü Hizmetleri (RDS) Cal 'Leri</span><span class="sxs-lookup"><span data-stu-id="f00fd-150">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="f00fd-151">SQL Server</span><span class="sxs-lookup"><span data-stu-id="f00fd-151">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="f00fd-152">Linux ISV yıllık abonelikleri</span><span class="sxs-lookup"><span data-stu-id="f00fd-152">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="f00fd-153">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="f00fd-153">SUSE Linux</span></span>
- <span data-ttu-id="f00fd-154">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="f00fd-154">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="f00fd-155">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="f00fd-155">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="f00fd-156">ISV yıllık abonelikleri</span><span class="sxs-lookup"><span data-stu-id="f00fd-156">ISV annual subscriptions</span></span>

- <span data-ttu-id="f00fd-157">CloudSimple tarafından sunulan Azure VMware Çözümü</span><span class="sxs-lookup"><span data-stu-id="f00fd-157">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="f00fd-158">Kullanmaya başlama</span><span class="sxs-lookup"><span data-stu-id="f00fd-158">Getting started</span></span>

<span data-ttu-id="f00fd-159">Azure ayırmalarını müşterilerinizle nasıl konumlandırabileceğinizi anlamak için, mümkün olduğunca hızlı bir şekilde çalışmaya başlayın ve en kısa sürede çalışır duruma getirmek için, hazırlık malzemelerini gözden geçirmek için aşağıdaki yaklaşımı öneririz:</span><span class="sxs-lookup"><span data-stu-id="f00fd-159">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="f00fd-160">Müşteri değeri teklifi ve konumlandırma için genel bakış sunularını ve ilgili web seminerlerini gözden geçirin</span><span class="sxs-lookup"><span data-stu-id="f00fd-160">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="f00fd-161">Modern ticaret Işletim kılavuzunu gözden geçirin ve anlayın</span><span class="sxs-lookup"><span data-stu-id="f00fd-161">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="f00fd-162">Azure RI ve sunucu aboneliklerini gözden geçirin SSS</span><span class="sxs-lookup"><span data-stu-id="f00fd-162">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="f00fd-163">Iş Ortağı Merkezi API 'sindeki Azure ayırmaları ve sunucu abonelikleri için güncelleştirmeleri anlama [(API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)</span><span class="sxs-lookup"><span data-stu-id="f00fd-163">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="f00fd-164">Kaynaklar</span><span class="sxs-lookup"><span data-stu-id="f00fd-164">Resources</span></span>

<span data-ttu-id="f00fd-165">Aşağıda, Iş Ortağı Merkezi aracılığıyla deneyimidir Azure ayırmalarını hızla eklemenize yardımcı olacak kaynakların kapsamlı bir listesi verilmiştir:</span><span class="sxs-lookup"><span data-stu-id="f00fd-165">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="f00fd-166">Satış hazırlığı</span><span class="sxs-lookup"><span data-stu-id="f00fd-166">Sales readiness</span></span>

- [<span data-ttu-id="f00fd-167">Azure Hibrit Avantajı genel bakış ile Azure ayırmaları ve sunucu abonelikleri</span><span class="sxs-lookup"><span data-stu-id="f00fd-167">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="f00fd-168">Satış sayfası</span><span class="sxs-lookup"><span data-stu-id="f00fd-168">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="f00fd-169">Azure ayırmaları için iş ortağı SSS</span><span class="sxs-lookup"><span data-stu-id="f00fd-169">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="f00fd-170">Azure ayırmaları ve SQL DB için iş ortağı SSS</span><span class="sxs-lookup"><span data-stu-id="f00fd-170">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="f00fd-171">Uzak Masaüstü Hizmetleri (RDS) Istemci erişim lisansı (CAL) (duyuru)</span><span class="sxs-lookup"><span data-stu-id="f00fd-171">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="f00fd-172">Azure ayrılmış VM örnekleri (Azure portal)</span><span class="sxs-lookup"><span data-stu-id="f00fd-172">Azure Reserved VM Instances (Azure portal)</span></span>](/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="f00fd-173">Sunucu abonelikleri</span><span class="sxs-lookup"><span data-stu-id="f00fd-173">Server Subscriptions</span></span>](csp-software-subscriptions.md)
- [<span data-ttu-id="f00fd-174">Azure 'da SQL DB 'ye Genel Bakış</span><span class="sxs-lookup"><span data-stu-id="f00fd-174">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="f00fd-175">SQL DB ayırmaları (Azure portal)</span><span class="sxs-lookup"><span data-stu-id="f00fd-175">SQL DB Reservations (Azure portal)</span></span>](/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="f00fd-176">Azure Cosmos DB (Azure portal)</span><span class="sxs-lookup"><span data-stu-id="f00fd-176">Azure Cosmos DB (Azure portal)</span></span>](/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="f00fd-177">SQL yönetilen örneği (Azure portal)</span><span class="sxs-lookup"><span data-stu-id="f00fd-177">SQL Managed Instance (Azure portal)</span></span>](/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="f00fd-178">SUSE ve Red Hat Enterprise Linux (Azure portal)</span><span class="sxs-lookup"><span data-stu-id="f00fd-178">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="f00fd-179">Azure 'da Red Hat Linux</span><span class="sxs-lookup"><span data-stu-id="f00fd-179">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="f00fd-180">Azure 'da SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="f00fd-180">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="f00fd-181">Azure’da Linux</span><span class="sxs-lookup"><span data-stu-id="f00fd-181">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="f00fd-182">Azure fiyatlandırmasına genel bakış</span><span class="sxs-lookup"><span data-stu-id="f00fd-182">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="f00fd-183">Azure Fiyatlandırma Hesaplayıcı</span><span class="sxs-lookup"><span data-stu-id="f00fd-183">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="f00fd-184">Azure Databricks birim ayırmaları</span><span class="sxs-lookup"><span data-stu-id="f00fd-184">Azure Databricks unit reservations</span></span>](/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="f00fd-185">CSP fiyat listeleri: **Microsoft Azure ayrılmış örnekler** ve **yazılım abonelikleri** fiyat listeleri, hem iş ortağı Merkezi [fiyatlandırma & teklifleri](https://partner.microsoft.com/pcv/sales) sayfasında bulunur.</span><span class="sxs-lookup"><span data-stu-id="f00fd-185">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="f00fd-186">Eğitim</span><span class="sxs-lookup"><span data-stu-id="f00fd-186">Training</span></span>

<span data-ttu-id="f00fd-187">[Ticari lisanslama hazırlığı web seminerlerini](https://commercial-licensing.eventbuilder.com/FY2019_ALL) ve isteğe bağlı olayları görüntülemek için kaydolun.</span><span class="sxs-lookup"><span data-stu-id="f00fd-187">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>

<span data-ttu-id="f00fd-188">Lisanslama hazırlığı isteğe bağlı olayları aşağıdakiler gibi konuları içerir:</span><span class="sxs-lookup"><span data-stu-id="f00fd-188">Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="f00fd-189">CSP çevrimiçi Hizmetleri, CSP Azure ve Azure dahil genel lisanslama güncelleştirmeleri (Kasım 2018)</span><span class="sxs-lookup"><span data-stu-id="f00fd-189">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>
- <span data-ttu-id="f00fd-190">SQL DB ayrılmış kapasitesi & örnek boyutu esnekliği (Ağustos 2018)</span><span class="sxs-lookup"><span data-stu-id="f00fd-190">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>
- <span data-ttu-id="f00fd-191">CSP 'de sunucu abonelikleri (Temmuz 2018)</span><span class="sxs-lookup"><span data-stu-id="f00fd-191">Server Subscriptions in CSP (July 2018)</span></span>
- <span data-ttu-id="f00fd-192">CSP 'de Azure ayırmaları genel bakış (Mayıs 2018)</span><span class="sxs-lookup"><span data-stu-id="f00fd-192">Azure Reservations Overview in CSP (May 2018)</span></span>

<span data-ttu-id="f00fd-193">Diğer yararlı eğitim, [Iş ortağı University 'de Azure lisanslama modülünü](https://aka.ms/azure_partner_licensing)içerir.</span><span class="sxs-lookup"><span data-stu-id="f00fd-193">Other useful training includes the [Azure Licensing Module on Partner University](https://aka.ms/azure_partner_licensing).</span></span>

### <a name="operations"></a><span data-ttu-id="f00fd-194">İşlemler</span><span class="sxs-lookup"><span data-stu-id="f00fd-194">Operations</span></span>

- <span data-ttu-id="f00fd-195">[Modern ticaret Işlemleri Kılavuzu](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (güncelleştirilmiş): anlaşma, Iş Ortağı Merkezi, fatura, Fiyat Listesi ayrıntıları, teşvikleri, mutabakat dosyası, API/SDK, korumalı alan ve Azure Iş ortağı paylaşılan hizmetleri gibi önemli ilke ve işlem yönlerini kapsayan kapsamlı bir kılavuz.</span><span class="sxs-lookup"><span data-stu-id="f00fd-195">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="f00fd-196">Modern ülke kullanılabilirliği ve müşteri para birimi matrisi sağlar</span><span class="sxs-lookup"><span data-stu-id="f00fd-196">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="f00fd-197">Ayrılmış Microsoft Azure örnekleri satma</span><span class="sxs-lookup"><span data-stu-id="f00fd-197">Sell Microsoft Azure Reserved Instances</span></span>](azure-reservations.md)
- [<span data-ttu-id="f00fd-198">Müşterileriniz adına Microsoft Azure ayırmaları satın alın</span><span class="sxs-lookup"><span data-stu-id="f00fd-198">Buy Microsoft Azure reservations on behalf of your customers</span></span>](azure-reservations-buying.md)
- [<span data-ttu-id="f00fd-199">Azure rezervasyonlarını müşterileriniz adına yönetme</span><span class="sxs-lookup"><span data-stu-id="f00fd-199">Manage Azure reservations on behalf of your customers</span></span>](azure-reservations-manage.md)
- [<span data-ttu-id="f00fd-200">Azure ayırmaları için faturalandırma</span><span class="sxs-lookup"><span data-stu-id="f00fd-200">Billing for Azure reservations</span></span>](azure-plan-billing.md)
- [<span data-ttu-id="f00fd-201">Maksimum ayırma kullanımı için VM boyutu</span><span class="sxs-lookup"><span data-stu-id="f00fd-201">VM sizing for maximum reservation usage</span></span>](azure-usage.md)
- [<span data-ttu-id="f00fd-202">İş Ortağı Merkezi API 'SI (API/SDK)</span><span class="sxs-lookup"><span data-stu-id="f00fd-202">Partner Center API (API/SDK)</span></span>](/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="f00fd-203">Uzak Masaüstü Hizmetleri</span><span class="sxs-lookup"><span data-stu-id="f00fd-203">Remote Desktop Services</span></span>](/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="f00fd-204">Azure Hibrit Avantajı</span><span class="sxs-lookup"><span data-stu-id="f00fd-204">Azure Hybrid Benefit</span></span>

<span data-ttu-id="f00fd-205">[Azure hibrit avantajı](https://azure.microsoft.com/pricing/hybrid-benefit) , Windows Server lisanslarınızdan daha fazla değer almanıza ve sanal makinelerde yüzde 47 ' a varan bir tasarruf etmenize yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="f00fd-205">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="f00fd-206">Yazılım Güvencesi kapsamındaki Windows Server Datacenter ve Standard Edition lisanslarıyla avantajını kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f00fd-206">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="f00fd-207">Sürüme bağlı olarak, Azure 'da Windows Server sanal makinelerini çalıştırmak için lisanslarınızı dönüştürebilir veya yeniden kullanabilir ve daha düşük bir temel işlem ücreti (Linux sanal makine ücretleri) ödeyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f00fd-207">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="f00fd-208">Ayrıca bkz. [Azure HIBRIT AVANTAJı SSS](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span><span class="sxs-lookup"><span data-stu-id="f00fd-208">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="f00fd-209">\* Gerçek tasarruf, bölgeye, örnek türüne veya kullanıma göre farklılık gösterebilir.</span><span class="sxs-lookup"><span data-stu-id="f00fd-209">\*Actual savings may vary based on region, instance type, or usage.</span></span>
