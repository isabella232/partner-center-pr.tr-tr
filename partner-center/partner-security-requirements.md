---
title: İş ortağı güvenlik gereksinimleri
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Çok Faktörlü Kimlik Doğrulamasını (MFA) etkinleştirmek ve çok faktörlü kimlik doğrulama çerçevesini benimsemek için Güvenli Uygulama Modeli sunar.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 59e3011099755b9342a00574e0c5bb390e2fd7030a38996368c4127d2fca9518
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115694005"
---
# <a name="security-requirements-for-using-partner-center-or-partner-center-apis"></a>Api'leri veya İş Ortağı Merkezi için İş Ortağı Merkezi gereksinimleri

**Uygun roller:** Tüm İş Ortağı Merkezi kullanıcılar

Bu makalede, Bulut Çözümü Sağlayıcısı programına katılan Danışmanlar, Denetim Masası Satıcıları ve iş ortakları için zorunlu güvenlik gereksinimlerinin yanı sıra kimlik doğrulama seçenekleri ve diğer güvenlik konuları açıklanmıştır. Gizlilik korumaları ve güvenliği en önemli önceliklerimiz arasında yer almaktadır. En iyi savunmanın önleme olduğunu ve en zayıf bağlantımız kadar güçlü olduğunu biliyoruz. İşte bu nedenle ekosistemimiz içinde herkesin harekete geçsin ve uygun güvenlik korumalarının hazır olduğundan emin olasın.

## <a name="mandatory-security-requirements"></a>Zorunlu güvenlik gereksinimleri

Zorunlu güvenlik gereksinimlerini uygulamayan iş ortakları, yönetici temsilcisi haklarını kullanarak Bulut Çözümü Sağlayıcısı programıyla işlem gerçekleştire Bulut Çözümü Sağlayıcısı müşteri kiracılarını yönete etmez. Buna ek olarak, güvenlik gereksinimlerini uygulamayan iş ortakları programlara katılımını riske atabilirsiniz. İş ortağı güvenlik gereksinimleriyle ilişkili koşullar, iş ortağı Microsoft İş Ortağı Sözleşmesi. Danışmanlar ile ilgili olarak, aynı sözleşme gereksinimleri yerine gelecektir.

Sizi ve müşterilerinizi korumak için iş ortaklarının aşağıdaki eylemleri hemen gerçekleştirerek işlemlerini hemen gerçekleştirin:  

1. **İş ortağı kiracınız içinde tüm kullanıcı hesapları için çok faktörlü kimlik doğrulamasını (MFA) etkinleştirin.** İş ortağı kiracıları içinde tüm kullanıcı hesaplarında MFA zorlamanız gerekir. Microsoft ticari bulut hizmetlerinde oturum açmaları veya Bulut Çözümü Sağlayıcısı aracılığıyla veya API'ler aracılığıyla İş Ortağı Merkezi kullanıcılardan MFA tarafından zorlanabilecek.

2. **Güvenli Uygulama Modeli benimseyen.** İş Ortağı Merkezi API'leriyle tüm iş ortaklarının tüm [uygulama ve Güvenli Uygulama Modeli](/partner-center/develop/enable-secure-app-model) kimlik doğrulama modeli uygulamaları için Güvenli Uygulama Modeli çerçevesini benimsemesi gerekir.

    > [!IMPORTANT]
    > İş ortaklarının, MFA zorlandıktan sonra kesinti yaşanmaması için Azure Resource Manager veya Microsoft Graph gibi bir Microsoft API'si ile tümleştirilecek Güvenli Uygulama Modeli'leri ya da kullanıcı kimlik bilgilerini kullanarak PowerShell gibi otomasyondan yararlanarak uygulamalarını kesinlikle öneririz.

Bu güvenlik gereksinimleri altyapınızı korumaya ve müşteri verilerinizi hırsızlık veya diğer sahtekarlık olaylarını tanımlama gibi olası güvenlik risklerinden korumaya yardımcı olur.  

## <a name="implementing-multi-factor-authentication"></a>Çok faktörlü kimlik doğrulamasını uygulama

İş ortağı güvenlik gereksinimlerine uymak için, iş ortağı kiracınız içinde her kullanıcı hesabı için MFA'nın uygulanması ve uygulanması gerekir. Bunu aşağıdaki yöntemlerden birini gerçekleştirebilirsiniz:

