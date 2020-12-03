---
title: Azure planı-abonelikleri & kaynakları yönetme
ms.topic: article
ms.date: 05/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: İş ortaklarının, bir müşterinin Azure kaynaklarının işletimsel denetimini ve yönetimini sağlamak için farklı rol tabanlı erişim denetimi (RBAC) seçeneklerini nasıl kullanabileceğinizi öğrenin.
author: amitravat
ms.author: amrava
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 31e9c6862a5aa19407fa6da5e15333bb7e696720
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534939"
---
# <a name="manage-subscriptions-and-resources-under-the-azure-plan"></a>Azure planı kapsamındaki abonelikleri ve kaynakları yönetme

**Uygun roller**

- Yönetim Aracısı


Bu makalede, CSP iş ortaklarının bir müşterinin Azure kaynaklarının işletimsel denetimini ve yönetimini sağlamak için farklı rol tabanlı erişim denetimi (RBAC) seçeneklerini nasıl kullanabileceği açıklanmaktadır. Bir müşteriyi Azure planına aktardığınızda, varsayılan olarak Azure 'da ayrıcalıklı yönetici hakları (adına yönetici aracılığıyla abonelik sahibi hakları) atanır.

 > [!NOTE]
 > Azure aboneliğine yönetici hakları bir abonelik, kaynak grubu veya iş yükü düzeyinde müşteri tarafından kaldırılabilir. 

 İş ortakları, rol tabanlı erişim denetimi özelliği (RBAC) ile sunulan farklı seçenekleri kullanarak bir müşterinin Azure kaynaklarını, CSP 'de 7/24 işletimsel denetim ve yönetim elde edebilir. 

- **Adına yönetici (Aobo)** - [AOCE](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO)ile, Iş ortağı kiracısında yönetici aracı rolüne sahip HERHANGI bir Kullanıcı, CSP programı aracılığıyla oluşturduğunuz Azure aboneliklerine RBAC sahibi erişimine sahip olur.

- **Azure açık Thouse**: Aobo, farklı müşterilerle çalışan ayrı gruplar oluşturma veya gruplar veya kullanıcılar için farklı rolleri etkinleştirme esnekliğine izin vermez. Azure Athouse kullanarak farklı müşterilere veya rollere farklı gruplar atayabilirsiniz. Kullanıcılar, Azure tarafından atanan kaynak yönetimi aracılığıyla uygun düzeyde erişime sahip olacağı için, Yönetim Aracısı rolüne sahip kullanıcı sayısını azaltabilir (ve bu nedenle tam AOBO erişimi vardır). Bu, müşterilerinizin kaynaklarına gereksiz erişimi sınırlayarak güvenliği artırmaya yardımcı olur. Ayrıca, birden çok müşteriyi ölçekli olarak yönetme konusunda daha fazla esneklik sağlar. Daha fazla bilgi için [Azure açık Thouse ve bulut çözümü sağlayıcısı programı](/azure/lighthouse/concepts/cloud-solution-provider)makalesini okuyun.

- **Dizin veya Konuk kullanıcılar veya [hizmet sorumluları](/azure/active-directory/develop/app-objects-and-service-principals)**: müşteri dizinine kullanıcı ekleyerek veya Konuk KULLANıCıLAR ekleyerek ve belırlı RBAC rolleri atayarak CSP aboneliklerine ayrıntılı erişim yetkisini atayabilirsiniz.

Microsoft, kullanıcıların işlerini bir güvenlik uygulaması olarak gerçekleştirmesi için gereken en düşük izinlere sahip olmasını önerir. Bkz. [Azure Active Directory Privileged Identity Management kaynakları](/azure/active-directory/privileged-identity-management/pim-configure).

## <a name="link-your-partner-id-mpn-idto-your-credentials-for-managing-customers-azure-resources"></a>İş ortağı KIMLIĞINIZI (MPN KIMLIĞI), müşterinin Azure kaynaklarını yönetmek için kimlik bilgilerinizle ilişkilendirin

Aşağıdaki tabloda, iş ortağı KIMLIĞINIZI çeşitli RBAC erişim seçenekleriyle ilişkilendirmek için kullanılan yöntemler gösterilmektedir.

