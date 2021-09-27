---
title: Kullanıcılara rol ve izin atama
ms.topic: article
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Iş Ortağı Merkezi 'nde ticari işlemleri, başvuruları, teşvikleri veya MPN üyeliklerini yöneten şirketinizin kullanıcılarına en uygun rolleri öğrenin.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperf-fy21q1
ms.openlocfilehash: 46d17de1ba7572c72162cfd38143ed9aa084c5c7
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129075763"
---
# <a name="assign-roles-and-permissions-to-users"></a>Kullanıcılara rol ve izin atama

**Uygun roller**: genel yönetici | Kullanıcı Yönetimi Yöneticisi | MPN iş ortağı Yöneticisi

İş ortağı profilinizi, yasal ad ve adres, destek ayrıntıları, dosya vergi muafiyeti, banka bilgileri ve şirketinizin birincil ilgili kişisi dahil olmak üzere ayarlamış olursunuz. Bir sonraki adımınız, kullanıcılarınızın sizinle Iş Ortağı Merkezi 'nde çalışmaya başlayabilmesi için parola ve rollerle ayarlanabilmesi.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Çalışanlarınızı iş ortağı merkezi 'nde çalışacak şekilde ayarlama

Kullanıcılarınıza verdiğiniz roller ve izinler tarafından Iş Ortağı Merkezi 'ne sahip olan erişim türlerini belirlersiniz. Roller, işletmenizin dahil olduğu program (ler) ile ilgilidir. örneğin, işiniz Bulut Çözümü Sağlayıcısı (CSP) bir iş ise, genel yönetici gibi yalnızca standart Azure Active Directory (Azure AD) kiracı yönetim rollerine sahip olmayacaktır, ancak CSP programına özgü rollere ihtiyaç duyarsınız. Her programın kendisine özgü rolleri vardır.

> [!NOTE]
> Azure AD kiracı rolleri, genel yönetici, Kullanıcı Yöneticisi ve CSP rollerini içerir. Azure dışı AD rolleri, kiracıyı yönetmeyen rollerdir ve MPN (Microsoft İş Ortağı Ağı) iş ortağı Yöneticisi, iş profili Yöneticisi, başvuru Yöneticisi, teşvik Yöneticisi ve kullanıcıyı teşvik eder. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Iş Ortağı Merkezi 'nde ticari işlemleri yönetme (Azure AD ve CSP rolleri)

