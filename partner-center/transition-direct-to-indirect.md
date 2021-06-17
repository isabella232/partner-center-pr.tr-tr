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
ms.openlocfilehash: e57c4a5d0a02079e887b38fa9754d276062d20cc
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276425"
---
# <a name="transition-from-cloud-solution-provider-csp-direct-bill-partner-to-csp-indirect-reseller"></a><span data-ttu-id="cabb8-103">Bulut Çözümü Sağlayıcısı (CSP) doğrudan faturalanan iş ortağından CSP dolaylı kurumsal bayiye geçiş</span><span class="sxs-lookup"><span data-stu-id="cabb8-103">Transition from Cloud Solution Provider (CSP) direct bill partner to CSP indirect reseller</span></span>

<span data-ttu-id="cabb8-104">**Uygun roller**: genel yönetici</span><span class="sxs-lookup"><span data-stu-id="cabb8-104">**Appropriate roles**: Global admin</span></span>

>[!Note]
><span data-ttu-id="cabb8-105">Bu makale, dolaylı satıcılara geçişe karar veren doğrudan fatura ortakları için tasarlanmıştır.</span><span class="sxs-lookup"><span data-stu-id="cabb8-105">This article is intended for direct bill partners who have decided to transition to indirect resellers.</span></span> <span data-ttu-id="cabb8-106">Ancak dolaylı bir satıcı olarak kaydolmak üzere açık bir karar vermemiş olsanız bile, doğrudan [Fatura özellikleri kısıtlandıktan](restricted-direct-bill-capabilities.md)sonra CSP doğrudan fatura ortağı programı için yeni [gereksinimleri](direct-partner-new-requirements.md) karşılamayan doğrudan fatura iş ortakları Microsoft tarafından bilgilendirilir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-106">However, even if you have not made an explicit decision yet to enroll as an indirect reseller, direct bill partners who do not meet the new [requirements](direct-partner-new-requirements.md) for the CSP direct bill partner program will be informed by Microsoft when their [direct bill capabilities will be restricted](restricted-direct-bill-capabilities.md).</span></span>
<br><span data-ttu-id="cabb8-107">2021 Ocak itibariyle yeni bir gelir gereksinimi eklenecektir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-107">As of January 2021, a new revenue requirement will be added.</span></span> <span data-ttu-id="cabb8-108">Doğrudan bir fatura ortağı olarak kaydedilen iş ortaklarının, önceki 12 aya göre ortak küresel hesap düzeyinde bulut çözümü sağlayıcısı program gelirinde en az ABD Doları $300K ' a kadar işlem yapması gerekir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-108">Partners enrolled as a direct bill partner will need to have transacted at least USD$300K in Cloud Solution Provider program revenue at a Partner Global Account level over the previous 12 months.</span></span>

<span data-ttu-id="cabb8-109">Mevcut doğrudan fatura kiracınızı kullanarak dolaylı satıcı programına kayıt yapabileceksiniz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-109">You will be able to enroll in the indirect reseller program using your existing direct bill tenant.</span></span>

## <a name="get-started"></a><span data-ttu-id="cabb8-110">başlarken</span><span class="sxs-lookup"><span data-stu-id="cabb8-110">Get started</span></span>

1. <span data-ttu-id="cabb8-111">Iş ortağı merkezi ve MPN KIMLIĞI 'ndeki iş ortağı profilinizin güncel olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="cabb8-111">Make sure your partner profile in Partner Center and MPN ID are current.</span></span>

2. <span data-ttu-id="cabb8-112">Dolaylı satıcıya geçiş yaptığınız doğrudan fatura kiracının genel yöneticisi olarak Iş Ortağı Merkezi ' nde oturum açın.</span><span class="sxs-lookup"><span data-stu-id="cabb8-112">Sign in to Partner Center as the global admin for the direct bill tenant you are transitioning to indirect reseller.</span></span>

   :::image type="content" source="images/direct/direct1.png" alt-text="Bakýþ.":::

3. <span data-ttu-id="cabb8-114">Kayıt formunda iş ortağı ayrıntılarınızı gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="cabb8-114">Review your partner details on the enrollment form.</span></span>

   :::image type="content" source="images/direct/direct2a.png" alt-text="Şimdi kaydolun.":::

4. <span data-ttu-id="cabb8-116">Şimdi Kaydet ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="cabb8-116">Select Enroll now.</span></span> <span data-ttu-id="cabb8-117">Dolaylı Bayi işiniz, doğrudan işletmeniz için kullandığınız AAD kiracısının aynısını kullanacaktır.</span><span class="sxs-lookup"><span data-stu-id="cabb8-117">Your indirect reseller business will use the same AAD tenant you use for your direct business.</span></span>

    > [!NOTE]
    > <span data-ttu-id="cabb8-118">Başlangıçta bu yeni geçiş özelliği, Aralık ayında Tarih/yıl olan iş ortakları tarafından kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-118">Initially, this new transition capability will be available for partners with September to December anniversary dates.</span></span> <span data-ttu-id="cabb8-119">Eylül ve Aralık arasında bir yıldönümü tarihi yoksa, bu özelliği şu anda görmezsiniz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-119">If you don"t have an anniversary date between September and December, you won't see the capability at this time.</span></span> <span data-ttu-id="cabb8-120">Aralık 2018 ' den sonra yıldönümü tarihleri olan iş ortakları, özellik iş ortakları için etkinleştirildikten sonra bilgilendirilir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-120">Partners with anniversary dates after December 2018 will be notified later once the feature is enabled for the partners.</span></span>

5. <span data-ttu-id="cabb8-121">Kaydınız onaylandığında Iş Ortağı Merkezi ' nde tekrar oturum açın.</span><span class="sxs-lookup"><span data-stu-id="cabb8-121">When your enrollment is approved, sign in to Partner Center again.</span></span>

    > [!NOTE]
    > <span data-ttu-id="cabb8-122">Onay genellikle anında, en fazla beş iş günü sürebilir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-122">While approval is usually immediate, it can take up to five business days.</span></span> <span data-ttu-id="cabb8-123">Onaylandığında, kayıt formunda birincil iletişim altında belirttiğiniz e-posta adresine bir bildirim alırsınız.</span><span class="sxs-lookup"><span data-stu-id="cabb8-123">Once approved, you will receive a notification to the email address you have specified under primary contact in the enrollment form.</span></span> <span data-ttu-id="cabb8-124">Kayıt durumunuzu **Ayarlar**  >  **Hesap ayarları**  >  **iş ortağı profili** > program bilgileri altında da denetleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-124">You can also check your enrollment status under **Settings** > **Account Settings** > **Partner Profile** > Program info.</span></span>

6. <span data-ttu-id="cabb8-125">**Genel bakış** sayfanızda, dolaylı satıcı sözleşmesini görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-125">On your **Overview** page, you will see the indirect reseller agreement.</span></span> <span data-ttu-id="cabb8-126">**Kabul et ve devam et '** i seçin.</span><span class="sxs-lookup"><span data-stu-id="cabb8-126">Select **Accept and continue**.</span></span> <span data-ttu-id="cabb8-127">Bu eylem, dolaylı satıcı yeteneklerini sunar.</span><span class="sxs-lookup"><span data-stu-id="cabb8-127">This action enables the indirect reseller capabilities.</span></span>

<span data-ttu-id="cabb8-128">Dolaylı satıcı sözleşmesini kabul ettiğinizde, Iş ortağı profilinizin sizi hem doğrudan fatura hem **de** dolaylı satıcı olarak tanımladığına dikkat edin.</span><span class="sxs-lookup"><span data-stu-id="cabb8-128">When you have accepted the indirect reseller agreement, notice that your Partner profile identifies you as **both** a direct bill and indirect reseller.</span></span>

:::image type="content" source="images/direct/direct3.png" alt-text="Dolaylı satıcı sözleşmesi.":::

