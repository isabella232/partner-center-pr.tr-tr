---
title: Kullanıcıları müşteri hesaplarına göre yönetme
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Iş Ortağı Merkezi 'nde müşterileriniz için kullanıcıları yönetme-Kullanıcı hesapları oluşturma, kullanıcı lisansları ekleme veya kaldırma, parolaları sıfırlama ve Kullanıcı hesaplarını silme veya geri yükleme.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0e2bb4ceb146174da83e9c08a9ff030380298bd0
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756090"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="9b5f1-103">Müşteri hesapları için kullanıcıları ve kullanıcı lisanslarını yönetme</span><span class="sxs-lookup"><span data-stu-id="9b5f1-103">Manage users and user licenses for customer accounts</span></span> 

<span data-ttu-id="9b5f1-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="9b5f1-104">**Appropriate roles**</span></span>

- <span data-ttu-id="9b5f1-105">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="9b5f1-105">Global admin</span></span>
- <span data-ttu-id="9b5f1-106">Kullanıcı Yönetimi Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="9b5f1-106">User management admin</span></span>
- <span data-ttu-id="9b5f1-107">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="9b5f1-107">Admin agent</span></span>


<span data-ttu-id="9b5f1-108">Müşterinin hesabındaki yeni kullanıcıları oluşturabilir ve silebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-108">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="9b5f1-109">Ayrıca, silmenin 30 gün içinde daha önce sildiğiniz bir veya daha fazla kullanıcı hesabını geri yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-109">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="9b5f1-110">Kullanıcının önceki abonelik atamaları da geri yüklenecektir (önceki ayırmaların kullanılabildiği varsayılarak).</span><span class="sxs-lookup"><span data-stu-id="9b5f1-110">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="9b5f1-111">Bir müşteri için yeni abonelikler satın aldığınızda, müşteri size hesap, Kullanıcı izinleri ve her kullanıcının ihtiyacı olan hizmetlere sahip olan tüm kullanıcıların bir listesini vermelidir.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-111">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

>[!NOTE]
><span data-ttu-id="9b5f1-112">**Müşteri** sekmesinin **Kullanıcılar ve lisanslar** bölümü, belirli bir müşterinin kiracısında oluşturulan, başka bir CSP ortağından veya başka bir satın alma kanalından satın alınmış lisanslardan oluşan kullanıcılar dahil olmak üzere tüm kullanıcıları gösterir.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-112">The **Users and licenses** section of **Customer** tab shows all users created in a specific customer’s tenant, including users that have licenses purchased from another CSP partner or from another purchasing channel.</span></span>

<span data-ttu-id="9b5f1-113">[Excel uyumlu bir. csv elektronik tablo dosyası](adding-multiple-users-to-a-customer-account.md)kullanarak adları içeri aktararak aynı anda [birden fazla kullanıcıya abonelik atayabilirsiniz](bulk-license-provisioning-for-multiple-users.md) .</span><span class="sxs-lookup"><span data-stu-id="9b5f1-113">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="9b5f1-114">Müşteri için kullanıcı hesapları oluşturma</span><span class="sxs-lookup"><span data-stu-id="9b5f1-114">Create user accounts for a customer</span></span>

1. <span data-ttu-id="9b5f1-115">Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-115">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="9b5f1-116">Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve listeden bir müşteri seçin.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-116">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="9b5f1-117">Müşteri menüsünde, **Kullanıcılar ve lisanslar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-117">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="9b5f1-118">Eklediğiniz her kullanıcı için **Abonelik Ekle**' yi seçin ve ardından izinler ve lisanslar dahil olmak üzere bilgileri doldurun.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-118">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="9b5f1-119">Değişikliklerinizi **kaydedin** .</span><span class="sxs-lookup"><span data-stu-id="9b5f1-119">**Save** your changes.</span></span>

