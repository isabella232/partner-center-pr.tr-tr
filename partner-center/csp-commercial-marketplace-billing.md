---
title: Ticari Market ürünleri için faturalandırma
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Faturalandırma, Iş Ortağı Merkezi 'nde ticari marketten müşteriler için satın alınan ISV SaaS ürünleri veya abonelikleri için nasıl çalıştığını öğrenin.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c03ab358b8fb6ab0f23ea5f42b9d35c6f6c2b80c
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/22/2020
ms.locfileid: "92531663"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a>Iş Ortağı Merkezi 'nde ticari Market ürünleri ve abonelikleri için faturalandırma

**Uygulama hedefi**

- İş Ortağı Merkezi
- CSP programındaki iş ortakları

**Uygun roller**

- Genel yönetici
- Faturalama yöneticisi

CSP programındaki bir iş ortağı olarak, ticari Market 'teki ISV yayımcılarından lisans tabanlı SaaS ürünlerini satın almak için Iş Ortağı Merkezi 'ni kullanabilirsiniz. Bunu yaptıktan sonra, bu tür satın alma işlemleri için bir faturaya erişebilirsiniz. Fatura dönemi, takvim ayının ilk gününde başlar ve takvim ayının son gününde sona erer. Faturalar, aşağıdaki ayın 8. gününde kullanılabilir hale getirilir.

