---
title: Azure aboneliğini bir Azure planına göre başka bir CSP ortağına aktarma
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Bir Azure planı kapsamındaki müşterinin Azure abonelikleriyle ilişkili bulut çözümü sağlayıcısı program ortağını nasıl değiştireceğinizi öğrenin.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: 092c76fb874eb7308bdb69503223f722657db957
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277326"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="ccd64-103">Müşterinin Azure planı aboneliklerini farklı bir ortağa aktarma</span><span class="sxs-lookup"><span data-stu-id="ccd64-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="ccd64-104">**Uygun roller**: Hesap Yöneticisi | Satış Aracısı | Faturalandırma Aracısı</span><span class="sxs-lookup"><span data-stu-id="ccd64-104">**Appropriate roles**: Account admin | Sales agent | Billing agent</span></span>

<span data-ttu-id="ccd64-105">Bu makalede, bir müşterinin Azure planına ait Azure aboneliklerinin bir bulut çözümü sağlayıcısından (CSP) diğerine nasıl geçbir şekilde değiştirileceği açıklanır.</span><span class="sxs-lookup"><span data-stu-id="ccd64-105">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="ccd64-106">Müşterinin Azure aboneliklerini farklı bir iş ortağından geçirmek için aşağıdaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="ccd64-106">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="ccd64-107">Hem iş ortağının hem de müşterinin tamamlanma adımları vardır.</span><span class="sxs-lookup"><span data-stu-id="ccd64-107">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="ccd64-108">Yalnızca Microsoft ile doğrudan faturalandırma ilişkisine sahip iş ortakları geçiş araçlarına erişebilir.</span><span class="sxs-lookup"><span data-stu-id="ccd64-108">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="ccd64-109">Bu geçiş aracından yararlanmak için dolaylı satıcıların dolaylı sağlayıcılarıyla birlikte çalışması gerekir.</span><span class="sxs-lookup"><span data-stu-id="ccd64-109">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="ccd64-110">Müşteri, bu araç yararlanılabilir önceki iş ortakları (geçerli ve gelecekteki) ile birlikte konuşmada olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="ccd64-110">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="ccd64-111">Karışıklık ve karmaşıklığın oluşmaması için çevrimdışı bir konuşma olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="ccd64-111">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="ccd64-112">Ayrıca, iş ortakları ve müşteriler bir geçişi başlatmadan önce bu konuları ve önkoşulları anlamalıdır:</span><span class="sxs-lookup"><span data-stu-id="ccd64-112">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="ccd64-113">**Önemli noktalar:**</span><span class="sxs-lookup"><span data-stu-id="ccd64-113">**Key considerations:**</span></span>

- <span data-ttu-id="ccd64-114">Azure ayırmaları gelecek iş ortağına abonelikle birlikte taşınmayacak</span><span class="sxs-lookup"><span data-stu-id="ccd64-114">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="ccd64-115">Geçerli iş ortağı kapsamındaki Azure hizmetleri için CSP fiyatlandırması geçiş olmayacak</span><span class="sxs-lookup"><span data-stu-id="ccd64-115">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="ccd64-116">Müşteri için destek sorumlulukları gelecek iş ortağına taşınır</span><span class="sxs-lookup"><span data-stu-id="ccd64-116">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="ccd64-117">Faturalandırma ve faturalama, aktarım sırasında gelecek iş ortağına taşınır</span><span class="sxs-lookup"><span data-stu-id="ccd64-117">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="ccd64-118">Azure Role-Based Access Control (RBAC) aktarımdan etkilenmiyor</span><span class="sxs-lookup"><span data-stu-id="ccd64-118">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="ccd64-119">(AOBO) adına yönetici, gelecek iş ortağı için varsayılan olarak verilmeyecektir</span><span class="sxs-lookup"><span data-stu-id="ccd64-119">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="ccd64-120">Ürünler Market uygunluk denetimini geçirmiş olduğu sürece, üçüncü taraf Market ürünleri aktarılır.</span><span class="sxs-lookup"><span data-stu-id="ccd64-120">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="ccd64-121">Özel indirimler veya bölgesel kısıtlama yoktur</span><span class="sxs-lookup"><span data-stu-id="ccd64-121">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="ccd64-122">Ürünler, abonelik olmayan tabanlı</span><span class="sxs-lookup"><span data-stu-id="ccd64-122">The products are non-subscription based</span></span>
    - <span data-ttu-id="ccd64-123">Gelecekteki iş ortağı, ürün dağıtımı için izin verilenler listesinde olduklarından emin olmak için Yayımcısıyla birlikte çalışmalıdır</span><span class="sxs-lookup"><span data-stu-id="ccd64-123">The future partner should work with the publisher to make sure they are on the allow list for deployment of the product</span></span>
    - <span data-ttu-id="ccd64-124">Market ürünlerinin aktarılması için bu koşulların tümü karşılanmazsa, Azure abonelikleri aktarılmalı ve yeni iş ortağıyla Market ürünlerinin yeniden oluşturulması gerekir</span><span class="sxs-lookup"><span data-stu-id="ccd64-124">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="ccd64-125">**Ön koşullar:**</span><span class="sxs-lookup"><span data-stu-id="ccd64-125">**Prerequisites:**</span></span>

