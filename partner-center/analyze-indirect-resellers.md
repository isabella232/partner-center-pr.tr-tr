---
title: Dolaylı satıcıların performansını çözümleme
description: Dolaylı satıcılarınızın, hem başarıları hem de daha fazla ilgilenilmesi gerekebilecek alanlarında nasıl çalıştığını öğrenmek için analiz kullanın.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh
ms.author: shganesh
ms.topic: article
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/13/2020
ms.openlocfilehash: 24316148fd237aa1fb466083c742ef4ddec36e22
ms.sourcegitcommit: c40f826bb1143555bf3a1c2c806c34024f0f6019
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/02/2020
ms.locfileid: "92531374"
---
# <a name="use-analytics-to-analyze-performance-of-your-indirect-resellers"></a><span data-ttu-id="0fb10-103">Dolaylı satıcılarınızın performansını analiz etmek için analiz kullanma</span><span class="sxs-lookup"><span data-stu-id="0fb10-103">Use analytics to analyze performance of your indirect resellers</span></span>

<span data-ttu-id="0fb10-104">**Uygulama hedefi**</span><span class="sxs-lookup"><span data-stu-id="0fb10-104">**Applies to**</span></span>

- <span data-ttu-id="0fb10-105">İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="0fb10-105">Partner Center</span></span>
- <span data-ttu-id="0fb10-106">Bulut çözümü sağlayıcısı program iş ortakları</span><span class="sxs-lookup"><span data-stu-id="0fb10-106">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="0fb10-107">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="0fb10-107">**Appropriate roles**</span></span>

- <span data-ttu-id="0fb10-108">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="0fb10-108">Global admin</span></span>
- <span data-ttu-id="0fb10-109">Kullanıcı Yönetimi Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="0fb10-109">User management admin</span></span>
- <span data-ttu-id="0fb10-110">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="0fb10-110">Admin agent</span></span>
- <span data-ttu-id="0fb10-111">Satış Aracısı</span><span class="sxs-lookup"><span data-stu-id="0fb10-111">Sales agent</span></span>

<span data-ttu-id="0fb10-112">Veri sürücüleri iş kararları.</span><span class="sxs-lookup"><span data-stu-id="0fb10-112">Data drives business decisions.</span></span> <span data-ttu-id="0fb10-113">Ortamınızı, dolaylı satıcılarınızın başarıları ve daha fazla ilgilenilmesi gereken bölgeleri belirlemek için **satıcı analizi** sayfasındaki ölçümleri kullanın.</span><span class="sxs-lookup"><span data-stu-id="0fb10-113">Use the metrics in the **Reseller analytics** page to identify your successes, your indirect resellers' successes, and areas that need more attention.</span></span> <span data-ttu-id="0fb10-114">Yeni iş hedeflerini planlarken bu bilgileri kullanın.</span><span class="sxs-lookup"><span data-stu-id="0fb10-114">Use this information as you plan new business goals.</span></span>

> [!NOTE]
> <span data-ttu-id="0fb10-115">Dolaylı satıcılar Analizi yalnızca bulut çözümü sağlayıcısı programındaki iş ortakları için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="0fb10-115">Indirect resellers analytics is available only for partners in the Cloud Solution Provider program.</span></span>

## <a name="types-of-reseller-analytics-metrics-you-can-view"></a><span data-ttu-id="0fb10-116">Görüntüleyebileceğiniz Satıcı Analizi ölçümlerinin türleri</span><span class="sxs-lookup"><span data-stu-id="0fb10-116">Types of reseller analytics metrics you can view</span></span>

<span data-ttu-id="0fb10-117">Aşağıdaki ölçümleri izliyoruz:</span><span class="sxs-lookup"><span data-stu-id="0fb10-117">We are tracking the following metrics:</span></span>

