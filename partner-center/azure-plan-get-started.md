---
title: Azure planına taşımaya başlama
description: İlk adımlar, güvenlik önlemleri ve kullanmaya başlama dahil olmak üzere, sizin ve müşterileriniz için Azure kullandırılan ödeme planını kullanma hakkında neleri öğrenmeniz gerekir?
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: amitravat
ms.author: amrava
ms.custom: SEOAPR.20
ms.localizationpriority: High
ms.date: 12/02/2019
ms.openlocfilehash: ca7b72e653af37307d3a2985ac57783b050ff408204a14d977ec7a5ec29dab77
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115691234"
---
# <a name="begin-using-pay-as-you-go-rates-with-the-azure-plan"></a>Azure planıyla kullansanız öde ücretlerini kullanmaya başlama

**Uygun roller:** Yönetici aracısı | Satış aracısı


Microsoft, yeni bir ticari deneyim İş Ortağı Merkezi.  Bu yeni ticaret deneyimiyle iş ortakları, azure hizmetleri için uygun fiyat kapsamındaki müşteriler için azure Microsoft Müşteri Sözleşmesi.

Bu plan satın alma deneyimini basitleştiriyor. Bir Azure planında birden çok Azure aboneliğiniz olabilir. Artık Azure aboneliği başına ayrı bir sipariş göndermeniz gerekmeyecek. Azure için bu yeni ticaret deneyiminde, CSP iş ortaklarının Yayımlanan fiyatlarda Azure'a teklif sunmalarına olanak sağlayan tek bir küresel fiyatlandırma ilkesine uygun hareket ettik.

Müşterilerimizin dijital dönüşüm ihtiyaçları, iş ortaklarının yeni becerilere ihtiyacı vardır. Birçok müşteri, bulut yolculuğunu daha sorunsuz hale getirir ve Azure hizmetlerini verimli bir şekilde tüketmeye yardımcı olmak için iş ortaklarının işlemlerin üzerinde ve ötesinde hizmet sağlamalarını sağlar. Microsoft iş ortakları, müşteri yaşam döngüsünün tüm aşamalarında kritik bir rol oynar. Bu tür iş ortağı hizmetleri doğası gereği devam ediyor ve Azure emlak izleme, ilke ve idare yönetimi, ayarlama ve yapılandırmada ince ayarlama, teknik destek ve diğer birçok farklı hizmeti içerir. Bir iş ortağının müşterinin Azure ortamı hakkında bilgi sahibi olması ve yönetecekleri temel kaynakların sürekli ve uygun idare ve denetimine sahip olması gerekir. Bu 24 X 7 bulut operasyonları yönetimini sağlayan faturalama iş ortakları, bu iş için yönetilen hizmetler için İş ortağı tarafından kazanılan **kredi** için uygun hale gelir.

## <a name="make-sure-your-customers-have-signed-the-microsoft-customer-agreement"></a>Müşterileriniz tarafından imzalanmış olduğundan emin Microsoft Müşteri Sözleşmesi

1 Ekim 2019'dan bu yana, Microsoft Müşteri Sözleşmesi tamamen dijital bir süreçle müşteri satın alma deneyimini basitleştiren ve kolaylaştıran kalıcı bir sözleşme olan Microsoft Müşteri Sözleşmesi, kullanılabilir. Azure için CSP'de yeni ticari deneyimden yararlanmak isteyen tüm müşterilerin bu hizmeti Microsoft Müşteri Sözleşmesi.

Yeni Azure planı kapsamında işlem yapmak ve yeni bir sipariş almak isteyen iş ortaklarının üretimde Microsoft Müşteri Sözleşmesi api'sini ve İş Ortağı Merkezi müşteri kabulünü onaylaması gerekir.

1 Şubat 2020'den başlayarak, Microsoft Bulut Anlaşması CSP programından kaldırılır. O zaman, Microsoft 365, Dynamics 365 ve mevcut Azure dahil olmak üzere yeni Microsoft Müşteri Sözleşmesi için iş ortağı onayı (onay) gerekli olacak. CSP'de iş ortakları, iş ortaklarının müşteri için yeni bir siparişte Microsoft Müşteri Sözleşmesi.

Tüm ayrıntılar için müşterinin kabul [etme işlemini onaylama Microsoft Müşteri Sözleşmesi](confirm-customer-agreement.md)

## <a name="security-and-access-control-practices"></a>Güvenlik ve erişim denetimi uygulamaları

İş ortaklarının ve müşterilerin korunmasına yardımcı olmak için Danışmanlar, Denetim Masası Satıcıları ve Bulut Çözümü Sağlayıcısı programa katılan iş ortakları için bir dizi zorunlu güvenlik Bulut Çözümü Sağlayıcısı sunuyoruz.

Zorunlu güvenlik gereksinimlerini uygulamayan iş ortakları, bu gereksinimler zorunlu kılınan Bulut Çözümü Sağlayıcısı yönetici haklarıyla müşteri kiracılarını yönetememektedir. Gereksinimler için bir teknik uygulama tarihi belirlenmektedir ve iş ortaklarına ayrıntılı bilgilerle tarihi bildireceğiz.

## <a name="actions-to-take-to-implement-mfa"></a>MFA uygulamak için uygulanması gereken eylemler

İş ortağı olmanın yüksek ayrıcalıklı doğasına göre her kullanıcının her bir kimlik doğrulamasında MFA zor olduğundan emin olmak gerekir. Bu, aşağıdaki yöntemlerden biri aracılığıyla gerçek olabilir:

- Uygulama Azure AD Premium ve her kullanıcı için çok faktörlü kimlik doğrulamasının (MFA) zorunlu tutul olduğundan emin olmak
- [Azure AD güvenlik varsayılanlarını uygulama](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- Üçüncü taraf çözümü uygulama ve her kullanıcı için MFA'nın zorunlu tutul olduğundan emin olmak

1 Ağustos 2019'dan başlayarak, tüm iş ortaklarının iş ortağı kiracılarında hizmet hesapları da dahil olmak üzere tüm kullanıcılar için çok faktörlü kimlik doğrulamasını zorlaması gerekir. Bu güvenlik gereksinimleri hakkında ayrıntılı bilgi İş ortağı güvenlik gereksinimleri [altında bulunabilir.](partner-security-requirements.md)

Microsoft, iş ortaklarının kaynakları aracılığıyla etkinleştiren en iyi yöntemleri kullanarak RBAC'yi dikkatli [Azure Active Directory Privileged Identity Management öneririz.](/azure/active-directory/privileged-identity-management/pim-configure)

## <a name="read-more-about-the-azure-plan"></a>Azure planı hakkında daha fazla bilgi edinin

- [Azure planı satın alma](purchase-azure-plan.md)

- [Azure tekliflerini karşılaştırma](compare-azure-offers.md)

- [İş ortağı tarafından kazanılan kredi - genel bakış](partner-earned-credit.md)

- İş ortağı tarafından kazanılan kredi (PEC) hesaplamaları ve iş ortağı tarafından kazanılmış kredileri almaya uygun roller ve izinler İş Ortağı Merkezi Panosu fiyat listesinden (oturum açma gereklidir) kullanılabilir.

## <a name="next-steps"></a>Sonraki adımlar 

- [İş ortağı tarafından kazanılan kredi nasıl belirlenir? - ayrıntılar](partner-earned-credit-explanation.md)
- [Azure planı fiyat listesi açıklandı](azure-plan-price-list.md)
- [Müşterinizi Azure planına geçirin](azure-plan-transition.md)
- [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)
- [Azure planının kullanılabilir olduğu ülkelerin/bölgelerin tam listesi](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x)