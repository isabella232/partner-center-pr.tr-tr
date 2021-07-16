---
title: Analiz verilerine programlı olarak erişim önkoşulları
description: Analiz verilerine programlı olarak erişim önkoşulları
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d4c39025aa3804435dd4d2359b93cd4a2e13ccc4
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376953"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a><span data-ttu-id="05991-103">Analiz verilerine programlı olarak erişim önkoşulları</span><span class="sxs-lookup"><span data-stu-id="05991-103">Prerequisites to programmatically access analytics data</span></span>

<span data-ttu-id="05991-104">**Uygun roller:** Genel yönetici | MPN Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="05991-104">**Appropriate roles:** Global admin | MPN admin</span></span>

<span data-ttu-id="05991-105">İş ortağı öngörüleri analiz verilerine programlı bir şekilde erişebilmeniz için aşağıdaki gereksinimleri karşılamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="05991-105">Before you can programmatically access partner insights analytics data, you need to meet the following requirements.</span></span>

## <a name="mpn-program-enrollment"></a><span data-ttu-id="05991-106">MPN program kaydı</span><span class="sxs-lookup"><span data-stu-id="05991-106">MPN Program enrollment</span></span>

<span data-ttu-id="05991-107">İş ortağı öngörüleri Analizi verilerine programlı bir şekilde erişmek için MPN programına kaydolduktan ve bir Iş Ortağı Merkezi hesabına sahip olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="05991-107">To access partner insights analytics data programmatically, you need to be enrolled in the MPN program and have a Partner Center account.</span></span> <span data-ttu-id="05991-108">Nasıl yapılacağını öğrenmek için bkz. [Iş Ortağı Merkezi 'nde MPN hesabı oluşturma](mpn-create-a-partner-center-account.md)</span><span class="sxs-lookup"><span data-stu-id="05991-108">To learn how, see [Create an MPN account in Partner Center](mpn-create-a-partner-center-account.md)</span></span>

## <a name="create-azure-active-directory-aad-application"></a><span data-ttu-id="05991-109">Azure Active Directory (AAD) uygulaması oluşturma</span><span class="sxs-lookup"><span data-stu-id="05991-109">Create Azure Active Directory (AAD) application</span></span>

<span data-ttu-id="05991-110">düzenli kullanıcı kimlik bilgileri, iş ortağı Analizler analiz verilerine programlı erişim için kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="05991-110">Regular user credentials cannot be used for programmatic access of Partner Insights Analytics data.</span></span> <span data-ttu-id="05991-111">programlı erişim apı 'lerine erişmek için bir Azure Active Directory (AAD) uygulamasının bir gizli anahtar (uygulama + kullanıcı erişimi) ile birlikte oluşturulması gerekir.</span><span class="sxs-lookup"><span data-stu-id="05991-111">An Azure Active Directory (AAD) application needs to be created along with a secret (application + user access) to access the programmatic access APIs.</span></span> <span data-ttu-id="05991-112">AAD uygulaması ve gizli dizi oluşturmayı öğrenmek için bkz [. hızlı başlangıç: Microsoft kimlik platformu bir uygulamayı kaydetme.](/azure/active-directory/develop/quickstart-register-app)   Microsoft Iş ortağı API 'sine erişmek için izin gerekir.</span><span class="sxs-lookup"><span data-stu-id="05991-112">To learn how to create an AAD application and secret, see [Quickstart: Register an application with the Microsoft identity platform.](/azure/active-directory/develop/quickstart-register-app) Permission is required to access Microsoft Partner API.</span></span> <span data-ttu-id="05991-113">İzin ekleme hakkında bilgi edinmek için bkz. [Iş ortağı API kimlik doğrulaması-Iş ortağı](/partner/develop/api-authentication#application-and-user-access)</span><span class="sxs-lookup"><span data-stu-id="05991-113">To learn how to add permission, see [Partner API authentication - Partner](/partner/develop/api-authentication#application-and-user-access)</span></span>

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a><span data-ttu-id="05991-114">Kullanıcıya Executive Report Viewer (ERV) rolü atama</span><span class="sxs-lookup"><span data-stu-id="05991-114">Assign Executive Report Viewer (ERV) role to the user</span></span>

<span data-ttu-id="05991-115">İş ortağı öngörüleri Analizi verilerine programlı bir şekilde erişmek için, Executive Report Viewer (ERV) olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="05991-115">To access partner insights analytics data programmatically, you should have Executive Report Viewer (ERV).</span></span> <span data-ttu-id="05991-116">kullanıcıya erv rolü atamayı öğrenmek için bkz. [partner center Analizler rol tabanlı erişim-iş ortağı merkezi](insights-roles.md)</span><span class="sxs-lookup"><span data-stu-id="05991-116">To learn how to assign ERV role to the user, see [Partner Center Insights role-based access - Partner Center](insights-roles.md)</span></span>

## <a name="generate-an-aad-token"></a><span data-ttu-id="05991-117">AAD belirteci oluşturma</span><span class="sxs-lookup"><span data-stu-id="05991-117">Generate an AAD token</span></span>

<span data-ttu-id="05991-118">Uygulama (istemci) KIMLIĞI, istemci parolası, Kullanıcı KIMLIĞINIZ ve parolanızı kullanarak bir AAD belirteci oluşturmanız gerekir. AAD belirteci oluşturma adımları için   [buraya bakın](insights-programmatic-first-api-call.md#token-generation) .</span><span class="sxs-lookup"><span data-stu-id="05991-118">You need to Generate an AAD token using the Application (client) ID, client secret, your user ID and password.  [Check here](insights-programmatic-first-api-call.md#token-generation) for steps to generate AAD token.</span></span>

> [!Note]
> <span data-ttu-id="05991-119">Belirteç bir saat için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="05991-119">The token is valid for one hour.</span></span>

## <a name="next-steps"></a><span data-ttu-id="05991-120">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="05991-120">Next steps</span></span>
[<span data-ttu-id="05991-121">Programlı erişim paradigması</span><span class="sxs-lookup"><span data-stu-id="05991-121">Programmatic access paradigm</span></span>](insights-programmatic-access-paradigm.md)