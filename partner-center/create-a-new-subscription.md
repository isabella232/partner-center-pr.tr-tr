---
title: Iş Ortağı Merkezi 'nde müşteri abonelikleri oluşturma
ms.topic: how-to
ms.date: 05/17/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft tarafından yayımlanan ürünlerin yanı sıra üçüncü taraf ISV 'Ler tarafından yayımlanan SaaS ürünleri için müşterilerinize abonelik satma hakkında bilgi edinin.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 3269fa994d704c0a0dae067087bad8589a7ce031
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148218"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="dc09c-103">Müşteri aboneliklerini oluşturma, askıya alma veya iptal etme</span><span class="sxs-lookup"><span data-stu-id="dc09c-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="dc09c-104">**Uygulama hedefi**: Iş Ortağı Merkezi | ABD kamu için Microsoft Bulut iş ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="dc09c-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="dc09c-105">**Uygun roller**: yönetici Aracısı | Faturalandırma Yöneticisi | Genel yönetici | Yardım Masası Aracısı | Satış Aracısı</span><span class="sxs-lookup"><span data-stu-id="dc09c-105">**Appropriate roles**: Admin agent | Billing admin | Global admin | Helpdesk agent | Sales agent</span></span>

<span data-ttu-id="dc09c-106">Iş Ortağı Merkezi 'nde müşterinizin bir kaydını oluşturduktan sonra, bu abonelikleri katalogdaki ürünlere satabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="dc09c-106">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="dc09c-107">Bu, üçüncü taraf bağımsız yazılım satıcıları (ISV 'Ler) tarafından [ticari Market](https://azuremarketplace.microsoft.com/marketplace)'e yayımlanan Microsoft ve hizmet olarak yazılım (SaaS) ürünleri tarafından yayımlanan ürünleri içerir.</span><span class="sxs-lookup"><span data-stu-id="dc09c-107">This includes products published by Microsoft and Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="dc09c-108">Bazı teklifler müşteri başına bir abonelikle sınırlıdır.</span><span class="sxs-lookup"><span data-stu-id="dc09c-108">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="dc09c-109">Hangi tekliflerin kısıtlı olduğunu görmek için Iş Ortağı Merkezi fiyatlandırma ve teklifleri sayfasını ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="dc09c-109">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="dc09c-110">CSP programındaki bir iş ortağı olarak, Iş Ortağı Merkezi 'nde ISV yayımcılarından **Lisans tabanlı** veya **ölçülen** SaaS abonelikleri satın alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="dc09c-110">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="dc09c-111">Bu, tüm **Lisans tabanlı** veya **tarifeli** SaaS tekliflerini, erişiminiz olan [özel TEKLIFLER](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) de dahil olmak üzere ISV yayımcısı kullanımınıza sunabileceğiniz anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="dc09c-111">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="dc09c-112">ISV 'lerden diğer, ticari Market tekliflerini satın almak veya yönetmek için (Azure uygulamaları, kapsayıcılar veya VM 'Leri içeren Kullanım tabanlı teklifler gibi) [Azure Portal](https://portal.azure.com/)gitmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="dc09c-112">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="dc09c-113">Yeni abonelik oluştur</span><span class="sxs-lookup"><span data-stu-id="dc09c-113">Create a new subscription</span></span>

1. <span data-ttu-id="dc09c-114">[İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="dc09c-114">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="dc09c-115">Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve listeden bir müşteri seçin.</span><span class="sxs-lookup"><span data-stu-id="dc09c-115">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="dc09c-116">**Abonelik Ekle**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="dc09c-116">Select **Add subscription**.</span></span> <span data-ttu-id="dc09c-117">**Çevrimiçi hizmetler** sekmesinde, tüm kullanılabilir Market SaaS teklifleri gösterilir.</span><span class="sxs-lookup"><span data-stu-id="dc09c-117">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="dc09c-118">Yalnızca belirli abonelik türlerini görmek için, kullanılabilir filtrelerdeki seçimleri yapın:</span><span class="sxs-lookup"><span data-stu-id="dc09c-118">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="dc09c-119">**Yayımcı**: ISV 'ler tarafından yayımlanan ticari Market ürünlerini görmek Için yalnızca Microsoft 'un veya **iş ortağının** tekliflerini görmek üzere **Microsoft** 'u seçin.</span><span class="sxs-lookup"><span data-stu-id="dc09c-119">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="dc09c-120">**Faturalandırma türü**: kullanmak istediğiniz abonelik faturalandırması türünü seçin: **Lisans** veya **kullanım**.</span><span class="sxs-lookup"><span data-stu-id="dc09c-120">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="dc09c-121">Aylık [ve yıllık faturalama sıklığı](license-based-billing.md) arasında karar alamanıza yardımcı olacak bilgiler için bkz. Lisans tabanlı faturalama.</span><span class="sxs-lookup"><span data-stu-id="dc09c-121">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="dc09c-122">**Kategori:** Kurumsal, **Küçük** **işletme veya** Deneme'yi **seçin.**</span><span class="sxs-lookup"><span data-stu-id="dc09c-122">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="dc09c-123">Deneme abonelikleri hakkında bilgi için [bkz. Müşterilerinize Microsoft ürünlerinin denemelerini teklif edin.](offer-your-customers-trials-of-microsoft-products.md)</span><span class="sxs-lookup"><span data-stu-id="dc09c-123">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="dc09c-124">Müşteriniz için satın almak istediğiniz ürün aboneliklerini seçin.</span><span class="sxs-lookup"><span data-stu-id="dc09c-124">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="dc09c-125">Gördüğünüz ürünler, müşteri segmenti türüne (eğitim, kamu vb.) ve sizin uyguladık filtrelere bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="dc09c-125">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="dc09c-126">Market'te gösterilen bazı teklifler belirli bir müşteri veya belirli bir CSP iş ortağı tarafından her zaman kullanılabilir olabilir.</span><span class="sxs-lookup"><span data-stu-id="dc09c-126">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="dc09c-127">Bunun nedeni:</span><span class="sxs-lookup"><span data-stu-id="dc09c-127">This can be because:</span></span>

   - <span data-ttu-id="dc09c-128">Müşterinin zaten bu ürüne bir aboneliği vardır ve yalnızca bir ürüne izin verilir</span><span class="sxs-lookup"><span data-stu-id="dc09c-128">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="dc09c-129">Müşterinin aboneliği askıya alınmış olabilir (Bu durumda yeni bir abonelik satın almak yerine aboneliği yeniden etkinleştirebilirsiniz.)</span><span class="sxs-lookup"><span data-stu-id="dc09c-129">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="dc09c-130">ISV SaaS tekliflerinin satın alınamama nedenlerinden birkaçı olabilir: ISV müşterinin fatura ülkesi veya bölgesi için destek sunmayabiliyor olabilir; ISV, teklifi CSP programı aracılığıyla kullanılabilir halememiş olabilir; veya ISV teklifi yalnızca belirli CSP [iş](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) ortaklarına özel yapmış olabilir.</span><span class="sxs-lookup"><span data-stu-id="dc09c-130">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="dc09c-131">ISV teklifi, kapsayıcılar veya kullanım tabanlı İş Ortağı Merkezi gibi) aracılığıyla işlem gerçekleştirilebilir de değildir.</span><span class="sxs-lookup"><span data-stu-id="dc09c-131">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="dc09c-132">Eklemek istediğiniz her abonelik için lisans sayısını girin (gerekirse) ve Sepete **ekle'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="dc09c-132">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="dc09c-133">Abonelik eklemeyi bitirdikten sonra Siparişinizi gözden **geçir'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="dc09c-133">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="dc09c-134">Siparişlerinizi gözden geçirerek bu abonelikleri satın almaya hazır olduktan sonra Satın Al'ı **seçin.**</span><span class="sxs-lookup"><span data-stu-id="dc09c-134">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="dc09c-135">Bir müşteri için abonelik satın alırsınız, aşağıdakiler gerçekleşir:</span><span class="sxs-lookup"><span data-stu-id="dc09c-135">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="dc09c-136">Müşterinin Abonelikler sayfasından abonelik adını seçerek aboneliği gözden geçirebilirsiniz veya **düzenleyebilirsiniz.**</span><span class="sxs-lookup"><span data-stu-id="dc09c-136">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="dc09c-137">Buradan, varsa eklenti lisanslarını seçin, lisans miktarını değiştirebilir veya aboneliği askıya alın.</span><span class="sxs-lookup"><span data-stu-id="dc09c-137">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="dc09c-138">**ISV SaaS (lisans tabanlı ve tarifeli) abonelikler için:**</span><span class="sxs-lookup"><span data-stu-id="dc09c-138">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="dc09c-139">ISV yayımcısının sitesine bir bağlantı alacaksınız.</span><span class="sxs-lookup"><span data-stu-id="dc09c-139">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="dc09c-140">Bu bağlantı, müşterinin aboneliğine ait dağıtım veya hesap kurulumunu tamamlamanıza yardımcı olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="dc09c-140">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="dc09c-141">Ne siz ne de müşteriniz bu tür ISV aboneliği için kurulumu/sağlamayı tamamlamaya yönelik yönergeleri içeren bir e-posta alacaksınız.)</span><span class="sxs-lookup"><span data-stu-id="dc09c-141">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="dc09c-142">Aboneliğiniz 30 günlük ücretsiz deneme sürümü ile birlikte geliyorsa, ücretsiz deneme süresi otomatik olarak uygulanır.</span><span class="sxs-lookup"><span data-stu-id="dc09c-142">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="dc09c-143">CSP programındaki bir iş ortağı olarak, müşteriler için satın aldığınız tekliflerle ilgili ücretsiz deneme süresini beklenemez.</span><span class="sxs-lookup"><span data-stu-id="dc09c-143">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="dc09c-144">Ücretsiz deneme süresi sona erdiğinde, abonelik dönemi başlar ve abonelik, ücretli duruma dönüştürülür.</span><span class="sxs-lookup"><span data-stu-id="dc09c-144">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="dc09c-145">Abonelik daha sonra aynı zamanlamaya göre otomatik olarak yenilenecek.</span><span class="sxs-lookup"><span data-stu-id="dc09c-145">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="dc09c-146">Eklentilerle abonelikleri güncelleştirme</span><span class="sxs-lookup"><span data-stu-id="dc09c-146">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="dc09c-147">Bir eklenti satın almak için müşterinin öncelikle etkin bir temel aboneliği olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="dc09c-147">To purchase an add-on, the customer must first have an active base subscription.</span></span>  <span data-ttu-id="dc09c-148">Eklentileri katalog aracılığıyla satın alamazsınız.</span><span class="sxs-lookup"><span data-stu-id="dc09c-148">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="dc09c-149">Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="dc09c-149">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="dc09c-150">Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve listeden bir müşteri seçin.</span><span class="sxs-lookup"><span data-stu-id="dc09c-150">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="dc09c-151">Yönetmek istediğiniz aboneliği seçin.</span><span class="sxs-lookup"><span data-stu-id="dc09c-151">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="dc09c-152">**Durum** bölümünün altında, abonelik Için kullanılabilen eklentilerin bir listesi bulunur.</span><span class="sxs-lookup"><span data-stu-id="dc09c-152">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="dc09c-153">Gerekli her eklenti için lisans miktarını güncelleştirin.</span><span class="sxs-lookup"><span data-stu-id="dc09c-153">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="dc09c-154">Sonra **Gönder** ile yaptığınız değişiklikleri gönderin.</span><span class="sxs-lookup"><span data-stu-id="dc09c-154">Then **Submit** your changes.</span></span>

<span data-ttu-id="dc09c-155">Iş Ortağı Merkezi aracılığıyla eklenti satın alma özelliği yalnızca doğrudan fatura ve dolaylı sağlayıcılar için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="dc09c-155">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="dc09c-156">Temel gereksinimlere ve bölgesel kullanılabilirliğe göre yalnızca uygun eklentiler görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="dc09c-156">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="dc09c-157">Fiyatlandırma ve teklifler hakkında daha fazla bilgi için bkz. Cloud Bayi teklif matrisi.</span><span class="sxs-lookup"><span data-stu-id="dc09c-157">For more information about pricing and offers, refer to the Cloud Reseller offer matrix.</span></span> <span data-ttu-id="dc09c-158">Temel abonelik askıya alındığında ilişkili tüm eklentiler de askıya alınır.</span><span class="sxs-lookup"><span data-stu-id="dc09c-158">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="dc09c-159">Eklentilerin başlangıç tarihleri temel abonelikle uyumludur; ücretler Ücret başlangıç tarihi ile Ücret bitiş tarihi kullanılarak hesaplanır ve ilk faturaya orantılı bir ücret uygulanır.</span><span class="sxs-lookup"><span data-stu-id="dc09c-159">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="dc09c-160">Daha fazla bilgi için bkz. [Lisans tabanlı faturalandırma](license-based-billing.md).</span><span class="sxs-lookup"><span data-stu-id="dc09c-160">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="dc09c-161">Aboneliği askıya alma veya iptal etme</span><span class="sxs-lookup"><span data-stu-id="dc09c-161">Suspend or cancel a subscription</span></span>

<span data-ttu-id="dc09c-162">İş ortakları, müşteri tarafından isteniyorsa veya ödeme veya sahtekarlık durumlarında bir aboneliği askıya alabilir veya iptal edebilir.</span><span class="sxs-lookup"><span data-stu-id="dc09c-162">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="dc09c-163">Bir aboneliği askıya alma</span><span class="sxs-lookup"><span data-stu-id="dc09c-163">Suspend a subscription</span></span>

<span data-ttu-id="dc09c-164">Aboneliğin durumunu **askıya alındı** olarak değiştirdiğinizde, kullanıcılar oturum açamaz veya hizmetlere erişemez.</span><span class="sxs-lookup"><span data-stu-id="dc09c-164">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="dc09c-165">İş Ortağı Merkezi [oturum açın.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="dc09c-165">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="dc09c-166">Yeni İş Ortağı Merkezi **Müşteriler'i** ve ardından listeden bir müşteri seçin.</span><span class="sxs-lookup"><span data-stu-id="dc09c-166">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="dc09c-167">Yönetmek istediğiniz aboneliği seçin.</span><span class="sxs-lookup"><span data-stu-id="dc09c-167">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="dc09c-168">**Durum** bölümünde **Askıya Alındı**'yı seçin.</span><span class="sxs-lookup"><span data-stu-id="dc09c-168">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="dc09c-169">Sonra **Gönder** ile yaptığınız değişiklikleri gönderin.</span><span class="sxs-lookup"><span data-stu-id="dc09c-169">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="dc09c-170">Abonelik 90 gün veya 90 gün içinde yeniden etkinleştirildiği sürece tüm veriler silinir ve hesabın açılmasıyla ilk faturalama dönemi (en fazla 120 gün) arasındaki gün sayısına ek olarak bu süreye dahil olur.</span><span class="sxs-lookup"><span data-stu-id="dc09c-170">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="dc09c-171">Bir aboneliği askıya alırsanız, Askıya Alınmış düğmesinin altında gördüğünüz tarih, aboneliği yeniden etkinleştirmezsanız aboneliğin süresinin otomatik olarak ne zaman dol olacağını gösterir. </span><span class="sxs-lookup"><span data-stu-id="dc09c-171">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

>[!NOTE]
><span data-ttu-id="dc09c-172">CSP abonelikleri, hizmetlerin çalışmaya devam eder ancak abonelik herhangi bir faturalama ücreti oluşturmazken süresi dolmuş bir süreye (doğrudan web abonelikleri gibi) sahip değildir.</span><span class="sxs-lookup"><span data-stu-id="dc09c-172">CSP subscriptions don't have an expired period (the way web-direct subscriptions do) during which the services are still working but the subscription doesn't generate any billing charges.</span></span> <span data-ttu-id="dc09c-173">CSP abonelikleri etkin veya askıya alınmış (veya tamamen silinmiş).</span><span class="sxs-lookup"><span data-stu-id="dc09c-173">CSP subscriptions are either active or suspended (or fully deleted).</span></span>

### <a name="cancel-a-subscription"></a><span data-ttu-id="dc09c-174">Aboneliği iptal etme</span><span class="sxs-lookup"><span data-stu-id="dc09c-174">Cancel a subscription</span></span>

<span data-ttu-id="dc09c-175">Lisans tabanlı SaaS aboneliklerini ticari market içindeki üçüncü taraf ISV yayımcılarından İş Ortağı Merkezi [edebilirsiniz.](csp-commercial-marketplace-overview.md)</span><span class="sxs-lookup"><span data-stu-id="dc09c-175">You can cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="dc09c-176">İptal süresi içinde iptal edersiniz, tam para iadesi alırsınız.</span><span class="sxs-lookup"><span data-stu-id="dc09c-176">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="dc09c-177">Aylık olarak faturalandırılan ISV teklifleri için:</span><span class="sxs-lookup"><span data-stu-id="dc09c-177">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="dc09c-178">Siparişi verdikten 24 saatten az bir süre sonra iptal edersiniz, sonraki faturada tam kredi alırsınız.</span><span class="sxs-lookup"><span data-stu-id="dc09c-178">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="dc09c-179">Siparişi verdikten 24 saat sonra iptal edersiniz, iptal işlemi yenileme sırasında yapılacak şekilde zamanlanmış olur.</span><span class="sxs-lookup"><span data-stu-id="dc09c-179">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="dc09c-180">Yıllık olarak faturalandırılan teklifler için:</span><span class="sxs-lookup"><span data-stu-id="dc09c-180">For offers billed annually:</span></span>

- <span data-ttu-id="dc09c-181">Siparişi verdikten 14 gün sonra iptal edersiniz, sonraki faturada tam kredi alırsınız.</span><span class="sxs-lookup"><span data-stu-id="dc09c-181">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="dc09c-182">Siparişi verdikten 14 gün sonra iptal edersiniz, iptal işlemi yenileme sırasında yapılacak şekilde zamanlanmış olur.</span><span class="sxs-lookup"><span data-stu-id="dc09c-182">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="dc09c-183">Bu süreler sona erdikten sonra aboneliği iptal etme seçeneğini artık göremeyeceksiniz.</span><span class="sxs-lookup"><span data-stu-id="dc09c-183">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="dc09c-184">Kullanım tabanlı ve tarifeli, üçüncü taraf ISV hizmetleri (örneğin, sanal makineleri veya kapsayıcıları kullananlar) iade için uygun değildir.</span><span class="sxs-lookup"><span data-stu-id="dc09c-184">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="dc09c-185">Kullanım tabanlı hizmetler bir iptal yöntemi olarak kullanımdan silindi.</span><span class="sxs-lookup"><span data-stu-id="dc09c-185">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="dc09c-186">Ücretler kullanımdan sonra faturalandırılana bu hizmetler para iadesi için uygun değildir.</span><span class="sxs-lookup"><span data-stu-id="dc09c-186">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="dc09c-187">Lisans tabanlı bir SaaS aboneliğini ISV yayımcısından iptal etmek için aşağıdakileri yapın:</span><span class="sxs-lookup"><span data-stu-id="dc09c-187">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="dc09c-188">Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="dc09c-188">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="dc09c-189">Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve listeden bir müşteri seçin.</span><span class="sxs-lookup"><span data-stu-id="dc09c-189">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="dc09c-190">İptal etmek istediğiniz aboneliği bulun.</span><span class="sxs-lookup"><span data-stu-id="dc09c-190">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="dc09c-191">**Durum** sütununda **iptal**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="dc09c-191">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="dc09c-192">Sonra **Gönder** ile yaptığınız değişiklikleri gönderin.</span><span class="sxs-lookup"><span data-stu-id="dc09c-192">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="dc09c-193">Bir iletişim kutusu görüntülenirse, ilgili ayrıntıları doldurun ve **Gönder**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="dc09c-193">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="dc09c-194">İptali onaylamak için **Evet, iptal**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="dc09c-194">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="dc09c-195">Ayrıca API 'Leri kullanarak bir Azure Marketi aboneliğini iptal etmeyi seçebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="dc09c-195">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="dc09c-196">Bunu yapmak için bkz. [Azure Marketi aboneliğini Iptal etme](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span><span class="sxs-lookup"><span data-stu-id="dc09c-196">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="dc09c-197">Bir ticari Market aboneliğinin otomatik olarak yenilenip yenilenmeyeceğini seçin</span><span class="sxs-lookup"><span data-stu-id="dc09c-197">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="dc09c-198">Etkin abonelikler varsayılan olarak abonelik süresi sona erdiğinde otomatik olarak yenilenecek şekilde ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="dc09c-198">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="dc09c-199">[Ticari Market ürünlerine yönelik abonelikler](csp-commercial-marketplace-overview.md)için, isteğe bağlı olarak, aboneliği otomatik olarak yenilemeyi seçebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="dc09c-199">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="dc09c-200">Etkin bir ticari Market aboneliğini otomatik olarak yenilemeyi durdurmak için:</span><span class="sxs-lookup"><span data-stu-id="dc09c-200">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="dc09c-201">Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="dc09c-201">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="dc09c-202">Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve listeden bir müşteri seçin.</span><span class="sxs-lookup"><span data-stu-id="dc09c-202">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="dc09c-203">**Abonelikler**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="dc09c-203">Select **Subscriptions**.</span></span> <span data-ttu-id="dc09c-204">Bu, müşteri için satın aldığınız lisans tabanlı abonelikleri listeler.</span><span class="sxs-lookup"><span data-stu-id="dc09c-204">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="dc09c-205">**Abonelik** sütununda, değiştirmek istediğiniz aboneliği seçin.</span><span class="sxs-lookup"><span data-stu-id="dc09c-205">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="dc09c-206">Abonelik Ayrıntıları sayfasında, **durum** bölümünü bulun ve **Otomatik Yenile** kutusunun işaretini kaldırın.</span><span class="sxs-lookup"><span data-stu-id="dc09c-206">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="dc09c-207">**Gönder**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="dc09c-207">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="dc09c-208">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="dc09c-208">Next steps</span></span>

- [<span data-ttu-id="dc09c-209">Müşterileriniz için ticari Market ürünleri satın alın</span><span class="sxs-lookup"><span data-stu-id="dc09c-209">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="dc09c-210">Müşterileriniz için ticari Market ürünlerini yönetme</span><span class="sxs-lookup"><span data-stu-id="dc09c-210">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="dc09c-211">Ticari markete genel bakış</span><span class="sxs-lookup"><span data-stu-id="dc09c-211">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)