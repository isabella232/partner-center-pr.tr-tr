---
title: Doğrudan fatura ortağını dolaylı satıcıya geçir
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Bir CSP program ortağının doğrudan fatura ortağından dolaylı satıcıya geçiş yapmak için Iş ortağı merkezini nasıl kullanabileceği hakkında bilgi edinin.
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e9ffa6ef8145099a90fde16e4ce8d6a3453973e0
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/22/2020
ms.locfileid: "92531735"
---
# <a name="transition-from-cloud-solution-provider-csp-direct-bill-partner-to-csp-indirect-reseller"></a><span data-ttu-id="4e0fe-103">Bulut Çözümü Sağlayıcısı (CSP) doğrudan faturalanan iş ortağından CSP dolaylı kurumsal bayiye geçiş</span><span class="sxs-lookup"><span data-stu-id="4e0fe-103">Transition from Cloud Solution Provider (CSP) direct bill partner to CSP indirect reseller</span></span>

<span data-ttu-id="4e0fe-104">**Aşağıdakiler cihazlar için geçerlidir:**</span><span class="sxs-lookup"><span data-stu-id="4e0fe-104">**Applies to:**</span></span>

- <span data-ttu-id="4e0fe-105">CSP iş ortakları</span><span class="sxs-lookup"><span data-stu-id="4e0fe-105">CSP partners</span></span>

>[!Note]
><span data-ttu-id="4e0fe-106">Bu makale, dolaylı satıcılara geçişe karar veren doğrudan fatura ortakları için tasarlanmıştır.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-106">This article is intended for direct bill partners who have decided to transition to indirect resellers.</span></span> <span data-ttu-id="4e0fe-107">Ancak dolaylı bir satıcı olarak kaydolmak üzere açık bir karar vermemiş olsanız bile, doğrudan [Fatura özellikleri kısıtlandıktan](restricted-direct-bill-capabilities.md)sonra CSP doğrudan fatura ortağı programı için yeni [gereksinimleri](direct-partner-new-requirements.md) karşılamayan doğrudan fatura iş ortakları Microsoft tarafından bilgilendirilir.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-107">However, even if you have not made an explicit decision yet to enroll as an indirect reseller, direct bill partners who do not meet the new [requirements](direct-partner-new-requirements.md) for the CSP direct bill partner program will be informed by Microsoft when their [direct bill capabilities will be restricted](restricted-direct-bill-capabilities.md).</span></span>

<span data-ttu-id="4e0fe-108">Mevcut doğrudan fatura kiracınızı kullanarak dolaylı satıcı programına kayıt yapabileceksiniz.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-108">You will be able to enroll in the indirect reseller program using your existing direct bill tenant.</span></span>

## <a name="get-started"></a><span data-ttu-id="4e0fe-109">başlarken</span><span class="sxs-lookup"><span data-stu-id="4e0fe-109">Get started</span></span>

1. <span data-ttu-id="4e0fe-110">Iş ortağı merkezi ve MPN KIMLIĞI 'ndeki iş ortağı profilinizin güncel olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-110">Make sure your partner profile in Partner Center and MPN ID are current.</span></span>

2. <span data-ttu-id="4e0fe-111">Dolaylı satıcıya geçiş yaptığınız doğrudan fatura kiracının genel yöneticisi olarak Iş Ortağı Merkezi ' nde oturum açın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-111">Sign in to Partner Center as the global admin for the direct bill tenant you are transitioning to indirect reseller.</span></span>

   :::image type="content" source="images/direct/direct1.png" alt-text="Genel Bakış":::

3. <span data-ttu-id="4e0fe-113">Kayıt formunda iş ortağı ayrıntılarınızı gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-113">Review your partner details on the enrollment form.</span></span>

   :::image type="content" source="images/direct/direct2a.png" alt-text="Hemen kaydolun":::

4. <span data-ttu-id="4e0fe-115">Şimdi Kaydet ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-115">Select Enroll now.</span></span> <span data-ttu-id="4e0fe-116">Dolaylı Bayi işiniz, doğrudan işletmeniz için kullandığınız AAD kiracısının aynısını kullanacaktır.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-116">Your indirect reseller business will use the same AAD tenant you use for your direct business.</span></span>

    > [!NOTE]
    > <span data-ttu-id="4e0fe-117">Başlangıçta bu yeni geçiş özelliği, Aralık ayında Tarih/yıl olan iş ortakları tarafından kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-117">Initially, this new transition capability will be available for partners with September to December anniversary dates.</span></span> <span data-ttu-id="4e0fe-118">Eylül ve Aralık arasında bir yıldönümü tarihi yoksa, bu özelliği şu anda görmezsiniz.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-118">If you don"t have an anniversary date between September and December, you won't see the capability at this time.</span></span> <span data-ttu-id="4e0fe-119">Aralık 2018 ' den sonra yıldönümü tarihleri olan iş ortakları, özellik iş ortakları için etkinleştirildikten sonra bilgilendirilir.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-119">Partners with anniversary dates after December 2018 will be notified later once the feature is enabled for the partners.</span></span>

5. <span data-ttu-id="4e0fe-120">Kaydınız onaylandığında Iş Ortağı Merkezi ' nde tekrar oturum açın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-120">When your enrollment is approved, sign in to Partner Center again.</span></span>

    > [!NOTE]
    > <span data-ttu-id="4e0fe-121">Onay genellikle anında, en fazla beş iş günü sürebilir.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-121">While approval is usually immediate, it can take up to five business days.</span></span> <span data-ttu-id="4e0fe-122">Onaylandığında, kayıt formunda birincil iletişim altında belirttiğiniz e-posta adresine bir bildirim alırsınız.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-122">Once approved, you will receive a notification to the email address you have specified under primary contact in the enrollment form.</span></span> <span data-ttu-id="4e0fe-123">Kayıt durumunuzu **Ayarlar**  >  **iş ortağı ayarları**  >  **iş ortağı profili** > program bilgileri altında da denetleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-123">You can also check your enrollment status under **Settings** > **Partner Settings** > **Partner Profile** > Program info.</span></span>

6. <span data-ttu-id="4e0fe-124">**Genel bakış** sayfanızda, dolaylı satıcı sözleşmesini görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-124">On your **Overview** page, you will see the indirect reseller agreement.</span></span> <span data-ttu-id="4e0fe-125">**Kabul et ve devam et '** i seçin.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-125">Select **Accept and continue** .</span></span> <span data-ttu-id="4e0fe-126">Bu eylem, dolaylı satıcı yeteneklerini sunar.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-126">This action enables the indirect reseller capabilities.</span></span>

<span data-ttu-id="4e0fe-127">Dolaylı satıcı sözleşmesini kabul ettiğinizde, Iş ortağı profilinizin sizi hem doğrudan fatura hem **de** dolaylı satıcı olarak tanımladığına dikkat edin.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-127">When you have accepted the indirect reseller agreement, notice that your Partner profile identifies you as **both** a direct bill and indirect reseller.</span></span>

:::image type="content" source="images/direct/direct3.png" alt-text="Dolaylı satıcı sözleşmesi":::

> [!IMPORTANT]
> <span data-ttu-id="4e0fe-129">Yeni yeteneği kullanarak dolaylı bir satıcı olarak kaydolduktan sonra doğrudan bir yalnızca fatura kiracıya geri dönme seçeneği yoktur.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-129">Once you enroll as an indirect reseller using the new capability, there is no option to roll back to a direct bill- only tenant.</span></span> <span data-ttu-id="4e0fe-130">Lütfen dolaylı bir satıcı olarak kaydolmadan önce iş gereksinimlerinizi tam olarak değerlendirdiğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-130">Please make sure that you fully evaluate your business needs before enrolling as an indirect reseller.</span></span>

