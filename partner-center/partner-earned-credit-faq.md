---
title: İş ortağı kazanılmış Kredi SSS
ms.topic: article
ms.date: 07/22/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: İş ortağı kazanılmış kredisi (PEC) ile ilgili sık sorulan soruların yanıtlarını bulun.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 4efffe1bb01fd2822e20c39b828197b422e63caa2141528f531ada882db231b4
ms.sourcegitcommit: dfed8309ec4ba4cbe5af05d0dcd30e4151ed17e6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/12/2021
ms.locfileid: "121469719"
---
# <a name="frequently-asked-questions-for-partner-earned-credit"></a>İş ortağı kazanılmış kredisi hakkında sık sorulan sorular

Uygun roller: genel yönetici | Kullanıcı Yönetimi Yöneticisi | Yönetici Aracısı | Faturalandırma Yöneticisi | Satış Aracısı

Aşağıda, ortağın kazanılmasıyla ilgili sık sorulan soruların bir listesi verilmiştir.

## <a name="how-much-is-pec"></a>PEC ne kadar?

PEC için kazanılabilecek miktar iş ortakları farklılık gösterir (bkz. [Hesaplama](partner-earned-credit-explanation.md#calculation)). Ücret, Iş Ortağı Merkezi içindeki fiyat listesi sayfasında bulunabilir.

## <a name="what-azure-services-are-eligible-for-pec"></a>PEC için hangi Azure hizmetleri uygun?

PEC, CSP 'de (Azure plan) yeni Azure teklifiyle ilgili tüm hizmetler için aşağıdakiler hariç uygundur: 
- Yeni Azure teklifi (Azure plan) ayırmaları
- Azure plan tüketim fiyatı listesinin Etiketler sütununda üçüncü taraf olarak tanımlanan üçüncü taraf ürünleri
- Market fiyat listesindeki ürünler
- [Azure spot sanal makineleri](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

## <a name="where-can-i-see-pec"></a>PEC 'i nereden görebilirim?

Bkz. [Hesaplama](partner-earned-credit-explanation.md#calculation).

## <a name="where-can-i-find-pec-details"></a>PEC 'in ayrıntılarını nerede bulabilirim?

PEC ayrıntıları, iş ortakları tarafından doğrudan API, [günlük keşfi dosyası](partner-earned-credit-explanation.md#calculation) ve [ACM (Azure Cost MGMT)](partner-earned-credit-explanation.md#azure-cost-management-and-pec) ile sorgulanabilir.

## <a name="how-can-i-reconcile-my-pec-information-across-the-two-recon-files"></a>PEC bilgilerimi iki keşfi dosyası arasında nasıl mutabık hale getirebilirsiniz?

Iş Ortağı Merkezi 'nde, kullanılabilen Faturalandırma bölümünde iki karşılaştırma dosyası bulunur.

- Günlük dereceli kullanım mutabakatı-son etkinlik (.csv)
- Mutabakat-son etkinlik (.csv)

İş ortağı, mutabık kılmak için, her bir SubscriptionID için ProductID, SKUID, kullanılabilirlik, kullanılabilirliği ve bu iki dosya alanını karşılaştırabilir.

:::image type="content" source="images/advanced-specializations/partner-billing.png" alt-text="Yinelenen ve tek seferlik satın alımlarını vurgulayan Iş ortağı merkezi faturalama sekmesinin ekran görüntüsü." border="false":::

## <a name="for-an-indirect-reseller-working-with-an-indirect-provider-does-an-indirect-provider-need-to-add-the-indirect-resellers-account-as-an-rbac-identity-and-access-management-iam-role-to-the-end-customers-subscription-in-order-to-utilize-acm"></a>Dolaylı bir sağlayıcı ile çalışan dolaylı bir satıcı için, bir dolaylı sağlayıcının, ACM 'yi kullanmak için son müşterinin aboneliğine bir RBAC kimliği ve erişim yönetimi (ıAM) rolü olarak dolaylı satıcının hesabını eklemesi gerekir mi?

Evet, CSP dolaylı sağlayıcısı, Azure aboneliğindeki dolaylı satıcıya [RBAC](/azure/role-based-access-control/overview) erişimini etkinleştirmelidir.

## <a name="what-happens-if-a-customer-removes-a-partners-rbac-admin-access"></a>Bir müşteri ortağın RBAC yönetici erişimini kaldırdığında ne olur?

CSP 'de uygun RBAC erişimi olmayan bir iş ortağı, müşterinin Azure Faturalandırma ilişkisini ve Microsoft ile sorumlulukta kalmaya devam eder. Bu, önceki Azure teklifini CSP 'de satan bir ortağı etkilemekle karşı, CSP 'deki yeni Azure teklifi için faturalanmış iş ortağı Azure faturasında PEC için uygun olmayacaktır. İş ortakları, RBAC kullanarak veya Azure athouse aracılığıyla Dizin/konuk erişimi aracılığıyla bir kullanıcı hesabı aracılığıyla erişim sağlayarak CSP 'de kısmi yönetici erişimi elde edebilir. Daha fazla bilgi için bkz. [bir müşterinin Azure CSP abonelikleri için yeniden devreye sokma yönetici ayrıcalıkları](revoke-reinstate-csp.md).

:::image type="content" source="images/advanced-specializations/partner-permissions.png" alt-text="Yönetici izinlerini yeniden devreye geçirebileceğiniz erişim denetimi sayfasının ekran görüntüsü." border="false":::

## <a name="how-do-i-know-if-im-earning-pec"></a>Nasıl yaparım? PEC 'i kazandığımı mi biliyoruz?

Bir iş ortağının bir müşterinin Azure kaynaklarına uygun erişimi olduğunu doğrulayabilecekleri çeşitli yollar vardır.

- Günlük kullanım dosyasını gözden geçirin: bir iş ortağı yönetilen hizmetler için ortağın kazanıldığını alıyorsa, yönetici erişimine sahip olurlar. Bu, günlük kullanım dosyası dahilinde birim fiyat ve geçerli birim fiyatı inceleyerek ve bir iskontonun uygulanmakta olup olmadığını onaylayarak belirlenebilir.
- Azure Izleyici uyarısı oluşturma: RBAC Erişimleriniz CSP aboneliklerinden kaldırıldığında bildirimleri almak için Azure Izleyici 'yi kullanarak [etkinlik günlüğü uyarıları oluşturabilirsiniz](/azure/azure-monitor/platform/alerts-activity-log) . Lütfen Iş ortağı kazanılmış kredi kılavuzunu ve teknik belgeleri anlama bölümüne bakın.

## <a name="why-dont-i-see-pec-on-the-invoice"></a>Faturada PEC 'i neden görmüyorum?

PEC, faturada açıkça çağrılmaz ve PEC 'in görüntüleneceği ayrı bir satır öğesi yoktur, ancak PEC kazancı, faturada ayarlanan net ücret miktarına göre belirlenir. PEC 'in ayrıntılarını görüntüleyebileceğiniz hakkında daha fazla bilgi edinmek için hesaplamayı ve PEC 'in nasıl ücretli bölümlerini görüntüleyin.

## <a name="next-steps"></a>Sonraki adımlar

- [CSP 'de Azure için yeni ticari deneyim fiyat listesi](azure-plan-price-list.md)
- [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)
- [CSP'de yeni ticari deneyim - Azure faturalama](azure-plan-billing.md)
- [Azure CSP abonelikleri için yönetici ayrıcalıklarını yeniden devreye sokma](revoke-reinstate-csp.md)
- [İş ortağı kazanılmış kredi-genel bakış](partner-earned-credit.md)
- [Roller, iş ortağı kazanılmış kredi için izinler](azure-roles-perms-pec.md)
- [Iş ortağı kazanılmış krediyi anlama (kılavuz)](https://partner.microsoft.com/resources/detail/understanding-partner-earned-credit-pdf) (oturum açma gerekir)
