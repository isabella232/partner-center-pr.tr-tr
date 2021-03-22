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
ms.openlocfilehash: 0e7676df62aa6ea91492f9904ac810397fb0e5aa
ms.sourcegitcommit: 35fe0fdc41886f6f5af71ec74e4a4ebd245dfe1d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/22/2021
ms.locfileid: "104768763"
---
# <a name="transition-from-cloud-solution-provider-csp-direct-bill-partner-to-csp-indirect-reseller"></a><span data-ttu-id="aacc5-103">Bulut Çözümü Sağlayıcısı (CSP) doğrudan faturalanan iş ortağından CSP dolaylı kurumsal bayiye geçiş</span><span class="sxs-lookup"><span data-stu-id="aacc5-103">Transition from Cloud Solution Provider (CSP) direct bill partner to CSP indirect reseller</span></span>

<span data-ttu-id="aacc5-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="aacc5-104">**Appropriate roles**</span></span>

- <span data-ttu-id="aacc5-105">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="aacc5-105">Global admin</span></span>

>[!Note]
><span data-ttu-id="aacc5-106">Bu makale, dolaylı satıcılara geçişe karar veren doğrudan fatura ortakları için tasarlanmıştır.</span><span class="sxs-lookup"><span data-stu-id="aacc5-106">This article is intended for direct bill partners who have decided to transition to indirect resellers.</span></span> <span data-ttu-id="aacc5-107">Ancak dolaylı bir satıcı olarak kaydolmak üzere açık bir karar vermemiş olsanız bile, doğrudan [Fatura özellikleri kısıtlandıktan](restricted-direct-bill-capabilities.md)sonra CSP doğrudan fatura ortağı programı için yeni [gereksinimleri](direct-partner-new-requirements.md) karşılamayan doğrudan fatura iş ortakları Microsoft tarafından bilgilendirilir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-107">However, even if you have not made an explicit decision yet to enroll as an indirect reseller, direct bill partners who do not meet the new [requirements](direct-partner-new-requirements.md) for the CSP direct bill partner program will be informed by Microsoft when their [direct bill capabilities will be restricted](restricted-direct-bill-capabilities.md).</span></span>
<br><span data-ttu-id="aacc5-108">2021 Ocak itibariyle yeni bir gelir gereksinimi eklenecektir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-108">As of January 2021, a new revenue requirement will be added.</span></span> <span data-ttu-id="aacc5-109">Doğrudan bir fatura ortağı olarak kaydedilen iş ortaklarının, önceki 12 aya göre ortak küresel hesap düzeyinde bulut çözümü sağlayıcısı program gelirinde en az ABD Doları $300K ' a kadar işlem yapması gerekir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-109">Partners enrolled as a direct bill partner will need to have transacted at least USD$300K in Cloud Solution Provider program revenue at a Partner Global Account level over the previous 12 months.</span></span>

<span data-ttu-id="aacc5-110">Mevcut doğrudan fatura kiracınızı kullanarak dolaylı satıcı programına kayıt yapabileceksiniz.</span><span class="sxs-lookup"><span data-stu-id="aacc5-110">You will be able to enroll in the indirect reseller program using your existing direct bill tenant.</span></span>

## <a name="get-started"></a><span data-ttu-id="aacc5-111">başlarken</span><span class="sxs-lookup"><span data-stu-id="aacc5-111">Get started</span></span>

1. <span data-ttu-id="aacc5-112">Iş ortağı merkezi ve MPN KIMLIĞI 'ndeki iş ortağı profilinizin güncel olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="aacc5-112">Make sure your partner profile in Partner Center and MPN ID are current.</span></span>

2. <span data-ttu-id="aacc5-113">Dolaylı satıcıya geçiş yaptığınız doğrudan fatura kiracının genel yöneticisi olarak Iş Ortağı Merkezi ' nde oturum açın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-113">Sign in to Partner Center as the global admin for the direct bill tenant you are transitioning to indirect reseller.</span></span>

   :::image type="content" source="images/direct/direct1.png" alt-text="Genel Bakış":::

3. <span data-ttu-id="aacc5-115">Kayıt formunda iş ortağı ayrıntılarınızı gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="aacc5-115">Review your partner details on the enrollment form.</span></span>

   :::image type="content" source="images/direct/direct2a.png" alt-text="Hemen kaydolun":::

4. <span data-ttu-id="aacc5-117">Şimdi Kaydet ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="aacc5-117">Select Enroll now.</span></span> <span data-ttu-id="aacc5-118">Dolaylı Bayi işiniz, doğrudan işletmeniz için kullandığınız AAD kiracısının aynısını kullanacaktır.</span><span class="sxs-lookup"><span data-stu-id="aacc5-118">Your indirect reseller business will use the same AAD tenant you use for your direct business.</span></span>

    > [!NOTE]
    > <span data-ttu-id="aacc5-119">Başlangıçta bu yeni geçiş özelliği, Aralık ayında Tarih/yıl olan iş ortakları tarafından kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-119">Initially, this new transition capability will be available for partners with September to December anniversary dates.</span></span> <span data-ttu-id="aacc5-120">Eylül ve Aralık arasında bir yıldönümü tarihi yoksa, bu özelliği şu anda görmezsiniz.</span><span class="sxs-lookup"><span data-stu-id="aacc5-120">If you don"t have an anniversary date between September and December, you won't see the capability at this time.</span></span> <span data-ttu-id="aacc5-121">Aralık 2018 ' den sonra yıldönümü tarihleri olan iş ortakları, özellik iş ortakları için etkinleştirildikten sonra bilgilendirilir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-121">Partners with anniversary dates after December 2018 will be notified later once the feature is enabled for the partners.</span></span>

5. <span data-ttu-id="aacc5-122">Kaydınız onaylandığında Iş Ortağı Merkezi ' nde tekrar oturum açın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-122">When your enrollment is approved, sign in to Partner Center again.</span></span>

    > [!NOTE]
    > <span data-ttu-id="aacc5-123">Onay genellikle anında, en fazla beş iş günü sürebilir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-123">While approval is usually immediate, it can take up to five business days.</span></span> <span data-ttu-id="aacc5-124">Onaylandığında, kayıt formunda birincil iletişim altında belirttiğiniz e-posta adresine bir bildirim alırsınız.</span><span class="sxs-lookup"><span data-stu-id="aacc5-124">Once approved, you will receive a notification to the email address you have specified under primary contact in the enrollment form.</span></span> <span data-ttu-id="aacc5-125">Kayıt durumunuzu **Ayarlar**  >  **Hesap ayarları**  >  **iş ortağı profili** > program bilgileri altında da denetleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="aacc5-125">You can also check your enrollment status under **Settings** > **Account Settings** > **Partner Profile** > Program info.</span></span>

6. <span data-ttu-id="aacc5-126">**Genel bakış** sayfanızda, dolaylı satıcı sözleşmesini görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="aacc5-126">On your **Overview** page, you will see the indirect reseller agreement.</span></span> <span data-ttu-id="aacc5-127">**Kabul et ve devam et '** i seçin.</span><span class="sxs-lookup"><span data-stu-id="aacc5-127">Select **Accept and continue**.</span></span> <span data-ttu-id="aacc5-128">Bu eylem, dolaylı satıcı yeteneklerini sunar.</span><span class="sxs-lookup"><span data-stu-id="aacc5-128">This action enables the indirect reseller capabilities.</span></span>

<span data-ttu-id="aacc5-129">Dolaylı satıcı sözleşmesini kabul ettiğinizde, Iş ortağı profilinizin sizi hem doğrudan fatura hem **de** dolaylı satıcı olarak tanımladığına dikkat edin.</span><span class="sxs-lookup"><span data-stu-id="aacc5-129">When you have accepted the indirect reseller agreement, notice that your Partner profile identifies you as **both** a direct bill and indirect reseller.</span></span>

:::image type="content" source="images/direct/direct3.png" alt-text="Dolaylı satıcı sözleşmesi":::

