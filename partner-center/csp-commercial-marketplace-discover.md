---
title: Teklifleri bulma-ticari Market
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP iş ortaklarının, bağımsız yazılım satıcılarından (ISV) SaaS teklifleri veya fiyatlandırma için Market 'i görüntülemek veya aramak üzere Iş ortağı merkezini nasıl kullanabileceği hakkında bilgi edinin.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f741ef4e44632e1d239285b58e99fbb38a8f37e7
ms.sourcegitcommit: a78dd3c532860d01867d116bfb4e2c88b84bcd25
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/08/2021
ms.locfileid: "97979609"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a><span data-ttu-id="1138e-103">Partner Center ticari marketi 'nde teklifleri ve fiyatları bulma</span><span class="sxs-lookup"><span data-stu-id="1138e-103">Discover offers and pricing in Partner Center commercial marketplace</span></span>

<span data-ttu-id="1138e-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="1138e-104">**Appropriate roles**</span></span>

- <span data-ttu-id="1138e-105">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="1138e-105">Global admin</span></span>
- <span data-ttu-id="1138e-106">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="1138e-106">Admin agent</span></span>

<span data-ttu-id="1138e-107">Bağımsız yazılım satıcıları (ISV 'Ler), ticari Market 'te teklif yayımlamayı tercih ettikleri zaman, teklifin CSP programında kullanılabilir hale getirilme konusunda da karar verebilir.</span><span class="sxs-lookup"><span data-stu-id="1138e-107">When Independent Software Vendors (ISVs) choose to publish an offer in the commercial marketplace, they can also decide if they want the offer to be made available in the CSP program.</span></span> <span data-ttu-id="1138e-108">Teklifi CSP programı aracılığıyla satmayı tercih ediyorsanız, CSP iş ortakları Partner Center marketi alanında teklifi görmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="1138e-108">If they choose to sell the offer through the CSP program, CSP partners should see the offer in Partner Center Marketplace area.</span></span>

<span data-ttu-id="1138e-109">Bir ISV teklifi, Iş Ortağı Merkezi 'nde beklemiş gibi görünmezse şu olabilir:</span><span class="sxs-lookup"><span data-stu-id="1138e-109">If an ISV offer does not appear as you expect in Partner Center, it may be because:</span></span>

- <span data-ttu-id="1138e-110">ISV, teklifi CSP programı aracılığıyla satmamaya karar verdi.</span><span class="sxs-lookup"><span data-stu-id="1138e-110">The ISV decided not to sell the offer through the CSP program.</span></span> <span data-ttu-id="1138e-111">Örneğin, bazı ISV ürünleri ticari Market 'in diğer alanlarında (örneğin, [Microsoft AppSource](https://appsource.microsoft.com/) ve [Azure Marketi](https://azuremarketplace.microsoft.com/)'nde) kullanıma sunulmuştur, ancak iş ortağı merkezi marketi 'nde CSP programındaki iş ortakları için görünmeyebilir.</span><span class="sxs-lookup"><span data-stu-id="1138e-111">For example, some ISV products may have been made available in other areas of the commercial marketplace (such as in [Microsoft AppSource](https://appsource.microsoft.com/) and [Azure Marketplace](https://azuremarketplace.microsoft.com/)), but may not appear for partners in the CSP program in Partner Center marketplace.</span></span>

- <span data-ttu-id="1138e-112">ISV, teklifi yalnızca belirli sayıda CSP iş ortağı için özel olarak yapmaya karar verdi.</span><span class="sxs-lookup"><span data-stu-id="1138e-112">The ISV decided to make the offer exclusive to only a select number of CSP partners.</span></span> <span data-ttu-id="1138e-113">Özel teklifler hakkında daha fazla bilgi için bu Yardım konusunun devamındaki bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="1138e-113">For more information about exclusive offers, see later in this help topic.</span></span>

- <span data-ttu-id="1138e-114">Teklif türü, Iş ortağı merkezi veya Azure portal (örn. kapsayıcılar veya bazı kullanım tabanlı teklifler) üzerinden transactable olamaz.</span><span class="sxs-lookup"><span data-stu-id="1138e-114">The offer type may not be transactable through Partner Center or Azure portal (e.g. Containers or some usage-based offers).</span></span>

- <span data-ttu-id="1138e-115">İlişkili müşterilerinizin faturalandırma ülkesi bu ISV teklifi için desteklenmiyor olabilir.</span><span class="sxs-lookup"><span data-stu-id="1138e-115">The billing country of your associated customer(s) may not be supported for this ISV offer.</span></span>

