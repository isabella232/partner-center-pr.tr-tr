---
title: İş Ortağı Merkezi öngörüleri
description: Bu Iş Ortağı Merkezi Birleşik raporlama panosunu gezin. Satış ve dağıtım için KPI 'ler, müşteri geliştirme ve daha fazlasını öğrenin.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/26/2020
ms.openlocfilehash: ba8389ff613b47b17b87a6769674e33948fdc37d
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/31/2021
ms.locfileid: "106086592"
---
# <a name="partner-center-insights---a-dashboard-that-shows-how-a-microsoft-commercial-partner-is-doing"></a><span data-ttu-id="5e8d6-104">İş Ortağı Merkezi öngörüleri-bir Microsoft ticari iş ortağının nasıl yaptığını gösteren bir pano</span><span class="sxs-lookup"><span data-stu-id="5e8d6-104">Partner Center Insights - a dashboard that shows how a Microsoft commercial partner is doing</span></span>

<span data-ttu-id="5e8d6-105">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="5e8d6-105">**Appropriate roles**</span></span>

- <span data-ttu-id="5e8d6-106">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="5e8d6-106">Global admin</span></span>
- <span data-ttu-id="5e8d6-107">Hesap yöneticisi</span><span class="sxs-lookup"><span data-stu-id="5e8d6-107">Account admin</span></span>
- <span data-ttu-id="5e8d6-108">Executive rapor Görüntüleyicisi</span><span class="sxs-lookup"><span data-stu-id="5e8d6-108">Executive report viewer</span></span>
- <span data-ttu-id="5e8d6-109">Rapor Görüntüleyicisi</span><span class="sxs-lookup"><span data-stu-id="5e8d6-109">Report viewer</span></span>

## <a name="introduction"></a><span data-ttu-id="5e8d6-110">Giriş</span><span class="sxs-lookup"><span data-stu-id="5e8d6-110">Introduction</span></span>

<span data-ttu-id="5e8d6-111">Öngörüler panosu, Microsoft 'un Microsoft İş Ortağı Ağı (MPN) programına kayıtlı ticari iş ortakları için Iş Ortağı Merkezi 'nde birleştirilmiş bir raporlama panodur.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-111">The Insights dashboard is a unified reporting dashboard in Partner Center for Microsoft’s Commercial partners who are enrolled in the Microsoft Partner Network (MPN) program.</span></span> <span data-ttu-id="5e8d6-112">Öngörüler panosu, Office, Azure, Dynamics ve CSP ve EA gibi lisanslama modelleri gibi bulut ürünlerinde önemli performans göstergelerinin (KPI) 360 derece görünümünü sağlar.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-112">The Insights dashboard provides 360-degree view of your key performance indicators (KPI) across Cloud products such as Office, Azure, Dynamics, and licensing models such as CSP and EA.</span></span> <span data-ttu-id="5e8d6-113">Kuruluşunuz için veri odaklı kararlar almanıza yardımcı olabilecek zengin bir KPI raporu kümesi sunar.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-113">It exposes a rich set of KPI reports that can help you make data driven decisions for your organization.</span></span> 

## <a name="role-based-access-control-to-the-insights-dashboard"></a><span data-ttu-id="5e8d6-114">Öngörüler panosuna rol tabanlı erişim denetimi</span><span class="sxs-lookup"><span data-stu-id="5e8d6-114">Role-based access control to the Insights dashboard</span></span>

<span data-ttu-id="5e8d6-115">Iş Ortağı Merkezi 'nde öngörülere erişim için özel olarak tasarlanan iki yeni rol vardır: **rapor Görüntüleyicisi** ve **Executive rapor Görüntüleyicisi**.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-115">There are two new roles in Partner Center designed specifically for access to Insights: **Report Viewer** and **Executive Report Viewer**.</span></span> <span data-ttu-id="5e8d6-116">Yönetim rapor Görüntüleyicisi rolündeki kullanıcıların tüm raporlama veri kümelerine erişimi vardır, ancak rapor Görüntüleyicisi rolündeki kullanıcılar gelir ve müşteri/çalışan kişisel verileri gibi hassas veri kümelerine erişemez.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-116">Users in the Executive Report Viewer role have access to all reporting data sets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span> 

