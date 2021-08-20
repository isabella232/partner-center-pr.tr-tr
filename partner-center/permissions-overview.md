---
title: Kullanıcılara roller & izinleri atama
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
description: Iş Ortağı Merkezi 'nde ticari işlemleri, başvuruları, teşvikleri veya MPN üyeliklerini yöneten şirketinizin kullanıcılarına en uygun rolleri öğrenin.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperf-fy21q1
ms.openlocfilehash: 7638a35b5aa583cd3a7c3b40833123402df7cb70
ms.sourcegitcommit: 9d155ff319ba2b2793bc9945d179ce1cb9c8f7c7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/19/2021
ms.locfileid: "122453807"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a>Şirket kullanıcılarının iş ortağı merkezi 'nde çalışması gereken kullanıcı rollerini ve izinlerini atama

**Uygun roller**: genel yönetici | Kullanıcı Yönetimi Yöneticisi | MPN iş ortağı Yöneticisi

İş ortağı profilinizi, yasal ad ve adres, destek ayrıntıları, dosya vergi muafiyeti, banka bilgileri ve şirketinizin birincil ilgili kişisi dahil olmak üzere ayarlamış olursunuz. Sonraki adım: kullanıcılarınızın sizinle Iş Ortağı Merkezi 'nde çalışmaya başlayabilmesi için parolalar ve rollerle birlikte kurulumunu öğrenin.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Çalışanlarınızı iş ortağı merkezi 'nde çalışacak şekilde ayarlama

Kullanıcılarınıza verdiğiniz roller ve izinler tarafından Iş Ortağı Merkezi 'ne sahip olan erişim türlerini belirlersiniz. Roller, işletmenizin dahil olduğu program (ler) ile ilgilidir. örneğin, işiniz Bulut Çözümü Sağlayıcısı (CSP) bir iş ise, genel yönetici gibi yalnızca standart Azure Active Directory (Azure AD) kiracı yönetim rollerine sahip olmayacaktır, ancak CSP programına özgü rollere ihtiyaç duyarsınız. Her programın kendisine özgü rolleri vardır.

>[!Note]
> Azure AD kiracı rolleri, genel yönetici, Kullanıcı Yöneticisi ve CSP rollerini içerir. Azure dışı AD rolleri, kiracıyı yönetmeyen rollerdir ve MPN (Microsoft İş Ortağı Ağı) iş ortağı Yöneticisi, iş profili Yöneticisi, başvuru Yöneticisi, teşvik Yöneticisi ve kullanıcıyı teşvik eder. 

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

CPVs, CSP iş ortakları tarafından sistemlerini Iş Ortağı Merkezi API 'Leri ile tümleştirmelerini sağlamak için kullanmak üzere uygulamalar geliştirir. 

