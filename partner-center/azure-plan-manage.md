---
title: Azure planı - Abonelikleri ve & yönetme
ms.topic: article
ms.date: 05/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: İş ortaklarının müşterinin Azure kaynaklarının operasyonel denetimi ve yönetimini elde etmek için farklı rol tabanlı erişim denetimi (RBAC) seçeneklerini nasıl kullanabileceğini öğrenin.
author: amitravat
ms.author: amrava
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 18cc5c62beaa76f6e3ade79f2f2069e0f2bd3c7e
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149613"
---
# <a name="manage-subscriptions-and-resources-under-the-azure-plan"></a>Azure planı kapsamındaki abonelikleri ve kaynakları yönetme

**Uygun roller:** Yönetici aracısı


Bu makalede, CSP iş ortaklarının müşterinin Azure kaynaklarının operasyonel denetimi ve yönetimini elde etmek için farklı rol tabanlı erişim denetimi (RBAC) seçeneklerini nasıl kullanabileceği açıklanmıştır. Bir müşteriyi Azure planına geçişte size varsayılan olarak Azure'da ayrıcalıklı yönetici hakları (adına yönetici aracılığıyla abonelik sahibi hakları) atanır.

 > [!NOTE]
 > Azure aboneliğine yönelik yönetici hakları müşteri tarafından abonelik, kaynak grubu veya iş yükü düzeyinde kaldırılabilir. 

 İş ortakları, rol tabanlı erişim denetimi özelliği (RBAC) aracılığıyla sağlanan farklı seçenekleri kullanarak CSP'de müşterinin Azure kaynaklarının 7x24 operasyonel denetimine ve yönetimine sahip olabilir. 

- **Adına Yönetici (AOBO)** - [AOBO](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO)ile, iş ortağı kiracısında Yönetici Aracısı rolüne sahip tüm kullanıcılar, CSP programı aracılığıyla oluşturacakları Azure aboneliklerine RBAC sahibi erişimine sahip olur.

- **Azure Lighthouse:** AOBO, farklı müşterilerle birlikte çalışmak veya gruplar ya da kullanıcılar için farklı roller etkinleştirmek için ayrı gruplar oluşturma esnekliğine izin vermez. Bu Azure Lighthouse kullanarak farklı müşterilere veya rollere farklı gruplar at attırma. Kullanıcılar Azure tarafından temsilci olarak yetki verilen kaynak yönetimi aracılığıyla uygun erişim düzeyine sahip olduğundan, Yönetici Aracısı rolüne (ve dolayısıyla tam AOBO erişimine sahip olan) kullanıcı sayısını azaltabilirsiniz. Bu, müşterilerin kaynaklarına gereksiz erişimi sınırlandırarak güvenliğin iyileştirilmesine yardımcı olur. Ayrıca, büyük ölçekte birden çok müşteriyi yönetmek için daha fazla esneklik sağlar. Daha fazla bilgi için [Azure Lighthouse programı Bulut Çözümü Sağlayıcısı okuyun.](/azure/lighthouse/concepts/cloud-solution-provider)

- **Dizin veya Konuk kullanıcılar veya [hizmet sorumluları](/azure/active-directory/develop/app-objects-and-service-principals)**: müşteri dizinine kullanıcı ekleyerek veya Konuk KULLANıCıLAR ekleyerek ve belırlı RBAC rolleri atayarak CSP aboneliklerine ayrıntılı erişim yetkisini atayabilirsiniz.

Microsoft, kullanıcıların işlerini bir güvenlik uygulaması olarak gerçekleştirmesi için gereken en düşük izinlere sahip olmasını önerir. Bkz. [Azure Active Directory Privileged Identity Management kaynakları](/azure/active-directory/privileged-identity-management/pim-configure).

## <a name="link-your-partner-id-mpn-id-to-your-credentials-for-managing-customers-azure-resources"></a>İş ortağı KIMLIĞINIZI (MPN KIMLIĞI), müşterinin Azure kaynaklarını yönetmek için kimlik bilgilerinizle ilişkilendirin

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

- üzerinden sağlanan erişimi [Azure Lighthouse.](https://azure.microsoft.com/services/azure-lighthouse/)

Rol tabanlı erişim, yönetici erişiminden farklıdır. Roller, neler yapa ve neleri yapamaylarını tam olarak sınırlandırma. Yönetici erişimi daha geniştir.

PEC puanı almaya uygun rolleri görmek için bkz. İş ortağı tarafından kazanılan [kredi için roller ve izinler.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2)

## <a name="next-steps"></a>Sonraki adımlar

- [Abonelikler için yönetici ayrıcalıklarını iptal Azure CSP geri alma](revoke-reinstate-csp.md)

- [İş ortağı tarafından kazanılan kredi - genel bakış](partner-earned-credit.md)

- [Yönetilen hizmetler için iş ortağı tarafından kazanılan kredi](partner-earned-credit-explanation.md)