---
title: Müşteriler için Azure harcama bütçesi ayarlama
ms.topic: how-to
ms.date: 03/17/2021
description: Müşterileriniz için aylık Azure harcama bütçeleri ayarlamayı veya kaldırmayı ve ayrıca Azure harcama verilerini görüntülemeyi ve bütçeyle ilgili bildirimleri ayarlamayı öğrenin.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a2085713f1fef474dd26cb66a30a37f701789859
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961075"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>Azure'daki müşteriler için aylık Azure harcama bütçelerini ayarlama, denetleme veya İş Ortağı Merkezi

**Uygun roller:** Yönetici aracısı

[Azure'da müşterileriniz için aylık Bir Azure harcama bütçesi](#set-azure-spending-budget) İş Ortağı Merkezi. Bu, müşterilerinize Azure harcamalarını yönetmeye yardımcı olur. Bu seçenek, müşterinizin Azure harcamalarını ay boyunca bütçeyle karşılaştırmanızı sağlar. Ayrıca, müşterilerin aylık faturalarının beklenenden yüksek olması için Azure harcamalarını bütçelerine göre düzenlemelerine de yardımcı olur.

> [!NOTE]  
> Bu özellik korumalı alan veya Üretimde Test (TIP) hesaplarında kullanılamaz.

Müşteriniz [için bir Azure harcama bütçesi ayardikten](#set-azure-spending-budget)sonra, aşağıdaki yollarla müşteri kullanımını da gözden geçirebilirsiniz. Bu seçenekler yanlış yapılandırılmış hizmetleri veya sahtekarlık öneren olağan dışı eğilimleri tespit etmeye yardımcı olabilir. Daha sonra kök nedeni belirlemek ve maliyetleri yönetmek için müşterileriyle çalışabileceksiniz. Gerekirse müşterinin bütçesini [daha yüksek bir miktarla](#set-azure-spending-budget) da değiştirebilirsiniz.

- [Geçerli Azure harcamalarını denetleme](#check-current-azure-spending)

- [Müşterinin harcaması bütçe sınırına yaklaşıyorsa e-posta bildirimlerini açma](#notifications-for-budget-limits)

- [Kullanım tabanlı abonelikler için hizmete göre maddeleştirilmiş maliyetleri görüntüleme](#itemized-costs-by-service)

Ayrıca, [müşteriler için azure harcama](#remove-azure-spending-budget) bütçesini istediğiniz zaman kaldırabilirsiniz.

## <a name="azure-spending-data"></a>Azure harcama verileri

Azure harcama verileri bir *tahmindir ve* *gerçek faturalama tutarları değişiklik gösterebilir.* Verilerin değeri *vergileri, kredileri,* düzeltmeleri veya geçerli olan diğer ücretleri yansıtmaz.

Harcama verileri günde *bir kez yenilenir.* Müşterileriniz, azure hizmet ve kaynaklarını kullanmadıkça (ve ücret ödemeye) devam edebilirsiniz. Bu işlemden sonra da azure Azure portal.

## <a name="set-azure-spending-budget"></a>Azure harcama bütçesini ayarlama

Birden çok *müşteri için aylık Azure harcama bütçesi* İş Ortağı Merkezi:

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.

2. **CSP'nin** altındaki sol menüde **Azure harcaması'ı seçin.**

3. Azure **harcama sayfasındaki** **Abonelikleri Microsoft Azure** altında, bütçe ayarlamak istediğiniz müşterileri seçin.

4. Aylık bütçe için **bir değer girin.**

5. Değişikliklerinizi **kaydetmek** için Uygula'ya tıklayın.

Ayrıca abonelik *ayarlarından tek bir müşteri için bütçe* de sebilirsiniz:

1. İş Ortağı Merkezi panosunda oturum açın.

2. **CSP'nin** altındaki sol menüde Müşteriler'i **seçin.**

3. Müşteriler **sayfasında** müşterinin Şirket adını **seçin.**

4. Müşterinin Abonelikler **sayfasındaki** Kullanım tabanlı abonelik **altında Bütçeyi değiştir'i** **seçin.**

5. Bütçe için bir değer girin.

6. Değişikliklerinizi **kaydetmek** için Uygula'ya tıklayın.

## <a name="remove-azure-spending-budget"></a>Azure harcama bütçesini kaldırma

Müşterinizin *aylık Azure harcama bütçesini* şu şekilde İş Ortağı Merkezi:

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.

2. **CSP'nin** altındaki sol menüde **Azure harcaması'ı seçin.**

3. Azure **harcaması** sayfasındaki **Abonelikleri Microsoft Azure** altında, bütçesini kaldırmak istediğiniz müşterileri seçin.

4. Bütçeyi **kaldır'ı seçin.**

## <a name="check-current-azure-spending"></a>Geçerli Azure harcamalarını denetleme

Müşterilerin *geçerli Azure harcamalarını ve aylık bütçelerini herhangi bir zamanda* izleyebilirsiniz:

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.

2. **CSP'nin** altındaki sol menüde **Azure harcaması'ı seçin.**

3. Azure harcama **sayfasındaki** Abonelikleri Microsoft Azure altında müşterilerin aylık bütçelerine, geçerli harcama tahminlerine ve kullanılan bütçe yüzdesine genel bir bakış görebilirsiniz.

## <a name="notifications-for-budget-limits"></a>Bütçe sınırları için bildirimler

Müşterinizin *aylık harcaması bütçe* sınırına yaklaşacaksa e-posta bildirimlerini açabilirsiniz. Bu seçeneği açsanız, müşteriler aylık bütçelerinin %80'ini veya daha fazlasını kullanıyorsa size bildirilecek. Bu seçenek, Azure faturanızı takip etmek için size yardımcı olur. E-posta bildirimlerini yapılandırmak için:

1. İş Ortağı Merkezi'nde oturum açın.

2. Ayarlar. 

3. **Tercihlerim'i seçin.**

4. Tercih edilen e-posta adresini yapılandırmadıysanız, bu adresi yapılandırma.

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
