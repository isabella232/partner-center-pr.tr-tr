---
title: Azure aboneliğini bir Azure planına göre başka bir CSP ortağına aktarma
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Bir Azure planı kapsamındaki müşterinin Azure abonelikleriyle ilişkili bulut çözümü sağlayıcısı program ortağını nasıl değiştireceğinizi öğrenin.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: 4213658fc131d83d6c0640552d862f4de9b5ad86
ms.sourcegitcommit: e10d2a19dea7e317d227d7fbdcf1bbc3dc4f6257
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/13/2020
ms.locfileid: "92531842"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a>Müşterinin Azure planı aboneliklerini farklı bir ortağa aktarma

## <a name="applies-to"></a>Şunlara uygulanır

- Bulut çözümü sağlayıcısı (CSP) programındaki iş ortakları

Bu makalede, bir müşterinin Azure planına ait Azure aboneliklerinin bir bulut çözümü sağlayıcısından (CSP) diğerine nasıl geçbir şekilde değiştirileceği açıklanır.

Müşterinin Azure aboneliklerini farklı bir iş ortağından geçirmek için aşağıdaki adımları izleyin. Hem iş ortağının hem de müşterinin tamamlanma adımları vardır.

>[!Note]  
>Yalnızca Microsoft ile doğrudan faturalandırma ilişkisine sahip iş ortakları geçiş araçlarına erişebilir. Bu geçiş aracından yararlanmak için dolaylı satıcıların dolaylı sağlayıcılarıyla birlikte çalışması gerekir.

Müşteri, bu araç yararlanılabilir önceki iş ortakları (geçerli ve gelecekteki) ile birlikte konuşmada olmalıdır. Karışıklık ve karmaşıklığın oluşmaması için çevrimdışı bir konuşma olması gerekir. Ayrıca, iş ortakları ve müşteriler bir geçişi başlatmadan önce bu konuları ve önkoşulları anlamalıdır:

**Önemli noktalar:**

- Azure ayırmaları gelecek iş ortağına abonelikle birlikte taşınmayacak
- Geçerli iş ortağı kapsamındaki Azure hizmetleri için CSP fiyatlandırması geçiş olmayacak  
- Müşteri için destek sorumlulukları gelecek iş ortağına taşınır
- Faturalandırma ve faturalama, aktarım sırasında gelecek iş ortağına taşınır
- Azure Role-Based Access Control (RBAC) aktarımdan etkilenmiyor
- (AOBO) adına yönetici, gelecek iş ortağı için varsayılan olarak verilmeyecektir
- Ürünler Market uygunluk denetimini geçirmiş olduğu sürece, üçüncü taraf Market ürünleri aktarılır.
    - Özel indirimler veya bölgesel kısıtlama yoktur
    - Ürünler, abonelik olmayan tabanlı
    - Gelecekteki iş ortağı, ürün dağıtımı için izin verilenler listesinde olduklarından emin olmak için Yayımcısıyla birlikte çalışmalıdır
    - Market ürünlerinin aktarılması için bu koşulların tümü karşılanmazsa, Azure abonelikleri aktarılmalı ve yeni iş ortağıyla Market ürünlerinin yeniden oluşturulması gerekir

**Ön koşullar:**

- Müşteri, geçerli CSP iş ortaklarının geçiş amacını karşılamalarını sağlar
- Gelecekteki CSP iş ortağı müşteri gereksinimlerinin karşılanabileceği sağlamak için müşteriyle birlikte çalışarak
- Gelecekteki CSP iş ortağı, geçiş başlamadan önce müşteri ile bir ilişki kurar  
- Müşteri, gelecek CSP ortağıyla Microsoft Müşteri anlaşmasını imzalayamalıdır
- Gelecekteki CSP iş ortağı bu aracı kullanmak için Microsoft Iş ortağı sözleşmesi 'Ni imzalamalıdır

## <a name="customer-tasks-to-be-completed"></a>Tamamlanacak müşteri görevleri

Bir Azure planı kapsamında bir Azure aboneliğini aktarmak için, müşterinin geçerli iş ortağıyla iletişim kurarak işlemi başlatması gerekir. Gelecekteki iş ortaklarının kendi adına aktarım isteği formunu tamamlayabilmeleri için, geçerli iş ortağının şirket adını ve etki alanını toplamaları gerekir.

Müşterinin ayrıca geçerli iş ortağından aktarmak istedikleri abonelikleri tanımlaması gerekir. Office 365, Enterprise Mobility Suite veya Microsoft Dynamics CRM abonelikleri için iş ortaklarını değiştiremezsiniz.

>[!Note]  
>Aktarım sürecini başlatan aktarım isteği formunu tamamlamaya yönelik gelecek iş ortağının sorumluluğundadır. Microsoft, müşteri veya geçerli iş ortağı adına müdahale edemez. Müşteri, geçişi sorunsuz bir şekilde hareket etmek için gelecekteki ve geçerli ortağıyla yakından çalışmayı planlıyor olmalıdır.

## <a name="future-partner-tasks-to-be-completed"></a>Tamamlanacak sonraki iş ortağı görevleri

Aboneliğin gelecek iş ortağının, abonelik aktarımı istemek için Iş Ortağı Merkezi 'nden bir aktarım isteği formunu tamamlaması gerekir:

1.  Iş Ortağı Merkezi menüsünde, **müşteriler** ' i seçin ve ardından bir aktarım isteği formunu gerçekleştirmek istediğiniz müşteriyi seçin.
2.  Müşteri menüsünden **abonelikler** ' i seçin.
3.  **Aktarım isteği** bölümünü seçin.
4.  **Aktarım isteği bölümünden** **yeni istek ekle** ' yi seçin.

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Aktarımlar bölümü":::

