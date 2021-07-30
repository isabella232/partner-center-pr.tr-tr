---
title: Güvenlik gereksinimleri durum raporu
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
description: Güvenlik gereksinimleri durum raporu ve Iş Ortağı Merkezi MFA raporuyla güvenlik gereksinimlerinizin uyumluluğunu nasıl denetleyeceğinizi öğrenin
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: db558062f5dab2a3f9ffbe99f7122a436f89d21f
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114844556"
---
# <a name="security-requirements-status-report"></a>Güvenlik gereksinimleri durum raporu

**Uygun roller**: CPV Yöneticisi | Genel yönetici

Bu makalede, Iş Ortağı Merkezi 'nde güvenlik gereksinimleri durum raporu açıklanır. Bu rapor, iş ortağı kiracınızdaki kullanıcılar için Multi-Factor Authentication (MFA) için [iş ortağı güvenlik gereksinimleriyle](partner-security-requirements.md) uyumluluk açısından ölçümler sunar.

[iş ortağı merkezi](https://partner.microsoft.com/dashboard)'nde bu rapora erişmek için **Ayarlar**  >  **hesap ayarları**  >  **güvenlik gereksinimlerinin durumu**' na gidin. Rapor günlük olarak güncelleştirilir ve son yedi gündeki oturum açma verilerini yansıtır.

>[!NOTE]
>Güvenlik gereksinimleri durum raporu yalnızca Iş Ortağı Merkezi 'nde desteklenir. Microsoft Cloud for US Government veya almanya Microsoft Bulut kullanılamaz. Bir sogeign bulutu üzerinden deneyimidir tüm iş ortaklarının (ABD devlet ve Almanya) bu yeni güvenlik gereksinimlerini hemen benimsemesini önemle öneririz. Ancak, bu iş ortaklarının yeni güvenlik gereksinimlerini karşılamak için şu anda gerekli değildir. Microsoft, daha sonra da bu güvenlik gereksinimlerinin zorlanmasıyla ilgili ek ayrıntılar sağlar.

## <a name="security-status-metrics"></a>Güvenlik durumu ölçümleri

Güvenlik gereksinimleri durum raporu, iş ortağı MFA uygulamasıyla ilgili öngörüler sunar ve iş ortağı kiracılarında MFA yapılandırması ve Iş Ortağı Merkezi etkinlikleri hakkında ölçümler sağlar. Aşağıdaki bölümlerde bu ölçümler daha ayrıntılı olarak açıklanmaktadır.

### <a name="mfa-configuration-on-a-partner-tenant"></a>Bir iş ortağı kiracısında MFA yapılandırması

**MFA ile etkinleştirilen kullanıcı hesaplarının ölçüm yüzdesi, burada listelenen seçenekler kullanılarak zorlandı:** iş ortağı kiracınızda MFA 'ya zorlanan etkin kullanıcı hesaplarının yüzdesini gösterir. Uyumluluk elde etmek için bu [MFA seçeneklerinden](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) birini kullanabilirsiniz. Bu veriler, günlük olarak yakalanır ve raporlanır. Örneğin:

- Contoso, kiracıda 110 Kullanıcı hesabı olan bir CSP iş ortağıdır, bu kullanıcı hesaplarının 10 ' u devre dışı bırakılır. 
- 100 Kullanıcı hesabının geri kalanında 90, sunulan [MFA seçenekleri](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started)kullanılarak MFA 'ya zorlanır. Bu nedenle, ölçüm %90 gösterir. 

### <a name="partner-center-requests-with-mfa"></a>MFA ile iş ortağı merkezi istekleri

Çalışanlarınıza iş ortağı merkezi 'nde çalışan veya API 'Ler aracılığıyla veri gönderen her oturum açışınızda, güvenlik durumu ne olur ve izlenir. Ayrıca, güvenlik-durum izlemede de yer alan Uygulamalarınız ve tüm Denetim Masası satıcı uygulamalardır. Bu veriler, **MFA Ile Iş Ortağı Merkezi 'ne yapılan Isteklerin yüzdesi** altında ölçümler bölümünde gösterilir ve son yedi günü yansıtır.

#### <a name="dashboard-mfa-verification"></a>Pano MFA doğrulaması

**Iş Ortağı Merkezi portalındaki** ölçüm, Iş Ortağı Merkezi panosu dahilinde etkinliklerle ilgilidir. MFA doğrulamasını tamamlayan kullanıcılar tarafından yapılan işlemlerin yüzdesini ölçer. Örneğin:

- Contoso, kemal ve John olmak üzere iki yönetici aracısına sahip bir CSP iş ortağıdır.
- İlk gün, Gamze doğrulaması olmadan Iş Ortağı Merkezi panosunda oturum açtı ve üç işlem yaptı.
- İkinci günde John, MFA doğrulaması olmadan Iş Ortağı Merkezi panosunda oturum açtı ve beş işlem yaptı.
- Üçüncü günde, Gamze, MFA doğrulaması ile Iş Ortağı Merkezi panosunda oturum açtı ve iki işlem yaptı.
- Kalan dört gün içinde herhangi bir aracı tarafından bir işlem yapılmadı.
- Yedi günlük pencerede yapılan 10 işlemden sonra, MFA doğrulaması ile Kullanıcı tarafından iki tanesi yapılmıştır. Bu nedenle, ölçüm %20 ' yi gösterir.

Iş Ortağı Merkezi panosunda MFA doğrulaması yapmadan hangi kullanıcının oturum açtığını ve raporlama penceresi sırasında en son ziyaret zamanını anlamak için **MFA olmadan dosya portalı isteklerini** kullanın.

#### <a name="appuser-mfa-verification"></a>Uygulama + Kullanıcı MFA doğrulaması

**API veya SDK aracılığıyla** ölçüm, Iş Ortağı Merkezi API Istekleri aracılığıyla App + kullanıcı kimlik doğrulaması ile ilgilidir. MFA talebine sahip bir erişim belirteci kullanılarak yapılan API isteklerinin yüzdesini ölçer. Örneğin:

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

Uyumluluğa ulaşmak için iş ortağı kiracınız için MFA uygulamanız gerekir. MFA 'yı uygulama hakkında daha fazla bilgi için bkz. [Iş ortağı merkezi veya Iş Ortağı Merkezi API 'leri kullanma Için güvenlik gereksinimleri](partner-security-requirements.md).

