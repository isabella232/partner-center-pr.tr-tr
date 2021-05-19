---
title: CSP bölgesel yetkilendirme kiracı birleştirmesi
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Farklı ülke/bölgeler için kiracıları birleştirmek için bu yönergeleri kullanın. Bu, müşteri hesaplarını ve müşteri aboneliklerini geçirme adımlarını içerir.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: d2168dcd60b8675a21960918dab49b778025fa51
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147590"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="fa62a-104">CSP bölgesel yetkilendirme kiracı birleştirme yönergeleri</span><span class="sxs-lookup"><span data-stu-id="fa62a-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="fa62a-105">**Uygulama:** İş Ortağı Merkezi | İş Ortağı Merkezi için Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="fa62a-105">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="fa62a-106">**Uygun roller:** Genel yönetici | Yönetici aracısı</span><span class="sxs-lookup"><span data-stu-id="fa62a-106">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="fa62a-107">\[Bazı bilgiler, ticari olarak yayınlanmadan önce önemli ölçüde değiştirilabilecek, önceden yayımlanan ürünle ilgilidir.</span><span class="sxs-lookup"><span data-stu-id="fa62a-107">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="fa62a-108">Burada verilen bilgilerle ilgili olarak Microsoft açık veya zımni hiçbir garanti vermez.\]</span><span class="sxs-lookup"><span data-stu-id="fa62a-108">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="fa62a-109">İşletmeniz için kiracıları birleştirin.</span><span class="sxs-lookup"><span data-stu-id="fa62a-109">You can consolidate tenants for your business.</span></span> <span data-ttu-id="fa62a-110">Farklı ülke/bölgeler için kiracıları birleştirmek için bu yönergeleri kullanın.</span><span class="sxs-lookup"><span data-stu-id="fa62a-110">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="fa62a-111">Geçişte olduğunuz hesapta yer alan müşterilerin her biri için sağlanan tüm aboneliklerin ve lisans sayılarının farkında olmak gerekir.</span><span class="sxs-lookup"><span data-stu-id="fa62a-111">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="fa62a-112">Geçiş işleminin bir parçası olarak yeni merkezi CSP hesabı altında aynı lisans sayılarını tam olarak aynı abonelikleri yeniden sağlarsınız.</span><span class="sxs-lookup"><span data-stu-id="fa62a-112">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="fa62a-113">Merkezi kiracıya taşınarak müşterilerin listesini oluşturmanıza yardımcı olmak için dışarı aktarma listesi özelliğini kullanın.</span><span class="sxs-lookup"><span data-stu-id="fa62a-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="fa62a-114">Birleştirme tamamlandıktan sonra önceki kiracı durumuna geri dönebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fa62a-114">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="fa62a-115">Müşteri eylemi de gerekli olabilir.</span><span class="sxs-lookup"><span data-stu-id="fa62a-115">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="fa62a-116">Geçiş için hazırlanma</span><span class="sxs-lookup"><span data-stu-id="fa62a-116">Prepare for migration</span></span>

- <span data-ttu-id="fa62a-117">Geçiş **İş Ortağı Merkezi** (yeni hesaba  geçiş yapmak için) kullanarak oturum açın ve tüm müşterileri ve bu müşteriler için sağlanan tüm hizmetleri gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="fa62a-117">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="fa62a-118">Bu hesabın oturumlarını açın.</span><span class="sxs-lookup"><span data-stu-id="fa62a-118">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="fa62a-119">Müşteri hesaplarını geçirme</span><span class="sxs-lookup"><span data-stu-id="fa62a-119">Migrate customer accounts</span></span>

