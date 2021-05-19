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
ms.openlocfilehash: 49a2b6e5461dacbe87c34b36805a5c240c2e5fd1
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148355"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="d0210-104">Ortak satış referans bağlayıcıları sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="d0210-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="d0210-105">**Için geçerlidir:** Dynamics 365 CRM | Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="d0210-105">**Applies to**: Dynamics 365 CRM | Salesforce CRM</span></span>

<span data-ttu-id="d0210-106">**Uygun roller:** Referans yöneticisi | CRM'de sistem yöneticisi veya sistem özelleştiricisi</span><span class="sxs-lookup"><span data-stu-id="d0210-106">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="d0210-107">Önkullar hakkında sorular ve yanıtlar</span><span class="sxs-lookup"><span data-stu-id="d0210-107">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="d0210-108">Ortamınız için bir deneme ortak satış referans bağlayıcısı çözümü kullanabilir misiniz?</span><span class="sxs-lookup"><span data-stu-id="d0210-108">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="d0210-109">Test/hazırlama ortamındaysanız deneme çözümünü tercih edin.</span><span class="sxs-lookup"><span data-stu-id="d0210-109">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="d0210-110">Bağlayıcıların ücretli sürümü, AppSource'ta aylık 15 ABD doları olarak kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="d0210-110">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="d0210-111">Ücretli bağlantıyla günde 10.000 API çağrısı alasınız.</span><span class="sxs-lookup"><span data-stu-id="d0210-111">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="d0210-112">Bağlayıcılar, referans API'lerinin İş Ortağı Merkezi sarmalayıcılardır.</span><span class="sxs-lookup"><span data-stu-id="d0210-112">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="d0210-113">Bağlayıcı çözümleri, İş Ortağı Merkezi  veya  CRM tarafındaki fırsatlarda Oluşturma veya Güncelleştirme olayı için her çalıştırısa, bir API çağrısı yapılır.</span><span class="sxs-lookup"><span data-stu-id="d0210-113">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="d0210-114">CRM ortamında bölümler oluşturmak için hangi role ihtiyacınız var?</span><span class="sxs-lookup"><span data-stu-id="d0210-114">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="d0210-115">Sistem yöneticisi veya sistem özelleştiricisi olan kullanıcılar değişiklikleri herkes için uygulayabilir.</span><span class="sxs-lookup"><span data-stu-id="d0210-115">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="d0210-116">Ancak tüm uygulama kullanıcıları sistemi kişiselleştirenin ve hatta bazı özelleştirmelerini başkalarıyla paylaşabilir.</span><span class="sxs-lookup"><span data-stu-id="d0210-116">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="d0210-117">İş ortağı satıcılarının iş ortaklarına özel rollere ihtiyacı İş Ortağı Merkezi?</span><span class="sxs-lookup"><span data-stu-id="d0210-117">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="d0210-118">İş ortağı satıcılarına "Referans yöneticisi" rolü atanmalı.</span><span class="sxs-lookup"><span data-stu-id="d0210-118">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="d0210-119">Daha fazla bilgi için bkz. [İzinlere genel bakış.](create-user-accounts-and-set-permissions.md)</span><span class="sxs-lookup"><span data-stu-id="d0210-119">For more information, see [Permissions overview](create-user-accounts-and-set-permissions.md).</span></span>

