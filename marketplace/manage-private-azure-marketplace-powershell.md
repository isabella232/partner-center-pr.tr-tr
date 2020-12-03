---
title: 'Hızlı başlangıç: PowerShell kullanarak özel bir Azure Marketi yönetme'
description: Bu hızlı başlangıçta, Azure PowerShell kullanarak özel bir Azure Marketi 'nde tekliflerin nasıl yönetileceği gösterilmektedir.
author: keferna
ms.author: keferna
ms.topic: quickstart
ms.prod: marketplace-customer
ms.devlang: azurepowershell
ms.date: 11/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: c5b8b9fcc247818315887109e2163c0722bfbd97
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96536268"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a>Hızlı başlangıç: PowerShell kullanarak özel bir Azure Marketi yönetme

Bu makalede, [az. Market](/powershell/module/az.marketplace) PowerShell modülünü kullanarak özel bir Azure Marketi 'nde teklifleri nasıl yönetebileceğinizi açıklanmaktadır.

> [!IMPORTANT]
> Özel Azure Marketi Şu anda genel önizleme aşamasındadır. Bu önizleme sürümü bir hizmet düzeyi sözleşmesi olmadan sağlanır. Üretim iş yüklerinde kullanılması önerilmez. Bazı özellikler desteklenmeyebilir veya kısıtlı özelliklere sahip olabilir. Daha fazla bilgi için bkz. [Microsoft Azure Önizlemeleri için Ek Kullanım Koşulları](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).

## <a name="requirements"></a>Gereksinimler

* Azure aboneliğiniz yoksa başlamadan önce [ücretsiz](https://azure.microsoft.com/free/) bir hesap oluşturun.

* Azure PowerShell yerel olarak kullanmayı tercih ederseniz:
  * [Az PowerShell modülünü yükler](/powershell/azure/install-az-ps).
  * [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet 'Ini kullanarak Azure hesabınıza bağlanın.
* Azure Cloud Shell kullanmayı seçerseniz:
  * Daha fazla bilgi için bkz. [Azure Cloud Shell Genel Bakış](https://docs.microsoft.com/azure/cloud-shell/overview) .

  > [!IMPORTANT]
  > **Az. Market** PowerShell modülü önizlemedeyken, cmdlet 'ini kullanarak ayrı olarak yüklemelisiniz `Install-Module` . Bu PowerShell modülü genel kullanıma sunulduğunda, gelecekteki az PowerShell modülü sürümlerinin bir parçası olur ve Azure Cloud Shell içinden varsayılan olarak kullanılabilir.

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* Birden çok Azure aboneliğiniz varsa, kaynakların faturalandırılması gereken uygun aboneliği seçin. [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet 'ini kullanarak belirli bir abonelik seçin.

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a>Özel depoları Listele

Özel mağazaların listesini almak için [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) cmdlet 'ini kullanırsınız. Aşağıdaki örnek, kiracı kapsamı altında oluşturulan özel depoları listeler.

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

## <a name="add-an-offer-to-a-private-marketplace"></a>Özel Market 'e teklif ekleme

Özel bir depoya teklif eklemek için [set-Azmarketplaceprivatestoreteklifin](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) cmdlet 'ini kullanırsınız. Aşağıdaki örnek, belirtilen teklifi kiracı kapsamı altında oluşturulan özel bir mağazaya özel bir market 'e ekler.

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

## <a name="get-private-store-offers"></a>Özel mağaza tekliflerini al

Bir veya daha fazla özel mağaza teklifi almak için [Get-Azmarketplaceprivatestoreteklifin](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) cmdlet 'ini kullanırsınız. Aşağıdaki örnek, kiracı kapsamı altına eklenen belirtilen özel depo ile ilişkili teklifleri alır.

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

## <a name="remove-an-offer"></a>Teklifi kaldırma

Özel bir mağazadan bir teklifi kaldırmak için [Remove-Azmarketplaceprivatestoreteklifin](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) cmdlet 'ini kullanırsınız. Aşağıdaki örnek, kiracı kapsamında oluşturulan özel bir mağazadan bir teklifi kaldırır.

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a>Sonraki adımlar

[Özel Azure Marketi oluşturun ve yönetin](create-manage-private-azure-marketplace.md).