## <a name="view-marketplace-offers-in-partner-center"></a><span data-ttu-id="1138e-116">Market tekliflerini Iş Ortağı Merkezi 'nde görüntüleyin</span><span class="sxs-lookup"><span data-stu-id="1138e-116">View Marketplace offers in Partner Center</span></span>

<span data-ttu-id="1138e-117">Kullanılabilir ticari Market tekliflerini CSP programında görüntülemek için:</span><span class="sxs-lookup"><span data-stu-id="1138e-117">To view available commercial marketplace offers in the CSP program:</span></span>

1. <span data-ttu-id="1138e-118">Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın ve ardından sol gezinti menüsünden **CSP** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="1138e-118">Sign into Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **CSP** from the left navigation menu.</span></span>

2. <span data-ttu-id="1138e-119">**Satış** ve ardından **Market**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="1138e-119">Select **Sell**, followed by **Marketplace**.</span></span> <span data-ttu-id="1138e-120">Varsayılan olarak, tüm türlerin ve kategorilerin ürünlerini görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="1138e-120">By default, you will see products of all types and categories.</span></span>

3. <span data-ttu-id="1138e-121">Türe veya kategoriye göre bir filtre seçin.</span><span class="sxs-lookup"><span data-stu-id="1138e-121">Select a filter by type or category.</span></span> <span data-ttu-id="1138e-122">Ayrıca, belirli anahtar sözcükleri, teklif adlarını veya ISV yayımcılarının adlarını bulmak için **Ara** ' yı kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1138e-122">You can also use **Search** to find specific keywords, offer names or the names of ISV publishers.</span></span>

4. <span data-ttu-id="1138e-123">Listeden belirli bir ürün teklifi seçin.</span><span class="sxs-lookup"><span data-stu-id="1138e-123">Select a specific product offer from the list.</span></span> <span data-ttu-id="1138e-124">Bu, size teklif hakkında daha fazla bilgi oluşturabileceğiniz bir ürün genel bakış sekmesine götürür.</span><span class="sxs-lookup"><span data-stu-id="1138e-124">This will take you to a product Overview tab where you can learn more about the offer.</span></span> <span data-ttu-id="1138e-125">Bu sekmeyle ilgili bilgiler şunları içerebilir:</span><span class="sxs-lookup"><span data-stu-id="1138e-125">Information on this tab might include:</span></span> 

    - <span data-ttu-id="1138e-126">Ürün veya teklifin açıklaması</span><span class="sxs-lookup"><span data-stu-id="1138e-126">A description of the product or offer</span></span>

    - <span data-ttu-id="1138e-127">ISV yayımcısı hakkında daha fazla bilgi</span><span class="sxs-lookup"><span data-stu-id="1138e-127">More information about the ISV publisher</span></span>

    - <span data-ttu-id="1138e-128">ISV yayımcısı tarafından karşıya yüklenen belgelerin veya pazarlama malzemelerinin bağlantıları</span><span class="sxs-lookup"><span data-stu-id="1138e-128">Links to documentation or marketing materials uploaded by the ISV publisher</span></span>

    - <span data-ttu-id="1138e-129">Müşteri desteği, mühendislik veya CSP programına yönelik bir iletişim için olası diğer ISV kişileri</span><span class="sxs-lookup"><span data-stu-id="1138e-129">Other possible ISV contacts for customer support, engineering, or a contact for the CSP program</span></span>

5. <span data-ttu-id="1138e-130">Bir teklifin kullanılabilir planları, SKU 'Ları veya fiyatlandırma hakkında daha fazla bilgi için **planlar + fiyatlandırma** sekmesini seçin. Bu sekmede şu görünür:</span><span class="sxs-lookup"><span data-stu-id="1138e-130">To see more information about an offer's available plans, SKUs, or pricing, select the **Plans + Pricing** tab. This tab will show you:</span></span>

    - <span data-ttu-id="1138e-131">Bu teklifin sizin için kullanılabildiği pazarlar</span><span class="sxs-lookup"><span data-stu-id="1138e-131">The markets where this offer is available to you</span></span>

    - <span data-ttu-id="1138e-132">Teklif için kullanılabilir SKU 'Ların veya planların listesi</span><span class="sxs-lookup"><span data-stu-id="1138e-132">A list of SKUs or plans available for the offer</span></span>

    - <span data-ttu-id="1138e-133">Her SKU veya plana ilişkin fiyatlandırma</span><span class="sxs-lookup"><span data-stu-id="1138e-133">Pricing for each SKU or Plan available</span></span>

## <a name="view-marketplace-offers-via-partner-center-apis"></a><span data-ttu-id="1138e-134">Market tekliflerini Iş Ortağı Merkezi API 'Leri aracılığıyla görüntüleme</span><span class="sxs-lookup"><span data-stu-id="1138e-134">View Marketplace offers via Partner Center APIs</span></span>