|**Role**   |**Yapabilecekleriniz**|**Daha fazla bilgi edinin**|
|------------------------------|:----------------------------|----|
|Genel yönetici| Denetim Masası satıcısı (CPV) profilinizi görüntüleyin ve yönetin|[CSP iş ortağı sistemlerini Iş Ortağı Merkezi API 'Leriyle tümleştirmenize yardımcı olmak için Denetim Masası satıcısı olarak kaydetme](enroll-as-cpv.md)
||CPV özelliklerine erişmesi gereken kullanıcılarınızı görüntüleyin ve yönetin|

### <a name="guest-user-must-be-added-to-the-azure-ad-tenant"></a>Konuk Kullanıcı (Azure AD kiracısına eklenmelidir)

|**Konuk Kullanıcı**   | **Roller**|
|---------------------------|:--------------------|
||MPN iş ortağı Yöneticisi|
||İş profili Yöneticisi|
||Başvuru Yöneticisi|


## <a name="manage-mpn-membership-and-your-company"></a>MPN üyeliğini ve şirketinizi yönetme 

Bu roller Azure AD rolleri değildir. Bu roller, kiracı yerine şirket işletmelerini yönetir.

|**Role** | **Yapabilecekleriniz**|**Daha fazla bilgi edinin**|
|----------------------------|:----------------------------|-----|
|MPN iş ortağı Yöneticisi|* İş ortağı hizmeti isteklerini görüntüleyin, oluşturun ve yönetin|[Microsoft Eylem Paketi aboneliği veya Silver ve Gold uzmanlık satın alma veya yenileme](mpn-get-action-pack.md)
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
||* İş için destek biletleri İş Ortağı Merkezi
||* İş ortağı destek biletlerini görüntüle
|Hesap yöneticisi| Konum ekleme|[Konumları yönetme](manage-locations.md)
|| Yönetici olduğunuz hesaplarla ilgili profilleri yönetme 
||* Kiracılı kullanıcılar için Azure AD olmayan rollere roller atama 
||* Konumları programlara kaydetme
||* İş için destek biletleri İş Ortağı Merkezi
||* İş ortağı destek biletlerini görüntüle

## <a name="manage-referrals"></a>Referansları yönetme

|**Role** | **Yapabilecekleriniz**|**Daha fazla bilgi edinin**
|------------------------------|:-------------------------|---|
|Referans yöneticisi|İş Ortağı Merkezi'de Referanslar sekmesinde her şeyi oluşturma ve yönetme|[Ortak satış fırsatlarını yönetme](manage-co-sell-opportunities.md)
||    Tüm ortak satış fırsatlarını ve müşteri adaylarını görüntüleyemez ve düzenleyebilir
||    Anlaşma için ekip üyeleri atay olabilir
||    İş profillerini görüntüleme ve düzenleme
||    Kazandı olarak işaretlenen ve anlaşma kaydı için uygun olan fırsatlar için anlaşmaları görüntüleme ve kaydetme
||    Destek biletleri oluşturabilir ve görüntüleme
|Referans kullanıcısı|Ortak satış fırsatlarını yalnızca ekibin bir parçası olanlar için oluşturma ve yönetme |[Ortak satış fırsatlarını yönetme](manage-co-sell-opportunities.md)
||    Rolün atandığı konumlar için ortak satış fırsatları oluşturabilir.
||    Takım üyesiyseniz, kazanildi olarak işaretlenen ve anlaşma kaydı için uygun olarak işaretlenen fırsatlar için anlaşmaları görüntüleme ve kaydetme.
||    Destek biletleri oluşturabilir ve görüntüleme
|İş profili yöneticisi|İş profilleri oluşturma ve yönetme | [İş profillerini yönetme](create-a-marketing-profile.md)
||    Destek biletleri oluşturabilir ve görüntüleme

Yeni referans kullanıcı rolünün yanı sıra anlaşmaların konum kapsamını da tanıtıyoruz. Aşağıdaki tabloda konuma bağlı olarak deals-access açıklanmıştır.

|**Kapsam** | **Yapabilecekleriniz** |
|------------------------------|:-------------------------|
|Tüm şirket | Hem yöneticiler hem de kullanıcılar, şirketlerinde herhangi bir konum için anlaşma oluşturma erişimine sahiptir|
|| Referans yöneticisinin tüm anlaşmaları görüntüleme ve düzenleme erişimi vardır |
|| Referans kullanıcıları, yalnızca ekibin bir parçası olan tüm anlaşmaları görüntüleme ve düzenleme erişimine sahiptir |
|Bir veya daha fazla konum | Hem yöneticiler hem de kullanıcılar, şirketlerinde atanan konum için anlaşmalar oluşturma erişimine sahiptir|
|| Referans yöneticisi, atanan konumlara ait tüm anlaşmaları görüntüleme ve düzenleme erişimine sahiptir|
|| Referans kullanıcıları, takımın parçası olan atanan konumlara ait tüm anlaşmaları görüntüleme ve düzenleme erişimine sahiptir|

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
||* Teşvik taleplerini görüntüleme ve başlatma
||* İndirim ve ortak kazançları görüntüleme
||* İş için destek biletleri İş Ortağı Merkezi
||* İş ortağı destek biletlerini görüntüle

## <a name="view-partner-center-insights-data"></a>Veri İş Ortağı Merkezi Analizler görüntüleme

|**Role** | **Yapabilecekleriniz**|**Daha fazla bilgi edinin**|
|------------------------------|:-------------------------|---|
|Yönetici raporu görüntüleyicisi|Tüm raporlama veri kümelerine erişim, iş ortağı destek biletleri oluşturma, sizin oluşturdukları iş ortağı destek biletlerini görüntüleme|[Genel bakış pano raporları İş Ortağı Merkezi Analizler](insights-overview-report.md)
|Rapor görüntüleyicisi|Gelir ve müşteri ve çalışan kişisel verileri dışında veri raporlarına erişim, iş ortağı destek biletleri oluşturma, sizin oluşturduz iş ortağı destek biletlerini görüntüleme|

## <a name="next-steps"></a>Sonraki adımlar

- [Kullanıcı hesabı oluşturup rol ve izin atama](create-user-accounts-and-set-permissions.md)
- [Yeni bir İş Ortağı Merkezi programına kaydolurken hesap bilgilerinizi doğrulama](verification-responses.md)
