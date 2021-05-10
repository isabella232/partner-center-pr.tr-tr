---
title: Azure Marketi için vergi ilkelerinin ödeme nasıl etkilediği
description: Vergi ilkelerinin Azure Marketi için ödeme 'yi nasıl etkilediğini öğrenin.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 343db43633245030a5eba213cb5c8b79d09a7dee
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686322"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="abf76-103">Azure Marketi için vergi ilkelerinin ödeme nasıl etkilediği</span><span class="sxs-lookup"><span data-stu-id="abf76-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="abf76-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="abf76-104">**Appropriate roles**</span></span>

- <span data-ttu-id="abf76-105">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="abf76-105">Global admin</span></span>
- <span data-ttu-id="abf76-106">Kullanıcı Yönetimi Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="abf76-106">User management admin</span></span>
- <span data-ttu-id="abf76-107">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="abf76-107">Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="abf76-108">Giriş</span><span class="sxs-lookup"><span data-stu-id="abf76-108">Introduction</span></span>

<span data-ttu-id="abf76-109">Microsoft ticari marketi 'nde küresel erişim vardır.</span><span class="sxs-lookup"><span data-stu-id="abf76-109">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="abf76-110">İşlemler, kenarlıkların tamamında ve ISV ve müşterinin bulunduğu yere bağlı olarak, vergi etkilerine karşı farklılık gösterebilir.</span><span class="sxs-lookup"><span data-stu-id="abf76-110">Transactions occur across borders and depending on where the ISV and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="abf76-111">Microsoft AppSource ve Azure Marketi, ISV 'nin ülkesini öğrenmek için Iş Ortağı Merkezi vergi profili bilgilerini kullanır.</span><span class="sxs-lookup"><span data-stu-id="abf76-111">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="abf76-112">Müşterinin ülkesini öğrenmek için müşterinin fatura bilgilerini kullanın ya da müşteri AB 'de ise iki farklı bilgi parçası kullanıyoruz.</span><span class="sxs-lookup"><span data-stu-id="abf76-112">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="abf76-113">Aşağıdaki senaryoları daha iyi anlamak için, Microsoft 'un yayımcı adına vergi toplayıp ödemediğini veya bu sorumluluğun yayımcıya ait olup olmadığını gösteren [vergi ayrıntıları](tax-details-marketplace.md) tablosuna bakın.</span><span class="sxs-lookup"><span data-stu-id="abf76-113">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="abf76-114">Bu konudaki tüm örnek satış değerleri ve vergi yüzdeleri, yalnızca tanım amaçlıdır ve tam sayılar değildir.</span><span class="sxs-lookup"><span data-stu-id="abf76-114">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="abf76-115">Microsoft tarafından yönetilen vergi ülkede yayımcı transacts</span><span class="sxs-lookup"><span data-stu-id="abf76-115">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="abf76-116">**Senaryo a** – [Microsoft tarafından yönetilen bir vergi ülkesindeki](tax-details-marketplace.md#microsoft-managed-countries)bir yayımcı ile müşteri arasında gerçekleşen işlemler.</span><span class="sxs-lookup"><span data-stu-id="abf76-116">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="abf76-117">Bu işlemler, satış sırasında geçerli vergi eklenerek, Microsoft bu vergiyi ilgili ülkeye gönderiyor.</span><span class="sxs-lookup"><span data-stu-id="abf76-117">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="abf76-118">Ödemelerden kesilen vergiler ve ödemesiz hesaplamalar vergi dışlamalı.</span><span class="sxs-lookup"><span data-stu-id="abf76-118">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="abf76-119">ABD dışı Yayımcı ve ABD müşterisi arasındaki işlemler için bkz. [senaryo D](#foreign-publisher-transacts-with-us-customer) .</span><span class="sxs-lookup"><span data-stu-id="abf76-119">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Ödeme işlem senaryosu A için iş akışını gösterir.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="abf76-121">Microsoft tarafından yönetilen ve Market ücreti vergilendirilebilir servis olan Microsoft tarafından yönetilen vergi ülkede yayımcı transacts</span><span class="sxs-lookup"><span data-stu-id="abf76-121">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="abf76-122">**Senaryo B** : ABD tabanlı bir Yayımcı (Iş Ortağı Merkezi vergi profili bilgileri tarafından tanımlandığı gibi) arasında, ülkenin Market ücretine (vergilendirilebilir hizmet) bir vergi sunan Microsoft tarafından yönetilen bir vergi ülkesindeki bir müşteriye yaptığı işlemler.</span><span class="sxs-lookup"><span data-stu-id="abf76-122">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="abf76-123">Bu senaryoda, mağaza hizmeti masrafında vergi, yayımcının ödemsından çıkarılır.</span><span class="sxs-lookup"><span data-stu-id="abf76-123">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Ödeme işlem senaryosu B için iş akışını gösterir.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="abf76-125">Yayımcı tarafından yönetilen vergi ülkesi içindeki Publisher transacts</span><span class="sxs-lookup"><span data-stu-id="abf76-125">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="abf76-126">**Senaryo C** : müşteriler üzerinde bir stopaj vergisi uygulamayan yayımcı tarafından yönetilen bir vergi ülkesindeki bir yayımcı ve müşteri arasında gerçekleşen işlemler.</span><span class="sxs-lookup"><span data-stu-id="abf76-126">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="abf76-127">Müşteriler satış noktasında vergi ödemesiz ve yayımcının tüm geçerli vergileri ödemekle ilgili yükümlülüğünüz.</span><span class="sxs-lookup"><span data-stu-id="abf76-127">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="abf76-128">Ülkeye özgü fiyatlandırmayla ilgili daha fazla bilgi için (örneğin, yaklaşan vergilendirme 'yi kaydırmak için) bkz. [ticari Market teklifleri Için planlar ve fiyatlandırma](/azure/marketplace/plans-pricing#custom-prices).</span><span class="sxs-lookup"><span data-stu-id="abf76-128">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Ödeme işlem senaryosu C için iş akışını gösterir.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="abf76-130">ABD müşterisi ile yabancı yayımcı transacts</span><span class="sxs-lookup"><span data-stu-id="abf76-130">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="abf76-131">**Senaryo D** – tüm yabancı yayımcılar (Iş Ortağı Merkezi vergi profili bilgileri tarafından tanımlandığı şekilde) ABD 'de bir müşteriye (müşteri hesabı adresleri tarafından tanımlandığı [gibi) bir](#foreign-publisher-with-a-treaty-transacts-with-us-customer)satış yapma.</span><span class="sxs-lookup"><span data-stu-id="abf76-131">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="abf76-132">ABD Kamu, Microsoft 'un yayımcı adına vergi stopajın olmasını gerektirir.</span><span class="sxs-lookup"><span data-stu-id="abf76-132">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="abf76-133">Ödemelerden yayımcıya kesilen vergi, teklif fiyatına göre hesaplanır.</span><span class="sxs-lookup"><span data-stu-id="abf76-133">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Ödeme işlem senaryosu D için iş akışını gösterir.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="abf76-135">ABD müşterisi ile bir Treaty transacts ile yabancı Yayımcı</span><span class="sxs-lookup"><span data-stu-id="abf76-135">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="abf76-136">**Senaryo E** – tüm yabancı yayımcılar (Iş Ortağı Merkezi vergi profili bilgileri tarafından tanımlandığı gibi) ABD ile ilgili bir müşteriye satış yapan (müşteri hesabı adresleri tarafından tanımlandığı şekılde) ABD</span><span class="sxs-lookup"><span data-stu-id="abf76-136">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="abf76-137">ABD Kamu, Microsoft 'un yayımcı adına vergi stopaj uygulamasına gerek yoktur.</span><span class="sxs-lookup"><span data-stu-id="abf76-137">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Ödeme işlem senaryosu E için iş akışını gösterir.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="abf76-139">Yabancı Yayımcı, Microsoft tarafından yönetilen bir ülkede (Irlanda dışında) bir AB KDV 'ye kayıtlı müşteriye satış sağlar</span><span class="sxs-lookup"><span data-stu-id="abf76-139">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="abf76-140">**Senaryo F** – Microsoft-Managed bir ülkede yabancı YAYıMCıLAR ve AB ile kayıtlı müşteriler (İrlanda dışında) arasındaki tüm işlemler.</span><span class="sxs-lookup"><span data-stu-id="abf76-140">**Scenario F** – All transactions between foreign publishers and EU VAT-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="abf76-141">Müşteri, satışla ilgili vergiyi ödemez.</span><span class="sxs-lookup"><span data-stu-id="abf76-141">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Ödeme işlem senaryosu F için iş akışını gösterir.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="abf76-143">Yabancı Yayımcı, Microsoft tarafından yönetilen bir ülkede bir AB KDV 'ye kayıtlı müşteriye satıl (Irlanda 'da)</span><span class="sxs-lookup"><span data-stu-id="abf76-143">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="abf76-144">**Senaryo G** – bir Microsoft-Managed ülkede yabancı YAYıMCıLAR ve AB ile kayıtlı müşteriler arasındaki tüm Işlemler (İrlanda içi).</span><span class="sxs-lookup"><span data-stu-id="abf76-144">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="abf76-145">Müşteri Irlanda KDV 'sini ödeder ve Microsoft bu vergiyi Irlanda devlet kurumuna ödeder.</span><span class="sxs-lookup"><span data-stu-id="abf76-145">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Ödeme işlem senaryosu G için iş akışını gösterir.":::

## <a name="next-steps"></a><span data-ttu-id="abf76-147">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="abf76-147">Next steps</span></span>

- [<span data-ttu-id="abf76-148">Yayımcı hakkında SSS</span><span class="sxs-lookup"><span data-stu-id="abf76-148">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="abf76-149">Ödeme ve vergi profilleri oluşturma yönergeleri</span><span class="sxs-lookup"><span data-stu-id="abf76-149">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)