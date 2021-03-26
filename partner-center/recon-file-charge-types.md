---
title: Mutabakat dosya ücreti türleri
ms.topic: article
ms.date: 06/05/2020
description: Iş Ortağı Merkezi mutabakatı dosyalarındaki ücret türlerini (örneğin, lisans tabanlı, kullanım tabanlı ve tek seferlik), kredilerin ve indirimlerle bulun.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ba42ac5beb28a3cf819c54a86385fb79853cdcd0
ms.sourcegitcommit: 700150044ea4f1a0b96cb4caeb97d7197da29ef6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/25/2021
ms.locfileid: "105549235"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="8ef14-103">Iş Ortağı Merkezi mutabakatı dosyalarındaki farklı ücret türlerini anlayın</span><span class="sxs-lookup"><span data-stu-id="8ef14-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="8ef14-104">**Şunlara uygulanır**</span><span class="sxs-lookup"><span data-stu-id="8ef14-104">**Applies to**</span></span>

- <span data-ttu-id="8ef14-105">Microsoft kamu bulutu için iş ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="8ef14-105">Partner Center for Microsoft Government cloud</span></span>

<span data-ttu-id="8ef14-106">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="8ef14-106">**Appropriate roles**</span></span>

- <span data-ttu-id="8ef14-107">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="8ef14-107">Admin agent</span></span>
- <span data-ttu-id="8ef14-108">Faturalama yöneticisi</span><span class="sxs-lookup"><span data-stu-id="8ef14-108">Billing admin</span></span>
- <span data-ttu-id="8ef14-109">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="8ef14-109">Global admin</span></span>

