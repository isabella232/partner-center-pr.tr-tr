---
title: İş ortağı güvenlik gereksinimleri SSS
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: İş ortağı güvenlik gereksinimleri hakkında sık sorulan sorular-ne olduğu, iş ortaklarının bunları nasıl uygulaması gerektiği ve bunları karşıladığınızı öğrenin.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f2bf6823fdd976632fb8ad9c8f11ce99835d76a5
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/31/2021
ms.locfileid: "106087085"
---
# <a name="common-questions-about-partner-security-requirements"></a>İş ortağı güvenlik gereksinimleriyle ilgili sık sorulan sorular

**Uygun roller**

- Tüm Iş Ortağı Merkezi kullanıcıları

Bu makalede, [iş ortağı güvenlik gereksinimleriyle](partner-security-requirements.md)ilgili bazı yaygın sorular yanıtlanmaktadır.

### <a name="what-are-the-partner-security-requirements-and-why-should-partners-implement-them"></a>İş ortağı güvenlik gereksinimleri nelerdir ve iş ortaklarının bunları neden uygulamalıdır?

Daha büyük ve sürekli güvenlik ve gizlilik korumaları, popüler önceliklerimiz arasında olduğundan iş ortaklarının müşterileri ve kiracılarını korumalarına yardımcı olmaya devam ediyoruz. Birincil olarak kimlik güvenliği çözme olayları ile ilgili daha gelişmiş, artan güvenlik saldırılarına karşı daha fazla bilgi görmeye devam ediyoruz. Engelleyici denetimler, güvenlik saldırılarına karşı genel savunma stratejisinde önemli bir rol oynadığında, 2019 ' de [zorunlu güvenlik gereksinimleri](partner-security-requirements.md) sunuyoruz. Bulut çözümü sağlayıcısı (CSP) programına, Denetim Masası satıcılarına ve danışmanlarına katılan tüm iş ortakları uyumlu kalmak için gereksinimleri gerçekleştirmelidir.

### <a name="what-are-the-key-timelines-and-milestones"></a>Anahtar zaman çizelgeleri ve kilometre taşları nelerdir?

Zaman çizelgeleri ve kilometre taşları dahil olmak üzere bu güvenlik gereksinimleriyle ilişkili koşullar, [Microsoft Iş ortağı sözleşmesi](microsoft-partner-agreement.md)'ne dahildir. CSP programına katılımınız ile uyumlu kalmak için, bu güvenlik gereksinimlerini en kısa sürede uygulamanız gerekir.

### <a name="what-will-happen-if-i-dont-implement-these-partner-security-requirements"></a>Bu iş ortağı güvenlik gereksinimlerini uygulamadığımda ne olur?

Microsoft Iş ortağı sözleşmesi, Kullanıcı hesapları için Multi-Factor Authentication 'ı zorunlu hale getirmek ve Iş Ortağı Merkezi API 'siyle etkileşim kurmak için güvenli uygulama modelini benimsemenizi gerektirir. 

Bu güvenlik uygulamalarında olmayan iş ortakları, CSP programını Transact veya temsilci yönetici hakları kullanarak müşteri kiracılarını yönetme olanağını kaybedebilir.

### <a name="do-the-security-requirements-apply-to-all-geographies"></a>Güvenlik gereksinimleri tüm coğrafi lıklar için geçerlidir mi?

Evet, güvenlik gereksinimleri tüm coğrafi lıklar için geçerlidir. Bir sogeign bulutu (ABD devlet ve Almanya) üzerinden deneyimidir tüm iş ortaklarının bu yeni güvenlik gereksinimlerini hemen benimsemesini ve benimsemesini önemle öneririz. Ancak, bu iş ortakları Şu anda güvenlik gereksinimlerini karşılamak için gerekli değildir. Microsoft, daha sonra da bu güvenlik gereksinimlerinin zorlanmasıyla ilgili ek ayrıntılar sağlar.

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>Bir hesap için dışlama almak mümkün midir?

Hayır, çok faktörlü kimlik doğrulamasının (MFA) zorlanmasına sahip olma gereksiniminden herhangi bir kullanıcı hesabını dışlamak mümkün değildir. İş ortağı olmak üzere yüksek ayrıcalıklı bir doğası verildiğinde, Microsoft Iş ortağı sözleşmesi, iş ortağı kiracınızdaki her bir kullanıcı hesabı için Multi-Factor Authentication 'ın uygulanmasını gerektirir.

### <a name="how-do-i-know-if-i-have-met-the-partner-security-requirements"></a>Nasıl yaparım? iş ortağı güvenlik gereksinimlerini karşıladığım hakkında bilgi sahibi misiniz?

Aşağıdaki adımları tamamlayın:

- [İş ortağı güvenlik gereksinimlerinde](partner-security-requirements.md)özetlenen tüm gereksinimleri karşılamanız gerekir.
- İş ortağı kiracınızdaki tüm Kullanıcı hesaplarının Multi-Factor Authentication 'ı zordığından emin olmanız gerekir.

