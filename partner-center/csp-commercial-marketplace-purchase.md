---
title: Ticari Market tekliflerini satın alma
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP program iş ortaklarının, bağımsız yazılım satıcıları (ISV) tarafından sunulan SaaS tekliflerinin müşteri satın alımları oluşturmak için Iş Ortağı Merkezi marketi ' ni nasıl kullanabileceğinizi öğrenin.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d8eb2faec7c2ddd70ed0cacedebf4f9824441a7a
ms.sourcegitcommit: f34f2f69e6df4f260479a205d94010cf47987ff2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/25/2020
ms.locfileid: "96038872"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>Iş Ortağı Merkezi 'nde müşterileriniz için ticari Market ürünleri satın alma

**Şunlara uygulanır**

- İş Ortağı Merkezi
- CSP programındaki iş ortakları

**Uygun roller**

- Genel yönetici
- Yönetim Aracısı

Bulut çözümü sağlayıcısı (CSP) programında bir iş ortağı olarak, müşterilerinizin bağımsız yazılım satıcıları (ISV 'Ler) tarafından sunulan belirli bir hizmet olarak yazılım (SaaS) ürününe yönelik abonelikler satın almak için ticari Market ' i kullanabilirsiniz.

Müşterilerinize ISV SaaS abonelikleri sunarak işletmenizin ayırt edilmesine yardımcı olabilirsiniz. Müşterilere belirli iş ihtiyaçlarını karşılayan yazılım paketleri erişimi de verebilirsiniz. Microsoft ürünlerine yönelik lisansları ve abonelikleri yönetirken, bu Market SaaS ürünlerinin lisanslarını ve aboneliklerini ISV yayımcılarından yönetirsiniz.

**Lisans tabanlı** SaaS abonelikleri ya da **Kullanım tabanlı** abonelikler satın alabilirsiniz. Lisans tabanlı ve kullanım tabanlı faturalandırma arasındaki fark hakkında daha fazla bilgi edinmek için bkz. [faturalandırma temelleri](billing-basics.md).

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a>Iş Ortağı Merkezi 'nde lisans tabanlı ve tarifeli SaaS abonelikleri satın alma

ISV yayımcıları tarafından sunulan lisans tabanlı veya ölçülen SaaS ürünlerinin aboneliklerini, Microsoft ürünlerine yönelik abonelikler satın almak için kullandığınız süreci kullanarak satın alabilirsiniz.

Iş Ortağı Merkezi 'ne lisans tabanlı veya tarifeli bir SaaS aboneliği satın almak için bkz. [Müşteri abonelikleri oluşturma, askıya alma veya iptal etme](create-a-new-subscription.md#create-a-new-subscription).

Müşterileriniz için ticari Market abonelikleri oluşturmak üzere [Iş Ortağı Merkezi API 'lerini](/partner-center/develop/) de kullanabilirsiniz. (Iş Ortağı Merkezi API 'Leri kullanma hakkında daha fazla bilgi için bkz. [ticari Market ürünleri için abonelik oluşturma](/partner-center/develop/create-subscription-azure-marketplace-products).)

>[!IMPORTANT]
> CSP programındaki bir iş ortağı olarak, Iş Ortağı Merkezi 'nde ISV yayımcılarından **Lisans tabanlı** veya **ölçülen** SaaS abonelikleri satın alabilirsiniz. Bu, tüm **Lisans tabanlı** veya **tarifeli** SaaS tekliflerini, erişiminiz olan [özel TEKLIFLER](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) de dahil olmak üzere ISV yayımcısı kullanımınıza sunabileceğiniz anlamına gelir. ISV 'lerden diğer, ticari Market tekliflerini satın almak veya yönetmek için (Azure uygulamaları, kapsayıcılar veya VM 'Leri içeren Kullanım tabanlı teklifler gibi) [Azure Portal](https://portal.azure.com/)gitmeniz gerekir.

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a>Azure portal kullanım tabanlı abonelikler satın alın

Üçüncü taraf ISV yayımcılarından lisans tabanlı SaaS aboneliklerinin aksine, önce kullanım tabanlı abonelikler için bir müşterinin bir Azure aboneliğine sahip olması gerekir. Ticari Market için faturalandırma, kullanım tabanlı kaynaklar müşterinin Azure aboneliği kapsamında yer alıyorsa. Müşterinizin bir Azure aboneliğine sahip olması durumunda, CSP programındaki bir iş ortağı için ticari bir market aboneliği satın almak üzere bu adımları takip edebilir:

1. Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın ve ardından sol taraftaki menüden **müşteriler** ' i seçin.

2. Belirli müşteriyi seçip **abonelikler**' i seçin.  

3. **Kullanım tabanlı abonelikler** altında **tüm kaynaklar**' ı seçin. Bu sizi Azure yönetim portalı 'na götürür.

4. Azure Yönetim Portalı ' nda, sol taraftaki menüden **kaynak oluştur** ' u seçin.

5. Azure Marketi listesinin en üstünde bulunan **Tümünü göster** ' i seçin.

6. Listenizi daraltmak için Market listesinin en üstünde bulunan filtreleri kullanın. Örneğin, yalnızca Microsoft 'tan veya bir ISV yayımcısından gelen teklifleri görüntülemek için **Yayımcı** açılan listesinden **Microsoft** veya **partner** ' ı seçebilirsiniz.

7. Belirli bir teklif seçin ve ardından **Oluştur**' u seçin.

## <a name="next-steps"></a>Sonraki adımlar

- [Ticari Market tekliflerini yönetme](csp-commercial-marketplace-purchase.md)