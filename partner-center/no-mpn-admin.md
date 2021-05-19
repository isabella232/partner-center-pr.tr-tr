---
title: MPN programınız için tek yönetici şirketten ayrıldıysa ne yapmalı?
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Yeni bir MPN Yöneticisi bulmak için ne yapılacağını öğrenin veya şirketinizin genel yöneticisinden yardım alın. Ayrıca, yeni bir Iş ortağı merkezi genel Yöneticisi ekleme hakkında bilgi edinin.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5efd157078acd72ca47418aaa9559a678fc5b129
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151177"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>MPN programınız için tek yönetici şirketten ayrıldıysa ne yapmalı?

**Uygun roller**: MPN iş ortağı Yöneticisi | Hesap Yöneticisi | Genel yönetici

Aşağıdaki makalede, MPN yöneticiniz şirketten ayrıldıysa ne yapacaklarıyla ilgili üç tipik senaryo gösterilmektedir.

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>Senaryo 1: MPN Iş ortağı yönetici/hesap yöneticisi şirketten ayrıldı, ancak hesapta hala genel yöneticiler var

Bu durumda, şirketteki başka bir kişiye MPN Iş ortağı Yöneticisi rolü atanabilir. Belirli bir MPN Iş ortağı Yöneticisi/hesabı yönetici rolü rolüne atamak için:

1. İş hesabınızla (örneğin,) iş ortağı Merkezi hesabınızda oturum açın tom@contoso.com .
1. Genel yönetici 'deki **Kullanıcı yönetimi** sayfasında, şirketinizin genel yöneticilerinin kim olduğunu görmek için filtre uygulayın. 
1. Genel yöneticilerden biriyle iletişim kurun ve sizden ihtiyacınız olan MPN 'ye özgü rolü atamasını isteyin. 

## <a name="scenario-2-mpn-partner-adminaccount-admin-has-left-the-company-and-there-are-no-global-admins-in-the-account"></a>Senaryo 2: MPN Iş ortağı yönetici/hesap yöneticisi şirketten ayrıldı ve hesapta genel yönetici yok 

**Kullanıcı yönetimi** sayfasına giderseniz ve genel yönetici için filtre uygulamanız, ancak şirketinizde MPN 'ye özgü rolü elde etmenize yardımcı olabilecek genel yönetici olmadığını fark ederseniz şu adımları izleyin:

1. [Portal.Azure.com](https://ms.portal.azure.com/)adresine gidin, iş hesabınızla oturum açın (örneğin, tom@contoso.com ). 
1. Sol taraftaki menü gezinti çubuğunda **Yardım + Destek** seçeneğini belirleyin.
1. Bir sonraki sayfada, açılan menüden **yeni destek isteği** ve **teknik sorun** türü ' nü seçin, ek ayrıntılar ekleyin ve **İleri: çözümler** ' e tıklayın.

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="Azure portal yöneticisi 'ni bul":::

4. Sonraki sayfada önerilen çözümleri inceledikten sonra **İleri: Ayrıntılar** ' ı seçin ve gerekli alanları doldurun.
1. Destek isteğini inceleyin ve oluşturun.


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>Senaryo 3: MPN İş Ortağı yöneticisi/Hesap yöneticisi/Genel yönetici şirketten ayrıldı ve şirketin Azure AD'lerine erişen başka kullanıcı yok. Bu, tam erişim kaybıdır.

Yönetici [olarak yönetimsiz](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) bir dizini yönetici olarak Azure Active Directory izleyin.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Şirketinizin zaten bir iş hesabı olup olmadığını emin değil misiniz?

Şirketinizin bir iş hesabı olup olmadığını kontrol etmek için aşağıdaki adımları izleyin.

1. Azure yönetim [portalında oturum açın.](https://ms.portal.azure.com)
2. Sol **menüden Azure Active Directory'yi** ve ardından Etki alanı **adları'ı seçin.**
Zaten bir iş hesabınız varsa, etki alanı adınız listelenir.

>[!Note]
>Microsoft Azure veya Office 365 için etkin bir aboneliğiniz varsa zaten bir iş hesabınız vardır ve oturum açma kimlik bilgileriniz bu hizmetlere erişmek için kullanılan kimlik bilgileriyle aynı olması gerekir.