---
title: Güvenlik gereksinimleri durum raporu
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Güvenlik gereksinimleri durum raporu ve MFA raporuyla uyumluluk durumunu denetlemeyi İş Ortağı Merkezi öğrenin
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: cfdb409b844d2e304a61654cbea144f9f1d14350
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129071752"
---
# <a name="security-requirements-status-report"></a>Güvenlik gereksinimleri durum raporu

**Uygun roller:** CPV yönetici | Genel yönetici

Bu makalede, İş Ortağı Merkezi'daki güvenlik gereksinimleri durum raporu açıklanmıştır. Bu rapor, iş ortağı kiracınız kullanıcıları [için çok](partner-security-requirements.md) faktörlü kimlik doğrulaması (MFA) için iş ortağı güvenlik gereksinimleriyle uyumluluk ölçümleri sağlar.

Bu rapora İş Ortağı Merkezi [için,](https://partner.microsoft.com/dashboard)Ayarlar dişli simgesini ve ardından Hesap **ayarları'nın** ardından **Güvenlik gereksinimleri durumunu seçin.** Rapor günlük olarak güncelleştirilir ve son yedi günün oturum açma verilerini yansıtıyor.

>[!NOTE]
>Güvenlik gereksinimleri durum raporu yalnızca İş Ortağı Merkezi. Microsoft Bulut Almanya'da Microsoft Cloud for US Government kullanılamaz. Bağımsız bir bulut (ABD Kamu ve Almanya) aracılığıyla işlem yapılan tüm iş ortaklarının bu yeni güvenlik gereksinimlerini hemen benimsemelerini kesinlikle öneririz. Ancak, bu iş ortaklarının şu anda yeni güvenlik gereksinimlerini karşılaması gerekli değildir. Microsoft, gelecekte bağımsız bulutlar için bu güvenlik gereksinimlerini uygulamayla ilgili ek ayrıntılar sağlayacaktır.

## <a name="security-status-metrics"></a>Güvenlik durumu ölçümleri

Güvenlik gereksinimleri durum raporu, iş ortağı MFA uygulamasıyla ilgili içgörüler sunar ve iş ortağı kiracıları üzerinde MFA yapılandırması ve İş Ortağı Merkezi etkinliklerine yönelik ölçümler sağlar. Aşağıdaki bölümlerde bu ölçümler daha ayrıntılı olarak açıklanmaktadır.

### <a name="mfa-configuration-on-a-partner-tenant"></a>İş ortağı kiracısı üzerinde MFA yapılandırması

Burada listelenen seçenekler kullanılarak MFA ile zorunlu kılınan etkin kullanıcı hesaplarının yüzdesi **ölçümü: MFA'nın** zorunlu olduğu iş ortağı kiracınız üzerinde etkin kullanıcı hesaplarının yüzdesini gösterir. Uyumluluk elde etmek için bu [MFA seçeneklerden](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) birini kullanabilirsiniz. Bu veriler günlük olarak yakalanır ve raporlanır. Örnek:

- Contoso kiracıda 110 kullanıcı hesabına sahip bir CSP iş ortağıdır ve bu kullanıcı hesaplarından 10'ları devre dışı bırakılmıştır. 
- Kalan 100 kullanıcı hesabından 90'ı, sağlanan MFA seçenekleri kullanılarak [MFA uygulanır.](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) Bu nedenle ölçüm %90 gösteriyor. 

### <a name="partner-center-requests-with-mfa"></a>İş Ortağı Merkezi MFA ile istekler

Çalışanlarınız çalışmak için İş Ortağı Merkezi API'ler aracılığıyla veri almak veya göndermek için her oturum İş Ortağı Merkezi durumunda güvenlik durumları isteniyor ve takip ediyor. Ayrıca, uygulamalarınız ve denetim masası satıcı uygulamaları, güvenlik durumu izlemesine de dahildir. Bu veriler, **MFA** ile İş Ortağı Merkezi yüzdesi altındaki ölçümlerde gösterilir ve son yedi günü yansıtıyor.

#### <a name="dashboard-mfa-verification"></a>Pano MFA doğrulaması

İş Ortağı Merkezi **portalı üzerinden ölçüm,** panonun içindeki etkinliklerle İş Ortağı Merkezi olur. MFA doğrulamayı tamamlayan kullanıcılar tarafından yapılan işlemlerin yüzdesini ölçür. Örnek:

- Contoso, Jane ve John adlı iki yönetici aracıya sahip bir CSP iş ortağıdır.
- İlk gün Jane, MFA doğrulaması olmadan İş Ortağı Merkezi panoda oturum açtı ve üç işlem yaptı.
- İkinci gün John, MFA doğrulaması olmadan İş Ortağı Merkezi panoda oturum açtı ve beş işlem yaptı.
- Üçüncü günde Jane, MFA doğrulaması ile İş Ortağı Merkezi panoda oturum açtı ve iki işlem yaptı.
- Kalan dört gün içinde herhangi bir aracı tarafından hiçbir işlem yoktu.
- Yedi günlük pencerede yapılan 10 işlemden ikisi kullanıcı tarafından MFA doğrulaması ile yapıldı. Bu nedenle ölçüm %20 gösteriyor.

**MFA doğrulamasına sahip** olmadan hangi kullanıcının İş Ortağı Merkezi panosunda oturum açtığını ve raporlama penceresi sırasında son ziyaret zamanını anlamak için MFA olmadan portal isteklerini kullanın.

#### <a name="appuser-mfa-verification"></a>Uygulama+Kullanıcı MFA doğrulaması

API veya **SDK aracılığıyla ölçüm, API** istekleri aracılığıyla App+User İş Ortağı Merkezi ilgilidir. MFA talebiyle erişim belirteci kullanılarak yapılan API isteklerinin yüzdesini ölçür. Örnek:

- Fabrikam bir CSP iş ortağıdır ve App+User kimlik doğrulaması ile yalnızca uygulama kimlik doğrulama yöntemlerinin bir karışımını kullanan bir CSP uygulamasına sahip.
- İlk gün, uygulama MFA doğrulaması olmadan App+User kimlik doğrulama yöntemi aracılığıyla alınan bir erişim belirteci tarafından desteklene üç API isteğinde bulundu.
- İkinci gün, uygulama yalnızca Uygulama kimlik doğrulaması kullanılarak alınan bir erişim belirteci tarafından desteklene beş API isteği yaptı.
- Üçüncü gün, uygulama MFA doğrulaması ile App+User kimlik doğrulama yöntemi kullanılarak alınan bir erişim belirteci tarafından desteklene iki API isteğinde bulundu.
- Kalan dört gün içinde herhangi bir aracı tarafından hiçbir işlem yoktu.
- İkinci gün, yalnızca Uygulama kimlik doğrulaması aracılığıyla alınan bir erişim belirteci tarafından desteklene beş API isteği, kullanıcı kimlik bilgilerini kullanmamalarından ölçümden atlanır. Kalan beş işlemden ikisi, MFA doğrulaması ile alınan bir erişim belirteci tarafından desteklemektedir. Bu nedenle ölçüm %40 gösteriyor.

Hangi Uygulama+kullanıcı etkinliklerinin bu ölçümde %100 olmayan bir sonuç elde etmek zorunda olduğunu anlamak için dosyaları kullanın:

- **Uygulamaya göre genel** MFA durumunu anlamak için API istekleri özeti.
- **Kiracınız kullanıcıları** tarafından yapılan her API isteğinin ayrıntısını anlamak için yapılan tüm API istekleri, daha iyi indirme deneyimi için en fazla 10.000 en son istekle sınırlıdır.

## <a name="actions-for-mfa-status-below-100"></a>MFA durumunun %100'den az olduğu eylemler

MFA uygulayan bazı iş ortakları rapor ölçümlerini %100'in altında görebilir. Bunun nedenlerini anlamak için göz önünde bulundurarak bazı faktörlere göz önünde bulundurarak.

> [!NOTE]
> İş ortağı kiracınız için kimlik yönetimi ve MFA uygulaması hakkında bilgi sahibi olan bir kullanıcıyla birlikte çalışmanız gerekir.

### <a name="implemented-mfa-for-your-partner-tenant"></a>İş ortağı kiracınız için MFA uygulama

İş ortağı kiracınız için uyumluluk sağlamak için MFA uygulamanız gerekir. MFA uygulama hakkında ayrıntılı bilgi için [bkz. Api'leri](partner-security-requirements.md)veya İş Ortağı Merkezi İş Ortağı Merkezi gereksinimleri.

>[!NOTE]
> MFA ölçümleri günlük olarak hesaplanır ve son yedi gün içinde gerçekleştirilen işlemleri dikkate alır. İş ortağı kiracınız için MFA uygulamasını yalnızca kısa süre önce tamamladıysanız, ölçümler henüz %100 göstereyem olabilir.

### <a name="verify-mfa-on-all-user-accounts"></a>Tüm kullanıcı hesaplarından MFA'nın doğrula

Geçerli MFA uygulamanın tüm kullanıcı hesaplarını mı yoksa yalnızca bir hesabı mı kapsıyor olduğunu anlama. Bazı MFA çözümleri ilke tabanlıdır ve kullanıcı dışlama desteği sunarken, diğerleri kullanıcı başına MFA'yi açıkça etkinleştirmeniz gerektirmektedir. Geçerli MFA uygulamanıza hiçbir kullanıcı dışlamamanızı doğrulayın. CsP, CPV veya Advisor ile ilgili herhangi bir İş Ortağı Merkezi gerçekleştirmek üzere dışlanan ve oturum açtığı tüm kullanıcı hesapları, ölçümlerin %100'e varmama durumuna neden olabilir.

### <a name="review-your-mfa-conditions"></a>MFA koşullarınızı gözden geçirme

Geçerli uygulamanın yalnızca belirli koşullar altında MFA'nın zorunlu olup olmadığını anlama. Bazı MFA çözümleri, MFA'nın yalnızca belirli koşullar karşılanan durumlarda zorunlu kılınma esnekliği sağlar. Örneğin, kullanıcı bilinmeyen cihazdan veya bilinmeyen konumdan erişmektedir. MFA için etkinleştirilen ancak İş Ortağı Merkezi'a erişirken MFA doğrulamayı tamamlaması gerek olmayan bir kullanıcı, ölçümlerin %100'e ulaşmama durumuna neden olabilir.

> [!NOTE]
> Azure AD güvenlik varsayılanlarını kullanarak MFA uygulayan iş ortakları için, yönetici olmayan kullanıcı hesapları için risk tabanlı çok faktörlü kimlik doğrulamasının zorunlu tutulacaklarını unutmayın. Kullanıcılardan yalnızca riskli oturum açma denemeleri sırasında MFA istenir (örneğin, kullanıcının farklı bir konumdan oturum açması). Ayrıca, kullanıcıların MFA'ya kaydolması en fazla 14 gün sürer. MFA kaydını tamamlayan kullanıcılardan 14 günlük süre boyunca MFA doğrulamasına sahip olması zorlanmaz. Bu nedenle, Azure AD güvenlik varsayılanlarını kullanarak MFA uygulayan iş ortakları için ölçümlerin %100 olması beklenmiyor olabilir.

### <a name="review-third-party-mfa-configurations"></a>Üçüncü taraf MFA yapılandırmalarını gözden geçirme

Üçüncü taraf MFA çözümü kullanıyorsanız, azure AD ile nasıl tümleştirildiklerini belirleme. Genel olarak, federasyon ve özel denetimler dahil olmak üzere iki yöntem vardır:

* **Kimlik federasyonu** - Azure AD bir kimlik doğrulama isteği aldığında Azure AD, kimlik doğrulaması için kullanıcıyı federasyon kimlik sağlayıcısına yeniden yönlendirecek. Başarılı bir kimlik doğrulamasının ardından, federasyon kimlik sağlayıcısı, bir SAML belirteci ile birlikte kullanıcıyı Azure AD'ye yeniden yönlendirecek. Azure AD'nin, kullanıcının federasyon kimlik sağlayıcısında kimlik doğrulamasında MFA doğrulamasını tamamlamış olduğunu tanıması için SAML belirtecin *authenticationmethodsreferences* talebi *(multipleauthn* değeriyle) içermesi gerekir. Federasyon kimlik sağlayıcısının böyle bir talep verme desteği olup olmadığını kontrol edin. Öyleyse, federasyon kimlik sağlayıcısının bunu yapacak şekilde yapılandırıldığından emin olun. Talep eksikse Azure AD (ve bu nedenle İş Ortağı Merkezi), kullanıcının MFA doğrulamasını tamamlamış olduğunu ve talebin eksik olduğunu bilemayacak ve ölçümün %100'e varmasına neden olabilir.

* **Özel Denetim** - Azure AD Özel Denetimi, bir kullanıcının üçüncü taraf MFA çözümü aracılığıyla MFA doğrulamayı tamamlamış olup olmadığını belirlemek için kullanılamaz. Sonuç olarak, özel denetim aracılığıyla MFA doğrulamayı tamamlayan tüm kullanıcılar her zaman MFA doğrulamayı tamamlamış değil olarak Azure AD'ye (ve İş Ortağı Merkezi) görünür. Mümkün olduğunda, Azure AD ile tümleştirdiğiniz zaman Özel Denetim yerine Kimlik Federasyonu'na geçmeniz önerilir.

### <a name="identify-which-users-have-signed-in-to-partner-center-without-mfa"></a>Hangi kullanıcıların MFA olmadan İş Ortağı Merkezi olduğunu belirleme

Hangi kullanıcıların MFA doğrulaması olmadan İş Ortağı Merkezi olduğunu belirlemek ve bunları geçerli MFA uygulamanıza göre doğrulamak yararlı olabilir. Kullanıcının MFA [doğrulamasını tamamlamış olup](/azure/active-directory/reports-monitoring/concept-sign-ins) olmadığını bulmak için Azure AD oturum açma raporunu kullanabilirsiniz. Azure AD oturum açma raporu şu anda yalnızca Azure AD Premium veya Azure AD Premium (EMS gibi) içeren O365 SKU'slarına abone olan iş ortakları tarafından kullanılabilir.

## <a name="next-steps"></a>Sonraki adımlar

- [İş Ortağı Merkezi rehberlik grubu topluluğu](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [İş Ortağı Merkezi güvenlik gereksinimleri](partner-security-requirements.md)
- [İş Ortağı Merkezi gereksinimleri hakkında SSS](partner-security-requirements-faq.yml)