5. <span data-ttu-id="9b5f1-120">Kullanıcıya göndermek için Kullanıcı adını ve geçici parolayı kaydettiğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-120">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="9b5f1-121">Birden çok kullanıcıyı aynı anda ekliyorsanız, **başka bir Kullanıcı Ekle** öğesini kullanın.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-121">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="9b5f1-122">Ayrıca, [Excel ile uyumlu bir. csv elektronik tablo dosyasını içeri aktararak](adding-multiple-users-to-a-customer-account.md)aynı anda birden fazla kullanıcı ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-122">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="9b5f1-123">Onay ekranından adları ve parolaları göndermeden veya yazdırmadan önce tüm küme ile işiniz tamamlanana kadar bekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-123">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="9b5f1-124">Müşteri için kullanıcı lisansları ekleme veya kaldırma</span><span class="sxs-lookup"><span data-stu-id="9b5f1-124">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="9b5f1-125">Aşağıdaki adımlar, Microsoft ürünlerine yönelik kullanıcı lisanslarını eklemek veya kaldırmak için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-125">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="9b5f1-126">Ticari Market 'teki lisans tabanlı SaaS aboneliklerine yönelik kullanıcı lisanslarını eklemek veya kaldırmak için bkz. [SaaS aboneliği için lisans ekleme veya kaldırma](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span><span class="sxs-lookup"><span data-stu-id="9b5f1-126">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="9b5f1-127">Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-127">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="9b5f1-128">Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve listeden bir müşteri seçin.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-128">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="9b5f1-129">Müşteri menüsünde, **Kullanıcılar ve lisanslar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-129">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="9b5f1-130">Listeden bir veya daha fazla kullanıcı seçin.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-130">Choose one or more users from the list.</span></span> <span data-ttu-id="9b5f1-131">Örneğin, müşteri yeni lisanslar satın almış ve bunları henüz sahip olmayan kişilere atamak istediğinizde, doğru grubu bulmak için **kullanıcıları filtreleme...** seçeneğini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-131">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="9b5f1-132">**Lisansları Yönet**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-132">Select **Manage licenses**.</span></span> <span data-ttu-id="9b5f1-133">Değişikliklerinizi yapın ve **kaydedin**.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-133">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="9b5f1-134">[Azure Market ürünleri](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)için lisans atama ve etkinleştirme, ürünü yayımlayan bağımsız yazılım SATıCıSı (ISV) üzerinden yönetilir.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-134">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="9b5f1-135">Kullanıcının bir müşterinin parolasını sıfırlama</span><span class="sxs-lookup"><span data-stu-id="9b5f1-135">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="9b5f1-136">İş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-136">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="9b5f1-137">Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve listeden bir müşteri seçin.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-137">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="9b5f1-138">Müşteri menüsünde, **Kullanıcılar ve lisanslar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-138">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="9b5f1-139">Listeden kullanıcıyı seçin.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-139">Choose the user from the list.</span></span>

4. <span data-ttu-id="9b5f1-140">Ekranın alt kısmındaki **Parolayı Sıfırla**' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-140">At the bottom of the screen, select **Reset password**.</span></span> 

5. <span data-ttu-id="9b5f1-141">Yeni geçici parolayı kullanıcıya gönderin.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-141">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="9b5f1-142">Müşterinin Kullanıcı hesaplarını silme</span><span class="sxs-lookup"><span data-stu-id="9b5f1-142">Delete user accounts for a customer</span></span>

1. <span data-ttu-id="9b5f1-143">**Iş Ortağı Merkezi** menüsünde **müşteriler**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-143">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="9b5f1-144">Listeden müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-144">Choose the customer from the list.</span></span>

2. <span data-ttu-id="9b5f1-145">Müşteri menüsünde, **Kullanıcılar ve lisanslar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-145">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="9b5f1-146">Listeden kullanıcıyı seçin.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-146">Choose the user from the list.</span></span>

3. <span data-ttu-id="9b5f1-147">Ekranın alt kısmındaki **Kullanıcı hesabını Sil**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-147">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="9b5f1-148">Bu hesabı geri yüklemeniz gerekiyorsa, müşterinin **Kullanıcılar ve lisanslar** listesinin **silinen kullanıcılar** sekmesinde bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-148">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="9b5f1-149">Silinen bir kullanıcıyı geri yüklemek için 30 gününüz vardır.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-149">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="9b5f1-150">Silinen kullanıcı hesaplarını geri yükleme</span><span class="sxs-lookup"><span data-stu-id="9b5f1-150">Restore deleted user accounts</span></span>

1. <span data-ttu-id="9b5f1-151">**Iş Ortağı Merkezi** menüsünde **müşteriler**' i seçin ve ardından listeden müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-151">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2. <span data-ttu-id="9b5f1-152">**Kullanıcılar ve lisanslar ' ı** seçin.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-152">Select **Users and licenses**.</span></span>

3. <span data-ttu-id="9b5f1-153">**Silinen kullanıcılar ()** sekmesini seçin. Geri yüklenebilecek silinen kullanıcılar varsa, **(1)** veya daha büyük bir bilgi almalıdır.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-153">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4. <span data-ttu-id="9b5f1-154">Silinen kullanıcıların onay kutularından bir veya daha fazlasını seçin ve ardından **geri yükle**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-154">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="9b5f1-155">Tüm seçili kullanıcı hesapları, **Kullanıcılar ve lisanslar** sayfasında yeniden görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="9b5f1-155">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9b5f1-156">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="9b5f1-156">Next steps</span></span>

- [<span data-ttu-id="9b5f1-157">Birden fazla kullanıcıya lisans atama veya atanmış lisansları iptal etme</span><span class="sxs-lookup"><span data-stu-id="9b5f1-157">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

- [<span data-ttu-id="9b5f1-158">Müşteri hesabı için birden çok Kullanıcı oluşturma</span><span class="sxs-lookup"><span data-stu-id="9b5f1-158">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)