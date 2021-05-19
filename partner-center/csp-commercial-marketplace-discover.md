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
ms.openlocfilehash: ab30f8391df58155c8511dc628b1fefd94c8d768
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147981"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a><span data-ttu-id="f2990-103">Partner Center ticari marketi 'nde teklifleri ve fiyatları bulma</span><span class="sxs-lookup"><span data-stu-id="f2990-103">Discover offers and pricing in Partner Center commercial marketplace</span></span>

<span data-ttu-id="f2990-104">**Uygun roller**: genel yönetici | Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="f2990-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="f2990-105">Bağımsız yazılım satıcıları (ISV 'Ler), ticari Market 'te teklif yayımlamayı tercih ettikleri zaman, teklifin CSP programında kullanılabilir hale getirilme konusunda da karar verebilir.</span><span class="sxs-lookup"><span data-stu-id="f2990-105">When Independent Software Vendors (ISVs) choose to publish an offer in the commercial marketplace, they can also decide if they want the offer to be made available in the CSP program.</span></span> <span data-ttu-id="f2990-106">Teklifi CSP programı aracılığıyla satmayı tercih ediyorsanız, CSP iş ortakları Partner Center marketi alanında teklifi görmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="f2990-106">If they choose to sell the offer through the CSP program, CSP partners should see the offer in Partner Center Marketplace area.</span></span>

<span data-ttu-id="f2990-107">Bir ISV teklifi, Iş Ortağı Merkezi 'nde beklemiş gibi görünmezse şu olabilir:</span><span class="sxs-lookup"><span data-stu-id="f2990-107">If an ISV offer does not appear as you expect in Partner Center, it may be because:</span></span>

- <span data-ttu-id="f2990-108">ISV, teklifi CSP programı aracılığıyla satmamaya karar verdi.</span><span class="sxs-lookup"><span data-stu-id="f2990-108">The ISV decided not to sell the offer through the CSP program.</span></span> <span data-ttu-id="f2990-109">Örneğin, bazı ISV ürünleri ticari Market 'in diğer alanlarında (örneğin, [Microsoft AppSource](https://appsource.microsoft.com/) ve [Azure Marketi](https://azuremarketplace.microsoft.com/)'nde) kullanıma sunulmuştur, ancak iş ortağı merkezi marketi 'nde CSP programındaki iş ortakları için görünmeyebilir.</span><span class="sxs-lookup"><span data-stu-id="f2990-109">For example, some ISV products may have been made available in other areas of the commercial marketplace (such as in [Microsoft AppSource](https://appsource.microsoft.com/) and [Azure Marketplace](https://azuremarketplace.microsoft.com/)), but may not appear for partners in the CSP program in Partner Center marketplace.</span></span>

- <span data-ttu-id="f2990-110">ISV, teklifi yalnızca belirli sayıda CSP iş ortağı için özel olarak yapmaya karar verdi.</span><span class="sxs-lookup"><span data-stu-id="f2990-110">The ISV decided to make the offer exclusive to only a select number of CSP partners.</span></span> <span data-ttu-id="f2990-111">Özel teklifler hakkında daha fazla bilgi için bu Yardım konusunun devamındaki bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="f2990-111">For more information about exclusive offers, see later in this help topic.</span></span>

- <span data-ttu-id="f2990-112">Teklif türü, Iş ortağı merkezi veya Azure portal (örn. kapsayıcılar veya bazı kullanım tabanlı teklifler) üzerinden transactable olamaz.</span><span class="sxs-lookup"><span data-stu-id="f2990-112">The offer type may not be transactable through Partner Center or Azure portal (e.g. Containers or some usage-based offers).</span></span>

- <span data-ttu-id="f2990-113">İlişkili müşterilerinizin faturalandırma ülkesi bu ISV teklifi için desteklenmiyor olabilir.</span><span class="sxs-lookup"><span data-stu-id="f2990-113">The billing country of your associated customer(s) may not be supported for this ISV offer.</span></span>

## <a name="view-marketplace-offers-in-partner-center"></a><span data-ttu-id="f2990-114">Market tekliflerini Iş Ortağı Merkezi 'nde görüntüleyin</span><span class="sxs-lookup"><span data-stu-id="f2990-114">View Marketplace offers in Partner Center</span></span>

<span data-ttu-id="f2990-115">Kullanılabilir ticari Market tekliflerini CSP programında görüntülemek için:</span><span class="sxs-lookup"><span data-stu-id="f2990-115">To view available commercial marketplace offers in the CSP program:</span></span>

