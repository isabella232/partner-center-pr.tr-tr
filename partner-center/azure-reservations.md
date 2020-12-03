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
ms.openlocfilehash: 9dc92685503fd4b9b05e40337f72e810c1693779
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534905"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="a5cea-104">Iş Ortağı Merkezi, Azure portal veya API 'Leri kullanarak müşterilere Microsoft Azure ayırmaları satma</span><span class="sxs-lookup"><span data-stu-id="a5cea-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="a5cea-105">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="a5cea-105">**Appropriate roles**</span></span>

- <span data-ttu-id="a5cea-106">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="a5cea-106">Admin agent</span></span>
- <span data-ttu-id="a5cea-107">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="a5cea-107">Global admin</span></span>
- <span data-ttu-id="a5cea-108">Yardım Masası Aracısı</span><span class="sxs-lookup"><span data-stu-id="a5cea-108">Helpdesk agent</span></span>
- <span data-ttu-id="a5cea-109">Satış Aracısı</span><span class="sxs-lookup"><span data-stu-id="a5cea-109">Sales agent</span></span>
- <span data-ttu-id="a5cea-110">Kullanıcı Yönetimi Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="a5cea-110">User management admin</span></span>

<span data-ttu-id="a5cea-111">Bulut çözümü sağlayıcısı programı 'nda (CSP) bir iş ortağı olarak müşteriler için Azure ayırmaları satın alabilir, sattabilir veya yönetebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a5cea-111">As a partner in the Cloud Solution Provider program (CSP), you can buy, sell, or manage Azure reservations for customers.</span></span> <span data-ttu-id="a5cea-112">Iş Ortağı Merkezi, Azure portal veya Iş Ortağı Merkezi API 'sini kullanın.</span><span class="sxs-lookup"><span data-stu-id="a5cea-112">Use Partner Center, the Azure portal, or the Partner Center API.</span></span>

> [!NOTE]
> <span data-ttu-id="a5cea-113">Bu makale yalnızca CSP 'deki iş ortakları için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="a5cea-113">This article applies only to partners in CSP.</span></span> <span data-ttu-id="a5cea-114">Diğer abonelik türleri (örneğin, Kullandıkça öde, bireysel, Microsoft Müşteri Sözleşmesi veya Kurumsal Anlaşma abonelikleri) kullanan müşteriler [Bu Azure ayırmaları belgelerini](/azure/cost-management-billing/reservations)okumalı olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="a5cea-114">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="a5cea-115">CSP programındaki iş ortakları, müşterilerine Microsoft Azure ayırmaları sunabilir.</span><span class="sxs-lookup"><span data-stu-id="a5cea-115">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="a5cea-116">Müşteriler, önceden ayrıldıklarında önemli tasarruf elde edebilirler.</span><span class="sxs-lookup"><span data-stu-id="a5cea-116">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="a5cea-117">Azure ayırmaları, müşterileri basitliği ve esnekliği aşağıdaki yollarla sunmaktadır:</span><span class="sxs-lookup"><span data-stu-id="a5cea-117">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="a5cea-118">Bir veya üç yıllık rezervasyon terimi</span><span class="sxs-lookup"><span data-stu-id="a5cea-118">One or three-year reservation terms</span></span>
- <span data-ttu-id="a5cea-119">Kullanmaya başlamak kolaydır; Kurulum saniye cinsinden tamamlandı</span><span class="sxs-lookup"><span data-stu-id="a5cea-119">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="a5cea-120">Ayarlanmış para iadesi için dilediğiniz zaman ayrılan örnekleri iptal edin veya değiştirin</span><span class="sxs-lookup"><span data-stu-id="a5cea-120">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="a5cea-121">Ayrılmış örnek kullanımını kurumsal veya ayrı departman düzeyinde yönetme</span><span class="sxs-lookup"><span data-stu-id="a5cea-121">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="a5cea-122">Azure ayırmaları, müşterilere aşağıdaki yollarla yol açabilir:</span><span class="sxs-lookup"><span data-stu-id="a5cea-122">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="a5cea-123">Rezervasyonlar, Kullandıkça Öde (PAYG) fiyatlandırmasına göre önemli tasarruf sağlayabilir</span><span class="sxs-lookup"><span data-stu-id="a5cea-123">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="a5cea-124">Tek yıllık veya üç yıllık şartlar için ön ödeme ile daha iyi bütçeleme ve tahmin</span><span class="sxs-lookup"><span data-stu-id="a5cea-124">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="a5cea-125">Azure bölgesinde ofislerine en yakın önceliğe sahip bilgi işlem kapasitesi</span><span class="sxs-lookup"><span data-stu-id="a5cea-125">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="a5cea-126">Azure ayırmaları, Microsoft Windows Server ve Azure SQL veritabanı gibi yazılımlarla birleştirildiğinde uçtan uca altyapı çözümlerine yönelik temel sağlar</span><span class="sxs-lookup"><span data-stu-id="a5cea-126">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="a5cea-127">Azure ayırmalarını hem Iş ortağı merkezi hem de Azure portal satın alabilir, satın alabilir ve yönetebilirsiniz ve Iş Ortağı Merkezi API 'sini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a5cea-127">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="a5cea-128">Müşterilerinize satın almış olduğunuz bir Azure aboneliğinden kendi Azure ayırmalarını satın alma izni verebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a5cea-128">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="a5cea-129">Hakkında bilgi edinmek için aşağıdaki bağlantıları izleyin.</span><span class="sxs-lookup"><span data-stu-id="a5cea-129">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="a5cea-130">Azure ayırmaları kaynakları</span><span class="sxs-lookup"><span data-stu-id="a5cea-130">Azure reservations resources</span></span>

