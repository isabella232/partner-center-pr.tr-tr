---
title: Iş ortağı üyeliği merkezinden taşıma
ms.topic: article
ms.date: 06/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: İşletmenizi iş ortağı üyeliği merkezinden iş ortağı merkezi 'ne taşımadan önce yararlı bilgileri ve sık sorulan soruları gözden geçirin.
author: parthpandyamsft
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: be4250864bd07e555b0eb2079c28f3dfb4920805
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/22/2020
ms.locfileid: "92531599"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Iş ortağı üyelik merkezinden (PMC) Iş Ortağı Merkezi 'ne geçiş için hazırlanma

**Uygun roller**
- Genel yönetici
- Kullanıcı yöneticisi
- Satış Aracısı
- Yönetim Aracısı

İş ilişkinizi Microsoft ile yönetmeye yönelik tek bir hedef olan iş ortağı üyelik Merkezi 'nden (PMC) üyelik yönetimini iş ortağı merkezi 'ne taşıdık. Iş Ortağı Merkezi 'ne taşınmanın mümkün olduğunca verimli ve kolay olmasını istiyoruz. Iş ortağı merkezinin PMC 'den farklı olduğu bazı bölümler belirledik ve taşımayı yapmadan önce bunları anlamak ve hazırlamak istediğinizi düşündük.

## <a name="account-and-identity-setup"></a>Hesap ve kimlik kurulumu

Hesap ve kimlik kurulumu hakkında sık sorulan sorulara yanıtlar için aşağıya bakın.

### <a name="what-is-an-azure-active-directory-azure-ad-work-account"></a>Azure Active Directory (Azure AD) iş hesabı nedir?

Azure iş hesabı, Azure genel bulutunda şirketinizin adanmış ve yalıtılmış bir sanal gösterimidir ve Azure, Microsoft Intune veya Office 365 gibi bir Microsoft bulut hizmetine abone olduğunuzda sizin için oluşturulur.

İş hesabınız, Azure AD kullanıcılarınızı ve bunlarla ilgili bilgileri (e-posta, parolalar, profil verileri, izinler vb.) barındırır. İş hesabı Ayrıca gruplar, uygulamalar ve bir şirketle ilgili ve güvenlikle ilgili diğer bilgileri de içerir. 

İş e-postanız Azure Active Directory kiracınızın bir parçasıdır. Iş Ortağı Merkezi 'nde bir hesaba sahip olmak için bir AAD Kiracınız olması gerekir. Azure Active Directory hakkında daha fazla bilgi için [Azure AD 'de dizininizi oluşturma](/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad)makalesini okuyun.

İş e-postanızı kullanarak kişisel e-postanız için hesabınızda oturum açmanız gerekir.

- İş hesabınız: john@contoso.com
- Kişisel hesabınız: John@outlook.com

### <a name="what-account-should-you-sign-into-partner-center-with-if-you-have-an-aad-tenant-with-microsoft-for-office-365-for-example-and-you-also-have-a-tenant-for-your-csp-business"></a>Microsoft ile bir AAD kiracınız varsa (örneğin, Office 365 için) ve ayrıca CSP işletmeniz için bir kiracınız varsa, Iş Ortağı Merkezi 'Nde oturum açmanız gereken hesap nedir?

Iş Ortağı Merkezi 'Nde CSP hesabı ya da MPN iş e-posta hesabınızla oturum açabilirsiniz. CSP iş e-postanızı kullanarak oturum açmayı seçerseniz, panonuzda sol gezinti, hem MPN hem de CSP program bilgilerini görüntüler. MPN Azure AD kiracısı iş e-postalarınız ile oturum açarsanız yalnızca MPN program bilgilerinizi görürsünüz. 

### <a name="if-you-dont-want-to-use-your-existing-office-365-azure-ad-tenant-for-partner-center-you-can-create-a-new-tenant-prior-to-migrating-from-pmc"></a>Iş Ortağı Merkezi için mevcut Office 365 Azure AD kiracınızı kullanmak istemiyorsanız, PMC 'den geçiş yapmadan önce yeni bir kiracı oluşturabilirsiniz.

Iş Ortağı Merkezi hesabınızı ayarlamak için mevcut bir Azure AD kiracısını kullanmak istememeniz pek çok nedeni olabilir. Iş Ortağı Merkezi 'ne geçiş yapmaya başlamadan önce, yeni bir Azure AD kiracısı oluşturmak için [Azure Portal](https://ms.portal.azure.com/#home) gidin. [Azure Active Directory yeni kiracı oluşturma](/azure/active-directory/develop/quickstart-create-new-tenant)bölümündeki yönergeleri izleyin. Iş Ortağı Merkezi hesabınızı ayarlamak için yeni AAD kiracısını kullanın. Kiracıyı oluşturmak için bir genel yönetici olmanız gerekir. 

### <a name="user-roles-including-guest-user-roles-in-partner-center"></a>Iş Ortağı Merkezi 'nde Konuk Kullanıcı rolleri dahil Kullanıcı rolleri

İş Ortağı Merkezi, yapılması gereken iş türlerine bağlı olarak farklı rol türlerine sahiptir. Azure AD rolleri olan genel yönetici gibi roller vardır. Bazı roller, bulut hizmeti sağlayıcısı programı veya teşvikleri gibi programlara özgüdür ve MPN 'ye özgü roller vardır. Tüm Iş Ortağı Merkezi rollerinin ne olduğunu öğrenmek için [Kullanıcı rolü rolleri ve izinleri](permissions-overview.md)oku makalesini okuyun.

### <a name="what-happens-to-my-users-roles-when-they-move-from-pmc-to-partner-center"></a>PMC 'den Iş Ortağı Merkezi 'ne geçtiğinde kullanıcılarınızın rollerine ne olur?

Geçiş işlerini yapan MPN genel yöneticisi veya birincil program ile ilgili kişi dışında, PMC 'deki tüm kullanıcılar yönetici rollerini kaybeder. Geçişi tamamlayan kişinin Iş Ortağı Merkezi 'ne rol ataması gerekir. Iş ortağı merkezindeki roller PMC 'deki rollerden farklıdır. Iş Ortağı Merkezi 'nde Kullanıcı rolleri hakkında daha fazla bilgi için bkz. [Kullanıcı rollerini ve izinlerini ata] (Permissions-overview.md ve [PMC 'Den Iş ortağı merkezine taşıma](move-pmc-pc-map.md#user-roles) .

### <a name="whats-the-difference-between-my-company-profile-and-my-business-profile"></a>Şirket profilimi ve iş profilim arasındaki fark nedir?

Şirket profiliniz, şirketiniz hakkında adres, konum, birincil kişi, banka ve vergi ayrıntılarını içeren bilgiler içerir.

İş profiliniz, kendinizi müşterilere sunma ve logonuzu, iş odağınızdaki ayrıntıları, uzmanlığınızı vb. görüntüleyen bir pazarlama sayfasıdır.

### <a name="what-does-account-consolidation-mean-for-my-account"></a>Hesabım için hesap birleştirme ne anlama geliyor?

Birden çok MPN hesabını Iş Ortağı Merkezi 'ne geçirmek için aynı Azure AD kiracısını kullanırsanız, sistem bunu otomatik olarak tanır ve hesaplarınızı birleştirmeniz istenir. Aynı Azure AD kiracısıyla ilişkilendirilmiş birden çok etki alanı olsa bile bu değer geçerlidir. 

Ayrı AAD kiracılarını kullanarak Iş Ortağı Merkezi 'ne geçişe yine de karar verebilirsiniz, ancak bu durum, uzmanlarınızın ve ek satın alma maliyetlerinizin yalıtılmış değerlendirmesiyle sonuçlanır. Hesap birleştirme hakkında daha fazla bilgi için [Şirket hesaplarınızı birleştirme](consolidate-accounts.md) konusunu okuyun

### <a name="if-i-have-multiple-aad-tenants-and-a-single-mpn-account-is-it-possible-to-link-them-in-partner-center"></a>Birden çok AAD kiracısın ve tek bir MPN hesabı varsa, bunları Iş Ortağı Merkezi 'nde bağlamak mümkün mü?

Evet, Iş Ortağı Merkezi 'nde birden çok Azure AD kiracıyı tek Iş Ortağı Merkezi hesabına bağlayabilirsiniz.
Hesap birleştirme hakkında daha fazla bilgi için [Şirket hesaplarınızı birleştirme](consolidate-accounts.md) konusunu okuyun

### <a name="are-there-restrictions-to-adding-multiple-azure-ad-tenants-to-a-single-partner-center-account"></a>Birden çok Azure AD kiracısın tek bir Iş Ortağı Merkezi hesabına eklenmesine yönelik kısıtlamalar var mı?

Azure AD kiracısı zaten mevcut bir Iş Ortağı Merkezi hesabıyla ilişkili ise, çok kiracılı özelliği kullanılarak yeni Iş Ortağı Merkezi hesaplarıyla ilişkilendirilemez. Bunu düşünmenin bir diğer yolu da, bir Azure AD kiracısı yalnızca bir Iş Ortağı Merkezi hesabıyla ilişkilendirilebilir, ancak bir Iş Ortağı Merkezi hesabına ilişkili birden fazla kiracı olabilir.

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Microsoft İş Ortağı Ağı (MPN) üyelik geçişi 

MPN üyelik geçişi hakkında sık sorulan sorulara yönelik aşağıdaki yanıtlara bakın.

### <a name="who-can-perform-the-move-from-pmc-to-partner-center"></a>PMC 'den Iş ortağı merkezine ne kadar geçiş yapabilir?

Şirketinizin MPN genel yöneticisi veya birincil program kişisi (Bu iki rol genellikle aynı kişi tarafından tutulur), taşımayı başlatabilir ve gerçekleştirebilir.

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

İş Ortağı Merkezi 'nde iş ortağı, iş hesapları ve Konuk Kullanıcı hesapları ekleyebilir ve bu, ortağın Azure AD kiracısında MPN Yöneticisi olduğu aynı kiracıdan MSA. İş ortağı birden çok Azure AD kiracısından genel yöneticiyse ve tüm bu kiracılar aynı Iş Ortağı Merkezi hesabıyla ilişkiliyse, iş ortağının tüm bu kiracılar genelinde, Visual Studio avantajları ve Azure kullanım tabanlı tahsislerine Kullanıcı eklemesine izin verilir.

Konuk kullanıcılara MPN Yöneticisi veya genel yönetici tarafından Visual Studio 'nun kullanım tabanlı abonelikleri atanabilse de Konuk kullanıcılar, MSA kullanarak Iş Ortağı Merkezi 'nde oturum açamaz. Ancak Konuk kullanıcılar, atanan avantajlarını doğrulamak ve kullanmak için Azure ve Visual Studio 'da oturum açabilir.

### <a name="how-should-we-manage-our-mcp-associations-and-our-partner-university-access"></a>MCP ilişkilerimizi ve Iş ortağı Üniversitesi erişimimizi nasıl yönetmeniz gerekir?

MCP ilişkilerinizden geçiş yapan hiçbir değişiklik yok. Ancak, Iş Ortağı Merkezi 'ne taşıdıktan sonra gelen yeni çalışanların Iş Ortağı Merkezi ile ilişkilendirilmesi gerekir. Mevcut kullanıcılar için tüm Iş ortağı Üniversitesi izinleriniz kalacak, ancak Iş ortağı University 'e nasıl erişecaklarına ilişkin bilgiler için yeni çalışanların [eğitim merkezine](https://partner.microsoft.com/training) gitmesi gerekir.

### <a name="how-do-i-view-mcp-information-once-i-move-to-partner-center"></a>Iş Ortağı Merkezi 'ne taşıdıktan sonra MCP bilgilerini Nasıl yaparım? görüntüleyin mi?

Panoda sol Gezinti alanındaki **Uzmanlıklar** ' ı seçin. **Uzmanlıklar** sayfasından yetenekler raporunu indirebilirsiniz. Yetenekler raporu, Iş ortağı merkezindeki Uzmanlıklar ve programlarla ilgili becerileri almış olan kullanıcılarınızı listeler. Kullanıcılarınız becerileri kazandıysanız ancak bu yetenekler, doğru çalıştığınız uzmanlarla ilgili değilse raporda listelenmez.

### <a name="are-customer-references-used-in-partner-center"></a>Müşteri başvuruları Iş Ortağı Merkezi 'nde mi kullanılıyor?

Hayır, Iş Ortağı Merkezi 'nde uzmanlığa gereksinimleri karşılamak için müşteri başvurularına gerek yoktur.

### <a name="will-partner-of-record-associations-move-to-partner-center"></a>Kayıt ilişkilerinin Iş Ortağı Merkezi 'ne taşınacaktır?

Evet, kayıt Iş ortağının bir değişikliği yoktur. [İş ortağı kimliğinizi müşterilerinize bağlama](/azure/billing/billing-partner-admin-link-started)hakkında daha fazla bilgi edinin.

### <a name="is-there-an-impact-to-incentives-because-of-the-move-to-partner-center"></a>Iş Ortağı Merkezi 'ne geçiş teşvikleri için bir etkisi var mı?

Hayır, siz hesabınızı birleştirmeden taşıdıysanız teşvikleri üzerinde hiçbir etkisi yoktur. İşletmenizde, PMC 'de birden çok hesap varsa ve iş ortağı Merkezi ' ne geçtiğinizde küresel bir hesapla birleştirmeye karar verirseniz, teşvikleri için bir kayıp olmaz, ancak bunun için bir gecikme olabilir. 

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

Başvurular, müşterinin tanımladığı arama parametrelerine göre atanır. Bir konumunuz veya çok fazla olsun, müşteriler istenen bir konum belirtiyorsa ve diğer parametreleri karşılayan bir işinize sahipseniz, başvuru o konuma gider.

### <a name="i-am-migrating-to-partner-center-from-within-russia-i-get-an-error-message-about-web-direct-how-do-i-continue-with-the-migration"></a>Rusya içinden Iş Ortağı Merkezi 'ne geçirdim. Web Direct hakkında bir hata iletisi alıyorum. Nasıl yaparım? geçişe devam edilsin mi?

Web doğrudan programına katıldığınız için bir hata iletisi alırsanız, aşağıdakileri yapmanız gerekir:

1. Portalda oturum açın. Azure.com ve yeni bir Azure AD kiracısı oluşturun. Daha fazla bilgi için [Yeni bir Azure AD kiracısı oluşturma](/azure/active-directory/fundamentals/active-directory-access-create-new-tenant)makalesini okuyun.

2. Yeni Azure AD kiracısını oluşturduktan sonra Iş ortağı üyeliği merkezinden Iş Ortağı Merkezi 'ne geçiş yapmak veya Iş Ortağı Merkezi 'nde bir net yeni olarak kaydetmek için kullanın.