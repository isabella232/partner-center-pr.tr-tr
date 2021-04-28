---
title: Geçerli birim fiyat hesaplaması
ms.topic: how-to
ms.date: 04/02/2021
description: Geçerli birim fiyatı ve nasıl hesaplandığı hakkında bilgi edinin. Bu makale, örnek bir hesaplama da içerir.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1473b3c0b90cca1152b4dab0b8efec86dbc3d22d
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172226"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="ae0a1-104">Azure plan tüketimi için geçerli birim fiyat hesaplaması</span><span class="sxs-lookup"><span data-stu-id="ae0a1-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="ae0a1-105">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="ae0a1-105">**Appropriate roles**</span></span>

- <span data-ttu-id="ae0a1-106">Faturalama yöneticisi</span><span class="sxs-lookup"><span data-stu-id="ae0a1-106">Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="ae0a1-107">Geçerli birim fiyatı</span><span class="sxs-lookup"><span data-stu-id="ae0a1-107">The effective unit price</span></span>

<span data-ttu-id="ae0a1-108">Etkin birim fiyatı ölçüm düzeyinde hesaplanır (kaynak düzeyinden farklı olarak) ve ölçüm kullanımına göre günlük olarak ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="ae0a1-108">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="ae0a1-109">Geçerli birim fiyatını aşağıdaki üç faktörle hesapladık:</span><span class="sxs-lookup"><span data-stu-id="ae0a1-109">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="ae0a1-110">Fatura döngüsünün tamamında günlük izlenen tüketim</span><span class="sxs-lookup"><span data-stu-id="ae0a1-110">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="ae0a1-111">Ölçüm için faturalandırılabilir maliyet</span><span class="sxs-lookup"><span data-stu-id="ae0a1-111">Billable cost for the meter</span></span>
- <span data-ttu-id="ae0a1-112">Katmanlama (varsa)</span><span class="sxs-lookup"><span data-stu-id="ae0a1-112">Tiering (if applicable)</span></span>

