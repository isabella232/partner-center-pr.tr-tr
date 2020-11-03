---
title: İş ortağı güvenlik gereksinimleri
ms.topic: article
ms.date: 10/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Multi-Factor Authentication 'ı (MFA) etkinleştirmek ve güvenli uygulama modeli çerçevesini benimsemek için iş ortağı gereksinimlerini tanıtır.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 361a36adf40af67769a9a24ba1c485f2ad95b98c
ms.sourcegitcommit: 8a4a3de728532533276a88b1fd40c82b7a4ebb15
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/06/2020
ms.locfileid: "92531831"
---
# <a name="partner-security-requirements-for-partners-using-partner-center-or-partner-center-apis"></a>Ortak Merkezi veya Iş Ortağı Merkezi API 'Leri kullanan iş ortakları için iş ortağı güvenlik gereksinimleri

**Uygulama hedefi**

- Bulut çözümü sağlayıcısı programındaki tüm iş ortakları
  - Doğrudan fatura
  - Dolaylı sağlayıcı
  - Dolaylı satıcı
- Tüm Denetim Masası satıcıları
- Tüm danışmanları

**Uygun kullanıcılar**

- Konuk kullanıcılar dahil tüm etkin kullanıcılar

Büyük gizlilik korumaları ve güvenlik, en iyi önceliklerimiz arasındadır. En iyi savunması önleme olduğunu ve yalnızca zayıf bağlantımız kadar güçlü olduğunu biliyoruz. Bu nedenle, ekosistemimizde herkesin işlem yapması ve uygun güvenlik korumalarının yerinde olduğundan emin olunması gerekir. İş ortaklarının ve müşterilerin korunmasına yardımcı olmak için, danışmanları, Denetim Masası satıcıları ve bulut çözümü sağlayıcısı programına katılan iş ortakları için bir dizi zorunlu güvenlik gereksinimi sunuyoruz.

## <a name="overview"></a>Genel Bakış

İş ortakları, iş ortağı kiracısındaki tüm Kullanıcı hesaplarında Multi-Factor Authentication 'ı zorlamak için gereklidir. İş ortağı güvenlik gereksinimleriyle ilişkili şartlar Microsoft Iş ortağı Sözleşmesi ' ne eklenmiştir. Danışmanlarıyla ilgili olarak, sözleşmeli gereksinimlerin de aynı olması gerekir.

Zorunlu güvenlik gereksinimlerini uygulamayan iş ortakları, bu gereksinimler zorlandıktan sonra bulut çözümü sağlayıcısı programında Transact veya yönetici haklarıyla Kullanıcı kiracılarını yönetemez. Ayrıca, güvenlik gereksinimlerini uygulamayan iş ortakları, risk altındaki programlara katılımını uygulayabilir.  

Sizi ve müşterilerinizi korumak için iş ortaklarının aşağıdaki eylemleri hemen ele geçirmesine gerek duyuluyoruz:  

1. **İş ortağı kiracınızdaki tüm Kullanıcı hesapları için Multi-Factor Authentication (MFA) özelliğini etkinleştirin** . İş ortağı kiraclarınızdaki tüm Kullanıcı hesaplarının, Microsoft ticari bulut hizmetlerinde oturum açtıklarında veya Iş Ortağı Merkezi aracılığıyla veya API 'Ler aracılığıyla bulut çözümü sağlayıcısı programı ile Transact, çok faktörlü kimlik doğrulaması (MFA) tarafından geçmesi gerekir.

2. **Güvenli uygulama modeli çerçevesini benimseyin** . Güvenli uygulama modeli çerçevesini benimseyin. Iş Ortağı Merkezi API 'siyle Tümleştirdiğiniz tüm iş ortakları, tüm App + kullanıcı kimlik doğrulama modeli uygulamaları için güvenli uygulama modeli çerçevesini benimsemelidir.

    > [!IMPORTANT]
    > Bu iş ortaklarının, MFA zorlandığında herhangi bir kesinti yaşamamak için Azure Resource Manager, Microsoft Graph veya PowerShell gibi Kullanıcı kimlik bilgilerini kullanarak bir Microsoft API 'SI ile tümleştirme için güvenli uygulama modeli uygulamasını kesinlikle öneririz.

Multi-Factor Authentication (MFA) ve güvenli uygulama modeli çerçevesini benimseme olanağı, altyapınızı korumanıza ve müşterinin verilerini hırsızlık veya diğer sahtekarlık olaylarını belirlemek gibi olası güvenlik risklerine karşı korumanıza yardımcı olur.  

