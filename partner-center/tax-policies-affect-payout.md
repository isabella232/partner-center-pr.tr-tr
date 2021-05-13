---
title: Azure Marketi için vergi ilkelerinin ödeme nasıl etkilediği
description: Vergi ilkelerinin Azure Marketi için ödeme 'yi nasıl etkilediğini öğrenin.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: a93e94912f840e4cb69c3cc834f03af1b34f19aa
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856024"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Azure Marketi için vergi ilkelerinin ödeme nasıl etkilediği

**Uygun roller**: genel yönetici | Kullanıcı Yönetimi Yöneticisi | Yönetim Aracısı

## <a name="introduction"></a>Giriş

Microsoft ticari marketi 'nde küresel erişim vardır. İşlemler, kenarlıkların tamamında ve ISV ve müşterinin bulunduğu yere bağlı olarak, vergi etkilerine karşı farklılık gösterebilir. Microsoft AppSource ve Azure Marketi, ISV 'nin ülkesini öğrenmek için Iş Ortağı Merkezi vergi profili bilgilerini kullanır. Müşterinin ülkesini öğrenmek için müşterinin fatura bilgilerini kullanın ya da müşteri AB 'de ise iki farklı bilgi parçası kullanıyoruz.

Aşağıdaki senaryoları daha iyi anlamak için, Microsoft 'un yayımcı adına vergi toplayıp ödemediğini veya bu sorumluluğun yayımcıya ait olup olmadığını gösteren [vergi ayrıntıları](tax-details-marketplace.md) tablosuna bakın.

> [!NOTE]
> Bu konudaki tüm örnek satış değerleri ve vergi yüzdeleri, yalnızca tanım amaçlıdır ve tam sayılar değildir.

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Microsoft tarafından yönetilen vergi ülkede yayımcı transacts

**Senaryo a** – [Microsoft tarafından yönetilen bir vergi ülkesindeki](tax-details-marketplace.md#microsoft-managed-countries)bir yayımcı ile müşteri arasında gerçekleşen işlemler. Bu işlemler, satış sırasında geçerli vergi eklenerek, Microsoft bu vergiyi ilgili ülkeye gönderiyor. Ödemelerden kesilen vergiler ve ödemesiz hesaplamalar vergi dışlamalı.

ABD dışı Yayımcı ve ABD müşterisi arasındaki işlemler için bkz. [senaryo D](#foreign-publisher-transacts-with-us-customer) .

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Ödeme işlem senaryosu A için iş akışını gösterir.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Microsoft tarafından yönetilen ve Market ücreti vergilendirilebilir servis olan Microsoft tarafından yönetilen vergi ülkede yayımcı transacts

**Senaryo B** : ABD tabanlı bir Yayımcı (Iş Ortağı Merkezi vergi profili bilgileri tarafından tanımlandığı gibi) arasında, ülkenin Market ücretine (vergilendirilebilir hizmet) bir vergi sunan Microsoft tarafından yönetilen bir vergi ülkesindeki bir müşteriye yaptığı işlemler. Bu senaryoda, mağaza hizmeti ücretine vergi yayımcının ödemelerinden çıkarılacaktır.

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Ödeme süreci senaryosu B için iş akışını gösterir.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>Yayımcı tarafından yönetilen Vergi Ülkesinde Yayımcı Transacts

**Senaryo C** : Yayımcı ile yayımcı tarafından yönetilen bir vergi ülkesi içinde yer alan ve müşterilere stopaj vergisi dayatmayacak olan müşteriler arasında yapılan işlemler. Müşteriler satış noktasında vergi ödemez ve yayımcının tüm geçerli vergileri ödeme yükümlülüğü vardır.

Ülkeye özgü fiyatlandırma (örneğin yaklaşan vergilendirmeyi dengelemek için) hakkında daha fazla bilgi için bkz. Ticari market [teklifleri için planlar ve fiyatlandırma.](/azure/marketplace/plans-pricing#custom-prices)

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Ödeme süreci senaryosu C için iş akışını gösterir.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>ABD Müşterisi ile Yabancı Yayımcı Transacts

**Senaryo D** – ABD merkezli bir müşteriye satış yapan (müşteri hesabı adresiyle tanımlandığı gibi) abd merkezli bir müşteriye satış yapan (senaryo [E'ye](#foreign-publisher-with-a-treaty-transacts-with-us-customer)bakın) olmayan ülkelerdeki tüm yabancı yayımcılar (İş Ortağı Merkezi Vergi Profili Bilgileriyle tanımlandığı şekilde). ABD kamu, Yayımcı adına Microsoft stopaj vergisi gerektirir. Ödemeden yayımcıya kadar olan vergiler teklif fiyatına göre hesaplanır.

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Ödeme süreci senaryosu D için iş akışını gösterir.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>ABD müşterisi ile Transacts olan yabancı yayımcı

**Senaryo E:** ABD tabanlı bir müşteriye satış yapan (müşteri hesabı adresiyle tanımlandığı şekilde) ABD'de bir satıcıya sahip olan tüm yabancı yayımcılar (İş Ortağı Merkezi Vergi Profili Bilgileri ile tanımlandığı şekilde). ABD kamu, Microsoft'un yayımcı adına vergi stopajı gerektirmez.

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Ödeme süreci senaryosu E için iş akışını gösterir.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>Yabancı yayımcı, Microsoft tarafından yönetilen bir ülkede (İrlanda dışında) AB'ye kayıtlı bir müşteriye satışlar

**Senaryo F:** Bir ülkede yabancı yayımcılar ve AB'de KDV kayıtlı müşteriler (İrlanda dışında) Microsoft-Managed işlemler. Müşteri satışta vergi ödemez.

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Ödeme süreci senaryosu F için iş akışını gösterir.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>Yabancı Yayımcı, Microsoft tarafından yönetilen bir ülkede bir AB KDV 'ye kayıtlı müşteriye satıl (Irlanda 'da)

**Senaryo G** – bir Microsoft-Managed ülkede yabancı YAYıMCıLAR ve AB ile kayıtlı müşteriler arasındaki tüm Işlemler (İrlanda içi). Müşteri Irlanda KDV 'sini ödeder ve Microsoft bu vergiyi Irlanda devlet kurumuna ödeder.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Ödeme işlem senaryosu G için iş akışını gösterir.":::

## <a name="next-steps"></a>Sonraki adımlar

- [Yayımcı hakkında SSS](/azure/marketplace/marketplace-faq-publisher-guide)
- [Ödeme ve vergi profilleri oluşturma yönergeleri](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)