---
title: Rezervasyonları Microsoft Azure müşterilere satma
description: Bir bulut çözümü sağlayıcısı olarak müşteriler için Azure ayırmaları satın alabilir, sattabilir veya yönetebilirsiniz. Iş Ortağı Merkezi, Azure portal veya Iş Ortağı Merkezi API 'sini kullanın.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 317d1f0295b79b79bf06f1091ae365bc7012b749
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/22/2020
ms.locfileid: "92531627"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="c74a2-104">Iş Ortağı Merkezi, Azure portal veya API 'Leri kullanarak müşterilere Microsoft Azure ayırmaları satma</span><span class="sxs-lookup"><span data-stu-id="c74a2-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="c74a2-105">**Uygulama hedefi**</span><span class="sxs-lookup"><span data-stu-id="c74a2-105">**Applies to**</span></span>

- <span data-ttu-id="c74a2-106">İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="c74a2-106">Partner Center</span></span>
- <span data-ttu-id="c74a2-107">Microsoft Azure portalı</span><span class="sxs-lookup"><span data-stu-id="c74a2-107">Microsoft Azure portal</span></span>
- <span data-ttu-id="c74a2-108">CSP programındaki iş ortakları</span><span class="sxs-lookup"><span data-stu-id="c74a2-108">Partners in the CSP program</span></span>

<span data-ttu-id="c74a2-109">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="c74a2-109">**Appropriate roles**</span></span>

- <span data-ttu-id="c74a2-110">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="c74a2-110">Admin agent</span></span>
- <span data-ttu-id="c74a2-111">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="c74a2-111">Global admin</span></span>
- <span data-ttu-id="c74a2-112">Yardım Masası Aracısı</span><span class="sxs-lookup"><span data-stu-id="c74a2-112">Helpdesk agent</span></span>
- <span data-ttu-id="c74a2-113">Satış Aracısı</span><span class="sxs-lookup"><span data-stu-id="c74a2-113">Sales agent</span></span>
- <span data-ttu-id="c74a2-114">Kullanıcı Yönetimi Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="c74a2-114">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="c74a2-115">Bu makale yalnızca bulut çözümü sağlayıcısı (CSP) programındaki iş ortakları için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="c74a2-115">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="c74a2-116">Diğer abonelik türleri (örneğin, Kullandıkça öde, bireysel, Microsoft Müşteri Sözleşmesi veya Kurumsal Anlaşma abonelikleri) kullanan müşteriler [Bu Azure ayırmaları belgelerini](/azure/cost-management-billing/reservations)okumalı olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="c74a2-116">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="c74a2-117">CSP programındaki iş ortakları, müşterilerine Microsoft Azure ayırmaları sunabilir.</span><span class="sxs-lookup"><span data-stu-id="c74a2-117">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="c74a2-118">Müşteriler, önceden ayrıldıklarında önemli tasarruf elde edebilirler.</span><span class="sxs-lookup"><span data-stu-id="c74a2-118">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="c74a2-119">Azure ayırmaları, müşterileri basitliği ve esnekliği aşağıdaki yollarla sunmaktadır:</span><span class="sxs-lookup"><span data-stu-id="c74a2-119">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="c74a2-120">Bir veya üç yıllık rezervasyon terimi</span><span class="sxs-lookup"><span data-stu-id="c74a2-120">One or three-year reservation terms</span></span>
- <span data-ttu-id="c74a2-121">Kullanmaya başlamak kolaydır; Kurulum saniye cinsinden tamamlandı</span><span class="sxs-lookup"><span data-stu-id="c74a2-121">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="c74a2-122">Ayarlanmış para iadesi için dilediğiniz zaman ayrılan örnekleri iptal edin veya değiştirin</span><span class="sxs-lookup"><span data-stu-id="c74a2-122">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="c74a2-123">Ayrılmış örnek kullanımını kurumsal veya ayrı departman düzeyinde yönetme</span><span class="sxs-lookup"><span data-stu-id="c74a2-123">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="c74a2-124">Azure ayırmaları, müşterilere aşağıdaki yollarla yol açabilir:</span><span class="sxs-lookup"><span data-stu-id="c74a2-124">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="c74a2-125">Rezervasyonlar, Kullandıkça Öde (PAYG) fiyatlandırmasına göre önemli tasarruf sağlayabilir</span><span class="sxs-lookup"><span data-stu-id="c74a2-125">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="c74a2-126">Tek yıllık veya üç yıllık şartlar için ön ödeme ile daha iyi bütçeleme ve tahmin</span><span class="sxs-lookup"><span data-stu-id="c74a2-126">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="c74a2-127">Azure bölgesinde ofislerine en yakın önceliğe sahip bilgi işlem kapasitesi</span><span class="sxs-lookup"><span data-stu-id="c74a2-127">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="c74a2-128">Azure ayırmaları, Microsoft Windows Server ve Azure SQL veritabanı gibi yazılımlarla birleştirildiğinde uçtan uca altyapı çözümlerine yönelik temel sağlar</span><span class="sxs-lookup"><span data-stu-id="c74a2-128">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="c74a2-129">Azure ayırmalarını hem Iş ortağı merkezi hem de Azure portal satın alabilir, satın alabilir ve yönetebilirsiniz ve Iş Ortağı Merkezi API 'sini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c74a2-129">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="c74a2-130">Müşterilerinize satın almış olduğunuz bir Azure aboneliğinden kendi Azure ayırmalarını satın alma izni verebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c74a2-130">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="c74a2-131">Hakkında bilgi edinmek için aşağıdaki bağlantıları izleyin.</span><span class="sxs-lookup"><span data-stu-id="c74a2-131">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="c74a2-132">Azure ayırmaları kaynakları</span><span class="sxs-lookup"><span data-stu-id="c74a2-132">Azure reservations resources</span></span>