<span data-ttu-id="1138e-135">CSP Program ortakları, uygun tekliflerin bir listesini döndürmek için API 'Leri de kullanabilir.</span><span class="sxs-lookup"><span data-stu-id="1138e-135">CSP program partners can also use APIs to return a list of eligible offers.</span></span> <span data-ttu-id="1138e-136">Uygun teklifler yalnızca iş ortağının Partner Center Marketi aracılığıyla satıtabilecekleri SaaS ISV teklifleri olacaktır.</span><span class="sxs-lookup"><span data-stu-id="1138e-136">Eligible offers will be only those SaaS ISV offers available for the partner to sell via Partner Center marketplace.</span></span> <span data-ttu-id="1138e-137">Katalogdaki teklifleri tanımlamak üzere API 'Leri kullanan iş ortakları için, [bir pazara yönelik tekliflerin bir listesini elde etme](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)kılavuzuna bakın.</span><span class="sxs-lookup"><span data-stu-id="1138e-137">For partners using APIs to identify offers in the catalog, refer to the guidance to [obtain a list of offers for a market](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market).</span></span>

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a><span data-ttu-id="1138e-138">Iş Ortağı Merkezi 'nde en son Market teklif fiyatlandırmasını görüntüleme</span><span class="sxs-lookup"><span data-stu-id="1138e-138">View the latest Marketplace offer pricing in Partner Center</span></span>

<span data-ttu-id="1138e-139">Teklifle ilişkili en son fiyatlandırma ayrıntıları için aşağıdaki adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="1138e-139">Follow these steps for the latest pricing details associated with an offer:</span></span>

1. <span data-ttu-id="1138e-140">Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın ve ardından sol gezinti menüsünden **CSP** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="1138e-140">Sign into Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **CSP** from the left navigation menu.</span></span>

2. <span data-ttu-id="1138e-141">**Satış**' yı, ardından **fiyatlandırma ve tekliflerle** seçin.</span><span class="sxs-lookup"><span data-stu-id="1138e-141">Select **Sell**, followed by **Pricing and offers**.</span></span>

3. <span data-ttu-id="1138e-142">**Market** bölümüne gidin, bir konum seçin ve **Market fiyatlandırmasını** indirin.</span><span class="sxs-lookup"><span data-stu-id="1138e-142">Scroll down to the **Marketplace** section, select a location and download **Marketplace pricing**.</span></span> <span data-ttu-id="1138e-143">Bu, ISV yayımcılarından sunulan SaaS, lisans tabanlı teklifler ve tarifeli tekliflerle ilgili en son fiyatlandırma verilerine sahip bir elektronik tablo oluşturur.</span><span class="sxs-lookup"><span data-stu-id="1138e-143">This generates a spreadsheet with the latest pricing data for SaaS, license-based offers and metered offers available from ISV publishers.</span></span> <span data-ttu-id="1138e-144">Burada bazı Azure uygulama fiyatları da görüntülenebilir.</span><span class="sxs-lookup"><span data-stu-id="1138e-144">Some Azure application pricing may also appear here.</span></span> <span data-ttu-id="1138e-145">Bu bilgiler günlük olarak güncelleştirilir, bu sayede seçtiğiniz sıklıkta geçerli fiyatlar için kontrol edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1138e-145">This information is updated daily, so you can check it for current prices as often as you choose.</span></span>

4. <span data-ttu-id="1138e-146">Bir ISV ürünü ücretsiz deneme süresi içeriyorsa, bu ürün için iki satır görüntülenir:</span><span class="sxs-lookup"><span data-stu-id="1138e-146">If an ISV product includes a free trial period, the spreadsheet will display two rows for that product:</span></span>

    - <span data-ttu-id="1138e-147">Bir satırda, sıfır olan ücretsiz deneme fiyatı gösterilmektedir.</span><span class="sxs-lookup"><span data-stu-id="1138e-147">One row shows the free trial price of zero.</span></span> <span data-ttu-id="1138e-148">Bu, ücretsiz deneme süresinin kullanılabildiği anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="1138e-148">This means a free trial period is available.</span></span>

    - <span data-ttu-id="1138e-149">Diğer satır, ücretsiz deneme süresi bittikten sonra uygulanacak fiyat ve koşulları gösterir.</span><span class="sxs-lookup"><span data-stu-id="1138e-149">The other row shows the price and terms that will apply after the free trial period is over.</span></span>

