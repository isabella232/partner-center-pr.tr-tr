---
title: Azure planı - Abonelikleri ve & yönetme
ms.topic: article
ms.date: 05/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: İş ortaklarının müşterinin Azure kaynaklarının operasyonel denetimi ve yönetimini elde etmek için farklı rol tabanlı erişim denetimi (RBAC) seçeneklerini nasıl kullanabileceğini öğrenin.
author: amitravat
ms.author: amrava
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: ce0eaa6a4ec04dc514b241b7f90bf32dd3106e41
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114841496"
---
# <a name="manage-subscriptions-and-resources-under-the-azure-plan"></a>Azure planı kapsamındaki abonelikleri ve kaynakları yönetme

**Uygun roller:** Yönetici aracısı


Bu makalede, CSP iş ortaklarının müşterinin Azure kaynaklarının operasyonel denetimi ve yönetimini elde etmek için farklı rol tabanlı erişim denetimi (RBAC) seçeneklerini nasıl kullanabileceği açıklanmıştır. Bir müşteriyi Azure planına geçişte, varsayılan olarak Azure'da ayrıcalıklı yönetici hakları (adına yönetici aracılığıyla abonelik sahibi hakları) atanır.

 > [!NOTE]
 > Azure aboneliğine yönelik yönetici hakları müşteri tarafından abonelik, kaynak grubu veya iş yükü düzeyinde kaldırılabilir. 

 İş ortakları, rol tabanlı erişim denetimi özelliği (RBAC) aracılığıyla sağlanan farklı seçenekleri kullanarak CSP'de müşterinin Azure kaynaklarının 7/24 operasyonel denetimine ve yönetimine sahip olabilir. 

- **Adına Yönetici (AOBO)** - [AOBO](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO)ile, iş ortağı kiracısında Yönetici Aracısı rolüne sahip olan tüm kullanıcılar, CSP programı aracılığıyla oluşturdukları Azure aboneliklerine RBAC sahibi erişimine sahip olur.

- **Azure Lighthouse:** AOBO, farklı müşterilerle birlikte çalışmak veya gruplar ya da kullanıcılar için farklı roller etkinleştirmek için ayrı gruplar oluşturma esnekliğine izin vermez. Bu Azure Lighthouse kullanarak farklı müşterilere veya rollere farklı gruplar at attırma. Kullanıcılar, Azure tarafından temsilci olarak yetki verilen kaynak yönetimi aracılığıyla uygun erişim düzeyine sahip olduğundan, Yönetici Aracısı rolüne (ve dolayısıyla tam AOBO erişimine sahip olan) kullanıcı sayısını azaltabilirsiniz. Bu, müşterilerin kaynaklarına gereksiz erişimi sınırlaarak güvenliğin iyileştirilmesine yardımcı olur. Ayrıca, büyük ölçekte birden çok müşteriyi yönetmek için daha fazla esneklik sağlar. Daha fazla bilgi için [Azure Lighthouse programı Bulut Çözümü Sağlayıcısı okuyun.](/azure/lighthouse/concepts/cloud-solution-provider)

- **Dizin veya Konuk Kullanıcılar veya [Hizmet](/azure/active-directory/develop/app-objects-and-service-principals)** Sorumluları: Müşteri dizinine kullanıcı ekleyerek veya konuk kullanıcılar ekleyerek ve belirli RBAC rollerini ataarak CSP aboneliklerine ayrıntılı erişim yetkisi veebilirsiniz.

Microsoft, kullanıcıların bir güvenlik uygulaması olarak çalışmalarını gerçekleştirmek için gereken en düşük izinlere sahip olması önerilir. Bkz. [Azure Active Directory Privileged Identity Management kaynakları.](/azure/active-directory/privileged-identity-management/pim-configure)

## <a name="link-your-partner-id-mpn-id-to-your-credentials-for-managing-customers-azure-resources"></a>Müşterinin Azure kaynaklarını yönetmek için iş ortağı kimliğinizi (MPN ID) kimlik bilgilerinize bağlama

Aşağıdaki tabloda iş ortağı kimliğinizi çeşitli RBAC erişim seçenekleriyle ilişkilendirmek için kullanılan yöntemler yer almaktadır.

