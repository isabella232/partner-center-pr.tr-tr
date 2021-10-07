---
title: Yönetilen hizmetler için iş ortağı kazanılmış kredisi
ms.topic: article
ms.date: 08/12/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Yönetilen hizmetler için Microsoft iş ortağı kredisi (PEC) nasıl hesaplanacağını ve ödendiğini ve uygun şekilde nasıl emin olduğunuzu öğrenin.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: e4ce75e246139ab2384d478ca02b281848fb7521
ms.sourcegitcommit: 76a7dac540d129ae15cd4c251a4ff43d768370da
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/06/2021
ms.locfileid: "129593336"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>İş ortağı kazanılmış kredisinin hesaplanması ve ödenmesi

**Uygun roller**: genel yönetici | Kullanıcı Yönetimi Yöneticisi | Yönetici Aracısı | Faturalandırma Yöneticisi | Satış Aracısı

Yönetilen hizmetler için iş ortağı kazanılmış kredisi (PEC), müşterilerin Azure ortamının bir kısmını veya tümünü, BT tarafından işletimsel denetim ve yönetimine sahip olan ortakları tanır ve depolar. 

Varsayılan olarak, bir CSP iş ortağı olarak, müşterinizin aboneliğine gerekli erişim hakları vermiş olursunuz ve bu, abonelik üzerindeki kaynakların işletimsel yönetimini ve denetimini gerçekleştirmenize olanak tanır. Müşterilerin deneyimidir iş ortakları için erişim sağlayabildiği diğer yollar aşağıdaki bölümde açıklanmıştır.

Aylık fatura miktarı, iş ortağının kazanılan kredisinin bir ağı olur. , Aylık keşfi dosyanızda PEC ayrıntılarını görebilirsiniz. Müşterinin deneyimidir iş ortağı için erişim sağlayabildiği ek yollar için aşağıdaki makalelere bakın:

- [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)
- [Azure CSP abonelikleri için yönetici ayrıcalıklarını yeniden devreye sokma](reinstate-csp.md)

## <a name="eligibility"></a>Önceliği

Ortağın kazanılmış kredisi (PEC) almak için aşağıdaki gereksinimler geçerlidir:

- Etkin bir MPN sözleşmenize ve geçerli rol tabanlı [erişim denetimi](azure-roles-perms-pec.md) [(RBAC)](/azure/role-based-access-control/overview) rolüne sahip olmanız gerekir.
- Müşterinin Azure aboneliğinde, Azure Kaynak grubunda veya Azure kaynağında veya geçerli bir [RBAC rolünde](azure-roles-perms-pec.md) [adına yönetici (Aobo)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) ayrıcalıklarına sahip olmanız gerekir.
- Dolaylı sağlayıcılar ve dolaylı satıcılarında, dolaylı sağlayıcı veya dolaylı satıcı veya her ikisinin de AOBO ayrıcalıklarına veya uygun bir RBAC rolüne sahip olması durumunda, bir dolaylı sağlayıcı PEC 'e uygundur. Daha fazla bilgi için bkz. [Azure CSP abonelikleri için yeniden devreye sokma yönetici ayrıcalıkları](reinstate-csp.md).
- İş ortağı MPN KIMLIĞI, Satınalmacı MPN KIMLIĞI veya kayıt Iş ortağı (POR) MPN KIMLIĞI ile aynı v-org 'a ait olmalıdır. Daha fazla bilgi için bkz. [İş ortağı kimliğinizi, temsilci atanan kaynaklardaki etkinizi izleyecek şekilde bağlama](/azure/lighthouse/how-to/partner-earned-credit).
- PEC, Azure Kaynak düzeyinde, kaynak grubunda veya abonelikte kazanıldır. Bir iş ortağı, abonelik veya kaynak grubu düzeyinde geçerli erişime sahipse, daha yüksek varlığa kaydolan her kaynak PEC 'e kazanacaktır.
- PEC, aşağıdaki hizmetler için geçerli değildir:
    - Azure plan ayırmaları
    - Azure plan tüketim fiyatının Etiketler sütununda üçüncü taraf olarak tanımlanan üçüncü taraf ürünleri
    - Market fiyat listesindeki ürünler
    - [Azure spot sanal makineleri](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

PEC, yukarıdaki gereksinimlere ek olarak yalnızca Azure plan tüketim fiyatlandırması 'nda listelenen hizmetlere uygulanabilir. Bunu [Azure plan fiyatlandırma](https://partner.microsoft.com/commerce/sales) sayfasından görüntüleyebilir ve dışarı aktarabilirsiniz.

PEC hakkında daha fazla bilgi için bkz. [Azure maliyet yönetimi](/azure/cost-management-billing/costs/get-started-partners) sayfası.

Uygunluk hakkında daha fazla bilgi için bkz. [iş ortağı kazanılmış krediyi kazanmak için gereken roller ve izinler](azure-roles-perms-pec.md).

## <a name="calculation"></a>Hesaplama

PEC, günlük olarak hesaplanır. Her bir abonelik için uygun şekilde erişim sahibi olduğunuz her gün için ücret ödemiştir. PEC ayrıntıları aylık faturanızda görünmese de, PEC kazancı faturada ayarlanan net ücretler satırına doğru şekilde bölünmüştür. [Günlük kullanım dosyasında](daily-rated-usage-recon-files.md) ve aylık fatura keşfi dosyasında daha fazla PEC ayrıntısı bulabilirsiniz.

:::image type="content" source="images/advanced-specializations/recon-file.png" alt-text="Bir Iş Ortağı Merkezi, sütunları tanımlayan bir dosya mutabakatı." border="false":::

Aşağıdaki tabloda, aylık fatura keşfi dosyasında bulunan PEC öğeleri açıklanmaktadır. Tüm değerler, AI, PricingCurrency sütununda gösterildiği gibi ABD doları cinsindendir.

| Sütun  | Açıklama  |
| --------  | -------  |
| Sütun C  | CustomerName  |
| Sütun P | UnitPrice |
| Sütun AD | Efekt. Bu, PEC uygulandıktan ve gereksinimlerin karşılandıktan sonraki fiyatıdır. PEC uygulandığında, AD sütunundaki efekt değeri, P sütunundaki UnitPrice değerinden küçük bir yüzde olduğunu görürsünüz.   |
| Sütun V  | PriceAdjustmentDescription. PEC için bir gereksinim karşılanmazsa veya BirimFiyat 'a uygulanacak PEC 'e sahip değilse bu boş olur. Ancak, ek krediler için uygun olabilirsiniz. Varsa, bu sütunda listelenecektir. Örnek: %100 katman 1 Indirim.   |

PEC erişimini izlemek için:

- **Günlük derecelendirildi kullanım dosyası** , her gün PEC 'in uygulandığını (veya değil) gösterir

- [**Azure izleyici uyarıları**](azure-plan-manage.md) kalıcı ayrıcalıklı erişimdeki değişiklikleri izler.

Günlük derecelendirildi kullanım dosyası:

:::image type="content" source="images/advanced-specializations/partner-daily.png" alt-text="Iş ortağı merkezinin günlük olarak derecelendirilmesine yönelik geçerli birim fiyatını vurgulayan ekran görüntüsü." border="false":::

## <a name="partner-earned-credit-api"></a>İş ortağı kazanılmış kredi API 'SI

PEC API 'SI, Azure API araç takımının bir parçası olarak kullanılabilir. PowerShell ve CLı API 'Leri hakkında bilgi için bkz. [Azure hesabını bir iş ortağı kimliğine bağlama](/azure/cost-management-billing/manage/link-partner-id).

## <a name="azure-cost-management-and-pec"></a>Azure maliyet yönetimi ve PEC

Maliyet analizini kullanan Azure maliyet yönetimi (ACM), PEC 'in avantajını almış olan maliyetleri görüntülemek için bir iş ortağı olarak size olanak sağlar. ACM üzerinde ayrıntılı bir sunum için [mayıs 2021 CSP Spotlight çağrısına](https://commercial_licensing.eventbuilder.com/2021MayCSPSpotlight)bakın.

## <a name="use-acm-to-view-your-partner-earned-credit"></a>İş ortağınızın kazanılmış krediyi görüntülemek için ACM kullanın

1. [Azure Portal](https://portal.azure.com/), iş ortağı kiracınızda oturum açın ve **maliyet yönetimi + faturalandırma**' i seçin.
2. **Maliyet yönetimi**' ni seçin.
3. **Maliyet analizini** seçin.
Maliyet analizi görünümü, satın alınan ve Microsoft 'a ödediğiniz fiyatlarla tüketilen tüm hizmetler için faturalandırma hesabınızın maliyetlerini görüntüler.

:::image type="content" source="images/advanced-specializations/partner-cost.png" alt-text="Maliyet yönetimi maliyet analizi sayfasının ekran görüntüsü." border="false":::

4. Özet Grafik açılan listesinde, Partnerearnedtappnda ' ı seçin. 

    Bu değer **true** ise, ilişkili maliyet, ortağın kazanılan kredisi avantajına sahiptir.

    Bu değer **false** ise, ilişkili maliyet kredi için gereken uygunluğu karşılanmaz veya satın alınan hizmet, ortağın kazanıldığı kredi için uygun değildir.

>[!NOTE]
>Genellikle, hizmetler için kullanım maliyet yönetiminde 8-24 saat sürer ve PEC kredileri, Azure maliyet yönetimi 'nde erişim zamanından itibaren 48 saat içinde görünür.

Ayrıca, **Gruplandırma** ölçütü ve filtre özellikleri **Ekle** ' yi kullanarak iş **ortağı** tarafından da gruplandırabilirsiniz ve filtre uygulayabilirsiniz. Bu, PEC 'e sahip maliyetlerin ve PEC uygulanmamış maliyetlerin ayrıntılarına gitmenizi sağlar.

## <a name="how-is-pec-paid"></a>PEC nasıl ücretli?
PEC kazancı, faturada ayarlanan net ücretler satırına bölünmüştür. Aşağıda gösterilen fatura **toplamı** bunu gösterir. Ayarlama ayrıntıları için, aylık fatura mutabakatı dosyası ve Azure günlük derecelendirmeli kullanım dosyası ' na bakın.

:::image type="content" source="images/advanced-specializations/invoice.png" alt-text="Düzeltme ayrıntılarının keşfi ve Azure günlük kullanım dosyalarında göründüğünü belirten bir Iş Ortağı Merkezi faturasının ekran görüntüsü." border="false":::

## <a name="next-steps"></a>Sonraki adımlar

- [CSP 'de Azure için yeni ticari deneyim fiyat listesi](azure-plan-price-list.md)
- [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)
- [CSP'de yeni ticari deneyim - Azure faturalama](azure-plan-billing.md)
- [Azure CSP abonelikleri için yönetici ayrıcalıklarını yeniden devreye sokma](reinstate-csp.md)
- [İş ortağı kazanılmış kredi-genel bakış](partner-earned-credit.md)
- [Roller, iş ortağı kazanılmış kredi için izinler](azure-roles-perms-pec.md)
- [Iş ortağı kazanılmış krediyi anlama (kılavuz)](https://partner.microsoft.com/resources/detail/understanding-partner-earned-credit-pdf) (oturum açma gerekir)