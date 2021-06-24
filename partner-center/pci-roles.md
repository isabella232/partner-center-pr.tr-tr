---
title: İş Ortağı Merkezi Insights rol tabanlı erişim
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: İş Ortağı Merkezi Insights raporlarını görmek için gereken roller hakkında bilgi edinin. Bunlar, Executive Report Viewer ve Report Viewer rollerini içerir.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: fb06a863218446b0e88b38af242b4dac044560c0
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565313"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a><span data-ttu-id="c8cf0-104">İş Ortağı Merkezi Insights panosuna rol tabanlı erişim denetimi</span><span class="sxs-lookup"><span data-stu-id="c8cf0-104">Role-based access control to the Partner Center Insights dashboard</span></span>

<span data-ttu-id="c8cf0-105">**Uygun roller:** Genel yönetici | Yönetici aracısı | Rapor görüntüleyici | Yönetici raporu görüntüleyicisi</span><span class="sxs-lookup"><span data-stu-id="c8cf0-105">**Appropriate roles**: Global admin | Admin agent | Report viewer | Executive report viewer</span></span>

<span data-ttu-id="c8cf0-106">Öngörüler panosu, raporlara çalışan erişimini İş Ortağı Merkezi için bu panoda iki yeni rol kullanır: Executive Report Viewer ve Report Viewer.</span><span class="sxs-lookup"><span data-stu-id="c8cf0-106">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="c8cf0-107">Yönetici Rapor Görüntüleyicisi rolünde bulunan kullanıcılar tüm raporlama veri kümelerine erişime sahipken Rapor Görüntüleyicisi rolünde bulunan kullanıcılar gelir ve müşteri/çalışan kişisel verileri gibi hassas veri kümelerine erişene sahip olmaz.</span><span class="sxs-lookup"><span data-stu-id="c8cf0-107">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="c8cf0-108">Diğer kullanıcı İş Ortağı Merkezi olduğu gibi, Genel yönetici veya Hesap yöneticisi Kullanıcı yönetimi sayfasında bu rollere kullanıcı atayacaktır.</span><span class="sxs-lookup"><span data-stu-id="c8cf0-108">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="c8cf0-109">Roller, şirketin tamamına veya belirli Microsoft İş Ortağı Ağı (MPN) konumlarına uygulanabilir.</span><span class="sxs-lookup"><span data-stu-id="c8cf0-109">The roles can be applicable across the entire company or for specific Microsoft Partner Network (MPN) location(s).</span></span> <span data-ttu-id="c8cf0-110">Belirli MPN konumları için atanan roller, kullanıcının yalnızca seçili MPN konumlarla ilişkili raporlama verilerini görüntülemesini sağlar.</span><span class="sxs-lookup"><span data-stu-id="c8cf0-110">Roles assigned for specific MPN location(s) limit the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="c8cf0-111">İş ortağı aşağıdaki görünümden bir veya birden çok konum seçin.</span><span class="sxs-lookup"><span data-stu-id="c8cf0-111">Partner can select one or multiple locations from the below view.</span></span>

:::image type="content" source="images/pci/roles.png" alt-text="Rapor görüntüleyicisi ve İş Ortağı Merkezi rapor görüntüleyicisi için Konuma özgü içgörüler rol ayarlarını gösterir.":::

>[!Note]
> <span data-ttu-id="c8cf0-113">20 Ocak 2020 itibariyle MPN iş ortağı yöneticisi olan kullanıcılar, bu  kiracının tüm konumları için şirket genelindeki Yönetici Rapor Görüntüleyicisi rolüne otomatik olarak eklenir.</span><span class="sxs-lookup"><span data-stu-id="c8cf0-113">Users who are MPN partner admins as of January 20, 2020 are automatically added to the company-wide **Executive Report Viewer** role for all locations for that tenant.</span></span> <span data-ttu-id="c8cf0-114">Bu kullanıcılar bu sayede Genel yönetici veya Hesap yöneticisi tarafından herhangi bir açık eylem gerekmeden raporlara Yönetici Raporu görüntüleyicisi olarak erişebilirsiniz. Genel yöneticiler ve Hesap yöneticileri, özelliklerini daha da artırmak veya sınırlamak için bu kullanıcıların otomatik olarak atanan rollerini geçersiz kabilir.</span><span class="sxs-lookup"><span data-stu-id="c8cf0-114">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c8cf0-115">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="c8cf0-115">Next steps</span></span>

- <span data-ttu-id="c8cf0-116">[İş Ortağı Merkezi Insights ve çeşitli raporları hakkında](partner-center-insights.md) daha fazla bilgi edinin.</span><span class="sxs-lookup"><span data-stu-id="c8cf0-116">Learn more about [Partner Center Insights](partner-center-insights.md) and its various reports.</span></span>
