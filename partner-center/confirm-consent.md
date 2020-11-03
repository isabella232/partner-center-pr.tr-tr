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
ms.openlocfilehash: aacca72e9af45b2777364734c2b07dbe8101989d
ms.sourcegitcommit: 22af0997d52a87417b62f44fb0a7d711bec77b35
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/19/2020
ms.locfileid: "92532123"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a><span data-ttu-id="3a158-104">Microsoft Müşteri sözleşmesinin müşteri tarafından kabul edildiğini onaylamak için yöntemi güncelleştirildi</span><span class="sxs-lookup"><span data-stu-id="3a158-104">Updated method to confirm customer acceptance of the Microsoft Customer Agreement</span></span>

<span data-ttu-id="3a158-105">**Uygulama hedefi**</span><span class="sxs-lookup"><span data-stu-id="3a158-105">**Applies to**</span></span>

-  <span data-ttu-id="3a158-106">İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="3a158-106">Partner Center</span></span>

<span data-ttu-id="3a158-107">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="3a158-107">**Appropriate roles**</span></span>

- <span data-ttu-id="3a158-108">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="3a158-108">Admin agent</span></span>
- <span data-ttu-id="3a158-109">Satış Aracısı</span><span class="sxs-lookup"><span data-stu-id="3a158-109">Sales agent</span></span>

> [!NOTE]
> <span data-ttu-id="3a158-110">Sözleşme kaynağı şu anda yalnızca Microsoft genel bulutundaki Iş Ortağı Merkezi tarafından desteklenmektedir.</span><span class="sxs-lookup"><span data-stu-id="3a158-110">The Agreement resource is currently supported by Partner Center in the Microsoft public cloud only.</span></span> <span data-ttu-id="3a158-111">Şunları yapmak için geçerli değildir:</span><span class="sxs-lookup"><span data-stu-id="3a158-111">It is not applicable to:</span></span>
> * <span data-ttu-id="3a158-112">21Vianet tarafından çalıştırılan iş ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="3a158-112">Partner Center operated by 21Vianet</span></span>
> * <span data-ttu-id="3a158-113">Microsoft Bulut Almanya için iş ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="3a158-113">Partner Center for Microsoft Cloud Germany</span></span>
> * <span data-ttu-id="3a158-114">ABD kamu için Microsoft Bulut iş ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="3a158-114">Partner Center for Microsoft Cloud for US Government</span></span>