4. <span data-ttu-id="d0210-120">CRM ortamınıza ilk olarak hangi alanların ayarlanmış olması gerekir?</span><span class="sxs-lookup"><span data-stu-id="d0210-120">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="d0210-121">• Para biriminiz konumunuza uygun olduğundan ve CRM ortamınızda doğru olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="d0210-121">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="d0210-122">• Satış ekibiniz, CRM ortamınızda CRM kullanıcıları olarak listelenmiş olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="d0210-122">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="d0210-123">Power otomatikleştirin ortam oluşturma için gerekenler ne gerekir?</span><span class="sxs-lookup"><span data-stu-id="d0210-123">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="d0210-124">Power otomatikleştir ortamını kullanmak için şunlar gerekir:</span><span class="sxs-lookup"><span data-stu-id="d0210-124">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="d0210-125">Güç otomatikleştirme lisansı gereklidir.</span><span class="sxs-lookup"><span data-stu-id="d0210-125">A Power Automate license is required.</span></span>
- <span data-ttu-id="d0210-126">En az 1 GB depolama alanı gereklidir.</span><span class="sxs-lookup"><span data-stu-id="d0210-126">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="d0210-127">Salesforce bağlayıcıları çözümünü kullanmak için bir Dynamics 365 aboneliğine ihtiyacınız var mı?</span><span class="sxs-lookup"><span data-stu-id="d0210-127">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="d0210-128">Salesforce bağlayıcı çözümü, diğer CRM sistemleriyle eşitlemeyi destekleyen "Dynamics Flow" türüdür.</span><span class="sxs-lookup"><span data-stu-id="d0210-128">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="d0210-129">Çözüm, Dynamics 365 örneğine veya aboneliğine sahip olmanızı gerektirmez.</span><span class="sxs-lookup"><span data-stu-id="d0210-129">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="d0210-130">Salesforce çözümünü yüklerken şirketinizdeki mevcut CD 'leri içeren bir açılır liste görüntülenebilir.</span><span class="sxs-lookup"><span data-stu-id="d0210-130">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="d0210-131">Bu ortamı seçmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="d0210-131">You need to select that environment.</span></span> <span data-ttu-id="d0210-132">Ayrıca, "oturum açan kullanıcıya bağlı bir Dynamics 365 organizasyonu bulamadık" hatasını alırsanız, bağlayıcı için yeni ortam oluşturmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="d0210-132">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="d0210-133">Yapılandırma ile ilgili sorular ve yanıtlar</span><span class="sxs-lookup"><span data-stu-id="d0210-133">Questions and answers about configuration</span></span>

1. <span data-ttu-id="d0210-134">Power otomatikleştir platformunda akışları etkinleştirirken aşağıdaki hatayla karşılaşırsanız ne yapmalısınız?</span><span class="sxs-lookup"><span data-stu-id="d0210-134">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="d0210-135">Hata: Azure Resource Manager Isteği şu hatayla başarısız oldu: ' {"Error": {"Code": "WorkflowTriggerNotFound", "Message": "iş akışı ' e14d00f1-1fdf-4b1b-AAAC-54a5064093d3 ' tetikleyici ' Manual ' bulunamadı."}} '.</span><span class="sxs-lookup"><span data-stu-id="d0210-135">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="d0210-136">Bu sorun giderme adımlarını izleyin:</span><span class="sxs-lookup"><span data-stu-id="d0210-136">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="d0210-137">CD bağlantısını silin ve ardından CD bağlantılarını yeniden oluşturun.</span><span class="sxs-lookup"><span data-stu-id="d0210-137">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="d0210-138">Alt akışı kapatma ve açma</span><span class="sxs-lookup"><span data-stu-id="d0210-138">Turn the child flow off and on</span></span> 
- <span data-ttu-id="d0210-139">Çözümü silin ve çözümü yeniden yükleyin.</span><span class="sxs-lookup"><span data-stu-id="d0210-139">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="d0210-140">Power otomatikleştir platformunda bir Iş Ortağı Merkezi Bağlayıcısı eklenirken "oturum aç" hatası varsa ne yapmalısınız?</span><span class="sxs-lookup"><span data-stu-id="d0210-140">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Oturum açma gerektiren hata iletisi":::

