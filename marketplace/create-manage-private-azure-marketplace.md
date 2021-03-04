---
title: Azure portal özel Azure Marketi oluşturun ve yönetin
description: Azure portal özel Azure Marketi (Önizleme) oluşturma ve yönetme hakkında bilgi edinin. Özel Azure Marketi (Önizleme), yöneticilerin kullanıcıların hangi üçüncü taraf çözümlerini kullanabileceği konusunda yönetmelerini sağlar.
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 73b9137728fba93704d9b0cb2bc93a3f6498bd90
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756922"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="4400c-104">Azure portal özel Azure Marketi oluşturun ve yönetin</span><span class="sxs-lookup"><span data-stu-id="4400c-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="4400c-105">Özel Azure Marketi, yöneticilerin kullanıcılarının kullanabileceği üçüncü taraf çözümlerini yönetmelerini sağlar.</span><span class="sxs-lookup"><span data-stu-id="4400c-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="4400c-106">Bu, kullanıcının yalnızca yönetici tarafından onaylanan ve kuruluşunuzun ilkelerine uygun olan teklifleri dağıtmalarına izin vererek bunu yapar.</span><span class="sxs-lookup"><span data-stu-id="4400c-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="4400c-107">Özel Azure Marketi sayesinde kullanıcılar, satın alıp dağıtmak üzere çevrimiçi mağazalarla uyumlu teklifler arayabilir.</span><span class="sxs-lookup"><span data-stu-id="4400c-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="4400c-108">Market Yöneticisi (atanan rol) olarak, onaylanan tekliflerinizi ve planlarınızı ekleyebileceğiniz devre dışı ve boş bir özel mağaza ile başlayacaksınız.</span><span class="sxs-lookup"><span data-stu-id="4400c-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="4400c-109">Bu makalede, gerekli rolün nasıl atanacağı, özel bir mağaza oluşturulması, öğelerin yönetilmesi, kullanıcı isteklerinin onaylanması ve kullanıcılarınız için özel Azure Marketi 'nin nasıl etkinleştirileceği açıklanır.</span><span class="sxs-lookup"><span data-stu-id="4400c-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="4400c-110">Özel Azure Marketi bir kiracı düzeyindedir, bu nedenle kiracı kapsamındaki tüm kullanıcılar aynı seçkin listeyi görür.</span><span class="sxs-lookup"><span data-stu-id="4400c-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="4400c-111">Tüm Microsoft çözümleri ( [onaylı Linux dağıtımları](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)dahil), özel Azure Marketi 'ne otomatik olarak eklenir.</span><span class="sxs-lookup"><span data-stu-id="4400c-111">All Microsoft solutions (including [Endorsed Linux Distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="4400c-112">Market yönetici rolünü atama</span><span class="sxs-lookup"><span data-stu-id="4400c-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="4400c-113">Kiracı Genel Yöneticisi, **Market yönetici** rolünü özel mağazayı yönetecek olan özel Azure Marketi yöneticisine atamalıdır.</span><span class="sxs-lookup"><span data-stu-id="4400c-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="4400c-114">Özel Azure Marketi yönetimine erişim yalnızca Market yönetici rolü atanmış BT yöneticileri tarafından kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="4400c-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="4400c-115">Önkoşullar</span><span class="sxs-lookup"><span data-stu-id="4400c-115">Prerequisites</span></span>

<span data-ttu-id="4400c-116">Bu Önkoşullar, kiracı kapsamındaki bir kullanıcıya Market yönetici rolünü atayabilmeniz için gereklidir:</span><span class="sxs-lookup"><span data-stu-id="4400c-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="4400c-117">Bir **genel yönetici** kullanıcısına erişiminiz var.</span><span class="sxs-lookup"><span data-stu-id="4400c-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="4400c-118">Kiracıda en az bir abonelik (herhangi bir tür olabilir) vardır.</span><span class="sxs-lookup"><span data-stu-id="4400c-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="4400c-119">Genel yönetici kullanıcısına, seçilen abonelik için **katkıda** bulunan rolü veya üzeri atanır.</span><span class="sxs-lookup"><span data-stu-id="4400c-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="4400c-120">Erişim denetimi (ıAM) ile Market yönetici rolünü atama</span><span class="sxs-lookup"><span data-stu-id="4400c-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="4400c-121">[Azure portalında](https://portal.azure.com/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="4400c-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
1. <span data-ttu-id="4400c-122">**Tüm hizmetler** ' i ve ardından **Market**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="4400c-122">Select **All services** and then **Marketplace**.</span></span>
1. <span data-ttu-id="4400c-123">Sol taraftaki menüden **özel Market** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="4400c-123">Select **Private Marketplace** from the menu on the left.</span></span>

    <span data-ttu-id="4400c-124">[![Market 'in sol tarafındaki özel Market menü seçeneğini gösterir.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4400c-124">[![Shows the private marketplace menu option on the left side of the Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span></span>

1. <span data-ttu-id="4400c-125">Market yönetici rolünü atamak için **erişim denetimi (IAM)** seçeneğini belirleyin.</span><span class="sxs-lookup"><span data-stu-id="4400c-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="M-M erişim denetimi ekranını gösterir.":::

1. <span data-ttu-id="4400c-127">**+ Ekle** > **Rol ataması ekle**’yi seçin.</span><span class="sxs-lookup"><span data-stu-id="4400c-127">Select **+ Add** > **Add role assignment**.</span></span>
1. <span data-ttu-id="4400c-128">**Rol** altında **Market Yöneticisi**' ni seçin.</span><span class="sxs-lookup"><span data-stu-id="4400c-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Rol atama menüsünü gösterir.":::

1. <span data-ttu-id="4400c-130">Açılan listeden istenen kullanıcıyı seçin, sonra **bitti**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="4400c-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="4400c-131">Market yönetici rolünü PowerShell ile atama</span><span class="sxs-lookup"><span data-stu-id="4400c-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="4400c-132">Market yönetici rolünü atamak için aşağıdaki PowerShell betiğini kullanın; Aşağıdaki parametreleri gerektirir:</span><span class="sxs-lookup"><span data-stu-id="4400c-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="4400c-133">**Tenantıd:** Kapsamdaki kiracının KIMLIĞI (Market yönetim rolü kiracı kapsamında atanabilir).</span><span class="sxs-lookup"><span data-stu-id="4400c-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="4400c-134">**Abonelik kimliği:** Genel yöneticiye **katkıda** bulunan rolü veya daha yüksek bir abonelik atanmış.</span><span class="sxs-lookup"><span data-stu-id="4400c-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="4400c-135">**GlobalAdminUsername:** Genel yöneticinin Kullanıcı adı.</span><span class="sxs-lookup"><span data-stu-id="4400c-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="4400c-136">**UsernameToAssignRoleFor:** Market yönetici rolü atanacak Kullanıcı adı.</span><span class="sxs-lookup"><span data-stu-id="4400c-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="4400c-137">Kiracıya davet edilen Konuk kullanıcılar için, bir hesabı Market yönetici rolü atama için kullanılabilir olana kadar 48 saat kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="4400c-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="4400c-138">Daha fazla bilgi için bkz. [Azure ACTIVE DIRECTORY B2B işbirliği kullanıcısının özellikleri](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="4400c-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="4400c-139">Az. Portal PowerShell modülünde bulunan cmdlet 'ler hakkında daha fazla bilgi için bkz. [Microsoft Azure PowerShell: Portal panosu cmdlet 'leri](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="4400c-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="4400c-140">Özel Azure Marketi oluştur</span><span class="sxs-lookup"><span data-stu-id="4400c-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="4400c-141">[Azure portalında](https://portal.azure.com/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="4400c-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="4400c-142">**Tüm hizmetler** ' i ve ardından **Market**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="4400c-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Ana pencereyi Azure portal gösterir.":::

3. <span data-ttu-id="4400c-144">Sol taraftaki menüden **özel Market** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="4400c-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="4400c-145">Özel Azure Marketi oluşturmak için **başlayın** ' ı seçin (bunu yalnızca bir kez yapmanız gerekir).</span><span class="sxs-lookup"><span data-stu-id="4400c-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="' Azure portal ' ın ana penceresindeki ' kullanmaya başlayın ' seçeneğini nasıl kullanacağınızı gösterir.":::

    <span data-ttu-id="4400c-147">Bu kiracı için özel Azure Marketi zaten mevcutsa Market 'i **Yönet** varsayılan olarak seçilidir.</span><span class="sxs-lookup"><span data-stu-id="4400c-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="4400c-148">Tamamlandıktan sonra boş ve devre dışı bir özel Azure Marketi olur.</span><span class="sxs-lookup"><span data-stu-id="4400c-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Boş özel Azure Marketi ekranını gösterir.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="4400c-150">Galeriden öğe Ekle</span><span class="sxs-lookup"><span data-stu-id="4400c-150">Add items from gallery</span></span>

<span data-ttu-id="4400c-151">Bir öğe, teklifin ve planın bir birleşimidir.</span><span class="sxs-lookup"><span data-stu-id="4400c-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="4400c-152">Market 'i Yönet sayfasında öğeleri arayabilir ve ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4400c-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="4400c-153">**Öğe Ekle**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="4400c-153">Select **Add items**.</span></span>

2. <span data-ttu-id="4400c-154">**Galeriye** gözatıp istediğiniz öğeyi bulmak için arama alanını kullanın.</span><span class="sxs-lookup"><span data-stu-id="4400c-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    <span data-ttu-id="4400c-155">[![Galeriye gözatmaya veya arama alanını nasıl kullanacağınızı gösterir.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4400c-155">[![Shows how to browse the gallery or use the search field.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span></span>

3. <span data-ttu-id="4400c-156">Varsayılan olarak, yeni bir teklif eklerken, tüm geçerli planlar onaylanan listeye eklenecektir.</span><span class="sxs-lookup"><span data-stu-id="4400c-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="4400c-157">Seçilen öğeleri eklemeden önce plan seçimini değiştirmek için, teklifin kutucuğunda açılan menüyü seçin ve gerekli planları güncelleştirin.</span><span class="sxs-lookup"><span data-stu-id="4400c-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Gerekli planların nasıl güncelleştirilmesini gösterir.":::

4. <span data-ttu-id="4400c-159">Seçimlerinizi yaptıktan sonra sol alttaki **bitti** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="4400c-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="4400c-160">Market 'e **öğe eklemek** yalnızca Microsoft dışı teklifler için kullanılabilir olacaktır.</span><span class="sxs-lookup"><span data-stu-id="4400c-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="4400c-161">Microsoft Solutions ( [onaylı Linux dağıtımları](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)dahil) "varsayılan olarak onaylandı" olarak etiketlenecek ve özel Market 'te yönetilemez.</span><span class="sxs-lookup"><span data-stu-id="4400c-161">Microsoft solutions (including [Endorsed Linux Distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) will be tagged as “Approved by default” and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="4400c-162">Öğenin planlarını Düzenle</span><span class="sxs-lookup"><span data-stu-id="4400c-162">Edit item's plans</span></span>

<span data-ttu-id="4400c-163">Bir öğenin planlarını Market yönetimi sayfasında düzenleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4400c-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="4400c-164">**Planlar** sütununda, bu öğenin açılan menüsünden kullanılabilir planları gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="4400c-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="4400c-165">Kullanıcılarınız için hangi planların kullanılabilir olduğunu seçmek için onay kutularını işaretleyin veya temizleyin.</span><span class="sxs-lookup"><span data-stu-id="4400c-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Gerekli öğe için onay kutusunu seçme veya temizleme işlemlerinin nasıl yapılacağını gösterir.":::

> [!NOTE]
> <span data-ttu-id="4400c-167">Her teklifin, güncelleştirmenin gerçekleşmesi için en az bir plan seçilmiş olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="4400c-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="4400c-168">Bir teklifle ilgili tüm planları kaldırmak için teklifin tamamını silin (sonraki bölüme bakın).</span><span class="sxs-lookup"><span data-stu-id="4400c-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="4400c-169">Teklifleri silme</span><span class="sxs-lookup"><span data-stu-id="4400c-169">Delete offers</span></span>

<span data-ttu-id="4400c-170">Market 'i Yönet sayfasında, teklif adının yanındaki onay kutusunu işaretleyin (yukarıdaki ekrana bakın) ve **öğeleri sil**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="4400c-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="4400c-171">Özel Azure Marketi 'ni etkinleştir/devre dışı bırak</span><span class="sxs-lookup"><span data-stu-id="4400c-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="4400c-172">Market 'i Yönet sayfasında, özel Azure Marketi 'nin geçerli durumunu gösteren bu başlık sayfasından birini görürsünüz:</span><span class="sxs-lookup"><span data-stu-id="4400c-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="' Durumu devre dışı bırak ' başlığını gösterir.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="' Durumu etkinleştir ' başlığını gösterir.":::

<span data-ttu-id="4400c-175">Özel Azure Marketi 'ni gerektiği şekilde etkinleştirebilir veya devre dışı bırakabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4400c-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="4400c-176">Devre dışı bırakılırsa, etkinleştirmek için **özel marketi etkinleştir** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="4400c-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="4400c-177">Etkinleştirilirse, devre dışı bırakmak için **özel marketi devre dışı bırak** seçeneğini belirleyin.</span><span class="sxs-lookup"><span data-stu-id="4400c-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="4400c-178">Özel Azure Marketi Bildirim Merkezi</span><span class="sxs-lookup"><span data-stu-id="4400c-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="4400c-179">Bildirim Merkezi üç tür bildirimden oluşur ve Market yöneticisinin bildirime göre eylem almasına izin verir:</span><span class="sxs-lookup"><span data-stu-id="4400c-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="4400c-180">Onaylanan listede olmayan öğeler için kullanıcılardan onay istekleri (bkz. [teklif veya plan ekleme isteği](#request-to-add-offers-or-plans) ).</span><span class="sxs-lookup"><span data-stu-id="4400c-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="4400c-181">Onaylanan listede zaten bir veya daha fazla plana sahip olan tekliflere yönelik yeni plan bildirimleri.</span><span class="sxs-lookup"><span data-stu-id="4400c-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="4400c-182">Onaylanan listede bulunan ancak genel Azure Marketi 'nden kaldırılan öğeler için plan bildirimleri kaldırıldı.</span><span class="sxs-lookup"><span data-stu-id="4400c-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="4400c-183">Bildirim merkezine erişmek için:</span><span class="sxs-lookup"><span data-stu-id="4400c-183">To access the notification center:</span></span>

1. <span data-ttu-id="4400c-184">Sol taraftaki menüden **Bildirimler** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="4400c-184">Select **Notifications** from the left-side menu.</span></span>

    <span data-ttu-id="4400c-185">[![Bildirimler menüsünü gösterir.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4400c-185">[![Shows the Notifications menu.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span></span>

1. <span data-ttu-id="4400c-186">Daha fazla eylem için üç nokta menüsünü seçin.</span><span class="sxs-lookup"><span data-stu-id="4400c-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Diğer Seçenekler menüsü sonuçlarını gösterir.":::

1. <span data-ttu-id="4400c-188">Plan istekleri için **Istekleri göster** , belirli bir teklifin tüm Kullanıcı isteklerini gözden geçirebileceğiniz onay isteği formunu açar.</span><span class="sxs-lookup"><span data-stu-id="4400c-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="4400c-189">**Onayla** veya **Reddet**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="4400c-189">Select **Approve** or **Reject**.</span></span>

    <span data-ttu-id="4400c-190">[![Onaylama ve reddetme seçeneklerini gösterir.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4400c-190">[![Shows the approve and reject options.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span></span>

1. <span data-ttu-id="4400c-191">Açılan menüden onaylanacak planı seçin.</span><span class="sxs-lookup"><span data-stu-id="4400c-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="4400c-192">Bir açıklama ekleyin ve **Gönder**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="4400c-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="4400c-193">Özel Azure Marketi 'ne göz atma</span><span class="sxs-lookup"><span data-stu-id="4400c-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="4400c-194">Özel Azure Marketi etkinleştirildiğinde, kullanıcılar Market yöneticisinin hangi planları onayladığını görür.</span><span class="sxs-lookup"><span data-stu-id="4400c-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="4400c-195">Yeşil **onaylı** bir bildirimde, onaylanan iş ortağı (Microsoft dışı) teklifi gösterilir.</span><span class="sxs-lookup"><span data-stu-id="4400c-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="4400c-196">Mavi **onaylanmış** bir bildirim, onaylanan bir Microsoft teklifini (onaylanmış [Linux dağıtımları](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)dahil) gösterir.</span><span class="sxs-lookup"><span data-stu-id="4400c-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="4400c-197">Kullanıcılar, ve onaylanmamış teklifler arasında filtre uygulayabilir:</span><span class="sxs-lookup"><span data-stu-id="4400c-197">Users can filter between offers that are and are not approved:</span></span>

<span data-ttu-id="4400c-198">[![Filtreleme seçeneğini gösterir.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4400c-198">[![Shows the filtering option.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span></span>

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="4400c-199">Özel Azure Marketi 'nde satın alın veya dağıtın</span><span class="sxs-lookup"><span data-stu-id="4400c-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="4400c-200">Ürün Ayrıntıları sayfası deneyimi küresel Azure Marketi 'ne benzer olsa da, özel Azure Market 'e özgü üç senaryo vardır.</span><span class="sxs-lookup"><span data-stu-id="4400c-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="4400c-201">Bir Kullanıcı onaylanan bir planı seçtiğinde **Oluştur** düğmesi etkinleştirilir:</span><span class="sxs-lookup"><span data-stu-id="4400c-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

    <span data-ttu-id="4400c-202">[![Bir planın oluşturulabileceği teklif başlığını gösterir.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4400c-202">[![Shows the offer banner noting a plan can be created.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span></span>

- <span data-ttu-id="4400c-203">Ürün planı seçimi ürün ayrıntıları sayfasında görünmezse ancak yönetici bir veya daha fazla planı onayladıysa, bir başlık hangi planların onaylandığını ve **Oluştur** düğmesi etkin ' i not edin:</span><span class="sxs-lookup"><span data-stu-id="4400c-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

    <span data-ttu-id="4400c-204">[![Bir planın oluşturulup kullanılabilir planların gösterilmediğini belirten teklif başlığını gösterir.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4400c-204">[![Shows the offer banner noting that a plan can be created and showing available plans.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span></span>

- <span data-ttu-id="4400c-205">Kullanıcı onaylanmamış bir plan seçtiğinde, bir başlık planı onaylanmamış olarak not edin ve **Oluştur** düğmesi devre dışıdır.</span><span class="sxs-lookup"><span data-stu-id="4400c-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="4400c-206">Kullanıcı yine de planı onaylanan listeye ekleme isteğinde bulunabilir (sonraki bölüme bakın).</span><span class="sxs-lookup"><span data-stu-id="4400c-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="4400c-207">Teklif veya plan ekleme isteği</span><span class="sxs-lookup"><span data-stu-id="4400c-207">Request to add offers or plans</span></span>

<span data-ttu-id="4400c-208">Özel Azure Marketi 'nde Şu anda onaylanmamış olan bir genel teklif veya plan ekleme isteyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4400c-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="4400c-209">**Erişim isteği formunu** açmak için başlıkta **eklenecek isteği** seçin.</span><span class="sxs-lookup"><span data-stu-id="4400c-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

    <span data-ttu-id="4400c-210">[![' Ekleme Isteği ' bağlantısı olan başlığı gösterir.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4400c-210">[![Shows the banner with the 'Request to add' link.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span></span>

    <span data-ttu-id="4400c-211">[![Teklifler veya planlar için erişim isteği formunu gösterir.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4400c-211">[![Shows the access request form for offers or plans.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span></span>

1. <span data-ttu-id="4400c-212">İsteğe hangi planların ekleneceğini seçin (**herhangi bir plan** , Market yöneticisine bir teklif içindeki bir plan için bir tercih olmadığını söyler).</span><span class="sxs-lookup"><span data-stu-id="4400c-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="4400c-213">İsteğinizi göndermek için bir **gerekçe** ve seçme **isteği** ekleyin.</span><span class="sxs-lookup"><span data-stu-id="4400c-213">Add a **Justification** and select **Request** to submit your request.</span></span>
  
    <span data-ttu-id="4400c-214">[![Örnek girişleri olan tekliflere veya planlara yönelik erişim isteği formunu gösterir.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4400c-214">[![Shows the access request form for offers or plans with sample entries.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span></span>

1. <span data-ttu-id="4400c-215">Bekleyen bir istek için gösterge, **istek geri çekme** seçeneğiyle birlikte erişim isteği formunda görünür.</span><span class="sxs-lookup"><span data-stu-id="4400c-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

    <span data-ttu-id="4400c-216">[![Geri çekme Isteği bağlantısıyla onaylanan veya bekleyen planların listesini gösterir.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4400c-216">[![Shows a list of approved or pending plans with Withdraw Request link.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span></span>

> [!NOTE]
> <span data-ttu-id="4400c-217">Gönderildikten sonra, onay isteği formu Market yöneticisinin isteği gözden geçirmesi ve işlem yapması için [bildirim merkezine](#private-azure-marketplace-notification-center) gönderilir.</span><span class="sxs-lookup"><span data-stu-id="4400c-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="4400c-218">Sık sorulan sorular (SSS)</span><span class="sxs-lookup"><span data-stu-id="4400c-218">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="4400c-219">Azure Ilkesi aracılığıyla Market üçüncü taraf uygulamasını zaten engelliyor.</span><span class="sxs-lookup"><span data-stu-id="4400c-219">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="4400c-220">Bu farklı midir?</span><span class="sxs-lookup"><span data-stu-id="4400c-220">How is this different?</span></span>

<span data-ttu-id="4400c-221">Market 'te üçüncü taraf hizmetleri kısıtlamak için şu anda iki yol vardır:</span><span class="sxs-lookup"><span data-stu-id="4400c-221">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="4400c-222">EA Portalı veya Azure portal aracılığıyla, üçüncü taraf hizmetleri devre dışı bırakın veya yalnızca "ücretsiz veya KLG SKU 'Ları" ile kısıtlayın.</span><span class="sxs-lookup"><span data-stu-id="4400c-222">Through EA portal or the Azure portal, disable third-party services or restrict to “Free or BYOL SKUs only”.</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Azure portal hizmetleri nasıl kısıtlayabileceğini gösterir.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="E-portalda hizmetleri nasıl kısıtlayabileceğini gösterir.":::

2. <span data-ttu-id="4400c-225">Yalnızca belirli VM 'Lere izin vermek için bir Azure ilkesi oluşturun.</span><span class="sxs-lookup"><span data-stu-id="4400c-225">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="4400c-226">Windows VM 'lerine ilke zorlama hakkında daha fazla bilgi için bkz. [Azure Resource Manager Ile Windows VM](https://docs.microsoft.com/azure/virtual-machines/windows/policy)'Lerine ilke uygulama.</span><span class="sxs-lookup"><span data-stu-id="4400c-226">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](https://docs.microsoft.com/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="4400c-227">Özel Azure Marketi, belirli tekliflere ve planlara kısıtlama ve izin verme konusunda daha fazla esneklik sağlar.</span><span class="sxs-lookup"><span data-stu-id="4400c-227">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="4400c-228">Son kullanıcılara, üçüncü taraf hizmetleri dağıtmayı denemeden önce Market galerisinde dağıtım için kullanılabilirliği bildirir.</span><span class="sxs-lookup"><span data-stu-id="4400c-228">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="4400c-229">Üçüncü taraf hizmetlerin dağıtımına izin vermek için, Azure Marketi ' ni EA portalında açık/etkin olarak ayarlayın ve Azure portal.</span><span class="sxs-lookup"><span data-stu-id="4400c-229">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="4400c-230">Özel Azure Marketi, sanal makinelerle sınırlı olmamak üzere iş ortağı çözümlerini açabilir.</span><span class="sxs-lookup"><span data-stu-id="4400c-230">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="4400c-231">Özel Azure Marketi, plan düzeyinde bulunabilir ve "geçerli ve gelecekteki plan" i de ayarlayabilir.</span><span class="sxs-lookup"><span data-stu-id="4400c-231">Private Azure Marketplace can curate at the plan level and can also set “Current and future plan”.</span></span>
- <span data-ttu-id="4400c-232">Özel Azure Marketi, son kullanıcıları, ne yapabilecekleri ve dağıtılamayacağını en baştan haberdar edebilir.</span><span class="sxs-lookup"><span data-stu-id="4400c-232">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="4400c-233">Özel bir teklif ve özel Azure Marketi arasındaki fark nedir?</span><span class="sxs-lookup"><span data-stu-id="4400c-233">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="4400c-234">**Özel bir teklif** , yayımcıların yalnızca hedeflenen müşterilere görünen planlar oluşturmalarına olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="4400c-234">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="4400c-235">Bu, özelleştirilmiş çözümleri, anlaşmalı fiyatlandırma, özel hüküm ve koşullar ve özelleştirilmiş yapılandırmalarda özel olarak paylaşmasına olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="4400c-235">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="4400c-236">Ayrıntılar için bkz. [ticari Market 'Teki özel teklifler](https://docs.microsoft.com/azure/marketplace/private-offers).</span><span class="sxs-lookup"><span data-stu-id="4400c-236">For details, see [Private offers in the commercial marketplace](https://docs.microsoft.com/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="4400c-237">Azure portal **özel Azure Marketi** , yöneticilerin kullanıcıların dağıtabilecek üçüncü taraf çözümlerini önceden onaylamasını sağlar.</span><span class="sxs-lookup"><span data-stu-id="4400c-237">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="4400c-238">Özel bir Azure Marketi sayesinde kullanıcılar, uyumlu teklifleri bularak, satın alarak ve dağıtarak Azure Marketi 'nin avantajlarından faydalanarak yararlanabilir.</span><span class="sxs-lookup"><span data-stu-id="4400c-238">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="4400c-239">Özel Market 'teki abonelik tabanlı özel teklifleri yönetmek için Market yöneticisinin, belirli abonelikte en az "okuma" rolüne sahip olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="4400c-239">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of “read” role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="4400c-240">Özel Azure Marketi 'ne özel bir teklif ekledim, neden Market 'i Yönet sekmesinde gösterilmiyor?</span><span class="sxs-lookup"><span data-stu-id="4400c-240">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="4400c-241">Abonelik tabanlı özel teklifler yalnızca özel teklif ayarlarındaki listelenen abonelikler için görülebilir.</span><span class="sxs-lookup"><span data-stu-id="4400c-241">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="4400c-242">Özel teklifi görüntülemek için genel abonelik filtresinin tüm abonelikleri belirttiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="4400c-242">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

<span data-ttu-id="4400c-243">[![Özel Market filtresini gösterir.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4400c-243">[![Shows the private marketplace filter.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span></span>

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="4400c-244">Özel Azure Marketi 'ne özel görüntüler ekleyebilir mi?</span><span class="sxs-lookup"><span data-stu-id="4400c-244">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="4400c-245">Hayır.</span><span class="sxs-lookup"><span data-stu-id="4400c-245">No.</span></span> <span data-ttu-id="4400c-246">Özel Azure Marketi, BT yöneticisinin küresel Azure Marketi 'nden üçüncü taraf çözümleri yönetmesine ve seçmesine olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="4400c-246">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="4400c-247">Özel görüntüler küresel Azure Marketi 'nde olmadığından, BT Yöneticisi özel görüntülerinizi seçip seçemez.</span><span class="sxs-lookup"><span data-stu-id="4400c-247">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="4400c-248">Özel görüntüleri paylaştırmak istiyorsanız [paylaşılan görüntü Galerisi](https://docs.microsoft.com/azure/virtual-machines/shared-image-galleries)' ni kullanın.</span><span class="sxs-lookup"><span data-stu-id="4400c-248">If you would like to share custom images, use [Shared Image Gallery](https://docs.microsoft.com/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="4400c-249">Adım adım kılavuz paylaşılan görüntü Galerisi (SıG) ([CLI](https://docs.microsoft.com/azure/virtual-machines/shared-images-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/shared-images-powershell)) oluşturma.</span><span class="sxs-lookup"><span data-stu-id="4400c-249">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](https://docs.microsoft.com/azure/virtual-machines/shared-images-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="4400c-250">Bir SıG içinde bir görüntü tanımı oluşturun.</span><span class="sxs-lookup"><span data-stu-id="4400c-250">Create an image definition within a SIG.</span></span> <span data-ttu-id="4400c-251">Müşteri, işletim sistemi durumu alanı için **Genelleştirilmiş** ' ı seçmelidir.</span><span class="sxs-lookup"><span data-stu-id="4400c-251">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="4400c-252">([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span><span class="sxs-lookup"><span data-stu-id="4400c-252">([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="4400c-253">Yönetilen görüntüyü paylaşılan görüntü galerisine getirin ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-powershell)).</span><span class="sxs-lookup"><span data-stu-id="4400c-253">Bring managed image into the Shared Image Gallery ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="4400c-254">SıG VM görüntüleri bir abonelikte yer alır.</span><span class="sxs-lookup"><span data-stu-id="4400c-254">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="4400c-255">Başka abonelikler için kullanılabilir hale getirmek için, bir uygulama kaydı ([CLI](https://docs.microsoft.com/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/windows/share-images-across-tenants)) kullanın.</span><span class="sxs-lookup"><span data-stu-id="4400c-255">To make it available to other subscriptions, use an app registration ([CLI](https://docs.microsoft.com/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="4400c-256">Yayımcı Microsoft olmasa da, neden **Varsayılan olarak onaylanan** bazı teklifleri görüyorum?</span><span class="sxs-lookup"><span data-stu-id="4400c-256">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="4400c-257">Microsoft, Azure 'da Linux ve açık kaynaklı teknolojiyi destekler.</span><span class="sxs-lookup"><span data-stu-id="4400c-257">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="4400c-258">Desteklenen [Linux dağıtımları](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) Azure 'da desteklenir ve fiyat sanal makinelerde tümleşiktir.</span><span class="sxs-lookup"><span data-stu-id="4400c-258">[Endorsed Linux distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="4400c-259">Azure Linux Aracısı zaten Azure Marketi 'nde önceden yüklenmiş olduğundan, Microsoft teklifi gibi davranılır.</span><span class="sxs-lookup"><span data-stu-id="4400c-259">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="4400c-260">Microsoft teklifleri varsayılan olarak onaylandığından, onaylanmış Linux dağıtımları özel Azure Marketi 'nde yönetilemez ve varsayılan olarak onaylanır.</span><span class="sxs-lookup"><span data-stu-id="4400c-260">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="4400c-261">Desteğe başvurun</span><span class="sxs-lookup"><span data-stu-id="4400c-261">Contact support</span></span>

- <span data-ttu-id="4400c-262">Azure Marketi desteği için [Microsoft Q&A](/answers/products/)adresini ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="4400c-262">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>
