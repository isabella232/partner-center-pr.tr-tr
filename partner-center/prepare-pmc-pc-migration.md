---
title: Partner Membership Center'den taşıma
ms.topic: article
ms.date: 06/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: İşletmenizi yeni bir işletmeye taşımadan önce yararlı bilgileri ve sık Partner Membership Center soruları İş Ortağı Merkezi.
author: parthpandyamsft
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 7f533240d5236f03fe277d4c6dfa02ed1c58b63c
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855021"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Partner Membership Center(PMC) ile İş Ortağı Merkezi

**Uygun roller:** Genel yönetici | Kullanıcı yönetimi yönetici | Satış aracısı | Yönetici aracısı

Microsoft ile iş ilişkilerinizi yönetmek Partner Membership Center için üyelik yönetimini İş Ortağı Merkezi (PMC) hedefine taşınıyoruz. Yeni bir İş Ortağı Merkezi mümkün olduğunca verimli ve kolay olması istiyoruz. PmC'den farklı olan İş Ortağı Merkezi alanları belirledik ve taşımadan önce bunları anlamak ve hazırlamak istediğinizi düşünüyoruz.

## <a name="account-and-identity-setup"></a>Hesap ve kimlik kurulumu

Hesap ve kimlik kurulumu hakkında sık sorulan soruların yanıtları için aşağıya bakın.

### <a name="what-is-an-azure-active-directory-azure-ad-work-account"></a>Azure Active Directory (Azure AD) iş hesabı nedir?

Azure iş hesabı, Azure, Microsoft Intune veya Office 365 gibi bir Microsoft bulut hizmetine abone olurken sizin için oluşturulan, Azure genel bulut'ta şirket için ayrılmış ve yalıtılmış bir sanal temsildir.

İş hesabınız, Azure AD kullanıcılarınızı ve bu kullanıcılarla ilgili bilgileri (e-posta, parolalar, profil verileri, izinler gibi) barındırıyor. İş hesabı ayrıca bir şirkete ve şirketin güvenliğine ilişkin grupları, uygulamaları ve diğer bilgileri içerir. 

İş e-postanız Azure Active Directory kiracınıza aittir. Hesap sahibi olmak İş Ortağı Merkezi AAD kiracısına sahip olmak gerekir. Azure AD'de dizininizi Azure Active Directory [hakkında daha fazla bilgi için, makaleyi okuyun.](/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad)

Bu İş Ortağı Merkezi iş e-postanızı kullanarak kişisel e-posta adresinizle değil, hesabınızla oturum açın.

- İş hesabınız: john@contoso.com
- Kişisel hesabınız: John@outlook.com

### <a name="what-account-should-you-sign-into-partner-center-with-if-you-have-an-aad-tenant-with-microsoft-for-office-365-for-example-and-you-also-have-a-tenant-for-your-csp-business"></a>Microsoft'ta (örneğin Office 365 için) bir AAD kiracınız varsa ve CSP işletmeniz için bir kiracınız varsa İş Ortağı Merkezi'de hangi hesapla oturum açmanız gerekir?

Iş Ortağı Merkezi 'Nde CSP hesabı ya da MPN iş e-posta hesabınızla oturum açabilirsiniz. CSP iş e-postanızı kullanarak oturum açmayı seçerseniz, panonuzda sol gezinti, hem MPN hem de CSP program bilgilerini görüntüler. MPN Azure AD kiracısı iş e-postalarınız ile oturum açarsanız yalnızca MPN program bilgilerinizi görürsünüz. 

### <a name="if-you-dont-want-to-use-your-existing-office-365-azure-ad-tenant-for-partner-center-you-can-create-a-new-tenant-prior-to-migrating-from-pmc"></a>Iş Ortağı Merkezi için mevcut Office 365 Azure AD kiracınızı kullanmak istemiyorsanız, PMC 'den geçiş yapmadan önce yeni bir kiracı oluşturabilirsiniz.

