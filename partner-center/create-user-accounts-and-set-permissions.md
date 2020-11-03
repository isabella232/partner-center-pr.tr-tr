---
title: Kullanıcı hesapları oluşturma ve rol atama
description: Iş Ortağı Merkezi 'Ne erişebilmek için her çalışana bir rol atanması gerekir. Kullanıcı hesapları oluşturma, rol atama ve izinleri ayarlama hakkında bilgi edinin.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperfq2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 41f7f68c61630daf30595e28bd5de52f5a5787c8
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/13/2020
ms.locfileid: "92531851"
---
# <a name="create-user-accounts"></a><span data-ttu-id="67d5c-104">Kullanıcı hesapları oluşturma</span><span class="sxs-lookup"><span data-stu-id="67d5c-104">Create user accounts</span></span>  

<span data-ttu-id="67d5c-105">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="67d5c-105">**Appropriate roles**</span></span>

- <span data-ttu-id="67d5c-106">Hesap yöneticisi</span><span class="sxs-lookup"><span data-stu-id="67d5c-106">Account admin</span></span>
- <span data-ttu-id="67d5c-107">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="67d5c-107">Global admin</span></span>
- <span data-ttu-id="67d5c-108">Kullanıcı Yönetimi Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="67d5c-108">User management admin</span></span>

<span data-ttu-id="67d5c-109">Iş Ortağı Merkezi 'ne erişmesi gereken çalışanlar için Kullanıcı hesapları oluşturun.</span><span class="sxs-lookup"><span data-stu-id="67d5c-109">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="67d5c-110">Bu görevlerin Kullanıcı Yönetimi Yöneticisi, hesap yöneticisi veya genel yönetici tarafından yapılması gerekir. Bu görevleri gerçekleştiren kullanıcıya ayrıca Kullanıcı Yöneticisi veya genel yönetici Azure Active Directory (AAD) rolleri atanmalıdır.</span><span class="sxs-lookup"><span data-stu-id="67d5c-110">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="67d5c-111">AAD rolleri hakkında daha fazla bilgi için [Azure Active Directory Içindeki yönetici rolü izinleri](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="67d5c-111">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>

## <a name="add-a-new-user"></a><span data-ttu-id="67d5c-112">Yeni kullanıcı ekleme</span><span class="sxs-lookup"><span data-stu-id="67d5c-112">Add a new user</span></span>

1. <span data-ttu-id="67d5c-113">Iş Ortağı Merkezi 'nin sağ üst köşesindeki **Ayarlar** simgesinden **Hesap ayarları** ' nı seçin ve ardından **Kullanıcı yönetimi** ' ni seçin.</span><span class="sxs-lookup"><span data-stu-id="67d5c-113">From the **Settings** icon at the top right of the Partner Center, select **Account settings** and then select **User management** .</span></span>

2. <span data-ttu-id="67d5c-114">**Kullanıcı ekle** 'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="67d5c-114">Select **Add user** .</span></span>

3. <span data-ttu-id="67d5c-115">Kullanıcının tam adını ve benzersiz e-posta adresini girin.</span><span class="sxs-lookup"><span data-stu-id="67d5c-115">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="67d5c-116">Aracının türünü ve/veya kullanıcıya atamak istediğiniz yönetici türünü seçin.</span><span class="sxs-lookup"><span data-stu-id="67d5c-116">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="67d5c-117">İş ortağı merkezi erişimi rol tabanlıdır, bu nedenle kullanıcının görünümünü yalnızca kullanıcının belirli görevleri tamamlaması için ihtiyaç duyacağı özellikleri gösterecek şekilde özelleştirmek için izinler atayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="67d5c-117">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="67d5c-118">Kullanıcılar bir rol ataması istiyorlarsa, genel yöneticilerle **Kullanıcı yönetimine** ve filtrelemeye geçerek genel yöneticileri iletişim kurmak üzere bulabilir.</span><span class="sxs-lookup"><span data-stu-id="67d5c-118">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="67d5c-119">Kullanıcı hesabını oluşturmak için **Ekle** 'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="67d5c-119">Select **Add** to create the user account.</span></span> <span data-ttu-id="67d5c-120">Sonraki sayfada kullanıcının ayrıntılarını onaylayın.</span><span class="sxs-lookup"><span data-stu-id="67d5c-120">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="67d5c-121">Yeni kullanıcının oturum açma bilgilerini bu sayfada bir yere unutmayın.</span><span class="sxs-lookup"><span data-stu-id="67d5c-121">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="67d5c-122">Daha sonra tekrar erişemeyeceksiniz, bu bilgileri kopyalayıp yeni kullanıcıya gönderdiğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="67d5c-122">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 

<span data-ttu-id="67d5c-123">Kullanıcının Iş Ortağı Merkezi 'nde Kullanıcı adı ve geçici parola ile oturum açması gerekir.</span><span class="sxs-lookup"><span data-stu-id="67d5c-123">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="67d5c-124">Kullanıcı Iş Ortağı Merkezi 'ne ilk kez oturum açtığında, kullanıcıların parolalarını değiştirmesi istenir.</span><span class="sxs-lookup"><span data-stu-id="67d5c-124">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span>

## <a name="assign-user-roles"></a><span data-ttu-id="67d5c-125">Kullanıcı rolleri atama</span><span class="sxs-lookup"><span data-stu-id="67d5c-125">Assign user roles</span></span>

<span data-ttu-id="67d5c-126">İş Ortağı Merkezi 'nde çalışmak için atanmış bir role sahip olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="67d5c-126">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="67d5c-127">Şu anda, roller Azure Active Directory kiracı rolleri, bulut çözümü sağlayıcısı (CSP) rolleri ve AAD olmayan şirket rollerini içerir.</span><span class="sxs-lookup"><span data-stu-id="67d5c-127">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="67d5c-128">Tek bir şirketin bu rollerin tümüne ihtiyacı olabilir.</span><span class="sxs-lookup"><span data-stu-id="67d5c-128">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="67d5c-129">Iş Ortağı Merkezi 'ne erişmek için kişisel kişilerin kiracınızda listelenmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="67d5c-129">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="67d5c-130">Rol atamaları ek erişim sağlar.</span><span class="sxs-lookup"><span data-stu-id="67d5c-130">Role assignments provide additional access.</span></span>

## <a name="next-steps"></a><span data-ttu-id="67d5c-131">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="67d5c-131">Next steps</span></span>

- [<span data-ttu-id="67d5c-132">İş Ortağı Merkezi 'nde çalışması gereken çalışanlar için Kullanıcı rolleri ve izinleri atama</span><span class="sxs-lookup"><span data-stu-id="67d5c-132">Assign users roles and permissions for employees needing to work in Partner Center</span></span>](permissions-overview.md)
