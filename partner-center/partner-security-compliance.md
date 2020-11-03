---
title: İş ortağı güvenlik gereksinimlerinin durumu
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Bulut çözümü sağlayıcısı programındaki danışmanların, Denetim Masası satıcılarının ve iş ortaklarının güvenliğini artıran yeni zorunlu gereksinimler hakkında bilgi edinin.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: 1b6c2d56a0747ddf2bd1a821886e371ed698a4a1
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/22/2020
ms.locfileid: "92531591"
---
# <a name="partner-security-requirements-status---get-answers-and-check-reports-about-current-status"></a>İş ortağı güvenlik gereksinimleri durumu-geçerli durumla ilgili yanıtları al ve raporları denetle

**Uygulama hedefi**

- Bulut çözümü sağlayıcısı programındaki tüm iş ortakları
  - Doğrudan fatura
  - Dolaylı sağlayıcı
  - Dolaylı satıcı
- Tüm Denetim Masası satıcıları
- Tüm danışmanları

**Uygun kullanıcılar**
- Konuk kullanıcılar dahil tüm etkin kullanıcılar

Büyük gizlilik korumaları ve güvenlik, en iyi önceliklerimiz arasındadır. En iyi savunması önleme olduğunu ve yalnızca zayıf bağlantımız kadar güçlü olduğunu biliyoruz. Bu nedenle, ekosistemimizde herkese uygun güvenlik korumalarının gerçekleşmesini ve uygun güvenlik korumalarının yapıldığından emin olmamız gerekir. İş ortaklarının ve müşterilerin korunmasına yardımcı olmak için, danışmanları, Denetim Masası satıcıları ve bulut çözümü sağlayıcısı programına katılan iş ortakları için bir dizi zorunlu güvenlik gereksinimi sunuyoruz.

1 Ağustos 2019 ' den itibaren, tüm iş ortakları, hizmet hesapları da dahil olmak üzere tüm kullanıcılar için iş ortağı kiracılarında Multi-Factor Authentication 'ı zorlamak için gereklidir. Yeni güvenlik ilkeleri hakkında daha ayrıntılı bilgi için [Iş ortağı güvenlik gereksinimlerini](partner-security-requirements.md)okuyun.

Her bir kullanıcının her tek kimlik doğrulaması için MFA sınamasına sahip olduğundan emin olmak istiyoruz. Bu deneyim aşağıdaki yollarla gerçekleştirilebilir:

- Her Kullanıcı için MFA 'nın uygulanmasını sağlamak üzere Azure AD Premium uygulama
- [Azure AD güvenlik varsayılanlarını](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults) uygulama
- Her Kullanıcı için MFA 'nın uygulanmasını sağlamak için üçüncü taraf bir çözüm uygulama

## <a name="partner-security-requirements-status"></a>İş ortağı güvenlik gereksinimlerinin durumu

Bu rapor, kısa süre düşerek nerede olabileceğini görmeniz için bir yol sağlayarak güvenlik gereksinimlerinin durumunu doğrulamanıza yardımcı olabilir. İzleme düzenli olarak güncelleştirilir.

>[!NOTE]
>Iş ortağı güvenlik gereksinimlerinin durum raporu yalnızca Iş Ortağı Merkezi 'nde desteklenir. ABD devlet veya Microsoft Bulut Almanya için Microsoft Bulut kullanılamaz. Bir sogeign bulutu (21Vianet, ABD kamu ve Almanya) üzerinden deneyimidir tüm iş ortaklarının bu yeni güvenlik gereksinimlerini hemen benimsemesini önemle öneririz. Ancak, bu iş ortakları 1 Ağustos 2019 ' den itibaren geçerli olan yeni güvenlik gereksinimlerini karşılamak için gerekli değildir. Microsoft, daha sonra da bu güvenlik gereksinimlerinin zorlanmasıyla ilgili ek ayrıntılar sağlar.

## <a name="multi-factor-authentication-mfa-report"></a>Multi-Factor Authentication ("MFA") raporu

Iş Ortağı Merkezi MFA raporu, CSP kiracısının MFA yapılandırmasına ve Iş Ortağı Merkezi etkinliklerine göre iki tür ölçüm sağlayarak iş ortağı MFA uygulamasıyla ilgili öngörüler sunar: 

