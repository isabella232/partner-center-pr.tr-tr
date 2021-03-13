---
title: 'Hızlı başlangıç: PowerShell kullanarak özel bir Azure Marketi yönetme'
description: Bu hızlı başlangıçta, Azure PowerShell kullanarak özel bir Azure Marketi 'nde tekliflerin nasıl yönetileceği gösterilmektedir.
author: keferna
ms.author: keferna
ms.topic: quickstart
ms.service: marketplace-customer
ms.devlang: azurepowershell
ms.date: 11/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: d7bd790eab2618822dbc5099ad1ad107794c82d2
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412463"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a><span data-ttu-id="1626e-103">Hızlı başlangıç: PowerShell kullanarak özel bir Azure Marketi yönetme</span><span class="sxs-lookup"><span data-stu-id="1626e-103">Quickstart: Manage a Private Azure Marketplace using PowerShell</span></span>

<span data-ttu-id="1626e-104">Bu makalede, [az. Market](/powershell/module/az.marketplace) PowerShell modülünü kullanarak özel bir Azure Marketi 'nde teklifleri nasıl yönetebileceğinizi açıklanmaktadır.</span><span class="sxs-lookup"><span data-stu-id="1626e-104">This article describes how you can manage offers in a Private Azure Marketplace using the [Az.Marketplace](/powershell/module/az.marketplace) PowerShell module.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="1626e-105">Özel Azure Marketi Şu anda genel önizleme aşamasındadır.</span><span class="sxs-lookup"><span data-stu-id="1626e-105">Private Azure Marketplace is currently in public preview.</span></span> <span data-ttu-id="1626e-106">Bu önizleme sürümü bir hizmet düzeyi sözleşmesi olmadan sağlanır.</span><span class="sxs-lookup"><span data-stu-id="1626e-106">This preview version is provided without a service level agreement.</span></span> <span data-ttu-id="1626e-107">Üretim iş yüklerinde kullanılması önerilmez.</span><span class="sxs-lookup"><span data-stu-id="1626e-107">It's not recommended for production workloads.</span></span> <span data-ttu-id="1626e-108">Bazı özellikler desteklenmeyebilir veya kısıtlı özelliklere sahip olabilir.</span><span class="sxs-lookup"><span data-stu-id="1626e-108">Some features might not be supported or might have constrained capabilities.</span></span> <span data-ttu-id="1626e-109">Daha fazla bilgi için bkz. [Microsoft Azure Önizlemeleri için Ek Kullanım Koşulları](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span><span class="sxs-lookup"><span data-stu-id="1626e-109">For more information, see [Supplemental Terms of Use for Microsoft Azure Previews](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span></span>

## <a name="requirements"></a><span data-ttu-id="1626e-110">Gereksinimler</span><span class="sxs-lookup"><span data-stu-id="1626e-110">Requirements</span></span>

* <span data-ttu-id="1626e-111">Azure aboneliğiniz yoksa başlamadan önce [ücretsiz](https://azure.microsoft.com/free/) bir hesap oluşturun.</span><span class="sxs-lookup"><span data-stu-id="1626e-111">If you don't have an Azure subscription, create a [free](https://azure.microsoft.com/free/) account before you begin.</span></span>

* <span data-ttu-id="1626e-112">Azure PowerShell yerel olarak kullanmayı tercih ederseniz:</span><span class="sxs-lookup"><span data-stu-id="1626e-112">If you choose to use Azure PowerShell locally:</span></span>
  * <span data-ttu-id="1626e-113">[Az PowerShell modülünü yükler](/powershell/azure/install-az-ps).</span><span class="sxs-lookup"><span data-stu-id="1626e-113">[Install the Az PowerShell module](/powershell/azure/install-az-ps).</span></span>
  * <span data-ttu-id="1626e-114">[Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet 'Ini kullanarak Azure hesabınıza bağlanın.</span><span class="sxs-lookup"><span data-stu-id="1626e-114">Connect to your Azure account using the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>
* <span data-ttu-id="1626e-115">Azure Cloud Shell kullanmayı seçerseniz:</span><span class="sxs-lookup"><span data-stu-id="1626e-115">If you choose to use Azure Cloud Shell:</span></span>
  * <span data-ttu-id="1626e-116">Daha fazla bilgi için bkz. [Azure Cloud Shell Genel Bakış](/azure/cloud-shell/overview) .</span><span class="sxs-lookup"><span data-stu-id="1626e-116">See [Overview of Azure Cloud Shell](/azure/cloud-shell/overview) for more information.</span></span>

  > [!IMPORTANT]
  > <span data-ttu-id="1626e-117">**Az. Market** PowerShell modülü önizlemedeyken, cmdlet 'ini kullanarak ayrı olarak yüklemelisiniz `Install-Module` .</span><span class="sxs-lookup"><span data-stu-id="1626e-117">While the **Az.Marketplace** PowerShell module is in preview, you must install it separately using the `Install-Module` cmdlet.</span></span> <span data-ttu-id="1626e-118">Bu PowerShell modülü genel kullanıma sunulduktan sonra, gelecekteki Az PowerShell modülü sürümlerinin bir parçası haline gelecek ve Azure Cloud Shell içinden varsayılan olarak sağlanacaktır.</span><span class="sxs-lookup"><span data-stu-id="1626e-118">After this PowerShell module becomes generally available, it will be part of future Az PowerShell module releases and available by default from within Azure Cloud Shell.</span></span>

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* <span data-ttu-id="1626e-119">Birden çok Azure aboneliğiniz varsa, kaynakların faturalandırılması gereken uygun aboneliği seçin.</span><span class="sxs-lookup"><span data-stu-id="1626e-119">If you have multiple Azure subscriptions, choose the appropriate subscription in which the resources should be billed.</span></span> <span data-ttu-id="1626e-120">[Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet 'ini kullanarak belirli bir abonelik seçin.</span><span class="sxs-lookup"><span data-stu-id="1626e-120">Select a specific subscription using the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet.</span></span>

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a><span data-ttu-id="1626e-121">Özel depoları Listele</span><span class="sxs-lookup"><span data-stu-id="1626e-121">List private stores</span></span>

<span data-ttu-id="1626e-122">Özel mağazaların listesini almak için [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) cmdlet 'ini kullanırsınız.</span><span class="sxs-lookup"><span data-stu-id="1626e-122">To retrieve a list of private stores, you use the [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) cmdlet.</span></span> <span data-ttu-id="1626e-123">Aşağıdaki örnek, kiracı kapsamı altında oluşturulan özel depoları listeler.</span><span class="sxs-lookup"><span data-stu-id="1626e-123">The following example lists private stores that were created under the tenant scope.</span></span>

```azurepowershell-interactive
Get-AzMarketplacePrivateStore
```

```Output
Availability   : enabled
PrivateStoreId : 00000000-0000-0000-0000-000000000000
ETag           : "00000000-0000-0000-0000-000000000000"
Id             : /providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000
Name           : 00000000-0000-0000-0000-000000000000
Type           : Microsoft.Marketplace/privateStores
```

## <a name="add-an-offer-to-a-private-marketplace"></a><span data-ttu-id="1626e-124">Özel Market 'e teklif ekleme</span><span class="sxs-lookup"><span data-stu-id="1626e-124">Add an offer to a private marketplace</span></span>

<span data-ttu-id="1626e-125">Özel bir depoya teklif eklemek için [set-Azmarketplaceprivatestoreteklifin](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) cmdlet 'ini kullanırsınız.</span><span class="sxs-lookup"><span data-stu-id="1626e-125">To add an offer to a private store, you use the [Set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="1626e-126">Aşağıdaki örnek, belirtilen teklifi kiracı kapsamı altında oluşturulan özel bir mağazaya özel bir market 'e ekler.</span><span class="sxs-lookup"><span data-stu-id="1626e-126">The following example adds the specified offer to a private marketplace for a private store that is created under the tenant scope.</span></span>

```azurepowershell-interactive
$Params = @{
  privateStoreId = '00000000-0000-0000-0000-000000000000'
  offerId = 'publisherid.offerid'
  SpecificPlanIdsLimitation =@('PublisherEnterpriseLinux72',
                               'PublisherEnterpriseLinux72-ARM',
                               'PublisherEnterpriseLinux73',
                               'PublisherEnterpriseLinux73-ARM',
                               'PublisherEnterpriseLinux73-ARM-pr'
  )
}
Set-AzMarketplacePrivateStoreOffer @Params
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {PublisherEnterpriseLinux72, PublisherEnterpriseLinux72-ARM,
PublisherEnterpriseLinux73, PublisherEnterpriseLinux73-ARM, PublisherEnterpriseLinux73-ARM-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="get-private-store-offers"></a><span data-ttu-id="1626e-127">Özel mağaza tekliflerini al</span><span class="sxs-lookup"><span data-stu-id="1626e-127">Get private store offers</span></span>

<span data-ttu-id="1626e-128">Bir veya daha fazla özel mağaza teklifi almak için [Get-Azmarketplaceprivatestoreteklifin](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) cmdlet 'ini kullanırsınız.</span><span class="sxs-lookup"><span data-stu-id="1626e-128">To get one or more private store offers, you use the [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="1626e-129">Aşağıdaki örnek, kiracı kapsamı altına eklenen belirtilen özel depo ile ilişkili teklifleri alır.</span><span class="sxs-lookup"><span data-stu-id="1626e-129">The following example gets offers that are associated with the specified private store that were added under the tenant scope.</span></span>

```azurepowershell-interactive
Get-AzMarketplacePrivateStoreOffer -PrivateStoreId 00000000-0000-0000-0000-000000000000
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {small, medium-with-upgraded-bandwidth, medium-with-upgraded-apps, large, large-pr,
small-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers

UniqueOfferId             : publisherid1.offerid1
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {azure_managedservices_professional ,azure_managedservices_professional-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid1.offerid1
Name                      : publisherid1.offerid1
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="remove-an-offer"></a><span data-ttu-id="1626e-130">Teklifi kaldırma</span><span class="sxs-lookup"><span data-stu-id="1626e-130">Remove an offer</span></span>

<span data-ttu-id="1626e-131">Özel bir mağazadan bir teklifi kaldırmak için [Remove-Azmarketplaceprivatestoreteklifin](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) cmdlet 'ini kullanırsınız.</span><span class="sxs-lookup"><span data-stu-id="1626e-131">To remove an offer from a private store, you use the [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="1626e-132">Aşağıdaki örnek, kiracı kapsamında oluşturulan özel bir mağazadan bir teklifi kaldırır.</span><span class="sxs-lookup"><span data-stu-id="1626e-132">The following example removes an offer from a private store that was created in the tenant scope.</span></span>

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a><span data-ttu-id="1626e-133">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="1626e-133">Next steps</span></span>

<span data-ttu-id="1626e-134">[Özel Azure Marketi oluşturun ve yönetin](create-manage-private-azure-marketplace.md).</span><span class="sxs-lookup"><span data-stu-id="1626e-134">[Create and manage Private Azure Marketplace](create-manage-private-azure-marketplace.md).</span></span>