Iş Ortağı Merkezi hesabınızı ayarlamak için mevcut bir Azure AD kiracısını kullanmak istememeniz pek çok nedeni olabilir. Iş Ortağı Merkezi 'ne geçiş yapmaya başlamadan önce, yeni bir Azure AD kiracısı oluşturmak için [Azure Portal](https://ms.portal.azure.com/#home) gidin. [Azure Active Directory yeni kiracı oluşturma](/azure/active-directory/develop/quickstart-create-new-tenant)bölümündeki yönergeleri izleyin. Iş Ortağı Merkezi hesabınızı ayarlamak için yeni AAD kiracısını kullanın. Kiracıyı oluşturmak için bir genel yönetici olmanız gerekir. 

### <a name="user-roles-including-guest-user-roles-in-partner-center"></a>Iş Ortağı Merkezi 'nde Konuk Kullanıcı rolleri dahil Kullanıcı rolleri

İş Ortağı Merkezi, yapılması gereken iş türlerine bağlı olarak farklı rol türlerine sahiptir. Azure AD rolleri olan genel yönetici gibi roller vardır. Bazı roller, bulut hizmeti sağlayıcısı programı veya teşvikleri gibi programlara özgüdür ve MPN 'ye özgü roller vardır. Tüm Iş Ortağı Merkezi rollerinin ne olduğunu öğrenmek için [Kullanıcı rolü rolleri ve izinleri](permissions-overview.md)oku makalesini okuyun.

### <a name="what-happens-to-my-users-roles-when-they-move-from-pmc-to-partner-center"></a>PMC 'den Iş Ortağı Merkezi 'ne geçtiğinde kullanıcılarınızın rollerine ne olur?