Faturalara Iş Ortağı Merkezi [panosundan](https://partner.microsoft.com/dashboard/) veya [Iş Ortağı Merkezi API 'leri](/partner-center/develop/)kullanarak erişebilirsiniz.

CSP programındaki iş ortakları, Iş Ortağı Merkezi 'nden veya Azure portal (müşterinin önceki, CSP tarafından satın alınan Azure kiracısı kullanılarak) bu ürünleri satın alırken müşteri için satın alınan ISV ticari Market çözümleri için faturalandırılır.

>[!NOTE]
>Müşteriler kendi Azure AD kiracısını (CSP programındaki bir iş ortağından satın almalarından değil) kullanıyorsa, müşteriler kendi ISV SaaS çözümünü doğrudan ([Microsoft AppSource](https://appsource.microsoft.com/) veya [Azure Marketi](https://azuremarketplace.microsoft.com/)) üzerinden satın almayı da seçebilirler. Bu durumda, doğrudan Microsoft 'tan kendi faturanızı alırlar. Benzer şekilde, CSP programındaki bir iş, müşteriye bir Azure aboneliği veya yeni Azure planı satmakta ve bu kiracıya müşteri (ya da dolaylı satıcı) [rol tabanlı erişim](/azure/role-based-access-control/built-in-roles) izni veriyorsa ( **okuyucunun** yanı sıra müşteriye herhangi bir rol atama), bu müşteri (veya dolaylı satıcı), CSP ortağına önceden onay veya bildirim olmaksızın ticari Market teklifleri de satın alabilir. Bu durumlarda, Microsoft, CSP programındaki iş ortaklarına müşterilerinin yaptığı satın alma işlemleri hakkında doğrudan bildirim vermez. Ancak Microsoft, bir Azure aboneliğinde etkinlik hakkında uyarı veya bildirim ayarlamak için kullanabileceğiniz isteğe bağlı bir [Azure izleyici](/azure/azure-monitor/platform/alerts-activity-log) mekanizması sunar.

## <a name="access-billing-information-for-commercial-marketplace-products"></a>Ticari Market ürünleri için faturalandırma bilgilerine erişin

Bir fatura görüntülemeye hazırsanız şirketinizin genel yönetici veya faturalama yöneticisi bir e-posta alır. Ticari Market ürün satın alımları için en son faturaya ve mutabakat dosyasına erişmek için:

1. Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard/)oturum açın.

2. Iş Ortağı Merkezi menüsünde **faturalandırma** ' i seçin. 

    Faturalandırma sayfasının en üstünde iki sekme görürsünüz: **yinelenen** ve **yinelenen ve tek seferlik satın** alma. Her sekme, farklı Market ürünleri için fatura ve mutabakat (keşfi) dosyalarına erişmenizi sağlar:

    - **Yinelenen** sekme: Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, Power BI Pro ve Microsoft Azure ile ilgili abonelikler için fatura ve mutabakat dosyalarını gösterir.

    - **Yinelenen ve tek seferlik satın** alma sekmesi: Azure planı, Azure ayırmaları, yazılım ve ticari Market ürünleri için fatura ve mutabakat dosyalarını gösterir.
  
3. **Yinelenen ve tek seferlik Satınalmalar** sekmesini seçin. Bir müşteri için abonelikleri farklı bir para birimiyle satın aldıysanız, her para birimi için bir sekme görürsünüz. Birkaç şey yapabilirsiniz fr: OM Bu sayfa:

    - En son fatura ve mutabakat dosyasını görmek için **Fatura** veya **Mutabakat dosyası** ' nı seçin. (İsterseniz, en son faturaya ve keşfi dosya verilerine [Iş Ortağı Merkezi API 'lerini](/partner-center/develop/)kullanarak da erişebilirsiniz.

    - Önceki faturaları ve keşfi dosyalarını görmek için, aşağıdaki **Faturalama geçmişi** satırını genişletin.

    - En son hesap etkinliğine bağlı olarak istediğiniz zaman tahmini hesap bakiyenizi veya faturanızı denetlemek için **tahminler** başlığı altında bir bağlantı seçin.  

    >[!NOTE]
    > Faturanız ayın 8. gününde faturalandırıldığımızda, vergiler ve diğer ilgili ücretleri ve krediler dahil edilir. Bu, son tutarın, fatura dönemi boyunca gördüklerinizden farklı olabileceği anlamına gelir.

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>Ticari Market ürünleri için faturalar ve keşfi dosyaları hakkında daha fazla bilgi

Bu bölümde, üçüncü taraf ISV yayımcılarından müşteriler için satın alınan ticari Market SaaS aboneliklerine yönelik fatura ve mutabakat dosyaları hakkında daha fazla bilgi sunulmaktadır.

Iş Ortağı Merkezi menüsündeki **faturalandırma** seçeneğinden **yinelenen ve tek seferlik satın alımlar** ' ı seçtiğinizde, hem Microsoft (birinci taraf) hem de ISV (üçüncü taraf) satın alımlarıyla ilgili ücretler için faturalara ve mutabakat dosyalarına erişim elde edersiniz. Bu satın almalarla ilişkilendirilebilir:

- SaaS abonelikleri (Microsoft ya da ISV yayımcılarından)

- Azure planı

- Azure rezervasyonları

- Diğer abonelik tabanlı yazılımlar (Microsoft ya da ISV yayımcılarından)

Bu satın almalara örnek olarak SUSE Linux yazılımı (yazılım aboneliği) veya bir Azure ISV SaaS ürün aboneliği bulunabilir.

>[!NOTE]
> Fatura ve keşfi dosyalarını okuma hakkında daha fazla bilgi için bkz. [faturalandırma genel bakış](billing.md).

### <a name="tips-on-reading-your-invoice"></a>Faturanızı okuma ipuçları

Üçüncü taraf bir ISV yayımcısından lisans tabanlı bir SaaS ürünü satın aldığınızda, yalnızca faturanızda lisans ücreti için ücret görüntülenir. ISV SaaS ürünü, temel alınan Azure altyapı kaynaklarını kullandığında (veya tükettiği), bu, geçerlidir. Bunun nedeni, müşterinizin bir ISV 'nin SaaS ürünü için Azure altyapı kullanım ücretlerinden doğrudan ISV 'ye faturalandırılması nedeniyle oluşur. (ISV 'Ler, ilişkili Azure tüketim ücretlerini kendi Azure kullanımı günlük derecelendirmeli fatura mutabakatı dosyasında görür.)

Faturanızda çeşitli sayfalar yer alacak:

- **Faturanın 1. sayfası:** CSP program ortağının faturalandırma ayrıntılarına bir Özet bakış içerir. Bu, fatura dönemi, fatura numarası, ödeme koşulları (NET 60 gün) ve tel veya çek aracılığıyla ödeme yapmak için ödeme ödemesi yöntemlerine yönelik ücretler özetini içerir.

- **Faturaya ait 2 (ve sonraki tüm sayfalar) sayfası:** Ticari Market 'ten hem birinci taraf Microsoft satınalmaları hem de üçüncü taraf ISV (lisans tabanlı) satın alma işlemleri için Ayrıntılar ücretleri. ISV lisansı tabanlı satın alımları her ürün adının altında **Yayımcı** satırıyla tanımlayabilirsiniz. İlişkili mutabakat dosyası, belirli fatura ücretleri için daha fazla faturalandırma ayrıntısı sunar.

- **Faturanın son sayfası:** Bir ISV 'den lisans tabanlı Market ürünleri için ücretlendirilmiş olmanız durumunda bu son sayfada ISV yayımcısının adı ve adresiyle ilgili daha fazla ayrıntı görüntülenir.

### <a name="tips-on-reading-your-reconciliation-file"></a>Mutabakat dosyanızı okuma ipuçları

**Yinelenen ve tek seferlik satın** alma mutabakatı dosyası, faturanızda ücretlerle eşlenen ek ayrıntıların bulunduğu birkaç sütun içerir. **PublisherName** sütunu, satınalmanın Microsoft veya üçüncü taraf bir ISV yayımcısı olup olmadığını gösterir.

Mutabakat dosyanızdaki bazı ücretler $0 maliyeti ile görünebilir. Bunun nedeni ISV "ücretsiz deneme" teklifi (genellikle 30 veya 60 gün) veya kendi lisansını getir teklifi olabilir.

Ücretsiz deneme ISV teklifleri söz konusu olduğunda:

- Ücretsiz deneme süresi, ISV 'nin lisans tabanlı SaaS ürününün maliyetini bu süre boyunca ele alır. Ayrıca, bu SaaS ürününün ilişkili Azure altyapı kullanımı için ücretlendirilmeyecektir.  Ancak, kullanım tabanlı bir ISV teklifi kullanıyorsanız, ücretsiz deneme, temel alınan Azure altyapı kullanımının maliyetini içermez. Bu durumda, Azure altyapı kullanım ücretleri ayrı bir Azure mutabakatı dosyasında görüntülenir.

- Müşterilerinizin müşterinizin ücretsiz deneme sürümünü satın alıp dağıttığınızda, müşteri otomatik olarak ISV yayımcısı tarafından ücretsiz denemeye kaydedilir. Ücretsiz deneme süresi, ISV yayımcısı tarafından tanımlanan dönemden sonra otomatik olarak sona erer. Süre bittikten sonra müşteri ücretlendirilecektir. Bu, mutabakat dosyasının deneme sürümü uygun bir ürün için iki satır gösterebileceği anlamına gelir: deneme süresini izleyen ve ücretli teklifi izleyen bir ücret (deneme süresi sona erdikten sonra $0 maliyeti gösterir). Deneme süresi bittikten sonra, ücretli teklifin gösterildiği satır ücretleri göstermeye başlayacaktır. 

Her sütunun temsil ettiği hakkında daha fazla bilgi için bkz. [karşılaştırma dosyalarınızı kullanma](use-the-reconciliation-files.md). Ayrıca bkz. [Iş Ortağı Merkezi 'nde faturalandırma türleri](billing-different-types.md)

## <a name="next-steps"></a>Sonraki adımlar

- [Müşteriler için ticari Market ürünlerini yönetme](csp-commercial-marketplace-manage.md)
- [Ticari Market ürünleri desteği hakkında bilgi edinin](csp-commercial-marketplace-support.md)