<span data-ttu-id="5e8d6-117">Genel yönetici veya hesap yöneticisi, kullanıcılara bu rolleri atayabilir ve tüm şirket veya belirli bir MPN konumu için atanır.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-117">The Global admin or the Account admin can assign users these roles and are assigned either for the entire company or for a specific MPN location.</span></span>  

>[!Note] 
><span data-ttu-id="5e8d6-118">20 Ocak 2020 itibariyle MPN yönetici olan kullanıcılar, şirket genelinde rapor Görüntüleyicisi rolüne otomatik olarak eklenmiştir.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-118">Users who were MPN admins as of Jan 20th, 2020 were automatically added to the company-wide report viewer role.</span></span> <span data-ttu-id="5e8d6-119">Genel yönetici veya hesap yöneticisi için gereken açık bir eylem olmadan raporlara rapor Görüntüleyicisi olarak erişebilirler. Gerekirse, genel Yöneticiler veya hesap yöneticisi bu atamaları geçersiz kılabilir.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-119">They are able to access the reports as a report viewer without any explicit action required by Global admin or Account admin. The Global admins or account admin can override these assignments if necessary.</span></span> 

## <a name="reports-available"></a><span data-ttu-id="5e8d6-120">Kullanılabilir raporlar</span><span class="sxs-lookup"><span data-stu-id="5e8d6-120">Reports available</span></span>

<span data-ttu-id="5e8d6-121">Aşağıdaki raporlar, Öngörüler panosu 'nun bir parçası olarak sunulmaktadır.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-121">The following reports are available as part of the Insights dashboard.</span></span>

<span data-ttu-id="5e8d6-122">**Genel bakış**: genel bakış raporu, size müşteri sayısı, etkin abonelik sayısı, Azure tüketim geliri, etkin lisanslar vb. gibi çeşitli KPI 'lerin bir anlık görüntü görünümünü sunar.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-122">**Overview**: The Overview report presents a snapshot view of various KPIs of interest to you such as Customer count, Active Subscriptions count, Azure Consumption Revenue, Active licenses etc.</span></span>

<span data-ttu-id="5e8d6-123">**Müşteri**: müşteri raporu, müşterilerinizin etrafında müşteri Alım verileri, etkin müşteriler vb. gibi analizler sunar.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-123">**Customer**: The Customer report presents analytics around your customers such as Customer acquisition data, Active customers, etc.</span></span>

<span data-ttu-id="5e8d6-124">**Ürün-abonelikler**: abonelikler raporu, bulut abonelikleriniz için alım ve kullanım analizlerini (O365, Azure, Dynamics vb.) sunar</span><span class="sxs-lookup"><span data-stu-id="5e8d6-124">**Product - Subscriptions**: The Subscriptions report presents acquisition and usage analytics for your Cloud subscriptions (such as O365, Azure, Dynamics etc.)</span></span>

<span data-ttu-id="5e8d6-125">**Ürün lisansları**: lisanslar panosu, O365, Dynamics, Power BI vb. gibi lisans tabanlı bulut ürünleri için lisans analizi sunar.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-125">**Product- Licenses**: The Licenses dashboard presents license analytics for license-based Cloud products such as O365, Dynamics, Power BI etc.</span></span>

<span data-ttu-id="5e8d6-126">**Ürün-Azure kullanımı**: Azure kullanım raporu, Azure tüketim geliri ve ölçüm kategorilerine göre kullanım dahil olmak üzere müşterilerinizin Azure abonelikleri ile ilgili ölçümleri sunar.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-126">**Product - Azure usage**: The Azure Usage report presents metrics related to your customers’ Azure subscriptions including Azure consumption revenue and usage by meter categories.</span></span>

<span data-ttu-id="5e8d6-127">**Uzmanlıklar**: Uzmanlıklar raporu, etkin, nitelikli ve risk altındaki uzmanlarınız hakkında ölçümler sunar.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-127">**Competencies**: The Competencies report presents metrics on your Active, Qualified, and At-risk competencies.</span></span>

