---
title: Karşılaştırma dosyalarınızı kullanın
ms.topic: article
ms.date: 03/10/2021
description: Iş Ortağı Merkezi 'nde mutabakat dosyaları ve belirli bir faturalandırma döngüsünün ücretlendirdiği ayrıntılı, satır öğesi görünümlerinin nasıl yorumlanacağı hakkında bilgi edinin.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e6b9e466402d71c988729052bd72ba2346a9d977
ms.sourcegitcommit: 868f90c54f26a037eee29749c207a7316bb4b475
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "103022783"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="607bd-103">Iş Ortağı Merkezi mutabakatı dosyalarınızda satır öğelerini okumayı öğrenin</span><span class="sxs-lookup"><span data-stu-id="607bd-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="607bd-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="607bd-104">**Appropriate roles**</span></span>

- <span data-ttu-id="607bd-105">Faturalama yöneticisi</span><span class="sxs-lookup"><span data-stu-id="607bd-105">Billing admin</span></span>
- <span data-ttu-id="607bd-106">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="607bd-106">Global admin</span></span>

<span data-ttu-id="607bd-107">Bir fatura döngüsündeki her bir ücret için ayrıntılı, satır öğesi görünümü için Iş Ortağı Merkezi ' nden mutabakat dosyalarınızı indirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="607bd-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="607bd-108">Satır öğesi ayrıntıları, her bir müşterinin aboneliğine ilişkin ücretleri ve ayrıntılı olayları (bir aboneliğe yönelik bir abonelik için orta dönem ekleme gibi) içerir.</span><span class="sxs-lookup"><span data-stu-id="607bd-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="607bd-109">**Faturanızı** okuma hakkında daha fazla bilgi için bkz. [faturanızı okuyun](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="607bd-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="607bd-110">Mutabakat dosyası alanlarını anlama</span><span class="sxs-lookup"><span data-stu-id="607bd-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="607bd-111">Lisans tabanlı mutabakat dosyası alanları</span><span class="sxs-lookup"><span data-stu-id="607bd-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="607bd-112">Kullanım tabanlı mutabakat dosyası alanları</span><span class="sxs-lookup"><span data-stu-id="607bd-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="607bd-113">Günlük fiyatlandırılan kullanım mutabakat dosyası alanları</span><span class="sxs-lookup"><span data-stu-id="607bd-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="607bd-114">Bir kerelik satın alma CSP 'si mutabakatı dosya alanları</span><span class="sxs-lookup"><span data-stu-id="607bd-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="607bd-115">Mutabakat dosyalarındaki ücretlendirme türlerini anlama</span><span class="sxs-lookup"><span data-stu-id="607bd-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="607bd-116">Mutabakat dosyalarındaki ( **Chargetype** sütunu) ücret türlerini anlamak için bkz. [mutabakatı dosya ücreti türleri](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="607bd-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="607bd-117">Biçimlendirme sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="607bd-117">Fix formatting issues</span></span>

<span data-ttu-id="607bd-118">Bazen bir mutabakat dosyasında biçimlendirme sorunları bulunabilir.</span><span class="sxs-lookup"><span data-stu-id="607bd-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="607bd-119">Örneğin, en-US yerel ayarı kullanılmazsa bu sorun oluşabilir.</span><span class="sxs-lookup"><span data-stu-id="607bd-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="607bd-120">Mutabakat dosyalarınızda biçimlendirme sorunlarını gidermek için aşağıdaki adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="607bd-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="607bd-121">Microsoft Excel 'de mutabakat dosyasını (. csv biçiminde) açın.</span><span class="sxs-lookup"><span data-stu-id="607bd-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="607bd-122">Dosyadaki ilk sütunu seçin.</span><span class="sxs-lookup"><span data-stu-id="607bd-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="607bd-123">**Metni sütunlara dönüştürme Sihirbazı**' nı açın.</span><span class="sxs-lookup"><span data-stu-id="607bd-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="607bd-124">Şeritte, **veriler**' i seçin ve **sütunlar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="607bd-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="607bd-125">Sihirbazda, **ayrılmış dosya türü**' nü seçin.</span><span class="sxs-lookup"><span data-stu-id="607bd-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="607bd-126">Ardından **İleri**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="607bd-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="607bd-127">**Sınırlayıcılar** alanında **virgül**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="607bd-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="607bd-128">( **Sekmesi** zaten seçildiyse, bu seçeneği seçili bırakabilirsiniz.) Ardından **İleri**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="607bd-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="607bd-129">**Sütun veri biçimi** alanında **Tarih: mdy**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="607bd-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="607bd-130">Ardından **İleri**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="607bd-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="607bd-131">**Sütun veri biçimi** alanında, tüm miktar sütunları için **metin** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="607bd-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="607bd-132">Ardından **Son**'u seçin.</span><span class="sxs-lookup"><span data-stu-id="607bd-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="607bd-133">Karşılaştırma dosyalarını programlı olarak indir</span><span class="sxs-lookup"><span data-stu-id="607bd-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="607bd-134">Mutabakat dosyaları çok büyük olabilir ve bazen indirmek zordur.</span><span class="sxs-lookup"><span data-stu-id="607bd-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="607bd-135">Karşılaştırma dosyalarını program aracılığıyla indirmek için bkz. [fatura satırı öğelerini Al](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="607bd-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="607bd-136">Vergiler veya KDV 'yi eşleştirin</span><span class="sxs-lookup"><span data-stu-id="607bd-136">Map taxes or VAT</span></span>

<span data-ttu-id="607bd-137">Vergiler veya katma değer vergi (KDV) faturanızı eşlemek için:</span><span class="sxs-lookup"><span data-stu-id="607bd-137">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="607bd-138">Lisans tabanlı dosyadaki **vergi** sütununu toplayın.</span><span class="sxs-lookup"><span data-stu-id="607bd-138">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="607bd-139">Kullanım tabanlı dosyadaki **TaxAmount** sütununu toplayın.</span><span class="sxs-lookup"><span data-stu-id="607bd-139">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="607bd-140">İş ortağına göre mutabakat dosyalarını dök</span><span class="sxs-lookup"><span data-stu-id="607bd-140">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="607bd-141">**Dolaylı modeldeki** iş ortakları, bu ek alanları hem lisans tabanlı hem de kullanım tabanlı mutabakat dosyalarında kullanarak dosyaları satıcıya göre silebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="607bd-141">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="607bd-142">MPN Kimliği</span><span class="sxs-lookup"><span data-stu-id="607bd-142">MPN ID</span></span> | <span data-ttu-id="607bd-143">Description</span><span class="sxs-lookup"><span data-stu-id="607bd-143">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="607bd-144">MPN Kimliği</span><span class="sxs-lookup"><span data-stu-id="607bd-144">MPN ID</span></span> | <span data-ttu-id="607bd-145">Bulut çözümü sağlayıcısı (CSP) ortağının (doğrudan veya dolaylı) Microsoft İş Ortağı Ağı (MPN) tanımlayıcısı.</span><span class="sxs-lookup"><span data-stu-id="607bd-145">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="607bd-146">Satıcı MPN KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="607bd-146">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="607bd-147">[Abonelik için kayıt satıcısının MPN tanımlayıcısı](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="607bd-147">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="607bd-148">Bu alan, Iş Ortağı Merkezi 'nde belirli bir abonelik için listelenen satıcı KIMLIĞINE karşılık gelir.</span><span class="sxs-lookup"><span data-stu-id="607bd-148">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="607bd-149">Yalnızca dolaylı modeldeki iş ortakları için mutabakat dosyaları üzerinde görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="607bd-149">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="607bd-150">Satıcı MPN KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="607bd-150">Reseller MPN ID</span></span>

<span data-ttu-id="607bd-151">Bir CSP iş ortağı aboneliği doğrudan müşteriye satmışsa **MPN kimliği** , hem **MPN kimliği** hem de **satıcı MPN kimliği** olarak iki kez listelenir.</span><span class="sxs-lookup"><span data-stu-id="607bd-151">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="607bd-152">Bir CSP iş ortağının **MPN kimliği** olmayan bir satıcısı varsa, bu değer bunun yerine ortağın **MPN kimliğine** ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="607bd-152">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="607bd-153">CSP iş ortağı bir **satıcı MPN kimliğini** kaldırdığında bu değer *-1* olarak ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="607bd-153">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="607bd-154">**Satıcı MPN kimliğini** görüntülemek veya güncelleştirmek için:</span><span class="sxs-lookup"><span data-stu-id="607bd-154">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="607bd-155">İş Ortağı Merkezi'nde oturum açın.</span><span class="sxs-lookup"><span data-stu-id="607bd-155">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="607bd-156">Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="607bd-156">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="607bd-157">Listeden müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="607bd-157">Choose the customer from the list.</span></span>
4. <span data-ttu-id="607bd-158">Müşteri menüsünde **abonelikler**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="607bd-158">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="607bd-159">Listeden aboneliği seçin.</span><span class="sxs-lookup"><span data-stu-id="607bd-159">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="607bd-160">**Satıcıdan (MPN kimliği)** değiştirmek için **Güncelleştir** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="607bd-160">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="607bd-161">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="607bd-161">Next steps</span></span>

- [<span data-ttu-id="607bd-162">Faturanız & keşfi dosyanızı okuma</span><span class="sxs-lookup"><span data-stu-id="607bd-162">How to read your bill & recon file</span></span>](read-your-bill.md) 