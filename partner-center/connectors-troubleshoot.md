---
title: Ortak satış referans bağlayıcıları sorunlarını giderme
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ortak satış bağlayıcılarını kullanma hakkında sık sorulan soruların yanıtlarını öğrenin. Ortak satış bağlayıcıları sorunlarını giderme hakkında bu SSS bölümünü okuyun.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: bb7a227624c548a29046b80d3bd5fa363a4aee2f
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276951"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="8bd4b-104">Ortak satış referans bağlayıcıları sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="8bd4b-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="8bd4b-105">**Için geçerlidir:** Dynamics 365 CRM | Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="8bd4b-105">**Applies to**: Dynamics 365 CRM | Salesforce CRM</span></span>

<span data-ttu-id="8bd4b-106">**Uygun roller:** Referans yöneticisi | CRM'de sistem yöneticisi veya sistem özelleştiricisi</span><span class="sxs-lookup"><span data-stu-id="8bd4b-106">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="8bd4b-107">Önkullar hakkında sorular ve yanıtlar</span><span class="sxs-lookup"><span data-stu-id="8bd4b-107">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="8bd4b-108">Ortamınız için bir deneme ortak satış referans bağlayıcısı çözümü kullanabilir misiniz?</span><span class="sxs-lookup"><span data-stu-id="8bd4b-108">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="8bd4b-109">Test/hazırlama ortamındaysanız deneme çözümünü tercih edin.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-109">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="8bd4b-110">Bağlayıcıların ücretli sürümü, AppSource'ta aylık 15 ABD doları olarak kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-110">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="8bd4b-111">Ücretli bağlantıyla günde 10.000 API çağrısı alasınız.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-111">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="8bd4b-112">Bağlayıcılar, referans API'lerinin İş Ortağı Merkezi sarmalayıcılardır.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-112">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="8bd4b-113">Bağlayıcı çözümleri, İş Ortağı Merkezi  veya  CRM tarafındaki fırsatlarda Oluşturma veya Güncelleştirme olayı için her çalıştırısa, bir API çağrısı yapılır.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-113">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="8bd4b-114">CRM ortamında bölümler oluşturmak için hangi role ihtiyacınız var?</span><span class="sxs-lookup"><span data-stu-id="8bd4b-114">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="8bd4b-115">Sistem yöneticisi veya sistem özelleştiricisi olan kullanıcılar değişiklikleri herkes için uygulayabilir.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-115">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="8bd4b-116">Ancak tüm uygulama kullanıcıları sistemi kişiselleştirenin ve hatta bazı özelleştirmelerini başkalarıyla paylaşabilir.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-116">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="8bd4b-117">İş ortağı satıcılarının iş ortaklarına özel rollere ihtiyacı İş Ortağı Merkezi?</span><span class="sxs-lookup"><span data-stu-id="8bd4b-117">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="8bd4b-118">İş ortağı satıcılarına "Referans yöneticisi" rolü atanmalı.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-118">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="8bd4b-119">Daha fazla bilgi için bkz. [İzinlere genel bakış.](create-user-accounts-and-set-permissions.md)</span><span class="sxs-lookup"><span data-stu-id="8bd4b-119">For more information, see [Permissions overview](create-user-accounts-and-set-permissions.md).</span></span>

