---
title: Kullanıcılara & rol atama
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Şirket içinde ticari işlemleri, referansları, teşvikleri veya MPN üyeliklerini yöneten şirket kullanıcıları için en iyi rolleri İş Ortağı Merkezi.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperf-fy21q1
ms.openlocfilehash: b1ac34bbb92d600805465ca5f6d1b28af54cd5e1
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855140"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a>Bir şirketin şirket içinde çalışması gereken kullanıcıları için kullanıcı rollerini ve izinlerini İş Ortağı Merkezi

**Uygun roller:** Genel yönetici | Kullanıcı yönetimi yönetici | MPN iş ortağı yöneticisi

Yasal ad ve adres, destek ayrıntıları, dosya vergi muafiyetleri, banka bilgileri ve şirketinizin birincil ilgili kişisi dahil olmak üzere iş ortağı profilinizi ayarladınız. Sonraki adım: Kullanıcılarınızı parolalar ve rollerle ayarlamalarını, böylece kullanıcılarınızı İş Ortağı Merkezi başlamalarını sağlar.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Çalışanlarınızı şirket içinde çalışacak şekilde İş Ortağı Merkezi

Kullanıcılarının sahip olduğu erişim türlerini İş Ortağı Merkezi izinlere göre belirlersiniz. Roller, işletmenizin dahil olduğu programlarla ilgilidir. Örneğin, işletmeniz bir Bulut Çözümü Sağlayıcısı (CSP) işletmesi ise, genel yönetici gibi standart Azure Active Directory kiracı yönetimi rollerine sahip olmakla birlikte CSP programına özgü rollere de ihtiyacınız vardır. Her programın belirli rolleri vardır.

>[!Note]
> Azure Active Directory rolleri genel yönetici, kullanıcı yöneticisi ve CSP rollerini içerir. Azure Active Directory dışı roller, kiracıyı yönetmeyen rollerdir ve MPN yöneticisi, iş profili yöneticisi, referans yöneticisi, teşvik yöneticisi ve teşvik kullanıcısını içerir. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Ticari işlemleri İş Ortağı Merkezi (Azure AD ve CSP rolleri)

|**Role**|**Neler yapabiliriz?**|**Daha fazla bilgi edinin**|
|----------------------------------|---|:---------------------------------|
|Genel yönetici|* Tüm Microsoft hesabı/hizmetlere tam ayrıcalıklarla erişebilir|[İş Ortağı Merkezi hesabınızı yönetme](partner-center-account-setup.md)
|      |* Uygulama için destek biletleri İş Ortağı Merkezi
||* İş ortağı destek biletlerini görüntüle
||* Anlaşmaları, fiyat listelerini ve teklifleri görüntüleme
||* İş ortağı kullanıcılarını görüntüleme, oluşturma ve yönetme|
||  Faturalama, faturalar ve mutabakat dosyalarını görüntüleme, oluşturma ve yönetme
|Kullanıcı yönetimi yöneticisi   | * Kullanıcıları görüntüleme, oluşturma ve yönetme|[Microsoft İş Ortağı Ağı üyelik avantajlarınızı ve tekliflerinizi İş Ortağı Merkezi](manage-your-partner-network-benefits.md)
||* Tümünü görüntüle iş ortağı profilleri
||* Uygulama için destek biletleri İş Ortağı Merkezi
||* İş ortağı destek biletlerini görüntüle
|Faturalama yöneticisi | - Faturalama, faturalar ve mutabakat dosyalarını görüntüleme, oluşturma ve yönetme|[Faturanızı okuma](billing.md)
||* Fiyatlandırmayı görüntüleme
||* Uygulama için destek biletleri İş Ortağı Merkezi
||* İş ortağı destek biletlerini görüntüle
|Varsayılan kullanıcı|  Görünüm Profilim   |[Parolanızı sıfırlama](reset-my-pasword.md)
|Yönetici aracısı | * Müşteri yönetimi|[Müşterilerinizle bağlantı kurma](connect-with-your-customers.md)
||* Cihaz listesini cihaz listesine İş Ortağı Merkezi
||* Cihazlara profil oluşturma ve uygulama
||* Abonelik yönetimi
||* Müşteriler için hizmet durumu ve hizmet istekleri
||* Yönetici temsilcisi ayrıcalıkları isteği
||* Fiyatlandırma ve teklifleri görüntüleme
||* Faturalandırma
||* Müşteri adına yönetme
||* Katma değerli satıcı kaydetme
||* Iş Ortağı Merkezi için destek biletleri oluşturma
||* Oluşturduğunuz iş ortağı destek biletlerini görüntüle|
|Satış Aracısı | * Müşteri yönetimi|[Müşterileriniz için faturalandırma desteği sağlayın ve faturalandırma sorularını cevaplayın](provide-billing-support.md)
||* Iş Ortağı Merkezi 'ne cihaz listesi ekleme
||* Abonelik yönetimi
||* Destek biletlerini görüntüle
||* Müşteriyle ilişki isteme
||* Fiyatlandırma ve teklifleri görüntüleme
||* Müşteri adaylarını yönetme
||* Müşteri anlaşmasını görüntüleme
||* Değere eklenen bir bayi Kaydet
||* Iş Ortağı Merkezi için destek biletleri oluşturma
||* Oluşturduğunuz iş ortağı destek biletlerini görüntüle|
|Yardım Masası Aracısı| * Bir müşteriyi arayın ve görüntüleyin|[Sorunları Microsoft 'a iletin ve Microsoft 'a yükseltme için hangi sorunların daha uygun olduğunu öğrenin](escalate-problems-to-microsoft.md)
||* Müşteri ayrıntılarını düzenleme
||* Faturalandırma veya abonelik yönetimiyle ilgili müşteri sorunlarını çözmeye yardımcı olun
||* Müşteriler adına destek isteyin 
||* Müşteriler adına abonelikleri ve faturalandırma sorunlarını yönetme
||* Iş Ortağı Merkezi için destek biletleri oluşturma
||* Oluşturduğunuz iş ortağı destek biletlerini görüntüle| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a>Denetim Masası satıcısı (CPV). (CSP rolü ve Azure dışı AD rolü)

