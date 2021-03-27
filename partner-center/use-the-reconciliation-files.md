---
title: Karşılaştırma dosyalarınızı kullanın
ms.topic: article
ms.date: 03/26/2021
description: Iş Ortağı Merkezi 'nde mutabakat dosyaları ve belirli bir faturalandırma döngüsünün ücretlendirdiği ayrıntılı, satır öğesi görünümlerinin nasıl yorumlanacağı hakkında bilgi edinin.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4a6a1455304f12e364d71e666cbd548821f8be55
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633905"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="4009a-103">Iş Ortağı Merkezi mutabakatı dosyalarınızda satır öğelerini okumayı öğrenin</span><span class="sxs-lookup"><span data-stu-id="4009a-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="4009a-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="4009a-104">**Appropriate roles**</span></span>

- <span data-ttu-id="4009a-105">Faturalama yöneticisi</span><span class="sxs-lookup"><span data-stu-id="4009a-105">Billing admin</span></span>
- <span data-ttu-id="4009a-106">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="4009a-106">Global admin</span></span>

<span data-ttu-id="4009a-107">Bir fatura döngüsündeki her bir ücret için ayrıntılı, satır öğesi görünümü için Iş Ortağı Merkezi ' nden mutabakat dosyalarınızı indirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4009a-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="4009a-108">Satır öğesi ayrıntıları, her bir müşterinin aboneliğine ilişkin ücretleri ve ayrıntılı olayları (bir aboneliğe yönelik bir abonelik için orta dönem ekleme gibi) içerir.</span><span class="sxs-lookup"><span data-stu-id="4009a-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="4009a-109">**Faturanızı** okuma hakkında daha fazla bilgi için bkz. [faturanızı okuyun](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="4009a-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="4009a-110">Mutabakat dosyası alanlarını anlama</span><span class="sxs-lookup"><span data-stu-id="4009a-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="4009a-111">Lisans tabanlı mutabakat dosyası alanları</span><span class="sxs-lookup"><span data-stu-id="4009a-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="4009a-112">Kullanım tabanlı mutabakat dosyası alanları</span><span class="sxs-lookup"><span data-stu-id="4009a-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="4009a-113">Günlük fiyatlandırılan kullanım mutabakat dosyası alanları</span><span class="sxs-lookup"><span data-stu-id="4009a-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="4009a-114">Bir kerelik satın alma CSP 'si mutabakatı dosya alanları</span><span class="sxs-lookup"><span data-stu-id="4009a-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="4009a-115">Mutabakat dosyalarındaki ücretlendirme türlerini anlama</span><span class="sxs-lookup"><span data-stu-id="4009a-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="4009a-116">Mutabakat dosyalarındaki ( **Chargetype** sütunu) ücret türlerini anlamak için bkz. [mutabakatı dosya ücreti türleri](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="4009a-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="4009a-117">Biçimlendirme sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="4009a-117">Fix formatting issues</span></span>

<span data-ttu-id="4009a-118">Bazen bir mutabakat dosyasında biçimlendirme sorunları bulunabilir.</span><span class="sxs-lookup"><span data-stu-id="4009a-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="4009a-119">Örneğin, en-US yerel ayarı kullanılmazsa bu sorun oluşabilir.</span><span class="sxs-lookup"><span data-stu-id="4009a-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="4009a-120">Mutabakat dosyalarınızda biçimlendirme sorunlarını gidermek için aşağıdaki adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="4009a-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="4009a-121">Microsoft Excel 'de mutabakat dosyasını (. csv biçiminde) açın.</span><span class="sxs-lookup"><span data-stu-id="4009a-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="4009a-122">Dosyadaki ilk sütunu seçin.</span><span class="sxs-lookup"><span data-stu-id="4009a-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="4009a-123">**Metni sütunlara dönüştürme Sihirbazı**' nı açın.</span><span class="sxs-lookup"><span data-stu-id="4009a-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="4009a-124">Şeritte, **veriler**' i seçin ve **sütunlar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="4009a-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="4009a-125">Sihirbazda, **ayrılmış dosya türü**' nü seçin.</span><span class="sxs-lookup"><span data-stu-id="4009a-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="4009a-126">Ardından **İleri**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="4009a-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="4009a-127">**Sınırlayıcılar** alanında **virgül**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="4009a-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="4009a-128">( **Sekmesi** zaten seçildiyse, bu seçeneği seçili bırakabilirsiniz.) Ardından **İleri**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="4009a-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="4009a-129">**Sütun veri biçimi** alanında **Tarih: mdy**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="4009a-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="4009a-130">Ardından **İleri**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="4009a-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="4009a-131">**Sütun veri biçimi** alanında, tüm miktar sütunları için **metin** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="4009a-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="4009a-132">Ardından **Son**'u seçin.</span><span class="sxs-lookup"><span data-stu-id="4009a-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="4009a-133">Karşılaştırma dosyalarını programlı olarak indir</span><span class="sxs-lookup"><span data-stu-id="4009a-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="4009a-134">Mutabakat dosyaları çok büyük olabilir ve bazen indirmek zordur.</span><span class="sxs-lookup"><span data-stu-id="4009a-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="4009a-135">Karşılaştırma dosyalarını program aracılığıyla indirmek için bkz. [fatura satırı öğelerini Al](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="4009a-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="4009a-136">Dosyanız Excel 'deki satır sınırını aşarsa</span><span class="sxs-lookup"><span data-stu-id="4009a-136">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="4009a-137">Bir mutabakat dosyasını indirebiliyor ancak Microsoft Excel 'de açmadıysanız, dosyada Excel 'In izin vermeyeceği daha fazla satır bulunduğu anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="4009a-137">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="4009a-138">Bu durumda, dosyayı açmak için aşağıdaki yordamlardan birini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4009a-138">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="4009a-139">Power BI bir keşfi dosyası açın</span><span class="sxs-lookup"><span data-stu-id="4009a-139">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="4009a-140">Mutabakat dosyasını normalde yaptığınız gibi indirin.</span><span class="sxs-lookup"><span data-stu-id="4009a-140">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="4009a-141">Power BI örneğini indirin, yükleyin ve açın.</span><span class="sxs-lookup"><span data-stu-id="4009a-141">Download, install, and open an instance of Power BI.</span></span>
3. <span data-ttu-id="4009a-142">Power BI **giriş** sekmesinde **veri al**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="4009a-142">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="4009a-143">**Ortak veri kaynakları** listesinde **metin/CSV**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="4009a-143">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="4009a-144">İstendiğinde, keşfi dosyanızı açın.</span><span class="sxs-lookup"><span data-stu-id="4009a-144">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="4009a-145">Excel Pivot tablosunda bir keşfi dosyası açma</span><span class="sxs-lookup"><span data-stu-id="4009a-145">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="4009a-146">Mutabakat dosyasını normalde yaptığınız gibi indirin.</span><span class="sxs-lookup"><span data-stu-id="4009a-146">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="4009a-147">Microsoft Excel 'de yeni bir dosya açın.</span><span class="sxs-lookup"><span data-stu-id="4009a-147">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="4009a-148">**Veri** sekmesinde **veri al**' ı seçin, dosyadan ' **ı SEÇIN ve** ardından **metin/CSV**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="4009a-148">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="4009a-149">İstendiğinde, keşfi dosyanızı açın.</span><span class="sxs-lookup"><span data-stu-id="4009a-149">When prompted, open your recon file.</span></span> <span data-ttu-id="4009a-150">Verileriniz görüntülenecektir.</span><span class="sxs-lookup"><span data-stu-id="4009a-150">Your data will appear.</span></span>
5. <span data-ttu-id="4009a-151">**Yük** açılır menüsünde, **Yükle**' yi ve ardından **Tamam**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="4009a-151">In the **Load** dropdown menu, select **Load to**, and then **OK**.</span></span>
6. <span data-ttu-id="4009a-152">**Verileri Içeri aktar** iletişim kutusunda Dosyanızı açmak Için **PivotTable raporu** ' nu seçin.</span><span class="sxs-lookup"><span data-stu-id="4009a-152">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="4009a-153">Vergiler veya KDV 'yi eşleştirin</span><span class="sxs-lookup"><span data-stu-id="4009a-153">Map taxes or VAT</span></span>

<span data-ttu-id="4009a-154">Vergiler veya katma değer vergi (KDV) faturanızı eşlemek için:</span><span class="sxs-lookup"><span data-stu-id="4009a-154">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="4009a-155">Lisans tabanlı dosyadaki **vergi** sütununu toplayın.</span><span class="sxs-lookup"><span data-stu-id="4009a-155">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="4009a-156">Kullanım tabanlı dosyadaki **TaxAmount** sütununu toplayın.</span><span class="sxs-lookup"><span data-stu-id="4009a-156">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="4009a-157">İş ortağına göre mutabakat dosyalarını dök</span><span class="sxs-lookup"><span data-stu-id="4009a-157">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="4009a-158">**Dolaylı modeldeki** iş ortakları, bu ek alanları hem lisans tabanlı hem de kullanım tabanlı mutabakat dosyalarında kullanarak dosyaları satıcıya göre silebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4009a-158">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="4009a-159">MPN Kimliği</span><span class="sxs-lookup"><span data-stu-id="4009a-159">MPN ID</span></span> | <span data-ttu-id="4009a-160">Description</span><span class="sxs-lookup"><span data-stu-id="4009a-160">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="4009a-161">MPN Kimliği</span><span class="sxs-lookup"><span data-stu-id="4009a-161">MPN ID</span></span> | <span data-ttu-id="4009a-162">Bulut çözümü sağlayıcısı (CSP) ortağının (doğrudan veya dolaylı) Microsoft İş Ortağı Ağı (MPN) tanımlayıcısı.</span><span class="sxs-lookup"><span data-stu-id="4009a-162">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="4009a-163">Satıcı MPN KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="4009a-163">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="4009a-164">[Abonelik için kayıt satıcısının MPN tanımlayıcısı](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="4009a-164">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="4009a-165">Bu alan, Iş Ortağı Merkezi 'nde belirli bir abonelik için listelenen satıcı KIMLIĞINE karşılık gelir.</span><span class="sxs-lookup"><span data-stu-id="4009a-165">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="4009a-166">Yalnızca dolaylı modeldeki iş ortakları için mutabakat dosyaları üzerinde görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="4009a-166">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="4009a-167">Satıcı MPN KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="4009a-167">Reseller MPN ID</span></span>

<span data-ttu-id="4009a-168">Bir CSP iş ortağı aboneliği doğrudan müşteriye satmışsa **MPN kimliği** , hem **MPN kimliği** hem de **satıcı MPN kimliği** olarak iki kez listelenir.</span><span class="sxs-lookup"><span data-stu-id="4009a-168">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="4009a-169">Bir CSP iş ortağının **MPN kimliği** olmayan bir satıcısı varsa, bu değer bunun yerine ortağın **MPN kimliğine** ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="4009a-169">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="4009a-170">CSP iş ortağı bir **satıcı MPN kimliğini** kaldırdığında bu değer *-1* olarak ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="4009a-170">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="4009a-171">**Satıcı MPN kimliğini** görüntülemek veya güncelleştirmek için:</span><span class="sxs-lookup"><span data-stu-id="4009a-171">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="4009a-172">İş Ortağı Merkezi'nde oturum açın.</span><span class="sxs-lookup"><span data-stu-id="4009a-172">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="4009a-173">Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="4009a-173">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="4009a-174">Listeden müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="4009a-174">Choose the customer from the list.</span></span>
4. <span data-ttu-id="4009a-175">Müşteri menüsünde **abonelikler**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="4009a-175">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="4009a-176">Listeden aboneliği seçin.</span><span class="sxs-lookup"><span data-stu-id="4009a-176">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="4009a-177">**Satıcıdan (MPN kimliği)** değiştirmek için **Güncelleştir** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="4009a-177">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4009a-178">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="4009a-178">Next steps</span></span>

- [<span data-ttu-id="4009a-179">Faturanız & keşfi dosyanızı okuma</span><span class="sxs-lookup"><span data-stu-id="4009a-179">How to read your bill & recon file</span></span>](read-your-bill.md) 