- Uygulama [Azure Active Directory (Azure AD) güvenlik varsayılanları.](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults) Sonraki bölümde daha [fazla bilgi bulabilirsiniz.](#security-defaults)

- Her Azure Active Directory Premium hesabı için satın alma hesabı. Daha fazla bilgi için [bkz. Azure AD Multi-Factor Authentication dağıtımı planlama.](/azure/active-directory/authentication/howto-mfa-getstarted)

- İş ortağı kiracınız içinde her kullanıcı hesabı için MFA'nın zorunlu tutulacak bir üçüncü taraf çözümü kullanın. Çözümün beklenen çözümü sağlamayı sağlamak için güvenlik [gereksinimlerinin nasıl uygulanacaklarına bakın.](#how-the-requirements-are-enforced)

> [!NOTE]
> Çok faktörlü kimlik doğrulaması, bağımsız bir bulut (ABD Kamu ve Almanya) için sözleşmeye dayalı olarak gerekli değildir ancak bu güvenlik gereksinimlerini benimsemenizi kesinlikle öneririz.

### <a name="security-defaults"></a>Güvenlik varsayılanları

İş ortaklarının MFA gereksinimlerini uygulamak için seçecekleri seçeneklerden biri, Azure AD'de güvenlik varsayılanlarını etkinleştirmektir. Güvenlik varsayılanları ek ücret ödemeden temel bir güvenlik düzeyi sağlar. Azure AD ile MFA'nın nasıl etkinleştirildiklerine ve güvenlik varsayılanlarını etkinleştirmeden önce aşağıdaki önemli noktalara göz atın.

- Temel ilkeleri zaten benimseyen iş ortaklarının güvenlik varsayılanlarına geçiş yapmak için eyleme geçmelisiniz.

- Güvenlik varsayılanları, önizleme temeli ilkelerinin genel kullanılabilirlik değiştirmesidir. İş ortağı güvenlik varsayılanlarını etkinleştirildiğinde, artık temel ilkeleri etkinleştiremeyecektir.

- Güvenlik varsayılanları ile tüm ilkeler aynı anda etkinleştirilir.

- Koşullu erişim kullanan [iş ortakları](/azure/active-directory/conditional-access/concept-conditional-access-policy-common)için [güvenlik varsayılanları kullanılamaz.](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults)

- Şu anda eski kimlik doğrulamasını engellemez. Ancak, güvenliği tehlikeye atılmış kimliklerle ilgili olayların çoğu eski kimlik doğrulaması kullanan oturum açma girişiminden geldikçe, iş ortaklarının bu eski protokollerden uzaklaşmaları teşvik edilecektir.

- Azure AD Bağlan eşitleme hesabı güvenlik varsayılanlarından dışlandı.

Ayrıntılı bilgi için [bkz. Azure AD Multi-Factor Authentication'a genel bakış ve Güvenlik](/azure/active-directory/authentication/concept-mfa-get-started) [varsayılanları nedir?](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

> [!NOTE]
> Azure AD güvenlik varsayılanları, temel koruma ilkelerinin basitleştirilmiş evrimidir. Temel koruma ilkelerini zaten etkinleştirdiyseniz, güvenlik varsayılanlarını [etkinleştirmeniz kesinlikle önerilir.](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)

## <a name="implementation-considerations"></a>Uygulama konuları

Bu gereksinimler iş ortağı kiracınız içinde tüm kullanıcı hesapları için geçerli olduğundan, sorunsuz bir dağıtım sağlamak için birkaç şeyi göz önünde bulundurmalısınız. Örneğin, Azure AD'de MFA gerçekleştiren kullanıcı hesaplarını ve modern kimlik doğrulamasını desteklemeen uygulamaları ve cihazları tanımlayabilirsiniz.

Herhangi bir eylem gerçekleştirmeden önce aşağıdaki doğrulamaları tamamlamanız önerilir. 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Modern kimlik doğrulaması kullanımını desteklemeen bir uygulama veya cihazınız var mı?

MFA'yi zorunlu tutularak IMAP, POP3, SMTP ve diğerleri gibi eski kimlik doğrulaması kullanım protokolleri engellenir çünkü bunlar MFA'yi desteklemez. Bu sınırlamaya çözüm olarak uygulama [veya cihazın kimliğini doğrulamaya](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) devam etmek için uygulama parolaları özelliğini kullanın. Ortamınız [içinde kullanılamayacaklarını belirlemek için](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) uygulama parolalarını kullanmayla ilgili dikkat edilmesi gerekenleri gözden geçirme.

#### <a name="do-you-have-office-365-users-with-licenses-associated-with-your-partner-tenant"></a>İş ortağı kiracınız Office 365 lisansları olan başka kullanıcılarınız var mı?

Herhangi bir çözümü uygulamadan önce, iş ortağı kiracınız Microsoft Office kullanıcılarının hangi sürümlerinin kullandığını belirlemenizi öneririz. Kullanıcılarınızı, Outlook gibi uygulamalarla ilgili bağlantı sorunlarıyla Outlook. MFA'yi zorlamadan önce, Outlook 2013 SP1 veya sonraki bir sp1 veya sonraki bir sp1'i kullanmaya devam etmek ve kurumda modern kimlik doğrulamasının etkinleştirildiğinden emin olmak önemlidir. Daha fazla bilgi için, [bkz. Enable modern authentication in Exchange Online](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online). 

Microsoft Office 2013 yüklü olan Windows cihazlarda modern kimlik doğrulamasını etkinleştirmek için iki kayıt defteri anahtarı oluşturmanız gerekir. Bkz. [Windows cihazlarda Office 2013 için Modern Windows etkinleştirme.](/office365/admin/security-and-compliance/enable-modern-authentication)

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Kullanıcılarınızı çalışırken mobil cihazlarını kullanmalarını engelleyen bir ilke var mı?

Çalışanların mobil cihazları kullanırken mobil cihazları kullanmalarını engelleyen herhangi bir şirket ilkesi belirlemek önemlidir çünkü bu, hangi MFA çözümünü uygulayanları etkiler. [Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)güvenlik varsayılanları uygulaması aracılığıyla sağlanan ve yalnızca doğrulama için bir kimlik doğrulayıcı uygulamasının kullanımına izin verecek çözümler vardır. Kurumda mobil cihazların kullanımını engelleyen bir ilke varsa aşağıdaki seçeneklerden birini göz önünde bulundurabilirsiniz:

- Güvenli sistemde çalıştırabilirsiniz zaman tabanlı bir kez temel parola (TOTP) uygulaması dağıtın.

- İş ortağı kiracısı içinde en uygun doğrulama seçeneğini sağlayan her kullanıcı hesabı için MFA uygulayan bir üçüncü taraf çözümü uygulama.

- Etkilenen [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) için lisans satın alın.

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>Kimlik doğrulaması için kullanıcı kimlik bilgilerden faydalanmanız gereken otomasyon veya tümleştirme nedir?

İş ortağı dizininize hizmet hesapları dahil olmak üzere her kullanıcı için MFA'nın uygulanması, kimlik doğrulaması için kullanıcı kimlik bilgilerini kullanan tüm otomasyon veya tümleştirmeleri etkiler. Bu nedenle, bu durumlarda hangi hesapların kullanılıyor olduğunu tanımlamanız önemlidir. Dikkate alınarak aşağıdaki örnek uygulama veya hizmetler listesine bakın:

- Müşterileriniz adına kaynak sağlamak için kullanılan denetim masası

- Faturalama için kullanılan tüm platformlarla tümleştirme (CSP programıyla ilgili olduğu gibi) ve müşterilerinize destek

- Az, AzureRM, Azure AD, MS Online ve diğer modülleri kullanan PowerShell betikleri

Yukarıdaki liste kapsamlı değildir. Bu nedenle, ortamınız içinde kimlik doğrulaması için kullanıcı kimlik bilgilerini kullanan tüm uygulama veya hizmetler için eksiksiz bir değerlendirme gerçekleştirmeniz önemlidir. MFA gereksinimini karşılamak için, mümkün olduğunca Güvenli Uygulama Modeli [gerekir.](/partner-center/develop/enable-secure-app-model)

## <a name="accessing-your-environment"></a>Ortamınıza erişme

MFA için ne veya kimlerin kimlik doğrulamasını daha iyi anlamak için oturum açma etkinliğini gözden geçirmenizi öneririz. Bu Azure Active Directory Premium oturum açma raporunu kullanabilirsiniz. Bu konu hakkında daha fazla bilgi için bkz. Azure Active Directory [portalında oturum açma etkinlik raporları.](/azure/active-directory/reports-monitoring/concept-sign-ins) PowerShell aracılığıyla Azure Active Directory Premium veya bu oturum açma etkinliğini elde etmek için bir yol arıyorsanız, powershell modülünden [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity) cmdlet'ini [İş Ortağı Merkezi](https://www.powershellgallery.com/packages/PartnerCenter/) gerekir.

## <a name="how-the-requirements-are-enforced"></a>Gereksinimlerin uygulanması

İş ortağı güvenlik gereksinimleri Azure AD tarafından uygulanır ve İş Ortağı Merkezi, MFA doğrulamasının doğrulanması için MFA talebi olup olamayacak şekilde denetlenerek uygulanır. 18 Kasım 2019'dan itibaren Microsoft, iş ortağı kiracılara ek güvenlik önlemlerini ("teknik uygulama" olarak da bilinir) etkinleştirdi.

Etkinleştirmeden sonra, iş ortağı kiracısı kullanıcılarının (AOBO) işlemleri adına herhangi bir yöneticiyi gerçekleştirirken, İş Ortağı Merkezi portalına erişirken veya api'leri çağırarak MFA doğrulamasını İş Ortağı Merkezi ister. Daha fazla bilgi için [bkz. İş ortağı kiracınız için Çok Faktörlü Kimlik Doğrulamasını (MFA) Mandating](partner-security-requirements-mandating-mfa.md). 

Gereksinimleri karşılamayan iş ortakları, iş kesintilerini önlemek için bu ölçüleri mümkün olan en kısa sürede uygulamalıdır. Multi-Factor Authentication Azure Active Directory Azure AD güvenlik varsayılanlarını kullanıyorsanız, başka bir eyleme ihtiyacınız yoktur.

Üçüncü taraf bir MFA çözümü kullanıyorsanız, MFA talebi verilene bir şans vardır. Bu talep eksikse Azure AD, kimlik doğrulama isteğinin MFA tarafından karşılandı olup olmadığını belirleyemayacak. Çözüme beklenen talebin nasıl verili olduğunu doğrulama hakkında bilgi için İş Ortağı Güvenlik [Gereksinimlerini Test Etme makalesi'ne bakın.](/powershell/partnercenter/test-partner-security-requirements) 

> [!IMPORTANT]
> Üçüncü taraf çözümünüz beklenen talebi yoksa, hangi eylemlerin gerçekleştirileceklerini belirlemek için çözümü geliştiren satıcıyla birlikte çalışmanız gerekir.

## <a name="resources-and-samples"></a>Kaynaklar ve örnekler

Destek ve örnek kod için aşağıdaki kaynaklara bakın:

- [İş Ortağı Merkezi Rehberlik](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)Grubu topluluğu: İş Ortağı Merkezi Güvenlik Kılavuzu Grubu topluluğu, yaklaşan etkinlikler hakkında bilgi edinebilirsiniz ve sorularınız varsa sorabilirsiniz.
- [İş Ortağı Merkezi .NET Örnekleri:](https://github.com/microsoft/partner-center-dotnet-samples)Bu GitHub deposu, .NET kullanılarak geliştirilen ve bu çerçeveyi nasıl uygulaya Güvenli Uygulama Modeli içerir.
- [İş Ortağı Merkezi Java Örnekleri:](https://github.com/microsoft/partner-center-java-samples)Bu GitHub, Java kullanılarak geliştirilen ve bu çerçeveyi nasıl uygulaya Güvenli Uygulama Modeli içerir.
- [İş Ortağı Merkezi PowerShell - Multi-Factor Authentication:](/powershell/partnercenter/multi-factor-auth)Bu Multi-Factor Authentication makalesi, PowerShell kullanarak Güvenli Uygulama Modeli çerçevesinin nasıl uygulanarak ilgili ayrıntıları sağlar.

## <a name="next-steps"></a>Sonraki adımlar

- [İş ortağı kiracınız için Çok Faktörlü Kimlik Doğrulaması'nın (MFA) mandating](partner-security-requirements-mandating-mfa.md)