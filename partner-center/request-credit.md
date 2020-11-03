---
title: Microsoft'tan SLA iade isteğinde bulunma
ms.topic: article
ms.date: 04/28/2020
description: Müşterileriniz bir hizmet kesintisi yaşanırsa, Microsoft 'tan bir hizmet düzeyi sözleşmesi (SLA) kredisi istemek için avantajları, kısıtlamaları ve yordamları öğrenin.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: cb8f6b2280318427b2015403b528fc288ef64d97
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/14/2020
ms.locfileid: "92530961"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a><span data-ttu-id="df444-103">Microsoft 'tan bir hizmet düzeyi sözleşmesi (SLA) kredisi isteme</span><span class="sxs-lookup"><span data-stu-id="df444-103">How and when to request a service-level agreement (SLA) credit from Microsoft</span></span>

<span data-ttu-id="df444-104">Müşterileriniz için sağladığınızı bir hizmet kesintiye neden olursa, Microsoft 'tan **hizmet düzeyi sözleşmesi (SLA) kredileri** isteyebileceksiniz.</span><span class="sxs-lookup"><span data-stu-id="df444-104">You're able to request **service-level agreement (SLA) credits** from Microsoft if a service that you're providing for your customers has an outage.</span></span>

## <a name="sla-credit-calculation"></a><span data-ttu-id="df444-105">SLA kredi hesaplaması</span><span class="sxs-lookup"><span data-stu-id="df444-105">SLA credit calculation</span></span>

<span data-ttu-id="df444-106">Microsoft 'tan alınan SLA kredileri, hangi hizmet (ler) in etkilendiğini temel alır.</span><span class="sxs-lookup"><span data-stu-id="df444-106">SLA credits from Microsoft are determined based on which service(s) were impacted.</span></span> <span data-ttu-id="df444-107">Örneğin, müşterinizin bir Office 365 paketi varsa ancak yalnızca bir SharePoint kesintisi yaşanıyorsa, SLA Kredisi yalnızca SharePoint için onaylanır ve müşterinin tüm planı değildir.</span><span class="sxs-lookup"><span data-stu-id="df444-107">For example, if your customer has an Office 365 suite but only experienced a SharePoint outage, the SLA credit is approved only for SharePoint and not the customer's entire plan.</span></span>

<span data-ttu-id="df444-108">*Krediler, etkilenen hizmet ve kesinti süresi temel alınarak Pro derecelendirilir.*</span><span class="sxs-lookup"><span data-stu-id="df444-108">*Credits are pro-rated based on the service affected and the duration of the outage.*</span></span> <span data-ttu-id="df444-109">SLA kredilerine uygun olan senaryoların türlerini görmek için bkz. [çevrimiçi hizmetler BIRLEŞTIRILMIŞ SLA belgesi](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37).</span><span class="sxs-lookup"><span data-stu-id="df444-109">To see the types of scenarios that qualify for SLA credits, see the [Online Services Consolidated SLA document](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37).</span></span> <span data-ttu-id="df444-110">Bu bilgiler, bulut çözümü sağlayıcısı programı aracılığıyla satılan hizmetler için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="df444-110">This information applies to services sold through the Cloud Solution Provider program, too.</span></span>

## <a name="request-an-sla-credit"></a><span data-ttu-id="df444-111">SLA Kredisi isteme</span><span class="sxs-lookup"><span data-stu-id="df444-111">Request an SLA credit</span></span>

<span data-ttu-id="df444-112">*Bulut çözümü sağlayıcısı (CSP) iş ortağı, olayın gerçekleştiği ay sonra takvim ayının sonuna kadar talebi ve tüm gerekli bilgileri göndermesi gerekir.*</span><span class="sxs-lookup"><span data-stu-id="df444-112">*The Cloud Solution Provider (CSP) partner must submit the claim and all required information by the end of the calendar month following the month in which the incident occurred.*</span></span> <span data-ttu-id="df444-113">Örneğin, olay 15 Şubat 'ta oluştuysa, Microsoft bu isteği ve tüm gerekli bilgileri 31 Mart tarihine kadar almalıdır.</span><span class="sxs-lookup"><span data-stu-id="df444-113">For example, if the incident occurred on February 15th, Microsoft must receive the claim and all required information by March 31st.</span></span> <span data-ttu-id="df444-114">Son müşteriler ve dolaylı satıcılar SLA kredi taleplerini gönderemez; dolaylı sağlayıcı veya doğrudan fatura ortağı kendi adına talepler göndermesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="df444-114">End customers and indirect resellers can't submit SLA credit claims; either the indirect provider or direct bill partner must submit claims on their behalf.</span></span>