1. <span data-ttu-id="f2990-116">Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın ve ardından sol gezinti menüsünden **CSP** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="f2990-116">Sign into Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **CSP** from the left navigation menu.</span></span>

2. <span data-ttu-id="f2990-117">**Satış** ve ardından **Market**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="f2990-117">Select **Sell**, followed by **Marketplace**.</span></span> <span data-ttu-id="f2990-118">Varsayılan olarak, tüm türlerin ve kategorilerin ürünlerini görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="f2990-118">By default, you will see products of all types and categories.</span></span>

3. <span data-ttu-id="f2990-119">Türe veya kategoriye göre bir filtre seçin.</span><span class="sxs-lookup"><span data-stu-id="f2990-119">Select a filter by type or category.</span></span> <span data-ttu-id="f2990-120">Ayrıca, belirli anahtar sözcükleri, teklif adlarını veya ISV yayımcılarının adlarını bulmak için **Ara** ' yı kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f2990-120">You can also use **Search** to find specific keywords, offer names or the names of ISV publishers.</span></span>

4. <span data-ttu-id="f2990-121">Listeden belirli bir ürün teklifi seçin.</span><span class="sxs-lookup"><span data-stu-id="f2990-121">Select a specific product offer from the list.</span></span> <span data-ttu-id="f2990-122">Bu sizi teklif hakkında daha fazla bilgi edinmek için bir ürüne Genel Bakış sekmesine alır.</span><span class="sxs-lookup"><span data-stu-id="f2990-122">This will take you to a product Overview tab where you can learn more about the offer.</span></span> <span data-ttu-id="f2990-123">Bu sekmede yer alan bilgiler şunlar olabilir:</span><span class="sxs-lookup"><span data-stu-id="f2990-123">Information on this tab might include:</span></span> 

    - <span data-ttu-id="f2990-124">Ürün veya teklif açıklaması</span><span class="sxs-lookup"><span data-stu-id="f2990-124">A description of the product or offer</span></span>

    - <span data-ttu-id="f2990-125">ISV yayımcısı hakkında daha fazla bilgi</span><span class="sxs-lookup"><span data-stu-id="f2990-125">More information about the ISV publisher</span></span>

    - <span data-ttu-id="f2990-126">ISV yayımcısı tarafından karşıya yüklenen belgelere veya pazarlama malzemelerine bağlantılar</span><span class="sxs-lookup"><span data-stu-id="f2990-126">Links to documentation or marketing materials uploaded by the ISV publisher</span></span>

    - <span data-ttu-id="f2990-127">Müşteri desteği, mühendislik veya CSP programıyla ilgili bir iletişim için diğer olası ISV kişileri</span><span class="sxs-lookup"><span data-stu-id="f2990-127">Other possible ISV contacts for customer support, engineering, or a contact for the CSP program</span></span>

5. <span data-ttu-id="f2990-128">Bir teklifin kullanılabilir planları, SKU'ları veya fiyatlandırması hakkında daha fazla bilgi için Planlar **+ Fiyatlandırma sekmesini** seçin. Bu sekme size şunları gösterir:</span><span class="sxs-lookup"><span data-stu-id="f2990-128">To see more information about an offer's available plans, SKUs, or pricing, select the **Plans + Pricing** tab. This tab will show you:</span></span>

    - <span data-ttu-id="f2990-129">Bu teklifin kullanılabilir olduğu pazarlar</span><span class="sxs-lookup"><span data-stu-id="f2990-129">The markets where this offer is available to you</span></span>

    - <span data-ttu-id="f2990-130">Teklif için kullanılabilen SKUS'ların veya planların listesi</span><span class="sxs-lookup"><span data-stu-id="f2990-130">A list of SKUs or plans available for the offer</span></span>

    - <span data-ttu-id="f2990-131">Kullanılabilir her SKU veya Plan için fiyatlandırma</span><span class="sxs-lookup"><span data-stu-id="f2990-131">Pricing for each SKU or Plan available</span></span>

## <a name="view-marketplace-offers-via-partner-center-apis"></a><span data-ttu-id="f2990-132">İş Ortağı Merkezi API'leri aracılığıyla Market tekliflerini görüntüleme</span><span class="sxs-lookup"><span data-stu-id="f2990-132">View Marketplace offers via Partner Center APIs</span></span>

