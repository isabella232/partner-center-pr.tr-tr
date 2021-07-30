---
title: Müşterilerin CSP'de kendi hizmetlerini satın almalarına izin verme
description: CSP programı iş ortaklarının, müşterilere azure rezervasyonları gibi kendi hizmetlerini satın almalarına nasıl izin ve İş Ortağı Merkezi.
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: aced617bbe46465d9a82478a41b2f1c4a05309be
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114841428"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a>Müşterilere kendi İş Ortağı Merkezi hizmetlerini satın almaları için izin verme

**Uygun roller:** Yönetici aracısı | Satış aracısı

Bu makalede, Bulut Çözümü Sağlayıcısı (CSP) programı kapsamındaki bir iş ortağının müşteriye kendi hizmet veya kaynaklarını satın alma izni vermesine nasıl izin ver olduğu gösterir.

CSP programı iş ortakları genellikle İş Ortağı Merkezi ve ticari marketini kullanarak müşterilerine çözüm ve hizmet satın alır. İş ortakları daha sonra bazı müşterilerin bu hizmetleri doğrudan doğrudan hizmetlerden sağlamalarına Azure portal.

Aşağıda bir örneği yer alır. Bir müşteri için azure planı aboneliği satın alasınız ve İş Ortağı Merkezi. Ardından bu aboneliğe müşteri adına başka kaynaklar veya hizmetler eklemeye karar veriyorsanız. Bu durumda, müşterinin aboneliğine (ayrılmış sanal makine örnekleri ekleme gibi) Azure rezervasyonları ekebilirsiniz. Daha sonra müşterinin Azure rezervasyon kaynaklarını daha fazla sağlamalarına izin ve Azure portal.

Şimdi Müşteri izinleri **özelliğiyle,** Müşterilere Azure kaynaklarıyla daha fazla self servis seçeneği sunarsınız. Müşterinin izinlerini alarak, müşterilerin kendi kaynaklarını satın almalarına (örneğin, kendi Azure rezervasyonlarını satın almalarına) izin vesersiniz.  

## <a name="overview-of-customer-permissions-in-partner-center"></a>İş Ortağı Merkezi'daki müşteri izinlerine genel bakış

Müşteri **izinlerini** açmak (veya kapatmak) için Müşteri Hesabı sayfasını kullanın. Şu anda bu özellik şunları destekler:

- **Azure rezervasyonları:** Bu iznin açması, müşterinin sizin satın aldığınız belirli bir Azure aboneliği için kendi Azure rezervasyonlarını satın almalarına olanak sağlar.

Müşteri izinlerini açmadan önce şu önemli noktalara dikkat olun:

- Varsayılan olarak, müşteri izinleri otomatik olarak devre dışı bırakılır (İş Ortağı Merkezi.

- Bir müşterinin izinlerini açabilirsiniz (veya kapatabilirsiniz) önce, bu hizmette Yönetici Aracısı rolü İş Ortağı Merkezi.

  Satış Aracısı veya Yardım Masası Aracısı rolünü atamış iş ortakları salt okunur erişime sahip olur ve müşteri izinlerini aç/kapatamz.

- Seçtiğiniz herhangi bir müşteri için izinleri etkinleştirebilirsiniz (etkinleştirebilirsiniz).

- İş Ortağı Merkezi panosu veya api'leri kullanarak müşteri izinlerini İş Ortağı Merkezi [kapatabilirsiniz.](/partner-center/develop/manage-customers)

- Belirli bir müşteri için izinleri etkinleştirdikten (etkinleştirdikten) sonra, bu müşteri tarafından yapılan sonraki satın almalar için ödeme yapmak sizin sorumluluğunda olur. Müşteriler yaptıkları bir satın alma işlemini değiştirmek, iptal etmek veya yenilemek (veya rezervasyonun ilk kapsamını değiştirmek) isterse, bunu kendileri yapmaları mümkün olmayacaktır. İş ortağı olarak sizden satın almaları değiştirmelerine, iptal etmelerine ve yenilemelerine veya rezervasyon kapsamında daha sonra değişiklikler yapmalarına yardımcı olmak için sizden istemesi gerekir.  

- Belirli bir müşteri için izinleri açmanın ardından, **daha** sonra müşteri tarafından yapılan satın almalar size bildirlanmaz.

- Müşteri tarafından daha sonra yapılan satın almalar, İş Ortağı Merkezi satın almaların yanı sıra bu hizmette görünür. Bu satın almaları müşterinin Sipariş **geçmişi** sayfasında, Rezervasyonlar **sayfasında** veya Etkinlik Günlüğünde [**bulabilirsiniz.**](activity-logs.md)

>[!NOTE]
> Müşterinin ödeyecekleri fiyatlar ve müşterilerin satın almalarını yönetmelerine nasıl yardımcı olacakları hakkında bilgi için bkz. Müşterilerin satın [aldıkları rezervasyonları yönetmelerine yardımcı olur.](give-customers-permission.md#help-customers-manage-reservations-they-purchase)

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>Müşterilere kendi Azure rezervasyonlarını satın alma izni verme

Azure rezervasyonları, Azure hizmetlerini indirimli fiyatla satın almak için harika bir yol sağlar. Azure rezervasyonlarının avantajları hakkında daha fazla bilgi edinmek için [bkz. Azure Rezervasyonları nedir?](/azure/cost-management-billing/reservations/save-compute-costs-reservations)

Artık zaten yapıyor gibi müşterileriniz adına Azure rezervasyonları satın alma seçeneğine sahipsiniz. Veya müşterilere kendi Azure rezervasyonlarını satın alma izni veabilirsiniz.

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

Bazı iş ortakları, etkin bir **şekilde** kendi Azure kaynaklarını yönetmek ve sağlamak isteyen müşterilere Sahip rolünü zaten atamış olabilir. Önceden satın aldığınız **abonelikleri** yönetmek için bir müşteriye Sahip durumu atadıysanız bu adımı atlayabilirsiniz.  

> [!IMPORTANT]
> Bir müşteriye Sahip rolü **atanmaması,** müşterinin Azure rezervasyonları satın Azure portal önleyen bir hata alır.

Müşteriye Bir Azure aboneliği için Sahip **rolü** atandığı doğrulamak için:

1. İş Ortağı Merkezi [oturum açın.](https://partner.microsoft.com/dashboard)

2. **CSP'yi** ve ardından **Müşteriler'i** ve belirli bir müşteriyi seçin.

3. Bu **müşteri** için Abonelikler'i seçin ve ilgili Azure aboneliğini bulun.

4. Müşterinin **aboneliğinin** yanındaki Yönet düğmesini seçin. Bunu yapmak, [Azure portal.](https://portal.azure.com/)

5. Sahip rolünü **belirli bir** kullanıcıya atamak için şu adımları [izleyin: Bir kullanıcıya yönetici olarak atamak için.](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator)

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>Kendi Azure rezervasyonlarını satın almak için müşteri izinlerini açma veya kapatma

Müşterinin mevcut bir Azure aboneliğine sahip olduğunu ve  kullanıcılara bu abonelik için Sahip rolü atandığı doğru olduktan sonra, müşteri izinlerini açma (etkinleştirme) için hazırsınız. Müşteri izinlerini kapatmak (devre dışı bırakmak) için de bu adımları kullanabilirsiniz. İş Ortağı Merkezi panosu veya api'leri kullanarak İş Ortağı Merkezi [devre dışı abilirsiniz.](/partner-center/develop/manage-customers)

Bu hizmette müşteri izinlerini açmak (veya kapatmak) İş Ortağı Merkezi:

1. İş Ortağı Merkezi [oturum açın.](https://partner.microsoft.com/dashboard)

2. Sol gezinti menüsünde **CSP'yi** ve ardından Müşteriler'i **seçin.** Bir müşteri listesi görüntülenir.

3. Belirli bir müşteri adı seçin.

4. Müşteri **menüsünden** Hesap'ı seçin. Müşteri **Hesabı** sayfası görüntülenir.

5. Sayfanın **en altındaki** Müşteri izinleri alanına gidin.

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="Hesap sayfasında müşteri izinleri." border="true":::

6. **Azure rezervasyonları** altında Müşterinin satın **almasına izin ver seçeneğini** bulun.

7. Müşteri izinlerini açmak için bu seçeneğin yanındaki anahtarı Açık **konuma** getirin. Müşteri izinlerini kapatmak için anahtarı Kapalı **konuma** getirin.

>[!NOTE]
> Bir müşterinin kendi Azure rezervasyonlarını satın alma izinlerini açarak başka ne olacağını öğrenmek için bkz. Azure'daki [müşteri izinlerine genel İş Ortağı Merkezi.](give-customers-permission.md#overview-of-customer-permissions-in-partner-center)
>
>Müşteri izinlerini aç (veya kapat) etkinlik günlüğü her eylemi günlüğe kaydeder. (Bu günlüğe panonun üst kısmından Dişli simgesini İş Ortağı Merkezi erişilebilir). Müşteri izinlerini aç veya kapat, eylem Etkinlik günlüğünde Müşteri **Satın** Alma İzinleri Oluştur veya **Müşteri** Satın Alma İzinlerini Sil olarak görünür.

## <a name="help-customers-manage-reservations-they-purchase"></a>Müşterilerin satın aldıkları rezervasyonları yönetmeye yardımcı olur

Müşterilere kendi Azure rezervasyonlarını satın alma izni verdiktan sonra, satın aldıkları tüm kaynakları daha iyi yönetmelerine yardımcı olabilirsiniz. Müşteriler, Azure rezervasyonlarının birçok farklı yönlerini doğrudan [Azure portal.](https://portal.azure.com/) CSP aboneliğiniz içinde satın aldıkları Azure rezervasyonlarının birkaç ve diğer yönlerini yönetmek için sizin yardıma ihtiyaçları olacaktır.  

Müşterilerin Azure rezervasyonlarının bu yönlerini yönetme hakkında daha fazla bilgi edinerek yardım edin:

- Müşterilerin Azure rezervasyonları için ödemesi yapılan fiyatlar
- Müşterilerin Azure rezervasyonlarının kullanımını iyileştirme
- Müşteriler paylaşılan bir kapsamla rezervasyon satın aldıklarında ne olur?
- Müşteriler bir rezervasyonu değiştirmek, iptal etmek ve yenilemek ya da kapsamını değiştirmek isterse ne olur?

**Müşterilerin rezervasyonları için ödeme yaptıkları fiyatlar.** Müşteriniz, CSP iş ortağı ödeme hesaplarında daha önce satın aldığınız bir aboneliğe göre Azure rezervasyonları satın alır. Bu aboneliğe göre satın aldıkları Tüm Azure rezervasyonları için müşterinin fiyatı da sizin tarafından ayarlanır. Bu fiyat, müşterinin web sitesinde gördüğü Web Direct fiyatından farklı Azure portal.

**Müşterilerin rezervasyon kullanımını nasıl en iyi duruma getirmeleri gerekir?** Bazı müşteriler, rezervasyon kullanımını iyileştirme veya satın alma sırasında rezervasyonun ilk kapsamını atama hakkında daha fazla bilgi elde etme avantajından yararlanabilir. Daha fazla bilgi için, müşterilerden Azure kaynakları [için rezervasyonları yönetme makalelerini okumalarını sorun.](/azure/cost-management-billing/reservations/manage-reserved-vm-instance)

**Bir müşteri, paylaşılan bir kapsama sahip bir rezervasyon satın aldığında ne olur?** Müşteriler önceki bir CSP aboneliğine göre bir ayırma satın alıp bu ayırmaya bir paylaşılan kapsam atadıktan sonra, müşterinin CSP tarafından verilen tüm indirimler, CSP iş ortağı tarafından satın alınan tüm abonelikler için eşleşen kullanım için geçerlidir.

**Müşteriler, yapmış oldukları bir satın alma, iptal etme veya yenileme ya da bir ayırmanın başlangıç kapsamını değiştirme amacıyla ne yapması gerekir?** Müşterilerin, bir ayırmanın ilk kapsamını değiştirmesine yardımcı olması için iş ortağlarına sormaları gerekir. Ayrıca, bir ayırmayı Exchange, iptal etme veya yenileme için bir iş ortağının yardımına de ihtiyacı vardır. Bu görevleri, kendilerine bir CSP iş ortağı tarafından satın alınan abonelikler temelinde rezervasyon ile gerçekleştiremez.

## <a name="next-steps"></a>Sonraki adımlar

- [Müşterileriniz adına Azure ayırmaları satın alın](azure-reservations-buying.md)

- [İş Ortağı Merkezi-Microsoft ayırmaları satma](azure-reservations.md)

- [Azure rezervasyonlarını müşterileriniz adına yönetme](azure-reservations-manage.md)