> [!IMPORTANT]
> <span data-ttu-id="aacc5-131">Yeni yeteneği kullanarak dolaylı bir satıcı olarak kaydolduktan sonra doğrudan bir yalnızca fatura kiracıya geri dönme seçeneği yoktur.</span><span class="sxs-lookup"><span data-stu-id="aacc5-131">Once you enroll as an indirect reseller using the new capability, there is no option to roll back to a direct bill- only tenant.</span></span> <span data-ttu-id="aacc5-132">Lütfen dolaylı bir satıcı olarak kaydolmadan önce iş gereksinimlerinizi tam olarak değerlendirdiğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="aacc5-132">Please make sure that you fully evaluate your business needs before enrolling as an indirect reseller.</span></span>

## <a name="while-you-transition-from-direct-to-indirect-reseller"></a><span data-ttu-id="aacc5-133">Doğrudan dolaylı satıcıya geçiş yaparken</span><span class="sxs-lookup"><span data-stu-id="aacc5-133">While you transition from direct to indirect reseller</span></span>

<span data-ttu-id="aacc5-134">Bu aşamada, faturalandırma süreci dahil olmak üzere doğrudan müşterilerinizin abonelik ihtiyaçlarını yönetmeye devam edersiniz.</span><span class="sxs-lookup"><span data-stu-id="aacc5-134">During this phase, you will continue to manage your direct customers' subscription needs including the billing process.</span></span> <span data-ttu-id="aacc5-135">Ayrıca, dolaylı sağlayıcıınızdan müşterileri kabul etmeye ve dolaylı bir satıcı olarak çalışmaya başlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="aacc5-135">You can also begin accepting customers from your Indirect provider and operating as an indirect reseller.</span></span>

:::image type="content" source="images/direct/direct4.png" alt-text="Hem doğrudan faturanız hem de dolaylı satıcı":::

## <a name="find-an-indirect-provider"></a><span data-ttu-id="aacc5-137">Dolaylı sağlayıcı bulma</span><span class="sxs-lookup"><span data-stu-id="aacc5-137">Find an indirect provider</span></span>

<span data-ttu-id="aacc5-138">Kaydolduktan sonra, sol gezinti ortamınızda dolaylı sağlayıcılara bir bağlantı görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-138">After enrolling, a link to Indirect providers will appear in your left nav.</span></span> <span data-ttu-id="aacc5-139">Dolaylı bir satıcı olarak, bir dolaylı sağlayıcıyla bir ilişki kurarsınız ve bu da faturanızı, müşterileriniz için satın alma ürünlerinizi ve destek altyapısını işleyebilir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-139">As an indirect reseller you will establish a relationship with an indirect provider who then can handle your billing, purchase products for your customers, and support infrastructure.</span></span>

<span data-ttu-id="aacc5-140">Farklı dolaylı sağlayıcılar farklı destek ve hizmetler sunmaktadır. bu nedenle, gereksinimlerinizi en iyi şekilde karşılayan Hizmetleri öğrenmek için bölgenizdeki sağlayıcıları değerlendirmelisiniz.</span><span class="sxs-lookup"><span data-stu-id="aacc5-140">Different indirect providers offer different support and services, so you should evaluate the providers in your area to determine which ones best meet your needs.</span></span> <span data-ttu-id="aacc5-141">Genellikle, çoğu sağlayıcı şunları olur:</span><span class="sxs-lookup"><span data-stu-id="aacc5-141">Generally, most providers will:</span></span>

- <span data-ttu-id="aacc5-142">Size teknik eğitim ve yardım sağlama</span><span class="sxs-lookup"><span data-stu-id="aacc5-142">Provide you with technical training and assistance</span></span>
- <span data-ttu-id="aacc5-143">Ürün ve hizmetlerinizi pazarlamanıza yardımcı olun</span><span class="sxs-lookup"><span data-stu-id="aacc5-143">Help you market your products and services</span></span>
- <span data-ttu-id="aacc5-144">Finans ve kredi koşullarınızı yönetin</span><span class="sxs-lookup"><span data-stu-id="aacc5-144">Manage your financing and credit terms</span></span>

