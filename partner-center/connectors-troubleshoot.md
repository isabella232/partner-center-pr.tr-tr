---
title: Ortak satış başvuruları bağlayıcıları sorunlarını giderme
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ortak satış bağlayıcıları kullanma hakkında sık sorulan soruların yanıtlarını öğrenin. Ortak satış bağlayıcılarının sorunlarını giderme hakkında bilgi edinmek için bu SSS bölümüne bakın.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 988a696a8a0a0abb4d37e3915c76f905ec5b35b0
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/14/2020
ms.locfileid: "92531890"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="38ab7-104">Ortak satış başvuruları bağlayıcıları sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="38ab7-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="38ab7-105">**Aşağıdakiler cihazlar için geçerlidir:**</span><span class="sxs-lookup"><span data-stu-id="38ab7-105">**Applies to:**</span></span>

- <span data-ttu-id="38ab7-106">İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="38ab7-106">Partner Center</span></span>
- <span data-ttu-id="38ab7-107">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="38ab7-107">Dynamics 365 CRM</span></span>
- <span data-ttu-id="38ab7-108">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="38ab7-108">Salesforce CRM</span></span>

<span data-ttu-id="38ab7-109">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="38ab7-109">**Appropriate roles**</span></span>

- <span data-ttu-id="38ab7-110">Başvuru Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="38ab7-110">Referrals admin</span></span>
- <span data-ttu-id="38ab7-111">CRM 'de Sistem Yöneticisi veya sistem özelleştiricisi</span><span class="sxs-lookup"><span data-stu-id="38ab7-111">System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="38ab7-112">Ön koşullar hakkında sorular ve yanıtlar</span><span class="sxs-lookup"><span data-stu-id="38ab7-112">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="38ab7-113">Ortamınız için bir deneme ortak satışı başvuruları Bağlayıcısı çözümü kullanabilir miyim?</span><span class="sxs-lookup"><span data-stu-id="38ab7-113">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="38ab7-114">Test/hazırlama ortamındaysanız, deneme çözümünü kabul edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="38ab7-114">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="38ab7-115">Bağlayıcıların ücretli sürümü, AppSource 'ta ABD $15/ay 'da bulunabilir.</span><span class="sxs-lookup"><span data-stu-id="38ab7-115">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="38ab7-116">Ücretli bağlantıyla, günde 10.000 API çağrısı elde edersiniz.</span><span class="sxs-lookup"><span data-stu-id="38ab7-116">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="38ab7-117">Bağlayıcılar, Iş ortağı merkezi başvuru API 'lerinin en üstünde sarmalayıcılardır.</span><span class="sxs-lookup"><span data-stu-id="38ab7-117">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="38ab7-118">Her iki Iş ortağı merkezi veya CRM tarafında fırsatlarda bir **oluşturma** veya **güncelleştirme** olayı için BAĞLAYıCı çözümleri çalıştırıldığında bir API çağrısı yapılır.</span><span class="sxs-lookup"><span data-stu-id="38ab7-118">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="38ab7-119">CRM ortamında bölüm oluşturmak için hangi rolü kullanmanız gerekir?</span><span class="sxs-lookup"><span data-stu-id="38ab7-119">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="38ab7-120">Sistem yöneticileri veya sistem özelleştiricileri olan kullanıcılar herkes için değişiklik uygulayabilir.</span><span class="sxs-lookup"><span data-stu-id="38ab7-120">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="38ab7-121">Ancak tüm uygulama kullanıcıları, sistemi kişiselleştirebilir ve hatta bazı özelleştirmelerini başkalarıyla paylaşabilir.</span><span class="sxs-lookup"><span data-stu-id="38ab7-121">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="38ab7-122">İş ortağı satıcıları iş ortağı merkezi 'nde çalışmak için özel rollere ihtiyaç duyuyor mu?</span><span class="sxs-lookup"><span data-stu-id="38ab7-122">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="38ab7-123">İş ortağı satıcılara "başvuru Yöneticisi" rolü atanmalıdır.</span><span class="sxs-lookup"><span data-stu-id="38ab7-123">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="38ab7-124">Daha fazla bilgi için, şu [Izinlere genel bakış) bakın (oluşturma-Kullanıcı-hesaplar-ve-ayarla-izinler).</span><span class="sxs-lookup"><span data-stu-id="38ab7-124">For more information, refer to the following [Permissions overview)(create-user-accounts-and-set-permissions).</span></span>

