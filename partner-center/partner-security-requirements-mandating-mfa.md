---
title: İş ortağı kiracınız için çok faktörlü kimlik doğrulamasını (MFA) mandating
ms.topic: article
ms.date: 10/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: İş ortağı kiracılar için MFA'nın zorunlu tutularak müşteri kaynaklarına erişiminizin güvenliğinin nasıl altına yardımcı olduğunu öğrenin. Örnek senaryoları içerir.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9fe1d894ec933072a64f2abdfbb795b6ef046168
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276017"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>İş ortağı kiracınız için çok faktörlü kimlik doğrulamasını (MFA) mandating

**Uygun roller:** Yönetici aracısı | Satış aracısı | Yardım masası aracısı | Faturalama yöneticisi | Genel yönetici

Bu makalede, çok faktörlü kimlik doğrulamasını (MFA) iş birliğinde İş Ortağı Merkezi. Bu özelliğin amacı, iş ortaklarının kimlik bilgilerinin tehlikeye atarak müşteri kaynaklarına erişiminin güvenliğini sağlamalarına yardımcı olmaktır. İş ortaklarının, konuk kullanıcılar da dahil olmak üzere iş ortağı kiracılarında tüm kullanıcı hesapları için MFA'nın uygulanması gerekir. Kullanıcıların aşağıdaki alanlar için MFA doğrulamayı tamamlamaları zorunlu tutulacak:

- [İş Ortağı Merkezi Panosu](#partner-center-dashboard)
- [İş Ortağı Merkezi API’si](#partner-center-api)
- [İş Ortağı Temsilci Yönetimi](#partner-delegated-administration)

Daha büyük ve sürekli güvenlik ve gizlilik korumaları en önemli önceliklerimiz arasında yer almaktadır ve iş ortaklarının müşterilerini ve kiracılarını korumasına yardımcı olmaya devam ediyoruz. Bulut Çözümü Sağlayıcısı (CSP) programına katılan tüm iş ortakları, Denetim Masası Satıcıları (CPV) ve Danışmanlar, uyumlu kalmak için İş Ortağı [Güvenlik](partner-security-requirements.md) Gereksinimlerini uygulamalıdır.

İş ortaklarının işletmelerini ve müşterilerini kimlik hırsızlığına ve yetkisiz erişime karşı korumasına yardımcı olmak için, MFA'nın zorunlu tutularak ve doğrulandırarak iş ortağı kiracıları için ek güvenlik önlemlerini etkinleştirildik. 

## <a name="partner-center-dashboard"></a>İş Ortağı Merkezi panosu

Aşağıdakiler dahil olmak İş Ortağı Merkezi panoda belirli sayfalar MFA korumalı olur:

- Müşteriler sekmesinin **altındaki** tüm sayfalar, örneğin aşağıdaki URL aracılığıyla erişilebilen tüm sayfalar: https://partner.microsoft.com/commerce/*
- Destek Ve Müşteri **> sekmesindeki** tüm sayfalar, örneğin altında erişilen sayfa https://partner.microsoft.com/dashboard/support/csp/customers/*
- Faturalandırma sayfası

Aşağıdaki tabloda, hangi kullanıcı türlerinin bu MFA korumalı sayfalara erişim yetkisi olduğu (ve bu nedenle bu özellikten etkilendiği) gösterir.


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

3. Contoso tarafından mevcut Azure AD MFA kurulumu nedeniyle Jane'in MFA doğrulamayı tamamlaması gerekir. Başarılı oturum açma ve MFA doğrulamasının ardından Jane, panoya İş Ortağı Merkezi sayfasına geri yönlendirildi.

4. Jane, veri koruma altındaki MFA korumalı sayfalardan İş Ortağı Merkezi. Jane daha önce oturum açma sırasında MFA doğrulamasını zaten tamamlamış olduğu için, Jane yeniden MFA doğrulamasından geçerek MFA korumalı sayfaya erişebilirsiniz.

### <a name="example-2-partner-has-implemented-third-party-mfa-using-identity-federation"></a>Örnek 2: İş ortağı kimlik federasyonu kullanarak üçüncü taraf MFA'sı uygulamaya aldı

1. Trent, CSP Wingtip için çalışır. Wingtip, kimlik federasyonu aracılığıyla Azure AD ile tümleştirilmiş üçüncü taraf MFA kullanarak Wingtip iş ortağı kiracısı altındaki tüm kullanıcıları için MFA'ya sahip oldu.

2. Trent yeni bir tarayıcı oturumu başlatır ve İş Ortağı Merkezi panoya genel bakış sayfasına (MFA korumalı değildir) gidin. İş Ortağı Merkezi için Trent'i Azure AD'ye yeniden yönlendirin.

3. Wingtip'te kimlik federasyonu ayarlandıktan sonra Azure AD, Oturum açma ve MFA doğrulamasını tamamlamak için Trent'i federasyon kimlik sağlayıcısına yeniden yönlendirmektedir. Başarılı oturum açma ve MFA doğrulamasının ardından, Trent Azure AD'ye geri ve ardından panoya İş Ortağı Merkezi sayfasına yeniden yönlendirildi.

4. Trent, İş Ortağı Merkezi'daki MFA korumalı sayfalardan İş Ortağı Merkezi. Trent daha önce oturum açma sırasında MFA doğrulamasını zaten tamamlamış olduğu için, Trent yeniden MFA doğrulamasından geçerek MFA korumalı sayfasına erişebilirsiniz.

### <a name="example-3-partner-hasnt-implemented-mfa"></a>Örnek 3: İş ortağı MFA uygulamadı

1. John, CSP Fabrikam'da çalışıyor. Fabrikam, Fabrikam iş ortağı kiracısı altındaki hiçbir kullanıcı için MFA uygulamadı.

2. John yeni bir tarayıcı oturumu başlatır ve İş Ortağı Merkezi panosuna genel bakış sayfasına (MFA korumalı değildir) gidin. İş Ortağı Merkezi john'u Azure AD'ye yeniden yönlendirin.

3. Fabrikam MFA uygulamamış olduğu için John'un MFA doğrulamayı tamamlaması gerekmez. Oturum başarıyla oturum açmanın ardından John panoya genel bakış İş Ortağı Merkezi yeniden yönlendirildi.

4. John, bir MFA korumalı sayfadan bir veritabanına erişmeye İş Ortağı Merkezi. John MFA doğrulamayı tamamlamamış olduğu için İş Ortağı Merkezi, MFA doğrulamayı tamamlamak için John'u Azure AD'ye yeniden yönlendirmektedir. Bu, John'un MFA'nın ilk kez tamamlanması gerektiğinden, John'dan [MFA'ya kaydolması da istenmektedir.](#mfa-registration-experience) Başarılı bir MFA kaydı ve MFA doğrulamasının ardından John artık MFA korumalı sayfasına erişebilirsiniz.

5. Fabrikam'ın herhangi bir kullanıcı için MFA uygulamadan bir gün önce, John yeni bir tarayıcı oturumu başlatır ve İş Ortağı Merkezi panoya genel bakış sayfasına (MFA korumalı değildir) gidin. İş Ortağı Merkezi, John'u MFA istemi olmadan oturum açması için Azure AD'ye yeniden yönlendirer. 

6. John, bir MFA korumalı sayfadan bir veritabanına erişmeye İş Ortağı Merkezi. John MFA doğrulamayı tamamlamamış olduğu için İş Ortağı Merkezi, MFA doğrulamayı tamamlamak için John'u Azure AD'ye yeniden yönlendirmektedir. John MFA'ya kayıtlı olduğu için bu kez yalnızca MFA doğrulamayı tamamlaması istenmektedir.

> [!NOTE]
>Eylem: Şirket yöneticilerinin MFA [uygulamak](partner-security-requirements.md#implementing-multi-factor-authentication) için üç seçeneği vardır.

## <a name="partner-center-api"></a>İş Ortağı Merkezi API’si

İş Ortağı Merkezi API'si hem Yalnızca uygulama kimlik doğrulamasını hem de App+User kimlik doğrulamasını destekler. 

Uygulama+Kullanıcı kimlik doğrulaması kullanılırken, İş Ortağı Merkezi kimlik doğrulaması gerekir. Daha açık olarak, bir iş ortağı uygulama İş Ortağı Merkezi API isteği göndermek istiyorsa, isteğin Yetkilendirme üst bilgisinde bir erişim belirteci içermesi gerekir. 

> [!NOTE]
>Güvenli Uygulama Modeli [çerçevesi,](/partner-center/develop/enable-secure-app-model) Microsoft Azure API'leri çağıran MFA mimarisi aracılığıyla CSP iş ortaklarının ve CPU'İş Ortağı Merkezi ölçeklenebilir bir çerçevedir. Kiracınız üzerinde MFA'ya etkinleştirmeden önce bu çerçeveyi uygulamanız gerekir. 

Bu İş Ortağı Merkezi App+User kimlik doğrulaması kullanılarak alınan erişim belirteci ile bir API isteği aldığında, İş Ortağı Merkezi API'si Kimlik Doğrulama Yöntemi Başvurusu *(AMR)* talepte *MFA* değerinin varlığını kontrol eder. Bir erişim belirtecin beklenen kimlik doğrulama yöntemi başvurusu (AMR) değerini içerdiğini doğrulamak için JWT kod çözücüsü kullanabilirsiniz:

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

Değer varsa, MFA İş Ortağı Merkezi tamamlandıktan ve API isteğini işlemektedir. Değer yoksa, İş Ortağı Merkezi API aşağıdaki yanıtla isteği reddeder:

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

Kimlik App-Only, kimlik doğrulamasını destekleyen API'App-Only MFA gerektirmeden sürekli olarak çalışmaya devam ediyor.

## <a name="partner-delegated-administration"></a>İş Ortağı Temsilci Yönetimi

Yönetici Aracıları ve Yardım Masası Aracıları dahil olmak üzere iş ortağı hesapları, Microsoft Online Services Portalları, komut satırı arabirimi (CLI) ve API'ler (App+User kimlik doğrulamasını kullanarak) aracılığıyla müşteri kaynaklarını yönetmek için İş Ortağı Temsilci Yönetici Ayrıcalıklarını kullanabilir.

### <a name="using-service-portals"></a>Hizmet portallarını kullanma

Müşteri kaynaklarını yönetmek için İş Ortağı Temsilcisi Yönetici Ayrıcalıkları (Yönetici-Adına) kullanarak Microsoft Online Services Portallarına erişirken, bu portalların çoğu, müşteri Azure AD kiracısı kimlik doğrulama bağlamı olarak ayarlanmış şekilde etkileşimli olarak kimlik doğrulaması yapmak için iş ortağı hesabının kimlik doğrulamasını gerektirir. Müşteri kiracısı oturum açması için iş ortağı hesabı gereklidir.

Azure AD bu tür kimlik doğrulama isteklerini aldığında, iş ortağı hesabının MFA doğrulamasını tamamlaması gerekir. İş ortağı hesabının yönetilen mi yoksa federasyon kimliği mi olduğuna bağlı olarak iki olası kullanıcı deneyimi vardır:

- İş ortağı hesabı yönetilen bir **kimlikse** Azure AD doğrudan kullanıcıdan MFA doğrulamayı tamamlaması istenir. İş ortağı hesabı daha önce Azure AD'ye MFA'ya kayıtlı değilse, kullanıcıdan önce [MFA kaydını tamamlaması istenecek.](#mfa-registration-experience)

- İş ortağı hesabı bir **federasyon kimliği ise** deneyim, iş ortağı yöneticisinin Azure AD'de federasyonu nasıl yapılandırmış olduğuna bağlıdır. Azure AD'de federasyon ayarlarken, iş ortağı yöneticisi Azure AD'ye federasyon kimlik sağlayıcısının MFA'ya destek olup olmadığını belirtebilirsiniz. Öyleyse Azure AD, MFA doğrulamayı tamamlamak için kullanıcıyı federasyon kimlik sağlayıcısına yeniden yönlendirecek. Aksi takdirde, Azure AD doğrudan kullanıcıdan MFA doğrulamayı tamamlaması istenir. İş ortağı hesabı daha önce Azure AD'ye MFA'ya kayıtlı değilse, kullanıcıdan önce [MFA kaydını tamamlaması istenecek.](#mfa-registration-experience)

Genel deneyim, son müşteri kiracısı yöneticileri için MFA'nın uygulanmış olduğu senaryoya benzer. Örneğin, müşteri [kiracısı, Yönetici](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)Aracıları ve Yardım Masası Aracıları dahil olmak üzere MFA doğrulaması ile müşteri kiracısına oturum açması için yönetici haklarına sahip tüm hesapların gerektirdiği Azure AD güvenlik varsayılanlarını etkinleştirdi. Test amacıyla, iş ortakları müşteri kiracısı [içinde Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) güvenlik varsayılanlarını etkinleştirebilir ve ardından müşteri kiracısına erişmek için İş Ortağı Temsilcisi Yönetim Ayrıcalıklarını kullanmayı deneyebilir.

> [!NOTE]
> Tüm Microsoft Online Service Portalları, İş Ortağı Temsilcisi Yönetici Ayrıcalıkları kullanarak müşteri kaynaklarına erişirken iş ortağı hesaplarının müşteri kiracısı içinde oturum açmasını gerektirmez. Bunun yerine, yalnızca iş ortağı hesaplarının iş ortağı kiracıda oturum açmasını gerektirir. Örneğin Exchange Yönetim Merkezi. Zaman içinde, bu portalların İş Ortağı Temsilcisi Yönetici Ayrıcalıkları kullanırken iş ortağı hesaplarının müşteri kiracısına oturum açmasını gerektirmesi gerekir.

### <a name="using-service-apis"></a>Hizmet API'lerini kullanma

Bazı Microsoft Online Services API'leri (Azure Resource Manager, Azure AD Graph, Microsoft Graph vb.) iş ortaklarını, müşteri kaynaklarını program aracılığıyla yönetmek için İş Ortağı Temsilcisi Yönetici Ayrıcalıkları kullanarak destekler. İş Ortağı Temsilcisi Yönetici Ayrıcalıklarını bu API'lerle kullanmak için, iş ortağı uygulaması API isteği Yetkilendirme üst bilgisinde bir erişim belirteci içermesi gerekir. Burada erişim belirteci Azure AD ile kimlik doğrulaması yapmak için bir iş ortağı kullanıcı hesabına sahip olur ve müşteri Azure AD kimlik doğrulama bağlamı olarak ayarlanır. İş ortağı uygulamasının müşteri kiracısı için bir iş ortağı kullanıcı hesabıyla oturum açması gerekir.

Azure AD kimlik doğrulama isteği gibi bir yanıt aldığında Azure AD, MFA doğrulamasını tamamlamak için iş ortağı kullanıcı hesabı gerektirir. İş ortağı kullanıcı hesabı daha önce MFA'ya kayıtlı değilse, kullanıcı hesabından önce MFA kaydını tamamlaması istenir.

İş Ortağı Temsilcisi Yönetici Ayrıcalıkları kullanılarak bu API'lerle tümleştirilmiş tüm iş ortağı uygulamaları bu özellikten etkilenir. İş ortağı uygulamalarının kesinti olmadan bu API'lerle çalışmaya devam etmek için:

- İş ortağının erişim belirteci almak için Azure AD ile etkileşimli olmayan kullanıcı kimlik doğrulama yöntemini kullanmaktan kaçınması gerekir. Parola Akışı gibi etkileşimli olmayan kullanıcı kimlik doğrulama [yöntemi](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password)kullanılırken Azure AD, kullanıcıdan MFA doğrulamasını tamamlamasını isteminde olmayacaktır. İş ortağının akış akışı gibi etkileşimli kullanıcı kimlik doğrulama [yöntemini OpenID Connect olması](/azure/active-directory/develop/v1-protocols-openid-connect-code) gerekir.

- Etkileşimli kullanıcı kimlik doğrulama yöntemi sırasında, iş ortağı MFA için zaten etkinleştirilmiş bir iş ortağı kullanıcı hesabı kullan olmalıdır. Alternatif olarak, Azure AD tarafından istendiğinde iş ortağı oturum açma sırasında MFA kaydını ve MFA doğrulamasını tamamlar.

- Bu, son müşteri kiracısı yöneticileri için MFA'nın uygulanmasına benzer. Örneğin, müşteri kiracısı [Yönetici](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)Aracıları ve Yardım Masası Aracıları dahil olmak üzere MFA doğrulaması ile müşteri kiracısına oturum açması için yönetici haklarına sahip tüm kullanıcı hesaplarının gerektirdiği Azure AD güvenlik varsayılanlarını etkinleştirdi. Test amacıyla, iş ortakları [müşteri](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) kiracısı içinde Azure AD güvenlik varsayılanlarını etkinleştirebilir ve ardından müşteri kiracısına programlı olarak erişmek için İş Ortağı Temsilcisi Yönetim Ayrıcalıkları kullanmayı deneyebilir.

### <a name="mfa-registration-experience"></a>MFA kayıt deneyimi

MFA doğrulaması sırasında, iş ortağı hesabı daha önce MFA'ya kayıtlı değilse, Azure AD kullanıcıdan önce MFA kaydını tamamlaması istenir:

:::image type="content" source="images/MfaRegistration1.png" alt-text="MFA kaydı 1. adım.":::

Sonraki **seçeneğine** tıklanmasından sonra, kullanıcıdan doğrulama yöntemleri listesinden seçim seçmesi istenecek.

:::image type="content" source="images/MfaRegistration2.png" alt-text="MFA kaydı 2. adım.":::

Kayıt başarıyla tamamlandıktan sonra kullanıcının, kullanıcı tarafından seçilen doğrulamaya göre MFA doğrulamayı tamamlaması gerekir.
 
## <a name="list-of-common-issues"></a>Yaygın sorunların listesi

MFA [gereksiniminden teknik özel](#how-to-submit-a-request-for-technical-exception) durum için başvurmadan önce, isteğinizin geçerli olup olmadığını anlamak için diğer iş ortakları tarafından bildirilen yaygın sorunların listesini gözden geçirebilirsiniz.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>Sorun 1: İş ortağının iş ortağı aracıları için MFA'nın uygulanması için daha fazla zaman gerekiyor
bir iş ortağı, müşteri kaynaklarını yönetmek için İş Ortağı Temsilcisi Yönetim Ayrıcalıkları kullanarak Microsoft Online Services Portallarına erişmesi gereken iş ortağı aracıları için MFA'nın uygulanmasına henüz başlamadı veya hala devam ediyor. İş ortağının MFA uygulamasını tamamlaması için daha fazla zaman gerekir. Bu sorun teknik özel durum için geçerli bir neden mi?

**Cevap:** Hayır. İş ortağının kesintiyi önlemek için kullanıcıları için MFA uygulama planları yapmaları gerekir.

> [!NOTE]
> İş ortağı, iş ortağı aracıları için MFA uygulamamış olsa da iş ortağı aracıları, müşteri kiracısına oturum açma sırasında istendiğinde MFA kaydını ve MFA doğrulamasını tamamlayabilecekleri şartıyla İş Ortağı Temsilcisi Yönetim Ayrıcalıklarını kullanarak Microsoft Online Services Portallarına erişmeye devam eder. MFA kaydının tamamlanması, kullanıcının MFA için otomatik olarak etkinleştirmez.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>Sorun 2: İş ortağı, Yönetici Ayrıcalıkları Temsilcisi kullanmayan kullanıcı hesapları için MFA uygulamadı
bir iş ortağının iş ortağı kiracılarında, İş Ortağı Temsilcisi Yönetim Ayrıcalıkları kullanarak müşteri kaynaklarını yönetmek için Microsoft Online Services Portallarına erişim gerektirmeyen bazı kullanıcıları vardır. İş ortağı bu kullanıcılar için MFA uygulama sürecindedir ve tamamlanması için daha fazla zaman gerekir. Bu sorun teknik özel durum için geçerli bir neden mi?

**Cevap:** Hayır. Bu kullanıcı hesapları müşteri kaynaklarını yönetmek için İş Ortağı Temsilcisi Yönetim Ayrıcalıkları kullanmayacaklarından, müşteri kiracısı için oturum açmaları gerekmez. Müşteri kiracısına oturum açma sırasında MFA doğrulaması gerektiren Azure AD'den etkilenmezler.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>Sorun 3: İş ortağı kullanıcı hizmeti hesapları için MFA uygulamadı
Bir iş ortağının, iş ortağı kiracılarında cihazlar tarafından hizmet hesabı olarak kullanılan bazı kullanıcı hesapları vardır. Bunlar, İş Ortağı Temsilcisi Yönetim Ayrıcalıkları'İş Ortağı Merkezi müşteri kaynaklarını yönetmek için Microsoft Online Services Portallarına veya Microsoft Online Services Portallarına erişim gerektirmeyen düşük ayrıcalıklı hesaplardır. Bu sorun teknik özel durum için geçerli bir neden mi?

**Cevap:** Hayır. Bu kullanıcı hesapları müşteri kaynaklarını yönetmek için İş Ortağı Temsilcisi Yönetim Ayrıcalıkları kullanmayacaklarından, müşteri kiracısı için oturum açmaları gerekmez. Müşteri kiracısına oturum açma sırasında MFA doğrulaması gerektiren Azure AD'den etkilenmezler.

##### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>Sorun 4: İş ortağı MS Authenticator Uygulaması kullanarak MFA uygulayamaz
Bir iş ortağının, çalışanların kişisel mobil cihazlarını iş alanlarına getirmelerine izin vermeyen "temiz masa" ilkesi vardır. Çalışanlar, kişisel mobil cihazlarına erişim olmadan, Azure AD güvenlik varsayılanları tarafından desteklenen tek MFA doğrulaması olan MS Authenticator Uygulamasını yükleyemeden. Bu sorun teknik özel durum için geçerli bir neden mi?

**Cevap:** Hayır, bu teknik özel durum için geçerli bir neden değildir. İş ortağı aşağıdaki alternatifleri göz önünde İş Ortağı Merkezi:
- İş ortağı ayrıca ek doğrulama Azure AD Premium veya üçüncü taraf MFA çözümlerine (Azure AD ile uyumlu) kaydolabilirsiniz.

##### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>Sorun 5: İş ortağı eski kimlik doğrulama protokollerinin kullanımı nedeniyle MFA uygulayamaz
Bir iş ortağının hala MFA uyumlu olmayan eski kimlik doğrulama protokollerini kullanan bazı iş ortağı aracıları vardır. Örneğin, kullanıcılar hala eski kimlik doğrulama protokollerini temel alan Outlook 2010 kullanıyor. Bu iş ortağı aracıları için MFA'nın etkinleştirilmesi, eski kimlik doğrulama protokollerinin kullanımını kesintiye neden olur.

**Cevap:** Hayır, bu teknik özel durum için geçerli bir neden değildir. Bu protokoller MFA doğrulamasıyla korunamaya ve kimlik bilgilerinin tehlikeye atlanmasına karşı çok daha duyarlı olduğundan, olası güvenlik etkileri nedeniyle iş ortaklarının eski kimlik doğrulama protokollerinin kullanımından uzak olması önemle tavsiye edilecektir. Eski kimlik doğrulama protokollerinin kullanımından uzaklaşan bir seçenek yoksa, iş ortaklarının Uygulama Parolaları kullanımını destekleyen Azure AD Premium için kaydolmayı göz önünde bulundurabilirsiniz. Uygulama Parolaları, sistem tarafından oluşturulan tek bir paroladır ve genellikle insan tarafından oluşturulan parolalardan daha güçlü olur. İş ortakları, Uygulama Parolalarını kullanarak kullanıcıları için MFA'yi uygulamaya alırken yalnızca eski kimlik doğrulama protokolleri için Uygulama Parolaları'ne geri döner.

Outlook için eski kimlik doğrulamasını destekleme planı hakkında en son planı anlamak için Temel Kimlik Doğrulaması ve [Exchange Online](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-auth-and-exchange-online-february-2020-update/ba-p/1191282) ile ilgili gönderiyi okuyun ve gelecek haberleri almak için Exchange ekip [bloglarını](https://techcommunity.microsoft.com/t5/exchange-team-blog/bg-p/Exchange) izleyin. 

> [!NOTE]
> İş ortağı, iş ortağı aracıları için MFA uygulamamış olsa da iş ortağı aracıları, müşteri kiracısına oturum açma sırasında istendiğinde MFA kaydını ve MFA doğrulamasını tamamlayabilecekleri şartıyla İş Ortağı Temsilcisi Yönetim Ayrıcalıklarını kullanarak Microsoft Online Services Portallarına erişmeye devam eder. MFA kaydının tamamlanması, kullanıcının MFA için otomatik olarak etkinleştirmez.

##### <a name="issue-6-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>Sorun 6: İş ortağı Azure AD tarafından tanınmamış üçüncü taraf MFA'sı uygulamaya aldı
Bir iş ortağı, üçüncü taraf bir MFA çözümü kullanarak kullanıcıları için MFA uygulamaya aldı. Ancak iş ortağı, kullanıcı kimlik doğrulaması sırasında MFA doğrulamasının tamamlandıktan sonra Azure AD'ye geçiş yapmak için üçüncü taraf MFA çözümünü doğru yapılandıramaz. Bu teknik özel durum için geçerli bir neden mi?

**Cevap:** Evet, bu sorun teknik özel durum için geçerli bir neden olarak değerlendirebilir. Teknik özel durum isteği göndermeden önce, üçüncü taraf MFA çözüm sağlayıcısıyla MFA çözümünün *authenticationmethodsreferences* talebini *(multipleauthn* değeriyle) Azure AD'ye akışla göndererek kullanıcı kimlik doğrulaması sırasında MFA doğrulamasının tamamlandıktan emin olun. Teknik özel durum isteği gönderme sırasında kullanılan üçüncü taraf MFA çözümünün ayrıntılarını sağlamanız ve tümleştirme yöntemini (örneğin kimlik federasyonu veya Azure AD Özel Denetimi kullanımı aracılığıyla) göstermeniz ve destek belgeleri olarak teknik özel durum isteğinde aşağıdaki bilgileri sağlamanız gerekir:

- Üçüncü taraf MFA yapılandırmaları.

- Üçüncü taraf MFA [etkin hesabı tarafından](/powershell/partnercenter/test-partner-security-requirements) çalışan İş Ortağı Güvenlik Gereksinimlerini Test Edin'in sonucu.

- Kullanmakta veya kullanmayı planlasanız üçüncü taraf MFA çözümünün satın alma siparişi.

## <a name="how-to-submit-a-request-for-technical-exception"></a>Teknik özel durum için istek gönderme

İş ortakları, Microsoft Online Services ile ilgili teknik sorunlarla karşılaşıyorsa ve uygulanabilir bir çözüm veya geçici çözüm yoksa, MFA doğrulamasını gizlemeye yönelik teknik özel durum için başvurabilir. Bunu yapmadan önce, [önceki bölümdeki yaygın sorunların](#list-of-common-issues) listesini gözden geçirebilirsiniz.

Teknik özel durum isteği göndermek için:

1. Genel Yönetici İş Ortağı Merkezi Yönetici Aracısı olarak oturum açma.

2. Destek İş Ortağı destek istekleri'ne giderek ve Yeni istek'i  >  **seçerek yeni** bir iş ortağı hizmet isteği **oluşturun.**

3. **MFA ara - Arama kutusunda özel** durum isteği; veya **Kategori'den CSP'yi** seçin, ardından **Hesaplar, Ekleme,** Konu başlığından Erişim'i ve ardından alt konu başlığından **MFA -** Özel durum isteği'yi seçin ve ardından sonraki **adımı seçin.**

4. Teknik özel durum için bir hizmet isteği göndermek için istenen ayrıntıları s sağlama ve Gönder'i **seçin.**

Microsoft'un teknik özel durum isteğine yanıt olarak sağlaması üç iş günü kadar zaman alır.

## <a name="next-steps"></a>Sonraki adımlar

 - [İş ortağı güvenlik gereksinimleri durumu](partner-security-compliance.md)