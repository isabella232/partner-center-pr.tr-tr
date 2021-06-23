---
title: Müşteri ilişkilendirmesi oluşturma
ms.topic: article
ms.date: 10/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Talepte Bulunan Kayıtlı İş Ortağı (CPOR) modeliyle müşteri ilişkilendirmeleri oluşturun. Dynamics 365 müşterileri için satış, Microsoft 365 & teşviklerin yönetimine yardımcı olur.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 196009d9271324377be02d0b2d12ba8a4d7a993c
ms.sourcegitcommit: 09eabb559aae25518caf3f2a59ef16a3e123c207
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/23/2021
ms.locfileid: "112489960"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a><span data-ttu-id="5b500-104">Microsoft 365 ve Dynamics 365 için Kayıt İş Ortağı (CPOR) modeli aracılığıyla müşteri ilişkilendirmeleri</span><span class="sxs-lookup"><span data-stu-id="5b500-104">Customer associations via the Claimed Partner of Record (CPOR) model for Microsoft 365 and Dynamics 365</span></span>


<span data-ttu-id="5b500-105">**Uygun roller:** Teşvikler yöneticisi</span><span class="sxs-lookup"><span data-stu-id="5b500-105">**Appropriate roles**: Incentives admin</span></span>

<span data-ttu-id="5b500-106">1 Ekim 2019'da Microsoft, Çevrimiçi Hizmetler Danışmanlığı (OSA) Satış, Çevrimiçi Hizmet Kullanımı (OSU)-Microsoft 365 ve OSU-Business Uygulama teşvikleri konusunda Microsoft 365 ve Dynamics 365 müşterilerinizle olan ilişkilendirmelerinizi yönetmek için Talepte Bulunan Kayıtlı İş Ortağı (CPOR) modelini kullanmaya başladı.</span><span class="sxs-lookup"><span data-stu-id="5b500-106">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regard to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365, and OSU-Business Application incentives.</span></span>

>[!Important]
> <span data-ttu-id="5b500-107">Müşteri İlişkisi (CPOR) talepleri yalnızca Çevrimiçi Hizmetler Danışmanlığı (OSA) Satış, Çevrimiçi Hizmet Kullanımı (OSU)-Microsoft 365 ve OSU-Business Uygulama teşvik programları için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="5b500-107">Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="5b500-108">Bulut Çözümü Sağlayıcısı (CSP), Managed Reseller, Hosting veya Surface gibi başka bir program için bir ortak çalışma talebi göndererek burada özetlenen Ortak çalışma talep süreci'ne bakın.</span><span class="sxs-lookup"><span data-stu-id="5b500-108">If you are submitting a co-op claim for another program such as Cloud Solution Provider (CSP), Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span> <br><br><span data-ttu-id="5b500-109">Talebinizi gönderdiğinizde Microsoft bunu doğrular.</span><span class="sxs-lookup"><span data-stu-id="5b500-109">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="5b500-110">Bu noktada sizden daha fazla bilgi istememiz gerekir.</span><span class="sxs-lookup"><span data-stu-id="5b500-110">We may ask you for more information at this point.</span></span> <span data-ttu-id="5b500-111">Ayrıca müşteriye ilişkilendirme isteğinizi bildirerek.</span><span class="sxs-lookup"><span data-stu-id="5b500-111">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="5b500-112">Müşterilerin geri almak için beş iş günü vardır. Kabul etmezlerse, bu kiracıyla ve iş yüküyle olan ilişkilendirmeniz resmi olur.</span><span class="sxs-lookup"><span data-stu-id="5b500-112">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="5b500-113">Bu noktada müşterinin kullanım verilerine erişebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5b500-113">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="5b500-114">Talebi tamamlamak için aşağıdaki bilgilere ihtiyacınız olacak:</span><span class="sxs-lookup"><span data-stu-id="5b500-114">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="5b500-115">Talebi **yapan varlığınız** için MPN kimliği (Microsoft İş Ortağı Ağı kimliği)</span><span class="sxs-lookup"><span data-stu-id="5b500-115">The **MPN ID** (Microsoft Partner Network ID) for your entity that makes the claim</span></span>

