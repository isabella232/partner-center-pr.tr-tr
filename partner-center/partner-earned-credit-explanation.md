---
title: Yönetilen hizmetler için iş ortağı tarafından kazanılan kredi
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Yönetilen hizmetler için Microsoft iş ortağı tarafından kazanılan kredinin (PEC) nasıl hesaplanmış ve ücretli olduğunu ve uygun olduğundan emin olun.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: ba422a2feae2affb9c2b60ad345c4d6bb0d525c7
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110145873"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>İş ortağı kazanılmış kredisinin hesaplanması ve ödenmesi

**Uygun roller:** Genel yönetici | Kullanıcı yönetimi yönetici | Yönetici aracısı | Faturalama yöneticisi | Satış aracısı

Yönetilen hizmetler (PEC) için iş ortağı tarafından kazanılan kredi, müşterilerinin Azure ortamının tamamını veya parçalarının 7x24 IT operasyonel denetimine ve yönetimine sahip olan iş ortaklarını tanır ve ödüllendirir. CSP'de varsayılan olarak, iş ortaklarına müşterinin aboneliğinde gerekli erişim hakları ve ardından abonelikte 7/24 operasyonel yönetim ve denetim gerçekleştirmelerine olanak sağlar. Müşterilerin işlem ortakları için erişim sağlamanın diğer yolları aşağıdaki bölümde açıklanmıştır. Aylık fatura tutarı, iş ortağı tarafından kazanılan kredinin net tutarıdır. İş ortakları, aylık mutabakat dosyasında PEC ayrıntılarını görebilir. Müşterinin işlem ortağına erişim sağlamanın diğer yolları için Azure planı altındaki Abonelikleri [ve kaynakları yönetme makalelerini okuyun.](azure-plan-manage.md)

Ayrıca [abonelikler için yönetici ayrıcalıklarını yeniden Azure CSP okuyun](revoke-reinstate-csp.md)

## <a name="eligibility"></a>Uygunluk

İş ortağı tarafından kazanılan krediyi (PEC) almak için aşağıdaki gereksinimler geçerlidir: 

- Yönetmekte olduğu Azure varlıkları için kazanılan krediyi almak için etkin bir MPN sözleşmeniz ve geçerli rol tabanlı erişim denetimi (RBAC) rolünüz olmalıdır.

- CSP'de müşterinin Azure kaynaklarının 7x24 operasyonel denetimine ve yönetimine sahip olmak gerekir. Bu, müşterinin Azure aboneliği, Azure kaynak grubu ve Azure kaynağı üzerinde yönetici ayrıcalıklarına sahip olmanız gerektiğini gösterir. Dolaylı sağlayıcılar ve dolaylı kurumsal bayileri durumunda, dolaylı sağlayıcı veya dolaylı kurumsal bayi ya da her ikisi de bu işlem denetimine sahipse dolaylı sağlayıcı PEC için uygun olur. Bu konuda daha fazla bilgi edinmek için [bkz. Abonelikler için yönetici ayrıcalıklarını Azure CSP.](./revoke-reinstate-csp.md)

- PEC, yukarıdaki gereksinimlere ek olarak yalnızca Azure plan [fiyatlandırma](https://partner.microsoft.com/commerce/sales) sayfasından dışarı aktarmak için Azure plan tüketim fiyatlandırması 'nda listelenen hizmetlere uygulanabilir.

- PEC, aşağıdaki hizmetler için geçerli **değildir** :
    - Azure plan ayırmaları
    - Azure plan tüketim fiyatının Etiketler sütununda üçüncü taraf olarak tanımlanan üçüncü taraf ürünleri
    - Market fiyat listesindeki ürünler
    - [Azure spot sanal makineleri](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- PEC, Azure Kaynak düzeyine kadar kazanılmakta. Abonelik veya kaynak grubu düzeyinde geçerli erişiminiz varsa, daha yüksek varlığa kaydolan her kaynak PEC 'e kazanacaktır.

- PEC ile ilgili ayrıntılar için [Azure maliyet yönetimi](/azure/cost-management-billing/costs/get-started-partners) sayfasından da ulaşılabilir.

### <a name="calculation"></a>Hesaplama

PEC günlük olarak hesaplanır ve günlük kullanım dosyasında ve aylık fatura keşfi dosyasında görüntülenebilir. Bir iş ortağı (dolaylı sağlayıcı veya dolaylı satıcı), PEC kazanıdıklarından emin olmak için tüm gün (7/24) erişimi olmalıdır. PEC, yönetilen Azure varlıklarının her gün temelinde hesaplanır. İş ortakları ayda kalıcı ayrıcalıklı erişimi (erişim kapsamı) ve tüm uygun kaynakların (erişim kapsamı) tam PEC kazanmasına sahip olur. Kapsam ve yayılma azaltma, ay için daha düşük PEC oranına neden olur. Günlük olarak derecelendirilen kullanım dosyası, PEC 'in uygulanıp uygulanmadığı bir Azure varlığı üzerinde günlük olarak gösterilir. İş ortakları, kalıcı ayrıcalıklı erişimdeki değişiklikleri izlemek için uyarılara de kaydolabilir.

## <a name="azure-cost-management"></a>Azure Maliyet Yönetimi

Maliyet analizini kullanan Azure maliyet yönetimi (ACM), PEC 'in avantajını almış olan maliyetleri görüntülemek için bir iş ortağı olarak size olanak sağlar.  

1. [Azure Portal](https://portal.azure.com), iş ortağı kiracınızda oturum açın ve **maliyet yönetimi + faturalandırma**' i seçin.

2. **Maliyet yönetimi** Seç

3. **Maliyet analizini** seçin

   Maliyet Analizi görünümü, Microsoft'un ödemesi yapılan fiyatlarla satın alınan ve tüketilen tüm hizmetler için ödeme hesabınız için maliyetleri görüntüler.

4. PEC uygulanmış maliyetleri görmek için özet grafiğin açılan listesinde **PartnerEarnedCreditApplied** öğesini seçin. **PartnerEarnedCreditApplied** özelliği True olduğunda ilişkili maliyet, iş ortağı tarafından kazanılan kredinin avantajına sahip olur. 

   PartnerEarnedCreditApplied özelliği False olduğunda, ilişkili maliyet kredi için gerekli uygunluğu karşılamamış veya satın alınan hizmet iş ortağı tarafından kazanılan kredi için uygun değildir.

   >[!NOTE] 
   >Genellikle, hizmetlerin kullanımının Maliyet Yönetimi'ne görünmesi  8-24 saat sürer ve PEC kredilerinin erişimden itibaren 48 saat içinde Azure Maliyet Yönetimi.

5. PEC'e ve PEC uygulanmamış maliyetlere detaya gitme için  Grupla ve Filtre özellikleri ekle'yi kullanarak **PartnerEarnedCreditApplied** özelliğine göre de gruplandırabilirsiniz.

## <a name="next-steps"></a>Sonraki adımlar

- [İş ortağı tarafından kazanılan kredi - genel bakış](partner-earned-credit.md)

- İş ortağı tarafından kazanılan kredi hesaplamalarının ayrıntılı örnekleri, İş Ortağı Merkezi panosu aracılığıyla ulaşabilirsiniz fiyat listesinde bulunur (oturum açma gerekir).

- [Azure planına taşıma - çalışmaya başlama](azure-plan-get-started.md)

- [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)

- [Abonelikler için yönetici ayrıcalıklarını iptal Azure CSP yeniden iade etme](revoke-reinstate-csp.md)