- <span data-ttu-id="ccd64-126">Müşteri, geçerli CSP iş ortaklarının geçiş amacını karşılamalarını sağlar</span><span class="sxs-lookup"><span data-stu-id="ccd64-126">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="ccd64-127">Gelecekteki CSP iş ortağı müşteri gereksinimlerinin karşılanabileceği sağlamak için müşteriyle birlikte çalışarak</span><span class="sxs-lookup"><span data-stu-id="ccd64-127">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="ccd64-128">Gelecekteki CSP iş ortağı, müşteri ile bir ilişki kurar ve geçiş başlamadan önce bir Azure planı satın alır</span><span class="sxs-lookup"><span data-stu-id="ccd64-128">Future CSP partner establishes a relationship with customer and purchases an Azure plan before the transition begins</span></span>  
- <span data-ttu-id="ccd64-129">Müşteri, gelecek CSP ortağıyla Microsoft Müşteri anlaşmasını imzalayamalıdır</span><span class="sxs-lookup"><span data-stu-id="ccd64-129">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="ccd64-130">Gelecekteki CSP iş ortağı bu aracı kullanmak için Microsoft Iş ortağı sözleşmesi 'Ni imzalamalıdır</span><span class="sxs-lookup"><span data-stu-id="ccd64-130">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="ccd64-131">Tamamlanacak müşteri görevleri</span><span class="sxs-lookup"><span data-stu-id="ccd64-131">Customer tasks to be completed</span></span>

<span data-ttu-id="ccd64-132">Bir Azure planı kapsamında bir Azure aboneliğini aktarmak için, müşterinin geçerli iş ortağıyla iletişim kurarak işlemi başlatması gerekir.</span><span class="sxs-lookup"><span data-stu-id="ccd64-132">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="ccd64-133">Gelecekteki iş ortaklarının kendi adına aktarım isteği formunu tamamlayabilmeleri için, geçerli iş ortağının şirket adını ve etki alanını toplamaları gerekir.</span><span class="sxs-lookup"><span data-stu-id="ccd64-133">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="ccd64-134">Müşterinin ayrıca geçerli iş ortağından aktarmak istedikleri abonelikleri tanımlaması gerekir.</span><span class="sxs-lookup"><span data-stu-id="ccd64-134">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="ccd64-135">Office 365, Enterprise Mobility Suite veya Microsoft Dynamics CRM abonelikleri için iş ortaklarını değiştiremezsiniz.</span><span class="sxs-lookup"><span data-stu-id="ccd64-135">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="ccd64-136">Aktarım sürecini başlatan aktarım isteği formunu tamamlamaya yönelik gelecek iş ortağının sorumluluğundadır.</span><span class="sxs-lookup"><span data-stu-id="ccd64-136">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="ccd64-137">Microsoft, müşteri veya geçerli iş ortağı adına müdahale edemez.</span><span class="sxs-lookup"><span data-stu-id="ccd64-137">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="ccd64-138">Müşteri, geçişi sorunsuz bir şekilde hareket etmek için gelecekteki ve geçerli ortağıyla yakından çalışmayı planlıyor olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="ccd64-138">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="ccd64-139">Tamamlanacak sonraki iş ortağı görevleri</span><span class="sxs-lookup"><span data-stu-id="ccd64-139">Future partner tasks to be completed</span></span>

<span data-ttu-id="ccd64-140">Aboneliğin gelecek iş ortağının, abonelik aktarımı istemek için Iş Ortağı Merkezi 'nden bir aktarım isteği formunu tamamlaması gerekir:</span><span class="sxs-lookup"><span data-stu-id="ccd64-140">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="ccd64-141">Iş Ortağı Merkezi menüsünde, **müşteriler**' i seçin ve ardından bir aktarım isteği formunu gerçekleştirmek istediğiniz müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="ccd64-141">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="ccd64-142">Müşteri menüsünden **abonelikler**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="ccd64-142">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="ccd64-143">**Aktarım isteği** bölümünü seçin.</span><span class="sxs-lookup"><span data-stu-id="ccd64-143">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="ccd64-144">**Aktarım isteği bölümünden** **yeni istek ekle**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="ccd64-144">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Aktarımlar bölümü.":::