### <a name="mfa-configuration-on-a-csp-tenant"></a>CSP kiracısında MFA yapılandırması

Bu ölçüm, günlük olarak yakalanan ve rapor veren bir CSP kiracısındaki MFA yapılandırmasıyla ilgilidir. Bu, MFA [seçeneklerinin](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started)herhangi birini kullanarak, MFA Zorlanmış olan etkin kullanıcı hesaplarının yüzdesini ölçer. Örneğin:

- Contoso, kiracıda 110 Kullanıcı hesabı olan bir CSP iş ortağıdır, bu kullanıcı hesaplarının 10 ' u devre dışı bırakılır. 
- 100 Kullanıcı hesabının geri kalanında 90, sunulan [MFA seçenekleri](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started)kullanılarak MFA 'ya zorlanır. Bu nedenle, ölçüm %90 gösterir. 

### <a name="partner-center-activities-with-mfa"></a>MFA ile iş ortağı Merkezi Etkinlikleri

Çalışanlarınıza iş ortağı merkezi 'nde çalışan veya API 'Ler aracılığıyla veri gönderen her oturum açışınızda, güvenlik durumu ne olur ve izlenir. Güvenlik-durum izlemeye de dahil olmak üzere, uygulamalarınız ve tüm Denetim Masası satıcı uygulamalarınız. Görünen durum, önceki yedi güne yöneliktir.

#### <a name="mfa-verification-completed-by-users"></a>MFA doğrulaması kullanıcılar tarafından tamamlandı

Bu ölçüm, Iş Ortağı Merkezi panosu dahilinde etkinliklerle ilgilidir. MFA doğrulamasını tamamlayan kullanıcılar tarafından yapılan işlemlerin yüzdesini ölçer. Örneğin:

- Contoso, kemal ve John olmak üzere iki yönetici aracısına sahip bir CSP iş ortağıdır.
- İlk gün, Gamze doğrulaması olmadan Iş Ortağı Merkezi panosunda oturum açtı ve üç işlem yaptı.
- İkinci günde John, MFA doğrulaması olmadan Iş Ortağı Merkezi panosunda oturum açtı ve beş işlem yaptı.
- Üçüncü günde, Gamze, MFA doğrulaması ile Iş Ortağı Merkezi panosunda oturum açtı ve iki işlem yaptı.
- Kalan dört gün içinde herhangi bir aracı tarafından bir işlem yapılmadı.
- 7 günlük pencerede yapılan 10 işlemden sonra, MFA doğrulaması ile Kullanıcı tarafından iki tanesi yapılmıştır. Bu nedenle, ölçüm %20 ' yi gösterir.

Iş Ortağı Merkezi panosunda MFA doğrulaması yapmadan hangi kullanıcının oturum açtığını ve raporlama penceresi sırasında en son ziyaret zamanını anlamak için **MFA olmadan dosya portalı isteklerini** kullanın.

#### <a name="appuser-authentication"></a>Uygulama + kullanıcı kimlik doğrulaması

Bu ölçüm, uygulama + kullanıcı kimlik doğrulaması kullanılarak yapılan Iş Ortağı Merkezi API 'SI isteklerinin kullanımıyla ilgilidir. MFA talebine sahip bir erişim belirteci kullanılarak yapılan API isteklerinin yüzdesini ölçer. Örneğin:

- Fabrikam bir CSP iş ortağıdır ve App + kullanıcı kimlik doğrulaması ve yalnızca uygulama kimlik doğrulama yöntemlerinin bir karışımını kullanan bir CSP uygulamasına sahiptir.
- İlk günde uygulama, MFA doğrulaması olmadan uygulama + kullanıcı kimlik doğrulama yöntemi aracılığıyla elde edilen bir erişim belirteciyle desteklenen üç API isteği yaptı.
- İkinci gün, uygulama yalnızca uygulama kimlik doğrulaması kullanılarak edinilen bir erişim belirteciyle desteklenen beş API isteği yaptı.
- Üçüncü günde uygulama, MFA doğrulaması ile App + kullanıcı kimlik doğrulama yöntemi kullanılarak edinilen bir erişim belirteciyle desteklenen iki API isteği yaptı.
- Kalan dört gün içinde herhangi bir aracı tarafından bir işlem yapılmadı.
- İkinci gün üzerindeki beş API isteği, yalnızca uygulama kimlik doğrulaması aracılığıyla elde edilen bir erişim belirteci tarafından desteklenen, Kullanıcı kimlik bilgilerini kullanmadığından ölçüden çıkarılır. Kalan beş işlemin dışında, bunların ikisi MFA doğrulaması ile elde edilen bir erişim belirteciyle destekleniyor. Bu nedenle, ölçüm %40 gösterir.

