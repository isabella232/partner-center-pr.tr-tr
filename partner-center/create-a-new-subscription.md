---
title: Iş Ortağı Merkezi 'nde müşteri abonelikleri oluşturma
ms.topic: how-to
ms.date: 07/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft tarafından yayımlanan ürünlerin yanı sıra üçüncü taraf ISV 'Ler tarafından yayımlanan SaaS ürünleri için müşterilerinize abonelik satma hakkında bilgi edinin.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 559d1fbd2efc1417ae89931279b9d3c9a1d67f7c
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502944"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="3050c-103">Müşteri aboneliklerini oluşturma, askıya alma veya iptal etme</span><span class="sxs-lookup"><span data-stu-id="3050c-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="3050c-104">**Şunlara uygulanır**</span><span class="sxs-lookup"><span data-stu-id="3050c-104">**Applies to**</span></span>

- <span data-ttu-id="3050c-105">Microsoft Cloud for US Government için İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="3050c-105">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="3050c-106">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="3050c-106">**Appropriate roles**</span></span>

- <span data-ttu-id="3050c-107">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="3050c-107">Admin agent</span></span>
- <span data-ttu-id="3050c-108">Faturalama yöneticisi</span><span class="sxs-lookup"><span data-stu-id="3050c-108">Billing admin</span></span>
- <span data-ttu-id="3050c-109">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="3050c-109">Global admin</span></span>
- <span data-ttu-id="3050c-110">Yardım Masası Aracısı</span><span class="sxs-lookup"><span data-stu-id="3050c-110">Helpdesk agent</span></span>
- <span data-ttu-id="3050c-111">Satış Aracısı</span><span class="sxs-lookup"><span data-stu-id="3050c-111">Sales agent</span></span>

