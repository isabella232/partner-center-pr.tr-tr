---
title: Teşvikleri SSS
ms.topic: how-to
ms.date: 02/05/2021
description: Microsoft teşvikleri hakkında sık sorulan sorular. Bu makale, Kullanıcı rolleri, kaydetme veya hata iletileriyle ilgili ne yapılacak hakkında sorular içerir.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.openlocfilehash: 332832b14e3434824aee2b1a6bcf7eb321fb7a60
ms.sourcegitcommit: 2d1f0d7bc897278ef37af6d43c1a088f5ca14807
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/08/2021
ms.locfileid: "99835076"
---
# <a name="frequently-asked-questions-on-incentives"></a>Teşvikleri hakkında sık sorulan sorular

**Uygun roller:**

- Teşvikleri Yöneticisi

- Teşvikleri kullanıcısı

## <a name="do-i-need-to-be-the-global-admin-to-enroll-in-incentives"></a>Teşvikleri 'e kaydolmak için genel yönetici olmam gerekiyor mu?

Hayır. Hem genel yönetici hem de hesap yöneticisi kullanıcıları teşvikleri yöneticileri olarak atayabilirler. Teşvikleri yöneticileri, şirketin teşvikleri programlarını Iş Ortağı Merkezi aracılığıyla yönetir. Daha fazla bilgi için bkz. [izinlere genel bakış](permissions-overview.md).

## <a name="what-do-i-need-to-do-if-i-find-my-company-is-already-a-member-of-the-microsoft-partner-network-mpn"></a>Şirketimin zaten Microsoft İş Ortağı Ağı (MPN) üyesi olduğunu buldum ne yapmam gerekir?

MPN 'ye katılmayı denerseniz ve şirketiniz zaten bir üyesiyse, MPN etki alanını tanıyacak ve mevcut hesapla ilişkilendirecektir. Mevcut hesap aynı şirket veya aynı e-posta etki alanını kullanan ilişkili bir şirket veya birden çok etki alanını yönetmek için aynı Azure etkinlik dizini (Azure AD) olabilir.

Birincil Ilgili kişiyi yasal profil sayfasından belirleyebilirsiniz. Konumunuzda MPNHQ konumu varsa, teşvikleri yönetmek için gerekli izinlerle ayarlamanız yeterlidir. Roller ve izinler hakkında daha fazla bilgi için bkz. [izinlere genel bakış](permissions-overview.md).

