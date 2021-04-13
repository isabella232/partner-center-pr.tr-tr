---
title: Iş Ortağı Merkezi 'nde oturum açılamıyor
ms.topic: troubleshooting
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Olası nedenlerde sorun giderin ve Iş Ortağı Merkezi 'nde oturum açamıyorum çözümler hakkında bilgi edinin. parolaları sıfırlama, rolleri denetleme ve kimlik bilgilerini denetleme hakkında daha fazla bilgi edinin.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 17087727afcaf3dbcf47801f8668388c370758e7
ms.sourcegitcommit: 9b04509f3830462628c1bb6af2ca41ed68b52619
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/09/2021
ms.locfileid: "107266580"
---
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a>Iş Ortağı Merkezi için oturum açma sorunlarını giderme

**Uygun roller**

- Iş Ortağı Merkezi ile ilgilenen tüm iş ortakları

Bu makale, Iş Ortağı Merkezi için ortak oturum açma sorunlarına yönelik çözümler içerir.

## <a name="youve-forgotten-your-password-for-partner-center"></a>Iş Ortağı Merkezi için parolanızı unuttunuz

Parolanızı unuttuysanız ve Iş Ortağı Merkezi 'Nde oturum açamıyor, desteğe başvurun. [Iş ürünleri Için desteğe](/microsoft-365/admin/contact-support-for-business-products)uygun kişiyi bulun.

Bir MPN iş ortağıysanız, genel yöneticinizden sizin için yeni bir parola oluşturmasını isteyin. Bir CSP dolaylı satıcısıysanız, dolaylı sağlayıcınızı Azure AD kiracınızda sizin için yeni bir genel yönetici oluşturmasını isteyin veya Temsilcili yönetici ayrıcalıklarını kullanarak sizin için yeni bir parola oluşturun.

Parolanızı nasıl sıfırlayabileceğinizi ve iş hesabınıza yeniden erişiminizi geri kazanmak için [güvenlik bilgilerini kullanarak iş veya okul parolanızı sıfırlayın](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password)makalesini okuyun.

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a>Iş Ortağı Merkezi 'nde beklenen sayfaları veya özellikleri görüntüleyemez veya yönetemezsiniz

Iş Ortağı Merkezi 'ndeki sayfalara erişim, atadığınız roller tarafından denetlenir. Hangi rollerin atandığını denetlemek için Iş Ortağı Merkezi ' nde ayarlar simgesini seçin, **Hesap ayarları**' nı seçin ve ardından hesap ayarları ' nda **Kullanıcı yönetimi**' ni seçin. Ara alanına adınızı yazın ve ardından sonuçları görüntüleyin.

İstediğiniz Uzmanlıklar, müşteriler, teşvikleri veya kullanıcıları görüntüleyebilmemişse veya yönetebiliyorsanız, aşağıdaki çözümleri deneyin:

- MPN, CSP ve başvuruların özelliklerine erişim için, genel yönetici veya hesap yöneticinizle görüşün. Roller ve Iş Ortağı Merkezi 'nde etkinleştirildikleri görevler hakkında daha fazla bilgi edinmek için bkz. [kullanıcılara rol & Izinleri atama](permissions-overview.md).
- Ticari Market ve Windows & Xbox, Office Mağazası, Microsoft Edge ve donanım geliştirici programlarının özelliklerine erişim için kuruluşunuzdaki sahip veya yönetici rolünde bulunan kişiyle iletişim kurun. Roller ve izinler hakkında daha fazla bilgi edinmek için bkz. [Microsoft Iş Ortağı Merkezi 'nde ticari Market hesabını yönetme](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions).

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a>Iş Ortağı Merkezi 'nde teklifinizi veya avantajlarınızı göremezsiniz

Oturum açmak için doğru kimlik bilgilerini kullandığınızı onaylayın. Örneğin, çalışmanız ve kişisel hesaplarınız aynı görünebilir (gibi abc@contoso.com ), ancak birisi sizin oluşturduğunuz bir kişisel hesap olabilir ve sizin adınıza bir iş hesabı olabilir. Bu durumda, oturum açtıysanız ancak MPN, CSP, ticari Market ile ilgili beklenen özellikleri görüntüleyemiyorsa, iş hesabınızı seçmeyi deneyin.

## <a name="next-steps"></a>Sonraki adımlar

- [Hesap bilgilerinizi doğrulama](verification-responses.md)
- [Parolamı sıfırlama](reset-my-pasword.md)
- [Kullanıcı parolasını sıfırlama](reset-a-user-password.md)