>[!NOTE]
> MFA ölçümleri günlük olarak hesaplanır ve son yedi gün içinde gerçekleştirilen hesap işlemlerini alır. İş ortağı kiracınız için yalnızca en son MFA uygulamasını tamamladıysanız ölçümler henüz %100 ' ı gösteremeyebilir.

### <a name="verify-mfa-on-all-user-accounts"></a>Tüm Kullanıcı hesaplarında MFA 'yı doğrula

Geçerli MFA uygulamanızın tüm Kullanıcı hesaplarını mı yoksa yalnızca bazılarını mı kapsamadığını anlayın. Bazı MFA çözümleri ilke tabanlıdır ve Kullanıcı dışlamasını destekler, diğerleri ise Kullanıcı başına MFA 'yı açıkça etkinleştirmenizi isteyebilir. Geçerli MFA uygulamanızdan herhangi bir kullanıcıyı dışmadığından emin olun. Tüm CSP, CPV veya danışman ile ilgili etkinlikleri gerçekleştirmek üzere Iş Ortağı Merkezi 'nde dışlanan ve oturum açan herhangi bir kullanıcı hesabı ölçümlerin %100 olmasına neden olabilir.

### <a name="review-your-mfa-conditions"></a>MFA koşullarınızı gözden geçirin

Geçerli uygulamanızın yalnızca belirli koşullar altında MFA 'ya uygulanıp zormadığını anlayın. Bazı MFA çözümleri, yalnızca belirli koşullar karşılandığında MFA 'yı zorlamak için esneklik sağlar. Örneğin, Kullanıcı bilinmeyen cihazdan veya bilinmeyen bir konumdan erişiyor. MFA için etkinleştirilen ancak Iş Ortağı Merkezi 'ne erişirken MFA doğrulamasını tamamlamaya gerek duyulmayan bir Kullanıcı, ölçümlerin %100 olmaması halinde neden olabilir.

