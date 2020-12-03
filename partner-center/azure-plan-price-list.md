---
title: CSP iş ortakları için Azure planı fiyat listesi
ms.topic: how-to
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP program iş ortaklarının, Azure planı kapsamındaki aboneliklerin fiyat listesini görmek için Iş Ortağı Merkezi 'ni nasıl kullanabileceği hakkında bilgi edinin.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 02cea980626ec32d3dd60f646b1f8744130792ea
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534735"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Azure için CSP'de yeni ticari deneyim için fiyat listesi

**Uygun roller**

- Yönetim Aracısı
- Faturalama yöneticisi
- Genel yönetici
- Yardım Masası Aracısı
- Satış Aracısı
- Kullanıcı Yönetimi Yöneticisi

CSP 'de yeni Azure Ticaret deneyiminin fiyat listesi Iş Ortağı Merkezi ' nde gönderilir. Fiyat listesi, gerçek zamanlı doğru bir dosyada dinamik olarak dağıtılır ve fiyatlar yalnızca USD olarak gösterilir. Ancak faturalandırma, müşterinin para birimi konumu için geçerli olan desteklenen para biriminde yapılır. Müşterinin para birimi konumunda faturalandırma hakkında daha fazla bilgi için [Azure planı-faturalandırma](azure-plan-billing.md)makalesini okuyun.

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Azure plan fiyatlandırması kapsamında abonelikler için fiyatlandırmayı inceleyin

1. Sol taraftaki Iş Ortağı Merkezi menüsünde, **Sat** ' ı seçin ve ardından **Market**' i seçin.

2. Azure planı fiyatlandırması altında, fiyatlandırma istediğiniz ülkeyi seçin.

3. **Dışarı aktarma türü**' nün yanındaki **Azure planı tüketim fiyatlandırması**, **Azure plan ayırmaları fiyatlandırma** veya **FX ücretleri**' ni seçin. 

>[!NOTE] 
>**FX ücretleri** ülkeye özgü değildir.

4. **Tarih fiyatlandırmasının** yanında, istediğiniz tarihi (örneğin, **geçerli**) seçin.

   :::image type="content" source="images/azure/pricingnew.png" alt-text="ülkeye özgü":::

>[!NOTE] 
>İki farklı fiyat listesini dışarı aktarabilirsiniz-Azure plan fiyatlandırması ve Market üçüncü taraf fiyatlandırması.

## <a name="azure-price-list-specifics"></a>Azure fiyat listesi özellikleri

- Azure plan fiyatlandırması, **Satış** kapsamındaki Iş Ortağı Merkezi ' ndeki Market sayfasından kullanılabilir olacaktır.

- Dışarı aktarmalar Azure plan tüketim Hizmetleri, Azure ayırmaları ve FX ücretleri için kullanılabilir olacaktır.

- Dışarı aktarma seçenekleri şunlardır:

  - **Bugünün fiyatlandırması**: Bu, ayın 1 ' inden geçerli ayın geçerli tarihine kadar olan tüm ölçümleri ve fiyatları içerir. Buna yeni fiyatlar, değiştirilen fiyatlar veya kaldırılan fiyatlar dahildir. Tüm fiyatların yeni mi yoksa kaldırılmış mı olduğunu açıklamak için geçerli başlangıç ve bitiş tarihleri olacaktır.

  - **Önceki ayın fiyatlandırması**: her kaynak türünün İndirmeleri aya göre olacaktır. Fiyatlandırma dosyaları için, bu ay içinde kullanılabilir olan tüm ölçümleri dahil eder. Ayın ortasında yeni bir ölçüm göründüyse, kullanılabilirliğini yansıtan etkin bir tarih ile ölçüm olarak gösterilecektir. Etkin olmayan fiyatlara benzer ve bu, artık kullanılamadığı zaman geçerli bir bitiş tarihi ile gösteriliyor.

  - **FX ücretleri**: FX oranları, ayın 1 ' inden önceki günü, 18:00 PST 'yi indirmek için kullanılabilir olacak. Örneğin, Kasım ücretleri istiyorsanız 31 Ekim 'e kadar olan ücretleri indirin. Önceki ay FX ücretleri de kullanıma sunulacaktır.

- Fiyat listelerindeki fiyatlar doğrudan fiyatlardır. Bazı iş ortakları, iş ortağı tarafından kazanılan krediler için uygun olabilir. Ortağın kazanılan kredisi nasıl hesaplandığı hakkında daha fazla bilgi için, [ortağın kazanıldığını ve ödendiğini](partner-earned-credit-explanation.md)okuyun.

