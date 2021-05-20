---
title: PMC'den İş Ortağı Merkezi
ms.topic: article
ms.date: 10/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Takip etmek için gereken adımlar dahil olmak Partner Membership Center (PMC) İş Ortağı Merkezi şirket geçişini öğrenin.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 511612042f7da5e43d045d2991fa7d5251612726
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150752"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>PMC'den İş Ortağı Merkezi'ne geçiş kılavuzu

**Uygun roller:** Genel yönetici

partner.microsoft.com Microsoft iş ortağı web sitesi, iş ortakları için birleşik bir dijital deneyimdir. İş ortağı web sitesinden, fırsatlarınızı keşfedecek ve microsoft ile uygulama ve hizmetlerinizi derlemenize ve satmanıza yardımcı olacak kılavuzlu deneyimlerle etkileşim kurabileceksiniz. İş ortağı web sitesinde bulunan Pano bağlantısını kullanarak Microsoft İş Ortağı Ağı üyeleri Microsoft ile ilişkinizi yönetebilirsiniz, programlara kaydolabilirsiniz ve tekliflere kaydolabilirsiniz.

Partner Membership Center (PMC) kaldıriliyor. Şirket, şirket üyeliği yönetiminizi Microsoft İş Ortağı Ağı geçişe İş Ortağı Merkezi. Bu kılavuz, PMC'den yeni bir İş Ortağı Merkezi.

>[!NOTE]
>Şirketinizin birden fazla hesabı veya konumu olsa bile, bir (ilk) İş Ortağı Merkezi bir hesap başka bir hesaba taşınarak İş Ortağı Merkezi.

## <a name="get-started"></a>başlarken

Taşıma PMC'de başlar. Genel yöneticiniz taşımaya başlamak için bir davet alır.

### <a name="prepare-in-pmc"></a>PMC'de hazırlama

- Şirket ayrıntılarınızı doğrulama
- Birincil program ilgili kişisi doğrulama
- İş konumlarını doğrulama
- Onaylı kullanıcılarınızı güncelleştirme

### <a name="when-youre-ready"></a>Hazır olduğunda

Davet **Kullanmaya başlayın** seçin. Oturum açma İş Ortağı Merkezi alınır.

:::image type="content" source="images/migration/getstarted.jpg" alt-text="Kullanmaya başlama":::

## <a name="start-with-your-work-email"></a>İş e-postalarınızı kullanmaya başlayın

Şirketinizde iş e-postası ve AAD kiracısı yoksa, iş ortağı merkezi oturum açma işlemi sırasında bir tane ayarlamanıza yardımcı olabilirsiniz. Kişisel hesabınız gibi iş e-postası olmayan bir e-posta hesabıyla oturum açmaya çalıştığınızda, bir AAD kiracısı ve iş e-postası ayarlayabilmemiz için şirketiniz hakkında bilgi sağlamak üzere yönlendirilirsiniz. Bu Şirket ayrıntıları, Iş Ortağı Merkezi 'nde hesabınızı tamamlamak için kullanılacaktır, bu yüzden doğru olduklarından emin olun.

>[!NOTE]
>Çin 'de bir iş ortağıysanız ve hem Microsoft İş Ortağı Ağı hem de bulut çözümü sağlayıcısı (CSP) programına kaydolduysanız her hesap için ayrı bir kiracıya sahip olursunuz. Bulut çözümü sağlayıcısı programı ile hesabınız Ulusal bulutta yönetilir ve Microsoft İş Ortağı Ağı hesabınız genel bulutta yönetilir. İki hesap bağlanamaz.

:::image type="content" source="images/migration/newtellusabout.png" alt-text="Bize şirketiniz hakkında bilgi verin":::

Bilgileri doğruladıktan veya güncelleştirdikten sonra, **kabul et ve devam et**' i seçin.
Bu sayfadaki hüküm ve koşullar, şirketinizin zaten PMC 'de oturum açmış olduğu anlaşmayla **aynıdır** .  
Bu adım, Azure AD kiracınızın oluşturulmasını başlatır ve size iş hesabı sağlar.

**Kabul et ve devam et '** i seçmek aşağıdakileri de yapar:

- Hesabınızı tüm konumlarına birlikte Iş Ortağı Merkezi 'ne geçirir

- PMC 'de satın almış olabileceğiniz tüm Uzmanlıklar veya haritaları geçirir

- PMC 'de bulunan tüm pazarlama kaynaklarını, teklifleri ve programları (haritalar, gümüş, altın) geçirir

## <a name="invite-employees-to-join-you"></a>Çalışanlara katılmaya davet edin

Yeni Azure AD kiracınız oluşturulduğunda, çalışanlarınızın Iş Ortağı Merkezi 'Nde oturum açmasını davet edebilirsiniz.

