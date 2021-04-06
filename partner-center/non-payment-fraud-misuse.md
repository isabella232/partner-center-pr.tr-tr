---
title: Ödeme yapılmaması, sahtekarlık veya suistimal durumlarını yönetme
description: Iş Ortağı Merkezi 'nde bu riskleri yönetmek ve azaltmak için çevrimiçi işlemlere ve en iyi yöntemlere dahil olan çeşitli riskler hakkında bilgi edinin.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: 9b3beef70052ad204327dd53c4aa9f477056bbcb
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441872"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a><span data-ttu-id="7261c-103">Ödeme alınamaması, dolandırıcılık veya kötüye kullanım durumlarını İş Ortağı Merkezi’nde yönetme</span><span class="sxs-lookup"><span data-stu-id="7261c-103">Managing non-payment, fraud, or misuse in Partner Center</span></span>

<span data-ttu-id="7261c-104">Aşağıdakiler cihazlar için geçerlidir:</span><span class="sxs-lookup"><span data-stu-id="7261c-104">Applies to:</span></span>

- <span data-ttu-id="7261c-105">Microsoft Cloud for US Government için İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="7261c-105">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="7261c-106">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="7261c-106">**Appropriate roles**</span></span>

- <span data-ttu-id="7261c-107">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="7261c-107">Global admin</span></span>
- <span data-ttu-id="7261c-108">Kullanıcı Yönetimi Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="7261c-108">User management admin</span></span>
- <span data-ttu-id="7261c-109">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="7261c-109">Admin agent</span></span>
- <span data-ttu-id="7261c-110">Faturalama yöneticisi</span><span class="sxs-lookup"><span data-stu-id="7261c-110">Billing admin</span></span>

<span data-ttu-id="7261c-111">Müşterileriniz ve/veya müşterilerin satın alınan hizmetlerin ödemesinden sorumlu satın alma işlemleri için mali olarak sorumlusunuz.</span><span class="sxs-lookup"><span data-stu-id="7261c-111">You are financially responsible for fraudulent purchases by your customers and/or customers' non-payment of purchased services.</span></span> <span data-ttu-id="7261c-112">Bu nedenle, *sahte önleme ve algılama riski azaltma denetimlerini yerleştirmenizi öneririz*.</span><span class="sxs-lookup"><span data-stu-id="7261c-112">Therefore, *we strongly recommend that you put in place fraud prevention and detection risk mitigation controls*.</span></span>

<span data-ttu-id="7261c-113">Sahte etkinlik veya kötüye kullanımı önlemek için, olası riskleri anlamak ve pozlandırmayı azaltabileceğiniz ilke ve uygulamalar geliştirmek önemlidir.</span><span class="sxs-lookup"><span data-stu-id="7261c-113">To avoid and/or address fraudulent activity or misuse, it's important to understand potential risks and to develop policies and practices that can reduce your exposure.</span></span>

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a><span data-ttu-id="7261c-114">Microsoft kabul edilebilir kullanım Ilkesi zorlaması</span><span class="sxs-lookup"><span data-stu-id="7261c-114">Enforcement of Microsoft Acceptable Use Policy</span></span>

<span data-ttu-id="7261c-115">Microsoft, kabul edilen kullanım Ilkesini ihlal ettiğimiz ya da şüpheli olduğunu düşündüğünüz iş ortağı veya müşteri etkinliğini algılarsa, zorlama adımları ele alınacaktır.</span><span class="sxs-lookup"><span data-stu-id="7261c-115">If Microsoft detects partner or customer activity that we confirm or suspect violates the Acceptable Use Policy, we will take enforcement steps.</span></span> <span data-ttu-id="7261c-116">Müşteri hemen askıya alınabilir.</span><span class="sxs-lookup"><span data-stu-id="7261c-116">The customer could be immediately suspended.</span></span> <span data-ttu-id="7261c-117">Microsoft tarafından yapılan istekleriniz için zorlama eylemleri hakkında bilgilendirilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7261c-117">You'll be notified of enforcement actions or updated on your requests by Microsoft.</span></span>

## <a name="abuse-of-service-risks"></a><span data-ttu-id="7261c-118">Hizmet riskleri kötüye kullanımı</span><span class="sxs-lookup"><span data-stu-id="7261c-118">Abuse of service risks</span></span>

<span data-ttu-id="7261c-119">**Hizmet riskleri kötüye kullanımı,** bulut hizmetlerini Microsoft 'un kabul edilebilir kullanım ilkesi ihlaline neden olan müşteriler anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="7261c-119">**Abuse of service** risks means customers who use cloud services in violation of Microsoft's Acceptable Use Policy.</span></span>

