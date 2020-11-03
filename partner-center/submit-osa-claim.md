---
title: Müşteri ilişkilendirmesi oluşturma
ms.topic: article
ms.date: 09/11/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Kayıt (CPOR) modelinin talep ortağı ile müşteri ilişkilendirmeleri oluşturun. Microsoft 365 & Dynamics 365 müşterileri için Sales, Usage, teşvikleri yönetimine yardımcı olur.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e34698b51a159445f4354e366f79f510533e6f30
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/19/2020
ms.locfileid: "92531999"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a><span data-ttu-id="14344-104">Microsoft 365 ve Dynamics 365 için Istenen kayıt ortağı (CPOR) modeli aracılığıyla müşteri ilişkilendirmeleri</span><span class="sxs-lookup"><span data-stu-id="14344-104">Customer associations via the Claimed Partner of Record (CPOR) model for Microsoft 365 and Dynamics 365</span></span>

<span data-ttu-id="14344-105">**Uygulama hedefi**</span><span class="sxs-lookup"><span data-stu-id="14344-105">**Applies to**</span></span>

- <span data-ttu-id="14344-106">İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="14344-106">Partner Center</span></span>

<span data-ttu-id="14344-107">**Uygun roller:**</span><span class="sxs-lookup"><span data-stu-id="14344-107">**Appropriate roles:**</span></span>

- <span data-ttu-id="14344-108">Teşvikleri Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="14344-108">Incentives admin</span></span>

<span data-ttu-id="14344-109">Microsoft, 1 Ekim 2019 ' de, Microsoft 365 sahip olduğunuz ilişkileri yönetmek için kayıt ortağı (CPOR) modelini kullanmaya başlamıştır 365 ve bu, çevrimiçi hizmetler danışmanlığı (OSA) satışı, çevrimiçi hizmetler kullanımı (OSU)-Microsoft 365 ve OSU-Business Application teşvikleri.</span><span class="sxs-lookup"><span data-stu-id="14344-109">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regards to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentives.</span></span>

>[!Important]
> <span data-ttu-id="14344-110">Müşteri Birliği (CPOR) talepleri yalnızca çevrimiçi hizmetler Danışma belgesi (OSA) satışı, çevrimiçi hizmetler kullanımı (OSU)-Microsoft 365 ve OSU-Business uygulama teşvik programları için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="14344-110">Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="14344-111">Bulut çözümü sağlayıcısı, yönetilen satıcı, barındırma veya yüzey gibi başka bir program için bir ortak op talebi gönderiyorsanız, lütfen burada özetlenen ortak op talep işlemine bakın.</span><span class="sxs-lookup"><span data-stu-id="14344-111">If you are submitting a co-op claim for another program such as Cloud Solution Provider, Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span> <br><br><span data-ttu-id="14344-112">Talep gönderdiğinizde, Microsoft onu doğrular.</span><span class="sxs-lookup"><span data-stu-id="14344-112">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="14344-113">Bu noktada daha fazla bilgi isteyeceğiz.</span><span class="sxs-lookup"><span data-stu-id="14344-113">We may ask you for more information at this point.</span></span> <span data-ttu-id="14344-114">İlişki isteğinizin müşterisini de bilgilendireceğiz.</span><span class="sxs-lookup"><span data-stu-id="14344-114">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="14344-115">Müşterilerin kabul etmek için beş iş günü vardır. Devre dışı kalmazsanız, bu belirli kiracı ve iş yüküyle olan ilişkilendirmeniz resmi olur.</span><span class="sxs-lookup"><span data-stu-id="14344-115">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="14344-116">Bu noktada müşterinin kullanım verilerine erişebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="14344-116">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="14344-117">Bir talebi tamamlayabilmeniz için aşağıdaki bilgilere ihtiyacınız vardır:</span><span class="sxs-lookup"><span data-stu-id="14344-117">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="14344-118">Varlığınızın, talebi yapan **MPN kimliği**</span><span class="sxs-lookup"><span data-stu-id="14344-118">The **MPN ID** for your entity that makes the claim</span></span>

- <span data-ttu-id="14344-119">Müşterinin **etki alanı adı** [bunu bulun](find-domain-name.md)</span><span class="sxs-lookup"><span data-stu-id="14344-119">Customer's **domain name** [Find this](find-domain-name.md)</span></span>

