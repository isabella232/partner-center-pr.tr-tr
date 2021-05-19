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
ms.openlocfilehash: a917f3648447ac273fae839d32a4b4d3ce80ae35
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152027"
---
# <a name="frequently-asked-questions-on-incentives"></a>Teşvikleri hakkında sık sorulan sorular

**Uygun roller**: teşvikleri admin | Teşvikleri kullanıcısı

## <a name="do-i-need-to-be-the-global-admin-to-enroll-in-incentives"></a>Teşvikleri 'e kaydolmak için genel yönetici olmam gerekiyor mu?

Hayır. Hem genel yönetici hem de hesap yöneticisi kullanıcıları teşvikleri yöneticileri olarak atayabilirler. Teşvikleri yöneticileri, şirketin teşvikleri programlarını Iş Ortağı Merkezi aracılığıyla yönetir. Daha fazla bilgi için bkz. [izinlere genel bakış](permissions-overview.md).

## <a name="what-do-i-need-to-do-if-i-find-my-company-is-already-a-member-of-the-microsoft-partner-network-mpn"></a>Şirketimin zaten Microsoft İş Ortağı Ağı (MPN) üyesi olduğunu buldum ne yapmam gerekir?

MPN 'ye katılmayı denerseniz ve şirketiniz zaten bir üyesiyse, MPN etki alanını tanıyacak ve mevcut hesapla ilişkilendirecektir. Mevcut hesap aynı şirket veya aynı e-posta etki alanını kullanan ilişkili bir şirket veya birden çok etki alanını yönetmek için aynı Azure etkinlik dizini (Azure AD) olabilir.

Birincil Ilgili kişiyi yasal profil sayfasından belirleyebilirsiniz. Konumunuzda MPNHQ konumu varsa, teşvikleri yönetmek için gerekli izinlerle ayarlamanız yeterlidir. Roller ve izinler hakkında daha fazla bilgi için bkz. [izinlere genel bakış](permissions-overview.md).

MPNHQ konumuyla aynı ülkede değilseniz, bu senaryo hakkında daha fazla bilgi için [çok milli hesaplara yönelik yönergelere](https://support.microsoft.com/help/4515619/special-considerations-for-multi-national-partners-joining-the-microso) bakın.

## <a name="what-user-roles-are-available"></a>Hangi kullanıcı rolleri kullanılabilir?

Iş Ortağı Merkezi 'nde şirketi kaydeden kişi, varsayılan olarak birincil Iletişim ve genel yönetici olur. Yönetici, portalda kullanıcıları davet edebilir ve yönetebilir.

Teşvikleri için temel roller teşvikleri admin ve teşvikleri User. Teşvikler yöneticisi teşvik programlarına kaydolarak iş ortağının banka ve vergi ayrıntılarını yönetebilir. Teşvikler kullanıcısı, neyin ödenmiş olduğunu ve her ödemenin dökümünü görmek için araçta raporları görüntüleyemez, ancak banka ayrıntılarını görüntüleyemez veya düzenleyemez. Her iki rol de İş ortağı genel hesabı altındaki tüm konumlara uygulanabilir.

Daha fazla bilgi için bkz. [İzinlere genel bakış.](permissions-overview.md)

## <a name="how-can-i-find-out-who-has-global-or-account-admin-rights-for-my-company"></a>Şirketim için kimlerin Genel veya Hesap yöneticisi haklarına sahip olduğunu nasıl bulamıyorum?

Rol değişiklikleri yapan veya yeni bir kullanıcıya rol atayan genel yöneticiyi veya Hesap yöneticisini bulmak için:

1. Uygulamanın sağ üst köşesindeki Hesap ayarları simgesinden kullanıcı **İş Ortağı Merkezi'yi seçin.**
2. Genel yönetici veya **Hesap yöneticisi** **filtresini seçin.**
3. Ayrıca,  **Profilim'a** gidebilir, Roller ve izinler'i seçerek izinlerinizi yükseltmenize yardımcı olacak farklı yöneticilerin listesini de ekleyebilirsiniz.
 
Daha fazla bilgi için [bkz. Rollerinizi bulma.](find-your-role.md)  

## <a name="i-cant-access-incentives-using-my-credentials"></a>Kimlik bilgilerimi kullanarak teşviklere erişe bilmiyorum.

Teşvikleri görememe ihtimaliniz, doğru izinlere sahip olmadığınızdır. Bunu düzeltmek için aşağıdaki yordamı kullanın.

1. Azure AD [kiracı İş Ortağı Merkezi (iş](https://partner.microsoft.com/dashboard/) kimlik bilgileriniz) ile panoda oturum açın. Oturum açamıyorsanız, şirketin genel yöneticisine başvurun.

2. Oturum aken, İş hesabınız veya Kişisel hesabınızdan seçmeniz **istenirse** İş hesabı'ı **seçin.**

3. Yeni İş Ortağı Merkezi Teşvikler'i **ve ardından** Genel Bakış'ı **seçin.** Teşvikler yöneticisi veya Teşvikler kullanıcı izinlerine sahip değilseniz, şirketinizin tüm genel ve hesap yöneticileri için iletişim bilgileri gösterilir. Gerekli MPN kimlikleri ve teşvik programları için teşvik rolünü almak için bu yöneticilerden biri ile iletişime geçin.

4. Zaten bir Teşvikler yönetici rolünüz varsa, erişiminiz olan MPN kimlikleri ve teşvik programları için şirketinizin kayıtlarına bakabilirsiniz.

## <a name="some-enrollments-are-missing-from-the-incentives-overview-page"></a>Teşviklere genel bakış sayfasında bazı kayıtlar eksik.

Panoda artık görünür olmayan bir teşvik programından davet aldıysanız veya kaydolduysanız, uygun erişime sahip olup olmadığınıza bir kez daha bakabilirsiniz. Programı yalnızca Teşvik Kullanıcısı veya Teşvik Yöneticisi rolüne sahip kullanıcılar görebilir. Bkz. [Rollerinizi bulma.](./find-your-role.md)

Rol veya izinlerinizi değiştirmeniz gerekirse, şirketin genel yöneticisine veya hesap yöneticisine ulaşın. Bu kişilerin kim olduğunu öğrenmek için Genel [yöneticinizi bulma makalenizi okuyun.](./find-your-role.md#find-your-global-admin)

Genel Bakış sayfasında yalnızca Azure AD kiracısı ile ilişkili İş Ortağı Genel Hesabı (PGA) ile ilişkili kayıtlar görüntülenir. Şirketinizin birden fazla PGA'sı varsa, her biri için farklı kimlik bilgilerine sahip olmak gerekir.

## <a name="who-should-i-contact-if-i-get-an-error-message-or-need-help-during-the-enrollment-process"></a>Hata iletisiyle karşılaştım veya kayıt işlemi sırasında yardıma ihtiyacım olursa kimle iletişim kurmam gerekir?

Panonun Teşvikler bölümünde herhangi bir sorunla karşılaşırsanız çevrimiçi bir destek hizmeti vardır; bkz. destek seçeneği (? Simgesi) seçin.

## <a name="next-steps"></a>Sonraki adımlar

- [Teşviklerle çalışmaya başlama](incentives-get-started-intro.md)