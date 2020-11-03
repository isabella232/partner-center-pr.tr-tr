---
title: CSP bölgesel yetkilendirme kiracı birleştirmesi
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Farklı ülkeler/bölgeler için kiracılar birleştirmek üzere bu yönergeleri kullanın. Bu, müşteri hesaplarını ve müşteri aboneliklerini geçirmeye yönelik adımları içerir.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 0ae107c005eaf6b8ff8a6d99a91075ebc560cf81
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/13/2020
ms.locfileid: "92531854"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="f783d-104">CSP bölgesel yetkilendirme kiracı birleştirme yönergeleri</span><span class="sxs-lookup"><span data-stu-id="f783d-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="f783d-105">**Uygulama hedefi**</span><span class="sxs-lookup"><span data-stu-id="f783d-105">**Applies to**</span></span>

-  <span data-ttu-id="f783d-106">İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="f783d-106">Partner Center</span></span>
-  <span data-ttu-id="f783d-107">ABD kamu için Microsoft Bulut iş ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="f783d-107">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="f783d-108">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="f783d-108">**Appropriate roles**</span></span>

- <span data-ttu-id="f783d-109">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="f783d-109">Global admin</span></span>
- <span data-ttu-id="f783d-110">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="f783d-110">Admin agent</span></span>

<span data-ttu-id="f783d-111">\[Bazı bilgiler, ticari olarak yayınlanmadan önce önemli ölçüde değiştirilebilecek, önceden yayınlanan ürünle ilgilidir.</span><span class="sxs-lookup"><span data-stu-id="f783d-111">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="f783d-112">Burada verilen bilgilerle ilgili olarak Microsoft açık veya zımni hiçbir garanti vermez.\]</span><span class="sxs-lookup"><span data-stu-id="f783d-112">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="f783d-113">İş için kiracılar birleştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f783d-113">You can consolidate tenants for your business.</span></span> <span data-ttu-id="f783d-114">Farklı ülkeler/bölgeler için kiracılar birleştirmek üzere bu yönergeleri kullanın.</span><span class="sxs-lookup"><span data-stu-id="f783d-114">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="f783d-115">Geçiş yaptığınız hesapta müşterilerinizin her biri için sağlanan aboneliklerin ve lisans sayılarının tümünün farkında olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="f783d-115">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="f783d-116">Geçiş işleminin bir parçası olarak, yeni merkezi CSP hesabı altında aynı lisans sayılarıyla aynı tam abonelikleri yeniden hazırlayacaksınız.</span><span class="sxs-lookup"><span data-stu-id="f783d-116">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="f783d-117">Merkezi kiracıya geçiş yapılacak müşterilerin bir listesini oluşturmaya yardımcı olması için listeyi dışarı aktar özelliğini kullanın.</span><span class="sxs-lookup"><span data-stu-id="f783d-117">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="f783d-118">Birleştirme işlemi tamamlandıktan sonra önceki kiracı durumuna geri döndüremezsiniz.</span><span class="sxs-lookup"><span data-stu-id="f783d-118">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="f783d-119">Müşteri eylemi de gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="f783d-119">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="f783d-120">Geçiş için hazırlanma</span><span class="sxs-lookup"><span data-stu-id="f783d-120">Prepare for migration</span></span>

- <span data-ttu-id="f783d-121">Geçiş **hesabını (** yeni hesaba geçigeçiizin) kullanarak **iş ortağı merkezi** 'nde oturum açın ve tüm müşterileri ve bu müşteriler için sağlanan tüm hizmetleri gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="f783d-121">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="f783d-122">Bu hesabın oturumunu kapatın.</span><span class="sxs-lookup"><span data-stu-id="f783d-122">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="f783d-123">Müşteri hesaplarını geçirme</span><span class="sxs-lookup"><span data-stu-id="f783d-123">Migrate customer accounts</span></span>

1. <span data-ttu-id="f783d-124">Geçiş (yeni) hesabıyla **Iş Ortağı Merkezi**  'nde oturum **açın (müşterileri** geçiş yaptığınız bir hesap).</span><span class="sxs-lookup"><span data-stu-id="f783d-124">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="f783d-125">**Müşteriler** ’i seçin.</span><span class="sxs-lookup"><span data-stu-id="f783d-125">Select **Customers** .</span></span>

