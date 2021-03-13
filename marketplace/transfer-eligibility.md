---
title: Aktarım uygunluğu – bir aboneliği faturalandırma hesapları, Azure Marketi arasında aktarmaya yönelik yönergeler
description: Azure portal faturalandırma hesapları arasında abonelik aktarmadan önce ticari denetimleri için yönergeler.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 4b235bd462915fc205813ae86e92f98b4fd49fe4
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412565"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a>Faturalama hesapları arasında bir abonelik için aktarım uygunluğu

Azure portal Faturalandırma bölümünde bir faturalandırma hesabından diğerine [abonelik aktarabilirsiniz](/azure/cost-management-billing/understand/subscription-transfer) . Bir aktarımdan önce abonelik, üçüncü taraf ürünleri için taranır. Aktarıma yalnızca *Tüm* ürünler aktarım için silinirse izin verilir (aşağıdaki [ölçütlere](#criteria-for-transfer-approval-or-denial) bakın). Sistem, sonraki adımları belirlemenize yardımcı olmak için temizlendirilemez uygulamalar için ilgili hata iletileri oluşturur.

> [!NOTE]
> SaaS kaynakları bir aboneliğe değil bir kiracıya eklendiğinden, bu makale SaaS teklifleri için geçerlidir. SaaS kaynakları bir faturalandırma hesabından diğerine aktarılabilir, ancak bu, kaynak başına ve destek talebi olarak Azure desteği tarafından yapılır.

## <a name="criteria-for-transfer-approval-or-denial"></a>Aktarım onayı veya reddetme ölçütü

Üçüncü taraf uygulamalarından herhangi biri aşağıdaki ölçütlerden herhangi birini karşılıyorsa aboneliği aktaramazsınız:

- Hedef hesap ticari ve uygulama iş ortakları aracılığıyla satılacak şekilde kabul edilir.
- Uygulama, seçilen iş ortakları için kabul ediyor ve hedef hesap izin verilenler listesinde değil.
- Teklif, geçmişte seçili abonelikler için bir önizleme teklifiydi veya özel bir teklifdi ve abonelik artık izin verilenler listesinde değil.
- Yeni faturalandırma hesabı, teklifin satışında farklı olan ve teklifin bu bölgede satılmama yeri dışında bir bölgedir.

Engellenen bir aktarım, kaynağı abonelikten kaldırana kadar etkin kalır, sonra aktarmayı yeniden deneyebilirsiniz.

## <a name="next-steps"></a>Sonraki adımlar

[Microsoft AppSource ve Azure Marketi için destek alın](get-support.md)