<span data-ttu-id="1138e-150">CSP program ortağı olarak, belirli ticari Market tekliflerle ilişkili diğer teşvikleri için uygun olabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1138e-150">As a CSP program partner, you may be eligible for other incentives associated with certain commercial marketplace offers.</span></span> <span data-ttu-id="1138e-151">Diğer teşvikleri hakkında daha fazla bilgi için bkz. [CSP özeni Kılavuzu](https://aka.ms/partnerincentives) (CSP oturumu gerektirir).</span><span class="sxs-lookup"><span data-stu-id="1138e-151">For more information about other incentives, see the [CSP incentive guide](https://aka.ms/partnerincentives) (requires CSP login).</span></span>

## <a name="learn-about-marketplace-exclusive-offers"></a><span data-ttu-id="1138e-152">Market özel teklifleri hakkında bilgi edinin</span><span class="sxs-lookup"><span data-stu-id="1138e-152">Learn about marketplace exclusive offers</span></span>

<span data-ttu-id="1138e-153">ISV 'Ler, tekliflerini yalnızca CSP programındaki belirli iş ortakları için kullanılabilir hale getirme seçeneğine sahiptir.</span><span class="sxs-lookup"><span data-stu-id="1138e-153">ISVs have the option to make their offers available only to specific partners in the CSP program.</span></span> <span data-ttu-id="1138e-154">Bu, özel bir teklif olarak bilinir.</span><span class="sxs-lookup"><span data-stu-id="1138e-154">This is known as an Exclusive offer.</span></span> <span data-ttu-id="1138e-155">CSP programındaki tüm iş ortakları, özel olarak işaretlenmiş teklifler de dahil olmak üzere Iş ortağı merkezi ticari Market 'teki tüm ISV tekliflerini hala görüntüleyebilir.</span><span class="sxs-lookup"><span data-stu-id="1138e-155">All partners in the CSP program can still view all ISV offers in Partner Center commercial marketplace, including those offers marked Exclusive.</span></span>

<span data-ttu-id="1138e-156">Bir teklif özel olarak **işaretlenmediğinde** , tüm iş ortakları bu teklifi satın alabilir (Seçili müşterinin faturalandırma ÜLKESI, ISV teklifinin ülke kullanılabilirliği ile eşleştiğinde).</span><span class="sxs-lookup"><span data-stu-id="1138e-156">If an offer is **not** marked Exclusive, all partners can purchase that offer (assuming the selected customer’s billing country matches the country availability of the ISV's offer).</span></span>

<span data-ttu-id="1138e-157">Ancak özel olarak işaretlenmiş tüm teklifler için, yalnızca ISV tarafından seçilen iş ortakları bu teklifi satın alabilir.</span><span class="sxs-lookup"><span data-stu-id="1138e-157">For any offer marked Exclusive, however, only those partners selected by the ISV will be able to purchase that offer.</span></span>

> [!NOTE]
> <span data-ttu-id="1138e-158">Müşterilerinize satmak istediğiniz özel olarak işaretlenmiş bir teklif görürseniz, doğrudan ISV 'ye ulaşın ve özel teklifi satma izni isteyin.</span><span class="sxs-lookup"><span data-stu-id="1138e-158">If you see an offer marked Exclusive that you would like to sell to your customers, reach out to the ISV directly and ask for permission to sell the Exclusive offer.</span></span> <span data-ttu-id="1138e-159">Özel bir teklifin ayrıntılarını görüntülediğinizde seçebileceğiniz bir **ILETIŞIM ISV** bağlantısı görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="1138e-159">When you view the details of an Exclusive offer, you may see a **Contact ISV** link that you can select.</span></span>

<span data-ttu-id="1138e-160">Ticari Market 'teki ISV deneyimi hakkında daha fazla bilgi edinmek için, [bulut çözümü sağlayıcılarını](/azure/marketplace/cloud-solution-providers)okuyun.</span><span class="sxs-lookup"><span data-stu-id="1138e-160">To learn more about the ISV experience in the commercial marketplace, read [Cloud Solution Providers](/azure/marketplace/cloud-solution-providers).</span></span>

<span data-ttu-id="1138e-161">Market 'teki CSP deneyimi hakkında daha fazla bilgi için [ticari Market 'e genel bakış](csp-commercial-marketplace-overview.md)makalesini okuyun.</span><span class="sxs-lookup"><span data-stu-id="1138e-161">For more information on the CSP experience in the marketplace, read [Commercial marketplace overview](csp-commercial-marketplace-overview.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="1138e-162">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="1138e-162">Next steps</span></span>

- [<span data-ttu-id="1138e-163">Ticari Market tekliflerini satın alma</span><span class="sxs-lookup"><span data-stu-id="1138e-163">Purchase commercial marketplace offers</span></span>](csp-commercial-marketplace-purchase.md)