---
title: İş ortağı kiracınız için Mandating Multi-Factor Authentication (MFA)
ms.topic: article
ms.date: 10/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
description: İş ortağı kiracılarınız için Mandating MFA 'nın müşteri kaynaklarına erişiminizi güvenli hale getirmenize nasıl yardımcı olacağını öğrenin. Örnek senaryolar içerir.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: ba45c4c3d596c926bb6bfb8cf786e7e873c2a6c7
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114836736"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>İş ortağı kiracınız için Mandating Multi-Factor Authentication (MFA)

**Uygun roller**: yönetici Aracısı | Satış Aracısı | Yardım Masası Aracısı | Faturalandırma Yöneticisi | Genel yönetici

Bu makale, Iş Ortağı Merkezi 'nde Mandating Multi-Factor Authentication (MFA) için ayrıntılı örnekler ve kılavuzluk sağlar. Bu özelliğin amacı, iş ortaklarının, kimlik bilgilerinin güvenliğinin aşılmasına karşı müşteri kaynaklarına erişiminin güvenliğini sağlamaya yardımcı olmak. İş ortakları, Konuk kullanıcılar dahil olmak üzere iş ortağı kiracısındaki tüm Kullanıcı hesapları için MFA 'yı zorlamak için gereklidir. Kullanıcılar, aşağıdaki alanlarda MFA doğrulamasını tamamlamaya uygulanan olacaktır:

- [İş Ortağı Merkezi panosu](#partner-center-dashboard)
- [İş Ortağı Merkezi API’si](#partner-center-api)
- [Ortak temsilci yönetimi](#partner-delegated-administration)

Daha büyük ve sürekli güvenlik ve gizlilik korumaları, popüler önceliklerimiz arasında olduğundan iş ortaklarının müşterileri ve kiracılarını korumalarına yardımcı olmaya devam ediyoruz. Bulut Çözümü Sağlayıcısı (CSP) programına katılan tüm iş ortakları, denetim masası satıcıları (cpvs) ve danışmanların uyumlu kalması için [iş ortağı güvenlik gereksinimlerini](partner-security-requirements.md) uygulaması gerekir.

İş ortaklarının, işletmelerini ve müşterileri kimlik hırsızlığı ve yetkisiz erişimden korumalarına yardımcı olmak için, iş ortağı kiracılarına yönelik ek güvenlik korumalarını ve MFA 'yı doğrular. 

## <a name="partner-center-dashboard"></a>İş Ortağı Merkezi panosu

Iş Ortağı Merkezi panosundaki belirli sayfalar, aşağıdakiler dahil olmak üzere MFA korumalı olacaktır:

- **Müşteriler** sekmesinin altındaki tüm sayfalar, ÖRNEĞIN aşağıdaki URL aracılığıyla erişilebilen tüm sayfalar:https://partner.microsoft.com/commerce/*
- **Destek > müşteri istekleri** sekmesi altındaki tüm sayfalar, örneğin altında erişilen sayfahttps://partner.microsoft.com/dashboard/support/csp/customers/*
- Faturalandırma sayfası

Aşağıdaki tabloda, bu MFA ile korunan sayfalara hangi Kullanıcı türlerinin (ve bu özellikten etkilenildiği) erişme yetkisi verilmiştir.


| MFA korumalı sayfa       | Yönetici aracıları      |  Satış aracıları     |   Yardım Masası aracıları     | Genel yönetici      |  Faturalama yöneticisi     | 
|---    |---    |---    |---    |---    |---    |
| Müşteriler sekmesi altındaki tüm sayfalar      |   x    |    x   |  x     |       |       |
| Destek > müşteri istekleri sekmesi altındaki tüm sayfalar     | x      |       |    x   |       |       |
| Faturalandırma sayfası     |   x    |       |       |    x   |   x    |

Bu sayfalardan birine erişmeyi denerseniz ve MFA doğrulamasını daha önce tamamlamadıysanız bunu yapmanız gerekecektir. Genel Bakış sayfası, hizmet durumu denetimi sayfası gibi Iş ortağı merkezindeki diğer sayfalar MFA gerektirmez.

## <a name="verification-examples"></a>Doğrulama örnekleri

Iş Ortağı Merkezi panosunda doğrulamanın nasıl çalıştığını görmek için aşağıdaki örnekleri göz önünde bulundurun.

### <a name="example-1-partner-has-implemented-azure-ad-mfa"></a>Örnek 1: Iş ortağı Azure AD MFA uygulamış

1. Gamze, CSP Contoso için çalışmaktadır. contoso, contoso iş ortağı kiracısı kapsamında Azure Active Directory (Azure AD) mfa kullanarak tüm kullanıcıları için mfa uygulamıştır.

2. Gamze yeni bir tarayıcı oturumu başlatır ve Iş Ortağı Merkezi panosuna genel bakış sayfasına gider (MFA korumalı değildir). İş Ortağı Merkezi, oturum açmak için Gamze 'yi Azure AD 'ye yönlendirir.

3. Contoso 'ya göre var olan Azure AD MFA kurulumu nedeniyle, MFA doğrulamasının tamamlanması için kemal gereklidir. Başarılı oturum açma ve MFA doğrulaması sonrasında, Gamze Iş Ortağı Merkezi panosuna genel bakış sayfasına yeniden yönlendirilir.

4. Gamze, Iş Ortağı Merkezi 'nde MFA korumalı sayfalardan birine erişmeyi dener. Gamze, daha önce oturum açma sırasında MFA doğrulamasını zaten tamamladığından, Gamze, MFA doğrulaması için gerekli olmadan MFA ile korunan sayfaya erişebilir.

### <a name="example-2-partner-has-implemented-third-party-mfa-using-identity-federation"></a>Örnek 2: Iş ortağı, Kimlik Federasyonu kullanarak üçüncü taraf MFA uygulamıştır

1. Nent, CSP Wingtip için geçerlidir. Wingtip, Kimlik Federasyonu aracılığıyla Azure AD ile tümleştirilmiş olan üçüncü taraf MFA kullanarak, Wingtip partner kiracısı kapsamındaki tüm kullanıcıları için MFA 'yı uygulamıştır.

2. Trent yeni bir tarayıcı oturumu başlatır ve Iş Ortağı Merkezi panosuna genel bakış sayfasına gider (MFA korumalı değildir). İş Ortağı Merkezi, oturum açmak için Azure AD 'ye yeniden yönlendirme sağlar.

3. Wingtip tarafından kurulum Kimlik Federasyonu olduğundan, Azure AD oturum açma ve MFA doğrulamasını gerçekleştirmek için federal kimlik sağlayıcısına yeniden yönlendirme yapın. Başarılı oturum açma ve MFA doğrulamadan sonra, Azure AD 'ye yeniden yönlendirilir ve sonra Iş Ortağı Merkezi panosuna genel bakış sayfasına yönlendirilirsiniz.

4. Trent, Iş Ortağı Merkezi 'nde MFA korumalı sayfalardan birine erişmeyi dener. Daha önce oturum açma sırasında MFA doğrulaması zaten tamamlanmış olduğundan, Trent MFA doğrulaması için gerekli olmadan MFA korumalı sayfasına erişebilir.

### <a name="example-3-partner-hasnt-implemented-mfa"></a>Örnek 3: ortak, MFA uygulanmamış

1. John, CSP Fabrikam için geçerlidir. Fabrikam, Fabrikam iş ortağı kiracısı kapsamındaki herhangi bir kullanıcı için MFA gerçekleştirmemiştir.

2. John yeni bir tarayıcı oturumu başlatır ve Iş Ortağı Merkezi panosuna genel bakış sayfasına gider (MFA korumalı değildir). İş Ortağı Merkezi John 'ı Azure AD 'ye yönlendirir ve oturum açın.

3. Fabrikam MFA uygulamadığından, John 'un MFA doğrulamasını tamamlaması gerekmez. Oturum açma başarılı olduğunda John Iş Ortağı Merkezi panosuna genel bakış sayfasına yeniden yönlendirilir.

4. John, Iş Ortağı Merkezi 'nde MFA korumalı sayfalardan birine erişmeyi dener. John, MFA doğrulaması tamamlanmadığından, Iş Ortağı Merkezi John 'u Azure AD 'ye yönlendirdiğinden MFA doğrulamasını tamamlayacak. Bu ilk John 'un MFA 'yı tamamlaması gerektiğinde, John 'un de [MFA 'ya kaydolması](#mfa-registration-experience)istenir. MFA kayıt ve MFA doğrulaması başarılı olduğunda John, artık MFA korumalı sayfasına erişebilir.

5. Diğer bir gün, Fabrikam 'ın herhangi bir kullanıcı için MFA uygulamadan önce yeni bir tarayıcı oturumu başlatır ve Iş Ortağı Merkezi panosuna genel bakış sayfasına (MFA korumalı değildir) gider. İş Ortağı Merkezi John 'ı Azure AD 'ye yönlendirir ve MFA istemi olmadan oturum açın. 

6. John, Iş Ortağı Merkezi 'nde MFA korumalı sayfalardan birine erişmeyi dener. John, MFA doğrulaması tamamlanmadığından, Iş Ortağı Merkezi John 'u Azure AD 'ye yönlendirdiğinden MFA doğrulamasını tamamlayacak. John, MFA 'ya kaydolduğundan, bu kez yalnızca MFA doğrulamasının tamamlanabilmesi istenir.

> [!NOTE]
>Eylem: Şirket yöneticilerinin MFA 'yı uygulamak için [üç seçeneği](partner-security-requirements.md#implementing-multi-factor-authentication) vardır.

## <a name="partner-center-api"></a>İş Ortağı Merkezi API’si

Iş Ortağı Merkezi API 'SI yalnızca uygulama kimlik doğrulaması ve uygulama + kullanıcı kimlik doğrulamasını destekler. 

Uygulama + kullanıcı kimlik doğrulaması kullanıldığında, Iş Ortağı Merkezi MFA doğrulaması gerektirir. Daha belirgin olarak, bir iş ortağı uygulaması Iş Ortağı Merkezi 'ne API isteği göndermek istediğinde, isteğin yetkilendirme üstbilgisine bir erişim belirteci içermelidir. 

> [!NOTE]
>[güvenli uygulama modeli çerçevesi](/partner-center/develop/enable-secure-app-model) , iş ortağı merkezi apı 'lerini çağırırken Microsoft Azure MFA mimarisine göre CSP iş ortakları ve cp'leri kimlik doğrulamaya yönelik ölçeklenebilir bir çerçevedir. Kiracınızda MFA 'yı etkinleştirmeden önce bu çerçeveyi uygulamanız gerekir. 

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

Yönetim aracıları ve yardım masası aracıları dahil iş ortağı hesapları, Microsoft Online Services portalları, komut satırı arabirimi (CLı) ve API 'Ler (uygulama + kullanıcı kimlik doğrulaması kullanarak) ile müşteri kaynaklarını yönetmek için Iş ortağı tarafından atanan yönetici ayrıcalıklarını kullanabilir.

### <a name="using-service-portals"></a>Hizmet portalları kullanma

Müşteri kaynaklarını yönetmek için Iş ortağı yönetici ayrıcalıkları (Şirket adına yönetici) kullanılarak Microsoft Online Services portallarına erişirken, bu portalların çoğu iş ortağı hesabının kimlik doğrulama bağlamı olarak ayarlanmış olan müşteri Azure AD kiracısı tarafından etkileşimli olarak kimlik doğrulaması yapmasını gerektirir. iş ortağı hesabı, müşteri kiracısında oturum açmak için gereklidir.

Azure AD, bu tür kimlik doğrulama isteklerini aldığında, iş ortağı hesabının MFA doğrulamasını tamamlamaları gerekir. İş ortağı hesabının yönetilen veya federal bir kimlik olmasına bağlı olarak, iki olası kullanıcı deneyimi vardır:

- İş ortağı hesabı **yönetilen** bir kimlik Ise, Azure AD kullanıcıdan MFA doğrulamasını tamamlamasını ister. İş ortağı hesabı daha önce Azure AD ile MFA için kaydedilmemişse, kullanıcıdan önce [MFA kaydını tamamlaması](#mfa-registration-experience) istenir.

- İş ortağı hesabı bir **Federasyon** kimliği ise, deneyim iş ortağı YÖNETICISININ Azure AD 'de Federasyonu nasıl yapılandırdığınıza bağlıdır. Azure AD 'de Federasyon ayarlarken, iş ortağı Yöneticisi Azure AD 'ye federal kimlik sağlayıcısının MFA 'yı destekleyip desteklemediğini gösterebilir. Bu durumda, Azure AD, MFA doğrulamasını tamamlaması için kullanıcıyı federal kimlik sağlayıcısına yönlendirir. Aksi takdirde, Azure AD kullanıcıdan MFA doğrulamasını tamamlamayı doğrudan soracaktır. İş ortağı hesabı daha önce Azure AD'ye MFA'ya kayıtlı değilse, kullanıcıdan önce [MFA kaydını tamamlaması istenecek.](#mfa-registration-experience)

Genel deneyim, son müşteri kiracısı yöneticileri için MFA'nın uygulanmış olduğu senaryoya benzer. Örneğin, müşteri kiracısı [Yönetici](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)Aracıları ve Yardım Masası Aracıları dahil olmak üzere MFA doğrulaması ile müşteri kiracısına oturum açması için yönetici haklarına sahip tüm hesapların gerektirdiği Azure AD güvenlik varsayılanlarını etkinleştirdi. Test amacıyla, iş ortakları müşteri kiracısı içinde [Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) güvenlik varsayılanlarını etkinleştirebilir ve ardından müşteri kiracısına erişmek için İş Ortağı Temsilcisi Yönetim Ayrıcalıklarını kullanmayı deneyebilir.

> [!NOTE]
> Tüm Microsoft Online Service Portalları, İş Ortağı Temsilcisi Yönetici Ayrıcalıkları kullanarak müşteri kaynaklarına erişirken iş ortağı hesaplarının müşteri kiracısı içinde oturum açmasını gerektirmez. Bunun yerine, yalnızca iş ortağı hesaplarının iş ortağı kiracıda oturum açmasını gerektirir. Yönetim Merkezi'nin Exchange örneğidir. Zaman içinde, bu portalların İş Ortağı Temsilcisi Yönetici Ayrıcalıkları kullanırken iş ortağı hesaplarının müşteri kiracısına oturum açmasını gerektirmesi gerekir.

### <a name="using-service-apis"></a>Hizmet API'lerini kullanma

Bazı Microsoft Online Services API'leri (Azure Resource Manager, Azure AD Graph, Microsoft Graph vb.) iş ortaklarını, müşteri kaynaklarını program aracılığıyla yönetmek için İş Ortağı Temsilcisi Yönetici Ayrıcalıkları kullanarak destekler. İş Ortağı Temsilcisi Yönetici Ayrıcalıklarını bu API'lerle kullanmak için, iş ortağı uygulaması API isteği Yetkilendirme üst bilgisinde bir erişim belirteci içermesi gerekir. Burada erişim belirteci Azure AD ile kimlik doğrulaması yapmak için bir iş ortağı kullanıcı hesabına sahip olur ve müşteri Azure AD kimlik doğrulama bağlamı olarak ayarlanır. İş ortağı uygulamasının müşteri kiracısı için bir iş ortağı kullanıcı hesabıyla oturum açması gerekir.

Azure AD kimlik doğrulama isteği gibi bir yanıt aldığında Azure AD, MFA doğrulamasını tamamlamak için iş ortağı kullanıcı hesabı gerektirir. İş ortağı kullanıcı hesabı daha önce MFA'ya kayıtlı değilse, kullanıcı hesabından önce MFA kaydını tamamlaması istenir.

İş Ortağı Yönetici Temsilcisi Ayrıcalıkları kullanılarak bu API'lerle tümleştirilmiş tüm iş ortağı uygulamaları bu özellikten etkilenir. İş ortağı uygulamalarının kesinti olmadan bu API'lerle çalışmaya devam etmek için:

- İş ortağının erişim belirteci almak için Azure AD ile etkileşimli olmayan kullanıcı kimlik doğrulama yöntemini kullanmaktan kaçınması gerekir. Password [Flow](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password)gibi etkileşimli olmayan kullanıcı kimlik doğrulama yöntemi kullanılırken Azure AD, kullanıcıdan MFA doğrulamasını tamamlamasını isteminde olmayacaktır. İş ortağının bunun yerine OpenID gibi etkileşimli kullanıcı kimlik [doğrulama yöntemini Bağlan gerekir.](/azure/active-directory/develop/v1-protocols-openid-connect-code)

- Etkileşimli kullanıcı kimlik doğrulama yöntemi sırasında, iş ortağı MFA için zaten etkinleştirilmiş bir iş ortağı kullanıcı hesabı kullan olmalıdır. Alternatif olarak, Azure AD tarafından istendiğinde iş ortağı oturum açma sırasında MFA kaydını ve MFA doğrulamasını tamamlar.

- Bu, son müşteri kiracısı yöneticileri için MFA'nın uygulanmasına benzer. Örneğin, müşteri kiracısı [Yönetici](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)Aracıları ve Yardım Masası Aracıları dahil olmak üzere MFA doğrulaması ile müşteri kiracısına oturum açması için yönetici haklarına sahip tüm kullanıcı hesaplarının gerektirdiği Azure AD güvenlik varsayılanlarını etkinleştirdi. Test amacıyla, iş ortakları [müşteri](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) kiracısı içinde Azure AD güvenlik varsayılanlarını etkinleştirebilir ve ardından müşteri kiracısına programlı olarak erişmek için İş Ortağı Temsilcisi Yönetim Ayrıcalıkları kullanmayı deneyebilir.

### <a name="mfa-registration-experience"></a>MFA kayıt deneyimi

MFA doğrulaması sırasında, iş ortağı hesabı daha önce MFA'ya kayıtlı değilse Azure AD kullanıcıdan önce MFA kaydını tamamlaması istenir:

:::image type="content" source="images/MfaRegistration1.png" alt-text="MFA kaydı 1. adım.":::

Sonraki **seçeneğine** tıklanmasından sonra, kullanıcıdan doğrulama yöntemleri listesinden seçim seçmesi istenecek.

:::image type="content" source="images/MfaRegistration2.png" alt-text="MFA kaydı 2. adım.":::

Kayıt başarıyla tamamlandıktan sonra kullanıcının, kullanıcı tarafından seçilen doğrulamaya göre MFA doğrulamayı tamamlaması gerekir.
 
## <a name="list-of-common-issues"></a>Yaygın sorunların listesi

MFA [gereksiniminden teknik özel](#how-to-submit-a-request-for-technical-exception) durum için başvurmadan önce, isteğinizin geçerli olup olmadığını anlamak için diğer iş ortakları tarafından bildirilen yaygın sorunların listesini gözden geçirebilirsiniz.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>Sorun 1: İş ortağının iş ortağı aracıları için MFA'nın uygulanması için daha fazla zaman gerekiyor
İş ortağı henüz başlamadı veya müşteri kaynaklarını yönetmek için İş Ortağı Temsilcisi Yönetim Ayrıcalıkları kullanarak Microsoft Online Services Portallarına erişmesi gereken iş ortağı aracıları için MFA uygulama sürecindedir. İş ortağının MFA uygulamasını tamamlaması için daha fazla zaman gerekir. Bu sorun teknik özel durum için geçerli bir neden mi?

**Cevap:** Hayır. İş ortağının kesintiyi önlemek için kullanıcıları için MFA uygulama planları yapmaları gerekir.

> [!NOTE]
> İş ortağı, iş ortağı aracıları için MFA uygulamamış olsa da iş ortağı aracıları, müşteri kiracısına oturum açma sırasında istendiğinde MFA kaydını ve MFA doğrulamasını tamamlayabilecekleri şartıyla İş Ortağı Temsilcisi Yönetim Ayrıcalıklarını kullanarak Microsoft Online Services Portallarına erişmeye devam eder. MFA kaydının tamamlanması, kullanıcının MFA için otomatik olarak etkinleştirmez.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>Sorun 2: İş ortağı, Yönetici Ayrıcalıkları Temsilcisi kullanmayan kullanıcı hesapları için MFA uygulamadı
bir iş ortağının iş ortağı kiracılarında, İş Ortağı Temsilcisi Yönetim Ayrıcalıkları kullanarak müşteri kaynaklarını yönetmek için Microsoft Online Services Portallarına erişim gerektirmeyen bazı kullanıcıları vardır. İş ortağı bu kullanıcılar için MFA uygulama sürecindedir ve tamamlanması için daha fazla zaman gerekir. Bu sorun teknik özel durum için geçerli bir neden mi?

**Cevap:** Hayır. Bu kullanıcı hesapları müşteri kaynaklarını yönetmek için İş Ortağı Temsilcisi Yönetim Ayrıcalıkları kullanmayacaklarından, müşteri kiracılarında oturum açmaları gerekmez. Müşteri kiracısına oturum açma sırasında MFA doğrulaması gerektiren Azure AD'den etkilenmezler.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>Sorun 3: İş ortağı kullanıcı hizmeti hesapları için MFA uygulamadı
bir iş ortağının, iş ortağı kiracılarında cihazlar tarafından hizmet hesabı olarak kullanılan bazı kullanıcı hesapları vardır. Bunlar, İş Ortağı Temsilcisi Yönetim Ayrıcalıkları'İş Ortağı Merkezi müşteri kaynaklarını yönetmek için Microsoft Online Services Portallarına veya Microsoft Online Services Portallarına erişim gerektirmeyen düşük ayrıcalıklı hesaplardır. Bu sorun teknik özel durum için geçerli bir neden mi?

**Cevap:** Hayır. Bu kullanıcı hesapları müşteri kaynaklarını yönetmek için İş Ortağı Temsilcisi Yönetim Ayrıcalıkları kullanmayacaklarından, müşteri kiracılarında oturum açmaları gerekmez. Müşteri kiracısına oturum açma sırasında MFA doğrulaması gerektiren Azure AD'den etkilenmezler.

##### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>Sorun 4: İş ortağı MS Authenticator Uygulaması kullanarak MFA uygulayamaz
Bir iş ortağının, çalışanların kişisel mobil cihazlarını iş alanlarına getirmelerine izin vermeyen "temiz masa" ilkesi vardır. Çalışanlar, kişisel mobil cihazlarına erişim olmadan, Azure AD güvenlik varsayılanları tarafından desteklenen tek MFA doğrulaması olan MS Authenticator Uygulamasını yükleyemzamaz. Bu sorun teknik özel durum için geçerli bir neden mi?

**Cevap:** Hayır, bu teknik özel durum için geçerli bir neden değildir. İş ortağı aşağıdaki alternatifleri göz önünde İş Ortağı Merkezi:
- İş ortağı ayrıca ek doğrulama Azure AD Premium üçüncü taraf MFA çözümlerine (Azure AD ile uyumlu) kaydolabilirsiniz.

##### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>Sorun 5: İş ortağı eski kimlik doğrulama protokollerinin kullanımı nedeniyle MFA uygulayamaz
Bir iş ortağının hala MFA uyumlu olmayan eski kimlik doğrulama protokollerini kullanan bazı iş ortağı aracıları vardır. Örneğin, kullanıcılar hala eski kimlik doğrulama protokollerini Outlook 2010'da kullanıyor. Bu iş ortağı aracıları için MFA'nın etkinleştirilmesi, eski kimlik doğrulama protokollerinin kullanımını kesintiye neden olur.

**Cevap:** Hayır, bu teknik özel durum için geçerli bir neden değildir. Bu protokoller MFA doğrulamasıyla korunamaya ve kimlik bilgilerinin tehlikeye atlanmasına karşı çok daha duyarlı olduğundan, olası güvenlik etkileri nedeniyle iş ortaklarının eski kimlik doğrulama protokollerinin kullanımından uzak olması önemle tavsiye edilecektir. Eski kimlik doğrulama protokollerinin kullanımından uzaklaşan bir seçenek yoksa, iş ortaklarının Uygulama Parolaları kullanımını destekleyen Azure AD Premium için kaydolmayı göz önünde bulundurabilirsiniz. Uygulama Parolaları, sistem tarafından oluşturulan tek bir paroladır ve genellikle insan tarafından oluşturulan parolalardan daha güçlü olur. İş ortakları, Uygulama Parolalarını kullanarak kullanıcıları için MFA'yi uygulamaya alırken yalnızca eski kimlik doğrulama protokolleri için Uygulama Parolaları'ne geri döner.

Outlook için eski kimlik doğrulamasını [desteklemeye](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-auth-and-exchange-online-february-2020-update/ba-p/1191282) Exchange Online planı anlamak için Temel Kimlik Doğrulaması ve Exchange ile ilgili gönderiyi okuyun ve [Exchange ekip bloglarını](https://techcommunity.microsoft.com/t5/exchange-team-blog/bg-p/Exchange) takip edin. 

> [!NOTE]
> İş ortağı, iş ortağı aracıları için MFA uygulamamış olsa da iş ortağı aracıları, müşteri kiracısına oturum açma sırasında istendiğinde MFA kaydını ve MFA doğrulamasını tamamlayabilecekleri şartıyla İş Ortağı Temsilcisi Yönetim Ayrıcalıklarını kullanarak Microsoft Online Services Portallarına erişmeye devam eder. MFA kaydının tamamlanması, kullanıcının MFA için otomatik olarak etkinleştirmez.

##### <a name="issue-6-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>Sorun 6: İş ortağı Azure AD tarafından tanınmamış üçüncü taraf MFA'sı uygulamaya aldı
Bir iş ortağı, üçüncü taraf bir MFA çözümü kullanarak kullanıcıları için MFA uygulamaya aldı. Ancak iş ortağı, kullanıcı kimlik doğrulaması sırasında MFA doğrulamasının tamamlandıktan sonra Azure AD'ye geçiş yapmak için üçüncü taraf MFA çözümünü doğru yapılandıramaz. Bu teknik özel durum için geçerli bir neden mi?

**Cevap:** Evet, bu sorun teknik özel durum için geçerli bir neden olarak değerlendirebilir. Teknik özel durum isteği göndermeden önce, üçüncü taraf MFA çözüm sağlayıcısına MFA çözümünün *authenticationmethodsreferences* talebini *(multipleauthn* değeriyle) azure AD'ye akışla göndererek kullanıcı kimlik doğrulaması sırasında MFA doğrulamasının tamamlandıktan emin olun. Teknik özel durum isteği gönderme sırasında kullanılan üçüncü taraf MFA çözümünün ayrıntılarını sağlamanız ve tümleştirme yöntemini (örneğin kimlik federasyonu veya Azure AD Özel Denetimi kullanımı aracılığıyla) göstermeniz ve destek belgeleri olarak teknik özel durum isteğinde aşağıdaki bilgileri sağlamanız gerekir:

- Üçüncü taraf MFA yapılandırmaları.

- Üçüncü taraf MFA [etkin hesabı tarafından](/powershell/partnercenter/test-partner-security-requirements) çalışan İş Ortağı Güvenlik Gereksinimlerini Test Edin'in sonucu.

- Kullanmakta veya kullanmayı planlasanız üçüncü taraf MFA çözümünün satın alma siparişi.

## <a name="how-to-submit-a-request-for-technical-exception"></a>Teknik özel durum için istek gönderme

İş ortakları, Microsoft Online Services ile ilgili teknik sorunlarla karşılaşıyorsa ve uygulanabilir bir çözüm veya geçici çözüm yoksa, MFA doğrulamasını gizlemeye yönelik teknik özel durum için başvurabilir. Bunu yapmadan önce, [önceki bölümdeki yaygın sorunların](#list-of-common-issues) listesini gözden geçirebilirsiniz.

Teknik özel durum isteği göndermek için:

1. Genel Yönetici İş Ortağı Merkezi Yönetici Aracısı olarak oturum açma.

2. Destek İş Ortağı destek istekleri'ne giderek ve Yeni istek'i  >  **seçerek yeni** bir iş ortağı hizmet isteği **oluşturun.**

3. **MFA ara - Arama kutusunda özel** durum isteği; veya **Kategori'den CSP'yi** seçin, sonra **Hesaplar, Ekleme,** Konu başlığından Erişim'i ve ardından alt konu başlığından **MFA -** Özel durum isteği'yi seçin ve ardından sonraki **adımı seçin.**

4. Teknik özel durum için bir hizmet isteği göndermek için istenen ayrıntıları s sağlama ve Gönder'i **seçin.**

Microsoft'un teknik özel durum isteğine yanıt olarak sağlaması üç iş günü kadar zaman alır.

## <a name="next-steps"></a>Sonraki adımlar

 - [İş ortağı güvenlik gereksinimleri durumu](partner-security-compliance.md)