---
title: Geçerli birim fiyat hesaplaması
ms.topic: how-to
ms.date: 04/02/2021
description: Geçerli birim fiyatı ve nasıl hesaplanmış olduğu hakkında bilgi edinmek. Bu makalede ayrıca bir örnek hesaplama da yer alanmıştır.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 84beac77d41b8c11be9ac3cad87460eec9632ac4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147131"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="b0001-104">Azure planı tüketimi için geçerli birim fiyat hesaplaması</span><span class="sxs-lookup"><span data-stu-id="b0001-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="b0001-105">**Uygun roller:** Faturalama yöneticisi</span><span class="sxs-lookup"><span data-stu-id="b0001-105">**Appropriate roles**: Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="b0001-106">Geçerli birim fiyatı</span><span class="sxs-lookup"><span data-stu-id="b0001-106">The effective unit price</span></span>

<span data-ttu-id="b0001-107">Geçerli birim fiyatı ölçüm düzeyinde (kaynak düzeyi yerine) hesaplanır ve ölçüm kullanımına göre günlük olarak ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="b0001-107">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="b0001-108">Geçerli birim fiyatını hesaplamak için aşağıdaki üç faktörü kullanıyoruz:</span><span class="sxs-lookup"><span data-stu-id="b0001-108">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="b0001-109">Faturalama döngüsü boyunca günlük olarak izlenen tüketim</span><span class="sxs-lookup"><span data-stu-id="b0001-109">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="b0001-110">Ölçüm için faturalanabilir maliyet</span><span class="sxs-lookup"><span data-stu-id="b0001-110">Billable cost for the meter</span></span>
- <span data-ttu-id="b0001-111">Katmanlama (varsa)</span><span class="sxs-lookup"><span data-stu-id="b0001-111">Tiering (if applicable)</span></span>

<span data-ttu-id="b0001-112">Faturalama dönemi boyunca tüketimi günlük olarak izlenmiz nedeniyle, geçerli birim fiyatı dalgalı olur.</span><span class="sxs-lookup"><span data-stu-id="b0001-112">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="b0001-113">Tüketim hesaplaması durdurduktan ve faturalama dönemini kapatarak, verilen faturalama döneminin son fiyatı kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="b0001-113">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="b0001-114">Dördüncü veya beşinci ondalık ayırıcıdan sonra tüketimde en fazla değişiklik olduğunu görüyorsunuz.</span><span class="sxs-lookup"><span data-stu-id="b0001-114">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="b0001-115">Ölçümün katmanlı fiyatlandırmayı kullandığını bulma</span><span class="sxs-lookup"><span data-stu-id="b0001-115">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="b0001-116">Ölçümün katmanlı fiyatlandırma mı kullandığını bilmiyorsanız, bunu bulmak için aşağıdaki yordamı kullanın.</span><span class="sxs-lookup"><span data-stu-id="b0001-116">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="b0001-117">[İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="b0001-117">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="b0001-118">**Satış'ı** seçin, Fiyatlandırma **ve teklifler'i ve** ardından Azure **planı fiyatlandırması'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="b0001-118">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="b0001-119">Ölçüm kimliğiniz ile ilgili bilgileri bulun ve fiyatlandırma verilerinizi indirin.</span><span class="sxs-lookup"><span data-stu-id="b0001-119">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="b0001-120">Örnek hesaplama</span><span class="sxs-lookup"><span data-stu-id="b0001-120">Sample calculation</span></span>

<span data-ttu-id="b0001-121">Aşağıdaki tabloda, açık dönem boyunca geçerli birim fiyatı nasıl hesaplay geçtiğimize bir örnek verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="b0001-121">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="b0001-122">Tabloda aşağıdaki değerler geçerlidir:</span><span class="sxs-lookup"><span data-stu-id="b0001-122">In the table, the following values apply:</span></span> 

- <span data-ttu-id="b0001-123">**Up** = kaynağın birim fiyatı/saat = 0,868</span><span class="sxs-lookup"><span data-stu-id="b0001-123">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="b0001-124">**BCU** = ölçüm için faturalandırılabilir tüketim birimi</span><span class="sxs-lookup"><span data-stu-id="b0001-124">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="b0001-125">**BC** = BCU \* UP \* 0,85 ölçümü için faturalandırılabilir maliyet.</span><span class="sxs-lookup"><span data-stu-id="b0001-125">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="b0001-126">Bu, %15 PEC indirimle ilgili bir ayarlamayı yansıtır.</span><span class="sxs-lookup"><span data-stu-id="b0001-126">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="b0001-127">Daha sonra, minimum miktarı ücretlendirmeniz için değeri ondalık işaretinden sonra iki basamakla sınırlamak üzere işlevin alt sınırını kullanıyoruz.</span><span class="sxs-lookup"><span data-stu-id="b0001-127">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="b0001-128">**Etkin birim fiyatı** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="b0001-128">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="b0001-129">Not: Bu örnekteki ölçüm fiyatlandırma veya diğer indirimlerdeki katmanlara sahip değildir. indirim yüzdeleri ve diğer ayarlamalar için geçerli birim fiyat faktörleri.</span><span class="sxs-lookup"><span data-stu-id="b0001-129">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="b0001-130">Tarih</span><span class="sxs-lookup"><span data-stu-id="b0001-130">Date</span></span> | <span data-ttu-id="b0001-131">BCU (Faturalanabilir tüketim birimi)</span><span class="sxs-lookup"><span data-stu-id="b0001-131">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="b0001-132">BC (Faturalanabilir maliyet)</span><span class="sxs-lookup"><span data-stu-id="b0001-132">BC (Billable cost)</span></span> | <span data-ttu-id="b0001-133">Geçerli birim fiyatı</span><span class="sxs-lookup"><span data-stu-id="b0001-133">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="b0001-134">3-Ağu</span><span class="sxs-lookup"><span data-stu-id="b0001-134">3-Aug</span></span> | <span data-ttu-id="b0001-135">29</span><span class="sxs-lookup"><span data-stu-id="b0001-135">29</span></span> | <span data-ttu-id="b0001-136">21,39</span><span class="sxs-lookup"><span data-stu-id="b0001-136">21.39</span></span> | <span data-ttu-id="b0001-137">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="b0001-137">0.737586206896552</span></span> |
| <span data-ttu-id="b0001-138">10 Ağu</span><span class="sxs-lookup"><span data-stu-id="b0001-138">10-Aug</span></span> | <span data-ttu-id="b0001-139">210,950039</span><span class="sxs-lookup"><span data-stu-id="b0001-139">210.950039</span></span> | <span data-ttu-id="b0001-140">155,63</span><span class="sxs-lookup"><span data-stu-id="b0001-140">155.63</span></span> | <span data-ttu-id="b0001-141">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="b0001-141">0.737757626107858</span></span> |
| <span data-ttu-id="b0001-142">25 Ağu</span><span class="sxs-lookup"><span data-stu-id="b0001-142">25-Aug</span></span> | <span data-ttu-id="b0001-143">555,950039</span><span class="sxs-lookup"><span data-stu-id="b0001-143">555.950039</span></span> | <span data-ttu-id="b0001-144">410,17</span><span class="sxs-lookup"><span data-stu-id="b0001-144">410.17</span></span> | <span data-ttu-id="b0001-145">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="b0001-145">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="b0001-146">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="b0001-146">Next steps</span></span>

- [<span data-ttu-id="b0001-147">Faturalama ve vergiler</span><span class="sxs-lookup"><span data-stu-id="b0001-147">Billing and taxes</span></span>](billing.md)
