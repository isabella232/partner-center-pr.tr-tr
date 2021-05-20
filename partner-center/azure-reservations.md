---
title: Müşterilere rezervasyon Microsoft Azure satış
description: Bir Bulut Çözümü Sağlayıcısı olarak, müşteriler için Azure rezervasyonları satın alabilir, satabilirsiniz veya yönetabilirsiniz. İş Ortağı Merkezi, Azure portal API'sini veya İş Ortağı Merkezi kullanın.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: b97cafea9ad2f36718418c7c7cfca5f91ee8849c
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149477"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="b4c5d-104">Microsoft Azure, Azure portal VEYA API'leri kullanarak müşterilere İş Ortağı Merkezi rezervasyonları satma</span><span class="sxs-lookup"><span data-stu-id="b4c5d-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="b4c5d-105">**Uygun roller:** Yönetici aracısı | Genel yönetici | Yardım masası aracısı | Satış aracısı | Kullanıcı yönetimi yöneticisi</span><span class="sxs-lookup"><span data-stu-id="b4c5d-105">**Appropriate roles**: Admin agent | Global admin | Helpdesk agent | Sales agent | User management admin</span></span>

<span data-ttu-id="b4c5d-106">Bulut Çözümü Sağlayıcısı programı (CSP) iş ortağı olarak müşteriler için Azure rezervasyonlarını satın alabilir, satabilirsiniz veya yönetabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b4c5d-106">As a partner in the Cloud Solution Provider program (CSP), you can buy, sell, or manage Azure reservations for customers.</span></span> <span data-ttu-id="b4c5d-107">İş Ortağı Merkezi, Azure portal API'sini veya İş Ortağı Merkezi kullanın.</span><span class="sxs-lookup"><span data-stu-id="b4c5d-107">Use Partner Center, the Azure portal, or the Partner Center API.</span></span>

> [!NOTE]
> <span data-ttu-id="b4c5d-108">Bu makale yalnızca CSP'de iş ortakları için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="b4c5d-108">This article applies only to partners in CSP.</span></span> <span data-ttu-id="b4c5d-109">Diğer abonelik türlerini (kullansanız öde, bireysel, Microsoft Müşteri Sözleşmesi veya Kurumsal Anlaşma abonelikler gibi) kullanan müşterilerin bu Azure rezervasyonları belgelerini [okuması gerekir.](/azure/cost-management-billing/reservations)</span><span class="sxs-lookup"><span data-stu-id="b4c5d-109">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="b4c5d-110">CSP programı iş ortakları, müşterilerine farklı rezervasyonlar Microsoft Azure sunabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b4c5d-110">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="b4c5d-111">Müşteriler önceden rezervasyonları yapılana kadar önemli tasarruflar elde eder.</span><span class="sxs-lookup"><span data-stu-id="b4c5d-111">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="b4c5d-112">Azure rezervasyonları müşterilere aşağıdaki yollarla kolaylık ve esneklik sunar:</span><span class="sxs-lookup"><span data-stu-id="b4c5d-112">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="b4c5d-113">Bir veya üç yıllık rezervasyon koşulları</span><span class="sxs-lookup"><span data-stu-id="b4c5d-113">One or three-year reservation terms</span></span>
- <span data-ttu-id="b4c5d-114">Kolayca çalışmaya başlama; kurulum saniyeler içinde tamamlandı</span><span class="sxs-lookup"><span data-stu-id="b4c5d-114">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="b4c5d-115">Ayarlanmış para iadesi için ayrılmış örnekleri istediğiniz zaman iptal etme veya değiştirme</span><span class="sxs-lookup"><span data-stu-id="b4c5d-115">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="b4c5d-116">Ayrılmış örnek kullanımını kuruluş veya bireysel departman düzeyinde yönetme</span><span class="sxs-lookup"><span data-stu-id="b4c5d-116">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="b4c5d-117">Azure rezervasyonları aşağıdaki yollarla müşterilere hitap eder:</span><span class="sxs-lookup"><span data-stu-id="b4c5d-117">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="b4c5d-118">Rezervasyonlar, öde (PAYG) fiyatlandırması üzerinden önemli tasarruflar sun olabilir</span><span class="sxs-lookup"><span data-stu-id="b4c5d-118">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="b4c5d-119">Bir yıllık veya üç yıllık dönemler için peşin ödeme ile daha iyi bütçe ve tahmin</span><span class="sxs-lookup"><span data-stu-id="b4c5d-119">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="b4c5d-120">Ofislerine en yakın Azure bölgesinde öncelikli bilgi işlem kapasitesi</span><span class="sxs-lookup"><span data-stu-id="b4c5d-120">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="b4c5d-121">Azure ayırmaları, Microsoft Windows Server ve Azure SQL veritabanı gibi yazılımlarla birleştirildiğinde uçtan uca altyapı çözümlerine yönelik temel sağlar</span><span class="sxs-lookup"><span data-stu-id="b4c5d-121">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="b4c5d-122">Azure ayırmalarını hem Iş ortağı merkezi hem de Azure portal satın alabilir, satın alabilir ve yönetebilirsiniz ve Iş Ortağı Merkezi API 'sini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b4c5d-122">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="b4c5d-123">Müşterilerinize satın almış olduğunuz bir Azure aboneliğinden kendi Azure ayırmalarını satın alma izni verebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b4c5d-123">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="b4c5d-124">Hakkında bilgi edinmek için aşağıdaki bağlantıları izleyin.</span><span class="sxs-lookup"><span data-stu-id="b4c5d-124">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="b4c5d-125">Azure ayırmaları kaynakları</span><span class="sxs-lookup"><span data-stu-id="b4c5d-125">Azure reservations resources</span></span>

