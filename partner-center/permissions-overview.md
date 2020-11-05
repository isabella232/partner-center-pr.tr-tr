---
title: Kullanıcılara roller & izinleri atama
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Iş Ortağı Merkezi 'nde ticari işlemleri, başvuruları, teşvikleri veya MPN üyeliklerini yöneten şirketinizin kullanıcılarına en uygun rolleri öğrenin.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperfq1
ms.openlocfilehash: 4839fbd6fac5f84e5a2ebc40d1f7f48da6114113
ms.sourcegitcommit: 92be474db61cc12f684850c2a7a8a8bdd5c93f97
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/05/2020
ms.locfileid: "93363631"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a>Şirket kullanıcılarının iş ortağı merkezi 'nde çalışması gereken kullanıcı rollerini ve izinlerini atama

**Uygun roller**

- Genel yönetici
- Kullanıcı yöneticisi
- MPN iş ortağı Yöneticisi

İş ortağı profilinizi, yasal ad ve adres, destek ayrıntıları, dosya vergi muafiyeti, banka bilgileri ve şirketinizin birincil ilgili kişisi dahil olmak üzere ayarlamış olursunuz. Sonraki adım: kullanıcılarınızın sizinle Iş Ortağı Merkezi 'nde çalışmaya başlayabilmesi için parolalar ve rollerle birlikte kurulumunu öğrenin.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Çalışanlarınızı iş ortağı merkezi 'nde çalışacak şekilde ayarlama

Kullanıcılarınıza verdiğiniz roller ve izinler tarafından Iş Ortağı Merkezi 'ne sahip olan erişim türlerini belirlersiniz. Roller, işletmenizin dahil olduğu program (ler) ile ilgilidir. Örneğin, işiniz bir bulut çözümü sağlayıcısı (CSP) işleridir, yalnızca genel yönetici gibi standart Azure Active Directory kiracı yönetim rollerine sahip olmaz, ancak CSP programına özgü rollere ihtiyaç duyarsınız. Her programın kendisine özgü rolleri vardır.

>[!Note]
> Azure Active Directory kiracı rolleri genel yönetici, Kullanıcı Yöneticisi ve CSP rollerini içerir. Azure olmayan-Active-Directory rolleri, kiracıyı yönetmeyen rollerdir ve MPN Yöneticisi, iş profili Yöneticisi, başvuru Yöneticisi, teşvik Yöneticisi ve kullanıcıyı teşvik eder. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Iş Ortağı Merkezi 'nde ticari işlemleri yönetme (Azure AD ve CSP rolleri)