CPVs, bulut çözümü sağlayıcısı (CSP) iş ortakları tarafından, sistemlerini Iş Ortağı Merkezi API 'Leri ile tümleştirmelerini sağlamak üzere uygulamalar geliştirmeyi sağlar. 

|**Role**   |**Yapabilecekleriniz**|**Daha fazla bilgi edinin**|
|------------------------------|:----------------------------|----|
|Genel yönetici| CPV profilinizi görüntüleyin ve yönetin|[CSP iş ortağı sistemlerini Iş Ortağı Merkezi API 'Leriyle tümleştirmenize yardımcı olmak için Denetim Masası satıcısı olarak kaydetme](enroll-as-cpv.md)
||CPV özelliklerine erişmesi gereken kullanıcılarınızı görüntüleyin ve yönetin|

### <a name="guest-user-must-be-added-to-the-azure-active-directory-tenant"></a>Konuk Kullanıcı (Azure Active Directory kiracısına eklenmelidir)

|**Konuk Kullanıcı**   | **Roller**|
|---------------------------|:--------------------|
||MPN iş ortağı Yöneticisi|
||İş profili Yöneticisi|
||Başvuru Yöneticisi|


## <a name="manage-mpn-membership-and-your-company"></a>MPN üyeliğini ve şirketinizi yönetme 

Bu roller tek Azure Active Directory değildir. Bu roller kiracı yerine şirket işletmelerini yönetir.

|**Role** | **Yapabilecekleriniz**|**Daha fazla bilgi edinin**|
|----------------------------|:----------------------------|-----|
|MPN iş ortağı yöneticisi|* İş ortağı hizmeti isteklerini görüntüleme, oluşturma ve yönetme|[Microsoft Eylem Paketi aboneliği veya Silver ve Gold uzmanlık satın alma veya yenileme](mpn-get-action-pack.md)
||* Yasal, şirket, iş ve MPN profillerini görüntüleme
||* Kullanıcı ayrıntılarını ve beceri verilerini görüntüleme
||* Yetkinlikleri görüntüleme
||* Avantajları görüntüleme ve yönetme
||* MPN tekliflerini görüntüleme ve satın alma
||* MPN tekliflerinin sipariş geçmişini ve faturalarını görüntüleme
||* İş ortağı katkısı gösterge verilerini görüntüleme
||* Kupon Doğrulama aracında çalışabilirsiniz|
||* Müşteri veri analizini görüntüleme
||* Şirket içindeki diğer kullanıcı rollerini görüntüleme, ancak rol ataymama
||* Uygulama için destek biletleri İş Ortağı Merkezi
||* İş ortağı destek biletlerini görüntüle
|Hesap yöneticisi| Konum ekleme|[Konumları yönetme](manage-locations.md)
|| Yönetici olduğunuz hesaplarla ilgili profilleri yönetme 
||* Kiracıda kullanıcılar için Azure Active Directory olmayan rollere roller atama 
||* Konumları programlara kaydetme
||* Iş Ortağı Merkezi için destek biletleri oluşturma
||* Oluşturduğunuz iş ortağı destek biletlerini görüntüle

## <a name="manage-referrals"></a>Başvuruları yönetme

|**Role** | **Yapabilecekleriniz**|**Daha fazla bilgi edinin**
|------------------------------|:-------------------------|---|
|Başvuru Yöneticisi|Iş Ortağı Merkezi 'nde Referanslar sekmesinde her şeyi oluşturun ve yönetin|[Ortak satış fırsatlarını yönetme](manage-co-sell-opportunities.md)
||    Tüm ortak satış fırsatlarını ve müşteri adaylarını görüntüleyebilir ve düzenleyebilir
||    , Bir anlaşma için takım üyeleri atayabilir
||    İş profillerini görüntüleyebilir ve düzenleyebilir
||    Kazanıldı olarak işaretlenen ve anlaşma kaydı için uygun olan fırsatlara yönelik anlaşmalar görüntüleyebilir ve kaydedebilirsiniz
||    Destek biletleri oluşturabilir ve görüntüleyebilir
|Başvuru kullanıcısı|Ortak satış fırsatlarını yalnızca ekibin bir parçasıysa oluşturun ve yönetin |[Ortak satış fırsatlarını yönetme](manage-co-sell-opportunities.md)
||    Rolün atandığı konumlar için ortak satış fırsatları oluşturabilir.
||    Kazanıldı olarak işaretlenen ve ekip üyesi olmaları durumunda anlaşma kaydı için uygun olan fırsatlara yönelik anlaşmalar görüntüleyebilir ve kaydedebilirsiniz.
||    Destek biletleri oluşturabilir ve görüntüleyebilir
|İş profili Yöneticisi|İş profilleri oluşturma ve yönetme | [İş profillerini yönetme](create-a-marketing-profile.md)
||    Destek biletleri oluşturabilir ve görüntüleyebilir

Yeni başvurular Kullanıcı rolüyle birlikte, anlaşmalar için de konum kapsamı da tanıtıyoruz. Aşağıdaki tabloda konuma göre deals-access açıklanmıştır.

|**Kapsam** | **Yapabilecekleriniz** |
|------------------------------|:-------------------------|
|Tüm şirket | Hem yöneticiler hem de kullanıcılar, şirketlerinde herhangi bir konum için anlaşma oluşturma erişimine sahiptir|
|| Referans yöneticisinin tüm anlaşmaları görüntüleme ve düzenleme erişimi vardır |
|| Referans kullanıcıları, yalnızca ekibin bir parçası olan tüm anlaşmaları görüntüleme ve düzenleme erişimine sahiptir |
|Bir veya daha fazla konum | Hem yöneticiler hem de kullanıcılar, şirketlerinde atanan konum için anlaşma oluşturma erişimine sahiptir|
|| Referans yöneticisi, atanan konumlara ait tüm anlaşmaları görüntüleme ve düzenleme erişimine sahiptir|
|| Referans kullanıcıları, takımın parçası olan atanan konumlara ait olan tüm anlaşmaları görüntüleme ve düzenleme erişimine sahiptir|

## <a name="manage-incentives"></a>Teşvikleri yönetme

|**Role** | **Yapabilecekleriniz**|**Daha fazla bilgi edinin**
|------------------------------|:-------------------------|---|
|Teşvikler yöneticisi|* Teşvikleri başlatıyor ve yönetir |[Teşvikleri kullanmaya başlamanıza yardımcı olmak için bu kaynakları kullanın](incentives-get-started-intro.md)
||* Teşvik programlarının tüm yönlerini görüntüleme ve düzenleme
||* Banka ve vergi ayrıntılarını görüntüleme ve düzenleme
||* İndirim ve ortak kazançları görüntüleme
||* Erişim desteği
||* Teşvik ödemeleri ile ilgili itiraz|
|Teşvikler kullanıcısı|* Teşvik programlarını görüntüleme
||* Teşvikleri taleplerini görüntüleyebilir ve başlatabilir
||* İndirim ve ortak işlem kazançlarını görüntüleme
||* Iş Ortağı Merkezi için destek biletleri oluşturma
||* Oluşturduğunuz iş ortağı destek biletlerini görüntüle

## <a name="view-partner-center-insights-data"></a>Iş Ortağı Merkezi Öngörüler verilerini görüntüle

|**Role** | **Yapabilecekleriniz**|**Daha fazla bilgi edinin**|
|------------------------------|:-------------------------|---|
|Executive rapor Görüntüleyicisi|Tüm raporlama veri kümelerine erişim, iş ortağı destek biletleri oluşturma, oluşturduğunuz iş ortağı destek biletlerini görüntüleme|[Iş Ortağı Merkezi öngörülerine Genel Bakış Panosu raporları](pci-overview-report.md)
|Rapor Görüntüleyicisi|Gelir ve müşteri ve çalışan kişisel verileri dışında veri raporlarına erişim, iş ortağı destek biletleri oluşturma, oluşturduğunuz iş ortağı destek biletlerini görüntüleme|

## <a name="next-steps"></a>Sonraki adımlar

- [Kullanıcı hesabı oluşturup rol ve izin atama](create-user-accounts-and-set-permissions.md)
- [Yeni bir Iş Ortağı Merkezi programına kayıt yaptığınızda hesap bilgilerinizi doğrulama](verification-responses.md)
