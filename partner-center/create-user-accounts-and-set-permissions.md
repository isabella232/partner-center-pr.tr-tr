---
title: Kullanıcı hesapları oluşturma ve rol atama
description: Her çalışana erişim izni olmadan önce bir rol İş Ortağı Merkezi. Kullanıcı hesapları oluşturma, rol atama ve izinleri ayarlama hakkında bilgi.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperf-fy21q2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 9621f0bc3283d7d3b08e2ebac62b4e5d8c95a4d4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148151"
---
# <a name="create-user-accounts"></a><span data-ttu-id="8cbd2-104">Kullanıcı hesapları oluşturma</span><span class="sxs-lookup"><span data-stu-id="8cbd2-104">Create user accounts</span></span>  

<span data-ttu-id="8cbd2-105">**Uygun roller:** Hesap yöneticisi | Genel yönetici | Kullanıcı yönetimi yöneticisi</span><span class="sxs-lookup"><span data-stu-id="8cbd2-105">**Appropriate roles**: Account admin | Global admin | User management admin</span></span>

<span data-ttu-id="8cbd2-106">Şirket hesabına erişmesi gereken çalışanlar için kullanıcı İş Ortağı Merkezi.</span><span class="sxs-lookup"><span data-stu-id="8cbd2-106">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="8cbd2-107">Bu görevlerin kullanıcı yönetimi yöneticisi, hesap yöneticisi veya genel yönetici tarafından yapılması gerekir. Bu görevleri gerçekleştiren kullanıcıya Kullanıcı yöneticisi veya Azure Active Directory (AAD) rolü de Genel yönetici.</span><span class="sxs-lookup"><span data-stu-id="8cbd2-107">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="8cbd2-108">AAD rolleri hakkında daha fazla bilgi için [bkz.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8cbd2-108">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>

## <a name="add-a-new-user"></a><span data-ttu-id="8cbd2-109">Yeni kullanıcı ekleme</span><span class="sxs-lookup"><span data-stu-id="8cbd2-109">Add a new user</span></span>

1. <span data-ttu-id="8cbd2-110">Uygulamanın **sağ** üst köşesindeki Ayarlar simgesinden Hesap İş Ortağı Merkezi'ı **ve ardından** Kullanıcı **yönetimi'ne tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="8cbd2-110">From the **Settings** icon at the top right of the Partner Center, select **Account settings** and then select **User management**.</span></span>

2. <span data-ttu-id="8cbd2-111">**Kullanıcı ekle**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="8cbd2-111">Select **Add user**.</span></span>

3. <span data-ttu-id="8cbd2-112">Kullanıcının tam adını ve benzersiz e-posta adresini girin.</span><span class="sxs-lookup"><span data-stu-id="8cbd2-112">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="8cbd2-113">Aracı türünü ve/veya kullanıcıya atamak istediğiniz yönetici türünü seçin.</span><span class="sxs-lookup"><span data-stu-id="8cbd2-113">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="8cbd2-114">İş Ortağı Merkezi rol tabanlıdır, bu nedenle kullanıcının görünümünü yalnızca kullanıcının belirli görevleri tamamlaması için gereken özellikleri gösterecek şekilde özelleştirmek için izinler atabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8cbd2-114">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="8cbd2-115">Kullanıcılar rol ataması yapmak isterse, Kullanıcı yönetimi'ne  gidip genel yöneticiyi filtreleerek genel yöneticilerin iletişim kuracaklarını bulabilirler.</span><span class="sxs-lookup"><span data-stu-id="8cbd2-115">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="8cbd2-116">Kullanıcı hesabını oluşturmak için **Ekle**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="8cbd2-116">Select **Add** to create the user account.</span></span> <span data-ttu-id="8cbd2-117">Sonraki sayfada kullanıcının ayrıntılarını onaylayın.</span><span class="sxs-lookup"><span data-stu-id="8cbd2-117">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="8cbd2-118">Bu sayfada görüntülenen yeni kullanıcının oturum açma bilgilerini not edin.</span><span class="sxs-lookup"><span data-stu-id="8cbd2-118">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="8cbd2-119">Bu bilgileri kopyalayıp yeni kullanıcıya gönderebilirsiniz çünkü daha sonra bu bilgilere yeniden erişesiniz.</span><span class="sxs-lookup"><span data-stu-id="8cbd2-119">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 

<span data-ttu-id="8cbd2-120">Kullanıcının kullanıcı adı ve geçici parolayla İş Ortağı Merkezi oturum açması gerekir.</span><span class="sxs-lookup"><span data-stu-id="8cbd2-120">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="8cbd2-121">Kullanıcı, İş Ortağı Merkezi kez oturum açınca parolasını değiştirmesi istenir.</span><span class="sxs-lookup"><span data-stu-id="8cbd2-121">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span>

## <a name="assign-user-roles"></a><span data-ttu-id="8cbd2-122">Kullanıcı rolleri atama</span><span class="sxs-lookup"><span data-stu-id="8cbd2-122">Assign user roles</span></span>

<span data-ttu-id="8cbd2-123">Bu rolde İş Ortağı Merkezi için atanmış bir rolünüz olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="8cbd2-123">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="8cbd2-124">Şu anda roller kiracı Azure Active Directory, Bulut Çözümü Sağlayıcısı (CSP) rolleri ve AAD dışı şirket rollerini içerir.</span><span class="sxs-lookup"><span data-stu-id="8cbd2-124">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="8cbd2-125">Tek bir şirketin bu rollerin tümüne ihtiyacı olabilir.</span><span class="sxs-lookup"><span data-stu-id="8cbd2-125">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="8cbd2-126">Iş Ortağı Merkezi 'ne erişmek için kişisel kişilerin kiracınızda listelenmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="8cbd2-126">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="8cbd2-127">Rol atamaları ek erişim sağlar.</span><span class="sxs-lookup"><span data-stu-id="8cbd2-127">Role assignments provide additional access.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8cbd2-128">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="8cbd2-128">Next steps</span></span>

- [<span data-ttu-id="8cbd2-129">İş Ortağı Merkezi 'nde çalışması gereken çalışanlar için Kullanıcı rolleri ve izinleri atama</span><span class="sxs-lookup"><span data-stu-id="8cbd2-129">Assign users roles and permissions for employees needing to work in Partner Center</span></span>](permissions-overview.md)