- **Uygun hizmetler**: iş ortağı kazanılmış kredisi, Azure planı [fiyatlandırma](https://partner.microsoft.com/commerce/sales) sayfasından dışarı aktarma işlemi için **Azure plan tüketim fiyatlandırma** iş ortakları ' nda listelenen hizmetler için geçerlidir. Azure plan tüketim fiyat listesi ve Azure plan ayırmaları 'nin Etiketler sütununda "üçüncü taraf" olarak tanımlanan üçüncü taraf ürünleri dahil, ancak bunlarla sınırlı olmamak üzere bir istisna vardır.

## <a name="price-list-data"></a>Fiyat listesi verileri

|**Alan**   |**Açıklama**   |
|--------------------------|:---------------------------|
|ProductTitle  |Ürünün başlığı veya adı|
|ProductID   |Ürünün KIMLIĞI|
|SkuId|SKU KIMLIĞI|
|SkuTitle|SKU 'nun başlığı veya adı|
|Publisher|Birinci taraf her zaman Microsoft olacaktır|
|SkuDescription|SKU 'nun açıklaması|
|UnitOfMeasure|Ücretlendirilebilecek veya faturalandırılacak birimler|
|TermDuration|Terim tabanlı ürünler için, dönemin uzunluğu, rezervasyonlar için geçerlidir|
|Pazara|Fiyatlandırma pazarı|
|Para Birimi|Fiyatlandırma para birimi|
|UnitPrice|Birim fiyat|
|PricingTierRangeMin|Katmanlı fiyatlandırma için, minimum fiyat geçerli olur|
|PricingTierRangeMax|Katmanlı fiyatlandırma için en yüksek fiyat geçerli olur|
|Efektbaşlangıçtarihi|Fiyatlandırma başlangıç tarihi|
|EffectiveEndDate|Fiyatlandırma bitiş tarihi|
|MeterIds|Ürün SKU 'sunun ölçüm KIMLIĞI|
|MeterType|Ölçüm türü|
|Etiketler|Bu öğe için özellikler, Azure plan fiyatlandırması için Azure ya da Azure ve rezervasyonlar (özellikle rezervasyonlar için) olacaktır|

Azure planına yönelik fiyat listeleri, Iş Ortağı Merkezi 'nde [fiyatlandırma ve teklifler sayfasından](https://partner.microsoft.com/dashboard/sell/pricingandoffers) aktarılabilir.

## <a name="tiered-pricing"></a>Katmanlı fiyatlandırma

Bazı Azure plan tüketim Hizmetleri katmanlı fiyatlandırmayı destekler. İş ortakları, Azure plan fiyatı listesinde bu ürünleri ve SKU 'ları bulabilir. Fiyatlandırma Katmanı aralığı sütunlarında değer bulunan öğeler, iş ortaklarının, kullanımı temel alarak fiyatı anlamasına imkan sağlar. Aşağıdaki örnekte, örnek verileri kullanarak üç Fiyatlandırma Katmanı içeren bir Ürün SKU 'su vardır.

|**ProductID**   |**SkuId**   |**UnitPrice**   |**PricingTierRangeMin**   |**PricingTierRangeMax**   |
|:---------------|:-----------|:---------------|:-------------------------|:-------------------------|
|DDD123456ABC|01AB|.50|100001|9223372036854780000|
|DDD123456ABC|01AB|.80|101|100000|
|DDD123456ABC|01AB|1|1|100|

Bu örnekte, 101 birimleri kullanılıyorsa, ücret 100,80 olur. İlk 100 birimi her biri ve sonraki birim,. 80 ' de ücretlendirilir.

## <a name="pricing-api-for-azure-plan"></a>Azure planına yönelik fiyatlandırma API 'SI

[FIYATLANDıRMA API](/partner/develop/pricing) 'sini kullanarak, tüketim ve ayırmalar için Azure plan fiyatlandırmasını programlama yoluyla alabilirsiniz. Yabancı Exchange ücretleri de alabilirsiniz.

Fiyatlandırma API 'SI, diğer Iş Ortağı Merkezi API 'Lerinden farklı bir uç noktada bulunur. Fiyatlandırma bilgileri, Azure plan aboneliklerine uygulanan Azure plan kaynakları ve rezervasyonlar fiyatlandırması için ABD Doları cinsinden ölçüm fiyatlandırması içerir.

Bu API ayrıca iş ortaklarının aylık Döviz kurlarını almasına olanak sağlar çünkü Azure plan fiyatlandırması yalnızca USD 'dir. API 'Leri, geçerli ay veya önceki aylar için hem fiyatlandırma hem de yabancı değişim ücretleri almak için kullanabilirsiniz.

>[!NOTE]
> Fiyatlandırma API 'SI, Azure plan fiyatlandırmasına özgüdür. Azure kaynakları veya Azure olmayan plan aboneliklerine dağıtılan rezervasyonlar için Iş Ortağı Merkezi 'nin "fiyatlandırma ve teklifler" sayfasına gönderilen mevcut RateCard API 'sini ve fiyat listelerini kullanmaya devam etmelisiniz. Azure plan fiyatlandırma API 'SI, Microsoft 365 veya Dynamics 365 gibi yazılım, Market veya lisans tabanlı fiyatlandırmayı desteklemez.

Azure plan fiyatlandırması ve yabancı değişim oranı API 'Leri hakkında daha fazla bilgi için, tam [fiyatlandırma API 'si belgelerine](/partner/develop/pricing)bakın.

## <a name="next-steps"></a>Sonraki adımlar

- [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)