<span data-ttu-id="aacc5-145">Resmi [Microsoft dolaylı sağlayıcıları](https://partnercenter.microsoft.com/partner/find-a-provider)listesinde arama yapın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-145">Search the list of official [Microsoft indirect providers](https://partnercenter.microsoft.com/partner/find-a-provider).</span></span>

<span data-ttu-id="aacc5-146">Daha fazla bilgi edinin, [dolaylı sağlayıcılarla Iş ortağı](indirect-reseller-tasks-in-partner-center.md) okuyun</span><span class="sxs-lookup"><span data-stu-id="aacc5-146">Learn more, read  [Partner with indirect providers](indirect-reseller-tasks-in-partner-center.md)</span></span>

## <a name="accept-a-partnership-invitation-from-your-indirect-provider"></a><span data-ttu-id="aacc5-147">Dolaylı sağlayıcınızdan bir ortaklık daveti kabul edin</span><span class="sxs-lookup"><span data-stu-id="aacc5-147">Accept a partnership invitation from your indirect provider</span></span>

<span data-ttu-id="aacc5-148">İş ortağına dolaylı bir sağlayıcı bulduğunuzda, Iş Ortağı Merkezi 'nde dolaylı sağlayıcıyla bir ortaklık kurun.</span><span class="sxs-lookup"><span data-stu-id="aacc5-148">When you find an indirect provider to partner with, establish a partnership with the indirect provider in Partner Center.</span></span>

<span data-ttu-id="aacc5-149">Seçtiğiniz dolaylı sağlayıcı sizi Iş ortağı merkezindeki davetine götürebileceğiniz bir ortaklık daveti e-postası adresine gönderir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-149">The indirect provider you select will send you in email a partnership invitation link that will take you to their invitation in Partner Center.</span></span> <span data-ttu-id="aacc5-150">Genel yöneticinizin Iş Ortağı Merkezi 'nde oturum açtığından ve davet bağlantısını izlediğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="aacc5-150">Be sure your global admin signs in to Partner Center and follows the invitation link.</span></span> <span data-ttu-id="aacc5-151">Daveti kabul ettiğinizde, sağlayıcının adı dolaylı sağlayıcı listenizde görünür.</span><span class="sxs-lookup"><span data-stu-id="aacc5-151">When you accept the invitation, the provider's name will appear in your indirect provider list.</span></span>

## <a name="acquire-new-customers-as-indirect-reseller"></a><span data-ttu-id="aacc5-152">Yeni müşterileri dolaylı satıcı olarak edinin</span><span class="sxs-lookup"><span data-stu-id="aacc5-152">Acquire new customers as indirect reseller</span></span>

<span data-ttu-id="aacc5-153">Hem siz hem de dolaylı sağlayıcınız müşterilerle satıcı ilişkilerine sahip olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="aacc5-153">Both you and your indirect provider need to have reseller relationships with customers.</span></span> <span data-ttu-id="aacc5-154">Bu satıcı ilişkileri, müşterinin aboneliklerini ve hizmetlerini kendi adına yönetmenize olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="aacc5-154">These reseller relationships enable you to manage a customer's subscriptions and services on their behalf.</span></span> <span data-ttu-id="aacc5-155">Mevcut bir Azure AD kiracısına sahip yeni bir müşteri edinmek için, müşteriyi hem sizinle hem de sağlayıcınızda aynı anda bir satıcı ilişkisi kurmaya davet edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="aacc5-155">To acquire a new customer who has an existing Azure AD tenant, you can invite the customer to establish a reseller relationship with both you and your provider at the same time.</span></span>

<span data-ttu-id="aacc5-156">Dolaylı bir satıcı daveti oluşturmak için:</span><span class="sxs-lookup"><span data-stu-id="aacc5-156">To create an indirect reseller invitation:</span></span>

1. <span data-ttu-id="aacc5-157">Iş ortağı merkezi sol gezininizden **dolaylı sağlayıcılar** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="aacc5-157">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="aacc5-158">Aynı anda hem sizin hem de dolaylı sağlayıcı ile satıcı ilişkisi kurmak üzere bir müşteriyi davet etmek için **yeni müşterileri davet et** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="aacc5-158">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="aacc5-159">Sağlayıcının müşteri ile bir satıcı ilişkisi olması gerekir, bu nedenle müşteri yeni abonelikler satın almak istediğinde veya mevcut aboneliklerde yeni lisanslar eklemek istediğinde müşterinin adına sipariş gönderebilirler.</span><span class="sxs-lookup"><span data-stu-id="aacc5-159">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

3. <span data-ttu-id="aacc5-160">Sonraki sayfada taslak e-posta iletisini gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="aacc5-160">On the next page, review the draft email message.</span></span> <span data-ttu-id="aacc5-161">Taslak iletisini e-postada açabilir veya iletiyi panonuza kopyalayabilir ve bir e-postaya yapıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="aacc5-161">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="aacc5-162">E-postadaki metni düzenleyerek, ihtiyacınız olanları söyleyin, ancak müşteriyi doğrudan hesabınıza ve sağlayıcınızın hesabınıza bağlamak için kişiselleştirildiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="aacc5-162">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="aacc5-163">Ardından **Bitti**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="aacc5-163">Then select **Done**.</span></span>

5. <span data-ttu-id="aacc5-164">Müşteri sizi ve sağlayıcınızı kendi kayıt satıcıları olarak doğruladıktan sonra, kendi adına aboneliklerini, lisanslarını ve kullanıcılarını yönetmek için yönetici izinlerine sahip olacaksınız ve dolaylı sağlayıcınız kendi adına sipariş gönderebilecektir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-164">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>
6. <span data-ttu-id="aacc5-165">Müşterinin hesabını, hizmetlerini, kullanıcılarını ve lisanslarını yönetmek için, adının yanındaki aşağı oku seçerek müşterinin kaydını genişletin.</span><span class="sxs-lookup"><span data-stu-id="aacc5-165">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

<span data-ttu-id="aacc5-166">Doğrudan fatura iş ortaklarının aksine, dolaylı satıcılar Iş Ortağı Merkezi 'nde yeni müşterileri için Azure AD kiracılar oluşturamaz.</span><span class="sxs-lookup"><span data-stu-id="aacc5-166">Unlike direct bill partners, indirect resellers can't create Azure AD tenants for their new customers in Partner Center.</span></span> <span data-ttu-id="aacc5-167">Sağlayıcınız kiracıyı oluşturacak ve size bu müşterinin dolaylı satıcısı olarak belirtmeyecektir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-167">Your provider will create the tenant and will specify you as the indirect reseller for this customer.</span></span> <span data-ttu-id="aacc5-168">Bu, müşterinin Iş Ortağı Merkezi 'nde müşteri listenizde görünmesini sağlar.</span><span class="sxs-lookup"><span data-stu-id="aacc5-168">This ensures that the customer will appear in your customer list in Partner Center.</span></span>

>[!Note]
><span data-ttu-id="aacc5-169">Dolaylı satıcı olarak aldığınız müşteriler için satın alma işlemleri oluşturmak üzere doğrudan fatura özelliğini kullanamazsınız.</span><span class="sxs-lookup"><span data-stu-id="aacc5-169">You will not be able to use your direct bill capability to create purchases for customers you acquire as an indirect reseller.</span></span>

## <a name="managing-your-direct-bill-customers-and-your-indirect-reseller-customers"></a><span data-ttu-id="aacc5-170">Doğrudan Bill müşterilerini ve dolaylı satıcı müşterilerinizi yönetme</span><span class="sxs-lookup"><span data-stu-id="aacc5-170">Managing your direct bill customers and your indirect reseller customers</span></span>

<span data-ttu-id="aacc5-171">Doğrudan fatura müşterilerinizi ve dolaylı satıcı müşterilerinizi farklı şekilde yönetirsiniz.</span><span class="sxs-lookup"><span data-stu-id="aacc5-171">You manage your direct bill customers and your indirect reseller customers differently.</span></span>

### <a name="direct-bill-customers-things-you-wont-do-as-an-indirect-reseller"></a><span data-ttu-id="aacc5-172">Doğrudan fatura müşterileri (dolaylı satıcı olarak yapamayabilmeniz gerekir)</span><span class="sxs-lookup"><span data-stu-id="aacc5-172">Direct bill customers (things you won't do as an indirect reseller)</span></span>

- <span data-ttu-id="aacc5-173">Ürünler için sipariş oluşturma</span><span class="sxs-lookup"><span data-stu-id="aacc5-173">Create orders for products</span></span>
- <span data-ttu-id="aacc5-174">Azure ayırmalarını yönetme</span><span class="sxs-lookup"><span data-stu-id="aacc5-174">Manage Azure reservations</span></span>
- <span data-ttu-id="aacc5-175">Sıra geçmişini yönetme</span><span class="sxs-lookup"><span data-stu-id="aacc5-175">Manage their order history</span></span>
- <span data-ttu-id="aacc5-176">Satın alma yazılımı</span><span class="sxs-lookup"><span data-stu-id="aacc5-176">Purchase software</span></span>
- <span data-ttu-id="aacc5-177">Doğrudan fatura müşterileri</span><span class="sxs-lookup"><span data-stu-id="aacc5-177">Bill customers directly</span></span>

### <a name="indirect-reseller-customers"></a><span data-ttu-id="aacc5-178">Dolaylı satıcı müşterileri</span><span class="sxs-lookup"><span data-stu-id="aacc5-178">Indirect reseller customers</span></span>

- <span data-ttu-id="aacc5-179">Dolaylı sağlayıcınız, müşterileriniz için ürünleri sipariş eden</span><span class="sxs-lookup"><span data-stu-id="aacc5-179">Your indirect provider orders products for your customers</span></span>
- <span data-ttu-id="aacc5-180">Müşterilerin lisanslarını ve kullanıcılarını yönetme</span><span class="sxs-lookup"><span data-stu-id="aacc5-180">Manage customers' licenses and users</span></span>
- <span data-ttu-id="aacc5-181">Abonelik yenilemeler işleme</span><span class="sxs-lookup"><span data-stu-id="aacc5-181">Handle subscription renewals</span></span>

### <a name="to-identify-customers-that-you-acquired-as-a-direct-bill-partner"></a><span data-ttu-id="aacc5-182">Doğrudan bir fatura ortağı olarak edindiğiniz müşterileri belirlemek için</span><span class="sxs-lookup"><span data-stu-id="aacc5-182">To identify customers that you acquired as a direct bill partner</span></span>

1. <span data-ttu-id="aacc5-183">**Müşteriler**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="aacc5-183">Select **Customers**.</span></span>

2. <span data-ttu-id="aacc5-184">Ayrıntılarını görüntülemek için bir müşteri seçin.</span><span class="sxs-lookup"><span data-stu-id="aacc5-184">Select a customer to view their details.</span></span>

3. <span data-ttu-id="aacc5-185">Bu müşteri doğrudan fatura ortağı olarak elde ediyorsanız, ürün **ekleme** veya **görüntüleme** seçeneklerini görürsünüz ve aboneliklerini görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="aacc5-185">If this customer is one you acquired as a direct bill partner, you will see options to **add** or **view products** and you will see their subscriptions.</span></span>

4. <span data-ttu-id="aacc5-186">Müşterinin sizinle dolaylı bir satıcı ilişkisi varsa, bu seçenekler kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="aacc5-186">If the customer has an indirect reseller relationship with you, those options will not be available.</span></span>

## <a name="move-your-direct-bill-customers-to-your-indirect-provider"></a><span data-ttu-id="aacc5-187">Doğrudan fatura müşterilerinizi dolaylı sağlayıcınıza taşıyın</span><span class="sxs-lookup"><span data-stu-id="aacc5-187">Move your direct bill customers to your indirect provider</span></span>

<span data-ttu-id="aacc5-188">Dolaylı sağlayıcınız, mevcut doğrudan fatura müşterileriniz için bir satıcı ilişkisine sahip olana kadar sipariş veya mevcut abonelik aktarımları gönderemez.</span><span class="sxs-lookup"><span data-stu-id="aacc5-188">Your indirect provider cannot submit orders or existing subscription transfers for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="aacc5-189">Dolaylı sağlayıcınız ile var olan doğrudan faturanız arasındaki satıcı ilişkilerini oluşturmak için aşağıdaki yöntemlerden birini kullanabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="aacc5-189">To establish the reseller relationship between your indirect provider and your existing direct bill customer, you can use one of the following methods:</span></span>

- [<span data-ttu-id="aacc5-190">Satıcı ilişki uzantısı</span><span class="sxs-lookup"><span data-stu-id="aacc5-190">Reseller relationship extension</span></span>](#reseller-relationship-extension)

- [<span data-ttu-id="aacc5-191">Müşteriye dolaylı bir satıcı davetiyesi gönderin</span><span class="sxs-lookup"><span data-stu-id="aacc5-191">Send an indirect reseller invitation to the customer</span></span>](#send-an-indirect-reseller-invitation-to-the-customer)

<span data-ttu-id="aacc5-192">[Doğrudan dolaylı geçiş belgesinde](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/) adım adım işleme yönelik ayrıntılı bir genel bakış bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="aacc5-192">You can find a detailed overview of the step-by-step process in the [Direct to indirect transition document](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span></span>

### <a name="reseller-relationship-extension"></a><span data-ttu-id="aacc5-193">Satıcı ilişki uzantısı</span><span class="sxs-lookup"><span data-stu-id="aacc5-193">Reseller relationship extension</span></span>

<span data-ttu-id="aacc5-194">Kurumsal ilişki uzantısı özelliğini kullanarak, mevcut doğrudan fatura müşterileriniz ve dolaylı sağlayıcınız arasında Iş Ortağı Merkezi panosunu kullanarak satıcı ilişkisi kurabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="aacc5-194">You can use the reseller relationship extension feature to establish reseller relationship between your existing direct bill customers and your indirect provider using Partner Center Dashboard.</span></span> <span data-ttu-id="aacc5-195">Özelliği kullanmadan önce, aşağıdakilere göz önüne alın:</span><span class="sxs-lookup"><span data-stu-id="aacc5-195">Before using the feature, note the following:</span></span>

- <span data-ttu-id="aacc5-196">Bu özellik yalnızca dolaylı satıcı olan dolaylı satıcı [kaydını](#get-started)tamamlamış olan doğrudan fatura ortakları tarafından kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-196">This feature is only available to direct bill partners who are transitioning to become an indirect reseller have completed the [indirect reseller enrollment](#get-started).</span></span>

- <span data-ttu-id="aacc5-197">Bu özelliği yalnızca var olan doğrudan fatura müşterilerine uygulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="aacc5-197">You can only apply this feature to existing direct bill customers.</span></span> <span data-ttu-id="aacc5-198">Bu, [dolaylı satıcı müşterileri](#acquire-new-customers-as-indirect-reseller)için geçerli değildir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-198">It is not applicable to [indirect reseller customers](#acquire-new-customers-as-indirect-reseller).</span></span>

- <span data-ttu-id="aacc5-199">Yalnızca [dolaylı sağlayıcıınızdan bir iş ortağı davetini kabul](#accept-a-partnership-invitation-from-your-indirect-provider)ettiğiniz bir dolaylı sağlayıcıyı seçebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="aacc5-199">You can only select an indirect provider for which you have [accepted a partner invitation from your indirect provider](#accept-a-partnership-invitation-from-your-indirect-provider).</span></span>

- <span data-ttu-id="aacc5-200">Bu müşteri için sahip olduğunuz fatura-bilgi bilgilerinin bir kopyası dolaylı sağlayıcı tarafından kullanılabilir hale getirilir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-200">A copy of the bill-to info you have for this customer will be made available to the indirect provider.</span></span> <span data-ttu-id="aacc5-201">Iş Ortağı Merkezi panosunda bu müşterinin hesap sayfasına erişerek fatura bilgilerine erişebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="aacc5-201">You can access the bill-to info by accessing the Account page for this customer in Partner Center Dashboard.</span></span>

    > [!NOTE]
    > <span data-ttu-id="aacc5-202">Satıcı ilişki uzantısı özelliğini kullanarak, bu müşteri için sahip olduğunuz fatura bilgilerini dolaylı sağlayıcıyla paylaşmayı kabul etmiş olursunuz.</span><span class="sxs-lookup"><span data-stu-id="aacc5-202">By using the reseller relationship extension feature, you consent to sharing the bill-to info you have for this customer with the indirect provider.</span></span>

- <span data-ttu-id="aacc5-203">Dolaylı sağlayıcınız, müşteri kiracısına [atanan yönetim ayrıcalıkları](customers-revoke-admin-privileges.md) ile birlikte sağlanmaz.</span><span class="sxs-lookup"><span data-stu-id="aacc5-203">Your indirect provider will not be provided with [delegated administration privileges](customers-revoke-admin-privileges.md) to the customer tenant.</span></span> <span data-ttu-id="aacc5-204">Dolaylı sağlayıcınız Temsilcili yönetim ayrıcalıkları gerektiriyorsa, bunun yerine müşteriye dolaylı bir satıcı daveti göndermeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-204">If your indirect provider requires delegated administration privileges, you must send an indirect reseller invitation to the customer instead.</span></span>

- <span data-ttu-id="aacc5-205">Satıcı ilişkisi kurulduktan sonra, dolaylı sağlayıcı, [Microsoft 365 Yönetim Merkezi](https://admin.microsoft.com/AdminPortal/Home#/partners) ve [Iş Microsoft Store iş](/microsoft-store/work-with-partner-microsoft-store-business)ortağı ilişkiler sayfasının altında, müşterinin bir CSP iş ortağı olarak görünür.</span><span class="sxs-lookup"><span data-stu-id="aacc5-205">Once the reseller relationship is established, the indirect provider will appear as a CSP partner to the customer under the Partner Relationships page in [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/partners) and [Microsoft Store for Business](/microsoft-store/work-with-partner-microsoft-store-business).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="aacc5-206">Karışıklık ve anlaşılmadan kaçınmak için, mevcut bir doğrudan fatura müşterisi ve dolaylı bir sağlayıcı arasında satıcı ilişkisi kurmak üzere ilişki uzantısı özelliğini kullanmadan önce, iş ortağı sözleşmenizde sözleşmeye dayalı yükümlülüğü vardır.</span><span class="sxs-lookup"><span data-stu-id="aacc5-206">To avoid confusion and misunderstanding, you are contractually obliged by your partner agreement to inform and obtain consent from the direct bill customer before you use the relationship extension feature to establish reseller relationship between an existing direct bill customer and an indirect provider.</span></span>

<span data-ttu-id="aacc5-207">Bu özelliği mevcut bir müşteri kiracısında kullanmak için:</span><span class="sxs-lookup"><span data-stu-id="aacc5-207">To use this feature on an existing customer tenant:</span></span>

1. <span data-ttu-id="aacc5-208">Iş Ortağı Merkezi ' nde bir **Yönetim Aracısı** olarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-208">Log in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="aacc5-209">**Müşteriler sayfasında**, mevcut bir müşteriyi seçin ve müşterinin Özet görünümünü genişletmek için **hızlı bağlantılar** simgesine tıklayın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-209">In the **Customers page**, select an existing customer and click on its **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="aacc5-210">**Dolaylı sağlayıcılar**' ın altında, **dolaylı bir sağlayıcıda müşteriyi aktar**' a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-210">Under **Indirect provider(s)**, click **Transfer customer on an indirect provider**.</span></span>

    :::image type="content" source="images/direct/direct5-1.png" alt-text="Müşteriyi dolaylı bir sağlayıcıya aktarma":::

4. <span data-ttu-id="aacc5-212">Açılır iletişim kutusunda, müşteri ile satıcı ilişkisi olmasını istediğiniz **dolaylı sağlayıcıyı** seçin.</span><span class="sxs-lookup"><span data-stu-id="aacc5-212">In the pop-up dialog, select the **Indirect Provider** you would like to have reseller relationship with the customer.</span></span>

5. <span data-ttu-id="aacc5-213">**Kaydet ve devam et**' e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-213">Click **Save and continue**.</span></span>

6. <span data-ttu-id="aacc5-214">Seçilen dolaylı sağlayıcının **dolaylı sağlayıcılar** altında görüntülendiğini doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-214">Verify the selected indirect provider shows up under **Indirect provider(s)**.</span></span>

    :::image type="content" source="images/direct/direct5-2.png" alt-text="Belirtilen dolaylı sağlayıcı":::

### <a name="send-an-indirect-reseller-invitation-to-the-customer"></a><span data-ttu-id="aacc5-216">Müşteriye dolaylı bir satıcı davetiyesi gönderin</span><span class="sxs-lookup"><span data-stu-id="aacc5-216">Send an indirect reseller invitation to the customer</span></span>

<span data-ttu-id="aacc5-217">Dolaylı sağlayıcınız, mevcut doğrudan fatura müşterileriniz için bir satıcı ilişkisine sahip olana kadar sipariş gönderemezler.</span><span class="sxs-lookup"><span data-stu-id="aacc5-217">Your indirect provider cannot submit orders for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="aacc5-218">Mevcut müşterileriniz ve dolaylı sağlayıcınız arasında satıcı ilişkisi kurmak için, dolaylı bir satıcı davetiyesi kullanarak müşteriyi davet edin.</span><span class="sxs-lookup"><span data-stu-id="aacc5-218">To establish the reseller relationship between your existing customers and your indirect provider, invite the customer using an indirect reseller invitation.</span></span>

1. <span data-ttu-id="aacc5-219">Iş ortağı merkezi sol gezininizden **dolaylı sağlayıcılar** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="aacc5-219">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="aacc5-220">Aynı anda hem sizin hem de dolaylı sağlayıcı ile satıcı ilişkisi kurmak üzere bir müşteriyi davet etmek için **yeni müşterileri davet et** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="aacc5-220">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="aacc5-221">Sağlayıcının müşteri ile bir satıcı ilişkisi olması gerekir, bu nedenle müşteri yeni abonelikler satın almak istediğinde veya mevcut aboneliklerde yeni lisanslar eklemek istediğinde müşterinin adına sipariş gönderebilirler.</span><span class="sxs-lookup"><span data-stu-id="aacc5-221">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

    :::image type="content" source="images/direct/direct6.png" alt-text="Yeni müşterileri davet et":::

3. <span data-ttu-id="aacc5-223">Sonraki sayfada taslak e-posta iletisini gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="aacc5-223">On the next page, review the draft email message.</span></span> <span data-ttu-id="aacc5-224">Taslak iletisini e-postada açabilir veya iletiyi panonuza kopyalayabilir ve bir e-postaya yapıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="aacc5-224">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="aacc5-225">E-postadaki metni düzenleyerek, ihtiyacınız olanları söyleyin, ancak müşteriyi doğrudan hesabınıza ve sağlayıcınızın hesabınıza bağlamak için kişiselleştirildiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="aacc5-225">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="aacc5-226">Ardından **Bitti**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="aacc5-226">Then select **Done**.</span></span>

5. <span data-ttu-id="aacc5-227">Müşteri sizi ve sağlayıcınızı kendi kayıt satıcıları olarak doğruladıktan sonra, kendi adına aboneliklerini, lisanslarını ve kullanıcılarını yönetmek için yönetici izinlerine sahip olacaksınız ve dolaylı sağlayıcınız kendi adına sipariş gönderebilecektir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-227">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>

6. <span data-ttu-id="aacc5-228">Müşterinin hesabını, hizmetlerini, kullanıcılarını ve lisanslarını yönetmek için, adının yanındaki aşağı oku seçerek müşterinin kaydını genişletin.</span><span class="sxs-lookup"><span data-stu-id="aacc5-228">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

### <a name="microsoft-customer-agreement-acceptance"></a><span data-ttu-id="aacc5-229">Microsoft Müşteri Sözleşmesi kabulü</span><span class="sxs-lookup"><span data-stu-id="aacc5-229">Microsoft Customer Agreement acceptance</span></span>

<span data-ttu-id="aacc5-230">Microsoft Bulut sözleşmesi 31 Ocak 2020 ' ye kadar geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-230">Microsoft Cloud Agreement is valid until January 31, 2020.</span></span> <span data-ttu-id="aacc5-231">Bu tarihten sonra, mevcut ve yeni olan tüm müşteriler yeni [Microsoft Müşteri sözleşmesinin](confirm-customer-agreement.md)imzalanmalıdır.</span><span class="sxs-lookup"><span data-stu-id="aacc5-231">After that date, all customers, existing and new, must sign the new [Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span> <span data-ttu-id="aacc5-232">Şu durumlarda müşterilerin geçişini yapmak için:</span><span class="sxs-lookup"><span data-stu-id="aacc5-232">For transitioning customers, if:</span></span>

- <span data-ttu-id="aacc5-233">**Müşteri henüz Microsoft Müşteri sözleşmesini kabul etmedi**</span><span class="sxs-lookup"><span data-stu-id="aacc5-233">**Customer has not accepted Microsoft Customer Agreement yet**</span></span>

   <span data-ttu-id="aacc5-234">Müşterinin [Microsoft Müşteri anlaşmasını kabul](confirm-customer-agreement.md)etmesi Için lütfen dolaylı sağlayıcıyla çalışın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-234">Please work with Indirect Provider to have customer [accept the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

- <span data-ttu-id="aacc5-235">**Müşteri, Microsoft 365 Yönetim Merkezi ile Microsoft Müşteri anlaşmasını sizinle kabul etti**</span><span class="sxs-lookup"><span data-stu-id="aacc5-235">**Customer has accepted Microsoft Customer Agreement with you through the Microsoft 365 Admin Center**</span></span>

   <span data-ttu-id="aacc5-236">Satıcı ilişkisi dolaylı sağlayıcıyla kurulduktan sonra kabul edilir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-236">The acceptance will be retained once the reseller relationship is established with the Indirect Provider.</span></span> <span data-ttu-id="aacc5-237">Yapmanız gereken bir şey yok.</span><span class="sxs-lookup"><span data-stu-id="aacc5-237">There is nothing you need to do.</span></span>

- <span data-ttu-id="aacc5-238">**Müşteri, iş ortağı kanıtlama ile Microsoft Müşteri sözleşmesini kabul etti**</span><span class="sxs-lookup"><span data-stu-id="aacc5-238">**Customer has accepted Microsoft Customer Agreement with you through partner attestation**</span></span>

   <span data-ttu-id="aacc5-239">Kabul tutulmayacaktır.</span><span class="sxs-lookup"><span data-stu-id="aacc5-239">The acceptance will not be retained.</span></span> <span data-ttu-id="aacc5-240">[Müşterinin Iş Ortağı Merkezi 'nin kabulünü güncelleştirmek](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers)Için lütfen dolaylı sağlayıcıyla çalışın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-240">Please work with Indirect Provider to [update the customer's acceptance in Partner Center](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span></span>

## <a name="transfer-existing-direct-bill-subscriptions-to-indirect-provider"></a><span data-ttu-id="aacc5-241">Mevcut doğrudan fatura aboneliklerini dolaylı sağlayıcıya aktar</span><span class="sxs-lookup"><span data-stu-id="aacc5-241">Transfer existing direct bill subscriptions to indirect provider</span></span>

<span data-ttu-id="aacc5-242">CSP dolaylı modeli kapsamında, dolaylı satıcıların Microsoft ile faturalandırma ilişkileri yoktur.</span><span class="sxs-lookup"><span data-stu-id="aacc5-242">Under CSP indirect model, indirect resellers do not have billing relationships with Microsoft.</span></span> <span data-ttu-id="aacc5-243">Bunun yerine dolaylı satıcılar, kendi dolaylı sağlayıcıları aracılığıyla müşterileri için abonelikler elde eder.</span><span class="sxs-lookup"><span data-stu-id="aacc5-243">Instead, indirect resellers obtain subscriptions for their customers through their indirect providers.</span></span> <span data-ttu-id="aacc5-244">Doğrudan fatura ortağından dolaylı satıcıya geçiş yaparken, sahip olduğunuz mevcut abonelikleri dolaylı sağlayıcınıza doğrudan fatura ortağı olarak aktarmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-244">While transitioning from direct bill partner to indirect reseller, you need to transfer the existing subscriptions you have as the direct bill partner to your indirect provider.</span></span> <span data-ttu-id="aacc5-245">Bunu yapmak için, Iş Ortağı Merkezi panosunda kendi kendine sunulan abonelik aktarma özelliğini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="aacc5-245">You can use the self-served subscription transfer feature in Partner Center Dashboard to do so.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="aacc5-246">Önkoşullar</span><span class="sxs-lookup"><span data-stu-id="aacc5-246">Prerequisites</span></span>

- <span data-ttu-id="aacc5-247">Bu özellik yalnızca mevcut doğrudan fatura ortağı kiracılarını kullanarak dolaylı satıcı kaydını tamamlamış olan iş ortakları arasında geçiş yapılabilir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-247">This feature is only available to transitioning partners who have completed the indirect reseller enrollment using their existing direct bill partner tenants.</span></span>

- <span data-ttu-id="aacc5-248">Belirli bir müşteriyle ilişkili abonelikleri aktarmadan önce, geçiş ortağı müşteriyi dolaylı bir sağlayıcıya taşımalıdır.</span><span class="sxs-lookup"><span data-stu-id="aacc5-248">Before transferring subscriptions associated with a given customer, the transitioning partner must move the customer to an indirect provider.</span></span>

- <span data-ttu-id="aacc5-249">Müşterinin [dolaylı sağlayıcı aracılığıyla Microsoft Müşteri anlaşmasını kabul](#microsoft-customer-agreement-acceptance)etmiş olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-249">Customer must have [accepted Microsoft Customer Agreement through the Indirect Provider](#microsoft-customer-agreement-acceptance).</span></span>

### <a name="how-to-transition-to-indirect-reseller-status"></a><span data-ttu-id="aacc5-250">Dolaylı satıcı durumuna geçiş</span><span class="sxs-lookup"><span data-stu-id="aacc5-250">How to transition to indirect reseller status</span></span>

<span data-ttu-id="aacc5-251">Özelliği 4 adımlı bir işlemdir; burada:</span><span class="sxs-lookup"><span data-stu-id="aacc5-251">The feature is a 4-step process, where:</span></span>

- <span data-ttu-id="aacc5-252">Geçiş ortağı bir abonelik aktarma isteği oluşturur.</span><span class="sxs-lookup"><span data-stu-id="aacc5-252">The transitioning partner creates a subscription transfer request.</span></span> <span data-ttu-id="aacc5-253">İstek, aynı müşteriyle ilişkili bir veya daha fazla var olan abonelik içeriyor ve dolaylı bir sağlayıcıya yönelik.</span><span class="sxs-lookup"><span data-stu-id="aacc5-253">The request contains one or more existing subscriptions associated with the same customer and is addressed to an indirect provider.</span></span>

- <span data-ttu-id="aacc5-254">Dolaylı sağlayıcı, aktarım isteğini gözden geçirir ve kabul eder (veya reddeder).</span><span class="sxs-lookup"><span data-stu-id="aacc5-254">The indirect provider reviews and accepts (or reject) the transfer request.</span></span>

- <span data-ttu-id="aacc5-255">Dolaylı sağlayıcı, aktarım isteğinin tamamlandığını doğrular.</span><span class="sxs-lookup"><span data-stu-id="aacc5-255">The indirect provider verifies that the transfer request is complete.</span></span>

- <span data-ttu-id="aacc5-256">Geçiş ortağı, aktarım isteğinin tamamlandığını doğrular.</span><span class="sxs-lookup"><span data-stu-id="aacc5-256">The transitioning partner verifies that the transfer request is complete.</span></span>

### <a name="transitioning-partner"></a><span data-ttu-id="aacc5-257">İş ortağı geçiyor</span><span class="sxs-lookup"><span data-stu-id="aacc5-257">Transitioning partner</span></span>

> [!NOTE]
> <span data-ttu-id="aacc5-258">Ayrıca, mevcut abonelikleri dolaylı sağlayıcınıza aktarmak için [Iş ortağı MERKEZI API/SDK](/partner-center/develop/manage-customers) 'sını de kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="aacc5-258">You can also use [Partner Center API/SDK](/partner-center/develop/manage-customers) to transfer the existing subscriptions to your indirect provider.</span></span>
>
> - [<span data-ttu-id="aacc5-259">Müşterinin abonelik aktarım uygunluğunu alma</span><span class="sxs-lookup"><span data-stu-id="aacc5-259">Get a customer's subscriptions transfer eligibility</span></span>](/partner-center/develop/get-customer-s-subscriptions-transfer-eligibility)
> - [<span data-ttu-id="aacc5-260">Müşterinin aktarımını oluşturma</span><span class="sxs-lookup"><span data-stu-id="aacc5-260">Create a customer's transfer</span></span>](/partner-center/develop/create-a-transfer)
> - [<span data-ttu-id="aacc5-261">Müşterinin aktarımını geri alma</span><span class="sxs-lookup"><span data-stu-id="aacc5-261">Withdraw a customer's transfer</span></span>](/partner-center/develop/withdraw-a-transfer)
> - [<span data-ttu-id="aacc5-262">Müşterinin aktarımını kabul etme</span><span class="sxs-lookup"><span data-stu-id="aacc5-262">Accept a customer's transfer</span></span>](/partner-center/develop/accept-a-transfer)
> - [<span data-ttu-id="aacc5-263">Müşterinin aktarımını reddetme</span><span class="sxs-lookup"><span data-stu-id="aacc5-263">Reject a Customer's transfer</span></span>](/partner-center/develop/reject-a-transfer)
> - [<span data-ttu-id="aacc5-264">Müşterinin aktarımlarını alma</span><span class="sxs-lookup"><span data-stu-id="aacc5-264">Get a customer's transfers</span></span>](/partner-center/develop/get-all-of-a-customer-s-transfers)
> - [<span data-ttu-id="aacc5-265">Kimliğe göre aktarım ayrıntılarını al</span><span class="sxs-lookup"><span data-stu-id="aacc5-265">Get transfer details by id</span></span>](/partner-center/develop/get-transfer-by-id)

### <a name="transitioning-partner---create-transfer-request"></a><span data-ttu-id="aacc5-266">İş ortağı geçişi-aktarım isteği oluşturma</span><span class="sxs-lookup"><span data-stu-id="aacc5-266">Transitioning partner - create transfer request</span></span>

<span data-ttu-id="aacc5-267">Geçiş ortağı olarak bir aktarım isteği oluşturmak için:</span><span class="sxs-lookup"><span data-stu-id="aacc5-267">To create a transfer request as the transitioning partner:</span></span>

1. <span data-ttu-id="aacc5-268">Iş Ortağı Merkezi ' nde bir **Yönetim Aracısı** olarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-268">Log in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="aacc5-269">**Müşteriler** sayfasında, istenen müşteriyi seçin ve hızlı bağlantılar simgesine tıklayarak müşterinin Özet görünümünü genişletin.</span><span class="sxs-lookup"><span data-stu-id="aacc5-269">In the **Customers** page, select the intended customer and click on the Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="aacc5-270">**Dolaylı sağlayıcılar**' ın altında, amaçlanan dolaylı sağlayıcının listelendiğini onaylayın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-270">Under **Indirect provider(s)**, confirm that the intended indirect provider is listed.</span></span>

4. <span data-ttu-id="aacc5-271">**Abonelikleri görüntüle**' ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-271">Click **View Subscriptions**.</span></span>

5. <span data-ttu-id="aacc5-272">**Abonelikler** sayfasında, **abonelik aktarımı**' nı arayın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-272">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

6. <span data-ttu-id="aacc5-273">**Abonelik aktarımı** altında **abonelik aktarımı iste**' ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-273">Under **Subscription Transfer**, click **Request subscription transfer**.</span></span>

    :::image type="content" source="images/direct/direct8.png" alt-text="Abonelik aktarımı iste":::

7. <span data-ttu-id="aacc5-275">Aktarım isteği iletişim kutusunda, aktarılacak bir veya daha fazla abonelik seçin.</span><span class="sxs-lookup"><span data-stu-id="aacc5-275">In the transfer request dialog, select one or more subscriptions to be transferred.</span></span>

    :::image type="content" source="images/direct/direct9.png" alt-text="Aktarım Isteği oluştur":::

8. <span data-ttu-id="aacc5-277">**Oluştur**’a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-277">Click **Create**.</span></span>

9. <span data-ttu-id="aacc5-278">**Abonelik aktarımı** altında, etkin bir abonelik aktarım isteği görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-278">An active subscription transfer request will appear under **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct10.png" alt-text="İstek listesini aktar":::

10. <span data-ttu-id="aacc5-280">Dolaylı sağlayıcınızı, bunlara bir abonelik aktarım isteği oluşturduğunu bildirin.</span><span class="sxs-lookup"><span data-stu-id="aacc5-280">Inform your indirect provider that you have created a subscription transfer request to them.</span></span>

### <a name="indirect-provider---accept-transfer-request"></a><span data-ttu-id="aacc5-281">Dolaylı sağlayıcı-aktarım isteğini kabul et</span><span class="sxs-lookup"><span data-stu-id="aacc5-281">Indirect provider - accept transfer request</span></span>

<span data-ttu-id="aacc5-282">Bir aktarım isteğini dolaylı sağlayıcı olarak gözden geçirmek ve kabul etmek için:</span><span class="sxs-lookup"><span data-stu-id="aacc5-282">To review and accept a transfer request as the indirect provider:</span></span>

1. <span data-ttu-id="aacc5-283">Iş Ortağı Merkezi 'nde bir **Yönetim** Aracısı veya **Satış Aracısı** olarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-283">Log in to Partner Center as an **Admin** Agent or **Sales Agent**.</span></span>

2. <span data-ttu-id="aacc5-284">**Müşteriler** sayfasında, istenen müşteriyi seçin ve müşterinin Özet görünümünü genişletmek için hızlı bağlantılar simgesine tıklayın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-284">In the **Customers** page, select the intended customer and click on its Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="aacc5-285">**Dolaylı satıcı (ler)** altında, geçiş ortağının listelendiğini onaylayın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-285">Under **Indirect reseller(s)**, confirm the transitioning partner is listed.</span></span>

4. <span data-ttu-id="aacc5-286">**Abonelikleri görüntüle**' ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-286">Click **View Subscriptions**.</span></span>

5. <span data-ttu-id="aacc5-287">**Abonelikler** sayfasında, **abonelik aktarımı**' nı arayın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-287">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct11.png" alt-text="Aktarım isteğini görüntüle":::

6. <span data-ttu-id="aacc5-289">**Abonelik aktarımı** altında, gözden geçirmek için aktarım isteğine tıklayın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-289">Under **Subscription Transfer**, click on the transfer request to review.</span></span>

7. <span data-ttu-id="aacc5-290">Uygun şekilde **kabul et** (veya **Reddet**) seçeneğine tıklayın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-290">Click **Accept** (or **Reject**) as appropriate.</span></span>

    :::image type="content" source="images/direct/direct12.png" alt-text="Aktarım isteğini kabul et":::

8. <span data-ttu-id="aacc5-292">Aktarım isteğinin tamamlanmasını bekleyin.</span><span class="sxs-lookup"><span data-stu-id="aacc5-292">Wait for the transfer request to complete.</span></span>

### <a name="indirect-provider---verify-transfer-request-is-complete"></a><span data-ttu-id="aacc5-293">Dolaylı sağlayıcı-aktarım isteğinin tamamlandığını doğrulama</span><span class="sxs-lookup"><span data-stu-id="aacc5-293">Indirect provider - verify transfer request is complete</span></span>

1. <span data-ttu-id="aacc5-294">Aktarım isteği başarıyla tamamlandıktan sonra, aboneliklerin **abonelikler** bölümünde göründüğünü görebildiğinizi doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-294">After the transfer request is completed successfully, verify that you can see the subscriptions appear under **Subscriptions**.</span></span>

2. <span data-ttu-id="aacc5-295">Geçiş ortağına bildirin.</span><span class="sxs-lookup"><span data-stu-id="aacc5-295">Inform the transitioning partner.</span></span>

### <a name="transitioning-partner---verify-transfer-request-is-complete"></a><span data-ttu-id="aacc5-296">Geçiş ortağı-aktarım isteğini doğrulama işlemi tamamlanmıştır</span><span class="sxs-lookup"><span data-stu-id="aacc5-296">Transitioning partner - verify transfer request is complete</span></span>

<span data-ttu-id="aacc5-297">Geçiş ortağı aşağıdakileri yapması gerekir:</span><span class="sxs-lookup"><span data-stu-id="aacc5-297">The transitioning partner should do the following:</span></span>

1. <span data-ttu-id="aacc5-298">Iş Ortağı Merkezi 'Nde bir **Yönetim Aracısı** veya **Satış Aracısı** olarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-298">Sign into Partner Center as an **Admin Agent** or **Sales Agent**.</span></span>

2. <span data-ttu-id="aacc5-299">**Müşteriler** sayfasında, istenen müşteriyi seçin ve **hızlı bağlantılar** simgesine tıklayarak müşterinin Özet görünümünü genişletin.</span><span class="sxs-lookup"><span data-stu-id="aacc5-299">In the **Customers** page, select the intended customer and click on the **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="aacc5-300">**Abonelikleri görüntüle**' ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-300">Click **View Subscriptions**.</span></span>

4. <span data-ttu-id="aacc5-301">**Abonelikler** sayfasında, **abonelik aktarımı**' nı arayın.</span><span class="sxs-lookup"><span data-stu-id="aacc5-301">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

5. <span data-ttu-id="aacc5-302">Aktarım isteğinin **Tamam** olarak işaretlendiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="aacc5-302">Verify that the transfer request is marked as **Complete**.</span></span>

6. <span data-ttu-id="aacc5-303">Aboneliğin artık **abonelikler** sayfasında etkin olarak görünmediğini doğrulayın:</span><span class="sxs-lookup"><span data-stu-id="aacc5-303">Verify that the subscription(s) no longer appear as active in the **Subscriptions** page:</span></span>

   1. <span data-ttu-id="aacc5-304">Bu bir Azure aboneliğse (MS-AZR-0145P), artık listelenmez.</span><span class="sxs-lookup"><span data-stu-id="aacc5-304">If this is an Azure subscription (MS-AZR-0145P), it will no longer be listed.</span></span>

   2. <span data-ttu-id="aacc5-305">Bu bir lisans tabanlı aboneliğiniz (Office 365, Dynamics, Intune), durumu **askıya alındı** olarak listelenir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-305">If this is a license-based subscription (Office 365, Dynamics, Intune), it will be listed with state as **Suspended**.</span></span>

   :::image type="content" source="images/direct/direct13.png" alt-text="Abonelik askıya alındı":::

### <a name="considerations"></a><span data-ttu-id="aacc5-307">Dikkat edilmesi gerekenler</span><span class="sxs-lookup"><span data-stu-id="aacc5-307">Considerations</span></span>

- <span data-ttu-id="aacc5-308">**Abonelik KIMLIĞI aktarımdan sonra farklı olacaktır.**</span><span class="sxs-lookup"><span data-stu-id="aacc5-308">**Subscription ID will be different after transfer.**</span></span> <span data-ttu-id="aacc5-309">Bu bir Azure aboneliğiyiyse (MS-AZR-0145P), buna ek olarak, önceki sahibinden tutulan ve Azure yönetim portalında görünecek bir Azure abonelik KIMLIĞI olur.</span><span class="sxs-lookup"><span data-stu-id="aacc5-309">If it is an Azure subscription (MS-AZR-0145P), additionally, it will have an Azure Subscription ID, which is retained from the previous owner, and will appear in the Azure management portal.</span></span>

- <span data-ttu-id="aacc5-310">**Aynı aboneliğe birden çok aktarım isteği tarafından başvurulamaz.**</span><span class="sxs-lookup"><span data-stu-id="aacc5-310">**The same subscription cannot be referenced by multiple transfer requests.**</span></span> <span data-ttu-id="aacc5-311">Mevcut bir aboneliği içeren bir aktarım isteği oluşturduktan sonra, ilk aktarım isteği iptal edilene kadar aynı abonelik dahil olmak üzere ek aktarım istekleri oluşturamazsınız.</span><span class="sxs-lookup"><span data-stu-id="aacc5-311">After you have created a transfer request, which includes an existing subscription, you cannot create additional transfer requests including the same subscription, until the first transfer request is canceled.</span></span>

- <span data-ttu-id="aacc5-312">**Lisans tabanlı abonelikler için eklentiler, temel abonelikleriyle birlikte aktarılmalıdır.**</span><span class="sxs-lookup"><span data-stu-id="aacc5-312">**Add-ons for license-based subscriptions must be transferred along with their base subscription.**</span></span> <span data-ttu-id="aacc5-313">Bir aktarım isteği oluştururken, bir veya daha fazla eklentiye sahip mevcut bir aboneliği seçerseniz, eklenti otomatik olarak aktarım isteğine dahil edilir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-313">When creating a transfer request, if you pick an existing subscription with one or more add-ons, the add-ons will automatically be included in the transfer request.</span></span>

- <span data-ttu-id="aacc5-314">**Bir abonelikte lisans sayısı değişiklikleri var olan aktarım isteğine yansıtılmayacaktır.**</span><span class="sxs-lookup"><span data-stu-id="aacc5-314">**License count changes to a subscription will not be reflected in existing transfer request.**</span></span> <span data-ttu-id="aacc5-315">Var olan bir aboneliği içeren bir aktarım isteği oluşturduktan sonra, aboneliğin lisans miktarını (veya ilişkili eklentiler) güncelleştirmeden kaçınmalısınız.</span><span class="sxs-lookup"><span data-stu-id="aacc5-315">After you have created a transfer request which includes an existing subscription, you should avoid updating the license quantity of the subscription (or associated addons).</span></span> <span data-ttu-id="aacc5-316">Bunu yaparsanız, yeni miktar aktarım isteğine yansıtılmayacaktır.</span><span class="sxs-lookup"><span data-stu-id="aacc5-316">If you do so, the new quantity will not be reflected in the transfer request.</span></span> <span data-ttu-id="aacc5-317">Dolaylı sağlayıcı aktarım isteğini kabul ettikten sonra, sonuçta elde edilen abonelik eski miktara sahip olur.</span><span class="sxs-lookup"><span data-stu-id="aacc5-317">After the indirect provider accepts the transfer request, the resultant subscription will have the old quantity.</span></span> <span data-ttu-id="aacc5-318">Yeni miktarın dolaylı sağlayıcıya aktarılmasını istiyorsanız, var olan aktarım isteğini iptal etmeniz ve yeni bir tane oluşturmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-318">If you wish for the new quantity to be transferred to the indirect provider, you must cancel the existing transfer request and recreate a new one.</span></span>

- <span data-ttu-id="aacc5-319">**Satın alma işlemleri, kendi kendine sunulan abonelik aktarımı kullanılarak aktarılamaz.**</span><span class="sxs-lookup"><span data-stu-id="aacc5-319">**Not all purchases can be transferred using self-served subscription transfer.**</span></span> <span data-ttu-id="aacc5-320">Şu anda, bu özelliği kullanarak yalnızca O365 aboneliklerini ve Azure PAYG aboneliklerini (MS-AZR-0145P) aktarabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="aacc5-320">Currently, you can only transfer O365 subscriptions and Azure PAYG subscriptions (MS-AZR-0145P) using this feature.</span></span> <span data-ttu-id="aacc5-321">Azure planları, Azure ayrılmış örnekleri, terim tabanlı abonelikler ve Azure Marketi için SaaS abonelikleri dahil diğer satın alma işlemleri desteklenmez.</span><span class="sxs-lookup"><span data-stu-id="aacc5-321">Other purchases including Azure Plans, Azure Reserved Instances, Term-based Subscriptions and SaaS subscriptions for Azure Marketplace are not supported.</span></span> <span data-ttu-id="aacc5-322">Aktarım isteği Gönder sayfasında aboneliğin neden aktarılamadığına ilişkin bir neden göreceksiniz.</span><span class="sxs-lookup"><span data-stu-id="aacc5-322">You will see a reason why a subscription cannot be transferred in the submit transfer request page.</span></span> <span data-ttu-id="aacc5-323">Bu abonelikleri aktarmak için, [mevcut aboneliği iptal](create-a-new-subscription.md#suspend-or-cancel-a-subscription) etmeniz ve dolaylı sağlayıcı aracılığıyla müşteri için yeni teklif satın almanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-323">To transfer these subscriptions, you will need to [cancel the existing subscription](create-a-new-subscription.md#suspend-or-cancel-a-subscription) and purchase new offer for customer through Indirect Provider.</span></span>

- <span data-ttu-id="aacc5-324">**Korumalı alan ortamı kullanılarak test edilemez.**</span><span class="sxs-lookup"><span data-stu-id="aacc5-324">**Cannot be tested using sandbox environment.**</span></span>

## <a name="enroll-for-indirect-reseller-incentives"></a><span data-ttu-id="aacc5-325">Dolaylı satıcı teşvikleri kaydolun</span><span class="sxs-lookup"><span data-stu-id="aacc5-325">Enroll for indirect reseller incentives</span></span>

<span data-ttu-id="aacc5-326">Mevcut doğrudan fatura ortağı kiracınızda dolaylı bir satıcı olarak başarıyla kaydolduktan sonra, 30 gün içinde dolaylı satıcı teşvik etmek için kaydolma daveti alacaksınız.</span><span class="sxs-lookup"><span data-stu-id="aacc5-326">After you have successfully enrolled as an indirect reseller on your existing direct bill partner tenant, you will receive an invitation to enroll for indirect reseller incentive within 30 days.</span></span> <span data-ttu-id="aacc5-327">Davet, CSP iş ortağı kiracınızla ilişkilendirilmiş olan iş ortağı MPN hesabına dayalıdır.</span><span class="sxs-lookup"><span data-stu-id="aacc5-327">The invitation is based on the partner MPN account that is currently associated with your CSP partner tenant.</span></span> <span data-ttu-id="aacc5-328">Davet, iş ortağı MPN hesabıyla ilişkili e-posta adresine gönderilir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-328">The invitation will be sent to the email address associated with the partner MPN account.</span></span>

<span data-ttu-id="aacc5-329">Ayrıca, aynı iş ortağı kiracısıyla doğrudan fatura teşvik programlarına kaydolma yetkiniz vardır.</span><span class="sxs-lookup"><span data-stu-id="aacc5-329">You are also eligible to enroll for direct bill incentive programs with that same partner tenant.</span></span> <span data-ttu-id="aacc5-330">Programları ayrı ayrı yönetmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="aacc5-330">You must manage the programs separately.</span></span>

## <a name="next-steps"></a><span data-ttu-id="aacc5-331">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="aacc5-331">Next steps</span></span>

- [<span data-ttu-id="aacc5-332">Dolaylı satıcı olma hakkında ek bilgiler</span><span class="sxs-lookup"><span data-stu-id="aacc5-332">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)
- [<span data-ttu-id="aacc5-333">CSP doğrudan iş ortağı yeni gereksinimler</span><span class="sxs-lookup"><span data-stu-id="aacc5-333">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)
- [<span data-ttu-id="aacc5-334">Kısıtlanmış doğrudan fatura özellikleri</span><span class="sxs-lookup"><span data-stu-id="aacc5-334">Restricted direct bill capabilities</span></span>](restricted-direct-bill-capabilities.md)
