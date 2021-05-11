---
title: Kiracı kimliğini, etki alanı adını, kullanıcı nesne kimliğini bulma
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Bir kuruluşun Azure AD kiracı kimliği Azure portal etki alanı adı veya belirli kullanıcı nesnesi kimliği gibi kimlikleri nasıl bulamıyorum? Bazı görevler bu bilgilere ihtiyaç gösterir.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 643b1eeb96a47ee4c438f733efe3be22234d02ff
ms.sourcegitcommit: e462f562e7f26b7d6870c22638a2a841499109d6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/11/2021
ms.locfileid: "109740293"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="7ecc1-104">Bir kullanıcı için önemli kimlikleri bulma</span><span class="sxs-lookup"><span data-stu-id="7ecc1-104">Locate important IDs for a user</span></span>

<span data-ttu-id="7ecc1-105">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="7ecc1-105">**Appropriate roles**</span></span>

- <span data-ttu-id="7ecc1-106">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="7ecc1-106">Global admin</span></span>

<span data-ttu-id="7ecc1-107">Bu makalede, bir kullanıcıya Azure portal [bilgileri](https://portal.azure.com/) bulmak için Azure portal nasıl kullanabileceğiniz açıklanmıştır:</span><span class="sxs-lookup"><span data-stu-id="7ecc1-107">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="7ecc1-108">Kullanıcının Microsoft Azure Active Directory kuruluşuna veya şirketin kiracı kimliğine (Azure AD) göre</span><span class="sxs-lookup"><span data-stu-id="7ecc1-108">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="7ecc1-109">Azure AD kiracısı ile ilişkili kuruluşun veya şirketin birincil etki alanı adı</span><span class="sxs-lookup"><span data-stu-id="7ecc1-109">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="7ecc1-110">Kullanıcı nesnesi kimliği</span><span class="sxs-lookup"><span data-stu-id="7ecc1-110">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="7ecc1-111">Kiracı kimliğini Microsoft Azure AD birincil etki alanı adını bulma</span><span class="sxs-lookup"><span data-stu-id="7ecc1-111">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="7ecc1-112">Azure AD kiracı kimliğini veya etki alanı içindeki birincil etki alanı adını bulmak için bu Azure portal.</span><span class="sxs-lookup"><span data-stu-id="7ecc1-112">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="7ecc1-113">(Kiracı kimliğini program aracılığıyla bulmak için bkz. [PowerShell](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell)veya CLI ile kiracı kimliğini bulma.)</span><span class="sxs-lookup"><span data-stu-id="7ecc1-113">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="7ecc1-114">Kiracı kimliği, farklı uygulamalarda veya kaynaklarda farklı adlar olarak çağrıl olabilir.</span><span class="sxs-lookup"><span data-stu-id="7ecc1-114">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="7ecc1-115">Örneğin, kiracı kimliğine dizin kimliği, Azure Active Directory (Azure AD) kiracısı, Microsoft kimliği veya belirli raporlar için, hatta kiracı tarafından yönlendirilen olarak *başvurul olabilir.*</span><span class="sxs-lookup"><span data-stu-id="7ecc1-115">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="7ecc1-116">[Azure portalında](https://portal.azure.com/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="7ecc1-116">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="7ecc1-117">Menüden **Azure Active Directory'yi** seçin.</span><span class="sxs-lookup"><span data-stu-id="7ecc1-117">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Menüden Azure portal seçerek Azure Active Directory seçeneğini gösterir.":::

3. <span data-ttu-id="7ecc1-119">Bir Azure Active Directory **Genel Bakış** sayfası görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="7ecc1-119">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="7ecc1-120">Azure AD kiracı kimliğini veya birincil etki alanı adını bulmak için Kiracı Kimliği **alanını ve** Birincil etki **alanı alanını** bulun.</span><span class="sxs-lookup"><span data-stu-id="7ecc1-120">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="7ecc1-121">Bu alanlar Kiracı bilgileri bölümünde görünür.</span><span class="sxs-lookup"><span data-stu-id="7ecc1-121">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Kiracı kimliği ve birincil etki alanı adı olmak için vurgulanmış iki alanla Genel Bakış sayfasını gösterir.":::

4. <span data-ttu-id="7ecc1-123">Kiracı KIMLIĞINI Azure portal birkaç farklı yolla bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7ecc1-123">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="7ecc1-124">Menüden **Azure Active Directory** seçin.</span><span class="sxs-lookup"><span data-stu-id="7ecc1-124">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="7ecc1-125">Ardından, menüdeki **Yönet** bölümünü bulun ve **Özellikler**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="7ecc1-125">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="7ecc1-126">Özellikler sayfası kullanıcının ilişkili kiracı KIMLIĞINI de görüntüler.</span><span class="sxs-lookup"><span data-stu-id="7ecc1-126">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Vurgulanan kiracı KIMLIĞI alanıyla birlikte Özellikler sayfasını gösterir.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="7ecc1-128">Kullanıcı nesne KIMLIĞINI bul</span><span class="sxs-lookup"><span data-stu-id="7ecc1-128">Find the user object ID</span></span>

<span data-ttu-id="7ecc1-129">Yalnızca etki alanı adını ve kiracı KIMLIĞINI bulmanın her zaman yeterli olmayabilir.</span><span class="sxs-lookup"><span data-stu-id="7ecc1-129">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="7ecc1-130">Ayrıca, bir kullanıcıya atanan belirli nesne KIMLIĞINI de bulmanız gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="7ecc1-130">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="7ecc1-131">Azure portal kullanıcının nesne KIMLIĞINI bulmak için şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="7ecc1-131">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="7ecc1-132">[Azure portalında](https://portal.azure.com/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="7ecc1-132">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="7ecc1-133">Menüden **Azure Active Directory** seçin.</span><span class="sxs-lookup"><span data-stu-id="7ecc1-133">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="7ecc1-134">Menüdeki **Yönet** bölümünü bulun ve ardından **Kullanıcılar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="7ecc1-134">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Vurgulanan, kullanıcılar seçeneğiyle birlikte Azure Active Directory menüsünü gösterir.":::

4. <span data-ttu-id="7ecc1-136">Kullanıcılar sayfasında, arama kutusuna kullanıcının adını yazın.</span><span class="sxs-lookup"><span data-stu-id="7ecc1-136">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Belirli bir kullanıcıyı aramak için arama kutusuyla birlikte kullanıcılar sayfasını gösterir.":::

5. <span data-ttu-id="7ecc1-138">Listede göründüğü kullanıcının adını seçin.</span><span class="sxs-lookup"><span data-stu-id="7ecc1-138">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Aranan Kullanıcı için bir satır görüntüleyen Kullanıcı sayfasını gösterir.":::

6. <span data-ttu-id="7ecc1-140">Kullanıcının profil sayfasında kimlik bölümünü bulun.</span><span class="sxs-lookup"><span data-stu-id="7ecc1-140">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="7ecc1-141">Nesne KIMLIĞI alanı, kullanıcının benzersiz nesne KIMLIĞIYLE birlikte görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="7ecc1-141">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Kimlik bölümü ve nesne KIMLIĞI için vurgulanmış bir alan olan kullanıcı profili sayfasını gösterir.":::

## <a name="next-steps"></a><span data-ttu-id="7ecc1-143">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="7ecc1-143">Next steps</span></span>

- [<span data-ttu-id="7ecc1-144">PowerShell veya CLı ile program aracılığıyla kiracı KIMLIĞINIZI bulun</span><span class="sxs-lookup"><span data-stu-id="7ecc1-144">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="7ecc1-145">Azure Active Directory'de kullanıcı profilleri hakkında daha fazla bilgi Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="7ecc1-145">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="7ecc1-146">İş ortaklarının müşteri ayrıntılarını nasıl göreceğini veya dışarı aktara İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="7ecc1-146">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

