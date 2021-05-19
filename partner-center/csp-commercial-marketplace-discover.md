---
title: Teklifleri bulma-ticari Market
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP iş ortaklarının, bağımsız yazılım satıcılarından (ISV) SaaS teklifleri veya fiyatlandırma için Market 'i görüntülemek veya aramak üzere Iş ortağı merkezini nasıl kullanabileceği hakkında bilgi edinin.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ab30f8391df58155c8511dc628b1fefd94c8d768
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147981"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a>Partner Center ticari marketi 'nde teklifleri ve fiyatları bulma

**Uygun roller**: genel yönetici | Yönetim Aracısı

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

4. Listeden belirli bir ürün teklifi seçin. Bu sizi teklif hakkında daha fazla bilgi edinmek için bir ürüne Genel Bakış sekmesine alır. Bu sekmede yer alan bilgiler şunlar olabilir: 

    - Ürün veya teklif açıklaması

    - ISV yayımcısı hakkında daha fazla bilgi

    - ISV yayımcısı tarafından karşıya yüklenen belgelere veya pazarlama malzemelerine bağlantılar

    - Müşteri desteği, mühendislik veya CSP programıyla ilgili bir iletişim için diğer olası ISV kişileri

5. Bir teklifin kullanılabilir planları, SKU'ları veya fiyatlandırması hakkında daha fazla bilgi için Planlar **+ Fiyatlandırma sekmesini** seçin. Bu sekme size şunları gösterir:

    - Bu teklifin kullanılabilir olduğu pazarlar

    - Teklif için kullanılabilen SKUS'ların veya planların listesi

    - Kullanılabilir her SKU veya Plan için fiyatlandırma

## <a name="view-marketplace-offers-via-partner-center-apis"></a>İş Ortağı Merkezi API'leri aracılığıyla Market tekliflerini görüntüleme

CSP programı iş ortakları uygun tekliflerin listesini almak için API'leri de kullanabilir. Uygun teklifler yalnızca iş ortağının market üzerinden satışa sunduğu SaaS ISV İş Ortağı Merkezi olur. Katalogda teklifleri belirlemek için API'leri kullanan iş ortakları için pazara yönelik [tekliflerin listesini almak için rehbere bakın.](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>En son Market teklifi fiyatlandırması bilgilerini İş Ortağı Merkezi

Teklifle ilişkili en son fiyatlandırma ayrıntıları için şu adımları izleyin:

1. Panoda İş Ortağı Merkezi [açın](https://partner.microsoft.com/dashboard)ve ardından sol gezinti **menüsünden CSP'yi** seçin.

2. **Satış'ı** ve ardından Fiyatlandırma **ve teklifler'i seçin.**

3. Sayfayı aşağı kaydırarak **Market** bölümüne gidin, bir konum seçin ve Market **fiyatlandırması'ı indirin.** Bu, ISV yayımcılarının sunduğu SaaS, lisans tabanlı teklifler ve tarifeli teklifler için en son fiyatlandırma verilerini içeren bir elektronik tablo oluşturulur. Bazı Azure uygulama fiyatlandırması da burada görünebilir. Bu bilgiler günlük olarak güncelleştirilir, bu nedenle seçtiğiniz sıklıkta geçerli fiyatları kontrol edin.

4. IsV ürünü ücretsiz deneme süresine sahipse elektronik tabloda bu ürün için iki satır görüntülenir:

    - Bir satırda ücretsiz deneme fiyatı sıfır olarak gösterir. Bu, ücretsiz deneme süresi olduğu anlamına gelir.

    - Diğer satırda, ücretsiz deneme süresi sona erdikten sonra uygulanacak fiyat ve koşullar yer atılır.

CSP programı iş ortağı olarak, belirli ticari market teklifleriyle ilişkili diğer teşvikler için uygun olabilirsiniz. Diğer teşvikler hakkında daha fazla bilgi için CSP teşvik [kılavuzuna](https://aka.ms/partnerincentives) bakın (CSP oturum açması gerekir).

## <a name="learn-about-marketplace-exclusive-offers"></a>Markete özel teklifler hakkında bilgi alın

ISV'ler tekliflerini yalnızca CSP programında belirli iş ortakları tarafından kullanılabilir yapma seçeneğine sahip. Bu, Özel teklif olarak bilinir. CSP programıyla tüm iş ortakları, Özel olarak işaretlenen teklifler de dahil İş Ortağı Merkezi ticari markette tüm ISV tekliflerini görüntülemeye devam ediyor.

Bir teklif Özel **olarak** işaretlenmemişse, tüm iş ortakları bu teklifi satın alır (seçilen müşterinin fatura ülkesi ISV'nin teklifinin ülke kullanılabilirliğiyle eş olduğu varsayıldı).

Ancak Özel olarak işaretlenen tüm tekliflere yalnızca ISV tarafından seçilen iş ortakları bu teklifi satın alma seçeneğine sahip olur.

> [!NOTE]
> Müşterilerinize satış yapmak için Özel olarak işaretlenmiş bir teklif görüyorsanız doğrudan ISV'ye ulaşıp Özel teklifin satış iznini istemeniz gerekir. Özel bir teklifin ayrıntılarını görüntülenin, seçerek bir **Kişi ISV** bağlantısıyla karşıdan ulaşabilirsiniz.

Ticari markette ISV deneyimi hakkında daha fazla bilgi edinmek için Bulut Çözümü Sağlayıcıları [makalelerini okuyun.](/azure/marketplace/cloud-solution-providers)

Markette CSP deneyimi hakkında daha fazla bilgi için Ticari markete [genel bakış makalelerini okuyun.](csp-commercial-marketplace-overview.md)

## <a name="next-steps"></a>Sonraki adımlar

- [Ticari market tekliflerini satın alma](csp-commercial-marketplace-purchase.md)