<span data-ttu-id="d0210-142">Bu sorun giderme adımını izleyin:</span><span class="sxs-lookup"><span data-stu-id="d0210-142">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="d0210-143">Akış ortamında İş Ortağı Merkezi için kimlik bilgilerinizi kullanın (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="d0210-143">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="d0210-144">Power Automate Platform'da CRM akışına İş Ortağı Merkezi etkinleştirirken aşağıdaki hatayı alırsanız ne Power Automate gerekir?</span><span class="sxs-lookup"><span data-stu-id="d0210-144">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Güncelleştirme gerektiren hata iletisi":::

<span data-ttu-id="d0210-146">Şu sorun giderme adımlarını izleyin:</span><span class="sxs-lookup"><span data-stu-id="d0210-146">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="d0210-147">CRM akışına yönelik akışı etkinleştirmeden önce aşağıdaki iki İş Ortağı Merkezi akışı etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="d0210-147">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="d0210-148">İş Ortağı Merkezi CRM ' e - Yardımcı (Insider Önizleme)</span><span class="sxs-lookup"><span data-stu-id="d0210-148">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="d0210-149">İş Ortağı Merkezi Microsoft'un CRM'ye Ortak Satış Referans Güncelleştirmeleri (Insider Önizlemesi)</span><span class="sxs-lookup"><span data-stu-id="d0210-149">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="d0210-150">Akışı düzenlemeye çalışmadan akışa bağlantı ekleye değilken ne yapacaksınız?</span><span class="sxs-lookup"><span data-stu-id="d0210-150">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="d0210-151">Akış çalışırken akışa bağlantılar ekler ve her akışa ayrı bağlantılar eklersiniz.</span><span class="sxs-lookup"><span data-stu-id="d0210-151">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="d0210-152">Bağlantı ekleme iletişim kutusu akışı düzenlerken otomatik olarak açılmazsa, akışların adımlarını ve alt adımlarını tek tek düzenleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d0210-152">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="d0210-153">Her akışı seçin ve ayrı ayrı düzenleyin.</span><span class="sxs-lookup"><span data-stu-id="d0210-153">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="d0210-154">Akışta tüm adımları genişletin</span><span class="sxs-lookup"><span data-stu-id="d0210-154">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Bağlantı gereken adımlar":::

- <span data-ttu-id="d0210-156">Bağlantıları ilişkilendirmek ve bağlantı eklemek için bir uyarı simgesi gördüğünüz adımları seçin.</span><span class="sxs-lookup"><span data-stu-id="d0210-156">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Akışı adım adım düzenleme":::


5. <span data-ttu-id="d0210-158">Ortak Satış Referansları Bağlayıcıları çözümünün akışları açık yoksa ne yapacaksınız?</span><span class="sxs-lookup"><span data-stu-id="d0210-158">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="d0210-159">A.</span><span class="sxs-lookup"><span data-stu-id="d0210-159">A.</span></span> <span data-ttu-id="d0210-160">Bu Power Automate, akışları aşağıdaki sırayla düzenlemeniz ve doğru bağlantıları kullanmak üzere güncelleştirmeniz gerekir:</span><span class="sxs-lookup"><span data-stu-id="d0210-160">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="d0210-161">İş Ortağı Merkezi Web Kancası Kaydı (Insider Önizlemesi)</span><span class="sxs-lookup"><span data-stu-id="d0210-161">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="d0210-162">Ortak satış başvurusu oluşturma-Salesforce 'a Iş Ortağı Merkezi 'ne (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="d0210-162">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="d0210-163">İş Ortağı Merkezi Microsoft ortak-başvuru güncelleştirmelerini Salesforce 'a satma (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="d0210-163">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="d0210-164">İş ortağı merkezini Salesforce 'a (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="d0210-164">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="d0210-165">Salesforce-Iş Ortağı Merkezi (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="d0210-165">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="d0210-166">Salesforce Iş Ortağı Merkezi (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="d0210-166">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="d0210-167">Salesforce Microsoft çözümlerini Iş Ortağı Merkezi 'ne (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="d0210-167">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="d0210-168">B.</span><span class="sxs-lookup"><span data-stu-id="d0210-168">B.</span></span> <span data-ttu-id="d0210-169">Her akış için **yalnızca kullanıcıları Çalıştır** seçeneğini belirleyin.</span><span class="sxs-lookup"><span data-stu-id="d0210-169">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="d0210-170">**Yalnızca çalıştırma kullanıcısı tarafından sağlanarak** **bağlantı kullan** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="d0210-170">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Bir akışı etkinleştirmek için":::


<span data-ttu-id="d0210-172">C.</span><span class="sxs-lookup"><span data-stu-id="d0210-172">C.</span></span> <span data-ttu-id="d0210-173">Bu yukarıda belirtilen akışlara aşağıdaki akışları etkinleştirin:</span><span class="sxs-lookup"><span data-stu-id="d0210-173">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="d0210-174">İş Ortağı Merkezi Microsoft ortak-başvuru güncelleştirmelerini Salesforce 'a satma (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="d0210-174">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="d0210-175">Salesforce-Iş Ortağı Merkezi (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="d0210-175">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="d0210-176">D.</span><span class="sxs-lookup"><span data-stu-id="d0210-176">D.</span></span> <span data-ttu-id="d0210-177">Kalan tüm akışları etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="d0210-177">Activate all the remaining flows.</span></span>

<span data-ttu-id="d0210-178">E.</span><span class="sxs-lookup"><span data-stu-id="d0210-178">E.</span></span> <span data-ttu-id="d0210-179">Flow Iş Ortağı Merkezi Web kancası kaydında **Çalıştır**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="d0210-179">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="d0210-180">**Iş Ortağı Merkezi** 'ndeki Ilk eylemden Salesforce akışına **http url 'sini** sağlayın.</span><span class="sxs-lookup"><span data-stu-id="d0210-180">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="d0210-181">**Kaydolmak Için olaylar** bölümündeki tüm dört seçeneği seçin ve üzerine yazmak için **Evet** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="d0210-181">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="d0210-182">Çalıştırma/bakım ile ilgili sorular ve yanıtlar</span><span class="sxs-lookup"><span data-stu-id="d0210-182">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="d0210-183">Power otomatikleştirin akış yürütme sırasında hatalardan nasıl sorun giderilir?</span><span class="sxs-lookup"><span data-stu-id="d0210-183">How do you troubleshoot failures during Power Automate flow execution?</span></span>

<span data-ttu-id="d0210-184">Güç otomatikleştirebileceğiniz akışlarınızın beklenen şekilde çalıştığından emin olmak ve yürütme sırasında hataların sorunlarını gidermek için bkz. [akış başarısızlıklarını](/power-automate/fix-flow-failures)giderme.</span><span class="sxs-lookup"><span data-stu-id="d0210-184">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="d0210-185">Iş ortağı merkezi veya CRM ortamında düzgün şekilde eşitlenmemiş başvurular görürseniz ne yapmalısınız?</span><span class="sxs-lookup"><span data-stu-id="d0210-185">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="d0210-186">Referans eşitleme durumunu belirlemek için Denetle'yi **seçin.**</span><span class="sxs-lookup"><span data-stu-id="d0210-186">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Referansları eşitleme":::

<span data-ttu-id="d0210-188">Aşağıdaki koşulların karşı olduğundan emin olmak:</span><span class="sxs-lookup"><span data-stu-id="d0210-188">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="d0210-189">Çözüm kimliği, fırsatın bir parçası olarak sağlanır.</span><span class="sxs-lookup"><span data-stu-id="d0210-189">Solution ID is provided as part of the opportunity.</span></span>

- <span data-ttu-id="d0210-190">İki harfli ülke kodu gereklidir.</span><span class="sxs-lookup"><span data-stu-id="d0210-190">Two letter country code is required.</span></span>

- <span data-ttu-id="d0210-191">Fırsat için Microsoft'tan yardım seçildiğinde müşteri iletişim bilgileri gereklidir.</span><span class="sxs-lookup"><span data-stu-id="d0210-191">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="d0210-192">Bir referansın çift yönlü olarak eşitlenmesi nasıl sağlandı?</span><span class="sxs-lookup"><span data-stu-id="d0210-192">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="d0210-193">Aşağıdaki adımları uygulayın:</span><span class="sxs-lookup"><span data-stu-id="d0210-193">Do the following steps:</span></span>

- <span data-ttu-id="d0210-194">İş ortağı satıcılarının CRM bölümünde İş Ortağı Merkezi **eşitle seçeneğini etkinleştirmiş** olduğundan emin olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="d0210-194">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Eşitleme'yi etkinleştirildiğinden emin olun":::

- <span data-ttu-id="d0210-196">Satış satıcılarının müşteri adayını kabul etmek için gelir ve kapanış tarihi sağlamaları gerekir.</span><span class="sxs-lookup"><span data-stu-id="d0210-196">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="d0210-197">CRM Kimliği ortak satış  fırsatının oluşturma veya güncelleştirme aşamasında sağlanıyorsa ancak CRM'de bu kimliğin bulunduğu bir müşteri adayı fırsatı yoksayılırsa güncelleştirme veya oluşturma yoksayılır. </span><span class="sxs-lookup"><span data-stu-id="d0210-197">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="d0210-198">Referans para birimi alanını Salesforce ortamında yapılandırıldığından emin olmak.</span><span class="sxs-lookup"><span data-stu-id="d0210-198">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="d0210-199">Bağlayıcının bağlantısı kesilirse ve referans eşitlemesini kaçırırsanız ne yapacaksınız?</span><span class="sxs-lookup"><span data-stu-id="d0210-199">What should you do if the connector gets disconnected and you miss a referral synchronization.?</span></span>

<span data-ttu-id="d0210-200">Deneyebilirsiniz seçeneklerden birkaçı şunlardır:</span><span class="sxs-lookup"><span data-stu-id="d0210-200">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="d0210-201">Referans yöneticisi rollerine sahip kullanıcı adı veya parolanın İş Ortağı Merkezi olup olmadığını kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="d0210-201">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="d0210-202">Eşitlenmemiş fırsata gidebilir, küçük bir güncelleştirme gerçekleştirip referansın eşitlenmiş olup olmadığını gözlemlersiniz.</span><span class="sxs-lookup"><span data-stu-id="d0210-202">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="d0210-203">Akışlar çalıştırlı ve başarısız olmuşsa akışı seçin ve başarısız olan çalıştırmayı yeniden gönderin.</span><span class="sxs-lookup"><span data-stu-id="d0210-203">If the flows have run and failed, then select the flow and re-submit the run that has failed.</span></span>

5. <span data-ttu-id="d0210-204">Erişim reddedildi hatalarına sahip olursanız ne yapacaksınız?</span><span class="sxs-lookup"><span data-stu-id="d0210-204">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="d0210-205">Uygun rollerin mevcut olduğundan emin olun</span><span class="sxs-lookup"><span data-stu-id="d0210-205">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="d0210-206">Iş Ortağı Merkezi satıcı için başvuru Yöneticisi rolü</span><span class="sxs-lookup"><span data-stu-id="d0210-206">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="d0210-207">CRM örneğiniz üzerinde sistem yöneticisi veya sistem özelleştirici rolü</span><span class="sxs-lookup"><span data-stu-id="d0210-207">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="d0210-208">Power otomatikleştirmenin akış hesabı kullanıcısının https://flow.microsoft.com önceden en az bir kez oturum açtığına sahip olduğundan emin olun</span><span class="sxs-lookup"><span data-stu-id="d0210-208">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="d0210-209">Ortak satış fırsatı oluştururken **müşteri hesabı ülke kodunun** eksik olduğunu görürseniz, ne yapmanız gerekir?</span><span class="sxs-lookup"><span data-stu-id="d0210-209">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="d0210-210">ISO 'nın iki harfli ülke kodunu CRM 'de müşteri hesabına eklemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="d0210-210">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="d0210-211">Ortak satış fırsatı oluştururken **Çözüm Kimliği 'nin gerekli** olduğu hatayı görürseniz ne yapmanız gerekir?</span><span class="sxs-lookup"><span data-stu-id="d0210-211">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="d0210-212">Ortak satış başvurusu oluşturmak için, Microsoft ortak satış için kullanabileceğiniz bir çözüme ihtiyacınız vardır.</span><span class="sxs-lookup"><span data-stu-id="d0210-212">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="d0210-213">Iş akışı hatası olmasa dahi, Iş Ortağı Merkezi 'nde oluşturulmuş ortak satış fırsatlarını gördüğünüzde ne yapmalısınız?</span><span class="sxs-lookup"><span data-stu-id="d0210-213">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors?</span></span>

<span data-ttu-id="d0210-214">Şunları yapın:</span><span class="sxs-lookup"><span data-stu-id="d0210-214">Do the following:</span></span>

- <span data-ttu-id="d0210-215">Iş Ortağı Merkezi 'nde yeni bir ortak satış sorunu oluşturduktan sonra, Dynamics 365 Flow Iş Ortağı Merkezi 'nin çağrılacağını (birden çok kez çağrılabilir) denetleyin.</span><span class="sxs-lookup"><span data-stu-id="d0210-215">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="d0210-216">Akış çağrılırsa, tüm çağrılan Akışlar ' ı işaretleyin ve bu, CRM 'yi güncelleştiren akış çalıştırmasını belirler.</span><span class="sxs-lookup"><span data-stu-id="d0210-216">If the flow gets invoked, check all invoked flows, and identify the flow run which that would update the CRM.</span></span> <span data-ttu-id="d0210-217">Eylemleri izleyebilir ve CRM 'yi güncelleştirip güncelleştirmediğinizi veya bir sorunla karşılaştıysanız emin olabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d0210-217">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="d0210-218">CRM KIMLIĞIYLE doldurulup doldurulmadığını görmek için Iş Ortağı Merkezi 'nde **yeni anlaşmayı** denetleyin.</span><span class="sxs-lookup"><span data-stu-id="d0210-218">Check **New deal** in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="d0210-219">Iş Ortağı Merkezi 'nde, anlaşmayı **kazanıldı** veya **kaybedildi** olarak kapanmadığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="d0210-219">Make sure that the deal is not accidentally closed as **Won** or **Lost** in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d0210-220">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="d0210-220">Next steps</span></span>

- [<span data-ttu-id="d0210-221">Müşteri adaylarını yönetme</span><span class="sxs-lookup"><span data-stu-id="d0210-221">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="d0210-222">Ortak satış fırsatlarını yönetme</span><span class="sxs-lookup"><span data-stu-id="d0210-222">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
