---
title: Iş Ortağı Merkezi hesabınıza kiracılar ekleyin
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Iş Ortağı Merkezi hesabınızda birden çok Azure AD kiracılarının nasıl ekleneceğini, birleştireceğinizi veya yönetileceğini öğrenin ve neden yapmak isteyebileceğiniz hakkında bilgi edinin.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124814"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Iş Ortağı Merkezi hesabınızda birden çok kiracı ekleme ve yönetme


**Uygun roller**

- Genel yönetici
- Hesap yöneticisi

Bu makalede, şirketiniz için birden çok Azure Active Directory (Azure AD) kiracılarının nasıl birleştirilmesi ve ardından bunları Iş Ortağı Merkezi hesabınıza eklemek ve yönetmek açıklanır. Bunu yapmanız pek çok neden vardır. Örnek:

- Şirketinizin, contoso, başka bir şirket olan Fabrikam almış olduğunu varsayalım. İki şirketin ayrı kalmasını istiyorsunuz, ancak yeni çalışanların Iş Ortağı Merkezi 'ni kullanmasını istiyorsunuz. Bu durumda, yeni şirketin Azure AD kiracısını Iş ortağı küresel hesabınızla (PGA) ilişkilendirirsiniz. Bu ilişki, her iki şirketteki kullanıcıların iş ortağı merkezi 'nde çalışmasına olanak sağlar.

- İşletmenizi birden fazla kiracı (örneğin, *contoso.com*, *contoso.uk* ve *contoso.in*) ile çalıştırırsanız, bunları aynı bilgisayar hesabında gruplamak için çoklu kiralama kullanabilirsiniz.

- Birleşmeler ve alma yönergeleri her iki şirketteki kiracılar ile çalışmanız gerekiyorsa, hem *constoso.com* hem de *fabrikam.com* kiracılarını kullanırsınız.

- Kiracıların herhangi birinin kullanıcılarının şunları yapabilmesi gerekir:
    * Eğitim, dijital indirmeler veya Microsoft Sertifikalı Profesyonel (MCP) ilişkisi için Iş Ortağı Merkezi 'Ne erişin.
    * Microsoft İş Ortağı Ağı (MPN) admin veya teşvikleri admin gibi Iş Ortağı Merkezi rolleri atanmalıdır.

## <a name="add-an-azure-ad-tenant-to-your-account"></a>Hesabınıza bir Azure AD kiracısı ekleyin

1. [Microsoft Iş Ortağı Merkezi](https://partner.microsoft.com/dashboard)'nde genel yönetici olarak oturum açın.

1. Sağ üst köşedeki **Ayarlar**' ı seçin, **Hesap ayarları**' nı seçin ve **kiracılar**' ı seçin.
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Azure AD profili bölmesindeki Ilişkilendir düğmesinin ekran görüntüsü."::: 

1. **İlişkilendir**' i seçin ve ardından ilişkilendirmek istediğiniz kiracıyı belirtin.

1. Sorulduğunda, ilişkilendirmek istediğiniz kiracıya genel yönetici olarak oturum açın ve ardından **Onayla**' yı seçin. 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Yeni Azure AD ilişkilendirmesini Onayla bölmesindeki Onayla düğmesinin ekran görüntüsü."::: 

   İlişkilendirmeyi onayladıktan sonra, **tüm küme** iletileri görüntülenir. Yeni eklenen kiracıyı görüntülemek için **kiracı yönetimine dön**' ü seçin. 
 
>[!NOTE]
>Zaten başka bir Iş Ortağı Merkezi hesabıyla ilişkili ise, bir kiracıyı bir hesap ile ilişkilendiremezsiniz.


## <a name="remove-a-tenant-from-your-account"></a>Bir kiracıyı hesabınızdan kaldırın
 
1. [Microsoft Iş Ortağı Merkezi](https://partner.microsoft.com/dashboard)'nde genel yönetici olarak oturum açın.

1. Sağ üst köşedeki **Ayarlar** simgesini seçin ve ardından **Hesap ayarları**' nı seçin.

1. Sol bölmede **kiracılar**' ı seçin. **Azure AD kiracılarını Yönet** altında **iş ortağı** sekmesini seçin.
 
1. İlişkilendirmesini kaldırmak istediğiniz kiracının yanındaki **Kaldır** ' ı seçin.

   :::image type="content" source="images/disassociate.png" alt-text="Geçerli kiracı ilişkilerinin ve bunların kaldırma bağlantılarının ekran görüntüsü.":::

   Önceki ekran görüntüsünde gösterildiği gibi, tüm ilişkili kiracılar için **kaldırma** bağlantıları etkinleştirilir, birincil kiracı ve şu anda oturum açtığınız kiracı hariç. 

   > [!NOTE]   
   > Bir kiracıyı kaldırdığınızda, bu Kiracıdaki kullanıcıların artık Iş Ortağı Merkezi hesabına erişimi olmaz ve kaldırma, uzmanlarınızın bir etkisi olabilir. 

## <a name="next-steps"></a>Sonraki adımlar

- [Kullanıcı hesapları oluşturma](create-user-accounts-and-set-permissions.md)






