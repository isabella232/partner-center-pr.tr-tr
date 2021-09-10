---
title: Aktarım uygunluğu – Bir aboneliği faturalama hesapları arasında aktarma yönergeleri, Azure Market
description: Bir aboneliği fatura hesabı arasında aktarmadan önce ticari denetimlere yönelik yönergeler Azure portal.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 4b235bd462915fc205813ae86e92f98b4fd49fe4
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123936975"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a>Faturalama hesapları arasında abonelik için uygunluğu aktarma

Aboneliği [bir ödeme hesabından](/azure/cost-management-billing/understand/subscription-transfer) diğerine, aboneliğin faturalama bölümünde Azure portal. Aktarımdan önce abonelikte üçüncü taraf ürünler taranır. Aktarıma yalnızca tüm ürünler *aktarım için* temizlenmiştir (aşağıdaki ölçütlere bakın) [izin](#criteria-for-transfer-approval-or-denial) verilir. Sistem, sonraki adımları belirlemenize yardımcı olmak için temizlenemedi uygulamalar için ilgili hata iletileri oluşturacak.

> [!NOTE]
> SaaS kaynakları aboneliğe değil kiracıya ekli olduğundan bu makale SaaS teklifleri için geçerli değildir. SaaS kaynakları bir ödeme hesabından diğerine aktarılabilir, ancak bu, kaynak başına ve Azure desteği isteği olarak yapılır.

## <a name="criteria-for-transfer-approval-or-denial"></a>Onay veya reddetme aktarımı ölçütleri

Üçüncü taraf uygulamalardan herhangi biri aşağıdaki ölçütlerden herhangi birini karşılarsa aboneliği aktaramazsınız:

- Hedef hesap ticaridir ve uygulama iş ortakları aracılığıyla satılmayı kabul etmektir.
- Uygulama seçili iş ortaklarını kabul ediyor ve hedef hesap izin verme listesinde değil.
- Teklif, geçmişte seçili abonelikler için bir önizleme teklifi veya özel bir teklifdi ve abonelik artık izin verme listesinde yer almadı.
- Yeni ödeme hesabı, teklifin satıldığı bölgeden farklı bir bölgededir VE teklif bu bölgede satılmamaktadır.

Siz kaynağı abonelikten kaldırana kadar engellenen aktarım devam ediyor ve ardından aktarımı yeniden denemeniz gerekiyor.

## <a name="next-steps"></a>Sonraki adımlar

[Microsoft AppSource ve Azure Market](get-support.md)

