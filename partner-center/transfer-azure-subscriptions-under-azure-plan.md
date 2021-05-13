---
title: Azure planı altındaki Azure aboneliğini başka bir CSP iş ortağına aktarma
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Müşterinin Azure abonelikleriyle ilişkili Bulut Çözümü Sağlayıcısı program iş ortağını azure planı kapsamında değiştirme hakkında bilgi edinin.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: dcacc6da51fe40c7eb05997f5409ef5fadbcf693
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856058"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="4d59e-103">Müşterinin Azure planı aboneliklerini farklı bir iş ortağına aktarma</span><span class="sxs-lookup"><span data-stu-id="4d59e-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="4d59e-104">**Uygun roller:** Hesap yöneticisi | Satış aracısı | Faturalama aracısı</span><span class="sxs-lookup"><span data-stu-id="4d59e-104">**Appropriate roles**: Account admin | Sales agent | Billing agent</span></span>

<span data-ttu-id="4d59e-105">Bu makalede bir müşterinin azure planı kapsamındaki Azure aboneliklerini bir abonelikten (CSP) Bulut Çözümü Sağlayıcısı nasıl değiştirip başka bir azure aboneliğine geçebilirsiniz?</span><span class="sxs-lookup"><span data-stu-id="4d59e-105">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="4d59e-106">Farklı bir iş ortağından müşterinin Azure aboneliklerini değiştirmek için aşağıdaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="4d59e-106">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="4d59e-107">Hem iş ortağının hem de müşterinin tamamlaması gereken adımları var.</span><span class="sxs-lookup"><span data-stu-id="4d59e-107">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="4d59e-108">Geçiş aracına yalnızca Microsoft ile doğrudan faturalama ilişkisi olan iş ortakları erişebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4d59e-108">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="4d59e-109">Dolaylı Kurumsal Bayilerin bu geçiş aracından yararlanılması için Dolaylı Sağlayıcılarıyla birlikte çalışması gerekir.</span><span class="sxs-lookup"><span data-stu-id="4d59e-109">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="4d59e-110">Bu araç kullanılana kadar müşterinin her iki iş ortağıyla (güncel ve gelecek) konuşmada olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="4d59e-110">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="4d59e-111">Karışıklığı ve karışıklığı önlemek için çevrimdışı bir konuşma yapılması gerekir.</span><span class="sxs-lookup"><span data-stu-id="4d59e-111">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="4d59e-112">Ayrıca, iş ortakları ve müşteriler bir geçişi başlatan önce bu konuları ve önkoşulları anlamalı:</span><span class="sxs-lookup"><span data-stu-id="4d59e-112">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="4d59e-113">**Dikkat edilmesi gereken önemli noktalar:**</span><span class="sxs-lookup"><span data-stu-id="4d59e-113">**Key considerations:**</span></span>

- <span data-ttu-id="4d59e-114">Azure Rezervasyonları abonelikle birlikte gelecekteki iş ortağına taşınmayacak</span><span class="sxs-lookup"><span data-stu-id="4d59e-114">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="4d59e-115">Geçerli iş ortağı altındaki Azure hizmetleri için CSP fiyatlandırması geçiş olmaz</span><span class="sxs-lookup"><span data-stu-id="4d59e-115">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="4d59e-116">Müşteri için destek sorumlulukları gelecekteki iş ortağına taşınacak</span><span class="sxs-lookup"><span data-stu-id="4d59e-116">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="4d59e-117">Faturalama, aktarım zamanında gelecekteki iş ortağına taşınacak</span><span class="sxs-lookup"><span data-stu-id="4d59e-117">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="4d59e-118">Azure Role-Based Access Control (RBAC) aktarımdan etkilenmez</span><span class="sxs-lookup"><span data-stu-id="4d59e-118">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="4d59e-119">Yönetici Adına (AOBO) varsayılan olarak gelecekteki iş ortağına verilmez</span><span class="sxs-lookup"><span data-stu-id="4d59e-119">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="4d59e-120">Üçüncü taraf market ürünleri, ürünler Market uygunluk denetimine geçeceği sürece aktaracak.</span><span class="sxs-lookup"><span data-stu-id="4d59e-120">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="4d59e-121">Özel indirimler veya bölgesel kısıtlamalar yoktur</span><span class="sxs-lookup"><span data-stu-id="4d59e-121">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="4d59e-122">Ürünler abonelik tabanlı değil</span><span class="sxs-lookup"><span data-stu-id="4d59e-122">The products are non-subscription based</span></span>
    - <span data-ttu-id="4d59e-123">Gelecekteki iş ortağı, ürünün dağıtımına izin verme listesinde olduğundan emin olmak için yayımcıyla birlikte çalışmalı</span><span class="sxs-lookup"><span data-stu-id="4d59e-123">The future partner should work with the publisher to make sure they are on the allow list for deployment of the product</span></span>
    - <span data-ttu-id="4d59e-124">Market ürünlerinin aktarımı için bu koşulların hepsi karşılanmazsa, Azure abonelikleri aktarıldı ve ardından Market ürünlerini yeni iş ortağıyla yeniden satın alma</span><span class="sxs-lookup"><span data-stu-id="4d59e-124">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="4d59e-125">**Ön koşullar:**</span><span class="sxs-lookup"><span data-stu-id="4d59e-125">**Prerequisites:**</span></span>

- <span data-ttu-id="4d59e-126">Müşteri, geçiş amacına bağlı olarak mevcut CSP iş ortağıyla etkileşime geç</span><span class="sxs-lookup"><span data-stu-id="4d59e-126">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="4d59e-127">Gelecekteki CSP iş ortağı müşteriyle birlikte çalışır ve müşteri ihtiyaçlarının karşılanamaması için</span><span class="sxs-lookup"><span data-stu-id="4d59e-127">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="4d59e-128">Gelecekteki CSP iş ortağı müşteriyle bir ilişki kuracak ve geçiş başlamadan önce bir Azure planı satın alır</span><span class="sxs-lookup"><span data-stu-id="4d59e-128">Future CSP partner establishes a relationship with customer and purchases an Azure plan before the transition begins</span></span>  
- <span data-ttu-id="4d59e-129">Müşterinin gelecekteki CSP Microsoft Müşteri Sözleşmesi oturum açması gerekir</span><span class="sxs-lookup"><span data-stu-id="4d59e-129">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="4d59e-130">Gelecekteki CSP iş ortağının bu aracı Microsoft İş Ortağı Sözleşmesi için iş ortağını imzalamış olması gerekir</span><span class="sxs-lookup"><span data-stu-id="4d59e-130">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="4d59e-131">Tamamlanması gereken müşteri görevleri</span><span class="sxs-lookup"><span data-stu-id="4d59e-131">Customer tasks to be completed</span></span>

<span data-ttu-id="4d59e-132">Azure planı kapsamındaki bir Azure aboneliğini aktarması için müşterinin geçerli iş ortağıyla iletişime geçerek süreci başlatması gerekir.</span><span class="sxs-lookup"><span data-stu-id="4d59e-132">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="4d59e-133">Gelecekteki iş ortaklarının kendi adına aktarım isteği formunu tamamlayamaları için geçerli iş ortağının şirket adını ve etki alanını toplaması gerekir.</span><span class="sxs-lookup"><span data-stu-id="4d59e-133">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="4d59e-134">Müşterinin ayrıca geçerli iş ortağından aktarma yapmak istediğiniz abonelikleri tanımlaması gerekir.</span><span class="sxs-lookup"><span data-stu-id="4d59e-134">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="4d59e-135">Office 365, Enterprise Mobility Suite veya Microsoft Dynamics CRM abonelikleri için iş ortaklarını değiştiremezsiniz.</span><span class="sxs-lookup"><span data-stu-id="4d59e-135">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="4d59e-136">Aktarım işlemini başlatan aktarım isteği formunu tamamlamak gelecekteki iş ortağının sorumluluğundadır.</span><span class="sxs-lookup"><span data-stu-id="4d59e-136">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="4d59e-137">Microsoft müşteri veya geçerli iş ortağı adına müdahalede bulunamaz.</span><span class="sxs-lookup"><span data-stu-id="4d59e-137">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="4d59e-138">Müşterinin, geçişi sorunsuz bir şekilde devam etmek için gelecekteki ve mevcut iş ortağıyla yakın bir çalışma planlaması gerekir.</span><span class="sxs-lookup"><span data-stu-id="4d59e-138">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="4d59e-139">Gelecekteki iş ortağı görevleri tamamlanacak</span><span class="sxs-lookup"><span data-stu-id="4d59e-139">Future partner tasks to be completed</span></span>

<span data-ttu-id="4d59e-140">Aboneliğin gelecekteki iş ortağının abonelik aktarımı isteği için İş Ortağı Merkezi aktarım isteği formunu tamamlaması gerekir:</span><span class="sxs-lookup"><span data-stu-id="4d59e-140">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="4d59e-141">Bu İş Ortağı Merkezi **Müşteriler'i** seçin ve ardından adına bir aktarım isteği formunu tamamlamak istediğiniz müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="4d59e-141">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="4d59e-142">Müşteri menüsünden **abonelikler**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="4d59e-142">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="4d59e-143">**Aktarım isteği** bölümünü seçin.</span><span class="sxs-lookup"><span data-stu-id="4d59e-143">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="4d59e-144">**Aktarım isteği bölümünden** **yeni istek ekle**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="4d59e-144">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Aktarımlar bölümü":::

5.  <span data-ttu-id="4d59e-146">**Yeni aktarım isteği** formunu doldurun.</span><span class="sxs-lookup"><span data-stu-id="4d59e-146">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="4d59e-147">**Gönderme aktarım isteği** Gönder ' i seçin  >  .</span><span class="sxs-lookup"><span data-stu-id="4d59e-147">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Aktarım isteği formunu doldurun":::

7.  <span data-ttu-id="4d59e-149">Aktarım isteği onayını gözden geçirme</span><span class="sxs-lookup"><span data-stu-id="4d59e-149">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Bekleyen aktarımı gözden geçirme":::

    >[!Note]
    ><span data-ttu-id="4d59e-151">Gelecekteki iş ortağı, yalnızca aktarım isteği durumu "bekliyor" olduğunda sağ üst köşede bulunan **isteği iptal** et ' i seçerek aktarım isteğini iptal edebilir.</span><span class="sxs-lookup"><span data-stu-id="4d59e-151">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="4d59e-152">Aktarım isteği durumu "sürüyor" veya "Tamam" olduktan sonra, iptaller mümkün olmayacaktır.</span><span class="sxs-lookup"><span data-stu-id="4d59e-152">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="4d59e-153">Tamamlanacak geçerli iş ortağı görevleri</span><span class="sxs-lookup"><span data-stu-id="4d59e-153">Current partner tasks to be completed</span></span>

<span data-ttu-id="4d59e-154">Geçerli iş ortağının müşterinin Yönetim Aracısı, müşterilerinin aboneliklerinin aktarımını istediğini belirten bir e-posta alır:</span><span class="sxs-lookup"><span data-stu-id="4d59e-154">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Gözden geçirme":::

<span data-ttu-id="4d59e-156">Abonelik aktarımını gerçekleştirmek için Iş Ortağı Merkezi 'nden aktarma isteği formunu gözden geçirin ve kabul edin.</span><span class="sxs-lookup"><span data-stu-id="4d59e-156">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="4d59e-157">Geçerli iş ortağı tarafından 30 gün içinde herhangi bir eylem yapılmaz, isteğin süresi sona erer ve gelecekteki iş ortağı yeni bir aktarım isteği oluşturmak için bir öğesine sahip olur.</span><span class="sxs-lookup"><span data-stu-id="4d59e-157">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="4d59e-158">E-postadaki veya **Aktarım Isteğini gözden geçirin** ' i seçin</span><span class="sxs-lookup"><span data-stu-id="4d59e-158">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="4d59e-159">Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve ardından bir aktarım isteğinin adına gönderildiği müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="4d59e-159">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="4d59e-160">Müşteri menüsünden **abonelikler**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="4d59e-160">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="4d59e-161">**Aktarım isteği** bölümünü seçin.</span><span class="sxs-lookup"><span data-stu-id="4d59e-161">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="4d59e-162">**Alınan istekler** altında seçilen **aktarım isteği kimliğini** seçerek aktarım bilgilerini genişletin</span><span class="sxs-lookup"><span data-stu-id="4d59e-162">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Kaynak incelemeleri aktarım isteği":::

5.  <span data-ttu-id="4d59e-164">Aktarım isteğini gözden geçirme.</span><span class="sxs-lookup"><span data-stu-id="4d59e-164">Review transfer request.</span></span> <span data-ttu-id="4d59e-165">Aktarımın istenen Azure aboneliklerini seçin.</span><span class="sxs-lookup"><span data-stu-id="4d59e-165">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="4d59e-166">Devam etmeden önce lütfen unutmayın: Artık seçili aboneliklere erişemeyeceksiniz.</span><span class="sxs-lookup"><span data-stu-id="4d59e-166">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="4d59e-167">Daha fazla kullanım için faturalanmaz.</span><span class="sxs-lookup"><span data-stu-id="4d59e-167">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="4d59e-168">Azure rezervasyonları aboneliklerle birlikte aktarlanmaz.</span><span class="sxs-lookup"><span data-stu-id="4d59e-168">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="4d59e-169">Ardından, **aktarım işlemini tamamlamak için Kabul** et ve aktar'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="4d59e-169">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Azure planlarınızı kullanarak aktarıla abonelikleri seçin":::

