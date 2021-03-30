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
ms.openlocfilehash: aefd5258c778fd8a7b92bfe49f245bf818497fb8
ms.sourcegitcommit: dd51744a4af3797493a5ebbfc766dab86ff00477
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/29/2021
ms.locfileid: "105730101"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="79c32-103">Iş Ortağı Merkezi mutabakatı dosyalarınızda satır öğelerini okumayı öğrenin</span><span class="sxs-lookup"><span data-stu-id="79c32-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="79c32-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="79c32-104">**Appropriate roles**</span></span>

- <span data-ttu-id="79c32-105">Faturalama yöneticisi</span><span class="sxs-lookup"><span data-stu-id="79c32-105">Billing admin</span></span>
- <span data-ttu-id="79c32-106">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="79c32-106">Global admin</span></span>

<span data-ttu-id="79c32-107">Bir fatura döngüsündeki her bir ücret için ayrıntılı, satır öğesi görünümü için Iş Ortağı Merkezi ' nden mutabakat dosyalarınızı indirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="79c32-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="79c32-108">Satır öğesi ayrıntıları, her bir müşterinin aboneliğine ilişkin ücretleri ve ayrıntılı olayları (bir aboneliğe yönelik bir abonelik için orta dönem ekleme gibi) içerir.</span><span class="sxs-lookup"><span data-stu-id="79c32-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="79c32-109">**Faturanızı** okuma hakkında daha fazla bilgi için bkz. [faturanızı okuyun](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="79c32-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="79c32-110">Mutabakat dosyası alanlarını anlama</span><span class="sxs-lookup"><span data-stu-id="79c32-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="79c32-111">Lisans tabanlı mutabakat dosyası alanları</span><span class="sxs-lookup"><span data-stu-id="79c32-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="79c32-112">Kullanım tabanlı mutabakat dosyası alanları</span><span class="sxs-lookup"><span data-stu-id="79c32-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="79c32-113">Günlük fiyatlandırılan kullanım mutabakat dosyası alanları</span><span class="sxs-lookup"><span data-stu-id="79c32-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="79c32-114">Bir kerelik satın alma CSP 'si mutabakatı dosya alanları</span><span class="sxs-lookup"><span data-stu-id="79c32-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="79c32-115">Mutabakat dosyalarındaki ücretlendirme türlerini anlama</span><span class="sxs-lookup"><span data-stu-id="79c32-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="79c32-116">Mutabakat dosyalarındaki ( **Chargetype** sütunu) ücret türlerini anlamak için bkz. [mutabakatı dosya ücreti türleri](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="79c32-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="79c32-117">Biçimlendirme sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="79c32-117">Fix formatting issues</span></span>

<span data-ttu-id="79c32-118">Bazen bir mutabakat dosyasında biçimlendirme sorunları bulunabilir.</span><span class="sxs-lookup"><span data-stu-id="79c32-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="79c32-119">Örneğin, en-US yerel ayarı kullanılmazsa bu sorun oluşabilir.</span><span class="sxs-lookup"><span data-stu-id="79c32-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="79c32-120">Mutabakat dosyalarınızda biçimlendirme sorunlarını gidermek için aşağıdaki adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="79c32-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="79c32-121">Microsoft Excel 'de mutabakat dosyasını (. csv biçiminde) açın.</span><span class="sxs-lookup"><span data-stu-id="79c32-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="79c32-122">Dosyadaki ilk sütunu seçin.</span><span class="sxs-lookup"><span data-stu-id="79c32-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="79c32-123">**Metni sütunlara dönüştürme Sihirbazı**' nı açın.</span><span class="sxs-lookup"><span data-stu-id="79c32-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="79c32-124">Şeritte, **veriler**' i seçin ve **sütunlar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="79c32-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="79c32-125">Sihirbazda, **ayrılmış dosya türü**' nü seçin.</span><span class="sxs-lookup"><span data-stu-id="79c32-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="79c32-126">Ardından **İleri**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="79c32-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="79c32-127">**Sınırlayıcılar** alanında **virgül**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="79c32-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="79c32-128">( **Sekmesi** zaten seçildiyse, bu seçeneği seçili bırakabilirsiniz.) Ardından **İleri**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="79c32-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="79c32-129">**Sütun veri biçimi** alanında **Tarih: mdy**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="79c32-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="79c32-130">Ardından **İleri**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="79c32-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="79c32-131">**Sütun veri biçimi** alanında, tüm miktar sütunları için **metin** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="79c32-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="79c32-132">Ardından **Son**'u seçin.</span><span class="sxs-lookup"><span data-stu-id="79c32-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="79c32-133">Karşılaştırma dosyalarını programlı olarak indir</span><span class="sxs-lookup"><span data-stu-id="79c32-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="79c32-134">Mutabakat dosyaları çok büyük olabilir ve bazen indirmek zordur.</span><span class="sxs-lookup"><span data-stu-id="79c32-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="79c32-135">Karşılaştırma dosyalarını program aracılığıyla indirmek için bkz. [fatura satırı öğelerini Al](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="79c32-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="79c32-136">Dosyanız Excel 'deki satır sınırını aşarsa</span><span class="sxs-lookup"><span data-stu-id="79c32-136">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="79c32-137">Bir mutabakat dosyasını indirebiliyor ancak Microsoft Excel 'de açmadıysanız, dosyada Excel 'In izin vermeyeceği daha fazla satır bulunduğu anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="79c32-137">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="79c32-138">Bu durumda, dosyayı açmak için aşağıdaki yordamlardan birini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="79c32-138">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="79c32-139">Power BI bir keşfi dosyası açın</span><span class="sxs-lookup"><span data-stu-id="79c32-139">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="79c32-140">Mutabakat dosyasını normalde yaptığınız gibi indirin.</span><span class="sxs-lookup"><span data-stu-id="79c32-140">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="79c32-141">Power BI örneğini indirin, yükleyin ve açın.</span><span class="sxs-lookup"><span data-stu-id="79c32-141">Download, install, and open an instance of Power BI.</span></span>
3. <span data-ttu-id="79c32-142">Power BI **giriş** sekmesinde **veri al**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="79c32-142">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="79c32-143">**Ortak veri kaynakları** listesinde **metin/CSV**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="79c32-143">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="79c32-144">İstendiğinde, keşfi dosyanızı açın.</span><span class="sxs-lookup"><span data-stu-id="79c32-144">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="79c32-145">Excel Pivot tablosunda bir keşfi dosyası açma</span><span class="sxs-lookup"><span data-stu-id="79c32-145">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="79c32-146">Mutabakat dosyasını normalde yaptığınız gibi indirin.</span><span class="sxs-lookup"><span data-stu-id="79c32-146">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="79c32-147">Microsoft Excel 'de yeni bir dosya açın.</span><span class="sxs-lookup"><span data-stu-id="79c32-147">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="79c32-148">**Veri** sekmesinde **veri al**' ı seçin, dosyadan ' **ı SEÇIN ve** ardından **metin/CSV**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="79c32-148">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="79c32-149">İstendiğinde, keşfi dosyanızı açın.</span><span class="sxs-lookup"><span data-stu-id="79c32-149">When prompted, open your recon file.</span></span> <span data-ttu-id="79c32-150">Verileriniz görüntülenecektir.</span><span class="sxs-lookup"><span data-stu-id="79c32-150">Your data will appear.</span></span>
5. <span data-ttu-id="79c32-151">**Yük** açılır menüsünde, **Yükle**' yi ve ardından **Tamam**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="79c32-151">In the **Load** dropdown menu, select **Load to**, and then **OK**.</span></span>
6. <span data-ttu-id="79c32-152">**Verileri Içeri aktar** iletişim kutusunda Dosyanızı açmak Için **PivotTable raporu** ' nu seçin.</span><span class="sxs-lookup"><span data-stu-id="79c32-152">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="79c32-153">Negatif miktar görüntülendi</span><span class="sxs-lookup"><span data-stu-id="79c32-153">Negative amount displayed</span></span>

<span data-ttu-id="79c32-154">Mutabakat dosyanızda negatif bir miktar görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="79c32-154">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="79c32-155">Bunun nedeni aşağıdakilerden biri olabilir:</span><span class="sxs-lookup"><span data-stu-id="79c32-155">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="79c32-156">Son zamanlarda lisans numaranızı iptal etmiş veya azalttı</span><span class="sxs-lookup"><span data-stu-id="79c32-156">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="79c32-157">Bir hizmet Lisans Sözleşmesi (SLA) ya da Azure tüketimi için kredi aldınız</span><span class="sxs-lookup"><span data-stu-id="79c32-157">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="79c32-158">Bu işlem hakkında daha fazla bilgi edinmek için mutabakat dosyanızdaki ücret türü özniteliğini gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="79c32-158">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="79c32-159">Vergiler veya KDV 'yi eşleştirin</span><span class="sxs-lookup"><span data-stu-id="79c32-159">Map taxes or VAT</span></span>

<span data-ttu-id="79c32-160">Vergiler veya katma değer vergi (KDV) faturanızı eşlemek için:</span><span class="sxs-lookup"><span data-stu-id="79c32-160">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="79c32-161">Lisans tabanlı dosyadaki **vergi** sütununu toplayın.</span><span class="sxs-lookup"><span data-stu-id="79c32-161">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="79c32-162">Kullanım tabanlı dosyadaki **TaxAmount** sütununu toplayın.</span><span class="sxs-lookup"><span data-stu-id="79c32-162">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="79c32-163">İş ortağına göre mutabakat dosyalarını dök</span><span class="sxs-lookup"><span data-stu-id="79c32-163">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="79c32-164">**Dolaylı modeldeki** iş ortakları, bu ek alanları hem lisans tabanlı hem de kullanım tabanlı mutabakat dosyalarında kullanarak dosyaları satıcıya göre silebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="79c32-164">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="79c32-165">MPN Kimliği</span><span class="sxs-lookup"><span data-stu-id="79c32-165">MPN ID</span></span> | <span data-ttu-id="79c32-166">Açıklama</span><span class="sxs-lookup"><span data-stu-id="79c32-166">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="79c32-167">MPN Kimliği</span><span class="sxs-lookup"><span data-stu-id="79c32-167">MPN ID</span></span> | <span data-ttu-id="79c32-168">Bulut çözümü sağlayıcısı (CSP) ortağının (doğrudan veya dolaylı) Microsoft İş Ortağı Ağı (MPN) tanımlayıcısı.</span><span class="sxs-lookup"><span data-stu-id="79c32-168">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="79c32-169">Satıcı MPN KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="79c32-169">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="79c32-170">[Abonelik için kayıt satıcısının MPN tanımlayıcısı](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="79c32-170">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="79c32-171">Bu alan, Iş Ortağı Merkezi 'nde belirli bir abonelik için listelenen satıcı KIMLIĞINE karşılık gelir.</span><span class="sxs-lookup"><span data-stu-id="79c32-171">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="79c32-172">Yalnızca dolaylı modeldeki iş ortakları için mutabakat dosyaları üzerinde görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="79c32-172">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="79c32-173">Satıcı MPN KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="79c32-173">Reseller MPN ID</span></span>

<span data-ttu-id="79c32-174">Bir CSP iş ortağı aboneliği doğrudan müşteriye satmışsa **MPN kimliği** , hem **MPN kimliği** hem de **satıcı MPN kimliği** olarak iki kez listelenir.</span><span class="sxs-lookup"><span data-stu-id="79c32-174">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="79c32-175">Bir CSP iş ortağının **MPN kimliği** olmayan bir satıcısı varsa, bu değer bunun yerine ortağın **MPN kimliğine** ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="79c32-175">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="79c32-176">CSP iş ortağı bir **satıcı MPN kimliğini** kaldırdığında bu değer *-1* olarak ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="79c32-176">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="79c32-177">**Satıcı MPN kimliğini** görüntülemek veya güncelleştirmek için:</span><span class="sxs-lookup"><span data-stu-id="79c32-177">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="79c32-178">İş Ortağı Merkezi'nde oturum açın.</span><span class="sxs-lookup"><span data-stu-id="79c32-178">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="79c32-179">Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="79c32-179">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="79c32-180">Listeden müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="79c32-180">Choose the customer from the list.</span></span>
4. <span data-ttu-id="79c32-181">Müşteri menüsünde **abonelikler**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="79c32-181">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="79c32-182">Listeden aboneliği seçin.</span><span class="sxs-lookup"><span data-stu-id="79c32-182">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="79c32-183">**Satıcıdan (MPN kimliği)** değiştirmek için **Güncelleştir** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="79c32-183">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="79c32-184">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="79c32-184">Next steps</span></span>

- [<span data-ttu-id="79c32-185">Faturanız & keşfi dosyanızı okuma</span><span class="sxs-lookup"><span data-stu-id="79c32-185">How to read your bill & recon file</span></span>](read-your-bill.md) 