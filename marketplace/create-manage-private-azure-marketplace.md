---
title: Azure portal 'de özel Azure Marketi oluşturun ve yönetin
description: Azure portal özel Azure Marketi (Önizleme) oluşturma ve yönetme hakkında bilgi edinin. Özel Azure Marketi (Önizleme), yöneticilerin kullanıcıların hangi üçüncü taraf çözümlerini kullanabileceği konusunda yönetmelerini sağlar.
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 12/22/2020
ms.openlocfilehash: 09f7bcb29dc619e4e31c0aa3d5c73fade5218819
ms.sourcegitcommit: 30d154cdf40aa75400be7805cd9b2685b66a1382
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/24/2020
ms.locfileid: "97760867"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a><span data-ttu-id="125a2-104">Azure portal özel Azure Marketi (Önizleme) oluşturma ve yönetme</span><span class="sxs-lookup"><span data-stu-id="125a2-104">Create and manage Private Azure Marketplace (preview) in the Azure portal</span></span>

<span data-ttu-id="125a2-105">Özel Azure Marketi (Önizleme), yöneticilerin kullanıcıların hangi üçüncü taraf çözümlerini kullanabileceği konusunda yönetmelerini sağlar.</span><span class="sxs-lookup"><span data-stu-id="125a2-105">Private Azure Marketplace (preview) lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="125a2-106">Bunu, yalnızca onayladığınız ve kuruluşunuzun ilkelerine uygun olan teklifleri dağıtmanıza olanak tanıyarak yapar.</span><span class="sxs-lookup"><span data-stu-id="125a2-106">It does this by allowing you to deploy only offers that you approve and that comply with your enterprise's policies.</span></span> <span data-ttu-id="125a2-107">Özel Azure Marketi sayesinde kullanıcılarınız, satın alıp dağıtmak üzere çevrimiçi mağazalarla uyumlu teklifler arayabilir.</span><span class="sxs-lookup"><span data-stu-id="125a2-107">With Private Azure Marketplace, your users can search the online store for compliant offers to purchase and deploy.</span></span> 

<span data-ttu-id="125a2-108">Market Yöneticisi (atanan rol) olarak, onaylanan tekliflerinizi ve planlarınızı ekleyebileceğiniz devre dışı ve boş bir özel mağaza ile başlayacaksınız.</span><span class="sxs-lookup"><span data-stu-id="125a2-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="125a2-109">Bu makalede, kullanıcılarınız için özel Azure Marketi oluşturma, yönetme ve etkinleştirme işlemleri açıklanmaktadır.</span><span class="sxs-lookup"><span data-stu-id="125a2-109">This article explains how to create, manage, and enable Private Azure Marketplace for your users.</span></span>

<span data-ttu-id="125a2-110">Notlar:</span><span class="sxs-lookup"><span data-stu-id="125a2-110">Notes:</span></span>

- <span data-ttu-id="125a2-111">Özel Azure Marketi bir kiracı düzeyindedir, bu nedenle kiracı kapsamındaki tüm kullanıcılar aynı seçkin listeyi görür.</span><span class="sxs-lookup"><span data-stu-id="125a2-111">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
- <span data-ttu-id="125a2-112">Tüm Microsoft çözümleri özel Azure Marketi 'ne otomatik olarak eklenir.</span><span class="sxs-lookup"><span data-stu-id="125a2-112">All Microsoft solutions are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="125a2-113">Market yönetici rolünü atama</span><span class="sxs-lookup"><span data-stu-id="125a2-113">Assign the Marketplace admin role</span></span>

<span data-ttu-id="125a2-114">Kiracı Genel Yöneticisi, **Market yönetici** rolünü özel mağazayı yönetecek olan özel Azure Marketi yöneticisine atamalıdır.</span><span class="sxs-lookup"><span data-stu-id="125a2-114">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="125a2-115">Özel Azure Marketi yönetimine erişim yalnızca Market yönetici rolü atanmış BT yöneticileri tarafından kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="125a2-115">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="125a2-116">Ön koşullar</span><span class="sxs-lookup"><span data-stu-id="125a2-116">Prerequisites</span></span>

