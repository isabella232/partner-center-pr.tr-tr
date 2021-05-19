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
ms.openlocfilehash: da3fc23a51cc70eec91a304f14189eb191c71339
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148117"
---
# <a name="credit-limit-enforcement-cle"></a><span data-ttu-id="9eeef-104">Kredi limiti zorlama (CLE)</span><span class="sxs-lookup"><span data-stu-id="9eeef-104">Credit limit enforcement (CLE)</span></span>

<span data-ttu-id="9eeef-105">**Uygun roller:** Faturalama yöneticisi</span><span class="sxs-lookup"><span data-stu-id="9eeef-105">**Appropriate roles**: Billing admin</span></span>

## <a name="your-credit-limit-and-how-it-works"></a><span data-ttu-id="9eeef-106">Kredi limiti ve nasıl çalıştığını</span><span class="sxs-lookup"><span data-stu-id="9eeef-106">Your credit limit and how it works</span></span>

<span data-ttu-id="9eeef-107">Kredi limitiniz, iş ortağı olarak bir iş ortağının belirli bir yıl içinde ürün veya abonelik satın almak için harcayabilirsiniz maksimum İş Ortağı Merkezi.</span><span class="sxs-lookup"><span data-stu-id="9eeef-107">Your credit limit is the maximum amount (in US dollars) that you as a partner can spend to purchase products or subscriptions in Partner Center.</span></span> <span data-ttu-id="9eeef-108">Kredi limitini aşarsanız, yeterli ödeme yapılana kadar yeni satın almalar yapamazsiniz.</span><span class="sxs-lookup"><span data-stu-id="9eeef-108">If you exceed your credit limit, you’ll be unable to make new purchases until sufficient payment has been made.</span></span> <span data-ttu-id="9eeef-109">Mevcut abonelikleriniz kesintisiz olarak devam eder.</span><span class="sxs-lookup"><span data-stu-id="9eeef-109">Your existing subscriptions will continue uninterrupted.</span></span>

<span data-ttu-id="9eeef-110">Kredi limitleri Azure planı, Azure rezervasyonları, Yazılım, Market, Azure 145 P, Office ve Dynamics ürünleri için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="9eeef-110">Credit limits apply to offers in Azure plan, Azure reservations, Software, Marketplace, Azure 145 P, Office, and Dynamics products.</span></span> <span data-ttu-id="9eeef-111">Kredi limitleri yenilemeler ve devam eden tüketim için geçerli değildir.</span><span class="sxs-lookup"><span data-stu-id="9eeef-111">Credit limits do not apply to renewals and ongoing consumption.</span></span>

<span data-ttu-id="9eeef-112">Ekleme döneminiz boyunca kredi limitini kiracı düzeyinde atariz.</span><span class="sxs-lookup"><span data-stu-id="9eeef-112">We assign your credit limit at the tenant level during your onboarding period.</span></span> <span data-ttu-id="9eeef-113">Bunu tahmini gelir, satın alma gücü ve ödeme geçmişinize göre temel alırız.</span><span class="sxs-lookup"><span data-stu-id="9eeef-113">We base it on your forecasted revenue, purchasing prowess, and payment history.</span></span> <span data-ttu-id="9eeef-114">Ardından kullanılabilir bakiyenizi hesaplamak için aşağıdaki formülü kullanıruz:</span><span class="sxs-lookup"><span data-stu-id="9eeef-114">We then use the following formula to calculate your available balance:</span></span>

<span data-ttu-id="9eeef-115">**[Kredi Limiti – (Gelen Satın Alma + Ödenmemiş Faturalar + Faturalanmamış Ücretler – Fazla Ödeme)]**</span><span class="sxs-lookup"><span data-stu-id="9eeef-115">**[Credit Limit – (Incoming Purchase + Outstanding Unpaid Invoices + Unbilled Charges – Overpayment)]**</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="9eeef-116">Sık Sorulan Sorular</span><span class="sxs-lookup"><span data-stu-id="9eeef-116">Frequently Asked Questions</span></span>

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a><span data-ttu-id="9eeef-117">Kredi limitim kiracıda mı yoksa genel düzeyde mi ayarlanmış?</span><span class="sxs-lookup"><span data-stu-id="9eeef-117">Is my credit limit set at the tenant or global level?</span></span>

<span data-ttu-id="9eeef-118">Kiracı düzeyi.</span><span class="sxs-lookup"><span data-stu-id="9eeef-118">The tenant level.</span></span> <span data-ttu-id="9eeef-119">Örneğin ABD, Kanada ve Japonya'dan faaliyette olduğunu varsayalım.</span><span class="sxs-lookup"><span data-stu-id="9eeef-119">For example, suppose you operate from the US, Canada, and Japan.</span></span> <span data-ttu-id="9eeef-120">Kanada kiracısı kredi sınırına ulaşırsa bu kiracı, kanada'da satın alma girişiminde İş Ortağı Merkezi.</span><span class="sxs-lookup"><span data-stu-id="9eeef-120">If the Canadian tenant reaches its credit limit, then that tenant will receive a notification when they attempt to make a purchase in Partner Center.</span></span> <span data-ttu-id="9eeef-121">Diğer kiracılar etkilenmez.</span><span class="sxs-lookup"><span data-stu-id="9eeef-121">The other tenants will not be affected.</span></span> 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a><span data-ttu-id="9eeef-122">Kredi sınırınızı aşsam, var olan müşterilere ve aboneliklere tam erişimle hizmet vermeye devam edebilir miyim?</span><span class="sxs-lookup"><span data-stu-id="9eeef-122">If I exceed my credit limit, can I continue servicing existing customers and subscriptions with full access?</span></span>

