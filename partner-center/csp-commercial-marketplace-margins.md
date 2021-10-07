---
title: Kenar boşluklarını bul-ticari Market
ms.topic: how-to
ms.date: 10/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Bulut Çözümü Sağlayıcısı (CSP) iş ortaklarının bağımsız yazılım satıcıları (ısv 'ler) tarafından yapılandırılan kenar boşluklarını öğrenmek için iş ortağı merkezini nasıl kullanabileceğinizi öğrenin.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8d7b5f077b3ea3f98f87121634427842db0a0f03
ms.sourcegitcommit: 77737d8f986a1afb3d923c130936e2f73ce07879
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/07/2021
ms.locfileid: "129661394"
---
# <a name="discover-margins-configured-by-independent-software-vendors-isvs"></a>Bağımsız yazılım satıcıları (ISV) tarafından yapılandırılan kenar boşluklarını bulma

**Uygun roller**: genel yönetici | Faturalandırma Yöneticisi | Yönetici Aracısı | Satış Aracısı | Yardım Masası Aracısı

Bağımsız yazılım satıcıları (ISV 'Ler), belirli bulut çözümü sağlayıcıları (CSP 'Ler) için bazı ticari Market teklifleri için kenar boşluğu iskontoları sunabilir. Bu kenar boşlukları, bu teklifleri müşterilerine satmak için CSP incentivize.

> [!NOTE]
> ISV 'den CSP kenar boşluğu iskontoları özelliği şu anda **genel önizleme** olarak sunulmaktadır. geri bildirimde bulunmak ve deneyimleri geliştirmek için devam ediyoruz.

## <a name="notes-about-the-public-preview"></a>Genel önizleme hakkında notlar

ISV 'den CSP kenar boşlukları özelliği, ISV 'nin belirli CSP 'lere hedeflenen indirimler oluşturmasını sağlar. Bu özellik şu anda kullanılabilir ancak genel önizleme aşamasındadır. Bu, genel CSP marketi deneyimlerini iyileştirmeye devam ederken özelliğin tamamen işlevsel ve kullanılabilir olduğu anlamına gelir. İş ortağı deneyimini geliştirdiğimiz için özellik artık önizleme aşamasında değil olarak bildirilecektir. Bu için belirli zaman çizelgeleri yoktur ve CSP Iş ortakları, olduğu gibi iskontolar özelliğini kullanmaya devam edebilir.

### <a name="public-preview-improvement-areas"></a>Genel Önizleme geliştirme alanı

- AppSource teklif kullanılabilirliği: bazı CSP Marketi teklifleri, birincil olarak AppSource tekliflerini, tümleştirme ve Iş Ortağı Merkezi 'nde kullanılabilir hale getirmek için daha fazla zaman alır. Bazı iş ortakları AppSource tekliflerini arıyor, ancak kullanılabilir hale gelene kadar beklemeniz gerekebilir. Iş Ortağı Merkezi ekibinin süresi, bir ISV 'nin teklif oluşturduğu ve kullanılabilir olduğu zaman arasındaki gecikme süresi ile ilgili iyileştirmeler gerçekleştirmeyecektir.
- Kenar boşlukları, CSP marketi Ürün SKU 'SU için yüzde indirim olarak tanımlanmıştır. İleri sarma, Fiyat noktasını gelecekteki fiyat listeleriyle tümleştirmek için ASP 'ler vardır. Bu gerçekleşene kadar, iş ortakları, Ürün SKU 'sunu (ve ilişkili API 'Ler), market fiyat listesi Ürün SKU 'Larını tahmin ücretlerine kadar değiştirebilir.
- Deneme sürümü etkin olan bazı Market teklifleri, kenar boşluğu indirimlerine göre değil, Market 'e yönelik tarama deneyiminde **$. 00** miktarları olarak gösterilir. İş ortakları, bu denemelerin, dönem sonunda ücretli tutarlarla yenilediğini anlamak için dikkatli olmalıdır. 
- Özel teklifler, iş ortakları tarafından kullanılabilir. Bunlar şu anda market fiyat listelerinde değil. Bu olana kadar, iş ortaklarının fiyatlandırma için istedikleri ürüne yönelik Market tarama deneyimini kullanarak fiyatlandırma için fiyatlandırma bulması gerekir.

