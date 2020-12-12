---
title: Microsoft Müşteri sözleşmesinin müşteri kabulünü Onayla
description: Microsoft Müşteri sözleşmesinin müşteri kabulünü onaylama hakkında bilgi edinin. Bu, müşterilerin Microsoft ürünlerini ve hizmetlerini sıralamak için gerekebilir.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/30/2020
ms.openlocfilehash: f2513213bff38a6296832253a13725ff2508f1f8
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354619"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a><span data-ttu-id="5ddbb-104">Microsoft Müşteri sözleşmesinin müşteri tarafından kabul edildiğini onaylamak için yöntemi güncelleştirildi</span><span class="sxs-lookup"><span data-stu-id="5ddbb-104">Updated method to confirm customer acceptance of the Microsoft Customer Agreement</span></span>


<span data-ttu-id="5ddbb-105">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="5ddbb-105">**Appropriate roles**</span></span>

- <span data-ttu-id="5ddbb-106">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="5ddbb-106">Admin agent</span></span>
- <span data-ttu-id="5ddbb-107">Satış Aracısı</span><span class="sxs-lookup"><span data-stu-id="5ddbb-107">Sales agent</span></span>

> [!NOTE]
> <span data-ttu-id="5ddbb-108">Sözleşme kaynağı şu anda yalnızca Microsoft genel bulutundaki Iş Ortağı Merkezi tarafından desteklenmektedir.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-108">The Agreement resource is currently supported by Partner Center in the Microsoft public cloud only.</span></span> <span data-ttu-id="5ddbb-109">Şunları yapmak için geçerli değildir:</span><span class="sxs-lookup"><span data-stu-id="5ddbb-109">It is not applicable to:</span></span>
> * <span data-ttu-id="5ddbb-110">21Vianet tarafından çalıştırılan iş ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="5ddbb-110">Partner Center operated by 21Vianet</span></span>
> * <span data-ttu-id="5ddbb-111">Microsoft Bulut Almanya için İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="5ddbb-111">Partner Center for Microsoft Cloud Germany</span></span>
> * <span data-ttu-id="5ddbb-112">Microsoft Cloud for US Government için İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="5ddbb-112">Partner Center for Microsoft Cloud for US Government</span></span>

>[!NOTE]
><span data-ttu-id="5ddbb-113">31 Ocak 2020 itibariyle, mevcut ve yeni olan tüm müşteriler yeni Microsoft Müşteri sözleşmesinin imzalanmalıdır.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-113">As of January 31, 2020, all customers, existing and new, must sign the new Microsoft Customer Agreement.</span></span> <span data-ttu-id="5ddbb-114">Daha fazla bilgi edinmek için [Microsoft Müşteri sözleşmesinin müşteri kabulünü Onayla](confirm-customer-agreement.md)makalesini okuyun.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-114">To learn more, read [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

<span data-ttu-id="5ddbb-115">İş ortağı olarak, müşterinin Microsoft ürünlerini ve hizmetlerini sipariş etmeden önce, müşterinizin Microsoft Müşteri sözleşmesini kabul etmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-115">As a partner, you need to obtain your customer's acceptance of the Microsoft Customer Agreement before you can order Microsoft products and services for that customer.</span></span> <span data-ttu-id="5ddbb-116">İş ortaklarının uyumluluk gereksinimlerini karşıladığından daha iyi yardımcı olması için, Microsoft, anlaşmayı kabul eden kişiyle ilgili aşağıdaki ayrıntıları sağlayarak iş ortaklarının kabul onaylamasını ister:</span><span class="sxs-lookup"><span data-stu-id="5ddbb-116">To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing the following details regarding the person who accepted the agreement:</span></span>

- <span data-ttu-id="5ddbb-117">Ad</span><span class="sxs-lookup"><span data-stu-id="5ddbb-117">First name</span></span>

- <span data-ttu-id="5ddbb-118">Soyadı</span><span class="sxs-lookup"><span data-stu-id="5ddbb-118">Last name</span></span>

- <span data-ttu-id="5ddbb-119">E-posta adresi</span><span class="sxs-lookup"><span data-stu-id="5ddbb-119">Email address</span></span>

- <span data-ttu-id="5ddbb-120">Telefon numarası (isteğe bağlı)</span><span class="sxs-lookup"><span data-stu-id="5ddbb-120">Phone number (optional)</span></span>

- <span data-ttu-id="5ddbb-121">Kabul tarihi</span><span class="sxs-lookup"><span data-stu-id="5ddbb-121">Date of acceptance</span></span>

<span data-ttu-id="5ddbb-122">Doğrudan fatura ortakları ve dolaylı sağlayıcılar, Iş ortağı merkezi veya Iş Ortağı Merkezi API 'SI aracılığıyla deneyimidir olduğunda Microsoft Müşteri sözleşmesinin müşteri kabulünü kabul etmelidir.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-122">Direct bill partners and Indirect Providers must confirm customer acceptance of the Microsoft Customer Agreement when transacting through Partner Center or Partner Center API.</span></span> <span data-ttu-id="5ddbb-123">Onay *zorunludur*.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-123">Confirmation is *mandatory*.</span></span>

<span data-ttu-id="5ddbb-124">Belirli bir müşteri için onay sağlanmazsa:</span><span class="sxs-lookup"><span data-stu-id="5ddbb-124">If confirmation is not provided for a given customer:</span></span>

- <span data-ttu-id="5ddbb-125">Bu müşteri için yeni siparişler oluşturamayacak.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-125">You won't be able to create new orders for this customer.</span></span>

- <span data-ttu-id="5ddbb-126">Bu müşteri için lisans tabanlı mevcut aboneliklerin lisans sayısını değiştiremeyeceksiniz.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-126">You won't be able to change the license count of existing license-based subscriptions for this customer.</span></span>

<span data-ttu-id="5ddbb-127">Müşteri kabulünü onaylama işlemi, Iş ortağı merkezi veya Iş Ortağı Merkezi API 'SI aracılığıyla yapılabilir.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-127">Confirmation of customer acceptance can be done via Partner Center or the Partner Center API.</span></span> <span data-ttu-id="5ddbb-128">Bunu Iş Ortağı Merkezi API 'SI aracılığıyla yapmak için aşağıdaki konulara bakın:</span><span class="sxs-lookup"><span data-stu-id="5ddbb-128">To do this through the Partner Center API, see the following topics:</span></span>

- [<span data-ttu-id="5ddbb-129">Müşteri onayı onayını al</span><span class="sxs-lookup"><span data-stu-id="5ddbb-129">Get confirmation of customer consent</span></span>](/partner-center/develop/get-confirmation-of-customer-consent)

- [<span data-ttu-id="5ddbb-130">Anlaşma meta verilerini al</span><span class="sxs-lookup"><span data-stu-id="5ddbb-130">Get agreement metadata</span></span>](/partner-center/develop/get-agreement-metadata)

- [<span data-ttu-id="5ddbb-131">Müşteri onayını Onayla</span><span class="sxs-lookup"><span data-stu-id="5ddbb-131">Confirm customer consent</span></span>](/partner-center/develop/confirm-customer-consent)

<span data-ttu-id="5ddbb-132">Bu, hem üretim hem de korumalı ortamlar için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-132">This applies to both production and sandbox environments.</span></span>

## <a name="confirm-customer-acceptance-for-a-new-customer"></a><span data-ttu-id="5ddbb-133">Yeni müşteri için müşteri kabulünü Onayla</span><span class="sxs-lookup"><span data-stu-id="5ddbb-133">Confirm customer acceptance for a new customer</span></span>

<span data-ttu-id="5ddbb-134">Iş Ortağı Merkezi 'nde yeni bir müşteri kiracısı oluştururken müşteri kabulünü onaylamak için aşağıdaki yordamı kullanın.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-134">Use the following procedure to confirm customer acceptance while you create a new customer tenant in Partner Center.</span></span> <span data-ttu-id="5ddbb-135">Bunu yapmak için bir Yönetim Aracısı veya satış aracısı olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-135">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="5ddbb-136">**Müşteriler**' i ve ardından **yeni müşteri** ' yi seçip **hesap bilgileri**' ni seçin.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-136">Select **Customers**, and then **New customer** and then select **Account info**.</span></span>

2. <span data-ttu-id="5ddbb-137">**Şirket** ve **birincil ilgili kişiyle** ilgili bilgileri girin.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-137">Enter the information about the **Company** and **Primary contact**.</span></span>

   :::image type="content" source="images/mca/mca1.png" alt-text="Şirket bilgileri":::

3. <span data-ttu-id="5ddbb-139">**Microsoft Müşteri Sözleşmesi** altında **müşterinin en son Microsoft Müşteri anlaşmasını kabul etmiş olduğunu** seçin.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-139">Under **Microsoft customer agreement**, select **The customer has accepted the latest Microsoft customer agreement**.</span></span>

4. <span data-ttu-id="5ddbb-140">**Sözleşme kabul tarihi** altında, uygun tarihi girin.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-140">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="5ddbb-141">Bunu gelecekteki bir tarihle ayarlayamazsınız.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-141">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="5ddbb-142">Kabulü sağlayan kullanıcının ayrıntılarını girin.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-142">Enter the details of the user who provided the acceptance.</span></span>

   :::image type="content" source="images/mca/MCA3.png" alt-text="Kabul tarihi Ekle":::

   <span data-ttu-id="5ddbb-144">Varsayılan olarak, birincil kişi Kullanıcı bilgileri görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-144">By default, the primary contact user information is displayed.</span></span> <span data-ttu-id="5ddbb-145">Bu doğru değilse **Güncelleştir** ' i seçin ve ardından sözleşmeyi kabul eden kişinin **adı**, **Soyadı**, **e-posta adresi** ve \**telefon numarasını* (isteğe bağlı) girin.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-145">If this isn't correct, select **Update** and then enter the **First name**, **Last name**, **Email address**, and \**Phone number* (optional) of the person who accepted the agreement.</span></span>

6. <span data-ttu-id="5ddbb-146">Müşteri kiracısını oluşturmaya yönelik kalan adımlara devam etmek için **İleri ' yi** seçin.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-146">Select **Next** to continue with the remaining steps to create the customer tenant.</span></span>

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="5ddbb-147">Mevcut bir müşteri için müşteri kabulünü Onayla</span><span class="sxs-lookup"><span data-stu-id="5ddbb-147">Confirm customer acceptance for an existing customer</span></span>

<span data-ttu-id="5ddbb-148">Bunu yapmak için bir Yönetim Aracısı veya satış aracısı olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-148">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="5ddbb-149">**Müşteriler**' i seçin ve ardından görmek istediğiniz müşteriyi bulun ve seçin.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-149">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="5ddbb-150">**Hesap bilgilerini** seçin.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-150">Select **Account info**.</span></span>

3. <span data-ttu-id="5ddbb-151">**Microsoft Müşteri Sözleşmesi** altında **Güncelleştir**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-151">Under **Microsoft customer agreement**, select **Update**.</span></span>

   :::image type="content" source="images/mca/mca4.png" alt-text="Güncelleştirme":::

4. <span data-ttu-id="5ddbb-153">Sözleşmeyi kabul eden kullanıcının **adını**, **soyadını**, **e-posta adresini** ve **telefon numarasını** (isteğe bağlı) girin.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-153">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

5. <span data-ttu-id="5ddbb-154">**Sözleşme kabul tarihi** altında, uygun tarihi girin.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-154">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="5ddbb-155">Bunu gelecekteki bir tarihle ayarlayamazsınız.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-155">You cannot set this to a future date.</span></span>

6. <span data-ttu-id="5ddbb-156">**Kaydet ve devam et**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-156">Select **Save and continue**.</span></span>

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a><span data-ttu-id="5ddbb-157">Mevcut bir müşteri için yeni sipariş oluştururken müşteri kabulünü Onayla</span><span class="sxs-lookup"><span data-stu-id="5ddbb-157">Confirm customer acceptance while creating new order for an existing customer</span></span>

<span data-ttu-id="5ddbb-158">Daha önce teyit edilmemiş mevcut bir müşteri için yeni bir sipariş oluşturmayı denerseniz, onayı tamamlamaya yönelik bir istem alırsınız.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-158">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="5ddbb-159">Bunu yapmak için aşağıdaki yordamı kullanın.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-159">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="5ddbb-160">Sözleşmeyi kabul eden kullanıcının **adını**, **soyadını**, **e-posta adresini** ve **telefon numarasını** (isteğe bağlı) girin.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-160">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="5ddbb-161">**Sözleşme kabul tarihi** altında, uygun tarihi girin.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-161">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="5ddbb-162">Bunu gelecekteki bir tarihle ayarlayamazsınız.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-162">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="5ddbb-163">**Kaydet ve devam et**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-163">Select **Save and continue**.</span></span>

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="5ddbb-164">Mevcut bir müşteri için müşteri kabulünün onayını alma</span><span class="sxs-lookup"><span data-stu-id="5ddbb-164">Retrieve confirmation of customer acceptance for an existing customer</span></span>

<span data-ttu-id="5ddbb-165">Aşağıdaki yordamı kullanarak daha önce sağlamış olduğunuz mevcut bir müşteri için müşteri kabulünün onayını alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-165">You can retrieve confirmation of customer acceptance for an existing customer that you have provided previously using the procedure below.</span></span> <span data-ttu-id="5ddbb-166">Bunu yapmak için bir Yönetim Aracısı veya satış aracısı olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-166">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="5ddbb-167">**Müşteriler**' i seçin ve ardından görmek istediğiniz müşteriyi bulun ve seçin.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-167">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="5ddbb-168">**Hesap bilgilerini** seçin.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-168">Select **Account info**.</span></span>

3. <span data-ttu-id="5ddbb-169">**Microsoft Müşteri Sözleşmesi**' nin altında, bu müşteri için onay verilip verilmeyeceğini görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="5ddbb-169">Under **Microsoft customer agreement**, you'll see whether or not confirmation has been provided for this customer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5ddbb-170">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="5ddbb-170">Next steps</span></span>

- [<span data-ttu-id="5ddbb-171">CSP iş ortağı programında Microsoft Müşteri Sözleşmesi 'nin müşteri kabulünü onaylayın</span><span class="sxs-lookup"><span data-stu-id="5ddbb-171">Confirm customer acceptance of the Microsoft Customer Agreement in the CSP partner program</span></span>](confirm-customer-agreement.md)

- [<span data-ttu-id="5ddbb-172">Müşterinizin adına Microsoft Müşteri sözleşmesinin onay onayı</span><span class="sxs-lookup"><span data-stu-id="5ddbb-172">Attest acceptance of the Microsoft Customer Agreement on behalf of your customer</span></span>](attest-acceptance-customer-agreement.md)