<span data-ttu-id="5e8d6-128">**Avantajlar**: avantajlar raporu, kazanılan ve tüketilen iş ortağı avantajları hakkında analizler sunar.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-128">**Benefits**: The Benefits report presents analytics on partner benefits you have earned vs consumed.</span></span>

## <a name="navigating-the-insights-reports"></a><span data-ttu-id="5e8d6-129">Öngörüler raporlarında gezinme</span><span class="sxs-lookup"><span data-stu-id="5e8d6-129">Navigating the Insights reports</span></span>

<span data-ttu-id="5e8d6-130">**Tarih aralığı filtreleri**: her sayfanın sağ üst köşesinde bir tarih aralığı seçimi bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-130">**Date range filters**: You can find a date range selection at the top-right corner of each page.</span></span> <span data-ttu-id="5e8d6-131">Genel Bakış sayfası grafiklerinin çıktısı, son 3, 6 veya 12 aya göre veya özel bir tarih aralığı seçilerek bir tarih aralığı seçilerek özelleştirilebilir.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-131">The output of the overview page graphs can be customized by selecting a date range based on the past 3, 6, or 12 months, or by selecting a custom date range.</span></span> <span data-ttu-id="5e8d6-132">Varsayılan tarih aralığı seçimi 12 aydır.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-132">The default date range selection is 12 months.</span></span> 

:::image type="content" source="images/pci/intro1.png" alt-text="Giriş Haritası":::

<span data-ttu-id="5e8d6-134">**Geri bildirim düğmesi**: tüm Öngörüler raporlarında her bir grafik/denetim, bir rapor özelliğinde örnek geri bildirim sağlamanıza olanak sağlamak için bir geri bildirim düğmesi ile birleştirilir.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-134">**Feedback button**: Each chart/control in all the Insights reports is incorporated with a feedback button to let you provide instance feedback on a report feature.</span></span> 

 
<span data-ttu-id="5e8d6-135">**Sayfa düzeyi filtreleri**: genel bakış, avantajlar ve uzmanlık raporlarının dışında, tüm Öngörüler raporları sayfa düzeyi filtreleri uygulamanıza olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-135">**Page level filters**: Except for the Overview, Benefits, and Competencies reports, all Insights reports enable you to apply page level filters.</span></span> 

- <span data-ttu-id="5e8d6-136">Seçilen filtreler, Özet bölümü dahil olmak üzere bir sayfadaki tüm grafikler ve ölçümler için geçerli olacaktır.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-136">The filters selected will be applicable for all charts and metrics on a page, including the summary section.</span></span> <span data-ttu-id="5e8d6-137">Filtre ölçütlerinde herhangi bir veriniz varsa, bir filtre öğesi kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-137">A filter item will be available if you have any data within that filter criteria.</span></span> 

- <span data-ttu-id="5e8d6-138">Her bir filtre listesinin varsayılan seçimi **hepsi**'dir.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-138">Default selection of each filter list is **all**.</span></span> <span data-ttu-id="5e8d6-139">Örneğin, ürünler filtresinde belirli bir ürünü seçmediyseniz, varsayılan seçim tüm ürünler olacaktır.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-139">For example, if you have not selected a specific product in products filter, default selection will be all products.</span></span>

- <span data-ttu-id="5e8d6-140">Seçilen filtreler sayfanın üstünde görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-140">Filters selected will be displayed at the top of the page.</span></span> 

:::image type="content" source="images/pci/filters.png" alt-text="Uygulanan filtreler çubuğunu ürünlerin, müşteri pazarlarının, Iş ortağı attribuve satış kanallarının filtre seçimleriyle gösteren kısmi ekran görüntüsü.":::

### <a name="filters-definitions"></a><span data-ttu-id="5e8d6-142">Filtre tanımları:</span><span class="sxs-lookup"><span data-stu-id="5e8d6-142">Filters definitions:</span></span>

