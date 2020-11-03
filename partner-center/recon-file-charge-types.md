---
title: Mutabakatı dosya ücreti türleri
ms.topic: article
ms.date: 06/05/2020
description: Iş Ortağı Merkezi mutabakatı dosyalarındaki ücret türlerini (örneğin, lisans tabanlı, kullanım tabanlı ve tek seferlik), kredilerin ve indirimlerle bulun.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f65c4a6496082934e8c38fbd924b96ef969be95b
ms.sourcegitcommit: e7931fbe7ce16a62124e00b2802520a17d7285b8
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/31/2020
ms.locfileid: "92531115"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="b25a7-103">Iş Ortağı Merkezi mutabakatı dosyalarındaki farklı ücret türlerini anlayın</span><span class="sxs-lookup"><span data-stu-id="b25a7-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="b25a7-104">**Uygulama hedefi**</span><span class="sxs-lookup"><span data-stu-id="b25a7-104">**Applies to**</span></span>

- <span data-ttu-id="b25a7-105">İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="b25a7-105">Partner Center</span></span>
- <span data-ttu-id="b25a7-106">ABD kamu için Microsoft Bulut iş ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="b25a7-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="b25a7-107">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="b25a7-107">**Appropriate roles**</span></span>

- <span data-ttu-id="b25a7-108">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="b25a7-108">Admin agent</span></span>
- <span data-ttu-id="b25a7-109">Faturalama yöneticisi</span><span class="sxs-lookup"><span data-stu-id="b25a7-109">Billing admin</span></span>
- <span data-ttu-id="b25a7-110">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="b25a7-110">Global admin</span></span>