5.  <span data-ttu-id="ccd64-146">**Yeni aktarım isteği** formunu doldurun.</span><span class="sxs-lookup"><span data-stu-id="ccd64-146">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="ccd64-147">**Gönderme aktarım isteği** Gönder ' i seçin  >  .</span><span class="sxs-lookup"><span data-stu-id="ccd64-147">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Aktarım isteği formunu doldurun.":::

7.  <span data-ttu-id="ccd64-149">Aktarım isteği onayını gözden geçirme</span><span class="sxs-lookup"><span data-stu-id="ccd64-149">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Bekleyen aktarımı gözden geçirin.":::

    >[!Note]
    ><span data-ttu-id="ccd64-151">Gelecekteki iş ortağı, yalnızca aktarım isteği durumu "bekliyor" olduğunda sağ üst köşede bulunan **isteği iptal** et ' i seçerek aktarım isteğini iptal edebilir.</span><span class="sxs-lookup"><span data-stu-id="ccd64-151">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="ccd64-152">Aktarım isteği durumu "sürüyor" veya "Tamam" olduktan sonra, iptaller mümkün olmayacaktır.</span><span class="sxs-lookup"><span data-stu-id="ccd64-152">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="ccd64-153">Tamamlanacak geçerli iş ortağı görevleri</span><span class="sxs-lookup"><span data-stu-id="ccd64-153">Current partner tasks to be completed</span></span>

<span data-ttu-id="ccd64-154">Geçerli iş ortağının müşterinin Yönetim Aracısı, müşterilerinin aboneliklerinin aktarımını istediğini belirten bir e-posta alır:</span><span class="sxs-lookup"><span data-stu-id="ccd64-154">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="İncelemeyi.":::

<span data-ttu-id="ccd64-156">Abonelik aktarımını gerçekleştirmek için Iş Ortağı Merkezi 'nden aktarma isteği formunu gözden geçirin ve kabul edin.</span><span class="sxs-lookup"><span data-stu-id="ccd64-156">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="ccd64-157">Geçerli iş ortağı tarafından 30 gün içinde herhangi bir eylem yapılmaz, isteğin süresi sona erer ve gelecekteki iş ortağı yeni bir aktarım isteği oluşturmak için bir öğesine sahip olur.</span><span class="sxs-lookup"><span data-stu-id="ccd64-157">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="ccd64-158">E-postadaki veya **Aktarım Isteğini gözden geçirin** ' i seçin</span><span class="sxs-lookup"><span data-stu-id="ccd64-158">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="ccd64-159">Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve ardından bir aktarım isteğinin adına gönderildiği müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="ccd64-159">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="ccd64-160">Müşteri menüsünden **abonelikler**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="ccd64-160">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="ccd64-161">**Aktarım isteği** bölümünü seçin.</span><span class="sxs-lookup"><span data-stu-id="ccd64-161">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="ccd64-162">**Alınan istekler** altında seçilen **aktarım isteği kimliğini** seçerek aktarım bilgilerini genişletin</span><span class="sxs-lookup"><span data-stu-id="ccd64-162">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Kaynak, aktarım isteğini gözden geçirir.":::

5.  <span data-ttu-id="ccd64-164">Aktarım isteğini gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="ccd64-164">Review transfer request.</span></span> <span data-ttu-id="ccd64-165">Aktarılacak istenen Azure aboneliklerini seçin.</span><span class="sxs-lookup"><span data-stu-id="ccd64-165">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="ccd64-166">Devam etmeden önce lütfen unutmayın: seçili aboneliklere artık erişemeyecektir.</span><span class="sxs-lookup"><span data-stu-id="ccd64-166">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="ccd64-167">Daha fazla kullanım için faturalandırlanmayacaktır.</span><span class="sxs-lookup"><span data-stu-id="ccd64-167">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="ccd64-168">Azure ayırmaları, aboneliklerle aktarılmaz.</span><span class="sxs-lookup"><span data-stu-id="ccd64-168">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="ccd64-169">Ardından, aktarma işlemini gerçekleştirmek için **kabul et ve Aktar '** ı seçin.</span><span class="sxs-lookup"><span data-stu-id="ccd64-169">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Azure planlarınız altında aktarılacak abonelikleri seçin.":::

