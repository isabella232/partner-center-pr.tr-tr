---
title: İş Ortağı Merkezi hesabınıza kiracı ekleme
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Iş Ortağı Merkezi hesabınızda birden çok Azure AD kiracılarının nasıl ekleneceğini, birleştireceğinizi veya yönetileceğini öğrenin ve neden yapmak isteyebileceğiniz hakkında bilgi edinin.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2bb4507fd7e5f60584c8fca99256c964a7521dc8
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248706"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Iş Ortağı Merkezi hesabınızda birden çok kiracı ekleme ve yönetme


**Uygun roller**: genel yönetici | Hesap Yöneticisi

bu makalede, şirketiniz için birden çok Azure Active Directory (Azure AD) kiracılarının nasıl birleştirilmesi ve ardından bunları iş ortağı merkezi hesabınıza eklemek ve yönetmek açıklanır. Bunu yapmanız pek çok neden vardır. Örnek:

- Şirketinizin, contoso, başka bir şirket olan Fabrikam almış olduğunu varsayalım. İki şirketin ayrı kalmasını istiyorsunuz, ancak yeni çalışanların Iş Ortağı Merkezi 'ni kullanmasını istiyorsunuz. Bu durumda, yeni şirketin Azure AD kiracısını Iş ortağı küresel hesabınızla (PGA) ilişkilendirirsiniz. Bu ilişki, her iki şirketteki kullanıcıların iş ortağı merkezi 'nde çalışmasına olanak sağlar.

- İşletmenizi birden fazla kiracı (örneğin, *contoso.com*, *contoso.uk* ve *contoso.in*) ile çalıştırırsanız, bunları aynı bilgisayar hesabında gruplamak için çoklu kiralama kullanabilirsiniz.

- Birleşmeler ve alma yönergeleri her iki şirketteki kiracılar ile çalışmanız gerekiyorsa, hem *constoso.com* hem de *fabrikam.com* kiracılarını kullanırsınız.

- Kiracıların herhangi birinin kullanıcılarının şunları yapabilmesi gerekir:
    * eğitim, dijital indirmeler veya Microsoft sertifikalı Professional (MCP) ilişkisi için iş ortağı merkezi 'ne erişin.
    * Microsoft İş Ortağı Ağı (MPN) admin veya teşvikleri admin gibi Iş Ortağı Merkezi rolleri atanmalıdır.

## <a name="add-an-azure-ad-tenant-to-your-account"></a>Hesabınıza bir Azure AD kiracısı ekleyin

1. [Microsoft Iş Ortağı Merkezi](https://partner.microsoft.com/dashboard)'nde genel yönetici olarak oturum açın.

1. sağ üst köşedeki **Ayarlar**' ı seçin, **hesap ayarları**' nı seçin ve **kiracılar**' ı seçin.
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Azure AD profili bölmesindeki Ilişkilendir düğmesinin ekran görüntüsü."::: 

1. **İlişkilendir**' i seçin ve ardından ilişkilendirmek istediğiniz kiracıyı belirtin.

1. Sorulduğunda, ilişkilendirmek istediğiniz kiracıya genel yönetici olarak oturum açın ve ardından **Onayla**' yı seçin. 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Yeni Azure AD ilişkilendirmesini Onayla bölmesindeki Onayla düğmesinin ekran görüntüsü."::: 

   İlişkilendirmeyi onayladıktan sonra, **tüm küme** iletileri görüntülenir. Yeni eklenen kiracıyı görüntülemek için **kiracı yönetimine dön**' ü seçin. 
 
>[!NOTE]
>Zaten başka bir Iş Ortağı Merkezi hesabıyla ilişkili ise, bir kiracıyı bir hesap ile ilişkilendiremezsiniz.


## <a name="remove-a-tenant-from-your-account"></a>Bir kiracıyı hesabınızdan kaldırın
 
1. [Microsoft Iş Ortağı Merkezi](https://partner.microsoft.com/dashboard)'nde genel yönetici olarak oturum açın.

1. sağ üst köşedeki **Ayarlar** simgesini seçin ve ardından **hesap ayarları**' nı seçin.

1. Sol bölmede **kiracılar**' ı seçin. **Azure AD kiracılarını Yönet** altında **iş ortağı** sekmesini seçin.
 
1. İlişkilendirmesini kaldırmak istediğiniz kiracının yanındaki **Kaldır** ' ı seçin.

   :::image type="content" source="images/disassociate.png" alt-text="Geçerli kiracı ilişkilerinin ve bunların kaldırma bağlantılarının ekran görüntüsü.":::

   Önceki ekran görüntüsünde gösterildiği gibi, tüm ilişkili kiracılar için **kaldırma** bağlantıları etkinleştirilir, birincil kiracı ve şu anda oturum açtığınız kiracı hariç. 

   > [!NOTE]   
   > Bir kiracıyı kaldırdığınızda, bu Kiracıdaki kullanıcıların artık Iş Ortağı Merkezi hesabına erişimi olmaz ve kaldırma, uzmanlarınızın bir etkisi olabilir. 

## <a name="next-steps"></a>Sonraki adımlar

- [Kullanıcı hesapları oluşturma](create-user-accounts-and-set-permissions.md)






