---
title: İş hesabınızı iş ortağı merkezine bağlama
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Şirketinizi Iş Ortağı Merkezi hesabınıza bağlayan bir iş hesabı oluşturun. Bu, şirketinizdeki çalışanların Iş Ortağı Merkezi 'ne erişmesini sağlar.
author: vinayks
ms.author: vinayks
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 11/25/2019
ms.openlocfilehash: bc837db5a9dbcf92fbfead54b552695a218ae675
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534803"
---
# <a name="create-a-work-account-that-links-your-company-to-your-partner-center-account"></a>Şirketinizi Iş Ortağı Merkezi hesabınıza bağlayan bir iş hesabı oluşturun

**Uygun roller**

- Genel yönetici
- Kullanıcı Yönetimi Yöneticisi

## <a name="why-you-need-a-work-account"></a>Neden bir iş hesabına ihtiyacınız var?

Microsoft, şirketinizin iş hesabını yeni Iş Ortağı Merkezi hesabınıza bağlamanız gerekir. Bağlantı, hesap kullanıcılarınızın iş hesabı kullanıcı adları ve parolalarla iş ortağı merkezi 'nde oturum açmasını sağlar.

## <a name="the-work-account-email-address"></a>İş hesabı e-posta adresi

İş hesabınız veya iş e-postanız, şirketiniz tarafından size sağlanmış olan e-posta adresidir. Bir iş hesabı e-postası genellikle biçimindedir `you@yourcompany.com` . Hotmail, Gmail veya Yahoo gibi kişisel e-posta adresleri iş e-postası değildir ve iş ortağı merkezi hesabınız için kullanılamaz.

Birden fazla geçerli iş e-posta adresiniz varsa, bölgesel departman yerine şirket merkezinizdeki ilişkili olanı kullanın, örneğin, `contoso.com` adres yerine e-postanızı kullanın `contoso.uk` .

> [!NOTE]  
> Mevcut bir iş hesabını kullanmaya karar vermeden önce, hesapta kaç kullanıcının iş ortağı merkezi 'nde çalışması gerektiğini düşünün. Hesapta iş ortağı merkezi 'nde çalışması gerekmeyen kullanıcılarınız varsa, yalnızca iş ortağı merkezinde çalışması gereken kullanıcılar için yeni bir hesap oluşturmayı göz önünde bulundurun.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Şirketiniz zaten bir iş hesabına sahip olup olmadığından emin değil misiniz?

Şirketinizde bir iş hesabı olup olmadığından emin değilseniz, denetlemek için aşağıdaki adımları izleyin. Microsoft Azure veya Office 365 için etkin bir aboneliğiniz varsa, zaten bir iş hesabınız olması gerekir.

1. [Azure portalında](https://portal.azure.com) oturum açın.

2. Menüden Azure Active Directory ' ı seçin ve ardından etki alanı adları ' nı seçin.

3. Zaten bir iş hesabınız varsa, etki alanı adınız listelenecektir.

Şirketinizde zaten bir iş hesabı yoksa, kayıt işlemi sırasında bir tane oluşturabilirsiniz.

Aşağıdaki diyagramda birkaç tipik senaryo için adımlar verilmiştir:

- iş hesabınız olup olmadığını belirleme
- iş hesabınızda oturum açmayı belirleme
- Yeni bir iş hesabı oluşturmanız gerekip gerekmediğini belirleme

:::image type="content" source="images/onboardingAADFlow.png" lightbox="images/onboardingAADFlow.png" alt-text="Bir iş hesabınız var mı veya bir hesap oluşturmanız mı gerekiyor?":::

Azure AD 'de etki alanları ekleme hakkında daha fazla bilgi için bkz. [Azure AD 'de etki alanı ekleme veya ilişkilendirme](/azure/active-directory/active-directory-add-domain)

## <a name="about-microsoft-azure"></a>Microsoft Azure hakkında

Microsoft Azure, şirketlerin Microsoft tarafından yönetilen küresel bir veri merkezi ağı üzerinde uygulama oluşturmak, dağıtmak ve yönetmek için kullanabileceği genel bir bulut platformudur. Şirketler, fiziksel makineler yerine sanal işlevler veya hizmetlerle sanal bir BT altyapısı oluşturmak için Azure 'u kullanır.

Bir Azure aboneliği satın aldığınızda, şirketinizin fiziksel işletmelerini barındırmak için Office binasında bir kata kadar farklı değil, Azure genel bulutundaki adanmış, güvenli bir alanı da bir yere yeniden sunuyoruz. Office binanın sahibine, şirketiniz bir kiracı.

Azure iş hesabı, Azure genel bulutunda şirketinizin adanmış ve yalıtılmış bir sanal gösterimidir ve Azure, Microsoft Intune veya Office 365 gibi bir Microsoft bulut hizmetine abone olduğunuzda sizin için oluşturulur.

İş hesabınız, Azure AD kullanıcılarınızı ve bunlarla ilgili bilgileri ve bunların parolaları, profil verileri, izinleri vb. barındırır. İş hesabı Ayrıca gruplar, uygulamalar ve bir şirketle ilgili ve güvenlikle ilgili diğer bilgileri de içerir.

## <a name="next-steps"></a>Sonraki adımlar

- [İş Ortağı Merkezi hesabınızı yönetme](partner-center-account-setup.md)
- [Doğrulama durumunu izle](verification-responses.md)