7.  <span data-ttu-id="ccd64-171">Aktarım kabulü onayını görüntüleyin.</span><span class="sxs-lookup"><span data-stu-id="ccd64-171">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="ccd64-172">Bu noktada, gelecek iş ortağı, müşteri ve geçerli iş ortağı, kabul edilen aktarım isteği ile e-posta üzerinden bildirilir.</span><span class="sxs-lookup"><span data-stu-id="ccd64-172">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="ccd64-173">Sonra, geçiş kabul edildikten sonra, sistem güncelleştirilirken aktarım durumu 15 dakikaya kadar beklemede kalabilir.</span><span class="sxs-lookup"><span data-stu-id="ccd64-173">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="ccd64-174">Daha uzun sürerse, sistem üç gün boyunca çalışmaya devam eder.</span><span class="sxs-lookup"><span data-stu-id="ccd64-174">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="ccd64-175">Aktarım durumu hala beklemede kalırsa, iş ortağı bir hizmet isteği göndermesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="ccd64-175">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="ccd64-176">Aktarım işlemi tamamlandıktan sonra, istek içine dahil edilen abonelikler gelecek iş ortağının Azure planında görüntülenir ve artık sizinle listelenmez.</span><span class="sxs-lookup"><span data-stu-id="ccd64-176">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="ccd64-177">Dolaylı sağlayıcılar için: lütfen dolaylı satıcınızla aktarım isteğinin kabul edildiğini bildirin.</span><span class="sxs-lookup"><span data-stu-id="ccd64-177">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="ccd64-178">Aktarılan müşteri aboneliklerinizi yönetme</span><span class="sxs-lookup"><span data-stu-id="ccd64-178">Managing your transferred customer subscriptions</span></span>

- <span data-ttu-id="ccd64-179">Bu geçiş, Azure rol tabanlı erişim denetimi (RBAC) kullanılarak atanan mevcut kullanıcı, grup ve hizmet sorumlularını etkilemez.</span><span class="sxs-lookup"><span data-stu-id="ccd64-179">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="ccd64-180">Azure rol tabanlı erişim denetimi [(Azure RBAC)](/azure/role-based-access-control/overview) , müşterinizin Azure kaynaklarına erişimi olan kişileri, bu kaynaklarla neler yapabileceğini ve hangi alanlara erişebileceğini yönetmesine yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="ccd64-180">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="ccd64-181">Yeni iş ortağı olarak, abonelik aktarımından sonra müşterinizin kaynaklarına herhangi bir RBAC erişimi verilmemiş.</span><span class="sxs-lookup"><span data-stu-id="ccd64-181">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="ccd64-182">Müşterinizin önceki iş ortağı RBAC erişimini korur.</span><span class="sxs-lookup"><span data-stu-id="ccd64-182">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="ccd64-183">Abonelikleriyle ilgili bir anlayış olduğunu ve istediğiniz değişiklikleri nasıl yapacağınızı anlamak için müşterinizden çalışın.</span><span class="sxs-lookup"><span data-stu-id="ccd64-183">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="ccd64-184">Sonuç olarak, müşterinizin Azure RBAC erişimini önceki iş ortakları için kaldırmasının yanı sıra yeni iş ortağı için de erişim eklemesi önemlidir.</span><span class="sxs-lookup"><span data-stu-id="ccd64-184">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="ccd64-185">Müşteriniz hakkında yeni erişim verme hakkında daha fazla bilgi için bkz. [Azure rol tabanlı erişim denetimi (Azure RBAC) nedir?](/azure/role-based-access-control/overview)</span><span class="sxs-lookup"><span data-stu-id="ccd64-185">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="ccd64-186">Önceki iş ortağınızın RBAC erişimini kaldırma müşteriniz hakkında daha fazla bilgi için bkz. [rol atamasını kaldırma](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span><span class="sxs-lookup"><span data-stu-id="ccd64-186">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="ccd64-187">Ayrıca, aboneliklerinize otomatik olarak [yönetici (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) erişimi de kalmaz.</span><span class="sxs-lookup"><span data-stu-id="ccd64-187">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="ccd64-188">AOININ, iş ortağının müşterilerinin Azure aboneliklerini kendi adına yönetmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="ccd64-188">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="ccd64-189">Azure ayrıcalıkları hakkında daha fazla bilgi için bkz [. bir müşterinin hizmetini veya aboneliğini yönetmek için Izinleri alma.](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="ccd64-189">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="ccd64-190">Sonraki adımlar:</span><span class="sxs-lookup"><span data-stu-id="ccd64-190">Next steps:</span></span>

- [<span data-ttu-id="ccd64-191">(Azure RBAC)</span><span class="sxs-lookup"><span data-stu-id="ccd64-191">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="ccd64-192">Müşterinin hizmetini veya aboneliğini yönetme izinleri alın.</span><span class="sxs-lookup"><span data-stu-id="ccd64-192">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