Bu ölçüm üzerinde %100 olmayan bir uygulama ve Kullanıcı etkinliği olduğunu anlamak istiyorsanız, dosyaları kullanın:

- API, uygulamanın genel MFA durumunu anlamak için **Özet ister** .
- **Tüm API** istekleri kiracınızın kullanıcıları tarafından YAPıLAN her API isteğinin ayrıntılarını anlamak için, sonuç daha iyi indirme deneyimi için en çok 10.000 en son istek ile sınırlıdır.

## <a name="what-should-i-do-if-the-metrics-under-mfa-report-arent-100"></a>MFA raporundaki ölçümler %100 değilse ne yapmam gerekir

Iş Ortağı Merkezi MFA raporu kapsamındaki ölçümler, MFA uygulamış olan iş ortakları için %100 olmayabilir. Nedenini anlamak için göz önünde bulundurmanız gereken bazı etmenler aşağıda verilmiştir.

> [!NOTE]
> Kuruluşunuz tarafından iş ortağı kiracınızın kimlik yönetimi ve MFA uygulamasıyla ilgili bilgi sahibi olan bir kişi ile çalışmanız gerekir.

### <a name="have-you-implemented-mfa-for-your-partner-tenant"></a>İş ortağı kiracınız için MFA uyguladık mı?

Aksi takdirde, önce iş ortağı kiracınız için MFA 'yı uygulamanız gerekir. MFA 'yı uygulama hakkında daha fazla bilgi için, makale [ortağı güvenlik gereksinimi](partner-security-requirements.md)bölümüne bakın.

### <a name="have-you-only-recently-completed-mfa-implementation"></a>Yalnızca son zamanlarda MFA uygulamasını tamamladınız mı?

Ölçümler günlük olarak hesaplanır ve son yedi gün içinde gerçekleştirilen hesap işlemlerini alır. İş ortağı kiracınız için yalnızca en son MFA uygulamasını tamamladıysanız ölçümler %100 olmayabilir.

### <a name="have-some-user-accounts-been-excluded-from-mfa-implementation"></a>MFA uygulamasından bazı Kullanıcı hesapları hariç tutuldu mı?

Geçerli MFA uygulamanızın tüm Kullanıcı hesaplarını mı yoksa yalnızca bazılarını mı kapsamadığını anlayın. Bazı MFA çözümleri ilke tabanlıdır ve Kullanıcı dışlamasını destekler, diğerleri ise Kullanıcı başına MFA 'yı açıkça etkinleştirmenizi isteyebilir. Geçerli MFA uygulamanızdan herhangi bir kullanıcıyı dışmadığından emin olun. Dahil edilen ve CSP ile ilgili herhangi bir etkinliği gerçekleştirmek üzere Iş Ortağı Merkezi 'nde oturum açan herhangi bir kullanıcı hesabı, ölçümlerin %100 olmasına neden olabilir.

### <a name="is-mfa-only-required-when-certain-conditions-are-met"></a>MFA yalnızca belirli koşullar karşılandığında gereklidir mi?

Geçerli uygulamanızın yalnızca belirli koşullar altında MFA 'ya uygulanıp zormadığını anlayın. Bazı MFA çözümleri, yalnızca belirli koşullar karşılandığında MFA 'yı zorlamak için esneklik sağlar. Örneğin, Kullanıcı bilinmeyen cihazdan veya bilinmeyen bir konumdan erişiyor. MFA için etkinleştirilen ancak Iş Ortağı Merkezi 'ne erişirken MFA doğrulamasını tamamlamaya gerek duyulmayan bir Kullanıcı, ölçümlerin %100 olmaması halinde neden olabilir.