3. <span data-ttu-id="f783d-126">**Satıcı Ilişkisi iste** ' ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="f783d-126">Click **Request a reseller relationship** .</span></span> <span data-ttu-id="f783d-127">Müşterilerinize göndermek için varsayılan bir e-posta iletisi sunulur.</span><span class="sxs-lookup"><span data-stu-id="f783d-127">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="f783d-128">Bu ileti, yeni Iş Ortağı Merkezi hesabınıza özel kuruluş KIMLIĞINE sahip bir URL içerir.</span><span class="sxs-lookup"><span data-stu-id="f783d-128">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="f783d-129">**Müşteri eylemi:** Geçirmek istediğiniz her bir etkin müşterilerin bu URL 'YI ziyaret etmesini sağlayın.</span><span class="sxs-lookup"><span data-stu-id="f783d-129">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="f783d-130">URL 'YI açarken, müşterinin Office 365 portalında oturum açması istenir.</span><span class="sxs-lookup"><span data-stu-id="f783d-130">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="f783d-131">Müşteri, Azure ve Office 365 yönetim portallarına erişmek için kullandıkları aynı kuruluş KIMLIĞINI kullanarak oturum açar.</span><span class="sxs-lookup"><span data-stu-id="f783d-131">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="f783d-132">Oturum açtıktan sonra, **müşteri hesabına** ait genel YÖNETICININ yeni CSP hesabına yönetici ayrıcalıkları sağlayan bir anlaşma göndermesi istenir.</span><span class="sxs-lookup"><span data-stu-id="f783d-132">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="f783d-133">Kabul ederse, müşteri onay kutusunu seçer ve ilişkiye izin vermeyi kabul eder.</span><span class="sxs-lookup"><span data-stu-id="f783d-133">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="f783d-134">Müşteriler, sözleşmeyi gönderdikten sonra iş ortağının müşteri listesinde görünür.</span><span class="sxs-lookup"><span data-stu-id="f783d-134">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="f783d-135">Office 365 ve Azure olmayan kullanım tabanlı abonelikleri geçirme</span><span class="sxs-lookup"><span data-stu-id="f783d-135">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="f783d-136">Müşterinizin Sözleşmesi imzalandıktan sonra, kendi aboneliklerini merkezi Iş ortağı kiracınız altında yeniden oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f783d-136">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="f783d-137">**Iş Ortağı Merkezi** 'nden **müşteriler** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="f783d-137">From **Partner Center** select **Customers** .</span></span>

3. <span data-ttu-id="f783d-138">Geçirmek istediğiniz müşterinin şirket adını açın.</span><span class="sxs-lookup"><span data-stu-id="f783d-138">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="f783d-139">**Abonelik Ekle** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="f783d-139">Select **Add subscription** .</span></span>

5. <span data-ttu-id="f783d-140">Katalogdan doğru abonelikleri ve lisans sayılarını ekleyin.</span><span class="sxs-lookup"><span data-stu-id="f783d-140">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="f783d-141">**İş ortağı** hesaplarından geçiş sırasında belirtilen bilgilerle doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="f783d-141">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="Müşteri listesi":::