>[!NOTE]
><span data-ttu-id="3a158-115">31 Ocak 2020 itibariyle, mevcut ve yeni olan tüm müşteriler yeni Microsoft Müşteri sözleşmesinin imzalanmalıdır.</span><span class="sxs-lookup"><span data-stu-id="3a158-115">As of January 31, 2020, all customers, existing and new, must sign the new Microsoft Customer Agreement.</span></span> <span data-ttu-id="3a158-116">Daha fazla bilgi edinmek için [Microsoft Müşteri sözleşmesinin müşteri kabulünü Onayla](confirm-customer-agreement.md)makalesini okuyun.</span><span class="sxs-lookup"><span data-stu-id="3a158-116">To learn more, read [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

<span data-ttu-id="3a158-117">İş ortağı olarak, müşterinin Microsoft ürünlerini ve hizmetlerini sipariş etmeden önce, müşterinizin Microsoft Müşteri sözleşmesini kabul etmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="3a158-117">As a partner, you need to obtain your customer's acceptance of the Microsoft Customer Agreement before you can order Microsoft products and services for that customer.</span></span> <span data-ttu-id="3a158-118">İş ortaklarının uyumluluk gereksinimlerini karşıladığından daha iyi yardımcı olması için, Microsoft, anlaşmayı kabul eden kişiyle ilgili aşağıdaki ayrıntıları sağlayarak iş ortaklarının kabul onaylamasını ister:</span><span class="sxs-lookup"><span data-stu-id="3a158-118">To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing the following details regarding the person who accepted the agreement:</span></span>

- <span data-ttu-id="3a158-119">Ad</span><span class="sxs-lookup"><span data-stu-id="3a158-119">First name</span></span>

- <span data-ttu-id="3a158-120">Soyadı</span><span class="sxs-lookup"><span data-stu-id="3a158-120">Last name</span></span>

- <span data-ttu-id="3a158-121">E-posta adresi</span><span class="sxs-lookup"><span data-stu-id="3a158-121">Email address</span></span>

- <span data-ttu-id="3a158-122">Telefon numarası (isteğe bağlı)</span><span class="sxs-lookup"><span data-stu-id="3a158-122">Phone number (optional)</span></span>

- <span data-ttu-id="3a158-123">Kabul tarihi</span><span class="sxs-lookup"><span data-stu-id="3a158-123">Date of acceptance</span></span>

<span data-ttu-id="3a158-124">Doğrudan fatura ortakları ve dolaylı sağlayıcılar, Iş ortağı merkezi veya Iş Ortağı Merkezi API 'SI aracılığıyla deneyimidir olduğunda Microsoft Müşteri sözleşmesinin müşteri kabulünü kabul etmelidir.</span><span class="sxs-lookup"><span data-stu-id="3a158-124">Direct bill partners and Indirect Providers must confirm customer acceptance of the Microsoft Customer Agreement when transacting through Partner Center or Partner Center API.</span></span> <span data-ttu-id="3a158-125">Onay *zorunludur* .</span><span class="sxs-lookup"><span data-stu-id="3a158-125">Confirmation is *mandatory* .</span></span>

<span data-ttu-id="3a158-126">Belirli bir müşteri için onay sağlanmazsa:</span><span class="sxs-lookup"><span data-stu-id="3a158-126">If confirmation is not provided for a given customer:</span></span>

- <span data-ttu-id="3a158-127">Bu müşteri için yeni siparişler oluşturamayacak.</span><span class="sxs-lookup"><span data-stu-id="3a158-127">You won't be able to create new orders for this customer.</span></span>

- <span data-ttu-id="3a158-128">Bu müşteri için lisans tabanlı mevcut aboneliklerin lisans sayısını değiştiremeyeceksiniz.</span><span class="sxs-lookup"><span data-stu-id="3a158-128">You won't be able to change the license count of existing license-based subscriptions for this customer.</span></span>

<span data-ttu-id="3a158-129">Müşteri kabulünü onaylama işlemi, Iş ortağı merkezi veya Iş Ortağı Merkezi API 'SI aracılığıyla yapılabilir.</span><span class="sxs-lookup"><span data-stu-id="3a158-129">Confirmation of customer acceptance can be done via Partner Center or the Partner Center API.</span></span> <span data-ttu-id="3a158-130">Bunu Iş Ortağı Merkezi API 'SI aracılığıyla yapmak için aşağıdaki konulara bakın:</span><span class="sxs-lookup"><span data-stu-id="3a158-130">To do this through the Partner Center API, see the following topics:</span></span>

- [<span data-ttu-id="3a158-131">Müşteri onayı onayını al</span><span class="sxs-lookup"><span data-stu-id="3a158-131">Get confirmation of customer consent</span></span>](/partner-center/develop/get-confirmation-of-customer-consent)

- [<span data-ttu-id="3a158-132">Anlaşma meta verilerini al</span><span class="sxs-lookup"><span data-stu-id="3a158-132">Get agreement metadata</span></span>](/partner-center/develop/get-agreement-metadata)

- [<span data-ttu-id="3a158-133">Müşteri onayını Onayla</span><span class="sxs-lookup"><span data-stu-id="3a158-133">Confirm customer consent</span></span>](/partner-center/develop/confirm-customer-consent)

<span data-ttu-id="3a158-134">Bu, hem üretim hem de korumalı ortamlar için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="3a158-134">This applies to both production and sandbox environments.</span></span>

## <a name="confirm-customer-acceptance-for-a-new-customer"></a><span data-ttu-id="3a158-135">Yeni müşteri için müşteri kabulünü Onayla</span><span class="sxs-lookup"><span data-stu-id="3a158-135">Confirm customer acceptance for a new customer</span></span>

<span data-ttu-id="3a158-136">Iş Ortağı Merkezi 'nde yeni bir müşteri kiracısı oluştururken müşteri kabulünü onaylamak için aşağıdaki yordamı kullanın.</span><span class="sxs-lookup"><span data-stu-id="3a158-136">Use the following procedure to confirm customer acceptance while you create a new customer tenant in Partner Center.</span></span> <span data-ttu-id="3a158-137">Bunu yapmak için bir Yönetim Aracısı veya satış aracısı olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="3a158-137">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="3a158-138">**Müşteriler** ' i ve ardından **yeni müşteri** ' yi seçip **hesap bilgileri** ' ni seçin.</span><span class="sxs-lookup"><span data-stu-id="3a158-138">Select **Customers** , and then **New customer** and then select **Account info** .</span></span>

2. <span data-ttu-id="3a158-139">**Şirket** ve **birincil ilgili kişiyle** ilgili bilgileri girin.</span><span class="sxs-lookup"><span data-stu-id="3a158-139">Enter the information about the **Company** and **Primary contact** .</span></span>

   :::image type="content" source="images/mca/mca1.png" alt-text="Şirket bilgileri":::

3. <span data-ttu-id="3a158-141">**Microsoft Müşteri Sözleşmesi** altında **müşterinin en son Microsoft Müşteri anlaşmasını kabul etmiş olduğunu** seçin.</span><span class="sxs-lookup"><span data-stu-id="3a158-141">Under **Microsoft customer agreement** , select **The customer has accepted the latest Microsoft customer agreement** .</span></span>

4. <span data-ttu-id="3a158-142">**Sözleşme kabul tarihi** altında, uygun tarihi girin.</span><span class="sxs-lookup"><span data-stu-id="3a158-142">Under **Agreement acceptance date** , enter the appropriate date.</span></span> <span data-ttu-id="3a158-143">Bunu gelecekteki bir tarihle ayarlayamazsınız.</span><span class="sxs-lookup"><span data-stu-id="3a158-143">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="3a158-144">Kabulü sağlayan kullanıcının ayrıntılarını girin.</span><span class="sxs-lookup"><span data-stu-id="3a158-144">Enter the details of the user who provided the acceptance.</span></span>

   :::image type="content" source="images/mca/MCA3.png" alt-text="Kabul tarihi Ekle":::

   <span data-ttu-id="3a158-146">Varsayılan olarak, birincil kişi Kullanıcı bilgileri görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="3a158-146">By default, the primary contact user information is displayed.</span></span> <span data-ttu-id="3a158-147">Bu doğru değilse **Güncelleştir** ' i seçin ve ardından sözleşmeyi kabul eden kişinin **adı** , **Soyadı** , **e-posta adresi** ve \* *telefon numarasını* (isteğe bağlı) girin.</span><span class="sxs-lookup"><span data-stu-id="3a158-147">If this isn't correct, select **Update** and then enter the **First name** , **Last name** , **Email address** , and \* *Phone number* (optional) of the person who accepted the agreement.</span></span>

6. <span data-ttu-id="3a158-148">Müşteri kiracısını oluşturmaya yönelik kalan adımlara devam etmek için **İleri ' yi** seçin.</span><span class="sxs-lookup"><span data-stu-id="3a158-148">Select **Next** to continue with the remaining steps to create the customer tenant.</span></span>

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="3a158-149">Mevcut bir müşteri için müşteri kabulünü Onayla</span><span class="sxs-lookup"><span data-stu-id="3a158-149">Confirm customer acceptance for an existing customer</span></span>

<span data-ttu-id="3a158-150">Bunu yapmak için bir Yönetim Aracısı veya satış aracısı olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="3a158-150">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="3a158-151">**Müşteriler** ' i seçin ve ardından görmek istediğiniz müşteriyi bulun ve seçin.</span><span class="sxs-lookup"><span data-stu-id="3a158-151">Select **Customers** , and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="3a158-152">**Hesap bilgilerini** seçin.</span><span class="sxs-lookup"><span data-stu-id="3a158-152">Select **Account info** .</span></span>

3. <span data-ttu-id="3a158-153">**Microsoft Müşteri Sözleşmesi** altında **Güncelleştir** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="3a158-153">Under **Microsoft customer agreement** , select **Update** .</span></span>

   :::image type="content" source="images/mca/mca4.png" alt-text="Güncelleştirme":::

4. <span data-ttu-id="3a158-155">Sözleşmeyi kabul eden kullanıcının **adını** , **soyadını** , **e-posta adresini** ve **telefon numarasını** (isteğe bağlı) girin.</span><span class="sxs-lookup"><span data-stu-id="3a158-155">Enter the **First name** , **Last name** , **Email address** , and **Phone number** (optional) of the user who accepted the agreement.</span></span>

5. <span data-ttu-id="3a158-156">**Sözleşme kabul tarihi** altında, uygun tarihi girin.</span><span class="sxs-lookup"><span data-stu-id="3a158-156">Under **Agreement acceptance date** , enter the appropriate date.</span></span> <span data-ttu-id="3a158-157">Bunu gelecekteki bir tarihle ayarlayamazsınız.</span><span class="sxs-lookup"><span data-stu-id="3a158-157">You cannot set this to a future date.</span></span>

6. <span data-ttu-id="3a158-158">**Kaydet ve devam et** ’i seçin.</span><span class="sxs-lookup"><span data-stu-id="3a158-158">Select **Save and continue** .</span></span>

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a><span data-ttu-id="3a158-159">Mevcut bir müşteri için yeni sipariş oluştururken müşteri kabulünü Onayla</span><span class="sxs-lookup"><span data-stu-id="3a158-159">Confirm customer acceptance while creating new order for an existing customer</span></span>

<span data-ttu-id="3a158-160">Daha önce teyit edilmemiş mevcut bir müşteri için yeni bir sipariş oluşturmayı denerseniz, onayı tamamlamaya yönelik bir istem alırsınız.</span><span class="sxs-lookup"><span data-stu-id="3a158-160">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="3a158-161">Bunu yapmak için aşağıdaki yordamı kullanın.</span><span class="sxs-lookup"><span data-stu-id="3a158-161">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="3a158-162">Sözleşmeyi kabul eden kullanıcının **adını** , **soyadını** , **e-posta adresini** ve **telefon numarasını** (isteğe bağlı) girin.</span><span class="sxs-lookup"><span data-stu-id="3a158-162">Enter the **First name** , **Last name** , **Email address** , and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="3a158-163">**Sözleşme kabul tarihi** altında, uygun tarihi girin.</span><span class="sxs-lookup"><span data-stu-id="3a158-163">Under **Agreement acceptance date** , enter the appropriate date.</span></span> <span data-ttu-id="3a158-164">Bunu gelecekteki bir tarihle ayarlayamazsınız.</span><span class="sxs-lookup"><span data-stu-id="3a158-164">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="3a158-165">**Kaydet ve devam et** ’i seçin.</span><span class="sxs-lookup"><span data-stu-id="3a158-165">Select **Save and continue** .</span></span>

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="3a158-166">Mevcut bir müşteri için müşteri kabulünün onayını alma</span><span class="sxs-lookup"><span data-stu-id="3a158-166">Retrieve confirmation of customer acceptance for an existing customer</span></span>

<span data-ttu-id="3a158-167">Aşağıdaki yordamı kullanarak daha önce sağlamış olduğunuz mevcut bir müşteri için müşteri kabulünün onayını alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="3a158-167">You can retrieve confirmation of customer acceptance for an existing customer that you have provided previously using the procedure below.</span></span> <span data-ttu-id="3a158-168">Bunu yapmak için bir Yönetim Aracısı veya satış aracısı olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="3a158-168">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="3a158-169">**Müşteriler** ' i seçin ve ardından görmek istediğiniz müşteriyi bulun ve seçin.</span><span class="sxs-lookup"><span data-stu-id="3a158-169">Select **Customers** , and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="3a158-170">**Hesap bilgilerini** seçin.</span><span class="sxs-lookup"><span data-stu-id="3a158-170">Select **Account info** .</span></span>

3. <span data-ttu-id="3a158-171">**Microsoft Müşteri Sözleşmesi** ' nin altında, bu müşteri için onay verilip verilmeyeceğini görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="3a158-171">Under **Microsoft customer agreement** , you'll see whether or not confirmation has been provided for this customer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3a158-172">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="3a158-172">Next steps</span></span>

- [<span data-ttu-id="3a158-173">CSP iş ortağı programında Microsoft Müşteri Sözleşmesi 'nin müşteri kabulünü onaylayın</span><span class="sxs-lookup"><span data-stu-id="3a158-173">Confirm customer acceptance of the Microsoft Customer Agreement in the CSP partner program</span></span>](confirm-customer-agreement.md)

- [<span data-ttu-id="3a158-174">Müşterinizin adına Microsoft Müşteri sözleşmesinin onay onayı</span><span class="sxs-lookup"><span data-stu-id="3a158-174">Attest acceptance of the Microsoft Customer Agreement on behalf of your customer</span></span>](attest-acceptance-customer-agreement.md)