## <a name="actions-that-you-need-to-take"></a>Gerçekleştirmeniz gereken eylemler

İş ortağı güvenlik gereksinimleriyle uyumlu olması için, iş ortağı kiracınızdaki her kullanıcı hesabı için Multi-Factor Authentication 'ı zorunlu kılabilirsiniz. Bunu aşağıdaki yollardan birini yapabilirsiniz:

- [Azure AD güvenlik varsayılanlarını](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)uygulama.

- Her Kullanıcı hesabı için Azure Active Directory Premium satın alma. Daha fazla bilgi için bkz. [bulut tabanlı Azure Multi-Factor Authentication dağıtımı planlama](/azure/active-directory/authentication/howto-mfa-getstarted).

- İş ortağı kiracınızdaki her kullanıcı hesabı için Multi-Factor Authentication 'ı zorlamak üzere bir üçüncü taraf çözümü kullanma. Çözümün beklenen çözümü sağlayacağız emin olmak için, bkz. [güvenlik gereksinimlerinin nasıl zorlanacağını](#how-the-requirements-will-be-enforced).

> [!NOTE]
> Bir sogeign bulutu (21Vianet, ABD kamu ve Almanya) için çok faktörlü kimlik doğrulaması sözleşmeye dayalı olmasa da bu güvenlik gereksinimlerini benimsemeniz önemle önerilir.

## <a name="security-defaults"></a>Güvenlik varsayılanları

Güvenlik Varsayılanları ilkesi, iş gereksinimlerine bağlı olarak iş ortaklarının MFA 'yı güvenlik gereksinimlerine göre uygulamak için seçim yapabileceğiniz [seçeneklerden](#actions-that-you-need-to-take) biridir. Ek bir ücret ödemeden temel düzeyde güvenlik özelliği sunar. Azure AD ile kuruluşunuz için MFA 'yı etkinleştirme ve güvenlik varsayılanlarını etkinleştirmeden önce aşağıdaki önemli noktalar hakkında gözden geçirin.

- Ana hat ilkeleri sonraki birkaç ayda kalır ve Şubat 2020 ' nin sonunda kullanım dışı bırakılır.

- Temel ilkelerini benimseyen iş ortaklarının, güvenlik varsayılanlarına geçiş yapmak için işlem yapması gerekir.

- Güvenlik Varsayılanları, önizleme temeli ilkelerinin genel kullanıma sunulduğuna yönelik olarak değişiklik yapar. Bir iş ortağı güvenlik varsayılanlarını etkinleştirdikten sonra, artık temel ilkeleri etkinleştiremeyecektir.

- Güvenlik varsayılanları ile tüm ilkeler aynı anda etkin olur.

- [Koşullu erişim](/azure/active-directory/conditional-access/concept-conditional-access-policy-common)kullanan iş ortakları için [güvenlik Varsayılanları kullanılabilir](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults)olmayacaktır.

- Şu anda iş ortakları için eski kimlik doğrulamasını engelleme zorlanmayacak. Ancak, güvenliği aşılmış kimlikler ile ilgili çoğu olay, eski kimlik doğrulaması kullanan oturum açma girişimlerinden karşılaştığından, iş ortaklarının bu eski protokollerden taşınması önerilir.

- Azure AD Connect eşitleme hesabı, güvenlik varsayılanlarından çıkarılır.

- Ayrıntılı bilgi için [Kuruluşunuz için Multi-Factor Authentication etkinleştirme](/azure/active-directory/authentication/concept-mfa-get-started) ve [güvenlik varsayılanlarını Azure Active Directory](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)makalesini okuyun.

> [!NOTE]
> Azure AD güvenlik Varsayılanları, ana hat koruma ilkelerinin basitleşme evidir. Temel koruma ilkelerini zaten etkinleştirdiyseniz, güvenlik varsayılanlarını etkinleştirmeniz önemle önerilir.

Temel ilkelerden güvenlik varsayılanlarına geçiş yapmak için, [güvenlik varsayılanlarını nelerdir?](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)bölümünü okuyun.

### <a name="consideration"></a>Değerlendirme

Bu gereksinimler iş ortağı kiracınızdaki tüm kullanıcı hesaplarına uygulandığından, çok faktörlü kimlik doğrulaması gerçekleştiremediği Azure Active Directory Kullanıcı hesaplarını belirleme ve kuruluşunuz tarafından modern kimlik doğrulamayı desteklemeyen uygulamalar ve cihazlar gibi bir kesintisiz dağıtım sağlamak için birkaç şeyi göz önünde bulundurmanız gerekir.