4. <span data-ttu-id="8bd4b-120">CRM ortamınıza ilk olarak hangi alanların ayarlanmış olması gerekir?</span><span class="sxs-lookup"><span data-stu-id="8bd4b-120">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="8bd4b-121">• Para biriminizin konumunuz için uygun olduğundan ve CRM ortamınıza uygun olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-121">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="8bd4b-122">• Satış takımınız CRM ortamınıza CRM kullanıcıları olarak listelenmiş olmalı.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-122">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="8bd4b-123">Ortam oluşturmak için hangi önk Power Automate gerekir?</span><span class="sxs-lookup"><span data-stu-id="8bd4b-123">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="8bd4b-124">Ortam ortamını Power Automate için aşağıdakiler gerekir:</span><span class="sxs-lookup"><span data-stu-id="8bd4b-124">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="8bd4b-125">Bir Power Automate lisansı gereklidir.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-125">A Power Automate license is required.</span></span>
- <span data-ttu-id="8bd4b-126">En az 1 GB depolama gereklidir.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-126">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="8bd4b-127">Salesforce Bağlayıcıları çözümünü kullanmak için Dynamics 365 aboneliğine ihtiyacınız var mı?</span><span class="sxs-lookup"><span data-stu-id="8bd4b-127">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="8bd4b-128">Salesforce Bağlayıcısı çözümü, diğer CRM sistemleriyle eşitlemeyi destekleyen "Dynamics Flow" türündedir.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-128">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="8bd4b-129">Çözüm için Dynamics 365 örneğine veya aboneliğe sahip olmak gerekli değildir.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-129">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="8bd4b-130">Salesforce çözümünü yüklerken, şirketiniz içinde var olan CDS ortamına sahip bir açılan liste görünebilir.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-130">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="8bd4b-131">Bu ortamı seçmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-131">You need to select that environment.</span></span> <span data-ttu-id="8bd4b-132">Ayrıca, "Oturum alıkan kullanıcıya bağlı bir Dynamics 365 kuruluşu bulamadı" hatasını alırsanız bağlayıcı için yeni bir ortam oluşturmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-132">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="8bd4b-133">Yapılandırmayla ilgili sorular ve yanıtlar</span><span class="sxs-lookup"><span data-stu-id="8bd4b-133">Questions and answers about configuration</span></span>

1. <span data-ttu-id="8bd4b-134">Power Automate Platform'da akışları etkinleştirirken aşağıdaki hatayla karşılaşıyorsanız ne Power Automate gerekir?</span><span class="sxs-lookup"><span data-stu-id="8bd4b-134">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="8bd4b-135">Hata: Azure Resource Manager isteği şu hatayla başarısız oldu: '{"error":{"code":"WorkflowTriggerNotFound","message":"'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' tetikleyicisi 'manual' bulunamadı."}}'.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-135">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="8bd4b-136">Şu sorun giderme adımlarını izleyin:</span><span class="sxs-lookup"><span data-stu-id="8bd4b-136">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="8bd4b-137">CDS bağlantısını silin ve ardından CDS bağlantılarını yeniden oluşturun.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-137">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="8bd4b-138">Alt akışı kapatma ve açma</span><span class="sxs-lookup"><span data-stu-id="8bd4b-138">Turn the child flow off and on</span></span> 
- <span data-ttu-id="8bd4b-139">Çözümü silin ve çözümü yeniden yükleyin.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-139">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="8bd4b-140">Power Automate Platform'da bir İş Ortağı Merkezi bağlayıcısı eklerken "Oturum açma" hatasıyla karşılaşıyorsanız ne Power Automate gerekir?</span><span class="sxs-lookup"><span data-stu-id="8bd4b-140">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Oturum açma gerektiren hata iletisi.":::

<span data-ttu-id="8bd4b-142">Bu sorun giderme adımını izleyin:</span><span class="sxs-lookup"><span data-stu-id="8bd4b-142">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="8bd4b-143">Akış ortamında İş Ortağı Merkezi için kimlik bilgilerinizi kullanın (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="8bd4b-143">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="8bd4b-144">Power Automate Platform'da CRM akışına İş Ortağı Merkezi etkinleştirirken aşağıdaki hatayı alırsanız ne Power Automate gerekir?</span><span class="sxs-lookup"><span data-stu-id="8bd4b-144">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Güncelleştirme gerektiren hata iletisi.":::

<span data-ttu-id="8bd4b-146">Şu sorun giderme adımlarını izleyin:</span><span class="sxs-lookup"><span data-stu-id="8bd4b-146">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="8bd4b-147">CRM akışına yönelik akışı etkinleştirmeden önce aşağıdaki iki İş Ortağı Merkezi akışı etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-147">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="8bd4b-148">İş Ortağı Merkezi CRM ' e - Yardımcı (Insider Önizleme)</span><span class="sxs-lookup"><span data-stu-id="8bd4b-148">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="8bd4b-149">İş Ortağı Merkezi Microsoft'un CRM'ye Ortak Satış Referans Güncelleştirmeleri (Insider Önizlemesi)</span><span class="sxs-lookup"><span data-stu-id="8bd4b-149">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="8bd4b-150">Akışı düzenlemeye çalışmadan akışa bağlantı ekleye değilken ne yapacaksınız?</span><span class="sxs-lookup"><span data-stu-id="8bd4b-150">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="8bd4b-151">Akış çalışırken akışa bağlantılar ekler ve her akışa ayrı olarak eklersiniz.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-151">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="8bd4b-152">Bağlantı ekleme iletişim kutusu akışı düzenlerken otomatik olarak açılmazsa, akışların adımlarını ve alt adımlarını tek tek düzenleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-152">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="8bd4b-153">Her akışı seçin ve ayrı ayrı düzenleyin.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-153">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="8bd4b-154">Akışta tüm adımları genişletin</span><span class="sxs-lookup"><span data-stu-id="8bd4b-154">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Bağlantı gereken adımlar.":::

- <span data-ttu-id="8bd4b-156">Bağlantıları ilişkilendirmek ve bağlantı eklemek için bir uyarı simgesi gördüğünüz adımları seçin.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-156">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Akışı adım adım düzenleyin.":::


5. <span data-ttu-id="8bd4b-158">Ortak Satış Referansları Bağlayıcıları çözümünün akışları açık yoksa ne yapacaksınız?</span><span class="sxs-lookup"><span data-stu-id="8bd4b-158">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="8bd4b-159">A.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-159">A.</span></span> <span data-ttu-id="8bd4b-160">Bu Power Automate, akışları aşağıdaki sırayla düzenlemeniz ve doğru bağlantıları kullanmak üzere güncelleştirmeniz gerekir:</span><span class="sxs-lookup"><span data-stu-id="8bd4b-160">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="8bd4b-161">İş Ortağı Merkezi Web Kancası Kaydı (Insider Önizlemesi)</span><span class="sxs-lookup"><span data-stu-id="8bd4b-161">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="8bd4b-162">Ortak Satış Referansı Oluşturma - İş Ortağı Merkezi salesforce (Insider Önizleme)</span><span class="sxs-lookup"><span data-stu-id="8bd4b-162">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="8bd4b-163">İş Ortağı Merkezi Microsoft Ortak Satış Referans Güncelleştirmelerini Salesforce'a (Insider Önizleme) yönlendirme</span><span class="sxs-lookup"><span data-stu-id="8bd4b-163">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="8bd4b-164">İş Ortağı Merkezi'a (Insider Önizleme)</span><span class="sxs-lookup"><span data-stu-id="8bd4b-164">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="8bd4b-165">Salesforce'tan İş Ortağı Merkezi 'a (Insider Önizleme)</span><span class="sxs-lookup"><span data-stu-id="8bd4b-165">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="8bd4b-166">Salesforce Opportunity to İş Ortağı Merkezi (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="8bd4b-166">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="8bd4b-167">İş Ortağı Merkezi için Salesforce Microsoft Solutions (Insider Önizleme)</span><span class="sxs-lookup"><span data-stu-id="8bd4b-167">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="8bd4b-168">B.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-168">B.</span></span> <span data-ttu-id="8bd4b-169">Akışın her biri için Yalnızca kullanıcıları **çalıştır seçeneğini** belirleyin.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-169">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="8bd4b-170">Yalnızca **çalıştıran kullanıcı** tarafından **sağlanan yerine Bağlantıyı kullan'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="8bd4b-170">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Akışı etkinleştirmek için.":::


<span data-ttu-id="8bd4b-172">C.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-172">C.</span></span> <span data-ttu-id="8bd4b-173">Aşağıda belirtilen akışları etkinleştirin:</span><span class="sxs-lookup"><span data-stu-id="8bd4b-173">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="8bd4b-174">İş Ortağı Merkezi Microsoft Ortak Satış Referans Güncelleştirmelerini Salesforce'a (Insider Önizleme) yönlendirme</span><span class="sxs-lookup"><span data-stu-id="8bd4b-174">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="8bd4b-175">Salesforce'tan İş Ortağı Merkezi 'a (Insider Önizleme)</span><span class="sxs-lookup"><span data-stu-id="8bd4b-175">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="8bd4b-176">D.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-176">D.</span></span> <span data-ttu-id="8bd4b-177">Kalan tüm akışları etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-177">Activate all the remaining flows.</span></span>

<span data-ttu-id="8bd4b-178">E.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-178">E.</span></span> <span data-ttu-id="8bd4b-179">Web Kancası İş Ortağı Merkezi akışında Çalıştır'ı **seçin.**</span><span class="sxs-lookup"><span data-stu-id="8bd4b-179">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="8bd4b-180">**İş Ortağı Merkezi'de Salesforce akışına ilk eylemden http URL'sini** girin. </span><span class="sxs-lookup"><span data-stu-id="8bd4b-180">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="8bd4b-181">Kaydolmak için Olaylar altında dört **seçeneğin de hepsini seçin ve Üzerine** Yaz için **evet'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-181">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="8bd4b-182">Çalıştırma/Bakım hakkında sorular ve yanıtlar</span><span class="sxs-lookup"><span data-stu-id="8bd4b-182">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="8bd4b-183">Akış yürütme sırasındaki hataları Power Automate giderin?</span><span class="sxs-lookup"><span data-stu-id="8bd4b-183">How do you troubleshoot failures during Power Automate flow execution?</span></span>

<span data-ttu-id="8bd4b-184">Akış akışlarının beklediğiniz Power Automate olduğundan emin olmak ve yürütme sırasındaki hataları gidermek için [bkz. Akış hatalarını düzeltme.](/power-automate/fix-flow-failures)</span><span class="sxs-lookup"><span data-stu-id="8bd4b-184">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="8bd4b-185">İş Ortağı Merkezi VEYA CRM ortamında düzgün eşitlenmemiş referanslar görüyorsanız ne yapacaksınız?</span><span class="sxs-lookup"><span data-stu-id="8bd4b-185">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="8bd4b-186">Referans eşitleme durumunu belirlemek için Denetle'yi **seçin.**</span><span class="sxs-lookup"><span data-stu-id="8bd4b-186">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Referansları eşitleme.":::

<span data-ttu-id="8bd4b-188">Aşağıdaki koşulların karşı olduğundan emin olmak:</span><span class="sxs-lookup"><span data-stu-id="8bd4b-188">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="8bd4b-189">Çözüm kimliği, fırsatın bir parçası olarak sağlanır.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-189">Solution ID is provided as part of the opportunity.</span></span>

- <span data-ttu-id="8bd4b-190">İki harfli ülke kodu gereklidir.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-190">Two letter country code is required.</span></span>

- <span data-ttu-id="8bd4b-191">Fırsat için Microsoft'tan yardım seçildiğinde müşteri iletişim bilgileri gereklidir.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-191">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="8bd4b-192">Bir referansın çift yönlü olarak eşitlenmesi nasıl sağlandı?</span><span class="sxs-lookup"><span data-stu-id="8bd4b-192">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="8bd4b-193">Aşağıdaki adımları uygulayın:</span><span class="sxs-lookup"><span data-stu-id="8bd4b-193">Do the following steps:</span></span>

- <span data-ttu-id="8bd4b-194">İş ortağı satıcılarının CRM bölümünde İş Ortağı Merkezi **eşitle seçeneğini etkinleştirmiş** olduğundan emin olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-194">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Eşitle'yi etkinleştirdikten emin olun.":::

- <span data-ttu-id="8bd4b-196">Satış satıcılarının müşteri adayını kabul etmek için gelir ve kapanış tarihi sağlamaları gerekir.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-196">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="8bd4b-197">CRM Kimliği ortak satış  fırsatının oluşturma veya güncelleştirme aşamasında sağlanıyorsa ancak CRM'de bu kimliğin bulunduğu bir müşteri adayı fırsatı yoksayılırsa güncelleştirme veya oluşturma yoksayılır. </span><span class="sxs-lookup"><span data-stu-id="8bd4b-197">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="8bd4b-198">Referans para biriminin Salesforce ortamında yapılandırıldığından emin olmak.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-198">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="8bd4b-199">Bağlayıcının bağlantısı kesilirse ve referans eşitlemesini kaçırırsanız ne yapacaksınız?</span><span class="sxs-lookup"><span data-stu-id="8bd4b-199">What should you do if the connector gets disconnected and you miss a referral synchronization.?</span></span>

<span data-ttu-id="8bd4b-200">Deneyebilirsiniz seçeneklerden birkaçı şunlardır:</span><span class="sxs-lookup"><span data-stu-id="8bd4b-200">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="8bd4b-201">Iş Ortağı Merkezi kullanıcısı için başvuru yöneticisi rollerine sahip kullanıcı adının veya parolanın dolup dolmadığını denetleyin.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-201">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="8bd4b-202">Eşitlenmemiş fırsata gidebilir, küçük bir güncelleştirme yapabilir ve başvurunun eşitlenip eşitlenmediğini gözlemleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-202">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="8bd4b-203">Akışlar çalıştırılmışsa ve başarısız olursa, akışı seçip başarısız olan çalıştırmayı yeniden gönderebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-203">If the flows have run and failed, then select the flow and re-submit the run that has failed.</span></span>

5. <span data-ttu-id="8bd4b-204">Erişim reddedildi hatalarını aldığınızda ne yapmalısınız?</span><span class="sxs-lookup"><span data-stu-id="8bd4b-204">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="8bd4b-205">Uygun rollerin mevcut olduğundan emin olun</span><span class="sxs-lookup"><span data-stu-id="8bd4b-205">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="8bd4b-206">Iş Ortağı Merkezi satıcı için başvuru Yöneticisi rolü</span><span class="sxs-lookup"><span data-stu-id="8bd4b-206">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="8bd4b-207">CRM örneğiniz üzerinde sistem yöneticisi veya sistem özelleştirici rolü</span><span class="sxs-lookup"><span data-stu-id="8bd4b-207">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="8bd4b-208">Power otomatikleştirmenin akış hesabı kullanıcısının https://flow.microsoft.com önceden en az bir kez oturum açtığına sahip olduğundan emin olun</span><span class="sxs-lookup"><span data-stu-id="8bd4b-208">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="8bd4b-209">Ortak satış fırsatı oluştururken **müşteri hesabı ülke kodunun** eksik olduğunu görürseniz, ne yapmanız gerekir?</span><span class="sxs-lookup"><span data-stu-id="8bd4b-209">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="8bd4b-210">ISO 'nın iki harfli ülke kodunu CRM 'de müşteri hesabına eklemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-210">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="8bd4b-211">Ortak satış fırsatı oluştururken **Çözüm Kimliği 'nin gerekli** olduğu hatayı görürseniz ne yapmanız gerekir?</span><span class="sxs-lookup"><span data-stu-id="8bd4b-211">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="8bd4b-212">Ortak satış başvurusu oluşturmak için, Microsoft ortak satış için kullanabileceğiniz bir çözüme ihtiyacınız vardır.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-212">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="8bd4b-213">Iş akışı hatası olmasa dahi, Iş Ortağı Merkezi 'nde oluşturulmuş ortak satış fırsatlarını gördüğünüzde ne yapmalısınız?</span><span class="sxs-lookup"><span data-stu-id="8bd4b-213">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors?</span></span>

<span data-ttu-id="8bd4b-214">Şunları yapın:</span><span class="sxs-lookup"><span data-stu-id="8bd4b-214">Do the following:</span></span>

- <span data-ttu-id="8bd4b-215">Iş Ortağı Merkezi 'nde yeni bir ortak satış sorunu oluşturduktan sonra, Dynamics 365 Flow Iş Ortağı Merkezi 'nin çağrılacağını (birden çok kez çağrılabilir) denetleyin.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-215">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="8bd4b-216">Akış çağrılırsa, tüm çağrılan Akışlar ' ı işaretleyin ve bu, CRM 'yi güncelleştiren akış çalıştırmasını belirler.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-216">If the flow gets invoked, check all invoked flows, and identify the flow run which that would update the CRM.</span></span> <span data-ttu-id="8bd4b-217">Eylemleri izleyebilir ve CRM 'yi güncelleştirip güncelleştirmediğinizi veya bir sorunla karşılaştıysanız emin olabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-217">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="8bd4b-218">CRM KIMLIĞIYLE doldurulup doldurulmadığını görmek için Iş Ortağı Merkezi 'nde **yeni anlaşmayı** denetleyin.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-218">Check **New deal** in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="8bd4b-219">Iş Ortağı Merkezi 'nde, anlaşmayı **kazanıldı** veya **kaybedildi** olarak kapanmadığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="8bd4b-219">Make sure that the deal is not accidentally closed as **Won** or **Lost** in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8bd4b-220">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="8bd4b-220">Next steps</span></span>

- [<span data-ttu-id="8bd4b-221">Müşteri adaylarını yönetme</span><span class="sxs-lookup"><span data-stu-id="8bd4b-221">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="8bd4b-222">Ortak satış fırsatlarını yönetme</span><span class="sxs-lookup"><span data-stu-id="8bd4b-222">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