### <a name="examples-of-abuse-of-service"></a><span data-ttu-id="7261c-120">Hizmetin kötüye kullanımı örnekleri</span><span class="sxs-lookup"><span data-stu-id="7261c-120">Examples of abuse of service</span></span>

<span data-ttu-id="7261c-121">Bu Microsoft 'un kabul edilebilir kullanım ilkesi ihlalleri örnekleri şunlar olabilir:</span><span class="sxs-lookup"><span data-stu-id="7261c-121">Examples of these violations of Microsoft's acceptable use policy can include:</span></span>

- <span data-ttu-id="7261c-122">Yığın posta</span><span class="sxs-lookup"><span data-stu-id="7261c-122">Spamming</span></span>
- <span data-ttu-id="7261c-123">Bilgisayar korsanlığı</span><span class="sxs-lookup"><span data-stu-id="7261c-123">Hacking</span></span>
- <span data-ttu-id="7261c-124">Dağıtılmış hizmet reddi (DDoS) saldırıları</span><span class="sxs-lookup"><span data-stu-id="7261c-124">Distributed denial-of-service (DDoS) attacks</span></span>
- <span data-ttu-id="7261c-125">Bitpara madenciliği</span><span class="sxs-lookup"><span data-stu-id="7261c-125">Bitcoin mining</span></span>
- <span data-ttu-id="7261c-126">Kötü amaçlı yazılım dağıtımı</span><span class="sxs-lookup"><span data-stu-id="7261c-126">Malware distribution</span></span>
- <span data-ttu-id="7261c-127">Korsan aboneliklerin el satımı</span><span class="sxs-lookup"><span data-stu-id="7261c-127">Resale of pirated subscriptions</span></span>

## <a name="theft-of-service-risks"></a><span data-ttu-id="7261c-128">Hizmet riskleri hırsızlığı</span><span class="sxs-lookup"><span data-stu-id="7261c-128">Theft of service risks</span></span>

<span data-ttu-id="7261c-129">**Hizmet riskleri hırsızlığı** , tüketilen hizmetler için ödeme yapma amacı olmayan müşteriler anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="7261c-129">**Theft of service** risks means customers who have no intention of paying for consumed services.</span></span> <span data-ttu-id="7261c-130">Bu hırsızlık, çalınmış ödeme araçları 'nı kullanarak, yanlış faturalandırma bilgileri sağlar ve/veya bekleyen bakiyelerde varsayılan değerleri içerir.</span><span class="sxs-lookup"><span data-stu-id="7261c-130">This theft may involve using stolen payment instruments, providing false billing information, and/or defaulting on outstanding balances.</span></span>

### <a name="examples-of-service-theft"></a><span data-ttu-id="7261c-131">Hizmet hırsızlığı örnekleri</span><span class="sxs-lookup"><span data-stu-id="7261c-131">Examples of service theft</span></span>

<span data-ttu-id="7261c-132">Bu çevrimiçi işlem risklerine örnek olarak şunlar verilebilir:</span><span class="sxs-lookup"><span data-stu-id="7261c-132">Examples of these online transaction risks can include:</span></span>

- <span data-ttu-id="7261c-133">Kişide olmayan işlemler ("kredi kartı yok" işlemleri)</span><span class="sxs-lookup"><span data-stu-id="7261c-133">Transactions that don't occur in person ("credit card not present" transactions)</span></span>
- <span data-ttu-id="7261c-134">Yanlış temsil edilen kimlikler</span><span class="sxs-lookup"><span data-stu-id="7261c-134">Misrepresented identities</span></span>
- <span data-ttu-id="7261c-135">İlk ödeme alınmadan önce sağlanan ve kullanılan hizmetler</span><span class="sxs-lookup"><span data-stu-id="7261c-135">Services provisioned and used before initial payment is received</span></span>
- <span data-ttu-id="7261c-136">Çevrimiçi sahtekarlık için gelişen pazarlar ve/veya yüksek riskli bölgeler</span><span class="sxs-lookup"><span data-stu-id="7261c-136">Emerging markets and/or high-risk regions for online fraud</span></span>
- <span data-ttu-id="7261c-137">Hesap oluşturmayı otomatikleştirin ve hatalı aktör yaparak satın alabilirsiniz</span><span class="sxs-lookup"><span data-stu-id="7261c-137">Automate account creation and purchasing by bad actors</span></span>

