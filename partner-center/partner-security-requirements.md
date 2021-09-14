---
title: İş ortağı güvenlik gereksinimleri
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Multi-Factor Authentication 'ı (MFA) etkinleştirmek ve güvenli uygulama modeli çerçevesini benimsemek için iş ortağı güvenlik gereksinimlerini tanıtır.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 8966d744dfb70a7850ef6d3dd68d2051344fe9cd
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248683"
---
# <a name="security-requirements-for-using-partner-center-or-partner-center-apis"></a>Iş ortağı merkezi veya Iş Ortağı Merkezi API 'Lerini kullanmaya yönelik güvenlik gereksinimleri

**Uygun roller**: tüm Iş Ortağı Merkezi kullanıcıları

bu makalede, danışmanların, denetim masası satıcılarının ve Bulut Çözümü Sağlayıcısı programına katılan iş ortaklarının yanı sıra kimlik doğrulama seçenekleri ve diğer güvenlik konuları için zorunlu güvenlik gereksinimleri açıklanmaktadır. Gizlilik korumaları ve güvenlik, en iyi önceliklerimiz arasındadır. En iyi savunması önleme olduğunu ve yalnızca zayıf bağlantımız kadar güçlü olduğunu biliyoruz. Bu nedenle, ekosistemimizde herkesin işlem yapması ve uygun güvenlik korumalarının yerinde olduğundan emin olunması gerekir.

## <a name="mandatory-security-requirements"></a>Zorunlu güvenlik gereksinimleri

zorunlu güvenlik gereksinimlerini uygulamayan iş ortakları Bulut Çözümü Sağlayıcısı programda transact veya yönetici temsilcisi hakları kullanarak müşteri kiracılarını yönetemez. Ayrıca, güvenlik gereksinimlerini uygulamayan iş ortakları, risk altındaki programlara katılımını uygulayabilir. İş ortağı güvenlik gereksinimleriyle ilişkili şartlar Microsoft Iş ortağı Sözleşmesi ' ne eklenmiştir. Danışmanlarıyla ilgili olarak, sözleşmeli gereksinimlerin de aynı olması gerekir.

Sizi ve müşterilerinizi korumak için iş ortaklarının aşağıdaki eylemleri hemen ele geçirmesine gerek duyuluyoruz:  

1. **İş ortağı kiracınızdaki tüm Kullanıcı hesapları için Multi-Factor Authentication 'ı (MFA) etkinleştirin**. İş ortağı kiracınızdaki tüm Kullanıcı hesaplarında MFA 'yı zorunlu kılabilirsiniz. kullanıcılar, Microsoft ticari bulut hizmetlerinde oturum açtıklarında veya iş ortağı merkezi aracılığıyla veya apı 'ler aracılığıyla Bulut Çözümü Sağlayıcısı programda transact, MFA tarafından öncelikli olarak gelmelidir.

2. **Güvenli uygulama modeli çerçevesini benimseyin**. Iş Ortağı Merkezi API 'Leriyle Tümleştirdiğiniz tüm iş ortakları, tüm uygulama ve Kullanıcı kimlik doğrulama modeli uygulamaları için [güvenli uygulama modeli çerçevesini](/partner-center/develop/enable-secure-app-model) benimsemelidir.

    > [!IMPORTANT]
    > iş ortaklarının, Azure Resource Manager veya Microsoft Graph gibi bir Microsoft apı 'siyle tümleştirme için ya da MFA zorlandığında herhangi bir kesinti yaşamamak için kullanıcı kimlik bilgilerini kullanarak PowerShell gibi otomasyondan yararlanmak üzere güvenli uygulama modelini uygulamanızı önemle öneririz.

Bu güvenlik gereksinimleri, altyapınızın korunmasına ve müşterilerinizin verilerini hırsızlık veya diğer sahtekarlık olaylarını belirlemek gibi olası güvenlik risklerine karşı korumanıza yardımcı olur.  

## <a name="implementing-multi-factor-authentication"></a>Multi-Factor Authentication uygulama

