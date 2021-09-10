---
title: Azure planına taşımaya başlayın
description: İlk adımlar, güvenlik önlemleri ve nasıl çalışmaya başladıklarını dahil olmak üzere Azure Kullandıkça Öde planını kullanma hakkında bilgi edinmek için sizin ve müşterilerinizin ne olduğunu öğrenin.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: amitravat
ms.author: amrava
ms.custom: SEOAPR.20
ms.localizationpriority: High
ms.date: 12/02/2019
ms.openlocfilehash: 40bf84ed47c946b84f511693d9f8351b3ffa5a95
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961074"
---
# <a name="begin-using-pay-as-you-go-rates-with-the-azure-plan"></a>Azure planıyla Kullandıkça Öde tarifesine kadar kullanmaya başlayın

**Uygun roller**: yönetici Aracısı | Satış Aracısı


Microsoft, Iş Ortağı Merkezi 'nde yeni bir ticari deneyim sunmuştur.  Bu yeni ticaret deneyimiyle, iş ortakları, Microsoft Müşteri anlaşmasındaki müşterilere yönelik Kullandıkça Öde tarifelerine göre Azure hizmetlerine erişim kazanacaktır.

Bu plan, satın alma deneyimini basitleştirir; bir Azure planında birden çok Azure aboneliğine sahip olabilirsiniz. Artık Azure aboneliği başına ayrı bir sıra göndermeniz gerekmez. Azure için sunulan bu yeni ticaret deneyiminde, CSP iş ortaklarının yayımlanan fiyatlarla Azure 'u sunmasına olanak tanıyan tek bir küresel fiyatlandırma ilkesine göre hizalandık.

Müşterilerimizin dijital dönüştürme gereksinimi, iş ortaklarından yeni yetenekler gerektirir. Birçok müşteri, bulut yolculuğunun daha sorunsuz hale getirme ve Azure hizmetlerini verimli bir şekilde kullanmanıza yardımcı olmak için iş ortaklarının üzerinde hizmet ve işlem işlemlerini daha iyi kullanmasını sağlar. Microsoft iş ortakları, müşteri yaşam döngüsünün tüm aşamalarında kritik bir rol oynar. Bu tür iş ortağı hizmetleri, yerleşik olarak bulunur ve Azure 'da izleme, ilke ve idare yönetimi, ince ayar yapma ve yapılandırma, teknik destek ve diğer çeşitli hizmetleri içerir. Müşterilerin, müşterinin Azure ortamına içkin hakkında bilgi sahibi olmaları ve yönettikleri temel kaynakların sürekli ve uygun yönetimi ve denetimi olması gerekir. Bu 24 X 7 bulut-işlem yönetimini sağlayan faturalandırma ortakları, bu iş için **yönetilen hizmetler için bir Iş ortağı tarafından kazanılan kredi** için uygun hale gelir.

## <a name="make-sure-your-customers-have-signed-the-microsoft-customer-agreement"></a>Müşterilerinizin Microsoft Müşteri sözleşmesinin imzalandığından emin olun

1 Ekim 2019 ' den itibaren, tam dijital işlemle müşteri satın alma deneyimini kolaylaştıran ve basitleştiren bir kalıcı anlaşma olan Microsoft Müşteri Sözleşmesi, kullanılabilir. Azure için CSP 'deki yeni ticari deneyimden yararlanmak isteyen tüm müşterilerin Microsoft Müşteri sözleşmesini imzalaması gerekir.

Yeni Azure planı altında Transact ve yeni bir sipariş oluşturmak isteyen iş ortakları, Iş Ortağı Merkezi panosunu ve üretimde API 'YI kullanarak Microsoft Müşteri sözleşmesinin müşteri kabul edildiğini onaylamanız gerekir.

1 Şubat 2020 ' den itibaren, mevcut Microsoft Bulut sözleşmesi CSP programından kaldırılır. bu süre içinde, yeni Microsoft müşteri sözleşmesi için müşteri kabulünün iş ortağı onayı (kanıtlama), Microsoft 365, Dynamics 365 ve mevcut Azure gibi diğer tüm teklifler için de gereklidir. CSP 'deki iş ortakları, Microsoft Müşteri sözleşmesinin kanıtı olmadan müşteri için yeni bir sipariş oluşturamayacak.

Tüm ayrıntılar için, [Microsoft Müşteri sözleşmesinin müşteri kabulünü Onayla](confirm-customer-agreement.md) konusunu okuyun

## <a name="security-and-access-control-practices"></a>Güvenlik ve erişim denetimi uygulamaları

iş ortaklarının ve müşterilerin korunmasına yardımcı olmak için, danışmanları, denetim masası satıcıları ve Bulut Çözümü Sağlayıcısı programına katılan iş ortakları için bir zorunlu güvenlik gereksinimleri kümesi sunuyoruz.

zorunlu güvenlik gereksinimlerini uygulamayan iş ortakları, bu gereksinimler zorlandıktan sonra Bulut Çözümü Sağlayıcısı programda transact veya temsilci yönetici haklarıyla bir müşteri kiracılarını yönetemez. Gereksinimler için teknik zorlama tarihi oluşturma sürecimiz ve bilgileri, ayrıntılı bilgilerle ilgili olarak iş ortakları bilgilendirdirecek.

## <a name="actions-to-take-to-implement-mfa"></a>MFA 'yı uygulamak için gerçekleştirilecek eylemler

Her bir kullanıcının her bir tek kimlik doğrulaması için MFA sınamasına sahip olması açısından, iş ortağı olmak üzere yüksek ayrıcalıklı bir iş ortağı olarak verilmiştir. Bu, aşağıdaki yollarla gerçekleştirilebilir:

- Azure AD Premium uygulama ve multi-factor authentication 'ın (MFA) her kullanıcı için zorlandığından emin olun
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