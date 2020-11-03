---
title: Yönetilen hizmetler için iş ortağı kazanılmış kredisi
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Yönetilen hizmetler için Microsoft iş ortağı kredisi (PEC) nasıl hesaplanacağını ve ödendiğini ve uygun şekilde nasıl emin olduğunuzu öğrenin.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 89fce612d5756da3f9674d4170ac8c0c3a48abfe
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/19/2020
ms.locfileid: "92532078"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>Ortağın kazanılmış kredisi nasıl hesaplanıp ödendiğini

**Uygun roller**

- Genel yönetici
- Kullanıcı yöneticisi
- Yönetim Aracısı
- Faturalama yöneticisi
- Satış Aracısı

Yönetilen hizmetler (PEC) için iş ortağı kazanılmış kredisi, müşterilerine 7/24 BT işletimsel denetim ve bunların bölümlerinin yönetimi ve müşterilerinin tüm Azure ortamı gibi iş ortaklarını tanır ve depolar. Varsayılan olarak, CSP 'de iş ortaklarına, aboneliğin abonelik üzerinde 24 X 7 işlemsel yönetim ve denetim gerçekleştirmesine izin veren, müşterinin aboneliğine gerekli erişim hakları verilir. Müşterinin deneyimidir iş ortağı için erişim sağlayabildiği diğer yollar aşağıdaki bölümde açıklanmıştır. Aylık fatura tutarı, iş ortağının kazandığı net kredi tutarıdır. İş ortakları, aylık keşfi dosyasında PEC ayrıntılarını görebilir. Müşterinin deneyimidir iş ortağı için erişim sağlayabildiği ek yollar için, [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)makalesini okuyun.

Ayrıca, [Azure CSP abonelikleri için yeniden devreye sokma yönetici ayrıcalıklarını](revoke-reinstate-csp.md) oku

## <a name="important-eligibility-and-calculation-information"></a>Önemli uygunluk ve hesaplama bilgileri

- İş ortağı, yönettikleri Azure varlıklarının kazanıldığını alacak bir etkin MPN sözleşmesine ve geçerli RBAC rolüne sahip olmalıdır. 

- Dolaylı sağlayıcılar ve dolaylı satıcılarında, dolaylı sağlayıcı veya dolaylı satıcı ya da her ikisi de satıcının CSP 'deki Azure kaynaklarının 7/24 işletimsel denetim ve yönetimine sahip olan dolaylı sağlayıcı PEC 'e uygun olacaktır.

- PEC, müşterinin iş ortağı tarafından yönetilen CSP 'de Azure 'un Azure 'da yaptığı Azure 'un faturalandırılma (Borçlandırılabilir) tüketimle ilişkilendirilir. PEC, yalnızca Microsoft tarafından faturalandırılan (dolaylı sağlayıcı ve doğrudan fatura ortağı) CSP 'deki iş ortakları için kullanılabilir hale getirilir. 

- Uygun hizmetler: Iş ortağı kazanılmış kredisi, Azure plan [fiyatlandırma](https://partner.microsoft.com/commerce/sales) sayfasından iş ortaklarının dışarı aktarılacağı **Azure plan tüketim fiyatlandırması** 'nda listelenen hizmetler için geçerlidir. İş ortağı kazanılmış kredisi, Azure plan tüketim fiyat listesi, Azure plan ayırmaları, market fiyat listesi ve [Azure spot sanal makinelerinde](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/) **Etiketler sütununda** **üçüncü taraf** olarak tanımlanan üçüncü taraf ürünleri için geçerli değildir.

- PEC günlük olarak hesaplanır ve günlük kullanım dosyasında ve aylık fatura keşfi dosyasında görüntülenebilir. Bir iş ortağı (dolaylı sağlayıcı veya dolaylı satıcı), PEC kazanıdıklarından emin olmak için tüm gün (7/24) erişimi olmalıdır. PEC, yönetilen Azure varlıkları için günlük olarak hesaplanır. Belirli bir fatura dönemi için maksimum PEC (ay) %15 ' tir. İş ortakları ay (erişim kapsamı) ile kalıcı ayrıcalıklı erişimi korur ve tüm uygun kaynaklar (erişim kapsamı) için tam PEC %15 kazanacaktır. Kapsam ve yayılma azaltma, ay için daha düşük PEC oranına neden olur. Günlük derecelendirildi kullanım dosyası, PEC 'in uygulanıp uygulanmadığı bir Azure varlığı üzerinde günlük olarak gösterilir. Ayrıca iş ortakları, kalıcı ayrıcalıklı erişim değişiklikleri olup olmadığını algılamak için uyarılara de kaydolabilir.

- PEC, Azure Kaynak düzeyine kadar kazanılmakta. İş ortağı abonelikte veya kaynak grubu düzeyinde geçerli erişime sahipse, daha yüksek varlığa kadar olan her bir kaynak PEC kazanıcaktır.  

- PEC ayrıntıları [Azure maliyet yönetimi](/azure/cost-management-billing/costs/get-started-partners) 'nde de kullanılabilir olacaktır

## <a name="azure-cost-management"></a>Azure Maliyet Yönetimi

Maliyet analizini kullanan Azure maliyet yönetimi (ACM), PEC 'in avantajını almış olan maliyetleri görüntülemek için bir iş ortağı olarak size olanak sağlar.  

1. [Azure Portal](https://portal.azure.com), iş ortağı kiracınızda oturum açın ve **maliyet yönetimi + faturalandırma** ' i seçin.

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
