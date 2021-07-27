---
title: İş ortağı kazanılmış kredisi sorunlarını giderme
ms.topic: article
ms.date: 07/22/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: İş ortağı kazanılmış kredisi (PEC) ile ilgili fatura sorunlarını ve diğer sorunları nasıl ele alabileceğinizi öğrenin.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9d7376b6224047176b5e6608ee190191a8f44824
ms.sourcegitcommit: d133c8b923b90ac5518cb989c0ce4dd69713abf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/22/2021
ms.locfileid: "114434225"
---
# <a name="troubleshooting-partner-earned-credit"></a>İş ortağı kazanılmış kredisi sorunlarını giderme

**Uygun roller**: genel yönetici | Kullanıcı Yönetimi Yöneticisi | Yönetici Aracısı | Faturalandırma Yöneticisi | Satış Aracısı

## <a name="troubleshooting-guide"></a>Sorun giderme kılavuzu

Erişim veya eksik bilgiler gibi PEC ile ilgili sorunlarınız varsa, listelenen sırayla aşağıdaki öğeleri kontrol edin.

1. G (modern) faturasına ve keşfi dosyasına baktığınızdan emin olun. Azure planı ve PEC, D (eski) faturasında veya keşfi dosyasında gösterilmez.

2. İş ortağının türünü belirler. (Dolaylı satıcılar uygun değildir.)

3. MPN sözleşmenizin etkin olduğunu doğrulayın.

4. Dolaylı sağlayıcılar için, Iş Ortağı Merkezi 'ne (veya API aracılığıyla) girilen Bayi MPN KIMLIĞININ Azure portal, satıcıdan girilen MPN KIMLIĞIYLE eşleştiğinden emin olun.

5. Teklifinizin uygun olduğunu onaylayın. (Eski Azure teklifleri, Azure ayrılmış örnekleri ve üçüncü taraf ürünleri uygun değildir.)

6. Abonelik/kaynak grubu/kaynak için geçerli bir Yönet adına (AOBO) veya Role-Based Access Control (RBAC) rolüne sahip olduğunu doğrulayın.

7. Müşterinin RBAC rolünüzü kaldırıp kaldırmadığını belirleme. Bu durumda, bkz. bir müşterinin Azure CSP abonelikleri için yeniden devreye sokma yönetici ayrıcalıkları

8. Tüm gün için yönetici erişiminizin olduğunu doğrulayın.

9. Günlük kullanım dosyanızda doğru sütunları gözden geçirolduğunuzu onaylayın.

## <a name="next-steps"></a>Sonraki adımlar

- [CSP 'de Azure için yeni ticari deneyim fiyat listesi](azure-plan-price-list.md)
- [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)
- [CSP'de yeni ticari deneyim - Azure faturalama](azure-plan-billing.md)
- [Azure CSP abonelikleri için yönetici ayrıcalıklarını yeniden devreye sokma](revoke-reinstate-csp.md)
- [İş ortağı kazanılmış kredi-genel bakış](partner-earned-credit.md)
- [Roller, iş ortağı kazanılmış kredi için izinler](azure-roles-perms-pec.md)
- [Iş ortağı kazanılmış krediyi anlama (kılavuz)](https://partner.microsoft.com/resources/detail/understanding-partner-earned-credit-pdf) (oturum açma gerekir)