1. <span data-ttu-id="fa62a-120">Geçiş **(yeni İş Ortağı Merkezi** **hesabıyla** (müşterileri geçişte olduğunuz hesap) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="fa62a-120">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="fa62a-121">**Müşteriler**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="fa62a-121">Select **Customers**.</span></span>

3. <span data-ttu-id="fa62a-122">Kurumsal **bayi ilişkisi isteğide bulun seçeneğini seçin.**</span><span class="sxs-lookup"><span data-stu-id="fa62a-122">Select **Request a reseller relationship**.</span></span> <span data-ttu-id="fa62a-123">Müşterilerinize göndermek için size varsayılan bir e-posta iletisi gönderilir.</span><span class="sxs-lookup"><span data-stu-id="fa62a-123">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="fa62a-124">Bu ileti, yeni İş Ortağı Merkezi hesabınız için benzersiz kuruluş kimliğine sahip bir URL içerir.</span><span class="sxs-lookup"><span data-stu-id="fa62a-124">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="fa62a-125">**Müşteri eylemi:** Geçirmek istediğiniz her bir etkin müşterilerin bu URL 'YI ziyaret etmesini sağlayın.</span><span class="sxs-lookup"><span data-stu-id="fa62a-125">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="fa62a-126">URL 'YI açarken, müşterinin Office 365 portalında oturum açması istenir.</span><span class="sxs-lookup"><span data-stu-id="fa62a-126">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="fa62a-127">Müşteri, Azure ve Office 365 yönetim portallarına erişmek için kullandıkları aynı kuruluş KIMLIĞINI kullanarak oturum açar.</span><span class="sxs-lookup"><span data-stu-id="fa62a-127">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="fa62a-128">Oturum açtıktan sonra, **müşteri hesabına** ait genel YÖNETICININ yeni CSP hesabına yönetici ayrıcalıkları sağlayan bir anlaşma göndermesi istenir.</span><span class="sxs-lookup"><span data-stu-id="fa62a-128">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="fa62a-129">Kabul ederse, müşteri onay kutusunu seçer ve ilişkiye izin vermeyi kabul eder.</span><span class="sxs-lookup"><span data-stu-id="fa62a-129">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="fa62a-130">Müşteriler, sözleşmeyi gönderdikten sonra iş ortağının müşteri listesinde görünür.</span><span class="sxs-lookup"><span data-stu-id="fa62a-130">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="fa62a-131">Office 365 ve Azure olmayan kullanım tabanlı abonelikleri geçirme</span><span class="sxs-lookup"><span data-stu-id="fa62a-131">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="fa62a-132">Müşterinizin Sözleşmesi imzalandıktan sonra, kendi aboneliklerini merkezi Iş ortağı kiracınız altında yeniden oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fa62a-132">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="fa62a-133">**Iş Ortağı Merkezi**'nden **müşteriler**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="fa62a-133">From **Partner Center**, select **Customers**.</span></span>

3. <span data-ttu-id="fa62a-134">Geçirmek istediğiniz müşterinin şirket adını açın.</span><span class="sxs-lookup"><span data-stu-id="fa62a-134">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="fa62a-135">**Abonelik Ekle**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="fa62a-135">Select **Add subscription**.</span></span>

5. <span data-ttu-id="fa62a-136">Katalogdan doğru abonelikleri ve lisans sayılarını ekleyin.</span><span class="sxs-lookup"><span data-stu-id="fa62a-136">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="fa62a-137">**İş ortağı** hesaplarından geçiş sırasında belirtilen bilgilerle doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="fa62a-137">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="Müşteri listesi":::

6. <span data-ttu-id="fa62a-139">Gönder ' i seçin **.**</span><span class="sxs-lookup"><span data-stu-id="fa62a-139">Select **Submit.**</span></span>

   <span data-ttu-id="fa62a-140">Hizmetler artık **müşteriye iş ortağı** hesabına geçiş üzerinden sağlanır.</span><span class="sxs-lookup"><span data-stu-id="fa62a-140">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="fa62a-141">Tüm ek müşterilerin aboneliklerini geçirmek için bu adımları tekrarlayın.</span><span class="sxs-lookup"><span data-stu-id="fa62a-141">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="fa62a-142">Bir sonraki bölüme geçmeden önce **, iş ortağı** hesaplarından geçiş altında bulunan tüm müşteri aboneliklerinin **iş ortağı hesabına** geçiş altında yeniden sağlandığını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="fa62a-142">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="fa62a-143">İş ortakları, iş ortağı Merkezi **'nde iş ortağı** kiracı hesabından geçiş sırasında abonelikleri askıya almalıdır. bu abonelikler, Çift faturalandırma işleminin gerçekleşmemesini sağlamak için Iş Ortağı Merkezi 'nde **iş ortağı kiracı** hesabı altına geçirilir ve ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="fa62a-143">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="fa62a-144">Aboneliklerden Geçiş doğru şekilde devre dışı bırakılamayarak oluşan faturalama çakışmaları nedeniyle krediler için **destek istekleri reddedilir.**</span><span class="sxs-lookup"><span data-stu-id="fa62a-144">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="fa62a-145">İş ortağı hesabından geçiş altında Office 365 aboneliklerini devre dışı bırakma</span><span class="sxs-lookup"><span data-stu-id="fa62a-145">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="fa62a-146">CSP aboneliğini İş ortağı hesaplarından **Geçiş altında devre** dışı bırakmak gelecekte faturalamayı durdurur.</span><span class="sxs-lookup"><span data-stu-id="fa62a-146">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="fa62a-147">Geçiş işlemi sırasında Azure abonelikleri otomatik olarak devre dışı bırakılana kadar Azure aboneliklerini el ile devre dışı bırakmanız gerekmez.</span><span class="sxs-lookup"><span data-stu-id="fa62a-147">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="fa62a-148">CSP **hesabından İş Ortağı Merkezi** **hesabıyla** oturum açın ve müşteri listesine gidin.</span><span class="sxs-lookup"><span data-stu-id="fa62a-148">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="fa62a-149">Devre dışı bırakmak için müşteriyi aboneliklerle açın ve devre dışı bırakmak için ilk teklifi seçin.</span><span class="sxs-lookup"><span data-stu-id="fa62a-149">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="fa62a-150">Aboneliği askıya alındı **olarak ayarlayın** ve gönder'i **seçin.**</span><span class="sxs-lookup"><span data-stu-id="fa62a-150">Set the subscription to **suspended**, and then select **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="fa62a-151">Aboneliğin askıya alınması, çift faturalamanın oluşmaz.</span><span class="sxs-lookup"><span data-stu-id="fa62a-151">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="fa62a-152">Abonelik, **abonelikler listesinde** askıya alınmış olarak görünür.</span><span class="sxs-lookup"><span data-stu-id="fa62a-152">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="fa62a-153">Müşteri altındaki tüm abonelikler için bu adımları tekrarlayın.</span><span class="sxs-lookup"><span data-stu-id="fa62a-153">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="fa62a-154">Tüm show askıya alınmış **olduğunu doğrulayın.**</span><span class="sxs-lookup"><span data-stu-id="fa62a-154">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="fa62a-155">Listeden bir sonraki müşteriyi seçin ve tüm abonelikleri devre dışı bırakma işlemini tekrarlayın.</span><span class="sxs-lookup"><span data-stu-id="fa62a-155">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="fa62a-156">Azure kullanım tabanlı abonelikleri kullanma</span><span class="sxs-lookup"><span data-stu-id="fa62a-156">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="fa62a-157">Azure, Office 365 CSP abonelikleri'nden farklı olarak kullanım tabanlı CSP aboneliklerini el ile geçirmeniz gerekmez.</span><span class="sxs-lookup"><span data-stu-id="fa62a-157">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="fa62a-158">Microsoft Azure Desteği, Azure aboneliklerini ve dağıtılan tüm hizmetleri veya kaynakları **CSP** kurumsal bayi hesaplarından **CSP** kurumsal bayi hesabına geçişten geçirir.</span><span class="sxs-lookup"><span data-stu-id="fa62a-158">Microsoft Azure Support will migrate the Azure subscriptions and all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="fa62a-159">Bu geçiş sırasında müşteriye hizmet kesintisi yaşanmaz.</span><span class="sxs-lookup"><span data-stu-id="fa62a-159">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="fa62a-160">Azure aboneliklerini geçirecek olan müşteri hesaplarının yeni CSP hesabına geçiş ile ilişkilendirilecek **sözleşmeyi kabul etmelerini** sağlar.</span><span class="sxs-lookup"><span data-stu-id="fa62a-160">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="fa62a-161">Microsoft'a hangi müşteri hesaplarının geçişe hazır olduğunu bildirecek ve bu müşterinin şirket adlarını sağlayacaksınız.</span><span class="sxs-lookup"><span data-stu-id="fa62a-161">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="fa62a-162">Microsoft, Azure kullanım tabanlı abonelikleri geçirir ve geçiş tamamlandığında size bilgi sağlar.</span><span class="sxs-lookup"><span data-stu-id="fa62a-162">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="fa62a-163">CSP satıcısı hesabından geçiş altında olan Azure **aboneliğinin, Iş** Ortağı Merkezi 'nde müşteri abonelikleri bölümünde **askıya alındı** olarak işaretlendiğinden emin olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="fa62a-163">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="fa62a-164">CSP satıcısı hesabına **geçilen** Azure aboneliğinin, artık müşteri abonelikleri bölümünde Iş Ortağı Merkezi 'nde **etkin** durumunu gösterdiğini doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="fa62a-164">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="fa62a-165">Müşterinin altındaki abonelikleri devre dışı bırakmak, müşterinin görünüşünü müşteriler listesinde değiştirmez.</span><span class="sxs-lookup"><span data-stu-id="fa62a-165">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="fa62a-166">Şu anda listedeki müşterileri kaldırma seçeneği yoktur.</span><span class="sxs-lookup"><span data-stu-id="fa62a-166">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="fa62a-167">İş **ortakları, gelecekteki hesaptan gelen** geçiş aşamasından bu müşterilere abonelikleri geri eklemektan kaçınmalıdır.</span><span class="sxs-lookup"><span data-stu-id="fa62a-167">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="fa62a-168">Hesap (ler) **den** geçiş için gelecekteki ücretleri durdurmak üzere tüm müşterileriniz kapsamındaki tüm abonelikler için bu adımları yineleyin.</span><span class="sxs-lookup"><span data-stu-id="fa62a-168">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="fa62a-169">İş ortağı, İptalin günü ile fatura döneminin son günü arasındaki kullanılmamış gün sayısı için krediyle birlikte bir son fatura alacaktır.</span><span class="sxs-lookup"><span data-stu-id="fa62a-169">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="fa62a-170">Son fatura döneminden sonra gelecek fatura üretilecektir.</span><span class="sxs-lookup"><span data-stu-id="fa62a-170">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="fa62a-171">Ek bilgiler</span><span class="sxs-lookup"><span data-stu-id="fa62a-171">Additional information</span></span>

- <span data-ttu-id="fa62a-172">Aboneliği devre dışı bırakmadan önce, CSP hesabından **geçilen** aboneliğin devre dışı bırakılması, **hizmetin CSP hesabından** sağlandığı sürece son müşterinin hizmetini etkilemez.</span><span class="sxs-lookup"><span data-stu-id="fa62a-172">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="fa62a-173">Abonelikler müşteri tarafından kullanılamaz ve askıya alındığında veya iptal edildiğinde ücret üretmez.</span><span class="sxs-lookup"><span data-stu-id="fa62a-173">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="fa62a-174">Şu anda **müşteriler** listesinden bir müşteriyi tamamen kaldırmanın bir yolu yoktur.</span><span class="sxs-lookup"><span data-stu-id="fa62a-174">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="fa62a-175">İş ortakları, iş ortağı merkezi 'nde iş ortağı kiracı hesabından **alınan** abonelikleri askıya almalıdır. bu abonelikler, Çift faturalandırma işleminin gerçekleşmemesini sağlamak **için hesap geçişi** altında hesaba geçirilir ve ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="fa62a-175">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="fa62a-176">Microsoft, **aboneliklerden** askıya alma işleminin askıya alınma durumuna doğru ayarlamamasından kaynaklanan herhangi bir çakışma nedeniyle kredilerin isteklerini desteklemez.</span><span class="sxs-lookup"><span data-stu-id="fa62a-176">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="fa62a-177">Dışarı aktarma kullanarak geçişi basitleştirme</span><span class="sxs-lookup"><span data-stu-id="fa62a-177">Simplify migration using Export</span></span>

<span data-ttu-id="fa62a-178">Dışarı **Aktarma İşlevini** kullanarak, yeni birleştirilmiş yapıda kullanmak için ihtiyacınız olan abonelikleri yakaabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="fa62a-178">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="fa62a-179">Müşterilerin **listesini** İş Ortağı Merkezi için İş Ortağı Merkezi'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="fa62a-179">Select **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="fa62a-180">İstediğiniz müşteri adını açın.</span><span class="sxs-lookup"><span data-stu-id="fa62a-180">Open the desired customer name.</span></span>

3. <span data-ttu-id="fa62a-181">Abonelikler **sayfasında Abonelikleri** Dışarı **Aktar'ı** seçerek aboneliklerin ayrıntılarını bir Excel dosyasına aktarın.</span><span class="sxs-lookup"><span data-stu-id="fa62a-181">On the **Subscriptions** page, select **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="fa62a-182">Yeni birleştirilmiş kiracınıza abonelikleri yeniden oluşturmak için bu listeyi kullanın.</span><span class="sxs-lookup"><span data-stu-id="fa62a-182">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="fa62a-183">API kaydı</span><span class="sxs-lookup"><span data-stu-id="fa62a-183">API registration</span></span>

<span data-ttu-id="fa62a-184">API kaydı hakkında daha fazla bilgi için [bkz. Api erişimini İş Ortağı Merkezi.](/partner-center/develop/set-up-api-access-in-partner-center)</span><span class="sxs-lookup"><span data-stu-id="fa62a-184">For more information about API registration, see [Set up API access in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span></span>

## <a name="next-steps"></a><span data-ttu-id="fa62a-185">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="fa62a-185">Next steps</span></span>

- [<span data-ttu-id="fa62a-186">Bulut Çözümü Sağlayıcısı CSP tekliflerini satarak bölgesel pazarları ve para birimlerini programla</span><span class="sxs-lookup"><span data-stu-id="fa62a-186">Cloud Solution Provider program regional markets and currencies where you can sell CSP offers</span></span>](regional-authorization-overview.md)