6. <span data-ttu-id="f783d-143">Gönder ' e tıklayın **.**</span><span class="sxs-lookup"><span data-stu-id="f783d-143">Click **Submit.**</span></span>

   <span data-ttu-id="f783d-144">Hizmetler artık **müşteriye iş ortağı** hesabına geçiş üzerinden sağlanır.</span><span class="sxs-lookup"><span data-stu-id="f783d-144">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="f783d-145">Tüm ek müşterilerin aboneliklerini geçirmek için bu adımları tekrarlayın.</span><span class="sxs-lookup"><span data-stu-id="f783d-145">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="f783d-146">Bir sonraki bölüme geçmeden önce **, iş ortağı** hesaplarından geçiş altında bulunan tüm müşteri aboneliklerinin **iş ortağı hesabına** geçiş altında yeniden sağlandığını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="f783d-146">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="f783d-147">İş ortakları, iş ortağı Merkezi **'nde iş ortağı** kiracı hesabından geçiş sırasında abonelikleri askıya almalıdır. bu abonelikler, Çift faturalandırma işleminin gerçekleşmemesini sağlamak için Iş Ortağı Merkezi 'nde **iş ortağı kiracı** hesabı altına geçirilir ve ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="f783d-147">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="f783d-148">Aboneliklerden geçiş işleminin doğru şekilde devre dışı bırakılmasından kaynaklanan bir çakışma nedeniyle, destek istekleri krediler için **Transitioning From** reddedilir.</span><span class="sxs-lookup"><span data-stu-id="f783d-148">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="f783d-149">İş ortağı hesabından geçilen Office 365 aboneliklerini devre dışı bırakma</span><span class="sxs-lookup"><span data-stu-id="f783d-149">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="f783d-150">**İş ortağı** hesaplarından GEÇIŞ altında CSP aboneliğini devre dışı bırakmak gelecekteki faturalandırmayı durduruyor.</span><span class="sxs-lookup"><span data-stu-id="f783d-150">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="f783d-151">Azure abonelikleri, geçiş işlemi sırasında otomatik olarak devre dışı bırakıldığından Azure aboneliklerini el ile devre dışı bırakmanız gerekmez.</span><span class="sxs-lookup"><span data-stu-id="f783d-151">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="f783d-152">**CSP hesabından** geçiş yaparken **iş ortağı merkezi** ' nde oturum açın ve müşteri listesine gidin.</span><span class="sxs-lookup"><span data-stu-id="f783d-152">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="f783d-153">Devre dışı bırakmak için abonelikleri olan müşteriyi açın ve ardından devre dışı bırakılacak ilk teklifi seçin.</span><span class="sxs-lookup"><span data-stu-id="f783d-153">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="f783d-154">Aboneliği **askıya alındı** olarak ayarlayın ve ardından **Gönder** ' e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="f783d-154">Set the subscription to **suspended** , and then click **submit** .</span></span>

   >[!Note]
   ><span data-ttu-id="f783d-155">Aboneliğin askıya alınması, iki faturalandırma gerçekleşmemesini sağlar.</span><span class="sxs-lookup"><span data-stu-id="f783d-155">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="f783d-156">Abonelik, abonelikler listesinde **askıya alındı** olarak gösterilir.</span><span class="sxs-lookup"><span data-stu-id="f783d-156">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="f783d-157">Müşterinin altındaki tüm abonelikler için bu adımları tekrarlayın.</span><span class="sxs-lookup"><span data-stu-id="f783d-157">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="f783d-158">Tüm Show askıda olduğunu doğrulayın **.**</span><span class="sxs-lookup"><span data-stu-id="f783d-158">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="f783d-159">Listede bir sonraki müşteriyi seçin ve tüm abonelikleri devre dışı bırakma işlemini tekrarlayın.</span><span class="sxs-lookup"><span data-stu-id="f783d-159">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="f783d-160">Azure kullanım tabanlı abonelikleri geçirme</span><span class="sxs-lookup"><span data-stu-id="f783d-160">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="f783d-161">Office 365 CSP aboneliklerinden farklı olarak, Azure, kullanım tabanlı CSP aboneliklerinin el ile geçirilmesi gerekmez.</span><span class="sxs-lookup"><span data-stu-id="f783d-161">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="f783d-162">Microsoft Azure desteği, Azure aboneliklerini, ayrıca CSP satıcı hesaplarından **alınan** tüm hizmet veya kaynakları **, CSP satıcısı** hesabına geçiş yapmak için geçirilecek.</span><span class="sxs-lookup"><span data-stu-id="f783d-162">Microsoft Azure Support will migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="f783d-163">Bu geçiş sırasında müşteriye hizmet kesintisi olmaz.</span><span class="sxs-lookup"><span data-stu-id="f783d-163">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="f783d-164">Azure abonelikleri 'nin geçirileceği müşteri hesaplarının, yeni CSP hesabına **geçme** ile ilişkilendirilecek anlaşmayı kabul ettiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="f783d-164">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="f783d-165">Microsoft 'un hangi müşteri hesaplarının geçirmeye hazırlanmaya yönelik olduğunu bilgilendirirsiniz ve bu müşterinin şirket adlarını sağlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f783d-165">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="f783d-166">Microsoft, Azure kullanım tabanlı abonelikleri geçirir ve geçiş tamamlandığında size bildirir.</span><span class="sxs-lookup"><span data-stu-id="f783d-166">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="f783d-167">CSP satıcısı hesabından geçiş altında olan Azure **aboneliğinin, Iş** Ortağı Merkezi 'nde müşteri abonelikleri bölümünde **askıya alındı** olarak işaretlendiğinden emin olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="f783d-167">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="f783d-168">CSP satıcısı hesabına **geçilen** Azure aboneliğinin, artık müşteri abonelikleri bölümünde Iş Ortağı Merkezi 'nde **etkin** durumunu gösterdiğini doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="f783d-168">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="f783d-169">Müşterinin altındaki abonelikleri devre dışı bırakmak, müşterinin görünüşünü müşteriler listesinde değiştirmez.</span><span class="sxs-lookup"><span data-stu-id="f783d-169">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="f783d-170">Şu anda listedeki müşterileri kaldırma seçeneği yoktur.</span><span class="sxs-lookup"><span data-stu-id="f783d-170">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="f783d-171">İş **ortakları, gelecekteki hesaptan gelen** geçiş aşamasından bu müşterilere abonelikleri geri eklemektan kaçınmalıdır.</span><span class="sxs-lookup"><span data-stu-id="f783d-171">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="f783d-172">Hesap (ler) **den** geçiş için gelecekteki ücretleri durdurmak üzere tüm müşterileriniz kapsamındaki tüm abonelikler için bu adımları yineleyin.</span><span class="sxs-lookup"><span data-stu-id="f783d-172">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="f783d-173">İş ortağı, İptalin günü ile fatura döneminin son günü arasındaki kullanılmamış gün sayısı için krediyle birlikte bir son fatura alacaktır.</span><span class="sxs-lookup"><span data-stu-id="f783d-173">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="f783d-174">Son fatura döneminden sonra gelecek fatura üretilecektir.</span><span class="sxs-lookup"><span data-stu-id="f783d-174">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="f783d-175">Ek bilgiler</span><span class="sxs-lookup"><span data-stu-id="f783d-175">Additional information</span></span>