|**Role**|**Neler yapabilecekleri**| **Çalışma alanı** | **Daha fazla bilgi edinin**|
|----------------------------------|---|---|:---------------------------------|
|Genel yönetici|* Tüm Microsoft hesabı/hizmetlere tam ayrıcalıklarla erişebilir| Hesap ayarları | [İş Ortağı Merkezi hesabınızı yönetme](partner-center-account-setup.md) |
||* Iş Ortağı Merkezi için destek biletleri oluşturma | Yardım + destek |
||* Oluşturduğunuz iş ortağı destek biletlerini görüntüle | Yardım + destek |
||* Sözleşmeleri, Fiyat listelerini ve teklifleri görüntüleme | Fiyatlandırma |
||* İş ortağı kullanıcılarını görüntüleme, oluşturma ve yönetme | Hesap ayarları |
||  Faturalandırma, faturalar ve keşfi dosyalarını görüntüleme, oluşturma ve yönetme | Faturalandırma |
| Kullanıcı Yönetimi Yöneticisi   | * Kullanıcıları görüntüleme, oluşturma ve yönetme| Avantajlar | [Iş Ortağı Merkezi 'nde Microsoft İş Ortağı Ağı üyelik avantajlarınızı ve tekliflerini yönetme](manage-your-partner-network-benefits.md)
||* Tüm iş ortağı profillerini görüntüle | Müşteriler |
||* Iş Ortağı Merkezi için destek biletleri oluşturma | Yardım + destek |
||* Oluşturduğunuz iş ortağı destek biletlerini görüntüle | Yardım + destek |
|Faturalama yöneticisi | -Faturalandırma, faturalar ve keşfi dosyalarını görüntüleyin, oluşturun ve yönetin| Faturalandırma | [Faturanızı okuma](billing.md)
||* Fiyatlandırmayı görüntüle | Faturalandırma |
||* Iş Ortağı Merkezi için destek biletleri oluşturma | Yardım + destek |
||* Oluşturduğunuz iş ortağı destek biletlerini görüntüle | Yardım + destek |
|Varsayılan Kullanıcı|  Profilimi görüntüle   | Hesap ayarları | [Parolanızı sıfırlama](reset-my-pasword.md)
|Yönetim Aracısı | * Müşteri yönetimi| Müşteriler | [Müşterilerinizle bağlantı kurma](connect-with-your-customers.md)
||* Iş Ortağı Merkezi 'ne cihaz listesi ekleme | Hesap ayarları |
||* Cihazlara profiller oluşturma ve uygulama | Hesap ayarları |
||* Abonelik yönetimi | Hesap ayarları |
||* Müşteriler için hizmet durumu ve hizmet istekleri | Yardım + destek |
||* Yönetici temsilcisi ayrıcalıkları iste | Hesap ayarları |
||* Fiyatlandırma ve teklifleri görüntüleme | Fiyatlandırma |
||* Faturalandırma | Faturalandırma |
||* Müşteri adına yönetme | Hesap ayarları |
||* Katma değerli satıcı kaydetme | Hesap ayarları |
||* Iş Ortağı Merkezi için destek biletleri oluşturma | Yardım + destek |
||* Oluşturduğunuz iş ortağı destek biletlerini görüntüle | Yardım + destek |
|Satış Aracısı | * Müşteri yönetimi| Faturalandırma | [Müşterileriniz için faturalandırma desteği sağlayın ve faturalandırma sorularını cevaplayın](provide-billing-support.md)
||* Iş Ortağı Merkezi 'ne cihaz listesi ekleme | Hesap ayarları |
||* Abonelik yönetimi | Hesap ayarları |
||* Destek biletlerini görüntüle | Yardım + destek |
||* Müşteriyle ilişki isteme | Müşteriler |
||* Fiyatlandırma ve teklifleri görüntüleme | Fiyatlandırma |
||* Müşteri adaylarını yönetme | Referanslar |
||* Müşteri anlaşmasını görüntüleme | Müşteriler |
||* Katma değerli kurumsal bayi kaydetme | Hesap ayarları |
||* İş için destek biletleri İş Ortağı Merkezi | Yardım + destek |
||* İş ortağı destek biletlerini görüntüle | Yardım + destek |
|Yardım masası aracısı| * Müşteri arama ve görüntüleme| Yardım + destek | [Sorunları Microsoft'a yükseltme ve Hangi sorunların Microsoft'un yükseltmeye daha uygun olduğunu öğrenme](escalate-problems-to-microsoft.md)
||* Müşteri ayrıntılarını düzenleme  | Yardım + destek |
||* Faturalama veya abonelik yönetimiyle ilgili müşteri sorunlarını çözmeye yardımcı olun | Yardım + destek |
||* Müşteriler adına destek isteği | Yardım + destek |
||* Müşteriler adına abonelikleri ve faturalama sorunlarını yönetme | Faturalandırma |
||* İş için destek biletleri İş Ortağı Merkezi | Yardım + destek |
||* İş ortağı destek biletlerini görüntüle  | Yardım + destek |

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a>Denetim Masası Satıcısı (CPV). (CSP rolü ve Azure AD dışı rol)

CPV'ler, csp iş ortakları tarafından kendi sistemlerini farklı API'lerle tümleştirerek İş Ortağı Merkezi geliştirmektedir.

|**Role**                   | **Yapabilecekleriniz**      | **Çalışma alanı** | **Daha fazla bilgi edinin**|
|------------------------------|:----------------------------|---------------|---------------|
|Genel yönetici| Denetim Masası Vendor (CPV) profilinizi görüntüleme ve yönetme|  | [CSP iş ortağı sistemlerini Denetim Masası API'lerle tümleştirip tümleştirin ve satıcı olarak İş Ortağı Merkezi olun](enroll-as-cpv.md)
||CPV özelliklerine erişmesi gereken kullanıcılarınızı görüntüleme ve yönetme |  |

### <a name="guest-user-must-be-added-to-the-azure-ad-tenant"></a>Konuk kullanıcı (Azure AD kiracısına eklenmiştir)

| **Konuk kullanıcı**    | **Roller**            |
|----------------------|:------------------------|
|                      | MPN iş ortağı yöneticisi       |
|                      | İş profili yöneticisi  |
|                      | Referans yöneticisi         |

## <a name="manage-mpn-membership-and-your-company"></a>MPN üyeliğini ve şirketinizi yönetme

Bu roller **Azure** AD rolleri değildir. Kiracı yerine şirket işletmelerini yönetmek için kullanılır.

| **Role** | **Yapabilecekleriniz** | **Çalışma alanı** | **Daha fazla bilgi edinin**|
|----------------------------|:----------------------------|-----|
|MPN iş ortağı yöneticisi|* İş ortağı hizmeti isteklerini görüntüleme, oluşturma ve yönetme| Üyelik | [Microsoft Eylem Paketi aboneliği veya Silver ve Gold uzmanlık satın alma veya yenileme](mpn-get-action-pack.md) |
| |* Yasal, şirket, iş ve MPN profillerini görüntüleme | Hesap ayarları |
| |* Kullanıcı ayrıntılarını ve beceri verilerini görüntüleme | Üyelik |
| |* Yetkinlikleri görüntüleme | Üyelik |
| |* Avantajları görüntüleme ve yönetme | Avantajlar |
| |* MPN tekliflerini görüntüleme ve satın alma | Üyelik |
| |* MPN tekliflerinin sipariş geçmişini ve faturalarını görüntüleme | Üyelik |
| |* İş ortağı katkısı gösterge verilerini görüntüleme | Üyelik |
| |* Kupon Doğrulama aracında çalışabilirsiniz | Üyelik |
| |* Müşteri veri analizini görüntüleme | Insights |
| |* Şirket içindeki diğer kullanıcı rollerini görüntüleme, ancak rol ataymama | Hesap ayarları |
| |* İş için destek biletleri İş Ortağı Merkezi | Yardım + destek |
| |* İş ortağı destek biletlerini görüntüle | Yardım + destek |
| Hesap yöneticisi| Konum ekleme| Hesap ayarları | [Konumları yönetme](manage-locations.md)
| |* Yönetici olduğunuz hesaplarla ilgili profilleri yönetme | Hesap ayarları |
| |* Kiracılı kullanıcılar için Azure AD olmayan rollere roller atama | Hesap ayarları |
| |* Konumları programlara kaydetme |  |
| |* İş için destek biletleri İş Ortağı Merkezi | Yardım + destek |
| |* İş ortağı destek biletlerini görüntüle | Yardım + destek |

## <a name="manage-referrals"></a>Referansları yönetme

|**Role** | **Yapabilecekleriniz**| **Çalışma alanı** | **Daha fazla bilgi edinin** |
|------------------------------|:---|-----------------------|---|
|Referans yöneticisi|İş Ortağı Merkezi'da Referanslar sekmesinde her şeyi oluşturma ve yönetme| Referanslar | [Ortak satış fırsatlarını yönetme](manage-co-sell-opportunities.md)
||    Tüm ortak satış fırsatlarını ve müşteri adaylarını görüntüleyemez ve düzenleyebilir | Referanslar |
||    Anlaşma için ekip üyeleri atay olabilir | Referanslar |
||    İş profillerini görüntüleyebilir ve düzenleyebilir | Referanslar |
||    Kazanıldı olarak işaretlenen ve anlaşma kaydı için uygun olan fırsatlara yönelik anlaşmalar görüntüleyebilir ve kaydedebilirsiniz | Referanslar |
||    Destek biletleri oluşturabilir ve görüntüleyebilir | Yardım + destek |
|Başvuru kullanıcısı|Ortak satış fırsatlarını yalnızca ekibin bir parçasıysa oluşturun ve yönetin | Referanslar | [Ortak satış fırsatlarını yönetme](manage-co-sell-opportunities.md)
||    Rolün atandığı konumlar için ortak satış fırsatları oluşturabilir. | Referanslar |
||    Kazanıldı olarak işaretlenen ve ekip üyesi olmaları durumunda anlaşma kaydı için uygun olan fırsatlara yönelik anlaşmalar görüntüleyebilir ve kaydedebilirsiniz. | Referanslar |
||    Destek biletleri oluşturabilir ve görüntüleyebilir | Yardım + destek |
|İş profili Yöneticisi|İş profilleri oluşturma ve yönetme | Referanslar | [İş profillerini yönetme](create-a-marketing-profile.md)
||    Destek biletleri oluşturabilir ve görüntüleyebilir | Yardım + destek |

Yeni başvurular Kullanıcı rolüyle birlikte, anlaşmalar için de konum kapsamı da tanıtıyoruz. Aşağıdaki tabloda, konuma göre anlaşmalar erişimi açıklanmaktadır.

|**Kapsam** | **Yapabilecekleriniz** | **Çalışma alanı** |
|------------------------------|:-----------------|--------|
|Tüm şirket | Her iki yönetici ve Kullanıcı, şirketlerinde herhangi bir konum için anlaşmalar oluşturma erişimine sahiptir| Referanslar |
|| Başvuru Yöneticisi tüm anlaşmaları görüntüleme ve düzenleme erişimine sahiptir | Referanslar |
|| Başvuru kullanıcıları yalnızca ekibin bir parçası olduklarında tüm anlaşmaları görüntüleme ve düzenleme erişimine sahiptir | Referanslar |
|Bir veya daha fazla konum | Her iki yönetici ve Kullanıcı, şirketlerinin atandığı konuma yönelik anlaşmalar oluşturmak için erişime sahiptir| Referanslar |
|| Başvuru Yöneticisi atanan konumlara ait tüm anlaşmaları görüntüleme ve düzenleme erişimine sahiptir| Referanslar |
|| Başvuru kullanıcıları ekibin parçasıysa atanan konumlara ait tüm anlaşmaları görüntüleme ve düzenleme erişimine sahiptir| Referanslar |

## <a name="manage-incentives"></a>Teşvikleri yönetme

|**Role** | **Yapabilecekleriniz**| **Çalışma alanı** | **Daha fazla bilgi edinin** |
|---------|:-------------------|---------------|----------------|
|Teşvikleri Yöneticisi|* Teşvikleri 'yi başlatır ve yönetir | Teşvikler | [Teşvikleri kullanmaya başlamanıza yardımcı olması için bu kaynakları kullanın](incentives-get-started-intro.md) |
||* Teşvikleri programlarının tüm yönlerini görüntüleyebilir ve düzenleyebilir | Teşvikler |
||* Banka ve vergi ayrıntılarını görüntüleyebilir ve düzenleyebilir | Teşvikler |
||* İndirim ve ortak işlem kazançlarını görüntüleme | Teşvikler |
||* Erişim desteği | Yardım + destek |
||* İtiraz teşvikleri ödemeleri | Teşvikler |
|Teşvikleri kullanıcısı|* Teşvikleri programlarını görüntüleyebilir | Teşvikler ||
||* Teşvikleri taleplerini görüntüleyebilir ve başlatabilir | Teşvikler |
||* İndirim ve ortak işlem kazançlarını görüntüleme | Teşvikler |
||* Iş Ortağı Merkezi için destek biletleri oluşturma | Yardım + destek |
||* Oluşturduğunuz iş ortağı destek biletlerini görüntüle | Yardım + destek |

## <a name="view-partner-center-insights-data"></a>iş ortağı merkezi Analizler verilerini görüntüle

|**Role** | **Yapabilecekleriniz** | **Çalışma alanı** | **Daha fazla bilgi edinin** |
|---------|:--------------------|---------------|----------------|
|Executive rapor Görüntüleyicisi|Tüm raporlama veri kümelerine erişim, iş ortağı destek biletleri oluşturma, oluşturduğunuz iş ortağı destek biletlerini görüntüleme| Insights | [iş ortağı merkezi 'nde bulunan pano raporlarının genel bakış Analizler](insights-overview-report.md) |
|Rapor Görüntüleyicisi|Gelir ve müşteri ve çalışan kişisel verileri dışında veri raporlarına erişim, iş ortağı destek biletleri oluşturma, oluşturduğunuz iş ortağı destek biletlerini görüntüleme | Insights | |

## <a name="next-steps"></a>Sonraki adımlar

- [Kullanıcı hesabı oluşturup rol ve izin atama](create-user-accounts-and-set-permissions.md)
- [Yeni bir İş Ortağı Merkezi programına kaydolurken hesap bilgilerinizi doğrulama](verification-responses.md)
