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
ms.openlocfilehash: e3cd791f5f9f781980d73c79f0ec18627585372a
ms.sourcegitcommit: b4771fd0781d95551e65baa481a572291c729d7d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/28/2020
ms.locfileid: "92795874"
---
# <a name="transition-from-cloud-solution-provider-csp-direct-bill-partner-to-csp-indirect-reseller"></a><span data-ttu-id="6db8f-103">Bulut Çözümü Sağlayıcısı (CSP) doğrudan faturalanan iş ortağından CSP dolaylı kurumsal bayiye geçiş</span><span class="sxs-lookup"><span data-stu-id="6db8f-103">Transition from Cloud Solution Provider (CSP) direct bill partner to CSP indirect reseller</span></span>

<span data-ttu-id="6db8f-104">**Aşağıdakiler cihazlar için geçerlidir:**</span><span class="sxs-lookup"><span data-stu-id="6db8f-104">**Applies to:**</span></span>
- <span data-ttu-id="6db8f-105">İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="6db8f-105">Partner Center</span></span>

<span data-ttu-id="6db8f-106">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="6db8f-106">**Appropriate roles**</span></span>

- <span data-ttu-id="6db8f-107">Tüm CSP doğrudan fatura ortakları</span><span class="sxs-lookup"><span data-stu-id="6db8f-107">All CSP direct bill partners</span></span>

>[!Note]
><span data-ttu-id="6db8f-108">Bu makale, dolaylı satıcılara geçişe karar veren doğrudan fatura ortakları için tasarlanmıştır.</span><span class="sxs-lookup"><span data-stu-id="6db8f-108">This article is intended for direct bill partners who have decided to transition to indirect resellers.</span></span> <span data-ttu-id="6db8f-109">Ancak dolaylı bir satıcı olarak kaydolmak üzere açık bir karar vermemiş olsanız bile, doğrudan [Fatura özellikleri kısıtlandıktan](restricted-direct-bill-capabilities.md)sonra CSP doğrudan fatura ortağı programı için yeni [gereksinimleri](direct-partner-new-requirements.md) karşılamayan doğrudan fatura iş ortakları Microsoft tarafından bilgilendirilir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-109">However, even if you have not made an explicit decision yet to enroll as an indirect reseller, direct bill partners who do not meet the new [requirements](direct-partner-new-requirements.md) for the CSP direct bill partner program will be informed by Microsoft when their [direct bill capabilities will be restricted](restricted-direct-bill-capabilities.md).</span></span>
<br><span data-ttu-id="6db8f-110">2021 Ocak itibariyle yeni bir gelir gereksinimi eklenecektir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-110">As of January 2021, a new revenue requirement will be added.</span></span> <span data-ttu-id="6db8f-111">Doğrudan bir fatura ortağı olarak kaydedilen iş ortaklarının, önceki 12 aya göre ortak küresel hesap düzeyinde bulut çözümü sağlayıcısı program gelirinde en az ABD Doları $300K ' a kadar işlem yapması gerekir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-111">Partners enrolled as a direct bill partner will need to have transacted at least USD$300K in Cloud Solution Provider program revenue at a Partner Global Account level over the previous 12 months.</span></span>

<span data-ttu-id="6db8f-112">Mevcut doğrudan fatura kiracınızı kullanarak dolaylı satıcı programına kayıt yapabileceksiniz.</span><span class="sxs-lookup"><span data-stu-id="6db8f-112">You will be able to enroll in the indirect reseller program using your existing direct bill tenant.</span></span>

## <a name="get-started"></a><span data-ttu-id="6db8f-113">başlarken</span><span class="sxs-lookup"><span data-stu-id="6db8f-113">Get started</span></span>

1. <span data-ttu-id="6db8f-114">Iş ortağı merkezi ve MPN KIMLIĞI 'ndeki iş ortağı profilinizin güncel olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="6db8f-114">Make sure your partner profile in Partner Center and MPN ID are current.</span></span>

2. <span data-ttu-id="6db8f-115">Dolaylı satıcıya geçiş yaptığınız doğrudan fatura kiracının genel yöneticisi olarak Iş Ortağı Merkezi ' nde oturum açın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-115">Sign in to Partner Center as the global admin for the direct bill tenant you are transitioning to indirect reseller.</span></span>

   :::image type="content" source="images/direct/direct1.png" alt-text="Genel Bakış":::

3. <span data-ttu-id="6db8f-117">Kayıt formunda iş ortağı ayrıntılarınızı gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="6db8f-117">Review your partner details on the enrollment form.</span></span>

   :::image type="content" source="images/direct/direct2a.png" alt-text="Hemen kaydolun":::

4. <span data-ttu-id="6db8f-119">Şimdi Kaydet ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="6db8f-119">Select Enroll now.</span></span> <span data-ttu-id="6db8f-120">Dolaylı Bayi işiniz, doğrudan işletmeniz için kullandığınız AAD kiracısının aynısını kullanacaktır.</span><span class="sxs-lookup"><span data-stu-id="6db8f-120">Your indirect reseller business will use the same AAD tenant you use for your direct business.</span></span>

    > [!NOTE]
    > <span data-ttu-id="6db8f-121">Başlangıçta bu yeni geçiş özelliği, Aralık ayında Tarih/yıl olan iş ortakları tarafından kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-121">Initially, this new transition capability will be available for partners with September to December anniversary dates.</span></span> <span data-ttu-id="6db8f-122">Eylül ve Aralık arasında bir yıldönümü tarihi yoksa, bu özelliği şu anda görmezsiniz.</span><span class="sxs-lookup"><span data-stu-id="6db8f-122">If you don"t have an anniversary date between September and December, you won't see the capability at this time.</span></span> <span data-ttu-id="6db8f-123">Aralık 2018 ' den sonra yıldönümü tarihleri olan iş ortakları, özellik iş ortakları için etkinleştirildikten sonra bilgilendirilir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-123">Partners with anniversary dates after December 2018 will be notified later once the feature is enabled for the partners.</span></span>

5. <span data-ttu-id="6db8f-124">Kaydınız onaylandığında Iş Ortağı Merkezi ' nde tekrar oturum açın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-124">When your enrollment is approved, sign in to Partner Center again.</span></span>

    > [!NOTE]
    > <span data-ttu-id="6db8f-125">Onay genellikle anında, en fazla beş iş günü sürebilir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-125">While approval is usually immediate, it can take up to five business days.</span></span> <span data-ttu-id="6db8f-126">Onaylandığında, kayıt formunda birincil iletişim altında belirttiğiniz e-posta adresine bir bildirim alırsınız.</span><span class="sxs-lookup"><span data-stu-id="6db8f-126">Once approved, you will receive a notification to the email address you have specified under primary contact in the enrollment form.</span></span> <span data-ttu-id="6db8f-127">Kayıt durumunuzu **Ayarlar**  >  **iş ortağı ayarları**  >  **iş ortağı profili** > program bilgileri altında da denetleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6db8f-127">You can also check your enrollment status under **Settings** > **Partner Settings** > **Partner Profile** > Program info.</span></span>

6. <span data-ttu-id="6db8f-128">**Genel bakış** sayfanızda, dolaylı satıcı sözleşmesini görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="6db8f-128">On your **Overview** page, you will see the indirect reseller agreement.</span></span> <span data-ttu-id="6db8f-129">**Kabul et ve devam et '** i seçin.</span><span class="sxs-lookup"><span data-stu-id="6db8f-129">Select **Accept and continue** .</span></span> <span data-ttu-id="6db8f-130">Bu eylem, dolaylı satıcı yeteneklerini sunar.</span><span class="sxs-lookup"><span data-stu-id="6db8f-130">This action enables the indirect reseller capabilities.</span></span>

<span data-ttu-id="6db8f-131">Dolaylı satıcı sözleşmesini kabul ettiğinizde, Iş ortağı profilinizin sizi hem doğrudan fatura hem **de** dolaylı satıcı olarak tanımladığına dikkat edin.</span><span class="sxs-lookup"><span data-stu-id="6db8f-131">When you have accepted the indirect reseller agreement, notice that your Partner profile identifies you as **both** a direct bill and indirect reseller.</span></span>

:::image type="content" source="images/direct/direct3.png" alt-text="Dolaylı satıcı sözleşmesi":::

> [!IMPORTANT]
> <span data-ttu-id="6db8f-133">Yeni yeteneği kullanarak dolaylı bir satıcı olarak kaydolduktan sonra doğrudan bir yalnızca fatura kiracıya geri dönme seçeneği yoktur.</span><span class="sxs-lookup"><span data-stu-id="6db8f-133">Once you enroll as an indirect reseller using the new capability, there is no option to roll back to a direct bill- only tenant.</span></span> <span data-ttu-id="6db8f-134">Lütfen dolaylı bir satıcı olarak kaydolmadan önce iş gereksinimlerinizi tam olarak değerlendirdiğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="6db8f-134">Please make sure that you fully evaluate your business needs before enrolling as an indirect reseller.</span></span>

## <a name="while-you-transition-from-direct-to-indirect-reseller"></a><span data-ttu-id="6db8f-135">Doğrudan dolaylı satıcıya geçiş yaparken</span><span class="sxs-lookup"><span data-stu-id="6db8f-135">While you transition from direct to indirect reseller</span></span>

<span data-ttu-id="6db8f-136">Bu aşamada, faturalandırma süreci dahil olmak üzere doğrudan müşterilerinizin abonelik ihtiyaçlarını yönetmeye devam edersiniz.</span><span class="sxs-lookup"><span data-stu-id="6db8f-136">During this phase, you will continue to manage your direct customers' subscription needs including the billing process.</span></span> <span data-ttu-id="6db8f-137">Ayrıca, dolaylı sağlayıcıınızdan müşterileri kabul etmeye ve dolaylı bir satıcı olarak çalışmaya başlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6db8f-137">You can also begin accepting customers from your Indirect provider and operating as an indirect reseller.</span></span>

:::image type="content" source="images/direct/direct4.png" alt-text="Hem doğrudan faturanız hem de dolaylı satıcı":::

## <a name="find-an-indirect-provider"></a><span data-ttu-id="6db8f-139">Dolaylı sağlayıcı bulma</span><span class="sxs-lookup"><span data-stu-id="6db8f-139">Find an indirect provider</span></span>

<span data-ttu-id="6db8f-140">Kaydolduktan sonra, sol gezinti ortamınızda dolaylı sağlayıcılara bir bağlantı görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-140">After enrolling, a link to Indirect providers will appear in your left nav.</span></span> <span data-ttu-id="6db8f-141">Dolaylı bir satıcı olarak, bir dolaylı sağlayıcıyla bir ilişki kurarsınız ve bu da faturanızı, müşterileriniz için satın alma ürünlerinizi ve destek altyapısını işleyebilir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-141">As an indirect reseller you will establish a relationship with an indirect provider who then can handle your billing, purchase products for your customers, and support infrastructure.</span></span>

<span data-ttu-id="6db8f-142">Farklı dolaylı sağlayıcılar farklı destek ve hizmetler sunmaktadır. bu nedenle, gereksinimlerinizi en iyi şekilde karşılayan Hizmetleri öğrenmek için bölgenizdeki sağlayıcıları değerlendirmelisiniz.</span><span class="sxs-lookup"><span data-stu-id="6db8f-142">Different indirect providers offer different support and services, so you should evaluate the providers in your area to determine which ones best meet your needs.</span></span> <span data-ttu-id="6db8f-143">Genellikle, çoğu sağlayıcı şunları olur:</span><span class="sxs-lookup"><span data-stu-id="6db8f-143">Generally, most providers will:</span></span>

- <span data-ttu-id="6db8f-144">Size teknik eğitim ve yardım sağlama</span><span class="sxs-lookup"><span data-stu-id="6db8f-144">Provide you with technical training and assistance</span></span>
- <span data-ttu-id="6db8f-145">Ürün ve hizmetlerinizi pazarlamanıza yardımcı olun</span><span class="sxs-lookup"><span data-stu-id="6db8f-145">Help you market your products and services</span></span>
- <span data-ttu-id="6db8f-146">Finans ve kredi koşullarınızı yönetin</span><span class="sxs-lookup"><span data-stu-id="6db8f-146">Manage your financing and credit terms</span></span>

<span data-ttu-id="6db8f-147">Resmi [Microsoft dolaylı sağlayıcıları](https://partnercenter.microsoft.com/partner/find-a-provider)listesinde arama yapın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-147">Search the list of official [Microsoft indirect providers](https://partnercenter.microsoft.com/partner/find-a-provider).</span></span>

<span data-ttu-id="6db8f-148">Daha fazla bilgi edinin, [dolaylı sağlayıcılarla Iş ortağı](indirect-reseller-tasks-in-partner-center.md) okuyun</span><span class="sxs-lookup"><span data-stu-id="6db8f-148">Learn more, read  [Partner with indirect providers](indirect-reseller-tasks-in-partner-center.md)</span></span>

## <a name="accept-a-partnership-invitation-from-your-indirect-provider"></a><span data-ttu-id="6db8f-149">Dolaylı sağlayıcınızdan bir ortaklık daveti kabul edin</span><span class="sxs-lookup"><span data-stu-id="6db8f-149">Accept a partnership invitation from your indirect provider</span></span>

<span data-ttu-id="6db8f-150">İş ortağına dolaylı bir sağlayıcı bulduğunuzda, Iş Ortağı Merkezi 'nde dolaylı sağlayıcıyla bir ortaklık kurun.</span><span class="sxs-lookup"><span data-stu-id="6db8f-150">When you find an indirect provider to partner with, establish a partnership with the indirect provider in Partner Center.</span></span>

<span data-ttu-id="6db8f-151">Seçtiğiniz dolaylı sağlayıcı sizi Iş ortağı merkezindeki davetine götürebileceğiniz bir ortaklık daveti e-postası adresine gönderir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-151">The indirect provider you select will send you in email a partnership invitation link that will take you to their invitation in Partner Center.</span></span> <span data-ttu-id="6db8f-152">Genel yöneticinizin Iş Ortağı Merkezi 'nde oturum açtığından ve davet bağlantısını izlediğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="6db8f-152">Be sure your global admin signs in to Partner Center and follows the invitation link.</span></span> <span data-ttu-id="6db8f-153">Daveti kabul ettiğinizde, sağlayıcının adı dolaylı sağlayıcı listenizde görünür.</span><span class="sxs-lookup"><span data-stu-id="6db8f-153">When you accept the invitation, the provider's name will appear in your indirect provider list.</span></span>

## <a name="acquire-new-customers-as-indirect-reseller"></a><span data-ttu-id="6db8f-154">Yeni müşterileri dolaylı satıcı olarak edinin</span><span class="sxs-lookup"><span data-stu-id="6db8f-154">Acquire new customers as indirect reseller</span></span>

<span data-ttu-id="6db8f-155">Hem siz hem de dolaylı sağlayıcınız müşterilerle satıcı ilişkilerine sahip olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="6db8f-155">Both you and your indirect provider need to have reseller relationships with customers.</span></span> <span data-ttu-id="6db8f-156">Bu satıcı ilişkileri, müşterinin aboneliklerini ve hizmetlerini kendi adına yönetmenize olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="6db8f-156">These reseller relationships enable you to manage a customer's subscriptions and services on their behalf.</span></span> <span data-ttu-id="6db8f-157">Mevcut bir Azure AD kiracısına sahip yeni bir müşteri edinmek için, müşteriyi hem sizinle hem de sağlayıcınızda aynı anda bir satıcı ilişkisi kurmaya davet edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6db8f-157">To acquire a new customer who has an existing Azure AD tenant, you can invite the customer to establish a reseller relationship with both you and your provider at the same time.</span></span>

<span data-ttu-id="6db8f-158">Dolaylı bir satıcı daveti oluşturmak için:</span><span class="sxs-lookup"><span data-stu-id="6db8f-158">To create an indirect reseller invitation:</span></span>

1. <span data-ttu-id="6db8f-159">Iş ortağı merkezi sol gezininizden **dolaylı sağlayıcılar** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="6db8f-159">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="6db8f-160">Aynı anda hem sizin hem de dolaylı sağlayıcı ile satıcı ilişkisi kurmak üzere bir müşteriyi davet etmek için **yeni müşterileri davet et** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="6db8f-160">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="6db8f-161">Sağlayıcının müşteri ile bir satıcı ilişkisi olması gerekir, bu nedenle müşteri yeni abonelikler satın almak istediğinde veya mevcut aboneliklerde yeni lisanslar eklemek istediğinde müşterinin adına sipariş gönderebilirler.</span><span class="sxs-lookup"><span data-stu-id="6db8f-161">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

3. <span data-ttu-id="6db8f-162">Sonraki sayfada taslak e-posta iletisini gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="6db8f-162">On the next page, review the draft email message.</span></span> <span data-ttu-id="6db8f-163">Taslak iletisini e-postada açabilir veya iletiyi panonuza kopyalayabilir ve bir e-postaya yapıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6db8f-163">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="6db8f-164">E-postadaki metni düzenleyerek, ihtiyacınız olanları söyleyin, ancak müşteriyi doğrudan hesabınıza ve sağlayıcınızın hesabınıza bağlamak için kişiselleştirildiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="6db8f-164">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="6db8f-165">Ardından **Bitti** 'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="6db8f-165">Then select **Done** .</span></span>

5. <span data-ttu-id="6db8f-166">Müşteri sizi ve sağlayıcınızı kendi kayıt satıcıları olarak doğruladıktan sonra, kendi adına aboneliklerini, lisanslarını ve kullanıcılarını yönetmek için yönetici izinlerine sahip olacaksınız ve dolaylı sağlayıcınız kendi adına sipariş gönderebilecektir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-166">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>
6. <span data-ttu-id="6db8f-167">Müşterinin hesabını, hizmetlerini, kullanıcılarını ve lisanslarını yönetmek için, adının yanındaki aşağı oku seçerek müşterinin kaydını genişletin.</span><span class="sxs-lookup"><span data-stu-id="6db8f-167">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

<span data-ttu-id="6db8f-168">Doğrudan fatura iş ortaklarının aksine, dolaylı satıcılar Iş Ortağı Merkezi 'nde yeni müşterileri için Azure AD kiracılar oluşturamaz.</span><span class="sxs-lookup"><span data-stu-id="6db8f-168">Unlike direct bill partners, indirect resellers can't create Azure AD tenants for their new customers in Partner Center.</span></span> <span data-ttu-id="6db8f-169">Sağlayıcınız kiracıyı oluşturacak ve size bu müşterinin dolaylı satıcısı olarak belirtmeyecektir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-169">Your provider will create the tenant and will specify you as the indirect reseller for this customer.</span></span> <span data-ttu-id="6db8f-170">Bu, müşterinin Iş Ortağı Merkezi 'nde müşteri listenizde görünmesini sağlar.</span><span class="sxs-lookup"><span data-stu-id="6db8f-170">This ensures that the customer will appear in your customer list in Partner Center.</span></span>

>[!Note]
><span data-ttu-id="6db8f-171">Dolaylı satıcı olarak aldığınız müşteriler için satın alma işlemleri oluşturmak üzere doğrudan fatura özelliğini kullanamazsınız.</span><span class="sxs-lookup"><span data-stu-id="6db8f-171">You will not be able to use your direct bill capability to create purchases for customers you acquire as an indirect reseller.</span></span>

## <a name="managing-your-direct-bill-customers-and-your-indirect-reseller-customers"></a><span data-ttu-id="6db8f-172">Doğrudan Bill müşterilerini ve dolaylı satıcı müşterilerinizi yönetme</span><span class="sxs-lookup"><span data-stu-id="6db8f-172">Managing your direct bill customers and your indirect reseller customers</span></span>

<span data-ttu-id="6db8f-173">Doğrudan fatura müşterilerinizi ve dolaylı satıcı müşterilerinizi farklı şekilde yönetirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6db8f-173">You manage your direct bill customers and your indirect reseller customers differently.</span></span>

### <a name="direct-bill-customers-things-you-wont-do-as-an-indirect-reseller"></a><span data-ttu-id="6db8f-174">Doğrudan fatura müşterileri (dolaylı satıcı olarak yapamayabilmeniz gerekir)</span><span class="sxs-lookup"><span data-stu-id="6db8f-174">Direct bill customers (things you won't do as an indirect reseller)</span></span>

- <span data-ttu-id="6db8f-175">Ürünler için sipariş oluşturma</span><span class="sxs-lookup"><span data-stu-id="6db8f-175">Create orders for products</span></span>
- <span data-ttu-id="6db8f-176">Azure ayırmalarını yönetme</span><span class="sxs-lookup"><span data-stu-id="6db8f-176">Manage Azure reservations</span></span>
- <span data-ttu-id="6db8f-177">Sıra geçmişini yönetme</span><span class="sxs-lookup"><span data-stu-id="6db8f-177">Manage their order history</span></span>
- <span data-ttu-id="6db8f-178">Satın alma yazılımı</span><span class="sxs-lookup"><span data-stu-id="6db8f-178">Purchase software</span></span>
- <span data-ttu-id="6db8f-179">Doğrudan fatura müşterileri</span><span class="sxs-lookup"><span data-stu-id="6db8f-179">Bill customers directly</span></span>

### <a name="indirect-reseller-customers"></a><span data-ttu-id="6db8f-180">Dolaylı satıcı müşterileri</span><span class="sxs-lookup"><span data-stu-id="6db8f-180">Indirect reseller customers</span></span>

- <span data-ttu-id="6db8f-181">Dolaylı sağlayıcınız, müşterileriniz için ürünleri sipariş eden</span><span class="sxs-lookup"><span data-stu-id="6db8f-181">Your indirect provider orders products for your customers</span></span>
- <span data-ttu-id="6db8f-182">Müşterilerin lisanslarını ve kullanıcılarını yönetme</span><span class="sxs-lookup"><span data-stu-id="6db8f-182">Manage customers' licenses and users</span></span>
- <span data-ttu-id="6db8f-183">Abonelik yenilemeler işleme</span><span class="sxs-lookup"><span data-stu-id="6db8f-183">Handle subscription renewals</span></span>

### <a name="to-identify-customers-that-you-acquired-as-a-direct-bill-partner"></a><span data-ttu-id="6db8f-184">Doğrudan bir fatura ortağı olarak edindiğiniz müşterileri belirlemek için</span><span class="sxs-lookup"><span data-stu-id="6db8f-184">To identify customers that you acquired as a direct bill partner</span></span>

1. <span data-ttu-id="6db8f-185">**Müşterileri** seçin</span><span class="sxs-lookup"><span data-stu-id="6db8f-185">Select **Customers**</span></span>

2. <span data-ttu-id="6db8f-186">Ayrıntılarını görüntülemek için bir müşteri seçin</span><span class="sxs-lookup"><span data-stu-id="6db8f-186">Select a customer to view their details</span></span>

3. <span data-ttu-id="6db8f-187">Bu müşteri doğrudan fatura ortağı olarak elde ediyorsanız, ürün **ekleme** veya **görüntüleme** seçeneklerini görürsünüz ve aboneliklerini görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="6db8f-187">If this customer is one you acquired as a direct bill partner, you will see options to **add** or **view products** and you will see their subscriptions.</span></span>

4. <span data-ttu-id="6db8f-188">Müşterinin sizinle dolaylı bir satıcı ilişkisi varsa, bu seçenekler kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="6db8f-188">If the customer has an indirect reseller relationship with you, those options will not be available.</span></span>

## <a name="move-your-direct-bill-customers-to-your-indirect-provider"></a><span data-ttu-id="6db8f-189">Doğrudan fatura müşterilerinizi dolaylı sağlayıcınıza taşıyın</span><span class="sxs-lookup"><span data-stu-id="6db8f-189">Move your direct bill customers to your indirect provider</span></span>

<span data-ttu-id="6db8f-190">Dolaylı sağlayıcınız, mevcut doğrudan fatura müşterileriniz için bir satıcı ilişkisine sahip olana kadar sipariş veya mevcut abonelik aktarımları gönderemez.</span><span class="sxs-lookup"><span data-stu-id="6db8f-190">Your indirect provider cannot submit orders or existing subscription transfers for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="6db8f-191">Dolaylı sağlayıcınız ile var olan doğrudan faturanız arasındaki satıcı ilişkilerini oluşturmak için aşağıdaki yöntemlerden birini kullanabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="6db8f-191">To establish the reseller relationship between your indirect provider and your existing direct bill customer, you can use one of the following methods:</span></span>

- [<span data-ttu-id="6db8f-192">Satıcı ilişki uzantısı</span><span class="sxs-lookup"><span data-stu-id="6db8f-192">Reseller relationship extension</span></span>](#reseller-relationship-extension)

- [<span data-ttu-id="6db8f-193">Müşteriye dolaylı bir satıcı davetiyesi gönderin</span><span class="sxs-lookup"><span data-stu-id="6db8f-193">Send an indirect reseller invitation to the customer</span></span>](#send-an-indirect-reseller-invitation-to-the-customer)

<span data-ttu-id="6db8f-194">[Doğrudan dolaylı geçiş belgesinde](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/) adım adım işleme yönelik ayrıntılı bir genel bakış bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6db8f-194">You can find a detailed overview of the step-by-step process in the [Direct to indirect transition document](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span></span>

### <a name="reseller-relationship-extension"></a><span data-ttu-id="6db8f-195">Satıcı ilişki uzantısı</span><span class="sxs-lookup"><span data-stu-id="6db8f-195">Reseller relationship extension</span></span>

<span data-ttu-id="6db8f-196">Kurumsal ilişki uzantısı özelliğini kullanarak, mevcut doğrudan fatura müşterileriniz ve dolaylı sağlayıcınız arasında Iş Ortağı Merkezi panosunu kullanarak satıcı ilişkisi kurabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6db8f-196">You can use the reseller relationship extension feature to establish reseller relationship between your existing direct bill customers and your indirect provider using Partner Center Dashboard.</span></span> <span data-ttu-id="6db8f-197">Özelliği kullanmadan önce, aşağıdakilere göz önüne alın:</span><span class="sxs-lookup"><span data-stu-id="6db8f-197">Before using the feature, note the following:</span></span>

- <span data-ttu-id="6db8f-198">Bu özellik yalnızca dolaylı satıcı olan dolaylı satıcı [kaydını](#get-started)tamamlamış olan doğrudan fatura ortakları tarafından kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-198">This feature is only available to direct bill partners who are transitioning to become an indirect reseller have completed the [indirect reseller enrollment](#get-started).</span></span>

- <span data-ttu-id="6db8f-199">Bu özelliği yalnızca var olan doğrudan fatura müşterilerine uygulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6db8f-199">You can only apply this feature to existing direct bill customers.</span></span> <span data-ttu-id="6db8f-200">Bu, [dolaylı satıcı müşterileri](#acquire-new-customers-as-indirect-reseller)için geçerli değildir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-200">It is not applicable to [indirect reseller customers](#acquire-new-customers-as-indirect-reseller).</span></span>

- <span data-ttu-id="6db8f-201">Yalnızca [dolaylı sağlayıcıınızdan bir iş ortağı davetini kabul](#accept-a-partnership-invitation-from-your-indirect-provider)ettiğiniz bir dolaylı sağlayıcıyı seçebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6db8f-201">You can only select an indirect provider for which you have [accepted a partner invitation from your indirect provider](#accept-a-partnership-invitation-from-your-indirect-provider).</span></span>

- <span data-ttu-id="6db8f-202">Bu müşteri için sahip olduğunuz fatura-bilgi bilgilerinin bir kopyası dolaylı sağlayıcı tarafından kullanılabilir hale getirilir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-202">A copy of the bill-to info you have for this customer will be made available to the indirect provider.</span></span> <span data-ttu-id="6db8f-203">Iş Ortağı Merkezi panosunda bu müşterinin hesap sayfasına erişerek fatura bilgilerine erişebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6db8f-203">You can access the bill-to info by accessing the Account page for this customer in Partner Center Dashboard.</span></span>

    > [!NOTE]
    > <span data-ttu-id="6db8f-204">Satıcı ilişki uzantısı özelliğini kullanarak, bu müşteri için sahip olduğunuz fatura bilgilerini dolaylı sağlayıcıyla paylaşmayı kabul etmiş olursunuz.</span><span class="sxs-lookup"><span data-stu-id="6db8f-204">By using the reseller relationship extension feature, you consent to sharing the bill-to info you have for this customer with the indirect provider.</span></span>

- <span data-ttu-id="6db8f-205">Dolaylı sağlayıcınız, müşteri kiracısına [atanan yönetim ayrıcalıkları](customers-revoke-admin-privileges.md) ile birlikte sağlanmaz.</span><span class="sxs-lookup"><span data-stu-id="6db8f-205">Your indirect provider will not be provided with [delegated administration privileges](customers-revoke-admin-privileges.md) to the customer tenant.</span></span> <span data-ttu-id="6db8f-206">Dolaylı sağlayıcınız Temsilcili yönetim ayrıcalıkları gerektiriyorsa, bunun yerine müşteriye dolaylı bir satıcı daveti göndermeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-206">If your indirect provider requires delegated administration privileges, you must send an indirect reseller invitation to the customer instead.</span></span>

- <span data-ttu-id="6db8f-207">Satıcı ilişkisi kurulduktan sonra, dolaylı sağlayıcı, [M365 Yönetim Merkezi](https://admin.microsoft.com/AdminPortal/Home#/partners) 'Nde ortak ilişkiler sayfasında ve [iş için Microsoft Store](/microsoft-store/work-with-partner-microsoft-store-business), müşteriye bir CSP iş ortağı olarak görünür.</span><span class="sxs-lookup"><span data-stu-id="6db8f-207">Once the reseller relationship is established, the indirect provider will appear as a CSP partner to the customer under the Partner Relationships page in [M365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/partners) and [Microsoft Store for Business](/microsoft-store/work-with-partner-microsoft-store-business).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="6db8f-208">Karışıklık ve anlaşılmadan kaçınmak için, mevcut bir doğrudan fatura müşterisi ve dolaylı bir sağlayıcı arasında satıcı ilişkisi kurmak üzere ilişki uzantısı özelliğini kullanmadan önce, iş ortağı sözleşmenizde sözleşmeye dayalı yükümlülüğü vardır.</span><span class="sxs-lookup"><span data-stu-id="6db8f-208">To avoid confusion and misunderstanding, you are contractually obliged by your partner agreement to inform and obtain consent from the direct bill customer before you use the relationship extension feature to establish reseller relationship between an existing direct bill customer and an indirect provider.</span></span>

<span data-ttu-id="6db8f-209">Bu özelliği mevcut bir müşteri kiracısında kullanmak için:</span><span class="sxs-lookup"><span data-stu-id="6db8f-209">To use this feature on an existing customer tenant:</span></span>

1. <span data-ttu-id="6db8f-210">Iş Ortağı Merkezi ' nde bir **Yönetim Aracısı** olarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-210">Log in to Partner Center as an **Admin Agent** .</span></span>

2. <span data-ttu-id="6db8f-211">**Müşteriler sayfasında** , mevcut bir müşteriyi seçin ve müşterinin Özet görünümünü genişletmek için **hızlı bağlantılar** simgesine tıklayın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-211">In the **Customers page** , select an existing customer and click on its **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="6db8f-212">**Dolaylı sağlayıcılar** ' ın altında, **dolaylı bir sağlayıcıda müşteriyi aktar** ' a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-212">Under **Indirect provider(s)** , click **Transfer customer on an indirect provider** .</span></span>

    :::image type="content" source="images/direct/direct5-1.png" alt-text="Müşteriyi dolaylı bir sağlayıcıya aktarma":::

4. <span data-ttu-id="6db8f-214">Açılır iletişim kutusunda, müşteri ile satıcı ilişkisi olmasını istediğiniz **dolaylı sağlayıcıyı** seçin.</span><span class="sxs-lookup"><span data-stu-id="6db8f-214">In the pop-up dialog, select the **Indirect Provider** you would like to have reseller relationship with the customer.</span></span>

5. <span data-ttu-id="6db8f-215">**Kaydet ve devam et** ' e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-215">Click **Save and continue** .</span></span>

6. <span data-ttu-id="6db8f-216">Seçilen dolaylı sağlayıcının **dolaylı sağlayıcılar** altında görüntülendiğini doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-216">Verify the selected indirect provider shows up under **Indirect provider(s)** .</span></span>

    :::image type="content" source="images/direct/direct5-2.png" alt-text="Belirtilen dolaylı sağlayıcı":::

### <a name="send-an-indirect-reseller-invitation-to-the-customer"></a><span data-ttu-id="6db8f-218">Müşteriye dolaylı bir satıcı davetiyesi gönderin</span><span class="sxs-lookup"><span data-stu-id="6db8f-218">Send an indirect reseller invitation to the customer</span></span>

<span data-ttu-id="6db8f-219">Dolaylı sağlayıcınız, mevcut doğrudan fatura müşterileriniz için bir satıcı ilişkisine sahip olana kadar sipariş gönderemezler.</span><span class="sxs-lookup"><span data-stu-id="6db8f-219">Your indirect provider cannot submit orders for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="6db8f-220">Mevcut müşterileriniz ve dolaylı sağlayıcınız arasında satıcı ilişkisi kurmak için, dolaylı bir satıcı davetiyesi kullanarak müşteriyi davet edin.</span><span class="sxs-lookup"><span data-stu-id="6db8f-220">To establish the reseller relationship between your existing customers and your indirect provider, invite the customer using an indirect reseller invitation.</span></span>

1. <span data-ttu-id="6db8f-221">Iş ortağı merkezi sol gezininizden **dolaylı sağlayıcılar** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="6db8f-221">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="6db8f-222">Aynı anda hem sizin hem de dolaylı sağlayıcı ile satıcı ilişkisi kurmak üzere bir müşteriyi davet etmek için **yeni müşterileri davet et** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="6db8f-222">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="6db8f-223">Sağlayıcının müşteri ile bir satıcı ilişkisi olması gerekir, bu nedenle müşteri yeni abonelikler satın almak istediğinde veya mevcut aboneliklerde yeni lisanslar eklemek istediğinde müşterinin adına sipariş gönderebilirler.</span><span class="sxs-lookup"><span data-stu-id="6db8f-223">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

    :::image type="content" source="images/direct/direct6.png" alt-text="Yeni müşterileri davet et":::

3. <span data-ttu-id="6db8f-225">Sonraki sayfada taslak e-posta iletisini gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="6db8f-225">On the next page, review the draft email message.</span></span> <span data-ttu-id="6db8f-226">Taslak iletisini e-postada açabilir veya iletiyi panonuza kopyalayabilir ve bir e-postaya yapıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6db8f-226">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="6db8f-227">E-postadaki metni düzenleyerek, ihtiyacınız olanları söyleyin, ancak müşteriyi doğrudan hesabınıza ve sağlayıcınızın hesabınıza bağlamak için kişiselleştirildiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="6db8f-227">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="6db8f-228">Ardından **Bitti** 'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="6db8f-228">Then select **Done** .</span></span>

5. <span data-ttu-id="6db8f-229">Müşteri sizi ve sağlayıcınızı kendi kayıt satıcıları olarak doğruladıktan sonra, kendi adına aboneliklerini, lisanslarını ve kullanıcılarını yönetmek için yönetici izinlerine sahip olacaksınız ve dolaylı sağlayıcınız kendi adına sipariş gönderebilecektir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-229">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>

6. <span data-ttu-id="6db8f-230">Müşterinin hesabını, hizmetlerini, kullanıcılarını ve lisanslarını yönetmek için, adının yanındaki aşağı oku seçerek müşterinin kaydını genişletin.</span><span class="sxs-lookup"><span data-stu-id="6db8f-230">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

### <a name="microsoft-customer-agreement-acceptance"></a><span data-ttu-id="6db8f-231">Microsoft Müşteri Sözleşmesi kabulü</span><span class="sxs-lookup"><span data-stu-id="6db8f-231">Microsoft Customer Agreement acceptance</span></span>

<span data-ttu-id="6db8f-232">Microsoft Bulut sözleşmesi 31 Ocak 2020 ' ye kadar geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-232">Microsoft Cloud Agreement is valid until January 31, 2020.</span></span> <span data-ttu-id="6db8f-233">Bu tarihten sonra, mevcut ve yeni olan tüm müşteriler yeni [Microsoft Müşteri sözleşmesinin](confirm-customer-agreement.md)imzalanmalıdır.</span><span class="sxs-lookup"><span data-stu-id="6db8f-233">After that date, all customers, existing and new, must sign the new [Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span> <span data-ttu-id="6db8f-234">Şu durumlarda müşterilerin geçişini yapmak için:</span><span class="sxs-lookup"><span data-stu-id="6db8f-234">For transitioning customers, if:</span></span>

- <span data-ttu-id="6db8f-235">**Müşteri henüz Microsoft Müşteri sözleşmesini kabul etmedi**</span><span class="sxs-lookup"><span data-stu-id="6db8f-235">**Customer has not accepted Microsoft Customer Agreement yet**</span></span>

   <span data-ttu-id="6db8f-236">Müşterinin [Microsoft Müşteri anlaşmasını kabul](confirm-customer-agreement.md)etmesi Için lütfen dolaylı sağlayıcıyla çalışın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-236">Please work with Indirect Provider to have customer [accept the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

- <span data-ttu-id="6db8f-237">**Müşteri, Microsoft 365 Yönetim Merkezi ile Microsoft Müşteri anlaşmasını sizinle kabul etti**</span><span class="sxs-lookup"><span data-stu-id="6db8f-237">**Customer has accepted Microsoft Customer Agreement with you through the Microsoft 365 Admin Center**</span></span>

   <span data-ttu-id="6db8f-238">Satıcı ilişkisi dolaylı sağlayıcıyla kurulduktan sonra kabul edilir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-238">The acceptance will be retained once the reseller relationship is established with the Indirect Provider.</span></span> <span data-ttu-id="6db8f-239">Yapmanız gereken bir şey yok.</span><span class="sxs-lookup"><span data-stu-id="6db8f-239">There is nothing you need to do.</span></span>

- <span data-ttu-id="6db8f-240">**Müşteri, iş ortağı kanıtlama ile Microsoft Müşteri sözleşmesini kabul etti**</span><span class="sxs-lookup"><span data-stu-id="6db8f-240">**Customer has accepted Microsoft Customer Agreement with you through partner attestation**</span></span>

   <span data-ttu-id="6db8f-241">Kabul tutulmayacaktır.</span><span class="sxs-lookup"><span data-stu-id="6db8f-241">The acceptance will not be retained.</span></span> <span data-ttu-id="6db8f-242">[Müşterinin Iş Ortağı Merkezi 'nin kabulünü güncelleştirmek](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers)Için lütfen dolaylı sağlayıcıyla çalışın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-242">Please work with Indirect Provider to [update the customer's acceptance in Partner Center](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span></span>

## <a name="transfer-existing-direct-bill-subscriptions-to-indirect-provider"></a><span data-ttu-id="6db8f-243">Mevcut doğrudan fatura aboneliklerini dolaylı sağlayıcıya aktar</span><span class="sxs-lookup"><span data-stu-id="6db8f-243">Transfer existing direct bill subscriptions to indirect provider</span></span>

<span data-ttu-id="6db8f-244">CSP dolaylı modeli kapsamında, dolaylı satıcıların Microsoft ile faturalandırma ilişkileri yoktur.</span><span class="sxs-lookup"><span data-stu-id="6db8f-244">Under CSP indirect model, indirect resellers do not have billing relationships with Microsoft.</span></span> <span data-ttu-id="6db8f-245">Bunun yerine dolaylı satıcılar, kendi dolaylı sağlayıcıları aracılığıyla müşterileri için abonelikler elde eder.</span><span class="sxs-lookup"><span data-stu-id="6db8f-245">Instead, indirect resellers obtain subscriptions for their customers through their indirect providers.</span></span> <span data-ttu-id="6db8f-246">Doğrudan fatura ortağından dolaylı satıcıya geçiş yaparken, sahip olduğunuz mevcut abonelikleri dolaylı sağlayıcınıza doğrudan fatura ortağı olarak aktarmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-246">While transitioning from direct bill partner to indirect reseller, you need to transfer the existing subscriptions you have as the direct bill partner to your indirect provider.</span></span> <span data-ttu-id="6db8f-247">Bunu yapmak için, Iş Ortağı Merkezi panosunda kendi kendine sunulan abonelik aktarma özelliğini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6db8f-247">You can use the self-served subscription transfer feature in Partner Center Dashboard to do so.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="6db8f-248">Ön koşullar</span><span class="sxs-lookup"><span data-stu-id="6db8f-248">Pre-requisites</span></span>

- <span data-ttu-id="6db8f-249">Bu özellik yalnızca mevcut doğrudan fatura ortağı kiracılarını kullanarak dolaylı satıcı kaydını tamamlamış olan iş ortakları arasında geçiş yapılabilir</span><span class="sxs-lookup"><span data-stu-id="6db8f-249">This feature is only available to transitioning partners who have completed the indirect reseller enrollment using their existing direct bill partner tenants</span></span>

- <span data-ttu-id="6db8f-250">Belirli bir müşteriyle ilişkili abonelikleri aktarmadan önce, geçiş ortağı müşteriyi dolaylı bir sağlayıcıya taşımalıdır.</span><span class="sxs-lookup"><span data-stu-id="6db8f-250">Before transferring subscriptions associated with a given customer, the transitioning partner must move the customer to an indirect provider.</span></span>

- <span data-ttu-id="6db8f-251">Müşterinin [dolaylı sağlayıcı aracılığıyla Microsoft Müşteri anlaşmasını kabul](#microsoft-customer-agreement-acceptance)etmiş olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-251">Customer must have [accepted Microsoft Customer Agreement through the Indirect Provider](#microsoft-customer-agreement-acceptance).</span></span>

### <a name="how-to-transition-to-indirect-reseller-status"></a><span data-ttu-id="6db8f-252">Dolaylı satıcı durumuna geçiş</span><span class="sxs-lookup"><span data-stu-id="6db8f-252">How to transition to indirect reseller status</span></span>

<span data-ttu-id="6db8f-253">Özelliği 4 adımlı bir işlemdir; burada:</span><span class="sxs-lookup"><span data-stu-id="6db8f-253">The feature is a 4-step process, where:</span></span>

- <span data-ttu-id="6db8f-254">Geçiş ortağı bir abonelik aktarma isteği oluşturur.</span><span class="sxs-lookup"><span data-stu-id="6db8f-254">The transitioning partner creates a subscription transfer request.</span></span> <span data-ttu-id="6db8f-255">İstek, aynı müşteriyle ilişkili bir veya daha fazla var olan abonelik içeriyor ve dolaylı bir sağlayıcıya yönelik.</span><span class="sxs-lookup"><span data-stu-id="6db8f-255">The request contains one or more existing subscriptions associated with the same customer and is addressed to an indirect provider.</span></span>

- <span data-ttu-id="6db8f-256">Dolaylı sağlayıcı, aktarım isteğini gözden geçirir ve kabul eder (veya reddeder).</span><span class="sxs-lookup"><span data-stu-id="6db8f-256">The indirect provider reviews and accepts (or reject) the transfer request.</span></span>

- <span data-ttu-id="6db8f-257">Dolaylı sağlayıcı, aktarım isteğinin tamamlandığını doğrular.</span><span class="sxs-lookup"><span data-stu-id="6db8f-257">The indirect provider verifies that the transfer request is complete.</span></span>

- <span data-ttu-id="6db8f-258">Geçiş ortağı, aktarım isteğinin tamamlandığını doğrular.</span><span class="sxs-lookup"><span data-stu-id="6db8f-258">The transitioning partner verifies that the transfer request is complete.</span></span>

### <a name="transitioning-partner"></a><span data-ttu-id="6db8f-259">İş ortağı geçiyor</span><span class="sxs-lookup"><span data-stu-id="6db8f-259">Transitioning partner</span></span>

> [!NOTE]
> <span data-ttu-id="6db8f-260">Ayrıca, mevcut abonelikleri dolaylı sağlayıcınıza aktarmak için [Iş ortağı MERKEZI API/SDK](/partner-center/develop/manage-customers) 'sını de kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6db8f-260">You can also use [Partner Center API/SDK](/partner-center/develop/manage-customers) to transfer the existing subscriptions to your indirect provider.</span></span>
>
> - [<span data-ttu-id="6db8f-261">Müşterinin abonelik aktarım uygunluğunu al</span><span class="sxs-lookup"><span data-stu-id="6db8f-261">Get a customer's subscriptions transfer eligibility</span></span>](/partner-center/develop/get-customer-s-subscriptions-transfer-eligibility)
> - [<span data-ttu-id="6db8f-262">Müşterinin aktarımını oluşturma</span><span class="sxs-lookup"><span data-stu-id="6db8f-262">Create a customer's transfer</span></span>](/partner-center/develop/create-a-transfer)
> - [<span data-ttu-id="6db8f-263">Müşterinin aktarımını geri alma</span><span class="sxs-lookup"><span data-stu-id="6db8f-263">Withdraw a customer's transfer</span></span>](/partner-center/develop/withdraw-a-transfer)
> - [<span data-ttu-id="6db8f-264">Müşterinin aktarımını kabul et</span><span class="sxs-lookup"><span data-stu-id="6db8f-264">Accept a customer's transfer</span></span>](/partner-center/develop/accept-a-transfer)
> - [<span data-ttu-id="6db8f-265">Müşterinin aktarımını reddetme</span><span class="sxs-lookup"><span data-stu-id="6db8f-265">Reject a Customer's transfer</span></span>](/partner-center/develop/reject-a-transfer)
> - [<span data-ttu-id="6db8f-266">Müşterinin aktarımlarını al</span><span class="sxs-lookup"><span data-stu-id="6db8f-266">Get a customer's transfers</span></span>](/partner-center/develop/get-all-of-a-customer-s-transfers)
> - [<span data-ttu-id="6db8f-267">Kimliğe göre aktarım ayrıntılarını al</span><span class="sxs-lookup"><span data-stu-id="6db8f-267">Get transfer details by id</span></span>](/partner-center/develop/get-transfer-by-id)

### <a name="transitioning-partner---create-transfer-request"></a><span data-ttu-id="6db8f-268">İş ortağı geçişi-aktarım isteği oluşturma</span><span class="sxs-lookup"><span data-stu-id="6db8f-268">Transitioning partner - create transfer request</span></span>

<span data-ttu-id="6db8f-269">Geçiş ortağı olarak bir aktarım isteği oluşturmak için:</span><span class="sxs-lookup"><span data-stu-id="6db8f-269">To create a transfer request as the transitioning partner:</span></span>

1. <span data-ttu-id="6db8f-270">Iş Ortağı Merkezi ' nde bir **Yönetim Aracısı** olarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-270">Log in to Partner Center as an **Admin Agent** .</span></span>

2. <span data-ttu-id="6db8f-271">**Müşteriler** sayfasında, istenen müşteriyi seçin ve hızlı bağlantılar simgesine tıklayarak müşterinin Özet görünümünü genişletin.</span><span class="sxs-lookup"><span data-stu-id="6db8f-271">In the **Customers** page, select the intended customer and click on the Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="6db8f-272">**Dolaylı sağlayıcılar** ' ın altında, amaçlanan dolaylı sağlayıcının listelendiğini onaylayın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-272">Under **Indirect provider(s)** , confirm that the intended indirect provider is listed.</span></span>

4. <span data-ttu-id="6db8f-273">**Abonelikleri görüntüle** ' ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-273">Click **View Subscriptions** .</span></span>

5. <span data-ttu-id="6db8f-274">**Abonelikler** sayfasında, **abonelik aktarımı** ' nı arayın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-274">In the **Subscriptions** page, look for **Subscription Transfer** .</span></span>

6. <span data-ttu-id="6db8f-275">**Abonelik aktarımı** altında **abonelik aktarımı iste** ' ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-275">Under **Subscription Transfer** , click **Request subscription transfer** .</span></span>

    :::image type="content" source="images/direct/direct8.png" alt-text="Abonelik aktarımı iste":::

7. <span data-ttu-id="6db8f-277">Aktarım isteği iletişim kutusunda, aktarılacak bir veya daha fazla abonelik seçin.</span><span class="sxs-lookup"><span data-stu-id="6db8f-277">In the transfer request dialog, select one or more subscriptions to be transferred.</span></span>

    :::image type="content" source="images/direct/direct9.png" alt-text="Aktarım Isteği oluştur":::

8. <span data-ttu-id="6db8f-279">**Oluştur** 'a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-279">Click **Create** .</span></span>

9. <span data-ttu-id="6db8f-280">**Abonelik aktarımı** altında, etkin bir abonelik aktarım isteği görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-280">An active subscription transfer request will appear under **Subscription Transfer** .</span></span>

    :::image type="content" source="images/direct/direct10.png" alt-text="İstek listesini aktar":::

10. <span data-ttu-id="6db8f-282">Dolaylı sağlayıcınızı, bunlara bir abonelik aktarım isteği oluşturduğunu bildirin.</span><span class="sxs-lookup"><span data-stu-id="6db8f-282">Inform your indirect provider that you have created a subscription transfer request to them.</span></span>

### <a name="indirect-provider---accept-transfer-request"></a><span data-ttu-id="6db8f-283">Dolaylı sağlayıcı-aktarım isteğini kabul et</span><span class="sxs-lookup"><span data-stu-id="6db8f-283">Indirect provider - accept transfer request</span></span>

<span data-ttu-id="6db8f-284">Bir aktarım isteğini dolaylı sağlayıcı olarak gözden geçirmek ve kabul etmek için:</span><span class="sxs-lookup"><span data-stu-id="6db8f-284">To review and accept a transfer request as the indirect provider:</span></span>

1. <span data-ttu-id="6db8f-285">Iş Ortağı Merkezi 'nde bir **Yönetim** Aracısı veya **Satış Aracısı** olarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-285">Log in to Partner Center as an **Admin** Agent or **Sales Agent** .</span></span>

2. <span data-ttu-id="6db8f-286">**Müşteriler** sayfasında, istenen müşteriyi seçin ve müşterinin Özet görünümünü genişletmek için hızlı bağlantılar simgesine tıklayın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-286">In the **Customers** page, select the intended customer and click on its Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="6db8f-287">**Dolaylı satıcı (ler)** altında, geçiş ortağının listelendiğini onaylayın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-287">Under **Indirect reseller(s)** , confirm the transitioning partner is listed.</span></span>

4. <span data-ttu-id="6db8f-288">**Abonelikleri görüntüle** ' ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-288">Click **View Subscriptions** .</span></span>

5. <span data-ttu-id="6db8f-289">**Abonelikler** sayfasında, **abonelik aktarımı** ' nı arayın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-289">In the **Subscriptions** page, look for **Subscription Transfer** .</span></span>

    :::image type="content" source="images/direct/direct11.png" alt-text="Aktarım isteğini görüntüle":::

6. <span data-ttu-id="6db8f-291">**Abonelik aktarımı** altında, gözden geçirmek için aktarım isteğine tıklayın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-291">Under **Subscription Transfer** , click on the transfer request to review.</span></span>

7. <span data-ttu-id="6db8f-292">Uygun şekilde **kabul et** (veya **Reddet** ) seçeneğine tıklayın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-292">Click **Accept** (or **Reject** ) as appropriate.</span></span>

    :::image type="content" source="images/direct/direct12.png" alt-text="Aktarım isteğini kabul et":::

8. <span data-ttu-id="6db8f-294">Aktarım isteğinin tamamlanmasını bekleyin.</span><span class="sxs-lookup"><span data-stu-id="6db8f-294">Wait for the transfer request to complete.</span></span>

### <a name="indirect-provider---verify-transfer-request-is-complete"></a><span data-ttu-id="6db8f-295">Dolaylı sağlayıcı-aktarım isteğinin tamamlandığını doğrulama</span><span class="sxs-lookup"><span data-stu-id="6db8f-295">Indirect provider - verify transfer request is complete</span></span>

1. <span data-ttu-id="6db8f-296">Aktarım isteği başarıyla tamamlandıktan sonra, aboneliklerin **abonelikler** bölümünde göründüğünü görebildiğinizi doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-296">After the transfer request is completed successfully, verify that you can see the subscriptions appear under **Subscriptions** .</span></span>

2. <span data-ttu-id="6db8f-297">Geçiş ortağına bildirin.</span><span class="sxs-lookup"><span data-stu-id="6db8f-297">Inform the transitioning partner.</span></span>

### <a name="transitioning-partner---verify-transfer-request-is-complete"></a><span data-ttu-id="6db8f-298">Geçiş ortağı-aktarım isteğini doğrulama işlemi tamamlanmıştır</span><span class="sxs-lookup"><span data-stu-id="6db8f-298">Transitioning partner - verify transfer request is complete</span></span>

<span data-ttu-id="6db8f-299">Geçiş ortağı aşağıdakileri yapması gerekir:</span><span class="sxs-lookup"><span data-stu-id="6db8f-299">The transitioning partner should do the following:</span></span>

1. <span data-ttu-id="6db8f-300">Iş Ortağı Merkezi 'Nde bir **Yönetim Aracısı** veya **Satış Aracısı** olarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-300">Sign into Partner Center as an **Admin Agent** or **Sales Agent** .</span></span>

2. <span data-ttu-id="6db8f-301">**Müşteriler** sayfasında, istenen müşteriyi seçin ve **hızlı bağlantılar** simgesine tıklayarak müşterinin Özet görünümünü genişletin.</span><span class="sxs-lookup"><span data-stu-id="6db8f-301">In the **Customers** page, select the intended customer and click on the **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="6db8f-302">**Abonelikleri görüntüle** ' ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-302">Click **View Subscriptions** .</span></span>

4. <span data-ttu-id="6db8f-303">**Abonelikler** sayfasında, **abonelik aktarımı** ' nı arayın.</span><span class="sxs-lookup"><span data-stu-id="6db8f-303">In the **Subscriptions** page, look for **Subscription Transfer** .</span></span>

5. <span data-ttu-id="6db8f-304">Aktarım isteğinin **Tamam** olarak işaretlendiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="6db8f-304">Verify that the transfer request is marked as **Complete** .</span></span>

6. <span data-ttu-id="6db8f-305">Aboneliğin artık **abonelikler** sayfasında etkin olarak görünmediğini doğrulayın:</span><span class="sxs-lookup"><span data-stu-id="6db8f-305">Verify that the subscription(s) no longer appear as active in the **Subscriptions** page:</span></span>

   1. <span data-ttu-id="6db8f-306">Bu bir Azure aboneliğse (MS-AZR-0145P), artık listelenmez.</span><span class="sxs-lookup"><span data-stu-id="6db8f-306">If this is an Azure subscription (MS-AZR-0145P), it will no longer be listed.</span></span>

   2. <span data-ttu-id="6db8f-307">Bu bir lisans tabanlı aboneliğiniz (Office 365, Dynamics, Intune), durumu **askıya alındı** olarak listelenir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-307">If this is a license-based subscription (Office 365, Dynamics, Intune), it will be listed with state as **Suspended** .</span></span>

   :::image type="content" source="images/direct/direct13.png" alt-text="Abonelik askıya alındı":::

### <a name="considerations"></a><span data-ttu-id="6db8f-309">Dikkat edilmesi gerekenler</span><span class="sxs-lookup"><span data-stu-id="6db8f-309">Considerations</span></span>

- <span data-ttu-id="6db8f-310">**Abonelik KIMLIĞI aktarımdan sonra farklı olacaktır.**</span><span class="sxs-lookup"><span data-stu-id="6db8f-310">**Subscription ID will be different after transfer.**</span></span> <span data-ttu-id="6db8f-311">Bu bir Azure aboneliğiyiyse (MS-AZR-0145P), buna ek olarak, önceki sahibinden tutulan ve Azure yönetim portalında görünecek bir Azure abonelik KIMLIĞI olur.</span><span class="sxs-lookup"><span data-stu-id="6db8f-311">If it is an Azure subscription (MS-AZR-0145P), additionally, it will have an Azure Subscription ID, which is retained from the previous owner, and will appear in the Azure management portal.</span></span>

- <span data-ttu-id="6db8f-312">**Aynı aboneliğe birden çok aktarım isteği tarafından başvurulamaz.**</span><span class="sxs-lookup"><span data-stu-id="6db8f-312">**The same subscription cannot be referenced by multiple transfer requests.**</span></span> <span data-ttu-id="6db8f-313">Mevcut bir aboneliği içeren bir aktarım isteği oluşturduktan sonra, ilk aktarım isteği iptal edilene kadar aynı abonelik dahil olmak üzere ek aktarım istekleri oluşturamazsınız.</span><span class="sxs-lookup"><span data-stu-id="6db8f-313">After you have created a transfer request, which includes an existing subscription, you cannot create additional transfer requests including the same subscription, until the first transfer request is canceled.</span></span>

- <span data-ttu-id="6db8f-314">**Lisans tabanlı abonelikler için eklentiler, temel abonelikleriyle birlikte aktarılmalıdır.**</span><span class="sxs-lookup"><span data-stu-id="6db8f-314">**Add-ons for license-based subscriptions must be transferred along with their base subscription.**</span></span> <span data-ttu-id="6db8f-315">Bir aktarım isteği oluştururken, bir veya daha fazla eklentiye sahip mevcut bir aboneliği seçerseniz, eklenti otomatik olarak aktarım isteğine dahil edilir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-315">When creating a transfer request, if you pick an existing subscription with one or more add-ons, the add-ons will automatically be included in the transfer request.</span></span>

- <span data-ttu-id="6db8f-316">**Bir abonelikte lisans sayısı değişiklikleri var olan aktarım isteğine yansıtılmayacaktır.**</span><span class="sxs-lookup"><span data-stu-id="6db8f-316">**License count changes to a subscription will not be reflected in existing transfer request.**</span></span> <span data-ttu-id="6db8f-317">Var olan bir aboneliği içeren bir aktarım isteği oluşturduktan sonra, aboneliğin lisans miktarını (veya ilişkili eklentiler) güncelleştirmeden kaçınmalısınız.</span><span class="sxs-lookup"><span data-stu-id="6db8f-317">After you have created a transfer request which includes an existing subscription, you should avoid updating the license quantity of the subscription (or associated addons).</span></span> <span data-ttu-id="6db8f-318">Bunu yaparsanız, yeni miktar aktarım isteğine yansıtılmayacaktır.</span><span class="sxs-lookup"><span data-stu-id="6db8f-318">If you do so, the new quantity will not be reflected in the transfer request.</span></span> <span data-ttu-id="6db8f-319">Dolaylı sağlayıcı aktarım isteğini kabul ettikten sonra, sonuçta elde edilen abonelik eski miktara sahip olur.</span><span class="sxs-lookup"><span data-stu-id="6db8f-319">After the indirect provider accepts the transfer request, the resultant subscription will have the old quantity.</span></span> <span data-ttu-id="6db8f-320">Yeni miktarın dolaylı sağlayıcıya aktarılmasını istiyorsanız, var olan aktarım isteğini iptal etmeniz ve yeni bir tane oluşturmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-320">If you wish for the new quantity to be transferred to the indirect provider, you must cancel the existing transfer request and recreate a new one.</span></span>

- <span data-ttu-id="6db8f-321">**Satın alma işlemleri, kendi kendine sunulan abonelik aktarımı kullanılarak aktarılamaz.**</span><span class="sxs-lookup"><span data-stu-id="6db8f-321">**Not all purchases can be transferred using self-served subscription transfer.**</span></span> <span data-ttu-id="6db8f-322">Şu anda, bu özelliği kullanarak yalnızca O365 aboneliklerini ve Azure PAYG aboneliklerini (MS-AZR-0145P) aktarabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6db8f-322">Currently, you can only transfer O365 subscriptions and Azure PAYG subscriptions (MS-AZR-0145P) using this feature.</span></span> <span data-ttu-id="6db8f-323">Azure planları, Azure ayrılmış örnekleri, terim tabanlı abonelikler ve Azure Marketi için SaaS abonelikleri dahil diğer satın alma işlemleri desteklenmez.</span><span class="sxs-lookup"><span data-stu-id="6db8f-323">Other purchases including Azure Plans, Azure Reserved Instances, Term-based Subscriptions and SaaS subscriptions for Azure Marketplace are not supported.</span></span> <span data-ttu-id="6db8f-324">Aktarım isteği Gönder sayfasında aboneliğin neden aktarılamadığına ilişkin bir neden göreceksiniz.</span><span class="sxs-lookup"><span data-stu-id="6db8f-324">You will see a reason why a subscription cannot be transferred in the submit transfer request page.</span></span> <span data-ttu-id="6db8f-325">Bu abonelikleri aktarmak için, [mevcut aboneliği iptal](create-a-new-subscription.md#suspend-or-cancel-a-subscription) etmeniz ve dolaylı sağlayıcı aracılığıyla müşteri için yeni teklif satın almanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-325">To transfer these subscriptions, you will need to [cancel the existing subscription](create-a-new-subscription.md#suspend-or-cancel-a-subscription) and purchase new offer for customer through Indirect Provider.</span></span>

- <span data-ttu-id="6db8f-326">**Korumalı alan ortamı kullanılarak test edilemez.**</span><span class="sxs-lookup"><span data-stu-id="6db8f-326">**Cannot be tested using sandbox environment.**</span></span>

## <a name="enroll-for-indirect-reseller-incentives"></a><span data-ttu-id="6db8f-327">Dolaylı satıcı teşvikleri kaydolun</span><span class="sxs-lookup"><span data-stu-id="6db8f-327">Enroll for indirect reseller incentives</span></span>

<span data-ttu-id="6db8f-328">Mevcut doğrudan fatura ortağı kiracınızda dolaylı bir satıcı olarak başarıyla kaydolduktan sonra, 30 gün içinde dolaylı satıcı teşvik etmek için kaydolma daveti alacaksınız.</span><span class="sxs-lookup"><span data-stu-id="6db8f-328">After you have successfully enrolled as an indirect reseller on your existing direct bill partner tenant, you will receive an invitation to enroll for indirect reseller incentive within 30 days.</span></span> <span data-ttu-id="6db8f-329">Davet, CSP iş ortağı kiracınızla ilişkilendirilmiş olan iş ortağı MPN hesabına dayalıdır.</span><span class="sxs-lookup"><span data-stu-id="6db8f-329">The invitation is based on the partner MPN account that is currently associated with your CSP partner tenant.</span></span> <span data-ttu-id="6db8f-330">Davet, iş ortağı MPN hesabıyla ilişkili e-posta adresine gönderilir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-330">The invitation will be sent to the email address associated with the partner MPN account.</span></span>

<span data-ttu-id="6db8f-331">Ayrıca, aynı iş ortağı kiracısıyla doğrudan fatura teşvik programlarına kaydolma yetkiniz vardır.</span><span class="sxs-lookup"><span data-stu-id="6db8f-331">You are also eligible to enroll for direct bill incentive programs with that same partner tenant.</span></span> <span data-ttu-id="6db8f-332">Programları ayrı ayrı yönetmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="6db8f-332">You must manage the programs separately.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6db8f-333">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="6db8f-333">Next steps</span></span>

- [<span data-ttu-id="6db8f-334">Dolaylı satıcı olma hakkında ek bilgiler</span><span class="sxs-lookup"><span data-stu-id="6db8f-334">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)
- [<span data-ttu-id="6db8f-335">CSP doğrudan iş ortağı yeni gereksinimler</span><span class="sxs-lookup"><span data-stu-id="6db8f-335">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)
- [<span data-ttu-id="6db8f-336">Kısıtlanmış doğrudan fatura özellikleri</span><span class="sxs-lookup"><span data-stu-id="6db8f-336">Restricted direct bill capabilities</span></span>](restricted-direct-bill-capabilities.md)