|**Kategori**   |**Senaryo**   |**MPN KIMLIK ilişkilendirmesi**|
|-----------------|:------------------------|:------------------|
|AOI   |CSP doğrudan iş ortağı veya dolaylı sağlayıcı, AOININ CSP doğrudan iş ortağı veya dolaylı sağlayıcının varsayılan sahibi olan bir abonelik oluşturur.; CSP doğrudan iş ortağı veya dolaylı sağlayıcı, AOI kullanarak aboneliğe dolaylı satıcı erişimi sağlar.|Otomatik (iş ortağı çalışması gerekmez)|
|Azure Lighthouse|İş ortağı [Market 'te yeni bir yönetilen hizmet teklifi](/azure/lighthouse/concepts/managed-services-offers)oluşturur. Bu teklif CSP aboneliğinde kabul edilir ve iş ortağı CSP aboneliğine erişim sağlar.|Otomatik (iş ortağı çalışması gerekmez)|
|Azure Lighthouse|İş ortağı [ARM şablonunu](/azure/lighthouse/how-to/onboard-customer) Azure aboneliğine dağıtır|İş ortağının MPN KIMLIĞINI iş ortağı kiracısındaki Kullanıcı veya hizmet sorumlusu ile ilişkilendirilmesi gerekir. Daha fazla bilgi için- [bağlantı Iş ortağı kimliği](/azure/billing/billing-partner-admin-link-started).|
|Dizin veya Konuk Kullanıcı|İş ortağı, müşteri dizininde yeni bir kullanıcı veya hizmet sorumlusu oluşturur ve CSP aboneliğine kullanıcıya erişim sağlar. İş ortağı, müşteri dizininde yeni bir kullanıcı veya hizmet sorumlusu oluşturur. İş ortağı kullanıcıyı bir gruba ekler ve CSP aboneliğine gruba erişim sağlar.|İş ortağının MPN KIMLIĞINI müşteri kiracısındaki Kullanıcı veya hizmet sorumlusu ile ilişkilendirilmesi gerekir. Daha fazla bilgi için- [bağlantı Iş ortağı kimliği](/azure/billing/billing-partner-admin-link-started).|

## <a name="confirm-that-you-have-admin-access"></a>Yönetici erişiminizin olduğunu onaylayın

Müşterinizin hizmetlerini yönetmek ve kazanılan kredilerin alınması için yönetici erişimine ihtiyacınız vardır. Kazanılan kredilerle ilgili ayrıntılı bilgi için [Iş ortağı kazanılan kredileri](partner-earned-credit.md) okuyun. Yönetici erişiminizin olduğunu bildiğinizden emin olmak için iki yol vardır.

- Günlük kullanım dosyasını gözden geçirin-bu, günlük kullanım dosyasında birim fiyat ve geçerli birim fiyatı inceleyerek ve bir indirimin uygulanmakta olup olmadığını onaylayarak belirlenebilir. İndirimi alıyorsanız, yönetici olursunuz.

- Azure izleyici uyarısı oluşturma-RBAC erişiminizin CSP aboneliğinden ne zaman kaldırılacağını bildiren bir Azure Izleyici etkinlik günlüğü [uyarısı](/azure/azure-monitor/platform/alerts-activity-log) oluşturabilirsiniz.

### <a name="create-an-azure-monitor-alert"></a>Azure izleyici uyarısı oluşturma

1. Uyarı oluştur.

   :::image type="content" source="images/azure/azurealert1.png" alt-text="Azure uyarısı":::

2. Uyarının yerine gelmesi istediğiniz eylem türünü seçin. Örneğin, bir e-posta istediğinizi belirtirseniz, herhangi bir rol ataması silme gerçekleşirse size bildirimde bulunan bir e-posta alırsınız.

   :::image type="content" source="images/azure/azureconfigurealert2.png" alt-text="Uyarı Yapılandır":::

### <a name="aobo-removal"></a>AOI kaldırma

Müşteriler Azure portal **Access Control** giderek aboneliklerine erişimi yönetebilir. **Rol atamaları** sekmesinden, **erişimi kaldır**' ı seçin. Bu durumda şunları yapabilirsiniz:

- Yönetici erişiminin tekrar ifade edilebilir olup olmadığını görmek için müşterinizle konuşun.

- [Rol tabanlı erişim denetimi (RBAC)](/azure/role-based-access-control/overview)ile sunulan erişimi kullanın.

- [Azure ışıklı kullanımı](https://azure.microsoft.com/services/azure-lighthouse/)üzerinden sunulan erişimi kullanın.

Rol tabanlı erişim, yönetici erişiminden farklıdır. Roller, ne yapabileceğinize ve yapabileceğinize tam olarak göre sınırlandırın. Yönetici erişimi daha geniş.

PEC kazanmak için uygun rolleri görmek için, [iş ortağı tarafından kazanılan kredi Için rolleri ve izinleri](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2)okuyun.

## <a name="next-steps"></a>Sonraki adımlar

- [Azure CSP abonelikleri için yönetici ayrıcalıklarını iptal etme ve yeniden verme](revoke-reinstate-csp.md)

- [İş ortağı kazanılmış kredi-genel bakış](partner-earned-credit.md)

- [Yönetilen hizmetler için iş ortağı kazanılmış kredisi](partner-earned-credit-explanation.md)