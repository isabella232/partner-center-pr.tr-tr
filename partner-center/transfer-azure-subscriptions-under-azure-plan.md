---
title: Azure planı kapsamındaki Azure aboneliğini başka bir CSP iş ortağına aktarma
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Müşterinin Azure abonelikleriyle ilişkili Bulut Çözümü Sağlayıcısı program iş ortağını azure planı kapsamında değiştirme hakkında bilgi edinin.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/21/2021
ms.openlocfilehash: 14f03a8eb899f7224a38b0f998edd72077b34b3b
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248298"
---
# <a name="transfer-a-customers-azure-subscriptions-to-a-different-csp-under-an-azure-plan"></a>Müşterinin Azure aboneliklerini farklı bir CSP'ye aktarma (Azure planı kapsamında)

**Uygun roller:** Hesap yöneticisi | Satış aracısı | Faturalama aracısı

Bu makalede, müşterilerin Azure planı kapsamında azure aboneliklerini Bulut Çözümü Sağlayıcısı (CSP) programından diğerine nasıl değiştireleri açıklanmıştır.

Farklı bir iş ortağından müşterinin Azure aboneliklerini değiştirmek için aşağıdaki adımları izleyin. Geçerli iş ortağı, gelecekteki iş ortağı ve müşterinin tamamlanacak adımları var.

> [!Note]  
> Geçiş aracına yalnızca Microsoft ile doğrudan faturalama ilişkisi olan iş ortakları erişebilirsiniz. Dolaylı kurumsal bayilerin bu geçiş aracını kullanmak için dolaylı sağlayıcılarıyla birlikte çalışması gerekir.

Geçiş aracının kullanılamadan önce müşterinin hem geçerli hem de gelecekteki iş ortağıyla iletişim kurması gerekir. Karışıklığı ve karışıklığı önlemek için çevrimdışı bir konuşma yapılması gerekir. İş ortakları ve müşteriler, geçişe başlamadan önce aşağıdaki konuları ve önkoşulları anlamalı.

## <a name="considerations"></a>Dikkat edilmesi gerekenler