<span data-ttu-id="f2990-133">CSP programı iş ortakları uygun tekliflerin listesini almak için API'leri de kullanabilir.</span><span class="sxs-lookup"><span data-stu-id="f2990-133">CSP program partners can also use APIs to return a list of eligible offers.</span></span> <span data-ttu-id="f2990-134">Uygun teklifler yalnızca iş ortağının market üzerinden satışa sunduğu SaaS ISV İş Ortağı Merkezi olur.</span><span class="sxs-lookup"><span data-stu-id="f2990-134">Eligible offers will be only those SaaS ISV offers available for the partner to sell via Partner Center marketplace.</span></span> <span data-ttu-id="f2990-135">Katalogda teklifleri belirlemek için API'leri kullanan iş ortakları için pazara yönelik [tekliflerin listesini almak için rehbere bakın.](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)</span><span class="sxs-lookup"><span data-stu-id="f2990-135">For partners using APIs to identify offers in the catalog, refer to the guidance to [obtain a list of offers for a market](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market).</span></span>

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a><span data-ttu-id="f2990-136">En son Market teklifi fiyatlandırması bilgilerini İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="f2990-136">View the latest Marketplace offer pricing in Partner Center</span></span>

<span data-ttu-id="f2990-137">Teklifle ilişkili en son fiyatlandırma ayrıntıları için şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="f2990-137">Follow these steps for the latest pricing details associated with an offer:</span></span>