- <span data-ttu-id="5e8d6-143">Ürünler: kuruluşunuz tarafından satılan/yönetilen tüm Microsoft Bulut ürünlerin listesi (örneğin, O365, Azure, D365, EMS, Power BI vb.).</span><span class="sxs-lookup"><span data-stu-id="5e8d6-143">Products: List of all Microsoft Cloud products sold/managed by your organization, for example,  O365, Azure, D365, EMS, Power BI, etc.</span></span>
- <span data-ttu-id="5e8d6-144">Müşteri pazarları: müşteri ülkelerin listesi</span><span class="sxs-lookup"><span data-stu-id="5e8d6-144">Customer markets: List of customer countries</span></span>
- <span data-ttu-id="5e8d6-145">İş ortağı attribu, örneğin dijital kayıt iş ortağı (DPOR), yönetici temsilcisi ayrıcalığı (DAP) ve Iş ortağı yönetici bağlantısı (PAL) gibi müşterilerinizin abonelikleriyle birlikte ilişki türüdür.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-145">Partner attributions: Your association type with your customers' subscriptions, for example, Digital partner of record (DPOR), Delegated admin privilege (DAP), and Partner Admin link (PAL).</span></span> 
- <span data-ttu-id="5e8d6-146">İş ortağı konumları: tüm kuruluşunuzun MPN konumlarının listesi.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-146">Partner locations: List of all your organization’s MPN locations.</span></span>
- <span data-ttu-id="5e8d6-147">Satış Kanalları: CSP, EA, CSP dolaylı, doğrudan, danışman, açık, diğerleri için satın alma/sağlama yaptığınız tüm satış kanalı/fiyatlandırma</span><span class="sxs-lookup"><span data-stu-id="5e8d6-147">Sales channels: All sales channel/pricing through which you are purchasing/provisioning products and services namely CSP, EA, CSP indirect, Direct, Advisor, Open, others</span></span>
- <span data-ttu-id="5e8d6-148">Müşteri segmentleri: iş ortakları müşteri tabanı genelinde Müşteri segmentlerinin listesi.</span><span class="sxs-lookup"><span data-stu-id="5e8d6-148">Customer segments: List of customer segments across the partners customer base.</span></span>

## <a name="read-about-each-of-the-dashboards-and-reports"></a><span data-ttu-id="5e8d6-149">Panolar ve raporlardan her biri hakkında bilgi edinin:</span><span class="sxs-lookup"><span data-stu-id="5e8d6-149">Read about each of the dashboards and reports:</span></span>

- [<span data-ttu-id="5e8d6-150">İş Ortağı Merkezi öngörüleri-Genel Bakış Panosu</span><span class="sxs-lookup"><span data-stu-id="5e8d6-150">Partner Center Insights - Overview dashboard</span></span>](pci-overview-report.md)

- [<span data-ttu-id="5e8d6-151">İş Ortağı Merkezi öngörüleri-müşteri panosu</span><span class="sxs-lookup"><span data-stu-id="5e8d6-151">Partner Center Insights - Customer dashboard</span></span>](pci-customer-report.md)

- [<span data-ttu-id="5e8d6-152">İş Ortağı Merkezi öngörüleri-abonelikler raporu</span><span class="sxs-lookup"><span data-stu-id="5e8d6-152">Partner Center Insights - Subscriptions report</span></span>](pci-product-subscriptions-report.md)

- [<span data-ttu-id="5e8d6-153">İş Ortağı Merkezi öngörüleri-lisanslar raporu</span><span class="sxs-lookup"><span data-stu-id="5e8d6-153">Partner Center Insights - Licenses report</span></span>](pci-product-licenses-report.md)

- [<span data-ttu-id="5e8d6-154">İş Ortağı Merkezi öngörüleri-Azure kullanım raporu</span><span class="sxs-lookup"><span data-stu-id="5e8d6-154">Partner Center Insights - Azure usage report</span></span>](pci-azure-usage-report.md)

- [<span data-ttu-id="5e8d6-155">İş Ortağı Merkezi öngörüleri-Ylilikler raporu</span><span class="sxs-lookup"><span data-stu-id="5e8d6-155">Partner Center Insights - Competencies report</span></span>](pci-competencies-report.md)

- [<span data-ttu-id="5e8d6-156">İş Ortağı Merkezi öngörüleri-avantajlar raporu</span><span class="sxs-lookup"><span data-stu-id="5e8d6-156">Partner Center Insights - Benefits report</span></span>](pci-benefits-report.md)