> [!IMPORTANT]
> <span data-ttu-id="cabb8-130">Yeni yeteneği kullanarak dolaylı bir satıcı olarak kaydolduktan sonra doğrudan bir yalnızca fatura kiracıya geri dönme seçeneği yoktur.</span><span class="sxs-lookup"><span data-stu-id="cabb8-130">Once you enroll as an indirect reseller using the new capability, there is no option to roll back to a direct bill- only tenant.</span></span> <span data-ttu-id="cabb8-131">Lütfen dolaylı bir satıcı olarak kaydolmadan önce iş gereksinimlerinizi tam olarak değerlendirdiğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="cabb8-131">Please make sure that you fully evaluate your business needs before enrolling as an indirect reseller.</span></span>

## <a name="while-you-transition-from-direct-to-indirect-reseller"></a><span data-ttu-id="cabb8-132">Doğrudan dolaylı satıcıya geçiş yaparken</span><span class="sxs-lookup"><span data-stu-id="cabb8-132">While you transition from direct to indirect reseller</span></span>

<span data-ttu-id="cabb8-133">Bu aşamada, faturalandırma süreci dahil olmak üzere doğrudan müşterilerinizin abonelik ihtiyaçlarını yönetmeye devam edersiniz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-133">During this phase, you will continue to manage your direct customers' subscription needs including the billing process.</span></span> <span data-ttu-id="cabb8-134">Ayrıca, dolaylı sağlayıcıınızdan müşterileri kabul etmeye ve dolaylı bir satıcı olarak çalışmaya başlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-134">You can also begin accepting customers from your Indirect provider and operating as an indirect reseller.</span></span>

:::image type="content" source="images/direct/direct4.png" alt-text="Hem doğrudan faturanız hem de dolaylı satıcı olursunuz.":::

## <a name="find-an-indirect-provider"></a><span data-ttu-id="cabb8-136">Dolaylı sağlayıcı bulma</span><span class="sxs-lookup"><span data-stu-id="cabb8-136">Find an indirect provider</span></span>

<span data-ttu-id="cabb8-137">Kaydolduktan sonra, sol gezinti ortamınızda dolaylı sağlayıcılara bir bağlantı görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-137">After enrolling, a link to Indirect providers will appear in your left nav.</span></span> <span data-ttu-id="cabb8-138">Dolaylı bir satıcı olarak, bir dolaylı sağlayıcıyla bir ilişki kurarsınız ve bu da faturanızı, müşterileriniz için satın alma ürünlerinizi ve destek altyapısını işleyebilir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-138">As an indirect reseller you will establish a relationship with an indirect provider who then can handle your billing, purchase products for your customers, and support infrastructure.</span></span>

<span data-ttu-id="cabb8-139">Farklı dolaylı sağlayıcılar farklı destek ve hizmetler sunmaktadır. bu nedenle, gereksinimlerinizi en iyi şekilde karşılayan Hizmetleri öğrenmek için bölgenizdeki sağlayıcıları değerlendirmelisiniz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-139">Different indirect providers offer different support and services, so you should evaluate the providers in your area to determine which ones best meet your needs.</span></span> <span data-ttu-id="cabb8-140">Genellikle, çoğu sağlayıcı şunları olur:</span><span class="sxs-lookup"><span data-stu-id="cabb8-140">Generally, most providers will:</span></span>

- <span data-ttu-id="cabb8-141">Size teknik eğitim ve yardım sağlama</span><span class="sxs-lookup"><span data-stu-id="cabb8-141">Provide you with technical training and assistance</span></span>
- <span data-ttu-id="cabb8-142">Ürün ve hizmetlerinizi pazarlamanıza yardımcı olun</span><span class="sxs-lookup"><span data-stu-id="cabb8-142">Help you market your products and services</span></span>
- <span data-ttu-id="cabb8-143">Finans ve kredi koşullarınızı yönetin</span><span class="sxs-lookup"><span data-stu-id="cabb8-143">Manage your financing and credit terms</span></span>

