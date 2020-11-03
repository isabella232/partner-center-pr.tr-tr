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
ms.openlocfilehash: 03cd603cf65b1e999cf95fd10d76e6ccc6c403e8
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/22/2020
ms.locfileid: "92531538"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>MPN programınız için tek yönetici şirketten ayrıldıysa ne yapmalı?

**Uygulama hedefi**

- İş Ortağı Merkezi

Aşağıdaki makalede, MPN yöneticiniz şirketten ayrıldıysa ne yapacaklarıyla ilgili üç tipik senaryo gösterilmektedir.

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>Senaryo 1: MPN Iş ortağı yönetici/hesap yöneticisi şirketten ayrıldı, ancak hesapta hala genel yöneticiler var

Bu durumda, şirketteki başka bir kişiye MPN Iş ortağı Yöneticisi rolü atanabilir. Belirli bir MPN Iş ortağı Yöneticisi/hesabı yönetici rolü rolüne atamak için:

1. İş hesabınız (ör.) ile iş ortağı Merkezi hesabınızda oturum açın tom@contoso.com .
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


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>Senaryo 3: MPN Iş ortağı yönetici/hesap yöneticisi/genel yönetici şirketten ayrıldı ve şirketin Azure AD 'ye erişebilen başka hiçbir Kullanıcı yok. Bu, erişimin tamamen kaybedilmesine neden olur.

Yönetilmeyen bir dizini Azure Active Directory yönetici olarak ele almak için [yöneticiye](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) ilişkin adımları izleyin.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Şirketiniz zaten bir iş hesabına sahip olup olmadığından emin değil misiniz?

Şirketinizde bir iş hesabı olup olmadığından emin değilseniz, denetlemek için aşağıdaki adımları izleyin.

1. [Azure yönetim portalı](https://ms.portal.azure.com)' nda oturum açın.
2. Sol menüden **Azure Active Directory** ' ı seçin ve ardından **etki alanı adları** ' nı seçin.
Zaten bir iş hesabınız varsa, etki alanı adınız listelenecektir.

>[!Note]
>Microsoft Azure veya Office 365 için etkin bir aboneliğiniz varsa, zaten bir iş hesabınız var ve oturum açma kimlik bilgileriniz bu hizmetlere erişmek için kullanılanlarla aynı olmalıdır.