|<span data-ttu-id="c74a2-133">**Hakkında bilgi için**</span><span class="sxs-lookup"><span data-stu-id="c74a2-133">**For information about**</span></span>   |<span data-ttu-id="c74a2-134">**Bunu okuyun**</span><span class="sxs-lookup"><span data-stu-id="c74a2-134">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="c74a2-135">Müşterileriniz için Azure ayırmaları belgeleri</span><span class="sxs-lookup"><span data-stu-id="c74a2-135">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="c74a2-136">Azure rezervasyonları nedir?</span><span class="sxs-lookup"><span data-stu-id="c74a2-136">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="c74a2-137">Iş Ortağı Merkezi 'nde müşterileriniz için Azure ayırmaları satın alma</span><span class="sxs-lookup"><span data-stu-id="c74a2-137">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="c74a2-138">Azure ayırmaları satın alma</span><span class="sxs-lookup"><span data-stu-id="c74a2-138">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="c74a2-139">Azure ayırmalarını Iş Ortağı Merkezi 'nde yönetme</span><span class="sxs-lookup"><span data-stu-id="c74a2-139">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="c74a2-140">Azure ayırmalarını Iş Ortağı Merkezi 'nde yönetme</span><span class="sxs-lookup"><span data-stu-id="c74a2-140">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="c74a2-141">Doğru VM boyutunu belirleme ve müşteri VM kullanımını doğrulama</span><span class="sxs-lookup"><span data-stu-id="c74a2-141">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="c74a2-142">Maksimum Azure ayırma kullanımı için VM boyutu</span><span class="sxs-lookup"><span data-stu-id="c74a2-142">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="c74a2-143">Iş Ortağı Merkezi API 'sini kullanarak Azure ayırmaları satın alma</span><span class="sxs-lookup"><span data-stu-id="c74a2-143">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="c74a2-144">[Azure ayrılmış VM örneklerini](/partner-center/develop/purchase-azure-reservations) Iş Ortağı Merkezi geliştirici belgelerinde satın alma</span><span class="sxs-lookup"><span data-stu-id="c74a2-144">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="c74a2-145">Kullanıcılara CSP aboneliğinizden kendi Azure ayırmalarını satın alma izni verme.</span><span class="sxs-lookup"><span data-stu-id="c74a2-145">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="c74a2-146">Müşterilere kendi Azure ayırmalarını satın alma izni verin</span><span class="sxs-lookup"><span data-stu-id="c74a2-146">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |