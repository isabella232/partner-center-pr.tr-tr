---
title: Azure planı altındaki Azure aboneliğini başka bir CSP iş ortağına aktarma
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Müşterinin Azure abonelikleriyle ilişkili Bulut Çözümü Sağlayıcısı program iş ortağını azure planı kapsamında değiştirme hakkında bilgi edinin.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: dcacc6da51fe40c7eb05997f5409ef5fadbcf693
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856058"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a>Müşterinin Azure planı aboneliklerini farklı bir iş ortağına aktarma

**Uygun roller:** Hesap yöneticisi | Satış aracısı | Faturalama aracısı

Bu makalede bir müşterinin azure planı kapsamındaki Azure aboneliklerini bir abonelikten (CSP) Bulut Çözümü Sağlayıcısı nasıl değiştirip başka bir azure aboneliğine geçebilirsiniz?

Farklı bir iş ortağından müşterinin Azure aboneliklerini değiştirmek için aşağıdaki adımları izleyin. Hem iş ortağının hem de müşterinin tamamlaması gereken adımları var.

>[!Note]  
>Geçiş aracına yalnızca Microsoft ile doğrudan faturalama ilişkisi olan iş ortakları erişebilirsiniz. Dolaylı Kurumsal Bayilerin bu geçiş aracından yararlanılması için Dolaylı Sağlayıcılarıyla birlikte çalışması gerekir.

Bu araç kullanılana kadar müşterinin her iki iş ortağıyla (güncel ve gelecek) konuşmada olması gerekir. Karışıklığı ve karışıklığı önlemek için çevrimdışı bir konuşma yapılması gerekir. Ayrıca, iş ortakları ve müşteriler bir geçişi başlatan önce bu konuları ve önkoşulları anlamalı:

**Dikkat edilmesi gereken önemli noktalar:**

- Azure Rezervasyonları abonelikle birlikte gelecekteki iş ortağına taşınmayacak
- Geçerli iş ortağı altındaki Azure hizmetleri için CSP fiyatlandırması geçiş olmaz  
- Müşteri için destek sorumlulukları gelecekteki iş ortağına taşınacak
- Faturalama, aktarım zamanında gelecekteki iş ortağına taşınacak
- Azure Role-Based Access Control (RBAC) aktarımdan etkilenmez
- Yönetici Adına (AOBO) varsayılan olarak gelecekteki iş ortağına verilmez
- Üçüncü taraf market ürünleri, ürünler Market uygunluk denetimine geçeceği sürece aktaracak.
    - Özel indirimler veya bölgesel kısıtlamalar yoktur
    - Ürünler abonelik tabanlı değil
    - Gelecekteki iş ortağı, ürünün dağıtımına izin verme listesinde olduğundan emin olmak için yayımcıyla birlikte çalışmalı
    - Market ürünlerinin aktarımı için bu koşulların hepsi karşılanmazsa, Azure abonelikleri aktarıldı ve ardından Market ürünlerini yeni iş ortağıyla yeniden satın alma

**Ön koşullar:**

- Müşteri, geçiş amacına bağlı olarak mevcut CSP iş ortağıyla etkileşime geç
- Gelecekteki CSP iş ortağı müşteriyle birlikte çalışır ve müşteri ihtiyaçlarının karşılanamaması için
- Gelecekteki CSP iş ortağı müşteriyle bir ilişki kuracak ve geçiş başlamadan önce bir Azure planı satın alır  
- Müşterinin gelecekteki CSP Microsoft Müşteri Sözleşmesi oturum açması gerekir
- Gelecekteki CSP iş ortağının bu aracı Microsoft İş Ortağı Sözleşmesi için iş ortağını imzalamış olması gerekir

## <a name="customer-tasks-to-be-completed"></a>Tamamlanması gereken müşteri görevleri

Azure planı kapsamındaki bir Azure aboneliğini aktarması için müşterinin geçerli iş ortağıyla iletişime geçerek süreci başlatması gerekir. Gelecekteki iş ortaklarının kendi adına aktarım isteği formunu tamamlayamaları için geçerli iş ortağının şirket adını ve etki alanını toplaması gerekir.

Müşterinin ayrıca geçerli iş ortağından aktarma yapmak istediğiniz abonelikleri tanımlaması gerekir. Office 365, Enterprise Mobility Suite veya Microsoft Dynamics CRM abonelikleri için iş ortaklarını değiştiremezsiniz.

>[!Note]  
>Aktarım işlemini başlatan aktarım isteği formunu tamamlamak gelecekteki iş ortağının sorumluluğundadır. Microsoft müşteri veya geçerli iş ortağı adına müdahalede bulunamaz. Müşterinin, geçişi sorunsuz bir şekilde devam etmek için gelecekteki ve mevcut iş ortağıyla yakın bir çalışma planlaması gerekir.

## <a name="future-partner-tasks-to-be-completed"></a>Gelecekteki iş ortağı görevleri tamamlanacak

Aboneliğin gelecekteki iş ortağının abonelik aktarımı isteği için İş Ortağı Merkezi aktarım isteği formunu tamamlaması gerekir:

1.  Bu İş Ortağı Merkezi **Müşteriler'i** seçin ve ardından adına bir aktarım isteği formunu tamamlamak istediğiniz müşteriyi seçin.
2.  Müşteri menüsünden **abonelikler**' i seçin.
3.  **Aktarım isteği** bölümünü seçin.
4.  **Aktarım isteği bölümünden** **yeni istek ekle**' yi seçin.

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Aktarımlar bölümü":::

5.  **Yeni aktarım isteği** formunu doldurun.

