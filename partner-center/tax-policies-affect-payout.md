---
title: Vergi ilkeleri, vergi ödemelerini Azure Market
description: Vergi ilkelerinin vergi ödemelerini nasıl etkileyeceğini Azure Market.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-payouts
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 6a069db0334b13309e39e08bcc7b70f22eaa5c69
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248415"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Vergi ilkeleri, vergi ödemelerini Azure Market

**Uygun roller:** Genel yönetici | Kullanıcı yönetimi yönetici | Yönetici aracısı

## <a name="introduction"></a>Giriş

Microsoft ticari marketi küresel olarak ulaşmaktadır. İşlemler sınırlar arasında gerçekleşir ve bağımsız yazılım satıcısının (ISV) ve müşterinin bulunduğu yere bağlı olarak vergi etkileri değişebilir. Microsoft AppSource ve Azure Market, ISV'nin İş Ortağı Merkezi Vergi Profili Bilgileri'nin kullanımını sağlar. Müşterinin ülkelerini belirlemek için müşterinin faturalama bilgilerini kullanın veya müşteri AB'de ise iki farklı bilgi parçası kullanıruz.

Aşağıdaki senaryoları daha iyi anlamak için [](tax-details-marketplace.md) Microsoft'un yayımcı adına vergi toplayıp ödemesi veya sorumluluğun yayımcıya ait olup olmadığını gösteren Vergi ayrıntıları tablosuna bakın.

> [!NOTE]
> Bu konudaki tüm satış değerleri ve vergi yüzdeleri, tam rakamlara değil yalnızca açıklayıcı amaçlara yöneliktir.

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Publisher Microsoft tarafından yönetilen Vergi Ülkesi'ne yapılan işlem

**Senaryo A** – Microsoft tarafından yönetilen bir vergi ülkesi olan bir yayımcı ile müşteri [arasında uzan işlemler.](tax-details-marketplace.md#microsoft-managed-countries) Bu işlemler, satış sırasında eklenen geçerli vergiye sahip olur ve Microsoft bu vergiyi ilgili ülkeye gönderir. Ödemeden vergiler muaf değildir ve ödeme hesaplamaları vergiye özeldir.

ABD [dışı bir](#foreign-publisher-transacts-with-us-customer) yayımcı ile ABD müşterisi arasındaki işlemler için D Senaryosuna bakın.

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Ödeme süreci senaryosu A için iş akışını gösterir.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Publisher Market Ücreti'nin VergiLanabilir Hizmet olduğu Microsoft tarafından yönetilen Vergi Ülkesi'ne yapılan işlem

**Senaryo B–** ABD tabanlı bir yayımcı (İş Ortağı Merkezi Vergi Profili Bilgileri tarafından tanımlandığı şekilde) ülkenin Market Ücretine (vergi uygulanabilir bir hizmet) vergi uygulama altında bulunduğu Microsoft tarafından yönetilen bir vergi ülkesi içinde yer alan bir müşteriye yapılan işlemler. Bu senaryoda, mağaza hizmeti ücretine vergi yayımcının ödemelerinden çıkarılacaktır.

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Ödeme süreci senaryosu B için iş akışını gösterir.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>Publisher Yönetilen vergi Publisher yapılan işlem

**Senaryo C** : Yayımcı ile yayımcı tarafından yönetilen bir vergi ülkesi içinde yer alan ve müşterilere stopaj vergisi dayatmayacak olan müşteriler arasında yapılan işlemler. Müşteriler satış noktasında vergi ödemez ve yayımcının tüm geçerli vergileri ödeme yükümlülüğü vardır.

Ülkeye özgü fiyatlandırma (örneğin yaklaşan vergilendirmeyi dengelemek için) hakkında daha fazla bilgi için bkz. Ticari market [teklifleri için planlar ve fiyatlandırma.](/azure/marketplace/plans-pricing#custom-prices)

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Ödeme süreci senaryosu C için iş akışını gösterir.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>ABD Publisher yabancı işlem transacts

**Senaryo D** : ABD merkezli bir müşteriye satış yapan (müşteri hesabı adresiyle tanımlandığı gibi) tüm yabancı yayımcılar (İş Ortağı Merkezi Vergi Profili Bilgileri ile tanımlandığı gibi) abd merkezli bir müşteriye satış yapan (senaryo [E'ye](#foreign-publisher-with-a-treaty-transacts-with-us-customer)bakın). ABD kamu, Yayımcı adına Microsoft stopaj vergisi gerektirir. Ödemeden yayımcıya kadar olan vergiler teklif fiyatına göre hesaplanır.

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Ödeme süreci senaryosu D için iş akışını gösterir.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>ABD müşterisi ile Transacts olan yabancı yayımcı

**Senaryo E:** ABD tabanlı bir müşteriye satış yapan (müşteri hesabı adresiyle tanımlanan şekilde) ABD'de satış yapan tüm yabancı yayımcılar (İş Ortağı Merkezi Vergi Profili Bilgileri ile tanımlandığı şekilde). ABD kamu, Microsoft'un yayımcı adına vergi stopajı gerektirmez.

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Ödeme süreci senaryosu E için iş akışını gösterir.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>Yabancı yayımcı, Microsoft tarafından yönetilen bir ülkede (İrlanda dışında) AB'de KDV kayıtlı bir müşteriye satışlar

**Senaryo F:** Bir ülkede yabancı yayımcılar ve AB katma değerli vergi (KDV) kayıtlı müşterileri (İrlanda dışında) Microsoft-Managed işlemler. Müşteri satışta vergi ödemez.

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Ödeme süreci senaryosu F için iş akışını gösterir.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>Yabancı yayımcı, Microsoft tarafından yönetilen bir ülkede (İrlanda'da) AB'ye kayıtlı bir müşteriye satışlar

**Senaryo G:** Bir ülkede yabancı yayımcılar ve AB'de KDV kayıtlı müşteriler (İrlanda'nın içinde) Microsoft-Managed işlemler. Müşteri Vergi KDVsi öder ve Microsoft bu vergiyi Devlet Dairesi'ne öder.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Ödeme süreci senaryosu G için iş akışını gösterir.":::

## <a name="next-steps"></a>Sonraki adımlar

- [Publisher SSS](/azure/marketplace/marketplace-faq-publisher-guide)
- [Ödeme ve vergi profilleri oluşturma yönergeleri](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)