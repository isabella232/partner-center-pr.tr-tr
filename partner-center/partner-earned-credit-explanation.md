---
title: Yönetilen hizmetler için iş ortağı kazanılmış kredisi
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Yönetilen hizmetler için Microsoft iş ortağı kredisi (PEC) nasıl hesaplanacağını ve ödendiğini ve uygun şekilde nasıl emin olduğunuzu öğrenin.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 3acc078b3de3c0443ee64fdaaba2d486d9c466c8
ms.sourcegitcommit: e9066768ab8e242c03f0a7e3ce460ae8cd2e3fda
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/17/2020
ms.locfileid: "97622176"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>İş ortağı kazanılmış kredisinin hesaplanması ve ödenmesi

**Uygun roller**

- Genel yönetici
- Kullanıcı yöneticisi
- Yönetim Aracısı
- Faturalama yöneticisi
- Satış Aracısı

Yönetilen hizmetler (PEC) için iş ortağı kazanılmış kredisi, müşterilerine 7/24 BT işletimsel denetim ve bunların bölümlerinin yönetimi ve müşterilerinin tüm Azure ortamı gibi iş ortaklarını tanır ve depolar. Varsayılan olarak, CSP 'de iş ortaklarına, aboneliğin abonelik üzerinde 24 X 7 işlemsel yönetim ve denetim gerçekleştirmesine izin veren, müşterinin aboneliğine gerekli erişim hakları verilir. Müşterinin deneyimidir iş ortağı için erişim sağlayabildiği diğer yollar aşağıdaki bölümde açıklanmıştır. Aylık fatura tutarı, iş ortağının kazandığı net kredi tutarıdır. İş ortakları, aylık keşfi dosyasında PEC ayrıntılarını görebilir. Müşterinin deneyimidir iş ortağı için erişim sağlayabildiği ek yollar için, [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)makalesini okuyun.

Ayrıca, [Azure CSP abonelikleri için yeniden devreye sokma yönetici ayrıcalıklarını](revoke-reinstate-csp.md) oku

## <a name="eligibility"></a>Önceliği

İş ortağı kazanılmış kredisi (PEC) almak için aşağıdaki gereksinimler geçerlidir: 

- Yönettiğiniz Azure varlıklarının kazanıldığını alacak bir etkin MPN anlaşmanız ve geçerli rol tabanlı erişim denetimi (RBAC) rolüne sahip olmanız gerekir.