Herhangi bir işlem gerçekleştirmeden önce aşağıdakileri tanımlamanızı öneririz:

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Modern kimlik doğrulaması kullanımını desteklemeyen bir uygulama veya cihazınız mı var?

Multi-Factor Authentication 'ı zorunlu kılabilirsiniz, çok faktörlü kimlik doğrulamasını desteklemediklerinden, IMAP, POP3, SMTP gibi eski kimlik doğrulama kullanım protokollerini engellenecektir. Bu kısıtlamayı gidermek için uygulama [Parolaları](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) olarak bilinen bir özellik, uygulamanın veya cihazın kimlik doğrulamasının devam ettiğinden emin olmak için kullanılabilir. Ortamınızda kullanılabilecekleri olup olmadıklarını öğrenmek için [burada](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) belgelenen uygulama parolalarını kullanma konularını gözden geçirmeniz gerekir.

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>İş ortağı kiracınızla ilişkili lisanslar tarafından sunulan Office 365 kullanan kullanıcılarınız var mı?

Herhangi bir çözümü uygulamadan önce, iş ortağı kiracınızdaki kullanıcılar tarafından hangi Microsoft Office sürümünün kullanıldığını belirlemenizi öneririz. Kullanıcılarınız Outlook gibi uygulamalarla bağlantı sorunlarıyla karşılaşacaktır. Multi-Factor Authentication 'ı uygulamadan önce, Outlook 2013 SP1, veya sonraki bir sürümünün kullanıldığından ve kuruluşunuzun modern kimlik doğrulamasının etkin olduğundan emin olmak önemlidir. Daha fazla bilgi için bkz. [Exchange Online 'da modern kimlik doğrulamasını etkinleştirme](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online) .

Microsoft Office 2013 yüklü olan Windows çalıştıran tüm cihazlarda modern kimlik doğrulamayı etkinleştirmek için, iki kayıt defteri anahtarı oluşturmanız gerekecektir. Bkz. [Windows cihazlarda Office 2013 Için modern kimlik doğrulamasını etkinleştirme](/office365/admin/security-and-compliance/enable-modern-authentication).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Kullanıcılarınız çalışırken kullanıcılarınızın mobil cihazlarını kullanmasını engellemiş bir ilke var mı?

Çalışan çok faktörlü kimlik doğrulama çözümünü etkilediğinden, çalışanların mobil cihazları kullanmasını engelleyen herhangi bir kurumsal ilkeyi tanımlamak önemlidir. [Azure AD güvenlik Varsayılanları](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)'nın uygulanmasıyla, yalnızca doğrulama için bir Authenticator uygulamasının kullanılmasına izin veren bir çözüm vardır. Kuruluşunuzun mobil cihazların kullanımını engellediği bir ilkesi varsa, aşağıdaki seçeneklerden birini göz önünde bulundurun:

- Güvenli sistemde çalışabilen zamana bağlı bir kerelik ana parola (TOTP) uygulaması dağıtın

- Ortak kiracısındaki her bir kullanıcı hesabı için çok faktörlü kimlik doğrulamasını zorlayan bir üçüncü taraf çözümünü uygulama, en uygun doğrulama seçeneğini sağlar

- Etkilenen kullanıcılar için [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) lisansları satın alın

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>Kimlik doğrulaması için Kullanıcı kimlik bilgileriyle hangi Otomasyon veya tümleştirmeyi kullanıyorsunuz?

Gereksinim, hizmet hesapları da dahil olmak üzere her bir kullanıcı için MFA 'yı zorlayacağı için, iş ortağı dizininizde kimlik doğrulama için Kullanıcı kimlik bilgilerini kullanan tüm otomasyon veya tümleştirme etkilenecektir. Bu nedenle, bu durumlarda hangi hesapların kullanıldığını belirlemeniz önemlidir. Göz önünde bulundurmanız gereken örnek uygulamalar veya Hizmetler listesine bakın:

- Müşterileriniz adına kaynak sağlamak için kullanılan denetim masası

- Faturalandırma için kullanılan platformlarla Tümleştirme (CSP programı ile ilişkili olduğu gibi) ve müşterilerinizi destekleme

- Az, AzureRM, Azure AD, MS Online, vb. modülleri kullanan PowerShell betikleri

Yukarıdaki liste kapsamlı değildir. Bu nedenle, ortamınızda kimlik doğrulaması için Kullanıcı kimlik bilgilerini kullanan herhangi bir uygulamayı veya hizmeti bir bütün olarak değerlendirmenizi öneririz. Multi-Factor Authentication gereksinimini karşılamak için, Kılavuzu mümkün olduğunda [güvenli uygulama modeli çerçevesinde](/partner-center/develop/enable-secure-app-model) uygulamanız gerekir.

