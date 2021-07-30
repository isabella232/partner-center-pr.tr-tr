---
title: Azure aboneliğini bir Azure planına göre başka bir CSP ortağına aktarma
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: bir azure planı kapsamındaki müşterinin azure abonelikleriyle ilişkili Bulut Çözümü Sağlayıcısı program ortağını nasıl değiştireceğinizi öğrenin.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/21/2021
ms.openlocfilehash: 14f03a8eb899f7224a38b0f998edd72077b34b3b
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114844284"
---
# <a name="transfer-a-customers-azure-subscriptions-to-a-different-csp-under-an-azure-plan"></a>Müşterinin Azure aboneliklerini farklı bir CSP 'ye aktarma (bir Azure planı altında)

**Uygun roller**: Hesap Yöneticisi | Satış Aracısı | Faturalandırma Aracısı

bu makalede, müşterilerin azure aboneliklerini bir azure planı altında Bulut Çözümü Sağlayıcısı (CSP) programındaki bir iş ortağından diğerine nasıl değiştirebilmeleri açıklanmaktadır.

Müşterinin Azure aboneliklerini farklı bir iş ortağından geçirmek için aşağıdaki adımları izleyin. Geçerli iş ortağı, gelecek iş ortağı ve müşterinin tümünün tamamlaması gereken adımları vardır.

> [!Note]  
> Yalnızca Microsoft ile doğrudan faturalandırma ilişkisine sahip iş ortakları Geçiş aracına erişebilir. Dolaylı satıcıların bu geçiş aracını kullanması için dolaylı sağlayıcılarıyla çalışması gerekir.

Geçiş aracının kullanılabilmesi için müşterinin hem geçerli hem de gelecekteki iş ortağıyla iletişim kurması gerekir. Karışıklık ve karmaşıklığın önüne geçmek için çevrimdışı bir konuşma oluşması gerekir. İş ortakları ve müşteriler bir geçişe başlamadan önce aşağıdaki önemli noktaları ve önkoşulları anlamalıdır.

## <a name="considerations"></a>Dikkat edilmesi gerekenler

