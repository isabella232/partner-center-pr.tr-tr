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
ms.openlocfilehash: 980c086a2ab1ee0a21592ceb1e2e018c0e1159ae
ms.sourcegitcommit: bcd0c09d3acd5eae4fbfca7ea6614a54d203eff6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/04/2020
ms.locfileid: "92531395"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a><span data-ttu-id="26398-104">Iş Ortağı Merkezi Öngörüler panosuna rol tabanlı erişim denetimi</span><span class="sxs-lookup"><span data-stu-id="26398-104">Role-based access control to the Partner Center Insights dashboard</span></span>

<span data-ttu-id="26398-105">Öngörüler panosu, çalışanların raporlar-Executive rapor görüntüleyicisine ve rapor görüntüleyicisine erişimini yönetmek için Iş Ortağı Merkezi 'nde iki yeni rol kullanır.</span><span class="sxs-lookup"><span data-stu-id="26398-105">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="26398-106">Yönetim rapor Görüntüleyicisi rolündeki kullanıcıların tüm raporlama veri kümelerine erişimi vardır, ancak rapor Görüntüleyicisi rolündeki kullanıcıların gelir ve müşteri/çalışan kişisel verileri gibi hassas veri kümelerine erişimi olmayacaktır.</span><span class="sxs-lookup"><span data-stu-id="26398-106">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="26398-107">Diğer Iş Ortağı Merkezi rollerinde olduğu gibi, genel yönetici veya hesap yöneticisi Kullanıcı Yönetimi sayfasında bu rollere Kullanıcı atayacaktır.</span><span class="sxs-lookup"><span data-stu-id="26398-107">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="26398-108">Roller tüm şirket genelinde veya belirli MPN konumlarına uygulanabilir.</span><span class="sxs-lookup"><span data-stu-id="26398-108">The roles can be applicable across the entire company or for specific MPN location(s).</span></span> <span data-ttu-id="26398-109">Belirli MPN konumları için atanan roller, kullanıcının yalnızca seçili MPN konumuyla ilişkili raporlama verilerini görüntülemesini kısıtlar.</span><span class="sxs-lookup"><span data-stu-id="26398-109">Roles assigned for specific MPN location(s) limits the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="26398-110">İş ortağı aşağıdaki görünümden bir veya daha fazla konum seçebilir.</span><span class="sxs-lookup"><span data-stu-id="26398-110">Partner can select one or multiple locations from the below view.</span></span>

:::image type="content" source="images/pci/roles.png" alt-text="Rapor Görüntüleyicisi ve Executive rapor Görüntüleyicisi için konuma özgü Iş Ortağı Merkezi Öngörüler rol ayarlarını gösterir.":::

>[!Note]
> <span data-ttu-id="26398-112">18 Ocak 2020 itibariyle MPN yöneticileri olan kullanıcılar, bu kiracının tüm konumları için şirket genelinde **Yönetim rapor Görüntüleyicisi** rolüne otomatik olarak eklenir.</span><span class="sxs-lookup"><span data-stu-id="26398-112">Users who are MPN admins as of Jan 20th, 2020 are automatically added to the company-wide **Executive Report Viewer** role for all locations for that tenant.</span></span> <span data-ttu-id="26398-113">Bu kullanıcılar, genel yönetici veya hesap yöneticisi için gerekli herhangi bir açık eylem olmadan raporlara bir Executive rapor Görüntüleyicisi olarak erişebilirler. Genel Yöneticiler ve hesap yöneticileri bu kullanıcıların yeteneklerini daha fazla artırmak veya sınırlamak için otomatik atanan rolleri geçersiz kılabilir.</span><span class="sxs-lookup"><span data-stu-id="26398-113">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>

## <a name="next-steps"></a><span data-ttu-id="26398-114">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="26398-114">Next steps</span></span>

- <span data-ttu-id="26398-115">[Iş Ortağı Merkezi öngörüleri](partner-center-insights.md) ve çeşitli raporları hakkında daha fazla bilgi edinin.</span><span class="sxs-lookup"><span data-stu-id="26398-115">Learn more about [Partner Center Insights](partner-center-insights.md) and its various reports.</span></span>
