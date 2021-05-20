---
title: Müşteri hesapları için kullanıcıları yönetme
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: İş Ortağı Merkezi'da müşterileriniz için kullanıcıları yönetme- kullanıcı hesapları oluşturun, kullanıcı lisansları ekleyin veya kaldırın, parolaları sıfırlayın ve kullanıcı hesaplarını silin veya geri yükleme.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc896ec3ce16ab0f05a8131de14f573ad96a8141
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149902"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="65bd4-103">Müşteri hesapları için kullanıcıları ve kullanıcı lisanslarını yönetme</span><span class="sxs-lookup"><span data-stu-id="65bd4-103">Manage users and user licenses for customer accounts</span></span> 

<span data-ttu-id="65bd4-104">**Uygun roller:** Genel yönetici | Kullanıcı yönetimi yönetici | Yönetici aracısı</span><span class="sxs-lookup"><span data-stu-id="65bd4-104">**Appropriate roles**: Global admin | User management admin | Admin agent</span></span>


<span data-ttu-id="65bd4-105">Müşterinin hesabında yeni kullanıcılar oluşturabilir ve silebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="65bd4-105">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="65bd4-106">Daha önce sildikten sonra 30 gün içinde silmiş olduğunu bir veya daha fazla kullanıcı hesabını da geri yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="65bd4-106">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="65bd4-107">Kullanıcının önceki abonelik atamaları da geri yüklenir (önceki ayırmalarının kullanılabilir olduğu varsayıldı).</span><span class="sxs-lookup"><span data-stu-id="65bd4-107">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="65bd4-108">Bir müşteri için yeni abonelikler satın alırsanız, müşteri size hesap, kullanıcı izinleri ve her kullanıcının hangi hizmetlere ihtiyacı olacak olan tüm kullanıcıların listesini versin.</span><span class="sxs-lookup"><span data-stu-id="65bd4-108">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

>[!NOTE]
><span data-ttu-id="65bd4-109">Müşteri **sekmesinin Kullanıcılar**  ve lisanslar bölümünde, başka bir CSP iş ortağından veya başka bir satın alma kanalından satın alınan lisanslara sahip kullanıcılar da dahil olmak üzere belirli bir müşterinin kiracısı içinde oluşturulan tüm kullanıcılar görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="65bd4-109">The **Users and licenses** section of **Customer** tab shows all users created in a specific customer’s tenant, including users that have licenses purchased from another CSP partner or from another purchasing channel.</span></span>

<span data-ttu-id="65bd4-110">Excel ile [uyumlu bir](bulk-license-provisioning-for-multiple-users.md) .csv elektronik tablo dosyası kullanarak adları içeri aktararak birden çok kullanıcıya [abonelik atabilirsiniz.](adding-multiple-users-to-a-customer-account.md)</span><span class="sxs-lookup"><span data-stu-id="65bd4-110">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="65bd4-111">Müşteri için kullanıcı hesapları oluşturma</span><span class="sxs-lookup"><span data-stu-id="65bd4-111">Create user accounts for a customer</span></span>

