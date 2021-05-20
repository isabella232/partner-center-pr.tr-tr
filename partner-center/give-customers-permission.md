---
title: Müşterilerin CSP'de kendi hizmetlerini satın almalarına izin verme
description: CSP programı iş ortaklarının, müşterilere azure rezervasyonları gibi kendi hizmetlerini satın almalarına nasıl izin ve İş Ortağı Merkezi.
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9fabd6bd188c9d596128672d9fce3321db9b5432
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150769"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a>Müşterilere kendi İş Ortağı Merkezi hizmetlerini satın almaları için izin verme

**Uygun roller:** Yönetici aracısı | Satış aracısı

Bu makalede, Bulut Çözümü Sağlayıcısı (CSP) programı kapsamındaki bir iş ortağının bir müşteriye kendi hizmet veya kaynaklarını satın alma izni vermesine nasıl izin ver olduğu gösterir.

CSP programı iş ortakları genellikle İş Ortağı Merkezi ve ticari marketini kullanarak müşterilerine çözüm ve hizmet satın alır. İş ortakları daha sonra bazı müşterilerin bu hizmetleri doğrudan doğrudan hizmetlerden sağlamalarına Azure portal.

Aşağıda bir örneği yer alır. Bir müşteri için azure planı aboneliği satın alasınız ve İş Ortağı Merkezi. Ardından bu aboneliğe müşteri adına başka kaynaklar veya hizmetler eklemeye karar veriyorsanız. Bu durumda, müşterinin aboneliğine (ayrılmış sanal makine örnekleri ekleme gibi) Azure rezervasyonları ekebilirsiniz. Daha sonra müşterinin Azure rezervasyon kaynaklarını daha fazla sağlamalarına izin ve Azure portal.

Şimdi Müşteri izinleri **özelliğiyle,** Müşterilere Azure kaynaklarıyla daha fazla self servis seçeneği sunarsınız. Müşterinin izinlerini kullanarak, müşterilerin kendi kaynaklarını satın almalarına (örneğin, kendi Azure rezervasyonlarını satın almalarına) izin vesersiniz.  

## <a name="overview-of-customer-permissions-in-partner-center"></a>İş Ortağı Merkezi'daki müşteri izinlerine genel bakış

Müşteri **izinlerini** açmak (veya kapatmak) için Müşteri Hesabı sayfasını kullanın. Şu anda bu özellik şunları destekler:

- **Azure rezervasyonları:** Bu iznin açması, müşterinin sizin satın aldığınız belirli bir Azure aboneliği için kendi Azure rezervasyonlarını satın almalarına olanak sağlar.

Müşteri izinlerini açmadan önce şu önemli noktalara dikkat olun:

- Varsayılan olarak, müşteri izinleri otomatik olarak devre dışı bırakılır (İş Ortağı Merkezi.

- Bir müşteri için izinleri açmak (veya devre dışı bırakmak) için önce Iş Ortağı Merkezi ' nde yönetici Aracısı rolüne atanmalısınız.

  Satış aracısının veya yardım masası aracısının rolüne atanan iş ortakları salt okuma erişimine sahiptir ve müşteri izinlerini açıp kapatamaz.

- Seçtiğiniz herhangi bir müşteri için izinleri açabilir (etkinleştirebilirsiniz).

- Iş Ortağı Merkezi panosunu ya da [Iş Ortağı Merkezi API 'lerini](/partner-center/develop/manage-customers)kullanarak müşteri izinlerini açabilir veya kapatabilirsiniz.

- Belirli bir müşteri için izinleri etkinleştirdikten (etkinleştirdikten) sonra, bu müşterinin yaptığı sonraki satınalmalara ödeme yapmaktan sorumlu olursunuz. Müşteriler yaptıkları bir satın alma işlemini iptal etmek veya yenilemek (ya da bir ayırmanın ilk kapsamını değiştirmek istiyorlarsa) istiyorlarsa, kendileri bu şekilde yapamazlar. İş ortağı olarak, iş ortakları olarak alışveriş, iptal etme ve yenileme işlemlerini ve daha sonra bir rezervasyon kapsamında değişiklik yapmayı ister.  

- Belirli bir müşteri için izinleri etkinleştirdikten sonra, müşteri tarafından yapılan daha sonraki **satın almalarla ilgili bilgilendirilmeyecektir** .

- Müşteri tarafından daha sonra yapılan satın alma işlemleri, Iş Ortağı Merkezi 'nde, sizin tarafınızdan yapılan tüm satın alımlar ile birlikte görüntülenir Bu satınalmaları müşterinin **Sipariş geçmişi** sayfasında, **rezervasyonlar** sayfasında veya [**etkinlik günlüğünde**](activity-logs.md)bulabilirsiniz.

>[!NOTE]
> Müşterinin ödeyecektir ve müşterilerin satın almalarını yönetmesine yardımcı olacak fiyatlar hakkında bilgi için bkz. [müşterilerin satın aldıkları ayırmaları yönetmesine yardımcı olma](give-customers-permission.md#help-customers-manage-reservations-they-purchase).

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>Müşterilere kendi Azure ayırmalarını satın alma izni verin

Azure ayırmaları, Azure hizmetlerini indirimli bir ücret karşılığında satın almanın harika bir yoludur. Azure ayırmalarının avantajları hakkında daha fazla bilgi edinmek için bkz. [Azure rezervasyonları nelerdir?](/azure/cost-management-billing/reservations/save-compute-costs-reservations)

Artık zaten yaptığınız gibi müşterileriniz adına Azure ayırmaları satın alma seçeneğiniz vardır. Ya da müşterilere kendi Azure ayırmalarını satın alma izni verebilirsiniz.

>[!NOTE]
> Müşterilere kendi Azure rezervasyonlarını satın alma izni verdikten sonra, satın aldıkları rezervasyonları yönetmelerine yardımcı olur. Daha fazla bilgi için [bkz. Müşterilerin satın aldıkları rezervasyonları yönetmeye yardımcı olur.](give-customers-permission.md#help-customers-manage-reservations-they-purchase)

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>Müşterilerin kendi Azure rezervasyonlarını satın almalarını sağlamak için

1. Müşterinin kendi adına satın aldığınız bir Azure Planı veya Azure Genel aboneliği olduğunu doğrulayın.

2. Müşteriye bu abonelik için Sahip **rolü atandığı** doğrulayın.

3. Kendi Azure rezervasyonlarını satın almak için **müşteri** izinlerini etkinleştirin (bu özelliği Aç) .

Her adım aşağıda görünür.

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>Müşterinin mevcut bir Azure aboneliğine sahip olduğunu doğrulama

Müşterilere kendi Azure rezervasyonlarını satın alma izni vermeden önce müşterinin mevcut bir Azure Planı veya Azure Genel aboneliğine sahip olduğunu doğrulamanız gerekir. Müşteri abonelikte geçerli Azure aboneliğini İş Ortağı Merkezi, müşteri izinlerini açmadan önce onun için bir abonelik satın alasınız.

- Müşterinin zaten bir Azure aboneliği olup olduğunu görmek için İş Ortağı Merkezi panosunda oturum açın, **ardından CSP'yi** ve ardından **Müşteriler'i seçin.** Listeden belirli bir müşteriyi seçin. Ardından **Abonelikler'i** seçin ve Azure Planı veya Azure Genel için kullanım tabanlı abonelikleri arama.

- Müşterinin mevcut bir Azure aboneliği yoksa, onun için bir abonelik satın alabilirsiniz. Bkz. [Azure Planı satın alma.](purchase-azure-plan.md)

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>Müşteriye Azure'da doğru rolün atandığı doğrulayın

Müşterinin mevcut bir Azure aboneliğine sahip olduğunu doğruladikten sonra, müşteriyle ilişkili önemli kullanıcılara bu Azure aboneliği için doğru **Sahip** rolünün atandığı da doğru olur. Bu, müşterinin satın aldığınız Azure aboneliği için Azure rezervasyonları satın almaları gereken rol tabanlı erişimdir (RBAC).

Bazı iş ortakları, kendi Azure kaynaklarını **etkin bir** şekilde yönetmek ve sağlamak isteyen müşterilere Zaten Sahip rolü atamış olabilir. Satın aldığınız önceki abonelikleri yönetmek üzere bir müşteriye zaten **sahip** durumu atadıysanız, bu adımı atlayabilirsiniz.  

> [!IMPORTANT]
> Bir müşteriye **sahip** rolü atanmamışsa, Azure ayırmaları satın almasını önlemek Azure Portal bir hata alırlar.

Müşteriyi, bir Azure aboneliği için **sahip** rolü atandığını doğrulamak için:

1. Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.

2. **CSP**' yi ve ardından **müşteriler** ' i seçin ve belirli müşteriyi seçin.

3. Bu müşteri için **abonelikler** ' i seçin ve belirli Azure aboneliğini bulun.

4. Müşterinin aboneliğinin yanındaki **Yönet** düğmesini seçin. Bunu yapmak [Azure Portal](https://portal.azure.com/)açar.

5. **Sahibi** rolünü belirli bir kullanıcıya atamak için, [bir kullanıcıyı yönetici olarak atamak üzere](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator)bu adımları izleyin.

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>Kendi Azure ayırmalarını satın almak için müşteri izinlerini açın veya kapatın

Müşterinin mevcut bir Azure aboneliğine sahip olduğunu ve kullanıcılara bu abonelik için **sahip** rolü atandığını doğruladıktan sonra, müşteri izinlerini açmaya (etkinleştirmeye) hazırsınız demektir. Ayrıca, müşteri izinlerini kapatmak (devre dışı bırakmak) için de bu adımları kullanabilirsiniz. Iş Ortağı Merkezi panosunu ya da [Iş Ortağı Merkezi API 'lerini](/partner-center/develop/manage-customers)kullanarak müşteri izinlerini etkinleştirebilir veya devre dışı bırakabilirsiniz.

Iş Ortağı Merkezi 'nde müşteri izinlerini açmak (veya devre dışı bırakmak) için:

1. Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.

2. Sol gezinti menüsünde, **CSP**' yi ve ardından **müşteriler**' i seçin. Bir müşteri listesi görüntülenir.

3. Belirli bir müşteri adı seçin.

4. Müşteri menüsünden **Hesap** ' ı seçin. Müşteri **hesabı** sayfası görüntülenir.

5. Sayfanın alt kısmındaki **Müşteri izinleri** alanını bulun.

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="Hesap sayfasında müşteri izinleri." border="true":::

6. **Azure ayırmaları** bölümünde **müşterinin satınalmaya izin ver** seçeneğini bulun.

7. Müşteri izinlerini açmak için bu seçeneğin yanındaki anahtarı **Açık** konuma taşıyın. Müşteri izinlerini kapatmak için, anahtarı **kapalı** konuma taşıyın.

>[!NOTE]
> Müşterinin kendi Azure ayırmalarını satın alma izinlerini açtığınızda ne olacağını öğrenmek için bkz. [Iş Ortağı Merkezi 'nde müşteri Izinlerine genel bakış](give-customers-permission.md#overview-of-customer-permissions-in-partner-center).
>
>Müşteri izinlerini açtığınızda (veya kapattığınızda), etkinlik günlüğü her eylemi kaydeder. (Iş Ortağı Merkezi panosunun en üstünden dişli simgesini seçtiğinizde bu günlüğe erişilebilir. Müşteri izinlerini açtığınızda veya devre dışı bırakırsanız, eylem, etkinlik günlüğündeki **müşteri satın alma Izinleri oluştur** veya **müşteri satın alma izinlerini Sil** olarak görüntülenir.

## <a name="help-customers-manage-reservations-they-purchase"></a>Müşterilerin satın aldıkları ayırmaları yönetmesine yardımcı olma

Müşterilere kendi Azure ayırmalarını satın alma izni verdiğinizde, satın aldıkları kaynakları daha iyi yönetebilmek için size yardımcı olabilirsiniz. Müşteriler, Azure ayırmalarının birçok yönünü doğrudan [Azure Portal](https://portal.azure.com/)yönetebilir. CSP aboneliğiniz dahilinde satın aldıkları Azure ayırmalarının birkaç, diğer yönlerini yönetmek için yardımınızın olması gerekir.  

Azure ayırmalarının bu yönlerini yönetme hakkında daha fazla bilgi edinmek için yardıma yardımcı olun:

- Müşterilerin Azure ayırmaları için ödeme yapacak fiyatlar
- Müşteriler Azure ayırmaları kullanımını nasıl iyileştirebilirler
- Müşteriler, bir paylaşılan kapsama sahip ayırmaları satın aldığında ne olur?
- Müşteriler bir ayırmayı değiştirmek, iptal etmek ve yenilemek ya da kapsamını değiştirmek istiyorsam ne olur?

**Müşteriler, ayırmaları için ödeme yapacak fiyatlar.** Müşteriniz, CSP iş ortağı faturalandırma hesabınızda daha önce satın aldığınız bir aboneliğe göre Azure ayırmaları satın alır. Bu aboneliğe göre satın aldıkları Tüm Azure rezervasyonları için müşterinin fiyatı da sizin tarafından ayarlanır. Bu fiyat, müşterinin hizmette gördüğü Web Direct fiyatından farklı Azure portal.

**Müşterilerin rezervasyon kullanımını nasıl en iyi duruma getirmeleri.** Bazı müşteriler, rezervasyon kullanımını iyileştirme veya satın alma sırasında rezervasyonun ilk kapsamını atama hakkında daha fazla bilgi elde etme avantajından yararlanabilir. Daha fazla bilgi için, müşterilerden Azure kaynakları [için rezervasyonları yönetme makalelerini okumalarını sorun.](/azure/cost-management-billing/reservations/manage-reserved-vm-instance)

**Müşteri, paylaşılan kapsamda bir rezervasyon satın aldıktan sonra ne olur?** Müşteriler önceki bir CSP aboneliğine göre rezervasyon satın alan ve bu rezervasyona paylaşılan bir kapsam atasa, CSP tarafından müşteriye verilen indirimler, CSP iş ortağının o müşteri için satın alan tüm abonelikler için eşleşen kullanım için geçerli olur.

**Müşterilerin, yapmış olduğu bir satın alma işlemini değiştirmek, iptal etmek veya yenilemek ya da rezervasyonun ilk kapsamını değiştirmek istemeleri durumunda ne yapmaları gerekir?** Müşterilerin iş ortaklarından rezervasyonun ilk kapsamını değiştirmelerine yardımcı olmak istemesi gerekir. Ayrıca rezervasyonu değiştirme, iptal etme veya yenileme için bir iş ortağının yardımı da gerekir. CsP iş ortağı tarafından satın alınan abonelikleri temel alan rezervasyonlarla bu görevleri kendileri gerçekleştirebilirler.

## <a name="next-steps"></a>Sonraki adımlar

- [Müşterileriniz adına Azure rezervasyonları satın alma](azure-reservations-buying.md)

- [İş Ortağı Merkezi - Microsoft rezervasyonları satma](azure-reservations.md)

- [Müşterileriniz adına Azure rezervasyonlarını yönetme](azure-reservations-manage.md)