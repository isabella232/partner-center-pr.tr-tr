---
title: Teklifleri bulma-ticari Market
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP iş ortaklarının, bağımsız yazılım satıcılarından (ISV) SaaS teklifleri veya fiyatlandırma için Market 'i görüntülemek veya aramak üzere Iş ortağı merkezini nasıl kullanabileceği hakkında bilgi edinin.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e89473cf095be4cc87c96f1c2a6d0da224eccedd
ms.sourcegitcommit: f34f2f69e6df4f260479a205d94010cf47987ff2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/25/2020
ms.locfileid: "96038871"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a>Partner Center ticari marketi 'nde teklifleri ve fiyatları bulma

**Şunlara uygulanır**

- İş Ortağı Merkezi
- CSP programındaki iş ortakları

**Uygun roller**

- Genel yönetici
- Yönetim Aracısı

Bağımsız yazılım satıcıları (ISV 'Ler), ticari Market 'te teklif yayımlamayı tercih ettikleri zaman, teklifin CSP programında kullanılabilir hale getirilme konusunda da karar verebilir. Teklifi CSP programı aracılığıyla satmayı tercih ediyorsanız, CSP iş ortakları Partner Center marketi alanında teklifi görmeniz gerekir.

Bir ISV teklifi, Iş Ortağı Merkezi 'nde beklemiş gibi görünmezse şu olabilir:

- ISV, teklifi CSP programı aracılığıyla satmamaya karar verdi. Örneğin, bazı ISV ürünleri ticari Market 'in diğer alanlarında (örneğin, [Microsoft AppSource](https://appsource.microsoft.com/) ve [Azure Marketi](https://azuremarketplace.microsoft.com/)'nde) kullanıma sunulmuştur, ancak iş ortağı merkezi marketi 'nde CSP programındaki iş ortakları için görünmeyebilir.

- ISV, teklifi yalnızca belirli sayıda CSP iş ortağı için özel olarak yapmaya karar verdi. Özel teklifler hakkında daha fazla bilgi için bu Yardım konusunun devamındaki bölümüne bakın.

- Teklif türü, Iş ortağı merkezi veya Azure portal (örn. kapsayıcılar veya bazı kullanım tabanlı teklifler) üzerinden transactable olamaz.

- İlişkili müşterilerinizin faturalandırma ülkesi bu ISV teklifi için desteklenmiyor olabilir.

## <a name="view-marketplace-offers-in-partner-center"></a>Market tekliflerini Iş Ortağı Merkezi 'nde görüntüleyin

Kullanılabilir ticari Market tekliflerini CSP programında görüntülemek için:

1. Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın ve ardından sol gezinti menüsünden **CSP** ' yi seçin.

2. **Satış** ve ardından **Market**' i seçin. Varsayılan olarak, tüm türlerin ve kategorilerin ürünlerini görürsünüz.

3. Türe veya kategoriye göre bir filtre seçin. Ayrıca, belirli anahtar sözcükleri, teklif adlarını veya ISV yayımcılarının adlarını bulmak için **Ara** ' yı kullanabilirsiniz.

4. Listeden belirli bir ürün teklifi seçin. Bu, size teklif hakkında daha fazla bilgi oluşturabileceğiniz bir ürün genel bakış sekmesine götürür. Bu sekmeyle ilgili bilgiler şunları içerebilir: 

    - Ürün veya teklifin açıklaması

    - ISV yayımcısı hakkında daha fazla bilgi

    - ISV yayımcısı tarafından karşıya yüklenen belgelerin veya pazarlama malzemelerinin bağlantıları

    - Müşteri desteği, mühendislik veya CSP programına yönelik bir iletişim için olası diğer ISV kişileri

5. Bir teklifin kullanılabilir planları, SKU 'Ları veya fiyatlandırma hakkında daha fazla bilgi için **planlar + fiyatlandırma** sekmesini seçin. Bu sekmede şu görünür:

    - Bu teklifin sizin için kullanılabildiği pazarlar

    - Teklif için kullanılabilir SKU 'Ların veya planların listesi

    - Her SKU veya plana ilişkin fiyatlandırma