- <span data-ttu-id="14344-120">Müşterinin **DIZIN kimliği** veya **Kiracı kimliği** şunu [bulun](find-domain-name.md)</span><span class="sxs-lookup"><span data-stu-id="14344-120">Customer's **Directory ID** or **Tenant ID** [Find this](find-domain-name.md)</span></span>

- <span data-ttu-id="14344-121">Business Applications veya Microsoft 365 gibi **çözüm alanı**</span><span class="sxs-lookup"><span data-stu-id="14344-121">The **Solution area** , such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="14344-122">Gerçekleştirdiğiniz **etkinlik** ve satış öncesi, kullanım veya gelir ilişkisi gibi yapmak istediğiniz talep türü</span><span class="sxs-lookup"><span data-stu-id="14344-122">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="14344-123">Müşterinizin **kişi adı** , başlığı ve e-posta adresi</span><span class="sxs-lookup"><span data-stu-id="14344-123">Your customer's **Contact name** , title, and email address</span></span>

- <span data-ttu-id="14344-124">Dynamics 365 için Ayrıca müşterinizin **teknik iletişim** adı, başlığı ve e-posta adresini sağlamanız gerekir</span><span class="sxs-lookup"><span data-stu-id="14344-124">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="14344-125">Kendi şirketinizin **kişi adı** ve e-posta adresi</span><span class="sxs-lookup"><span data-stu-id="14344-125">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="14344-126">Bu talep için bir **ad** oluşturacaksınız</span><span class="sxs-lookup"><span data-stu-id="14344-126">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="14344-127">Seçtiğiniz **ürün (ler)** veya iş yükleri</span><span class="sxs-lookup"><span data-stu-id="14344-127">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="14344-128">Müşteri tarafından imzalanan iş beyanı gibi **yürütme kanıtı (PoE)** .</span><span class="sxs-lookup"><span data-stu-id="14344-128">**Proof of execution (PoE)** , such as a statement of work signed by the customer.</span></span> <span data-ttu-id="14344-129">Ayrıca, kullanmak üzere bir PoE şablonu indirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="14344-129">You can also download a PoE template to use.</span></span>

- <span data-ttu-id="14344-130">İş ortakları yalnızca gelir ilişkilendirmesini talep etmek için: **Dynamics çözüm satıcı adı** , **MÜŞTERI adı** ve **ISV ürün/çözüm adı** .</span><span class="sxs-lookup"><span data-stu-id="14344-130">For partners claiming revenue association only: **Dynamics solution seller name** , **Customer name** , and **Name of ISV product/solution** .</span></span> 

<span data-ttu-id="14344-131">Ayrıca aşağıdaki noktaları da anlamanız gerekir:</span><span class="sxs-lookup"><span data-stu-id="14344-131">You should also understand the following points:</span></span>

- <span data-ttu-id="14344-132">Mevcut Microsoft 365 müşterileriniz varsa, bu işlemi kullanarak OSU teşvikleri kazanmak için devam etmek istediğinize yeniden ilişkilendirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="14344-132">If you have existing Microsoft 365 customers, you'll need to re-associate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="14344-133">Dynamics 365 veya Power BI müşterilerle mevcut ilişkilendirmeleriniz varsa, bu ilişkilendirmeler aboneliklerinin süresi dolmadan geçerli olmaya devam eder.</span><span class="sxs-lookup"><span data-stu-id="14344-133">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="14344-134">Müşterinin birden çok iş ortağı olabilir, ancak her iş yükü (OSU-Microsoft 365 için) veya abonelik (OSA-Sell ve OSU-Business uygulamalar için) yalnızca bir ortağıyla ilişkilendirilebilir.</span><span class="sxs-lookup"><span data-stu-id="14344-134">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="14344-135">Müşteri ilişkilendirmesi oluşturma</span><span class="sxs-lookup"><span data-stu-id="14344-135">Create a customer association</span></span>

1. <span data-ttu-id="14344-136">[İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="14344-136">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="14344-137">**Teşvikleri** sekmesini seçin, **genel bakış** ' ı seçin ve ardından **Müşteri ilişkilendirmeleri** ' ni seçin.</span><span class="sxs-lookup"><span data-stu-id="14344-137">Select the **Incentives** tab, select **Overview** , and then select **Customer associations** .</span></span>

3. <span data-ttu-id="14344-138">Müşteri ilişkilendirmeleri sayfasının en üstünde **+ müşteri ilişkisi** ' nı seçin.</span><span class="sxs-lookup"><span data-stu-id="14344-138">At the top of the Customer associations page, select **+ Customer association** .</span></span>

4. <span data-ttu-id="14344-139">Müşteriyle ilişkilendirilecek iş ortağı konumunun **MPN kimliğini** seçip müşterinin etki alanı adını ve dizin kimliğini ekleyin.</span><span class="sxs-lookup"><span data-stu-id="14344-139">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="14344-140">Bunu bulun</span><span class="sxs-lookup"><span data-stu-id="14344-140">Find this</span></span>](find-domain-name.md)

