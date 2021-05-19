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
ms.openlocfilehash: 174c56ce9bb5fb3d9d92c1ef18af73479619f4bb
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110145890"
---
# <a name="common-questions-about-partner-security-requirements"></a>İş ortağı güvenlik gereksinimleriyle ilgili sık sorulan sorular

**Uygun roller**: tüm Iş Ortağı Merkezi kullanıcıları

Bu makalede, [iş ortağı güvenlik gereksinimleriyle](partner-security-requirements.md)ilgili bazı yaygın sorular yanıtlanmaktadır.

### <a name="what-are-the-partner-security-requirements-and-why-should-partners-implement-them"></a>İş ortağı güvenlik gereksinimleri nelerdir ve iş ortaklarının bunları neden uygulamalıdır?

Daha büyük ve sürekli güvenlik ve gizlilik korumaları, popüler önceliklerimiz arasında olduğundan iş ortaklarının müşterileri ve kiracılarını korumalarına yardımcı olmaya devam ediyoruz. Birincil olarak kimlik güvenliği çözme olayları ile ilgili daha gelişmiş, artan güvenlik saldırılarına karşı daha fazla bilgi görmeye devam ediyoruz. Engelleyici denetimler, güvenlik saldırılarına karşı genel savunma stratejisinde önemli bir rol oynadığında, 2019 ' de [zorunlu güvenlik gereksinimleri](partner-security-requirements.md) sunuyoruz. Bulut çözümü sağlayıcısı (CSP) programına, Denetim Masası satıcılarına ve danışmanlarına katılan tüm iş ortakları uyumlu kalmak için gereksinimleri gerçekleştirmelidir.

### <a name="what-are-the-key-timelines-and-milestones"></a>Anahtar zaman çizelgeleri ve kilometre taşları nelerdir?

Zaman çizelgeleri ve kilometre taşları dahil olmak üzere bu güvenlik gereksinimleriyle ilişkili koşullar, [Microsoft Iş ortağı sözleşmesi](microsoft-partner-agreement.md)'ne dahildir. CSP programına katılımınız ile uyumlu kalmak için, bu güvenlik gereksinimlerini en kısa sürede uygulamanız gerekir.

### <a name="what-will-happen-if-i-dont-implement-these-partner-security-requirements"></a>Bu iş ortağı güvenlik gereksinimlerini uygulamadığımda ne olur?

Microsoft Iş ortağı sözleşmesi, Kullanıcı hesapları için Multi-Factor Authentication 'ı zorunlu hale getirmek ve Iş Ortağı Merkezi API 'siyle etkileşim kurmak için güvenli uygulama modelini benimsemenizi gerektirir. 

Bu güvenlik uygulamalarında olmayan iş ortakları, CSP programını Transact veya temsilci yönetici hakları kullanarak müşteri kiracılarını yönetme olanağını kaybedebilir.

### <a name="do-the-security-requirements-apply-to-all-geographies"></a>Güvenlik gereksinimleri tüm coğrafi lıklar için geçerlidir mi?

Evet, güvenlik gereksinimleri tüm coğrafi lıklar için geçerlidir. Bağımsız bir bulut (ABD Kamu ve Almanya) aracılığıyla işlem yapılan tüm iş ortaklarının bu yeni güvenlik gereksinimlerini hemen harekete geçerek benimsemelerini kesinlikle öneririz. Ancak, bu iş ortaklarının şu anda güvenlik gereksinimlerini karşılaması gerekli değildir. Microsoft gelecekte bağımsız bulutlar için bu güvenlik gereksinimlerini uygulamayla ilgili ek ayrıntılar sağlayacaktır.

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>Bir hesap için dışlama elde etmek mümkün mü?

Hayır, hiçbir kullanıcı hesabını çok faktörlü kimlik doğrulaması (MFA) zorlama gereksiniminin dışında tutmak mümkün değildir. İş ortağı olmanın yüksek ayrıcalıklı yapısı göz Microsoft İş Ortağı Sözleşmesi iş ortağı kiracınız için çok faktörlü kimlik doğrulamasının zorunlu kılınmasını gerektirir.

### <a name="how-do-i-know-if-i-have-met-the-partner-security-requirements"></a>Nasıl yaparım? güvenlik gereksinimlerini karşıladım mı?

Aşağıdaki adımları tamamlayın:

- İş ortağı güvenlik gereksinimlerinde belirtilen tüm gereksinimleri [karşılamanız gerekir.](partner-security-requirements.md)
- İş ortağı kiracınız içinde tüm kullanıcı hesaplarının çok faktörlü kimlik doğrulamasının zorunlu olduğundan emin olun.

Eylem gerçekleştirebilirsiniz önemli alanları belirlemeye yardımcı olmak için, güvenlik gereksinimleri [durum](https://partner.microsoft.com/commerce/security/compliance) raporu aracılığıyla kullanılabilir İş Ortağı Merkezi.

Durum raporu hakkında daha fazla bilgi için bkz. [iş ortağı güvenlik gereksinimleri durumu.](partner-security-compliance.md)

## <a name="required-actions"></a>Gerekli Eylemler

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>Gereksinimleri karşılamak için hangi önemli eylemleri gerçekleştir ihtiyacım var?

CSP programı (doğrudan fatura, dolaylı sağlayıcı ve dolaylı kurumsal bayi), Danışmanlar ve Denetim Masası Satıcılarının gereksinimleri karşılaması gerekir.

1. **Tüm kullanıcılar için MFA zorlama**

    CSP programı, Danışmanlar ve Denetim Masası Satıcılarının iş ortağı kiracılarında tüm kullanıcılar için MFA'nın uygulanması gerekir.

    Ek hususlar:

    - Dolaylı sağlayıcıların, henüz bunu yapmamışsa İş Ortağı Merkezi dolaylı kurumsal bayilerle birlikte çalışması ve kurumsal bayilerini gereksinimleri karşılamaya teşvik etmek için çalışması gerekir.
    - Azure MFA, zaman tabanlı tek kullanımlık parolaları (TOTP) destekleyen bir kimlik doğrulayıcı uygulamanın tek doğrulama yöntemiyle Azure AD güvenlik varsayılanları aracılığıyla iş ortağı kiracısı tüm kullanıcılara ücretsiz olarak sunulmaktadır.
    - Telefon çağrısı veya kısa mesaj [Azure Active Directory Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium) diğer yöntemler varsa SKUS'lar aracılığıyla ek doğrulama yöntemleri kullanılabilir.
    - İş ortakları, Microsoft ticari bulut hizmetlerine erişirken her hesap için bir üçüncü taraf MFA çözümü de kullanabilir.

2. **Güvenli Uygulama Modeli benimseme**

    Herhangi bir API (Azure Resource Manager, Microsoft Graph, İş Ortağı Merkezi API gibi) kullanarak özel tümleştirme geliştiren veya PowerShell gibi araçları kullanarak özel otomasyon uygulayan tüm iş ortaklarının Microsoft bulut hizmetleriyle tümleştirilecek [Güvenli Uygulama Modeli](/partner-center/develop/enable-secure-app-model) çerçevesini benimsemesi gerekir. Bunu yapmaması, MFA dağıtımı nedeniyle bir kesintiye neden olabilir. Aşağıdaki kaynaklar, modeli benimsemeye ilişkin bir genel bakış ve rehberlik sağlar.

    - [Güvenli Uygulama Modeli genel bakış](/partner-center/develop/enable-secure-app-model)
    - [İş Ortağı Merkezi: Güvenli Uygulama Modeli kılavuzu](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [CSP programındaki iş ortakları: Uygulamanın etkinleştirilmesi için .NET Güvenli Uygulama Modeli](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
    - [CSP programındaki iş ortakları: Uygulamaları etkinleştirmek için Java Güvenli Uygulama Modeli](/samples/microsoft/partner-center-java-samples/secure-app-model/)
    - [İş Ortağı Merkezi kimlik doğrulaması belgesi](/partner-center/develop/partner-center-authentication)
    - [İş Ortağı Merkezi PowerShell Multi-Factor Authentication (MFA) belgesi](/powershell/partnercenter/multi-factor-auth)

    Güvenli Uygulama Modeli çerçevesinin benimsenmesiyle ilgili bir denetim masası kullanıyorsanız satıcıya başvurun.

    Denetim masası satıcılarının denetim [masası satıcısı](enroll-as-cpv.md) olarak İş Ortağı Merkezi ve bu gereksinimi hemen uygulamaya başlaması gerekir. İş Ortağı Merkezi: [Güvenli Uygulama Modeli bakın.](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) Denetim masası satıcılarının kimlik bilgileri yerine CSP iş ortaklarının onaylarını kabul etmeleri ve yönetmeleri ve tüm mevcut CSP iş ortaklarının kimlik bilgilerini temizlemeleri gerekir.

## <a name="multi-factor-authentication"></a>Multi-factor authentication

### <a name="what-is-multi-factor-authentication-mfa"></a>Çok faktörlü kimlik doğrulaması (MFA) nedir?

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

Hayır, üçüncü taraf bir çözüm kullanıyorsanız Active Directory Federasyon Hizmeti (ADFS) olması gerekmez. Çözümünün gereksinimlerini belirlemek için çözümün satıcısıyla birlikte çalışmanız önerilir.

### <a name="is-it-a-requirement-to-enable-azure-ad-security-defaults"></a>Azure AD güvenlik varsayılanlarını etkinleştirme gereksinimi var mı?

Hayır, Azure AD güvenlik varsayılanlarını etkinleştirmeniz gerekmez.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>MFA gereksinimini karşılamak için koşullu erişim kullanılabilir mi?

Evet, iş ortağı kiracınıza hizmet hesapları da dahil olmak üzere her kullanıcı için MFA uygulamak üzere koşullu erişimi kullanabilirsiniz. Ancak, iş ortağı olmanın yüksek ayrıcalıklı doğasına göre her kullanıcının her bir kimlik doğrulamasında MFA zor olduğundan emin olmak gerekir. Bu, MFA gereksinimini yitiren koşullu erişim özelliğini kullana anlamına gelir.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>İş ortağı tarafından kullanılan hizmet Azure AD Connect iş ortağı güvenlik gereksinimleri etkilemayacak mı?

Hayır, iş ortağı tarafından Azure AD Connect hesabı, iş ortağı güvenlik gereksinimleri tarafından etkilenmez. MFA'nın zorlanma Azure AD Connect bir sorun yaşamanız, Ardından Microsoft desteğiyle bir teknik destek isteği açın.

## <a name="secure-application-model"></a>Güvenli Uygulama Modeli

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>Gereksinimleri karşılamak için güvenli uygulama modelini kimler benimsemeli?

Microsoft, Multi-Factor Authentication kullanan Bulut Çözümü Sağlayıcısı (CSP) iş ortaklarının ve Denetim Masası Satıcılarının (CPV) kimlik doğrulamasını sağlamak için güvenli, ölçeklenebilir bir çerçeve tanıtmaktadır. Daha fazla bilgi için [bkz. Güvenli Uygulama Modeli kılavuzu.](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) Herhangi bir API (Azure Resource Manager, Microsoft Graph, İş Ortağı Merkezi API gibi) kullanarak özel tümleştirme geliştiren veya PowerShell gibi araçları kullanarak özel otomasyon uygulayan tüm iş ortaklarının Microsoft bulut hizmetleriyle tümleştirilecek [Güvenli Uygulama Modeli](/partner-center/develop/enable-secure-app-model) çerçevesini benimsemesi gerekir.

### <a name="what-is-the-secure-application-model"></a>Hangi Güvenli Uygulama Modeli?

Microsoft, Multi-Factor Authentication'Bulut Çözümü Sağlayıcısı (CSP) iş ortaklarının ve Denetim Masası Satıcılarının (CPV) kimlik doğrulamasını sağlamak için güvenli, ölçeklenebilir bir çerçeve tanıtmaktadır. Daha fazla [Güvenli Uygulama Modeli için bkz.](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) Güvenli Uygulama Modeli kılavuzu.  

### <a name="how-do-i-implement-the-secure-application-model"></a>Nasıl yaparım? uygulamak Güvenli Uygulama Modeli?

Herhangi bir API (Azure Resource Manager, Microsoft Graph, İş Ortağı Merkezi API gibi) kullanarak özel tümleştirme geliştiren veya PowerShell gibi araçları kullanarak özel otomasyon uygulayan tüm iş ortaklarının Microsoft bulut hizmetleriyle tümleştirilecek [Güvenli Uygulama Modeli](/partner-center/develop/enable-secure-app-model) çerçevesini benimsemesi gerekir. Bunu yapmaması, MFA dağıtımı nedeniyle bir kesintiye neden olabilir. Aşağıdaki kaynaklar, modeli benimsemeye ilişkin bir genel bakış ve rehberlik sağlar.

- [Güvenli Uygulama Modeli genel bakış](/partner-center/develop/enable-secure-app-model)
- [İş Ortağı Merkezi: Güvenli Uygulama Modeli kılavuzu](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [CSP programındaki iş ortakları: Uygulamanın etkinleştirilmesi için .NET Güvenli Uygulama Modeli](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [CSP programındaki iş ortakları: Uygulamaları etkinleştirmek için Java Güvenli Uygulama Modeli](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [İş Ortağı Merkezi kimlik doğrulaması belgesi](/partner-center/develop/partner-center-authentication)
- [İş Ortağı Merkezi PowerShell Multi-Factor Authentication (MFA) belgesi](/powershell/partnercenter/multi-factor-auth)

Denetim masası kullanıyorsanız, Güvenli Uygulama Modeli çerçevesinin benimsenmesi konusunda satıcıya başvurmanız gerekir.

Denetim masası satıcılarının denetim [masası satıcısı](enroll-as-cpv.md) olarak İş Ortağı Merkezi ve bu gereksinimi hemen uygulamaya başlaması gerekir. İş Ortağı Merkezi: [Güvenli Uygulama Modeli bakın.](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) Denetim masası satıcılarının kimlik bilgileri yerine CSP iş ortaklarının onaylarını kabul etmeleri ve yönetmeleri ve tüm mevcut CSP iş ortaklarının kimlik bilgilerini temizlemeleri gerekir.

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>Uygulamanın Güvenli Uygulama Modeli API/SDK için İş Ortağı Merkezi gerekiyor mu?

Tüm kullanıcı hesapları için çok faktörlü kimlik doğrulamasını zorlayarak, etkileşimli olmayan bir şekilde çalışması amaçlanan tüm otomasyon veya tümleştirmeler etkileniyor. İş ortağı güvenlik gereksinimleri, İş Ortağı Merkezi API'si için güvenli uygulama modelini etkinleştirmeniz gerektirmektedir ancak otomasyon ve tümleştirme ile ikinci bir kimlik doğrulaması faktörüne ihtiyaç karşılamak için kullanılabilir.

>[!Note] 
>Erişilen kaynakların, erişim belirteci tabanlı kimlik doğrulamasını desteklemesi gerekir.

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

### <a name="i-am-a-cpv-how-do-i-enroll"></a>Ben bir CPV'yim. Nasıl yaparım? mi?

Denetim masası satıcısı (CPV) olarak kaydolmak için burada sağlanan yönergeleri [izleyin.](enroll-as-cpv.md)

CPV'lerin kayıt bağlantısını almak ve CPV ile iş ilişkisi olan veya işletmesini bilen bir Microsoft çalışanı sponsoru sağlamak için [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) iletişim kurması gerekir. Örneğin, bir İş Ortağı Geliştirme Yöneticisi (PDM).

Uygulamanıza kaydol İş Ortağı Merkezi ve uygulamalarınızı kaydettiniz mi, bu API'lere İş Ortağı Merkezi sahip oluruz. Yeni bir CPV'niz İş Ortağı Merkezi korumalı alan bilgilerini bir uyarı bildirimiyle alırsınız. Microsoft CPV olarak kaydı tamamlandıktan ve CPV anlaşmasını kabul ettiktan sonra:

1. Çok kiracılı uygulamayı yönetme (uygulamaları Azure portal uygulama ekleme ve uygulama kayıttan İş Ortağı Merkezi).

   >[!Note]
   >CPV'lerin api'ler için İş Ortağı Merkezi için yetkilendirilen uygulamaları İş Ortağı Merkezi gerekir. Uygulamalar tek başına Azure portal api'ler için CPV uygulamalarını İş Ortağı Merkezi yetkilendirmez.

1. CPV profilinizi görüntüleme ve yönetme.

1. CPV özelliklerine erişmesi gereken kullanıcılarınızı görüntüleme ve yönetme. CPV yalnızca Genel Yönetici rolüne sahip olabilir.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>İş Ortağı Merkezi SDK'sı. SDK otomatik olarak bu Güvenli Uygulama Modeli?

Hayır, bu kılavuzda sağlanan yönergeleri Güvenli Uygulama Modeli [gerekir.](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-dont-have-mfa-enabled"></a>MFA'nın etkin olduğu hesaplarla güvenli uygulama modeli için bir yenileme belirteci oluşturmam gerekir mi?

Evet, MFA uygulanmadan bir hesap kullanılarak yenileme belirteci oluşturulabilirsiniz. Ancak bu durum önılmalıdır. MFA'nın etkin olduğu bir hesap kullanılarak oluşturulan belirteçler, MFA gereksinimi nedeniyle kaynaklara erişe olmayacaktır.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>MFA'yi etkinleştirirken uygulamam nasıl erişim belirteci elde eder?

Yeni güvenlik gereksinimlerine [uygun Güvenli Uygulama Modeli](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) ayrıntılı bilgi sağlayan Güvenli Uygulama Modeli kılavuzuna uyması gerekir. .NET örnek kodunu burada ve Java [örnek](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) kodunu burada [bulabilirsiniz.](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>CPV olarak, CPV kiracımızda veya CSP iş ortağının kiracısı olarak bir Azure AD uygulaması oluşturabilir miyim?

CPV'nin, CPV olarak Azure Active Directory kiracıda bir uygulama oluşturması gerekir.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>Yalnızca uygulama kimlik doğrulaması kullanan bir CSP'yim. Herhangi bir değişiklik yapmak zorunda musunuz?

Yalnızca uygulama kimlik doğrulaması etkilenmez çünkü erişim belirteci isteği için kullanıcı kimlik bilgileri kullanılmaz. Kullanıcı kimlik bilgileri paylaşılıyorsa denetim masası satıcılarının (CPV) Güvenli Uygulama Modeli çerçeveyi benimsemesi ve mevcut iş ortağı kimlik bilgilerini temizlemesi gerekir. [](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>CPV olarak erişim belirteçlerini almak için yalnızca uygulama kimlik doğrulama stili kullanılabilir mi?

Hayır, Denetim Masası iş ortakları, erişim belirteçlerini iş ortağı adına talep etmek için yalnızca uygulama kimlik doğrulama stilini kullanamaz. Uygulama + kullanıcı kimlik doğrulaması stilini kullanan güvenli uygulama modelini uygulamalı.

## <a name="technical-enforcement"></a>Teknik Zorlama

### <a name="what-is-the-activation-of-security-safeguards"></a>Güvenlik önlemlerinin etkinleştirilmesi nedir?

Bulut Çözümü Sağlayıcısı (CSP) programına katılan tüm iş ortakları, Denetim Masası Satıcıları (CPV) ve Danışmanlar, uyumlu kalmak için zorunlu güvenlik gereksinimlerini uygulamalıdır.

Microsoft, ek koruma sağlamak için, iş ortaklarının yetkisiz erişimi önlemek için çok faktörlü kimlik doğrulaması (MFA) doğrulamasını kullanarak kiracılarını ve müşterilerinin güvenliğini sağlamalarına yardımcı olan güvenlik önlemlerini etkinleştirmeye başladı.  

Tüm iş ortağı kiracıları için adına yönetici (AOBO) özellikleri için etkinleştirmeyi başarıyla tamamladık. İş ortaklarının ve müşterilerin korunmasına yardımcı olmak ve Q2 CY2020'yi hedeflemek için CSP'de İş Ortağı Merkezi işlemleri için etkinleştirmeyi başlatacak, iş ortaklarının işletmelerini ve müşterilerini kimlik hırsızlığıyla ilgili olaylardan korumalarına yardımcı olacağız.

Daha fazla bilgi için İş ortağı kiracınız için Çok Faktörlü Kimlik Doğrulamasını [(MFA) Mandating (MFA) sayfasını ziyaret](partner-security-requirements-mandating-mfa.md) edin.

### <a name="i-am-using-a-third-party-mfa-solution-and-i-am-being-blocked-what-should-i-do"></a>Üçüncü taraf bir MFA çözümü kullanıyor ve engellenmişim, ne yapabilirim?

Kaynaklara erişen hesabın çok faktörlü kimlik doğrulaması için zorlanmış olduğunu doğrulamak için, MFA'nın listelenmiş olup olduğunu görmek için kimlik doğrulama yöntemi başvuru talebi denetlenecek. [](https://tools.ietf.org/html/rfc8176) Bazı üçüncü taraf çözümleri bu talebi veya MFA değerini dahil etmemektedir. Talep eksikse veya MFA değeri listelenmiyorsa, kimliği doğrulanmış hesabın çok faktörlü kimlik doğrulaması için zorlanmış olup olmadığını belirlemenin bir yolu yoktur. Çözümün kimlik doğrulama yöntemi başvuru talebi göndermesi için hangi eylemlerin gerçekleştireceklerini belirlemek üzere üçüncü taraf çözümünüz için satıcıyla birlikte çalışmanız gerekir.

Beklenen [talebi üçüncü taraf çözüme](/powershell/partnercenter/test-partner-security-requirements) verme konusunda emin değilseniz bkz. İş Ortağı Güvenlik Gereksinimlerini Test Etme.

### <a name="mfa-is-blocking-me-from-supporting-my-customer-using-aobo-what-should-i-do"></a>MFA, AOBO kullanarak müşterimi desteklememi engelliyor, ne yapabilirim?

İş ortağı güvenlik gereksinimlerinin teknik zorlaması, kimliği doğrulanmış hesabın çok faktörlü kimlik doğrulaması için zorlandığı denetlenir. Hesap henüz açıksa oturum açma sayfasına yeniden yönlendirilen ve yeniden kimlik doğrulaması yapılan bir hesap istenir. İş ortağı kiracınız için Çok [Faktörlü Kimlik Doğrulamasını (MFA) Mandating this Mandating multi-factor authentication (MFA) belgelerinde ek deneyim ve rehberlik okuyun.](partner-security-requirements-mandating-mfa.md#partner-delegated-administration) Etki alanınız federasyona alınmamıştır, başarıyla kimlik doğrulaması yapıldıktan sonra çok faktörlü kimlik doğrulamasını ayarlamanız istenir. Bu tamamlandıktan sonra, AOBO kullanarak müşterinizi yönetabileceksiniz. Etki alanının federe olduğu senaryoda, hesabın Multi-Factor Authentication için gerekmekte olduğundan emin olmanız gerekir.

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
- Yaklaşan iş ortağı ofis saatlerini ve web seminerlerini ziyaret edin. Ayrıntılı [zamanlamayı ve kaynakları burada kontrol edin.](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)

### <a name="resources-for-adopting-secure-application-model"></a>Güvenli uygulama modelini benimseme kaynakları

- [Güvenli Uygulama Modeli genel bakış](/partner-center/develop/enable-secure-app-model)
- [İş Ortağı Merkezi: Güvenli Uygulama Modeli kılavuzu](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [CSP programındaki iş ortakları: Uygulamanın etkinleştirilmesi için .NET Güvenli Uygulama Modeli](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [CSP programındaki iş ortakları: Uygulamaları etkinleştirmek için Java Güvenli Uygulama Modeli](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [İş Ortağı Merkezi kimlik doğrulaması belgesi](/partner-center/develop/partner-center-authentication)
- [İş Ortağı Merkezi PowerShell Multi-Factor Authentication (MFA) belgesi](/powershell/partnercenter/multi-factor-auth)

## <a name="support"></a>Destek

### <a name="where-can-i-get-support"></a>Nereden destek a bilmiyorum?

Destek kaynaklarının güvenlik gereksinimlerini karşılaması için, İş Ortakları için Gelişmiş Destek (ASfP) varsa Hizmet Hesap Yöneticinize başvurun; İş Premier Destek sözleşmesi (PSfP) için Service Account Manager ve Technical Account Manager ile iletişime geçin.

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>Nasıl yaparım? uygulama modeli çerçevesini benimsememe yardımcı olacak teknik bilgiler ve destek mi alasınız?

MpN avantajlarınız aracılığıyla Azure Active Directory için teknik ürün destek seçenekleri mevcuttur. Etkin bir ASfP veya PSfP aboneliğine erişimi olan iş ortakları, kullanılabilir seçenekleri en iyi şekilde anlamak için ilişkili hesap yöneticisi (SAM/TAM) ile birlikte kullanılabilir.

### <a name="how-do-i-contact-support-if-ive-lost-access-to-partner-center"></a>Nasıl yaparım? erişimimi kaybetmem halinde de destekle iletişime İş Ortağı Merkezi?

MFA sorunu nedeniyle erişimi kaybederseniz kiracınız için genel yöneticiye ulaşın. Şirket içi IT departmanınız size genel yöneticinizin kim olduğunu söyler. 

Parolanızı unuttuysanız yardım için [Oturum açamıyor'a](unable-to-sign-in.md) bakın.

### <a name="where-can-i-find-more-information-about-common-technical-issues"></a>Yaygın teknik sorunlar hakkında daha fazla bilgiyi nerede bulamıyorum?

Yaygın teknik sorunlar hakkında bilgi, iş ortaklarının api'lerini kullanan iş ortakları [için İş Ortağı Merkezi güvenlik İş Ortağı Merkezi bulunabilir](partner-security-requirements.md)