4. <span data-ttu-id="38ab7-125">CRM ortamınızda ilk olarak hangi alanların ayarlanması gerekir?</span><span class="sxs-lookup"><span data-stu-id="38ab7-125">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="38ab7-126">• Para biriminiz konumunuza uygun olduğundan ve CRM ortamınızda doğru olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="38ab7-126">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="38ab7-127">• Satış ekibiniz, CRM ortamınızda CRM kullanıcıları olarak listelenmiş olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="38ab7-127">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="38ab7-128">Power otomatikleştirin ortam oluşturma için gerekenler ne gerekir?</span><span class="sxs-lookup"><span data-stu-id="38ab7-128">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="38ab7-129">Power otomatikleştir ortamını kullanmak için şunlar gerekir:</span><span class="sxs-lookup"><span data-stu-id="38ab7-129">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="38ab7-130">Güç otomatikleştirme lisansı gereklidir.</span><span class="sxs-lookup"><span data-stu-id="38ab7-130">A Power Automate license is required.</span></span>
- <span data-ttu-id="38ab7-131">En az 1 GB depolama alanı gereklidir.</span><span class="sxs-lookup"><span data-stu-id="38ab7-131">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="38ab7-132">Salesforce bağlayıcıları çözümünü kullanmak için bir Dynamics 365 aboneliğine ihtiyacınız var mı?</span><span class="sxs-lookup"><span data-stu-id="38ab7-132">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="38ab7-133">Salesforce bağlayıcı çözümü, diğer CRM sistemleriyle eşitlemeyi destekleyen "Dynamics Flow" türüdür.</span><span class="sxs-lookup"><span data-stu-id="38ab7-133">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="38ab7-134">Çözüm, Dynamics 365 örneğine veya aboneliğine sahip olmanızı gerektirmez.</span><span class="sxs-lookup"><span data-stu-id="38ab7-134">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="38ab7-135">Salesforce çözümünü yüklerken şirketinizdeki mevcut CD 'leri içeren bir açılır liste görüntülenebilir.</span><span class="sxs-lookup"><span data-stu-id="38ab7-135">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="38ab7-136">Bu ortamı seçmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="38ab7-136">You need to select that environment.</span></span> <span data-ttu-id="38ab7-137">Ayrıca, "oturum açan kullanıcıya bağlı bir Dynamics 365 organizasyonu bulamadık" hatasını alırsanız, bağlayıcı için yeni ortam oluşturmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="38ab7-137">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="38ab7-138">Yapılandırma ile ilgili sorular ve yanıtlar</span><span class="sxs-lookup"><span data-stu-id="38ab7-138">Questions and answers about configuration</span></span>

1. <span data-ttu-id="38ab7-139">Power otomatikleştir platformunda akışları etkinleştirirken aşağıdaki hatayla karşılaşırsanız ne yapmalısınız?</span><span class="sxs-lookup"><span data-stu-id="38ab7-139">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="38ab7-140">Hata: Azure Resource Manager Isteği şu hatayla başarısız oldu: ' {"Error": {"Code": "WorkflowTriggerNotFound", "Message": "iş akışı ' e14d00f1-1fdf-4b1b-AAAC-54a5064093d3 ' tetikleyici ' Manual ' bulunamadı."}} '.</span><span class="sxs-lookup"><span data-stu-id="38ab7-140">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="38ab7-141">Bu sorun giderme adımlarını izleyin:</span><span class="sxs-lookup"><span data-stu-id="38ab7-141">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="38ab7-142">CD bağlantısını silin ve ardından CD bağlantılarını yeniden oluşturun.</span><span class="sxs-lookup"><span data-stu-id="38ab7-142">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="38ab7-143">Alt akışı kapatma ve açma</span><span class="sxs-lookup"><span data-stu-id="38ab7-143">Turn the child flow off and on</span></span> 
- <span data-ttu-id="38ab7-144">Çözümü silin ve çözümü yeniden yükleyin.</span><span class="sxs-lookup"><span data-stu-id="38ab7-144">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="38ab7-145">Power otomatikleştir platformunda bir Iş Ortağı Merkezi Bağlayıcısı eklenirken "oturum aç" hatası varsa ne yapmalısınız?</span><span class="sxs-lookup"><span data-stu-id="38ab7-145">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Oturum açma gerektiren hata iletisi":::

