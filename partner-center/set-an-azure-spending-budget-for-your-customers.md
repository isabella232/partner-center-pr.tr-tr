---
title: Müşteriler için Azure harcama bütçesi ayarlama
ms.topic: how-to
ms.date: 03/17/2021
description: Müşterileriniz için aylık Azure harcama bütçelerini ayarlamayı veya kaldırmayı ve ayrıca Azure harcama verilerini görüntülemeyi ve bütçeye ilişkin bildirimleri ayarlamayı öğrenin.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a2085713f1fef474dd26cb66a30a37f701789859
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248578"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>Iş Ortağı Merkezi 'nde müşterilere yönelik aylık Azure harcama bütçelerini ayarlama, denetleme veya kaldırma

**Uygun roller**: Yönetim Aracısı

Iş Ortağı Merkezi 'nde [müşterileriniz için aylık bir Azure harcama bütçesi ayarlayabilirsiniz](#set-azure-spending-budget) . Bu, müşterilerinizin Azure harcamalarını yönetmesine yardımcı olur. Bu seçenek, müşterilerinizin aylık dönemi boyunca Azure harcamalarınızı bütçenize göre karşılaştırmanızı sağlar. Ayrıca, müşterilerinizin aylık faturanız düşünenden daha yüksek olmaması için Azure harcamalarını bütçelerinize de yardımcı olur.

> [!NOTE]  
> Bu özellik korumalı alanda veya üretimde test (tıp) hesaplarında kullanılamaz.

Müşterilerinizin [Azure harcama bütçesini ayarladıktan](#set-azure-spending-budget)sonra, müşteri kullanımını aşağıdaki yollarla da gözden geçirebilirsiniz. Bu seçenekler, yanlış yapılandırılmış Hizmetleri veya sahtekarlık önereceği olağan dışı eğilimleri belirlemenize yardımcı olabilir. Bundan sonra, temel nedeni belirlemek ve maliyetleri yönetmek için müşteri (ler) i ile çalışabilirsiniz. Gerekirse, [müşterinin bütçesini](#set-azure-spending-budget) daha yüksek bir tutara de değiştirebilirsiniz.

- [Geçerli Azure harcamayı denetle](#check-current-azure-spending)

- [Müşterinin harcama süresi Bütçe limitine yaklaştığı zaman için e-posta bildirimlerini aç](#notifications-for-budget-limits)

- [Kullanım tabanlı abonelikler için hizmete göre listelenen maliyetleri görüntüleme](#itemized-costs-by-service)

Ayrıca, müşteriler için [bir Azure harcama bütçesini](#remove-azure-spending-budget) dilediğiniz zaman kaldırabilirsiniz.

## <a name="azure-spending-data"></a>Azure harcama verileri

Azure harcama verileri bir *tahmindir* ve *gerçek faturalandırma miktarları farklılık* gösterebilir. Verilerin değeri vergileri, kredilerin, ayarlamaların veya uygulayabilen diğer ücretleri *yansıtmaz* .

Harcama verileri *günde bir kez yenilenir*. Müşterileriniz, Azure portal hesap ayarlarını değiştirmediğiniz müddetçe Azure hizmetleri ve kaynakları kullanmaya ve ücretlendirmeye devam edebilir.

## <a name="set-azure-spending-budget"></a>Azure harcama bütçesini ayarlama

Iş Ortağı Merkezi 'nde birden çok müşteri için *aylık bir Azure harcama bütçesi ayarlayabilirsiniz* :

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.

2. **CSP** altındaki sol menüde **Azure harcama**' i seçin.

3. **Azure harcama** sayfasında, **Microsoft Azure abonelikleri olan müşteriler** altında, bütçesini ayarlamak istediğiniz müşteri (ler) i seçin.

4. **Aylık bütçe** için bir değer girin.

5. Değişikliklerinizi kaydetmek için **Uygula** ' yı seçin.

Ayrıca, abonelik ayarlarında *tek bir müşteri için bir bütçe ayarlayabilirsiniz* :

1. İş Ortağı Merkezi panosunda oturum açın.

2. **CSP** altındaki sol menüde **müşteriler**' i seçin.

3. **Müşteriler** sayfasında, müşterinin **şirket adını** seçin.

4. Müşterinin **abonelikler** sayfasında, **Kullanım tabanlı abonelik**' ın altında, **bütçeyi Değiştir**' i seçin.

5. Bütçe için bir değer girin.

6. Değişikliklerinizi kaydetmek için **Uygula** ' yı seçin.

## <a name="remove-azure-spending-budget"></a>Azure harcama bütçesini kaldırma

Iş Ortağı Merkezi 'nde müşteri (ler) için *aylık bir Azure harcama bütçesini kaldırabilirsiniz* :

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.

2. **CSP** altındaki sol menüde **Azure harcama**' i seçin.

3. **Azure harcama** sayfasında, **Microsoft Azure abonelikleri olan müşteriler** altında, bütçesini kaldırmak istediğiniz müşteri (ler) i seçin.

4. **Bütçeyi Kaldır**' ı seçin.

## <a name="check-current-azure-spending"></a>Geçerli Azure harcamayı denetle

*Müşterilerinizin geçerli Azure harcamalarını ve aylık bütçelerinin* dilediğiniz zaman izlenmesini sağlayabilirsiniz:

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.

2. **CSP** altındaki sol menüde **Azure harcama**' i seçin.

3. **Azure harcama** sayfasında, **Microsoft Azure abonelikleri olan müşteriler** altında müşterilerin aylık bütçeleri, geçerli harcama tahminleri ve kullanılan bütçenin yüzdesi hakkında bir genel bakış görebilirsiniz.

## <a name="notifications-for-budget-limits"></a>Bütçe limitlerinin bildirimleri

Müşterinizin aylık harcama süresi Bütçe limitine yaklaştığı zaman için *e-posta bildirimlerini açabilirsiniz* . Bu seçeneği etkinleştirdiğinizde, müşteriler aylık bütçesinden %80 veya daha fazlasını kullandıklarında bildirim alırsınız. Bu seçenek, Azure faturanızda bir göz kalmanıza yardımcı olur. E-posta bildirimlerini yapılandırmak için:

1. İş Ortağı Merkezi'nde oturum açın.

2. **Ayarlar** gidin.

3. **Tercihlerimi** seçin.

4. Yapmadıysanız tercih edilen e-posta adresini yapılandırın.

5. Bildirim için tercih edilen dili yapılandırın.

6. **Bildirim tercihleri** bölümünde **CSP** sekmesini seçin.

7. **Azure harcama** bildirimi Için e-posta seçeneğini Işaretleyin ve **kaydedin**.


## <a name="itemized-costs-by-service"></a>Hizmete göre listelenen maliyetler

*Kullanım tabanlı abonelikler için, hizmete göre listelenen maliyeti (ve tahmini kullanımı)* görebilirsiniz:

1. İş Ortağı Merkezi'nde oturum açın.

2. **CSP** altındaki sol menüde **müşteriler**' i seçin.

3. **Müşteriler** sayfasında, müşterinin **şirket adını** seçin.

4. Müşterinin **abonelikler** sayfasında, **Kullanım tabanlı abonelikler**' in altında, **aboneliğin** adını seçin.

5. Aboneliğin sayfasında, hizmete göre **listelenen maliyeti** ve geçerli ay için **Tahmini kullanımı** gözden geçirebilirsiniz.


## <a name="next-steps"></a>Sonraki adımlar

- [CSP'de yeni ticari deneyim - Azure faturalama](azure-plan-billing.md)