1. <span data-ttu-id="f2990-138">Panoda İş Ortağı Merkezi [açın](https://partner.microsoft.com/dashboard)ve ardından sol gezinti **menüsünden CSP'yi** seçin.</span><span class="sxs-lookup"><span data-stu-id="f2990-138">Sign into Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **CSP** from the left navigation menu.</span></span>

2. <span data-ttu-id="f2990-139">**Satış'ı** ve ardından Fiyatlandırma **ve teklifler'i seçin.**</span><span class="sxs-lookup"><span data-stu-id="f2990-139">Select **Sell**, followed by **Pricing and offers**.</span></span>

3. <span data-ttu-id="f2990-140">Sayfayı aşağı kaydırarak **Market** bölümüne gidin, bir konum seçin ve Market **fiyatlandırması'ı indirin.**</span><span class="sxs-lookup"><span data-stu-id="f2990-140">Scroll down to the **Marketplace** section, select a location and download **Marketplace pricing**.</span></span> <span data-ttu-id="f2990-141">Bu, ISV yayımcılarının sunduğu SaaS, lisans tabanlı teklifler ve tarifeli teklifler için en son fiyatlandırma verilerini içeren bir elektronik tablo oluşturulur.</span><span class="sxs-lookup"><span data-stu-id="f2990-141">This generates a spreadsheet with the latest pricing data for SaaS, license-based offers and metered offers available from ISV publishers.</span></span> <span data-ttu-id="f2990-142">Bazı Azure uygulama fiyatlandırması da burada görünebilir.</span><span class="sxs-lookup"><span data-stu-id="f2990-142">Some Azure application pricing may also appear here.</span></span> <span data-ttu-id="f2990-143">Bu bilgiler günlük olarak güncelleştirilir, bu nedenle seçtiğiniz sıklıkta geçerli fiyatları kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="f2990-143">This information is updated daily, so you can check it for current prices as often as you choose.</span></span>

4. <span data-ttu-id="f2990-144">IsV ürünü ücretsiz deneme süresine sahipse elektronik tabloda bu ürün için iki satır görüntülenir:</span><span class="sxs-lookup"><span data-stu-id="f2990-144">If an ISV product includes a free trial period, the spreadsheet will display two rows for that product:</span></span>

    - <span data-ttu-id="f2990-145">Bir satırda ücretsiz deneme fiyatı sıfır olarak gösterir.</span><span class="sxs-lookup"><span data-stu-id="f2990-145">One row shows the free trial price of zero.</span></span> <span data-ttu-id="f2990-146">Bu, ücretsiz deneme süresi olduğu anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="f2990-146">This means a free trial period is available.</span></span>

    - <span data-ttu-id="f2990-147">Diğer satırda, ücretsiz deneme süresi sona erdikten sonra uygulanacak fiyat ve koşullar yer atılır.</span><span class="sxs-lookup"><span data-stu-id="f2990-147">The other row shows the price and terms that will apply after the free trial period is over.</span></span>

<span data-ttu-id="f2990-148">CSP programı iş ortağı olarak, belirli ticari market teklifleriyle ilişkili diğer teşvikler için uygun olabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f2990-148">As a CSP program partner, you may be eligible for other incentives associated with certain commercial marketplace offers.</span></span> <span data-ttu-id="f2990-149">Diğer teşvikler hakkında daha fazla bilgi için CSP teşvik [kılavuzuna](https://aka.ms/partnerincentives) bakın (CSP oturum açması gerekir).</span><span class="sxs-lookup"><span data-stu-id="f2990-149">For more information about other incentives, see the [CSP incentive guide](https://aka.ms/partnerincentives) (requires CSP login).</span></span>

## <a name="learn-about-marketplace-exclusive-offers"></a><span data-ttu-id="f2990-150">Markete özel teklifler hakkında bilgi alın</span><span class="sxs-lookup"><span data-stu-id="f2990-150">Learn about marketplace exclusive offers</span></span>

<span data-ttu-id="f2990-151">ISV'ler tekliflerini yalnızca CSP programında belirli iş ortakları tarafından kullanılabilir yapma seçeneğine sahip.</span><span class="sxs-lookup"><span data-stu-id="f2990-151">ISVs have the option to make their offers available only to specific partners in the CSP program.</span></span> <span data-ttu-id="f2990-152">Bu, Özel teklif olarak bilinir.</span><span class="sxs-lookup"><span data-stu-id="f2990-152">This is known as an Exclusive offer.</span></span> <span data-ttu-id="f2990-153">CSP programıyla tüm iş ortakları, Özel olarak işaretlenen teklifler de dahil İş Ortağı Merkezi ticari markette tüm ISV tekliflerini görüntülemeye devam ediyor.</span><span class="sxs-lookup"><span data-stu-id="f2990-153">All partners in the CSP program can still view all ISV offers in Partner Center commercial marketplace, including those offers marked Exclusive.</span></span>

<span data-ttu-id="f2990-154">Bir teklif Özel **olarak** işaretlenmemişse, tüm iş ortakları bu teklifi satın alır (seçilen müşterinin fatura ülkesi ISV'nin teklifinin ülke kullanılabilirliğiyle eş olduğu varsayıldı).</span><span class="sxs-lookup"><span data-stu-id="f2990-154">If an offer is **not** marked Exclusive, all partners can purchase that offer (assuming the selected customer’s billing country matches the country availability of the ISV's offer).</span></span>

<span data-ttu-id="f2990-155">Ancak Özel olarak işaretlenen tüm tekliflere yalnızca ISV tarafından seçilen iş ortakları bu teklifi satın alma seçeneğine sahip olur.</span><span class="sxs-lookup"><span data-stu-id="f2990-155">For any offer marked Exclusive, however, only those partners selected by the ISV will be able to purchase that offer.</span></span>

> [!NOTE]
> <span data-ttu-id="f2990-156">Müşterilerinize satış yapmak için Özel olarak işaretlenmiş bir teklif görüyorsanız doğrudan ISV'ye ulaşıp Özel teklifin satış iznini istemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="f2990-156">If you see an offer marked Exclusive that you would like to sell to your customers, reach out to the ISV directly and ask for permission to sell the Exclusive offer.</span></span> <span data-ttu-id="f2990-157">Özel bir teklifin ayrıntılarını görüntülenin, seçerek bir **Kişi ISV** bağlantısıyla karşıdan ulaşabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f2990-157">When you view the details of an Exclusive offer, you may see a **Contact ISV** link that you can select.</span></span>

<span data-ttu-id="f2990-158">Ticari markette ISV deneyimi hakkında daha fazla bilgi edinmek için Bulut Çözümü Sağlayıcıları [makalelerini okuyun.](/azure/marketplace/cloud-solution-providers)</span><span class="sxs-lookup"><span data-stu-id="f2990-158">To learn more about the ISV experience in the commercial marketplace, read [Cloud Solution Providers](/azure/marketplace/cloud-solution-providers).</span></span>

<span data-ttu-id="f2990-159">Markette CSP deneyimi hakkında daha fazla bilgi için Ticari markete [genel bakış makalelerini okuyun.](csp-commercial-marketplace-overview.md)</span><span class="sxs-lookup"><span data-stu-id="f2990-159">For more information on the CSP experience in the marketplace, read [Commercial marketplace overview](csp-commercial-marketplace-overview.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="f2990-160">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="f2990-160">Next steps</span></span>

- [<span data-ttu-id="f2990-161">Ticari market tekliflerini satın alma</span><span class="sxs-lookup"><span data-stu-id="f2990-161">Purchase commercial marketplace offers</span></span>](csp-commercial-marketplace-purchase.md)