<span data-ttu-id="ae0a1-113">Tüketimi faturalandırma döngüsünün tamamında günlük olarak izleyediğimiz için, etkin birim fiyatı dalgalanacaktır.</span><span class="sxs-lookup"><span data-stu-id="ae0a1-113">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="ae0a1-114">Belirli bir faturalandırma döngüsünün son fiyatı, tüketim hesaplamasını durdurup faturalandırma dönemini kapatdığımızda kullanılabilir olacaktır.</span><span class="sxs-lookup"><span data-stu-id="ae0a1-114">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="ae0a1-115">En fazla değişikliğin dördüncü veya beşinci ondalık konumdan sonra olduğunu görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="ae0a1-115">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="ae0a1-116">Ölçenin katmanlı fiyatlandırma kullanıp kullanmadığını öğrenin</span><span class="sxs-lookup"><span data-stu-id="ae0a1-116">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="ae0a1-117">Ölçmeniz katmanlı fiyatlandırma kullanıp kullanmadığını bilmiyorsanız, öğrenmek için aşağıdaki yordamı kullanın.</span><span class="sxs-lookup"><span data-stu-id="ae0a1-117">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="ae0a1-118">[İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="ae0a1-118">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="ae0a1-119">**Satış** öğesini seçin, **fiyatlandırma ve teklifler**' i seçin ve ardından **Azure plan fiyatlandırması**' nı seçin.</span><span class="sxs-lookup"><span data-stu-id="ae0a1-119">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="ae0a1-120">Ölçerinizi KIMLIĞE göre bulun ve ardından fiyatlandırma verilerinizi indirin.</span><span class="sxs-lookup"><span data-stu-id="ae0a1-120">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="ae0a1-121">Örnek hesaplama</span><span class="sxs-lookup"><span data-stu-id="ae0a1-121">Sample calculation</span></span>

<span data-ttu-id="ae0a1-122">Aşağıdaki tabloda, açık dönemde geçerli birim fiyatını nasıl hesapladığımızda bir örnek verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="ae0a1-122">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="ae0a1-123">Tabloda aşağıdaki değerler geçerlidir:</span><span class="sxs-lookup"><span data-stu-id="ae0a1-123">In the table, the following values apply:</span></span> 

- <span data-ttu-id="ae0a1-124">**Up** = kaynağın birim fiyatı/saat = 0,868</span><span class="sxs-lookup"><span data-stu-id="ae0a1-124">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="ae0a1-125">**BCU** = ölçüm için faturalandırılabilir tüketim birimi</span><span class="sxs-lookup"><span data-stu-id="ae0a1-125">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="ae0a1-126">**BC** = BCU \* UP \* 0,85 ölçümü için faturalandırılabilir maliyet.</span><span class="sxs-lookup"><span data-stu-id="ae0a1-126">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="ae0a1-127">Bu, %15 PEC indirimle ilgili bir ayarlamayı yansıtır.</span><span class="sxs-lookup"><span data-stu-id="ae0a1-127">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="ae0a1-128">Daha sonra, minimum miktarı ücretlendirmeniz için değeri ondalık işaretinden sonra iki basamakla sınırlamak üzere işlevin alt sınırını kullanıyoruz.</span><span class="sxs-lookup"><span data-stu-id="ae0a1-128">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="ae0a1-129">**Etkin birim fiyatı** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="ae0a1-129">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="ae0a1-130">Not: Bu örnekteki ölçüm fiyatlandırma veya diğer indirimlerdeki katmanlara sahip değildir. indirim yüzdeleri ve diğer ayarlamalar için geçerli birim fiyat faktörleri.</span><span class="sxs-lookup"><span data-stu-id="ae0a1-130">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="ae0a1-131">Tarih</span><span class="sxs-lookup"><span data-stu-id="ae0a1-131">Date</span></span> | <span data-ttu-id="ae0a1-132">BCU (Faturalanabilir tüketim birimi)</span><span class="sxs-lookup"><span data-stu-id="ae0a1-132">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="ae0a1-133">BC (Faturalanabilir maliyet)</span><span class="sxs-lookup"><span data-stu-id="ae0a1-133">BC (Billable cost)</span></span> | <span data-ttu-id="ae0a1-134">Geçerli birim fiyatı</span><span class="sxs-lookup"><span data-stu-id="ae0a1-134">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="ae0a1-135">3-Ağu</span><span class="sxs-lookup"><span data-stu-id="ae0a1-135">3-Aug</span></span> | <span data-ttu-id="ae0a1-136">29</span><span class="sxs-lookup"><span data-stu-id="ae0a1-136">29</span></span> | <span data-ttu-id="ae0a1-137">21,39</span><span class="sxs-lookup"><span data-stu-id="ae0a1-137">21.39</span></span> | <span data-ttu-id="ae0a1-138">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="ae0a1-138">0.737586206896552</span></span> |
| <span data-ttu-id="ae0a1-139">10 Ağu</span><span class="sxs-lookup"><span data-stu-id="ae0a1-139">10-Aug</span></span> | <span data-ttu-id="ae0a1-140">210,950039</span><span class="sxs-lookup"><span data-stu-id="ae0a1-140">210.950039</span></span> | <span data-ttu-id="ae0a1-141">155,63</span><span class="sxs-lookup"><span data-stu-id="ae0a1-141">155.63</span></span> | <span data-ttu-id="ae0a1-142">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="ae0a1-142">0.737757626107858</span></span> |
| <span data-ttu-id="ae0a1-143">25 Ağu</span><span class="sxs-lookup"><span data-stu-id="ae0a1-143">25-Aug</span></span> | <span data-ttu-id="ae0a1-144">555,950039</span><span class="sxs-lookup"><span data-stu-id="ae0a1-144">555.950039</span></span> | <span data-ttu-id="ae0a1-145">410,17</span><span class="sxs-lookup"><span data-stu-id="ae0a1-145">410.17</span></span> | <span data-ttu-id="ae0a1-146">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="ae0a1-146">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="ae0a1-147">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="ae0a1-147">Next steps</span></span>

- [<span data-ttu-id="ae0a1-148">Faturalama ve vergiler</span><span class="sxs-lookup"><span data-stu-id="ae0a1-148">Billing and taxes</span></span>](billing.md)
