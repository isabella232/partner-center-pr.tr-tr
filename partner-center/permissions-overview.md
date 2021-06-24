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
ms.openlocfilehash: 582fdc98617be7d82c0bc61a0bf46ceb662954d3
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565092"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a>Bir şirketin şirket içinde çalışması gereken kullanıcıları için kullanıcı rollerini ve izinlerini İş Ortağı Merkezi

**Uygun roller:** Genel yönetici | Kullanıcı yönetimi yönetici | MPN iş ortağı yöneticisi

Yasal ad ve adres, destek ayrıntıları, dosya vergi muafiyetleri, banka bilgileri ve şirketinizin birincil ilgili kişisi dahil olmak üzere iş ortağı profilinizi ayarladınız. Sonraki adım: Kullanıcılarınızı parolalar ve rollerle ayarlamalarını, böylece kullanıcılarınızı İş Ortağı Merkezi başlamalarını sağlar.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Çalışanlarınızı şirket içinde çalışacak şekilde İş Ortağı Merkezi

Kullanıcılarının sahip olduğu erişim türlerini İş Ortağı Merkezi izinlere göre belirlersiniz. Roller, işletmenizin dahil olduğu programlarla ilgilidir. Örneğin, işletmeniz bir Bulut Çözümü Sağlayıcısı (CSP) işletmesi ise, genel yönetici gibi standart Azure Active Directory (Azure AD) kiracı yönetimi rollerine sahip olmakla birlikte CSP programına özgü rollere de ihtiyacınız vardır. Her programın belirli rolleri vardır.

