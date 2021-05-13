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
ms.openlocfilehash: 9526a47d0b6d734bde48f403c11fa84d734511c1
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856109"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a><span data-ttu-id="5551e-104">Microsoft 365 ve Dynamics 365 için Kayıt Talebi İş Ortağı (CPOR) modeli aracılığıyla müşteri ilişkilendirmeleri</span><span class="sxs-lookup"><span data-stu-id="5551e-104">Customer associations via the Claimed Partner of Record (CPOR) model for Microsoft 365 and Dynamics 365</span></span>


<span data-ttu-id="5551e-105">**Uygun roller:** Teşvikler yöneticisi</span><span class="sxs-lookup"><span data-stu-id="5551e-105">**Appropriate roles**: Incentives admin</span></span>

<span data-ttu-id="5551e-106">1 Ekim 2019'da Microsoft, Çevrimiçi Hizmetler Danışmanlığı (OSA) Satış, Çevrimiçi Hizmet Kullanımı (OSU)-Microsoft 365 ve OSU-Business Uygulama teşvikleri konusunda Microsoft 365 ve Dynamics 365 müşterilerinizle olan ilişkilendirmelerinizi yönetmek için Talepte Bulunan Kayıtlı İş Ortağı (CPOR) modelini kullanmaya başladı.</span><span class="sxs-lookup"><span data-stu-id="5551e-106">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regard to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365, and OSU-Business Application incentives.</span></span>

>[!Important]
> <span data-ttu-id="5551e-107">Müşteri İlişkisi (CPOR) talepleri yalnızca Çevrimiçi Hizmetler Danışmanlığı (OSA) Satış, Çevrimiçi Hizmet Kullanımı (OSU)-Microsoft 365 ve OSU-Business Uygulama teşvik programları için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="5551e-107">Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="5551e-108">Bulut Çözümü Sağlayıcısı, Managed Reseller, Hosting veya Surface gibi başka bir program için ortak çalışma talebi göndererek burada açıklanan Ortak çalışma talep süreci'ne bakın.</span><span class="sxs-lookup"><span data-stu-id="5551e-108">If you are submitting a co-op claim for another program such as Cloud Solution Provider, Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span> <br><br><span data-ttu-id="5551e-109">Talebinizi gönderdiğinizde Microsoft bunu doğrular.</span><span class="sxs-lookup"><span data-stu-id="5551e-109">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="5551e-110">Bu noktada sizden daha fazla bilgi istememiz gerekir.</span><span class="sxs-lookup"><span data-stu-id="5551e-110">We may ask you for more information at this point.</span></span> <span data-ttu-id="5551e-111">Ayrıca ilişkilendirme isteğinizi müşteriye bildirerek.</span><span class="sxs-lookup"><span data-stu-id="5551e-111">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="5551e-112">Müşterilerin geri almak için beş iş günü vardır. Kabul etmezlerse, bu kiracıyla ve iş yüküyle olan ilişkilendirmeniz resmi olur.</span><span class="sxs-lookup"><span data-stu-id="5551e-112">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="5551e-113">Bu noktada müşterinin kullanım verilerine erişebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5551e-113">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="5551e-114">Talebi tamamlamak için aşağıdaki bilgilere ihtiyacınız olacak:</span><span class="sxs-lookup"><span data-stu-id="5551e-114">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="5551e-115">Talebi **yapan varlığınız** için MPN kimliği</span><span class="sxs-lookup"><span data-stu-id="5551e-115">The **MPN ID** for your entity that makes the claim</span></span>