- Azure ayırmaları gelecek iş ortağına bir abonelikle birlikte taşınmayacaktır.
- Geçerli iş ortağı kapsamındaki Azure hizmetleri için CSP fiyatlandırması geçmez.
- [Önceki Azure teklifi (MS-azr-0145p)](https://go.microsoft.com/fwlink/p/?linkid=2164140) aboneliklerini aktarırsanız, bu Azure abonelikleri eşzamanlı olarak bir Azure planı Içindeki yeni Azure teklifi aboneliklerine dönüştürülür.
- Müşteri için destek sorumlulukları gelecek iş ortağına taşınır.
- Faturalandırma ve faturalama, abonelik aktarılırken gelecek iş ortağına taşınır.
- Azure rol tabanlı erişim denetimi (RBAC) aktarımlardan etkilenmez.
- (AOBO) adına yönetici, gelecek iş ortağı tarafından varsayılan olarak verilmez.
- Ürünler Azure Market uygunluk denetimini geçirmiş olduğu sürece, üçüncü taraf Azure Marketi ürünleri aktarılır.
    - Özel indirim veya bölgesel kısıtlama yoktur.
    - Ürünler, abonelik olmayan tabanlıdır.
    - Gelecekteki iş ortağı, yayımcının ürünün dağıtımına yönelik izin üzerinde olduğundan emin olmak için Yayımcısıyla birlikte çalışmalıdır.
    - Bu koşullardan herhangi biri karşılanmazsa, Azure Marketi ürünlerinin iptal edilmesi gerekir. Ardından, Azure abonelikleri aktarılmalıdır ve Azure Market ürünleri yeni iş ortağıyla satın alınmalıdır.

## <a name="prerequisites"></a>Önkoşullar

- Müşteri, geçerli CSP iş ortağının geçiş hedefini bilgilendirir.
- Gelecekteki CSP iş ortağı müşteriyle birlikte çalışarak müşteri gereksinimlerinin karşılanabileceği güvence altına alınabilir.
- Gelecek CSP iş ortağı, müşteriyle bir ilişki kurar ve geçiş başlamadan önce bir Azure planı satın alır.
- Müşteri, gelecek CSP ortağıyla bir Microsoft Müşteri Sözleşmesi imzalar.
- Gelecek CSP iş ortağı, geçiş aracını kullanmadan önce Microsoft Iş ortağı sözleşmesi 'Ni imzalar.

> [!NOTE]
> Self Servis geçiş aracı, müşterinin geçerli iş ortağı önceki Azure teklifi (MS-AZR-0145p) ya da yeni Azure teklifi (Azure planı) olduğunda kullanılabilir. Her iki durumda da, Aktarım tamamlandığında Azure abonelikleri gelecek iş ortağıyla bir Azure planı altında olacaktır.

## <a name="customer-tasks"></a>Müşteri görevleri

Azure aboneliklerini aktarmak için, müşterinin geçerli iş ortağıyla iletişim kurarak süreci başlatması gerekir. Müşteri, gelecek iş ortağının müşteri adına aktarım isteği formunu tamamlayabilmesi için geçerli ortağın şirket adını ve Microsoft KIMLIĞINI toplamalıdır.

Müşteriler, geçerli iş ortağından aktarmak istedikleri abonelikleri de tanımlamalıdır. Office 365, Enterprise Mobility Suite veya Microsoft Dynamics CRM abonelikleri için iş ortaklarını değiştiremezsiniz.

> [!NOTE]  
> Bu, aktarım sürecini başlatan aktarım isteği formunu tamamlamaya yönelik gelecek iş ortağının sorumluluğundadır. Microsoft, müşteri veya geçerli iş ortağı adına müdahale edemiyor. Müşteri, geçişin sorunsuz bir şekilde çalışmasını sağlamak için gelecek ve geçerli iş ortaklarıyla yakından çalışmayı planlıyor olmalıdır.

## <a name="future-partner-tasks"></a>Gelecekteki iş ortağı görevleri 

Aboneliğin gelecek iş ortağının, abonelik aktarımı istemek için Iş Ortağı Merkezi 'nden bir aktarım isteği formunu tamamlaması gerekir:

1.  Iş Ortağı Merkezi 'nin sol bölmesinde **müşteriler**' i seçin ve ardından aktarım isteğini gerçekleştirmek istediğiniz müşteriyi seçin.
2.  Müşteriye özgü menüsünde **abonelikler**' i seçin.
3.  **Aktarım istekleri** sekmesinde **yeni istek ekle**' yi seçin:

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Aktarım istekleri sekmesini gösteren ekran görüntüsü.":::

5.  **Yeni aktarım isteği** formunu doldurun:

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Yeni aktarım isteği formunu gösteren ekran görüntüsü.":::

6.  **Gönderme aktarım isteği** Gönder ' i seçin  >  .

7.  Aktarım isteği onayını gözden geçirin:

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Aktarım isteği onayını gösteren ekran görüntüsü.":::

    > [!NOTE]
    > Gelecekteki iş ortağı, yalnızca aktarım isteği durumu "bekliyor" olduğunda pencerenin sağ üst köşesinde bulunan **Isteği iptal** et ' i seçerek aktarım isteğini iptal edebilir. Aktarım isteği durumu "sürüyor" veya "Tamam" olduktan sonra, iptaller mümkün değildir.

## <a name="current-partner-tasks"></a>Geçerli iş ortağı görevleri 

Geçerli iş ortağının müşteri için Yönetim Aracısı, bir müşterinin aboneliklerin aktarımını istediğini bildiren bir e-posta alır:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Aktarım için bir müşteri isteğinin e-posta bildirimini gösteren ekran görüntüsü.":::

Geçerli iş ortağının, abonelik aktarımını tamamlaması için Iş Ortağı Merkezi 'nden aktarım isteği formunu gözden geçirmesi ve kabul etmesi gerekir.

> [!NOTE]  
> Geçerli iş ortağı 30 gün içinde yanıt vermezse, isteğin süresi sona erer ve gelecek iş ortağının yeni bir aktarım isteği oluşturması gerekir.

1. Aşağıdaki eylemlerden birini uygulayın: 
   - E-postadaki **Aktarım Isteğini gözden geçir** ' i seçin.

     veya

    - Iş Ortağı Merkezi 'nin sol bölmesinde **müşteriler**' i seçin ve ardından aktarım isteğinin gönderildiği müşteriyi seçin.
      1. Müşteriye özgü menüsünde **abonelikler**' i seçin.
      1. **Aktarım istekleri** sekmesinde, **alınan istekler** altındaki **aktarım isteği kimliğini** seçerek aktarım bilgilerini genişletin:

      :::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Geçerli iş ortağı tarafından görüldüğü gibi aktarım istekleri sekmesini gösteren ekran görüntüsü.":::

5. Aktarım isteğini gözden geçirin. Aktarılacak istenen Azure aboneliklerini seçin.
 
   Devam etmeden önce, şunu göz önüne alın:
   - Artık seçili aboneliklere erişebileceksiniz.
   - Daha fazla kullanım için faturalandırılmayan.
   - Azure ayırmaları aboneliklerle aktarılmaz.

6. Aktarım işlemini gerçekleştirmek için **kabul et ve Aktar ' ı** seçin:

   :::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Aktarım isteği gözden geçirme ekranını gösteren ekran görüntüsü.":::

   Önceki Azure teklifi aboneliklerine (MS-AZR-0145p) sahip bir müşteriniz varsa aynı şekilde devam edin, aktarılacak abonelikleri seçin ve ardından **kabul et ve aktar** ' ı seçerek aktarım sürecini doldurun.

7. Aktarım kabulü onayını görüntüleyin.

   Bu noktada, bir e-posta, kabul edilen aktarım isteğiyle ilgili gelecek iş ortağı, müşteri ve geçerli iş ortağı hakkında bilgilendirir.

   Geçiş kabul edildikten sonra, sistem güncelleştirilirken aktarım durumu 15 dakikaya kadar "bekliyor" olarak kalabilir. Bu işlem daha uzun sürerse, sistem üç gün boyunca çalışmaya devam eder. Aktarım durumu, üç günden uzun bir süre boyunca "bekliyor" durumunda kalırsa, iş ortağı bir hizmet isteği göndermesi gerekir.

   Aktarım tamamlandıktan sonra, istekte yer alan abonelikler gelecek iş ortağının Azure planında görüntülenir. Artık geçerli iş ortağı ile listelenmeyecektir.

>[!Note]  
>Dolaylı sağlayıcılar, dolaylı satıcılarını aktarım isteğinin kabul edildiğini bilgilendirmelidir.

### <a name="managing-your-transferred-customer-subscriptions"></a>Aktarılan müşteri aboneliklerinizi yönetme

Azure RBAC aracılığıyla atanan mevcut kullanıcılara, gruplara veya hizmet ilkelerine erişim, geçiş sırasında etkilenmez. [Azure RBAC](/azure/role-based-access-control/overview) , müşterinizin Azure kaynaklarına erişimi olan kişileri, bu kaynaklarla neler yapabileceğini ve hangi alanlara erişebileceğini yönetmesine yardımcı olur. 

Yeni bir iş ortağı olarak, abonelik aktarımından sonra müşterinizin kaynaklarına hiçbir RBAC erişimi olmayacaktır. Müşterinizin önceki iş ortağı RBAC erişimini korur. Aboneliklerle ilgili bir anlayış olduğunu ve gerekli değişiklikleri nasıl yapacağınızı anlamak için müşterinizden çalışın.

Müşterinizin, önceki iş ortağı için Azure RBAC erişimini kaldırması ve sizin için erişim eklemesi gerekir. Erişim sağlama hakkında daha fazla bilgi için bkz. [Azure rol tabanlı erişim denetimi (Azure RBAC) nedir?](/azure/role-based-access-control/overview). Erişimi kaldırma hakkında daha fazla bilgi için bkz. [rol atamasını kaldırma](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).

Ayrıca, aboneliklerinize otomatik olarak [yönetici (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) erişimi de kalmaz. Müşterinizin Azure aboneliklerini yönetebilmeniz için AOIMIZ gereklidir. Azure ayrıcalıkları hakkında daha fazla bilgi için bkz. [Müşterinin hizmetini veya aboneliğini yönetme izinleri alma](./customers-revoke-admin-privileges.md).

## <a name="next-steps"></a>Sonraki adımlar

- [Azure RBAC](/azure/role-based-access-control/overview)
- [Müşterinin hizmetini veya aboneliğini yönetme izinleri alma](./customers-revoke-admin-privileges.md)
