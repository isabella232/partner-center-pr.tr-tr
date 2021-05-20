---
title: Otomatik hizmet bildirimleri için API'leri kullanma
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: İş ortakları Gerçek zamanlı hizmet durumu, ileti merkezi iletişimleri ve Microsoft Azure bakım olayları için Office 365 ve Microsoft Azure İş Ortakları için API'leri kullanabilir.
author: Kim-Davis
ms.author: kimnich
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b5092113ca90bccab6414fdf4013c76dd0ab4969
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150820"
---
# <a name="use-apis-for-automated-service-notifications-for-azure-insights--office-365-service-communications"></a><span data-ttu-id="6bb61-103">Azure Insights ve Office 365 hizmet iletişimleri için & bildirimleri için API'leri kullanma</span><span class="sxs-lookup"><span data-stu-id="6bb61-103">Use APIs for automated service notifications for Azure Insights & Office 365 service communications</span></span>

<span data-ttu-id="6bb61-104">**Uygun roller:** Yönetici aracısı | Genel yönetici | Satış aracısı | Yardım masası aracısı</span><span class="sxs-lookup"><span data-stu-id="6bb61-104">**Appropriate roles**: Admin agent | Global admin | Sales agent | Helpdesk agent</span></span>

<span data-ttu-id="6bb61-105">Office 365 ve Microsoft Azure, iş ortaklarının gerçek zamanlı hizmet durumunu, ileti merkezi iletişimlerini ve planlı bakım olaylarını almak için kullanabileceği bir API sağlar.</span><span class="sxs-lookup"><span data-stu-id="6bb61-105">Office 365 and Microsoft Azure each provide an API that partners can use to retrieve real-time service health, message center communications, and planned maintenance events.</span></span> <span data-ttu-id="6bb61-106">Bu API'ler genel kullanıma açıktır ve iş ortakları, temsilci olarak yönetici ayrıcalıkları nedeniyle bunları müşterileri adına kullanabilir.</span><span class="sxs-lookup"><span data-stu-id="6bb61-106">These APIs are publicly available, and partners can use them on behalf of their customers because of their delegated admin privileges.</span></span>

<span data-ttu-id="6bb61-107">Bu API'ler geliştiricileriniz tarafından kullanılabilir:</span><span class="sxs-lookup"><span data-stu-id="6bb61-107">These APIs are available for your developers:</span></span>

- [<span data-ttu-id="6bb61-108">Office 365 hizmet iletişimleri API'si</span><span class="sxs-lookup"><span data-stu-id="6bb61-108">Office 365 service communications API</span></span>](/office/office-365-management-api/office-365-service-communications-api-reference)
- <span data-ttu-id="6bb61-109">Azure Insights REST [API başvurusu](/rest/api/monitor/)</span><span class="sxs-lookup"><span data-stu-id="6bb61-109">Azure Insights REST [API reference](/rest/api/monitor/)</span></span>