<span data-ttu-id="38ab7-147">Bu sorun giderme adımını izleyin:</span><span class="sxs-lookup"><span data-stu-id="38ab7-147">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="38ab7-148">Iş ortağı merkezi kimlik bilgilerinizi kullanarak Flow ortamında bir kez oturum açın (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="38ab7-148">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="38ab7-149">Power otomatikleştir platformunda Iş ortağı merkezini CRM akışına etkinleştirirken aşağıdaki hatayı alırsanız ne yapmalısınız?</span><span class="sxs-lookup"><span data-stu-id="38ab7-149">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Güncelleştirme gerektiren hata iletisi":::

<span data-ttu-id="38ab7-151">Bu sorun giderme adımlarını izleyin:</span><span class="sxs-lookup"><span data-stu-id="38ab7-151">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="38ab7-152">Iş ortağı merkezini CRM akışına etkinleştirmeden önce aşağıdaki iki alt akışı etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="38ab7-152">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="38ab7-153">İş Ortağı Merkezi 'ne CRM Yardımcısı (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="38ab7-153">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="38ab7-154">İş Ortağı Merkezi Microsoft ortak-CRM 'ye başvuru güncelleştirmeleri satma (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="38ab7-154">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="38ab7-155">Akışı düzenlemeye çalıştığınızda akışla bağlantı ekleyemeyebilirsiniz ne yapmalısınız?</span><span class="sxs-lookup"><span data-stu-id="38ab7-155">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="38ab7-156">Akış çalışırken akışa bağlantı ekler ve her bir akışa ayrı olarak eklersiniz.</span><span class="sxs-lookup"><span data-stu-id="38ab7-156">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="38ab7-157">Bağlantı ekleme iletişim kutusu akışı düzenlerken otomatik olarak açılmazsa, akışların her birini ve alt adımını ayrı ayrı düzenleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="38ab7-157">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="38ab7-158">Her bir akışı seçin ve tek tek düzenleyin.</span><span class="sxs-lookup"><span data-stu-id="38ab7-158">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="38ab7-159">Akıştaki tüm adımları Genişlet</span><span class="sxs-lookup"><span data-stu-id="38ab7-159">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Bağlantı gerektiren adımlar":::

- <span data-ttu-id="38ab7-161">Bağlantıları ilişkilendirmek ve bağlantı eklemek isteyen bir uyarı simgesi gördüğünüz adımları seçin.</span><span class="sxs-lookup"><span data-stu-id="38ab7-161">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Adıma göre akış adımını Düzenle":::


5. <span data-ttu-id="38ab7-163">Ortak satış başvuruları bağlayıcılar çözümünün akışları açık değilse ne yapmalısınız?</span><span class="sxs-lookup"><span data-stu-id="38ab7-163">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="38ab7-164">A.</span><span class="sxs-lookup"><span data-stu-id="38ab7-164">A.</span></span> <span data-ttu-id="38ab7-165">Power otomatikleştirmede akışları aşağıdaki sırayla düzenlemeniz ve doğru bağlantıları kullanacak şekilde güncelleştirmeniz gerekir:</span><span class="sxs-lookup"><span data-stu-id="38ab7-165">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="38ab7-166">İş Ortağı Merkezi Web kancası kaydı (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="38ab7-166">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="38ab7-167">Ortak satış başvurusu oluşturma-Salesforce 'a Iş Ortağı Merkezi 'ne (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="38ab7-167">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="38ab7-168">İş Ortağı Merkezi Microsoft ortak-başvuru güncelleştirmelerini Salesforce 'a satma (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="38ab7-168">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="38ab7-169">İş ortağı merkezini Salesforce 'a (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="38ab7-169">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="38ab7-170">Salesforce-Iş Ortağı Merkezi (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="38ab7-170">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="38ab7-171">Salesforce Iş Ortağı Merkezi (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="38ab7-171">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="38ab7-172">Salesforce Microsoft çözümlerini Iş Ortağı Merkezi 'ne (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="38ab7-172">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="38ab7-173">B.</span><span class="sxs-lookup"><span data-stu-id="38ab7-173">B.</span></span> <span data-ttu-id="38ab7-174">Her akış için **yalnızca kullanıcıları Çalıştır** seçeneğini belirleyin.</span><span class="sxs-lookup"><span data-stu-id="38ab7-174">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="38ab7-175">**Yalnızca çalıştırma kullanıcısı tarafından sağlanarak** **bağlantı kullan** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="38ab7-175">Select **Use connection** instead of **Provided by run-only user** .</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Bir akışı etkinleştirmek için":::


<span data-ttu-id="38ab7-177">C.</span><span class="sxs-lookup"><span data-stu-id="38ab7-177">C.</span></span> <span data-ttu-id="38ab7-178">Bu yukarıda belirtilen akışlara aşağıdaki akışları etkinleştirin:</span><span class="sxs-lookup"><span data-stu-id="38ab7-178">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="38ab7-179">İş Ortağı Merkezi Microsoft ortak-başvuru güncelleştirmelerini Salesforce 'a satma (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="38ab7-179">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="38ab7-180">Salesforce-Iş Ortağı Merkezi (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="38ab7-180">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="38ab7-181">D.</span><span class="sxs-lookup"><span data-stu-id="38ab7-181">D.</span></span> <span data-ttu-id="38ab7-182">Kalan tüm akışları etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="38ab7-182">Activate all the remaining flows.</span></span>

<span data-ttu-id="38ab7-183">E.</span><span class="sxs-lookup"><span data-stu-id="38ab7-183">E.</span></span> <span data-ttu-id="38ab7-184">Flow Iş Ortağı Merkezi Web kancası kaydında **Çalıştır** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="38ab7-184">At flow Partner Center Webhook Registration, select **Run** .</span></span> <span data-ttu-id="38ab7-185">**Iş Ortağı Merkezi** 'ndeki Ilk eylemden Salesforce akışına **http url 'sini** sağlayın.</span><span class="sxs-lookup"><span data-stu-id="38ab7-185">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="38ab7-186">**Kaydolmak Için olaylar** bölümündeki tüm dört seçeneği seçin ve üzerine yazmak için **Evet** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="38ab7-186">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="38ab7-187">Çalıştırma/bakım ile ilgili sorular ve yanıtlar</span><span class="sxs-lookup"><span data-stu-id="38ab7-187">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="38ab7-188">Güç otomatikleştirme akış yürütmesi sırasında oluşan hatalarda nasıl sorun giderilir?</span><span class="sxs-lookup"><span data-stu-id="38ab7-188">How do you troubleshoot in case of failures during Power Automate flow execution?</span></span>

<span data-ttu-id="38ab7-189">Güç otomatikleştirebileceğiniz akışlarınızın beklenen şekilde çalıştığından emin olmak ve yürütme sırasında hataların sorunlarını gidermek için bkz. [akış başarısızlıklarını](/power-automate/fix-flow-failures)giderme.</span><span class="sxs-lookup"><span data-stu-id="38ab7-189">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="38ab7-190">Iş ortağı merkezi veya CRM ortamında düzgün şekilde eşitlenmemiş başvurular görürseniz ne yapmalısınız?</span><span class="sxs-lookup"><span data-stu-id="38ab7-190">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="38ab7-191">Başvuru eşitlemesinin durumunu belirlemek için **Denetim** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="38ab7-191">To determine the status of referral synchronization, select **Audit** .</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Başvuruları senkronize etme":::

<span data-ttu-id="38ab7-193">Aşağıdaki koşulların karşılandığından emin olun:</span><span class="sxs-lookup"><span data-stu-id="38ab7-193">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="38ab7-194">Çözüm kimliği, fırsatın bir parçası olarak sağlanır.</span><span class="sxs-lookup"><span data-stu-id="38ab7-194">Solution id is provided as part of the opportunity.</span></span>

- <span data-ttu-id="38ab7-195">İki harfli ülke kodu gereklidir.</span><span class="sxs-lookup"><span data-stu-id="38ab7-195">Two letter country code is required.</span></span>

- <span data-ttu-id="38ab7-196">Fırsat için Microsoft 'tan yardım seçiliyken müşteri iletişim bilgileri gereklidir.</span><span class="sxs-lookup"><span data-stu-id="38ab7-196">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="38ab7-197">Bir başvurunun çift yönlü olarak eşitlenmesini sağlamak mı istiyorsunuz?</span><span class="sxs-lookup"><span data-stu-id="38ab7-197">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="38ab7-198">Aşağıdaki adımları uygulayın:</span><span class="sxs-lookup"><span data-stu-id="38ab7-198">Do the following steps:</span></span>

- <span data-ttu-id="38ab7-199">İş ortaklarının satıcıları, CRM bölümündeki **Iş Ortağı Merkezi Ile eşitlemeyi** etkinleştirdiklerinden emin olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="38ab7-199">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Eşitleme özelliğinin etkinleştirildiğinden emin olun":::

- <span data-ttu-id="38ab7-201">Satıcıların bir müşteri adayını nitelerken gelir ve kapanış tarihi sağlaması gerekir.</span><span class="sxs-lookup"><span data-stu-id="38ab7-201">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="38ab7-202">Ortak satış fırsatının **Oluştur** veya **GÜNCELLEŞTIR** aşamasında CRM kimliği SAĞLANMıŞSA, ancak bu kimliğe sahip BIR müşteri adayı fırsatı CRM 'de bulunamazsa güncelleştirme veya oluşturma yok sayılır.</span><span class="sxs-lookup"><span data-stu-id="38ab7-202">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="38ab7-203">Başvuru para birimi alanının Salesforce ortamında yapılandırıldığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="38ab7-203">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="38ab7-204">Bağlayıcının bağlantısı kesilirse ve bir başvuru eşitlemesini kaçırdıysanız ne yapmalısınız?</span><span class="sxs-lookup"><span data-stu-id="38ab7-204">What should you do if the connector gets disconnected and you miss a referral synchronization.</span></span> 

<span data-ttu-id="38ab7-205">Deneyebileceğiniz seçeneklerden bazıları aşağıda verilmiştir:</span><span class="sxs-lookup"><span data-stu-id="38ab7-205">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="38ab7-206">Iş Ortağı Merkezi kullanıcısı için başvuru yöneticisi rollerine sahip kullanıcı adının veya parolanın dolup dolmadığını denetleyin.</span><span class="sxs-lookup"><span data-stu-id="38ab7-206">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="38ab7-207">Eşitlenmemiş fırsata gidebilir, küçük bir güncelleştirme yapabilir ve başvurunun eşitlenip eşitlenmediğini gözlemleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="38ab7-207">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="38ab7-208">Akışlar çalıştırılmışsa ve başarısız olursa, akışı seçip başarısız olan çalıştırmayı yeniden gönderebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="38ab7-208">If the flows have run and failed, then select the flow and re-submit the run which has failed.</span></span>

5. <span data-ttu-id="38ab7-209">Erişim reddedildi hatalarını aldığınızda ne yapmalısınız?</span><span class="sxs-lookup"><span data-stu-id="38ab7-209">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="38ab7-210">Uygun rollerin mevcut olduğundan emin olun</span><span class="sxs-lookup"><span data-stu-id="38ab7-210">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="38ab7-211">Iş Ortağı Merkezi satıcı için başvuru Yöneticisi rolü</span><span class="sxs-lookup"><span data-stu-id="38ab7-211">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="38ab7-212">CRM örneğiniz üzerinde sistem yöneticisi veya sistem özelleştirici rolü</span><span class="sxs-lookup"><span data-stu-id="38ab7-212">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="38ab7-213">Power otomatikleştirmenin akış hesabı kullanıcısının https://flow.microsoft.com önceden en az bir kez oturum açtığına sahip olduğundan emin olun</span><span class="sxs-lookup"><span data-stu-id="38ab7-213">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="38ab7-214">Ortak satış fırsatı oluştururken **müşteri hesabı ülke kodunun** eksik olduğunu görürseniz, ne yapmanız gerekir?</span><span class="sxs-lookup"><span data-stu-id="38ab7-214">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="38ab7-215">ISO 'nın iki harfli ülke kodunu CRM 'de müşteri hesabına eklemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="38ab7-215">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="38ab7-216">Ortak satış fırsatı oluştururken **Çözüm Kimliği 'nin gerekli** olduğu hatayı görürseniz ne yapmanız gerekir?</span><span class="sxs-lookup"><span data-stu-id="38ab7-216">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="38ab7-217">Ortak satış başvurusu oluşturmak için, Microsoft ortak satış için kullanabileceğiniz bir çözüme ihtiyacınız vardır.</span><span class="sxs-lookup"><span data-stu-id="38ab7-217">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="38ab7-218">Iş Ortağı Merkezi 'nde oluşturulan ortak satış fırsatlarını, hiçbir akış hatası olmasa dahi, CRM ile eşitlenmemiş olan bir şekilde gördüğünüzde ne yapmalısınız:</span><span class="sxs-lookup"><span data-stu-id="38ab7-218">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors:</span></span>

<span data-ttu-id="38ab7-219">Şunları yapın:</span><span class="sxs-lookup"><span data-stu-id="38ab7-219">Do the following:</span></span>

- <span data-ttu-id="38ab7-220">Iş Ortağı Merkezi 'nde yeni bir ortak satış sorunu oluşturduktan sonra, Dynamics 365 Flow Iş Ortağı Merkezi 'nin çağrılacağını (birden çok kez çağrılabilir) denetleyin.</span><span class="sxs-lookup"><span data-stu-id="38ab7-220">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="38ab7-221">Akış çağrılırsa, tüm çağrılan Akışlar ' ı işaretleyin ve bu, CRM 'yi güncelleştiren akış çalıştırmasını belirler.</span><span class="sxs-lookup"><span data-stu-id="38ab7-221">If the flow gets invoked, check all invoked flows, and identify the flow run which would update the CRM.</span></span> <span data-ttu-id="38ab7-222">Eylemleri izleyebilir ve CRM 'yi güncelleştirip güncelleştirmediğinizi veya bir sorunla karşılaştıysanız emin olabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="38ab7-222">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="38ab7-223">CRM KIMLIĞIYLE doldurulup doldurulmadığını görmek için Iş Ortağı Merkezi 'nde *yeni anlaşmayı* denetleyin.</span><span class="sxs-lookup"><span data-stu-id="38ab7-223">Check *New deal* \* in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="38ab7-224">Iş Ortağı Merkezi 'nde, anlaşmayı "kazanıldı" veya "kaybedildi" olarak kapanmadığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="38ab7-224">Make sure that the deal is not accidentally closed as “Won” or “Lost” in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="38ab7-225">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="38ab7-225">Next steps</span></span>

- [<span data-ttu-id="38ab7-226">Müşteri adaylarını yönetme</span><span class="sxs-lookup"><span data-stu-id="38ab7-226">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="38ab7-227">Ortak satış fırsatlarını yönetme</span><span class="sxs-lookup"><span data-stu-id="38ab7-227">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)