- <span data-ttu-id="f783d-176">Aboneliği devre dışı bırakmadan önce, CSP hesabından **geçilen** aboneliğin devre dışı bırakılması, **hizmetin CSP hesabından** sağlandığı sürece son müşterinin hizmetini etkilemez.</span><span class="sxs-lookup"><span data-stu-id="f783d-176">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="f783d-177">Abonelikler müşteri tarafından kullanılamaz ve askıya alındığında veya iptal edildiğinde ücret üretmez.</span><span class="sxs-lookup"><span data-stu-id="f783d-177">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="f783d-178">Şu anda **müşteriler** listesinden bir müşteriyi tamamen kaldırmanın bir yolu yoktur.</span><span class="sxs-lookup"><span data-stu-id="f783d-178">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="f783d-179">İş ortakları, iş ortağı merkezi 'nde iş ortağı kiracı hesabından **alınan** abonelikleri askıya almalıdır. bu abonelikler, Çift faturalandırma işleminin gerçekleşmemesini sağlamak **için hesap geçişi** altında hesaba geçirilir ve ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="f783d-179">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="f783d-180">Microsoft, **aboneliklerden** askıya alma işleminin askıya alınma durumuna doğru ayarlamamasından kaynaklanan herhangi bir çakışma nedeniyle kredilerin isteklerini desteklemez.</span><span class="sxs-lookup"><span data-stu-id="f783d-180">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="f783d-181">Dışarı aktarma kullanarak geçişi basitleştirme</span><span class="sxs-lookup"><span data-stu-id="f783d-181">Simplify migration using Export</span></span>

<span data-ttu-id="f783d-182">**Dışarı aktarma işlevini** kullanarak, yeni birleştirilmiş yapınıza kullanmanız gereken abonelikleri yakalayabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="f783d-182">Using the **Export Function** , you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="f783d-183">Müşterilerin listesini görmek için Iş Ortağı Merkezi ' nde **müşteriler** ' e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="f783d-183">Click **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="f783d-184">İstenen müşteri adını açın.</span><span class="sxs-lookup"><span data-stu-id="f783d-184">Open the desired customer name.</span></span>

3. <span data-ttu-id="f783d-185">**Abonelikler sayfasında,** aboneliklerin ayrıntılarını bir Excel dosyasına dışarı aktarmak Için **abonelikleri dışarı aktar** ' a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="f783d-185">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="f783d-186">Yeni birleştirilmiş kiracınızdaki abonelikleri yeniden oluşturmak için bu listeyi kullanın.</span><span class="sxs-lookup"><span data-stu-id="f783d-186">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="f783d-187">API kaydı</span><span class="sxs-lookup"><span data-stu-id="f783d-187">API registration</span></span>

<span data-ttu-id="f783d-188">API kaydı hakkında daha fazla bilgi için bkz. [Iş Ortağı Merkezi 'NDE API erişimi ayarlama](/partner-center/develop/set-up-api-access-in-partner-center).</span><span class="sxs-lookup"><span data-stu-id="f783d-188">For more information about API registration, see [Set up API access in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span></span>

## <a name="next-steps"></a><span data-ttu-id="f783d-189">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="f783d-189">Next steps</span></span>

- [<span data-ttu-id="f783d-190">CSP teklifleri oluşturabileceğiniz bulut çözümü sağlayıcısı program bölgesel pazarlar ve para birimleri</span><span class="sxs-lookup"><span data-stu-id="f783d-190">Cloud Solution Provider program regional markets and currencies where you can sell CSP offers</span></span>](regional-authorization-overview.md)