5.  **Yeni aktarım isteği** formunu doldurun.

6.  **Gönderme aktarım isteği** Gönder ' i seçin  >  **Send** .

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Aktarımlar bölümü":::

7.  Aktarım isteği onayını gözden geçirme

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Aktarımlar bölümü" olduktan sonra, iptaller mümkün olmayacaktır.

## <a name="current-partner-tasks-to-be-completed"></a>Tamamlanacak geçerli iş ortağı görevleri

Geçerli iş ortağının müşterinin Yönetim Aracısı, müşterilerinin aboneliklerinin aktarımını istediğini belirten bir e-posta alır:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Aktarımlar bölümü":::

Abonelik aktarımını gerçekleştirmek için Iş Ortağı Merkezi 'nden aktarma isteği formunu gözden geçirin ve kabul edin.

>[!Note]  
>Geçerli iş ortağı tarafından 30 gün içinde herhangi bir eylem yapılmaz, isteğin süresi sona erer ve gelecekteki iş ortağı yeni bir aktarım isteği oluşturmak için bir öğesine sahip olur.

1.  E-postadaki veya **Aktarım Isteğini gözden geçirin** ' i seçin
1.  Iş Ortağı Merkezi menüsünde **müşteriler** ' i seçin ve ardından bir aktarım isteğinin adına gönderildiği müşteriyi seçin.
2.  Müşteri menüsünden **abonelikler** ' i seçin.
3.  **Aktarım isteği** bölümünü seçin.
4.  **Alınan istekler** altında seçilen **aktarım isteği kimliğini** seçerek aktarım bilgilerini genişletin

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Aktarımlar bölümü":::

5.  Aktarım isteğini gözden geçirin. Aktarılacak istenen Azure aboneliklerini seçin.

>[!Note]  
> Devam etmeden önce lütfen unutmayın: seçili aboneliklere artık erişemeyecektir.
> Daha fazla kullanım için faturalandırlanmayacaktır.
> Azure ayırmaları, aboneliklerle aktarılmaz.

6.  Ardından, aktarma işlemini gerçekleştirmek için **kabul et ve Aktar '** ı seçin.

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Aktarımlar bölümü":::

7.  Aktarım kabulü onayını görüntüleyin.

   Bu noktada, gelecek iş ortağı, müşteri ve geçerli iş ortağı, kabul edilen aktarım isteği ile e-posta üzerinden bildirilir.

   Sonra, geçiş kabul edildikten sonra, sistem güncelleştirilirken aktarım durumu 15 dakikaya kadar beklemede kalabilir. Daha uzun sürerse, sistem üç gün boyunca çalışmaya devam eder. Aktarım durumu hala beklemede kalırsa, iş ortağı bir hizmet isteği göndermesi gerekir.

   Aktarım işlemi tamamlandıktan sonra, istek içine dahil edilen abonelikler gelecek iş ortağının Azure planında görüntülenir ve artık sizinle listelenmez.

>[!Note]  
>Dolaylı sağlayıcılar için: lütfen dolaylı satıcınızla aktarım isteğinin kabul edildiğini bildirin.

### <a name="managing-your-transferred-customer-subscriptions"></a>Aktarılan müşteri aboneliklerinizi yönetme
- Bu geçiş, Azure rol tabanlı erişim denetimi (RBAC) kullanılarak atanan mevcut kullanıcı, grup ve hizmet sorumlularını etkilemez. Azure rol tabanlı erişim denetimi [(Azure RBAC)](/azure/role-based-access-control/overview) , müşterinizin Azure kaynaklarına erişimi olan kişileri, bu kaynaklarla neler yapabileceğini ve hangi alanlara erişebileceğini yönetmesine yardımcı olur. Yeni iş ortağı olarak, abonelik aktarımından sonra müşterinizin kaynaklarına herhangi bir RBAC erişimi verilmemiş. Müşterinizin önceki iş ortağı RBAC erişimini korur. Abonelikleriyle ilgili bir anlayış olduğunu ve istediğiniz değişiklikleri nasıl yapacağınızı anlamak için müşterinizden çalışın.

- Sonuç olarak, müşterinizin Azure RBAC erişimini önceki iş ortakları için kaldırmasının yanı sıra yeni iş ortağı için de erişim eklemesi önemlidir. Müşteriniz hakkında yeni erişim verme hakkında daha fazla bilgi için bkz. [Azure rol tabanlı erişim denetimi (Azure RBAC) nedir?](/azure/role-based-access-control/overview) Önceki iş ortağınızın RBAC erişimini kaldırma müşteriniz hakkında daha fazla bilgi için bkz. [rol atamasını kaldırma](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).

- Ayrıca, aboneliklerinize otomatik olarak [yönetici (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) erişimi de kalmaz. AOININ, iş ortağının müşterilerinin Azure aboneliklerini kendi adına yönetmesi gerekir. Azure ayrıcalıkları hakkında daha fazla bilgi için bkz [. bir müşterinin hizmetini veya aboneliğini yönetmek için Izinleri alma.](./customers-revoke-admin-privileges.md)

## <a name="next-steps"></a>Sonraki adımlar:

- [(Azure RBAC)](/azure/role-based-access-control/overview)
- [Müşterinin hizmetini veya aboneliğini yönetme izinleri alın.](./customers-revoke-admin-privileges.md)