## <a name="view-margins-in-partner-center"></a>Iş Ortağı Merkezi 'nde kenar boşluklarını görüntüleme

Bir CSP, kenar boşlukları sayfasında ISV 'Ler için yapılandırılmış olan kenar boşluklarını görüntüleyebilir:

> [!NOTE]
> Çalışma alanları arabirimi hakkında daha fazla bilgi edinmek için bkz. [Iş ortağı merkezini alma](get-around-partner-center.md#turn-workspaces-on-and-off).

#### <a name="workspaces-view"></a>[Çalışma alanları görünümü](#tab/workspaces-view)

1. Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard) oturum açın ve **fiyatlandırma** kutucuğunu seçin.

2. **Kenar boşluklarını** seçin. İş ortakları, ISV 'lerin için kenar boşluklarını yapılandırmakta olan market tekliflerinin bir listesini görür.

3. CSP iş ortakları, kullanılabilir kenar boşluklarının listesine gözatabilir veya verileri virgülle ayrılmış bir biçimde **indirebilir** .

#### <a name="current-view"></a>[Geçerli görünüm](#tab/current-view)

1. Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın ve ardından sol gezinti menüsünden **CSP** ' yi seçin.

2. **Satışı** ve ardından **kenar boşlukları**' nı seçin. İş ortakları, ISV 'lerin için kenar boşluklarını yapılandırmakta olan market tekliflerinin bir listesini görür.

3. CSP iş ortakları, kullanılabilir kenar boşluklarının listesine gözatabilir veya verileri virgülle ayrılmış bir biçimde **indirebilir** .

* * *

## <a name="margins-overview"></a>Kenar boşluklarına genel bakış

CSP Iş ortaklarıyla ilişki kurdu olan ISV 'Ler, teklifleri müşterilerine satmak için CSP Iş ortağı incentivize için kenar boşluğu iskontoları sunmak isteyebilir. Bu durumlarda, CSP Iş ortağı genellikle ISV ile bir kenar boşluğu üzerinde anlaşır veya ISV, CSP Iş ortağıyla danışmadan bir kenar boşluğu sağlayabilir. ISV, lisans tabanlı ya da tüketim tabanlı tekliflerle ilgili bir kenar boşluğu sunabilir. Tüketim tabanlı kenar boşlukları yalnızca ISV ürünleri için geçerlidir, ISV ürününün sizinle birlikte çalıştığı herhangi bir Azure tüketim ürününe uygulanmaz.

## <a name="margins-and-pricing"></a>Kenar boşlukları ve fiyatlandırma

Iş ortağı merkezi market fiyat listesi, tekliflere yönelik orijinal CSP fiyatlandırmasını içerir. CSP marketi fiyat listeleri tüm iş ortakları genelinde paylaşılır ve perakende fiyatlandırması içerir. İş ortakları daha sonra satın alınmadan önce maddenin son fiyatını anlamak üzere satın almak istedikleri Ürün SKU 'SU için marj yüzdesi iskontosunu uygular. CSP iş ortakları ayrıca Azure portal (yalnızca tüketim tabanlı ürünler için) aracılığıyla Azure fiyat listesi 'nde perakende fiyatlandırmasına da sahip olur. Ayrıca, bu fiyat sayfasında, bunlara genişletilmiş kenar boşluğunun ayrıntılarını görürler. 

## <a name="purchasing-offers"></a>Satın alma teklifleri

