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
ms.openlocfilehash: c25d4ab3077c6a0f648c767472e8b7b60ef53a9c
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148032"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a>Iş Ortağı Merkezi 'nde ticari Market ürünleri ve abonelikleri için faturalandırma


**Uygun roller**: genel yönetici | Faturalama yöneticisi

CSP programındaki bir iş ortağı olarak, ticari Market 'teki ISV yayımcılarından lisans tabanlı SaaS ürünlerini satın almak için Iş Ortağı Merkezi 'ni kullanabilirsiniz. Bunu yaptıktan sonra, bu tür satın alma işlemleri için bir faturaya erişebilirsiniz. Fatura dönemi, takvim ayının ilk gününde başlar ve takvim ayının son gününde sona erer. Faturalar, aşağıdaki ayın 8. gününde kullanılabilir hale getirilir.

Faturalara Iş Ortağı Merkezi [panosundan](https://partner.microsoft.com/dashboard/) veya [Iş Ortağı Merkezi API 'leri](/partner-center/develop/)kullanarak erişebilirsiniz.

CSP programındaki iş ortakları, Iş Ortağı Merkezi 'nden veya Azure portal (müşterinin önceki, CSP tarafından satın alınan Azure kiracısı kullanılarak) bu ürünleri satın alırken müşteri için satın alınan ISV ticari Market çözümleri için faturalandırılır.

>[!NOTE]
>Müşteriler kendi Azure AD kiracısını (CSP programındaki bir iş ortağından satın almalarından değil) kullanıyorsa, müşteriler kendi ISV SaaS çözümünü doğrudan ([Microsoft AppSource](https://appsource.microsoft.com/) veya [Azure Marketi](https://azuremarketplace.microsoft.com/)) üzerinden satın almayı da seçebilirler. Bu durumda, doğrudan Microsoft 'tan kendi faturanızı alırlar. Benzer şekilde, CSP programındaki bir iş, müşteriye bir Azure aboneliği veya yeni Azure planı satmakta ve bu kiracıya müşteri (ya da dolaylı satıcı) [rol tabanlı erişim](/azure/role-based-access-control/built-in-roles) izni veriyorsa ( **okuyucunun** yanı sıra müşteriye herhangi bir rol atama), bu müşteri (veya dolaylı satıcı), CSP ortağına önceden onay veya bildirim olmaksızın ticari Market teklifleri de satın alabilir. Bu durumlarda, Microsoft, CSP programındaki iş ortaklarına müşterilerinin yaptığı satın alma işlemleri hakkında doğrudan bildirim vermez. Ancak Microsoft, bir Azure aboneliğinde etkinlik hakkında uyarı veya bildirim ayarlamak için kullanabileceğiniz isteğe bağlı bir [Azure izleyici](/azure/azure-monitor/platform/alerts-activity-log) mekanizması sunar.

## <a name="access-billing-information-for-commercial-marketplace-products"></a>Ticari Market ürünleri için faturalandırma bilgilerine erişin

Bir fatura görüntülemeye hazırsanız şirketinizin genel yönetici veya faturalama yöneticisi bir e-posta alır. Ticari Market ürün satın alımları için en son faturaya ve mutabakat dosyasına erişmek için:

1. İş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard/) oturum açın.

2. Iş Ortağı Merkezi menüsünde **faturalandırma**' i seçin. 

    Faturalandırma sayfasının en üstünde iki sekme görürsünüz: **yinelenen** ve **yinelenen ve tek seferlik satın** alma. Her sekme, farklı Market ürünleri için fatura ve mutabakat (keşfi) dosyalarına erişmenizi sağlar:

    - **Yinelenen** sekme: Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, Power BI Pro ve Microsoft Azure ile ilgili abonelikler için fatura ve mutabakat dosyalarını gösterir.

    - **Yinelenen ve tek seferlik satın** alma sekmesi: Azure planı, Azure ayırmaları, yazılım ve ticari Market ürünleri için fatura ve mutabakat dosyalarını gösterir.
  
3. **Yinelenen ve tek seferlik Satınalmalar** sekmesini seçin. Bir müşteri için abonelikleri farklı bir para birimiyle satın aldıysanız, her para birimi için bir sekme görürsünüz. Bu sayfadan birkaç şey yapabilirsiniz:

    - En son fatura ve mutabakat dosyasını görmek için **Fatura** veya **Mutabakat dosyası**' nı seçin. (İsterseniz, en son faturaya ve keşfi dosya verilerine [Iş Ortağı Merkezi API 'lerini](/partner-center/develop/)kullanarak da erişebilirsiniz.

    - Önceki faturaları ve keşfi dosyalarını görmek için, aşağıdaki **Faturalama geçmişi** satırını genişletin.

    - En son hesap etkinliğine bağlı olarak istediğiniz zaman tahmini hesap bakiyenizi veya faturanızı denetlemek için **tahminler** başlığı altında bir bağlantı seçin.  

    >[!NOTE]
    > Faturanız ayın 8. gününde faturalandırıldığımızda, vergiler ve diğer ilgili ücretleri ve krediler dahil edilir. Bu, son tutarın, fatura dönemi boyunca gördüklerinizden farklı olabileceği anlamına gelir.

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>Ticari market ürünleri için faturalar ve mutabakat dosyaları hakkında daha fazla bilgi

Bu bölümde, üçüncü taraf ISV yayımcılarından müşteriler için satın alınan ticari market SaaS abonelikleri için fatura ve mutabakat dosyaları hakkında daha fazla bilgi sunulmaktadır.

İş Ortağı Merkezi menüsündeki Faturalama seçeneğinden Yinelenen  ve tek kez satın almalar'ı seçerek hem Microsoft (birinci taraf) hem de ISV (üçüncü taraf) satın almaları ile ilgili ücretler için faturalara ve mutabakat dosyalarına erişim elde edersiniz.  Bu satın almalar aşağıdakilerle ilişkili olabilir:

- SaaS abonelikleri (Microsoft veya ISV yayımcılarından)

- Azure planı

- Azure rezervasyonları

- Diğer abonelik tabanlı yazılımlar (Microsoft veya ISV yayımcılarından)

Bu satın alma örnekleri arasında SUSE Linux yazılımı (yazılım aboneliği) veya Azure ISV SaaS ürün aboneliği yer alır.

>[!NOTE]
> Fatura ve mutabakat dosyalarını okuma hakkında daha fazla bilgi için bkz. Faturalamaya [genel bakış.](billing.md)

### <a name="tips-on-reading-your-invoice"></a>Faturanızı okuma ipuçları

Üçüncü taraf BIR ISV yayımcısı tarafından lisans tabanlı SaaS ürünü satın aldığınız zaman, faturanıza yalnızca lisans ücreti için ücret yansıtılacaktır. ISV'nin SaaS ürünü temel Alınan Azure altyapı kaynaklarını kullandığında (veya kullandığında) bile bu doğrudur. Bunun nedeni, müşterinizin BIR ISV SaaS ürününün Azure altyapısı kullanım ücretlerinin doğrudan ISV'ye faturalandırılatır. (ISV'ler ilişkili Azure tüketim ücretlerini kendi Azure kullanımları günlük olarak derecelendirilmiş fatura mutabakat dosyasında görebilir.)

Faturanız birkaç sayfa içerir:

- **Faturanın 1. sayfası:** CSP programı iş ortağının faturalama ayrıntılarına genel bir bakış içerir. Buna faturalama dönemi ücretlerinin özeti, fatura numarası, ödeme koşulları (Net 60 gün) ve havaleyle veya çekle ödemeye yönelik faturalama ödeme yöntemleri dahildir.

- **Faturanın 2. Sayfası (ve sonraki sayfalar):** Ticari marketten hem birinci taraf Microsoft satın almaları hem de üçüncü taraf ISV (lisans tabanlı) satın almaları için ayrıntılar. ISV lisansı tabanlı satın alımları her ürün adının altında **Yayımcı** satırıyla tanımlayabilirsiniz. İlişkili mutabakat dosyası, belirli fatura ücretleri için daha fazla faturalandırma ayrıntısı sunar.

- **Faturanın son sayfası:** Bir ISV 'den lisans tabanlı Market ürünleri için ücretlendirilmiş olmanız durumunda bu son sayfada ISV yayımcısının adı ve adresiyle ilgili daha fazla ayrıntı görüntülenir.

### <a name="tips-on-reading-your-reconciliation-file"></a>Mutabakat dosyanızı okuma ipuçları

**Yinelenen ve tek seferlik satın** alma mutabakatı dosyası, faturanızda ücretlerle eşlenen ek ayrıntıların bulunduğu birkaç sütun içerir. **PublisherName** sütunu, satınalmanın Microsoft veya üçüncü taraf bir ISV yayımcısı olup olmadığını gösterir.

Mutabakat dosyanızdaki bazı ücretler $0 maliyeti ile görünebilir. Bunun nedeni ISV "ücretsiz deneme" teklifi (genellikle 30 veya 60 gün) veya kendi lisansını getir teklifi olabilir.

Ücretsiz deneme ISV teklifleri söz konusu olduğunda:

- Ücretsiz deneme süresi, ISV 'nin lisans tabanlı SaaS ürününün maliyetini bu süre boyunca ele alır. Ayrıca, bu SaaS ürününün ilişkili Azure altyapı kullanımı için ücretlendirilmeyecektir.  Ancak, kullanım tabanlı bir ISV teklifi kullanıyorsanız, ücretsiz deneme, temel alınan Azure altyapı kullanımının maliyetini içermez. Bu durumda, Azure altyapı kullanım ücretleri ayrı bir Azure mutabakatı dosyasında görüntülenir.

- Müşterilerinizin müşterinizin ücretsiz deneme sürümünü satın alıp dağıttığınızda, müşteri otomatik olarak ISV yayımcısı tarafından ücretsiz denemeye kaydedilir. Ücretsiz deneme süresi, ISV yayımcısı tarafından tanımlanan dönemden sonra otomatik olarak sona erer. Süre bittikten sonra müşteri ücretlendirilecektir. Bu, mutabakat dosyasının deneme sürümü uygun bir ürün için iki satır gösterebileceği anlamına gelir: deneme süresini izleyen ve ücretli teklifi izleyen bir ücret (deneme süresi sona erdikten sonra $0 maliyeti gösterir). Deneme süresi bittikten sonra, ücretli teklifin gösterildiği satır ücretleri göstermeye başlayacaktır. 

Her sütunun neyi temsil ettiği hakkında daha fazla bilgi için [bkz. Mutabakat dosyalarınızı kullanma.](use-the-reconciliation-files.md) Ayrıca [bkz. İş Ortağı Merkezi'da faturalama türleri](./billing-basics.md)

## <a name="next-steps"></a>Sonraki adımlar

- [Müşteriler için ticari market ürünlerini yönetme](csp-commercial-marketplace-manage.md)
- [Ticari market ürünlerine yönelik destek hakkında bilgi alın](csp-commercial-marketplace-support.md)