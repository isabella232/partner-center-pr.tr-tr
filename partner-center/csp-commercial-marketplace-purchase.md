---
title: Ticari Market tekliflerini satın alma
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: CSP program iş ortaklarının, bağımsız yazılım satıcıları (ISV) tarafından sunulan SaaS tekliflerinin müşteri satın alımları oluşturmak için Iş Ortağı Merkezi marketi ' ni nasıl kullanabileceğinizi öğrenin.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d06f64280ee89df241e150b2ad9c44adb7f7aa2f
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129072274"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>Iş Ortağı Merkezi 'nde müşterileriniz için ticari Market ürünleri satın alma


**Uygun roller**: genel yönetici | Yönetim Aracısı

Bulut Çözümü Sağlayıcısı (CSP) programında bir iş ortağı olarak, müşterilerinizin bağımsız yazılım satıcıları (ısv) tarafından sunulan belirli bir hizmet olarak yazılım (SaaS) ürününe yönelik abonelikler satın almak için ticari market ' i kullanabilirsiniz.

Müşterilerinize ISV SaaS abonelikleri sunarak işletmenizin ayırt edilmesine yardımcı olabilirsiniz. Müşterilere belirli iş ihtiyaçlarını karşılayan yazılım paketleri erişimi de verebilirsiniz. Microsoft ürünlerine yönelik lisansları ve abonelikleri yönetirken, bu Market SaaS ürünlerinin lisanslarını ve aboneliklerini ISV yayımcılarından yönetirsiniz.

**Lisans tabanlı** SaaS abonelikleri ya da **Kullanım tabanlı** abonelikler satın alabilirsiniz. Lisans tabanlı ve kullanım tabanlı faturalandırma arasındaki fark hakkında daha fazla bilgi edinmek için bkz. [faturalandırma temelleri](billing-basics.md).

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a>Iş Ortağı Merkezi 'nde lisans tabanlı ve tarifeli SaaS abonelikleri satın alma

ISV yayımcıları tarafından sunulan lisans tabanlı veya ölçülen SaaS ürünlerinin aboneliklerini, Microsoft ürünlerine yönelik abonelikler satın almak için kullandığınız süreci kullanarak satın alabilirsiniz.

Iş Ortağı Merkezi 'ne lisans tabanlı veya tarifeli bir SaaS aboneliği satın almak için bkz. [Müşteri abonelikleri oluşturma, askıya alma veya iptal etme](create-a-new-subscription.md#create-a-new-subscription).

Müşterileriniz için ticari Market abonelikleri oluşturmak üzere [Iş Ortağı Merkezi API 'lerini](/partner-center/develop/) de kullanabilirsiniz. (Iş Ortağı Merkezi API 'Leri kullanma hakkında daha fazla bilgi için bkz. [ticari Market ürünleri için abonelik oluşturma](/partner-center/develop/create-subscription-azure-marketplace-products).)

> [!IMPORTANT]
> CSP programındaki bir iş ortağı olarak, Iş Ortağı Merkezi 'nde ISV yayımcılarından **Lisans tabanlı** veya **ölçülen** SaaS abonelikleri satın alabilirsiniz. Bu, tüm **Lisans tabanlı** veya **tarifeli** SaaS tekliflerini, erişiminiz olan [özel TEKLIFLER](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) de dahil olmak üzere ISV yayımcısı kullanımınıza sunabileceğiniz anlamına gelir. ISV 'lerden diğer, ticari Market tekliflerini satın almak veya yönetmek için (Azure uygulamaları, kapsayıcılar veya VM 'Leri içeren Kullanım tabanlı teklifler gibi) [Azure Portal](https://portal.azure.com/)gitmeniz gerekir.

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a>Azure portal kullanım tabanlı abonelikler satın alın

Üçüncü taraf ISV yayımcılarından lisans tabanlı SaaS aboneliklerinin aksine, önce kullanım tabanlı abonelikler için bir müşterinin bir Azure aboneliğine sahip olması gerekir. Ticari Market için faturalandırma, kullanım tabanlı kaynaklar müşterinin Azure aboneliği kapsamında yer alıyorsa. Müşterinizin bir Azure aboneliğine sahip olması durumunda, CSP programındaki bir iş ortağı için ticari bir market aboneliği satın almak üzere bu adımları takip edebilir:

> [!NOTE]
> Iş Ortağı Merkezi önizleme arabirimi, mantıksal olarak gruplanmış çalışma alanları aracılığıyla daha verimli ve üretken bir kullanıcı deneyimi sağlar. Çalışma alanları arabirimi ve nasıl kullanılacağı hakkında daha fazla bilgi edinmek için bkz. [Iş ortağı merkezini alma](get-around-partner-center.md#turn-workspaces-on-and-off).

#### <a name="workspaces-view"></a>[Çalışma alanları görünümü](#tab/workspaces-view)

1. Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın ve **müşteriler** kutucuğunu seçin.

2. Belirli müşteriyi seçip **abonelikler**' i seçin.  

3. **Kullanım tabanlı abonelikler** altında **tüm kaynaklar**' ı seçin. Bu sizi Azure yönetim portalı 'na götürür.

4. Azure Yönetim Portalı ' nda, sol taraftaki menüden **kaynak oluştur** ' u seçin.

5. Azure Marketi listesinin en üstünde bulunan **Tümünü göster** ' i seçin.

6. Listenizi daraltmak için Market listesinin en üstünde bulunan filtreleri kullanın. örneğin, yalnızca microsoft 'tan veya bir ısv yayımcısından gelen teklifleri görüntülemek için **Publisher** açılır listesinden **microsoft** veya **Partner** ' ı seçebilirsiniz.

7. Belirli bir teklif seçin ve ardından **Oluştur**' u seçin.

#### <a name="current-view"></a>[Geçerli görünüm](#tab/current-view)

1. Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın ve ardından sol taraftaki menüden **müşteriler** ' i seçin.

2. Belirli müşteriyi seçip **abonelikler**' i seçin.  

3. **Kullanım tabanlı abonelikler** altında **tüm kaynaklar**' ı seçin. Bu sizi Azure yönetim portalı 'na götürür.

4. Azure Yönetim Portalı ' nda, sol taraftaki menüden **kaynak oluştur** ' u seçin.

5. Azure Marketi listesinin en üstünde bulunan **Tümünü göster** ' i seçin.

6. Listenizi daraltmak için Market listesinin en üstünde bulunan filtreleri kullanın. örneğin, yalnızca microsoft 'tan veya bir ısv yayımcısından gelen teklifleri görüntülemek için **Publisher** açılır listesinden **microsoft** veya **Partner** ' ı seçebilirsiniz.

7. Belirli bir teklif seçin ve ardından **Oluştur**' u seçin.

* * *

## <a name="next-steps"></a>Sonraki adımlar

- [Ticari Market tekliflerini yönetme](csp-commercial-marketplace-purchase.md)