## <a name="while-you-transition-from-direct-to-indirect-reseller"></a><span data-ttu-id="4e0fe-131">Doğrudan dolaylı satıcıya geçiş yaparken</span><span class="sxs-lookup"><span data-stu-id="4e0fe-131">While you transition from direct to indirect reseller</span></span>

<span data-ttu-id="4e0fe-132">Bu aşamada, faturalandırma süreci dahil olmak üzere doğrudan müşterilerinizin abonelik ihtiyaçlarını yönetmeye devam edersiniz.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-132">During this phase, you will continue to manage your direct customers' subscription needs including the billing process.</span></span> <span data-ttu-id="4e0fe-133">Ayrıca, dolaylı sağlayıcıınızdan müşterileri kabul etmeye ve dolaylı bir satıcı olarak çalışmaya başlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-133">You can also begin accepting customers from your Indirect provider and operating as an indirect reseller.</span></span>

:::image type="content" source="images/direct/direct4.png" alt-text="Hem doğrudan faturanız hem de dolaylı satıcı":::

## <a name="find-an-indirect-provider"></a><span data-ttu-id="4e0fe-135">Dolaylı sağlayıcı bulma</span><span class="sxs-lookup"><span data-stu-id="4e0fe-135">Find an indirect provider</span></span>

<span data-ttu-id="4e0fe-136">Kaydolduktan sonra, sol gezinti ortamınızda dolaylı sağlayıcılara bir bağlantı görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-136">After enrolling, a link to Indirect providers will appear in your left nav.</span></span> <span data-ttu-id="4e0fe-137">Dolaylı bir satıcı olarak, bir dolaylı sağlayıcıyla bir ilişki kurarsınız ve bu da faturanızı, müşterileriniz için satın alma ürünlerinizi ve destek altyapısını işleyebilir.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-137">As an indirect reseller you will establish a relationship with an indirect provider who then can handle your billing, purchase products for your customers, and support infrastructure.</span></span>

<span data-ttu-id="4e0fe-138">Farklı dolaylı sağlayıcılar farklı destek ve hizmetler sunmaktadır. bu nedenle, gereksinimlerinizi en iyi şekilde karşılayan Hizmetleri öğrenmek için bölgenizdeki sağlayıcıları değerlendirmelisiniz.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-138">Different indirect providers offer different support and services, so you should evaluate the providers in your area to determine which ones best meet your needs.</span></span> <span data-ttu-id="4e0fe-139">Genellikle, çoğu sağlayıcı şunları olur:</span><span class="sxs-lookup"><span data-stu-id="4e0fe-139">Generally, most providers will:</span></span>

- <span data-ttu-id="4e0fe-140">Size teknik eğitim ve yardım sağlama</span><span class="sxs-lookup"><span data-stu-id="4e0fe-140">Provide you with technical training and assistance</span></span>
- <span data-ttu-id="4e0fe-141">Ürün ve hizmetlerinizi pazarlamanıza yardımcı olun</span><span class="sxs-lookup"><span data-stu-id="4e0fe-141">Help you market your products and services</span></span>
- <span data-ttu-id="4e0fe-142">Finans ve kredi koşullarınızı yönetin</span><span class="sxs-lookup"><span data-stu-id="4e0fe-142">Manage your financing and credit terms</span></span>