- Azure Rezervasyonları bir abonelikle gelecekteki iş ortağına taşınmaz.
- Geçerli iş ortağı altındaki Azure hizmetleri için CSP fiyatlandırması geçiş olmayacaktır.
- Önceki Azure teklifi [(MS-AZR-0145p)](https://go.microsoft.com/fwlink/p/?linkid=2164140) aboneliklerini aktardısanız, bu Azure abonelikleri aynı anda bir Azure planı içindeki yeni Azure teklifi abonelikleri olacak şekilde dönüştürülür.
- Müşterinin destek sorumlulukları gelecekteki iş ortağına taşınacak.
- Faturalama ve faturalama, abonelik aktarıldıklarında gelecekteki iş ortağına taşınacak.
- Azure rol tabanlı erişim denetimi (RBAC) aktarımlardan etkilenmez.
- Yönetici Adına (AOBO) varsayılan olarak gelecekteki iş ortağına verilmez.
- Üçüncü taraf Azure Market, ürünler uygunluk denetimine geçeceği sürece Azure Market aktaracak.
    - Özel indirimler veya bölgesel kısıtlamalar yoktur.
    - Ürünler abonelik tabanlı değil.
    - Gelecekteki iş ortağı, yayımcının ürünün dağıtımı için izin verme listesine sahip olduğundan emin olmak için yayımcıyla birlikte çalışmalı.
    - Bu koşullardan herhangi biri karşı koşulların karşı Azure Market iptal edilmesi gerekir. Ardından Azure abonelikleri aktarıldı ve Azure Market yeni iş ortağıyla birlikte satın alınmaktadır.

## <a name="prerequisites"></a>Önkoşullar

- Müşteri, geçiş amacının geçerli CSP iş ortağına bilgi sağlar.
- Gelecekteki CSP iş ortağı, müşterinin ihtiyaçlarının karşılanamaması için müşteriyle birlikte çalışır.
- Gelecekteki CSP iş ortağı müşteriyle bir ilişki kuracak ve geçiş başlamadan önce bir Azure planı satın alır.
- Müşteri, gelecekteki CSP Microsoft Müşteri Sözleşmesi bir iş ortağıyla bir iş ortağı imzalar.
- Gelecekteki CSP iş ortağı, Microsoft İş Ortağı Sözleşmesi aracını kullanmadan önce iş ortağını imzalar.

> [!NOTE]
> Self servis geçiş aracı, müşterinin geçerli iş ortağı önceki Azure teklifine (MS-AZR-0145p) veya yeni Azure teklifine (Azure planı) sahip olduğunda kullanılabilir. Her iki durumda da aktarım tamamlandığında, Azure abonelikleri gelecekteki iş ortağıyla bir Azure planı altında olacaktır.

## <a name="customer-tasks"></a>Müşteri görevleri

Azure aboneliklerini aktarması için müşterinin geçerli iş ortağıyla iletişime geçerek süreci başlatması gerekir. Gelecekteki iş ortağının müşteri adına aktarım isteği formunu tamamlaması için müşterinin geçerli iş ortağının şirket adını ve Microsoft kimliğini toplaması gerekir.

Müşterilerin ayrıca geçerli iş ortağından aktarma yapmak istediğiniz abonelikleri tanımlaması gerekir. Office 365, Enterprise Mobility Suite veya Microsoft Dynamics CRM iş Microsoft Dynamics CRM değiştiremezsiniz.

> [!NOTE]  
> Aktarım işlemini başlatan aktarım isteği formunu tamamlamak gelecekteki iş ortağının sorumluluğundadır. Microsoft, müşteri veya geçerli iş ortağı adına müdahalede bulunacak bir çözüme neden olabilir. Müşterinin, geçişin sorunsuz bir şekilde devam ettiğine emin olmak için gelecekteki ve mevcut iş ortaklarıyla yakın bir çalışma planlaması gerekir.

## <a name="future-partner-tasks"></a>Gelecekteki iş ortağı görevleri 

Aboneliğin gelecekteki iş ortağının, abonelik aktarımı isteği için İş Ortağı Merkezi bir aktarım isteği formunu tamamlaması gerekir:

1.  Veri aktarımının sol İş Ortağı Merkezi **Müşteriler'i** seçin ve ardından aktarım isteğini tamamlamak istediğiniz müşteriyi seçin.
2.  Müşteriye özgü menüde Abonelikler'i **seçin.**
3.  Aktarım istekleri **sekmesinde Yeni istek** **ekle'yi seçin:**

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Aktarım istekleri sekmesini gösteren ekran görüntüsü.":::

5.  Yeni aktarım **isteği formunu** doldurun:

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Yeni aktarım isteği formunu gösteren ekran görüntüsü.":::

6.  Aktarım **isteği gönder Gönder'i**  >  **seçin.**

7.  Aktarım isteği onaylarını gözden geçirme:

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Aktarım isteği onayı gösteren ekran görüntüsü.":::

    > [!NOTE]
    > Gelecekteki iş ortağı, pencerenin sağ  üst köşesindeki İsteği iptal et'i seçerek ancak aktarım isteği durumu "beklemede" olduğunda aktarım isteğini iptal edebilir. Aktarım isteği durumu "sürüyor" veya "tamamlandı" olduktan sonra iptaller mümkün değildir.

## <a name="current-partner-tasks"></a>Geçerli iş ortağı görevleri 

Müşterinin geçerli iş ortağının Yönetici aracısı, müşterinin abonelik aktarımı isteğinda olduğunu belirten bir e-posta alır:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Aktarım için müşteri isteğinin e-posta bildirimini gösteren ekran görüntüsü.":::

Geçerli iş ortağının abonelik aktarımını tamamlamak için İş Ortağı Merkezi isteği formunu gözden geçirmesi ve kabul etmesi gerekir.

> [!NOTE]  
> Geçerli iş ortağı 30 gün içinde yanıt vermiyorsa isteğin süresi dolar ve gelecekteki iş ortağının yeni bir aktarım isteği oluşturması gerekir.

1. Aşağıdaki eylemlerden birini uygulayın: 
   - **E-postada Aktarım isteğini gözden** geçir'i seçin.

     veya

    - Veri bölmesinin sol İş Ortağı Merkezi Müşteriler'i seçin ve ardından aktarım isteğinin gönder olduğu müşteriyi seçin. 
      1. Müşteriye özgü menüde Abonelikler'i **seçin.**
      1. Aktarım **istekleri sekmesinde,** Alınan istekler altında Aktarım isteği kimliğini seçerek **aktarım** **bilgilerini genişletin:**

      :::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Geçerli iş ortağı tarafından görülen Aktarım istekleri sekmesini gösteren ekran görüntüsü.":::

5. Aktarım isteğini gözden geçirme. Aktarımın istenen Azure aboneliklerini seçin.
 
   Devam etmek için şunları unutmayın:
   - Artık seçili aboneliklere erişemeyeceksiniz.
   - Daha fazla kullanım için fatura ödemezsiniz.
   - Azure rezervasyonları aboneliklerle aktarnmaz.

6. Aktarım **işlemini tamamlamak için Kabul** et ve aktar'ı seçin:

   :::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Aktarım isteğini gözden geçir ekran görüntüsünü gösteren ekran görüntüsü.":::

   Önceki Azure teklifi aboneliklerine (MS-AZR-0145p) sahip bir müşteriniz varsa, aynı şekilde devam edin, aktarlanacak abonelikleri seçin ve ardından aktarım işlemini tamamlamak için Kabul et **ve aktar'ı** seçin.

7. Aktarım kabul onaylarını görüntüleme.

   Bu noktada, gelecekteki iş ortağına, müşteriye ve geçerli iş ortağına kabul edilen aktarım isteği hakkında bir e-posta gönderilir.

   Geçiş kabul edildikten sonra, sistem güncelleştirilirken aktarım durumu 15 dakika boyunca "beklemede" olarak kalabilirsiniz. Bu işlem daha uzun sürerse, sistem üç gün boyunca bunu yapmaya devam ediyor olur. Aktarım durumu üç günden uzun süre "beklemede" kalırsa, iş ortağı bir hizmet isteği göndermesi gerekir.

   Aktarım tamamlandıktan sonra, istekte yer alan abonelikler gelecekteki iş ortağının Azure planında görünür. Artık geçerli iş ortağıyla listelenmiyor.

>[!Note]  
>Dolaylı sağlayıcılar, dolaylı kurumsal bayilerine aktarım isteğinin kabul edildiklerini bildirmeleri gerekir.

### <a name="managing-your-transferred-customer-subscriptions"></a>Aktarılan müşteri aboneliklerinizi yönetme

Azure RBAC aracılığıyla atanan mevcut kullanıcılara, gruplara veya hizmet sorumlularına erişim, geçiş sırasında etkilenmez. [Azure RBAC,](/azure/role-based-access-control/overview) müşterinizin Azure kaynaklarına kimlerin erişimi olduğunu, bu kaynaklarla neler yapalarını ve hangi alanlara erişimleri olduğunu yönetmelerine yardımcı olur. 

Yeni bir iş ortağı olarak, abonelik aktarımı sonrasında müşterinizin kaynaklarına RBAC erişimine sahip olmayacaksınız. Müşterinizin önceki iş ortağı RBAC erişimini korur. Aboneliklerle ilgili kimlerin içgörüleri olduğunu ve gerekli değişiklikleri nasıl yapacaklarını anlamak için müşteriyle birlikte çalışabilirsiniz.

Müşterinizin önceki iş ortağı için Azure RBAC erişimini kaldırması ve sizin için erişim eklemesi gerekir. Erişim sağlama hakkında daha fazla bilgi için [bkz. Azure rol tabanlı erişim denetimi (Azure RBAC) nedir?](/azure/role-based-access-control/overview). Erişimi kaldırma hakkında daha fazla bilgi için [bkz. Rol ataması kaldırma.](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)

Ayrıca aboneliklerinize Otomatik Olarak [Yönetici Adına (AOBO) erişim](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) elde edersiniz. AOBO, müşterinizin Azure aboneliklerini yönetebilirsiniz. Azure ayrıcalıkları hakkında daha fazla bilgi için bkz. [Müşterinin hizmetini veya aboneliğini yönetme izinleri alma](./customers-revoke-admin-privileges.md).

## <a name="next-steps"></a>Sonraki adımlar

- [Azure RBAC](/azure/role-based-access-control/overview)
- [Müşterinin hizmetini veya aboneliğini yönetmek için izinler alma](./customers-revoke-admin-privileges.md)
