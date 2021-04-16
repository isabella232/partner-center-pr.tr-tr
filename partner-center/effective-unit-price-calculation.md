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
ms.openlocfilehash: 6c3c3a672de015c9f38fa0e34232da8d9913177c
ms.sourcegitcommit: 9f6be9bc8d9a065422d1ec8388bd770eb6cd9f33
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/16/2021
ms.locfileid: "107528566"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="c9b50-104">Azure plan tüketimi için geçerli birim fiyat hesaplaması</span><span class="sxs-lookup"><span data-stu-id="c9b50-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="c9b50-105">Geçerli birim fiyatı</span><span class="sxs-lookup"><span data-stu-id="c9b50-105">The effective unit price</span></span>

<span data-ttu-id="c9b50-106">Etkin birim fiyatı ölçüm düzeyinde hesaplanır (kaynak düzeyinden farklı olarak) ve ölçüm kullanımına göre günlük olarak ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="c9b50-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="c9b50-107">Geçerli birim fiyatını aşağıdaki üç faktörle hesapladık:</span><span class="sxs-lookup"><span data-stu-id="c9b50-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="c9b50-108">Fatura döngüsünün tamamında günlük izlenen tüketim</span><span class="sxs-lookup"><span data-stu-id="c9b50-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="c9b50-109">Ölçüm için faturalandırılabilir maliyet</span><span class="sxs-lookup"><span data-stu-id="c9b50-109">Billable cost for the meter</span></span>
- <span data-ttu-id="c9b50-110">Katmanlama (varsa)</span><span class="sxs-lookup"><span data-stu-id="c9b50-110">Tiering (if applicable)</span></span>

<span data-ttu-id="c9b50-111">Tüketimi faturalandırma döngüsünün tamamında günlük olarak izleyediğimiz için, etkin birim fiyatı dalgalanacaktır.</span><span class="sxs-lookup"><span data-stu-id="c9b50-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="c9b50-112">Belirli bir faturalandırma döngüsünün son fiyatı, tüketim hesaplamasını durdurup faturalandırma dönemini kapatdığımızda kullanılabilir olacaktır.</span><span class="sxs-lookup"><span data-stu-id="c9b50-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="c9b50-113">En fazla değişikliğin dördüncü veya beşinci ondalık konumdan sonra olduğunu görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="c9b50-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="c9b50-114">Ölçenin katmanlı fiyatlandırma kullanıp kullanmadığını öğrenin</span><span class="sxs-lookup"><span data-stu-id="c9b50-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="c9b50-115">Ölçmeniz katmanlı fiyatlandırma kullanıp kullanmadığını bilmiyorsanız, öğrenmek için aşağıdaki yordamı kullanın.</span><span class="sxs-lookup"><span data-stu-id="c9b50-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="c9b50-116">[İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="c9b50-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="c9b50-117">**Satış** öğesini seçin, **fiyatlandırma ve teklifler**' i seçin ve ardından **Azure plan fiyatlandırması**' nı seçin.</span><span class="sxs-lookup"><span data-stu-id="c9b50-117">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="c9b50-118">Ölçerinizi KIMLIĞE göre bulun ve ardından fiyatlandırma verilerinizi indirin.</span><span class="sxs-lookup"><span data-stu-id="c9b50-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="c9b50-119">Örnek hesaplama</span><span class="sxs-lookup"><span data-stu-id="c9b50-119">Sample calculation</span></span>

<span data-ttu-id="c9b50-120">Aşağıdaki tabloda, açık dönemde geçerli birim fiyatını nasıl hesapladığımızda bir örnek verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="c9b50-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="c9b50-121">Tabloda aşağıdaki değerler geçerlidir:</span><span class="sxs-lookup"><span data-stu-id="c9b50-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="c9b50-122">**Up** = kaynağın birim fiyatı/saat = 0,868</span><span class="sxs-lookup"><span data-stu-id="c9b50-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="c9b50-123">**BCU** = ölçüm için faturalandırılabilir tüketim birimi</span><span class="sxs-lookup"><span data-stu-id="c9b50-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="c9b50-124">**BC** = BCU \* UP \* 0,85 ölçümü için faturalandırılabilir maliyet.</span><span class="sxs-lookup"><span data-stu-id="c9b50-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="c9b50-125">Bu, %15 PEC indirimle ilgili bir ayarlamayı yansıtır.</span><span class="sxs-lookup"><span data-stu-id="c9b50-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="c9b50-126">Daha sonra, minimum miktarı ücretlendirmeniz için değeri ondalık işaretinden sonra iki basamakla sınırlamak üzere işlevin alt sınırını kullanıyoruz.</span><span class="sxs-lookup"><span data-stu-id="c9b50-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="c9b50-127">**Etkin birim fiyatı** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="c9b50-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="c9b50-128">Not: Bu örnekteki ölçüm fiyatlandırma veya diğer indirimlerdeki katmanlara sahip değildir. indirim yüzdeleri ve diğer ayarlamalar için geçerli birim fiyat faktörleri.</span><span class="sxs-lookup"><span data-stu-id="c9b50-128">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="c9b50-129">Tarih</span><span class="sxs-lookup"><span data-stu-id="c9b50-129">Date</span></span> | <span data-ttu-id="c9b50-130">BCU (Faturalanabilir tüketim birimi)</span><span class="sxs-lookup"><span data-stu-id="c9b50-130">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="c9b50-131">BC (Faturalanabilir maliyet)</span><span class="sxs-lookup"><span data-stu-id="c9b50-131">BC (Billable cost)</span></span> | <span data-ttu-id="c9b50-132">Geçerli birim fiyatı</span><span class="sxs-lookup"><span data-stu-id="c9b50-132">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="c9b50-133">3-Ağu</span><span class="sxs-lookup"><span data-stu-id="c9b50-133">3-Aug</span></span> | <span data-ttu-id="c9b50-134">29</span><span class="sxs-lookup"><span data-stu-id="c9b50-134">29</span></span> | <span data-ttu-id="c9b50-135">21,39</span><span class="sxs-lookup"><span data-stu-id="c9b50-135">21.39</span></span> | <span data-ttu-id="c9b50-136">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="c9b50-136">0.737586206896552</span></span> |
| <span data-ttu-id="c9b50-137">10 Ağu</span><span class="sxs-lookup"><span data-stu-id="c9b50-137">10-Aug</span></span> | <span data-ttu-id="c9b50-138">210,950039</span><span class="sxs-lookup"><span data-stu-id="c9b50-138">210.950039</span></span> | <span data-ttu-id="c9b50-139">155,63</span><span class="sxs-lookup"><span data-stu-id="c9b50-139">155.63</span></span> | <span data-ttu-id="c9b50-140">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="c9b50-140">0.737757626107858</span></span> |
| <span data-ttu-id="c9b50-141">25 Ağu</span><span class="sxs-lookup"><span data-stu-id="c9b50-141">25-Aug</span></span> | <span data-ttu-id="c9b50-142">555,950039</span><span class="sxs-lookup"><span data-stu-id="c9b50-142">555.950039</span></span> | <span data-ttu-id="c9b50-143">410,17</span><span class="sxs-lookup"><span data-stu-id="c9b50-143">410.17</span></span> | <span data-ttu-id="c9b50-144">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="c9b50-144">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="c9b50-145">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="c9b50-145">Next steps</span></span>

- [<span data-ttu-id="c9b50-146">Faturalama ve vergiler</span><span class="sxs-lookup"><span data-stu-id="c9b50-146">Billing and taxes</span></span>](billing.md)