<span data-ttu-id="0fb10-118">**Özet**</span><span class="sxs-lookup"><span data-stu-id="0fb10-118">**Summary**</span></span>  
 - <span data-ttu-id="0fb10-119">**Toplam satıcılar** : aboneliğin son günündeki etkin satıcıların sayısı</span><span class="sxs-lookup"><span data-stu-id="0fb10-119">**Total resellers** : Count of active resellers on the last day of the subscription</span></span>  
 - <span data-ttu-id="0fb10-120">**Yeni satıcılar** : belirtilen dönemin yeni dolaylı satıcıların sayısı</span><span class="sxs-lookup"><span data-stu-id="0fb10-120">**New resellers** : Count of new indirect resellers for the specified time period</span></span>  
 - <span data-ttu-id="0fb10-121">**Etkin satıcılar** : mpnıd 'nin en az 1 abonelik olduğu ve abonelik durumunun sağlanmamış olduğu dolaylı satıcıların sayısı</span><span class="sxs-lookup"><span data-stu-id="0fb10-121">**Active resellers** : Count of indirect resellers where the MPNID is at least 1 subscription, and where the subscription status is not deprovisioned</span></span>  
 - <span data-ttu-id="0fb10-122">**Deneyimidir satıcıları** : belirtilen dönemde satılan bir aboneliğe sahip dolaylı satıcıların sayısı</span><span class="sxs-lookup"><span data-stu-id="0fb10-122">**Transacting resellers** : Count of indirect resellers with a subscription sold in the specified time period</span></span>  

<span data-ttu-id="0fb10-123">**Pazara göre satıcılar**</span><span class="sxs-lookup"><span data-stu-id="0fb10-123">**Resellers by market**</span></span>  
 - <span data-ttu-id="0fb10-124">Coğrafi konuma göre toplam satıcılar</span><span class="sxs-lookup"><span data-stu-id="0fb10-124">Total resellers by geographic location</span></span>  

<span data-ttu-id="0fb10-125">**Satılan aboneliklere göre popüler satıcılar**</span><span class="sxs-lookup"><span data-stu-id="0fb10-125">**Top resellers by subscriptions sold**</span></span>
 - <span data-ttu-id="0fb10-126">Satılan abonelik sayısına göre sıralanan satıcıların bir listesi</span><span class="sxs-lookup"><span data-stu-id="0fb10-126">A list of resellers, sorted by the number of subscriptions they've sold</span></span>  

<span data-ttu-id="0fb10-127">**Abonelik sayısına göre popüler ürünler**</span><span class="sxs-lookup"><span data-stu-id="0fb10-127">**Top products by subscription count**</span></span>  
 - <span data-ttu-id="0fb10-128">**Dynamics 365** : satılan aboneliklere göre sıralanan Dynamics 365 ürünleri</span><span class="sxs-lookup"><span data-stu-id="0fb10-128">**Dynamics 365** : Dynamics 365 products sorted by subscriptions sold</span></span>  
 - <span data-ttu-id="0fb10-129">**EMS** : satılan Kurumsal Yönetim Hizmetleri aboneliklerinin sayısı</span><span class="sxs-lookup"><span data-stu-id="0fb10-129">**EMS** : Number of Enterprise Management Services subscriptions sold</span></span>  
 - <span data-ttu-id="0fb10-130">**Microsoft 365** : satılan Microsoft 365 aboneliklerin sayısı</span><span class="sxs-lookup"><span data-stu-id="0fb10-130">**Microsoft 365** : Number of Microsoft 365 subscriptions sold</span></span>  
 - <span data-ttu-id="0fb10-131">**Office 365** : satılan aboneliklere göre sıralanan Office 365 ürünleri</span><span class="sxs-lookup"><span data-stu-id="0fb10-131">**Office 365** : Office 365 products sorted by subscriptions sold</span></span>  

<span data-ttu-id="0fb10-132">**Yeni abonelikler**</span><span class="sxs-lookup"><span data-stu-id="0fb10-132">**New subscriptions**</span></span>  
 - <span data-ttu-id="0fb10-133">Tarihe göre eklenen yeni aboneliklerin sayısı</span><span class="sxs-lookup"><span data-stu-id="0fb10-133">The number of new subscriptions added by date</span></span>  