<span data-ttu-id="b25a7-111">Bu konuda, bir fatura bölümü ve mutabakat dosyanızda olabilecek ilişkili ücret türleri arasındaki eşlemeler açıklanmaktadır.</span><span class="sxs-lookup"><span data-stu-id="b25a7-111">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="b25a7-112">Faturanızda ücretler özeti sağlanmaktadır.</span><span class="sxs-lookup"><span data-stu-id="b25a7-112">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="b25a7-113">Mutabakat dosyanız, ücret türleri dahil olmak üzere satır öğesi işlemlerinin ayrıntılı bir dökümünü sağlar.</span><span class="sxs-lookup"><span data-stu-id="b25a7-113">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="b25a7-114">Karşılaştırma dosyaları hakkında daha fazla bilgi için bkz. [karşılaştırma dosyalarını kullanma](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="b25a7-114">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="b25a7-115">Hem [Kullanım tabanlı](usage-based-recon-files.md) hem de [Lisans tabanlı mutabakat dosyaları](license-based-recon-files.md) yalnızca kullanımla ilgili işlemler ve ücretler (tüketilen birimler ve ilgili ücretler) gösterir.</span><span class="sxs-lookup"><span data-stu-id="b25a7-115">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="b25a7-116">Tek kapalı krediler, faturada görüntülenen iskontolar veya para iadesi, mutabakat dosyasında **Adjustments** gösterilmez.</span><span class="sxs-lookup"><span data-stu-id="b25a7-116">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="b25a7-117">Ücret türlerini fatura ücretlerine eşleyin</span><span class="sxs-lookup"><span data-stu-id="b25a7-117">Map charge types to invoice charges</span></span>

<span data-ttu-id="b25a7-118">Fatura ve mutabakat dosyanız arasında çapraz başvuru ücret miktarları için, Microsoft Excel 'deki filtre seçeneklerini kullanın.</span><span class="sxs-lookup"><span data-stu-id="b25a7-118">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="b25a7-119">Mutabakat dosyasındaki ücretlendirme türlerine göre filtreleme yaparak fatura ücretlerini mutabakat dosyasındaki bir dizi ücret dökümü ile eşleyin.</span><span class="sxs-lookup"><span data-stu-id="b25a7-119">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="b25a7-120">Lisans tabanlı ücretler</span><span class="sxs-lookup"><span data-stu-id="b25a7-120">License-based charges</span></span>

<span data-ttu-id="b25a7-121">Bu lisans tabanlı ücretleri faturanızda eşlemek için, lisans tabanlı dosyadaki **tutar** sütununu toplayın.</span><span class="sxs-lookup"><span data-stu-id="b25a7-121">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="b25a7-122">Ücretlendirme açıklaması (mutabakat dosyasındaki ChargeType sütunu)</span><span class="sxs-lookup"><span data-stu-id="b25a7-122">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="b25a7-123">Ücret açıklaması</span><span class="sxs-lookup"><span data-stu-id="b25a7-123">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="b25a7-124">Etkinleştirme ücreti</span><span class="sxs-lookup"><span data-stu-id="b25a7-124">Activation fee</span></span> | <span data-ttu-id="b25a7-125">Satın alma işleminden sonra aboneliği kullandıklarında müşteriye ücretlendirilen miktar.</span><span class="sxs-lookup"><span data-stu-id="b25a7-125">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="b25a7-126">Ücreti iptal et</span><span class="sxs-lookup"><span data-stu-id="b25a7-126">Cancel fee</span></span> | <span data-ttu-id="b25a7-127">İlişkili lisanslar değiştirildiğinde müşteriye eşit olarak dağıtılmış ücretler müşteriye iade edildi.</span><span class="sxs-lookup"><span data-stu-id="b25a7-127">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="b25a7-128">Örnek eşit olarak iptal et</span><span class="sxs-lookup"><span data-stu-id="b25a7-128">Cancel instance prorate</span></span> | <span data-ttu-id="b25a7-129">Aylık aboneliğe sahip müşteri, abonelik askıya alındı ve ilişkili lisanslar aynı ay içinde değiştiği zaman eşit olarak dağıtılmış ücretler iptal edilir.</span><span class="sxs-lookup"><span data-stu-id="b25a7-129">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="b25a7-130">Bisiklet ücreti</span><span class="sxs-lookup"><span data-stu-id="b25a7-130">Cycle fee</span></span> | <span data-ttu-id="b25a7-131">Bir abonelik için dönemsel ücretler.</span><span class="sxs-lookup"><span data-stu-id="b25a7-131">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="b25a7-132">Bisiklet örneği eşit</span><span class="sxs-lookup"><span data-stu-id="b25a7-132">Cycle instance prorate</span></span> | <span data-ttu-id="b25a7-133">İlişkili lisanslar değiştirildiğinde müşteriden alınan eşit oranda dağıtılmış ücretler.</span><span class="sxs-lookup"><span data-stu-id="b25a7-133">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="b25a7-134">İptal edildiğinde eşit ücret ücretleri</span><span class="sxs-lookup"><span data-stu-id="b25a7-134">Prorate fees when cancel</span></span> | <span data-ttu-id="b25a7-135">İptal sonrasında hizmetin kullanılmayan bölümü için eşit olarak dağıtılmış para iadesi.</span><span class="sxs-lookup"><span data-stu-id="b25a7-135">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="b25a7-136">Geçerli sunumdan uzakta değişiklik yaparken eşit ücretler</span><span class="sxs-lookup"><span data-stu-id="b25a7-136">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="b25a7-137">Geçerli aylık abonelikten bir yıllık aboneliğe dönüştürmeden sonra eşit olarak dağıtılmış ücretler.</span><span class="sxs-lookup"><span data-stu-id="b25a7-137">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="b25a7-138">Yeni bir teklife dönüştürülürken eşit ücretler ücretleri</span><span class="sxs-lookup"><span data-stu-id="b25a7-138">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="b25a7-139">Aylık bir aboneliği yeni bir yıllık aboneliğe dönüştürdükten sonra eşit olarak dağıtılmış ücretler.</span><span class="sxs-lookup"><span data-stu-id="b25a7-139">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="b25a7-140">Satın alma sırasında ücretleri eşit oranda artır</span><span class="sxs-lookup"><span data-stu-id="b25a7-140">Prorate fees when purchase</span></span> | <span data-ttu-id="b25a7-141">Aylık veya yıllık faturalandırma kullanılırken bir abonelik için ücret türü.</span><span class="sxs-lookup"><span data-stu-id="b25a7-141">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="b25a7-142">Yenileme sırasında eşit ücret ücreti</span><span class="sxs-lookup"><span data-stu-id="b25a7-142">Prorate fee when renew</span></span> | <span data-ttu-id="b25a7-143">Abonelik yenileme sonrasında eşit olarak dağıtılmış ücretler.</span><span class="sxs-lookup"><span data-stu-id="b25a7-143">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="b25a7-144">Ücretleri Yenile</span><span class="sxs-lookup"><span data-stu-id="b25a7-144">Renew fee</span></span> | <span data-ttu-id="b25a7-145">Abonelik yenileme ücreti</span><span class="sxs-lookup"><span data-stu-id="b25a7-145">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="b25a7-146">Etkinleştirmede eşit ücretler</span><span class="sxs-lookup"><span data-stu-id="b25a7-146">Prorate fees when activate</span></span> | <span data-ttu-id="b25a7-147">Faturalandırma döneminin sonuna kadar etkinleştirilmesinin eşit olarak dağıtılmış ücretleri.</span><span class="sxs-lookup"><span data-stu-id="b25a7-147">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="b25a7-148">Tek seferlik ücretler</span><span class="sxs-lookup"><span data-stu-id="b25a7-148">One-time charges</span></span>

<span data-ttu-id="b25a7-149">Bu tek seferlik ücretleri faturanızda eşlemek için, **tutar** sütununu lisans tabanlı dosyadan toplayın.</span><span class="sxs-lookup"><span data-stu-id="b25a7-149">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="b25a7-150">Ücretlendirme açıklaması (mutabakat dosyasındaki ChargeType sütunu)</span><span class="sxs-lookup"><span data-stu-id="b25a7-150">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="b25a7-151">Ücret açıklaması</span><span class="sxs-lookup"><span data-stu-id="b25a7-151">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="b25a7-152">Yeni</span><span class="sxs-lookup"><span data-stu-id="b25a7-152">New</span></span> | <span data-ttu-id="b25a7-153">Yeni bir satın alma oluşturulduğunda kullanılır.</span><span class="sxs-lookup"><span data-stu-id="b25a7-153">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="b25a7-154">addQuantity</span><span class="sxs-lookup"><span data-stu-id="b25a7-154">addQuantity</span></span> | <span data-ttu-id="b25a7-155">Hem orijinal satınalmanın para iadesi hem de bir artmadan sonraki yeni miktarın kullanıldığı.</span><span class="sxs-lookup"><span data-stu-id="b25a7-155">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="b25a7-156">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="b25a7-156">removeQuantity</span></span> | <span data-ttu-id="b25a7-157">Orijinal satınalmanın para iadesi ve yeni miktarın bir azalmadan sonraki aşamasında kullanılır.</span><span class="sxs-lookup"><span data-stu-id="b25a7-157">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="b25a7-158">İptal</span><span class="sxs-lookup"><span data-stu-id="b25a7-158">Cancel</span></span> | <span data-ttu-id="b25a7-159">Abonelik iptal edildiğinde kullanılır.</span><span class="sxs-lookup"><span data-stu-id="b25a7-159">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="b25a7-160">Dönüştür</span><span class="sxs-lookup"><span data-stu-id="b25a7-160">Convert</span></span> | <span data-ttu-id="b25a7-161">Bir lisans yükseltildiğinde, ancak lisansların sayısı değişmeden kaldığı zaman kullanılır.</span><span class="sxs-lookup"><span data-stu-id="b25a7-161">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="b25a7-162">Kullanım ücretleri</span><span class="sxs-lookup"><span data-stu-id="b25a7-162">Usage charges</span></span>

<span data-ttu-id="b25a7-163">Bu kullanım ücretlerini faturanızda eşlemek için, kullanım tabanlı dosyadaki **Pretaxcharges** sütununu toplayın.</span><span class="sxs-lookup"><span data-stu-id="b25a7-163">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="b25a7-164">Ücretlendirme açıklaması (mutabakat dosyasındaki ChargeType sütunu)</span><span class="sxs-lookup"><span data-stu-id="b25a7-164">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="b25a7-165">Ücret açıklaması</span><span class="sxs-lookup"><span data-stu-id="b25a7-165">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="b25a7-166">İptal edildiğinde kullanım ücretini değerlendir</span><span class="sxs-lookup"><span data-stu-id="b25a7-166">Assess usage fee when cancel</span></span> | <span data-ttu-id="b25a7-167">Geçerli fatura döneminde ücretsiz kullanım için İptalden sonra kullanım ücretini erişin.</span><span class="sxs-lookup"><span data-stu-id="b25a7-167">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="b25a7-168">Geçerli döngüyle ilgili kullanım ücretini değerlendir</span><span class="sxs-lookup"><span data-stu-id="b25a7-168">Assess usage fee for current cycle</span></span> | <span data-ttu-id="b25a7-169">Geçerli fatura dönemi için kullanım ücretine erişin.</span><span class="sxs-lookup"><span data-stu-id="b25a7-169">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="b25a7-170">Krediler</span><span class="sxs-lookup"><span data-stu-id="b25a7-170">Credits</span></span>

<span data-ttu-id="b25a7-171">Bu kredileri faturanızda eşlemek için:</span><span class="sxs-lookup"><span data-stu-id="b25a7-171">To map these credits to your invoice:</span></span>

- <span data-ttu-id="b25a7-172">Lisans tabanlı dosyadan **Totalforcustomer** toplamını toplayın.</span><span class="sxs-lookup"><span data-stu-id="b25a7-172">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="b25a7-173">Kullanım tabanlı dosyadaki **Posttaxtotal** sütununu toplayın.</span><span class="sxs-lookup"><span data-stu-id="b25a7-173">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="b25a7-174">Ücretlendirme açıklaması (mutabakat dosyasındaki ChargeType sütunu)</span><span class="sxs-lookup"><span data-stu-id="b25a7-174">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="b25a7-175">Ücret açıklaması</span><span class="sxs-lookup"><span data-stu-id="b25a7-175">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="b25a7-176">Bir satır öğesinin sapmasını</span><span class="sxs-lookup"><span data-stu-id="b25a7-176">Offset a line item</span></span> | <span data-ttu-id="b25a7-177">Vergiler dahil olmak üzere bir satır öğesine kısmi veya tam para iadesi.</span><span class="sxs-lookup"><span data-stu-id="b25a7-177">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="b25a7-178">Kullanım tabanlı indirimler</span><span class="sxs-lookup"><span data-stu-id="b25a7-178">Usage-based discounts</span></span>

<span data-ttu-id="b25a7-179">Bu kullanım tabanlı indirimleri faturanızda eşlemek için, kullanım tabanlı dosyadaki **Pretaxcharges** sütununu toplayın.</span><span class="sxs-lookup"><span data-stu-id="b25a7-179">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="b25a7-180">Ücretlendirme açıklaması (mutabakat dosyasındaki ChargeType sütunu)</span><span class="sxs-lookup"><span data-stu-id="b25a7-180">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="b25a7-181">Ücret açıklaması</span><span class="sxs-lookup"><span data-stu-id="b25a7-181">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="b25a7-182">Etkinleştirme indirimi</span><span class="sxs-lookup"><span data-stu-id="b25a7-182">Activation discount</span></span> | <span data-ttu-id="b25a7-183">Abonelik etkinleştirildiğinde uygulanan indirim.</span><span class="sxs-lookup"><span data-stu-id="b25a7-183">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="b25a7-184">Devir indirimi</span><span class="sxs-lookup"><span data-stu-id="b25a7-184">Cycle discount</span></span> | <span data-ttu-id="b25a7-185">Düzenli ücretlere uygulanan indirim.</span><span class="sxs-lookup"><span data-stu-id="b25a7-185">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="b25a7-186">İndirimi Yenile</span><span class="sxs-lookup"><span data-stu-id="b25a7-186">Renew discount</span></span> | <span data-ttu-id="b25a7-187">Abonelik yenilendiğinde uygulanan indirim.</span><span class="sxs-lookup"><span data-stu-id="b25a7-187">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="b25a7-188">İndirimi iptal et</span><span class="sxs-lookup"><span data-stu-id="b25a7-188">Cancel discount</span></span> | <span data-ttu-id="b25a7-189">İndirimler iptal edildiğinde uygulanan ücretler.</span><span class="sxs-lookup"><span data-stu-id="b25a7-189">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="b25a7-190">Lisans tabanlı indirimler</span><span class="sxs-lookup"><span data-stu-id="b25a7-190">License-based discounts</span></span>

<span data-ttu-id="b25a7-191">Lisans tabanlı indirimleri faturanızda eşlemek için, **TotalOtherDiscount** sütununu lisans tabanlı dosyadan toplayın.</span><span class="sxs-lookup"><span data-stu-id="b25a7-191">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="b25a7-192">*Lisans tabanlı indirimler, birden çok ücret türüne uygulanabilir.*</span><span class="sxs-lookup"><span data-stu-id="b25a7-192">*License-based discounts may be applied to multiple charge types.*</span></span>
