---
title: Azure aboneliğini bir Azure planına göre başka bir CSP ortağına aktarma
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: bir azure planı kapsamındaki müşterinin azure abonelikleriyle ilişkili Bulut Çözümü Sağlayıcısı program ortağını nasıl değiştireceğinizi öğrenin.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/21/2021
ms.openlocfilehash: 258b593935e9fd599e0f5c524cd7ec935c50bcad
ms.sourcegitcommit: d133c8b923b90ac5518cb989c0ce4dd69713abf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/22/2021
ms.locfileid: "114434141"
---
# <a name="transfer-a-customers-azure-subscriptions-to-a-different-partner-in-csp-under-an-azure-plan"></a>Müşterinin Azure aboneliklerini CSP 'de farklı bir ortağa aktarma (bir Azure planı altında)

**Uygun roller**: Hesap Yöneticisi | Satış Aracısı | Faturalandırma Aracısı

bu makalede, bir müşterinin azure aboneliklerini Bulut Çözümü Sağlayıcısı (CSP) içindeki bir iş ortağından bir azure planı altında diğerine nasıl geçbir bir şekilde (bir müşterinin) nasıl bir bir

Müşterinin Azure aboneliklerini farklı bir iş ortağından geçirmek için aşağıdaki adımları izleyin. Hem iş ortağının hem de müşterinin tamamlanma adımları vardır.

> [!Note]  
> Yalnızca Microsoft ile doğrudan faturalandırma ilişkisine sahip iş ortakları geçiş araçlarına erişebilir. Bu geçiş aracından yararlanmak için dolaylı satıcıların dolaylı sağlayıcılarıyla birlikte çalışması gerekir.

Müşteri, bu araç yararlanılabilir önceki iş ortakları (geçerli ve gelecekteki) ile birlikte konuşmada olmalıdır. Karışıklık ve karmaşıklığın oluşmaması için çevrimdışı bir konuşma olması gerekir. Ayrıca, iş ortakları ve müşteriler bir geçişi başlatmadan önce bu konuları ve önkoşulları anlamalıdır:

**Önemli noktalar:**

