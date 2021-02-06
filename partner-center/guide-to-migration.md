---
title: PMC 'den Iş Ortağı Merkezi 'ne geçiş
ms.topic: article
ms.date: 10/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Şirketinizi, izlemeniz gereken adımlar da dahil olmak üzere Iş ortağı üyelik Merkezi 'nden (PMC) Iş Ortağı Merkezi 'ne geçirmeyi öğrenin.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: dd566a6d9ef60747eb7fd515b4d63d87d991da2a
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624196"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>PMC'den İş Ortağı Merkezi'ne geçiş kılavuzu

**Uygun roller**

- Genel yönetici

Partner.microsoft.com adresindeki Microsoft iş ortağı web sitesi, iş ortakları için Birleşik bir dijital deneyimdir. İş ortağı web sitesinden, fırsatlarınızı keşfedebileceğiniz gibi, şirketinizin Microsoft ile uygulamalarınızı ve hizmetlerinizi oluşturmasına ve satmaya yardımcı olan Kılavuzlu deneyimlerden de yararlanabileceksiniz. İş ortağı web sitesinde bulunan pano bağlantısını kullanarak, Microsoft İş Ortağı Ağı üyeleri Microsoft ile ilişkinizi yönettiğiniz iş ortağı merkezinde oturum açabilir, programlara kaydolur ve tekliflere kaydolabilirsiniz.

İş ortağı üyelik Merkezi (PMC) kullanımdan kaldırıldı. Şirketiniz, Microsoft İş Ortağı Ağı üyelik yönetiliğinizi Iş Ortağı Merkezi 'ne geçirmeye davet edildi. Bu kılavuz, PMC 'den Iş ortağı merkezine geçiş yaparken ne beklendiğini size hazırlar.

>[!NOTE]
>Şirketiniz birden fazla hesaba veya konuma sahip olsa bile, Iş Ortağı Merkezi 'ne taşıma işlemi bir (ilk) hesabınızı Iş ortağı merkezine taşıyarak başlar.

## <a name="get-started"></a>başlarken

Taşıma, PMC 'de başlar. Genel yöneticiniz taşımaya başlamak için bir davet alacak.

### <a name="prepare-in-pmc"></a>PMC 'de hazırla

- Şirketinizin ayrıntılarını doğrulayın
- Birincil program ile ilgili kişiyi doğrula
- İş konumlarını doğrulama
- Onaylanan kullanıcılarınızı güncelleştirme

### <a name="when-youre-ready"></a>Hazırsanız

Davetinizi **kullanmaya başlayın** ' ı seçin. Iş Ortağı Merkezi oturum açma sayfasına yönlendirilirsiniz.

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

Mevcut bir AAD kiracısı ile oturum açtıysanız, çalışanlarınız sizinle birlikte taşınacaktır. Bu durumda, Iş Ortağı Merkezi 'nde neler yapabileceğini belirleyen çalışanlar rollerinizi atayın. 

>[!NOTE] 
>Iş ortağı merkezindeki roller PMC 'de rollerden farklıdır. Daha fazla bilgi için bkz. [PMC 'Den Iş ortağı merkezine geçme](move-pmc-pc-map.md).

## <a name="verify-your-domain-and-become-a-global-admin"></a>Etki alanınızı doğrulama ve genel yönetici olma  

AAD kiracınız yeni ise, hiç kimse genel yönetici rolü atanmaz. Genel yönetici olmak için etki alanı sahipliğiniz doğrulamanız gerekir. Bu konuda size yardımcı olması için etki alanı yöneticisine ihtiyacınız olabilir.

Zaten satın almış olduğunuz teklifleri kullanabilmeniz mümkün olsa da, genel yönetici atama adımını tamamlayana kadar yeni bir teklif satın almanız mümkün olmayacaktır.

:::image type="content" source="images/migration/takecontrol.png" alt-text="Denetim al":::

Kullanmaya başlayın ' ı seçtiğinizde aşağıdaki ekranı görürsünüz:

:::image type="content" source="images/migration/verifytxt.png" alt-text="Etki alanı sahipliğini doğrulama":::

Etki alanı kayıt şirketiniz sizin için zaten doldurulmuştur. Yalnızca etki alanı sahibi DNS dosyasını güncelleştirebilir, bu nedenle metin dosyasını kopyalayarak ve DNS kayda ekleyerek, sahibi olduğunuzu doğrulayabiliriz. Güncelleştirmenin gerçekleşmesi birkaç dakika sürer. Iş Ortağı Merkezi oturumunuzu kapatıp yeniden oturum açmanız gerekir. Rolünüzün genel yönetici olarak değiştirilmesi gerekir.

## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>Panonuz ve Iş ortağı merkezinize göre tanışın

Panonuzun turuna katılın. Burada, üyeliğinizi yönetebileceğiniz, başvurular için bir iş profili ekleyebileceğiniz, bulut çözümü sağlayıcısı programına kaydolma ve **Pano**' yı seçerek istediğiniz zaman iş ve tekliflerle ilgili teklifler hakkında bilgi edinebilirsiniz. Ayrıca teşvikleri yönetebilir, Market 'te satın alabilir, pazara sunma hizmetleri için kaydolabilirsiniz ve daha fazlasını yapabilirsiniz.  

:::image type="content" source="images/migration/fre.png" alt-text="Tura katılın":::

## <a name="sign-the-microsoft-partner-agreement"></a>Microsoft Iş ortağı sözleşmesi 'Ni imzala

Dolaylı bir satıcıysanız, Iş Ortağı Merkezi hesabınızı ayarladıktan sonra yine de bulut çözümü sağlayıcısı programına resmi kayıt yapmanız gerekir. Üyelik durumunuzu denetlemek için, [yasal profilinize](https://partner.microsoft.com/pcv/accountsettings/partnerprofile) gidin ve hesap türünü onaylayın. Ardından, CSP 'de dolaylı bir [satıcı](enrolling-in-the-csp-program.md)olarak kaydolun.

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