<span data-ttu-id="9eeef-123">Evet.</span><span class="sxs-lookup"><span data-stu-id="9eeef-123">Yes.</span></span> <span data-ttu-id="9eeef-124">Müşterilerinizin mevcut abonelikleriniz kesinti olmadan devam edecektir.</span><span class="sxs-lookup"><span data-stu-id="9eeef-124">Your customers’ existing subscriptions will continue without interruption.</span></span> <span data-ttu-id="9eeef-125">Ancak, müşterileriniz için yeni abonelikler satın alamaz.</span><span class="sxs-lookup"><span data-stu-id="9eeef-125">However, you cannot buy new subscriptions for your customers.</span></span>

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a><span data-ttu-id="9eeef-126">Hem doğrudan fatura ortakları hem de dolaylı sağlayıcılar için su geçerlidir mı?</span><span class="sxs-lookup"><span data-stu-id="9eeef-126">Does CLE apply to both direct bill partners and indirect providers?</span></span>

<span data-ttu-id="9eeef-127">Evet, her ikisi için de geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="9eeef-127">Yes, it applies to both.</span></span>

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a><span data-ttu-id="9eeef-128">Ödemem daha sonra hesabım halinde gönderdikten sonra daha fazla abonelik satın alabilir miyim?</span><span class="sxs-lookup"><span data-stu-id="9eeef-128">After I submit my payment to reinstate my account, when can I purchase more subscriptions?</span></span> 

<span data-ttu-id="9eeef-129">Microsoft 'un kredi denetimi sürecine devam etmek için tüm gereksinimleri aldığı varsayılırsa, ödemenizin 24 saat içinde satın alınması devam edebilir.</span><span class="sxs-lookup"><span data-stu-id="9eeef-129">You should be able to resume purchasing within 24 hours of your payment, assuming Microsoft has received all the requirements to proceed with the credit check process.</span></span>

### <a name="how-can-i-check-my-credit-limit"></a><span data-ttu-id="9eeef-130">Kredi sınırınızı nasıl denetlerim?</span><span class="sxs-lookup"><span data-stu-id="9eeef-130">How can I check my credit limit?</span></span>

<span data-ttu-id="9eeef-131">[ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com)Kredi sınırınızı görmek ve son satın alımlarla ilgili bilgi almak için iletişim kurun.</span><span class="sxs-lookup"><span data-stu-id="9eeef-131">Contact [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to see your credit limit and get information about recent purchases.</span></span>

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a><span data-ttu-id="9eeef-132">İtiraz durumunda olan faturalar kredi limitine karşı yapılsın mı?</span><span class="sxs-lookup"><span data-stu-id="9eeef-132">Do invoices that are in dispute count against the credit limit?</span></span>

<span data-ttu-id="9eeef-133">Evet.</span><span class="sxs-lookup"><span data-stu-id="9eeef-133">Yes.</span></span> <span data-ttu-id="9eeef-134">Bununla birlikte, sorunu çözmek için Microsoft ile iletişim kurun [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) .</span><span class="sxs-lookup"><span data-stu-id="9eeef-134">However, you can contact Microsoft at [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to resolve the issue.</span></span>

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a><span data-ttu-id="9eeef-135">Yazdığımda ne kadar süre sonra geri almam gerekir ucmwrcsp@microsoft.com ?</span><span class="sxs-lookup"><span data-stu-id="9eeef-135">How soon will I hear back if I write to ucmwrcsp@microsoft.com?</span></span>

<span data-ttu-id="9eeef-136">24 saatten az bir yanıt almanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="9eeef-136">You should have a response in less than 24 hours.</span></span> 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a><span data-ttu-id="9eeef-137">Microsoft, iş ortağının kredi limitini ayarlamak için hangi kriterleri kullanır?</span><span class="sxs-lookup"><span data-stu-id="9eeef-137">What criteria does Microsoft use for setting a partner’s credit limit?</span></span>

<span data-ttu-id="9eeef-138">Kredi sınırınızı tahmini gelirinize, satın alma destekine ve ödeme geçmişine göre belirliyoruz.</span><span class="sxs-lookup"><span data-stu-id="9eeef-138">We determine your credit limit based on your forecasted revenue, purchasing prowess, and payment history.</span></span>

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a><span data-ttu-id="9eeef-139">Kredi limiti Şu anda yeni ticaret deneyiminde zorlansın mı?</span><span class="sxs-lookup"><span data-stu-id="9eeef-139">Is the credit limit currently enforced on the New Commerce Experience?</span></span>

<span data-ttu-id="9eeef-140">Evet.</span><span class="sxs-lookup"><span data-stu-id="9eeef-140">Yes.</span></span> <span data-ttu-id="9eeef-141">Kredi limitleri, Iş ortağı merkezindeki tüm CSP programları ve ürünleri için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="9eeef-141">Credit limits apply to all CSP programs and products in Partner Center.</span></span>

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a><span data-ttu-id="9eeef-142">Kuruluşum kredi sınırına yaklaştığı zaman bildirimi alacak?</span><span class="sxs-lookup"><span data-stu-id="9eeef-142">Who will receive the notification when my organization is nearing its credit limit?</span></span>

<span data-ttu-id="9eeef-143">Kuruluşunuzun finans hesabı borçları ilgili kişisi bildirimi almalıdır.</span><span class="sxs-lookup"><span data-stu-id="9eeef-143">Your organization's Finance Account Payable contact should receive the notification.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9eeef-144">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="9eeef-144">Next steps</span></span>

[<span data-ttu-id="9eeef-145">Fatura temel bilgileri</span><span class="sxs-lookup"><span data-stu-id="9eeef-145">Billing basics</span></span>](./billing-basics.md)
