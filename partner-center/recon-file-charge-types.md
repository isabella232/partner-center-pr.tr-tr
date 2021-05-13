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
ms.openlocfilehash: 5a1f45de59fc9dac6a443bb8a14c3a80b36ba3f7
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855888"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="3f21e-103">Iş Ortağı Merkezi mutabakatı dosyalarındaki farklı ücret türlerini anlayın</span><span class="sxs-lookup"><span data-stu-id="3f21e-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="3f21e-104">**Uygulama hedefi**: Iş Ortağı Merkezi | ABD kamu için Microsoft Bulut iş ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="3f21e-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="3f21e-105">**Uygun roller**: yönetici Aracısı | Faturalandırma Yöneticisi | Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="3f21e-105">**Appropriate roles**: Admin agent | Billing admin | Global admin</span></span>

<span data-ttu-id="3f21e-106">Bu makalede, bir fatura bölümü ve mutabakat dosyanızda olabilecek ilişkili ücret türleri arasındaki eşlemeler açıklanır.</span><span class="sxs-lookup"><span data-stu-id="3f21e-106">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="3f21e-107">Faturanızda ücretler özeti sağlanmaktadır.</span><span class="sxs-lookup"><span data-stu-id="3f21e-107">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="3f21e-108">Mutabakat dosyanız, ücret türleri dahil olmak üzere satır öğesi işlemlerinin ayrıntılı bir dökümünü sağlar.</span><span class="sxs-lookup"><span data-stu-id="3f21e-108">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="3f21e-109">Karşılaştırma dosyaları hakkında daha fazla bilgi için bkz. [karşılaştırma dosyalarını kullanma](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="3f21e-109">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="3f21e-110">Hem [Kullanım tabanlı](usage-based-recon-files.md) hem de [Lisans tabanlı mutabakat dosyaları](license-based-recon-files.md) yalnızca kullanımla ilgili işlemler ve ücretler (tüketilen birimler ve ilgili ücretler) gösterir.</span><span class="sxs-lookup"><span data-stu-id="3f21e-110">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="3f21e-111">Tek kapalı krediler, faturada görüntülenen iskontolar veya para iadesi, mutabakat dosyasında  gösterilmez.</span><span class="sxs-lookup"><span data-stu-id="3f21e-111">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="3f21e-112">Ücret türlerini fatura ücretlerine eşleyin</span><span class="sxs-lookup"><span data-stu-id="3f21e-112">Map charge types to invoice charges</span></span>

<span data-ttu-id="3f21e-113">Fatura ve mutabakat dosyanız arasında çapraz başvuru ücret miktarları için, Microsoft Excel 'deki filtre seçeneklerini kullanın.</span><span class="sxs-lookup"><span data-stu-id="3f21e-113">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="3f21e-114">Mutabakat dosyasındaki ücretlendirme türlerine göre filtreleme yaparak fatura ücretlerini mutabakat dosyasındaki bir dizi ücret dökümü ile eşleyin.</span><span class="sxs-lookup"><span data-stu-id="3f21e-114">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="3f21e-115">Lisans tabanlı ücretler</span><span class="sxs-lookup"><span data-stu-id="3f21e-115">License-based charges</span></span>

<span data-ttu-id="3f21e-116">Bu lisans tabanlı ücretleri faturanızda eşlemek için, lisans tabanlı dosyadaki **tutar** sütununu toplayın.</span><span class="sxs-lookup"><span data-stu-id="3f21e-116">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="3f21e-117">Ücretlendirme açıklaması (mutabakat dosyasındaki ChargeType sütunu)</span><span class="sxs-lookup"><span data-stu-id="3f21e-117">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="3f21e-118">Ücret açıklaması</span><span class="sxs-lookup"><span data-stu-id="3f21e-118">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="3f21e-119">Etkinleştirme ücreti</span><span class="sxs-lookup"><span data-stu-id="3f21e-119">Activation fee</span></span> | <span data-ttu-id="3f21e-120">Satın alma işleminden sonra aboneliği kullandıklarında müşteriye ücretlendirilen miktar.</span><span class="sxs-lookup"><span data-stu-id="3f21e-120">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="3f21e-121">Ücreti iptal et</span><span class="sxs-lookup"><span data-stu-id="3f21e-121">Cancel fee</span></span> | <span data-ttu-id="3f21e-122">İlişkili lisanslar değiştiriken müşteriye iade edilecek, proratlı ücretler.</span><span class="sxs-lookup"><span data-stu-id="3f21e-122">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="3f21e-123">Örnek prorate işlemini iptal etme</span><span class="sxs-lookup"><span data-stu-id="3f21e-123">Cancel instance prorate</span></span> | <span data-ttu-id="3f21e-124">Aylık aboneliği olan müşterinin aboneliği askıya alındı ve ilişkili lisanslar aynı ay içinde değişti.</span><span class="sxs-lookup"><span data-stu-id="3f21e-124">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="3f21e-125">Döngü ücreti</span><span class="sxs-lookup"><span data-stu-id="3f21e-125">Cycle fee</span></span> | <span data-ttu-id="3f21e-126">Bir abonelik için düzenli ücretler.</span><span class="sxs-lookup"><span data-stu-id="3f21e-126">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="3f21e-127">Döngü örneği hızı</span><span class="sxs-lookup"><span data-stu-id="3f21e-127">Cycle instance prorate</span></span> | <span data-ttu-id="3f21e-128">İlişkili lisanslar değiştiriken müşteri tarafından değerlendirilen, proratılmış ücretler.</span><span class="sxs-lookup"><span data-stu-id="3f21e-128">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="3f21e-129">İptal edilirken ücretlerin prorate işlemi</span><span class="sxs-lookup"><span data-stu-id="3f21e-129">Prorate fees when cancel</span></span> | <span data-ttu-id="3f21e-130">İptalin ardından hizmetin kullanılmayan kısmı için prorated para iadesi.</span><span class="sxs-lookup"><span data-stu-id="3f21e-130">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="3f21e-131">Geçerli tekliften dönüştürülürken ücretlerin prorate (prorate)</span><span class="sxs-lookup"><span data-stu-id="3f21e-131">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="3f21e-132">Geçerli aylık abonelikten yıllık aboneliğe dönüştürüldikten sonra prorated ücretler.</span><span class="sxs-lookup"><span data-stu-id="3f21e-132">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="3f21e-133">Yeni bir teklife dönüştüren ücretlerin prorate (prorate)</span><span class="sxs-lookup"><span data-stu-id="3f21e-133">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="3f21e-134">Aylık abonelik yeni bir yıllık aboneliğe dönüştürüldikten sonra prorated ücretler.</span><span class="sxs-lookup"><span data-stu-id="3f21e-134">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="3f21e-135">Satın almada ücret prorate</span><span class="sxs-lookup"><span data-stu-id="3f21e-135">Prorate fees when purchase</span></span> | <span data-ttu-id="3f21e-136">Aylık veya yıllık faturalama kullanırken aboneliğin ücret türü.</span><span class="sxs-lookup"><span data-stu-id="3f21e-136">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="3f21e-137">Yenilemede prorate ücreti</span><span class="sxs-lookup"><span data-stu-id="3f21e-137">Prorate fee when renew</span></span> | <span data-ttu-id="3f21e-138">Abonelik yenilemesi sırasında prorated ücretler.</span><span class="sxs-lookup"><span data-stu-id="3f21e-138">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="3f21e-139">Ücreti yenileme</span><span class="sxs-lookup"><span data-stu-id="3f21e-139">Renew fee</span></span> | <span data-ttu-id="3f21e-140">Aboneliği yenileme ücreti</span><span class="sxs-lookup"><span data-stu-id="3f21e-140">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="3f21e-141">Etkinleştiren ücretler için prorate (prorate)</span><span class="sxs-lookup"><span data-stu-id="3f21e-141">Prorate fees when activate</span></span> | <span data-ttu-id="3f21e-142">Etkinleştirmeden faturalama döneminin sonuna kadar protratılmış ücretler.</span><span class="sxs-lookup"><span data-stu-id="3f21e-142">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="3f21e-143">Tek seferlik ücretler</span><span class="sxs-lookup"><span data-stu-id="3f21e-143">One-time charges</span></span>

<span data-ttu-id="3f21e-144">Bu tek seferlik ücretleri faturanıza eşlemek için lisans tabanlı **dosyadan** Amount sütununu topla.</span><span class="sxs-lookup"><span data-stu-id="3f21e-144">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="3f21e-145">Ücret açıklaması (mutabakat dosyasında ChargeType sütunu)</span><span class="sxs-lookup"><span data-stu-id="3f21e-145">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="3f21e-146">Ücret açıklaması</span><span class="sxs-lookup"><span data-stu-id="3f21e-146">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="3f21e-147">Yeni</span><span class="sxs-lookup"><span data-stu-id="3f21e-147">New</span></span> | <span data-ttu-id="3f21e-148">Yeni bir satın alma oluşturulduğunda kullanılır.</span><span class="sxs-lookup"><span data-stu-id="3f21e-148">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="3f21e-149">addQuantity</span><span class="sxs-lookup"><span data-stu-id="3f21e-149">addQuantity</span></span> | <span data-ttu-id="3f21e-150">Hem özgün satın alma para iadesi hem de artış sonrasında yeni miktar için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="3f21e-150">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="3f21e-151">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="3f21e-151">removeQuantity</span></span> | <span data-ttu-id="3f21e-152">Hem özgün satın alma para iadesi hem de düşüş sonrasında yeni miktar için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="3f21e-152">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="3f21e-153">İptal</span><span class="sxs-lookup"><span data-stu-id="3f21e-153">Cancel</span></span> | <span data-ttu-id="3f21e-154">Abonelik iptal edilirken kullanılır.</span><span class="sxs-lookup"><span data-stu-id="3f21e-154">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="3f21e-155">Dönüştür</span><span class="sxs-lookup"><span data-stu-id="3f21e-155">Convert</span></span> | <span data-ttu-id="3f21e-156">Bir lisans yükseltilirken, ancak lisans sayısı değişmeden kalır.</span><span class="sxs-lookup"><span data-stu-id="3f21e-156">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="3f21e-157">Kullanım ücretleri</span><span class="sxs-lookup"><span data-stu-id="3f21e-157">Usage charges</span></span>

<span data-ttu-id="3f21e-158">Bu kullanım ücretlerini faturanıza eşlemek için kullanım tabanlı dosyadan **PretaxCharges** sütununu toplamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="3f21e-158">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="3f21e-159">Ücret açıklaması (mutabakat dosyasında ChargeType sütunu)</span><span class="sxs-lookup"><span data-stu-id="3f21e-159">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="3f21e-160">Ücret açıklaması</span><span class="sxs-lookup"><span data-stu-id="3f21e-160">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="3f21e-161">İptal edilirken kullanım ücretini değerlendirme</span><span class="sxs-lookup"><span data-stu-id="3f21e-161">Assess usage fee when cancel</span></span> | <span data-ttu-id="3f21e-162">Geçerli faturalama dönemi boyunca ödenmemiş kullanım iptali sırasında kullanım ücretine erişin.</span><span class="sxs-lookup"><span data-stu-id="3f21e-162">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="3f21e-163">Geçerli döngü için kullanım ücretini değerlendirme</span><span class="sxs-lookup"><span data-stu-id="3f21e-163">Assess usage fee for current cycle</span></span> | <span data-ttu-id="3f21e-164">Geçerli faturalama dönemi için kullanım ücretine erişin.</span><span class="sxs-lookup"><span data-stu-id="3f21e-164">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="3f21e-165">Krediler</span><span class="sxs-lookup"><span data-stu-id="3f21e-165">Credits</span></span>

<span data-ttu-id="3f21e-166">Bu kredileri faturanıza eşlemek için:</span><span class="sxs-lookup"><span data-stu-id="3f21e-166">To map these credits to your invoice:</span></span>

- <span data-ttu-id="3f21e-167">Lisans tabanlı dosyadan **Totalforcustomer** toplamını toplayın.</span><span class="sxs-lookup"><span data-stu-id="3f21e-167">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="3f21e-168">Kullanım tabanlı dosyadaki **Posttaxtotal** sütununu toplayın.</span><span class="sxs-lookup"><span data-stu-id="3f21e-168">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="3f21e-169">Ücretlendirme açıklaması (mutabakat dosyasındaki ChargeType sütunu)</span><span class="sxs-lookup"><span data-stu-id="3f21e-169">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="3f21e-170">Ücret açıklaması</span><span class="sxs-lookup"><span data-stu-id="3f21e-170">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="3f21e-171">Bir satır öğesinin sapmasını</span><span class="sxs-lookup"><span data-stu-id="3f21e-171">Offset a line item</span></span> | <span data-ttu-id="3f21e-172">Vergiler dahil olmak üzere bir satır öğesine kısmi veya tam para iadesi.</span><span class="sxs-lookup"><span data-stu-id="3f21e-172">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="3f21e-173">Kullanım tabanlı indirimler</span><span class="sxs-lookup"><span data-stu-id="3f21e-173">Usage-based discounts</span></span>

<span data-ttu-id="3f21e-174">Bu kullanım tabanlı indirimleri faturanızda eşlemek için, kullanım tabanlı dosyadaki **Pretaxcharges** sütununu toplayın.</span><span class="sxs-lookup"><span data-stu-id="3f21e-174">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="3f21e-175">Ücretlendirme açıklaması (mutabakat dosyasındaki ChargeType sütunu)</span><span class="sxs-lookup"><span data-stu-id="3f21e-175">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="3f21e-176">Ücret açıklaması</span><span class="sxs-lookup"><span data-stu-id="3f21e-176">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="3f21e-177">Etkinleştirme indirimi</span><span class="sxs-lookup"><span data-stu-id="3f21e-177">Activation discount</span></span> | <span data-ttu-id="3f21e-178">Abonelik etkinleştirildiğinde uygulanan indirim.</span><span class="sxs-lookup"><span data-stu-id="3f21e-178">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="3f21e-179">Devir indirimi</span><span class="sxs-lookup"><span data-stu-id="3f21e-179">Cycle discount</span></span> | <span data-ttu-id="3f21e-180">Düzenli ücretlere uygulanan indirim.</span><span class="sxs-lookup"><span data-stu-id="3f21e-180">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="3f21e-181">İndirimi Yenile</span><span class="sxs-lookup"><span data-stu-id="3f21e-181">Renew discount</span></span> | <span data-ttu-id="3f21e-182">Abonelik yenilendiğinde uygulanan indirim.</span><span class="sxs-lookup"><span data-stu-id="3f21e-182">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="3f21e-183">İndirimi iptal et</span><span class="sxs-lookup"><span data-stu-id="3f21e-183">Cancel discount</span></span> | <span data-ttu-id="3f21e-184">İndirimler iptal edildiğinde uygulanan ücretler.</span><span class="sxs-lookup"><span data-stu-id="3f21e-184">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="3f21e-185">Lisans tabanlı indirimler</span><span class="sxs-lookup"><span data-stu-id="3f21e-185">License-based discounts</span></span>

<span data-ttu-id="3f21e-186">Lisans tabanlı indirimleri faturanızda eşlemek için, **TotalOtherDiscount** sütununu lisans tabanlı dosyadan toplayın.</span><span class="sxs-lookup"><span data-stu-id="3f21e-186">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="3f21e-187">*Lisans tabanlı indirimler, birden çok ücret türüne uygulanabilir.*</span><span class="sxs-lookup"><span data-stu-id="3f21e-187">*License-based discounts may be applied to multiple charge types.*</span></span>