7.  <span data-ttu-id="4d59e-171">Aktarım kabul onaylarını görüntüleme.</span><span class="sxs-lookup"><span data-stu-id="4d59e-171">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="4d59e-172">Bu noktada, gelecekteki iş ortağı, müşteri ve geçerli iş ortağı, kabul edilen aktarım isteğine e-posta ile bildirilecek.</span><span class="sxs-lookup"><span data-stu-id="4d59e-172">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="4d59e-173">Geçiş kabul edildikten sonra, sistem güncelleştirilirken aktarım durumu 15 dakika kadar Beklemede kalabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4d59e-173">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="4d59e-174">Daha uzun sürerse, sistem üç gün boyunca bunu yapmaya devam ediyor olur.</span><span class="sxs-lookup"><span data-stu-id="4d59e-174">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="4d59e-175">Aktarım durumu hala Beklemede olarak kalırsa, iş ortağı bir hizmet isteği göndermektedir.</span><span class="sxs-lookup"><span data-stu-id="4d59e-175">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="4d59e-176">Aktarım tamamlandıktan sonra, istekte yer alan abonelikler gelecekteki iş ortağının Azure planında görünür ve artık sizin için listelenmiyor.</span><span class="sxs-lookup"><span data-stu-id="4d59e-176">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="4d59e-177">Dolaylı Sağlayıcılar için: Lütfen Dolaylı Kurumsal Bayinize aktarım isteğinin kabul olduğunu bildirin.</span><span class="sxs-lookup"><span data-stu-id="4d59e-177">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="4d59e-178">Aktarılan müşteri aboneliklerinizi yönetme</span><span class="sxs-lookup"><span data-stu-id="4d59e-178">Managing your transferred customer subscriptions</span></span>

- <span data-ttu-id="4d59e-179">Bu geçiş, Azure rol tabanlı erişim denetimi (RBAC) kullanılarak atanan mevcut kullanıcı, grup ve hizmet sorumlularını etkilemez.</span><span class="sxs-lookup"><span data-stu-id="4d59e-179">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="4d59e-180">Azure rol tabanlı erişim denetimi [(Azure RBAC),](/azure/role-based-access-control/overview) müşterinizin Azure kaynaklarına kimlerin erişimi olduğunu, bu kaynaklarla neler yapalarını ve erişim sahip olduğu alanları yönetmelerine yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="4d59e-180">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="4d59e-181">Yeni iş ortağı olarak, abonelik aktarımı sonrasında müşterinizin kaynaklarına RBAC erişimi verilmez.</span><span class="sxs-lookup"><span data-stu-id="4d59e-181">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="4d59e-182">Müşterinizin önceki iş ortağı RBAC erişimini korur.</span><span class="sxs-lookup"><span data-stu-id="4d59e-182">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="4d59e-183">Abonelikleri hakkında kimlerin içgörüleri olduğunu ve istediği değişiklikleri nasıl yapacaklarını anlamak için müşteriyle birlikte çalışabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4d59e-183">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="4d59e-184">Sonuç olarak, müşterinizin Azure RBAC erişimini önceki iş ortakları için kaldırmasının yanı sıra yeni iş ortağı için de erişim eklemesi önemlidir.</span><span class="sxs-lookup"><span data-stu-id="4d59e-184">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="4d59e-185">Müşteriniz hakkında yeni erişim verme hakkında daha fazla bilgi için bkz. [Azure rol tabanlı erişim denetimi (Azure RBAC) nedir?](/azure/role-based-access-control/overview)</span><span class="sxs-lookup"><span data-stu-id="4d59e-185">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="4d59e-186">Önceki iş ortağınızın RBAC erişimini kaldırma müşteriniz hakkında daha fazla bilgi için bkz. [rol atamasını kaldırma](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span><span class="sxs-lookup"><span data-stu-id="4d59e-186">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="4d59e-187">Ayrıca, aboneliklerinize otomatik olarak [yönetici (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) erişimi de kalmaz.</span><span class="sxs-lookup"><span data-stu-id="4d59e-187">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="4d59e-188">AOININ, iş ortağının müşterilerinin Azure aboneliklerini kendi adına yönetmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="4d59e-188">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="4d59e-189">Azure ayrıcalıkları hakkında daha fazla bilgi için bkz [. bir müşterinin hizmetini veya aboneliğini yönetmek için Izinleri alma.](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="4d59e-189">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="4d59e-190">Sonraki adımlar:</span><span class="sxs-lookup"><span data-stu-id="4d59e-190">Next steps:</span></span>

- [<span data-ttu-id="4d59e-191">(Azure RBAC)</span><span class="sxs-lookup"><span data-stu-id="4d59e-191">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="4d59e-192">Müşterinin hizmetini veya aboneliğini yönetme izinleri alın.</span><span class="sxs-lookup"><span data-stu-id="4d59e-192">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
