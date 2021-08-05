---
title: Yönetilen hizmetler için iş ortağı tarafından kazanılan kredi
ms.topic: article
ms.date: 07/22/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Yönetilen hizmetler için Microsoft iş ortağı tarafından kazanılan kredinin (PEC) nasıl hesaplanmış ve ücretli olduğunu ve uygun olduğundan emin olun.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: e897aad48dd04489e340952ba4cd4e27f7e2a9de
ms.sourcegitcommit: 90bf27df911b428b1222f483c32ba6367870e7c5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/04/2021
ms.locfileid: "115101325"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>İş ortağı kazanılmış kredisinin hesaplanması ve ödenmesi

**Uygun roller:** Genel yönetici | Kullanıcı yönetimi yönetici | Yönetici aracısı | Faturalama yöneticisi | Satış aracısı

Yönetilen hizmetler için iş ortağı tarafından kazanılmış kredi (PEC), bir müşterilerin Azure ortamının bir veya bir veya hepsi için, IT operasyonel denetimine ve yönetimine sahip olan iş ortaklarını tanır ve ödüllendirir. 

CsP iş ortağı olarak varsayılan olarak, müşterinizin aboneliği üzerinde gerekli erişim haklarınız olur ve abonelikte işlem yönetimi ve denetimi gerçekleştirmenize olanak sağlar. Müşterilerin işlem ortakları için erişim sağlamanın diğer yolları aşağıdaki bölümde açıklanmıştır.

Aylık fatura tutarı, iş ortağı tarafından kazanılan kredinin net tutarıdır. Aylık mutabakat dosyanız üzerinde PEC ayrıntılarını görebilir. Müşterinin işlem ortağına erişim sağlamanın ek yolları için aşağıdaki makalelere bakın:

- [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)
- [Azure CSP abonelikleri için yönetici ayrıcalıklarını yeniden devreye sokma](/revoke-reinstate-csp.md)

## <a name="eligibility"></a>Uygunluk

İş Ortağı Tarafından Kazanılan Kredi (PEC) almak için aşağıdaki gereksinimler geçerlidir:

- Etkin bir MPN sözleşmeye ve geçerli rol tabanlı erişim [denetimi](azure-roles-perms-pec.md) [(RBAC) rolüne sahip olmak](/azure/role-based-access-control/overview) gerekir.
- Müşterinin Azure aboneliğinde, Azure kaynak grubunda veya Azure kaynağında Yönetici Adına [(AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) ayrıcalıklarına veya geçerli bir RBAC rolüne [sahip olmanız gerekir.](azure-roles-perms-pec.md)
- Dolaylı sağlayıcı veya dolaylı kurumsal bayi ya da her ikisi de AOBO ayrıcalıklarına veya uygun bir RBAC rolüne sahipse dolaylı sağlayıcı, dolaylı sağlayıcı PEC için uygun olur. Daha fazla bilgi için [bkz. Abonelikler için yönetici ayrıcalıklarını Azure CSP.](revoke-reinstate-csp.md)
- İş ortağı MPN Kimliği, satın alan MPN Kimliği veya Kayıt Ortağı (MPN) MPN Kimliği ile aynı v-kuruluşa ait olması gerekir. Daha fazla bilgi için bkz. [İş ortağı kimliğinizi, temsilci atanan kaynaklardaki etkinizi izleyecek şekilde bağlama](/azure/lighthouse/how-to/partner-earned-credit).
- PEC, Azure kaynak düzeyinde, kaynak grubunda veya abonelikte kazanılır. Bir iş ortağının abonelik veya kaynak grubu düzeyinde geçerli erişimi varsa, daha yüksek bir varlığa yuvarlanan her kaynak PEC kazanır.
- PEC aşağıdaki hizmetler için geçerli değildir:
    - Azure planı rezervasyonları
    - Azure planı tüketim fiyatının Etiketler sütununda Üçüncü Taraf olarak tanımlanan üçüncü taraf ürünleri
    - Market fiyat listesinde yer alan ürünler
    - [Azure Spot Sanal Makineler](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

Yukarıdaki gereksinimlere ek olarak, PEC yalnızca Azure planı tüketim fiyatlandırması içinde listelenen hizmetler için geçerlidir. Bunu Azure planı fiyatlandırma sayfasından [görüntüleyebilirsiniz ve dışarı aktarabilirsiniz.](https://partner.microsoft.com/commerce/sales)

PEC hakkında daha fazla bilgi için [bkz. Azure Maliyet yönetimi](/azure/cost-management-billing/costs/get-started-partners) sayfası.

Uygunluk hakkında daha fazla bilgi için bkz. [İş ortağı tarafından kazanılan kredi kazanmak için gereken roller ve izinler.](azure-roles-perms-pec.md)

## <a name="calculation"></a>Hesaplama

PEC günlük olarak hesaplanır. Her abonelikte PEC uygun erişiminizin olduğu her gün için ödemeniz olur. PEC ayrıntıları aylık faturanız gibi görünmese de, PEC kazançları faturanın içindeki ayarlanmış net ücretler satırına dahil edildi. Günlük kullanım dosyasında ve aylık fatura mutabakat [dosyasında daha](daily-rated-usage-recon-files.md) fazla PEC ayrıntısı bulabilirsiniz.

Aşağıdaki tabloda aylık fatura mutabakat dosyasında bulunan PEC öğeleri açıklanmıştır. Tüm değerler, PricingCurrency sütununda gösterildiği gibi ABD doları olarak gösterilir.

| Sütun  | Açıklama  |
| --------  | -------  |
| Sütun C  | CustomerName  |
| Sütun P | UnitPrice |
| Sütun AD | EffectiveUnitPrice. Bu, PEC uygulandıktan ve gereksinimler karşı uygulandıktan sonra fiyattır. PEC uygulandığında, AD sütunundaki EffectiveUnitPrice'ın P sütunundaki UnitPrice'dan daha düşük bir yüzde olduğunu görüyorsunuz.   |
| Sütun V  | PriceAdjustmentDescription. PEC için herhangi bir gereklilik karşılamıyorsa veya UnitPrice'a uygulanacak PEC % 'ine sahipse bu boş olur. Ancak, ek krediler için uygun olabilir. Öyleyse, bunlar bu sütunda listelenir. Örnek: %100 Katman 1 İndirimi.   |

PEC erişimini izlemek için:

- **Günlük olarak derecelendirilmiş kullanım** dosyası, PEC'in günlük olarak nerede uygulandığını (veya uygulanmaz) gösterir

- [**Azure İzleyici uyarıları, kalıcı**](azure-plan-manage.md) ayrıcalıklı erişimde yapılan değişiklikleri izleyebilir.

## <a name="partner-earned-credit-api"></a>İş ortağı tarafından kazanılan kredi API'si

Azure API araç kümesi kapsamında bir PEC API'si kullanılabilir. PowerShell ve CLI API'leri hakkında bilgi için [bkz. Azure hesabını iş ortağı kimliğine bağlama.](/azure/cost-management-billing/manage/link-partner-id)

## <a name="azure-cost-management-and-pec"></a>Azure Maliyet Yönetimi ve PEC

Azure Maliyet Yönetimi Analizi'nin (ACM) kullanımı, iş ortağı olarak PEC avantajını alan maliyetleri görüntülemeye olanak sağlar. ACM hakkında ayrıntılı bir sunum için Mayıs [2021 CSP Spotlight çağrısına bakın.](https://commercial_licensing.eventbuilder.com/2021MayCSPSpotlight)

## <a name="use-acm-to-view-your-partner-earned-credit"></a>ACM kullanarak iş ortağı tarafından kazanılan kredinizi görüntüleme

1. Giriş [Azure portal](https://portal.azure.com/)iş ortağı kiracınıza oturum açma ve Maliyet Yönetimi **+ Faturalama'yi seçin.**
2. Maliyet **yönetimi'ne seçin.**
3. Maliyet **Analizi'ne seçin.**
Maliyet Analizi görünümü, Microsoft'un ödemesi yapılan fiyatlarla satın alınan ve tüketilen tüm hizmetler için ödeme hesabınız için maliyetleri görüntüler.
4. Özet grafik açılan listesinde PartnerEarnedCreditApplied öğesini seçin. 

    Bu değer True **ise** ilişkili maliyet, iş ortağı tarafından kazanılan kredinin avantajına sahip olur.

    Bu değer **False** ise, ilişkili maliyet kredi için gerekli uygunluğu karşılamadı veya satın alınan hizmet iş ortağı tarafından kazanılan kredi için uygun değildir.

>[!NOTE]
>Genellikle, hizmetlerin kullanımının Maliyet Yönetimi'ne görünmesi 8-24 saat sürer ve PEC kredileri, hizmetlere erişimden itibaren 48 saat içinde Azure Maliyet Yönetimi.

Ayrıca Grupla ve Filtre özellikleri ekle'yi kullanarak **PartnerEarnedCreditApplied** özelliğine **göre gruplandırabilirsiniz** **ve filtreye göre** filtreleysiniz. Bunlar, PEC'e sahip olan maliyetlerin ve PEC uygulanmadan maliyetlerin detaya gitmelerini sağlar.

## <a name="how-is-pec-paid"></a>PEC nasıl ödeniyor?
PEC kazançları, fatura içindeki ayarlanmış net ücretler satırına dahil edildi. Ayarlama ayrıntıları için aylık fatura mutabakat dosyası ve Azure günlük olarak derecelendirilmiş kullanım dosyasına bakın.

## <a name="next-steps"></a>Sonraki adımlar

- [Yeni ticari deneyim için fiyat listesi CSP'de Azure](azure-plan-price-list.md)
- [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)
- [CSP'de yeni ticari deneyim - Azure faturalama](azure-plan-billing.md)
- [Azure CSP abonelikleri için yönetici ayrıcalıklarını yeniden devreye sokma](revoke-reinstate-csp.md)
- [İş ortağı tarafından kazanılan kredi - genel bakış](partner-earned-credit.md)
- [Roller, iş ortağı tarafından kazanılan kredi izinleri](azure-roles-perms-pec.md)
- [İş Ortağı Tarafından Kazanılan Krediyi Anlama (kılavuz)](https://partner.microsoft.com/resources/detail/understanding-partner-earned-credit-pdf) (oturum açma gereklidir)