İş ortağı güvenlik gereksinimleriyle uyum sağlamak için, iş ortağı kiracınızdaki her kullanıcı hesabı için MFA 'yı uygulamanız ve zorunlu kılabilirsiniz. Bunu aşağıdaki yollardan birini yapabilirsiniz:

- [Azure Active Directory (Azure AD) güvenlik varsayılanlarını](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)uygulayın. [Sonraki bölümde](#security-defaults)daha fazla bilgi bulabilirsiniz.

- her kullanıcı hesabı için Azure Active Directory Premium satın alın. Daha fazla bilgi için bkz. [Azure AD Multi-Factor Authentication dağıtımı planlaması](/azure/active-directory/authentication/howto-mfa-getstarted).

- İş ortağı kiracınızdaki her kullanıcı hesabı için MFA 'yı zorlamak üzere bir üçüncü taraf çözümü kullanın. Çözümün beklenen çözümü sağlayacağız emin olmak için, bkz. [güvenlik gereksinimlerinin nasıl zorlanacağını](#how-the-requirements-are-enforced).

> [!NOTE]
> Çok faktörlü kimlik doğrulaması, bir sogeign bulutu için gerekli olmasa da (ABD devlet ve Almanya), bu güvenlik gereksinimlerini benimsemeniz kesinlikle önerilir.

### <a name="security-defaults"></a>Güvenlik varsayılanları

İş ortaklarının MFA gereksinimlerini uygulamak için seçim seçebileceğine ilişkin seçeneklerden biri, Azure AD 'de güvenlik varsayılanlarını etkinleştirmektir. Güvenlik Varsayılanları, ek ücret ödemeden temel düzeyde güvenlik sunar. Azure AD ile kuruluşunuz için MFA 'yı etkinleştirme ve güvenlik varsayılanlarını etkinleştirmeden önce aşağıdaki önemli noktalar hakkında gözden geçirin.

- Temel ilkelerini benimseyen iş ortaklarının, güvenlik varsayılanlarına geçiş yapmak için işlem yapması gerekir.

- Güvenlik Varsayılanları, önizleme temeli ilkelerinin genel kullanıma sunulduğuna yönelik olarak değişiklik yapar. Bir iş ortağı güvenlik varsayılanlarını etkinleştirdikten sonra, artık temel ilkeleri etkinleştiremeyecektir.

- Güvenlik varsayılanları ile tüm ilkeler aynı anda etkin olur.

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

#### <a name="do-you-have-office-365-users-with-licenses-associated-with-your-partner-tenant"></a>iş ortağı kiracınızla ilişkili lisansa sahip Office 365 kullanıcılarınız var mı?

herhangi bir çözümü uygulamadan önce, iş ortağı kiracınızda Microsoft Office kullanıcıların hangi sürümlerinin kullandığını belirlemenizi öneririz. Kullanıcılarınızın Outlook gibi uygulamalarla bağlantı sorunlarıyla karşılaşması olasılığı vardır. MFA 'yı zorlamadan önce, Outlook 2013 SP1 veya sonraki bir sürümünü kullandığınızdan ve kuruluşunuzun modern kimlik doğrulamasının etkin olduğundan emin olmak önemlidir. Daha fazla bilgi için bkz. [Exchange Online modern kimlik doğrulamasını etkinleştirme](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online). 

Microsoft Office 2013 yüklü Windows çalıştıran cihazlarda modern kimlik doğrulamayı etkinleştirmek için iki kayıt defteri anahtarı oluşturmanız gerekir. bkz. [Windows cihazlarda Office 2013 için Modern kimlik doğrulamasını etkinleştirme](/office365/admin/security-and-compliance/enable-modern-authentication).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Kullanıcılarınız çalışırken kullanıcılarınızın mobil cihazlarını kullanmasını engellemiş bir ilke var mı?

Çalışanların mobil cihazları kullanmasını engelleyen herhangi bir kurumsal ilkeyi tanımlamak önemlidir çünkü bu, hangi MFA çözümünü uygulayacağınızı etkiler. [Azure AD güvenlik Varsayılanları](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)'nın uygulanmasıyla, yalnızca doğrulama için bir Authenticator uygulamasının kullanılmasına izin veren bir çözüm vardır. Kuruluşunuzun mobil cihazların kullanımını engellediği bir ilkesi varsa, aşağıdaki seçeneklerden birini göz önünde bulundurun:

- Güvenli sistem üzerinde çalışabilen zamana bağlı bir kerelik ana parola (TOTP) uygulaması dağıtın.

- En uygun doğrulama seçeneğini sağlayan iş ortağı kiracısındaki her kullanıcı hesabı için MFA 'yı zorlayan bir üçüncü taraf çözümü uygulayın.

- etkilenen kullanıcılar için [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) lisansları satın alın.

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>Kimlik doğrulaması için Kullanıcı kimlik bilgileriyle hangi Otomasyon veya tümleştirmeyi kullanıyorsunuz?

Hizmet hesapları da dahil olmak üzere her bir kullanıcı için MFA 'yı zorlayacağız, bu, kimlik doğrulaması için Kullanıcı kimlik bilgilerini kullanan tüm otomasyonu veya tümleştirmeyi etkileyecektir. Bu nedenle, bu durumlarda hangi hesapların kullanıldığını belirlemeniz önemlidir. Göz önünde bulundurmanız gereken örnek uygulamalar veya Hizmetler listesine bakın:

- Müşterileriniz adına kaynak sağlamak için kullanılan denetim masası

- Faturalandırma için kullanılan platformlarla Tümleştirme (CSP programı ile ilişkili olduğu gibi) ve müşterilerinizi destekleme

- Az, AzureRM, Azure AD, MS online ve diğer modülleri kullanan PowerShell betikleri

Yukarıdaki liste kapsamlı değildir. Bu nedenle, ortamınızda kimlik doğrulaması için Kullanıcı kimlik bilgilerini kullanan herhangi bir uygulamayı veya hizmeti bir bütün değerlendirmede gerçekleştirmeniz önemlidir. MFA gereksinimini karşılamak için, Kılavuzu mümkün olduğunda [güvenli uygulama modeli çerçevesinde](/partner-center/develop/enable-secure-app-model) uygulamanız gerekir.

## <a name="accessing-your-environment"></a>Ortamınıza erişme

MFA için istemeden kimlik doğrulaması yapan ne olduğunu daha iyi anlamak için oturum açma etkinliğini incelemenizi öneririz. Azure Active Directory Premium aracılığıyla oturum açma raporunu kullanabilirsiniz. bu konu hakkında daha fazla bilgi için, [Azure Active Directory portalındaki oturum açma etkinliği raporları](/azure/active-directory/reports-monitoring/concept-sign-ins)bölümüne bakın. Azure Active Directory Premium yoksa veya PowerShell aracılığıyla bu oturum açma etkinliğini elde etmek istiyorsanız, [iş ortağı merkezi powershell](https://www.powershellgallery.com/packages/PartnerCenter/) modülünden [Get-partnerusersignactivity](/powershell/module/partnercenter/get-partnerusersigninactivity) cmdlet 'ini kullanmanız gerekir.

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
- [iş ortağı merkezi .net örnekleri](https://github.com/microsoft/partner-center-dotnet-samples): bu GitHub deposu, .net kullanılarak geliştirilen ve güvenli uygulama modeli çerçevesini nasıl uygulayabileceğinizi gösteren örnekler içerir.
- [iş ortağı merkezi java örnekleri](https://github.com/microsoft/partner-center-java-samples): bu GitHub deposu, java kullanılarak geliştirilen ve güvenli uygulama modeli çerçevesini nasıl uygulayabileceğinizi gösteren örnekler içerir.
- [Iş Ortağı Merkezi PowerShell-Multi-Factor Authentication](/powershell/partnercenter/multi-factor-auth): bu Multi-Factor Authentication makale, PowerShell kullanarak güvenli uygulama modeli çerçevesinin nasıl uygulanacağı hakkında ayrıntılı bilgi sağlar.

## <a name="next-steps"></a>Sonraki adımlar

- [İş ortağı kiracınız için Mandating Multi-Factor Authentication (MFA)](partner-security-requirements-mandating-mfa.md)