### <a name="required-information"></a><span data-ttu-id="df444-115">Gerekli bilgiler</span><span class="sxs-lookup"><span data-stu-id="df444-115">Required information</span></span>

<span data-ttu-id="df444-116">Microsoft 'a [BIR SLA Kredisi isteği göndermeden](#submit-sla-credit-request) önce, destek biletine dahil etmek için aşağıdaki bilgileri toplamanız gerekir:</span><span class="sxs-lookup"><span data-stu-id="df444-116">Before you [submit an SLA credit request](#submit-sla-credit-request) to Microsoft, you must gather the following information to include in your support ticket:</span></span>

- <span data-ttu-id="df444-117">Müşteri kiracının GUID 'SI</span><span class="sxs-lookup"><span data-stu-id="df444-117">The customer tenant's GUID</span></span>
- <span data-ttu-id="df444-118">[Kesinti olayı tanımlayıcısı](#outage-incident-identifier)?</span><span class="sxs-lookup"><span data-stu-id="df444-118">The [outage incident identifier](#outage-incident-identifier)?</span></span>
- <span data-ttu-id="df444-119">CSP aracılığıyla satın alınan etkilenen abonelikler mi?</span><span class="sxs-lookup"><span data-stu-id="df444-119">Were the impacted subscriptions purchased through CSP?</span></span> <span data-ttu-id="df444-120">( *Evet* veya *Hayır* )</span><span class="sxs-lookup"><span data-stu-id="df444-120">( *yes* or *no* )</span></span>

#### <a name="outage-incident-identifier"></a><span data-ttu-id="df444-121">Kesinti olayı tanımlayıcısı</span><span class="sxs-lookup"><span data-stu-id="df444-121">Outage incident identifier</span></span>

<span data-ttu-id="df444-122">Kesinti olayı tanıtıcısını, Microsoft 365 Yönetim Merkezi 'ndeki **hizmet durumu** sayfasında bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="df444-122">You can find the identifier for the outage incident on the **Service Health** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="df444-123">**Kesinti OLAYı kimliği** , etkilenen hizmeti (örneğin, Exchange Online kesintisi için *EX25194* ) gösteren iki harfli kısaltmadan önce gelen bir sayıdır.</span><span class="sxs-lookup"><span data-stu-id="df444-123">The **Outage Incident ID** is a number preceded by a two-letter abbreviation that indicates the affected service (for example, *EX25194* for an Exchange Online outage).</span></span> <span data-ttu-id="df444-124">Takip tablosu yaygın hizmet kısaltmalarını açıklar:</span><span class="sxs-lookup"><span data-stu-id="df444-124">The follow table describes common service abbreviations:</span></span>

| <span data-ttu-id="df444-125">İki harfli kısaltma</span><span class="sxs-lookup"><span data-stu-id="df444-125">Two-letter abbreviation</span></span> | <span data-ttu-id="df444-126">Microsoft hizmeti</span><span class="sxs-lookup"><span data-stu-id="df444-126">Microsoft service</span></span> |
| ----------------------- | ----------------- |
| <span data-ttu-id="df444-127">DEĞERINE</span><span class="sxs-lookup"><span data-stu-id="df444-127">EX</span></span> | <span data-ttu-id="df444-128">Exchange Online</span><span class="sxs-lookup"><span data-stu-id="df444-128">Exchange Online</span></span> |
| <span data-ttu-id="df444-129">INFO</span><span class="sxs-lookup"><span data-stu-id="df444-129">FO</span></span> | <span data-ttu-id="df444-130">Exchange Online koruması</span><span class="sxs-lookup"><span data-stu-id="df444-130">Exchange Online Protection</span></span> |
| <span data-ttu-id="df444-131">Ise</span><span class="sxs-lookup"><span data-stu-id="df444-131">SB</span></span> | <span data-ttu-id="df444-132">Skype Kurumsal Çevrimiçi (eski adıyla Lync Online)</span><span class="sxs-lookup"><span data-stu-id="df444-132">Skype for Business Online (formerly Lync Online)</span></span> |
| <span data-ttu-id="df444-133">İşletim Sistemi</span><span class="sxs-lookup"><span data-stu-id="df444-133">OS</span></span> | <span data-ttu-id="df444-134">Office aboneliği</span><span class="sxs-lookup"><span data-stu-id="df444-134">Office Subscription</span></span> |
| <span data-ttu-id="df444-135">PB</span><span class="sxs-lookup"><span data-stu-id="df444-135">PB</span></span> | <span data-ttu-id="df444-136">Office 365 için Power BI</span><span class="sxs-lookup"><span data-stu-id="df444-136">Power BI for Office 365</span></span> |
| <span data-ttu-id="df444-137">SP2</span><span class="sxs-lookup"><span data-stu-id="df444-137">SP</span></span> | <span data-ttu-id="df444-138">SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="df444-138">SharePoint Online</span></span> |
| <span data-ttu-id="df444-139">ASKıYA</span><span class="sxs-lookup"><span data-stu-id="df444-139">YA</span></span> | <span data-ttu-id="df444-140">Yammer Kurumsal</span><span class="sxs-lookup"><span data-stu-id="df444-140">Yammer Enterprise</span></span> |
| <span data-ttu-id="df444-141">MO</span><span class="sxs-lookup"><span data-stu-id="df444-141">MO</span></span> | <span data-ttu-id="df444-142">Portal hatası</span><span class="sxs-lookup"><span data-stu-id="df444-142">Portal error</span></span> |

### <a name="submit-sla-credit-request"></a><span data-ttu-id="df444-143">SLA kredi isteği gönder</span><span class="sxs-lookup"><span data-stu-id="df444-143">Submit SLA credit request</span></span>

<span data-ttu-id="df444-144">SLA kredi isteğinizi Iş Ortağı Merkezi panosu üzerinden Microsoft 'a göndermek için:</span><span class="sxs-lookup"><span data-stu-id="df444-144">To submit your SLA credit request to Microsoft through the Partner Center dashboard:</span></span>

1. <span data-ttu-id="df444-145">Iş Ortağı Merkezi panosunda oturum açın.</span><span class="sxs-lookup"><span data-stu-id="df444-145">Sign in to the Partner Center dashboard.</span></span>
2. <span data-ttu-id="df444-146">Sol taraftaki menüde **hizmet istekleri** ' ni seçin ve **iş ortağı destek istekleri** ' ni seçin.</span><span class="sxs-lookup"><span data-stu-id="df444-146">In the left-hand menu, choose **Service requests** , then select **Partner support requests** .</span></span>
3. <span data-ttu-id="df444-147">**Iş ortağı isteği** sayfasında, **yeni istek** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="df444-147">On the **Partner request** page, choose **New request** .</span></span>
4. <span data-ttu-id="df444-148">**Isteği Başlat** sayfasında, **CSP-müşteriler, siparişler ve abonelikler** bölümünü bulun.</span><span class="sxs-lookup"><span data-stu-id="df444-148">On the **Start the request** page, find the section **CSP - customers, orders and subscriptions** .</span></span> <span data-ttu-id="df444-149">Bu bölümde, **bir sorun türü seçin** ' i seçin ve ardından **Müşteri Hizmetleri kredi istekleri** ' ni seçin.</span><span class="sxs-lookup"><span data-stu-id="df444-149">In this section, choose **Select an issue type** , then select **Customer services credit requests** .</span></span>
5. <span data-ttu-id="df444-150">**Önerilen çözümler** sayfasında, **daha fazla yardıma mı ihtiyacınız var?** altında **Evet** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="df444-150">On the **Recommended solutions** page, under **Do you need more help?** , choose **Yes** .</span></span>
6. <span data-ttu-id="df444-151">**Ayrıntılar** sayfasında, **Sorun ayrıntıları** bölümünü doldurun.</span><span class="sxs-lookup"><span data-stu-id="df444-151">On the **Details** page, fill out the **Issue details** section.</span></span> <span data-ttu-id="df444-152">**Ayrıntılar** metin kutusunda, daha önce topladığınız [gerekli bilgileri](#required-information) girdiğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="df444-152">In the **Details** text box, be sure to enter the [required information](#required-information) that you gathered earlier.</span></span>
7. <span data-ttu-id="df444-153">SLA kredi isteğiniz içinde göndermek için **Gönder** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="df444-153">Choose **Submit** to send in your SLA credit request.</span></span>
