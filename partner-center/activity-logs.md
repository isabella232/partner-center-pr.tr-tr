---
title: Müşteri etkinlik günlükleri ile içgörüler elde edin
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Müşteri hesabı işlemleri ve müşteriyle ilgili diğer iş ortağı yönetimi etkinlikleri hakkında içgörü elde etmek için etkinlik günlüklerini görüntülemeyi ve dışarı aktarmayı öğrenin.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1bb98dd71c9e46914b90d5efbfe14404d08275f9
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150599"
---
# <a name="view-or-export-customer-activity-logs-for-more-insight-into-customer-transactions"></a><span data-ttu-id="8f8c0-103">Müşteri işlemleriyle ilgili daha fazla içgörü için müşteri etkinlik günlüklerini görüntüleme veya dışarı aktarma</span><span class="sxs-lookup"><span data-stu-id="8f8c0-103">View or export customer activity logs for more insight into customer transactions</span></span>

<span data-ttu-id="8f8c0-104">**Uygun roller:** Genel yönetici | Faturalama yöneticisi | Kullanıcı yönetimi yönetici | Yönetici aracısı | Satış aracısı | Yardım masası aracısı</span><span class="sxs-lookup"><span data-stu-id="8f8c0-104">**Appropriate roles**: Global admin | Billing admin | User management admin | Admin agent | Sales agent | Helpdesk agent</span></span>

<span data-ttu-id="8f8c0-105">Etkinlik günlükleri, müşteriler için işlemler ve İş ortağı yönetimi eylemleri hakkında bilgi sağlar.</span><span class="sxs-lookup"><span data-stu-id="8f8c0-105">Activity logs provide information on transactions and Partner management actions for customers.</span></span> <span data-ttu-id="8f8c0-106">İşlemlerin günlükleri, satın alınan abonelikler de dahil olmak üzere işlem hakkında ayrıntılı bilgi sağlar.</span><span class="sxs-lookup"><span data-stu-id="8f8c0-106">Logs for transactions provide detailed information about the transaction, including purchased subscriptions.</span></span> <span data-ttu-id="8f8c0-107">Etkinlik günlüklerini Excel ile uyumlu virgülle ayrılmış değer dosyası biçimine (.csv) de aktarabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8f8c0-107">You can also export activity logs to an Excel-compatible comma-separated value file format (.csv).</span></span>

<span data-ttu-id="8f8c0-108">Etkinlik günlükleri, müşteri hesapları ve ürün işlemleriyle ilgili iş ortağı eylemleri için kayıtlar sağlar.</span><span class="sxs-lookup"><span data-stu-id="8f8c0-108">Activity logs provide records for Partner actions on customer accounts and product transactions.</span></span> <span data-ttu-id="8f8c0-109">Etkinlik günlüklerini bir .csv dosyasına da aktarabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8f8c0-109">You can also export activity logs to a .csv file.</span></span>

## <a name="view-and-export-activity-logs"></a><span data-ttu-id="8f8c0-110">Etkinlik günlüklerini görüntüleme ve dışarı aktarma</span><span class="sxs-lookup"><span data-stu-id="8f8c0-110">View and export activity logs</span></span>

1. <span data-ttu-id="8f8c0-111">İş Ortağı Merkezi [oturum açın.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="8f8c0-111">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="8f8c0-112">Hesap ayarları **menüsünde Etkinlik** **Günlüğü'yü seçin.**</span><span class="sxs-lookup"><span data-stu-id="8f8c0-112">From the **Account settings** menu, select **Activity Log**.</span></span>

3. <span data-ttu-id="8f8c0-113">From and to alanlarında **etkinlik günlüğü** **dönemini** seçin.</span><span class="sxs-lookup"><span data-stu-id="8f8c0-113">Select the activity log period in the **From** and **to** fields.</span></span> <span data-ttu-id="8f8c0-114">Etkinlik günlüğü dışarı aktarma varsayılan olarak en son aya göredir.</span><span class="sxs-lookup"><span data-stu-id="8f8c0-114">The activity log export defaults to the most recent month.</span></span>

   <span data-ttu-id="8f8c0-115">Her etkinlik günlüğü, listelenen müşterinin Abonelikler sayfasına bir **bağlantı** sağlar.</span><span class="sxs-lookup"><span data-stu-id="8f8c0-115">Each activity log provides a link to the listed customer's **Subscriptions** page.</span></span>

   <span data-ttu-id="8f8c0-116">Günlüğe kaydedilen bir eylemle ilgili ayrıntıları görüntülemek için herhangi bir etkinlik günlüğü için aşağı oku seçin.</span><span class="sxs-lookup"><span data-stu-id="8f8c0-116">Select a down arrow for any activity log to view details about a logged action.</span></span> <span data-ttu-id="8f8c0-117">Tek bir etkinlik günlüğü, birden çok ürün sipariş etmek gibi önemli miktarda veri gösterebilir.</span><span class="sxs-lookup"><span data-stu-id="8f8c0-117">A single activity log can show a significant amount of data, such as the ordering of multiple products.</span></span>

4. <span data-ttu-id="8f8c0-118">Günlüğün veri sütunları aşağıdakileri içerir:</span><span class="sxs-lookup"><span data-stu-id="8f8c0-118">The data columns of the log include the following:</span></span>
   - <span data-ttu-id="8f8c0-119">**Tarih-Saat**- eylemin tarihi ve saati;</span><span class="sxs-lookup"><span data-stu-id="8f8c0-119">**Date-Time**-the date and time of the action;</span></span>
   - <span data-ttu-id="8f8c0-120">**Etkilenen müşteri**— müşterinin şirket adı;</span><span class="sxs-lookup"><span data-stu-id="8f8c0-120">**Affected customer**—the customer's company name;</span></span>
   - <span data-ttu-id="8f8c0-121">**Eylem**— "bir başvuru oluşturuldu" gibi müşteri tarafından gerçekleştirilen eylem;</span><span class="sxs-lookup"><span data-stu-id="8f8c0-121">**Action**—the action taken by the customer such as "created a referral";</span></span>
   - <span data-ttu-id="8f8c0-122">**Iş Ortağı kullanıcısı**— faaliyetle ilişkili iş ortağı.</span><span class="sxs-lookup"><span data-stu-id="8f8c0-122">**Partner user**—the partner associated with the activity.</span></span>

5. <span data-ttu-id="8f8c0-123">Müşterinin abonelik verilerini bir. csv dosyasına kopyalamak ve bilgisayarınızdaki varsayılan indirme klasörüne indirmek için **günlüğü dışarı aktar** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="8f8c0-123">Select **Export log** to copy the customer's subscription data into a .csv file and download it to the default download folder on your computer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8f8c0-124">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="8f8c0-124">Next steps</span></span>

- [<span data-ttu-id="8f8c0-125">İş kararlarını sağlamaya yardımcı olmak için abonelikleri ve lisansları çözümleyin</span><span class="sxs-lookup"><span data-stu-id="8f8c0-125">Analyze subscriptions and licenses to help drive business decisions</span></span>](analyze-subscriptions-licenses.md)
