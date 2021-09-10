---
title: Yayımlama sonrası market ürünlerinde fiyat değişiklikleri
description: Bu makalede, yayımlama sonrasında planlarda fiyatları değiştirme hakkında sık sorulan sorular açıklanmıştır.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 08/27/2021
ms.openlocfilehash: bfb99986483d0aaaa5d685c266c8118c1345517c
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123936976"
---
# <a name="price-changes-to-marketplace-products"></a>Market ürünlerinde fiyat değişiklikleri

Ürünlerini Azure Market aracılığıyla satan Bağımsız Yazılım Satıcıları (ISV' ler) zaman zaman plan (veya SKU) fiyatlarını güncelleştirmektedir. SKU'nun yeni fiyatı önceki fiyattan daha yüksek veya daha düşük olabilir. Fiyat değişikliği ürün/SKU/pazar düzeyinde güncelleştirilir. Bu nedenle, bazı pazarlar için uygun olan ancak hepsi için uygun fiyat güncelleştirmeleri olabilir.

Bazı durumlarda (aşağıya bakın) fiyat değişikliği geçmişte satın alınan ürünleri etkileyebilir ve müşteri aylık faturalarında fiyat değişikliğini görebilir. Azure Market yeni fiyatın etkili olmadan en az 90 gün önce bu ürünleri kullanan müşterilere bildirecek.

## <a name="which-offer-types-can-be-affected-from-price-change"></a>Fiyat değişikliğinden hangi teklif türleri etkilenebilir?

Bir veya daha fazla planı olan ürünler Azure Market AppSource ve AppSource aracılığıyla satılan işlemleştirilebilir tüm ürünler.

## <a name="can-a-free-sku-turn-one-day-into-a-paid-one"></a>Ücretsiz bir SKU, bir günü ücretli bir SKU'ya dönüştürer mi?

Hayır. ISV ücretsiz SKU'ları ücretli bir SKU'ya dönüştüramaz. Ürünü faturalandırılabilir yapmak isteyen bir ISV'nin yeni bir ücretli SKU yayımlaması gerekir.

## <a name="price-increase-awareness-in-the-marketplace-product-pages"></a>Market ürün sayfalarında fiyat artışı farkındalığı

Daha önce belirtildiği gibi, fiyat artışı yayımlamak isteyen ISV'lerin yeni fiyatın etkili olması için en az 90 gün uyarı vermeleri gerekir. Bu, ürün satın alma planlamasına müşterilere bildirim vermektir. Market ürün sayfaları, gelecek değişiklikle birlikte en az 90 gün önceden güncelleştirilir. Sayfalar, fiyat değişikliğinin yaklaşan tarihini ve yeni fiyatın ayrıntılarıyla bir iletiyle güncelleştirilir

:::image type="content" source="media/price-change/plan-pricing.png" alt-text="Plan fiyatlandırma sayfasını göstermektedir":::

> [!NOTE]
> Yukarıdaki görüntüde yer alan fiyatlandırma yalnızca örnek amaçlıdır. Gerçek fiyatlar farklılık gösterebilir.

Bu tür bildirimler yalnızca fiyatın yukarıya doğru ilerler ve fiyatın düştükleri durumlarda gösterlanmaz.

## <a name="when-is-the-new-price-taking-effect"></a>Yeni fiyat ne zaman etkili oluyor?

 Yeni fiyat geçerli tarihi her zaman bir takvim ayı başlangıcında olur. 90 günlük bildirim süresiyle tipik bir fiyat güncelleştirme zaman çizelgesi şöyle görünür:

15 Ocak – ISV, katalogda gelecekteki bir fiyat güncelleştirmesini SKU'ya güncelleştirdi

16-18 Ocak – ürün sayfası, 1 Mayıs'ta (Ocak sonu + 90 gün) gelecek fiyat artışıyla ilgili bir uyarı iletisiyle güncelleştirildi.

1 Mayıs – yeni fiyat yürürlüğe girdi

## <a name="customers-affected-from-a-price-change-post-purchase"></a>Fiyat değişikliğinden etkilenen müşteriler (satın alma sonrası)

Fiyat artışının geçerli olduğu tarihten önce ürün satın *almak,* ürün dağıtımının kullanım ömrü boyunca satın alma fiyatını garanti eder. Etkilenen farklı teklif türleri:

- Tüketime dayalı ürünler (örneğin, SaaS veya yönetilen uygulama teklifinin tarifeli kullanımına göre faturalandırılan VM'ler), yeni fiyat geçerli olduktan sonra tüketim birimi maliyetleri artacaktır. Ayın ortasında faturalandırılacak müşteriler için aylık kullanım raporunda iki satır vardır: biri yeni fiyat geçerli tarihine kadar tüketim için (yukarıdaki örnekte: 1 Mayıs) ve biri de geçerli tarihten sonra tüketim için
- Aylık ücrete sahip tüketime dayalı ürünler (özel metre ile SaaS gibi), yeni fiyat markette etkili olduğu için tüketim birimleri fiyatı etkilenir. Aylık ücret, yetkilendirme döneminin sonuna kadar değiştirilmeden tutulur.
- Lisans tabanlı ürünler (lisans tabanlı SaaS hizmetleri gibi) fiyat değişikliğinin geçerli olduğu tarih satın alma sonrasında gerçekleşirse satın alma fiyatı, aylık yenileme veya yıllık yenileme tarihi gibi bir sonraki yenileme tarihine kadar garanti olur.
    - Fiyat değişikliğinin geçerli olduğu tarihten sonra lisans ekleme veya kaldırma işlemi, sözleşmenin yenilenme tarihi öncesinde ilk satın alma fiyatında tutulur. Yenilemeden sonra yeni fiyat yürürlüğe girecektir.
    - SKU'nun değiştirilmesi, fiyat değişikliğinin geçerli olduğu tarihten sonra SKU'nun değiştirilmesi yeni satın alma olarak kabul edilir ve yeni fiyata tabi olur. Bu değişiklik, yer sayısını değiştirmenin müşterinin SKU's unu değiştirmesini gerektirdiği senaryolar için de geçerlidir. Örneğin, 400 lisanstan 500 lisansa geçildi ve bu da müşterinin üründen yeni bir katman/SKU satın almalarını gerekli olabilir.

## <a name="customer-notifications"></a>Müşteri bildirimleri

Yaklaşan fiyat artışının etkilendiği bir markette ürünü/SKU'ları zaten kullanan müşterilere, gelecek değişiklikle ilgili e-posta ile bildirilecek. Bu, tercih yapmaları için bu konuda eylem gerçekleştirecekleri bir durum olabilir. E-posta bildirimi, yeni fiyatın geçerli olmasından 90 gün önce gönderilir ve fiyat değişikliğinin geçerli olduğu tarihten 30 gün önce ikinci bir ileti gönderilir. İleti fatura bölümü (proje) sahibine, faturalama grubu sahiplerine ve aboneliğin ödeme hesabı sahiplerine gönderilir.

## <a name="next-steps"></a>Sonraki adımlar

- [Azure Market nedir?](azure-marketplace-overview.md)
- [Azure Market satın alma](azure-purchasing-invoicing.md)