MPNHQ konumuyla aynı ülkede değilseniz, bu senaryo hakkında daha fazla bilgi için [çok milli hesaplara yönelik yönergelere](https://support.microsoft.com/help/4515619/special-considerations-for-multi-national-partners-joining-the-microso) bakın.

## <a name="what-user-roles-are-available"></a>Hangi kullanıcı rolleri kullanılabilir?

Iş Ortağı Merkezi 'nde şirketi kaydeden kişi, varsayılan olarak birincil Iletişim ve genel yönetici olur. Yönetici, portalda kullanıcıları davet edebilir ve yönetebilir.

Teşvikleri için temel roller teşvikleri admin ve teşvikleri User. Teşvikleri Yöneticisi, bir iş ortağı için, ister program, hem de banka ve vergi ayrıntılarını yönetebilir. Teşvikleri Kullanıcı, bir yandan nelerin ödendiğini ve her ödemenin dökümünü, ancak banka ayrıntılarını görüntüleyemez veya düzenleyebileceklerini görmek için araç raporlarını görüntüleyebilir. Her iki rol de Iş ortağı küresel hesabının altındaki tüm konumlara uygulanabilir.

Daha fazla bilgi için bkz. [izinlere genel bakış](permissions-overview.md).

## <a name="how-can-i-find-out-who-has-global-or-account-admin-rights-for-my-company"></a>Şirketim için kimin genel veya hesap yöneticisi haklarına sahip olduğunu nasıl öğrenebilirim?

Rol değişikliği yapan veya yeni bir kullanıcıya rol atayan bir genel yönetici veya hesap yöneticisi bulmak için:

1. Iş Ortağı Merkezi 'nin sağ üst köşesindeki hesap ayarları simgesinden **Kullanıcı yönetimi**' ni seçin.
2. **Genel yönetici** veya **Hesap Yöneticisi** üzerinde filtreleme yapın.
3. Ayrıca, **profilime** gidebilir, **Roller ve izinler** ' i seçebilir ve izinlerinizi yükseltebilmeniz için farklı yöneticilerin bir listesini görebilirsiniz.
 
Daha fazla bilgi için bkz. [rolünüzü bulma](find-your-role.md).  

## <a name="i-cant-access-incentives-using-my-credentials"></a>Kimlik bilgilerimi kullanarak teşvikleri 'ye erişemiyorum.

Teşvikleri görmeme nedeni, doğru izinlere sahip olmadığınızdan emin olmanızdır. Aşağıdaki yordamı kullanarak bkz. çözümü

1. Azure AD Kiracı kimlik bilgilerinizle (iş kimlik bilgileriniz) iş [Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın. Oturum açamıyor, şirketinizin genel yöneticisine başvurun.

2. Oturum açarken, **iş hesabınız** veya **kişisel hesabınız** arasından seçim yapmanız istenirse **iş hesabı**' nı seçin.

3. Iş Ortağı Merkezi menüsünde **teşvikleri**' i seçin ve **genel bakış**' ı seçin. Teşvikleri admin veya teşvikleri User izinleriniz yoksa, şirketinizin tüm genel ve hesap yöneticileri için iletişim bilgileri gösterilir. Gerekli MPN kimliklerine yönelik özenk rolünü almak ve programları teşvik etmek için bu yöneticilerden birine başvurun.

4. Zaten bir teşvikleri yönetici rolüne sahipseniz, kullanıcılarınızın erişim sahibi olduğu MPN kimlikleri ve programları teşvik etmek için kayıtları görürsünüz.

## <a name="some-enrollments-are-missing-from-the-incentives-overview-page"></a>Teşvikleri Genel Bakış sayfasında bazı kayıtlar eksik.

' Dan bir davet aldınız veya ' a kaydolduysanız, artık panoda görünmeyen bir özenk programı ile, uygun erişime sahip olup olmadığınızı iki kez kontrol etmelisiniz. Yalnızca teşvik eden Kullanıcı veya teşvik yönetici rolü olan kullanıcılar programı görebilir. Bkz. [rolünüzü bulma](https://docs.microsoft.com/partner-center/find-your-role).

Rolünüzü veya izinlerinizi değiştirmeniz gerekiyorsa, şirketinizin genel veya hesap yöneticisine başvurun. Bu kişilerin kim olduğunu öğrenmek için [genel yöneticinizle bulun](https://docs.microsoft.com/partner-center/find-your-role#find-your-global-admin)makalesini okuyun.

Genel Bakış sayfasının yalnızca Azure AD kiracısı ile ilişkili Iş ortağı genel hesabıyla (PGA) ilişkili kayıtları görüntüleydiğine göz atın. Şirketinizde birden fazla PGA varsa, her biri için farklı kimlik bilgilerine sahip olmanız gerekir.

## <a name="who-should-i-contact-if-i-get-an-error-message-or-need-help-during-the-enrollment-process"></a>Kayıt işlemi sırasında bir hata iletisi aldığımda veya yardıma ihtiyaç duysam kimler başvurmalıyım?

Panonun teşvikleri bölümünde herhangi bir sorunla karşılaşırsanız çevrimiçi bir destek hizmeti mevcuttur – bkz. destek seçeneği (? Simgesini) sağ üst köşedeki.

## <a name="next-steps"></a>Sonraki adımlar

- [Teşviklerle çalışmaya başlama](incentives-get-started-intro.md)
