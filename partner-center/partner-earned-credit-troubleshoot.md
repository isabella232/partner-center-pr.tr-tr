---
title: İş ortağı tarafından kazanılan kredi sorunlarını giderme
ms.topic: article
ms.date: 07/22/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: İş ortağı tarafından kazanılan kredi (PEC) ile ilgili fatura sorunlarını ve diğer sorunları çözmeyi öğrenin.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: a8bb370c7154c8033990cac798c28e01eec7e17f
ms.sourcegitcommit: 76a7dac540d129ae15cd4c251a4ff43d768370da
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/06/2021
ms.locfileid: "129593234"
---
# <a name="troubleshooting-partner-earned-credit"></a>İş ortağı tarafından kazanılan kredi sorunlarını giderme

**Uygun roller:** Genel yönetici | Kullanıcı yönetimi yönetici | Yönetici aracısı | Faturalama yöneticisi | Satış aracısı

## <a name="troubleshooting-guide"></a>Sorun giderme kılavuzu

PEC ile ilgili erişim veya eksik bilgiler gibi sorunları varsa aşağıdaki öğeleri listelenen sırayla kontrol edin.

1. G (Modern) fatura ve mutabakat dosyasına bakarak emin olun. Azure planı ve PEC, D (Eski) fatura veya mutabakat dosyasında gösterilmez.

2. İş ortağının türünü belirleme. (Dolaylı Kurumsal Bayiler uygun değildir.)

3. MPN sözleşmenizin etkin olduğunu onaylayın.

4. Dolaylı Sağlayıcılar için, İş Ortağı Merkezi 'a (veya API aracılığıyla) girilen kurumsal bayinin MPN Kimliğinin, satıcıya girilen mpN kimliğiyle eş Azure portal.

5. Teklifinizin uygun olduğunu onaylayın. (Eski Azure teklifleri, Azure Ayrılmış Örnekleri ve üçüncü taraf ürünleri uygun değildir.)

6. Abonelik/kaynak grubu/kaynak için geçerli bir Adına Yönet (AOBO) veya Role-Based Access Control (RBAC) rolüne sahip olduğunu onaylayın.

7. Müşterinin RBAC rollerinizi kaldırıp kaldıra olmadığını belirleme. Öyleyse, bkz. Müşterinin abonelikleri için yönetici ayrıcalıklarını Azure CSP durumuna alma

8. Gün boyunca yönetici erişimine sahip olduğunu onaylayın.

9. Günlük kullanım dosyanıza doğru sütunları gözden geçirerek onaylayın.

## <a name="next-steps"></a>Sonraki adımlar

- [Yeni ticari deneyim için fiyat listesi CSP'de Azure](azure-plan-price-list.md)
- [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)
- [CSP'de yeni ticari deneyim - Azure faturalama](azure-plan-billing.md)
- [Azure CSP abonelikleri için yönetici ayrıcalıklarını yeniden devreye sokma](reinstate-csp.md)
- [İş ortağı tarafından kazanılan kredi - genel bakış](partner-earned-credit.md)
- [Roller, iş ortağı tarafından kazanılan kredi izinleri](azure-roles-perms-pec.md)
- [İş Ortağı Tarafından Kazanılan Krediyi Anlama (kılavuz)](https://partner.microsoft.com/resources/detail/understanding-partner-earned-credit-pdf) (oturum açma gereklidir)