>[!Note]
> Azure AD kiracı rolleri genel yönetici, kullanıcı yöneticisi ve CSP rollerini içerir. Azure AD dışı roller, kiracıyı yönetmeyen rollerdir ve MPN (Microsoft İş Ortağı Ağı) iş ortağı yöneticisi, iş profili yöneticisi, referans yöneticisi, teşvik yöneticisi ve teşvik kullanıcısını içerir. 

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
||* Fiyatlandırmayı ve teklifleri görüntüleme
||* Faturalama
||* Müşteri adına yönetme
||* Katma değerli kurumsal bayi kaydetme
||* Uygulama için destek biletleri İş Ortağı Merkezi
||* İş ortağı destek biletlerini görüntüle|
|Satış aracısı | * Müşteri yönetimi|[Müşterileriniz için faturalama desteği sağlama ve faturalama sorularını yanıtlamaya yardımcı olun](provide-billing-support.md)
||* Cihaz listesini cihaz listesine İş Ortağı Merkezi
||* Abonelik yönetimi
||* Destek biletlerini görüntüleme
||* Müşteriyle ilişki isteği
||* Fiyatlandırmayı ve teklifleri görüntüleme
||* Müşteri adaylarını yönetme
||* Müşteri sözleşmelerini görüntüleme
||* Katma değerli kurumsal bayi kaydetme
||* Uygulama için destek biletleri İş Ortağı Merkezi
||* İş ortağı destek biletlerini görüntüle|
|Yardım masası aracısı| * Müşteri arama ve görüntüleme|[Sorunları Microsoft'a yükseltme ve Microsoft yükseltme için daha uygun olan sorunları öğrenme](escalate-problems-to-microsoft.md)
||* Müşteri ayrıntılarını düzenleme
||* Faturalama veya abonelik yönetimiyle ilgili müşteri sorunlarını çözme yardımı
||* Müşteriler adına destek isteği 
||* Müşteriler adına abonelikleri ve faturalama sorunlarını yönetme
||* Uygulama için destek biletleri İş Ortağı Merkezi
||* İş ortağı destek biletlerini görüntüle| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a>Denetim Masası Satıcısı (CPV). (CSP rolü ve Azure AD dışı rol)

CPV'ler, sistemlerini farklı API'lerle tümleştirerek CSP iş ortakları tarafından İş Ortağı Merkezi geliştirmektedir. 

|**Role**   |**Yapabilecekleriniz**|**Daha fazla bilgi edinin**|
|------------------------------|:----------------------------|----|
|Genel yönetici| Denetim Masası Vendor (CPV) profilinizi görüntüleme ve yönetme|[CSP iş ortağı sistemlerini Denetim Masası API'lerle tümleştirin ve satıcı olarak İş Ortağı Merkezi olun](enroll-as-cpv.md)
||CPV özelliklerine erişmesi gereken kullanıcılarınızı görüntüleme ve yönetme|

### <a name="guest-user-must-be-added-to-the-azure-ad-tenant"></a>Konuk kullanıcı (Azure AD kiracısına eklenmiştir)

|**Konuk kullanıcı**   | **Roller**|
|---------------------------|:--------------------|
||MPN iş ortağı yöneticisi|
||İş profili yöneticisi|
||Referans yöneticisi|


## <a name="manage-mpn-membership-and-your-company"></a>MPN üyeliğini ve şirketinizi yönetme 

Bu roller Azure AD rolleri değildir. Bu roller kiracı yerine şirket işletmelerini yönetir.

|**Role** | **Yapabilecekleriniz**|**Daha fazla bilgi edinin**|
|----------------------------|:----------------------------|-----|
|MPN iş ortağı yöneticisi|* İş ortağı hizmet isteklerini görüntüleme, oluşturma ve yönetme|[Microsoft Eylem Paketi aboneliği veya Silver ve Gold uzmanlık satın alma veya yenileme](mpn-get-action-pack.md)
||* Yasal, şirket, işletme ve MPN profillerini görüntüleme
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
||* Kiracılı kullanıcılar için Azure AD olmayan rollere roller atama 
||* Konumları programlara kaydetme
||* Uygulama için destek biletleri İş Ortağı Merkezi
||* İş ortağı destek biletlerini görüntüle

## <a name="manage-referrals"></a>Referansları yönetme

|**Role** | **Yapabilecekleriniz**|**Daha fazla bilgi edinin**
|------------------------------|:-------------------------|---|
|Referans yöneticisi|Verilerde Referanslar sekmesinde her şeyi oluşturma ve İş Ortağı Merkezi|[Ortak satış fırsatlarını yönetme](manage-co-sell-opportunities.md)
||    Tüm ortak satış fırsatlarını ve müşteri adaylarını görüntüleme ve düzenleme
||    Anlaşma için ekip üyeleri atay olabilir
||    İş profillerini görüntüleme ve düzenleme
||    Kazandı olarak işaretlenen ve anlaşma kaydı için uygun olan fırsatlar için anlaşmaları görüntüleme ve kaydetme
||    Destek biletleri oluşturabilir ve görüntüleme
|Referans kullanıcısı|Ortak satış fırsatlarını yalnızca ekibin bir parçası olanlar için oluşturma ve yönetme |[Ortak satış fırsatlarını yönetme](manage-co-sell-opportunities.md)
||    Rolün atandığı konumlar için ortak satış fırsatları oluşturabilir.
||    Takım üyesi olan, kazanildi olarak işaretlenen ve anlaşma kaydı için uygun olan fırsatlar için anlaşmaları görüntüleme ve kaydetme.
||    Destek biletleri oluşturabilir ve görüntüleme
|İş profili yöneticisi|İş profilleri oluşturma ve yönetme | [İş profillerini yönetme](create-a-marketing-profile.md)
||    Destek biletleri oluşturabilir ve görüntüleme

Yeni referans kullanıcı rolünün yanı sıra anlaşmaların konum kapsamını da tanıtıyoruz. Aşağıdaki tabloda konuma göre deals-access açıklanmıştır.

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
|Teşvikler yöneticisi|* Teşvikleri başlatma ve yönetme |[Teşvikleri kullanmaya başlamanıza yardımcı olmak için bu kaynakları kullanın](incentives-get-started-intro.md)
||* Teşvik programlarının tüm yönlerini görüntüleme ve düzenleme
||* Banka ve vergi ayrıntılarını görüntüleme ve düzenleme
||* İndirim ve ortak kazançları görüntüleme
||* Erişim desteği
||* Teşvik ödemeleri ile ilgili itiraz|
|Teşvikler kullanıcısı|* Teşvik programlarını görüntüleme
||* Teşvik taleplerini görüntüleme ve başlatma
||* İndirim ve ortak kazançları görüntüleme
||* Uygulama için destek biletleri İş Ortağı Merkezi
||* İş ortağı destek biletlerini görüntüle

## <a name="view-partner-center-insights-data"></a>İş Ortağı Merkezi Insights verilerini görüntüleme

|**Role** | **Yapabilecekleriniz**|**Daha fazla bilgi edinin**|
|------------------------------|:-------------------------|---|
|Yönetici raporu görüntüleyicisi|Tüm raporlama veri kümelerine erişim, iş ortağı destek biletleri oluşturma, sizin oluşturdukları iş ortağı destek biletlerini görüntüleme|[İş Ortağı Merkezi Insights'ta kullanılabilen pano raporlarına genel bakış](pci-overview-report.md)
|Rapor görüntüleyicisi|Gelir ve müşteri ve çalışan kişisel verileri dışında veri raporlarına erişim, iş ortağı destek biletleri oluşturma, sizin oluşturdurarak iş ortağı destek biletlerini görüntüleme|

## <a name="next-steps"></a>Sonraki adımlar

- [Kullanıcı hesabı oluşturup rol ve izin atama](create-user-accounts-and-set-permissions.md)
- [Yeni bir İş Ortağı Merkezi programına kaydolarak hesap İş Ortağı Merkezi doğrulayın](verification-responses.md)
