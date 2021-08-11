---
title: Müşterilere Microsoft ürünlerinin denemelerini sun
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Müşterilerin Microsoft abonelik ürünlerini 30 gün boyunca denemesine izin verme. Diğer birçok denemede olduğu gibi katalogda bu ücretsiz denemelere çevrimiçi hizmetler.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 01234eaf64beaceb0b5511c64013a67196a71b95121fe1bd831ffa93ea19054f
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115687035"
---
# <a name="give-customers-30-day-free-trials-of-microsoft-products"></a>Müşterilere Microsoft ürünlerinin 30 günlük, ücretsiz denemelerini verme

**Uygun roller:** Genel yönetici | Kullanıcı yönetimi yönetici | Satış aracısı

Müşterileri yeni Microsoft ürünleriyle tanıtmanın iyi bir yolu, 30 günlük ücretsiz denemeler sunmaktır. Diğer birçok denemede olduğu gibi katalogda denemeler için çevrimiçi hizmetler. Tüm iş ortakları katılabilir.

## <a name="available-trial-offers"></a>Kullanılabilir deneme teklifleri

Bekleyen deneme tekliflerinizi müşteri sayfasında **bulabilirsiniz.** Bu sayfada ücretsiz denemeler ve ücretli abonelikler dahil olmak üzere tüm abonelikler listeleyebilirsiniz. (Bu özellik şu anda Çin'de kullanılamaz.)

Her müşteri, kullanılabilir her teklif için bir ücretsiz deneme hakkına sahip. Örneğin, Microsoft 365 İş Standart için bir ücretsiz deneme ve Office 365 E3. Ancak, teklif müşteri tarafından zaten sahibi ise, bu teklif için ücretsiz denemeyi kullanamıyr.

### <a name="available-products"></a>Kullanılabilir ürünler

Daha kapsamlı ve popüler licesen tabanlı teklifler için ücretsiz denemeler kullanılabilir. Yeni deneme teklifleri aylık olarak tanıtabilirsiniz.

İş ortakları, aylık fiyat listesinde denemeleri fiyatlandırma ve **teklifler sayfasında** bulabilirsiniz İş Ortağı Merkezi. Deneme teklifleri, İkincil Lisans Türü sütunundaki fiyat listesinde **"DENEME" olarak listelenir.**

Şu anda kamu **teklifleri, eğitim** teklifleri veya eklenti teklifleri için ücretsiz denemeler yoktur.

## <a name="licenses-for-free-trial-offers"></a>Ücretsiz deneme teklifleri için lisanslar

Tüm ücretsiz denemeler 25 lisans sağlar. Deneme süresi boyunca bu s numarayı değiştiremezsiniz. Ücretsiz deneme sürümüne lisans ekli veya kaldıraaz. Deneme sürümü ücretli aboneliğe dönüştürüldikten sonra aboneliğe daha fazla lisans abilirsiniz.

Deneme lisansları, ücretli hizmetler lisansının atandığı şekilde kullanıcılara atanabilir.

## <a name="sign-customers-up-for-trials"></a>Denemeler için müşterileri kaydolma

Şu hizmetlerde müşteriniz için bir deneme İş Ortağı Merkezi:

1. **İş Ortağı Merkezi'de** Satış'tan Katalog'a **gidin.** 
2. Katalogda Faturalama **sıklığı'nın altında Deneme** **teklifi'ne tıklayın.** Bu, yalnızca ücretsiz denemelerin görünmesini sağlar ve ücretsiz olan diğer teklifleri devre dışı bıraktır. Denemeler katalogda **Denemeler** sekmesinde görünür.
3. Sunmak istediğiniz ücretsiz denemeyi seçin ve gönder'i **seçin.** Tüm denemeler 30 gündür ve bu süre boyunca faturalandırlanmaz. Deneme süresi boyunca istediğiniz zaman ücretli aboneliğe de dönüştürebilirsiniz.

## <a name="converting-trials-to-paid-subscriptions"></a>Denemeleri ücretli aboneliklere dönüştürme

Ücretsiz deneme sürümü otomatik olarak ücretli aboneliğe dönüştürülmesiz. 30 gün sonra ücretsiz denemenin ücretli aboneliğe dönüştürülmesi gerekir, yoksa aboneliğin süresi [dolar.](#expiring-offers) Ücretsiz denemeler genişletilemez.

Denemeyi kendiniz ücretli aboneliğe dönüştürmeniz gerekir. Bunu yapmak için [İş Ortağı Merkezi](#convert-trials-using-partner-center) [api'leri İş Ortağı Merkezi.](#convert-trials-using-apis)

> [!NOTE]
> Bulut Çözümü Sağlayıcısı (CSP) programı için müşteri ücretsiz denemeleri başka bir program kiracısına (EA, Open veya MOSP gibi) dönüştürülemesi mümkün değil.

### <a name="convert-trials-using-partner-center"></a>Denemeleri İş Ortağı Merkezi

Denemeleri ücretli aboneliklere dönüştürmek için şu İş Ortağı Merkezi:

1. Müşterinin abonelik sayfasına gidin ve ücretsiz denemeyi seçin.
2. Denemeyi **ücretli aboneliğe dönüştür seçeneğini seçin.**
3. İstediğiniz lisans miktarını ve faturalama sıklığını girin ve Uygula'yi **seçin.**
4. Ücretli aboneliğin faturalaması dönüştürme tarihinde başlar ve abonelik, dönüştürme tarihinden itibaren 12 ay sonra otomatik olarak yeniler. 

### <a name="convert-trials-using-apis"></a>API'leri kullanarak denemeleri dönüştürme

Ücretsiz denemenin ücretli aboneliğe dönüştürmesi için API'lerinizi değiştirmeniz gerekir. Daha fazla bilgi için aşağıdaki geliştirici belgelerine bakın:

- [Deneme aboneliğini ücretli aboneliğe dönüştürme](/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Deneme dönüştürme tekliflerinin bir listesini alma](/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="trials-without-conversions"></a>Dönüştürme olmadan denemeler

Tüm denemeler ücretli aboneliklere dönüştürülemeyecektir. İş ortakları, son kullanma tarihine kadar dönüştürmesi olan bir deneme sürümü kullanabilir. İş ortakları, deneme teklifiyle aynı hizmetleri destekleyen uyumlu teklifler satın alınabilir.  Bu, yeni satın alınan tekliflerin hizmetlerinin denemenin hizmetleriyle uyumlu olduğundan emin olmak için deneme süresi dolmadan önce yapılması gerekir. 

|**Deneme**   |**Uyumlu Küçük İşletme teklifleri**   |**Uyumlu Enterprise teklifleri**   |
|----------------------------|:---------------------------------|:------------------------------------------|
|Microsoft Teams Ticari Bulut (Kullanıcı Tarafından Başlatılan) Deneme Sürümü   |Microsoft 365 İş Temel, Microsoft 365 İş Standart, Microsoft 365 İş Ekstra   | F3 (eski adı F1), Office 365 için Enterprise (E1, E3 ve E5), Microsoft 365 F1/F3, Microsoft 365 Kurumsal (E3)   |

>[!NOTE]
>Yukarıdaki teklifler benzer işlevlere sahip benzer hizmet planlarına sahip ancak teklifler arasında bazı farklılıklar olabilir.

### <a name="expiring-offers"></a>Süresi dolan teklifler

Süresi dolan teklifler size bildirilecek değil. Sonraki sona erme tarihlerini takip etmek için İş Ortağı Merkezi müşteri görünümünü kullanabilir veya API'yi sorgulaabilirsiniz. Bir karar noktasına yaklaşan müşterilerle uygun takip eylemlerini gerçekleştiresiniz diye bu tarihleri sık sık izlemek iyi bir fikirdir.

Deneme süresi dolsa da, bu denemede oturum açma girişiminde bulunan bir müşteri süre sonu iletisiyle karşılar. Ancak, veriler veri saklama standartlarına uygun olarak depolanır. Aynı hizmet planlarına sahip yeni bir abonelik satın alındıktan sonra müşterinizin bilgilerine yeni etkinleştirilen abonelikten yeniden erişilebilir.

## <a name="billing"></a>Faturalandırma

Bağımsız bulutlarda ve genel bulutta yıllık faturalandırma ve ücretsiz denemeler aynıdır. Tek fark, fırlatma zamanında kullanılabilen deneme SKUS'larıdır.

## <a name="billing-for-free-trials"></a>Ücretsiz denemeler için faturalama

Ücretsiz denemeler hem aylık hem de yıllık faturalandırılan abonelikler için kullanılabilir. Denemeyi ücretli aboneliğe dönüştürürken faturalama sıklığını seçin.

Abonelik başlangıç tarihi, dönüştürme tarihine göredir. Ücretsiz deneme sürümü yıllık faturalama ile ücretli bir teklife dönüştürülürse, abonelik yenileme tarihi dönüştürme tarihine 12 ay sonra gelir. Ücretsiz deneme sürümü aylık faturalamalı ücretli bir teklife dönüştürülürse, abonelik yenileme tarihi, dönüştürme tarihini takip eden faturalama tarihine on iki ay sonra gelir.

### <a name="invoices"></a>Faturalar

Fatura veya lisans tabanlı mutabakat dosyanız içinde ücretsiz denemeler listelenmiyor. Ücretsiz denemeler yalnızca ücretsiz denemeyi ücretli aboneliğe dönüştürdikten sonra faturanız ve lisans tabanlı mutabakat dosyanız üzerinde görünür. Dönüştürülen abonelik, yeni abonelikle aynı şekilde görünür.

### <a name="incentives"></a>Teşvikler

Ücretsiz denemelerin teşvikler üzerinde bir etkisi olmaz.

## <a name="support"></a>Destek

Ücretsiz denemeler için, ücretsiz denemeler aracılığıyla bir hizmet İş Ortağı Merkezi.