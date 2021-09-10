---
title: 'Hızlı Başlangıç: PowerShell kullanarak Azure Market Özel Ağ Yönetme'
description: Bu hızlı başlangıçta, özel bir Azure Market'daki teklifleri Azure PowerShell.
author: keferna
ms.author: keferna
ms.topic: quickstart
ms.service: marketplace-customer
ms.devlang: azurepowershell
ms.date: 11/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: d7bd790eab2618822dbc5099ad1ad107794c82d2
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123937004"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a>Hızlı Başlangıç: PowerShell kullanarak Azure Market Özel Ağ Yönetme

Bu makalede, [Az.Marketplace](/powershell/module/az.marketplace) PowerShell modülünü kullanarak özel Azure Market tekliflerini nasıl yönettniz açıklanmıştır.

> [!IMPORTANT]
> Özel Azure Market şu anda genel önizlemede. Bu önizleme sürümü bir hizmet düzeyi sözleşmesi olmadan sağlanır. Üretim iş yüklerinde kullanılması önerilmez. Bazı özellikler desteklenmiyor veya kısıtlı özelliklere sahip olabilir. Daha fazla bilgi için bkz. [Microsoft Azure Önizlemeleri için Ek Kullanım Koşulları](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).

## <a name="requirements"></a>Gereksinimler

* Azure aboneliğiniz yoksa başlamadan önce [ücretsiz](https://azure.microsoft.com/free/) bir hesap oluşturun.

* Yerel olarak kullanmak Azure PowerShell:
  * [Az PowerShell modülünü yükleyin.](/powershell/azure/install-az-ps)
  * [Bağlan-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet'ini kullanarak Azure Bağlan oturum açın.
* Şu bilgileri kullanmayı Azure Cloud Shell:
  * Daha [fazla bilgi için Azure Cloud Shell](/azure/cloud-shell/overview) Genel Bakış'a bakın.

  > [!IMPORTANT]
  > **Az.Marketplace** PowerShell modülü önizlemedeyken, cmdlet'ini kullanarak modülü ayrı `Install-Module` olarak yüklemeniz gerekir. Bu PowerShell modülü genel kullanıma sunulduktan sonra, gelecekteki Az PowerShell modülü sürümlerinin bir parçası haline gelecek ve Azure Cloud Shell içinden varsayılan olarak sağlanacaktır.

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* Birden çok Azure aboneliğiniz varsa, kaynakların faturalandırilmesi gereken uygun aboneliği seçin. [Set-AzContext cmdlet'ini kullanarak belirli bir](/powershell/module/az.accounts/set-azcontext) aboneliği seçin.

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a>Özel depoları listele

Özel mağazaların listesini almak için [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) cmdlet'ini kullanın. Aşağıdaki örnek, kiracı kapsamında oluşturulan özel depoları listeler.

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

## <a name="add-an-offer-to-a-private-marketplace"></a>Özel markete teklif ekleme

Özel bir mağazaya teklif eklemek için [Set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) cmdlet'ini kullanın. Aşağıdaki örnek, kiracı kapsamında oluşturulan özel bir mağaza için belirtilen teklifi özel markete ekler.

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

Bir veya daha fazla özel mağaza teklifi almak için [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) cmdlet'ini kullanın. Aşağıdaki örnek, kiracı kapsamında eklenen belirtilen özel depoyla ilişkili teklifleri alır.

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

Bir teklifi özel mağazadan kaldırmak için [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) cmdlet'ini kullanın. Aşağıdaki örnek, kiracı kapsamında oluşturulmuş özel bir mağazadan bir teklifi kaldırır.

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a>Sonraki adımlar

[Özel uygulama oluşturma ve Azure Market.](create-manage-private-azure-marketplace.md)