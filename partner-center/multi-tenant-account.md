---
title: Iş Ortağı Merkezi hesabınıza ek kiracılar ekleyin
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Iş Ortağı Merkezi hesabınızda birden çok Azure AD kiracılarının nasıl ekleneceğini, birleştireceğinizi veya yönetileceğini öğrenin. Bunu yapmak isteyebileceğiniz bazı nedenler hakkında bilgi edinin.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 22f85bda0a651559da1717ae1e5365da40d62aff
ms.sourcegitcommit: 8cb98de420f6ab5bb4cb3efc9007262c4d7d3327
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/12/2021
ms.locfileid: "98105565"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Iş Ortağı Merkezi hesabınızda birden çok kiracı ekleme ve yönetme


**Uygun roller**

- Genel yönetici

Bu özellik şirketiniz için birden çok kiracıyı yönetmenizi ve bunları İş Ortağı Merkezi hesabında birleştirmenizi sağlar. Iş Ortağı Merkezi hesabınızda birden çok Azure AD kiracıyı yönetmeniz gerekebileceği birçok neden vardır. Örneğin:

- Şirketiniz başka bir şirket satın alabilir ve yeni şirketteki çalışanların Iş ortağı merkezini kullanmasını istiyorsunuz. Ancak, iki şirketin ayrı kalmasını istersiniz. Bu durumda, yeni şirketin Azure AD kiracısını Iş ortağı küresel hesabınızla (PGA) ilişkilendirirsiniz. Bu ilişki, her iki şirketteki kullanıcıların iş ortağı merkezi 'nde çalışmasını sağlar.

- İşletmenizi çalıştırmak için birden fazla kiracınız varsa (örn. contoso.com, contoso.uk, contoso.in), aynı bılgısayar hesabı altına bağlamak için çok kiracılı bir şekilde kullanabilirsiniz.

- Birleşmeler ve alımlar birden fazla kiracı ile çalışmanız gerekir (örn. contoso fabrikam 'ı edindiğinde, hem Constoso.com hem de Fabrikam.com ilgili kiracılar kullanabilmek gerekir).

- Kiracıların herhangi birinden kullanıcıların şunları yapabilmesi gerekir:
    1.  Eğitim, dijital indirmeler, MCP ilişkilendirmesi için Iş Ortağı Merkezi 'Ne erişin
    2.  MPN admin, teşvikleri admin vb. gibi Iş Ortağı Merkezi rolleri atanmalıdır.


## <a name="add-another-azure-ad-tenant-to-your-account"></a>Hesabınıza başka bir Azure AD kiracısı ekleyin

1. Genel yönetici olarak, Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.
1. **Ayarlar** simgesinden **Hesap ayarları** ' nı seçin ve **kiracılar**' ı seçin.
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Kiracılar ilişkilendir"::: 

3. **Başka BIR ad kiracısını ilişkilendir** ' i seçin ve ilişkilendirmek istediğiniz kiracıyı belirtin.

1. Genel yönetici olarak, ilişkilendirmek istediğiniz kiracıda oturum açın ve ilişkilendirmeyi onaylayın. 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Kiracılar ilişkilendirmeyi Onayla"::: 

5. ' Yi doğruladıktan sonra, bir **küme** bildirimi görürsünüz.  **Kiracı yönetimine dön** ' ü seçin ve yeni eklenen kiracıyı listelendiğini görürsünüz. 
 

>[!NOTE]
>Bir kiracıyı zaten başka bir Iş Ortağı Merkezi hesabıyla ilişkili ise bir firmayla ilişkilendiremezsiniz.


## <a name="remove-a-tenant-from-your-account"></a>Bir kiracıyı hesabınızdan kaldırın
 
1. Genel yönetici olarak, Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.

1. **Ayarlar** simgesinden **Hesap ayarları** -kiracılar > seçin ve **iş ortağı** sekmesine tıklayın.
 
3. İlişkilendirmesini **kaldırmak** istediğiniz kiracı için Kaldır ' a tıklayın.

4. Bir kiracının ilişkilendirmesini kaldırmak, söz konusu Kiracıdaki kullanıcıların artık Iş Ortağı Merkezi hesabına erişemeyeceği anlamına gelir ve bu, uzmanlarınızın bir etkisi olabilir. 

Birincil kiracı ve şu anda oturum açtığınız Kiracı dışında, ilişkili tüm kiracılar için **Kaldır** düğmesi etkinleştirilir.

:::image type="content" source="images/disassociate.png" alt-text="Kaldır düğmesi olan kiracılar":::
 

## <a name="next-steps"></a>Sonraki adımlar

- [Kullanıcı ekle](create-user-accounts-and-set-permissions.md)