|<span data-ttu-id="b4c5d-126">**Hakkında bilgi için**</span><span class="sxs-lookup"><span data-stu-id="b4c5d-126">**For information about**</span></span>   |<span data-ttu-id="b4c5d-127">**Bunu okuyun**</span><span class="sxs-lookup"><span data-stu-id="b4c5d-127">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="b4c5d-128">Müşterileriniz için Azure ayırmaları belgeleri</span><span class="sxs-lookup"><span data-stu-id="b4c5d-128">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="b4c5d-129">Azure rezervasyonları nedir?</span><span class="sxs-lookup"><span data-stu-id="b4c5d-129">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="b4c5d-130">Iş Ortağı Merkezi 'nde müşterileriniz için Azure ayırmaları satın alma</span><span class="sxs-lookup"><span data-stu-id="b4c5d-130">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="b4c5d-131">Azure ayırmaları satın alma</span><span class="sxs-lookup"><span data-stu-id="b4c5d-131">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="b4c5d-132">Azure ayırmalarını Iş Ortağı Merkezi 'nde yönetme</span><span class="sxs-lookup"><span data-stu-id="b4c5d-132">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="b4c5d-133">Azure ayırmalarını Iş Ortağı Merkezi 'nde yönetme</span><span class="sxs-lookup"><span data-stu-id="b4c5d-133">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="b4c5d-134">Doğru VM boyutunu belirleme ve müşteri VM kullanımını doğrulama</span><span class="sxs-lookup"><span data-stu-id="b4c5d-134">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="b4c5d-135">Maksimum Azure ayırma kullanımı için VM boyutu</span><span class="sxs-lookup"><span data-stu-id="b4c5d-135">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="b4c5d-136">Iş Ortağı Merkezi API 'sini kullanarak Azure ayırmaları satın alma</span><span class="sxs-lookup"><span data-stu-id="b4c5d-136">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="b4c5d-137">[Azure ayrılmış VM örneklerini](/partner-center/develop/purchase-azure-reservations) Iş Ortağı Merkezi geliştirici belgelerinde satın alma</span><span class="sxs-lookup"><span data-stu-id="b4c5d-137">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="b4c5d-138">Kullanıcılara CSP aboneliğinizden kendi Azure ayırmalarını satın alma izni verme.</span><span class="sxs-lookup"><span data-stu-id="b4c5d-138">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="b4c5d-139">Müşterilere kendi Azure ayırmalarını satın alma izni verin</span><span class="sxs-lookup"><span data-stu-id="b4c5d-139">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |