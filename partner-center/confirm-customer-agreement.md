---
title: Müşterinizin, Microsoft Müşteri anlaşmasını CSP programına kabul ettiğini onaylama
description: Bulut çözümü sağlayıcısı (CSP) iş ortaklarının, müşteriler için Microsoft hizmetlerini sipariş etmeden önce Microsoft Müşteri sözleşmesinin müşteri tarafından kabul edilmesini onaylamanız gerekir.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: 9deebf3d9aab2d4dc7953da67a7eb17078b3d30c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277020"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a><span data-ttu-id="7d004-103">Müşterinizin, Microsoft Müşteri anlaşmasını CSP programına kabul ettiğini onaylama</span><span class="sxs-lookup"><span data-stu-id="7d004-103">How to confirm that your customer has accepted the Microsoft Customer Agreement to the CSP program</span></span>

<span data-ttu-id="7d004-104">**Uygun roller**: yönetici Aracısı | Satış Aracısı</span><span class="sxs-lookup"><span data-stu-id="7d004-104">**Appropriate roles**: Admin agent | Sales agent</span></span>


<span data-ttu-id="7d004-105">Müşterilerin, Microsoft Müşteri anlaşmasını kabul ettikleri iki seçeneği vardır.</span><span class="sxs-lookup"><span data-stu-id="7d004-105">Customers have two options for how they accept the Microsoft Customer Agreement.</span></span>

<span data-ttu-id="7d004-106">**Seçenek 1**: müşteri kabulünü kabul eden iş ortağı kanıtı Iş Ortağı Merkezi API/SDK kullanarak veya Iş Ortağı Merkezi panosu aracılığıyla müşteri kabulünü doğrulayabilirler.</span><span class="sxs-lookup"><span data-stu-id="7d004-106">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="7d004-107">**Seçenek 2**: müşteri doğrudan kabul-iş ortağı, Microsoft 365 Yönetim merkezinde sözleşmeyi gözden geçirmek ve kabul etmek IÇIN bir URL aracılığıyla müşteriyi davet edebilir.</span><span class="sxs-lookup"><span data-stu-id="7d004-107">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="7d004-108">Microsoft müşteri anlaşması şablonuna erişin</span><span class="sxs-lookup"><span data-stu-id="7d004-108">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="7d004-109">Microsoft müşteri anlaşması şablonunun en son sürümünü [buradan](https://aka.ms/customeragreement)el ile indirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7d004-109">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="7d004-110">Microsoft Müşteri Sözleşmesi ülkeye özeldir.</span><span class="sxs-lookup"><span data-stu-id="7d004-110">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="7d004-111">Microsoft müşteri anlaşması şablonunu istenirken, müşterinin konumuna göre doğru ülkeyi seçtiğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="7d004-111">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="7d004-112">Seçenek 1: Iş Ortağı Merkezi 'nde müşteri kabulünü onaylayın</span><span class="sxs-lookup"><span data-stu-id="7d004-112">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="7d004-113">Doğrudan fatura ortakları, yeni ve mevcut müşteriler için Iş Ortağı Merkezi 'nde Microsoft Müşteri sözleşmesinin müşteri tarafından kabul edildiğini doğrulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7d004-113">Direct bill partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="7d004-114">Dolaylı satıcılar müşterilerinin adına test edemez ve kanıtlama tamamlandı olarak kendi dolaylı sağlayıcısıyla birlikte çalışmalıdır.</span><span class="sxs-lookup"><span data-stu-id="7d004-114">Indirect resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="7d004-115">Yeni müşteriler için müşteri kabulünü Onayla</span><span class="sxs-lookup"><span data-stu-id="7d004-115">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="7d004-116">Iş Ortağı Merkezi 'nde yeni bir müşteri kiracısı oluşturduğunuzda, müşterinin Microsoft Müşteri sözleşmesinin kabul edildiğini onaylamak için aşağıdaki adımları kullanın.</span><span class="sxs-lookup"><span data-stu-id="7d004-116">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="7d004-117">Bu adımları gerçekleştirmek için bir yönetici Aracısı veya satış aracısı olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="7d004-117">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="7d004-118">**Müşteriler**' i ve ardından **yeni müşteri**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="7d004-118">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="7d004-119">**Hesap bilgileri** altında şirketin ve birincil kişisinin bilgilerini girin.</span><span class="sxs-lookup"><span data-stu-id="7d004-119">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="7d004-120">**Microsoft sözleşmesi**' nin altında, müşterinin Microsoft Müşteri anlaşmasını kabul etmiş olduğunu doğrulamak için kutuyu seçin.</span><span class="sxs-lookup"><span data-stu-id="7d004-120">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="7d004-121">**Sözleşme kabul tarihi** altında, uygun tarihi girin.</span><span class="sxs-lookup"><span data-stu-id="7d004-121">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="7d004-122">Bunu gelecekteki bir tarihle ayarlayamazsınız.</span><span class="sxs-lookup"><span data-stu-id="7d004-122">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="7d004-123">Görüntülenen birincil kullanıcı iletişim bilgilerinin doğru olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="7d004-123">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="7d004-124">Yanlış ise **Güncelleştir** ' i seçin ve sözleşmeyi kabul eden kişi için doğru bilgileri girin.</span><span class="sxs-lookup"><span data-stu-id="7d004-124">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="7d004-125">Müşteri kiracısını oluşturmaya devam etmek için **İleri ' yi** seçin.</span><span class="sxs-lookup"><span data-stu-id="7d004-125">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Yeni müşteri.":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="7d004-127">Mevcut müşteriler için müşteri kabulünü Onayla</span><span class="sxs-lookup"><span data-stu-id="7d004-127">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="7d004-128">Bunu yapmak için bir Yönetim Aracısı veya satış aracısı olmanız gerekir:</span><span class="sxs-lookup"><span data-stu-id="7d004-128">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="7d004-129">**Müşteriler**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="7d004-129">Select **Customers**.</span></span> <span data-ttu-id="7d004-130">Müşteriyi bulun ve seçin.</span><span class="sxs-lookup"><span data-stu-id="7d004-130">Find and select the customer.</span></span>

2. <span data-ttu-id="7d004-131">**Hesap bilgilerini** seçin.</span><span class="sxs-lookup"><span data-stu-id="7d004-131">Select **Account info**.</span></span>

3. <span data-ttu-id="7d004-132">**Microsoft Müşteri Sözleşmesi** altında **Güncelleştir**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="7d004-132">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="7d004-133">Sözleşmeyi kabul eden kişinin **adı**, **Soyadı**, **e-posta adresi** ve **telefon numarasını** (isteğe bağlı) girin.</span><span class="sxs-lookup"><span data-stu-id="7d004-133">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="7d004-134">**Sözleşme kabul tarihi** altında, uygun tarihi girin.</span><span class="sxs-lookup"><span data-stu-id="7d004-134">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="7d004-135">Bunu gelecekteki bir tarihle ayarlayamazsınız.</span><span class="sxs-lookup"><span data-stu-id="7d004-135">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="7d004-136">**Kaydet** ve devam et ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="7d004-136">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="Mevcut müşteri.":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="7d004-138">Müşteri kabulü onayını al</span><span class="sxs-lookup"><span data-stu-id="7d004-138">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="7d004-139">Mevcut bir müşterinin Microsoft Müşteri anlaşmasını kabul etmiş olduğunu onaylamak için aşağıdaki adımları kullanın.</span><span class="sxs-lookup"><span data-stu-id="7d004-139">To retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement, use the following steps.</span></span> <span data-ttu-id="7d004-140">Bunu yapmak için bir Yönetim Aracısı veya satış aracısı olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="7d004-140">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="7d004-141">**Müşteriler**' i seçin ve ardından görmek istediğiniz müşteriyi bulun ve seçin.</span><span class="sxs-lookup"><span data-stu-id="7d004-141">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="7d004-142">**Hesap bilgilerini** seçin.</span><span class="sxs-lookup"><span data-stu-id="7d004-142">Select **Account info**.</span></span>

3. <span data-ttu-id="7d004-143">**Microsoft Müşteri Sözleşmesi**' nin altında, bu müşteri tarafından onay olup olmadığını veya bu müşteri tarafından sağlanmadığını görüntüleyin.</span><span class="sxs-lookup"><span data-stu-id="7d004-143">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="7d004-144">Iş Ortağı Merkezi API/SDK kullanarak müşteri kabulünü onaylama</span><span class="sxs-lookup"><span data-stu-id="7d004-144">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="7d004-145">Iş Ortağı Merkezi API/SDK 'sını, Microsoft Müşteri sözleşmesinin müşteri tarafından kabul edildiğini onaylamak için kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7d004-145">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="7d004-146">API/SDK hakkında daha fazla bilgi için bkz:</span><span class="sxs-lookup"><span data-stu-id="7d004-146">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="7d004-147">Microsoft Müşteri Sözleşmesi için anlaşma meta verilerini alma</span><span class="sxs-lookup"><span data-stu-id="7d004-147">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="7d004-148">Microsoft Müşteri Sözleşmesinin müşteri kabulünü onaylama</span><span class="sxs-lookup"><span data-stu-id="7d004-148">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="7d004-149">Microsoft Müşteri Sözleşmesinin müşteri kabulünün onayını alma</span><span class="sxs-lookup"><span data-stu-id="7d004-149">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="7d004-150">Microsoft müşteri anlaşması şablonu için bir indirme bağlantısı alın</span><span class="sxs-lookup"><span data-stu-id="7d004-150">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="7d004-151">Seçenek 2: Microsoft 365 Yönetim merkezinde müşteri kabulü</span><span class="sxs-lookup"><span data-stu-id="7d004-151">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="7d004-152">İş ortakları yeni ve mevcut müşterileri bir URL aracılığıyla davet ederek Microsoft 365 Yönetim Merkezi 'ndeki sözleşmeyi gözden geçirebilir ve kabul edebilir.</span><span class="sxs-lookup"><span data-stu-id="7d004-152">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="7d004-153">Sonraki birkaç bölümde nasıl yapılacağı gösterilmektedir:</span><span class="sxs-lookup"><span data-stu-id="7d004-153">The next few sections show you how to:</span></span>

- <span data-ttu-id="7d004-154">Yeni bir müşteri oluşturun ve sözleşmeyi gözden geçirmek ve kabul etmek için müşteriyi davet edin.</span><span class="sxs-lookup"><span data-stu-id="7d004-154">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="7d004-155">Satıcı ilişkilerini ve anlaşmasını gözden geçirmek ve kabul etmek için yeni bir müşteri davet edin.</span><span class="sxs-lookup"><span data-stu-id="7d004-155">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="7d004-156">Mevcut bir müşteriyi gözden geçirip sözleşmeyi kabul edecek şekilde davet edin.</span><span class="sxs-lookup"><span data-stu-id="7d004-156">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="7d004-157">[Iş ortağı MERKEZI API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) 'sını, müşterinin Microsoft Müşteri sözleşmesinin doğrudan kabulüne ilişkin durumunu almak için kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7d004-157">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="7d004-158">Yeni bir müşteri oluşturun ve sözleşmeyi gözden geçirmek ve kabul etmek için müşteriyi davet edin</span><span class="sxs-lookup"><span data-stu-id="7d004-158">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="7d004-159">Iş Ortağı Merkezi 'nde yeni bir müşteri oluşturmak için aşağıdaki adımları kullanın ve ardından Microsoft 365 Yönetim Merkezi 'nde Microsoft Müşteri anlaşmasını gözden geçirip kabul edin.</span><span class="sxs-lookup"><span data-stu-id="7d004-159">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="7d004-160">Iş Ortağı Merkezi 'nin içindeki **müşteriler** sekmesinden **Müşteri Ekle**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="7d004-160">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="7d004-161">**Hesap bilgileri** altında, müşterinin Şirket adı ve birincil ilgili kişisi dahil olmak üzere tüm gerekli alanlara yeni müşteri hakkındaki bilgileri girin.</span><span class="sxs-lookup"><span data-stu-id="7d004-161">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="7d004-162">**Müşteri Sözleşmesi**' nin altında, **Microsoft 365 Yönetim Merkezi ' ndeki Microsoft Müşteri anlaşmasını kabul etmesi istenecek müşteri**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="7d004-162">Under **Customer Agreement**, select **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="7d004-163">Sayfadaki diğer tüm gerekli alanları doldurun.</span><span class="sxs-lookup"><span data-stu-id="7d004-163">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="7d004-164">Ileri ' yi seçin **: gözden geçirin** ve ardından müşteri kiracısını oluşturma adımlarına devam edin.</span><span class="sxs-lookup"><span data-stu-id="7d004-164">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="7d004-165">Yeni müşteriler, Microsoft Müşteri anlaşmasını kabul edene kadar satın alma yapamaz.</span><span class="sxs-lookup"><span data-stu-id="7d004-165">New customers cannot make a purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Yeni müşteri oluşturun.":::

5. <span data-ttu-id="7d004-167">Yeni müşteri iş akışındaki **onay** ekranına ulaştığınızda müşteri kimlik bilgilerini kaydedin.</span><span class="sxs-lookup"><span data-stu-id="7d004-167">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="7d004-168">Bu kimlik bilgilerini müşterinize daha sonra sağlamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="7d004-168">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="7d004-169">Iş ortağı merkezi dışında, Microsoft 365 Yönetim merkezinde Microsoft Müşteri anlaşmasını kabul etmek üzere müşteriyi davet eden bir e-posta oluşturun ve gönderin.</span><span class="sxs-lookup"><span data-stu-id="7d004-169">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="7d004-170">Bu öğeleri e-postaya eklediğinizden emin olun:</span><span class="sxs-lookup"><span data-stu-id="7d004-170">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="7d004-171">Bu [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) 'ye bir bağlantı (oturum açma gerekir)</span><span class="sxs-lookup"><span data-stu-id="7d004-171">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="7d004-172">5. adımda kaydettiğiniz müşterinin kimlik bilgileri.</span><span class="sxs-lookup"><span data-stu-id="7d004-172">The customer's credentials that you saved in Step 5.</span></span>

7. <span data-ttu-id="7d004-173">Müşteri, daha sonra iş ortağından gelen daveti alacak ve [URL 'yi](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement)seçmeyecektir.</span><span class="sxs-lookup"><span data-stu-id="7d004-173">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="7d004-174">Müşteri, girdiğiniz müşteri kimlik bilgilerini kullanarak Microsoft 365 Yönetim Merkezi 'Nde oturum açar.</span><span class="sxs-lookup"><span data-stu-id="7d004-174">The customer signs into Microsoft 365 Admin Center using the customer credentials you provided.</span></span>

9. <span data-ttu-id="7d004-175">Müşteri, Microsoft Müşteri anlaşmasını kabul etmek için kutuyu kontrol eder.</span><span class="sxs-lookup"><span data-stu-id="7d004-175">The customer checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="7d004-176">Satıcı ilişkilerini gözden geçirmek ve kabul etmek için yeni bir müşteri davet edin ve Microsoft Müşteri Sözleşmesi</span><span class="sxs-lookup"><span data-stu-id="7d004-176">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="7d004-177">Yeni bir müşteriyi gözden geçirmek ve satıcı ilişkilerini ve Microsoft Müşteri anlaşmasını kabul etmek üzere davet etmek için aşağıdaki adımları kullanın.</span><span class="sxs-lookup"><span data-stu-id="7d004-177">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="7d004-178">Iş Ortağı Merkezi 'nin içindeki **müşteriler** sekmesinden **bir satıcı ilişki iste** bağlantısı ' nı seçin.</span><span class="sxs-lookup"><span data-stu-id="7d004-178">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="7d004-179">Metin ve müşteriyi Microsoft 365 yönetim merkezine yönlendiren parametreli bir URL dahil olmak üzere otomatik e-posta şablonu oluşturulacaktır.</span><span class="sxs-lookup"><span data-stu-id="7d004-179">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="7d004-180">Otomatik olarak oluşturulan e-posta şablonunu özelleştirebilir ve sonra **Panoya Kopyala** ' yı seçerek **e-posta ile açabilirsiniz**.</span><span class="sxs-lookup"><span data-stu-id="7d004-180">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="7d004-181">Müşteriyi **satıcı ilişki** Isteği ve **Microsoft Müşteri Sözleşmesi 'ni** kabul etmek üzere davet etmek için bu e-posta şablonunu kullanın.</span><span class="sxs-lookup"><span data-stu-id="7d004-181">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="7d004-182">(Örneğin, e-posta davetinin Içinde, iş ortağının otomatik olarak sağlanmış URL 'YI ve son zamanlarda oluşturulan müşteri kimlik bilgilerini de içerdiğinden emin olun.)</span><span class="sxs-lookup"><span data-stu-id="7d004-182">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="ilişki oluşturun.":::

5. <span data-ttu-id="7d004-184">Müşteri e-posta ile davet alır ve parametreli URL 'yi tıklatır.</span><span class="sxs-lookup"><span data-stu-id="7d004-184">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="7d004-185">Müşteri, Microsoft 365 Yönetim Merkezi 'Nde oturum açmak için e-posta içinde sağladığınız kimlik bilgilerini kullanır.</span><span class="sxs-lookup"><span data-stu-id="7d004-185">Customer uses credentials you provide within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="7d004-186">Müşteri, **satıcı ilişkilerini** ve **Microsoft Müşteri anlaşmasını** kabul etmek için kutuyu kontrol eder.</span><span class="sxs-lookup"><span data-stu-id="7d004-186">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="7d004-187">Aynı URL içinde, müşteri üzerinde çalıştıkları farklı iş ortaklarının birleştirilmiş bir listesini görebilir.</span><span class="sxs-lookup"><span data-stu-id="7d004-187">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="7d004-188">Ayrıntıları görmek için bir iş ortağı seçebilir.</span><span class="sxs-lookup"><span data-stu-id="7d004-188">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="Sözleşmeyi kabul edin.":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="7d004-190">Anlaşmayı gözden geçirmek ve kabul etmek için mevcut bir müşteriyi davet etme</span><span class="sxs-lookup"><span data-stu-id="7d004-190">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="7d004-191">Mevcut bir müşteriyi gözden geçirmek ve Microsoft Müşteri anlaşmasını kabul etmek üzere davet etmek için aşağıdaki adımları kullanın.</span><span class="sxs-lookup"><span data-stu-id="7d004-191">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="7d004-192">Müşteri e-postasını, Microsoft Müşteri anlaşmasını kabul etmek için müşterinize davet eden gömülü URL ile oluşturun.</span><span class="sxs-lookup"><span data-stu-id="7d004-192">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="7d004-193">Müşteriniz daveti e-posta yoluyla alır ve [URL 'yi](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement)tıklatır.</span><span class="sxs-lookup"><span data-stu-id="7d004-193">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="7d004-194">Müşteri kimlik bilgilerini Microsoft 365 yönetim merkezine girer.</span><span class="sxs-lookup"><span data-stu-id="7d004-194">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="7d004-195">Müşteriniz, Microsoft Müşteri anlaşmasını kabul etmek için kutuyu kontrol eder.</span><span class="sxs-lookup"><span data-stu-id="7d004-195">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="7d004-196">Aynı URL içinde, müşteri üzerinde çalıştıkları farklı iş ortaklarının birleştirilmiş listesini görebilir.</span><span class="sxs-lookup"><span data-stu-id="7d004-196">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="7d004-197">Ayrıntıları görmek için bir iş ortağı seçebilir.</span><span class="sxs-lookup"><span data-stu-id="7d004-197">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="müşterisi.":::

>[!NOTE]
><span data-ttu-id="7d004-199">Bazı senaryolarda, müşteriler Microsoft Müşteri anlaşmasını doğrudan kabul edemeyebilir.</span><span class="sxs-lookup"><span data-stu-id="7d004-199">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="7d004-200">Bu durumlar hakkında daha fazla bilgi edinmek için, aşağıdaki Müşterinizin adına sınamanız gereken Iki senaryoyu okuyun.</span><span class="sxs-lookup"><span data-stu-id="7d004-200">To learn more about these situations, read Two scenarios where you need to attest on behalf of your customer, below.</span></span>

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a><span data-ttu-id="7d004-201">Müşteriniz adına bunu test etmek için ihtiyacınız olan iki senaryo</span><span class="sxs-lookup"><span data-stu-id="7d004-201">Two scenarios where you need to attest on behalf of your customer</span></span>

<span data-ttu-id="7d004-202">Müşterilerin Yönetim Merkezi'nde doğrudan Microsoft Müşteri Sözleşmesi kabul Microsoft 365 senaryo vardır.</span><span class="sxs-lookup"><span data-stu-id="7d004-202">There are two scenarios where customers may not be able to directly accept the Microsoft Customer Agreement within the Microsoft 365 Admin Center.</span></span>

<span data-ttu-id="7d004-203">**Senaryo 1:** Mevcut bir müşteri, mevcut iş ortağı ilişkisi aracılığıyla aşağıdakilerin herhangi birini satın aldı: teklifler, yazılım veya yazılım abonelikleri, Ayrılmış Örnekler veya Azure Planı.</span><span class="sxs-lookup"><span data-stu-id="7d004-203">**Scenario 1**: An existing customer has purchased any of the following through an existing partner relationship: offers, software or software subscriptions, Reserved Instances, or Azure Plan.</span></span> <span data-ttu-id="7d004-204">Müşteri şimdi yeni satın alma işlemleri yapmaya (otomatik yenileme hariç) başvurur.</span><span class="sxs-lookup"><span data-stu-id="7d004-204">The customer is now attempting to make any new purchase (excluding auto renewal).</span></span> <span data-ttu-id="7d004-205">Müşteri URL'ye tıkladığında "Lütfen İş Ortağınıza ulaşarak url'yi kabul Microsoft Müşteri Sözleşmesi."</span><span class="sxs-lookup"><span data-stu-id="7d004-205">When that customer clicks the URL, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="7d004-206">**Sorununu çözmek** için: Müşteri adına bunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="7d004-206">**To resolve**: You must attest on behalf of the customer.</span></span>

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="İş Microsoft 365 kabul etmek için iş ortağınıza ulaşmanızı isteyen Yönetim Merkezi sayfasının ekran Microsoft Müşteri Sözleşmesi.":::

<span data-ttu-id="7d004-208">**Senaryo 2:** Mevcut bir müşteri aşağıdaki tekliflerden, yazılım ve yazılım aboneliklerinin, Ayrılmış Örneklerin ve Azure Planı'nın herhangi birini satın aldı.</span><span class="sxs-lookup"><span data-stu-id="7d004-208">**Scenario 2**: An existing customer has purchased any of the following offers, software and software subscriptions, Reserved Instances, and Azure Plan.</span></span> <span data-ttu-id="7d004-209">Müşteri şimdi yeni bir iş ortağıyla yeni satın alma girişiminde bulundu.</span><span class="sxs-lookup"><span data-stu-id="7d004-209">The customer is now attempting to make any new purchase with a new partner.</span></span>

<span data-ttu-id="7d004-210">Müşteri yeni iş ortağı ilişkisini ve sözleşmeyi kabul etmek için Microsoft 365 Yönetim Merkezi'nin URL'sini tıkladığında" "Lütfen İş Ortağınıza ulaşarak bu ilişkiyi kabul ettiğiniz Microsoft Müşteri Sözleşmesi."</span><span class="sxs-lookup"><span data-stu-id="7d004-210">When the customer clicks the URL to Microsoft 365 Admin Center to accept the new partner relationship and the agreement, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="7d004-211">**Sorununu çözmek** için: Müşteri adına bunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="7d004-211">**To resolve**: You must attest on behalf of the customer.</span></span>  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a><span data-ttu-id="7d004-212">Müşterinin sözleşmeyi kabul etmiş olduğunu onaylayın</span><span class="sxs-lookup"><span data-stu-id="7d004-212">Confirm that a customer has accepted the agreement</span></span>

<span data-ttu-id="7d004-213">Daha önce onaylamadınız mevcut bir müşteri için yeni bir sipariş oluşturmanız gerekirse, onayı tamamlamanız için bir istem alırsınız.</span><span class="sxs-lookup"><span data-stu-id="7d004-213">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="7d004-214">Bunu yapmak için aşağıdaki yordamı kullanın.</span><span class="sxs-lookup"><span data-stu-id="7d004-214">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="7d004-215">Sözleşmeyi **kabul eden** kullanıcının **Ad,** Soyadı, **E-posta** adresi ve Telefon numarasını (isteğe bağlı) girin. </span><span class="sxs-lookup"><span data-stu-id="7d004-215">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="7d004-216">Sözleşme **kabul tarihi'nin** altında uygun tarihi girin.</span><span class="sxs-lookup"><span data-stu-id="7d004-216">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="7d004-217">Bunu gelecekteki bir tarihe ayaramazsiniz.</span><span class="sxs-lookup"><span data-stu-id="7d004-217">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="7d004-218">**Kaydet ve devam et**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="7d004-218">Select **Save and continue**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="7d004-219">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="7d004-219">Next steps</span></span>

- [<span data-ttu-id="7d004-220">Şirket profili bilgilerini doğrulama veya güncelleştirme</span><span class="sxs-lookup"><span data-stu-id="7d004-220">Verify or update your company profile information</span></span>](update-your-partner-profile.md)
- [<span data-ttu-id="7d004-221">Microsoft Müşteri Sözleşmeleri (bölgeye, dile göre)</span><span class="sxs-lookup"><span data-stu-id="7d004-221">Microsoft Customer Agreements (by region, language)</span></span>](Agreements.md)