<span data-ttu-id="8ef14-110">Bu makalede, bir fatura bölümü ve mutabakat dosyanızda olabilecek ilişkili ücret türleri arasındaki eşlemeler açıklanır.</span><span class="sxs-lookup"><span data-stu-id="8ef14-110">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="8ef14-111">Faturanızda ücretler özeti sağlanmaktadır.</span><span class="sxs-lookup"><span data-stu-id="8ef14-111">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="8ef14-112">Mutabakat dosyanız, ücret türleri dahil olmak üzere satır öğesi işlemlerinin ayrıntılı bir dökümünü sağlar.</span><span class="sxs-lookup"><span data-stu-id="8ef14-112">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="8ef14-113">Karşılaştırma dosyaları hakkında daha fazla bilgi için bkz. [karşılaştırma dosyalarını kullanma](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="8ef14-113">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="8ef14-114">Hem [Kullanım tabanlı](usage-based-recon-files.md) hem de [Lisans tabanlı mutabakat dosyaları](license-based-recon-files.md) yalnızca kullanımla ilgili işlemler ve ücretler (tüketilen birimler ve ilgili ücretler) gösterir.</span><span class="sxs-lookup"><span data-stu-id="8ef14-114">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="8ef14-115">Tek kapalı krediler, faturada görüntülenen iskontolar veya para iadesi, mutabakat dosyasında  gösterilmez.</span><span class="sxs-lookup"><span data-stu-id="8ef14-115">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="8ef14-116">Ücret türlerini fatura ücretlerine eşleyin</span><span class="sxs-lookup"><span data-stu-id="8ef14-116">Map charge types to invoice charges</span></span>

<span data-ttu-id="8ef14-117">Fatura ve mutabakat dosyanız arasında çapraz başvuru ücret miktarları için, Microsoft Excel 'deki filtre seçeneklerini kullanın.</span><span class="sxs-lookup"><span data-stu-id="8ef14-117">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="8ef14-118">Mutabakat dosyasındaki ücretlendirme türlerine göre filtreleme yaparak fatura ücretlerini mutabakat dosyasındaki bir dizi ücret dökümü ile eşleyin.</span><span class="sxs-lookup"><span data-stu-id="8ef14-118">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="8ef14-119">Lisans tabanlı ücretler</span><span class="sxs-lookup"><span data-stu-id="8ef14-119">License-based charges</span></span>

<span data-ttu-id="8ef14-120">Bu lisans tabanlı ücretleri faturanızda eşlemek için, lisans tabanlı dosyadaki **tutar** sütununu toplayın.</span><span class="sxs-lookup"><span data-stu-id="8ef14-120">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="8ef14-121">Ücretlendirme açıklaması (mutabakat dosyasındaki ChargeType sütunu)</span><span class="sxs-lookup"><span data-stu-id="8ef14-121">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="8ef14-122">Ücret açıklaması</span><span class="sxs-lookup"><span data-stu-id="8ef14-122">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="8ef14-123">Etkinleştirme ücreti</span><span class="sxs-lookup"><span data-stu-id="8ef14-123">Activation fee</span></span> | <span data-ttu-id="8ef14-124">Satın alma işleminden sonra aboneliği kullandıklarında müşteriye ücretlendirilen miktar.</span><span class="sxs-lookup"><span data-stu-id="8ef14-124">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="8ef14-125">Ücreti iptal et</span><span class="sxs-lookup"><span data-stu-id="8ef14-125">Cancel fee</span></span> | <span data-ttu-id="8ef14-126">İlişkili lisanslar değiştirildiğinde müşteriye eşit olarak dağıtılmış ücretler müşteriye iade edildi.</span><span class="sxs-lookup"><span data-stu-id="8ef14-126">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="8ef14-127">Örnek eşit olarak iptal et</span><span class="sxs-lookup"><span data-stu-id="8ef14-127">Cancel instance prorate</span></span> | <span data-ttu-id="8ef14-128">Aylık aboneliğe sahip müşteri, abonelik askıya alındı ve ilişkili lisanslar aynı ay içinde değiştiği zaman eşit olarak dağıtılmış ücretler iptal edilir.</span><span class="sxs-lookup"><span data-stu-id="8ef14-128">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="8ef14-129">Bisiklet ücreti</span><span class="sxs-lookup"><span data-stu-id="8ef14-129">Cycle fee</span></span> | <span data-ttu-id="8ef14-130">Bir abonelik için dönemsel ücretler.</span><span class="sxs-lookup"><span data-stu-id="8ef14-130">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="8ef14-131">Bisiklet örneği eşit</span><span class="sxs-lookup"><span data-stu-id="8ef14-131">Cycle instance prorate</span></span> | <span data-ttu-id="8ef14-132">İlişkili lisanslar değiştirildiğinde müşteriden alınan eşit oranda dağıtılmış ücretler.</span><span class="sxs-lookup"><span data-stu-id="8ef14-132">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="8ef14-133">İptal edildiğinde eşit ücret ücretleri</span><span class="sxs-lookup"><span data-stu-id="8ef14-133">Prorate fees when cancel</span></span> | <span data-ttu-id="8ef14-134">İptal sonrasında hizmetin kullanılmayan bölümü için eşit olarak dağıtılmış para iadesi.</span><span class="sxs-lookup"><span data-stu-id="8ef14-134">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="8ef14-135">Geçerli sunumdan uzakta değişiklik yaparken eşit ücretler</span><span class="sxs-lookup"><span data-stu-id="8ef14-135">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="8ef14-136">Geçerli aylık abonelikten bir yıllık aboneliğe dönüştürmeden sonra eşit olarak dağıtılmış ücretler.</span><span class="sxs-lookup"><span data-stu-id="8ef14-136">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="8ef14-137">Yeni bir teklife dönüştürülürken eşit ücretler ücretleri</span><span class="sxs-lookup"><span data-stu-id="8ef14-137">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="8ef14-138">Aylık bir aboneliği yeni bir yıllık aboneliğe dönüştürdükten sonra eşit olarak dağıtılmış ücretler.</span><span class="sxs-lookup"><span data-stu-id="8ef14-138">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="8ef14-139">Satın alma sırasında ücretleri eşit oranda artır</span><span class="sxs-lookup"><span data-stu-id="8ef14-139">Prorate fees when purchase</span></span> | <span data-ttu-id="8ef14-140">Aylık veya yıllık faturalandırma kullanılırken bir abonelik için ücret türü.</span><span class="sxs-lookup"><span data-stu-id="8ef14-140">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="8ef14-141">Yenileme sırasında eşit ücret ücreti</span><span class="sxs-lookup"><span data-stu-id="8ef14-141">Prorate fee when renew</span></span> | <span data-ttu-id="8ef14-142">Abonelik yenileme sonrasında eşit olarak dağıtılmış ücretler.</span><span class="sxs-lookup"><span data-stu-id="8ef14-142">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="8ef14-143">Ücretleri Yenile</span><span class="sxs-lookup"><span data-stu-id="8ef14-143">Renew fee</span></span> | <span data-ttu-id="8ef14-144">Abonelik yenileme ücreti</span><span class="sxs-lookup"><span data-stu-id="8ef14-144">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="8ef14-145">Etkinleştirmede eşit ücretler</span><span class="sxs-lookup"><span data-stu-id="8ef14-145">Prorate fees when activate</span></span> | <span data-ttu-id="8ef14-146">Faturalandırma döneminin sonuna kadar etkinleştirilmesinin eşit olarak dağıtılmış ücretleri.</span><span class="sxs-lookup"><span data-stu-id="8ef14-146">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="8ef14-147">Tek seferlik ücretler</span><span class="sxs-lookup"><span data-stu-id="8ef14-147">One-time charges</span></span>

<span data-ttu-id="8ef14-148">Bu tek seferlik ücretleri faturanızda eşlemek için, **tutar** sütununu lisans tabanlı dosyadan toplayın.</span><span class="sxs-lookup"><span data-stu-id="8ef14-148">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="8ef14-149">Ücretlendirme açıklaması (mutabakat dosyasındaki ChargeType sütunu)</span><span class="sxs-lookup"><span data-stu-id="8ef14-149">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="8ef14-150">Ücret açıklaması</span><span class="sxs-lookup"><span data-stu-id="8ef14-150">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="8ef14-151">Yeni</span><span class="sxs-lookup"><span data-stu-id="8ef14-151">New</span></span> | <span data-ttu-id="8ef14-152">Yeni bir satın alma oluşturulduğunda kullanılır.</span><span class="sxs-lookup"><span data-stu-id="8ef14-152">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="8ef14-153">addQuantity</span><span class="sxs-lookup"><span data-stu-id="8ef14-153">addQuantity</span></span> | <span data-ttu-id="8ef14-154">Hem orijinal satınalmanın para iadesi hem de bir artmadan sonraki yeni miktarın kullanıldığı.</span><span class="sxs-lookup"><span data-stu-id="8ef14-154">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="8ef14-155">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="8ef14-155">removeQuantity</span></span> | <span data-ttu-id="8ef14-156">Orijinal satınalmanın para iadesi ve yeni miktarın bir azalmadan sonraki aşamasında kullanılır.</span><span class="sxs-lookup"><span data-stu-id="8ef14-156">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="8ef14-157">İptal</span><span class="sxs-lookup"><span data-stu-id="8ef14-157">Cancel</span></span> | <span data-ttu-id="8ef14-158">Abonelik iptal edildiğinde kullanılır.</span><span class="sxs-lookup"><span data-stu-id="8ef14-158">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="8ef14-159">Dönüştür</span><span class="sxs-lookup"><span data-stu-id="8ef14-159">Convert</span></span> | <span data-ttu-id="8ef14-160">Bir lisans yükseltildiğinde, ancak lisansların sayısı değişmeden kaldığı zaman kullanılır.</span><span class="sxs-lookup"><span data-stu-id="8ef14-160">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="8ef14-161">Kullanım ücretleri</span><span class="sxs-lookup"><span data-stu-id="8ef14-161">Usage charges</span></span>

<span data-ttu-id="8ef14-162">Bu kullanım ücretlerini faturanızda eşlemek için, kullanım tabanlı dosyadaki **Pretaxcharges** sütununu toplayın.</span><span class="sxs-lookup"><span data-stu-id="8ef14-162">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="8ef14-163">Ücretlendirme açıklaması (mutabakat dosyasındaki ChargeType sütunu)</span><span class="sxs-lookup"><span data-stu-id="8ef14-163">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="8ef14-164">Ücret açıklaması</span><span class="sxs-lookup"><span data-stu-id="8ef14-164">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="8ef14-165">İptal edildiğinde kullanım ücretini değerlendir</span><span class="sxs-lookup"><span data-stu-id="8ef14-165">Assess usage fee when cancel</span></span> | <span data-ttu-id="8ef14-166">Geçerli fatura döneminde ücretsiz kullanım için İptalden sonra kullanım ücretini erişin.</span><span class="sxs-lookup"><span data-stu-id="8ef14-166">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="8ef14-167">Geçerli döngüyle ilgili kullanım ücretini değerlendir</span><span class="sxs-lookup"><span data-stu-id="8ef14-167">Assess usage fee for current cycle</span></span> | <span data-ttu-id="8ef14-168">Geçerli fatura dönemi için kullanım ücretine erişin.</span><span class="sxs-lookup"><span data-stu-id="8ef14-168">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="8ef14-169">Krediler</span><span class="sxs-lookup"><span data-stu-id="8ef14-169">Credits</span></span>

<span data-ttu-id="8ef14-170">Bu kredileri faturanızda eşlemek için:</span><span class="sxs-lookup"><span data-stu-id="8ef14-170">To map these credits to your invoice:</span></span>

- <span data-ttu-id="8ef14-171">Lisans tabanlı dosyadan **Totalforcustomer** toplamını toplayın.</span><span class="sxs-lookup"><span data-stu-id="8ef14-171">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="8ef14-172">Kullanım tabanlı dosyadaki **Posttaxtotal** sütununu toplayın.</span><span class="sxs-lookup"><span data-stu-id="8ef14-172">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="8ef14-173">Ücretlendirme açıklaması (mutabakat dosyasındaki ChargeType sütunu)</span><span class="sxs-lookup"><span data-stu-id="8ef14-173">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="8ef14-174">Ücret açıklaması</span><span class="sxs-lookup"><span data-stu-id="8ef14-174">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="8ef14-175">Bir satır öğesinin sapmasını</span><span class="sxs-lookup"><span data-stu-id="8ef14-175">Offset a line item</span></span> | <span data-ttu-id="8ef14-176">Vergiler dahil olmak üzere bir satır öğesine kısmi veya tam para iadesi.</span><span class="sxs-lookup"><span data-stu-id="8ef14-176">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="8ef14-177">Kullanım tabanlı indirimler</span><span class="sxs-lookup"><span data-stu-id="8ef14-177">Usage-based discounts</span></span>

<span data-ttu-id="8ef14-178">Bu kullanım tabanlı indirimleri faturanızda eşlemek için, kullanım tabanlı dosyadaki **Pretaxcharges** sütununu toplayın.</span><span class="sxs-lookup"><span data-stu-id="8ef14-178">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="8ef14-179">Ücretlendirme açıklaması (mutabakat dosyasındaki ChargeType sütunu)</span><span class="sxs-lookup"><span data-stu-id="8ef14-179">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="8ef14-180">Ücret açıklaması</span><span class="sxs-lookup"><span data-stu-id="8ef14-180">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="8ef14-181">Etkinleştirme indirimi</span><span class="sxs-lookup"><span data-stu-id="8ef14-181">Activation discount</span></span> | <span data-ttu-id="8ef14-182">Abonelik etkinleştirildiğinde uygulanan indirim.</span><span class="sxs-lookup"><span data-stu-id="8ef14-182">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="8ef14-183">Devir indirimi</span><span class="sxs-lookup"><span data-stu-id="8ef14-183">Cycle discount</span></span> | <span data-ttu-id="8ef14-184">Düzenli ücretlere uygulanan indirim.</span><span class="sxs-lookup"><span data-stu-id="8ef14-184">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="8ef14-185">İndirimi Yenile</span><span class="sxs-lookup"><span data-stu-id="8ef14-185">Renew discount</span></span> | <span data-ttu-id="8ef14-186">Abonelik yenilendiğinde uygulanan indirim.</span><span class="sxs-lookup"><span data-stu-id="8ef14-186">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="8ef14-187">İndirimi iptal et</span><span class="sxs-lookup"><span data-stu-id="8ef14-187">Cancel discount</span></span> | <span data-ttu-id="8ef14-188">İndirimler iptal edildiğinde uygulanan ücretler.</span><span class="sxs-lookup"><span data-stu-id="8ef14-188">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="8ef14-189">Lisans tabanlı indirimler</span><span class="sxs-lookup"><span data-stu-id="8ef14-189">License-based discounts</span></span>

<span data-ttu-id="8ef14-190">Lisans tabanlı indirimleri faturanızda eşlemek için, **TotalOtherDiscount** sütununu lisans tabanlı dosyadan toplayın.</span><span class="sxs-lookup"><span data-stu-id="8ef14-190">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="8ef14-191">*Lisans tabanlı indirimler, birden çok ücret türüne uygulanabilir.*</span><span class="sxs-lookup"><span data-stu-id="8ef14-191">*License-based discounts may be applied to multiple charge types.*</span></span>