6.  **Gönderme aktarım isteği** Gönder ' i seçin  >  .

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Aktarım isteği formunu doldurun":::

7.  Aktarım isteği onayını gözden geçirme

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Bekleyen aktarımı gözden geçirme":::

    >[!Note]
    >Gelecekteki iş ortağı, yalnızca aktarım isteği durumu "bekliyor" olduğunda sağ üst köşede bulunan **isteği iptal** et ' i seçerek aktarım isteğini iptal edebilir. Aktarım isteği durumu "sürüyor" veya "Tamam" olduktan sonra, iptaller mümkün olmayacaktır.

## <a name="current-partner-tasks-to-be-completed"></a>Tamamlanacak geçerli iş ortağı görevleri

Geçerli iş ortağının müşterinin Yönetim Aracısı, müşterilerinin aboneliklerinin aktarımını istediğini belirten bir e-posta alır:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Gözden geçirme":::

Abonelik aktarımını gerçekleştirmek için Iş Ortağı Merkezi 'nden aktarma isteği formunu gözden geçirin ve kabul edin.

>[!Note]  
>Geçerli iş ortağı tarafından 30 gün içinde herhangi bir eylem yapılmaz, isteğin süresi sona erer ve gelecekteki iş ortağı yeni bir aktarım isteği oluşturmak için bir öğesine sahip olur.

1.  E-postadaki veya **Aktarım Isteğini gözden geçirin** ' i seçin
1.  Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve ardından bir aktarım isteğinin adına gönderildiği müşteriyi seçin.
2.  Müşteri menüsünden **abonelikler**' i seçin.
3.  **Aktarım isteği** bölümünü seçin.
4.  **Alınan istekler** altında seçilen **aktarım isteği kimliğini** seçerek aktarım bilgilerini genişletin

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Kaynak incelemeleri aktarım isteği":::

5.  Aktarım isteğini gözden geçirme. Aktarımın istenen Azure aboneliklerini seçin.

>[!Note]  
> Devam etmeden önce lütfen unutmayın: Artık seçili aboneliklere erişemeyeceksiniz.
> Daha fazla kullanım için faturalanmaz.
> Azure rezervasyonları aboneliklerle birlikte aktarlanmaz.

6.  Ardından, **aktarım işlemini tamamlamak için Kabul** et ve aktar'ı seçin.

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Azure planlarınızı kullanarak aktarıla abonelikleri seçin":::

7.  Aktarım kabul onaylarını görüntüleme.

   Bu noktada, gelecekteki iş ortağı, müşteri ve geçerli iş ortağı, kabul edilen aktarım isteğine e-posta ile bildirilecek.

   Geçiş kabul edildikten sonra, sistem güncelleştirilirken aktarım durumu 15 dakika kadar Beklemede kalabilirsiniz. Daha uzun sürerse, sistem üç gün boyunca bunu yapmaya devam ediyor olur. Aktarım durumu hala Beklemede olarak kalırsa, iş ortağı bir hizmet isteği göndermektedir.

   Aktarım tamamlandıktan sonra, istekte yer alan abonelikler gelecekteki iş ortağının Azure planında görünür ve artık sizin için listelenmiyor.

>[!Note]  
>Dolaylı Sağlayıcılar için: Lütfen Dolaylı Kurumsal Bayinize aktarım isteğinin kabul olduğunu bildirin.

### <a name="managing-your-transferred-customer-subscriptions"></a>Aktarılan müşteri aboneliklerinizi yönetme

- Bu geçiş, Azure rol tabanlı erişim denetimi (RBAC) kullanılarak atanan mevcut kullanıcı, grup ve hizmet sorumlularını etkilemez. Azure rol tabanlı erişim denetimi [(Azure RBAC),](/azure/role-based-access-control/overview) müşterinizin Azure kaynaklarına kimlerin erişimi olduğunu, bu kaynaklarla neler yapalarını ve erişim sahip olduğu alanları yönetmelerine yardımcı olur. Yeni iş ortağı olarak, abonelik aktarımı sonrasında müşterinizin kaynaklarına RBAC erişimi verilmez. Müşterinizin önceki iş ortağı RBAC erişimini korur. Abonelikleri hakkında kimlerin içgörüleri olduğunu ve istediği değişiklikleri nasıl yapacaklarını anlamak için müşteriyle birlikte çalışabilirsiniz.

- Sonuç olarak, müşterinizin Azure RBAC erişimini önceki iş ortakları için kaldırmasının yanı sıra yeni iş ortağı için de erişim eklemesi önemlidir. Müşteriniz hakkında yeni erişim verme hakkında daha fazla bilgi için bkz. [Azure rol tabanlı erişim denetimi (Azure RBAC) nedir?](/azure/role-based-access-control/overview) Önceki iş ortağınızın RBAC erişimini kaldırma müşteriniz hakkında daha fazla bilgi için bkz. [rol atamasını kaldırma](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).

- Ayrıca, aboneliklerinize otomatik olarak [yönetici (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) erişimi de kalmaz. AOININ, iş ortağının müşterilerinin Azure aboneliklerini kendi adına yönetmesi gerekir. Azure ayrıcalıkları hakkında daha fazla bilgi için bkz [. bir müşterinin hizmetini veya aboneliğini yönetmek için Izinleri alma.](./customers-revoke-admin-privileges.md)

## <a name="next-steps"></a>Sonraki adımlar:

- [(Azure RBAC)](/azure/role-based-access-control/overview)
- [Müşterinin hizmetini veya aboneliğini yönetme izinleri alın.](./customers-revoke-admin-privileges.md)
