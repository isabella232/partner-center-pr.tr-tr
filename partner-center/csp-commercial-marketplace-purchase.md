---
title: Ticari market tekliflerini satın alma
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP programı iş ortaklarının, Bağımsız Yazılım Satıcılarından (ISV) saaS tekliflerini müşteri satın almak için İş Ortağı Merkezi marketi nasıl kullanabileceğini öğrenin.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3f5cf4895fa4d66c65215989d808a1dd18ef9064
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147862"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>İş Ortağı Merkezi'da müşterileriniz için ticari market ürünleri satın İş Ortağı Merkezi


**Uygun roller:** Genel yönetici | Yönetici aracısı

Bulut Çözümü Sağlayıcısı (CSP) programında iş ortağı olarak, ticari marketi kullanarak müşterileriniz için Bağımsız Yazılım Satıcıları (ISV) tarafından sunulan belirli Hizmet Olarak Yazılım (SaaS) ürünlerine abonelik satın alabilirsiniz.

Müşterilerinize ISV SaaS abonelikleri sunarak işlerinizi ayırt etmeye yardımcı olabilir. Ayrıca, müşterilere kendi özel iş ihtiyaçlarını ele alan yazılım paketlerine de erişim veabilirsiniz. Aynı Microsoft ürünlerinin lisanslarını ve aboneliklerini yönetirken ISV yayımcılarından bu market SaaS ürünleri için lisansları ve abonelikleri yönetirsiniz.

Lisans tabanlı SaaS **abonelikleri veya** kullanım tabanlı **abonelikler satın** alabilirsiniz. Lisans tabanlı ve kullanım tabanlı faturalama arasındaki fark hakkında daha fazla bilgi edinmek için bkz. [Faturalama temelleri.](billing-basics.md)

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a>İş Ortağı Merkezi'da lisans tabanlı ve tarifeli SaaS abonelikleri satın İş Ortağı Merkezi

ISV yayımcıları tarafından sunulan lisans tabanlı veya tarifeli SaaS ürünleri için abonelikleri, Microsoft ürünleri için abonelik satın almak için aynı işlemi kullanarak satın alabilirsiniz.

İş Ortağı Merkezi'da lisans tabanlı veya tarifeli SaaS aboneliği satın almak için bkz. Müşteri [aboneliklerini oluşturma, askıya](create-a-new-subscription.md#create-a-new-subscription)alma veya iptal etme.

Müşterileriniz için ticari [İş Ortağı Merkezi api'leri](/partner-center/develop/) de kullanabilirsiniz. (Api'leri İş Ortağı Merkezi daha fazla bilgi için [bkz. Ticari market ürünleri için abonelik oluşturma.)](/partner-center/develop/create-subscription-azure-marketplace-products)

>[!IMPORTANT]
> CSP programında iş ortağı olarak,  lisans tabanlı veya tarifeli **SaaS** abonelikleri satın almak için iş ortağınız içindeki ISV yayımcılarından İş Ortağı Merkezi. Bu, tüm **Lisans tabanlı** veya **tarifeli** SaaS tekliflerini, erişiminiz olan [özel TEKLIFLER](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) de dahil olmak üzere ISV yayımcısı kullanımınıza sunabileceğiniz anlamına gelir. ISV 'lerden diğer, ticari Market tekliflerini satın almak veya yönetmek için (Azure uygulamaları, kapsayıcılar veya VM 'Leri içeren Kullanım tabanlı teklifler gibi) [Azure Portal](https://portal.azure.com/)gitmeniz gerekir.

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