<span data-ttu-id="125a2-117">Kiracı kapsamındaki bir kullanıcıya Market yönetici rolünü atayabilmeniz için önce bu önkoşulları karşılamanız gerekir:</span><span class="sxs-lookup"><span data-stu-id="125a2-117">You must meet these prerequisites before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="125a2-118">Bir **genel yönetici** kullanıcısına erişiminiz var.</span><span class="sxs-lookup"><span data-stu-id="125a2-118">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="125a2-119">Kiracıda en az bir abonelik (herhangi bir tür olabilir) vardır.</span><span class="sxs-lookup"><span data-stu-id="125a2-119">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="125a2-120">Genel yönetici kullanıcısına, seçilen abonelik için **katkıda** bulunan rolü veya üzeri atanır.</span><span class="sxs-lookup"><span data-stu-id="125a2-120">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-iam"></a><span data-ttu-id="125a2-121">IAM ile Market yönetici rolünü atama</span><span class="sxs-lookup"><span data-stu-id="125a2-121">Assign the Marketplace admin role with IAM</span></span>

1. <span data-ttu-id="125a2-122">[Azure Portal](https://portal.azure.com/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="125a2-122">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
1. <span data-ttu-id="125a2-123">**Tüm hizmetler** ' i ve ardından **Market**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="125a2-123">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Ana pencere Azure portal.":::

3. <span data-ttu-id="125a2-125">Soldaki seçeneklerden **özel Market** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="125a2-125">Select **Private Marketplace** from the options on the left.</span></span>
1. <span data-ttu-id="125a2-126">Market yönetici rolünü atamak için **erişim denetimi (IAM)** seçeneğini belirleyin.</span><span class="sxs-lookup"><span data-stu-id="125a2-126">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="IAM erişim denetimi ekranı.":::

1. <span data-ttu-id="125a2-128">**+ Ekle** > **Rol ataması ekle**’yi seçin.</span><span class="sxs-lookup"><span data-stu-id="125a2-128">Select **+ Add** > **Add role assignment**.</span></span>
1. <span data-ttu-id="125a2-129">**Rol** altında **Market Yöneticisi**' ni seçin.</span><span class="sxs-lookup"><span data-stu-id="125a2-129">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Rol atama menüsü.":::

1. <span data-ttu-id="125a2-131">Açılan listeden istenen kullanıcıyı seçin, sonra **bitti**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="125a2-131">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="125a2-132">Market yönetici rolünü PowerShell ile atama</span><span class="sxs-lookup"><span data-stu-id="125a2-132">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="125a2-133">Market yönetici rolünü atamak için aşağıdaki PowerShell betiğini kullanın; Aşağıdaki parametreleri gerektirir:</span><span class="sxs-lookup"><span data-stu-id="125a2-133">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="125a2-134">**Tenantıd:** Kapsamdaki kiracının KIMLIĞI (Market yönetim rolü kiracı kapsamında atanabilir).</span><span class="sxs-lookup"><span data-stu-id="125a2-134">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="125a2-135">**Abonelik kimliği:** Genel yöneticiye **katkıda** bulunan rolü veya daha yüksek bir abonelik atanmış.</span><span class="sxs-lookup"><span data-stu-id="125a2-135">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="125a2-136">**GlobalAdminUsername:** Genel yöneticinin Kullanıcı adı.</span><span class="sxs-lookup"><span data-stu-id="125a2-136">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="125a2-137">**UsernameToAssignRoleFor:** Market yönetici rolü atanacak Kullanıcı adı.</span><span class="sxs-lookup"><span data-stu-id="125a2-137">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="125a2-138">Kiracıya davet edilen Konuk kullanıcılar için, bir hesabı Market yönetici rolü atama için kullanılabilir olana kadar 48 saat kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="125a2-138">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace admin role.</span></span> <span data-ttu-id="125a2-139">Daha fazla bilgi için bkz. [Azure ACTIVE DIRECTORY B2B işbirliği kullanıcısının özellikleri](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="125a2-139">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

```PowerShell
function Assign-MarketplaceAdminRole { 
[CmdletBinding()] 
param( 
[Parameter(Mandatory)] 
[string]$TenantId, 
 
[Parameter(Mandatory)] 
[string]$SubscriptionId, 

 

[Parameter(Mandatory)] 
[string]$GlobalAdminUsername, 

 

[Parameter(Mandatory)] 
[string]$UsernameToAssignRoleFor 
) 

$MarketplaceAdminRoleDefinitionName = "Marketplace Admin" 

 

Write-Output "TenantId = $TenantId" 
Write-Output "SubscriptionId = $SubscriptionId" 
Write-Output "GlobalAdminUsername = $GlobalAdminUsername" 
Write-Output "UsernameToAssignRoleFor = $UsernameToAssignRoleFor" 

 

Write-Output "$($GlobalAdminUsername) is about to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)" 

 

$profile = Connect-AzAccount -Tenant $TenantId -SubscriptionId $SubscriptionId

 

 
if($profile -eq $null) 
{ 
Write-Error -Message "Failed to connect to tenant and/or subscription" -ErrorAction Stop 
} 
elseif($profile.Context.Account.Id -ne $GlobalAdminUsername) 
{ 
Write-Error "Connected with $($profile.Context.Account.Id) instead of with the global admin that was specified in the script parameters, which is $($GlobalAdminUsername)" 
} 
else 
{ 
Write-Output "$($GlobalAdminUsername) was connected successfully to Tenant=$($profile.Context.Tenant), Subscription=$($profile.Context.Subscription), AccountId=$($profile.Context.Account.Id), Environment=$($profile.Context.Environment)" 
} 

 

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

 

if($MarketPlaceAdminRole -eq $null) 
{ 
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop 
} 
else 
{ 
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available" 
} 

 

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..." 

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace" 

} 

Assign-MarketplaceAdminRole 
```

<span data-ttu-id="125a2-140">Az. Portal PowerShell modülünde bulunan cmdlet 'ler hakkında daha fazla bilgi için bkz. [Microsoft Azure PowerShell: Portal panosu cmdlet 'leri](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="125a2-140">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="125a2-141">Özel Azure Marketi oluştur</span><span class="sxs-lookup"><span data-stu-id="125a2-141">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="125a2-142">[Azure Portal](https://portal.azure.com/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="125a2-142">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="125a2-143">**Tüm hizmetler** ' i ve ardından **Market**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="125a2-143">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Ana pencere Azure portal.":::

3. <span data-ttu-id="125a2-145">Soldaki seçeneklerden **özel Market** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="125a2-145">Select **Private Marketplace** from the options on the left.</span></span>

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Azure portal ana penceresinde özel Market seçme.":::

4. <span data-ttu-id="125a2-147">Özel Azure Marketi oluşturmak için **başlayın** ' ı seçin (bunu yalnızca bir kez yapmanız gerekir).</span><span class="sxs-lookup"><span data-stu-id="125a2-147">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Azure portal ana penceresinde Başlarken ' i seçin.":::

    <span data-ttu-id="125a2-149">Bu kiracı için özel Azure Marketi zaten mevcutsa Market 'i **Yönet** varsayılan olarak seçilidir.</span><span class="sxs-lookup"><span data-stu-id="125a2-149">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="125a2-150">Tamamlandıktan sonra boş ve devre dışı bir özel Azure Marketi olur.</span><span class="sxs-lookup"><span data-stu-id="125a2-150">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Boş özel Azure Marketi ekranı.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="125a2-152">Galeriden öğe Ekle</span><span class="sxs-lookup"><span data-stu-id="125a2-152">Add items from gallery</span></span>

<span data-ttu-id="125a2-153">Bir öğe, teklifin ve planın bir birleşimidir.</span><span class="sxs-lookup"><span data-stu-id="125a2-153">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="125a2-154">Market 'i Yönet sayfasında öğe arayabilir ve ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="125a2-154">You can search for and add item in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="125a2-155">**Öğe Ekle**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="125a2-155">Select **Add items**.</span></span>

2. <span data-ttu-id="125a2-156">**Galeriye** gözatıp istediğiniz öğeyi bulmak için arama alanını kullanın.</span><span class="sxs-lookup"><span data-stu-id="125a2-156">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Galeriye göz atma veya arama alanını kullanma.":::

3. <span data-ttu-id="125a2-158">Varsayılan olarak, yeni bir teklif eklenirken, tüm geçerli planlar izin verilenler listesine eklenir.</span><span class="sxs-lookup"><span data-stu-id="125a2-158">As default, when adding a new offer, all current plans will be added to the allowed list.</span></span> <span data-ttu-id="125a2-159">Seçilen öğeleri eklemeden önce plan seçimini değiştirmek için, teklifin kutucuğunda açılan menüyü seçin ve gerekli planları güncelleştirin.</span><span class="sxs-lookup"><span data-stu-id="125a2-159">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Gerekli planları güncelleştirin.":::

4. <span data-ttu-id="125a2-161">Seçimlerinizi yaptıktan sonra sol alttaki **bitti** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="125a2-161">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="125a2-162">Market 'e **öğe eklemek** yalnızca Microsoft dışı teklifler için kullanılabilir olacaktır.</span><span class="sxs-lookup"><span data-stu-id="125a2-162">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="125a2-163">Varsayılan olarak Microsoft tekliflere izin verilir.</span><span class="sxs-lookup"><span data-stu-id="125a2-163">Microsoft offers are allowed by default.</span></span>

## <a name="edit-item-plans"></a><span data-ttu-id="125a2-164">Öğe planlarını Düzenle</span><span class="sxs-lookup"><span data-stu-id="125a2-164">Edit item plans</span></span>

<span data-ttu-id="125a2-165">Market 'i Yönet sayfasında bir öğenin planlarını düzenleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="125a2-165">You can edit an item's plans in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="125a2-166">**Planlar** sütununda, bu öğenin açılan menüsünden kullanılabilir planları gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="125a2-166">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="125a2-167">Kullanıcılarınız için hangi planların kullanılabilir olduğunu seçmek için onay kutularını işaretleyin veya temizleyin.</span><span class="sxs-lookup"><span data-stu-id="125a2-167">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Gerekli öğe için onay kutusunu seçme veya temizleme.":::

> [!NOTE]
> <span data-ttu-id="125a2-169">Her teklifin, güncelleştirmenin gerçekleşmesi için en az bir plan seçilmiş olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="125a2-169">Each offer needs at least one plan selected in order for the update to occur.</span></span> <span data-ttu-id="125a2-170">Bir teklifle ilgili tüm planları kaldırmak için teklifin tamamını silin (sonraki bölüme bakın).</span><span class="sxs-lookup"><span data-stu-id="125a2-170">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="125a2-171">Teklifleri silme</span><span class="sxs-lookup"><span data-stu-id="125a2-171">Delete offers</span></span>

<span data-ttu-id="125a2-172">Market 'i Yönet sayfasında, teklif adının yanındaki onay kutusunu işaretleyin (yukarıdaki ekrana bakın) ve **öğeleri sil**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="125a2-172">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="125a2-173">Özel Azure Marketi 'ni etkinleştir/devre dışı bırak</span><span class="sxs-lookup"><span data-stu-id="125a2-173">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="125a2-174">Market 'i Yönet sayfasında, özel Azure Marketi 'nin geçerli durumunu gösteren bu başlık sayfasından birini görürsünüz:</span><span class="sxs-lookup"><span data-stu-id="125a2-174">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Durum başlığını devre dışı bırak":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Durum başlığını etkinleştir":::

<span data-ttu-id="125a2-177">Özel Azure Marketi 'ni gerektiği şekilde etkinleştirebilir veya devre dışı bırakabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="125a2-177">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="125a2-178">Devre dışı bırakılırsa, etkinleştirmek için **özel marketi etkinleştir** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="125a2-178">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="125a2-179">Etkinleştirilirse, devre dışı bırakmak için **özel marketi devre dışı bırak** seçeneğini belirleyin.</span><span class="sxs-lookup"><span data-stu-id="125a2-179">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="125a2-180">Özel Azure Marketi 'ne göz atma</span><span class="sxs-lookup"><span data-stu-id="125a2-180">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="125a2-181">Özel Azure Marketi etkinleştirildiğinde, kullanıcılar Market yöneticisinin hangi planlara izin verileceğini görür.</span><span class="sxs-lookup"><span data-stu-id="125a2-181">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has allowed.</span></span>

- <span data-ttu-id="125a2-182">Yeşil **izin** verilen bir bildirimde, izin verilen bir iş ortağı (Microsoft dışı) teklifi gösterilir.</span><span class="sxs-lookup"><span data-stu-id="125a2-182">A green **Allowed** notice indicates a Partner (non-Microsoft) offer that is allowed.</span></span>
- <span data-ttu-id="125a2-183">Bir mavi **izin** verilen bildirim, izin verilen bir Microsoft teklifini gösterir.</span><span class="sxs-lookup"><span data-stu-id="125a2-183">A blue **Allowed** notice indicates a Microsoft offer that is allowed.</span></span>

<span data-ttu-id="125a2-184">Kullanıcılar, ve izin verilmeyen teklifler arasında filtre uygulayabilir:</span><span class="sxs-lookup"><span data-stu-id="125a2-184">Users can filter between offers that are and are not allowed:</span></span>

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Filtreleme seçeneği.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="125a2-186">Özel Azure Marketi 'nde satın alın veya dağıtın</span><span class="sxs-lookup"><span data-stu-id="125a2-186">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="125a2-187">Ürün Ayrıntıları sayfası deneyimi Genel Azure Marketi 'ne benzer olsa da, özel Azure Market 'e özgü üç senaryo vardır.</span><span class="sxs-lookup"><span data-stu-id="125a2-187">While the product details page experience is similar to the public Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="125a2-188">Kullanıcı izin verilen bir planı seçtiğinde **Oluştur** düğmesi etkinleştirilir:</span><span class="sxs-lookup"><span data-stu-id="125a2-188">When a user selects an allowed plan, the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Bir planın oluşturulabileceği teklif başlığı.":::

- <span data-ttu-id="125a2-190">Kullanıcı izin verilmeyen bir plan seçtiğinde, plana izin verilmeyen bir başlık ve **Oluştur** düğmesi devre dışı bırakılır.</span><span class="sxs-lookup"><span data-stu-id="125a2-190">When a user selects a non-allowed plan, a banner notes that the plan is not allowed and the **Create** button is disabled.</span></span>

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Bir plana dikkat eden teklif başlığı oluşturulamıyor.":::

- <span data-ttu-id="125a2-192">Ürün planı seçimi ürün ayrıntıları sayfasında görünmezse, ancak yönetici bir veya daha fazla planı onayladıysa, bir başlık, planlara izin verilen ve **Oluştur** düğmesi etkin olur:</span><span class="sxs-lookup"><span data-stu-id="125a2-192">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are allowed and the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Bir planın oluşturulup kullanılabilir planları göstermediğini gösteren bir başlık sunar.":::

## <a name="contact-support"></a><span data-ttu-id="125a2-194">Desteğe başvurun</span><span class="sxs-lookup"><span data-stu-id="125a2-194">Contact support</span></span>

<span data-ttu-id="125a2-195">Azure Marketi desteği için [Microsoft Q&A](/answers/products/)adresini ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="125a2-195">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span> 