>[!NOTE]
>Azure AD güvenlik varsayılanlarını kullanarak MFA uygulamış olan iş ortakları için yönetici olmayan kullanıcı hesapları için çok faktörlü kimlik doğrulamasının risk temelinde zorlanacağını unutmayın. Kullanıcılardan yalnızca riskli oturum açma girişimleri (örneğin, Kullanıcı farklı bir konumdan oturum açması) sırasında MFA sorulur. Ayrıca, kullanıcıların MFA 'ya kaydolması 14 güne kadar olacaktır. MFA kaydını tamammayan kullanıcılara, 14 günlük süre boyunca MFA doğrulaması uygulanmaz. Bu nedenle, Azure AD güvenlik varsayılanlarını kullanarak MFA uygulamış olan iş ortakları için ölçümlerin %100 olmaması beklenmektedir.

### <a name="review-third-party-mfa-configurations"></a>Üçüncü taraf MFA yapılandırmasını gözden geçirme

Üçüncü taraf MFA çözümünü kullanıyorsanız, bunu Azure AD ile nasıl tümleştirirsiniz. Genel olarak, Federasyon ve özel denetimler dahil olmak üzere iki yöntem vardır:

* **Kimlik Federasyonu** -Azure AD bir kimlik doğrulama isteği aldığında, Azure AD kimlik doğrulaması için kullanıcıyı federal kimlik sağlayıcısına yönlendirir. Kimlik doğrulaması başarılı olduğunda, Federasyon kimlik sağlayıcısı kullanıcıyı bir SAML belirteci ile birlikte Azure AD 'ye yeniden yönlendirir. Azure AD 'nin federal kimlik sağlayıcısı 'nda kimlik doğrulanırken MFA doğrulamasını tamamladığını tanıması için, SAML belirtecinin *authenticationmethodsreferences* talebini ( *multipleauthn* değeri ile) içermesi gerekir. Federal Kimlik sağlayıcısının böyle bir talebi vermeyi destekleyip desteklemediğini denetleyin. Bu durumda, federal kimlik sağlayıcısının bu şekilde yapılandırılıp yapılandırılmadığını denetleyin. Talep yoksa, Azure AD (ve dolayısıyla Iş Ortağı Merkezi), kullanıcının MFA doğrulamasını tamamladığını ve 100 talebin eksik olduğunu bilmez.

* **Özel denetim** -Azure AD özel denetimi, bir kullanıcının bir üçüncü taraf MFA çözümü aracılığıyla MFA doğrulamasını tamamlayıp tamamlamadığınızı belirlemek için kullanılamaz. Sonuç olarak, özel bir denetim aracılığıyla MFA doğrulamasını tamamlamış olan tüm kullanıcılar, her zaman Azure AD 'ye (ve Iş Ortağı Merkezi 'nde), MFA doğrulaması tamamlanmayacak şekilde görünür. Mümkün olduğunda, Azure AD ile tümleştirilirken özel denetim yerine Kimlik Federasyonu kullanmaya geçmeniz önerilir.

### <a name="identify-which-users-have-signed-in-to-partner-center-without-mfa"></a>MFA olmadan Iş Ortağı Merkezi 'nde oturum açan kullanıcıları belirler

MFA doğrulaması olmadan Iş Ortağı Merkezi 'nde oturum açan kullanıcıları belirlemek ve bunları geçerli MFA uygulamanıza karşı doğrulamak faydalı olabilir. [Azure AD oturum açma raporunu](/azure/active-directory/reports-monitoring/concept-sign-ins) , BIR kullanıcının MFA doğrulamasını tamamlayıp tamamlamadığınızı öğrenmek için kullanabilirsiniz. Azure AD oturum açma raporu şu anda yalnızca Azure AD Premium abone olan iş ortakları veya Azure AD Premium (örneğin, EMS) içeren O365 SKU 'sunda kullanılabilir.

## <a name="next-steps"></a>Sonraki adımlar

- [İş Ortağı Merkezi Güvenlik Kılavuzu grubu topluluğu](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [İş Ortağı Merkezi güvenlik gereksinimleri](partner-security-requirements.md)
- [İş Ortağı Merkezi güvenlik gereksinimleri SSS](partner-security-requirements-faq.yml)
