---
title: İş ortağı tarafından kazanılan kredi hakkında SSS
ms.topic: article
ms.date: 07/22/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: İş ortağı tarafından kazanılan kredi (PEC) ile ilgili sık sorulan soruların yanıtlarını bulun.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: e5d6aa77a02a24648828f06fb2c56640abdbfc56
ms.sourcegitcommit: d133c8b923b90ac5518cb989c0ce4dd69713abf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/22/2021
ms.locfileid: "114434226"
---
# <a name="frequently-asked-questions-for-partner-earned-credit"></a>İş ortağı tarafından kazanılan kredi için sık sorulan sorular

Uygun roller: Genel yönetici | Kullanıcı yönetimi yönetici | Yönetici aracısı | Faturalama yöneticisi | Satış aracısı

Aşağıda, iş ortağı tarafından kazanılmış krediyle ilgili sık sorulan soruların bir listesi ve ardından ve ardından gelir.

## <a name="how-much-is-pec"></a>PEC ne kadardır?

İş ortaklarının PEC için kazandığı miktar farklılık gösterir (bkz. [Hesaplama).](partner-earned-credit-explanation.md#calculation) Fiyat, fiyat listesi sayfasındaki fiyat listesi sayfasında İş Ortağı Merkezi.

## <a name="what-azure-services-are-eligible-for-pec"></a>Hangi Azure hizmetleri PEC için uygun?

PEC, CSP'de (Azure planı) yeni Azure teklifiyle ilgili aşağıdakiler dışında tüm hizmetler için uygundur: 
- Yeni Azure teklifi (Azure planı) rezervasyonları
- Azure planı tüketim fiyatı listesinin Etiketler sütununda Üçüncü Taraf olarak tanımlanan üçüncü taraf ürünleri
- Market fiyat listesinde yer alan ürünler
- [Azure Spot Sanal Makineler](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

## <a name="where-can-i-see-pec"></a>PEC'i nerede görebilirim?

Bkz. [Hesaplama.](partner-earned-credit-explanation.md#calculation)

## <a name="where-can-i-find-pec-details"></a>PEC ayrıntılarını nerede bulamıyorum?

PEC ayrıntıları doğrudan iş ortakları tarafından API, [günlük keşif](partner-earned-credit-explanation.md#calculation) dosyası ve [ACM (Azure Maliyet Mgmt)](partner-earned-credit-explanation.md#azure-cost-management-and-pec) tarafından sorguilebilir.

## <a name="how-can-i-reconcile-my-pec-information-across-the-two-recon-files"></a>İki mutabakat dosyası arasında PEC bilgilerimi nasıl mu mutabakata varabilirsiniz?

Faturalama'nın altında bulunan İş Ortağı Merkezi iki mutabakat dosyası bulunur.

- Günlük puanlanan kullanım mutabakatı-son etkinlik (.csv)
- Mutabakat-son etkinlik (.csv)

Mutabık olmak için iş ortağı her SubscriptionID için bu iki dosyadan ProductID, SKUID ve AvailabilityID alanlarını karşılaştırabilirsiniz.

## <a name="for-an-indirect-reseller-working-with-an-indirect-provider-does-an-indirect-provider-need-to-add-the-indirect-resellers-account-as-an-rbac-identity-and-access-management-iam-role-to-the-end-customers-subscription-in-order-to-utilize-acm"></a>Dolaylı Sağlayıcı ile çalışan Dolaylı Kurumsal Bayilerde, ACM'yi kullanabilmek için Dolaylı Sağlayıcının dolaylı kurumsal bayinin hesabını son müşterinin aboneliğine RBAC Kimlik ve Erişim Yönetimi (IAM) rolü olarak eklemesi gerekir mi?

Evet, CSP Indirect Provider Azure aboneliği üzerinde Dolaylı Kurumsal Bayi'ye [RBAC](/azure/role-based-access-control/overview) erişimini etkinleştirmesi gerekir.

## <a name="what-happens-if-a-customer-removes-a-partners-rbac-admin-access"></a>Müşteri iş ortağının RBAC yönetici erişimini kaldırırsa ne olur?

CSP'de uygun RBAC erişimi olmayan bir iş ortağı, müşterinin Azure faturalama ilişkisini ve Microsoft ile sorumluluklarını korur. Bu, CSP'de önceki Azure teklifini satan bir iş ortağını etkilemese de, CSP'de yeni Azure teklifi için faturalanmış iş ortağı, Azure faturalarında PEC için uygun olmayacaktır. İş ortakları, RBAC kullanarak Dizin/Konuk erişimi aracılığıyla bir kullanıcı hesabı üzerinden veya sanal ağ üzerinden erişim elde etmek yoluyla CSP'de kısmi yönetici Azure Lighthouse. Daha fazla bilgi için [bkz. Müşterinin abonelikleri için yönetici ayrıcalıklarını Azure CSP.](revoke-reinstate-csp.md)

## <a name="how-do-i-know-if-im-earning-pec"></a>Nasıl yaparım? PEC kazancım olduğunu biliyor musunuz?

bir iş ortağının müşterinin Azure kaynaklarına uygun erişime sahip olduğunu onaylamanın birkaç yolu vardır.

- Günlük kullanım dosyasını gözden geçirme: Bir iş ortağı Yönetilen Hizmetler için İş Ortağı Tarafından Kazanılan Krediyi alıyorsa yönetici erişimine sahip olur. Bu, günlük kullanım dosyasındaki birim fiyatı ve geçerli birim fiyatı gözden geçirerek ve indirim uygulanıyorsa onay ile belirlenebilirsiniz.
- Özel Azure İzleyici oluşturma: CSP [](/azure/azure-monitor/platform/alerts-activity-log) aboneliklerinden RBAC Azure İzleyici kaldırıldığı zaman bildirim almak için Azure İzleyici kullanarak etkinlik günlüğü uyarıları oluşturabilirsiniz. İş Ortağı Tarafından Kazanılan Krediyi Anlama kılavuzuna ve teknik belgelere bakın.

## <a name="why-dont-i-see-pec-on-the-invoice"></a>Neden faturada PEC göremiyorum?

PEC açıkça faturada çağrılmaz ve PEC'i görüntülemek için ayrı bir satır öğesi yoktur, ancak PEC kazançları faturada ayarlanmış net ücretler tutarına dahil olur. PEC ayrıntılarını nerede görüntüleyebilirsiniz hakkında daha fazla bilgi edinmek için hesaplamayı ve PEC ücretli bölümlerini görüntüleme.

## <a name="next-steps"></a>Sonraki adımlar

- [Yeni ticari deneyim için fiyat listesi CSP'de Azure](azure-plan-price-list.md)
- [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)
- [CSP'de yeni ticari deneyim - Azure faturalama](azure-plan-billing.md)
- [Azure CSP abonelikleri için yönetici ayrıcalıklarını yeniden devreye sokma](revoke-reinstate-csp.md)
- [İş ortağı tarafından kazanılan kredi - genel bakış](partner-earned-credit.md)
- [Roller, iş ortağı tarafından kazanılan kredi izinleri](azure-roles-perms-pec.md)
- [İş Ortağı Tarafından Kazanılan Krediyi Anlama (kılavuz)](https://partner.microsoft.com/resources/detail/understanding-partner-earned-credit-pdf) (oturum açma gereklidir)
