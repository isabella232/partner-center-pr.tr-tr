---
title: İş ortağı kiracınız için MFA'yı zorunlu tutma
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: İş ortağı kiracılarınız için Mandating MFA 'nın müşteri kaynaklarına erişiminizi güvenli hale getirmenize nasıl yardımcı olacağını öğrenin. Örnek senaryolar içerir.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 4a85a7e415eac7f54ccd52302e350ce20de9856d
ms.sourcegitcommit: 0cea15df24a6a1b310535eb1cb5e167dc2248a95
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/16/2020
ms.locfileid: "92531982"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>İş ortağı kiracınız için Mandating Multi-Factor Authentication (MFA)

**Uygulama hedefi**

- Bulut çözümü sağlayıcısı programındaki tüm iş ortakları
  - Doğrudan fatura
  - Dolaylı sağlayıcı
  - Dolaylı satıcı
- Tüm danışmanları

**Etkilenen roller**

- Yönetim Aracısı
- Satış Aracısı
- Yardım Masası Aracısı
- Faturalama yöneticisi
- Genel yönetici

Bu özelliğin amacı, iş ortaklarının, kimlik bilgilerinin güvenliğinin aşılmasına karşı müşteri kaynaklarına erişiminin güvenliğini sağlamaya yardımcı olmak.
İş ortakları, Konuk Kullanıcı da dahil olmak üzere iş ortağı kiracısındaki tüm Kullanıcı hesapları için Multi-Factor Authentication (MFA) zorlamak için gereklidir. Bu özellik, bu iş ortağı rollerinin aşağıdaki alanlarda MFA doğrulamasını tamamlaması için uygulanan olacaktır:

- [İş Ortağı Merkezi panosu](#partner-center-dashboard)
- [İş Ortağı Merkezi API’si](#partner-center-api)
- [Ortak temsilci yönetimi](#partner-delegated-administration)

Daha büyük ve sürekli güvenlik ve gizlilik korumaları, popüler önceliklerimiz arasında olduğundan iş ortaklarının müşterileri ve kiracılarını korumalarına yardımcı olmaya devam ediyoruz. Bulut çözümü sağlayıcısı (CSP) programına katılan tüm iş ortakları, Denetim Masası satıcıları (CPVs) ve danışmanları uyumlu kalmak için [Iş ortağı güvenlik gereksinimlerini](partner-security-requirements.md) uygulamalıdır.

Microsoft, iş ortağı kiracılar için ek güvenlik önlemlerinin etkinleştirilmesini başlamıştır. Bu korumalar etkinleştirildiğinde, iş ortaklarının kiracılarının ve müşterilerinin, yetkisiz erişimi önlemek için Mandating Multi-Factor Authentication (MFA) doğrulamasına göre Güvenliği sağlanmasına yardımcı olur.

İş ortağı tarafından sunulan yönetim olanaklarına yönelik etkinleştirmeyi tüm iş ortağı kiracılarına başarıyla tamamladınız. İş ortakları ve müşterilerin korunmasına daha fazla yardımcı olmak için, 1 Mayıs 2020 ' den itibaren, iş ortaklarının iş ve müşterilerinin kimlik hırsızlığı ile ilgili olaylardan korunmasına yardımcı olmak için CSP 'de Iş Ortağı Merkezi işlemlerine yönelik etkinleştirmeye başlayacağız.

Bu belge, güvenlik önlemlerinin etkinleştirilmesiyle ilgili ayrıntılı deneyim ve kılavuza sahip iş ortakları sağlar.

## <a name="partner-center-dashboard"></a>İş Ortağı Merkezi panosu

Iş Ortağı Merkezi panosundaki belirli sayfalar, aşağıdakiler dahil olmak üzere MFA korumalı olacaktır:

- **Müşteriler** sekmesinin altındaki tüm sayfalar, ÖRNEĞIN aşağıdaki URL aracılığıyla erişilebilen tüm sayfalar:https://partner.microsoft.com/commerce/*
- **Destek > müşteri istekleri** sekmesi altındaki tüm sayfalar, örneğin altında erişilen sayfahttps://partner.microsoft.com/dashboard/support/csp/customers/*
- Faturalandırma sayfası

Bu sayfalardan birine erişmeyi denerseniz ve MFA doğrulamasını daha önce tamamlamadıysanız bunu yapmanız gerekecektir.

> [!NOTE]
> Genel Bakış sayfası, hizmet durumu denetimi sayfası gibi Iş Ortağı Merkezi 'ndeki diğer sayfalar MFA korumalı olmayacaktır.

Aşağıdaki kullanıcı türleri, bu MFA korumalı sayfalara erişme yetkisine sahiptir ve bu nedenle bu özellikten etkilenir


| MFA korumalı sayfalar       | Yönetici aracıları      |  Satış aracıları     |   Yardım Masası aracıları     | Genel yönetici      |  Faturalama yöneticisi     | 
|---    |---    |---    |---    |---    |---    |
| Müşteriler sekmesi altındaki tüm sayfalar      |   x    |    x   |  x     |       |       |
| Destek > müşteri istekleri sekmesi altındaki tüm sayfalar     | x      |       |    x   |       |       |
| Faturalandırma sayfası     |   x    |       |       |    x   |   x    |

## <a name="examples-showing-how-verification-works"></a>Doğrulamanın nasıl çalıştığını gösteren örnekler

Doğrulamanın nasıl çalıştığını görmek için aşağıdaki iki örneği göz önünde bulundurun.

### <a name="example-1-partner-has-implemented-azure-ad-mfa"></a>Örnek 1: Iş ortağı Azure AD MFA uygulamış

1. Gamze, CSP Contoso için çalışmaktadır. Contoso, contoso iş ortağı kiracısı kapsamında Azure Active Directory (Azure AD) MFA kullanarak tüm kullanıcıları için MFA uygulamıştır.

2. Gamze yeni bir tarayıcı oturumu başlatır ve Iş Ortağı Merkezi panosuna genel bakış sayfasına gider (MFA korumalı değildir). İş Ortağı Merkezi, oturum açmak için Gamze 'yi Azure AD 'ye yönlendirir.

3. Contoso 'ya göre var olan Azure AD MFA kurulumu nedeniyle, MFA doğrulamasının tamamlanması için kemal gereklidir. Başarılı oturum açma ve MFA doğrulaması sonrasında, Gamze Iş Ortağı Merkezi panosuna genel bakış sayfasına yeniden yönlendirilir.

4. Gamze, Iş Ortağı Merkezi 'nde MFA korumalı sayfalardan birine erişmeyi dener. Gamze, daha önce oturum açma sırasında MFA doğrulamasını zaten tamamladığından, Gamze, MFA doğrulaması için gerekli olmadan MFA ile korunan sayfaya erişebilir.

### <a name="example-2-partner-has-implemented-third-party-mfa-using-identity-federation"></a>Örnek 2: Iş ortağı, Kimlik Federasyonu kullanarak üçüncü taraf MFA uygulamıştır

1. Nent, CSP Wingtip için geçerlidir. Wingtip, Kimlik Federasyonu aracılığıyla Azure AD ile tümleştirilmiş olan üçüncü taraf MFA kullanarak, Wingtip partner kiracısı kapsamındaki tüm kullanıcıları için MFA 'yı uygulamıştır.

2. Trent yeni bir tarayıcı oturumu başlatır ve Iş Ortağı Merkezi panosuna genel bakış sayfasına gider (MFA korumalı değildir). İş Ortağı Merkezi, oturum açmak için Azure AD 'ye yeniden yönlendirme sağlar.

3. Wingtip tarafından kurulum Kimlik Federasyonu olduğundan, Azure AD oturum açma ve MFA doğrulamasını gerçekleştirmek için federal kimlik sağlayıcısına yeniden yönlendirme yapın. Başarılı oturum açma ve MFA doğrulaması sonrasında, Trent Azure AD 'ye yeniden yönlendirilir ve sonra Iş Ortağı Merkezi panosuna genel bakış sayfasına yönlendirilir.

4. Trent, Iş Ortağı Merkezi 'nde MFA korumalı sayfalardan birine erişmeyi dener. Daha önce oturum açma sırasında MFA doğrulaması zaten tamamlanmış olduğundan, Trent MFA doğrulaması için gerekli olmadan MFA korumalı sayfasına erişebilir.

### <a name="example-3-partner-hasnt-implemented-mfa"></a>Örnek 3: ortak, MFA uygulanmamış

1. John, CSP Fabrikam için geçerlidir. Fabrikam, Fabrikam iş ortağı kiracısı kapsamındaki herhangi bir kullanıcı için MFA gerçekleştirmemiştir.

2. John yeni bir tarayıcı oturumu başlatır ve Iş Ortağı Merkezi panosuna genel bakış sayfasına gider (MFA korumalı değildir). İş Ortağı Merkezi John 'ı Azure AD 'ye yönlendirir ve oturum açın.

3. Fabrikam MFA uygulamadığından, John 'un MFA doğrulamasını tamamlaması gerekmez. John başarıyla oturum açtığında, John Iş Ortağı Merkezi panosuna genel bakış sayfasına yeniden yönlendirilir.

4. John, Iş Ortağı Merkezi 'nde MFA korumalı sayfalardan birine erişmeyi dener. John, MFA doğrulaması tamamlanmadığından, Iş Ortağı Merkezi John 'u Azure AD 'ye yönlendirdiğinden MFA doğrulamasını tamamlayacak. Bu ilk John 'un MFA 'yı tamamlaması gerektiğinde, John 'un de [MFA 'ya kaydolması](#mfa-registration-experience)istenir. MFA kayıt ve MFA doğrulaması başarılı olduğunda John, artık MFA korumalı sayfasına erişebilir.

5. Diğer bir gün, Fabrikam 'ın herhangi bir kullanıcı için MFA uygulamadan önce yeni bir tarayıcı oturumu başlatır ve Iş Ortağı Merkezi panosuna genel bakış sayfasına (MFA korumalı değildir) gider. İş Ortağı Merkezi John 'ı Azure AD 'ye yönlendirir ve MFA istemi olmadan oturum açın. 

6. John, Iş Ortağı Merkezi 'nde MFA korumalı sayfalardan birine erişmeyi dener. John, MFA doğrulaması tamamlanmadığından, Iş Ortağı Merkezi John 'u Azure AD 'ye yönlendirdiğinden MFA doğrulamasını tamamlayacak. John, MFA 'ya kaydolduğundan, bu kez yalnızca MFA doğrulamasının tamamlanabilmesi istenir.

> [!NOTE]
>Eylem: Şirket Yöneticisi, artık Iş Ortağı Merkezi tarafından önerilen [seçeneklerden](partner-security-requirements.md#actions-that-you-need-to-take) herhangi bırı aracılığıyla MFA 'yı uygulamalıdır.

## <a name="partner-center-api"></a>İş Ortağı Merkezi API’si

İş Ortağı Merkezi API 'SI yalnızca uygulama kimlik doğrulaması ve uygulama + kullanıcı kimlik doğrulamasını destekler. 

Uygulama + kullanıcı kimlik doğrulaması kullanıldığında, Iş Ortağı Merkezi MFA doğrulaması gerektirir. Daha belirgin olarak, bir iş ortağı uygulaması Iş Ortağı Merkezi 'ne API isteği göndermek istediğinde, isteğin yetkilendirme üstbilgisine bir erişim belirteci içermelidir. 

> [!NOTE]
>[Güvenli uygulama modeli](/partner-center/develop/enable-secure-app-model) , Iş Ortağı Merkezi API 'SINI çağırırken CSP iş ortaklarının ve cp'in Microsoft Azure MFA mimarisine göre kimlik doğrulamasına yönelik güvenli, ölçeklenebilir bir çerçevedir. KIRACıNıZDA MFA 'yı etkinleştirmeden önce bu uygulamayı uygulamanız gerekir. 

Iş Ortağı Merkezi, uygulama + kullanıcı kimlik doğrulaması kullanılarak elde edilen bir erişim belirtecine sahip bir API isteği aldığında, Iş Ortağı Merkezi API 'SI, *kimlik doğrulama yöntemi başvurusu (AMR)* talebinde *MFA* değeri olup olmadığını denetler. Bir erişim belirtecinin beklenen kimlik doğrulama yöntemi başvurusu (AMR) değerini içerip içermediğini doğrulamak için bir JWT kod çözücüsü kullanabilirsiniz:

``` csharp
{
  "aud": "https://api.partnercenter.microsoft.com",
  "iss": "https://sts.windows.net/df845f1a-7b35-40a2-ba78-6481de91f8ae/",
  "iat": 1549088552,
  "nbf": 1549088552,
  "exp": 1549092452,
  "acr": "1",
  "amr": [
    "pwd",
    "mfa"
  ],
  "appid": "23ec45a3-5127-4185-9eff-c8887839e6ab",
  "appidacr": "0",
  "family_name": "Adminagent",
  "given_name": "CSP",
  "ipaddr": "127.0.0.1",
  "name": "Adminagent CSP",
  "oid": "4988e250-5aee-482a-9136-6d269cb755c0",
  "scp": "user_impersonation",
  "tenant_region_scope": "NA",
  "tid": "df845f1a-7b35-40a2-ba78-6481de91f8ae",
  "unique_name": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "upn": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "ver": "1.0"
}
```

Değer varsa, Iş Ortağı Merkezi MFA doğrulamasının tamamlandığını ve API isteğini işler. Değer yoksa, Iş Ortağı Merkezi API 'SI aşağıdaki Yanıtla isteği reddeder:

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

App-Only kimlik doğrulaması kullanıldığında, App-Only kimlik doğrulamasını destekleyen API 'Ler MFA gerektirmeksizin sürekli olarak çalışır.

## <a name="partner-delegated-administration"></a>Ortak temsilci yönetimi

### <a name="using-service-portals"></a>Hizmet portalları kullanma

Yönetim aracıları ve yardım masası aracıları dahil iş ortağı hesapları, Microsoft Online Services portalları, komut satırı arabirimi (CLı) ve API 'Ler (uygulama + kullanıcı kimlik doğrulaması kullanarak) ile müşteri kaynaklarını yönetmek için Iş ortağı tarafından atanan yönetici ayrıcalıklarını kullanabilir.

Müşteri kaynaklarını yönetmek için Iş ortağı yönetici ayrıcalıkları (Şirket adına yönetici) kullanılarak Microsoft Online Services portallarına erişirken, bu portalların çoğu iş ortağı hesabının kimlik doğrulama bağlamı olarak ayarlanmış olan müşteri Azure Active Directory kiracı tarafından etkileşimli olarak kimlik doğrulaması yapmasını gerektirir. iş ortağı hesabı, müşteri kiracısında oturum açmak için gereklidir.

Azure Active Directory bu kimlik doğrulama isteklerini aldığında, iş ortağı hesabının MFA doğrulamasını tamamlaması gerekir. İş ortağı hesabının yönetilen veya federal bir kimlik olmasına bağlı olarak, iki olası kullanıcı deneyimi vardır:

- İş ortağı hesabı **yönetilen** bir kimlik ise, Azure Active Directory doğrudan kullanıcıdan MFA doğrulamasını tamamlamasını ister. İş ortağı hesabı daha önce Azure Active Directory MFA için kaydedilmemişse, kullanıcıdan önce [MFA kaydını tamamlaması](#mfa-registration-experience) istenir.

- İş ortağı hesabı bir **Federasyon** kimliği ise, deneyim iş ortağı yöneticisinin Azure Active Directory ' de Federasyonu nasıl yapılandırdığınıza bağlıdır. Azure Active Directory ' de Federasyon ayarlarken, iş ortağı Yöneticisi federal kimlik sağlayıcısının MFA 'yı destekleyip desteklemediğini Azure Active Directory gösterebilir. Bu durumda, Azure Active Directory MFA doğrulamasını tamamlaması için kullanıcıyı federal kimlik sağlayıcısına yönlendirir. Aksi takdirde, Azure Active Directory doğrudan kullanıcıdan MFA doğrulamasını tamamlamasını ister. İş ortağı hesabı daha önce Azure Active Directory MFA için kaydedilmemişse, kullanıcıdan önce [MFA kaydını tamamlaması](#mfa-registration-experience) istenir.

Genel deneyim, son müşteri kiracının yöneticileri için MFA uyguladığı senaryoya benzerdir. Örneğin, müşteri kiracısı, yönetici haklarına sahip tüm hesapların, yönetim aracıları ve yardım masası aracıları dahil olmak üzere MFA doğrulaması ile müşteri kiracısında oturum açmasını gerektiren [Azure AD güvenlik varsayılanlarını](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)etkinleştirdi. İş ortakları, test amacıyla müşteri kiracısında [Azure AD güvenlik varsayılanlarını](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) etkinleştirebilir ve ardından müşteri kiracıya erişmek Için iş ortağı tarafından atanan yönetim ayrıcalıklarını kullanmayı deneyebilir.

> [!NOTE]
> Tüm Microsoft Online hizmet portalları, iş ortağı yönetici ayrıcalıklarını kullanarak müşteri kaynaklarına erişirken müşteri kiracısında oturum açmak için iş ortağı hesapları gerektirmez. Bunun yerine, yalnızca iş ortağı hesaplarının iş ortağı kiracısında oturum açmasını gerektirir. Exchange Yönetim Merkezi bir örnektir. Zaman içinde, Iş ortaklarının yönetici ayrıcalıklarını kullanırken iş ortağı hesaplarının müşteri kiracısında oturum açmasını gerektirmemiz beklenir.

### <a name="using-service-apis"></a>Hizmet API 'Lerini kullanma

Bazı Microsoft Online Services API 'Leri (örneğin, Azure Resource Manager, Azure AD Graph, Microsoft Graph vb.), müşteri kaynaklarını programlı bir şekilde yönetmek için Iş ortağı tarafından yetkilendirilen yönetici ayrıcalıklarını kullanan iş ortaklarını destekler. Bu API 'lerle Iş ortağı tarafından atanan yönetim ayrıcalıklarına ulaşmak için iş ortağı uygulaması, API isteği yetkilendirme üst bilgisinde bir erişim belirteci içermelidir, bu da erişim belirtecinin, kimlik doğrulama bağlamı olarak Azure AD kümesi ile Azure AD ile kimlik doğrulaması yapmak için bir iş ortağı Kullanıcı hesabı olması gerekir. İş ortağı uygulamasının, müşteri kiracısında bir iş ortağı Kullanıcı hesabının oturum açması gerekir.

Azure AD, kimlik doğrulama isteği gibi aldığında, iş ortağı Kullanıcı hesabının MFA doğrulamasını tamamlaması gerekir. İş ortağı Kullanıcı hesabı daha önce MFA için kaydedilmemişse, önce Kullanıcı hesabının MFA kaydını tamamlaması istenir.

Ortak yönetici temsilcisi ayrıcalıkları kullanılarak bu API 'lerle tümleştirilen tüm iş ortağı uygulamaları bu özellikten etkilenir. İş ortağı uygulamalarının bu API 'lerle kesintiye uğramadan çalışmaya devam edememesini sağlamak için:

- İş ortağı, erişim belirtecini almak için Azure AD ile etkileşimli olmayan kullanıcı kimlik doğrulama yöntemi kullanmaktan kaçınmalıdır. [Parola akışı](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password)gibi etkileşimli olmayan kullanıcı kimlik doğrulama yöntemi kullanılırken, Azure AD kullanıcıdan MFA doğrulamasını tamamlamasını istemez. İş ortağı, bunun yerine [OpenID Connect Flow](/azure/active-directory/develop/v1-protocols-openid-connect-code) gibi etkileşimli kullanıcı kimlik doğrulama yöntemini kullanmaya bağlanmalıdır.

- Etkileşimli kullanıcı kimlik doğrulama yöntemi sırasında, iş ortağının MFA için zaten etkinleştirilmiş bir iş ortağı Kullanıcı hesabı kullanması gerekir. Alternatif olarak, Azure AD tarafından istendiğinde, iş ortağı, oturum açma sırasında MFA kaydını ve MFA doğrulamasını tamamlayabilir.

- Bu, bir son müşteri kiracının yöneticileri için MFA uyguladığı senaryoya benzerdir. Örneğin, müşteri kiracısı, yönetici haklarına sahip tüm Kullanıcı hesaplarının, yönetim aracıları ve yardım masası aracıları dahil olmak üzere MFA doğrulaması ile müşteri kiracısında oturum açmasını gerektiren [Azure AD güvenlik varsayılanlarını](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)etkinleştirdi. İş ortakları, test amacıyla müşteri kiracısında [Azure AD güvenlik varsayılanlarını](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) etkinleştirebilir ve ardından müşteri kiracıya programlı bir şekilde erişmek Için iş ortağı tarafından atanan yönetim ayrıcalıklarını kullanmayı deneyebilir.

### <a name="mfa-registration-experience"></a>MFA kayıt deneyimi

MFA doğrulaması sırasında, iş ortağı hesabı MFA için kayıtlı değilse, Azure AD kullanıcıdan önce MFA kaydını tamamlamasını ister:

:::image type="content" source="images/MfaRegistration1.png" alt-text="MFA kayıt adımı 1":::

**İleri** ' ye tıkladıktan sonra kullanıcıdan doğrulama yöntemlerinin bir listesinden seçmesi istenir.

:::image type="content" source="images/MfaRegistration2.png" alt-text="MFA kayıt adımı 1":::

Kayıt başarıyla tamamlandığında, Kullanıcı tarafından seçilen doğrulamaya göre MFA doğrulamasını tamamlaması gerekir.

## <a name="request-for-technical-exception"></a>Teknik özel durum isteği

İş ortakları, Microsoft Online Services ile ilgili teknik sorunlarla karşılaştıklarında ve uygun bir çözüm ya da geçici çözüm yoksa MFA doğrulamasını bastırmak için Teknik özel durum uygulayabilir. Bunu yapmadan önce aşağıdaki bölümleri gözden geçirin:

- [İş ortakları tarafından raporlanan yaygın sorunların listesi](#list-of-common-issues-reported-by-partners)
- [Teknik özel durum için istek gönderme](#how-to-submit-a-request-for-technical-exception)
 
### <a name="list-of-common-issues-reported-by-partners"></a>İş ortakları tarafından raporlanan yaygın sorunların listesi
Teknik özel durum için uygulamadan önce, diğer iş ortakları tarafından bildirilen yaygın sorunların listesini inceleyerek, Teknik özel durum için geçerli nedenler olup olmadığını anlayın.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>Sorun 1: Iş ortağının iş ortağı aracıları için MFA uygulaması daha fazla zaman gerektirir
İş ortağı başlatılmamış veya iş ortağı aracıları için, müşteri kaynaklarını yönetmek üzere Iş ortağı tarafından yetkilendirilen yönetim ayrıcalıklarını kullanarak Microsoft Online Services portallarına erişmesi gereken MFA uygulama işlemi hala devam ediyor. İş ortağının MFA uygulamasını tamamlaması daha fazla zaman gerektirir. Bu sorun, Teknik özel durum için geçerli bir neden mi?

**Cevap** : Hayır. İş ortağının, kesintiye uğramaması için kullanıcıları için MFA 'yı uygulamaya yönelik planlar yapması gerekir.

> [!NOTE]
> İş ortağı, iş ortağı aracıları için MFA uygulamamış olsa da, iş ortağı aracıları, müşteri kiracısında oturum açma sırasında istendiğinde MFA kaydını ve MFA doğrulamasını tamamlayabilecekleri için iş ortağı tarafından sunulan yönetim ayrıcalıklarını kullanarak Microsoft Online Services portallarına erişmeye devam edebilir. MFA kaydını tamamlamak, kullanıcıyı MFA için otomatik olarak etkinleştirmez.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>Sorun 2: Iş ortağı, temsilci yönetici ayrıcalıkları kullanmayan Kullanıcı hesapları için MFA uygulanmadı
Bir iş ortağı, iş ortağı kiracılarında, Iş ortağı tarafından verilen yönetim ayrıcalıklarını kullanarak müşteri kaynaklarını yönetmek için Microsoft Online Services portallarına erişim gerektirmeyen bazı kullanıcıları içerir. İş ortağı, bu kullanıcılar için MFA 'yı uygulama sürecinin yanı sıra daha fazla zaman tamamlaması gerekir. Bu sorun, Teknik özel durum için geçerli bir neden mi?

**Cevap** : Hayır. Bu Kullanıcı hesapları, müşteri kaynaklarını yönetmek için ortak Temsilcili yönetim ayrıcalıkları kullanmıyor olduğundan, müşteri kiracısında oturum açması gerekmez. Müşteri kiracısında oturum açma sırasında MFA doğrulaması gerektiren Azure AD tarafından etkilenmeyecektir.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>Sorun 3: Iş ortağı, Kullanıcı Hizmeti hesapları için MFA uygulanmadı
İş ortağı, iş ortağı kiracılarında cihazlar tarafından hizmet hesabı olarak kullanılan bazı kullanıcı hesaplarına sahip olur. Bunlar, Iş ortağı temsilcisi yönetim ayrıcalıklarını kullanarak müşteri kaynaklarını yönetmek için erişim Iş ortağı merkezi veya Microsoft Online Services portalları gerektirmeyen düşük ayrıcalıklı hesaplardır. Bu sorun, Teknik özel durum için geçerli bir neden mi?

**Cevap** : Hayır. Bu Kullanıcı hesapları, müşteri kaynaklarını yönetmek için ortak Temsilcili yönetim ayrıcalıkları kullanmıyor olduğundan, müşteri kiracısında oturum açması gerekmez. Müşteri kiracısında oturum açma sırasında MFA doğrulaması gerektiren Azure AD tarafından etkilenmeyecektir.

##### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>Sorun 4: Iş ortağı MS Authenticator uygulamasını kullanarak MFA uygulayamaz
Bir iş ortağı, kişisel mobil cihazlarını iş alanına getiren çalışanların çalışmasına izin verilmeyen "Temizleme masası" ilkesine sahiptir. Çalışanlar kişisel mobil cihazlarına erişim olmadan, Azure AD güvenlik Varsayılanları tarafından desteklenen tek MFA doğrulaması olan MS Authenticator uygulamasını yükleyemez. Bu sorun, Teknik özel durum için geçerli bir neden mi?

**Cevap** : Hayır, bu, Teknik özel durum için geçerli bir neden değil. İş ortağı aşağıdaki alternatifleri dikkate almalıdır, böylelikle çalışanlar Iş Ortağı Merkezi 'ne erişirken MFA doğrulamasını yine de tamamlayabilirler:
- İş ortağı Ayrıca, ek doğrulama yöntemleri sağlayabilen Azure AD Premium veya üçüncü taraf MFA çözümlerine (Azure AD ile uyumlu) kaydolabilir.

##### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>Sorun 5: Iş ortağı eski kimlik doğrulama protokollerinin kullanımı nedeniyle MFA uygulayamaz
Bir iş ortağı, hala, MFA uyumlu olmayan eski kimlik doğrulama protokollerini kullanan bazı iş ortakları aracılarıdır. Örneğin, kullanıcılar hala eski kimlik doğrulama protokollerini temel alan Outlook 2010 'yi kullanıyor. Bu iş ortağı aracılarında MFA etkinleştirildiğinde eski kimlik doğrulama protokollerinin kullanımı kesintiye uğracaktır.

**Cevap** : Hayır, bu, Teknik özel durum için geçerli bir neden değil. Bu protokollerin MFA doğrulaması ile korunamadığı ve kimlik bilgilerinin tehlikeye düşmesi açısından çok daha açıktır olması nedeniyle, iş ortaklarının eski kimlik doğrulama protokollerinin kullanılmasından uzaklaşması önemle önerilir. Eski kimlik doğrulama protokollerinin kullanımını tercih eden bir seçenek yoksa, iş ortakları, uygulama parolalarının kullanımını destekleyen Azure AD Premium için kaydolmayı düşünmelidir. Uygulama parolaları tek seferlik sistem tarafından oluşturulan parolalardır ve genellikle insan tarafından oluşturulan parolalardan daha güçlüdür. Uygulama parolalarını kullanarak, iş ortakları kullanıcıları için MFA uygulayabilir ve yalnızca eski kimlik doğrulama protokolleri için uygulama parolalarına geri dönebilir.

Outlook için eski kimlik doğrulamasını desteklemeye yönelik en son planı anlamak üzere [temel kimlik doğrulaması ve Exchange Online](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-auth-and-exchange-online-february-2020-update/ba-p/1191282) hakkındaki gönderiyi okuyun ve yaklaşan haberleri almak için [Exchange Ekibi blogunu](https://techcommunity.microsoft.com/t5/exchange-team-blog/bg-p/Exchange) izleyin. 

> [!NOTE]
> İş ortağı, iş ortağı aracıları için MFA uygulamamış olsa da, iş ortağı aracıları, müşteri kiracısında oturum açma sırasında istendiğinde MFA kaydını ve MFA doğrulamasını tamamlayabilecekleri için iş ortağı tarafından sunulan yönetim ayrıcalıklarını kullanarak Microsoft Online Services portallarına erişmeye devam edebilir. MFA kaydını tamamlamak, kullanıcıyı MFA için otomatik olarak etkinleştirmez.

##### <a name="issue-6-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>Sorun 6: Iş ortağı Azure AD tarafından tanınmayan üçüncü taraf MFA uygulamış
Bir iş ortağı, kullanıcıları için bir üçüncü taraf MFA çözümü kullanan MFA uygulamıştır. Bununla birlikte, iş ortağı, Kullanıcı kimlik doğrulaması sırasında MFA doğrulamasının tamamlandığı Azure AD 'ye geçiş yapmak için üçüncü taraf MFA çözümünü doğru şekilde yapılandıramadı. Bu, Teknik özel durum için geçerli bir neden mi?

**Cevap** : Evet, bu sorun Teknik özel durum için geçerli bir neden olarak düşünülebilir. Teknik özel durum için bir istek göndermeden önce, MFA çözümünün, Kullanıcı kimlik doğrulaması sırasında MFA doğrulamasının tamamlandığını göstermek üzere *authenticationmethodsreferences* talebini ( *multipleauthn* DEĞERI ile) Azure AD 'ye akışa almak üzere YAPıLANDıRıLAMADıĞıNı üçüncü taraf MFA çözüm sağlayıcısı ile doğrulayın. Teknik özel durum için bir istek gönderilirken, kullanılan üçüncü taraf MFA çözümünün ayrıntılarını sağlamanız ve tümleştirme yöntemini (Kimlik Federasyonu veya Azure AD özel denetimi aracılığıyla) belirtmeniz ve destekleyici belgeler olarak Teknik özel durum isteğinde aşağıdaki bilgileri sağlamanız gerekir:

- Üçüncü taraf MFA yapılandırması.

- Üçüncü taraf MFA etkin hesabıyla çalışan [Iş ortağı güvenlik gereksinimlerinin test](/powershell/partnercenter/test-partner-security-requirements) sonucu.

- Kullanmakta olduğunuz veya kullanmayı planladığınız üçüncü taraf MFA çözümünün satın alma siparişi.

### <a name="how-to-submit-a-request-for-technical-exception"></a>Teknik özel durum için istek gönderme

Teknik özel durum için bir istek göndermek için:

1. Iş Ortağı Merkezi 'nde genel yönetici veya yönetici Aracısı olarak oturum açın.

2. **Destek**  >  **ortağı destek isteklerini** ve **yeni istek** ' ı tıklayarak yeni bir iş ortağı hizmeti isteği oluşturun.

3. Arama kutusunda **özel durum Için MFA-istek** araması yapın; veya kategorisinden **CSP** ' yi seçin, sonra da **Hesap, ekleme, konudan erişim** ' i seçin, ardından alt konudan **özel durum için MFA-isteği** ' ni seçin ve ardından **İleri adım** ' ı seçin

4. Teknik özel durum için bir hizmet isteği göndermek için istenen ayrıntıları sağlayın ve **Gönder** ' e tıklayın.

Microsoft 'un Teknik özel durum isteğine yanıt vermesi için en fazla üç çalışma günü bulunabilir.