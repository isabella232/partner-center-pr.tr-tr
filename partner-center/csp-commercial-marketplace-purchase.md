---
title: Ticari market tekliflerini satın alma
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: CSP programı iş ortaklarının, Bağımsız Yazılım Satıcılarından (ISV) saaS tekliflerini satın almak için İş Ortağı Merkezi marketi nasıl kullanabileceğini öğrenin.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2984dbb3a02df91d5a2a284182476bf348a24f47
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114837677"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>İş Ortağı Merkezi'da müşterileriniz için ticari market ürünleri satın İş Ortağı Merkezi


**Uygun roller:** Genel yönetici | Yönetici aracısı

Bulut Çözümü Sağlayıcısı (CSP) programında iş ortağı olarak, ticari marketi kullanarak müşterileriniz için Bağımsız Yazılım Satıcıları (ISV) tarafından sunulan belirli Hizmet Olarak Yazılım (SaaS) ürünlerine abonelik satın alabilirsiniz.

Müşterilerinize ISV SaaS abonelikleri sunarak işlerinizi ayırt etmeye yardımcı olabilir. Ayrıca, müşterilere kendi özel iş ihtiyaçlarını ele alan yazılım paketlerine de erişim veabilirsiniz. Aynı Microsoft ürünlerinin lisanslarını ve aboneliklerini yönetirken ISV yayımcılarından bu market SaaS ürünleri için lisansları ve abonelikleri yönetirsiniz.

Lisans tabanlı SaaS **abonelikleri veya** kullanım tabanlı **abonelikler satın alabilirsiniz.** Lisans tabanlı ve kullanım tabanlı faturalama arasındaki fark hakkında daha fazla bilgi edinmek için bkz. [Faturalamanın temelleri.](billing-basics.md)

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a>İş Ortağı Merkezi'da lisans tabanlı ve tarifeli SaaS abonelikleri satın İş Ortağı Merkezi

ISV yayımcıları tarafından sunulan lisans tabanlı veya tarifeli SaaS ürünleri için abonelikleri, Microsoft ürünleri için abonelik satın almak için aynı işlemi kullanarak satın alabilirsiniz.

İş Ortağı Merkezi'da lisans tabanlı veya tarifeli SaaS aboneliği satın almak için bkz. Müşteri [aboneliklerini oluşturma, askıya](create-a-new-subscription.md#create-a-new-subscription)alma veya iptal etme.

Müşterileriniz için ticari [İş Ortağı Merkezi api'leri](/partner-center/develop/) de kullanabilirsiniz. (Api'leri İş Ortağı Merkezi daha fazla bilgi için [bkz. Ticari market ürünleri için abonelik oluşturma.)](/partner-center/develop/create-subscription-azure-marketplace-products)

>[!IMPORTANT]
> CSP programında iş ortağı olarak,  lisans tabanlı veya tarifeli **SaaS** abonelikleri satın almak için iş ortağınız içindeki ISV yayımcılarından İş Ortağı Merkezi. Bu, ISV **yayımcının** sizin için sunduğu lisans tabanlı veya tarifeli **SaaS** tekliflerini, erişiminiz olan özel teklifler de dahil olmak üzere satın almak anlamına gelir. [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) ISV'lerden (Azure uygulamaları, Kapsayıcılar veya VM'ler içeren kullanım tabanlı teklifler gibi) diğer ticari market tekliflerini satın almak veya yönetmek için, [Azure portal.](https://portal.azure.com/)

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a>Azure portal'de kullanım tabanlı abonelikler satın Azure portal

Üçüncü taraf ISV yayımcılarından gelen lisans tabanlı SaaS aboneliklerinden farklı olarak, kullanım tabanlı abonelikler önce bir müşterinin Azure aboneliğine sahip olduğunu gerektirir. Ticari market faturalaması, kullanım tabanlı kaynaklar müşterinin Azure aboneliğinin altında yer alır. Müşteriniz Bir Azure aboneliğine sahip olduktan sonra CSP programı iş ortağı bu adımları takip eder ve bunlar için ticari market aboneliği satın alır:

1. Panoda oturum İş Ortağı Merkezi [ve](https://partner.microsoft.com/dashboard) **ardından** sol menüden Müşteriler'i seçin.

2. Belirli bir müşteriyi ve ardından Abonelikler'i **seçin.**  

3. Kullanım tabanlı **abonelikler altında Tüm** **kaynaklar'ı seçin.** Bu sizi Azure Yönetim portalına alır.

4. Azure Yönetim portalında, sol **menüden** Kaynak oluştur'a tıklayın.

5. Aşağıdakiler **listesinin** en üstünde Yer alan Hepsini Azure Market seçin.

6. Listenizi daraltmak için Market listesinin en üstünde yer alan filtreleri kullanın. Örneğin, yalnızca **Microsoft'un veya** bir ISV **yayımcısı tarafından Publisher** açılan listesinden Microsoft'u veya İş Ortağı'ı seçebilirsiniz. 

7. Belirli bir teklifi ve ardından **Oluştur'ı seçin.**

## <a name="next-steps"></a>Sonraki adımlar

- [Ticari market tekliflerini yönetme](csp-commercial-marketplace-purchase.md)