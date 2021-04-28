---
title: İş Ortağı Merkezi öngörüleri rol tabanlı erişim
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Iş Ortağı Merkezi öngörüleri raporlarını görmek için gereken belirli roller hakkında bilgi edinin. Bunlar, Executive rapor Görüntüleyicisi ve rapor görüntüleyicisinin rollerini içerir.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a6af9c7d674d1956332a564628b6b2ea0b1796f6
ms.sourcegitcommit: 078eac1456f68585ff1003b21e5e1fe777af314b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/28/2021
ms.locfileid: "108120792"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a><span data-ttu-id="47068-104">Iş Ortağı Merkezi Öngörüler panosuna rol tabanlı erişim denetimi</span><span class="sxs-lookup"><span data-stu-id="47068-104">Role-based access control to the Partner Center Insights dashboard</span></span>

<span data-ttu-id="47068-105">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="47068-105">**Appropriate roles**</span></span>

- <span data-ttu-id="47068-106">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="47068-106">Global admin</span></span>
- <span data-ttu-id="47068-107">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="47068-107">Admin agent</span></span>
- <span data-ttu-id="47068-108">Rapor Görüntüleyicisi</span><span class="sxs-lookup"><span data-stu-id="47068-108">Report viewer</span></span>
- <span data-ttu-id="47068-109">Executive rapor Görüntüleyicisi</span><span class="sxs-lookup"><span data-stu-id="47068-109">Executive report viewer</span></span>

<span data-ttu-id="47068-110">Öngörüler panosu, çalışanların raporlar-Executive rapor görüntüleyicisine ve rapor görüntüleyicisine erişimini yönetmek için Iş Ortağı Merkezi 'nde iki yeni rol kullanır.</span><span class="sxs-lookup"><span data-stu-id="47068-110">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="47068-111">Yönetim rapor Görüntüleyicisi rolündeki kullanıcıların tüm raporlama veri kümelerine erişimi vardır, ancak rapor Görüntüleyicisi rolündeki kullanıcıların gelir ve müşteri/çalışan kişisel verileri gibi hassas veri kümelerine erişimi olmayacaktır.</span><span class="sxs-lookup"><span data-stu-id="47068-111">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="47068-112">Diğer Iş Ortağı Merkezi rollerinde olduğu gibi, genel yönetici veya hesap yöneticisi Kullanıcı Yönetimi sayfasında bu rollere Kullanıcı atayacaktır.</span><span class="sxs-lookup"><span data-stu-id="47068-112">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="47068-113">Roller tüm şirket genelinde veya belirli MPN konumlarına uygulanabilir.</span><span class="sxs-lookup"><span data-stu-id="47068-113">The roles can be applicable across the entire company or for specific MPN location(s).</span></span> <span data-ttu-id="47068-114">Belirli MPN konumları için atanan roller, kullanıcıyı yalnızca seçili MPN konumuyla ilişkili raporlama verilerini görüntülemeye göre sınırlandırır.</span><span class="sxs-lookup"><span data-stu-id="47068-114">Roles assigned for specific MPN location(s) limit the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="47068-115">İş ortağı aşağıdaki görünümden bir veya daha fazla konum seçebilir.</span><span class="sxs-lookup"><span data-stu-id="47068-115">Partner can select one or multiple locations from the below view.</span></span>

:::image type="content" source="images/pci/roles.png" alt-text="Rapor Görüntüleyicisi ve Executive rapor Görüntüleyicisi için konuma özgü Iş Ortağı Merkezi Öngörüler rol ayarlarını gösterir.":::

>[!Note]
> <span data-ttu-id="47068-117">18 Ocak 2020 itibariyle MPN yöneticileri olan kullanıcılar, bu kiracının tüm konumları için şirket genelinde **Yönetim rapor Görüntüleyicisi** rolüne otomatik olarak eklenir.</span><span class="sxs-lookup"><span data-stu-id="47068-117">Users who are MPN admins as of Jan 20th, 2020 are automatically added to the company-wide **Executive Report Viewer** role for all locations for that tenant.</span></span> <span data-ttu-id="47068-118">Bu kullanıcılar, genel yönetici veya hesap yöneticisi için gerekli herhangi bir açık eylem olmadan raporlara bir Executive rapor Görüntüleyicisi olarak erişebilirler. Genel Yöneticiler ve hesap yöneticileri bu kullanıcıların yeteneklerini daha fazla artırmak veya sınırlamak için otomatik atanan rolleri geçersiz kılabilir.</span><span class="sxs-lookup"><span data-stu-id="47068-118">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>

## <a name="next-steps"></a><span data-ttu-id="47068-119">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="47068-119">Next steps</span></span>

- <span data-ttu-id="47068-120">[Iş Ortağı Merkezi öngörüleri](partner-center-insights.md) ve çeşitli raporları hakkında daha fazla bilgi edinin.</span><span class="sxs-lookup"><span data-stu-id="47068-120">Learn more about [Partner Center Insights](partner-center-insights.md) and its various reports.</span></span>