## <a name="view-marketplace-offers-via-partner-center-apis"></a>Market tekliflerini Iş Ortağı Merkezi API 'Leri aracılığıyla görüntüleme

CSP Program ortakları, uygun tekliflerin bir listesini döndürmek için API 'Leri de kullanabilir. Uygun teklifler yalnızca iş ortağının Partner Center Marketi aracılığıyla satıtabilecekleri SaaS ISV teklifleri olacaktır. Katalogdaki teklifleri tanımlamak üzere API 'Leri kullanan iş ortakları için, [bir pazara yönelik tekliflerin bir listesini elde etme](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)kılavuzuna bakın.

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>Iş Ortağı Merkezi 'nde en son Market teklif fiyatlandırmasını görüntüleme

Teklifle ilişkili en son fiyatlandırma ayrıntıları için aşağıdaki adımları izleyin:

1. Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın ve ardından sol gezinti menüsünden **CSP** ' yi seçin.

2. **Satış**' yı, ardından **fiyatlandırma ve tekliflerle** seçin.

3. **Market** bölümüne gidin, bir konum seçin ve **Market fiyatlandırmasını** indirin. Bu, ISV yayımcılarından sunulan SaaS, lisans tabanlı teklifler ve tarifeli tekliflerle ilgili en son fiyatlandırma verilerine sahip bir elektronik tablo oluşturur. Burada bazı Azure uygulama fiyatları da görüntülenebilir. Bu bilgiler günlük olarak güncelleştirilir, bu sayede seçtiğiniz sıklıkta geçerli fiyatlar için kontrol edebilirsiniz.

4. Bir ISV ürünü ücretsiz deneme süresi içeriyorsa, bu ürün için iki satır görüntülenir:

    - Bir satırda, sıfır olan ücretsiz deneme fiyatı gösterilmektedir. Bu, ücretsiz deneme süresinin kullanılabildiği anlamına gelir.

    - Diğer satır, ücretsiz deneme süresi bittikten sonra uygulanacak fiyat ve koşulları gösterir.

CSP program ortağı olarak, belirli ticari Market tekliflerle ilişkili diğer teşvikleri için uygun olabilirsiniz. Diğer teşvikleri hakkında daha fazla bilgi için bkz. [CSP özeni Kılavuzu](https://aka.ms/partnerincentives) (CSP oturumu gerektirir).

## <a name="learn-about-marketplace-exclusive-offers"></a>Market özel teklifleri hakkında bilgi edinin

ISV 'Ler, tekliflerini yalnızca CSP programındaki belirli iş ortakları için kullanılabilir hale getirme seçeneğine sahiptir. Bu, özel bir teklif olarak bilinir. CSP programındaki tüm iş ortakları, özel olarak işaretlenmiş teklifler de dahil olmak üzere Iş ortağı merkezi ticari Market 'teki tüm ISV tekliflerini hala görüntüleyebilir.

Bir teklif özel olarak **işaretlenmediğinde** , tüm iş ortakları bu teklifi satın alabilir (Seçili müşterinin faturalandırma ÜLKESI, ISV teklifinin ülke kullanılabilirliği ile eşleştiğinde).

Ancak özel olarak işaretlenmiş tüm teklifler için, yalnızca ISV tarafından seçilen iş ortakları bu teklifi satın alabilir.

> [!NOTE]
> Müşterilerinize satmak istediğiniz özel olarak işaretlenmiş bir teklif görürseniz, doğrudan ISV 'ye ulaşın ve özel teklifi satma izni isteyin. Özel bir teklifin ayrıntılarını görüntülediğinizde seçebileceğiniz bir **ILETIŞIM ISV** bağlantısı görürsünüz.

Ticari Market 'teki ISV deneyimi hakkında daha fazla bilgi edinmek için, [bulut çözümü sağlayıcılarını](/azure/marketplace/cloud-solution-providers)okuyun.

Market 'teki CSP deneyimi hakkında daha fazla bilgi için [ticari Market 'e genel bakış](csp-commercial-marketplace-overview.md)makalesini okuyun.

## <a name="next-steps"></a>Sonraki adımlar

- [Ticari Market tekliflerini satın alma](csp-commercial-marketplace-purchase.md)