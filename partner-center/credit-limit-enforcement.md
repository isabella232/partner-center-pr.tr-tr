---
title: Kredi limiti zorlama
ms.topic: how-to
ms.date: 05/11/2021
description: Kredi limitini ve nasıl hesaplanmış olduğunu öğrenin. SSS'yi içerir.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cf0d3c38b301c363a4a990db5258cf2a3f30d487
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/12/2021
ms.locfileid: "109819386"
---
# <a name="credit-limit-enforcement-cle"></a><span data-ttu-id="488e5-104">Kredi limiti zorlama (CLE)</span><span class="sxs-lookup"><span data-stu-id="488e5-104">Credit limit enforcement (CLE)</span></span>

<span data-ttu-id="488e5-105">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="488e5-105">**Appropriate roles**</span></span>

- <span data-ttu-id="488e5-106">Faturalama yöneticisi</span><span class="sxs-lookup"><span data-stu-id="488e5-106">Billing admin</span></span>

## <a name="your-credit-limit-and-how-it-works"></a><span data-ttu-id="488e5-107">Kredi limiti ve nasıl çalıştığını</span><span class="sxs-lookup"><span data-stu-id="488e5-107">Your credit limit and how it works</span></span>

<span data-ttu-id="488e5-108">Kredi limitiniz, iş ortağı olarak bir iş ortağının belirli bir yıl içinde ürün veya abonelik satın almak için harcayabilirsiniz maksimum İş Ortağı Merkezi.</span><span class="sxs-lookup"><span data-stu-id="488e5-108">Your credit limit is the maximum amount (in US dollars) that you as a partner can spend to purchase products or subscriptions in Partner Center.</span></span> <span data-ttu-id="488e5-109">Kredi limitini aşarsanız, yeterli ödeme yapılana kadar yeni satın almalar yapamazsiniz.</span><span class="sxs-lookup"><span data-stu-id="488e5-109">If you exceed your credit limit, you’ll be unable to make new purchases until sufficient payment has been made.</span></span> <span data-ttu-id="488e5-110">Mevcut abonelikleriniz kesintisiz olarak devam eder.</span><span class="sxs-lookup"><span data-stu-id="488e5-110">Your existing subscriptions will continue uninterrupted.</span></span>

<span data-ttu-id="488e5-111">Kredi limitleri Azure planı, Azure rezervasyonları, Yazılım, Market, Azure 145 P, Office ve Dynamics ürünleri için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="488e5-111">Credit limits apply to offers in Azure plan, Azure reservations, Software, Marketplace, Azure 145 P, Office, and Dynamics products.</span></span> <span data-ttu-id="488e5-112">Kredi limitleri yenilemeler ve devam eden tüketim için geçerli değildir.</span><span class="sxs-lookup"><span data-stu-id="488e5-112">Credit limits do not apply to renewals and ongoing consumption.</span></span>

<span data-ttu-id="488e5-113">Ekleme döneminiz boyunca kredi limitini kiracı düzeyinde atariz.</span><span class="sxs-lookup"><span data-stu-id="488e5-113">We assign your credit limit at the tenant level during your onboarding period.</span></span> <span data-ttu-id="488e5-114">Bunu tahmini gelir, satın alma gücü ve ödeme geçmişinize göre temel alırız.</span><span class="sxs-lookup"><span data-stu-id="488e5-114">We base it on your forecasted revenue, purchasing prowess, and payment history.</span></span> <span data-ttu-id="488e5-115">Ardından kullanılabilir bakiyenizi hesaplamak için aşağıdaki formülü kullanıruz:</span><span class="sxs-lookup"><span data-stu-id="488e5-115">We then use the following formula to calculate your available balance:</span></span>

<span data-ttu-id="488e5-116">**[Kredi Limiti – (Gelen Satın Alma + Ödenmemiş Faturalar + Faturalanmamış Ücretler – Fazla Ödeme)]**</span><span class="sxs-lookup"><span data-stu-id="488e5-116">**[Credit Limit – (Incoming Purchase + Outstanding Unpaid Invoices + Unbilled Charges – Overpayment)]**</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="488e5-117">Sık Sorulan Sorular</span><span class="sxs-lookup"><span data-stu-id="488e5-117">Frequently Asked Questions</span></span>

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a><span data-ttu-id="488e5-118">Kredi limitim kiracıda mı yoksa genel düzeyde mi ayarlanmış?</span><span class="sxs-lookup"><span data-stu-id="488e5-118">Is my credit limit set at the tenant or global level?</span></span>

<span data-ttu-id="488e5-119">Kiracı düzeyi.</span><span class="sxs-lookup"><span data-stu-id="488e5-119">The tenant level.</span></span> <span data-ttu-id="488e5-120">Örneğin ABD, Kanada ve Japonya'dan faaliyette olduğunu varsayalım.</span><span class="sxs-lookup"><span data-stu-id="488e5-120">For example, suppose you operate from the US, Canada, and Japan.</span></span> <span data-ttu-id="488e5-121">Kanada kiracısı kredi sınırına ulaşırsa bu kiracı, kanada'da satın alma girişiminde İş Ortağı Merkezi.</span><span class="sxs-lookup"><span data-stu-id="488e5-121">If the Canadian tenant reaches its credit limit, then that tenant will receive a notification when they attempt to make a purchase in Partner Center.</span></span> <span data-ttu-id="488e5-122">Diğer kiracılar etkilenmez.</span><span class="sxs-lookup"><span data-stu-id="488e5-122">The other tenants will not be affected.</span></span> 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a><span data-ttu-id="488e5-123">Kredi limitimi aşarsa, mevcut müşterilere ve aboneliklere tam erişimle hizmet vermeye devam miyim?</span><span class="sxs-lookup"><span data-stu-id="488e5-123">If I exceed my credit limit, can I continue servicing existing customers and subscriptions with full access?</span></span>