Geçiş işlerini yapan MPN genel yöneticisi veya birincil program ile ilgili kişi dışında, PMC 'deki tüm kullanıcılar yönetici rollerini kaybeder. Geçişi tamamlayan kişinin Iş Ortağı Merkezi 'ne rol ataması gerekir. Iş ortağı merkezindeki roller PMC 'deki rollerden farklıdır. Iş Ortağı Merkezi 'nde Kullanıcı rolleri hakkında daha fazla bilgi için bkz. [Kullanıcı rollerini ve izinlerini ata] (Permissions-overview.md ve [PMC 'Den Iş ortağı merkezine taşıma](move-pmc-pc-map.md#user-roles) .

### <a name="whats-the-difference-between-my-company-profile-and-my-business-profile"></a>Şirket profilimi ve iş profilim arasındaki fark nedir?

Şirket profiliniz; adresi, konumları, birincil ilgili kişiyi, bankayı ve vergi ayrıntılarını içeren, şirketinize ilişkin bilgilerdir.

İş profiliniz, kendinizi müşterilere nasıl sunabilirsiniz? Logonuzu, iş odağınızı ve uzmanlığınızı gösteren bir pazarlama sayfasıdır.

### <a name="what-does-account-consolidation-mean-for-my-account"></a>Hesap birleştirme hesabım için ne anlama geliyor?

Birden çok MPN hesabını İş Ortağı Merkezi geçirmek için aynı Azure AD kiracısını kullanırsanız, sistem bunu otomatik olarak tanır ve hesaplarınızı birleştirmenizi sorar. Aynı Azure AD kiracısı ile ilişkilendirilmiş birden çok etki alanınız olsa bile bu durum doğrudur. 

Ayrı AAD kiracıları kullanarak İş Ortağı Merkezi yine de geçişe karar veresiniz, ancak bunun yetkinliklerinizi yalıtılmış olarak değerlendirmesine ve ek satın alma maliyetlerine neden olduğunu unutmayın. Hesap birleştirme hakkında daha fazla bilgi için şirket [hesaplarınızı birleştirme makalesini okuyun](consolidate-accounts.md)

### <a name="if-i-have-multiple-aad-tenants-and-a-single-mpn-account-is-it-possible-to-link-them-in-partner-center"></a>Birden çok AAD kiracım ve tek bir MPN hesabım varsa, bunları birden çok AAD kiracısına İş Ortağı Merkezi?

Evet, İş Ortağı Merkezi Azure AD kiracılarını tek bir azure hesabına İş Ortağı Merkezi.
Hesap birleştirme hakkında daha fazla bilgi için şirket [hesaplarınızı birleştirme makalesini okuyun](consolidate-accounts.md)

### <a name="are-there-restrictions-to-adding-multiple-azure-ad-tenants-to-a-single-partner-center-account"></a>Tek bir azure hesabına birden çok Azure AD kiracısı eklemeye yönelik İş Ortağı Merkezi var mı?

Azure AD kiracısı zaten mevcut bir İş Ortağı Merkezi hesabıyla ilişkilendirilmişse, çok kiracılı özelliği İş Ortağı Merkezi yeni kiracı hesaplarıyla ilişkilendirilemez. Bunu düşünmenin bir diğer yolu da Azure AD kiracısı yalnızca bir İş Ortağı Merkezi hesabıyla ilişkilendirilebilirsiniz ancak İş Ortağı Merkezi hesabıyla ilişkilendirilmiş birden çok kiracı olabilir.

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Microsoft İş Ortağı Ağı (MPN) üyelik geçişi 

MPN üyelik geçişi hakkında sık sorulan soruların yanıtlarına aşağıdaki yanıtlara bakın.

### <a name="who-can-perform-the-move-from-pmc-to-partner-center"></a>PMC'den İş Ortağı Merkezi'a taşımayı kim İş Ortağı Merkezi?

Şirket MPN genel yöneticiniz veya birincil program ilgili kişisi (bu iki rol genellikle aynı kişi tarafından tutularak) taşıma işlemini başlatarak gerçekleştir olabilir.

### <a name="will-the-person-completing-the-migration-become-the-primary-contact-on-the-company-legal-profile-in-partner-center"></a>Geçiş işlemini tamamlayan kişi, Iş Ortağı Merkezi 'nde şirket yasal profilinde birincil iletişim olur mu?

Ancak, birincil iletişim sözleşmesinin anlaşmaları imzalama yetkisi olan birisi olması gerekir.

### <a name="can-microsoft-migrate-my-mpn-membership-for-me"></a>Microsoft, MPN üyeliğimi bana geçirebilir mi?

Hayır. Microsoft, üyelik hesabınızı iş ortağı merkezi 'ne taşımanıza yardımcı olamaz. Geçiş işlemini başlatmak için iş hesabınızla (oturum açma kimlik bilgileri) oturum açarak hesabınızı taşımanız gerekir. Hesabınızı taşıma adımlarını tamamladıktan sonra, avantajlarınızı yönetmeye başlayabilir ve haklara erişebilmek ve üyeliği yönetmeye yardımcı olması için Kullanıcı rollerini ve izinlerini ekibinize atayabilirsiniz. 

Microsoft, teşvikleri için geçerli Uzmanlıklar, avantajları, konum bilgilerini, banka/vergi bilgilerini ve Iş ortağı Üniversitesi erişimi de dahil olmak üzere MCP ilişkilendirmelerini otomatik olarak taşıyacaktır.

### <a name="how-will-the-renewal-policy-change"></a>Yenileme ilkesi nasıl değiştirilir?

Iş Ortağı Merkezi 'nde, yenileme penceresi, yıl dönümü tarihinizden aşağıdaki 30 gün içinde olur.

### <a name="will-our-competencies-remain-unchanged-after-we-move-to-partner-center"></a>Iş Ortağı Merkezi 'ne taşıdıktan sonra, uzmanlarımızın değişmeden kalsın mı?

Evet, Uzmanlıklar Iş Ortağı Merkezi 'ne geçiş tarafından etkilenmeyecektir. Tutarsızlıklarla karşılaşırsanız [desteğe](https://partner.microsoft.com/support)başvurun.

### <a name="will-my-benefits-including-cloud-benefits-technical-support-software-benefits-visual-studio-change-after-we-move"></a>Avantajlarım (bulut avantajları, teknik destek, yazılım avantajları, Visual Studio dahil), taşıdıktan sonra değişiklik mi?

Uygun avantajlarınız değişmeyecektir. Tutarsızlıklarla karşılaşırsanız [desteğe](https://partner.microsoft.com/support)başvurun.

### <a name="will-our-microsoft-accounts-that-have-visual-studio-benefits-allocations-be-honored"></a>Visual Studio avantajlar ayırmaları olan Microsoft hesaplarımıza göre kabul edilecek mi?

Evet. MSAs 'ye ayrılan Visual Studio avantajları kabul edilir ve korunur. Ayrıca Iş Ortağı Merkezi 'nde yenilemeden sonra da korunacaktır. Ancak, Iş Ortağı Merkezi 'nde geçiş yapıldıktan sonra bir MSA ayırmayı kaldırırsanız, Iş Ortağı Merkezi 'ne geri eklenemez.

İş Ortağı Merkezi 'nde iş ortağı, iş hesapları ve Konuk Kullanıcı hesapları ekleyebilir ve bu, ortağın Azure AD kiracısında MPN Yöneticisi olduğu aynı kiracıdan MSA. İş ortağı birden çok Azure AD kiracısı içinde genel yönetici ise ve tüm bu kiracılar aynı İş Ortağı Merkezi hesabıyla ilişkili ise, iş ortağının tüm bu kiracılar arasında kullanıcıları Visual Studio avantajlarına ve Azure kullanım tabanlı ayırmalara eklemesine izin verilir.

Konuk kullanıcılara MPN yöneticisi veya genel yönetici tarafından Visual Studio tabanlı abonelikler atanabilir, ancak konuk kullanıcılar MSA'larını kullanarak İş Ortağı Merkezi oturum açmaz. Öte yandan konuk kullanıcılar Azure'da oturum Visual Studio ve atanan avantajlarını doğrulamak ve kullanmak için kullanılabilir.

### <a name="how-should-we-manage-our-mcp-associations-and-our-partner-university-access"></a>MCP ilişkilendirmelerimizi ve Partner University erişimimizi nasıl yöneteceğiz?

PMC'den hareket edecek MCP ilişkilendirmeleri üzerinde değişiklik yoktur. Ancak, İş Ortağı Merkezi'a İş Ortağı Merkezi tüm yeni çalışanların şirket içinde İş Ortağı Merkezi. Mevcut kullanıcılar için Tüm Partner University izinlerinizi kullanabilirsiniz [](https://partner.microsoft.com/training) ancak yeni çalışanlar Partner University'ye nasıl erişim elde edecekleri hakkında bilgi almak için eğitim merkezine gitmektedir.

### <a name="how-do-i-view-mcp-information-once-i-move-to-partner-center"></a>Nasıl yaparım?'a taşınarak MCP bilgilerini İş Ortağı Merkezi?

Panonun **sol** gezinti çubuğundan Yetkinlikler'i seçin. Yetkinlikler **sayfasından** beceri raporunu indirebilirsiniz. Beceri raporu, iş birliğine ilişkin yetkinliklere ve programlara uygun beceriler edinen kullanıcılarınızı İş Ortağı Merkezi. Kullanıcılarınız beceri kazandı ancak bu beceriler üzerinde çalışmakta olduğunuz yetkinliklerle ilgili değilse, bunlar raporda listelenmiyor.

### <a name="are-customer-references-used-in-partner-center"></a>Müşteri başvuruları veri kaynaklarında İş Ortağı Merkezi?

Hayır, bu hizmetlerde uzmanlık gereksinimlerini karşılamak için müşteri başvurularını İş Ortağı Merkezi.

### <a name="will-partner-of-record-associations-move-to-partner-center"></a>Kayıt İş Ortağı ilişkilendirmeleri İş Ortağı Merkezi?

Evet, Kayıt İş Ortağı'nın hiçbir değişikliği yoktur. İş ortağı kimliğinizi [müşterilerinize bağlama hakkında daha fazla bilgi bulabilirsiniz.](/azure/billing/billing-partner-admin-link-started)

### <a name="is-there-an-impact-to-incentives-because-of-the-move-to-partner-center"></a>Teşviklerin bir etkisi var mı? Bu, İş Ortağı Merkezi?

Hayır, konum birleştirmeden hesabını taşıdıysanız teşvikler üzerinde hiçbir etkisi olmaz. İşletmenizde, PMC 'de birden çok hesap varsa ve iş ortağı Merkezi ' ne geçtiğinizde küresel bir hesapla birleştirmeye karar verirseniz, teşvikleri için bir kayıp olmaz, ancak bunun için bir gecikme olabilir. 

Teşvikleri programlarında yer alan tüm PMC hesaplarınızı taşımadıysanız, bu hesaplara bağlı teşvikleri kazanmanın durulabiliriz.

### <a name="what-are-the-incentive-roles-in-partner-center"></a>Iş Ortağı Merkezi 'nde teşvik rolleri nelerdir?

Iş Ortağı Merkezi 'ndeki rolleri, konum tabanlıdır ve teşvikleri admin ve teşvikleri User içerir. Bu rollerin ne yapabilecekleri hakkında daha fazla bilgi için bkz. [Kullanıcı rolleri ve Izinleri atama](permissions-overview.md).

### <a name="can-incentives-admins-be-assigned-at-the-global-and-location-level"></a>Teşvikleri yöneticileri genel ve konum düzeyinde atanabilir mi?

Evet. Bir teşvikleri yöneticisini tüm konumlar için teşvikleri Yöneticisi olacak şekilde atayabilirsiniz veya her konum kendi teşvikleri yöneticisine sahip olabilir.

### <a name="can-incentives-be-paid-at-the-global-or-location-level"></a>Teşvikleri genel veya konum düzeyinde ücretli olabilir mi?

Teşvikleri yalnızca konum düzeyinde ödemiştir.

### <a name="regarding-referrals-how-many-business-profiles-can-we-create"></a>Başvurularla ilgili olarak, kaç iş profili oluşturuyoruz?

Şirketiniz, şirketinizin ilgi alanlarınızı tam olarak göstermek için ihtiyaç duyduğunuz kadar çok iş profili oluşturabilir. Her iş profilinde, ülkeye göre tek bir konum olmak üzere en fazla beş konum listeleyebilirsiniz. İş profillerinin her biri, konumlarına her biri için başvurular alabilir.

### <a name="how-will-referrals-be-assigned-what-changes-can-i-expect-for-example-if-i-have-a-global-company-in-one-market-and-locations-in-other-markets-how-will-referrals-be-assigned"></a>Başvurular nasıl atanacaktır, hangi değişiklikleri beklemeliyim? Örneğin, bir Pazar ve diğer pazarlardaki konumlarda küresel bir şirketiniz varsa, nasıl başvuru atanır?

Başvurular, müşterinin tanımladığı arama parametrelerine göre atanır. Bir veya daha çok bir konuma sahip olup olmadığına bakılmaksızın, müşteri istenen bir konum belirtiyorsa ve diğer parametreleri karşılayan bir işletmeniz varsa, başvuru o konuma gider.

### <a name="i-am-migrating-to-partner-center-from-within-russia-i-get-an-error-message-about-web-direct-how-do-i-continue-with-the-migration"></a>Rusya içinden Iş Ortağı Merkezi 'ne geçirdim. Web Direct hakkında bir hata iletisi alıyorum. Nasıl yaparım? geçişe devam edilsin mi?

Web Direct programına katıldığınız için bir hata iletisi alırsanız, aşağıdaki adımları gerçekleştirin:

1. Portalda oturum açın. Azure.com Azure AD kiracısı oluşturun ve yeni bir kiracı oluşturun. Daha fazla bilgi için [yeni Bir Azure AD kiracısı oluşturma makalesi okuyun.](/azure/active-directory/fundamentals/active-directory-access-create-new-tenant)

2. Yeni Azure AD kiracısı oluşturduktan sonra bu kiracıyı kullanarak Partner Membership Center'İş Ortağı Merkezi'ye geçiş veya İş Ortağı Merkezi.