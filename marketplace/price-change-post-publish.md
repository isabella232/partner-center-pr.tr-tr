---
title: Market ürünlerine ilişkin fiyat değişiklikleri yayımlama sonrası
description: Bu makalede, yayımlamadan sonra planlardaki fiyatları değiştirme hakkında sık sorulan sorular açıklanmaktadır.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 08/27/2021
ms.openlocfilehash: bfb99986483d0aaaa5d685c266c8118c1345517c
ms.sourcegitcommit: 09d251409c2070fdb8ae5f9caa79152665fb2ddb
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/30/2021
ms.locfileid: "123164883"
---
# <a name="price-changes-to-marketplace-products"></a>Market ürünlerine ilişkin fiyat değişiklikleri

Ürünlerini Azure Marketi aracılığıyla satan bağımsız yazılım satıcıları (ISV), plan (veya STB) fiyatlarını zaman zaman güncelleştirebilir. SKU 'nun yeni fiyatı önceki fiyattan daha yüksek veya daha düşük olabilir. Fiyat değişikliği Ürün/SKU/Pazar düzeyinde güncelleştirilir. Bu nedenle, bazı pazarlar için uygun fiyat güncelleştirmeleri olabilir, ancak tümüne yönelik değildir.

Belirli durumlarda (aşağıya bakın) fiyat değişikliği geçmişte satın alınan ürünleri etkileyebilir ve müşteri aylık faturasında bir fiyat değişikliği görür. Azure Marketi, yeni fiyat yürürlüğe girmeden önce bu ürünleri en az 90 gün önce kullanarak müşterileri bilgilendirir.

## <a name="which-offer-types-can-be-affected-from-price-change"></a>Fiyat değişikliğinden hangi teklif türleri etkilenebilir?

Azure Market ve AppSource ile satılan tüm transactable ürünleri, örneğin bir veya daha fazla planı olan ürünler.

## <a name="can-a-free-sku-turn-one-day-into-a-paid-one"></a>Ücretsiz bir SKU bir günü ücretli bir şekilde mi açabilir?

Hayır. ISV, ücretsiz bir SKU 'yu ücretli bir SKU 'ya alamaz. Bir ürünün faturalandırılabilir olmasını isteyen bir ISV 'nin yeni bir ücretli SKU yayımlaması gerekir.

## <a name="price-increase-awareness-in-the-marketplace-product-pages"></a>Market ürün sayfalarındaki fiyat artışı artışı

Belirtildiği gibi, bir fiyat artışı yayınlamak isteyen ISV 'Ler, yeni fiyat yürürlüğe girmeden önce en az 90 gün önce uyarı vermelidir. Bu, müşterilere bir ürün satın almayı planlayan bir bildirim vermektir. Market ürün sayfaları, gelecek değişikliğe göre en az 90 gün önce güncelleştirilir. Sayfalar, Fiyat değişikliğinin yaklaşan tarihini ve yeni oranı açıklayan bir iletiyle güncelleştirilir

:::image type="content" source="media/price-change/plan-pricing.png" alt-text="Plan fiyatlandırma sayfasını gösterir":::

> [!NOTE]
> Yukarıdaki görüntüdeki fiyatlandırma yalnızca örnek amaçlıdır. Gerçek fiyatlar farklılık gösterebilir.

Bu bildirim yalnızca fiyat ' ı geçse, Fiyat daha sonra değilse görünür.

## <a name="when-is-the-new-price-taking-effect"></a>Yeni Fiyat ne zaman yürürlüğe girer?

 Yeni Fiyat geçerlilik tarihi her zaman bir takvim ayının başlangıcında olacaktır. 90 gün bildirim dönemi ile tipik bir fiyat güncelleştirme zaman çizelgesi şöyle görünür:

15 Ocak – ISV güncelleştirme katalogdaki bir SKU 'ya gelecekteki bir fiyat güncelleştirmesi

Jan-16-18 – ürün sayfası, 1 Mayıs 'ta (Ocak + 90 gün sonunda) gerçekleştirilecek olan fiyat artışına ilişkin bir uyarı iletisiyle güncelleştirilir.

Mayıs-1 – yeni fiyat devreye girer

## <a name="customers-affected-from-a-price-change-post-purchase"></a>Fiyat değişikliğinden etkilenen müşteriler (satın alma sonrası)

Fiyat artışı geçerlilik tarihinden önce bir ürünün satın alınması, ürün dağıtımının kullanım ömrü için satınalma fiyatını garanti *etmez* . Etkilenen farklı teklif türleri şunlardır:

- Tüketim tabanlı ürünler (örneğin, saat veya, SaaS veya yönetilen uygulama teklifinin ölçülen kullanım fiyatı ile faturalandırılan VM 'Ler), yeni fiyat geçerli olduğunda tüketim birimi maliyeti artar. Ayın ortasında faturalandırılan müşteriler söz konusu olduğunda aylık kullanım raporunda iki satır olacaktır: biri, yeni fiyat geçerlilik tarihine (Yukarıdaki örnekte:-1) ve biri tüketim geçerlilik tarihi için bir tane olacak şekilde tüketimine yöneliktir.
- Aylık ücretle tüketim tabanlı ürünler (özel ölçümlerle SaaS gibi), yeni fiyat Market 'te yürürlüğe girer, tüketim birimleri fiyatı etkilenecektir. Aylık ücret, yetkilendirme döneminin sonuna kadar değişmeden tutulur.
- Bilgisayar tabanlı ürünler (örneğin, lisans tabanlı SaaS Hizmetleri), Fiyat değişikliği geçerlilik tarihi gerçekleşirse, satın alma sonrası, bir sonraki yenileme tarihine kadar, aylık yenileme veya yıllık yenileme tarihi olarak garanti edilir.
    - Fiyat değişikliği geçerlilik tarihinden sonra, ancak sözleşmenin yenileme tarihi önce, başlangıçtaki satın alma fiyatında tutulacak şekilde bilgisayar ekleme veya kaldırma. Yenilemeden sonra, yeni fiyat geçerli olur.
    - SKU değiştirme, Fiyat değişikliği geçerlilik tarihinden sonra SKU 'nun değiştirilmesi, yeni satın alma olarak değerlendirilir ve yeni fiyata tabi olur. Bu değişiklik Ayrıca, lisans sayısını değiştirmenin müşterinin SKU 'sunda değiştirilmesini gerektiren senaryolar için de geçerlidir. Örneğin, 400 koltuk 'dan 500 ' ye geçerek, müşterinin ürünün yeni bir katmanını/SKU 'SU satın almasını gerektirebilir.

## <a name="customer-notifications"></a>Müşteri bildirimleri

Yaklaşan fiyat artışına göre etkilenen bir pazarda Ürün/SKU 'SU kullanmakta olan müşterilere, gelecek değişiklik hakkında e-posta ile bildirim gönderilir. Bu, bunu tercih ettikleri takdirde onunla ilgili eylemler gerçekleştirebilir. E-posta bildirimi, yeni fiyat yürürlüğe madan 90 gün önce gönderilir ve fiyat değişikliği geçerlilik tarihinden önce ikinci bir ileti 30 gün önce gönderilir. İleti fatura bölümüne (proje) sahip, fatura grubu sahipleri ve aboneliğin faturalama hesabı sahiplerine gönderilir.

## <a name="next-steps"></a>Sonraki adımlar

- [Azure Market nedir?](azure-marketplace-overview.md)
- [Azure Marketi satın alma](azure-purchasing-invoicing.md)