5. <span data-ttu-id="14344-141">**Devam** ’ı seçin.</span><span class="sxs-lookup"><span data-stu-id="14344-141">Select **Continue** .</span></span>

6. <span data-ttu-id="14344-142">**Çözüm alanını** ve **etkinliği** seçin.</span><span class="sxs-lookup"><span data-stu-id="14344-142">Select the **Solution area** and **Activity** .</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="14344-143">Business Applications ' yi seçerseniz, **kullanım ve/veya satış öncesi** ya da **gelir ilişkilendirmesini** seçin ve ardından **devam** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="14344-143">If you select Business Applications, select either **Usage and/or Pre-sales** , or **Revenue association** , and then select **Continue** .</span></span> 
   <br><br><span data-ttu-id="14344-144">Gelir ilişkilendirmesini seçerseniz aşağıda listelenenlerden biraz farklı bilgiler istenir.</span><span class="sxs-lookup"><span data-stu-id="14344-144">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

7. <span data-ttu-id="14344-145">**Müşteri ilişkilendir** sayfasında uygun bilgileri girin ve **Talep Oluştur** ' u seçin.</span><span class="sxs-lookup"><span data-stu-id="14344-145">Enter the appropriate information on the **Associate customer** page, and then select **Create claim** .</span></span>

8. <span data-ttu-id="14344-146">Bu müşteri ilişkisiyle ilişkili ürünleri seçin ve ardından **devam** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="14344-146">Select the product(s) associated with this customer association, and then select **Continue** .</span></span>

9. <span data-ttu-id="14344-147">Müşterinin ve şirketinizin iletişim bilgilerini girin.</span><span class="sxs-lookup"><span data-stu-id="14344-147">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="14344-148">Tüm alanlar zorunludur.</span><span class="sxs-lookup"><span data-stu-id="14344-148">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="14344-149">Ürününüz Dynamics 365 ise ve seçtiğiniz üründe bu müşteri için birden çok abonelik varsa, abonelik KIMLIĞINI de girmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="14344-149">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

10. <span data-ttu-id="14344-150">Yürütme kanıtı (PoE) sağlayın.</span><span class="sxs-lookup"><span data-stu-id="14344-150">Supply your proof of execution (PoE).</span></span> <span data-ttu-id="14344-151">Bunu kutuya sürükleyebilir, kendi destekleyici belgelerinize göz atabilir veya **Şablonu indir** 'i seçerek bir şablon kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="14344-151">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template** .</span></span> 

11. <span data-ttu-id="14344-152">İsteğe bağlı olarak açıklama ekleyip kaydedin ve ardından **Talebi gönder** 'i seçin.</span><span class="sxs-lookup"><span data-stu-id="14344-152">Add and save comments if you like, and then select **Submit claim** .</span></span> <span data-ttu-id="14344-153">Müşteriye, müşteri ilişkilendirmenizi onaylamanızı isteyen bir e-posta göndereceğiz.</span><span class="sxs-lookup"><span data-stu-id="14344-153">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="14344-154">Müşteri ilişkilendirmesini gönderdikten sonra düzenleyemezsiniz.</span><span class="sxs-lookup"><span data-stu-id="14344-154">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="14344-155">Müşteri ilişkilendirmenizin durumu, **Durum** alanında görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="14344-155">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="14344-156">Bir müşteri ilişkilendirmesinin geçmişini görüntülemek için **Geçmiş** 'i seçin.</span><span class="sxs-lookup"><span data-stu-id="14344-156">Select **History** to view the history of a customer association.</span></span>

## <a name="next-steps"></a><span data-ttu-id="14344-157">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="14344-157">Next steps</span></span>

- [<span data-ttu-id="14344-158">Müşteri ilişkilendirmelerini yönetme</span><span class="sxs-lookup"><span data-stu-id="14344-158">Manage customer associations</span></span>](incentives-manage-customer-associations.md)