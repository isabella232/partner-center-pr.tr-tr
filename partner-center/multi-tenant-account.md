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
ms.openlocfilehash: caea2002b5edc2958c0af316762408e309bcf14a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151211"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Iş Ortağı Merkezi hesabınızda birden çok kiracı ekleme ve yönetme


**Uygun roller**: genel yönetici | Hesap Yöneticisi

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

1. İstendiğinde, ilişkilendirmek istediğiniz kiracıda genel yönetici olarak oturum açın ve Onayla'ya **seçin.** 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Yeni Azure AD ilişkilendirmesi onaylayın bölmesindeki Onayla düğmesinin ekran görüntüsü."::: 

   İlişkiyi onaylandıktan sonra Tüm **ayarlamalar iletisi** görüntülenir. Yeni eklenen kiracıyı görüntülemek için Kiracı yönetimine **geri dön seçeneğini seçin.** 
 
>[!NOTE]
>Zaten başka bir kiracı hesabıyla ilişkilendirilmişse kiracıyı bir hesapla İş Ortağı Merkezi.


## <a name="remove-a-tenant-from-your-account"></a>Bir kiracıyı hesabınızdan kaldırma
 
1. Microsoft'ta genel yönetici olarak [oturum İş Ortağı Merkezi.](https://partner.microsoft.com/dashboard)

1. Sağ üst kısımda Ayarlar simgesini **ve** ardından Hesap **ayarları'ı seçin.**

1. Sol bölmede **Kiracılar'ı seçin.** **Azure AD kiracılarını yönet altında** İş ortağı **sekmesini** seçin.
 
1. **İlişkilerini** kaldırmak istediğiniz kiracının yanındaki Kaldır'ı seçin.

   :::image type="content" source="images/disassociate.png" alt-text="Geçerli kiracı ilişkilendirmelerinin ve bunların Kaldır bağlantılarının ekran görüntüsü.":::

   Önceki ekran görüntüsünde gösterildiği  gibi, Birincil kiracı ve o anda oturum asanız kiracı dışında tüm ilişkili kiracılar için Kaldır bağlantıları etkinleştirilir. 

   > [!NOTE]   
   > Bir kiracıyı kaldırsanız, kiracı üzerindeki kullanıcılar artık İş Ortağı Merkezi hesabı erişimine sahip olmaz ve kaldırmanın yetkinliklerinizi etkilemesi olabilir. 

## <a name="next-steps"></a>Sonraki adımlar

- [Kullanıcı hesapları oluşturma](create-user-accounts-and-set-permissions.md)






