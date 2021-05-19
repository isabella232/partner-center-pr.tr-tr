---
title: İş ortağı güvenlik gereksinimleri
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Çok Faktörlü Kimlik Doğrulamasını (MFA) etkinleştirmek ve çok faktörlü kimlik doğrulama çerçevesini benimsemek için Güvenli Uygulama Modeli sunar.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 201ea34d30814974936da032805f1ee7dfa590be
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110145856"
---
# <a name="security-requirements-for-using-partner-center-or-partner-center-apis"></a>Api'leri veya İş Ortağı Merkezi için İş Ortağı Merkezi gereksinimleri

**Uygun roller:** Tüm İş Ortağı Merkezi kullanıcılar

Bu makalede, Bulut Çözümü Sağlayıcısı programına katılan Danışmanlar, Denetim Masası Satıcıları ve iş ortakları için zorunlu güvenlik gereksinimlerinin yanı sıra kimlik doğrulama seçenekleri ve diğer güvenlik konuları açıklanmıştır. Gizlilik korumaları ve güvenliği en önemli önceliklerimiz arasında yer almaktadır. En iyi savunmanın önleme olduğunu ve en zayıf bağlantımız kadar güçlü olduğunu biliyoruz. İşte bu nedenle ekosistemimiz içinde herkesin harekete geçsin ve uygun güvenlik korumalarının hazır olduğundan emin olasın.

## <a name="mandatory-security-requirements"></a>Zorunlu güvenlik gereksinimleri

Zorunlu güvenlik gereksinimlerini uygulamayan iş ortakları, yönetici temsilcisi haklarını kullanarak Bulut Çözümü Sağlayıcısı programıyla işlem gerçekleştire Bulut Çözümü Sağlayıcısı müşteri kiracılarını yönete etmez. Buna ek olarak, güvenlik gereksinimlerini uygulamayan iş ortakları programlara katılımını riske atabilirsiniz. İş ortağı güvenlik gereksinimleriyle ilişkili koşullar, Microsoft İş Ortağı Sözleşmesi. Danışmanlar ile ilgili olarak, aynı sözleşme gereksinimleri yerine gelecektir.

Sizi ve müşterilerinizi korumak için iş ortaklarının aşağıdaki eylemleri hemen gerçekleştirerek işlemlerden birini gerçekleştirin:  

1. **İş ortağı kiracınız içinde tüm kullanıcı hesapları için çok faktörlü kimlik doğrulamasını (MFA) etkinleştirin.** İş ortağı kiracıları içinde tüm kullanıcı hesaplarında MFA zorlamanız gerekir. Microsoft ticari bulut hizmetlerinde oturum açmaları veya Bulut Çözümü Sağlayıcısı aracılığıyla veya API'ler aracılığıyla İş Ortağı Merkezi kullanıcılardan MFA tarafından zorlanabilecek.

2. **Güvenli Uygulama Modeli benimseyen.** İş Ortağı Merkezi API'leriyle tüm iş ortaklarının tüm [uygulama ve Güvenli Uygulama Modeli](/partner-center/develop/enable-secure-app-model) kimlik doğrulama modeli uygulamaları için Güvenli Uygulama Modeli çerçevesini benimsemesi gerekir.

    > [!IMPORTANT]
    > İş ortaklarının Azure Resource Manager veya Microsoft Graph gibi bir Microsoft API'si ile tümleştirme için Güvenli Uygulama Modeli'yi veya MFA zorlandıktan sonra kesinti yaşanmaması için PowerShell gibi otomasyondan kullanıcı kimlik bilgilerini kullanarak kullanmalarını kesinlikle öneririz.

Bu güvenlik gereksinimleri altyapınızı korumaya ve müşteri verilerinizi hırsızlık veya diğer sahtekarlık olaylarını tanımlama gibi olası güvenlik risklerinden korumaya yardımcı olur.  

## <a name="implementing-multi-factor-authentication"></a>Çok faktörlü kimlik doğrulamasını uygulama

İş ortağı güvenlik gereksinimlerine uymak için, iş ortağı kiracınız içinde her kullanıcı hesabı için MFA'nın uygulanması ve uygulanması gerekir. Bunu aşağıdaki yöntemlerden birini gerçekleştirebilirsiniz:

- Uygulama [Azure Active Directory (Azure AD) güvenlik varsayılanları.](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults) Sonraki bölümde daha [fazla bilgi bulabilirsiniz.](#security-defaults)

- Her Azure Active Directory Premium hesabı için satın alma hesabı. Daha fazla bilgi için [bkz. Azure AD Multi-Factor Authentication dağıtımı planlama.](/azure/active-directory/authentication/howto-mfa-getstarted)

- İş ortağı kiracınız içinde her kullanıcı hesabı için MFA'nın zorunlu tutulacak bir üçüncü taraf çözümü kullanın. Çözümün beklenen çözümü sağlamalarını sağlamak için güvenlik [gereksinimlerinin nasıl uygulanacaklarına bakın.](#how-the-requirements-are-enforced)

> [!NOTE]
> Çok faktörlü kimlik doğrulaması, bağımsız bir bulut (ABD Kamu ve Almanya) için sözleşmeye dayalı olarak gerekli değildir ancak bu güvenlik gereksinimlerini benimsemenizi kesinlikle öneririz.

### <a name="security-defaults"></a>Güvenlik varsayılanları

İş ortaklarının MFA gereksinimlerini uygulamak için seçecekleri seçeneklerden biri, Azure AD'de güvenlik varsayılanlarını etkinleştirmektir. Güvenlik varsayılanları ek ücret ödemeden temel bir güvenlik düzeyi sağlar. Azure AD ile MFA'nın nasıl etkinleştirildi ve güvenlik varsayılanlarını etkinleştirmeden önce aşağıdaki önemli noktalara göz atın.

- Temel ilkeleri zaten benimseyen iş ortaklarının güvenlik varsayılanlarına geçiş yapmak için eyleme geçmelisiniz.

- Güvenlik varsayılanları, önizleme temeli ilkelerinin genel kullanılabilirlik değiştirmesidir. İş ortağı güvenlik varsayılanlarını etkinleştirildiğinde, artık temel ilkeleri etkinleştiremeyecektir.

- Güvenlik varsayılanları ile tüm ilkeler aynı anda etkinleştirilir.

- [Koşullu erişim](/azure/active-directory/conditional-access/concept-conditional-access-policy-common)kullanan iş ortakları için [güvenlik Varsayılanları kullanılabilir](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults)olmayacaktır.

- Şu anda eski kimlik doğrulamasını engelliyoruz. Ancak, güvenliği aşılmış kimlikler ile ilgili çoğu olay, eski kimlik doğrulamasını kullanan oturum açma girişiminizden geliyorsa, iş ortaklarının bu eski protokollerden uzaklaşmaları önerilir.

- Azure AD Connect eşitleme hesabı, güvenlik varsayılanlarından çıkarılır.

Ayrıntılı bilgi için, [Kuruluşunuz Için Azure AD Multi-Factor Authentication genel bakış](/azure/active-directory/authentication/concept-mfa-get-started) ve [güvenlik Varsayılanları nelerdir?](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

> [!NOTE]
> Azure AD güvenlik Varsayılanları, ana hat koruma ilkelerinin basitleşme evidir. Temel koruma ilkelerini zaten etkinleştirdiyseniz, [güvenlik varsayılanlarını](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)etkinleştirmeniz önemle önerilir.

## <a name="implementation-considerations"></a>Uygulama konuları

Bu gereksinimler iş ortağı kiracınızdaki tüm kullanıcı hesaplarına uygulandığından, sorunsuz bir dağıtım sağlamak için birkaç şeyi göz önünde bulundurmanız gerekir. Örneğin, Azure AD 'de, kuruluşunuzda modern kimlik doğrulamayı desteklemeyen MFA ve uygulamalar ve cihazlar gerçekleştirebilecek Kullanıcı hesaplarını belirleyebilirsiniz.

Herhangi bir işlem gerçekleştirmeden önce aşağıdaki doğrulamaları tamamlamanızı öneririz. 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Modern kimlik doğrulaması kullanımını desteklemeyen bir uygulama veya cihazınız mı var?

MFA 'yı zorunlu kılmak için, eski kimlik doğrulama, IMAP, POP3, SMTP ve diğer kullanıcıların MFA 'yı desteklemediği için bu protokolleri engellenecektir. Bu sınırlamaya yönelik olarak, uygulamanın veya cihazın kimlik doğrulamasının devam ettiğinden emin olmak için [Uygulama parolaları](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) özelliğini kullanın. Ortamınızda kullanılabilecekleri olup olmadıklarını öğrenmek için [uygulama parolalarını kullanma konularını](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) gözden geçirin.

#### <a name="do-you-have-office-365-users-with-licenses-associated-with-your-partner-tenant"></a>Office 365 kullanıcılarınıza iş ortağı kiracınızla ilişkili lisanslar mı var?

Herhangi bir çözümü uygulamadan önce, iş ortağı kiracınızda Microsoft Office kullanıcıların hangi sürümlerinin kullandığını belirlemenizi öneririz. Kullanıcılarınız Outlook gibi uygulamalarla bağlantı sorunlarıyla karşılaşacaktır. MFA'yi zorlamadan önce, Outlook 2013 SP1 veya sonraki bir sonraki bir sp1'i kullanmak ve modern kimlik doğrulamasının etkinleştirildiğinden emin olmak önemlidir. Daha fazla bilgi için [bkz. Exchange Online'da modern kimlik doğrulamasını etkinleştirme.](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online) 

Microsoft Office 2013 yüklü Windows çalıştıran cihazlarda modern kimlik doğrulamasını etkinleştirmek için iki kayıt defteri anahtarı oluşturmanız gerekir. Bkz. [Windows cihazlarda Office 2013 için Modern Kimlik Doğrulamasını Etkinleştirme.](/office365/admin/security-and-compliance/enable-modern-authentication)

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Kullanıcılarınızı çalışırken mobil cihazlarını kullanmalarını engelleyen bir ilke var mı?

Çalışanların mobil cihazları kullanırken mobil cihazları kullanmalarını engelleyen herhangi bir şirket ilkesi belirlemek önemlidir çünkü bu, hangi MFA çözümünü uygulayanları etkiler. [Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)güvenlik varsayılanları uygulaması aracılığıyla sağlanan ve yalnızca doğrulama için bir kimlik doğrulayıcı uygulamasının kullanımına izin verecek çözümler vardır. Kurumda mobil cihazların kullanımını engelleyen bir ilke varsa aşağıdaki seçeneklerden birini göz önünde bulundurabilirsiniz:

- Güvenli sistemde çalıştırabilirsiniz zaman tabanlı bir kez temel parola (TOTP) uygulaması dağıtın.

- İş ortağı kiracısı içinde en uygun doğrulama seçeneğini sağlayan her kullanıcı hesabı için MFA uygulayan bir üçüncü taraf çözümü uygulama.

- Etkilenen [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) için lisans satın alın.

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>Kimlik doğrulaması için kullanıcı kimlik bilgilerden faydalanmanız gereken otomasyon veya tümleştirme nedir?

İş ortağı dizininize hizmet hesapları dahil olmak üzere her kullanıcı için MFA'nın uygulanması, kimlik doğrulaması için kullanıcı kimlik bilgilerini kullanan tüm otomasyon veya tümleştirmeleri etkiler. Bu nedenle, bu durumlarda hangi hesapların kullanılıyor olduğunu tanımlamanız önemlidir. Dikkate alınarak aşağıdaki örnek uygulamalar veya hizmetler listesine bakın:

- Müşterileriniz adına kaynak sağlamak için kullanılan denetim masası

- Faturalama için kullanılan tüm platformlarla tümleştirme (CSP programıyla ilgili olduğu gibi) ve müşterilerinize destek

- Az, AzureRM, Azure AD, MS online ve diğer modülleri kullanan PowerShell betikleri

Yukarıdaki liste kapsamlı değildir. Bu nedenle, ortamınızda kimlik doğrulaması için Kullanıcı kimlik bilgilerini kullanan herhangi bir uygulamayı veya hizmeti bir bütün değerlendirmede gerçekleştirmeniz önemlidir. MFA gereksinimini karşılamak için, Kılavuzu mümkün olduğunda [güvenli uygulama modeli çerçevesinde](/partner-center/develop/enable-secure-app-model) uygulamanız gerekir.

## <a name="accessing-your-environment"></a>Ortamınıza erişme

MFA için istemeden kimlik doğrulaması yapan ne olduğunu daha iyi anlamak için oturum açma etkinliğini incelemenizi öneririz. Azure Active Directory Premium aracılığıyla oturum açma raporunu kullanabilirsiniz. Bu konu hakkında daha fazla bilgi için, [Azure Active Directory portalındaki oturum açma etkinliği raporları](/azure/active-directory/reports-monitoring/concept-sign-ins)bölümüne bakın. Azure Active Directory Premium yoksa veya PowerShell aracılığıyla bu oturum açma etkinliğini elde etmek istiyorsanız, [Iş Ortağı Merkezi PowerShell](https://www.powershellgallery.com/packages/PartnerCenter/) modülünden [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity) cmdlet 'ini kullanmanız gerekir.

## <a name="how-the-requirements-are-enforced"></a>Gereksinimler nasıl zorlanır

İş ortağı güvenlik gereksinimleri, Azure AD tarafından zorlanır ve Iş Ortağı Merkezi 'nde MFA doğrulamasının gerçekleştiğinden emin olmak için MFA talebinin varlığını kontrol ederek yapılır. Microsoft, 18 Kasım 2019 ' den itibaren iş ortağı kiracılarına ek güvenlik korumalarını (daha önce "teknik uygulama" olarak biliniyordu) etkinleştirdi.

Etkinleştirme sonrasında, iş ortağı kiracısındaki kullanıcıların her türlü yönetici (AOBO) işlemini gerçekleştirirken, Iş Ortağı Merkezi portalına erişirken veya Iş Ortağı Merkezi API 'Lerini çağırarak MFA doğrulamasını tamamlaması istenir. Daha fazla bilgi için bkz. [iş ortağı kiracınız Için Mandating Multi-Factor Authentication (MFA)](partner-security-requirements-mandating-mfa.md). 

Gereksinimleri karşılamayan iş ortakları, herhangi bir iş kesintilerini önlemek için bu ölçüleri en kısa sürede uygulamalıdır. Azure Active Directory Multi-Factor Authentication veya Azure AD güvenlik varsayılanlarını kullanıyorsanız, uygulamanız gereken başka bir eylem yoktur.

Üçüncü taraf bir MFA çözümü kullanıyorsanız, MFA talebinin verilmeyebilir bir şansınız vardır. Bu talep yoksa, Azure AD kimlik doğrulama isteğinin MFA tarafından mı öncelikli olduğunu belirleyemeyecektir. Çözümünüzün beklenen talebi verme hakkında daha fazla bilgi için, [Iş ortağı güvenlik gereksinimlerini test](/powershell/partnercenter/test-partner-security-requirements)edin. 

> [!IMPORTANT]
> Üçüncü taraf çözümünüz beklenen talebi yayınleyemiyorsa, hangi eylemlerin alınacağını belirlemek için çözümü geliştiren satıcıyla çalışmanız gerekir.

## <a name="resources-and-samples"></a>Kaynaklar ve örnekler

Destek ve örnek kod için aşağıdaki kaynaklara bakın:

- [Iş Ortağı Merkezi Güvenlik Kılavuzu grubu topluluğu](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): Iş Ortağı Merkezi Güvenlik Kılavuzu grubu topluluğu, yaklaşan olaylar hakkında bilgi edinmek ve sahip olabileceğiniz sorularınızı sormak için kullanabileceğiniz bir çevrimiçi toplulukdır.
- [Iş ortağı merkezi .NET örnekleri](https://github.com/microsoft/partner-center-dotnet-samples): Bu GitHub deposu, .NET kullanılarak geliştirilen ve güvenli uygulama modeli çerçevesini nasıl uygulayabileceğinizi gösteren örnekler içerir.
- [Iş ortağı merkezi Java örnekleri](https://github.com/microsoft/partner-center-java-samples): Bu GitHub deposu, Java kullanılarak geliştirilen ve güvenli uygulama modeli çerçevesini nasıl uygulayabileceğinizi gösteren örnekler içerir.
- [Iş Ortağı Merkezi PowerShell-Multi-Factor Authentication](/powershell/partnercenter/multi-factor-auth): bu Multi-Factor Authentication makale, PowerShell kullanarak güvenli uygulama modeli çerçevesinin nasıl uygulanacağı hakkında ayrıntılı bilgi sağlar.

## <a name="next-steps"></a>Sonraki adımlar

- [İş ortağı kiracınız için Mandating Multi-Factor Authentication (MFA)](partner-security-requirements-mandating-mfa.md)