CSP iş ortakları, [Iş Ortağı Merkezi](https://partner.microsoft.com) 'nde Market Teklifini satın alarak veya ürünü Microsoft [Azure Portal](https://portal.azure.com)dağıtarak yapılandırılmış kenar boşluklarını elde edin. Deneyimidir iş ortağı, başka bir adım almak zorunda kalmadan kenar boşluğu iskontosunu alacaktır. ISV bunu CSP için yapılandırdıysa iş ortakları kenar boşluklarını devre dışı bırakılamaz.

Kenar boşlukları, iş ortağının yürütüldüğü ve müşterilerinin herhangi birine uygulanan tüm işlemler için geçerlidir. CSP Iş ortağının bir teklifi kabul etmesi ve bir ISV teklifine yönelik yükümlülüğü olmaması gerekmez, ancak bunları bir kenar boşluğu varsa otomatik olarak uygulanır. 

## <a name="margins-and-indirect-resellers"></a>Kenar boşlukları ve dolaylı satıcılar

Kenar boşlukları yalnızca Microsoft tarafından faturalanan iş ortakları tarafından, dolaylı sağlayıcılar ve doğrudan fatura ortakları gibi deneyimidir iş ortakları tarafından kullanılabilir hale getirilir. ISV dolaylı bir satıcıya doğrudan bir kenar boşluğu sağlayamaz, ancak dolaylı sağlayıcı, dolaylı satıcı aracılığıyla bir kenar boşluğu geçirmeye karar verebilir. Dolaylı sağlayıcılar, kenar boşluklarını dolaylı satıcılarına geçirmeye tercih edebilir, ancak yükümlülüğü yoktur. 

## <a name="terms-and-billing"></a>Hüküm ve faturalandırma

İş ortakları, Azure portal Azure maliyet yönetimi özelliklerini kullanarak, tüketim tabanlı teklifler için kenar boşluğunun uygulandığını doğrulayabilirler. İş ortakları, faturalandırma döngüsünün sonunda mutabakat dosyasını inceleyerek, bu marjın lisans tabanlı tekliflere uygulandığını doğrulayabilirsiniz.

Her kenar boşluğunda başlangıç ve bitiş tarihi vardır. Marj indirimine dayalı fiyat azaltma, satın alma terimine uygulanır. Bir iş ortağı, kenar boşluğu ile yeni bir terim almak için terimlerinden sonra aynı teklifi yeniden alabilir. Yenilemeler kenar boşluğunun başlangıç ve bitiş tarihleri içinde gerçekleşdiğinde, bu kenar boşluğunu uygular. Bir kenar boşluğunun bitiş tarihleri her zaman ayın sonuna hizalanır. 

## <a name="margins-for-metered-billing"></a>Ölçülen faturalandırma için kenar boşlukları

Bazı CSP ürünleri, tarifeli faturalandırma ile gelir. CSP iş ortağı, ölçülen faturalandırmayla ilgili olarak herhangi bir teklifi artırdığı takdirde, ücretlerden oluşan Yetkilendirme tabanlı bölüm fiyatlandırması, yıllık abonelik döneminin sonuna kadar iskontoyu korur, ancak ölçülen faturalandırma fiyatına uygulanan kenar boşluğu, kenar boşluğunun bitiş döneminden sonra korunmaz. Buradaki geçici çözüm, ISV 'Lerin, abonelik döneminin sonuna kadar söz konusu CSP iş ortağı için yeni bir kenar boşluğu oluşturmasına yöneliktir. 

## <a name="margins-notifications"></a>Kenar boşlukları bildirimleri

ISV, CSP ile e-posta üzerinden iletişim kurmadığı ve bir kenar boşluğu genişlettikleri takdirde öngörülü bir bildirim yoktur. CSP iş ortağı, Iş ortağı merkezindeki kenar boşlukları sekmesinden kullanılabilen tüm kenar boşluklarını görüntüleyebilecektir.   

### <a name="recon-files"></a>Keşfi dosyaları

CSP iş ortağı, oluşturulduktan sonra **yinelenen ve tek seferlik** satın alma keşfi dosyasında genişletilmiş kenar boşluklarının ayrıntılarını bulur. Kenar boşluklarını açıklamak için keşfi dosyasındaki önemli veriler:

- BirimFiyat, ISV tarafından ayarlanan fiyata göre kalır.  

- Bir efekt, kenar boşluğu uygulandıktan sonra fiyat gösterir.  

- PriceAdjustmentDescription, CSP ortağına bir kenar boşluğunun ne kadarının sağlandığını ayrıntılı olarak içerir. 

## <a name="discover-and-operationalize-margins-using-the-partner-center-apis"></a>Iş Ortağı Merkezi API 'Lerini kullanarak kenar boşluklarını bulma ve kullanma

İş ortakları, kullanılabilir kenar boşluklarını görüntülemek veya dışarı aktarmak için Iş Ortağı Merkezi Kullanıcı arabirimini ya da API 'Leri kullanabilir.

### <a name="apis-to-retrieve-margins"></a>Kenar boşluklarını almak için API 'Ler

İş ortakları aşağıdaki API 'Leri çağırarak verileri çalıştırabilirsiniz. Bu API 'lerin her biri, ortağın ISV tarafından tanımlanan bir kenar boşluklarının listesini döndürür. Her iki API de aynı verileri döndürür.

- [Get kenar BOŞLUKLARı](/partner-center/develop/get-margins) API sonuç biçimindeki verileri döndürüyor

- [Indirme kenar boşlukları](/partner-center/develop/download-margins) , verileri virgülle ayrılmış bir biçimde döndürür

### <a name="apis-to-discover-marketplace-offers"></a>Market tekliflerini bulmaya yönelik API 'Ler

CSP Program ortakları, API 'Leri tarafından kullanılabilen kenar boşluklarının bir listesini döndürmek için de kullanabilir. Uygun teklifler yalnızca iş ortağının Partner Center Marketi aracılığıyla satıtabilecekleri SaaS ISV teklifleri olacaktır. İş ortakları, [pazara yönelik tekliflerin bir listesini alarak](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)Market SaaS tekliflerinin bir listesini alabilir.

CSP iş ortakları, transactable hizmet olarak yazılım (SaaS) tekliflerinin listesini çekmek ve müşterileri için sipariş göndermek üzere Iş Ortağı Merkezi API 'Lerini kullanabilir. Daha fazla bilgi için bkz. [ticari Market ürünleri için abonelik oluşturma](/partner-center/develop/create-subscription-azure-marketplace-products).

CSP iş ortakları, tüm Market tekliflerini görüntülemek için Azure portal UX kullanabilir. Market VM tekliflerinin listesini çekmek ve müşterileri için sipariş göndermek üzere aşağıdaki API 'Leri kullanabilirler.  
- [VM 'ler: VM 'lerin bir listesini alın API 'Ler sunar](/azure/virtual-machines/windows/cli-ps-findimage)
- [VM 'Ler: satın alma API 'Leri (CLı, PowerShell, ARM)](/azure/virtual-machines/linux/quick-create-cli) 

Azure portal için bir filtre yoktur, bu teklif için CSP aracılığıyla satılmasını tercih edilir. İş ortaklarının, hangi tekliflerin CSP aracılığıyla işlem kullanabileceğini anlamak için fiyat listesini gözden geçirmesi gerekir. Şu anda Transact SaaS veya yönetilen uygulama Marketi teklifleri için kullanılabilir Azure portal API yok. 

Market 'teki CSP deneyimi hakkında daha fazla bilgi için [ticari Market 'e genel bakış](csp-commercial-marketplace-overview.md)makalesini okuyun.

## <a name="next-steps"></a>Sonraki adımlar

- [Ticari markete genel bakış](csp-commercial-marketplace-overview.md)
- [Ticari Market tekliflerini satın alma](csp-commercial-marketplace-purchase.md)
- [CSP teşvik Kılavuzu](https://aka.ms/partnerincentives)