>[!NOTE]
>Azure AD güvenlik varsayılanlarını kullanarak MFA uygulamış olan iş ortakları için yönetici olmayan kullanıcı hesapları için çok faktörlü kimlik doğrulamasının risk temelinde zorlanacağını unutmayın. Kullanıcılardan yalnızca riskli oturum açma girişimleri (örneğin, Kullanıcı farklı bir konumdan oturum açması) sırasında MFA sorulur. Ayrıca, kullanıcıların MFA 'ya kaydolması 14 güne kadar olacaktır. MFA kaydını tamammayan kullanıcılara, 14 günlük süre boyunca MFA doğrulaması uygulanmaz. Bu nedenle, Azure AD güvenlik varsayılanlarını kullanarak MFA uygulamış olan iş ortakları için ölçümlerin %100 olmaması beklenmektedir.

### <a name="are-you-using-third-party-mfa-solution"></a>Üçüncü taraf MFA çözümünü mi kullanıyorsunuz?

Üçüncü taraf MFA çözümünü kullanıyorsanız, bunu Azure AD ile nasıl tümleştirirsiniz. Genel olarak, Federasyon ve özel denetimler dahil olmak üzere iki yöntem vardır:

* **Kimlik Federasyonu** -Azure AD bir kimlik doğrulama isteği aldığında, Azure AD kimlik doğrulaması için kullanıcıyı federal kimlik sağlayıcısına yönlendirir. Kimlik doğrulaması başarılı olduğunda, Federasyon kimlik sağlayıcısı kullanıcıyı bir SAML belirteci ile birlikte Azure AD 'ye yeniden yönlendirir. Azure AD 'nin federal kimlik sağlayıcısı 'nda kimlik doğrulanırken MFA doğrulamasını tamamladığını tanıması için, SAML belirtecinin *authenticationmethodsreferences* talebini ( *multipleauthn* değeri ile) içermesi gerekir. Federal Kimlik sağlayıcısının böyle bir talebi vermeyi destekleyip desteklemediğini denetleyin. Bu durumda, federal kimlik sağlayıcısının bu şekilde yapılandırılıp yapılandırılmadığını denetleyin. Talep yoksa, Azure AD (ve dolayısıyla Iş Ortağı Merkezi), kullanıcının MFA doğrulamasını tamamladığını ve 100 talebin eksik olduğunu bilmez.

* **Özel denetim** -Azure AD özel denetimi, bir kullanıcının bir üçüncü taraf MFA çözümü aracılığıyla MFA doğrulamasını tamamlayıp tamamlamadığınızı belirlemek için kullanılamaz. Sonuç olarak, özel bir denetim aracılığıyla MFA doğrulamasını tamamlamış olan tüm kullanıcılar, her zaman Azure AD 'ye (ve Iş Ortağı Merkezi 'nde), MFA doğrulaması tamamlanmayacak şekilde görünür. Mümkün olduğunda, Azure AD ile tümleştirilirken özel denetim yerine Kimlik Federasyonu kullanmaya geçmeniz önerilir.

### <a name="identify-which-users-have-logged-into-partner-center-without-mfa"></a>MFA olmadan Iş Ortağı Merkezi 'Nde oturum açan kullanıcıları belirler

MFA doğrulaması olmadan Iş Ortağı Merkezi 'nde oturum açan kullanıcıları belirlemek ve bunları geçerli MFA uygulamanıza karşı doğrulamak faydalı olabilir. [Azure AD oturum açma raporunu](/azure/active-directory/reports-monitoring/concept-sign-ins) , BIR kullanıcının MFA doğrulamasını tamamlayıp tamamlamadığınızı öğrenmek için kullanabilirsiniz. Azure AD oturum açma raporu şu anda yalnızca Azure AD Premium abone olan iş ortakları veya Azure AD Premium (örneğin, EMS) içeren O365 SKU 'sunda kullanılabilir.

## <a name="next-steps"></a>Sonraki adımlar

- [İş Ortağı Merkezi Güvenlik Kılavuzu grubu topluluğu](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [İş Ortağı Merkezi güvenlik gereksinimleri](partner-security-requirements.md)
- [İş Ortağı Merkezi güvenlik gereksinimleri SSS](partner-security-requirements-faq.md)