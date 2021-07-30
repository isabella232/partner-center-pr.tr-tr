---
title: Microsoft ürünleriyle müşterilerin deneme sürümlerini sunun
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Müşterilerin Microsoft abonelik ürünlerini 30 gün boyunca denemesini sağlayın. Diğer pek çok çevrimiçi hizmetler gibi, katalogdaki bu ücretsiz denemelerle kaydolun.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 393bd70096ba3cd7d1c9889d5b521cc94a389d90
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114845984"
---
# <a name="give-customers-30-day-free-trials-of-microsoft-products"></a>Müşterilere 30 günlük ücretsiz Microsoft ürünlerinin ücretsiz deneme sürümü verin

**Uygun roller**: genel yönetici | Kullanıcı Yönetimi Yöneticisi | Satış Aracısı

Yeni Microsoft ürünlerine müşterileri tanıtmak için iyi bir yöntem, 30 günlük ücretsiz deneme sunmaya yönelik bir yoldur. Diğer birçok çevrimiçi hizmetler benzer şekilde katalogdaki denemelerle kaydolabilirsiniz. Tüm iş ortakları katılabilirler.

## <a name="available-trial-offers"></a>Kullanılabilir deneme teklifleri

Bekleyen deneme tekliflerinizin tümünü **Müşteri** sayfasında bulabilirsiniz. Bu sayfa, ücretsiz denemeler ve ücretli abonelikler dahil olmak üzere tüm abonelikleri listeler. (Bu özellik şu anda Çin 'de kullanılamaz.)

Her müşteri, kullanılabilir her teklif için bir ücretsiz denemeye hak kazanır. örneğin, Office 365 E3 için bir ücretsiz deneme Microsoft 365 İş Standart ve ücretsiz deneme sürümü alabilirler. Ancak müşteri teklifi zaten kullanıyorsa, bu teklif için ücretsiz deneme kullanamaz.

### <a name="available-products"></a>Kullanılabilir ürünler

Ücretsiz denemeler, daha kapsamlı ve popüler licesen tabanlı teklifler için kullanılabilir. Yeni deneme teklifleri aylık olarak ortaya çıkabilir.

İş ortakları, Iş Ortağı Merkezi 'nde **fiyatlandırma ve teklifler** sayfasındaki aylık fiyat listesinde denemeleri bulabilir. Deneme tekliflarında, Fiyat listesi **Ikincil lisans türü** sütununda "deneme" listelenir.

Şu anda kamu teklifleri, eğitim teklifleri veya eklenti teklifleri için **ücretsiz deneme** yoktur.

## <a name="licenses-for-free-trial-offers"></a>Ücretsiz deneme teklifleri için lisanslar

Tüm ücretsiz denemeler 25 lisans sağlar. Deneme sırasında bu numarayı değiştiremezsiniz. Ücretsiz deneme sürümünde lisans ekleyemez veya kaldıramazsınız. Deneme sürümü ücretli aboneliğe dönüştürüldükten sonra aboneliğe daha fazla lisans ekleyebilirsiniz.

Deneme lisansları, ücretli hizmetler lisansının atandığı şekilde kullanıcılara atanmalıdır.

## <a name="sign-customers-up-for-trials"></a>Deneme için müşterileri imzalayın

Iş Ortağı Merkezi 'nde müşteriniz için bir deneme sürümü alın:

1. Iş Ortağı Merkezi 'nin **satışlarından** , **Katalog**' a gidin. 
2. Katalogda **faturalandırma sıklığından** **deneme teklifi**' ni seçin. Bu, yalnızca ücretsiz denemelerin görünmesine olanak sağlar ve ücretsiz olmayan diğer teklifleri devre dışı bırakır. Denemeler, katalogdaki **denemeler** sekmesinde görünür.
3. Sunmak istediğiniz ücretsiz denemeyi seçin ve ardından **Gönder**' i seçin. Tüm denemeler, faturalandırılmayacak 30 gün boyunca yapılır. Ayrıca, deneme süresi boyunca istediğiniz zaman ücretli aboneliğe dönüştürebilirsiniz.

## <a name="converting-trials-to-paid-subscriptions"></a>Denemeleri ücretli aboneliklere dönüştürme

Ücretsiz deneme, ücretli aboneliğe otomatik olarak dönüştürülmez. 30 gün sonra, ücretsiz deneme süresi ücretli aboneliğe dönüştürülmelidir, bu da [sona erer](#expiring-offers). Ücretsiz denemeler genişletilemiyor.

Denemeyi ücretli aboneliğe kendiniz dönüştürmeniz gerekir. Bunu [Iş Ortağı Merkezi](#convert-trials-using-partner-center) 'Ni veya [Iş Ortağı Merkezi API 'leri aracılığıyla](#convert-trials-using-apis)yapabilirsiniz.

> [!NOTE]
> Bulut Çözümü Sağlayıcısı (CSP) programı için müşteri ücretsiz denemeleri başka bir program kiracısına dönüştürülemez (EA, Open veya mosp gibi).

### <a name="convert-trials-using-partner-center"></a>Iş ortağı merkezini kullanarak denemeleri dönüştürme

Deneme sürümlerini, Iş Ortağı Merkezi 'ni kullanarak ücretli aboneliklere dönüştürebilirsiniz:

1. Müşterinin abonelik sayfasına gidin ve ücretsiz denemeyi seçin.
2. **Denemeyi ücretli aboneliğe Dönüştür**' ü seçin.
3. İstenen lisans miktarını ve faturalama sıklığını girip **Uygula**' yı seçin.
4. Ücretli abonelik için faturalandırma, dönüştürme tarihinde başlar ve abonelik, dönüştürme tarihinden itibaren 12 ay otomatik olarak yenilenir. 

### <a name="convert-trials-using-apis"></a>API 'Leri kullanarak denemeleri dönüştürme

Ücretsiz deneme sürümünün ücretli aboneliğe dönüştürülmesine uyum sağlamak için API 'lerinizi değiştirmeniz gerekebilir. Daha fazla bilgi için aşağıdaki geliştirici belgelerine bakın:

- [Deneme aboneliğini ücretli aboneliğe dönüştürme](/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Deneme dönüştürme tekliflerinin bir listesini alma](/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="trials-without-conversions"></a>Dönüşümler olmadan denemeler

Tüm denemeler, ücretli aboneliklere dönüştürülemez. İş ortakları, sona erme tarihine kadar dönüştürmesiz bir deneme kullanabilir. İş ortakları, deneme teklifiyle aynı hizmetleri destekleyen uyumlu teklifler satın alabilir.  Bu, yeni satın alınan tekliflerin hizmetlerinin deneme hizmetleriyle aynı şekilde hizalanmasını sağlamak için deneme süresi dolmadan önce gerçekleştirilmelidir. 

|**Deneme**   |**Uyumlu küçük Işletme teklifleri**   |**uyumlu Enterprise teklifleri**   |
|----------------------------|:---------------------------------|:------------------------------------------|
|Microsoft Teams Ticari bulut (Kullanıcı tarafından başlatılan) denemesi   |Microsoft 365 İş Temel, Microsoft 365 İş Standart, Microsoft 365 İş Ekstra   | F3 (eski adıyla F1), Enterprise için Office 365 (E1, E3 ve E5), Microsoft 365 F1/f3, Microsoft 365 Kurumsal (E3)   |

>[!NOTE]
>Yukarıdaki teklifler benzer işlevlerle benzer hizmet planlarına sahiptir, ancak teklifler arasında bazı farklılıklar olabilir.

### <a name="expiring-offers"></a>Süresi dolan teklifler

Süresi dolan tekliflerle bilgilendirilmeyecektir. Gelecek süre sonu tarihlerini, Iş Ortağı Merkezi 'nde müşteri görünümünü kullanarak veya API 'yi sorgulayarak izleyebilirsiniz. Bu tarihleri sıklıkla izlemek iyi bir fikirdir. böylece, bir karar noktasına yaklaşımında müşterilerle ilgili izleme eylemlerini gerçekleştirebilirsiniz.

Deneme süresi dolduktan sonra, bu deneme sürümünde oturum açmayı deneyen bir müşteri bir süre sonu iletisi görür. Ancak, veriler veri saklama standartları ile birlikte kaydedilir. Aynı hizmet planlarına sahip yeni bir abonelik satın aldıktan sonra, müşterinizin bilgilerine yeni etkinleştirilen abonelikten tekrar erişilebilir.

## <a name="billing"></a>Faturalandırma

Yıllık faturalandırma ve ücretsiz denemeler, bağımsız bulutlarda ve genel bulutta aynıdır. Tek fark, başlatma sırasında sunulan deneme SKU 'larıyla aynıdır.

## <a name="billing-for-free-trials"></a>Ücretsiz deneme için faturalandırma

Ücretsiz denemeler, aylık ve yıllık olarak faturalandırılan abonelikler için kullanılabilir. Denemeyi ücretli bir aboneliğe dönüştürdüğünüzde faturalandırma sıklığını seçebilirsiniz.

Abonelik başlangıç tarihi, dönüştürme tarihini temel alır. Ücretsiz deneme yıllık faturalandırmayla ücretli bir teklifine dönüştürülürse, abonelik yenileme tarihi dönüştürme tarihinden itibaren 12 ay olur. Ücretsiz deneme, aylık faturalandırma ile ücretli bir teklifine dönüştürülürse, abonelik yenileme tarihi, dönüştürme tarihinden sonraki fatura tarihinden itibaren on iki ay olacaktır.

### <a name="invoices"></a>Faturalar

Faturanızda veya lisans tabanlı mutabakat dosyanızda listelenen ücretsiz denemeleri göremezsiniz. Ücretsiz denemeler, ücretsiz bir denemeyi ücretli aboneliğe dönüştürdükten sonra faturanızda ve lisans tabanlı mutabakat dosyanızda görüntülenir. Dönüştürülen abonelik, yeni abonelikle aynı şekilde görünür.

### <a name="incentives"></a>Teşvikler

Ücretsiz denemelerdeki teşvikleri üzerinde bir etkisi yoktur.

## <a name="support"></a>Destek

Ücretsiz denemelerdeki destek için Iş Ortağı Merkezi aracılığıyla bir hizmet isteği gönderebilirsiniz.