<span data-ttu-id="488e5-124">Evet.</span><span class="sxs-lookup"><span data-stu-id="488e5-124">Yes.</span></span> <span data-ttu-id="488e5-125">Müşterilerin mevcut abonelikleri kesintisiz olarak devam eder.</span><span class="sxs-lookup"><span data-stu-id="488e5-125">Your customers’ existing subscriptions will continue without interruption.</span></span> <span data-ttu-id="488e5-126">Ancak, müşterileriniz için yeni abonelikler satın aamazsınız.</span><span class="sxs-lookup"><span data-stu-id="488e5-126">However, you cannot buy new subscriptions for your customers.</span></span>

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a><span data-ttu-id="488e5-127">CLE hem doğrudan fatura iş ortakları hem de dolaylı sağlayıcılar için geçerli mi?</span><span class="sxs-lookup"><span data-stu-id="488e5-127">Does CLE apply to both direct bill partners and indirect providers?</span></span>

<span data-ttu-id="488e5-128">Evet, her ikisi için de geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="488e5-128">Yes, it applies to both.</span></span>

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a><span data-ttu-id="488e5-129">Hesabımı yeniden iade etmek için ödememi gönderdikten sonra, ne zaman daha fazla abonelik satın a bilmiyorum?</span><span class="sxs-lookup"><span data-stu-id="488e5-129">After I submit my payment to reinstate my account, when can I purchase more subscriptions?</span></span> 

<span data-ttu-id="488e5-130">Microsoft'un kredi denetimi işlemine devam etmek için tüm gereksinimleri aldığı varsayıldı ise, ödemenizi 24 saat içinde satın almayı sürdürebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="488e5-130">You should be able to resume purchasing within 24 hours of your payment, assuming Microsoft has received all the requirements to proceed with the credit check process.</span></span>

### <a name="how-can-i-check-my-credit-limit"></a><span data-ttu-id="488e5-131">Kredi limitimi nasıl kontrol miyim?</span><span class="sxs-lookup"><span data-stu-id="488e5-131">How can I check my credit limit?</span></span>

<span data-ttu-id="488e5-132">Kredi [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) limitini görmek ve son satın almalar hakkında bilgi almak için ile iletişime geçin.</span><span class="sxs-lookup"><span data-stu-id="488e5-132">Contact [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to see your credit limit and get information about recent purchases.</span></span>

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a><span data-ttu-id="488e5-133">İtiraz konusu olan faturalar kredi limiti üzerinde sayılır mı?</span><span class="sxs-lookup"><span data-stu-id="488e5-133">Do invoices that are in dispute count against the credit limit?</span></span>

<span data-ttu-id="488e5-134">Evet.</span><span class="sxs-lookup"><span data-stu-id="488e5-134">Yes.</span></span> <span data-ttu-id="488e5-135">Bununla birlikte, sorunu çözmek için microsoft [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) ile iletişime geçin.</span><span class="sxs-lookup"><span data-stu-id="488e5-135">However, you can contact Microsoft at [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to resolve the issue.</span></span>

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a><span data-ttu-id="488e5-136">'a yazarsanız ne kadar kısa süre sonra geri ucmwrcsp@microsoft.com dinleyeceğiz?</span><span class="sxs-lookup"><span data-stu-id="488e5-136">How soon will I hear back if I write to ucmwrcsp@microsoft.com?</span></span>

<span data-ttu-id="488e5-137">Yanıtın 24 saatten kısa bir sürede yanıta sahip olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="488e5-137">You should have a response in less than 24 hours.</span></span> 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a><span data-ttu-id="488e5-138">Microsoft, iş ortağının kredi limitini ayarlarken hangi ölçütleri kullanır?</span><span class="sxs-lookup"><span data-stu-id="488e5-138">What criteria does Microsoft use for setting a partner’s credit limit?</span></span>

<span data-ttu-id="488e5-139">Kredi limitini tahmin edilen gelir, satın alma gücü ve ödeme geçmişinize göre belirleriz.</span><span class="sxs-lookup"><span data-stu-id="488e5-139">We determine your credit limit based on your forecasted revenue, purchasing prowess, and payment history.</span></span>

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a><span data-ttu-id="488e5-140">Kredi limiti şu anda Yeni Ticaret Deneyimi'ne mi uygulanıyor?</span><span class="sxs-lookup"><span data-stu-id="488e5-140">Is the credit limit currently enforced on the New Commerce Experience?</span></span>

<span data-ttu-id="488e5-141">Evet.</span><span class="sxs-lookup"><span data-stu-id="488e5-141">Yes.</span></span> <span data-ttu-id="488e5-142">Kredi limitleri, tüm csP programlarına ve ürünlerine İş Ortağı Merkezi.</span><span class="sxs-lookup"><span data-stu-id="488e5-142">Credit limits apply to all CSP programs and products in Partner Center.</span></span>

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a><span data-ttu-id="488e5-143">Kuruluşum kredi sınırına yaklaşacaksa kim bildirim alacak?</span><span class="sxs-lookup"><span data-stu-id="488e5-143">Who will receive the notification when my organization is nearing its credit limit?</span></span>

<span data-ttu-id="488e5-144">Bildirimin, kuruluşun Finans Hesabı Borç ilgili kişisi tarafından verilmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="488e5-144">Your organization's Finance Account Payable contact should receive the notification.</span></span>

## <a name="next-steps"></a><span data-ttu-id="488e5-145">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="488e5-145">Next steps</span></span>

[<span data-ttu-id="488e5-146">Fatura temel bilgileri</span><span class="sxs-lookup"><span data-stu-id="488e5-146">Billing basics</span></span>](./billing-basics.md)
