---
title: Azure Marketi için vergi ilkelerinin ödeme nasıl etkilediği
description: Vergi ilkelerinin Azure Marketi için ödeme 'yi nasıl etkilediğini öğrenin.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-payouts
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: ef6520ff6ed4439e975dddaeff0b89ea2a912678c3871f1fc14bfb3cbe6bbff2
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115691547"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Azure Marketi için vergi ilkelerinin ödeme nasıl etkilediği

**Uygun roller**: genel yönetici | Kullanıcı Yönetimi Yöneticisi | Yönetim Aracısı

## <a name="introduction"></a>Giriş

Microsoft ticari marketi 'nde küresel erişim vardır. İşlemler, sınırlar genelinde gerçekleşir ve bağımsız yazılım satıcısının (ISV) ve müşterinin bulunduğu yere bağlı olarak, vergi etkilerine karşı farklılık gösterebilir. Microsoft AppSource ve Azure Marketi, ISV 'nin ülkesini öğrenmek için Iş Ortağı Merkezi vergi profili bilgilerini kullanır. Müşterinin ülkesini öğrenmek için müşterinin fatura bilgilerini kullanın ya da müşteri AB 'de ise iki farklı bilgi parçası kullanıyoruz.

Aşağıdaki senaryoları daha iyi anlamak için, Microsoft 'un yayımcı adına vergi toplayıp ödemediğini veya bu sorumluluğun yayımcıya ait olup olmadığını gösteren [vergi ayrıntıları](tax-details-marketplace.md) tablosuna bakın.

> [!NOTE]
> Bu konudaki tüm örnek satış değerleri ve vergi yüzdeleri, yalnızca tanım amaçlıdır ve tam sayılar değildir.

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Publisher Transacts Microsoft tarafından yönetilen vergi ülkesi

**Senaryo a** – [Microsoft tarafından yönetilen bir vergi ülkesindeki](tax-details-marketplace.md#microsoft-managed-countries)bir yayımcı ile müşteri arasında gerçekleşen işlemler. Bu işlemler, satış sırasında geçerli vergi eklenerek, Microsoft bu vergiyi ilgili ülkeye gönderiyor. Ödemelerden kesilen vergiler ve ödemesiz hesaplamalar vergi dışlamalı.

ABD dışı Yayımcı ve ABD müşterisi arasındaki işlemler için bkz. [senaryo D](#foreign-publisher-transacts-with-us-customer) .

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Ödeme işlem senaryosu A için iş akışını gösterir.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Publisher Market ücreti vergilendirilebilir servis olan Microsoft tarafından yönetilen vergi ülkesinde transacts

**Senaryo B** : ABD tabanlı bir Yayımcı (Iş Ortağı Merkezi vergi profili bilgileri tarafından tanımlandığı gibi) arasında, ülkenin Market ücretine (vergilendirilebilir hizmet) bir vergi sunan Microsoft tarafından yönetilen bir vergi ülkesindeki bir müşteriye yaptığı işlemler. Bu senaryoda, mağaza hizmeti masrafında vergi, yayımcının ödemsından çıkarılır.

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Ödeme işlem senaryosu B için iş akışını gösterir.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>Publisher Publisher yönetilen vergi ülkesindeki Transacts

**Senaryo C** : müşteriler üzerinde bir stopaj vergisi uygulamayan yayımcı tarafından yönetilen bir vergi ülkesindeki bir yayımcı ve müşteri arasında gerçekleşen işlemler. Müşteriler satış noktasında vergi ödemesiz ve yayımcının tüm geçerli vergileri ödemekle ilgili yükümlülüğünüz.

Ülkeye özgü fiyatlandırmayla ilgili daha fazla bilgi için (örneğin, yaklaşan vergilendirme 'yi kaydırmak için) bkz. [ticari Market teklifleri Için planlar ve fiyatlandırma](/azure/marketplace/plans-pricing#custom-prices).

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Ödeme işlem senaryosu C için iş akışını gösterir.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>abd müşterisi ile yabancı Publisher Transacts

**Senaryo D** – tüm yabancı yayımcılar (Iş Ortağı Merkezi vergi profili bilgileri tarafından tanımlandığı şekilde) ABD 'de bir müşteriye (müşteri hesabı adresleri tarafından tanımlandığı [gibi) bir](#foreign-publisher-with-a-treaty-transacts-with-us-customer)satış yapma. ABD Kamu, Microsoft 'un yayımcı adına vergi stopajın olmasını gerektirir. Ödemelerden yayımcıya kesilen vergi, teklif fiyatına göre hesaplanır.

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Ödeme işlem senaryosu D için iş akışını gösterir.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>ABD müşterisi ile bir Treaty transacts ile yabancı Yayımcı

**Senaryo E** – tüm yabancı yayımcılar (Iş Ortağı Merkezi vergi profili bilgileri tarafından tanımlandığı gibi) ABD ile ilgili bir müşteriye satış yapan (müşteri hesabı adresleri tarafından tanımlandığı şekılde) ABD ABD Kamu, Microsoft 'un yayımcı adına vergi stopaj uygulamasına gerek yoktur.

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Ödeme işlem senaryosu E için iş akışını gösterir.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>Yabancı Yayımcı, Microsoft tarafından yönetilen bir ülkede (Irlanda dışında) bir AB KDV 'ye kayıtlı müşteriye satış sağlar

**Senaryo F** – bir Microsoft-Managed ülkede yabancı YAYıMCıLAR ve AB katma VERGI (KDV) ile kaydedilen müşteriler arasındaki tüm işlemler. Müşteri, satışla ilgili vergiyi ödemez.

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Ödeme işlem senaryosu F için iş akışını gösterir.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>Yabancı Yayımcı, Microsoft tarafından yönetilen bir ülkede bir AB KDV 'ye kayıtlı müşteriye satıl (Irlanda 'da)

**Senaryo G** – bir Microsoft-Managed ülkede yabancı YAYıMCıLAR ve AB ile kayıtlı müşteriler arasındaki tüm Işlemler (İrlanda içi). Müşteri Irlanda KDV 'sini ödeder ve Microsoft bu vergiyi Irlanda devlet kurumuna ödeder.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Ödeme işlem senaryosu G için iş akışını gösterir.":::

## <a name="next-steps"></a>Sonraki adımlar

- [Publisher SSS](/azure/marketplace/marketplace-faq-publisher-guide)
- [Ödeme ve vergi profilleri oluşturma yönergeleri](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)