:::image type="content" source="images/migration/invite.png" alt-text="Çalışanları davet et":::

Mevcut bir AAD kiracısı ile oturum açtıysanız, çalışanlarınız sizinle birlikte taşınacaktır. Bu durumda, Iş Ortağı Merkezi 'nde neler yapabileceğini yönetmek için çalışanlar rollerinizi atayın. 

>[!NOTE] 
>Bu İş Ortağı Merkezi PMC'de yer alan rollerden farklıdır. Daha fazla bilgi için [bkz. PMC'den İş Ortağı Merkezi.](move-pmc-pc-map.md)

## <a name="verify-your-domain-and-become-a-global-admin"></a>Etki alanınızı doğrulayın ve genel yönetici olun  

AAD kiracınız yeni ise, hiç kimse genel yönetici rolüne atanmaz. Genel yönetici olmak için etki alanı sahipliğinizi doğrulamanız gerekir. Bu konuda size yardımcı olmak için etki alanı yöneticisine ihtiyacınız olabilir.

Önceden satın aldığınız teklifleri kullanabilirsiniz ancak genel yönetici atama adımını tamamlayana kadar yeni teklif satın alamayabileceksiniz.

:::image type="content" source="images/migration/takecontrol.png" alt-text="Denetimi ele alma":::

Çalışmaya başlama'yi seçerek aşağıdaki ekranı görürsünüz:

:::image type="content" source="images/migration/verifytxt.png" alt-text="Etki alanı sahipliğini doğrulama":::

Etki alanı kayıt şirketiniz sizin için zaten doldurulur. DNS dosyasını yalnızca etki alanı sahibi güncelleştirene kadar, metin dosyasını kopyalayıp DNS kaydınıza ekleyerek sahibin siz olduğunu doğrularız. Güncelleştirmenin gerçekleşmesi birkaç dakika sürer. Oturum açma ve İş Ortağı Merkezi yeniden oturum açmanız gerekir. Rolünüz genel yönetici olarak değiştirilmiştir.

## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>Pano ve panolar hakkında bilgi İş Ortağı Merkezi

Pano turlarını izleyin. Burada üyeliğinizi yönetebilirsiniz, referanslar için bir iş profili ekleyebilir, Bulut Çözümü Sağlayıcısı programına kaydolabilirsiniz ve Pano'u seçerek istediğiniz zaman işletmenize uygun bildirimleri ve teklifleri **görebilirsiniz.** Ayrıca teşvikleri yönetebilir, marketten satın alabilirsiniz, pazara giriş hizmetleri için kaydolabilirsiniz ve daha fazlasını da kullanabilirsiniz.  

:::image type="content" source="images/migration/fre.png" alt-text="Tura at":::

## <a name="sign-the-microsoft-partner-agreement"></a>Oturum Microsoft İş Ortağı Sözleşmesi

Dolaylı kurumsal bayiysiniz, İş Ortağı Merkezi hesabı ayar Bulut Çözümü Sağlayıcısı gerekir. Üyelik durumunuzu denetlemek için, [yasal profilinize](https://partner.microsoft.com/pcv/accountsettings/partnerprofile) gidin ve hesap türünü onaylayın. Ardından, CSP 'de dolaylı bir [satıcı](enrolling-in-the-csp-program.md)olarak kaydolun.

 Dolaylı bir satıcı olarak kaydolduktan sonra, [dolaylı sağlayıcınızla CSP ilişki isteğini](indirect-reseller-tasks-in-partner-center.md)kabul edin.

Sonra, genel yönetici kimlik bilgilerini kullanarak Iş Ortağı Merkezi [panosuna](https://partner.microsoft.com/pvc/dashboard) genel bakış ' a Microsoft Iş ortağı sözleşmesi 'ni kabul edin Iş ortağı profilinin program bilgileri bölümünde Microsoft Iş ortağı Sözleşmesi ' ni imzaladığınızı doğrulayın. Ayrıca, CSP Genel Bakış sayfasında bir onay başlığı bildirimi görürsünüz. 

## <a name="next-steps"></a>Sonraki adımlar

- [Genel yöneticinizle bulun](become-global-admin.md)

- [Microsoft İş Ortağı Sözleşmesi](microsoft-partner-agreement.md)

- [Kullanıcı hesapları oluşturma](create-user-accounts-and-set-permissions.md)

- [Kullanıcı rollerini ve izinlerini atama](permissions-overview.md)

- [Üyelik programlarınızı yönetme](renew-mpn-offers.md)

- [Şirketinizin iş profilini oluşturma](create-a-marketing-profile.md)

- [Başvurular aracılığıyla müşterilerle bağlantı kurmak](manage-leads.md)

- [Birden çok şirketi PMC 'den Iş Ortağı Merkezi 'ne geçirmeye yönelik kılavuz](move-multiple-companies.md)