<span data-ttu-id="3050c-112">Iş Ortağı Merkezi 'nde müşterinizin bir kaydını oluşturduktan sonra, bu abonelikleri katalogdaki ürünlere satabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="3050c-112">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="3050c-113">Bu, üçüncü taraf bağımsız yazılım satıcıları (ISV 'Ler) tarafından [ticari Market](https://azuremarketplace.microsoft.com/marketplace)'e yayımlanan Microsoft ve hizmet olarak yazılım (SaaS) ürünleri tarafından yayımlanan ürünleri içerir.</span><span class="sxs-lookup"><span data-stu-id="3050c-113">This includes products published by Microsoft and Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="3050c-114">Bazı teklifler müşteri başına bir abonelikle sınırlıdır.</span><span class="sxs-lookup"><span data-stu-id="3050c-114">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="3050c-115">Hangi tekliflerin kısıtlı olduğunu görmek için Iş Ortağı Merkezi fiyatlandırma ve teklifleri sayfasını ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="3050c-115">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="3050c-116">CSP programındaki bir iş ortağı olarak, Iş Ortağı Merkezi 'nde ISV yayımcılarından **Lisans tabanlı** veya **ölçülen** SaaS abonelikleri satın alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="3050c-116">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="3050c-117">Bu, tüm **Lisans tabanlı** veya **tarifeli** SaaS tekliflerini, erişiminiz olan [özel TEKLIFLER](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) de dahil olmak üzere ISV yayımcısı kullanımınıza sunabileceğiniz anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="3050c-117">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="3050c-118">ISV 'lerden diğer, ticari Market tekliflerini satın almak veya yönetmek için (Azure uygulamaları, kapsayıcılar veya VM 'Leri içeren Kullanım tabanlı teklifler gibi) [Azure Portal](https://portal.azure.com/)gitmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="3050c-118">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="3050c-119">Yeni abonelik oluştur</span><span class="sxs-lookup"><span data-stu-id="3050c-119">Create a new subscription</span></span>

1. <span data-ttu-id="3050c-120">[İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="3050c-120">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="3050c-121">Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve listeden bir müşteri seçin.</span><span class="sxs-lookup"><span data-stu-id="3050c-121">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="3050c-122">**Abonelik Ekle**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="3050c-122">Select **Add subscription**.</span></span> <span data-ttu-id="3050c-123">**Çevrimiçi hizmetler** sekmesinde, tüm kullanılabilir Market SaaS teklifleri gösterilir.</span><span class="sxs-lookup"><span data-stu-id="3050c-123">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="3050c-124">Yalnızca belirli abonelik türlerini görmek için, kullanılabilir filtrelerdeki seçimleri yapın:</span><span class="sxs-lookup"><span data-stu-id="3050c-124">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="3050c-125">**Yayımcı**: ISV 'ler tarafından yayımlanan ticari Market ürünlerini görmek Için yalnızca Microsoft 'un veya **iş ortağının** tekliflerini görmek üzere **Microsoft** 'u seçin.</span><span class="sxs-lookup"><span data-stu-id="3050c-125">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="3050c-126">**Faturalandırma türü**: kullanmak istediğiniz abonelik faturalandırması türünü seçin: **Lisans** veya **kullanım**.</span><span class="sxs-lookup"><span data-stu-id="3050c-126">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="3050c-127">Aylık ve yıllık faturalandırma sıklığıyla ilgili karar vermenize yardımcı olacak bilgiler için [Lisans tabanlı faturalandırma](license-based-billing.md) konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="3050c-127">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="3050c-128">**Kategori**: **Kurumsal**, **küçük iş** veya **deneme**' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="3050c-128">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="3050c-129">Deneme abonelikleri hakkında bilgi için bkz. [Microsoft ürünlerine yönelik müşterilerinizin deneme sürümlerini sunma](offer-your-customers-trials-of-microsoft-products.md).</span><span class="sxs-lookup"><span data-stu-id="3050c-129">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="3050c-130">Müşteriniz için satın almak istediğiniz ürün aboneliklerini seçin.</span><span class="sxs-lookup"><span data-stu-id="3050c-130">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="3050c-131">Gördüğünüz ürünler, müşteri segmentinin (eğitim, Kamu, vb.) ve uyguladığınız filtrelerin türüne bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="3050c-131">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="3050c-132">Market 'te gösterilen bazı teklifler, belirli bir müşteri veya belirli bir CSP iş ortağı tarafından her zaman kullanılabilir olmayabilir.</span><span class="sxs-lookup"><span data-stu-id="3050c-132">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="3050c-133">Bunun nedeni şu olabilir:</span><span class="sxs-lookup"><span data-stu-id="3050c-133">This can be because:</span></span>

   - <span data-ttu-id="3050c-134">Müşterinin zaten bu ürüne yönelik bir aboneliği var ve yalnızca bir tane kullanılabilir</span><span class="sxs-lookup"><span data-stu-id="3050c-134">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="3050c-135">Müşterinin aboneliği askıya alınmış olabilir (Bu durumda, yeni bir tane satın almak yerine aboneliği yeniden etkinleştirebilirsiniz.)</span><span class="sxs-lookup"><span data-stu-id="3050c-135">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="3050c-136">ISV SaaS teklifleri için teklifin satın alma için sunulmamasının birkaç nedeni olabilir: ISV müşterinin fatura ülkesini veya bölgesini desteklemiyor olabilir; ISV, teklifi CSP programı aracılığıyla kullanılabilir hale getirmek için seçilmiş olabilir; ya da ISV, teklifi yalnızca belirli CSP iş ortakları için [özel](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) olarak yapmış olabilir.</span><span class="sxs-lookup"><span data-stu-id="3050c-136">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="3050c-137">ISV teklifi Ayrıca Iş Ortağı Merkezi (örneğin, kapsayıcılar veya bazı kullanım tabanlı teklifler) üzerinden transactable de olmayabilir.</span><span class="sxs-lookup"><span data-stu-id="3050c-137">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="3050c-138">Eklemek istediğiniz her abonelik için, lisansların (gerekirse) sayısını girin ve **Sepete Ekle**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="3050c-138">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="3050c-139">Abonelik eklemeyi bitirdiğinizde, **gözden geçir** ' i seçin ve siparişinizi gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="3050c-139">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="3050c-140">Siparişlerinizi gözden geçirdikten ve bu abonelikleri satın almaya hazırladıktan sonra **satın al**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="3050c-140">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="3050c-141">Bir müşteri için abonelik satın aldıktan sonra aşağıdakiler gerçekleşir:</span><span class="sxs-lookup"><span data-stu-id="3050c-141">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="3050c-142">Bu müşterinin **abonelikler** sayfasından abonelik adı ' nı seçerek aboneliği gözden geçirebilir veya düzenleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="3050c-142">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="3050c-143">Buradan, varsa eklenti lisanslarını seçebilirsiniz, lisans miktarını değiştirebilir veya aboneliği askıya alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="3050c-143">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="3050c-144">**ISV SaaS (lisans tabanlı ve tarifeli) abonelikler için:**</span><span class="sxs-lookup"><span data-stu-id="3050c-144">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="3050c-145">ISV yayımcısının sitesine bir bağlantı alacaksınız.</span><span class="sxs-lookup"><span data-stu-id="3050c-145">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="3050c-146">Bu bağlantı, müşterinin aboneliğine ait dağıtım veya hesap kurulumunu tamamlamanıza yardımcı olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="3050c-146">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="3050c-147">Ne siz ne de müşteriniz bu tür ISV aboneliği için kurulumu/sağlamayı tamamlamaya yönelik yönergeleri içeren bir e-posta alacaksınız.)</span><span class="sxs-lookup"><span data-stu-id="3050c-147">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="3050c-148">Aboneliğiniz 30 günlük ücretsiz deneme sürümü ile birlikte geliyorsa, ücretsiz deneme süresi otomatik olarak uygulanır.</span><span class="sxs-lookup"><span data-stu-id="3050c-148">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="3050c-149">CSP programındaki bir iş ortağı olarak, müşteriler için satın aldığınız tekliflerle ilgili ücretsiz deneme süresini beklenemez.</span><span class="sxs-lookup"><span data-stu-id="3050c-149">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="3050c-150">Ücretsiz deneme süresi sona erdiğinde, abonelik dönemi başlar ve abonelik, ücretli duruma dönüştürülür.</span><span class="sxs-lookup"><span data-stu-id="3050c-150">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="3050c-151">Abonelik daha sonra aynı zamanlamaya göre otomatik olarak yenilenecek.</span><span class="sxs-lookup"><span data-stu-id="3050c-151">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="3050c-152">Eklentilerle abonelikleri güncelleştirme</span><span class="sxs-lookup"><span data-stu-id="3050c-152">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="3050c-153">Bir eklenti satın almak için müşterinin öncelikle etkin bir temel aboneliği olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="3050c-153">To purchase an add-on, the customer must first have an active base subscription.</span></span>  <span data-ttu-id="3050c-154">Eklentileri katalog aracılığıyla satın alamazsınız.</span><span class="sxs-lookup"><span data-stu-id="3050c-154">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="3050c-155">Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="3050c-155">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="3050c-156">Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve listeden bir müşteri seçin.</span><span class="sxs-lookup"><span data-stu-id="3050c-156">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="3050c-157">Yönetmek istediğiniz aboneliği seçin.</span><span class="sxs-lookup"><span data-stu-id="3050c-157">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="3050c-158">**Durum** bölümünün altında, abonelik Için kullanılabilen eklentilerin bir listesi bulunur.</span><span class="sxs-lookup"><span data-stu-id="3050c-158">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="3050c-159">Gerekli her eklenti için lisans miktarını güncelleştirin.</span><span class="sxs-lookup"><span data-stu-id="3050c-159">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="3050c-160">Sonra **Gönder** ile yaptığınız değişiklikleri gönderin.</span><span class="sxs-lookup"><span data-stu-id="3050c-160">Then **Submit** your changes.</span></span>

<span data-ttu-id="3050c-161">Iş Ortağı Merkezi aracılığıyla eklenti satın alma özelliği yalnızca doğrudan fatura ve dolaylı sağlayıcılar için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="3050c-161">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="3050c-162">Temel gereksinimlere ve bölgesel kullanılabilirliğe göre yalnızca uygun eklentiler görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="3050c-162">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="3050c-163">Fiyatlandırma ve teklifler hakkında daha fazla bilgi için bkz. Cloud Bayi teklif matrisi.</span><span class="sxs-lookup"><span data-stu-id="3050c-163">For more information about pricing and offers, refer to the Cloud Reseller offer matrix.</span></span> <span data-ttu-id="3050c-164">Temel abonelik askıya alındığında ilişkili tüm eklentiler de askıya alınır.</span><span class="sxs-lookup"><span data-stu-id="3050c-164">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="3050c-165">Eklentilerin başlangıç tarihleri temel abonelikle uyumludur; ücretler Ücret başlangıç tarihi ile Ücret bitiş tarihi kullanılarak hesaplanır ve ilk faturaya orantılı bir ücret uygulanır.</span><span class="sxs-lookup"><span data-stu-id="3050c-165">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="3050c-166">Daha fazla bilgi için bkz. [Lisans tabanlı faturalandırma](license-based-billing.md).</span><span class="sxs-lookup"><span data-stu-id="3050c-166">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="3050c-167">Aboneliği askıya alma veya iptal etme</span><span class="sxs-lookup"><span data-stu-id="3050c-167">Suspend or cancel a subscription</span></span>

<span data-ttu-id="3050c-168">İş ortakları, müşteri tarafından isteniyorsa veya ödeme veya sahtekarlık durumlarında bir aboneliği askıya alabilir veya iptal edebilir.</span><span class="sxs-lookup"><span data-stu-id="3050c-168">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="3050c-169">Bir aboneliği askıya alma</span><span class="sxs-lookup"><span data-stu-id="3050c-169">Suspend a subscription</span></span>

<span data-ttu-id="3050c-170">Aboneliğin durumunu **askıya alındı** olarak değiştirdiğinizde, kullanıcılar oturum açamaz veya hizmetlere erişemez.</span><span class="sxs-lookup"><span data-stu-id="3050c-170">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="3050c-171">Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="3050c-171">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="3050c-172">Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve listeden bir müşteri seçin.</span><span class="sxs-lookup"><span data-stu-id="3050c-172">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="3050c-173">Yönetmek istediğiniz aboneliği seçin.</span><span class="sxs-lookup"><span data-stu-id="3050c-173">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="3050c-174">**Durum** bölümünde **Askıya Alındı**'yı seçin.</span><span class="sxs-lookup"><span data-stu-id="3050c-174">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="3050c-175">Sonra **Gönder** ile yaptığınız değişiklikleri gönderin.</span><span class="sxs-lookup"><span data-stu-id="3050c-175">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="3050c-176">Abonelik 90 gün içinde yeniden etkinleştirilmediği veya 90 gün ile hesabın açıldığı zaman arasındaki gün sayısı ile ilk fatura dönemi (maksimum 120 gün) arasında tüm veriler silinir.</span><span class="sxs-lookup"><span data-stu-id="3050c-176">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="3050c-177">Bir aboneliği askıya aldığınızda, **askıya alınmış** düğmesinin altında gördüğünüz Tarih, yeniden etkinleştirmezseniz aboneliğin otomatik olarak ne zaman dolacağını gösterir.</span><span class="sxs-lookup"><span data-stu-id="3050c-177">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

### <a name="cancel-a-subscription"></a><span data-ttu-id="3050c-178">Aboneliği iptal et</span><span class="sxs-lookup"><span data-stu-id="3050c-178">Cancel a subscription</span></span>

<span data-ttu-id="3050c-179">Iş Ortağı Merkezi [ticari marketi](csp-commercial-marketplace-overview.md)kapsamındaki üçüncü taraf ISV yayımcılarından lisans tabanlı SaaS aboneliklerini iptal edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="3050c-179">You can cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="3050c-180">İptal dönemi içinde iptal ettiğiniz sürece, tam bir para iadesi alırsınız.</span><span class="sxs-lookup"><span data-stu-id="3050c-180">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="3050c-181">Aylık olarak faturalandırılan ISV teklifleri için:</span><span class="sxs-lookup"><span data-stu-id="3050c-181">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="3050c-182">Siparişi yerleştirdikten sonra 24 saatten az iptal ederseniz bir sonraki faturada bir tam kredi alacaksınız.</span><span class="sxs-lookup"><span data-stu-id="3050c-182">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="3050c-183">Siparişi yerleştirdikten sonra 24 saatten sonra iptal ederseniz, iptal etme, yenileme sırasında gerçekleşecek şekilde zamanlanır.</span><span class="sxs-lookup"><span data-stu-id="3050c-183">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="3050c-184">Yıllık olarak faturalandırılan teklifler için:</span><span class="sxs-lookup"><span data-stu-id="3050c-184">For offers billed annually:</span></span>

- <span data-ttu-id="3050c-185">Siparişi girdikten sonra 14 günden daha az bir süre sonra iptal ederseniz, sonraki faturada bir tam kredi alırsınız.</span><span class="sxs-lookup"><span data-stu-id="3050c-185">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="3050c-186">Siparişi girdikten sonra 14 günden daha sonra iptal ederseniz iptali, yenileme sırasında gerçekleşecek şekilde zamanlanır.</span><span class="sxs-lookup"><span data-stu-id="3050c-186">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="3050c-187">Bu dönemler bittikten sonra, aboneliği iptal etme seçeneğini artık göremezsiniz.</span><span class="sxs-lookup"><span data-stu-id="3050c-187">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="3050c-188">Kullanım tabanlı ve tarifeli, üçüncü taraf ISV Hizmetleri (örneğin, sanal makineleri veya kapsayıcıları kullanan), return için uygun değildir.</span><span class="sxs-lookup"><span data-stu-id="3050c-188">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="3050c-189">Kullanım tabanlı hizmetler, iptal yöntemi olarak geçersiz bir şekilde sağlanabilir.</span><span class="sxs-lookup"><span data-stu-id="3050c-189">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="3050c-190">Ücretler kullanım sonrasında faturalandırıladıklarından, bu hizmetler para iadesi için uygun değildir.</span><span class="sxs-lookup"><span data-stu-id="3050c-190">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="3050c-191">Lisans tabanlı bir SaaS aboneliğini ISV yayımcısından iptal etmek için aşağıdakileri yapın:</span><span class="sxs-lookup"><span data-stu-id="3050c-191">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="3050c-192">Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="3050c-192">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="3050c-193">Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve listeden bir müşteri seçin.</span><span class="sxs-lookup"><span data-stu-id="3050c-193">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="3050c-194">İptal etmek istediğiniz aboneliği bulun.</span><span class="sxs-lookup"><span data-stu-id="3050c-194">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="3050c-195">**Durum** sütununda **iptal**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="3050c-195">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="3050c-196">Sonra **Gönder** ile yaptığınız değişiklikleri gönderin.</span><span class="sxs-lookup"><span data-stu-id="3050c-196">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="3050c-197">Bir iletişim kutusu görüntülenirse, ilgili ayrıntıları doldurun ve **Gönder**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="3050c-197">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="3050c-198">İptali onaylamak için **Evet, iptal**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="3050c-198">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="3050c-199">Ayrıca API 'Leri kullanarak bir Azure Marketi aboneliğini iptal etmeyi seçebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="3050c-199">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="3050c-200">Bunu yapmak için bkz. [Azure Marketi aboneliğini Iptal etme](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span><span class="sxs-lookup"><span data-stu-id="3050c-200">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="3050c-201">Bir ticari Market aboneliğinin otomatik olarak yenilenip yenilenmeyeceğini seçin</span><span class="sxs-lookup"><span data-stu-id="3050c-201">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="3050c-202">Etkin abonelikler varsayılan olarak abonelik süresi sona erdiğinde otomatik olarak yenilenecek şekilde ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="3050c-202">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="3050c-203">[Ticari Market ürünlerine yönelik abonelikler](csp-commercial-marketplace-overview.md)için, isteğe bağlı olarak, aboneliği otomatik olarak yenilemeyi seçebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="3050c-203">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="3050c-204">Etkin bir ticari Market aboneliğini otomatik olarak yenilemeyi durdurmak için:</span><span class="sxs-lookup"><span data-stu-id="3050c-204">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="3050c-205">Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="3050c-205">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="3050c-206">Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve listeden bir müşteri seçin.</span><span class="sxs-lookup"><span data-stu-id="3050c-206">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="3050c-207">**Abonelikler**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="3050c-207">Select **Subscriptions**.</span></span> <span data-ttu-id="3050c-208">Bu, müşteri için satın aldığınız lisans tabanlı abonelikleri listeler.</span><span class="sxs-lookup"><span data-stu-id="3050c-208">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="3050c-209">**Abonelik** sütununda, değiştirmek istediğiniz aboneliği seçin.</span><span class="sxs-lookup"><span data-stu-id="3050c-209">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="3050c-210">Abonelik Ayrıntıları sayfasında, **durum** bölümünü bulun ve **Otomatik Yenile** kutusunun işaretini kaldırın.</span><span class="sxs-lookup"><span data-stu-id="3050c-210">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="3050c-211">**Gönder**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="3050c-211">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3050c-212">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="3050c-212">Next steps</span></span>

- [<span data-ttu-id="3050c-213">Müşterileriniz için ticari Market ürünleri satın alın</span><span class="sxs-lookup"><span data-stu-id="3050c-213">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="3050c-214">Müşterileriniz için ticari Market ürünlerini yönetme</span><span class="sxs-lookup"><span data-stu-id="3050c-214">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="3050c-215">Ticari markete genel bakış</span><span class="sxs-lookup"><span data-stu-id="3050c-215">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)