|<span data-ttu-id="a5cea-131">**Hakkında bilgi için**</span><span class="sxs-lookup"><span data-stu-id="a5cea-131">**For information about**</span></span>   |<span data-ttu-id="a5cea-132">**Bunu okuyun**</span><span class="sxs-lookup"><span data-stu-id="a5cea-132">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="a5cea-133">Müşterileriniz için Azure ayırmaları belgeleri</span><span class="sxs-lookup"><span data-stu-id="a5cea-133">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="a5cea-134">Azure rezervasyonları nedir?</span><span class="sxs-lookup"><span data-stu-id="a5cea-134">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="a5cea-135">Iş Ortağı Merkezi 'nde müşterileriniz için Azure ayırmaları satın alma</span><span class="sxs-lookup"><span data-stu-id="a5cea-135">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="a5cea-136">Azure ayırmaları satın alma</span><span class="sxs-lookup"><span data-stu-id="a5cea-136">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="a5cea-137">Azure ayırmalarını Iş Ortağı Merkezi 'nde yönetme</span><span class="sxs-lookup"><span data-stu-id="a5cea-137">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="a5cea-138">Azure ayırmalarını Iş Ortağı Merkezi 'nde yönetme</span><span class="sxs-lookup"><span data-stu-id="a5cea-138">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="a5cea-139">Doğru VM boyutunu belirleme ve müşteri VM kullanımını doğrulama</span><span class="sxs-lookup"><span data-stu-id="a5cea-139">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="a5cea-140">Maksimum Azure ayırma kullanımı için VM boyutu</span><span class="sxs-lookup"><span data-stu-id="a5cea-140">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="a5cea-141">Iş Ortağı Merkezi API 'sini kullanarak Azure ayırmaları satın alma</span><span class="sxs-lookup"><span data-stu-id="a5cea-141">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="a5cea-142">[Azure ayrılmış VM örneklerini](/partner-center/develop/purchase-azure-reservations) Iş Ortağı Merkezi geliştirici belgelerinde satın alma</span><span class="sxs-lookup"><span data-stu-id="a5cea-142">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="a5cea-143">Kullanıcılara CSP aboneliğinizden kendi Azure ayırmalarını satın alma izni verme.</span><span class="sxs-lookup"><span data-stu-id="a5cea-143">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="a5cea-144">Müşterilere kendi Azure ayırmalarını satın alma izni verin</span><span class="sxs-lookup"><span data-stu-id="a5cea-144">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |