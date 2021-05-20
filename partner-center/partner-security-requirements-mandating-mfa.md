---
title: İş ortağı kiracınız için Mandating Multi-Factor Authentication (MFA)
ms.topic: article
ms.date: 10/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: İş ortağı kiracılarınız için Mandating MFA 'nın müşteri kaynaklarına erişiminizi güvenli hale getirmenize nasıl yardımcı olacağını öğrenin. Örnek senaryolar içerir.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: b1b02967209ba36088b0c7bb7487428ab08b8a37
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152588"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>İş ortağı kiracınız için Mandating Multi-Factor Authentication (MFA)

**Uygun roller**: yönetici Aracısı | Satış Aracısı | Yardım Masası Aracısı | Faturalandırma Yöneticisi | Genel yönetici

Bu makale, Iş Ortağı Merkezi 'nde Mandating Multi-Factor Authentication (MFA) için ayrıntılı örnekler ve kılavuzluk sağlar. Bu özelliğin amacı, iş ortaklarının, kimlik bilgilerinin güvenliğinin aşılmasına karşı müşteri kaynaklarına erişiminin güvenliğini sağlamaya yardımcı olmak. İş ortakları, Konuk kullanıcılar dahil olmak üzere iş ortağı kiracısındaki tüm Kullanıcı hesapları için MFA 'yı zorlamak için gereklidir. Kullanıcılar, aşağıdaki alanlarda MFA doğrulamasını tamamlamaya uygulanan olacaktır:

- [İş Ortağı Merkezi panosu](#partner-center-dashboard)
- [İş Ortağı Merkezi API’si](#partner-center-api)
- [Ortak temsilci yönetimi](#partner-delegated-administration)

Daha büyük ve sürekli güvenlik ve gizlilik korumaları, popüler önceliklerimiz arasında olduğundan iş ortaklarının müşterileri ve kiracılarını korumalarına yardımcı olmaya devam ediyoruz. Bulut çözümü sağlayıcısı (CSP) programına, Denetim Masası satıcılarına (CPVs) ve danışmanlarına katılan tüm iş ortakları, uyumlu kalmak için [Iş ortağı güvenlik gereksinimlerini](partner-security-requirements.md) uygulamalıdır.

İş ortaklarının, işletmelerini ve müşterileri kimlik hırsızlığı ve yetkisiz erişimden korumalarına yardımcı olmak için, iş ortağı kiracılarına yönelik ek güvenlik korumalarını ve MFA 'yı doğrular. 

## <a name="partner-center-dashboard"></a>İş Ortağı Merkezi panosu

Iş Ortağı Merkezi panosundaki belirli sayfalar, aşağıdakiler dahil olmak üzere MFA korumalı olacaktır:

- **Müşteriler** sekmesinin altındaki tüm sayfalar, ÖRNEĞIN aşağıdaki URL aracılığıyla erişilebilen tüm sayfalar:https://partner.microsoft.com/commerce/*
- **Destek > müşteri istekleri** sekmesi altındaki tüm sayfalar, örneğin altında erişilen sayfahttps://partner.microsoft.com/dashboard/support/csp/customers/*
- Faturalandırma sayfası

Aşağıdaki tabloda, bu MFA ile korunan sayfalara hangi Kullanıcı türlerinin (ve bu özellikten etkilenildiği) erişme yetkisi verilmiştir.


| MFA korumalı sayfa       | Yönetici aracıları      |  Satış temsilcileri     |   Yardım masası aracıları     | Genel yönetici      |  Faturalama yöneticisi     | 
|---    |---    |---    |---    |---    |---    |
| Müşteriler sekmesinin altındaki tüm sayfalar      |   x    |    x   |  x     |       |       |
| Destek ve Müşteri > altındaki tüm sayfalar     | x      |       |    x   |       |       |
| Faturalandırma sayfası     |   x    |       |       |    x   |   x    |

Bu sayfalardan herhangi bir'a erişmeyi dener ve daha önce MFA doğrulamayı tamamladıysanız, bunu yapmak zorunda oluruz. Genel bakış İş Ortağı Merkezi, Hizmet Durumu denetim sayfası gibi sayfalarda MFA gerekli değildir.

## <a name="verification-examples"></a>Doğrulama örnekleri

Doğrulamanın İş Ortağı Merkezi nasıl çalıştığını göstermek için aşağıdaki örnekleri göz önünde bulundurabilirsiniz.

### <a name="example-1-partner-has-implemented-azure-ad-mfa"></a>Örnek 1: İş ortağı Azure AD MFA'sı uygulamaya alındı

1. Jane, Contoso CSP'de çalışıyor. Contoso, Azure Active Directory (Azure AD) MFA'sı kullanarak Contoso iş ortağı kiracısı altındaki tüm kullanıcıları için MFA'ya sahip oldu.

2. Jane yeni bir tarayıcı oturumu başlatır ve İş Ortağı Merkezi panoya genel bakış sayfasına (MFA korumalı değildir) gidin. İş Ortağı Merkezi, Jane'i oturum açması için Azure AD'ye yeniden yönlendirer.

3. Contoso tarafından mevcut Azure AD MFA kurulumu nedeniyle Jane'in MFA doğrulamayı tamamlaması gerekir. Başarılı oturum açma ve MFA doğrulamasının ardından Jane, panoya İş Ortağı Merkezi sayfasına yeniden yönlendirildi.

4. Jane, MFA korumalı sayfalardan bir veritabanına erişmeye İş Ortağı Merkezi. Jane daha önce oturum açma sırasında MFA doğrulamasını zaten tamamlamış olduğu için, Jane yeniden MFA doğrulamasından geçerek MFA korumalı sayfaya erişebilirsiniz.

### <a name="example-2-partner-has-implemented-third-party-mfa-using-identity-federation"></a>Örnek 2: İş ortağı kimlik federasyonu kullanarak üçüncü taraf MFA'sı uygulamaya aldı

1. Trent, CSP Wingtip için çalışır. Wingtip, kimlik federasyonu aracılığıyla Azure AD ile tümleştirilmiş üçüncü taraf MFA kullanarak Wingtip iş ortağı kiracısı altındaki tüm kullanıcıları için MFA'ya sahip oldu.

2. Trent yeni bir tarayıcı oturumu başlatır ve İş Ortağı Merkezi panoya genel bakış sayfasına (MFA korumalı değildir) gidin. İş Ortağı Merkezi için Trent'i Azure AD'ye yeniden yönlendirin.

3. Wingtip'te kimlik federasyonu ayarlandıktan sonra Azure AD, Oturum açma ve MFA doğrulamasını tamamlamak için Trent'i federasyon kimlik sağlayıcısına yeniden yönlendirmektedir. Başarılı oturum açma ve MFA doğrulamasının ardından, Trent Azure AD'ye geri ve ardından panoya İş Ortağı Merkezi sayfasına yeniden yönlendirildi.

4. Trent, İş Ortağı Merkezi'daki MFA korumalı sayfalardan İş Ortağı Merkezi. Daha önce oturum açma sırasında Trent MFA doğrulamasını zaten tamamlamış olduğu için, Trent MFA korumalı sayfasına MFA doğrulamasını yeniden yapmak zorunda kalmadan erişebilirsiniz.

### <a name="example-3-partner-hasnt-implemented-mfa"></a>Örnek 3: İş ortağı MFA uygulamadı

1. John, CSP Fabrikam'da çalışıyor. Fabrikam, Fabrikam iş ortağı kiracısı altındaki hiçbir kullanıcı için MFA uygulamadı.

2. John yeni bir tarayıcı oturumu başlatır ve İş Ortağı Merkezi panosuna genel bakış sayfasına (MFA korumalı değildir) gidin. İş Ortağı Merkezi, John'u oturum açması için Azure AD'ye yeniden yönlendirer.

3. Fabrikam MFA uygulamamış olduğu için John'un MFA doğrulamayı tamamlaması gerekmez. Oturum başarıyla oturum açmanın ardından John panoya genel bakış İş Ortağı Merkezi yeniden yönlendirildi.

4. John, bir MFA korumalı sayfadan bir veritabanına erişmeye İş Ortağı Merkezi. John MFA doğrulamayı tamamlamamış olduğu için İş Ortağı Merkezi, MFA doğrulamayı tamamlamak için John'u Azure AD'ye yeniden yönlendirmektedir. Bu, John'un MFA'nın ilk kez tamamlanması gerektiğinden, John'dan [MFA'ya kaydolması da istenmektedir.](#mfa-registration-experience) Başarılı bir MFA kaydı ve MFA doğrulamasının ardından John artık MFA korumalı sayfasına erişebilirsiniz.

5. Fabrikam'ın herhangi bir kullanıcı için MFA uygulamadan bir gün önce, John yeni bir tarayıcı oturumu başlatır ve İş Ortağı Merkezi panoya genel bakış sayfasına (MFA korumalı değildir) gidin. İş Ortağı Merkezi John 'ı Azure AD 'ye yönlendirir ve MFA istemi olmadan oturum açın. 

6. John, Iş Ortağı Merkezi 'nde MFA korumalı sayfalardan birine erişmeyi dener. John, MFA doğrulaması tamamlanmadığından, Iş Ortağı Merkezi John 'u Azure AD 'ye yönlendirdiğinden MFA doğrulamasını tamamlayacak. John, MFA 'ya kaydolduğundan, bu kez yalnızca MFA doğrulamasının tamamlanabilmesi istenir.

> [!NOTE]
>Eylem: Şirket yöneticilerinin MFA 'yı uygulamak için [üç seçeneği](partner-security-requirements.md#implementing-multi-factor-authentication) vardır.

## <a name="partner-center-api"></a>İş Ortağı Merkezi API’si

Iş Ortağı Merkezi API 'SI yalnızca uygulama kimlik doğrulaması ve uygulama + kullanıcı kimlik doğrulamasını destekler. 

Uygulama + kullanıcı kimlik doğrulaması kullanıldığında, Iş Ortağı Merkezi MFA doğrulaması gerektirir. Daha belirgin olarak, bir iş ortağı uygulaması Iş Ortağı Merkezi 'ne API isteği göndermek istediğinde, isteğin yetkilendirme üstbilgisine bir erişim belirteci içermelidir. 

> [!NOTE]
>[Güvenli uygulama modeli çerçevesi](/partner-center/develop/enable-secure-app-model) , Iş Ortağı Merkezi API 'lerini ÇAĞıRıRKEN Microsoft Azure MFA MIMARISINE göre CSP iş ortakları ve CP'leri kimlik doğrulamaya yönelik ölçeklenebilir bir çerçevedir. Kiracınızda MFA 'yı etkinleştirmeden önce bu çerçeveyi uygulamanız gerekir. 

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

Yönetici Aracıları ve Yardım Masası Aracıları dahil olmak üzere iş ortağı hesapları, Microsoft Online Services Portalları, komut satırı arabirimi (CLI) ve API'ler (App+User kimlik doğrulamasını kullanarak) aracılığıyla müşteri kaynaklarını yönetmek için İş Ortağı Temsilci Yönetici Ayrıcalıklarını kullanabilir.

### <a name="using-service-portals"></a>Hizmet portallarını kullanma

Müşteri kaynaklarını yönetmek için İş Ortağı Tarafından Temsilci Olarak Yönetici Ayrıcalıkları (Yönetici-Adına) kullanılarak Microsoft Online Services Portallarına erişilirken, bu portalların çoğu müşteri Azure AD kiracısı kimlik doğrulama bağlamı olarak ayarlanmış şekilde etkileşimli olarak kimlik doğrulaması yapmak için iş ortağı hesabının kimlik doğrulamasını gerektirir. İş ortağı hesabının müşteri kiracıda oturum açması gerekir.

Azure AD bu tür kimlik doğrulama isteklerini aldığında, iş ortağı hesabının MFA doğrulamasını tamamlamasını gerektirir. İş ortağı hesabının yönetilen mi yoksa federasyon kimliği mi olduğuna bağlı olarak iki olası kullanıcı deneyimi vardır:

- İş ortağı hesabı yönetilen bir **kimlikse** Azure AD doğrudan kullanıcıdan MFA doğrulamayı tamamlaması istenir. İş ortağı hesabı daha önce Azure AD'ye MFA'ya kayıtlı değilse, kullanıcıdan önce [MFA kaydını tamamlaması istenecek.](#mfa-registration-experience)

- İş ortağı hesabı bir **federasyon kimliği ise** deneyim, iş ortağı yöneticisinin Azure AD'de federasyonu nasıl yapılandırmış olduğuna bağlıdır. Azure AD'de federasyon ayarlarken, iş ortağı yöneticisi Azure AD'ye federasyon kimlik sağlayıcısının MFA'ya destek olup olmadığını belirtebilirsiniz. Öyleyse Azure AD, MFA doğrulamayı tamamlamak için kullanıcıyı federasyon kimlik sağlayıcısına yeniden yönlendirecek. Aksi takdirde, Azure AD doğrudan kullanıcıdan MFA doğrulamayı tamamlaması istenir. İş ortağı hesabı daha önce Azure AD'ye MFA'ya kayıtlı değilse, kullanıcıdan önce [MFA kaydını tamamlaması istenecek.](#mfa-registration-experience)

Genel deneyim, son müşteri kiracısı yöneticileri için MFA'nın uygulanmış olduğu senaryoya benzer. Örneğin, müşteri kiracısı, yönetici haklarına sahip tüm hesapların, yönetim aracıları ve yardım masası aracıları dahil olmak üzere MFA doğrulaması ile müşteri kiracısında oturum açmasını gerektiren [Azure AD güvenlik varsayılanlarını](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)etkinleştirdi. İş ortakları, test amacıyla müşteri kiracısında [Azure AD güvenlik varsayılanlarını](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) etkinleştirebilir ve ardından müşteri kiracıya erişmek Için iş ortağı tarafından atanan yönetim ayrıcalıklarını kullanmayı deneyebilir.

> [!NOTE]
> Tüm Microsoft Online hizmet portalları, iş ortağı yönetici ayrıcalıklarını kullanarak müşteri kaynaklarına erişirken müşteri kiracısında oturum açmak için iş ortağı hesapları gerektirmez. Bunun yerine, yalnızca iş ortağı hesaplarının iş ortağı kiracısında oturum açmasını gerektirir. Exchange Yönetim Merkezi bir örnektir. Zaman içinde, Iş ortaklarının yönetici ayrıcalıklarını kullanırken iş ortağı hesaplarının müşteri kiracısında oturum açmasını gerektirmemiz beklenir.

### <a name="using-service-apis"></a>Hizmet API 'Lerini kullanma

Bazı Microsoft Online Services API 'Leri (örneğin, Azure Resource Manager, Azure AD Graph, Microsoft Graph vb.), müşteri kaynaklarını programlı bir şekilde yönetmek için Iş ortağı tarafından yetkilendirilen yönetici ayrıcalıklarını kullanan iş ortaklarını destekler. Iş ortağı yönetici ayrıcalıklarını bu API 'lerle birlikte kullanmak için, iş ortağı uygulaması, kimlik doğrulama bağlamı olarak Azure AD kümesi ile Azure AD ile kimlik doğrulaması yapmak için bir iş ortağı Kullanıcı hesabı sunarak, API isteği yetkilendirme üst bilgisinde erişim belirteci içermelidir. İş ortağı uygulamasının, müşteri kiracısında bir iş ortağı Kullanıcı hesabının oturum açması gerekir.

Azure AD, kimlik doğrulama isteği gibi aldığında, iş ortağı Kullanıcı hesabının MFA doğrulamasını tamamlaması gerekir. İş ortağı Kullanıcı hesabı daha önce MFA için kaydedilmemişse, önce Kullanıcı hesabının MFA kaydını tamamlaması istenir.

Ortak yönetici temsilcisi ayrıcalıkları kullanılarak bu API 'lerle tümleştirilen tüm iş ortağı uygulamaları bu özellikten etkilenir. İş ortağı uygulamalarının bu API 'lerle kesintiye uğramadan çalışmaya devam edememesini sağlamak için:

- İş ortağı, erişim belirtecini almak için Azure AD ile etkileşimli olmayan kullanıcı kimlik doğrulama yöntemi kullanmaktan kaçınmalıdır. [Parola akışı](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password)gibi etkileşimli olmayan kullanıcı kimlik doğrulama yöntemi kullanılırken, Azure AD kullanıcıdan MFA doğrulamasını tamamlamasını istemez. İş ortağı, bunun yerine [OpenID Connect Flow](/azure/active-directory/develop/v1-protocols-openid-connect-code) gibi etkileşimli kullanıcı kimlik doğrulama yöntemini kullanmaya bağlanmalıdır.

- Etkileşimli kullanıcı kimlik doğrulama yöntemi sırasında, iş ortağının MFA için zaten etkinleştirilmiş bir iş ortağı Kullanıcı hesabı kullanması gerekir. Alternatif olarak, Azure AD tarafından istendiğinde, iş ortağı, oturum açma sırasında MFA kaydını ve MFA doğrulamasını tamamlayabilir.

- Bu, bir son müşteri kiracının yöneticileri için MFA uyguladığı senaryoya benzerdir. Örneğin, müşteri kiracısı, yönetici haklarına sahip tüm Kullanıcı hesaplarının, yönetim aracıları ve yardım masası aracıları dahil olmak üzere MFA doğrulaması ile müşteri kiracısında oturum açmasını gerektiren [Azure AD güvenlik varsayılanlarını](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)etkinleştirdi. İş ortakları, test amacıyla müşteri kiracısında [Azure AD güvenlik varsayılanlarını](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) etkinleştirebilir ve ardından müşteri kiracıya programlı bir şekilde erişmek Için iş ortağı tarafından atanan yönetim ayrıcalıklarını kullanmayı deneyebilir.

### <a name="mfa-registration-experience"></a>MFA kayıt deneyimi

MFA doğrulaması sırasında, iş ortağı hesabı MFA için kayıtlı değilse, Azure AD kullanıcıdan önce MFA kaydını tamamlamasını ister:

:::image type="content" source="images/MfaRegistration1.png" alt-text="MFA kayıt adımı 1":::

**İleri**' ye tıkladıktan sonra kullanıcıdan doğrulama yöntemlerinin bir listesinden seçmesi istenir.

:::image type="content" source="images/MfaRegistration2.png" alt-text="MFA kayıt adımı 2":::

Kayıt başarıyla tamamlandığında, Kullanıcı tarafından seçilen doğrulamaya göre MFA doğrulamasını tamamlaması gerekir.
 
## <a name="list-of-common-issues"></a>Yaygın sorunların listesi

MFA gereksiniminden [Teknik özel duruma](#how-to-submit-a-request-for-technical-exception) uygulamadan önce, isteğinizin geçerli olup olmadığını anlamak için diğer iş ortakları tarafından raporlanan yaygın sorunların listesini gözden geçirin.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>Sorun 1: Iş ortağının iş ortağı aracıları için MFA uygulaması daha fazla zaman gerektirir
bir iş ortağı, müşteri kaynaklarını yönetmek için İş Ortağı Temsilcisi Yönetim Ayrıcalıkları kullanarak Microsoft Online Services Portallarına erişmesi gereken iş ortağı aracıları için MFA'nın uygulanmasına henüz başlamadı veya hala devam ediyor. İş ortağının MFA uygulamasını tamamlaması için daha fazla zaman gerekir. Bu sorun teknik özel durum için geçerli bir neden mi?

**Cevap:** Hayır. İş ortağının kesintiyi önlemek için kullanıcıları için MFA uygulama planları yapmaları gerekir.

> [!NOTE]
> İş ortağı, iş ortağı aracıları için MFA uygulamamış olsa da iş ortağı aracıları, müşteri kiracısına oturum açma sırasında istendiğinde MFA kaydını ve MFA doğrulamasını tamamlayabilecekleri şartıyla İş Ortağı Temsilcisi Yönetim Ayrıcalıklarını kullanarak Microsoft Online Services Portallarına erişmeye devam eder. MFA kaydının tamamlanması, kullanıcının MFA için otomatik olarak etkinleştirmez.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>Sorun 2: İş ortağı, Yönetici Ayrıcalıkları Temsilcisi kullanmayan kullanıcı hesapları için MFA uygulamadı
bir iş ortağının iş ortağı kiracılarında, İş Ortağı Temsilcisi Yönetim Ayrıcalıkları kullanarak müşteri kaynaklarını yönetmek için Microsoft Online Services Portallarına erişim gerektirmeyen bazı kullanıcıları vardır. İş ortağı bu kullanıcılar için MFA uygulama sürecindedir ve tamamlanması için daha fazla zaman gerekir. Bu sorun teknik özel durum için geçerli bir neden mi?

**Cevap:** Hayır. Bu kullanıcı hesapları müşteri kaynaklarını yönetmek için İş Ortağı Temsilcisi Yönetim Ayrıcalıkları kullanmayacaklarından, müşteri kiracısı için oturum açmaları gerekmez. Bunlar, müşteri kiracısına oturum açma sırasında MFA doğrulaması gerektiren Azure AD'den etkilenmez.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>Sorun 3: İş ortağı kullanıcı hizmeti hesapları için MFA uygulamadı
bir iş ortağının, iş ortağı kiracılarında cihazlar tarafından hizmet hesabı olarak kullanılan bazı kullanıcı hesapları vardır. Bunlar, İş Ortağı Temsilcisi Yönetim Ayrıcalıkları'İş Ortağı Merkezi müşteri kaynaklarını yönetmek için Microsoft Online Services Portallarına veya Microsoft Online Services Portallarına erişim gerektirmeyen düşük ayrıcalıklı hesaplardır. Bu sorun teknik özel durum için geçerli bir neden mi?

**Cevap:** Hayır. Bu Kullanıcı hesapları, müşteri kaynaklarını yönetmek için ortak Temsilcili yönetim ayrıcalıkları kullanmıyor olduğundan, müşteri kiracısında oturum açması gerekmez. Müşteri kiracısında oturum açma sırasında MFA doğrulaması gerektiren Azure AD tarafından etkilenmeyecektir.

##### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>Sorun 4: Iş ortağı MS Authenticator uygulamasını kullanarak MFA uygulayamaz
Bir iş ortağı, kişisel mobil cihazlarını iş alanına getiren çalışanların çalışmasına izin verilmeyen "Temizleme masası" ilkesine sahiptir. Çalışanlar kişisel mobil cihazlarına erişim olmadan, Azure AD güvenlik Varsayılanları tarafından desteklenen tek MFA doğrulaması olan MS Authenticator uygulamasını yükleyemez. Bu sorun, Teknik özel durum için geçerli bir neden mi?

**Cevap**: Hayır, bu, Teknik özel durum için geçerli bir neden değil. İş ortağı aşağıdaki alternatifleri dikkate almalıdır, böylelikle çalışanlar Iş Ortağı Merkezi 'ne erişirken MFA doğrulamasını yine de tamamlayabilirler:
- İş ortağı Ayrıca, ek doğrulama yöntemleri sağlayabilen Azure AD Premium veya üçüncü taraf MFA çözümlerine (Azure AD ile uyumlu) kaydolabilir.

##### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>Sorun 5: Iş ortağı eski kimlik doğrulama protokollerinin kullanımı nedeniyle MFA uygulayamaz
Bir iş ortağı, hala, MFA uyumlu olmayan eski kimlik doğrulama protokollerini kullanan bazı iş ortakları aracılarıdır. Örneğin, kullanıcılar hala eski kimlik doğrulama protokollerini temel alan Outlook 2010 'yi kullanıyor. Bu iş ortağı aracılarında MFA etkinleştirildiğinde eski kimlik doğrulama protokollerinin kullanımı kesintiye uğracaktır.

**Cevap**: Hayır, bu, Teknik özel durum için geçerli bir neden değil. Bu protokollerin MFA doğrulaması ile korunamadığı ve kimlik bilgilerinin tehlikeye düşmesi açısından çok daha açıktır olması nedeniyle, iş ortaklarının eski kimlik doğrulama protokollerinin kullanılmasından uzaklaşması önemle önerilir. Eski kimlik doğrulama protokollerinin kullanımını tercih eden bir seçenek yoksa, iş ortakları, uygulama parolalarının kullanımını destekleyen Azure AD Premium için kaydolmayı düşünmelidir. Uygulama Parolaları, sistem tarafından oluşturulan tek bir paroladır ve genellikle insan tarafından oluşturulan parolalardan daha güçlü olur. İş ortakları, Uygulama Parolalarını kullanarak kullanıcıları için MFA'yi uygulamaya alırken yalnızca eski kimlik doğrulama protokolleri için Uygulama Parolaları'ne geri döner.

Outlook için eski kimlik doğrulamasını destekleme planı hakkında en son planı anlamak için Temel Kimlik Doğrulaması ve [Exchange Online](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-auth-and-exchange-online-february-2020-update/ba-p/1191282) ile ilgili gönderiyi okuyun ve gelecek haberleri almak için Exchange ekip [bloglarını](https://techcommunity.microsoft.com/t5/exchange-team-blog/bg-p/Exchange) izleyin. 

> [!NOTE]
> İş ortağı, iş ortağı aracıları için MFA uygulamamış olsa da iş ortağı aracıları, müşteri kiracısına oturum açma sırasında istendiğinde MFA kaydını ve MFA doğrulamasını tamamlayabilecekleri şartıyla İş Ortağı Temsilcisi Yönetim Ayrıcalıklarını kullanarak Microsoft Online Services Portallarına erişmeye devam eder. MFA kaydının tamamlanması, kullanıcının MFA için otomatik olarak etkinleştirmez.

##### <a name="issue-6-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>Sorun 6: İş ortağı Azure AD tarafından tanınmamış üçüncü taraf MFA'sı uygulamaya aldı
Bir iş ortağı, üçüncü taraf bir MFA çözümü kullanarak kullanıcıları için MFA uygulamaya aldı. Ancak iş ortağı, kullanıcı kimlik doğrulaması sırasında MFA doğrulamasının tamamlandıktan sonra Azure AD'ye geçiş yapmak için üçüncü taraf MFA çözümünü doğru yapılandıramaz. Bu teknik özel durum için geçerli bir neden mi?

**Cevap:** Evet, bu sorun teknik özel durum için geçerli bir neden olarak düşünülebilir. Teknik özel durum isteği göndermeden önce, üçüncü taraf MFA çözüm sağlayıcısıyla MFA çözümünün *authenticationmethodsreferences* talebini *(multipleauthn* değeriyle) Azure AD'ye akışla göndererek kullanıcı kimlik doğrulaması sırasında MFA doğrulamasının tamamlandıktan emin olun. Teknik özel durum isteği gönderme sırasında kullanılan üçüncü taraf MFA çözümünün ayrıntılarını sağlamanız ve tümleştirme yöntemini (örneğin kimlik federasyonu veya Azure AD Özel Denetimi kullanımı) göstermeniz ve destek belgeleri olarak teknik özel durum isteğinde aşağıdaki bilgileri sağlamanız gerekir:

- Üçüncü taraf MFA yapılandırması.

- Üçüncü taraf MFA etkin hesabıyla çalışan [Iş ortağı güvenlik gereksinimlerinin test](/powershell/partnercenter/test-partner-security-requirements) sonucu.

- Kullanmakta olduğunuz veya kullanmayı planladığınız üçüncü taraf MFA çözümünün satın alma siparişi.

## <a name="how-to-submit-a-request-for-technical-exception"></a>Teknik özel durum için istek gönderme

İş ortakları, Microsoft Online Services ile ilgili teknik sorunlarla karşılaştıklarında ve uygun bir çözüm ya da geçici çözüm yoksa MFA doğrulamasını bastırmak için Teknik özel durum uygulayabilir. Bunu yapmadan önce, önceki bölümde yer aldığı [yaygın sorunların listesini](#list-of-common-issues) gözden geçirin.

Teknik özel durum için bir istek göndermek için:

1. Iş Ortağı Merkezi 'nde genel yönetici veya yönetici Aracısı olarak oturum açın.

2. **Destek**  >  **ortağı destek isteklerini** ve **yeni istek**' i seçerek yeni bir iş ortağı hizmeti isteği oluşturun.

3. Arama kutusunda **özel durum Için MFA-istek** araması yapın; veya kategorisinden **CSP** ' yi seçin, ardından **hesaplar, ekleme, konudan erişim** ' i seçin, sonra da alt konudan **MFA-özel durum iste** ' yi seçin ve ardından **İleri adım**' ı seçin.

4. Teknik özel durum için bir hizmet isteği göndermek için istenen ayrıntıları sağlayın ve **Gönder**' i seçin.

Microsoft 'un Teknik özel durum isteğine yanıt vermesi için en fazla üç çalışma günü bulunabilir.

## <a name="next-steps"></a>Sonraki adımlar

 - [İş ortağı güvenlik gereksinimlerinin durumu](partner-security-compliance.md)