<span data-ttu-id="cabb8-144">Resmi [Microsoft dolaylı sağlayıcıları](https://partnercenter.microsoft.com/partner/find-a-provider)listesinde arama yapın.</span><span class="sxs-lookup"><span data-stu-id="cabb8-144">Search the list of official [Microsoft indirect providers](https://partnercenter.microsoft.com/partner/find-a-provider).</span></span>

<span data-ttu-id="cabb8-145">Daha fazla bilgi edinin, [dolaylı sağlayıcılarla Iş ortağı](indirect-reseller-tasks-in-partner-center.md) okuyun</span><span class="sxs-lookup"><span data-stu-id="cabb8-145">Learn more, read  [Partner with indirect providers](indirect-reseller-tasks-in-partner-center.md)</span></span>

## <a name="accept-a-partnership-invitation-from-your-indirect-provider"></a><span data-ttu-id="cabb8-146">Dolaylı sağlayıcınızdan bir ortaklık daveti kabul edin</span><span class="sxs-lookup"><span data-stu-id="cabb8-146">Accept a partnership invitation from your indirect provider</span></span>

<span data-ttu-id="cabb8-147">İş ortağına dolaylı bir sağlayıcı bulduğunuzda, Iş Ortağı Merkezi 'nde dolaylı sağlayıcıyla bir ortaklık kurun.</span><span class="sxs-lookup"><span data-stu-id="cabb8-147">When you find an indirect provider to partner with, establish a partnership with the indirect provider in Partner Center.</span></span>

<span data-ttu-id="cabb8-148">Seçtiğiniz dolaylı sağlayıcı sizi Iş ortağı merkezindeki davetine götürebileceğiniz bir ortaklık daveti e-postası adresine gönderir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-148">The indirect provider you select will send you in email a partnership invitation link that will take you to their invitation in Partner Center.</span></span> <span data-ttu-id="cabb8-149">Genel yöneticinizin Iş Ortağı Merkezi 'nde oturum açtığından ve davet bağlantısını izlediğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="cabb8-149">Be sure your global admin signs in to Partner Center and follows the invitation link.</span></span> <span data-ttu-id="cabb8-150">Daveti kabul ettiğinizde, sağlayıcının adı dolaylı sağlayıcı listenizde görünür.</span><span class="sxs-lookup"><span data-stu-id="cabb8-150">When you accept the invitation, the provider's name will appear in your indirect provider list.</span></span>

## <a name="acquire-new-customers-as-indirect-reseller"></a><span data-ttu-id="cabb8-151">Yeni müşterileri dolaylı satıcı olarak edinin</span><span class="sxs-lookup"><span data-stu-id="cabb8-151">Acquire new customers as indirect reseller</span></span>

<span data-ttu-id="cabb8-152">Hem siz hem de dolaylı sağlayıcınız müşterilerle satıcı ilişkilerine sahip olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="cabb8-152">Both you and your indirect provider need to have reseller relationships with customers.</span></span> <span data-ttu-id="cabb8-153">Bu satıcı ilişkileri, müşterinin aboneliklerini ve hizmetlerini kendi adına yönetmenize olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="cabb8-153">These reseller relationships enable you to manage a customer's subscriptions and services on their behalf.</span></span> <span data-ttu-id="cabb8-154">Mevcut bir Azure AD kiracısına sahip yeni bir müşteri edinmek için, müşteriyi hem sizinle hem de sağlayıcınızda aynı anda bir satıcı ilişkisi kurmaya davet edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-154">To acquire a new customer who has an existing Azure AD tenant, you can invite the customer to establish a reseller relationship with both you and your provider at the same time.</span></span>

<span data-ttu-id="cabb8-155">Dolaylı bir satıcı daveti oluşturmak için:</span><span class="sxs-lookup"><span data-stu-id="cabb8-155">To create an indirect reseller invitation:</span></span>

1. <span data-ttu-id="cabb8-156">Iş ortağı merkezi sol gezininizden **dolaylı sağlayıcılar** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="cabb8-156">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="cabb8-157">Aynı anda hem sizin hem de dolaylı sağlayıcı ile satıcı ilişkisi kurmak üzere bir müşteriyi davet etmek için **yeni müşterileri davet et** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="cabb8-157">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="cabb8-158">Sağlayıcının müşteri ile bir satıcı ilişkisi olması gerekir, bu nedenle müşteri yeni abonelikler satın almak istediğinde veya mevcut aboneliklerde yeni lisanslar eklemek istediğinde müşterinin adına sipariş gönderebilirler.</span><span class="sxs-lookup"><span data-stu-id="cabb8-158">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

3. <span data-ttu-id="cabb8-159">Sonraki sayfada taslak e-posta iletisini gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="cabb8-159">On the next page, review the draft email message.</span></span> <span data-ttu-id="cabb8-160">Taslak iletisini e-postada açabilir veya iletiyi panonuza kopyalayabilir ve bir e-postaya yapıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-160">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="cabb8-161">E-postadaki metni düzenleyerek, ihtiyacınız olanları söyleyin, ancak müşteriyi doğrudan hesabınıza ve sağlayıcınızın hesabınıza bağlamak için kişiselleştirildiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="cabb8-161">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="cabb8-162">Ardından **Bitti**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="cabb8-162">Then select **Done**.</span></span>

5. <span data-ttu-id="cabb8-163">Müşteri sizi ve sağlayıcınızı kendi kayıt satıcıları olarak doğruladıktan sonra, kendi adına aboneliklerini, lisanslarını ve kullanıcılarını yönetmek için yönetici izinlerine sahip olacaksınız ve dolaylı sağlayıcınız kendi adına sipariş gönderebilecektir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-163">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>
6. <span data-ttu-id="cabb8-164">Müşterinin hesabını, hizmetlerini, kullanıcılarını ve lisanslarını yönetmek için, adının yanındaki aşağı oku seçerek müşterinin kaydını genişletin.</span><span class="sxs-lookup"><span data-stu-id="cabb8-164">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

<span data-ttu-id="cabb8-165">Doğrudan fatura iş ortaklarının aksine, dolaylı satıcılar Iş Ortağı Merkezi 'nde yeni müşterileri için Azure AD kiracılar oluşturamaz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-165">Unlike direct bill partners, indirect resellers can't create Azure AD tenants for their new customers in Partner Center.</span></span> <span data-ttu-id="cabb8-166">Sağlayıcınız kiracıyı oluşturacak ve size bu müşterinin dolaylı satıcısı olarak belirtmeyecektir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-166">Your provider will create the tenant and will specify you as the indirect reseller for this customer.</span></span> <span data-ttu-id="cabb8-167">Bu, müşterinin Iş Ortağı Merkezi 'nde müşteri listenizde görünmesini sağlar.</span><span class="sxs-lookup"><span data-stu-id="cabb8-167">This ensures that the customer will appear in your customer list in Partner Center.</span></span>

>[!Note]
><span data-ttu-id="cabb8-168">Dolaylı satıcı olarak aldığınız müşteriler için satın alma işlemleri oluşturmak üzere doğrudan fatura özelliğini kullanamazsınız.</span><span class="sxs-lookup"><span data-stu-id="cabb8-168">You will not be able to use your direct bill capability to create purchases for customers you acquire as an indirect reseller.</span></span>

## <a name="managing-your-direct-bill-customers-and-your-indirect-reseller-customers"></a><span data-ttu-id="cabb8-169">Doğrudan Bill müşterilerini ve dolaylı satıcı müşterilerinizi yönetme</span><span class="sxs-lookup"><span data-stu-id="cabb8-169">Managing your direct bill customers and your indirect reseller customers</span></span>

<span data-ttu-id="cabb8-170">Doğrudan fatura müşterilerinizi ve dolaylı satıcı müşterilerinizi farklı şekilde yönetirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-170">You manage your direct bill customers and your indirect reseller customers differently.</span></span>

### <a name="direct-bill-customers-things-you-wont-do-as-an-indirect-reseller"></a><span data-ttu-id="cabb8-171">Doğrudan fatura müşterileri (dolaylı satıcı olarak yapamayabilmeniz gerekir)</span><span class="sxs-lookup"><span data-stu-id="cabb8-171">Direct bill customers (things you won't do as an indirect reseller)</span></span>

- <span data-ttu-id="cabb8-172">Ürünler için sipariş oluşturma</span><span class="sxs-lookup"><span data-stu-id="cabb8-172">Create orders for products</span></span>
- <span data-ttu-id="cabb8-173">Azure ayırmalarını yönetme</span><span class="sxs-lookup"><span data-stu-id="cabb8-173">Manage Azure reservations</span></span>
- <span data-ttu-id="cabb8-174">Sıra geçmişini yönetme</span><span class="sxs-lookup"><span data-stu-id="cabb8-174">Manage their order history</span></span>
- <span data-ttu-id="cabb8-175">Satın alma yazılımı</span><span class="sxs-lookup"><span data-stu-id="cabb8-175">Purchase software</span></span>
- <span data-ttu-id="cabb8-176">Doğrudan fatura müşterileri</span><span class="sxs-lookup"><span data-stu-id="cabb8-176">Bill customers directly</span></span>

### <a name="indirect-reseller-customers"></a><span data-ttu-id="cabb8-177">Dolaylı satıcı müşterileri</span><span class="sxs-lookup"><span data-stu-id="cabb8-177">Indirect reseller customers</span></span>

- <span data-ttu-id="cabb8-178">Dolaylı sağlayıcınız, müşterileriniz için ürünleri sipariş eden</span><span class="sxs-lookup"><span data-stu-id="cabb8-178">Your indirect provider orders products for your customers</span></span>
- <span data-ttu-id="cabb8-179">Müşterilerin lisanslarını ve kullanıcılarını yönetme</span><span class="sxs-lookup"><span data-stu-id="cabb8-179">Manage customers' licenses and users</span></span>
- <span data-ttu-id="cabb8-180">Abonelik yenilemeler işleme</span><span class="sxs-lookup"><span data-stu-id="cabb8-180">Handle subscription renewals</span></span>

### <a name="to-identify-customers-that-you-acquired-as-a-direct-bill-partner"></a><span data-ttu-id="cabb8-181">Doğrudan bir fatura ortağı olarak edindiğiniz müşterileri belirlemek için</span><span class="sxs-lookup"><span data-stu-id="cabb8-181">To identify customers that you acquired as a direct bill partner</span></span>

1. <span data-ttu-id="cabb8-182">**Müşteriler**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="cabb8-182">Select **Customers**.</span></span>

2. <span data-ttu-id="cabb8-183">Ayrıntılarını görüntülemek için bir müşteri seçin.</span><span class="sxs-lookup"><span data-stu-id="cabb8-183">Select a customer to view their details.</span></span>

3. <span data-ttu-id="cabb8-184">Bu müşteri doğrudan fatura ortağı olarak elde ediyorsanız, ürün **ekleme** veya **görüntüleme** seçeneklerini görürsünüz ve aboneliklerini görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-184">If this customer is one you acquired as a direct bill partner, you will see options to **add** or **view products** and you will see their subscriptions.</span></span>

4. <span data-ttu-id="cabb8-185">Müşterinin sizinle dolaylı bir satıcı ilişkisi varsa, bu seçenekler kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-185">If the customer has an indirect reseller relationship with you, those options will not be available.</span></span>

## <a name="move-your-direct-bill-customers-to-your-indirect-provider"></a><span data-ttu-id="cabb8-186">Doğrudan fatura müşterilerinizi dolaylı sağlayıcınıza taşıyın</span><span class="sxs-lookup"><span data-stu-id="cabb8-186">Move your direct bill customers to your indirect provider</span></span>

<span data-ttu-id="cabb8-187">Dolaylı sağlayıcınız, mevcut doğrudan fatura müşterileriniz için bir satıcı ilişkisine sahip olana kadar sipariş veya mevcut abonelik aktarımları gönderemez.</span><span class="sxs-lookup"><span data-stu-id="cabb8-187">Your indirect provider cannot submit orders or existing subscription transfers for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="cabb8-188">Dolaylı sağlayıcınız ile var olan doğrudan faturanız arasındaki satıcı ilişkilerini oluşturmak için aşağıdaki yöntemlerden birini kullanabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="cabb8-188">To establish the reseller relationship between your indirect provider and your existing direct bill customer, you can use one of the following methods:</span></span>

- [<span data-ttu-id="cabb8-189">Satıcı ilişki uzantısı</span><span class="sxs-lookup"><span data-stu-id="cabb8-189">Reseller relationship extension</span></span>](#reseller-relationship-extension)

- [<span data-ttu-id="cabb8-190">Müşteriye dolaylı bir satıcı davetiyesi gönderin</span><span class="sxs-lookup"><span data-stu-id="cabb8-190">Send an indirect reseller invitation to the customer</span></span>](#send-an-indirect-reseller-invitation-to-the-customer)

<span data-ttu-id="cabb8-191">[Doğrudan dolaylı geçiş belgesinde](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/) adım adım işleme yönelik ayrıntılı bir genel bakış bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-191">You can find a detailed overview of the step-by-step process in the [Direct to indirect transition document](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span></span>

### <a name="reseller-relationship-extension"></a><span data-ttu-id="cabb8-192">Satıcı ilişki uzantısı</span><span class="sxs-lookup"><span data-stu-id="cabb8-192">Reseller relationship extension</span></span>

<span data-ttu-id="cabb8-193">Kurumsal ilişki uzantısı özelliğini kullanarak, mevcut doğrudan fatura müşterileriniz ve dolaylı sağlayıcınız arasında Iş Ortağı Merkezi panosunu kullanarak satıcı ilişkisi kurabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-193">You can use the reseller relationship extension feature to establish reseller relationship between your existing direct bill customers and your indirect provider using Partner Center Dashboard.</span></span> <span data-ttu-id="cabb8-194">Özelliği kullanmadan önce, aşağıdakilere göz önüne alın:</span><span class="sxs-lookup"><span data-stu-id="cabb8-194">Before using the feature, note the following:</span></span>

- <span data-ttu-id="cabb8-195">Bu özellik yalnızca dolaylı satıcı olan dolaylı satıcı [kaydını](#get-started)tamamlamış olan doğrudan fatura ortakları tarafından kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-195">This feature is only available to direct bill partners who are transitioning to become an indirect reseller have completed the [indirect reseller enrollment](#get-started).</span></span>

- <span data-ttu-id="cabb8-196">Bu özelliği yalnızca var olan doğrudan fatura müşterilerine uygulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-196">You can only apply this feature to existing direct bill customers.</span></span> <span data-ttu-id="cabb8-197">Bu, [dolaylı satıcı müşterileri](#acquire-new-customers-as-indirect-reseller)için geçerli değildir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-197">It is not applicable to [indirect reseller customers](#acquire-new-customers-as-indirect-reseller).</span></span>

- <span data-ttu-id="cabb8-198">Yalnızca [dolaylı sağlayıcıınızdan bir iş ortağı davetini kabul](#accept-a-partnership-invitation-from-your-indirect-provider)ettiğiniz bir dolaylı sağlayıcıyı seçebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-198">You can only select an indirect provider for which you have [accepted a partner invitation from your indirect provider](#accept-a-partnership-invitation-from-your-indirect-provider).</span></span>

- <span data-ttu-id="cabb8-199">Bu müşteri için sahip olduğunuz fatura-bilgi bilgilerinin bir kopyası dolaylı sağlayıcı tarafından kullanılabilir hale getirilir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-199">A copy of the bill-to info you have for this customer will be made available to the indirect provider.</span></span> <span data-ttu-id="cabb8-200">Iş Ortağı Merkezi panosunda bu müşterinin hesap sayfasına erişerek fatura bilgilerine erişebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-200">You can access the bill-to info by accessing the Account page for this customer in Partner Center Dashboard.</span></span>

    > [!NOTE]
    > <span data-ttu-id="cabb8-201">Kurumsal bayi ilişkisi uzantısı özelliğini kullanarak, bu müşteri için sahip olduğunuz fatura bilgilerini dolaylı sağlayıcıyla paylaşmayı kabul edersiniz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-201">By using the reseller relationship extension feature, you consent to sharing the bill-to info you have for this customer with the indirect provider.</span></span>

- <span data-ttu-id="cabb8-202">Dolaylı sağlayıcınıza müşteri kiracısına [yönetici temsilcisi ayrıcalıkları](customers-revoke-admin-privileges.md) sağlanmaz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-202">Your indirect provider will not be provided with [delegated administration privileges](customers-revoke-admin-privileges.md) to the customer tenant.</span></span> <span data-ttu-id="cabb8-203">Dolaylı sağlayıcınız için temsilcili yönetim ayrıcalıklarına ihtiyaç varsa, bunun yerine müşteriye dolaylı kurumsal bayi daveti göndermeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-203">If your indirect provider requires delegated administration privileges, you must send an indirect reseller invitation to the customer instead.</span></span>

- <span data-ttu-id="cabb8-204">Kurumsal bayi ilişkisi kurulduktan sonra dolaylı sağlayıcı, Microsoft 365 Yönetim Merkezi'nde İş Ortağı İlişkileri sayfasında müşteriye CSP iş [ortağı](https://admin.microsoft.com/AdminPortal/Home#/partners) [İş İçin Microsoft Store.](/microsoft-store/work-with-partner-microsoft-store-business)</span><span class="sxs-lookup"><span data-stu-id="cabb8-204">Once the reseller relationship is established, the indirect provider will appear as a CSP partner to the customer under the Partner Relationships page in [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/partners) and [Microsoft Store for Business](/microsoft-store/work-with-partner-microsoft-store-business).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="cabb8-205">Karışıklığı ve yanlış anlamayı önlemek için, mevcut bir doğrudan fatura müşterisi ile dolaylı sağlayıcı arasında kurumsal bayi ilişkisi kurmak üzere ilişki uzantısı özelliğini kullanmadan önce doğrudan fatura müşterisini bilgilendirmek ve ondan onay almak için iş ortağı sözleşmenize bağlı olarak zorunludur.</span><span class="sxs-lookup"><span data-stu-id="cabb8-205">To avoid confusion and misunderstanding, you are contractually obliged by your partner agreement to inform and obtain consent from the direct bill customer before you use the relationship extension feature to establish reseller relationship between an existing direct bill customer and an indirect provider.</span></span>

<span data-ttu-id="cabb8-206">Bu özelliği mevcut bir müşteri kiracısı üzerinde kullanmak için:</span><span class="sxs-lookup"><span data-stu-id="cabb8-206">To use this feature on an existing customer tenant:</span></span>

1. <span data-ttu-id="cabb8-207">İş Ortağı Merkezi Yönetici Aracısı olarak **oturum açma.**</span><span class="sxs-lookup"><span data-stu-id="cabb8-207">Log in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="cabb8-208">Müşteriler **sayfasında var olan** bir müşteriyi seçin ve Hızlı bağlantılar **simgesine** tıklar ve müşterinin özet görünümünü genişletin.</span><span class="sxs-lookup"><span data-stu-id="cabb8-208">In the **Customers page**, select an existing customer and click on its **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="cabb8-209">Dolaylı **sağlayıcılar altında Dolaylı sağlayıcıda** **müşteriyi aktar'a tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="cabb8-209">Under **Indirect provider(s)**, click **Transfer customer on an indirect provider**.</span></span>

    :::image type="content" source="images/direct/direct5-1.png" alt-text="Müşteriyi dolaylı sağlayıcıya aktarma.":::

4. <span data-ttu-id="cabb8-211">Açılan iletişim kutusunda müşteriyle kurumsal **bayi ilişkisine** sahip olmak istediğiniz Dolaylı Sağlayıcıyı seçin.</span><span class="sxs-lookup"><span data-stu-id="cabb8-211">In the pop-up dialog, select the **Indirect Provider** you would like to have reseller relationship with the customer.</span></span>

5. <span data-ttu-id="cabb8-212">Kaydet ve **devam'a tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="cabb8-212">Click **Save and continue**.</span></span>

6. <span data-ttu-id="cabb8-213">Seçilen dolaylı sağlayıcının Dolaylı sağlayıcılar **altında olduğunu doğrulayın.**</span><span class="sxs-lookup"><span data-stu-id="cabb8-213">Verify the selected indirect provider shows up under **Indirect provider(s)**.</span></span>

    :::image type="content" source="images/direct/direct5-2.png" alt-text="Dolaylı Sağlayıcı listelenir.":::

### <a name="send-an-indirect-reseller-invitation-to-the-customer"></a><span data-ttu-id="cabb8-215">Müşteriye dolaylı kurumsal bayi daveti gönderme</span><span class="sxs-lookup"><span data-stu-id="cabb8-215">Send an indirect reseller invitation to the customer</span></span>

<span data-ttu-id="cabb8-216">Dolaylı sağlayıcınız, mevcut doğrudan fatura müşterilerinizle bir kurumsal bayi ilişkisine sahip olana kadar sipariş gönderemiyor.</span><span class="sxs-lookup"><span data-stu-id="cabb8-216">Your indirect provider cannot submit orders for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="cabb8-217">Mevcut müşterilerinizle dolaylı sağlayıcınız arasındaki kurumsal bayi ilişkisini kurmak için dolaylı kurumsal bayi davetini kullanarak müşteriyi davet edin.</span><span class="sxs-lookup"><span data-stu-id="cabb8-217">To establish the reseller relationship between your existing customers and your indirect provider, invite the customer using an indirect reseller invitation.</span></span>

1. <span data-ttu-id="cabb8-218">Sol **gezinti gezinti çubuğundan** Dolaylı İş Ortağı Merkezi'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="cabb8-218">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="cabb8-219">Yeni **müşterileri davet et'i** seçerek bir müşteriyi hem sizin hem de dolaylı sağlayıcıyla aynı anda kurumsal bayi ilişkisi kurması için davet edin.</span><span class="sxs-lookup"><span data-stu-id="cabb8-219">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="cabb8-220">Müşteri yeni abonelikler satın almak veya mevcut aboneliklere yeni lisanslar eklemek isterse müşterinin adına sipariş gönderesin diye sağlayıcının müşteriyle kurumsal bayi ilişkisi olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-220">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

    :::image type="content" source="images/direct/direct6.png" alt-text="Yeni müşteriler davet etme.":::

3. <span data-ttu-id="cabb8-222">Sonraki sayfada taslak e-posta iletisini gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="cabb8-222">On the next page, review the draft email message.</span></span> <span data-ttu-id="cabb8-223">Taslak iletiyi e-postayla açabilir veya panoya kopyalayıp bir e-postaya yapıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-223">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="cabb8-224">E-postada yer alan metni düzenleyemezsiniz ancak bağlantıyı dahil edin çünkü müşteriyi doğrudan hem hesabınıza hem de sağlayıcınızın hesabına bağlamaya yönelik kişiselleştirilmiş bir bağlantıdır.</span><span class="sxs-lookup"><span data-stu-id="cabb8-224">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="cabb8-225">Ardından **Bitti**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="cabb8-225">Then select **Done**.</span></span>

5. <span data-ttu-id="cabb8-226">Müşteri sizi ve sağlayıcınızı kendi kayıt kurumsal bayileri olarak yetkilendikten sonra aboneliklerini, lisanslarını ve kullanıcılarını kendi adına yönetmek için yönetici izinlerine sahip olursunuz ve dolaylı sağlayıcınız kendi adına siparişler gönderebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-226">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>

6. <span data-ttu-id="cabb8-227">Müşterinin hesabını, hizmetlerini, kullanıcılarını ve lisanslarını yönetmek için, adının yanındaki aşağı oku seçerek müşterinin kaydını genişletin.</span><span class="sxs-lookup"><span data-stu-id="cabb8-227">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

### <a name="microsoft-customer-agreement-acceptance"></a><span data-ttu-id="cabb8-228">Microsoft Müşteri Sözleşmesi kabul etme</span><span class="sxs-lookup"><span data-stu-id="cabb8-228">Microsoft Customer Agreement acceptance</span></span>

<span data-ttu-id="cabb8-229">Microsoft Bulut Anlaşması 31 Ocak 2020'ye kadar geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-229">Microsoft Cloud Agreement is valid until January 31, 2020.</span></span> <span data-ttu-id="cabb8-230">Bu tarihten sonra var olan ve yeni olan tüm müşterilerin yeni [Microsoft Müşteri Sözleşmesi.](confirm-customer-agreement.md)</span><span class="sxs-lookup"><span data-stu-id="cabb8-230">After that date, all customers, existing and new, must sign the new [Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span> <span data-ttu-id="cabb8-231">Geçiş müşterileri için:</span><span class="sxs-lookup"><span data-stu-id="cabb8-231">For transitioning customers, if:</span></span>

- <span data-ttu-id="cabb8-232">**Müşteri henüz kabul Microsoft Müşteri Sözleşmesi**</span><span class="sxs-lookup"><span data-stu-id="cabb8-232">**Customer has not accepted Microsoft Customer Agreement yet**</span></span>

   <span data-ttu-id="cabb8-233">Müşterinin Microsoft Müşteri Sözleşmesi'i kabul etmelerini [sağlamak için dolaylı sağlayıcıyla Microsoft Müşteri Sözleşmesi.](confirm-customer-agreement.md)</span><span class="sxs-lookup"><span data-stu-id="cabb8-233">Please work with Indirect Provider to have customer [accept the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

- <span data-ttu-id="cabb8-234">**Müşteri, Microsoft Müşteri Sözleşmesi Yönetim Merkezi aracılığıyla Microsoft 365 kabul etti**</span><span class="sxs-lookup"><span data-stu-id="cabb8-234">**Customer has accepted Microsoft Customer Agreement with you through the Microsoft 365 Admin Center**</span></span>

   <span data-ttu-id="cabb8-235">Dolaylı Sağlayıcı ile kurumsal bayi ilişkisi kurulduktan sonra kabul korunur.</span><span class="sxs-lookup"><span data-stu-id="cabb8-235">The acceptance will be retained once the reseller relationship is established with the Indirect Provider.</span></span> <span data-ttu-id="cabb8-236">Hiçbir şey yapmak zorunda değildir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-236">There is nothing you need to do.</span></span>

- <span data-ttu-id="cabb8-237">**Müşteri, iş Microsoft Müşteri Sözleşmesi ile birlikte kabul etti**</span><span class="sxs-lookup"><span data-stu-id="cabb8-237">**Customer has accepted Microsoft Customer Agreement with you through partner attestation**</span></span>

   <span data-ttu-id="cabb8-238">Kabul tutmaz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-238">The acceptance will not be retained.</span></span> <span data-ttu-id="cabb8-239">Müşteri kabulünü güncelleştirmek için [lütfen Dolaylı Sağlayıcı ile birlikte İş Ortağı Merkezi.](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers)</span><span class="sxs-lookup"><span data-stu-id="cabb8-239">Please work with Indirect Provider to [update the customer's acceptance in Partner Center](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span></span>

## <a name="transfer-existing-direct-bill-subscriptions-to-indirect-provider"></a><span data-ttu-id="cabb8-240">Mevcut doğrudan fatura aboneliklerini dolaylı sağlayıcıya aktarma</span><span class="sxs-lookup"><span data-stu-id="cabb8-240">Transfer existing direct bill subscriptions to indirect provider</span></span>

<span data-ttu-id="cabb8-241">CSP dolaylı modelinde dolaylı kurumsal bayilerin Microsoft ile faturalama ilişkileri olmaz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-241">Under CSP indirect model, indirect resellers do not have billing relationships with Microsoft.</span></span> <span data-ttu-id="cabb8-242">Bunun yerine dolaylı kurumsal bayiler, dolaylı sağlayıcıları aracılığıyla müşterileri için abonelikler alır.</span><span class="sxs-lookup"><span data-stu-id="cabb8-242">Instead, indirect resellers obtain subscriptions for their customers through their indirect providers.</span></span> <span data-ttu-id="cabb8-243">Doğrudan fatura iş ortağından dolaylı kurumsal bayiye geçiş yaparken, doğrudan fatura iş ortağı olarak sahip olduğunuz mevcut abonelikleri dolaylı sağlayıcınıza aktarmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-243">While transitioning from direct bill partner to indirect reseller, you need to transfer the existing subscriptions you have as the direct bill partner to your indirect provider.</span></span> <span data-ttu-id="cabb8-244">Bunu yapmak için İş Ortağı Merkezi Panosu'İş Ortağı Merkezi abonelik aktarımı özelliğini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-244">You can use the self-served subscription transfer feature in Partner Center Dashboard to do so.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="cabb8-245">Önkoşullar</span><span class="sxs-lookup"><span data-stu-id="cabb8-245">Prerequisites</span></span>

- <span data-ttu-id="cabb8-246">Bu özellik yalnızca mevcut doğrudan fatura iş ortağı kiracılarını kullanarak dolaylı kurumsal bayi kaydı tamamlayan iş ortaklarına geçiş için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-246">This feature is only available to transitioning partners who have completed the indirect reseller enrollment using their existing direct bill partner tenants.</span></span>

- <span data-ttu-id="cabb8-247">Belirli bir müşteriyle ilişkili abonelikleri aktarmadan önce, geçiş ortağının müşteriyi dolaylı sağlayıcıya taşıması gerekir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-247">Before transferring subscriptions associated with a given customer, the transitioning partner must move the customer to an indirect provider.</span></span>

- <span data-ttu-id="cabb8-248">Müşterinin Dolaylı Sağlayıcı [aracılığıyla Microsoft Müşteri Sözleşmesi kabul etmiş olması gerekir.](#microsoft-customer-agreement-acceptance)</span><span class="sxs-lookup"><span data-stu-id="cabb8-248">Customer must have [accepted Microsoft Customer Agreement through the Indirect Provider](#microsoft-customer-agreement-acceptance).</span></span>

### <a name="how-to-transition-to-indirect-reseller-status"></a><span data-ttu-id="cabb8-249">Dolaylı kurumsal bayi durumuna geçiş</span><span class="sxs-lookup"><span data-stu-id="cabb8-249">How to transition to indirect reseller status</span></span>

<span data-ttu-id="cabb8-250">Özellik 4 adımlı bir işlemdir; burada:</span><span class="sxs-lookup"><span data-stu-id="cabb8-250">The feature is a 4-step process, where:</span></span>

- <span data-ttu-id="cabb8-251">Geçiş iş ortağı bir abonelik aktarım isteği oluşturur.</span><span class="sxs-lookup"><span data-stu-id="cabb8-251">The transitioning partner creates a subscription transfer request.</span></span> <span data-ttu-id="cabb8-252">İstek, aynı müşteriyle ilişkili bir veya daha fazla mevcut abonelik içerir ve dolaylı sağlayıcıya giderildi.</span><span class="sxs-lookup"><span data-stu-id="cabb8-252">The request contains one or more existing subscriptions associated with the same customer and is addressed to an indirect provider.</span></span>

- <span data-ttu-id="cabb8-253">Dolaylı sağlayıcı aktarım isteğini gözden kullanır ve kabul eder (veya reddeder).</span><span class="sxs-lookup"><span data-stu-id="cabb8-253">The indirect provider reviews and accepts (or reject) the transfer request.</span></span>

- <span data-ttu-id="cabb8-254">Dolaylı sağlayıcı, aktarım isteğinin tamam olduğunu doğrular.</span><span class="sxs-lookup"><span data-stu-id="cabb8-254">The indirect provider verifies that the transfer request is complete.</span></span>

- <span data-ttu-id="cabb8-255">Geçiş ortağı, aktarım isteğinin tamamlandıktan sonra doğrular.</span><span class="sxs-lookup"><span data-stu-id="cabb8-255">The transitioning partner verifies that the transfer request is complete.</span></span>

### <a name="transitioning-partner"></a><span data-ttu-id="cabb8-256">İş ortağını geçişe</span><span class="sxs-lookup"><span data-stu-id="cabb8-256">Transitioning partner</span></span>

> [!NOTE]
> <span data-ttu-id="cabb8-257">Mevcut abonelikleri dolaylı [İş Ortağı Merkezi api/SDK'sı](/partner-center/develop/manage-customers) olarak da kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-257">You can also use [Partner Center API/SDK](/partner-center/develop/manage-customers) to transfer the existing subscriptions to your indirect provider.</span></span>
>
> - [<span data-ttu-id="cabb8-258">Müşterinin abonelik aktarım uygunluğunu alma</span><span class="sxs-lookup"><span data-stu-id="cabb8-258">Get a customer's subscriptions transfer eligibility</span></span>](/partner-center/develop/get-customer-s-subscriptions-transfer-eligibility)
> - [<span data-ttu-id="cabb8-259">Müşterinin aktarımını oluşturma</span><span class="sxs-lookup"><span data-stu-id="cabb8-259">Create a customer's transfer</span></span>](/partner-center/develop/create-a-transfer)
> - [<span data-ttu-id="cabb8-260">Müşterinin aktarımını geri alma</span><span class="sxs-lookup"><span data-stu-id="cabb8-260">Withdraw a customer's transfer</span></span>](/partner-center/develop/withdraw-a-transfer)
> - [<span data-ttu-id="cabb8-261">Müşterinin aktarımını kabul etme</span><span class="sxs-lookup"><span data-stu-id="cabb8-261">Accept a customer's transfer</span></span>](/partner-center/develop/accept-a-transfer)
> - [<span data-ttu-id="cabb8-262">Müşterinin aktarımını reddetme</span><span class="sxs-lookup"><span data-stu-id="cabb8-262">Reject a Customer's transfer</span></span>](/partner-center/develop/reject-a-transfer)
> - [<span data-ttu-id="cabb8-263">Müşterinin aktarımlarını alma</span><span class="sxs-lookup"><span data-stu-id="cabb8-263">Get a customer's transfers</span></span>](/partner-center/develop/get-all-of-a-customer-s-transfers)
> - [<span data-ttu-id="cabb8-264">Kimlikle aktarım ayrıntılarını al</span><span class="sxs-lookup"><span data-stu-id="cabb8-264">Get transfer details by id</span></span>](/partner-center/develop/get-transfer-by-id)

### <a name="transitioning-partner---create-transfer-request"></a><span data-ttu-id="cabb8-265">Geçiş iş ortağı - aktarım isteği oluşturma</span><span class="sxs-lookup"><span data-stu-id="cabb8-265">Transitioning partner - create transfer request</span></span>

<span data-ttu-id="cabb8-266">Geçiş iş ortağı olarak bir aktarım isteği oluşturmak için:</span><span class="sxs-lookup"><span data-stu-id="cabb8-266">To create a transfer request as the transitioning partner:</span></span>

1. <span data-ttu-id="cabb8-267">İş Ortağı Merkezi Yönetici Aracısı olarak **oturum açma.**</span><span class="sxs-lookup"><span data-stu-id="cabb8-267">Log in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="cabb8-268">Müşteriler **sayfasında,** hedeflenen müşteriyi seçin ve Hızlı bağlantılar simgesine tıklar ve müşterinin özet görünümünü genişletin.</span><span class="sxs-lookup"><span data-stu-id="cabb8-268">In the **Customers** page, select the intended customer and click on the Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="cabb8-269">Dolaylı **sağlayıcılar altında,** hedeflenen dolaylı sağlayıcının listelenmiş olduğunu onaylayın.</span><span class="sxs-lookup"><span data-stu-id="cabb8-269">Under **Indirect provider(s)**, confirm that the intended indirect provider is listed.</span></span>

4. <span data-ttu-id="cabb8-270">Abonelikleri **Görüntüle'ye tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="cabb8-270">Click **View Subscriptions**.</span></span>

5. <span data-ttu-id="cabb8-271">Abonelikler **sayfasında** Abonelik **Aktarımı'nın bulun.**</span><span class="sxs-lookup"><span data-stu-id="cabb8-271">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

6. <span data-ttu-id="cabb8-272">Abonelik **Aktarımı'nın altında** Abonelik **aktarımı isteği'ne tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="cabb8-272">Under **Subscription Transfer**, click **Request subscription transfer**.</span></span>

    :::image type="content" source="images/direct/direct8.png" alt-text="Abonelik aktarımı isteği.":::

7. <span data-ttu-id="cabb8-274">Aktarım isteği iletişim kutusunda, aktar kullanmak istediğiniz bir veya daha fazla aboneliği seçin.</span><span class="sxs-lookup"><span data-stu-id="cabb8-274">In the transfer request dialog, select one or more subscriptions to be transferred.</span></span>

    :::image type="content" source="images/direct/direct9.png" alt-text="Aktarım İsteği oluşturma.":::

8. <span data-ttu-id="cabb8-276">**Oluştur**’a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="cabb8-276">Click **Create**.</span></span>

9. <span data-ttu-id="cabb8-277">Etkin bir abonelik aktarım isteği Abonelik Aktarımı **altında görünür.**</span><span class="sxs-lookup"><span data-stu-id="cabb8-277">An active subscription transfer request will appear under **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct10.png" alt-text="Aktarım isteği listesi.":::

10. <span data-ttu-id="cabb8-279">Dolaylı sağlayıcınıza, onlara bir abonelik aktarım isteği oluşturduğunuz konusunda bilgi edin.</span><span class="sxs-lookup"><span data-stu-id="cabb8-279">Inform your indirect provider that you have created a subscription transfer request to them.</span></span>

### <a name="indirect-provider---accept-transfer-request"></a><span data-ttu-id="cabb8-280">Dolaylı sağlayıcı - aktarım isteğini kabul etme</span><span class="sxs-lookup"><span data-stu-id="cabb8-280">Indirect provider - accept transfer request</span></span>

<span data-ttu-id="cabb8-281">Dolaylı sağlayıcı olarak bir aktarım isteğini gözden geçirmek ve kabul etmek için:</span><span class="sxs-lookup"><span data-stu-id="cabb8-281">To review and accept a transfer request as the indirect provider:</span></span>

1. <span data-ttu-id="cabb8-282">İş Ortağı Merkezi Aracısı veya **Satış Aracısı** olarak **oturum açma.**</span><span class="sxs-lookup"><span data-stu-id="cabb8-282">Log in to Partner Center as an **Admin** Agent or **Sales Agent**.</span></span>

2. <span data-ttu-id="cabb8-283">Müşteriler **sayfasında,** hedeflenen müşteriyi seçin ve Hızlı bağlantılar simgesine tıklar ve müşterinin özet görünümünü genişletin.</span><span class="sxs-lookup"><span data-stu-id="cabb8-283">In the **Customers** page, select the intended customer and click on its Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="cabb8-284">Dolaylı **kurumsal bayiler altında,** geçiş iş ortağının listelenmiş olduğunu onaylayın.</span><span class="sxs-lookup"><span data-stu-id="cabb8-284">Under **Indirect reseller(s)**, confirm the transitioning partner is listed.</span></span>

4. <span data-ttu-id="cabb8-285">Abonelikleri **Görüntüle'ye tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="cabb8-285">Click **View Subscriptions**.</span></span>

5. <span data-ttu-id="cabb8-286">Abonelikler **sayfasında** Abonelik **Aktarımı'nın bulun.**</span><span class="sxs-lookup"><span data-stu-id="cabb8-286">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct11.png" alt-text="Aktarım isteğini görüntüleme.":::

6. <span data-ttu-id="cabb8-288">Abonelik **Aktarımı altında,** gözden geçirmek istediğiniz aktarım isteğine tıklayın.</span><span class="sxs-lookup"><span data-stu-id="cabb8-288">Under **Subscription Transfer**, click on the transfer request to review.</span></span>

7. <span data-ttu-id="cabb8-289">Uygun **şekilde Kabul** Et **(veya Reddet)** seçeneğini tıklayın.</span><span class="sxs-lookup"><span data-stu-id="cabb8-289">Click **Accept** (or **Reject**) as appropriate.</span></span>

    :::image type="content" source="images/direct/direct12.png" alt-text="Aktarım isteğini kabul etme.":::

8. <span data-ttu-id="cabb8-291">Aktarım isteğinin tamamlandıktan sonra tamamlanır.</span><span class="sxs-lookup"><span data-stu-id="cabb8-291">Wait for the transfer request to complete.</span></span>

### <a name="indirect-provider---verify-transfer-request-is-complete"></a><span data-ttu-id="cabb8-292">Dolaylı sağlayıcı - aktarım isteğinin tamamlandıktan emin olun</span><span class="sxs-lookup"><span data-stu-id="cabb8-292">Indirect provider - verify transfer request is complete</span></span>

1. <span data-ttu-id="cabb8-293">Aktarım isteği başarıyla tamamlandıktan sonra aboneliklerin Abonelikler altında görüntü olduğunu **doğrulayın.**</span><span class="sxs-lookup"><span data-stu-id="cabb8-293">After the transfer request is completed successfully, verify that you can see the subscriptions appear under **Subscriptions**.</span></span>

2. <span data-ttu-id="cabb8-294">Geçiş iş ortağını bilgilendirin.</span><span class="sxs-lookup"><span data-stu-id="cabb8-294">Inform the transitioning partner.</span></span>

### <a name="transitioning-partner---verify-transfer-request-is-complete"></a><span data-ttu-id="cabb8-295">İş ortağı geçişi - aktarım isteğinin tamamlandıktan emin olun</span><span class="sxs-lookup"><span data-stu-id="cabb8-295">Transitioning partner - verify transfer request is complete</span></span>

<span data-ttu-id="cabb8-296">Geçiş ortağı aşağıdaki adımları gerçekleştirerek şunları gerçekleştirin:</span><span class="sxs-lookup"><span data-stu-id="cabb8-296">The transitioning partner should do the following:</span></span>

1. <span data-ttu-id="cabb8-297">Yönetici Aracısı İş Ortağı Merkezi Satış **Aracısı olarak oturum** **açma.**</span><span class="sxs-lookup"><span data-stu-id="cabb8-297">Sign into Partner Center as an **Admin Agent** or **Sales Agent**.</span></span>

2. <span data-ttu-id="cabb8-298">Müşteriler **sayfasında,** hedeflenen müşteriyi seçin ve Hızlı bağlantılar **simgesine** tıklar ve müşterinin özet görünümünü genişletin.</span><span class="sxs-lookup"><span data-stu-id="cabb8-298">In the **Customers** page, select the intended customer and click on the **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="cabb8-299">Abonelikleri **Görüntüle'ye tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="cabb8-299">Click **View Subscriptions**.</span></span>

4. <span data-ttu-id="cabb8-300">Abonelikler **sayfasında** Abonelik **Aktarımı'nın bulun.**</span><span class="sxs-lookup"><span data-stu-id="cabb8-300">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

5. <span data-ttu-id="cabb8-301">Aktarım isteğinin **Tamam** olarak işaretlendiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="cabb8-301">Verify that the transfer request is marked as **Complete**.</span></span>

6. <span data-ttu-id="cabb8-302">Aboneliğin artık **abonelikler** sayfasında etkin olarak görünmediğini doğrulayın:</span><span class="sxs-lookup"><span data-stu-id="cabb8-302">Verify that the subscription(s) no longer appear as active in the **Subscriptions** page:</span></span>

   1. <span data-ttu-id="cabb8-303">Bu bir Azure aboneliğse (MS-AZR-0145P), artık listelenmez.</span><span class="sxs-lookup"><span data-stu-id="cabb8-303">If this is an Azure subscription (MS-AZR-0145P), it will no longer be listed.</span></span>

   2. <span data-ttu-id="cabb8-304">Bu bir lisans tabanlı aboneliğiniz (Office 365, Dynamics, Intune), durumu **askıya alındı** olarak listelenir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-304">If this is a license-based subscription (Office 365, Dynamics, Intune), it will be listed with state as **Suspended**.</span></span>

   :::image type="content" source="images/direct/direct13.png" alt-text="Abonelik askıya alındı.":::

### <a name="considerations"></a><span data-ttu-id="cabb8-306">Dikkat edilmesi gerekenler</span><span class="sxs-lookup"><span data-stu-id="cabb8-306">Considerations</span></span>

- <span data-ttu-id="cabb8-307">**Abonelik KIMLIĞI aktarımdan sonra farklı olacaktır.**</span><span class="sxs-lookup"><span data-stu-id="cabb8-307">**Subscription ID will be different after transfer.**</span></span> <span data-ttu-id="cabb8-308">Bu bir Azure aboneliğiyiyse (MS-AZR-0145P), buna ek olarak, önceki sahibinden tutulan ve Azure yönetim portalında görünecek bir Azure abonelik KIMLIĞI olur.</span><span class="sxs-lookup"><span data-stu-id="cabb8-308">If it is an Azure subscription (MS-AZR-0145P), additionally, it will have an Azure Subscription ID, which is retained from the previous owner, and will appear in the Azure management portal.</span></span>

- <span data-ttu-id="cabb8-309">**Aynı aboneliğe birden çok aktarım isteği tarafından başvurulamaz.**</span><span class="sxs-lookup"><span data-stu-id="cabb8-309">**The same subscription cannot be referenced by multiple transfer requests.**</span></span> <span data-ttu-id="cabb8-310">Mevcut bir aboneliği içeren bir aktarım isteği oluşturduktan sonra, ilk aktarım isteği iptal edilene kadar aynı abonelik dahil olmak üzere ek aktarım istekleri oluşturamazsınız.</span><span class="sxs-lookup"><span data-stu-id="cabb8-310">After you have created a transfer request, which includes an existing subscription, you cannot create additional transfer requests including the same subscription, until the first transfer request is canceled.</span></span>

- <span data-ttu-id="cabb8-311">**Lisans tabanlı abonelikler için eklentiler, temel abonelikleriyle birlikte aktarılmalıdır.**</span><span class="sxs-lookup"><span data-stu-id="cabb8-311">**Add-ons for license-based subscriptions must be transferred along with their base subscription.**</span></span> <span data-ttu-id="cabb8-312">Bir aktarım isteği oluştururken, bir veya daha fazla eklentiye sahip mevcut bir aboneliği seçerseniz, eklenti otomatik olarak aktarım isteğine dahil edilir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-312">When creating a transfer request, if you pick an existing subscription with one or more add-ons, the add-ons will automatically be included in the transfer request.</span></span>

- <span data-ttu-id="cabb8-313">**Bir abonelikte lisans sayısı değişiklikleri var olan aktarım isteğine yansıtılmayacaktır.**</span><span class="sxs-lookup"><span data-stu-id="cabb8-313">**License count changes to a subscription will not be reflected in existing transfer request.**</span></span> <span data-ttu-id="cabb8-314">Var olan bir aboneliği içeren bir aktarım isteği oluşturduktan sonra, aboneliğin lisans miktarını (veya ilişkili eklentiler) güncelleştirmeden kaçınmalısınız.</span><span class="sxs-lookup"><span data-stu-id="cabb8-314">After you have created a transfer request which includes an existing subscription, you should avoid updating the license quantity of the subscription (or associated addons).</span></span> <span data-ttu-id="cabb8-315">Bunu yaparsanız, yeni miktar aktarım isteğine yansıtılmayacaktır.</span><span class="sxs-lookup"><span data-stu-id="cabb8-315">If you do so, the new quantity will not be reflected in the transfer request.</span></span> <span data-ttu-id="cabb8-316">Dolaylı sağlayıcı aktarım isteğini kabul ettikten sonra, sonuçta elde edilen abonelik eski miktara sahip olur.</span><span class="sxs-lookup"><span data-stu-id="cabb8-316">After the indirect provider accepts the transfer request, the resultant subscription will have the old quantity.</span></span> <span data-ttu-id="cabb8-317">Yeni miktarın dolaylı sağlayıcıya aktarılmasını istiyorsanız, var olan aktarım isteğini iptal etmeniz ve yeni bir tane oluşturmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-317">If you wish for the new quantity to be transferred to the indirect provider, you must cancel the existing transfer request and recreate a new one.</span></span>

- <span data-ttu-id="cabb8-318">**Satın alma işlemleri, kendi kendine sunulan abonelik aktarımı kullanılarak aktarılamaz.**</span><span class="sxs-lookup"><span data-stu-id="cabb8-318">**Not all purchases can be transferred using self-served subscription transfer.**</span></span> <span data-ttu-id="cabb8-319">Şu anda, bu özelliği kullanarak yalnızca O365 aboneliklerini ve Azure PAYG aboneliklerini (MS-AZR-0145P) aktarabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-319">Currently, you can only transfer O365 subscriptions and Azure PAYG subscriptions (MS-AZR-0145P) using this feature.</span></span> <span data-ttu-id="cabb8-320">Azure planları, Azure ayrılmış örnekleri, terim tabanlı abonelikler ve Azure Marketi için SaaS abonelikleri dahil diğer satın alma işlemleri desteklenmez.</span><span class="sxs-lookup"><span data-stu-id="cabb8-320">Other purchases including Azure Plans, Azure Reserved Instances, Term-based Subscriptions and SaaS subscriptions for Azure Marketplace are not supported.</span></span> <span data-ttu-id="cabb8-321">Aktarım isteği Gönder sayfasında aboneliğin neden aktarılamadığına ilişkin bir neden göreceksiniz.</span><span class="sxs-lookup"><span data-stu-id="cabb8-321">You will see a reason why a subscription cannot be transferred in the submit transfer request page.</span></span> <span data-ttu-id="cabb8-322">Bu abonelikleri aktarmak için, [mevcut aboneliği iptal](create-a-new-subscription.md#suspend-or-cancel-a-subscription) etmeniz ve dolaylı sağlayıcı aracılığıyla müşteri için yeni teklif satın almanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-322">To transfer these subscriptions, you will need to [cancel the existing subscription](create-a-new-subscription.md#suspend-or-cancel-a-subscription) and purchase new offer for customer through Indirect Provider.</span></span>

- <span data-ttu-id="cabb8-323">**Korumalı alan ortamı kullanılarak test edilemez.**</span><span class="sxs-lookup"><span data-stu-id="cabb8-323">**Cannot be tested using sandbox environment.**</span></span>

## <a name="enroll-for-indirect-reseller-incentives"></a><span data-ttu-id="cabb8-324">Dolaylı satıcı teşvikleri kaydolun</span><span class="sxs-lookup"><span data-stu-id="cabb8-324">Enroll for indirect reseller incentives</span></span>

<span data-ttu-id="cabb8-325">Mevcut doğrudan fatura ortağı kiracınızda dolaylı bir satıcı olarak başarıyla kaydolduktan sonra, 30 gün içinde dolaylı satıcı teşvik etmek için kaydolma daveti alacaksınız.</span><span class="sxs-lookup"><span data-stu-id="cabb8-325">After you have successfully enrolled as an indirect reseller on your existing direct bill partner tenant, you will receive an invitation to enroll for indirect reseller incentive within 30 days.</span></span> <span data-ttu-id="cabb8-326">Davet, CSP iş ortağı kiracınızla ilişkilendirilmiş olan iş ortağı MPN hesabına dayalıdır.</span><span class="sxs-lookup"><span data-stu-id="cabb8-326">The invitation is based on the partner MPN account that is currently associated with your CSP partner tenant.</span></span> <span data-ttu-id="cabb8-327">Davet, iş ortağı MPN hesabıyla ilişkili e-posta adresine gönderilir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-327">The invitation will be sent to the email address associated with the partner MPN account.</span></span>

<span data-ttu-id="cabb8-328">Ayrıca, aynı iş ortağı kiracısıyla doğrudan fatura teşvik programlarına kaydolma yetkiniz vardır.</span><span class="sxs-lookup"><span data-stu-id="cabb8-328">You are also eligible to enroll for direct bill incentive programs with that same partner tenant.</span></span> <span data-ttu-id="cabb8-329">Programları ayrı ayrı yönetmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="cabb8-329">You must manage the programs separately.</span></span>

## <a name="next-steps"></a><span data-ttu-id="cabb8-330">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="cabb8-330">Next steps</span></span>

- [<span data-ttu-id="cabb8-331">Dolaylı satıcı olma hakkında ek bilgiler</span><span class="sxs-lookup"><span data-stu-id="cabb8-331">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)
- [<span data-ttu-id="cabb8-332">CSP doğrudan iş ortağı yeni gereksinimler</span><span class="sxs-lookup"><span data-stu-id="cabb8-332">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)
- [<span data-ttu-id="cabb8-333">Kısıtlanmış doğrudan fatura özellikleri</span><span class="sxs-lookup"><span data-stu-id="cabb8-333">Restricted direct bill capabilities</span></span>](restricted-direct-bill-capabilities.md)