|**Role**|**Neler yapabilecekleri**|**Daha fazla bilgi edinin**|
|----------------------------------|---|:---------------------------------|
|Genel yönetici|* Tüm Microsoft hesabı/hizmetlere tam ayrıcalıklarla erişebilir|[İş Ortağı Merkezi hesabınızı yönetme](partner-center-account-setup.md)
|      |* Iş Ortağı Merkezi için destek biletleri oluşturma
||* Oluşturduğunuz iş ortağı destek biletlerini görüntüle
||* Sözleşmeleri, Fiyat listelerini ve teklifleri görüntüleme
||* İş ortağı kullanıcılarını görüntüleme, oluşturma ve yönetme|
||  Faturalandırma, faturalar ve keşfi dosyalarını görüntüleme, oluşturma ve yönetme
|Kullanıcı Yönetimi Yöneticisi   | * Kullanıcıları görüntüleme, oluşturma ve yönetme|[Iş Ortağı Merkezi 'nde Microsoft İş Ortağı Ağı üyelik avantajlarınızı ve tekliflerini yönetme](manage-your-partner-network-benefits.md)
||* Tüm iş ortağı profillerini görüntüle
||* Iş Ortağı Merkezi için destek biletleri oluşturma
||* Oluşturduğunuz iş ortağı destek biletlerini görüntüle
|Faturalama yöneticisi | -Faturalandırma, faturalar ve keşfi dosyalarını görüntüleyin, oluşturun ve yönetin|[Faturanızı okuma](billing.md)
||* Fiyatlandırmayı görüntüle
||* Iş Ortağı Merkezi için destek biletleri oluşturma
||* Oluşturduğunuz iş ortağı destek biletlerini görüntüle
|Varsayılan Kullanıcı|  Profilimi görüntüle   |[Parolanızı sıfırlama](reset-my-pasword.md)
|Yönetim Aracısı | * Müşteri yönetimi|[Müşterilerinizle bağlantı kurma](connect-with-your-customers.md)
||* Iş Ortağı Merkezi 'ne cihaz listesi ekleme
||* Cihazlara profiller oluşturma ve uygulama
||* Abonelik yönetimi
||* Müşteriler için hizmet durumu ve hizmet istekleri
||* Yönetici temsilcisi ayrıcalıkları iste
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

Bu roller Azure Active Directory roller değildir. Bu roller, kiracı yerine şirket işletmelerini yönetir.

|**Role** | **Yapabilecekleriniz**|**Daha fazla bilgi edinin**|
|----------------------------|:----------------------------|-----|
|MPN iş ortağı Yöneticisi|* İş ortağı hizmeti isteklerini görüntüleyin, oluşturun ve yönetin|[Microsoft Eylem Paketi aboneliği veya Silver ve Gold uzmanlık satın alma veya yenileme](mpn-get-action-pack.md)
||* Yasal, Şirket, iş ve MPN profillerini görüntüleme
||* Kullanıcı ayrıntılarını ve yetenek verilerini görüntüleyin
||* Uzmanlıklar görüntüle
||* Avantajları görüntüleyin ve yönetin
||* MPN tekliflerini görüntüleme ve satın alma
||* MPN 'nin sipariş geçmişini ve faturalarını görüntüleme
||* İş ortağı katkısı gösterge verilerini görüntüle
||*, Fiş doğrulama aracında çalışabilir|
||* Müşteri verileri analizlerini görüntüle
||* Şirket içindeki diğer Kullanıcı rollerini görüntüleme, ancak rolleri atayamıyorum
||* Iş Ortağı Merkezi için destek biletleri oluşturma
||* Oluşturduğunuz iş ortağı destek biletlerini görüntüle
|Hesap yöneticisi| Konum Ekle|[Konumları yönetme](manage-locations.md)
|| Yönetici olduğunuz hesaplarla ilgili Profilleri yönetme 
||* Kiracıdaki kullanıcılara Azure olmayan-Active-Directory rollerine roller atama 
||* Konumları programlara kaydetme
||* Iş Ortağı Merkezi için destek biletleri oluşturma
||* Oluşturduğunuz iş ortağı destek biletlerini görüntüle

## <a name="manage-referrals"></a>Başvuruları yönetme

> [!Note]
>Yeni başvurular Kullanıcı rolü, 15 Kasım 2020 tarihinden itibaren kullanılabilir. Mevcut başvuru yöneticileri, referans yönetici rollerini tüm şirket kapsamında tutar.

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

Yeni başvurular Kullanıcı rolüyle birlikte, anlaşmalar için de konum kapsamı da tanıtıyoruz. Aşağıdaki tabloda, konuma göre anlaşmalar erişimi açıklanmaktadır.

|**Kapsam** | **Yapabilecekleriniz** |
|------------------------------|:-------------------------|
|Tüm şirket | Her iki yönetici ve Kullanıcı, şirketlerinde herhangi bir konum için anlaşmalar oluşturma erişimine sahiptir|
|| Başvuru Yöneticisi tüm anlaşmaları görüntüleme ve düzenleme erişimine sahiptir |
|| Başvuru kullanıcıları yalnızca ekibin bir parçası olduklarında tüm anlaşmaları görüntüleme ve düzenleme erişimine sahiptir |
|Bir veya daha fazla konum | Her iki yönetici ve Kullanıcı, şirketlerinin atandığı konuma yönelik anlaşmalar oluşturmak için erişime sahiptir|
|| Başvuru Yöneticisi atanan konumlara ait tüm anlaşmaları görüntüleme ve düzenleme erişimine sahiptir|
|| Başvuru kullanıcıları ekibin parçasıysa atanan konumlara ait tüm anlaşmaları görüntüleme ve düzenleme erişimine sahiptir|

## <a name="manage-incentives"></a>Teşvikleri yönetme

|**Role** | **Yapabilecekleriniz**|**Daha fazla bilgi edinin**
|------------------------------|:-------------------------|---|
|Teşvikleri Yöneticisi|* Teşvikleri 'yi başlatır ve yönetir |[Teşvikleri kullanmaya başlamanıza yardımcı olması için bu kaynakları kullanın](incentives-get-started-intro.md)
||* Teşvikleri programlarının tüm yönlerini görüntüleyebilir ve düzenleyebilir
||* Banka ve vergi ayrıntılarını görüntüleyebilir ve düzenleyebilir
||* İndirim ve ortak işlem kazançlarını görüntüleme
||* Erişim desteği
||* İtiraz teşvikleri ödemeleri|
|Teşvikleri kullanıcısı|* Teşvikleri programlarını görüntüleyebilir
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
