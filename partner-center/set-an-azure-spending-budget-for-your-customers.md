---
title: Müşteriler için Azure harcama bütçesi ayarlama
ms.topic: how-to
ms.date: 03/17/2021
description: Müşterileriniz için aylık Azure harcama bütçeleri ayarlamayı veya kaldırmayı ve ayrıca Azure harcama verilerini görüntülemeyi ve bütçeyle ilgili bildirimleri ayarlamayı öğrenin.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14e901f51841e58b28a3cbbb1b7a19ce89d7c324
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855361"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>Azure'daki müşteriler için aylık Azure harcama bütçelerini ayarlama, denetleme veya İş Ortağı Merkezi

**Uygun roller:** Yönetici aracısı

[Azure'da müşterileriniz için aylık Bir Azure harcama bütçesi](#set-azure-spending-budget) İş Ortağı Merkezi. Bu, müşterilerinize Azure harcamalarını yönetmeye yardımcı olur. Bu seçenek, müşterinizin Azure harcamalarını ay boyunca bütçeyle karşılaştırmanızı sağlar. Ayrıca, müşterilerin aylık faturalarının beklenenden yüksek olması için Azure harcamaları için bütçelerini düzenlemelerine de yardımcı olur.

> [!NOTE]  
> Bu özellik korumalı alan veya Üretimde Test (TIP) hesaplarında kullanılamaz.

Müşteriniz [için bir Azure harcama bütçesi ayardikten](#set-azure-spending-budget)sonra, aşağıdaki yollarla müşteri kullanımını da gözden geçirebilirsiniz. Bu seçenekler yanlış yapılandırılmış hizmetleri veya sahtekarlık öneren olağan dışı eğilimleri tespit etmeye yardımcı olabilir. Daha sonra kök nedeni belirlemek ve maliyetleri yönetmek için müşterileriyle çalışabileceksiniz. Gerekirse müşterinin bütçesini [daha yüksek bir miktarla](#set-azure-spending-budget) da değiştirebilirsiniz.

- [Geçerli Azure harcamalarını denetleme](#check-current-azure-spending)

- [Müşterinin harcaması bütçe sınırına yaklaşıyorsa e-posta bildirimlerini açma](#notifications-for-budget-limits)

- [Kullanım tabanlı abonelikler için hizmete göre maddeleştirilmiş maliyetleri görüntüleme](#itemized-costs-by-service)

Ayrıca, [müşteriler için azure harcama](#remove-azure-spending-budget) bütçesini istediğiniz zaman kaldırabilirsiniz.

## <a name="azure-spending-data"></a>Azure harcama verileri

Azure harcama verileri bir *tahmindir ve* *gerçek faturalama tutarları değişiklik gösterebilir.* Verilerin değeri *vergileri, kredileri,* düzeltmeleri veya uygulanabilecek diğer ücretleri yansıtmaz.

Harcama verileri günde *bir kez yenilenir.* Müşterileriniz, Azure portal hesap ayarlarını değiştirmediğiniz müddetçe Azure hizmetleri ve kaynakları kullanmaya ve ücretlendirmeye devam edebilir.

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

2. **CSP'nin** altındaki sol menüde **Azure harcaması'ı seçin.**

3. Azure **harcaması sayfasındaki** Microsoft Azure abonelikleri olan müşteriler altında müşterilerin aylık bütçelerine, geçerli harcama tahminlerine ve kullanılan bütçe yüzdesine genel bir bakış görebilirsiniz. 

## <a name="notifications-for-budget-limits"></a>Bütçe sınırları için bildirimler

Müşterinizin *aylık harcaması bütçe* sınırına yaklaşacaksa e-posta bildirimlerini açabilirsiniz. Bu seçeneği açsanız, müşteriler aylık bütçelerinin %80'ini veya daha fazlasını kullanıyorsa size bildirilecek. Bu seçenek, Azure faturanızı takip etmek için size yardımcı olur. E-posta bildirimlerini yapılandırmak için:

1. İş Ortağı Merkezi'nde oturum açın.

2. **Ayarlar'a gidin.**

3. **Tercihlerim'i seçin.**

4. Tercih edilen bir e-posta adresi yapılandırmadısanız.

5. Bildirim için tercih edilen dili yapılandırma.

6. Bildirim **tercihleri bölümünde CSP** **sekmesini** seçin.

7. Azure Harcama bildirimi için **E-posta seçeneğini işaretleyin** ve **Kaydet'i seçin.**


## <a name="itemized-costs-by-service"></a>Hizmete göre maddeleştirilmiş maliyetler

Kullanım tabanlı *abonelikler için hizmete göre maddeleştirilmiş maliyetleri (ve tahmini kullanımı) görüntüebilirsiniz:*

1. İş Ortağı Merkezi'nde oturum açın.

2. **CSP'nin** altındaki sol menüde Müşteriler'i **seçin.**

3. Müşteriler **sayfasında** müşterinin Şirket adını **seçin.**

4. Müşterinin Abonelikler **sayfasındaki** Kullanım **tabanlı abonelikler** altında Aboneliğin adını **seçin.**

5. Aboneliğin sayfasında Hizmete göre maddeleştirilmiş maliyetleri **ve** geçerli aya yönelik **tahmini kullanımı** gözden geçirebilirsiniz.


## <a name="next-steps"></a>Sonraki adımlar

- [CSP'de yeni ticari deneyim - Azure faturalama](azure-plan-billing.md)