<span data-ttu-id="4e0fe-143">Resmi [Microsoft dolaylı sağlayıcıları](https://partnercenter.microsoft.com/partner/find-a-provider)listesinde arama yapın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-143">Search the list of official [Microsoft indirect providers](https://partnercenter.microsoft.com/partner/find-a-provider).</span></span>

<span data-ttu-id="4e0fe-144">Daha fazla bilgi edinin, [dolaylı sağlayıcılarla Iş ortağı](indirect-reseller-tasks-in-partner-center.md) okuyun</span><span class="sxs-lookup"><span data-stu-id="4e0fe-144">Learn more, read  [Partner with indirect providers](indirect-reseller-tasks-in-partner-center.md)</span></span>

## <a name="accept-a-partnership-invitation-from-your-indirect-provider"></a><span data-ttu-id="4e0fe-145">Dolaylı sağlayıcınızdan bir ortaklık daveti kabul edin</span><span class="sxs-lookup"><span data-stu-id="4e0fe-145">Accept a partnership invitation from your indirect provider</span></span>

<span data-ttu-id="4e0fe-146">İş ortağına dolaylı bir sağlayıcı bulduğunuzda, Iş Ortağı Merkezi 'nde dolaylı sağlayıcıyla bir ortaklık kurun.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-146">When you find an indirect provider to partner with, establish a partnership with the indirect provider in Partner Center.</span></span>

<span data-ttu-id="4e0fe-147">Seçtiğiniz dolaylı sağlayıcı sizi Iş ortağı merkezindeki davetine götürebileceğiniz bir ortaklık daveti e-postası adresine gönderir.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-147">The indirect provider you select will send you in email a partnership invitation link that will take you to their invitation in Partner Center.</span></span> <span data-ttu-id="4e0fe-148">Genel yöneticinizin Iş Ortağı Merkezi 'nde oturum açtığından ve davet bağlantısını izlediğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-148">Be sure your global admin signs in to Partner Center and follows the invitation link.</span></span> <span data-ttu-id="4e0fe-149">Daveti kabul ettiğinizde, sağlayıcının adı dolaylı sağlayıcı listenizde görünür.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-149">When you accept the invitation, the provider's name will appear in your indirect provider list.</span></span>

## <a name="acquire-new-customers-as-indirect-reseller"></a><span data-ttu-id="4e0fe-150">Yeni müşterileri dolaylı satıcı olarak edinin</span><span class="sxs-lookup"><span data-stu-id="4e0fe-150">Acquire new customers as indirect reseller</span></span>

<span data-ttu-id="4e0fe-151">Hem siz hem de dolaylı sağlayıcınız müşterilerle satıcı ilişkilerine sahip olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-151">Both you and your indirect provider need to have reseller relationships with customers.</span></span> <span data-ttu-id="4e0fe-152">Bu satıcı ilişkileri, müşterinin aboneliklerini ve hizmetlerini kendi adına yönetmenize olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-152">These reseller relationships enable you to manage a customer's subscriptions and services on their behalf.</span></span> <span data-ttu-id="4e0fe-153">Mevcut bir Azure AD kiracısına sahip yeni bir müşteri edinmek için, müşteriyi hem sizinle hem de sağlayıcınızda aynı anda bir satıcı ilişkisi kurmaya davet edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-153">To acquire a new customer who has an existing Azure AD tenant, you can invite the customer to establish a reseller relationship with both you and your provider at the same time.</span></span>

<span data-ttu-id="4e0fe-154">Dolaylı bir satıcı daveti oluşturmak için:</span><span class="sxs-lookup"><span data-stu-id="4e0fe-154">To create an indirect reseller invitation:</span></span>

1. <span data-ttu-id="4e0fe-155">Iş ortağı merkezi sol gezininizden **dolaylı sağlayıcılar** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-155">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="4e0fe-156">Aynı anda hem sizin hem de dolaylı sağlayıcı ile satıcı ilişkisi kurmak üzere bir müşteriyi davet etmek için **yeni müşterileri davet et** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-156">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="4e0fe-157">Sağlayıcının müşteri ile bir satıcı ilişkisi olması gerekir, bu nedenle müşteri yeni abonelikler satın almak istediğinde veya mevcut aboneliklerde yeni lisanslar eklemek istediğinde müşterinin adına sipariş gönderebilirler.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-157">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

3. <span data-ttu-id="4e0fe-158">Sonraki sayfada taslak e-posta iletisini gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-158">On the next page, review the draft email message.</span></span> <span data-ttu-id="4e0fe-159">Taslak iletisini e-postada açabilir veya iletiyi panonuza kopyalayabilir ve bir e-postaya yapıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-159">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="4e0fe-160">E-postadaki metni düzenleyerek, ihtiyacınız olanları söyleyin, ancak müşteriyi doğrudan hesabınıza ve sağlayıcınızın hesabınıza bağlamak için kişiselleştirildiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-160">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="4e0fe-161">Ardından **Bitti** 'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-161">Then select **Done** .</span></span>

5. <span data-ttu-id="4e0fe-162">Müşteri sizi ve sağlayıcınızı kendi kayıt satıcıları olarak doğruladıktan sonra, kendi adına aboneliklerini, lisanslarını ve kullanıcılarını yönetmek için yönetici izinlerine sahip olacaksınız ve dolaylı sağlayıcınız kendi adına sipariş gönderebilecektir.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-162">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>
6. <span data-ttu-id="4e0fe-163">Müşterinin hesabını, hizmetlerini, kullanıcılarını ve lisanslarını yönetmek için, adının yanındaki aşağı oku seçerek müşterinin kaydını genişletin.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-163">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

<span data-ttu-id="4e0fe-164">Doğrudan fatura iş ortaklarının aksine, dolaylı satıcılar Iş Ortağı Merkezi 'nde yeni müşterileri için Azure AD kiracılar oluşturamaz.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-164">Unlike direct bill partners, indirect resellers can't create Azure AD tenants for their new customers in Partner Center.</span></span> <span data-ttu-id="4e0fe-165">Sağlayıcınız kiracıyı oluşturacak ve size bu müşterinin dolaylı satıcısı olarak belirtmeyecektir.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-165">Your provider will create the tenant and will specify you as the indirect reseller for this customer.</span></span> <span data-ttu-id="4e0fe-166">Bu, müşterinin Iş Ortağı Merkezi 'nde müşteri listenizde görünmesini sağlar.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-166">This ensures that the customer will appear in your customer list in Partner Center.</span></span>

>[!Note]
><span data-ttu-id="4e0fe-167">Dolaylı satıcı olarak aldığınız müşteriler için satın alma işlemleri oluşturmak üzere doğrudan fatura özelliğini kullanamazsınız.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-167">You will not be able to use your direct bill capability to create purchases for customers you acquire as an indirect reseller.</span></span>

## <a name="managing-your-direct-bill-customers-and-your-indirect-reseller-customers"></a><span data-ttu-id="4e0fe-168">Doğrudan Bill müşterilerini ve dolaylı satıcı müşterilerinizi yönetme</span><span class="sxs-lookup"><span data-stu-id="4e0fe-168">Managing your direct bill customers and your indirect reseller customers</span></span>

<span data-ttu-id="4e0fe-169">Doğrudan fatura müşterilerinizi ve dolaylı satıcı müşterilerinizi farklı şekilde yönetirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-169">You manage your direct bill customers and your indirect reseller customers differently.</span></span>

### <a name="direct-bill-customers-things-you-wont-do-as-an-indirect-reseller"></a><span data-ttu-id="4e0fe-170">Doğrudan fatura müşterileri (dolaylı satıcı olarak yapamayabilmeniz gerekir)</span><span class="sxs-lookup"><span data-stu-id="4e0fe-170">Direct bill customers (things you won't do as an indirect reseller)</span></span>

- <span data-ttu-id="4e0fe-171">Ürünler için sipariş oluşturma</span><span class="sxs-lookup"><span data-stu-id="4e0fe-171">Create orders for products</span></span>
- <span data-ttu-id="4e0fe-172">Azure ayırmalarını yönetme</span><span class="sxs-lookup"><span data-stu-id="4e0fe-172">Manage Azure reservations</span></span>
- <span data-ttu-id="4e0fe-173">Sıra geçmişini yönetme</span><span class="sxs-lookup"><span data-stu-id="4e0fe-173">Manage their order history</span></span>
- <span data-ttu-id="4e0fe-174">Satın alma yazılımı</span><span class="sxs-lookup"><span data-stu-id="4e0fe-174">Purchase software</span></span>
- <span data-ttu-id="4e0fe-175">Doğrudan fatura müşterileri</span><span class="sxs-lookup"><span data-stu-id="4e0fe-175">Bill customers directly</span></span>

### <a name="indirect-reseller-customers"></a><span data-ttu-id="4e0fe-176">Dolaylı satıcı müşterileri</span><span class="sxs-lookup"><span data-stu-id="4e0fe-176">Indirect reseller customers</span></span>

- <span data-ttu-id="4e0fe-177">Dolaylı sağlayıcınız, müşterileriniz için ürünleri sipariş eden</span><span class="sxs-lookup"><span data-stu-id="4e0fe-177">Your indirect provider orders products for your customers</span></span>
- <span data-ttu-id="4e0fe-178">Müşterilerin lisanslarını ve kullanıcılarını yönetme</span><span class="sxs-lookup"><span data-stu-id="4e0fe-178">Manage customers' licenses and users</span></span>
- <span data-ttu-id="4e0fe-179">Abonelik yenilemeler işleme</span><span class="sxs-lookup"><span data-stu-id="4e0fe-179">Handle subscription renewals</span></span>

### <a name="to-identify-customers-that-you-acquired-as-a-direct-bill-partner"></a><span data-ttu-id="4e0fe-180">Doğrudan bir fatura ortağı olarak edindiğiniz müşterileri belirlemek için</span><span class="sxs-lookup"><span data-stu-id="4e0fe-180">To identify customers that you acquired as a direct bill partner</span></span>

1. <span data-ttu-id="4e0fe-181">**Müşterileri** seçin</span><span class="sxs-lookup"><span data-stu-id="4e0fe-181">Select **Customers**</span></span>

2. <span data-ttu-id="4e0fe-182">Ayrıntılarını görüntülemek için bir müşteri seçin</span><span class="sxs-lookup"><span data-stu-id="4e0fe-182">Select a customer to view their details</span></span>

3. <span data-ttu-id="4e0fe-183">Bu müşteri doğrudan fatura ortağı olarak elde ediyorsanız, ürün **ekleme** veya **görüntüleme** seçeneklerini görürsünüz ve aboneliklerini görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-183">If this customer is one you acquired as a direct bill partner, you will see options to **add** or **view products** and you will see their subscriptions.</span></span>

4. <span data-ttu-id="4e0fe-184">Müşterinin sizinle dolaylı bir satıcı ilişkisi varsa, bu seçenekler kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-184">If the customer has an indirect reseller relationship with you, those options will not be available.</span></span>

## <a name="move-your-direct-bill-customers-to-your-indirect-provider"></a><span data-ttu-id="4e0fe-185">Doğrudan fatura müşterilerinizi dolaylı sağlayıcınıza taşıyın</span><span class="sxs-lookup"><span data-stu-id="4e0fe-185">Move your direct bill customers to your indirect provider</span></span>

<span data-ttu-id="4e0fe-186">Dolaylı sağlayıcınız, mevcut doğrudan fatura müşterileriniz için bir satıcı ilişkisine sahip olana kadar sipariş veya mevcut abonelik aktarımları gönderemez.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-186">Your indirect provider cannot submit orders or existing subscription transfers for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="4e0fe-187">Dolaylı sağlayıcınız ile var olan doğrudan faturanız arasındaki satıcı ilişkilerini oluşturmak için aşağıdaki yöntemlerden birini kullanabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="4e0fe-187">To establish the reseller relationship between your indirect provider and your existing direct bill customer, you can use one of the following methods:</span></span>

- [<span data-ttu-id="4e0fe-188">Satıcı ilişki uzantısı</span><span class="sxs-lookup"><span data-stu-id="4e0fe-188">Reseller relationship extension</span></span>](#reseller-relationship-extension)

- [<span data-ttu-id="4e0fe-189">Müşteriye dolaylı bir satıcı davetiyesi gönderin</span><span class="sxs-lookup"><span data-stu-id="4e0fe-189">Send an indirect reseller invitation to the customer</span></span>](#send-an-indirect-reseller-invitation-to-the-customer)

<span data-ttu-id="4e0fe-190">[Doğrudan dolaylı geçiş belgesinde](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/) adım adım işleme yönelik ayrıntılı bir genel bakış bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-190">You can find a detailed overview of the step-by-step process in the [Direct to indirect transition document](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span></span>

### <a name="reseller-relationship-extension"></a><span data-ttu-id="4e0fe-191">Satıcı ilişki uzantısı</span><span class="sxs-lookup"><span data-stu-id="4e0fe-191">Reseller relationship extension</span></span>

<span data-ttu-id="4e0fe-192">Kurumsal ilişki uzantısı özelliğini kullanarak, mevcut doğrudan fatura müşterileriniz ve dolaylı sağlayıcınız arasında Iş Ortağı Merkezi panosunu kullanarak satıcı ilişkisi kurabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-192">You can use the reseller relationship extension feature to establish reseller relationship between your existing direct bill customers and your indirect provider using Partner Center Dashboard.</span></span> <span data-ttu-id="4e0fe-193">Özelliği kullanmadan önce, aşağıdakilere göz önüne alın:</span><span class="sxs-lookup"><span data-stu-id="4e0fe-193">Before using the feature, note the following:</span></span>

- <span data-ttu-id="4e0fe-194">Bu özellik yalnızca dolaylı satıcı olan dolaylı satıcı [kaydını](#get-started)tamamlamış olan doğrudan fatura ortakları tarafından kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-194">This feature is only available to direct bill partners who are transitioning to become an indirect reseller have completed the [indirect reseller enrollment](#get-started).</span></span>

- <span data-ttu-id="4e0fe-195">Bu özelliği yalnızca var olan doğrudan fatura müşterilerine uygulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-195">You can only apply this feature to existing direct bill customers.</span></span> <span data-ttu-id="4e0fe-196">Bu, [dolaylı satıcı müşterileri](#acquire-new-customers-as-indirect-reseller)için geçerli değildir.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-196">It is not applicable to [indirect reseller customers](#acquire-new-customers-as-indirect-reseller).</span></span>

- <span data-ttu-id="4e0fe-197">Yalnızca [dolaylı sağlayıcıınızdan bir iş ortağı davetini kabul](#accept-a-partnership-invitation-from-your-indirect-provider)ettiğiniz bir dolaylı sağlayıcıyı seçebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-197">You can only select an indirect provider for which you have [accepted a partner invitation from your indirect provider](#accept-a-partnership-invitation-from-your-indirect-provider).</span></span>

- <span data-ttu-id="4e0fe-198">Bu müşteri için sahip olduğunuz fatura-bilgi bilgilerinin bir kopyası dolaylı sağlayıcı tarafından kullanılabilir hale getirilir.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-198">A copy of the bill-to info you have for this customer will be made available to the indirect provider.</span></span> <span data-ttu-id="4e0fe-199">Iş Ortağı Merkezi panosunda bu müşterinin hesap sayfasına erişerek fatura bilgilerine erişebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-199">You can access the bill-to info by accessing the Account page for this customer in Partner Center Dashboard.</span></span>

    > [!NOTE]
    > <span data-ttu-id="4e0fe-200">Satıcı ilişki uzantısı özelliğini kullanarak, bu müşteri için sahip olduğunuz fatura bilgilerini dolaylı sağlayıcıyla paylaşmayı kabul etmiş olursunuz.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-200">By using the reseller relationship extension feature, you consent to sharing the bill-to info you have for this customer with the indirect provider.</span></span>

- <span data-ttu-id="4e0fe-201">Dolaylı sağlayıcınız, müşteri kiracısına [atanan yönetim ayrıcalıkları](customers-revoke-admin-privileges.md) ile birlikte sağlanmaz.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-201">Your indirect provider will not be provided with [delegated administration privileges](customers-revoke-admin-privileges.md) to the customer tenant.</span></span> <span data-ttu-id="4e0fe-202">Dolaylı sağlayıcınız Temsilcili yönetim ayrıcalıkları gerektiriyorsa, bunun yerine müşteriye dolaylı bir satıcı daveti göndermeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-202">If your indirect provider requires delegated administration privileges, you must send an indirect reseller invitation to the customer instead.</span></span>

- <span data-ttu-id="4e0fe-203">Satıcı ilişkisi kurulduktan sonra, dolaylı sağlayıcı, [M365 Yönetim Merkezi](https://admin.microsoft.com/AdminPortal/Home#/partners) 'Nde ortak ilişkiler sayfasında ve [iş için Microsoft Store](/microsoft-store/work-with-partner-microsoft-store-business), müşteriye bir CSP iş ortağı olarak görünür.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-203">Once the reseller relationship is established, the indirect provider will appear as a CSP partner to the customer under the Partner Relationships page in [M365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/partners) and [Microsoft Store for Business](/microsoft-store/work-with-partner-microsoft-store-business).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="4e0fe-204">Karışıklık ve anlaşılmadan kaçınmak için, mevcut bir doğrudan fatura müşterisi ve dolaylı bir sağlayıcı arasında satıcı ilişkisi kurmak üzere ilişki uzantısı özelliğini kullanmadan önce, iş ortağı sözleşmenizde sözleşmeye dayalı yükümlülüğü vardır.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-204">To avoid confusion and misunderstanding, you are contractually obliged by your partner agreement to inform and obtain consent from the direct bill customer before you use the relationship extension feature to establish reseller relationship between an existing direct bill customer and an indirect provider.</span></span>

<span data-ttu-id="4e0fe-205">Bu özelliği mevcut bir müşteri kiracısında kullanmak için:</span><span class="sxs-lookup"><span data-stu-id="4e0fe-205">To use this feature on an existing customer tenant:</span></span>

1. <span data-ttu-id="4e0fe-206">Iş Ortağı Merkezi ' nde bir **Yönetim Aracısı** olarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-206">Log in to Partner Center as an **Admin Agent** .</span></span>

2. <span data-ttu-id="4e0fe-207">**Müşteriler sayfasında** , mevcut bir müşteriyi seçin ve müşterinin Özet görünümünü genişletmek için **hızlı bağlantılar** simgesine tıklayın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-207">In the **Customers page** , select an existing customer and click on its **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="4e0fe-208">**Dolaylı sağlayıcılar** ' ın altında, **dolaylı bir sağlayıcıda müşteriyi aktar** ' a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-208">Under **Indirect provider(s)** , click **Transfer customer on an indirect provider** .</span></span>

    :::image type="content" source="images/direct/direct5-1.png" alt-text="Müşteriyi dolaylı bir sağlayıcıya aktarma":::

4. <span data-ttu-id="4e0fe-210">Açılır iletişim kutusunda, müşteri ile satıcı ilişkisi olmasını istediğiniz **dolaylı sağlayıcıyı** seçin.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-210">In the pop-up dialog, select the **Indirect Provider** you would like to have reseller relationship with the customer.</span></span>

5. <span data-ttu-id="4e0fe-211">**Kaydet ve devam et** ' e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-211">Click **Save and continue** .</span></span>

6. <span data-ttu-id="4e0fe-212">Seçilen dolaylı sağlayıcının **dolaylı sağlayıcılar** altında görüntülendiğini doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-212">Verify the selected indirect provider shows up under **Indirect provider(s)** .</span></span>

    :::image type="content" source="images/direct/direct5-2.png" alt-text="Belirtilen dolaylı sağlayıcı":::

### <a name="send-an-indirect-reseller-invitation-to-the-customer"></a><span data-ttu-id="4e0fe-214">Müşteriye dolaylı bir satıcı davetiyesi gönderin</span><span class="sxs-lookup"><span data-stu-id="4e0fe-214">Send an indirect reseller invitation to the customer</span></span>

<span data-ttu-id="4e0fe-215">Dolaylı sağlayıcınız, mevcut doğrudan fatura müşterileriniz için bir satıcı ilişkisine sahip olana kadar sipariş gönderemezler.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-215">Your indirect provider cannot submit orders for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="4e0fe-216">Mevcut müşterileriniz ve dolaylı sağlayıcınız arasında satıcı ilişkisi kurmak için, dolaylı bir satıcı davetiyesi kullanarak müşteriyi davet edin.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-216">To establish the reseller relationship between your existing customers and your indirect provider, invite the customer using an indirect reseller invitation.</span></span>

1. <span data-ttu-id="4e0fe-217">Iş ortağı merkezi sol gezininizden **dolaylı sağlayıcılar** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-217">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="4e0fe-218">Aynı anda hem sizin hem de dolaylı sağlayıcı ile satıcı ilişkisi kurmak üzere bir müşteriyi davet etmek için **yeni müşterileri davet et** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-218">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="4e0fe-219">Sağlayıcının müşteri ile bir satıcı ilişkisi olması gerekir, bu nedenle müşteri yeni abonelikler satın almak istediğinde veya mevcut aboneliklerde yeni lisanslar eklemek istediğinde müşterinin adına sipariş gönderebilirler.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-219">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

    :::image type="content" source="images/direct/direct6.png" alt-text="Yeni müşterileri davet et":::

3. <span data-ttu-id="4e0fe-221">Sonraki sayfada taslak e-posta iletisini gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-221">On the next page, review the draft email message.</span></span> <span data-ttu-id="4e0fe-222">Taslak iletisini e-postada açabilir veya iletiyi panonuza kopyalayabilir ve bir e-postaya yapıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-222">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="4e0fe-223">E-postadaki metni düzenleyerek, ihtiyacınız olanları söyleyin, ancak müşteriyi doğrudan hesabınıza ve sağlayıcınızın hesabınıza bağlamak için kişiselleştirildiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-223">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="4e0fe-224">Ardından **Bitti** 'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-224">Then select **Done** .</span></span>

5. <span data-ttu-id="4e0fe-225">Müşteri sizi ve sağlayıcınızı kendi kayıt satıcıları olarak doğruladıktan sonra, kendi adına aboneliklerini, lisanslarını ve kullanıcılarını yönetmek için yönetici izinlerine sahip olacaksınız ve dolaylı sağlayıcınız kendi adına sipariş gönderebilecektir.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-225">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>

6. <span data-ttu-id="4e0fe-226">Müşterinin hesabını, hizmetlerini, kullanıcılarını ve lisanslarını yönetmek için, adının yanındaki aşağı oku seçerek müşterinin kaydını genişletin.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-226">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

### <a name="microsoft-customer-agreement-acceptance"></a><span data-ttu-id="4e0fe-227">Microsoft Müşteri Sözleşmesi kabulü</span><span class="sxs-lookup"><span data-stu-id="4e0fe-227">Microsoft Customer Agreement acceptance</span></span>

<span data-ttu-id="4e0fe-228">Microsoft Bulut sözleşmesi 31 Ocak 2020 ' ye kadar geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-228">Microsoft Cloud Agreement is valid until January 31, 2020.</span></span> <span data-ttu-id="4e0fe-229">Bu tarihten sonra, mevcut ve yeni olan tüm müşteriler yeni [Microsoft Müşteri sözleşmesinin](confirm-customer-agreement.md)imzalanmalıdır.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-229">After that date, all customers, existing and new, must sign the new [Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span> <span data-ttu-id="4e0fe-230">Şu durumlarda müşterilerin geçişini yapmak için:</span><span class="sxs-lookup"><span data-stu-id="4e0fe-230">For transitioning customers, if:</span></span>

- <span data-ttu-id="4e0fe-231">**Müşteri henüz Microsoft Müşteri sözleşmesini kabul etmedi**</span><span class="sxs-lookup"><span data-stu-id="4e0fe-231">**Customer has not accepted Microsoft Customer Agreement yet**</span></span>

   <span data-ttu-id="4e0fe-232">Müşterinin [Microsoft Müşteri anlaşmasını kabul](confirm-customer-agreement.md)etmesi Için lütfen dolaylı sağlayıcıyla çalışın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-232">Please work with Indirect Provider to have customer [accept the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

- <span data-ttu-id="4e0fe-233">**Müşteri, Microsoft 365 Yönetim Merkezi ile Microsoft Müşteri anlaşmasını sizinle kabul etti**</span><span class="sxs-lookup"><span data-stu-id="4e0fe-233">**Customer has accepted Microsoft Customer Agreement with you through the Microsoft 365 Admin Center**</span></span>

   <span data-ttu-id="4e0fe-234">Satıcı ilişkisi dolaylı sağlayıcıyla kurulduktan sonra kabul edilir.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-234">The acceptance will be retained once the reseller relationship is established with the Indirect Provider.</span></span> <span data-ttu-id="4e0fe-235">Yapmanız gereken bir şey yok.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-235">There is nothing you need to do.</span></span>

- <span data-ttu-id="4e0fe-236">**Müşteri, iş ortağı kanıtlama ile Microsoft Müşteri sözleşmesini kabul etti**</span><span class="sxs-lookup"><span data-stu-id="4e0fe-236">**Customer has accepted Microsoft Customer Agreement with you through partner attestation**</span></span>

   <span data-ttu-id="4e0fe-237">Kabul tutulmayacaktır.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-237">The acceptance will not be retained.</span></span> <span data-ttu-id="4e0fe-238">[Müşterinin Iş Ortağı Merkezi 'nin kabulünü güncelleştirmek](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers)Için lütfen dolaylı sağlayıcıyla çalışın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-238">Please work with Indirect Provider to [update the customer's acceptance in Partner Center](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span></span>

## <a name="transfer-existing-direct-bill-subscriptions-to-indirect-provider"></a><span data-ttu-id="4e0fe-239">Mevcut doğrudan fatura aboneliklerini dolaylı sağlayıcıya aktar</span><span class="sxs-lookup"><span data-stu-id="4e0fe-239">Transfer existing direct bill subscriptions to indirect provider</span></span>

<span data-ttu-id="4e0fe-240">CSP dolaylı modeli kapsamında, dolaylı satıcıların Microsoft ile faturalandırma ilişkileri yoktur.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-240">Under CSP indirect model, indirect resellers do not have billing relationships with Microsoft.</span></span> <span data-ttu-id="4e0fe-241">Bunun yerine dolaylı satıcılar, kendi dolaylı sağlayıcıları aracılığıyla müşterileri için abonelikler elde eder.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-241">Instead, indirect resellers obtain subscriptions for their customers through their indirect providers.</span></span> <span data-ttu-id="4e0fe-242">Doğrudan fatura ortağından dolaylı satıcıya geçiş yaparken, sahip olduğunuz mevcut abonelikleri dolaylı sağlayıcınıza doğrudan fatura ortağı olarak aktarmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-242">While transitioning from direct bill partner to indirect reseller, you need to transfer the existing subscriptions you have as the direct bill partner to your indirect provider.</span></span> <span data-ttu-id="4e0fe-243">Bunu yapmak için, Iş Ortağı Merkezi panosunda kendi kendine sunulan abonelik aktarma özelliğini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-243">You can use the self-served subscription transfer feature in Partner Center Dashboard to do so.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="4e0fe-244">Ön koşullar</span><span class="sxs-lookup"><span data-stu-id="4e0fe-244">Pre-requisites</span></span>

- <span data-ttu-id="4e0fe-245">Bu özellik yalnızca mevcut doğrudan fatura ortağı kiracılarını kullanarak dolaylı satıcı kaydını tamamlamış olan iş ortakları arasında geçiş yapılabilir</span><span class="sxs-lookup"><span data-stu-id="4e0fe-245">This feature is only available to transitioning partners who have completed the indirect reseller enrollment using their existing direct bill partner tenants</span></span>

- <span data-ttu-id="4e0fe-246">Belirli bir müşteriyle ilişkili abonelikleri aktarmadan önce, geçiş ortağı müşteriyi dolaylı bir sağlayıcıya taşımalıdır.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-246">Before transferring subscriptions associated with a given customer, the transitioning partner must move the customer to an indirect provider.</span></span>

- <span data-ttu-id="4e0fe-247">Müşterinin [dolaylı sağlayıcı aracılığıyla Microsoft Müşteri anlaşmasını kabul](#microsoft-customer-agreement-acceptance)etmiş olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-247">Customer must have [accepted Microsoft Customer Agreement through the Indirect Provider](#microsoft-customer-agreement-acceptance).</span></span>

### <a name="how-to-transition-to-indirect-reseller-status"></a><span data-ttu-id="4e0fe-248">Dolaylı satıcı durumuna geçiş</span><span class="sxs-lookup"><span data-stu-id="4e0fe-248">How to transition to indirect reseller status</span></span>

<span data-ttu-id="4e0fe-249">Özelliği 4 adımlı bir işlemdir; burada:</span><span class="sxs-lookup"><span data-stu-id="4e0fe-249">The feature is a 4-step process, where:</span></span>

- <span data-ttu-id="4e0fe-250">Geçiş ortağı bir abonelik aktarma isteği oluşturur.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-250">The transitioning partner creates a subscription transfer request.</span></span> <span data-ttu-id="4e0fe-251">İstek, aynı müşteriyle ilişkili bir veya daha fazla var olan abonelik içeriyor ve dolaylı bir sağlayıcıya yönelik.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-251">The request contains one or more existing subscriptions associated with the same customer and is addressed to an indirect provider.</span></span>

- <span data-ttu-id="4e0fe-252">Dolaylı sağlayıcı, aktarım isteğini gözden geçirir ve kabul eder (veya reddeder).</span><span class="sxs-lookup"><span data-stu-id="4e0fe-252">The indirect provider reviews and accepts (or reject) the transfer request.</span></span>

- <span data-ttu-id="4e0fe-253">Dolaylı sağlayıcı, aktarım isteğinin tamamlandığını doğrular.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-253">The indirect provider verifies that the transfer request is complete.</span></span>

- <span data-ttu-id="4e0fe-254">Geçiş ortağı, aktarım isteğinin tamamlandığını doğrular.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-254">The transitioning partner verifies that the transfer request is complete.</span></span>

### <a name="transitioning-partner"></a><span data-ttu-id="4e0fe-255">İş ortağı geçiyor</span><span class="sxs-lookup"><span data-stu-id="4e0fe-255">Transitioning partner</span></span>

> [!NOTE]
> <span data-ttu-id="4e0fe-256">Ayrıca, mevcut abonelikleri dolaylı sağlayıcınıza aktarmak için [Iş ortağı MERKEZI API/SDK](/partner-center/develop/manage-customers) 'sını de kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-256">You can also use [Partner Center API/SDK](/partner-center/develop/manage-customers) to transfer the existing subscriptions to your indirect provider.</span></span>
>
> - [<span data-ttu-id="4e0fe-257">Müşterinin abonelik aktarım uygunluğunu al</span><span class="sxs-lookup"><span data-stu-id="4e0fe-257">Get a customer's subscriptions transfer eligibility</span></span>](/partner-center/develop/get-customer-s-subscriptions-transfer-eligibility)
> - [<span data-ttu-id="4e0fe-258">Müşterinin aktarımını oluşturma</span><span class="sxs-lookup"><span data-stu-id="4e0fe-258">Create a customer's transfer</span></span>](/partner-center/develop/create-a-transfer)
> - [<span data-ttu-id="4e0fe-259">Müşterinin aktarımını geri alma</span><span class="sxs-lookup"><span data-stu-id="4e0fe-259">Withdraw a customer's transfer</span></span>](/partner-center/develop/withdraw-a-transfer)
> - [<span data-ttu-id="4e0fe-260">Müşterinin aktarımını kabul et</span><span class="sxs-lookup"><span data-stu-id="4e0fe-260">Accept a customer's transfer</span></span>](/partner-center/develop/accept-a-transfer)
> - [<span data-ttu-id="4e0fe-261">Müşterinin aktarımını reddetme</span><span class="sxs-lookup"><span data-stu-id="4e0fe-261">Reject a Customer's transfer</span></span>](/partner-center/develop/reject-a-transfer)
> - [<span data-ttu-id="4e0fe-262">Müşterinin aktarımlarını al</span><span class="sxs-lookup"><span data-stu-id="4e0fe-262">Get a customer's transfers</span></span>](/partner-center/develop/get-all-of-a-customer-s-transfers)
> - [<span data-ttu-id="4e0fe-263">Kimliğe göre aktarım ayrıntılarını al</span><span class="sxs-lookup"><span data-stu-id="4e0fe-263">Get transfer details by id</span></span>](/partner-center/develop/get-transfer-by-id)

### <a name="transitioning-partner---create-transfer-request"></a><span data-ttu-id="4e0fe-264">İş ortağı geçişi-aktarım isteği oluşturma</span><span class="sxs-lookup"><span data-stu-id="4e0fe-264">Transitioning partner - create transfer request</span></span>

<span data-ttu-id="4e0fe-265">Geçiş ortağı olarak bir aktarım isteği oluşturmak için:</span><span class="sxs-lookup"><span data-stu-id="4e0fe-265">To create a transfer request as the transitioning partner:</span></span>

1. <span data-ttu-id="4e0fe-266">Iş Ortağı Merkezi ' nde bir **Yönetim Aracısı** olarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-266">Log in to Partner Center as an **Admin Agent** .</span></span>

2. <span data-ttu-id="4e0fe-267">**Müşteriler** sayfasında, istenen müşteriyi seçin ve hızlı bağlantılar simgesine tıklayarak müşterinin Özet görünümünü genişletin.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-267">In the **Customers** page, select the intended customer and click on the Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="4e0fe-268">**Dolaylı sağlayıcılar** ' ın altında, amaçlanan dolaylı sağlayıcının listelendiğini onaylayın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-268">Under **Indirect provider(s)** , confirm that the intended indirect provider is listed.</span></span>

4. <span data-ttu-id="4e0fe-269">**Abonelikleri görüntüle** ' ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-269">Click **View Subscriptions** .</span></span>

5. <span data-ttu-id="4e0fe-270">**Abonelikler** sayfasında, **abonelik aktarımı** ' nı arayın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-270">In the **Subscriptions** page, look for **Subscription Transfer** .</span></span>

6. <span data-ttu-id="4e0fe-271">**Abonelik aktarımı** altında **abonelik aktarımı iste** ' ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-271">Under **Subscription Transfer** , click **Request subscription transfer** .</span></span>

    :::image type="content" source="images/direct/direct8.png" alt-text="Abonelik aktarımı iste":::

7. <span data-ttu-id="4e0fe-273">Aktarım isteği iletişim kutusunda, aktarılacak bir veya daha fazla abonelik seçin.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-273">In the transfer request dialog, select one or more subscriptions to be transferred.</span></span>

    :::image type="content" source="images/direct/direct9.png" alt-text="Aktarım Isteği oluştur":::

8. <span data-ttu-id="4e0fe-275">**Oluştur** 'a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-275">Click **Create** .</span></span>

9. <span data-ttu-id="4e0fe-276">**Abonelik aktarımı** altında, etkin bir abonelik aktarım isteği görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-276">An active subscription transfer request will appear under **Subscription Transfer** .</span></span>

    :::image type="content" source="images/direct/direct10.png" alt-text="İstek listesini aktar":::

10. <span data-ttu-id="4e0fe-278">Dolaylı sağlayıcınızı, bunlara bir abonelik aktarım isteği oluşturduğunu bildirin.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-278">Inform your indirect provider that you have created a subscription transfer request to them.</span></span>

### <a name="indirect-provider---accept-transfer-request"></a><span data-ttu-id="4e0fe-279">Dolaylı sağlayıcı-aktarım isteğini kabul et</span><span class="sxs-lookup"><span data-stu-id="4e0fe-279">Indirect provider - accept transfer request</span></span>

<span data-ttu-id="4e0fe-280">Bir aktarım isteğini dolaylı sağlayıcı olarak gözden geçirmek ve kabul etmek için:</span><span class="sxs-lookup"><span data-stu-id="4e0fe-280">To review and accept a transfer request as the indirect provider:</span></span>

1. <span data-ttu-id="4e0fe-281">Iş Ortağı Merkezi 'nde bir **Yönetim** Aracısı veya **Satış Aracısı** olarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-281">Log in to Partner Center as an **Admin** Agent or **Sales Agent** .</span></span>

2. <span data-ttu-id="4e0fe-282">**Müşteriler** sayfasında, istenen müşteriyi seçin ve müşterinin Özet görünümünü genişletmek için hızlı bağlantılar simgesine tıklayın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-282">In the **Customers** page, select the intended customer and click on its Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="4e0fe-283">**Dolaylı satıcı (ler)** altında, geçiş ortağının listelendiğini onaylayın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-283">Under **Indirect reseller(s)** , confirm the transitioning partner is listed.</span></span>

4. <span data-ttu-id="4e0fe-284">**Abonelikleri görüntüle** ' ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-284">Click **View Subscriptions** .</span></span>

5. <span data-ttu-id="4e0fe-285">**Abonelikler** sayfasında, **abonelik aktarımı** ' nı arayın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-285">In the **Subscriptions** page, look for **Subscription Transfer** .</span></span>

    :::image type="content" source="images/direct/direct11.png" alt-text="Aktarım isteğini görüntüle":::

6. <span data-ttu-id="4e0fe-287">**Abonelik aktarımı** altında, gözden geçirmek için aktarım isteğine tıklayın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-287">Under **Subscription Transfer** , click on the transfer request to review.</span></span>

7. <span data-ttu-id="4e0fe-288">Uygun şekilde **kabul et** (veya **Reddet** ) seçeneğine tıklayın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-288">Click **Accept** (or **Reject** ) as appropriate.</span></span>

    :::image type="content" source="images/direct/direct12.png" alt-text="Aktarım isteğini kabul et":::

8. <span data-ttu-id="4e0fe-290">Aktarım isteğinin tamamlanmasını bekleyin.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-290">Wait for the transfer request to complete.</span></span>

### <a name="indirect-provider---verify-transfer-request-is-complete"></a><span data-ttu-id="4e0fe-291">Dolaylı sağlayıcı-aktarım isteğinin tamamlandığını doğrulama</span><span class="sxs-lookup"><span data-stu-id="4e0fe-291">Indirect provider - verify transfer request is complete</span></span>

1. <span data-ttu-id="4e0fe-292">Aktarım isteği başarıyla tamamlandıktan sonra, aboneliklerin **abonelikler** bölümünde göründüğünü görebildiğinizi doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-292">After the transfer request is completed successfully, verify that you can see the subscriptions appear under **Subscriptions** .</span></span>

2. <span data-ttu-id="4e0fe-293">Geçiş ortağına bildirin.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-293">Inform the transitioning partner.</span></span>

### <a name="transitioning-partner---verify-transfer-request-is-complete"></a><span data-ttu-id="4e0fe-294">Geçiş ortağı-aktarım isteğini doğrulama işlemi tamamlanmıştır</span><span class="sxs-lookup"><span data-stu-id="4e0fe-294">Transitioning partner - verify transfer request is complete</span></span>

<span data-ttu-id="4e0fe-295">Geçiş ortağı aşağıdakileri yapması gerekir:</span><span class="sxs-lookup"><span data-stu-id="4e0fe-295">The transitioning partner should do the following:</span></span>

1. <span data-ttu-id="4e0fe-296">Iş Ortağı Merkezi 'Nde bir **Yönetim Aracısı** veya **Satış Aracısı** olarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-296">Sign into Partner Center as an **Admin Agent** or **Sales Agent** .</span></span>

2. <span data-ttu-id="4e0fe-297">**Müşteriler** sayfasında, istenen müşteriyi seçin ve **hızlı bağlantılar** simgesine tıklayarak müşterinin Özet görünümünü genişletin.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-297">In the **Customers** page, select the intended customer and click on the **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="4e0fe-298">**Abonelikleri görüntüle** ' ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-298">Click **View Subscriptions** .</span></span>

4. <span data-ttu-id="4e0fe-299">**Abonelikler** sayfasında, **abonelik aktarımı** ' nı arayın.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-299">In the **Subscriptions** page, look for **Subscription Transfer** .</span></span>

5. <span data-ttu-id="4e0fe-300">Aktarım isteğinin **Tamam** olarak işaretlendiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-300">Verify that the transfer request is marked as **Complete** .</span></span>

6. <span data-ttu-id="4e0fe-301">Aboneliğin artık **abonelikler** sayfasında etkin olarak görünmediğini doğrulayın:</span><span class="sxs-lookup"><span data-stu-id="4e0fe-301">Verify that the subscription(s) no longer appear as active in the **Subscriptions** page:</span></span>

   1. <span data-ttu-id="4e0fe-302">Bu bir Azure aboneliğse (MS-AZR-0145P), artık listelenmez.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-302">If this is an Azure subscription (MS-AZR-0145P), it will no longer be listed.</span></span>

   2. <span data-ttu-id="4e0fe-303">Bu bir lisans tabanlı aboneliğiniz (Office 365, Dynamics, Intune), durumu **askıya alındı** olarak listelenir.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-303">If this is a license-based subscription (Office 365, Dynamics, Intune), it will be listed with state as **Suspended** .</span></span>

   :::image type="content" source="images/direct/direct13.png" alt-text="Abonelik askıya alındı":::

### <a name="considerations"></a><span data-ttu-id="4e0fe-305">Dikkat edilmesi gerekenler</span><span class="sxs-lookup"><span data-stu-id="4e0fe-305">Considerations</span></span>

- <span data-ttu-id="4e0fe-306">**Abonelik KIMLIĞI aktarımdan sonra farklı olacaktır.**</span><span class="sxs-lookup"><span data-stu-id="4e0fe-306">**Subscription ID will be different after transfer.**</span></span> <span data-ttu-id="4e0fe-307">Bu bir Azure aboneliğiyiyse (MS-AZR-0145P), buna ek olarak, önceki sahibinden tutulan ve Azure yönetim portalında görünecek bir Azure abonelik KIMLIĞI olur.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-307">If it is an Azure subscription (MS-AZR-0145P), additionally, it will have an Azure Subscription ID, which is retained from the previous owner, and will appear in the Azure management portal.</span></span>

- <span data-ttu-id="4e0fe-308">**Aynı aboneliğe birden çok aktarım isteği tarafından başvurulamaz.**</span><span class="sxs-lookup"><span data-stu-id="4e0fe-308">**The same subscription cannot be referenced by multiple transfer requests.**</span></span> <span data-ttu-id="4e0fe-309">Mevcut bir aboneliği içeren bir aktarım isteği oluşturduktan sonra, ilk aktarım isteği iptal edilene kadar aynı abonelik dahil olmak üzere ek aktarım istekleri oluşturamazsınız.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-309">After you have created a transfer request, which includes an existing subscription, you cannot create additional transfer requests including the same subscription, until the first transfer request is canceled.</span></span>

- <span data-ttu-id="4e0fe-310">**Lisans tabanlı abonelikler için eklentiler, temel abonelikleriyle birlikte aktarılmalıdır.**</span><span class="sxs-lookup"><span data-stu-id="4e0fe-310">**Add-ons for license-based subscriptions must be transferred along with their base subscription.**</span></span> <span data-ttu-id="4e0fe-311">Bir aktarım isteği oluştururken, bir veya daha fazla eklentiye sahip mevcut bir aboneliği seçerseniz, eklenti otomatik olarak aktarım isteğine dahil edilir.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-311">When creating a transfer request, if you pick an existing subscription with one or more add-ons, the add-ons will automatically be included in the transfer request.</span></span>

- <span data-ttu-id="4e0fe-312">**Bir abonelikte lisans sayısı değişiklikleri var olan aktarım isteğine yansıtılmayacaktır.**</span><span class="sxs-lookup"><span data-stu-id="4e0fe-312">**License count changes to a subscription will not be reflected in existing transfer request.**</span></span> <span data-ttu-id="4e0fe-313">Var olan bir aboneliği içeren bir aktarım isteği oluşturduktan sonra, aboneliğin lisans miktarını (veya ilişkili eklentiler) güncelleştirmeden kaçınmalısınız.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-313">After you have created a transfer request which includes an existing subscription, you should avoid updating the license quantity of the subscription (or associated addons).</span></span> <span data-ttu-id="4e0fe-314">Bunu yaparsanız, yeni miktar aktarım isteğine yansıtılmayacaktır.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-314">If you do so, the new quantity will not be reflected in the transfer request.</span></span> <span data-ttu-id="4e0fe-315">Dolaylı sağlayıcı aktarım isteğini kabul ettikten sonra, sonuçta elde edilen abonelik eski miktara sahip olur.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-315">After the indirect provider accepts the transfer request, the resultant subscription will have the old quantity.</span></span> <span data-ttu-id="4e0fe-316">Yeni miktarın dolaylı sağlayıcıya aktarılmasını istiyorsanız, var olan aktarım isteğini iptal etmeniz ve yeni bir tane oluşturmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-316">If you wish for the new quantity to be transferred to the indirect provider, you must cancel the existing transfer request and recreate a new one.</span></span>

- <span data-ttu-id="4e0fe-317">**Satın alma işlemleri, kendi kendine sunulan abonelik aktarımı kullanılarak aktarılamaz.**</span><span class="sxs-lookup"><span data-stu-id="4e0fe-317">**Not all purchases can be transferred using self-served subscription transfer.**</span></span> <span data-ttu-id="4e0fe-318">Şu anda, bu özelliği kullanarak yalnızca O365 aboneliklerini ve Azure PAYG aboneliklerini (MS-AZR-0145P) aktarabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-318">Currently, you can only transfer O365 subscriptions and Azure PAYG subscriptions (MS-AZR-0145P) using this feature.</span></span> <span data-ttu-id="4e0fe-319">Azure planları, Azure ayrılmış örnekleri, terim tabanlı abonelikler ve Azure Marketi için SaaS abonelikleri dahil diğer satın alma işlemleri desteklenmez.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-319">Other purchases including Azure Plans, Azure Reserved Instances, Term-based Subscriptions and SaaS subscriptions for Azure Marketplace are not supported.</span></span> <span data-ttu-id="4e0fe-320">Aktarım isteği Gönder sayfasında aboneliğin neden aktarılamadığına ilişkin bir neden göreceksiniz.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-320">You will see a reason why a subscription cannot be transferred in the submit transfer request page.</span></span> <span data-ttu-id="4e0fe-321">Bu abonelikleri aktarmak için, [mevcut aboneliği iptal](create-a-new-subscription.md#suspend-or-cancel-a-subscription) etmeniz ve dolaylı sağlayıcı aracılığıyla müşteri için yeni teklif satın almanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-321">To transfer these subscriptions, you will need to [cancel the existing subscription](create-a-new-subscription.md#suspend-or-cancel-a-subscription) and purchase new offer for customer through Indirect Provider.</span></span>

- <span data-ttu-id="4e0fe-322">**Korumalı alan ortamı kullanılarak test edilemez.**</span><span class="sxs-lookup"><span data-stu-id="4e0fe-322">**Cannot be tested using sandbox environment.**</span></span>

## <a name="enroll-for-indirect-reseller-incentives"></a><span data-ttu-id="4e0fe-323">Dolaylı satıcı teşvikleri kaydolun</span><span class="sxs-lookup"><span data-stu-id="4e0fe-323">Enroll for indirect reseller incentives</span></span>

<span data-ttu-id="4e0fe-324">Mevcut doğrudan fatura ortağı kiracınızda dolaylı bir satıcı olarak başarıyla kaydolduktan sonra, 30 gün içinde dolaylı satıcı teşvik etmek için kaydolma daveti alacaksınız.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-324">After you have successfully enrolled as an indirect reseller on your existing direct bill partner tenant, you will receive an invitation to enroll for indirect reseller incentive within 30 days.</span></span> <span data-ttu-id="4e0fe-325">Davet, CSP iş ortağı kiracınızla ilişkilendirilmiş olan iş ortağı MPN hesabına dayalıdır.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-325">The invitation is based on the partner MPN account that is currently associated with your CSP partner tenant.</span></span> <span data-ttu-id="4e0fe-326">Davet, iş ortağı MPN hesabıyla ilişkili e-posta adresine gönderilir.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-326">The invitation will be sent to the email address associated with the partner MPN account.</span></span>

<span data-ttu-id="4e0fe-327">Ayrıca, aynı iş ortağı kiracısıyla doğrudan fatura teşvik programlarına kaydolma yetkiniz vardır.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-327">You are also eligible to enroll for direct bill incentive programs with that same partner tenant.</span></span> <span data-ttu-id="4e0fe-328">Programları ayrı ayrı yönetmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="4e0fe-328">You must manage the programs separately.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4e0fe-329">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="4e0fe-329">Next steps</span></span>

- [<span data-ttu-id="4e0fe-330">Dolaylı satıcı olma hakkında ek bilgiler</span><span class="sxs-lookup"><span data-stu-id="4e0fe-330">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)
- [<span data-ttu-id="4e0fe-331">CSP doğrudan iş ortağı yeni gereksinimler</span><span class="sxs-lookup"><span data-stu-id="4e0fe-331">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)
- [<span data-ttu-id="4e0fe-332">Kısıtlanmış doğrudan fatura özellikleri</span><span class="sxs-lookup"><span data-stu-id="4e0fe-332">Restricted direct bill capabilities</span></span>](restricted-direct-bill-capabilities.md)