Eylem gerçekleştirebileceğiniz önemli alanların tanımlanmasına yardımcı olmak için Iş Ortağı Merkezi aracılığıyla kullanılabilen [güvenlik gereksinimleri durum raporunu](https://partner.microsoft.com/commerce/security/compliance) sunuyoruz.

Durum raporu hakkında daha fazla bilgi için bkz. [iş ortağı güvenlik gereksinimleri durumu](partner-security-compliance.md).

## <a name="required-actions"></a>Gerekli eylemler

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>Gereksinimleri karşılamak için yapmam gereken önemli eylemler nelerdir?

CSP programındaki tüm iş ortakları (doğrudan fatura, dolaylı sağlayıcı ve dolaylı satıcı), danışmanların ve Denetim Masası satıcılarının gereksinimleri karşılaması gerekir.

1. **Tüm kullanıcılar için MFA 'yı zorla**

    CSP programındaki tüm iş ortakları, danışmanları ve Denetim Masası satıcıları, iş ortağı kiracısındaki tüm kullanıcılar için MFA 'yı zorlamak için gereklidir.

    Ek hususlar:

    - Dolaylı sağlayıcıların, Iş Ortağı Merkezi 'ne eklemek için dolaylı satıcılarla birlikte çalışması gerekir ve satıcıları gereksinimleri karşılayacak şekilde teşvik eder.
    - Azure MFA, Azure AD güvenlik Varsayılanları aracılığıyla iş ortağı kiracısındaki tüm kullanıcılar için, zamana bağlı bir kerelik parolaları (TOTP) destekleyen bir kimlik doğrulayıcı uygulamasının tek doğrulama yöntemiyle kullanılabilir hale getirilir.
    - Telefon araması veya kısa mesaj gibi başka yöntemler gerekliyse [Azure Active Directory Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium) SKU 'ları aracılığıyla ek doğrulama yöntemleri kullanılabilir.
    - İş ortakları, Microsoft ticari bulut hizmetlerine erişirken her hesap için bir üçüncü taraf MFA çözümü de kullanabilir.

2. **Güvenli uygulama modeli çerçevesini benimseyin**

    Herhangi bir API (Azure Resource Manager, Microsoft Graph, Iş Ortağı Merkezi API, vb.) kullanarak özel tümleştirme geliştiren tüm iş ortaklarının veya PowerShell gibi araçlar kullanılarak özel otomasyon uygulayan, Microsoft bulut hizmetleriyle tümleştirmek için [güvenli uygulama modeli çerçevesini](/partner-center/develop/enable-secure-app-model) benimsemeleri gerekir. Bunun yapılmaması, MFA dağıtımı nedeniyle kesintiye neden olabilir. Aşağıdaki kaynaklar, modelin nasıl benimseneceği hakkında bir genel bakış ve kılavuz sağlar.

    - [Güvenli uygulama modeline genel bakış](/partner-center/develop/enable-secure-app-model)
    - [İş Ortağı Merkezi: güvenli uygulama modeli Kılavuzu](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [CSP programındaki iş ortakları: güvenli uygulama modelini etkinleştirmek için .NET örnek kodu](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
    - [CSP programındaki iş ortakları: güvenli uygulama modelini etkinleştirmek için Java örnek kodu](/samples/microsoft/partner-center-java-samples/secure-app-model/)
    - [İş ortağı merkezi kimlik doğrulama belgesi](/partner-center/develop/partner-center-authentication)
    - [İş Ortağı Merkezi PowerShell Multi-Factor Authentication (MFA) belgesi](/powershell/partnercenter/multi-factor-auth)

    Güvenli uygulama modeli çerçevesinin benimsenmesiyle ilgili bir denetim masası kullanıyorsanız, satıcıya başvurun.

    Denetim Masası satıcıları, Iş Ortağı Merkezi 'ne Denetim Masası satıcısı olarak eklemek ve bu gereksinimi hemen uygulamaya [başlamak için gereklidir](enroll-as-cpv.md) . [Iş Ortağı Merkezi: güvenli uygulama modeli çerçevesi](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)' ne bakın. Denetim Masası satıcıları kimlik bilgileri yerine CSP iş ortaklarının onayını kabul edip Yönetmeli ve tüm mevcut CSP iş ortaklarının kimlik bilgilerini temizlemelidir.

## <a name="multi-factor-authentication"></a>Multi-factor authentication

### <a name="what-is-multi-factor-authentication-mfa"></a>Multi-Factor Authentication (MFA) nedir?

MFA, birden fazla gerekli güvenlik ve doğrulama yordamıyla kişilerin kimliğini doğrulamak için bir güvenlik mekanizmasıdır. Aşağıdaki kimlik doğrulama yöntemlerinin iki veya daha fazlasını gerektirerek işe yarar:

- Bildiğiniz bir şey (genellikle bir parola)
- Sahip olduğunuz bir şey (telefon gibi kolayca çoğaltılmayan güvenilir bir cihaz)
- Bir şeyler (Biyometri)

### <a name="what-is-the-cost-of-enabling-mfa"></a>MFA 'yı etkinleştirme maliyeti nedir?

Microsoft, Azure AD güvenlik Varsayılanları 'nın uygulanması aracılığıyla MFA 'yı ücretsiz olarak sağlar. MFA 'nın bu sürümü kullanılarak kullanılabilen tek doğrulama seçeneği bir Authenticator uygulamasıdır. Telefon araması veya SMS mesajı gerekliyse, [Azure Active Directory Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium) lisansın satın alınması gerekir. Alternatif olarak, iş ortağı kiracınızdaki her bir kullanıcı için MFA sağlamak üzere bir üçüncü taraf çözümünü kullanabilirsiniz. Bu durumda, MFA çözümünüzün zorlandığından ve uyumlu olduğunuzdan emin olmak sizin sorumluluğunuzdadır.

### <a name="what-actions-do-i-need-to-take-if-i-already-have-an-mfa-solution"></a>MFA çözümünüz varsa hangi eylemleri gerçekleştirmeniz gerekir?

Bu güvenlik gereksinimlerine göre, bir iş ortağı kiracısındaki kullanıcıların, Microsoft ticari bulut hizmetlerine erişirken MFA kullanarak kimlik doğrulaması yapması gerekir. Üçüncü taraf çözümler, bu gereksinimleri karşılamak için kullanılabilir. Microsoft artık Azure Active Directory uyumluluk için bağımsız kimlik sağlayıcılarına doğrulama testi sağlamaz. Ürününüzü birlikte çalışabilirlik için test etmek üzere bu [yönergelere](https://www.microsoft.com/download/details.aspx?id=56843)bakın.

> [!IMPORTANT]
> Üçüncü taraf bir çözüm kullanırken, çözümün MFA değerini içeren kimlik doğrulama yöntemi başvurusu (AMR) talebini yayınlamasını doğrulamak önemlidir. Üçüncü taraf çözümünüzün beklenen talebi nasıl doğruladığını öğrenmek için bkz. [Iş ortağı güvenlik gereksinimlerini test etme](/powershell/partnercenter/test-partner-security-requirements) .

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>Transact için birden çok iş ortağı kiracıyı kullanıyorum. Bunlara MFA 'yı uygulamam gerekir mi?

Evet, CSP programıyla veya danışman programıyla ilişkilendirilen Azure Active Directory her bir kiracı için MFA 'yı zorunlu kılabilirsiniz. Azure Active Directory Premium Lisansı satın almak için, her bir Azure Active Directory kiracısındaki kullanıcılar için bir Azure Active Directory lisansı satın almanız gerekir. 

### <a name="does-each-user-account-in-my-partner-tenant-need-to-have-mfa-enforced"></a>İş ortağı kiracısındaki her bir kullanıcı hesabının MFA 'nın zorlanmış olması gerekir mi?

Evet, her kullanıcının MFA 'nın zorlanmış olması gerekir. Ancak, Azure AD güvenlik varsayılanlarını kullanıyorsanız, bu özellik tüm Kullanıcı hesapları için MFA uyguladığından, ek bir işlem yapmanız gerekmez. Güvenlik varsayılanlarını etkinleştirmek, Kullanıcı hesaplarınızın MFA ile uyumlu olduğundan ve MFA zorlandığında etkilenmediğinden emin olmanın ücretsiz ve kolay bir yoludur.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Microsoft ile doğrudan bir Bill partner kullanıyorum. Neler yapmam gerekir?

Doğrudan fatura bulut çözümü sağlayıcısı iş ortakları, iş ortağı kiracılarında her kullanıcı için MFA 'yı zorlayamalıdır.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-enable-mfa"></a>Bir dolaylı satıcıyım ve yalnızca bir dağıtıcı Transact. MFA 'yı etkinleştirmeyi hala yapmam gerekir mi?

Tüm dolaylı satıcıların, iş ortağı kiracısındaki her bir kullanıcı için MFA 'yı zorlaması gerekir. Dolaylı satıcı MFA 'yı etkinleştirmelidir.

### <a name="i-dont-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>Iş Ortağı Merkezi API 'sini kullanmıyorum. MFA 'yı yine de uygulamam gerekir mi?

Evet, bu güvenlik gereksinimi, ortak yönetici kullanıcıları ve bir iş ortağı kiracısındaki son kullanıcılar dahil tüm kullanıcılara yöneliktir.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Hangi üçüncü taraf satıcıları Azure Active Directory ile uyumlu MFA çözümleri sağlıyor?

MFA satıcıları ve çözümlerini gözden geçirirken iş ortakları, seçtikleri çözümün Azure Active Directory uyumlu olduğundan emin olmalıdır.

Microsoft artık Azure Active Directory uyumluluk için bağımsız kimlik sağlayıcılarına doğrulama testi sağlamaz. Ürününüzü birlikte çalışabilirlik için test etmek isterseniz, bu [yönergelere](https://www.microsoft.com/download/details.aspx?id=56843)bakın.

Daha fazla bilgi için bkz. [Azure AD Federasyon uyumluluğu listesi](/azure/active-directory/hybrid/how-to-connect-fed-compatibility).

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>Tümleştirme korumalı alanında MFA 'yı nasıl test edebilirim?

Azure AD güvenlik Varsayılanları özelliği etkinleştirilmelidir veya alternatif olarak, Federasyon kullanan bir üçüncü taraf çözümü kullanabilirsiniz.

### <a name="will-enabling-mfa-affect-how-i-interact-with-my-customers-tenant"></a>MFA 'nın, müşterimin kiracısıyla nasıl etkileşime gireceğini etkilemesi gerekir mi?

Hayır. Bu güvenlik gereksinimlerinin yerine getirilmesi, müşterilerinizi nasıl yöneteceğinizi etkilemeyecektir. Temsilcili yönetim işlemlerini gerçekleştirme olanağınız kesintiye uğramaz.

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>Müşterilerimiz iş ortağı güvenlik gereksinimlerine tabidir mi?

Hayır, müşterinizin Azure AD kiracılarındaki her bir kullanıcı için MFA 'yı zorlayabilmeniz gerekli değildir. Ancak, kullanıcılarının ne kadar en iyi şekilde korunacağını öğrenmek için her müşteriyle çalışmanız önerilir.

### <a name="can-any-user-be-excluded-from-the-mfa-requirement"></a>Herhangi bir Kullanıcı, MFA gereksiniminden dışlanamaz mi?

Hayır, iş ortağı kiracınızdaki hizmet hesapları da dahil olmak üzere her kullanıcının MFA kullanarak kimlik doğrulaması yapması gerekecektir.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>İş ortağı güvenlik gereksinimleri tümleştirme korumalı alanı için mi uygulanır?

Evet, iş ortağı güvenlik gereksinimleri tümleştirme korumalı alanı için geçerlidir. Bu, tümleştirme korumalı alanı kiracısındaki kullanıcılar için uygun MFA çözümünü uygulamanız gereken anlamına gelir. MFA sağlamak için Azure AD güvenlik varsayılanlarını uygulamanız önerilir.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Acil bir erişim (kesme camı) hesabı Nasıl yaparım? mi?

Azure AD kiracınızdan yanlışlıkla kilitlenmesini engellemek için bir veya iki acil durum erişim hesabı oluşturmak için en iyi uygulama olarak kabul edilir. İş ortağı güvenlik gereksinimlerine göre, her kullanıcının MFA kullanarak kimlik doğrulaması yapması gerekir. Bu gereksinim, bir acil durum erişim hesabının tanımını değiştirmeniz gereken anlamına gelir. MFA için bir üçüncü taraf çözümü kullanan bir hesap olabilir.

### <a name="is-active-directory-federation-service-adfs-required-if-i-am-using-a-third-party-solution"></a>Üçüncü taraf bir çözüm kullandığım takdirde Active Directory Federasyon Hizmeti (ADFS) gerekiyor mu?

Hayır, üçüncü taraf bir çözüm kullanıyorsanız Active Directory Federasyon Hizmeti (ADFS) olması gerekmez. Çözüm için gereksinimlerin ne olduğunu belirlemek için çözümün satıcısı ile çalışmanız önerilir.

### <a name="is-it-a-requirement-to-enable-azure-ad-security-defaults"></a>Azure AD güvenlik varsayılanlarını etkinleştirmek için bir gereksinim mı var?

Hayır, Azure AD güvenlik varsayılanlarını etkinleştirmeniz gerekli değildir.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>MFA gereksinimini karşılamak için koşullu erişim kullanılabilir mi?

Evet, iş ortağı kiracınızdaki hizmet hesapları da dahil olmak üzere her bir kullanıcı için MFA 'yı zorlamak üzere koşullu erişimi kullanabilirsiniz. Bununla birlikte, her kullanıcının her bir tek kimlik doğrulaması için MFA sınamasına sahip olduğundan emin olmak için, iş ortağı olmak üzere yüksek ayrıcalıklı bir iş ortağı olarak verilmiştir. Bu, MFA gereksinimini atlayabilecek koşullu erişim özelliğini kullanmayamayabilmeniz anlamına gelir.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Azure AD Connect tarafından kullanılan hizmet hesabı iş ortağı güvenlik gereksinimlerinden etkilensin mi?

Hayır, Azure AD Connect tarafından kullanılan hizmet hesabı iş ortağı güvenlik gereksinimlerinden etkilenmeyecektir. MFA zorlama sonucu Azure AD Connect ile ilgili bir sorun yaşıyorsanız, Microsoft desteği ile bir teknik destek isteği açın.

## <a name="secure-application-model"></a>Güvenli uygulama modeli

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>Gereksinimleri karşılamak için güvenli uygulama modelini kimler benimsemelidir?

Microsoft, Multi-Factor Authentication kullanan bulut çözümü sağlayıcısı (CSP) iş ortaklarının ve Denetim Masası satıcılarının (CPV) kimlik doğrulaması için güvenli ve ölçeklenebilir bir çerçeve sunuyor. Daha fazla bilgi için bkz. [güvenli uygulama modeli Kılavuzu](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Herhangi bir API (Azure Resource Manager, Microsoft Graph, Iş Ortağı Merkezi API, vb.) kullanarak özel tümleştirme geliştiren tüm iş ortaklarının veya PowerShell gibi araçlar kullanılarak özel otomasyon uygulayan, Microsoft bulut hizmetleriyle tümleştirmek için [güvenli uygulama modeli çerçevesini](/partner-center/develop/enable-secure-app-model) benimsemeleri gerekir.

### <a name="what-is-the-secure-application-model"></a>Güvenli uygulama modeli nedir?

Microsoft, Multi-Factor Authentication yararlanan bulut çözümü sağlayıcısı (CSP) iş ortaklarının ve Denetim Masası satıcılarının (CPV) kimlik doğrulaması için güvenli ve ölçeklenebilir bir çerçeve sunuyor. Daha fazla bilgi için bkz. [güvenli uygulama modeli Kılavuzu](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) .  

### <a name="how-do-i-implement-the-secure-application-model"></a>Güvenli uygulama modelini uygulama Nasıl yaparım? mı?

Herhangi bir API (Azure Resource Manager, Microsoft Graph, Iş Ortağı Merkezi API, vb.) kullanarak özel tümleştirme geliştiren tüm iş ortaklarının veya PowerShell gibi araçlar kullanılarak özel otomasyon uygulayan, Microsoft bulut hizmetleriyle tümleştirmek için [güvenli uygulama modeli çerçevesini](/partner-center/develop/enable-secure-app-model) benimsemeleri gerekir. Bunun yapılmaması, MFA dağıtımı nedeniyle kesintiye neden olabilir. Aşağıdaki kaynaklar, modelin nasıl benimseneceği hakkında bir genel bakış ve kılavuz sağlar.

- [Güvenli uygulama modeline genel bakış](/partner-center/develop/enable-secure-app-model)
- [İş Ortağı Merkezi: güvenli uygulama modeli Kılavuzu](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [CSP programındaki iş ortakları: güvenli uygulama modelini etkinleştirmek için .NET örnek kodu](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [CSP programındaki iş ortakları: güvenli uygulama modelini etkinleştirmek için Java örnek kodu](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [İş ortağı merkezi kimlik doğrulama belgesi](/partner-center/develop/partner-center-authentication)
- [İş Ortağı Merkezi PowerShell Multi-Factor Authentication (MFA) belgesi](/powershell/partnercenter/multi-factor-auth)

Bir denetim masası kullanıyorsanız, güvenli uygulama modeli çerçevesinin benimsenmesiyle ilgili olarak satıcıya danışmanız gerekir.

Denetim Masası satıcıları, Iş Ortağı Merkezi 'ne Denetim Masası satıcısı olarak eklemek ve bu gereksinimi hemen uygulamaya [başlamak için gereklidir](enroll-as-cpv.md) . [Iş Ortağı Merkezi: güvenli uygulama modeli çerçevesi](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)' ne bakın. Denetim Masası satıcıları kimlik bilgileri yerine CSP iş ortaklarının onayını kabul edip Yönetmeli ve tüm mevcut CSP iş ortaklarının kimlik bilgilerini temizlemelidir.

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>Güvenli uygulama modelinin yalnızca Iş Ortağı Merkezi API/SDK için uygulanması gerekiyor mu?

Tüm Kullanıcı hesaplarında Multi-Factor Authentication 'ı zorunlu tutarak, etkileşimli olmayan bir şekilde çalışmak için tasarlanan tüm otomasyon veya tümleştirme etkilenecektir. İş ortağı güvenlik gereksinimleri, Iş Ortağı Merkezi API 'SI için güvenli uygulama modelini etkinleştirmenizi gerektirdiğinden, otomasyon ve tümleştirmeyle ikinci bir kimlik doğrulama gereksinimini karşılamak için kullanılabilir.

>[!Note] 
>Erişilmekte olan kaynakların belirteç tabanlı kimlik doğrulamasına erişimi desteklemesi gerekir.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>PowerShell gibi Otomasyon araçlarını kullanıyorum. Güvenli uygulama modelini uygulama Nasıl yaparım? mı?

Otomasyonunun etkileşimli olmayan şekilde çalıştırılması amaçlanıyorsa ve kimlik doğrulaması için Kullanıcı kimlik bilgilerini temel alıyorsa güvenli uygulama modelini uygulamanız gerekir. Bkz. [güvenli uygulama modeli | ](/powershell/partnercenter/multi-factor-auth) Bu çerçevenin nasıl uygulanacağını gösteren yönergeler için iş ortağı merkezi PowerShell.  

>[!Note] 
>Tüm otomasyon araçları, erişim belirteçlerini kullanarak kimlik doğrulaması yapma olanağı sağlamaz. Hangi değişikliklerin yapılması gerektiğini anlamak için yardıma ihtiyacınız varsa [Iş Ortağı Merkezi Güvenlik Kılavuzu](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) grubuna bir ileti gönderin. 

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>Uygulama Yöneticisi, onay işlemini gerçekleştirirken hangi kullanıcı kimlik bilgilerini sağlamalıdır?

En az ayrıcalıklı izinlere atanmış bir hizmet hesabı kullanmanız önerilir. Iş Ortağı Merkezi API 'sine göre, Sales Agent veya admin Agents rolüne atanmış bir hesabı kullanmanız gerekir.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>Uygulama Yöneticisi neden onay işlemini gerçekleştirirken genel yönetici kullanıcı kimlik bilgilerini sağlamamalıdır?

En az ayrıcalıklı kimlik kullanmak en iyi uygulamadır.  Bu, riski azaltır. Bu, gerekenden daha fazla izin sağlayacağından, genel yönetici ayrıcalıklarına sahip bir hesap kullanılması önerilmez.

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>Bir CSP iş ortağıyım. Nasıl yaparım? Denetim Masası satıcımın (CPV) çözümü uygulamaya çalışıp çalışmadığını bilir mi?

Bulut çözümü sağlayıcısı (CSP) programında Transact 'ya bir denetim masası satıcısı (CPV) çözümü kullanan iş ortakları için, CPV 'nize danışmanız sizin sorumluluğunuzdadır.

### <a name="who-is-a-control-panel-vendor-cpv"></a>Denetim Masası satıcısı (CPV) kim?

Denetim Masası satıcısı, CSP Iş ortakları tarafından Iş Ortağı Merkezi API 'Leri ile tümleştirme için kullanılacak uygulamaları geliştiren bağımsız bir yazılım satıcıdır. Bir denetim masası satıcısı, Iş Ortağı Merkezi panosuna veya API 'Lerine doğrudan erişimli bir CSP Iş ortağı değildir. Iş Ortağı Merkezi 'nde ayrıntılı bir açıklama mevcuttur [: güvenli uygulamalar model Kılavuzu](https://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="i-am-a-cpv-how-do-i-enroll"></a>Bir CPV kullanıyorum. Nasıl yaparım? kaydetmek istiyor musunuz?

Bir denetim masası satıcısı (CPV) olarak kaydetmek için, [burada](enroll-as-cpv.md)belirtilen yönergeleri izleyin.

CPVs, [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) kayıt bağlantısını almak ve CPV ile iş ilişkisine sahip olan veya işletmelerini bilen bir Microsoft çalışanı sponsori sağlamak için başvurmalıdır. Örneğin, bir Iş ortağı Geliştirme Yöneticisi (PDM).

Iş Ortağı Merkezi 'ne kaydolduktan ve uygulamalarınızı kaydettikten sonra, Iş Ortağı Merkezi API 'Lerine erişebilirsiniz. Yeni bir CPV kullanıyorsanız, bir Iş Ortağı Merkezi bildirimi aracılığıyla korumalı alan bilgilerinizi alacaksınız. Kayıt işlemini Microsoft CPV olarak tamamladıktan sonra CPV sözleşmesini kabul etmiş olursunuz, şunları yapabilirsiniz:

1. Çok kiracılı uygulamayı yönetin (Azure portal uygulamalar ekleyin ve Iş Ortağı Merkezi 'nde uygulamaları kaydedin ve kaydını kaldırın).

   >[!Note]
   >Iş Ortağı Merkezi API 'Lerine yetki almak için, CPVs 'nin uygulamalarını Iş Ortağı Merkezi 'ne kaydetmesi gerekir. Uygulamaları tek başına Azure portal eklemek, Iş Ortağı Merkezi API 'Leri için CPV uygulamalarına yetki vermez.

1. CPV profilinizi görüntüleyin ve yönetin.

1. CPV özelliklerine erişmesi gereken kullanıcılarınızı görüntüleyin ve yönetin. Bir CPV yalnızca genel yönetici rolüne sahip olabilir.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>Iş Ortağı Merkezi SDK 'sını kullanıyorum. SDK, güvenli uygulama modelini otomatik olarak benimsesin mi?

Hayır, [güvenli uygulama modeli kılavuzunda](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)belirtilen yönergeleri izlemeniz gerekir.

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-dont-have-mfa-enabled"></a>MFA 'nın etkin olmadığı hesaplara sahip güvenli uygulama modeli için yenileme belirteci oluşturabilir miyim?

Evet, bir yenileme belirteci MFA Zorlanmış olmayan bir hesap kullanılarak oluşturulabilir. Ancak, bu kaçınılmalıdır. MFA 'nın etkin olmadığı bir hesap kullanılarak oluşturulan herhangi bir belirteç, MFA gereksinimi nedeniyle kaynaklara erişemeyecektir.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>MFA 'yı etkinleştireceğim uygulamamın erişim belirtecini nasıl alması gerekir?

Yeni güvenlik gereksinimleriyle uyumlu hale getirmek için nasıl yapılacağı hakkında ayrıntılı bilgi sağlayan [güvenli uygulama modeli kılavuzunu](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) izlemeniz gerekir. [Burada .NET örnek kodunu ve Java](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) örnek kodunu [burada](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)bulabilirsiniz.

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>Bir CPV olarak, CPV kiracımızda veya CSP iş ortağının kiracısında bir Azure AD uygulaması oluştururum mı?

CPV 'nin, kendi kaydıyla ilişkili kiracıda bir CPV olarak Azure Active Directory uygulamayı oluşturması gerekir.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>Yalnızca uygulama kimlik doğrulaması kullanan bir CSP kullanıyorum. Herhangi bir değişiklik yapmam gerekiyor mu?

Erişim belirteci istemek için Kullanıcı kimlik bilgileri kullanılmadığından yalnızca uygulama kimlik doğrulaması etkilenmez. Kullanıcı kimlik bilgileri paylaşılmışsa, Denetim Masası satıcıları (CPVs) [güvenli uygulama modeli çerçevesini](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) benimsemeli ve sahip oldukları tüm mevcut iş ortağı kimlik bilgilerini temizlemelidir.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>Bir CPV olarak erişim belirteçlerini almak için yalnızca uygulama kimlik doğrulama stilinden yararlanabilir miyim?

Hayır, Denetim Masası satıcı iş ortakları, iş ortağı adına erişim belirteçleri istemek için yalnızca uygulama kimlik doğrulama stilini kullanamaz. Uygulama + kullanıcı kimlik doğrulama stiliyle yararlanan güvenli uygulama modelini uygulamalıdır.

## <a name="technical-enforcement"></a>Teknik uygulama

### <a name="what-is-the-activation-of-security-safeguards"></a>Güvenlik korumalarının etkinleştirilmesi nedir?

Bulut çözümü sağlayıcısı (CSP) programına, Denetim Masası satıcılarına (CPVs) ve danışmanlarına katılan tüm iş ortakları, uyumlu kalmak için zorunlu güvenlik gereksinimlerini uygulamalıdır.

Microsoft, ek koruma sağlamak için, iş ortaklarının kiracılarının ve müşterilerinin, yetkisiz erişimi engellemek için Mandating Multi-Factor Authentication (MFA) doğrulamasına erişmesini sağlayan güvenlik önlemlerinin etkinleştirilmesini başlamıştır.  

Şirket adına yönetici (AOBO) özellikleri için etkinleştirmeyi tüm iş ortağı kiracılarına başarıyla tamamladınız. S2 CY2020 'i hedefleyen iş ortakları ve müşterilerin korunmasına daha fazla yardımcı olmak için, iş ortaklarının Iş ve müşterilerinin kimlik hırsızlığına ilişkin olayları korumalarına yardımcı olması için CSP 'de Iş Ortağı Merkezi işlemlerine yönelik etkinleştirmeye başlayacağız.

Daha fazla bilgi için, [iş ortağı kiracı sayfanız Için Mandating Multi-Factor Authentication (MFA)](partner-security-requirements-mandating-mfa.md) makalesini ziyaret edin.

### <a name="i-am-using-a-third-party-mfa-solution-and-i-am-being-blocked-what-should-i-do"></a>Üçüncü taraf MFA çözümünü kullanıyorum ve engellendim, ne yapmam gerekir?

Kaynaklara erişen hesabın çok faktörlü kimlik doğrulamasına yönelik olduğunu doğrulamak için, MFA 'nın listelenip listelenmediğini görmek üzere [kimlik doğrulama yöntemi başvuru](https://tools.ietf.org/html/rfc8176) talebini denetliyoruz. Bazı üçüncü taraf çözümleri bu talebi vermez veya MFA değeri içermez. Talep eksikse veya MFA değeri listelenmiyorsa, kimliği doğrulanmış hesabın Multi-Factor Authentication için talep olup olmadığını belirlemenin bir yolu yoktur. Çözümün kimlik doğrulama yöntemi başvuru talebini vermesi için hangi eylemlerin alınması gerektiğini belirlemek üzere üçüncü taraf çözümünüz için satıcıyla çalışmanız gerekir.

Üçüncü taraf çözümünüzün beklenen talebi mi yayınlayacağına emin değilseniz [, Iş ortağı güvenlik gereksinimlerini test](/powershell/partnercenter/test-partner-security-requirements) edin bölümüne bakın.

### <a name="mfa-is-blocking-me-from-supporting-my-customer-using-aobo-what-should-i-do"></a>MFA, AOIMIN Kullanıcı tarafından desteklenmem, ne yapmam gerekir?

Kimliği doğrulanmış hesap çok faktörlü kimlik doğrulaması için gerekişse, iş ortağı güvenlik gereksinimleri için teknik zorlama denetlenir. Hesap yoksa, oturum açma sayfasına yönlendirilirsiniz ve yeniden kimlik doğrulaması istenir. [İş ortağı kiracı belgeleriniz için bu Mandating Multi-Factor Authentication (MFA) ile ilgili](partner-security-requirements-mandating-mfa.md#partner-delegated-administration) ek deneyimi ve kılavuzları okuyun. Etki alanı Federal olmayan senaryoda, başarıyla kimlik doğrulamasından geçtikten sonra Multi-Factor Authentication 'ı ayarlamanız istenecektir. Bu işlemi tamamladıktan sonra, AOINI kullanarak müşterilerinizi yönetebilirsiniz. Etki alanının federe olduğu senaryoda, hesabın Multi-Factor Authentication için gerekmekte olduğundan emin olmanız gerekir.

## <a name="security-defaults-transition"></a>Güvenlik Varsayılanları geçişi

### <a name="how-can-i-transition-from-baseline-policies-to-security-defaults-or-other-mfa-solutions"></a>Temel ilkelerden, güvenlik varsayılanlarına veya diğer MFA çözümlerine nasıl geçiş yapabilirim?

Azure Active Directory (Azure AD) ["taban çizgisi" ilkeleri kaldırılıyor ve](/azure/active-directory/fundamentals/whats-new#replacement-of-baseline-policies-with-security-defaults) siz ve müşterileriniz için daha kapsamlı bir koruma ilkeleri kümesi olan "güvenlik Varsayılanları" ile değiştiriliyor. [Güvenlik Varsayılanları](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) , kuruluşunuzun kimlik hırsızlığı ile ilgili güvenlik saldırılarına karşı korunmasına yardımcı olabilir.

Çok faktörlü kimlik doğrulaması (MFA) uygulamanız, temel ilkelerden güvenlik Varsayılanları ilkesine veya [DIĞER MFA uygulama seçeneklerine](partner-security-requirements.md#implementing-multi-factor-authentication)geçiş yapmadığınız takdirde, ana hat ilkeleri kullanımdan kaldırılmasının nedeniyle kaldırılır. İş ortağı Kiracılarınızın MFA korumalı işlemleri gerçekleştirdiği tüm kullanıcılara MFA doğrulamasının tamamlanabilmesi istenecektir. Daha ayrıntılı Kılavuzu [burada](partner-security-requirements-mandating-mfa.md)gözden geçirin.
Uyumlu kalmak ve kesintilerini en aza indirmek için aşağıdaki eylemlerden birini gerçekleştirin:

- Güvenlik varsayılanlarına geçiş
    - Güvenlik Varsayılanları ilkesi, iş ortaklarının MFA uygulamak için seçebileceğine ilişkin seçeneklerden biridir. Ek bir ücret ödemeden temel düzeyde güvenlik özelliği sunar.
    - Azure AD ile kuruluşunuz için MFA 'yı etkinleştirme hakkında bilgi edinin ve [güvenlik Varsayılanları temel konularını](partner-security-requirements.md#security-defaults)gözden geçirin.
    - İş gereksinimlerinizi karşılıyorsa güvenlik Varsayılanları ilkesini etkinleştirin.
- Koşullu erişime geçiş
    - Güvenlik Varsayılanları ilkesi gereksinimlerinize uygun değilse, koşullu erişimi etkinleştirin. Daha fazla bilgi için Azure AD koşullu erişim belgelerini gözden geçirin.

## <a name="key-resources"></a>Ana kaynaklar

### <a name="how-to-get-started"></a>Nasıl kullanmaya başlarım

- [Iş ortağı güvenlik gereksinimleri: adım adım kılavuz](partner-security-requirements.md).
- Sorularınızı ve geri bildiriminizi bu [Iş Ortağı Merkezi Güvenlik Kılavuzu grubuna](https://aka.ms/MPCSecurityGuidance)yönlendirin.
- Gelecek iş ortağı ofis saatlerine ve web seminerine katılın. [Ayrıntılı zamanlamayı ve kaynakları buradan](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)denetleyin.

### <a name="resources-for-adopting-secure-application-model"></a>Güvenli uygulama modeli benimseme kaynakları

- [Güvenli uygulama modeline genel bakış](/partner-center/develop/enable-secure-app-model)
- [İş Ortağı Merkezi: güvenli uygulama modeli Kılavuzu](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [CSP programındaki iş ortakları: güvenli uygulama modelini etkinleştirmek için .NET örnek kodu](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [CSP programındaki iş ortakları: güvenli uygulama modelini etkinleştirmek için Java örnek kodu](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [İş ortağı merkezi kimlik doğrulama belgesi](/partner-center/develop/partner-center-authentication)
- [İş Ortağı Merkezi PowerShell Multi-Factor Authentication (MFA) belgesi](/powershell/partnercenter/multi-factor-auth)

## <a name="support"></a>Destek

### <a name="where-can-i-get-support"></a>Nereden destek alabilirim?

Güvenlik gereksinimlerini karşılayacak destek kaynakları için, Iş ortakları için gelişmiş destek (ASfP) hizmet hesabı yöneticinize başvurun; Iş ortakları sözleşmesi için Premier Destek (PSfP) için hizmet hesabı yöneticinize ve teknik hesap yöneticinize başvurun.

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>Güvenli uygulama modeli çerçevesini benimsememe yardımcı olacak teknik bilgi ve Destek Nasıl yaparım?.

Azure Active Directory için teknik ürün desteği seçenekleri MPN avantajlarınız aracılığıyla kullanılabilir. Etkin bir ASfP veya PSfP aboneliğine erişimi olan iş ortakları, kendilerine sunulan seçenekleri en iyi şekilde anlayabilmek için ilişkili hesap yöneticisi (SAM/TAM) ile çalışabilir.

### <a name="how-do-i-contact-support-if-ive-lost-access-to-partner-center"></a>Iş Ortağı Merkezi 'ne erişimi kaybetdiğimde Nasıl yaparım? desteğe başvurun mi?

Bir MFA sorunu nedeniyle erişimi kaybederseniz, kiracınız için genel yöneticiye başvurun. Dahili BT departmanınız, genel yöneticinizin kim olduğunu söyleyebilir. 

Parolanızı unuttuysanız yardım için [oturum açılamıyor](unable-to-sign-in.md) bölümünü okuyun.

### <a name="where-can-i-find-more-information-about-common-technical-issues"></a>Yaygın teknik sorunlar hakkında daha fazla bilgiyi nerede bulabilirim?

Ortak teknik sorunlarla ilgili bilgiler, iş ortağı [merkezi veya Iş Ortağı Merkezi API 'leri kullanan iş ortakları Için Iş ortağı güvenlik gereksinimlerinde](partner-security-requirements.md) bulunabilir