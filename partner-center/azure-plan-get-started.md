---
title: Azure planına taşımaya başlama
description: İlk adımlar, güvenlik önlemleri ve kullanmaya başlama dahil olmak üzere, sizin ve müşterileriniz için Azure kullandırılan ödeme planını kullanma hakkında neleri öğrenmeniz gerekir?
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.custom: SEOAPR.20
ms.localizationpriority: High
ms.date: 12/02/2019
ms.openlocfilehash: 58feabdefb02660559c69f61190070310768b947
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149664"
---
# <a name="begin-using-pay-as-you-go-rates-with-the-azure-plan"></a>Azure planıyla kullansanız öde ücretlerini kullanmaya başlama

**Uygun roller:** Yönetici aracısı | Satış aracısı


Microsoft, yeni bir ticari deneyim İş Ortağı Merkezi.  Bu yeni ticaret deneyimiyle iş ortakları, azure hizmetleri için uygun fiyat kapsamındaki müşteriler için azure Microsoft Müşteri Sözleşmesi.

Bu plan satın alma deneyimini basitleştiriyor. Bir Azure planında birden çok Azure aboneliğiniz olabilir. Artık Azure aboneliği başına ayrı bir sipariş göndermeniz gerekmeyecek. Azure için bu yeni ticaret deneyiminde, CSP iş ortaklarının Yayımlanan fiyatlarda Azure'a teklif sunmalarını sağlayan tek bir genel fiyatlandırma ilkesine uygun hareket ettik.

Müşterilerimizin dijital dönüşüm ihtiyaçları, iş ortaklarının yeni becerilere ihtiyacı vardır. Birçok müşteri, bulut yolculuğunu daha sorunsuz hale getirir ve Azure hizmetlerini verimli bir şekilde tüketmeye yardımcı olmak için iş ortaklarının işlemlerin üzerinde ve ötesinde hizmetler sağlamalarını sağlar. Microsoft iş ortakları, müşteri yaşam döngüsünün tüm aşamalarında kritik bir rol oynar. Bu tür iş ortağı hizmetleri doğası gereği devam ediyor ve Azure emlak izleme, ilke ve idare yönetimi, ayarlama ve yapılandırmada ince ayarlama, teknik destek ve diğer birçok farklı hizmeti içerir. Bir iş ortağının müşterinin Azure ortamı hakkında bilgi sahibi olması ve yönetecekleri temel kaynakların sürekli ve uygun idare ve denetimine sahip olması gerekir. Bu 24 X 7 bulut operasyonları yönetimini sağlayan faturalama iş ortakları, bu iş için yönetilen hizmetler için İş ortağı tarafından kazanılan **kredi** için uygun hale gelir.

## <a name="make-sure-your-customers-have-signed-the-microsoft-customer-agreement"></a>Müşterileriniz tarafından imzalanmış olduğundan emin Microsoft Müşteri Sözleşmesi

1 Ekim 2019 ' den itibaren, tam dijital işlemle müşteri satın alma deneyimini kolaylaştıran ve basitleştiren bir kalıcı anlaşma olan Microsoft Müşteri Sözleşmesi, kullanılabilir. Azure için CSP 'deki yeni ticari deneyimden yararlanmak isteyen tüm müşterilerin Microsoft Müşteri sözleşmesini imzalaması gerekir.

Yeni Azure planı altında Transact ve yeni bir sipariş oluşturmak isteyen iş ortakları, Iş Ortağı Merkezi panosunu ve üretimde API 'YI kullanarak Microsoft Müşteri sözleşmesinin müşteri kabul edildiğini onaylamanız gerekir.

1 Şubat 2020 ' den itibaren, mevcut Microsoft Bulut sözleşmesi CSP programından kaldırılır. Bu süre içinde, yeni Microsoft Müşteri Sözleşmesi için müşteri kabulünün iş ortağı onayı (kanıtlama), Microsoft 365, Dynamics 365 ve mevcut Azure gibi diğer tüm teklifler için de gereklidir. CSP 'deki iş ortakları, Microsoft Müşteri sözleşmesinin kanıtı olmadan müşteri için yeni bir sipariş oluşturamayacak.

Tüm ayrıntılar için, [Microsoft Müşteri sözleşmesinin müşteri kabulünü Onayla](confirm-customer-agreement.md) konusunu okuyun

## <a name="security-and-access-control-practices"></a>Güvenlik ve erişim denetimi uygulamaları

İş ortaklarının ve müşterilerin korunmasına yardımcı olmak için, danışmanları, Denetim Masası satıcıları ve bulut çözümü sağlayıcısı programına katılan iş ortakları için bir dizi zorunlu güvenlik gereksinimi sunuyoruz.

Zorunlu güvenlik gereksinimlerini uygulamayan iş ortakları, bu gereksinimler zorlandıktan sonra bulut çözümü sağlayıcısı programında Transact veya temsilci yönetici haklarıyla bir müşteri kiracıları yönetemez. Gereksinimler için teknik zorlama tarihi oluşturma sürecimiz ve bilgileri, ayrıntılı bilgilerle ilgili olarak iş ortakları bilgilendirdirecek.

## <a name="actions-to-take-to-implement-mfa"></a>MFA 'yı uygulamak için gerçekleştirilecek eylemler

Her bir kullanıcının her bir tek kimlik doğrulaması için MFA sınamasına sahip olması açısından, iş ortağı olmak üzere yüksek ayrıcalıklı bir iş ortağı olarak verilmiştir. Bu, aşağıdaki yollarla gerçekleştirilebilir:

- Azure AD Premium uygulama ve Multi-Factor Authentication 'ın (MFA) her kullanıcı için zorlandığından emin olun
- [Azure AD güvenlik varsayılanlarını](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults) uygulama
- Bir üçüncü taraf çözümü uygulama ve MFA 'nın her kullanıcı için zorlanmasını sağlamak

1 Ağustos 2019 ' den itibaren, tüm iş ortakları, hizmet hesapları da dahil olmak üzere tüm kullanıcılar için iş ortağı kiracılarında Multi-Factor Authentication 'ı zorlamak için gereklidir. Bu güvenlik gereksinimleriyle ilgili ayrıntılı bilgiler, [Iş ortağı güvenlik gereksinimleri](partner-security-requirements.md)' nde bulunabilir.

Microsoft, [Azure Active Directory Privileged Identity Management kaynakları](/azure/active-directory/privileged-identity-management/pim-configure)aracılığıyla etkinleştirilen en iyi uygulamaları takip eden iş ortaklarının RBAC ile kullanımını öneriyor.

## <a name="read-more-about-the-azure-plan"></a>Azure planı hakkında daha fazla bilgi edinin

- [Azure planı satın alma](purchase-azure-plan.md)

- [Azure tekliflerini karşılaştırma](compare-azure-offers.md)

- [İş ortağı kazanılmış kredi-genel bakış](partner-earned-credit.md)

- İş ortağı kazanılmış kredi (PEC) hesaplamaları ve iş ortağı kazanılan kredilerin kazanılabilecek roller ve izinler, Iş Ortağı Merkezi Pano fiyat listenizden (oturum açma gerekir) alınabilir.

## <a name="next-steps"></a>Sonraki adımlar 

- [Ortağın kazanıldığı kredi nasıl belirlenir-Ayrıntılar](partner-earned-credit-explanation.md)
- [Azure planı fiyat listesi açıklanıyor](azure-plan-price-list.md)
- [Müşterinizi Azure planına geçirin](azure-plan-transition.md)
- [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)
- [Azure planının kullanılabildiği ülkelerin/bölgelerin tam listesi](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x)