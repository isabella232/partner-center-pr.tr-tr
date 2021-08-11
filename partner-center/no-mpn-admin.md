---
title: MPN programınızın tek yöneticisi şirketten ayrıldığında ne yapmalısınız?
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Yeni bir MPN Yöneticisi bulmak için ne yapılacağını öğrenin veya şirketinizin genel yöneticisinden yardım alın. Ayrıca, yeni bir Iş ortağı merkezi genel Yöneticisi ekleme hakkında bilgi edinin.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a673aad22bd5f9609fcbde656fb45e93ef2f227e92aba59988708769471e09e7
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115685878"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>MPN programınızın tek yöneticisi şirketten ayrıldığında ne yapmalısınız?

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

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="Azure portal içindeki yöneticiyi bulun.":::

4. Sonraki sayfada önerilen çözümleri inceledikten sonra **İleri: Ayrıntılar** ' ı seçin ve gerekli alanları doldurun.
1. Destek isteğini inceleyin ve oluşturun.


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>Senaryo 3: MPN Iş ortağı yönetici/hesap yöneticisi/genel yönetici şirketten ayrıldı ve şirketin Azure AD 'ye erişebilen başka hiçbir Kullanıcı yok. Bu, erişimin tamamen kaybedilmesine neden olur.

yönetilmeyen bir dizini Azure Active Directory yönetici olarak ele almak için [yöneticiye](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) ilişkin adımları izleyin.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Şirketiniz zaten bir iş hesabına sahip olup olmadığından emin değil misiniz?

Şirketinizde bir iş hesabı olup olmadığından emin değilseniz, denetlemek için aşağıdaki adımları izleyin.

1. [Azure yönetim portalı](https://ms.portal.azure.com)' nda oturum açın.
2. sol menüden **Azure Active Directory** ' ı seçin ve ardından **etki alanı adları**' nı seçin.
Zaten bir iş hesabınız varsa, etki alanı adınız listelenecektir.

>[!Note]
>Microsoft Azure veya Office 365 için etkin bir aboneliğiniz varsa, zaten bir iş hesabınız var ve oturum açma kimlik bilgileriniz bu hizmetlere erişmek için kullanılanlarla aynı olmalıdır.