<span data-ttu-id="0fb10-134">**Abonelik karmaşıklığı**</span><span class="sxs-lookup"><span data-stu-id="0fb10-134">**Subscription churn**</span></span>  
 - <span data-ttu-id="0fb10-135">**Yeni abonelikler** : tarihe göre eklenen yeni aboneliklerin sayısı</span><span class="sxs-lookup"><span data-stu-id="0fb10-135">**New subscriptions** : Count of new subscriptions added by date</span></span>  
 - <span data-ttu-id="0fb10-136">Sağlaması **kaldırılmış abonelikler** : tarihe göre sağlanan veya askıya alınan abonelik sayısı</span><span class="sxs-lookup"><span data-stu-id="0fb10-136">**Deprovisioned subscriptions** : Count of subscriptions deprovisioned or suspended by date</span></span>  

<span data-ttu-id="0fb10-137">**Yeni satıcı ayrıntıları**</span><span class="sxs-lookup"><span data-stu-id="0fb10-137">**New reseller details**</span></span>  
 - <span data-ttu-id="0fb10-138">**Satıcı adı** : dolaylı satıcıların adları</span><span class="sxs-lookup"><span data-stu-id="0fb10-138">**Reseller name** : Names of indirect resellers</span></span>  
 - <span data-ttu-id="0fb10-139">**Konum** : dolaylı satıcıların çalışacağı pazarlar</span><span class="sxs-lookup"><span data-stu-id="0fb10-139">**Location** : Markets where the indirect resellers operate</span></span>  
 - <span data-ttu-id="0fb10-140">**Abonelikler** : satıcıdan satılan abonelik sayısı</span><span class="sxs-lookup"><span data-stu-id="0fb10-140">**Subscriptions** : Number of subscriptions the reseller has sold</span></span>  
 - <span data-ttu-id="0fb10-141">**Lisanslar** : satıcıdan tüm abonelikler arasında satılan toplam lisans sayısı</span><span class="sxs-lookup"><span data-stu-id="0fb10-141">**Licenses** : Total number of licenses the reseller has sold across all subscriptions</span></span>  

<span data-ttu-id="0fb10-142">**MPA imzalı durumu**</span><span class="sxs-lookup"><span data-stu-id="0fb10-142">**MPA signed status**</span></span>

<span data-ttu-id="0fb10-143">Bu bölüm, CSP dolaylı satıcıların MPA imzalı durumunun durumunu sağlar.</span><span class="sxs-lookup"><span data-stu-id="0fb10-143">This section provides the status of MPA signed status of the CSP Indirect Resellers.</span></span>

 - <span data-ttu-id="0fb10-144">**Satıcı adı** : CSP dolaylı satıcı adı</span><span class="sxs-lookup"><span data-stu-id="0fb10-144">**Reseller name** : Name of the CSP indirect reseller</span></span>
 - <span data-ttu-id="0fb10-145">**MPN kimliği** : dolaylı satıcıdan MPN kimliği</span><span class="sxs-lookup"><span data-stu-id="0fb10-145">**MPN ID** : MPN ID of the indirect reseller</span></span>
 - <span data-ttu-id="0fb10-146">**Bölge** : dolaylı satıcıdan çalışan bölge</span><span class="sxs-lookup"><span data-stu-id="0fb10-146">**Region** : Region where the indirect reseller operates</span></span>
 - <span data-ttu-id="0fb10-147">**MPN vetting durumu** : dolaylı satıcının durumu</span><span class="sxs-lookup"><span data-stu-id="0fb10-147">**MPN vetting status** : Vetting status of the indirect reseller</span></span>
 - <span data-ttu-id="0fb10-148">**MPa imzalı durum** : dolaylı satıcı için MPa imzalama durumu</span><span class="sxs-lookup"><span data-stu-id="0fb10-148">**MPA signed status** : MPA signing status for the indirect reseller</span></span>

<span data-ttu-id="0fb10-149">MPA imzalı durum verilerini ek boyutlarla indirmek için grafikteki indir simgesine tıklayın</span><span class="sxs-lookup"><span data-stu-id="0fb10-149">Click on the download icon in the chart to download MPA signed status data with additional dimensions</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="0fb10-150">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="0fb10-150">Next steps</span></span>

- [<span data-ttu-id="0fb10-151">İş kararlarını sağlamaya yardımcı olmak için abonelikleri ve lisansları çözümleyin</span><span class="sxs-lookup"><span data-stu-id="0fb10-151">Analyze subscriptions and licenses to help drive business decisions</span></span>](analyze-subscriptions-licenses.md)