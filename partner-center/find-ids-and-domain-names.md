---
title: Kiracı KIMLIĞINI, etki alanı adını, Kullanıcı nesne KIMLIĞINI bulun
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure portal-bir kuruluşun Azure AD kiracı KIMLIĞI, etki alanı adı veya belirli bir kullanıcı nesne KIMLIĞINDE kimlik bulmayı öğrenin. Bazı görevlerde bu bilgiler gereklidir.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: b88d6e11c7f4d56cf58d136a91b530688b3e5413
ms.sourcegitcommit: fdc32c0afce88f8266f75746ec15bf04745590ad
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/07/2020
ms.locfileid: "94360080"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="036a6-104">Bir kullanıcı için önemli kimlikleri bulma</span><span class="sxs-lookup"><span data-stu-id="036a6-104">Locate important IDs for a user</span></span>

<span data-ttu-id="036a6-105">Bu makalede, bir kullanıcı için aşağıdaki bilgileri bulmak üzere [Azure Portal](https://portal.azure.com/) nasıl kullanılacağı açıklanır:</span><span class="sxs-lookup"><span data-stu-id="036a6-105">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="036a6-106">Kullanıcının kuruluşunun veya şirketinin Microsoft Azure Active Directory (Azure AD) kiracı KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="036a6-106">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="036a6-107">Azure AD kiracısı ile ilişkili kuruluşun veya şirketin birincil etki alanı adı</span><span class="sxs-lookup"><span data-stu-id="036a6-107">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="036a6-108">Kullanıcı nesnesi KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="036a6-108">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="036a6-109">Microsoft Azure AD kiracı KIMLIĞINI ve birincil etki alanı adını bulun</span><span class="sxs-lookup"><span data-stu-id="036a6-109">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="036a6-110">Azure portal içinde Azure AD kiracı KIMLIĞINI veya birincil etki alanı adını bulmak için bu adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="036a6-110">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="036a6-111">(Bir kiracı KIMLIĞINI programlı bir şekilde bulmak istiyorsanız bkz. [PowerShell veya CLI ile KIRACı kimliğini bulma](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell).)</span><span class="sxs-lookup"><span data-stu-id="036a6-111">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="036a6-112">Kiracı KIMLIĞINE farklı uygulamalarda veya kaynaklarda farklı adlar adı verilir.</span><span class="sxs-lookup"><span data-stu-id="036a6-112">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="036a6-113">Örneğin, kiracı KIMLIĞI, dizin KIMLIĞI, Azure Active Directory (Azure AD) kiracısı, Microsoft KIMLIĞI veya belirli raporlar için, hatta *tenantguıd* olarak adlandırılır.</span><span class="sxs-lookup"><span data-stu-id="036a6-113">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="036a6-114">[Azure Portal](https://portal.azure.com/)’ında oturum açın.</span><span class="sxs-lookup"><span data-stu-id="036a6-114">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="036a6-115">Menüden **Azure Active Directory** seçin.</span><span class="sxs-lookup"><span data-stu-id="036a6-115">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Menüden Azure Active Directory seçeneğini seçen Azure portal gösterir.":::

3. <span data-ttu-id="036a6-117">Azure Active Directory **genel bakış** sayfası görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="036a6-117">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="036a6-118">Azure AD kiracı KIMLIĞINI veya birincil etki alanı adını bulmak için **KIRACı kimliği** alanını ve **birincil etki alanı** alanını bulun.</span><span class="sxs-lookup"><span data-stu-id="036a6-118">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="036a6-119">Bu alanlar, kiracı bilgileri bölümünde görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="036a6-119">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="İki Vurgulanan alan, kiracı KIMLIĞI ve birincil etki alanı adı içeren genel bakış sayfasını gösterir.":::

4. <span data-ttu-id="036a6-121">Kiracı KIMLIĞINI Azure portal birkaç farklı yolla bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="036a6-121">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="036a6-122">Menüden **Azure Active Directory** seçin.</span><span class="sxs-lookup"><span data-stu-id="036a6-122">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="036a6-123">Ardından, menüdeki **Yönet** bölümünü bulun ve **Özellikler** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="036a6-123">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="036a6-124">Özellikler sayfası kullanıcının ilişkili kiracı KIMLIĞINI de görüntüler.</span><span class="sxs-lookup"><span data-stu-id="036a6-124">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Vurgulanan kiracı KIMLIĞI alanıyla birlikte Özellikler sayfasını gösterir.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="036a6-126">Kullanıcı nesne KIMLIĞINI bul</span><span class="sxs-lookup"><span data-stu-id="036a6-126">Find the user object ID</span></span>

<span data-ttu-id="036a6-127">Yalnızca etki alanı adını ve kiracı KIMLIĞINI bulmanın her zaman yeterli olmayabilir.</span><span class="sxs-lookup"><span data-stu-id="036a6-127">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="036a6-128">Ayrıca, bir kullanıcıya atanan belirli nesne KIMLIĞINI de bulmanız gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="036a6-128">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="036a6-129">Azure portal kullanıcının nesne KIMLIĞINI bulmak için şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="036a6-129">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="036a6-130">[Azure Portal](https://portal.azure.com/)’ında oturum açın.</span><span class="sxs-lookup"><span data-stu-id="036a6-130">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="036a6-131">Menüden **Azure Active Directory** seçin.</span><span class="sxs-lookup"><span data-stu-id="036a6-131">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="036a6-132">Menüdeki **Yönet** bölümünü bulun ve ardından **Kullanıcılar** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="036a6-132">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Vurgulanan, kullanıcılar seçeneğiyle birlikte Azure Active Directory menüsünü gösterir.":::

4. <span data-ttu-id="036a6-134">Kullanıcılar sayfasında, arama kutusuna kullanıcının adını yazın.</span><span class="sxs-lookup"><span data-stu-id="036a6-134">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Belirli bir kullanıcıyı aramak için arama kutusuyla birlikte kullanıcılar sayfasını gösterir.":::

5. <span data-ttu-id="036a6-136">Listede göründüğü kullanıcının adını seçin.</span><span class="sxs-lookup"><span data-stu-id="036a6-136">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Aranan Kullanıcı için bir satır görüntüleyen Kullanıcı sayfasını gösterir.":::

6. <span data-ttu-id="036a6-138">Kullanıcının profil sayfasında kimlik bölümünü bulun.</span><span class="sxs-lookup"><span data-stu-id="036a6-138">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="036a6-139">Nesne KIMLIĞI alanı, kullanıcının benzersiz nesne KIMLIĞIYLE birlikte görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="036a6-139">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Kimlik bölümü ve nesne KIMLIĞI için vurgulanmış bir alan olan kullanıcı profili sayfasını gösterir.":::

## <a name="next-steps"></a><span data-ttu-id="036a6-141">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="036a6-141">Next steps</span></span>

- [<span data-ttu-id="036a6-142">PowerShell veya CLı ile program aracılığıyla kiracı KIMLIĞINIZI bulun</span><span class="sxs-lookup"><span data-stu-id="036a6-142">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="036a6-143">Azure Active Directory 'de Kullanıcı profilleri hakkında daha fazla bilgi edinin</span><span class="sxs-lookup"><span data-stu-id="036a6-143">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="036a6-144">İş ortaklarının Iş Ortağı Merkezi 'nde müşteri ayrıntılarını nasıl görebileceğine veya dışa verebileceğine öğrenin</span><span class="sxs-lookup"><span data-stu-id="036a6-144">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)