- <span data-ttu-id="5551e-116">Müşterinin etki **alanı adı** Bunu [bulun](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="5551e-116">Customer's **domain name** [Find this](find-ids-and-domain-names.md)</span></span>

- <span data-ttu-id="5551e-117">Müşterinin Dizin **Kimliği veya** Kiracı **Kimliği** Bunu [bulun](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="5551e-117">Customer's **Directory ID** or **Tenant ID** [Find this](find-ids-and-domain-names.md)</span></span>

- <span data-ttu-id="5551e-118">Çözüm **alanı**, örneğin Business Applications veya Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="5551e-118">The **Solution area**, such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="5551e-119">**Gerçekleştirilen** Etkinlik ve satış öncesi, Kullanım veya Gelir ilişkilendirmesi gibi yapmak istediğiniz talep türü</span><span class="sxs-lookup"><span data-stu-id="5551e-119">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="5551e-120">Müşterinizin Kişi **adı,** başlığı ve e-posta adresi</span><span class="sxs-lookup"><span data-stu-id="5551e-120">Your customer's **Contact name**, title, and email address</span></span>

- <span data-ttu-id="5551e-121">Dynamics 365 için müşterinizin Teknik iletişim  adını, başlığını ve e-posta adresini de sağlayabilirsiniz</span><span class="sxs-lookup"><span data-stu-id="5551e-121">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="5551e-122">Kendi şirketinizin **kişi adı** ve e-posta adresi</span><span class="sxs-lookup"><span data-stu-id="5551e-122">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="5551e-123">Bu talep için bir **ad** oluşturacaksınız</span><span class="sxs-lookup"><span data-stu-id="5551e-123">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="5551e-124">Seçtiğiniz **ürün (ler)** veya iş yükleri</span><span class="sxs-lookup"><span data-stu-id="5551e-124">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="5551e-125">Müşteri tarafından imzalanan iş beyanı gibi **yürütme kanıtı (PoE)**.</span><span class="sxs-lookup"><span data-stu-id="5551e-125">**Proof of execution (PoE)**, such as a statement of work signed by the customer.</span></span> <span data-ttu-id="5551e-126">Ayrıca, kullanmak üzere bir PoE şablonu indirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5551e-126">You can also download a PoE template to use.</span></span>

- <span data-ttu-id="5551e-127">İş ortakları yalnızca gelir ilişkilendirmesini talep etmek için: **Dynamics çözüm satıcı adı**, **MÜŞTERI adı** ve **ISV ürün/çözüm adı**.</span><span class="sxs-lookup"><span data-stu-id="5551e-127">For partners claiming revenue association only: **Dynamics solution seller name**, **Customer name**, and **Name of ISV product/solution**.</span></span> 

<span data-ttu-id="5551e-128">Ayrıca aşağıdaki noktaları da anlamanız gerekir:</span><span class="sxs-lookup"><span data-stu-id="5551e-128">You should also understand the following points:</span></span>

- <span data-ttu-id="5551e-129">Mevcut Microsoft 365 müşterileriniz varsa, bu işlemi kullanarak OSU teşvikleri kazanmak için devam etmek istediğinize yeniden ilişkilendirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="5551e-129">If you have existing Microsoft 365 customers, you'll need to re-associate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="5551e-130">Dynamics 365 veya Power BI müşterilerle mevcut ilişkilendirmeleriniz varsa, bu ilişkilendirmeler aboneliklerinin süresi dolmadan geçerli olmaya devam eder.</span><span class="sxs-lookup"><span data-stu-id="5551e-130">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="5551e-131">Müşterinin birden çok iş ortağı olabilir, ancak her iş yükü (OSU-Microsoft 365 için) veya abonelik (OSA-Sell ve OSU-Business uygulamalar için) yalnızca bir ortağıyla ilişkilendirilebilir.</span><span class="sxs-lookup"><span data-stu-id="5551e-131">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="5551e-132">Müşteri ilişkilendirmesi oluşturma</span><span class="sxs-lookup"><span data-stu-id="5551e-132">Create a customer association</span></span>

1. <span data-ttu-id="5551e-133">[İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="5551e-133">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="5551e-134">**Teşvikleri** sekmesini seçin, **genel bakış**' ı seçin ve ardından **Müşteri ilişkilendirmeleri**' ni seçin.</span><span class="sxs-lookup"><span data-stu-id="5551e-134">Select the **Incentives** tab, select **Overview**, and then select **Customer associations**.</span></span>

3. <span data-ttu-id="5551e-135">Müşteri ilişkilendirmeleri sayfasının en üstünde **+ müşteri ilişkisi**' nı seçin.</span><span class="sxs-lookup"><span data-stu-id="5551e-135">At the top of the Customer associations page, select **+ Customer association**.</span></span>

4. <span data-ttu-id="5551e-136">Müşteriyle ilişkilendirilecek iş ortağı konumunun **MPN kimliğini** seçip müşterinin etki alanı adını ve dizin kimliğini ekleyin.</span><span class="sxs-lookup"><span data-stu-id="5551e-136">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="5551e-137">Bunu bulun</span><span class="sxs-lookup"><span data-stu-id="5551e-137">Find this</span></span>](find-ids-and-domain-names.md)

5. <span data-ttu-id="5551e-138">**Devam**’ı seçin.</span><span class="sxs-lookup"><span data-stu-id="5551e-138">Select **Continue**.</span></span>

6. <span data-ttu-id="5551e-139">**Çözüm alanını** ve **etkinliği** seçin.</span><span class="sxs-lookup"><span data-stu-id="5551e-139">Select the **Solution area** and **Activity**.</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="5551e-140">Business Applications ' yi seçerseniz, **kullanım ve/veya satış öncesi** ya da **gelir ilişkilendirmesini** seçin ve ardından **devam**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="5551e-140">If you select Business Applications, select either **Usage and/or Pre-sales**, or **Revenue association**, and then select **Continue**.</span></span> 
   <br><br><span data-ttu-id="5551e-141">Gelir ilişkilendirmesini seçerseniz aşağıda listelenenlerden biraz farklı bilgiler istenir.</span><span class="sxs-lookup"><span data-stu-id="5551e-141">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

7. <span data-ttu-id="5551e-142">**Müşteri ilişkilendir** sayfasında uygun bilgileri girin ve **Talep Oluştur**' u seçin.</span><span class="sxs-lookup"><span data-stu-id="5551e-142">Enter the appropriate information on the **Associate customer** page, and then select **Create claim**.</span></span>

8. <span data-ttu-id="5551e-143">Bu müşteri ilişkisiyle ilişkili ürünleri seçin ve ardından **devam**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="5551e-143">Select the product(s) associated with this customer association, and then select **Continue**.</span></span>

9. <span data-ttu-id="5551e-144">Müşterinin ve şirketinizin iletişim bilgilerini girin.</span><span class="sxs-lookup"><span data-stu-id="5551e-144">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="5551e-145">Tüm alanlar zorunludur.</span><span class="sxs-lookup"><span data-stu-id="5551e-145">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="5551e-146">Ürününüz Dynamics 365 ise ve seçtiğiniz üründe bu müşteri için birden çok abonelik varsa, abonelik KIMLIĞINI de girmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="5551e-146">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

10. <span data-ttu-id="5551e-147">Yürütme kanıtı (PoE) sağlayın.</span><span class="sxs-lookup"><span data-stu-id="5551e-147">Supply your proof of execution (PoE).</span></span> <span data-ttu-id="5551e-148">Bunu kutuya sürükleyebilir, kendi destekleyici belgelerinize göz atabilir veya **Şablonu indir**'i seçerek bir şablon kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5551e-148">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template**.</span></span> 

11. <span data-ttu-id="5551e-149">İsteğe bağlı olarak açıklama ekleyip kaydedin ve ardından **Talebi gönder**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="5551e-149">Add and save comments if you like, and then select **Submit claim**.</span></span> <span data-ttu-id="5551e-150">Müşteriye, müşteri ilişkilendirmenizi onaylamanızı isteyen bir e-posta göndereceğiz.</span><span class="sxs-lookup"><span data-stu-id="5551e-150">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="5551e-151">Müşteri ilişkilendirmesini gönderdikten sonra düzenleyemezsiniz.</span><span class="sxs-lookup"><span data-stu-id="5551e-151">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="5551e-152">Müşteri ilişkilendirmenizin durumu, **Durum** alanında görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="5551e-152">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="5551e-153">Bir müşteri ilişkilendirmesinin geçmişini görüntülemek için **Geçmiş**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="5551e-153">Select **History** to view the history of a customer association.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5551e-154">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="5551e-154">Next steps</span></span>

- [<span data-ttu-id="5551e-155">Müşteri ilişkilendirmelerini yönetme</span><span class="sxs-lookup"><span data-stu-id="5551e-155">Manage customer associations</span></span>](incentives-manage-customer-associations.md)