## <a name="managing-online-risk"></a><span data-ttu-id="7261c-138">Çevrimiçi riski yönetme</span><span class="sxs-lookup"><span data-stu-id="7261c-138">Managing online risk</span></span>

<span data-ttu-id="7261c-139">Müşteri ilişkilerinizin yaşam döngülerinde çevrimiçi işlem risklerinin pozlamasını azaltmak üzere ilke ve uygulamalar geliştirmenize yardımcı olması için aşağıdaki önerileri kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7261c-139">You can use the following recommendations to help you develop policies and practices to reduce your exposure to online transaction risks in the lifecycle of your customer relationships.</span></span>

### <a name="onboarding-new-customers"></a><span data-ttu-id="7261c-140">Yeni müşterileri ekleme</span><span class="sxs-lookup"><span data-stu-id="7261c-140">Onboarding new customers</span></span>

<span data-ttu-id="7261c-141">Yeni müşterileri ekleme sırasında çevrimiçi riskleri azaltmaya yönelik öneriler şunlardır:</span><span class="sxs-lookup"><span data-stu-id="7261c-141">Suggestions for reducing online risks when onboarding new customers include:</span></span>

- <span data-ttu-id="7261c-142">Mümkün olduğunda müşterilerle kişisel ilişkiler oluşturun (örneğin, müşterilere telefonla iletişim kurun).</span><span class="sxs-lookup"><span data-stu-id="7261c-142">Establish personal relationships with customers when possible (for example, contacting customers by phone).</span></span>
- <span data-ttu-id="7261c-143">Daha iyi Yöntemler (kredi ofisleri veya iş ticari rapor kuruluşlarını kullanma gibi) sayesinde müşterilerin kimlik bilgilerini ve arka planını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="7261c-143">Verify customers' credentials and background through better methods (such as using credit bureaus or business commercial report agencies).</span></span>
- <span data-ttu-id="7261c-144">Robot hesap oluşturma ve satın alma işlemlerini en aza indirmek için kaydolma sırasında Multi-Factor Authentication (SMS doğrulaması gibi) kullanın.</span><span class="sxs-lookup"><span data-stu-id="7261c-144">Use multi-factor authentication (such as SMS verification) during sign-up to minimize exposure to robotic account creation and purchasing.</span></span>
- <span data-ttu-id="7261c-145">Hizmetleri (dijital kimlik hizmetleri gibi) kullanarak kimlikleri yönetin ve izleyin.</span><span class="sxs-lookup"><span data-stu-id="7261c-145">Manage and track identities using services (such as digital identity services).</span></span>
- <span data-ttu-id="7261c-146">Yoğun kredi kartı sahtekarlık algılama sistemleriyle müşterinin mali gücünü değerlendirin.</span><span class="sxs-lookup"><span data-stu-id="7261c-146">Assess customer financial strength through rigorous credit card fraud detection systems.</span></span>
- <span data-ttu-id="7261c-147">Açık koleksiyonlar ilkesi oluşturun.</span><span class="sxs-lookup"><span data-stu-id="7261c-147">Establish a clear collections policy.</span></span> <span data-ttu-id="7261c-148">Koleksiyonlar işleminizi ayrıntılandırın ve aboneliklerde erişim ne zaman ödemesiz olarak etkilenecektir.</span><span class="sxs-lookup"><span data-stu-id="7261c-148">Detail your collections process and when access to subscriptions will be impacted by non-payment.</span></span> <span data-ttu-id="7261c-149">(Ödeme dışı [bir müşterinin aboneliğini](create-a-new-subscription.md#suspend-a-subscription) devre dışı bırakabilir veya askıya alabilirsiniz.)</span><span class="sxs-lookup"><span data-stu-id="7261c-149">(You can disable access or [suspend a customer's subscriptions](create-a-new-subscription.md#suspend-a-subscription) for non-payment.)</span></span>

### <a name="managing-customer-accounts"></a><span data-ttu-id="7261c-150">Müşteri hesaplarını yönetme</span><span class="sxs-lookup"><span data-stu-id="7261c-150">Managing customer accounts</span></span>

<span data-ttu-id="7261c-151">Müşteri hesaplarını yönetme önerileri satın alma sonrası şunları içerir:</span><span class="sxs-lookup"><span data-stu-id="7261c-151">Suggestions for managing customer accounts post-purchase include:</span></span>

- <span data-ttu-id="7261c-152">Microsoft bildirimlerini hızlıca alma, gözden geçirme, işlem yapması ve yanıt vermeye yönelik bir işlem uygulayın.</span><span class="sxs-lookup"><span data-stu-id="7261c-152">Implement a process to quickly receive, review, act on, and respond to Microsoft notifications.</span></span>
- <span data-ttu-id="7261c-153">Ayarlar uygun izleme eşiklerini yaparken, bulut kullanımı iş ihtiyaçlarını anlamak için müşterilerle birlikte çalışın.</span><span class="sxs-lookup"><span data-stu-id="7261c-153">Work with customers to understand their cloud usage business needs while settings appropriate monitoring thresholds.</span></span> <span data-ttu-id="7261c-154">(Örneğin, Iş Ortağı Merkezi 'nde [aylık bir Azure harcama bütçesi ayarlayabilirsiniz](set-an-azure-spending-budget-for-your-customers.md) .</span><span class="sxs-lookup"><span data-stu-id="7261c-154">(For example, you can [set a monthly Azure spending budget](set-an-azure-spending-budget-for-your-customers.md) in Partner Center.</span></span> <span data-ttu-id="7261c-155">Bu anlama, ay içinde müşteri kullanımını izlemenizi ve müşteriler bütçesine yakın olduğunda bildirim gönderilmesini sağlar.)</span><span class="sxs-lookup"><span data-stu-id="7261c-155">This understanding allows you to monitor customer usage during the month and be notified when customers are close to their budget.)</span></span>
- <span data-ttu-id="7261c-156">Dolandırıcılığın erken algılanmasına yardımcı olmak için [Müşteri etkinlik günlüklerini](activity-logs.md) düzenli olarak izleyin.</span><span class="sxs-lookup"><span data-stu-id="7261c-156">Monitor [customer activity logs](activity-logs.md) regularly to help detect fraud early.</span></span>
- <span data-ttu-id="7261c-157">Şüpheli etkinlikler algılandığında hızlı bir işlem yapın.</span><span class="sxs-lookup"><span data-stu-id="7261c-157">Take quick action when suspicious activities are detected.</span></span>
- <span data-ttu-id="7261c-158">Müşterilerin, risk azaltma denetimlerini uygulamadan aboneliğe tam yönetim erişimi vermekten kaçının.</span><span class="sxs-lookup"><span data-stu-id="7261c-158">Avoid giving customers full administrative access to subscriptions without first implementing risk mitigation controls.</span></span>

### <a name="managing-customer-billing"></a><span data-ttu-id="7261c-159">Müşteri faturalandırmasını yönetme</span><span class="sxs-lookup"><span data-stu-id="7261c-159">Managing customer billing</span></span>

<span data-ttu-id="7261c-160">Müşteri faturalandırma sonrası satın alma için öneriler şunları içerir:</span><span class="sxs-lookup"><span data-stu-id="7261c-160">Suggestions for managing customer billing post-purchase include:</span></span>

- <span data-ttu-id="7261c-161">İlk işlem ve faturalandırma öncesinde ön ödeme isteği.</span><span class="sxs-lookup"><span data-stu-id="7261c-161">Request prepayments prior to initial transactions and billing.</span></span>
- <span data-ttu-id="7261c-162">Yüksek riskli ödeme gereçleri (ön ödemeli kartlar veya depolanan değer kartları gibi) kabul etmeyin.</span><span class="sxs-lookup"><span data-stu-id="7261c-162">Don't accept high-risk payment instruments (such as pre-paid cards or stored-value cards).</span></span>
- <span data-ttu-id="7261c-163">Müşteri ödemelerini ve yaşlandırma hesaplarının alacakları izleyin.</span><span class="sxs-lookup"><span data-stu-id="7261c-163">Monitor customer payments and aging accounts receivables.</span></span> <span data-ttu-id="7261c-164">Geç ödemeler veya ödeme yapılmadığı için standartlaştırılmış hatırlatarak süreçlerini zorlayacağı.</span><span class="sxs-lookup"><span data-stu-id="7261c-164">Aggressively enforce standardized dunning processes for late payments or non-payment.</span></span>

<span data-ttu-id="7261c-165">Çevrimiçi riski azaltmaya yönelik daha ayrıntılı stratejiler için [çevrimiçi işlem risk yönetimi kılavuzuna bakın.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)</span><span class="sxs-lookup"><span data-stu-id="7261c-165">For more detailed strategies for mitigating online risk, see the [Online transaction risk management guide.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)</span></span>