1. <span data-ttu-id="65bd4-112">İş Ortağı Merkezi [oturum açın.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="65bd4-112">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="65bd4-113">Yeni İş Ortağı Merkezi **Müşteriler'i** ve ardından listeden bir müşteri seçin.</span><span class="sxs-lookup"><span data-stu-id="65bd4-113">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="65bd4-114">Müşteri menüsünde Kullanıcılar ve **lisanslar'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="65bd4-114">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="65bd4-115">Ekleyilen her kullanıcı için Abonelik **ekle'yi** seçin ve ardından izinler ve lisanslar dahil olmak üzere bilgileri doldurun.</span><span class="sxs-lookup"><span data-stu-id="65bd4-115">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="65bd4-116">**Değişikliklerinizi** kaydedin.</span><span class="sxs-lookup"><span data-stu-id="65bd4-116">**Save** your changes.</span></span>

5. <span data-ttu-id="65bd4-117">Kullanıcıya göndermek için kullanıcı adını ve geçici parolayı kaydetmeyi emin olun.</span><span class="sxs-lookup"><span data-stu-id="65bd4-117">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="65bd4-118">Bir defada birden çok kullanıcı ekliyorsanız Başka bir kullanıcı **ekle'yi kullanın.**</span><span class="sxs-lookup"><span data-stu-id="65bd4-118">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="65bd4-119">Excel ile uyumlu bir .csv elektronik tablo [dosyasını içeri aktararak aynı anda birden çok kullanıcı abilirsiniz.](adding-multiple-users-to-a-customer-account.md)</span><span class="sxs-lookup"><span data-stu-id="65bd4-119">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="65bd4-120">Onay ekranından adları ve parolaları e-posta ile göndermeden veya yazdırmadan önce tüm kümeyi tamamlaya kadar bekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="65bd4-120">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="65bd4-121">Müşteri için kullanıcı lisanslarını ekleme veya kaldırma</span><span class="sxs-lookup"><span data-stu-id="65bd4-121">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="65bd4-122">Aşağıdaki adımlar, Microsoft ürünleri için kullanıcı lisansları eklemek veya kaldırmak için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="65bd4-122">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="65bd4-123">Ticari Market 'teki lisans tabanlı SaaS aboneliklerine yönelik kullanıcı lisanslarını eklemek veya kaldırmak için bkz. [SaaS aboneliği için lisans ekleme veya kaldırma](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span><span class="sxs-lookup"><span data-stu-id="65bd4-123">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="65bd4-124">Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="65bd4-124">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="65bd4-125">Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve listeden bir müşteri seçin.</span><span class="sxs-lookup"><span data-stu-id="65bd4-125">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="65bd4-126">Müşteri menüsünde, **Kullanıcılar ve lisanslar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="65bd4-126">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="65bd4-127">Listeden bir veya birden fazla kullanıcı seçin.</span><span class="sxs-lookup"><span data-stu-id="65bd4-127">Choose one or more users from the list.</span></span> <span data-ttu-id="65bd4-128">Örneğin, müşteri yeni lisanslar satın almış ve bunları henüz sahip olmayan kişilere atamak istediğinizde, doğru grubu bulmak için **kullanıcıları filtreleme...** seçeneğini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="65bd4-128">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="65bd4-129">**Lisansları Yönet**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="65bd4-129">Select **Manage licenses**.</span></span> <span data-ttu-id="65bd4-130">Değişikliklerinizi yapın ve **kaydedin**.</span><span class="sxs-lookup"><span data-stu-id="65bd4-130">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="65bd4-131">[Azure Market ürünleri](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)için lisans atama ve etkinleştirme, ürünü yayımlayan bağımsız yazılım SATıCıSı (ISV) üzerinden yönetilir.</span><span class="sxs-lookup"><span data-stu-id="65bd4-131">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="65bd4-132">Kullanıcının bir müşterinin parolasını sıfırlama</span><span class="sxs-lookup"><span data-stu-id="65bd4-132">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="65bd4-133">İş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="65bd4-133">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="65bd4-134">Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve listeden bir müşteri seçin.</span><span class="sxs-lookup"><span data-stu-id="65bd4-134">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="65bd4-135">Müşteri menüsünde, **Kullanıcılar ve lisanslar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="65bd4-135">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="65bd4-136">Listeden kullanıcıyı seçin.</span><span class="sxs-lookup"><span data-stu-id="65bd4-136">Choose the user from the list.</span></span>

4. <span data-ttu-id="65bd4-137">Ekranın alt kısmındaki **Parolayı Sıfırla**' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="65bd4-137">At the bottom of the screen, select **Reset password**.</span></span> 

5. <span data-ttu-id="65bd4-138">Yeni geçici parolayı kullanıcıya gönderin.</span><span class="sxs-lookup"><span data-stu-id="65bd4-138">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="65bd4-139">Müşterinin Kullanıcı hesaplarını silme</span><span class="sxs-lookup"><span data-stu-id="65bd4-139">Delete user accounts for a customer</span></span>

1. <span data-ttu-id="65bd4-140">**Iş Ortağı Merkezi** menüsünde **müşteriler**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="65bd4-140">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="65bd4-141">Listeden müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="65bd4-141">Choose the customer from the list.</span></span>

2. <span data-ttu-id="65bd4-142">Müşteri menüsünde, **Kullanıcılar ve lisanslar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="65bd4-142">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="65bd4-143">Listeden kullanıcıyı seçin.</span><span class="sxs-lookup"><span data-stu-id="65bd4-143">Choose the user from the list.</span></span>

3. <span data-ttu-id="65bd4-144">Ekranın alt kısmındaki **Kullanıcı hesabını Sil**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="65bd4-144">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="65bd4-145">Bu hesabı geri yüklemeniz gerekiyorsa, müşterinin **Kullanıcılar ve lisanslar** listesinin **silinen kullanıcılar** sekmesinde bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="65bd4-145">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="65bd4-146">Silinen bir kullanıcıyı geri yüklemek için 30 gününüz vardır.</span><span class="sxs-lookup"><span data-stu-id="65bd4-146">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="65bd4-147">Silinen kullanıcı hesaplarını geri yükleme</span><span class="sxs-lookup"><span data-stu-id="65bd4-147">Restore deleted user accounts</span></span>

1. <span data-ttu-id="65bd4-148">**Iş Ortağı Merkezi** menüsünde **müşteriler**' i seçin ve ardından listeden müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="65bd4-148">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2. <span data-ttu-id="65bd4-149">**Kullanıcılar ve lisanslar ' ı** seçin.</span><span class="sxs-lookup"><span data-stu-id="65bd4-149">Select **Users and licenses**.</span></span>

3. <span data-ttu-id="65bd4-150">**Silinen kullanıcılar ()** sekmesini seçin. Geri yüklenebilecek silinen kullanıcılar varsa, **(1)** veya daha büyük bir bilgi almalıdır.</span><span class="sxs-lookup"><span data-stu-id="65bd4-150">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4. <span data-ttu-id="65bd4-151">Silinen kullanıcıların onay kutularından bir veya daha fazlasını seçin ve ardından **geri yükle**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="65bd4-151">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="65bd4-152">Tüm seçili kullanıcı hesapları, **Kullanıcılar ve lisanslar** sayfasında yeniden görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="65bd4-152">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="65bd4-153">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="65bd4-153">Next steps</span></span>

- [<span data-ttu-id="65bd4-154">Birden fazla kullanıcıya lisans atama veya atanmış lisansları iptal etme</span><span class="sxs-lookup"><span data-stu-id="65bd4-154">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

- [<span data-ttu-id="65bd4-155">Müşteri hesabı için birden çok Kullanıcı oluşturma</span><span class="sxs-lookup"><span data-stu-id="65bd4-155">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)