|**Kategori**   |**Senaryo**   |**MPN KIMLIĞI ilişkilendirmesi**|
|-----------------|:------------------------|:------------------|
|Aobo   |CSP doğrudan iş ortağı veya dolaylı sağlayıcı, AOBO kullanarak CSP doğrudan iş ortağı veya dolaylı sağlayıcı varsayılan sahibi olan müşteri için aboneliği oluşturur. CSP doğrudan iş ortağı veya dolaylı sağlayıcı, AOBO kullanarak aboneliğe dolaylı kurumsal bayi erişimi sağlar.|Otomatik (iş ortağı çalışması gerekmez)|
|Azure Lighthouse|İş ortağı Market'te [yeni bir Yönetilen Hizmetler teklifi oluşturur.](/azure/lighthouse/concepts/managed-services-offers) Bu teklif CSP aboneliği üzerinde kabul edilir ve iş ortağı CSP aboneliğine erişim sağlar.|Otomatik (iş ortağı çalışması gerekmez)|
|Azure Lighthouse|İş ortağı Azure [aboneliğinde ARM](/azure/lighthouse/how-to/onboard-customer) şablonu dağıtır|İş ortağının MPN kimliğini iş ortağı kiracısı kullanıcı veya hizmet sorumlusuyla ilişkilendirmesi gerekir. Daha fazla bilgi için - [Bağlantı Ortak Kimliği.](/azure/billing/billing-partner-admin-link-started)|
|Dizin veya konuk kullanıcı|İş ortağı, müşteri dizininde yeni bir kullanıcı veya hizmet sorumlusu oluşturur ve kullanıcıya CSP aboneliğine erişim verir. İş ortağı müşteri dizininde yeni bir kullanıcı veya hizmet sorumlusu oluşturur. İş ortağı, kullanıcıyı bir gruba ekler ve gruba CSP aboneliğine erişim verir.|İş ortağının MPN kimliğini müşteri kiracısı kullanıcı veya hizmet sorumlusuyla ilişkilendirmesi gerekir. Daha fazla bilgi için - [Bağlantı Ortak Kimliği.](/azure/billing/billing-partner-admin-link-started)|

## <a name="confirm-that-you-have-admin-access"></a>Yönetici erişimine sahip olduğunu onaylayın

Müşteri hizmetlerinizi yönetmek ve kazanılan kredileri almak için yönetici erişimine sahip olmak gerekir. Kazanılan [krediler hakkında ayrıntılı bilgi](partner-earned-credit.md) için İş ortağı tarafından kazanılan krediler'i okuyun. Yönetici erişimine sahip olduğundan emin olmak için iki yol vardır.

- Günlük kullanım dosyasını gözden geçirme - Bu, günlük kullanım dosyasındaki birim fiyatı ve geçerli birim fiyatı gözden geçirerek ve bir indirim uygulanarak onaylandırarak belirlenebilirsiniz. İndirimi alıyorsanız yönetici sizsiniz.

- Azure izleyici uyarısı oluşturma - RBAC Azure İzleyici CSP aboneliğinden kaldırıldığı zaman bildirilecek bir etkinlik günlüğü uyarısı oluşturabilirsiniz. [](/azure/azure-monitor/platform/alerts-activity-log)

### <a name="create-an-azure-monitor-alert"></a>Azure İzleyici uyarısı oluşturma

1. Uyarı oluşturma.

   :::image type="content" source="images/azure/azurealert1.png" alt-text="azure uyarısı.":::

2. Uyarının hangi türde bir eylemde yer almalarını istediğinizi seçin. Örneğin, bir e-posta almak istediğiniz belirtirse, rol ataması silme işlemi gerçekleşirse size bildiren bir e-posta alırsınız.

   :::image type="content" source="images/azure/azureconfigurealert2.png" alt-text="uyarıyı yapılandırma.":::

### <a name="aobo-removal"></a>AOBO kaldırma

Müşteriler aboneliklerine erişimi yönetmek için  Access Control'Azure portal. Rol **atamaları sekmesinde Erişimi** **kaldır'ı seçer.** Böyle bir durumla karşı karşılasanız şunları da s olursanız:

- Yönetici erişiminin yeniden iade ed olup olamay olduğunu görmek için müşteriyle iletişime gidin.

- Rol tabanlı erişim denetimi [(RBAC) aracılığıyla sağlanan erişimi kullanın.](/azure/role-based-access-control/overview)

- üzerinden sağlanan erişimi [Azure Lighthouse.](https://azure.microsoft.com/services/azure-lighthouse/)

Rol tabanlı erişim, yönetici erişiminden farklıdır. Roller, neler yapa ve neleri yapamaylarını tam olarak sınırlandırma. Yönetici erişimi daha geniştir.

PEC puanı almaya uygun rolleri görmek için bkz. İş ortağı tarafından kazanılan [kredi için roller ve izinler.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2)

## <a name="next-steps"></a>Sonraki adımlar

- [Abonelikler için yönetici ayrıcalıklarını iptal Azure CSP geri alma](revoke-reinstate-csp.md)

- [İş ortağı tarafından kazanılan kredi - genel bakış](partner-earned-credit.md)

- [Yönetilen hizmetler için iş ortağı tarafından kazanılan kredi](partner-earned-credit-explanation.md)