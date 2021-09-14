---
title: Müşterilerin CSP 'de kendi hizmetlerini satın almasına izin ver
description: CSP program iş ortaklarının, müşterilerin, Iş Ortağı Merkezi 'nde satın alınan bir abonelik için Azure ayırmaları gibi kendi hizmetlerini satın almasına nasıl yardımcı olabileceğini öğrenin.
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 23ca72fada539b5036dfd6cf0ac04a5c18b5d96d
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248643"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a>Iş Ortağı Merkezi 'nde müşterilere kendi ürünlerini veya hizmetlerini satın alma izni verin

**Uygun roller**: yönetici Aracısı | Satış Aracısı

bu makalede, Bulut Çözümü Sağlayıcısı (CSP) programındaki bir ortağın bir müşterinin kendi hizmet veya kaynaklarından bazılarını satın alma izni verme yöntemi gösterilmektedir.

CSP programındaki iş ortakları, müşterilerine yönelik çözümler ve hizmetler satın almak için genellikle Iş Ortağı Merkezi 'ni ve ticari marketi 'ni kullanır. İş ortakları daha sonra bazı müşterilerin bu hizmetleri doğrudan Azure portal sağlamasına izin verir.

Aşağıda bir örneği yer alır. Iş Ortağı Merkezi 'nde müşteri için bir Azure plan aboneliği satın aldığınızı varsayalım. Daha sonra bu aboneliğe diğer kaynakları veya Hizmetleri Müşterinin adına eklemeye karar verirsiniz. Bu durumda, müşterinin aboneliğine Azure ayırmaları ekleyebilirsiniz (örneğin, ayrılmış, sanal makine örnekleri ekleme). Daha sonra müşterinin Azure portal Azure ayırma kaynaklarını daha fazla sağlamasını sağlayabilirsiniz.

Artık **Müşteri izinleri** özelliği Ile müşterilere Azure kaynaklarıyla daha fazla self servis seçeneği verirsiniz. Müşteri için izinleri etkinleştirerek müşterilerin kendi kaynaklarını satın almasını (örneğin, kendi Azure ayırmalarını satın almasını) sağlayabilirsiniz.  

## <a name="overview-of-customer-permissions-in-partner-center"></a>Iş Ortağı Merkezi 'nde müşteri izinlerine genel bakış

Müşteri izinlerini açmak (veya devre dışı bırakmak) için müşteri **hesabı** sayfasını kullanın. Şu anda bu özellik şunları destekler:

- **Azure ayırmaları:** Bu izni açmak, müşterinin satın almış olduğunuz belirli bir Azure aboneliği için kendi Azure ayırmalarını satın almasına izin verir.

Müşteri izinlerini açmadan önce şu önemli noktaları aklınızda bulabilirsiniz:

- Varsayılan olarak, Iş Ortağı Merkezi 'nde müşteri izinleri otomatik olarak devre dışı bırakılır (kapalı bırakılır).

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
> Müşterilere kendi Azure ayırmalarını satın alma izni verdikten sonra, satın aldıkları rezervasyonları yönetmesine yardımcı olun. Daha fazla bilgi için bkz. [müşterilerin satın aldıkları ayırmaları yönetmesine yardımcı olma](give-customers-permission.md#help-customers-manage-reservations-they-purchase).

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>Müşterilerin kendi Azure ayırmalarını satın almasını sağlamak için

1. Müşterinin kendi adına satın aldığınız mevcut bir Azure planına veya Azure genel aboneliğine sahip olduğunu doğrulayın.

2. Müşterinin bu abonelik için **sahip** rolüne atandığını doğrulayın.

3. Kendi Azure ayırmalarını satın almak için müşteri izinlerini etkinleştirin (Bu özelliği **etkinleştirin).**

Her adım aşağıda görünür.

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>Müşterinin mevcut bir Azure aboneliğine sahip olduğunu doğrulayın

Müşterilere kendi Azure ayırmalarını satın alma izni vermeden önce, müşterinin mevcut bir Azure planına veya Azure genel aboneliğine sahip olduğunu doğrulamanız gerekir. Müşteri, Iş Ortağı Merkezi 'nde geçerli bir Azure aboneliği gösteriyorsa, müşteri izinlerini açmadan önce bu abonelik için bir abonelik satın almanız gerekir.

- Bir müşterinin zaten bir Azure aboneliğine sahip olup olmadığını görmek için Iş Ortağı Merkezi panosunda oturum açın ve ardından **CSP** ' yi ve ardından **müşteriler**' i seçin. Listeden belirli müşteriyi seçin. Ardından **abonelikler** ' i seçin ve Azure planı ya da Azure Global için kullanım tabanlı abonelikler için arama yapın.

- Bir müşterinin mevcut bir Azure aboneliği yoksa, bunlar için bir abonelik satın alabilirsiniz. Bkz. [Azure planını satın alma](purchase-azure-plan.md).

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>Müşterinin Azure 'da doğru rolün atandığını doğrulayın

Müşterinin mevcut bir Azure aboneliğine sahip olduğunu doğruladıktan sonra, müşterinizin ilişkilendirildiği anahtar kullanıcılara bu Azure aboneliği için doğru **sahip** rolü atandığını da doğrulamanız gerekir. Bu, müşterinin satın aldığınız bir Azure aboneliği için Azure ayırmaları satın alması gereken rol tabanlı erişimdir (RBAC).

Bazı iş ortakları, kendi Azure kaynaklarını etkin bir şekilde yönetmek ve sağlamak isteyen müşterilere **sahip** rolüne zaten atanmış olabilir. Satın aldığınız önceki abonelikleri yönetmek üzere bir müşteriye zaten **sahip** durumu atadıysanız, bu adımı atlayabilirsiniz.  

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

**Müşteriler, ayırmaları için ödeme yapacak fiyatlar.** Müşteriniz, CSP iş ortağı faturalandırma hesabınızda daha önce satın aldığınız bir aboneliğe göre Azure ayırmaları satın alır. Müşterinin, bu aboneliğe göre satın aldıkları tüm Azure ayırmaları için fiyatı sizin sizin tarafınızdan de ayarlanır. Bu fiyat, müşterinin Azure portal gördüğü web doğrudan fiyatından farklı olabilir.

**Müşteriler bir ayırma kullanımını nasıl iyileştirebilirler.** Bazı müşteriler, bir ayırma kullanımını iyileştirmek veya satın alma sırasında rezervasyonun ilk kapsamını atamak hakkında daha fazla bilgi edinmeye yarar sağlayabilir. Daha fazla bilgi için müşterilerin [Azure kaynakları için ayırmaları yönetme](/azure/cost-management-billing/reservations/manage-reserved-vm-instance)bilgilerini okumasını isteyin.

**Bir müşteri, paylaşılan bir kapsama sahip bir rezervasyon satın aldığında ne olur?** Müşteriler önceki bir CSP aboneliğine göre bir ayırma satın alıp bu ayırmaya bir paylaşılan kapsam atadıktan sonra, müşterinin CSP tarafından verilen tüm indirimler, CSP iş ortağı tarafından satın alınan tüm abonelikler için eşleşen kullanım için geçerlidir.

**Müşteriler, yapmış oldukları bir satın alma, iptal etme veya yenileme ya da bir ayırmanın başlangıç kapsamını değiştirme amacıyla ne yapması gerekir?** Müşterilerin, bir ayırmanın ilk kapsamını değiştirmesine yardımcı olması için iş ortağlarına sormaları gerekir. Ayrıca, bir ayırmayı Exchange, iptal etme veya yenileme için bir iş ortağının yardımına de ihtiyacı vardır. Bu görevleri, kendilerine bir CSP iş ortağı tarafından satın alınan abonelikler temelinde rezervasyon ile gerçekleştiremez.

## <a name="next-steps"></a>Sonraki adımlar

- [Müşterileriniz adına Azure ayırmaları satın alın](azure-reservations-buying.md)

- [İş Ortağı Merkezi-Microsoft ayırmaları satma](azure-reservations.md)

- [Azure rezervasyonlarını müşterileriniz adına yönetme](azure-reservations-manage.md)