- CSP 'de müşterinin Azure kaynaklarını 7/24 işletimsel denetim ve yönetimine sahip olmanız gerekir. Bu, müşterinin Azure aboneliği, Azure Kaynak grubu, Azure kaynağı üzerinde yönetici ayrıcalıklarına sahip olmanız gerektiği anlamına gelir. Dolaylı sağlayıcılar ve dolaylı satıcıları söz konusu olduğunda, dolaylı sağlayıcı veya dolaylı satıcı ya da her ikisinin de bu işlemsel denetimi varsa, dolaylı sağlayıcı PEC 'e uygun olacaktır. Bunun hakkında daha fazla bilgi edinmek için bkz. [Azure CSP abonelikleri için yeniden devreye alma yönetici ayrıcalıkları](https://docs.microsoft.com/partner-center/revoke-reinstate-csp).

- PEC, yukarıdaki gereksinimlere ek olarak yalnızca Azure plan [fiyatlandırma](https://partner.microsoft.com/commerce/sales) sayfasından dışarı aktarmak için Azure plan tüketim fiyatlandırması 'nda listelenen hizmetlere uygulanabilir.

- PEC, aşağıdaki hizmetler için geçerli **değildir** :
    - Azure plan ayırmaları
    - Azure plan tüketim fiyatının Etiketler sütununda üçüncü taraf olarak tanımlanan üçüncü taraf ürünleri
    - Market fiyat listesindeki ürünler
    - [Azure spot sanal makineleri](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- PEC, Azure Kaynak düzeyine kadar kazanılmakta. Abonelik veya kaynak grubu düzeyinde geçerli erişiminiz varsa, daha yüksek varlığa kaydolan her kaynak PEC 'e kazanacaktır.

- PEC ile ilgili ayrıntılar için [Azure maliyet yönetimi](https://docs.microsoft.com/azure/cost-management-billing/costs/get-started-partners) sayfasından da ulaşılabilir.

### <a name="calculation"></a>Hesaplama

PEC günlük olarak hesaplanır ve günlük kullanım dosyasında ve aylık fatura keşfi dosyasında görüntülenebilir. Bir iş ortağı (dolaylı sağlayıcı veya dolaylı satıcı), PEC kazanıdıklarından emin olmak için tüm gün (7/24) erişimi olmalıdır. PEC, yönetilen Azure varlıklarının her gün temelinde hesaplanır. Belirli bir fatura dönemi için maksimum PEC (ay) %15 ' tir. İş ortakları ay (erişim kapsamı) ile kalıcı ayrıcalıklı erişimi korur ve tüm uygun kaynaklar (erişim kapsamı) için tam PEC %15 kazanacaktır. Kapsam ve yayılma azaltma, ay için daha düşük PEC oranına neden olur. Günlük olarak derecelendirilen kullanım dosyası, PEC 'in uygulanıp uygulanmadığı bir Azure varlığı üzerinde günlük olarak gösterilir. İş ortakları, kalıcı ayrıcalıklı erişimdeki değişiklikleri izlemek için uyarılara de kaydolabilir.

## <a name="azure-cost-management"></a>Azure Maliyet Yönetimi

Maliyet analizini kullanan Azure maliyet yönetimi (ACM), PEC 'in avantajını almış olan maliyetleri görüntülemek için bir iş ortağı olarak size olanak sağlar.  

1. [Azure Portal](https://portal.azure.com), iş ortağı kiracınızda oturum açın ve **maliyet yönetimi + faturalandırma**' i seçin.

2. **Maliyet yönetimi** Seç

3. **Maliyet analizini** seçin

   Maliyet analizi görünümü, satın alınan ve Microsoft 'a ödediğiniz fiyatlarla tüketilen tüm hizmetler için faturalandırma hesabınızın maliyetlerini görüntüler.

4. PEC 'in uygulandığı maliyetleri görmek için bir Özet grafiğinde açılan kutuda **Partnerearnedtappnda** ' u seçin. **Partnerearnedkredtappekonomi** özelliği true olduğunda, ilişkili maliyet iş ortağının kazanılan kredisi avantajına sahiptir. 

   Partnertatnedkredtappekonomi özelliği false olduğunda, ilişkili maliyet kredi için gereken uygunluğu karşılamıyor veya satın alınan hizmet, iş ortağı tarafından kazanılan kredi için uygun değil.

   >[!NOTE] 
   >Genellikle, hizmetler için kullanım **Maliyet yönetiminde** 8-24 saat sürer ve Pec kredileri, Azure maliyet yönetimi 'nde erişim zamanından itibaren 48 saat içinde görünür.

5. Ayrıca, **Grup ölçütü** ' ne göre gruplandırma yapabilir ve filtreleme özellikleri **ekleyerek, PEC** 'e ve Pec uygulanmamış maliyetlere sahip olan maliyetlerde detaya gitme özelliği ekleyebilirsiniz.

## <a name="next-steps"></a>Sonraki adımlar

- [İş ortağı kazanılmış kredi-genel bakış](partner-earned-credit.md)

- İş ortağı kazanılmış kredi hesaplamalarının ayrıntılı örnekleri, Iş Ortağı Merkezi panosu (oturum açma gerekir) aracılığıyla ulaşabileceğiniz fiyat listesinde bulunur.

- [Azure planına taşıma-kullanmaya başlama](azure-plan-get-started.md)

- [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)

- [Azure CSP abonelikleri için yönetici ayrıcalıklarını iptal etme veya yeniden alma](revoke-reinstate-csp.md)
