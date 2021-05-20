---
title: Güvenlik gereksinimleri durum raporu
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Güvenlik gereksinimleri durum raporu ve Iş Ortağı Merkezi MFA raporuyla güvenlik gereksinimlerinizin uyumluluğunu nasıl denetleyeceğinizi öğrenin
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: c9bba02744d466741d7625b1624995084c0a3492
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152571"
---
# <a name="security-requirements-status-report"></a>Güvenlik gereksinimleri durum raporu

**Uygun roller**: CPV Yöneticisi | Genel yönetici

Bu makalede, Iş Ortağı Merkezi 'nde güvenlik gereksinimleri durum raporu açıklanır. Bu rapor, iş ortağı kiracınızdaki kullanıcılar için Multi-Factor Authentication (MFA) için [iş ortağı güvenlik gereksinimleriyle](partner-security-requirements.md) uyumluluk açısından ölçümler sunar.

[İş ortağı merkezi](https://partner.microsoft.com/dashboard)'nde bu rapora erişmek için **Ayarlar**  >  **Hesap ayarları**  >  **güvenlik gereksinimleri durum**' a gidin. Rapor günlük olarak güncelleştirilir ve son yedi gündeki oturum açma verilerini yansıtır.

>[!NOTE]
>Güvenlik gereksinimleri durum raporu yalnızca Iş Ortağı Merkezi 'nde desteklenir. ABD devlet veya Microsoft Bulut Almanya için Microsoft Bulut kullanılamaz. Bir sogeign bulutu üzerinden deneyimidir tüm iş ortaklarının (ABD devlet ve Almanya) bu yeni güvenlik gereksinimlerini hemen benimsemesini önemle öneririz. Ancak, bu iş ortaklarının yeni güvenlik gereksinimlerini karşılamak için şu anda gerekli değildir. Microsoft, daha sonra da bu güvenlik gereksinimlerinin zorlanmasıyla ilgili ek ayrıntılar sağlar.

## <a name="security-status-metrics"></a>Güvenlik durumu ölçümleri

Güvenlik gereksinimleri durum raporu, iş ortağı MFA uygulamasıyla ilgili öngörüler sunar ve iş ortağı kiracılarında MFA yapılandırması ve Iş Ortağı Merkezi etkinlikleri hakkında ölçümler sağlar. Aşağıdaki bölümlerde bu ölçümler daha ayrıntılı olarak açıklanmaktadır.

### <a name="mfa-configuration-on-a-partner-tenant"></a>Bir iş ortağı kiracısında MFA yapılandırması

**MFA ile etkinleştirilen kullanıcı hesaplarının ölçüm yüzdesi, burada listelenen seçenekler kullanılarak zorlandı:** iş ortağı kiracınızda MFA 'ya zorlanan etkin kullanıcı hesaplarının yüzdesini gösterir. Uyumluluk elde etmek için bu [MFA seçeneklerinden](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) birini kullanabilirsiniz. Bu veriler, günlük olarak yakalanır ve raporlanır. Örnek:

- Contoso kiracıda 110 kullanıcı hesabına sahip bir CSP iş ortağıdır ve bu kullanıcı hesaplarından 10'ları devre dışı bırakılmıştır. 
- 100 kullanıcı hesabının geri kalanında, sağlanan MFA seçenekleri kullanılarak 90 [MFA uygulanır.](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) Bu nedenle ölçüm %90 gösteriyor. 

### <a name="partner-center-requests-with-mfa"></a>İş Ortağı Merkezi MFA ile istekler

Çalışanlarınız çalışmak için İş Ortağı Merkezi API'ler aracılığıyla veri almak veya göndermek için her oturum İş Ortağı Merkezi güvenlik durumlarıyla ilgili bir zorlukla karşı karşıyadır ve takiptedir. Uygulamalarınız ve denetim masası satıcı uygulamaları, güvenlik durumu izlemesine de dahildir. Bu veriler, **MFA** ile yapılan İş Ortağı Merkezi yüzdesi altındaki ölçümlerde gösterilir ve son yedi günü yansıtıyor.

#### <a name="dashboard-mfa-verification"></a>Pano MFA doğrulaması

İş Ortağı Merkezi **portalı üzerinden ölçüm,** panonun içindeki etkinliklerle İş Ortağı Merkezi olur. MFA doğrulamayı tamamlayan kullanıcılar tarafından yapılan işlemlerin yüzdesini ölçür. Örnek:

- Contoso, Jane ve John adlı iki yönetici aracıya sahip bir CSP iş ortağıdır.
- İlk gün Jane, MFA doğrulaması olmadan İş Ortağı Merkezi panoda oturum açtı ve üç işlem yaptı.
- İkinci gün John, MFA doğrulaması olmadan İş Ortağı Merkezi panoda oturum açtı ve beş işlem yaptı.
- Üçüncü günde Jane, MFA doğrulaması ile İş Ortağı Merkezi panoda oturum açtı ve iki işlem yaptı.
- Kalan dört gün içinde iki aracı tarafından da herhangi bir işlem yoktu.
- Yedi günlük pencerede yapılan 10 işlemden ikisi kullanıcı tarafından MFA doğrulaması ile yapıldı. Bu nedenle ölçüm %20 gösteriyor.

**MFA doğrulamasına sahip** olmadan hangi kullanıcının İş Ortağı Merkezi panosunda oturum açtığını ve raporlama penceresi sırasında son ziyaret zamanını anlamak için MFA olmadan portal isteklerini kullanın.

#### <a name="appuser-mfa-verification"></a>Uygulama+Kullanıcı MFA doğrulaması

API veya **SDK aracılığıyla ölçüm, API** istekleri aracılığıyla App+User İş Ortağı Merkezi ilgilidir. MFA talebine sahip bir erişim belirteci kullanılarak yapılan API isteklerinin yüzdesini ölçer. Örnek:

- Fabrikam bir CSP iş ortağıdır ve App + kullanıcı kimlik doğrulaması ve yalnızca uygulama kimlik doğrulama yöntemlerinin bir karışımını kullanan bir CSP uygulamasına sahiptir.
- İlk günde uygulama, MFA doğrulaması olmadan uygulama + kullanıcı kimlik doğrulama yöntemi aracılığıyla elde edilen bir erişim belirteciyle desteklenen üç API isteği yaptı.
- İkinci gün, uygulama yalnızca uygulama kimlik doğrulaması kullanılarak edinilen bir erişim belirteciyle desteklenen beş API isteği yaptı.
- Üçüncü günde uygulama, MFA doğrulaması ile App + kullanıcı kimlik doğrulama yöntemi kullanılarak edinilen bir erişim belirteciyle desteklenen iki API isteği yaptı.
- Kalan dört gün içinde herhangi bir aracı tarafından bir işlem yapılmadı.
- İkinci gün üzerindeki beş API isteği, yalnızca uygulama kimlik doğrulaması aracılığıyla elde edilen bir erişim belirteci tarafından desteklenen, Kullanıcı kimlik bilgilerini kullanmadığından ölçüden çıkarılır. Kalan beş işlemin dışında, bunların ikisi MFA doğrulaması ile elde edilen bir erişim belirteciyle destekleniyor. Bu nedenle, ölçüm %40 gösterir.

Bu ölçüm üzerinde %100 olmayan bir uygulama ve Kullanıcı etkinliği olduğunu anlamak istiyorsanız, dosyaları kullanın:

- API, uygulamanın genel MFA durumunu anlamak için **Özet ister** .
- **Tüm API** istekleri kiracınızın kullanıcıları tarafından YAPıLAN her API isteğinin ayrıntılarını anlamak için, sonuç daha iyi indirme deneyimi için en çok 10.000 en son istek ile sınırlıdır.

## <a name="actions-for-mfa-status-below-100"></a>MFA durumu eylemleri %100 altında

MFA 'yı uygulayan bazı iş ortakları rapor ölçümlerini %100 oranında görebilirler. Nedenini anlamak için göz önünde bulundurmanız gereken bazı etmenler aşağıda verilmiştir.

> [!NOTE]
> Kuruluşunuz tarafından iş ortağı kiracınızın kimlik yönetimi ve MFA uygulamasıyla ilgili bilgi sahibi olan bir kişi ile çalışmanız gerekir.

### <a name="implemented-mfa-for-your-partner-tenant"></a>İş ortağı kiracınız için MFA uygulandı

Uyumluluğa ulaşmak için iş ortağı kiracınız için MFA uygulamanız gerekir. MFA uygulama hakkında ayrıntılı bilgi için bkz. İş Ortağı Merkezi veya [İş Ortağı Merkezi api'lerini kullanmaya yönelik güvenlik gereksinimleri.](partner-security-requirements.md)

>[!NOTE]
> MFA ölçümleri günlük olarak hesaplanır ve son yedi gün içinde gerçekleştirilen işlemleri dikkate alır. İş ortağı kiracınız için MFA uygulamasını yalnızca yakın zamanda tamamladıysanız, ölçümler henüz %100 göstereyem olabilir.

### <a name="verify-mfa-on-all-user-accounts"></a>Tüm kullanıcı hesaplarından MFA'nın doğrula

Geçerli MFA uygulamanın tüm kullanıcı hesaplarını mı yoksa yalnızca bir hesabı mı kapsıyor olduğunu anlama. Bazı MFA çözümleri ilke tabanlıdır ve kullanıcı dışlama desteği sunarken, diğerleri MFA'yi kullanıcı başına açıkça etkinleştirmeniz gerektirmektedir. Geçerli MFA uygulamanıza hiçbir kullanıcı dışlamamanızı doğrulayın. CsP, CPV veya Advisor ile ilgili herhangi bir İş Ortağı Merkezi gerçekleştirmek üzere dışlanan ve oturum açtığı tüm kullanıcı hesapları, ölçümlerin %100'e varmama durumuna neden olabilir.

### <a name="review-your-mfa-conditions"></a>MFA koşullarınızı gözden geçirme

Geçerli uygulamanın yalnızca belirli koşullar altında MFA'nın zorunlu olup olmadığını anlama. Bazı MFA çözümleri, MFA'nın yalnızca belirli koşullar karşılanan durumlarda zorunlu kılınma esnekliği sağlar. Örneğin, kullanıcı bilinmeyen cihazdan veya bilinmeyen konumdan erişmektedir. MFA için etkinleştirilen ancak İş Ortağı Merkezi'a erişirken MFA doğrulamayı tamamlaması gerek olmayan bir kullanıcı, ölçümlerin %100'e ulaşmama durumuna neden olabilir.

>[!NOTE]
>Azure AD güvenlik varsayılanlarını kullanarak MFA uygulayan iş ortakları için, yönetici olmayan kullanıcı hesapları için risk tabanlı çok faktörlü kimlik doğrulamasının zorunlu tutulacaklarını unutmayın. Kullanıcılardan yalnızca riskli oturum açma denemeleri sırasında MFA istenir (örneğin, kullanıcının farklı bir konumdan oturum açması). Ayrıca, kullanıcıların MFA'ya kaydolması en fazla 14 gün sürer. MFA kaydını tamamlayan kullanıcılardan 14 günlük süre boyunca MFA doğrulamasına sahip olması zorlanmaz. Bu nedenle, Azure AD güvenlik varsayılanlarını kullanarak MFA uygulayan iş ortakları için ölçümlerin %100 olması beklenmiyor olabilir.

### <a name="review-third-party-mfa-configurations"></a>Üçüncü taraf MFA yapılandırmalarını gözden geçirme

Üçüncü taraf MFA çözümünü kullanıyorsanız, bunu Azure AD ile nasıl tümleştirirsiniz. Genel olarak, Federasyon ve özel denetimler dahil olmak üzere iki yöntem vardır:

* **Kimlik Federasyonu** -Azure AD bir kimlik doğrulama isteği aldığında, Azure AD kimlik doğrulaması için kullanıcıyı federal kimlik sağlayıcısına yönlendirir. Kimlik doğrulaması başarılı olduğunda, Federasyon kimlik sağlayıcısı kullanıcıyı bir SAML belirteci ile birlikte Azure AD 'ye yeniden yönlendirir. Azure AD 'nin federal kimlik sağlayıcısı 'nda kimlik doğrulanırken MFA doğrulamasını tamamladığını tanıması için, SAML belirtecinin *authenticationmethodsreferences* talebini ( *multipleauthn* değeri ile) içermesi gerekir. Federal Kimlik sağlayıcısının böyle bir talebi vermeyi destekleyip desteklemediğini denetleyin. Bu durumda, federal kimlik sağlayıcısının bu şekilde yapılandırılıp yapılandırılmadığını denetleyin. Talep yoksa, Azure AD (ve dolayısıyla Iş Ortağı Merkezi), kullanıcının MFA doğrulamasını tamamladığını ve 100 talebin eksik olduğunu bilmez.

* **Özel denetim** -Azure AD özel denetimi, bir kullanıcının bir üçüncü taraf MFA çözümü aracılığıyla MFA doğrulamasını tamamlayıp tamamlamadığınızı belirlemek için kullanılamaz. Sonuç olarak, özel bir denetim aracılığıyla MFA doğrulamasını tamamlamış olan tüm kullanıcılar, her zaman Azure AD 'ye (ve Iş Ortağı Merkezi 'nde), MFA doğrulaması tamamlanmayacak şekilde görünür. Mümkün olduğunda, Azure AD ile tümleştirilirken özel denetim yerine Kimlik Federasyonu kullanmaya geçmeniz önerilir.

### <a name="identify-which-users-have-signed-in-to-partner-center-without-mfa"></a>MFA olmadan Iş Ortağı Merkezi 'nde oturum açan kullanıcıları belirler

MFA doğrulaması olmadan Iş Ortağı Merkezi 'nde oturum açan kullanıcıları belirlemek ve bunları geçerli MFA uygulamanıza karşı doğrulamak faydalı olabilir. [Azure AD oturum açma raporunu](/azure/active-directory/reports-monitoring/concept-sign-ins) , BIR kullanıcının MFA doğrulamasını tamamlayıp tamamlamadığınızı öğrenmek için kullanabilirsiniz. Azure AD oturum açma raporu şu anda yalnızca Azure AD Premium veya herhangi bir O365 SKU's una (emS gibi) abone Azure AD Premium iş ortakları tarafından kullanılabilir.

## <a name="next-steps"></a>Sonraki adımlar

- [İş Ortağı Merkezi rehberlik grubu topluluğu](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [İş Ortağı Merkezi güvenlik gereksinimleri](partner-security-requirements.md)
- [İş Ortağı Merkezi gereksinimleri hakkında SSS](partner-security-requirements-faq.md)