- Azure ayırmaları gelecek iş ortağına abonelikle birlikte taşınmayacak
- Geçerli iş ortağı kapsamındaki Azure hizmetleri için CSP fiyatlandırması geçiş olmayacak
- [Önceki Azure teklifini aktarma (MS-AZR-0145p)](https://go.microsoft.com/fwlink/p/?linkid=2164140) abonelikleri, bu Azure aboneliklerinin aynı anda bir Azure planı Içindeki yeni Azure teklifi aboneliklerine dönüştürülmesine neden olur
- Müşteri için destek sorumlulukları gelecek iş ortağına taşınır
- Faturalandırma ve faturalama, aktarım sırasında gelecek iş ortağına taşınır
- Azure Role-Based Access Control (RBAC) aktarımdan etkilenmiyor
- (AOBO) adına yönetici, gelecek iş ortağı için varsayılan olarak verilmeyecektir
- Ürünler Market uygunluk denetimini geçirmiş olduğu sürece, üçüncü taraf Market ürünleri aktarılır.
    - Özel indirimler veya bölgesel kısıtlama yoktur
    - Ürünler, abonelik olmayan tabanlı
    - Gelecekteki iş ortağı, ürün dağıtımı için izin üzerinde olduklarından emin olmak için Yayımcısıyla birlikte çalışmalıdır
    - Market ürünlerinin aktarılması için bu koşulların tümü karşılanmazsa, Azure abonelikleri aktarılmalı ve yeni iş ortağıyla Market ürünlerinin yeniden oluşturulması gerekir

**Ön koşullar:**

- Müşteri, geçerli CSP iş ortaklarının geçiş amacını karşılamalarını sağlar
- Gelecekteki CSP iş ortağı müşteri gereksinimlerinin karşılanabileceği sağlamak için müşteriyle birlikte çalışarak
- Gelecekteki CSP iş ortağı, müşteri ile bir ilişki kurar ve geçiş başlamadan önce bir Azure planı satın alır  
- Müşteri, gelecek CSP ortağıyla Microsoft Müşteri anlaşmasını imzalayamalıdır
- Gelecekteki CSP iş ortağı bu aracı kullanmak için Microsoft Iş ortağı sözleşmesi 'Ni imzalamalıdır

> [!NOTE]
> Bu self servis aracı, müşterinin geçerli iş ortağı önceki Azure teklifi (MS-AZR-0145p) ya da yeni Azure teklifi (Azure planı) olduğunda kullanılabilir. Bu aktarımın her iki durumda da tamamlanması, gelecek iş ortağıyla bir Azure planı kapsamındaki Azure aboneliklerine neden olur.

## <a name="customer-tasks-to-be-completed"></a>Tamamlanacak müşteri görevleri

Azure aboneliklerini aktarmak için müşterinin geçerli iş ortağıyla iletişim kurarak süreci başlatması gerekir. Gelecekteki iş ortaklarının kendi adına aktarım isteği formunu tamamlayabilmeleri için, geçerli iş ortağının şirket adını ve Microsoft KIMLIĞINI toplamaları gerekir.

Müşterinin ayrıca geçerli iş ortağından aktarmak istedikleri abonelikleri tanımlaması gerekir. Office 365, Enterprise Mobility Suite veya Microsoft Dynamics CRM abonelikleri için iş ortaklarını değiştiremezsiniz.

> [!NOTE]  
> Aktarım sürecini başlatan aktarım isteği formunu tamamlamaya yönelik gelecek iş ortağının sorumluluğundadır. Microsoft, müşteri veya geçerli iş ortağı adına müdahale edemez. Müşteri, geçişi sorunsuz bir şekilde hareket etmek için gelecekteki ve geçerli ortağıyla yakından çalışmayı planlıyor olmalıdır.

## <a name="future-partner-tasks-to-be-completed"></a>Tamamlanacak sonraki iş ortağı görevleri

Aboneliğin gelecek iş ortağının, abonelik aktarımı istemek için Iş Ortağı Merkezi 'nden bir aktarım isteği formunu tamamlaması gerekir:

1.  Iş Ortağı Merkezi menüsünde, **müşteriler**' i seçin ve ardından bir aktarım isteği formunu gerçekleştirmek istediğiniz müşteriyi seçin.
2.  Müşteri menüsünden **abonelikler**' i seçin.
3.  **Aktarım isteği** bölümünü seçin.
4.  **Aktarım isteği bölümünden** **yeni istek ekle**' yi seçin.

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Aktarımlar bölümü.":::

5.  **Yeni aktarım isteği** formunu doldurun.

6.  **Gönderme aktarım isteği** Gönder ' i seçin  >  .

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Aktarım isteği formunu doldurun.":::

7.  Aktarım isteği onayını gözden geçirme

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Bekleyen aktarımı gözden geçirin.":::

    > [!NOTE]
    > Gelecekteki iş ortağı, yalnızca aktarım isteği durumu "bekliyor" olduğunda sağ üst köşede bulunan **isteği iptal** et ' i seçerek aktarım isteğini iptal edebilir. Aktarım isteği durumu "sürüyor" veya "Tamam" olduktan sonra, iptaller mümkün olmayacaktır.

## <a name="current-partner-tasks-to-be-completed"></a>Tamamlanacak geçerli iş ortağı görevleri

Geçerli iş ortağının müşterinin Yönetim Aracısı, müşterilerinin aboneliklerinin aktarımını istediğini belirten bir e-posta alır:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="İncelemeyi.":::

Abonelik aktarımını gerçekleştirmek için Iş Ortağı Merkezi 'nden aktarma isteği formunu gözden geçirin ve kabul edin.

> [!NOTE]  
> Geçerli iş ortağı tarafından 30 gün içinde herhangi bir eylem yapılmaz, isteğin süresi sona erer ve gelecekteki iş ortağı yeni bir aktarım isteği oluşturmak için bir öğesine sahip olur.

- E-postadaki **Aktarım Isteğini gözden geçir** ' i seçin

   -veya-

1. Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve ardından bir aktarım isteğinin adına gönderildiği müşteriyi seçin.
2. Müşteri menüsünden **abonelikler**' i seçin.
3. **Aktarım isteği** bölümünü seçin.
4. **alınan istekler** altında seçilen **aktarım isteği kimliğini** seçerek aktarım bilgilerini genişletin

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Kaynak, aktarım isteğini gözden geçirir.":::

5. Aktarım isteğini gözden geçirin. Aktarılacak istenen Azure aboneliklerini seçin.
 
Devam etmeden önce lütfen unutmayın:
- Artık seçili aboneliklere erişemeyecektir.
- Daha fazla kullanım için faturalandırlanmayacaktır.
- Azure ayırmaları, aboneliklerle aktarılmaz.

6. Ardından, aktarma işlemini gerçekleştirmek için **kabul et ve Aktar '** ı seçin.

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Azure planlarınız altında aktarılacak abonelikleri seçin.":::

Geçerli iş ortağının önceki Azure teklif abonelikleri (MS-AZR-0145p) içeren bir müşterisi varsa, aktarım işlemini tamamlamaya yönelik abonelikler ' i seçip kabul et ve Aktar ' ı seçerek aynı şekilde devam edecektir.

7. Aktarım kabulü onayını görüntüleyin.

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
