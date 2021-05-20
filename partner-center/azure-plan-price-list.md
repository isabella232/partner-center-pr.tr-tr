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
ms.openlocfilehash: 6d8e73e664d400e8e6d80e529326e566c5fd88a8
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149579"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Azure için CSP'de yeni ticari deneyim için fiyat listesi

**Uygun roller**: yönetici Aracısı | Faturalandırma Yöneticisi | Genel yönetici | Yardım Masası Aracısı | Satış Aracısı | Kullanıcı Yönetimi Yöneticisi

CSP 'de yeni Azure Ticaret deneyiminin fiyat listesi Iş Ortağı Merkezi ' nde gönderilir. Fiyat listesi, gerçek zamanlı doğru bir dosyada dinamik olarak dağıtılır ve fiyatlar yalnızca USD olarak gösterilir. 25 Ocak 2021 tarihinden itibaren, AB/EFTA ve Birleşik Krallık bölgesindeki iş ortakları, yeni müşteriler ve mevcut CSP müşterileri, kiracıların 11 Mayıs 2020 ' den önce oluşturulduğu ilk kez yeni ticaret teklifleri satın alarak, iş ortağı konumu para birimi için bu Satınalmalar için faturalandırılır.  AB/EFTA ve UK bölgesinin dışında bulunan iş ortakları, iş ortağı konumu para biriminde faturalandırılmaya devam edecektir, [Azure planı-faturalandırma](azure-plan-billing.md)' i okuyun.

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

  - **Bugünün fiyatlandırması**: Bu, ayın 1 ' inden geçerli ayın geçerli tarihine kadar olan tüm ölçümleri ve fiyatları içerir. Buna yeni fiyatlar, değiştirilen fiyatlar veya kaldırılan fiyatlar dahildir. Tüm fiyatlar, yeni veya kaldırılmış olup olmadığını açıklamak için geçerli başlangıç ve bitiş tarihlerine sahip olur.

  - **Önceki ayın fiyatlandırması:** Her kaynak türünün indirmeleri aya göre olacak. Fiyatlandırma dosyaları için bu, o ay boyunca kullanılabilen tüm metreleri içerir. Ayın ortasında yeni bir ölçüm belirse, kullanılabilirliğini yansıtan geçerli bir tarihe sahip bir ölçüm olarak gösterirum. Durdurulan fiyatlara benzer şekilde, artık ne zaman kullanılabilir olduklarını açıklayan geçerli bir bitiş tarihiyle gösteriliyor.

  - **FX Oranları:** FX fiyatları, ayın 13:00 PST'sinde 18:00'den önceki bir gün indirilebilir. Örneğin, Kasım için fiyatları görmek için 31 Ekim'de fiyatları indirin. Önceki ay FX fiyatları da kullanılabilir olacak.

- Fiyat listelerinde yer alan fiyatlar doğrudan fiyatlardır. Bazı iş ortakları, iş ortağı tarafından kazanılan krediler için uygun olabilir. İş ortağı tarafından kazanılan kredinin nasıl hesaplanması hakkında bilgi için iş ortağı [tarafından kazanılan kredinin hesaplanması ve ücretli olduğu makaleyi okuyun.](partner-earned-credit-explanation.md)

- **Uygun hizmetler:** İş ortağı tarafından kazanılan **kredi, Azure planı** tüketim fiyatlandırma iş ortaklarının Azure planı fiyatlandırma sayfasından dışarı aktarabilecekleri [hizmetler için](https://partner.microsoft.com/commerce/sales) geçerlidir. Azure planı tüketim fiyatı listesinin Ve Azure Planı rezervasyonlarının Etiketler sütununda "Üçüncü Taraf" olarak tanımlanan üçüncü taraf ürünleri de dahil ancak bunlarla sınırlı olmayan özel durumlar olduğunu unutmayın.

## <a name="price-list-data"></a>Fiyat listesi verileri

|**Alan**   |**Açıklama**   |
|--------------------------|:---------------------------|
|ProductTitle  |Ürünün başlığı veya adı|
|ProductID   |Ürünün kimliği|
|SKuId|SKU kimliği|
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
|MeterIds|Ürün sku'su ölçüm kimliği|
|MeterType|Ölçüm Türü|
|Etiketler|Öğenin özellikleri, Azure planı fiyatlandırması için bu Azure veya Azure ve Rezervasyonlar 'dır (özel olarak rezervasyonlar için)|

Azure planı için fiyat listeleri, fiyatlandırma ve teklifler sayfasından dışarı [İş Ortağı Merkezi.](https://partner.microsoft.com/dashboard/sell/pricingandoffers)

## <a name="tiered-pricing"></a>Katmanlı fiyatlandırma

Bazı Azure planı tüketim hizmetleri katmanlı fiyatlandırmayı destekler. İş ortakları bu ürünleri ve SKU'ları Azure planı fiyat listesinde bulabilir. Fiyatlandırma katmanı aralık sütunlarında değerleri olan öğeler, iş ortaklarının kullanımı temel alarak fiyatı anlamalarına olanak sağlar. Aşağıdaki örnekte örnek verileri kullanarak üç fiyatlandırma katmanına sahip bir ürün sku'suz vardır.

|**Productıd**   |**SkuId**   |**UnitPrice**   |**PricingTierRangeMin**   |**PricingTierRangeMax**   |
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