## <a name="accessing-your-environment"></a>Ortamınıza erişme

Multi-Factor Authentication için istemeden kimlik doğrulaması yapan ne olduğunu daha iyi anlamak için oturum açma etkinliğini incelemenizi öneririz. Azure Active Directory Premium aracılığıyla, oturum açma raporundan yararlanabilirsiniz. Daha fazla bilgi için [Azure Active Directory portalındaki oturum açma etkinlik raporları '](/azure/active-directory/reports-monitoring/concept-sign-ins) na bakın. Azure Active Directory Premium yoksa veya PowerShell aracılığıyla bunu elde etmek istiyorsanız, [Iş Ortağı Merkezi PowerShell](https://www.powershellgallery.com/packages/PartnerCenter/) modülünden [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity) cmdlet 'ini kullanmanız gerekir.

## <a name="how-the-requirements-will-be-enforced"></a>Gereksinimlerin nasıl zorlanacaktır

İş ortağı güvenlik gereksinimleri, çok faktörlü kimlik doğrulaması doğrulamasının gerçekleştiğine ilişkin MFA talebinin varlığını denetleyerek Azure Active Directory ve Iş Ortağı Merkezi ' nde zorlanır. Microsoft, 18 Kasım 2019 ' den itibaren iş ortağı kiracılarına ek güvenlik korumalarını (daha önce "teknik uygulama" olarak bilinir) etkinleşdirecek. 

Etkinleştirme sonrasında, iş ortağı kiracısındaki kullanıcılar, (AOBO) işlemleri üzerinde herhangi bir yönetici gerçekleştirirken Multi-Factor Authentication (MFA) doğrulamasının tamamlanmasını talep eder. Güvenlik önlemlerinin kapsamını ek senaryolar ve Kullanıcı rollerine genişletmeye devam edeceğiz ve bu iş ortakları, ön bildirim sağlar. Daha fazla bilgi için lütfen bu belgeye başvurun. Bu, sık olarak güncelleştirilecektir. Gereksinimleri karşılamayan iş ortakları, herhangi bir iş kesintilerini önlemek için bu ölçüleri en kısa sürede uygulamalıdır. 

Azure Multi-Factor Authentication veya Azure AD güvenlik varsayılanlarını kullanıyorsanız, uygulamanız gereken başka bir eylem yoktur.

Üçüncü taraf bir Multi-Factor Authentication çözümü kullanırken, MFA talebinin verilmeyebilir bir şansınız vardır. Bu talep eksikse Azure Active Directory, kimlik doğrulama isteğinin Multi-Factor Authentication tarafından mı öncelikli olduğunu belirleyemeyecektir. Çözümünüzün beklenen talebi verme hakkında daha fazla bilgi için, [Iş ortağı güvenlik gereksinimlerini test](/powershell/partnercenter/test-partner-security-requirements)edin. 

> [!IMPORTANT]
> Üçüncü taraf çözümünüz beklenen talebi yayınleyemiyorsa, hangi eylemlerin alınacağını belirlemek için çözümü geliştiren satıcıyla çalışmanız gerekir.

## <a name="resources-and-support"></a>Kaynaklar ve destek

Destek ve örnek kod için aşağıdaki kaynaklara bakın:

- [Iş Ortağı Merkezi Güvenlik Kılavuzu grubu topluluğu](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): Iş Ortağı Merkezi Güvenlik Kılavuzu grubu topluluğu, yaklaşan olaylar hakkında bilgi edinmek ve sahip olabileceğiniz sorularınızı sormak için kullanabileceğiniz bir çevrimiçi toplulukdır.
- [Iş ortağı merkezi .NET örnekleri](https://github.com/microsoft/partner-center-dotnet-samples): Bu GitHub deposu, .NET kullanılarak geliştirilen ve güvenli uygulama modeli çerçevesini nasıl uygulayabileceğinizi gösteren örnekler içerir.
- [Iş ortağı merkezi Java örnekleri](https://github.com/microsoft/partner-center-java-samples): Bu GitHub deposu, Java kullanılarak geliştirilen ve güvenli uygulama modeli çerçevesini nasıl uygulayabileceğinizi gösteren örnekler içerir.
- [Iş Ortağı Merkezi PowerShell-Multi-Factor Authentication](/powershell/partnercenter/multi-factor-auth): bu Multi-Factor Authentication makale, PowerShell kullanarak güvenli uygulama modeli çerçevesinin nasıl uygulanacağı hakkında ayrıntılı bilgi sağlar.