- <span data-ttu-id="5b500-116">Müşterinin etki **alanı adı (daha** fazla bilgi için bkz. [Kiracı kimliğini, etki alanı adını, kullanıcı nesne kimliğini bulma)](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="5b500-116">Customer's **domain name** (for more information, see [Find tenant ID, domain name, user object ID](find-ids-and-domain-names.md))</span></span>

- <span data-ttu-id="5b500-117">Müşterinin Dizin **Kimliği veya Kiracı** Kimliği **(daha** fazla bilgi için bkz. [Kiracı kimliğini, etki alanı adını, kullanıcı nesne kimliğini bulma)](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="5b500-117">Customer's **Directory ID** or **Tenant ID** (for more information, see [Find tenant ID, domain name, user object ID](find-ids-and-domain-names.md))</span></span>

- <span data-ttu-id="5b500-118">Çözüm **alanı**, örneğin Business Applications veya Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="5b500-118">The **Solution area**, such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="5b500-119">**Gerçekleştirilen** Etkinlik ve satış öncesi, Kullanım veya Gelir ilişkilendirmesi gibi yapmak istediğiniz talep türü</span><span class="sxs-lookup"><span data-stu-id="5b500-119">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="5b500-120">Müşterinizin Kişi **adı,** başlığı ve e-posta adresi</span><span class="sxs-lookup"><span data-stu-id="5b500-120">Your customer's **Contact name**, title, and email address</span></span>

- <span data-ttu-id="5b500-121">Dynamics 365 için müşterinizin Teknik iletişim  adını, başlığını ve e-posta adresini de sağlayabilirsiniz</span><span class="sxs-lookup"><span data-stu-id="5b500-121">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="5b500-122">Kendi şirketinizin Kişi **adı ve e-posta** adresi</span><span class="sxs-lookup"><span data-stu-id="5b500-122">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="5b500-123">Bu talep için **bir Ad** oluştur</span><span class="sxs-lookup"><span data-stu-id="5b500-123">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="5b500-124">**Talepte bulundurarak** ürün veya iş yükleri</span><span class="sxs-lookup"><span data-stu-id="5b500-124">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="5b500-125">Müşteri tarafından imzalanan iş bildirimi gibi yürütme kanıtı **(PoE).**</span><span class="sxs-lookup"><span data-stu-id="5b500-125">**Proof of execution (PoE)**, such as a statement of work signed by the customer.</span></span> <span data-ttu-id="5b500-126">Ayrıca kullanmak üzere bir PoE şablonu indirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5b500-126">You can also download a PoE template to use.</span></span>

- <span data-ttu-id="5b500-127">Yalnızca gelir ilişkilendirmesi talep eden iş ortakları için: **Dynamics çözüm satıcısı adı,** Müşteri **adı** ve **ISV ürününün/çözümünün adı.**</span><span class="sxs-lookup"><span data-stu-id="5b500-127">For partners claiming revenue association only: **Dynamics solution seller name**, **Customer name**, and **Name of ISV product/solution**.</span></span> 

<span data-ttu-id="5b500-128">Ayrıca aşağıdaki noktaları da anlamalısınız:</span><span class="sxs-lookup"><span data-stu-id="5b500-128">You should also understand the following points:</span></span>

- <span data-ttu-id="5b500-129">Mevcut Microsoft 365 müşteriniz varsa, bu süreci kullanarak OSU teşvikleri kazanmaya devam etmek istediğiniz müşterilerle yeniden ilişkilendirilmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="5b500-129">If you have existing Microsoft 365 customers, you'll need to reassociate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="5b500-130">Dynamics 365 veya Power BI mevcut ilişkilendirmeniz varsa, bu ilişkilendirmeler aboneliklerinin süresi sona erinceye kadar geçerli kalır.</span><span class="sxs-lookup"><span data-stu-id="5b500-130">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="5b500-131">Müşterinin birden çok iş ortağı olabilir, ancak her iş yükü (OSU-Microsoft 365 için) veya abonelik (OSA-Sell ve OSU-Business Uygulamaları için) yalnızca bir iş ortağıyla ilişkilendirilebilir.</span><span class="sxs-lookup"><span data-stu-id="5b500-131">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="5b500-132">Müşteri ilişkilendirmesi oluşturma</span><span class="sxs-lookup"><span data-stu-id="5b500-132">Create a customer association</span></span>

1. <span data-ttu-id="5b500-133">[İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="5b500-133">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="5b500-134">Teşvikler **sekmesini,** Genel **Bakış'ı ve** ardından Müşteri **ilişkilendirmeleri'ne tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="5b500-134">Select the **Incentives** tab, select **Overview**, and then select **Customer associations**.</span></span>

3. <span data-ttu-id="5b500-135">Müşteri ilişkilendirmeleri sayfasının üst kısmında + Müşteri **ilişkilendirme'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="5b500-135">At the top of the Customer associations page, select **+ Customer association**.</span></span>

4. <span data-ttu-id="5b500-136">Müşteriyle ilişkilendirilecek iş ortağı konumunun **MPN kimliğini** seçip müşterinin etki alanı adını ve dizin kimliğini ekleyin.</span><span class="sxs-lookup"><span data-stu-id="5b500-136">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="5b500-137">Bunu bulun</span><span class="sxs-lookup"><span data-stu-id="5b500-137">Find this</span></span>](find-ids-and-domain-names.md)

5. <span data-ttu-id="5b500-138">**Devam**’ı seçin.</span><span class="sxs-lookup"><span data-stu-id="5b500-138">Select **Continue**.</span></span>

6. <span data-ttu-id="5b500-139">Çözüm alanı **ve Etkinlik'i** **seçin.**</span><span class="sxs-lookup"><span data-stu-id="5b500-139">Select the **Solution area** and **Activity**.</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="5b500-140">Bir satış Business Applications, Kullanım **ve/veya** Satış Öncesi veya Gelir ilişkilendirmesi'ne ve ardından Devam'ı **seçin.**</span><span class="sxs-lookup"><span data-stu-id="5b500-140">If you select Business Applications, select either **Usage and/or Pre-sales**, or **Revenue association**, and then select **Continue**.</span></span> 
   <br><br><span data-ttu-id="5b500-141">Gelir ilişkilendirmesini seçerseniz aşağıda listelenenlerden biraz farklı bilgiler istenir.</span><span class="sxs-lookup"><span data-stu-id="5b500-141">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

7. <span data-ttu-id="5b500-142">Müşteriyi ilişkilendirme sayfasında uygun **bilgileri girin** ve Talep oluştur'a **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="5b500-142">Enter the appropriate information on the **Associate customer** page, and then select **Create claim**.</span></span>

8. <span data-ttu-id="5b500-143">Bu müşteri ilişkilendirmesi ile ilişkili ürünleri ve ardından Devam'ı **seçin.**</span><span class="sxs-lookup"><span data-stu-id="5b500-143">Select the product(s) associated with this customer association, and then select **Continue**.</span></span>

9. <span data-ttu-id="5b500-144">Müşterinin ve şirketinizin iletişim bilgilerini girin.</span><span class="sxs-lookup"><span data-stu-id="5b500-144">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="5b500-145">Tüm alanlar zorunludur.</span><span class="sxs-lookup"><span data-stu-id="5b500-145">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="5b500-146">Ürününüz Dynamics 365 ise ve seçtiğiniz ürünün bu müşteri için birden çok aboneliği varsa abonelik kimliğini de girmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="5b500-146">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

10. <span data-ttu-id="5b500-147">PoE'nizi teminin.</span><span class="sxs-lookup"><span data-stu-id="5b500-147">Supply your PoE.</span></span> <span data-ttu-id="5b500-148">Bunu kutuya sürükleyebilir, kendi destekleyici belgelerinize göz atabilir veya **Şablonu indir**'i seçerek bir şablon kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5b500-148">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template**.</span></span> 

11. <span data-ttu-id="5b500-149">İsteğe bağlı olarak açıklama ekleyip kaydedin ve ardından **Talebi gönder**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="5b500-149">Add and save comments if you like, and then select **Submit claim**.</span></span> <span data-ttu-id="5b500-150">Müşteriye, müşteri ilişkilendirmenizi onaylamanızı isteyen bir e-posta göndereceğiz.</span><span class="sxs-lookup"><span data-stu-id="5b500-150">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="5b500-151">Müşteri ilişkilendirmenizi gönderdiktan sonra düzenleyemezsiniz.</span><span class="sxs-lookup"><span data-stu-id="5b500-151">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="5b500-152">Müşteri ilişkilendirmenizin durumu, **Durum** alanında görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="5b500-152">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="5b500-153">Bir müşteri ilişkilendirmesinin geçmişini görüntülemek için **Geçmiş**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="5b500-153">Select **History** to view the history of a customer association.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5b500-154">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="5b500-154">Next steps</span></span>

- [<span data-ttu-id="5b500-155">Müşteri ilişkilendirmelerini yönetme</span><span class="sxs-lookup"><span data-stu-id="5b500-155">Manage customer associations</span></span>](incentives-manage-customer-associations.md)