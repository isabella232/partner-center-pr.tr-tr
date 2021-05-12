---
title: Mutabakat dosyalarınızı kullanma
ms.topic: article
ms.date: 03/26/2021
description: Hesap hesaplarında mutabakat İş Ortağı Merkezi ve verilen faturalama dönemi için ücretlerin ayrıntılı, satır öğesi görünümlerini yorumlama hakkında bilgi öğrenin.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 755881d0bd96b9d601346ebb6271bd524c31d0a3
ms.sourcegitcommit: 837d3c5b52ab056b2b761cd85eb2426f56b62614
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/12/2021
ms.locfileid: "109794964"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="e5333-103">Mutabakat dosyalarında satır öğelerini okumayı İş Ortağı Merkezi öğrenin</span><span class="sxs-lookup"><span data-stu-id="e5333-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="e5333-104">**Uygun roller:** Faturalama yöneticisi | Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="e5333-104">**Appropriate roles**: Billing admin | Global admin</span></span>

<span data-ttu-id="e5333-105">Bir faturalama döngüsünde her bir İş Ortağı Merkezi ayrıntılı ve satır öğesi görünümü için mutabakat dosyalarınızı bir hesaptan indirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="e5333-105">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="e5333-106">Satır öğesi ayrıntıları, her müşterinin aboneliklerinin ücretlerini ve ayrıntılı olayları (bir aboneliğe lisansların orta dönem eklemesi gibi) içerir.</span><span class="sxs-lookup"><span data-stu-id="e5333-106">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="e5333-107">Faturanızı okuma hakkında bilgi **için bkz.** [Faturanızı okuma.](read-your-bill.md)</span><span class="sxs-lookup"><span data-stu-id="e5333-107">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="e5333-108">Mutabakat dosyası alanlarını anlama</span><span class="sxs-lookup"><span data-stu-id="e5333-108">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="e5333-109">Lisans tabanlı mutabakat dosyası alanları</span><span class="sxs-lookup"><span data-stu-id="e5333-109">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="e5333-110">Kullanım tabanlı mutabakat dosyası alanları</span><span class="sxs-lookup"><span data-stu-id="e5333-110">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="e5333-111">Günlük fiyatlandırılan kullanım mutabakat dosyası alanları</span><span class="sxs-lookup"><span data-stu-id="e5333-111">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="e5333-112">Tek sefer satın alma CSP mutabakat dosyası alanları</span><span class="sxs-lookup"><span data-stu-id="e5333-112">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="e5333-113">Mutabakat dosyalarında ücret türlerini anlama</span><span class="sxs-lookup"><span data-stu-id="e5333-113">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="e5333-114">Mutabakat dosyalarında **(ChargeType** sütunu) ücret türlerini anlamak için [bkz. Mutabakat dosyası ücret türleri.](recon-file-charge-types.md)</span><span class="sxs-lookup"><span data-stu-id="e5333-114">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="e5333-115">Biçimlendirme sorunlarını düzeltme</span><span class="sxs-lookup"><span data-stu-id="e5333-115">Fix formatting issues</span></span>

<span data-ttu-id="e5333-116">Bazen bir mutabakat dosyası biçimlendirme sorunları içerebilir.</span><span class="sxs-lookup"><span data-stu-id="e5333-116">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="e5333-117">Örneğin, en-US yerel yereli kullanılmazsa bu sorun oluşabilir.</span><span class="sxs-lookup"><span data-stu-id="e5333-117">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="e5333-118">Mutabakat dosyalarınıza ilişkin biçimlendirme sorunlarını düzeltmek için şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="e5333-118">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="e5333-119">Mutabakat dosyasını (.csv biçiminde) Microsoft Excel'de açın.</span><span class="sxs-lookup"><span data-stu-id="e5333-119">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="e5333-120">Dosyadaki ilk sütunu seçin.</span><span class="sxs-lookup"><span data-stu-id="e5333-120">Select the first column in the file.</span></span>
3. <span data-ttu-id="e5333-121">Metni **Sütunlara Dönüştürme Sihirbazı'nı açın.**</span><span class="sxs-lookup"><span data-stu-id="e5333-121">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="e5333-122">Şeritte Veri'yi **ve ardından** Metinden **Sütunlar'a'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="e5333-122">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="e5333-123">Sihirbazda Sınırlandırılmış **dosya türü'ne tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="e5333-123">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="e5333-124">Ardından **İleri**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="e5333-124">Then, select **Next**.</span></span>
5. <span data-ttu-id="e5333-125">**Sınırlayıcılar** alanında **virgül**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="e5333-125">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="e5333-126">( **Sekmesi** zaten seçildiyse, bu seçeneği seçili bırakabilirsiniz.) Ardından **İleri**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="e5333-126">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="e5333-127">**Sütun veri biçimi** alanında **Tarih: mdy**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="e5333-127">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="e5333-128">Ardından **İleri**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="e5333-128">Then, select **Next**.</span></span>
7. <span data-ttu-id="e5333-129">**Sütun veri biçimi** alanında, tüm miktar sütunları için **metin** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="e5333-129">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="e5333-130">Ardından **Son**'u seçin.</span><span class="sxs-lookup"><span data-stu-id="e5333-130">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="e5333-131">Karşılaştırma dosyalarını programlı olarak indir</span><span class="sxs-lookup"><span data-stu-id="e5333-131">Download reconciliation files programmatically</span></span>

<span data-ttu-id="e5333-132">Mutabakat dosyaları çok büyük olabilir ve bazen indirmek zordur.</span><span class="sxs-lookup"><span data-stu-id="e5333-132">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="e5333-133">Karşılaştırma dosyalarını program aracılığıyla indirmek için bkz. [fatura satırı öğelerini Al](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="e5333-133">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="e5333-134">Dosyanız Excel 'deki satır sınırını aşarsa</span><span class="sxs-lookup"><span data-stu-id="e5333-134">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="e5333-135">Bir mutabakat dosyasını indirebiliyor ancak Microsoft Excel 'de açmadıysanız, dosyada Excel 'In izin vermeyeceği daha fazla satır bulunduğu anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="e5333-135">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="e5333-136">Bu durumda, dosyayı açmak için aşağıdaki yordamlardan birini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="e5333-136">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="e5333-137">Power BI bir keşfi dosyası açın</span><span class="sxs-lookup"><span data-stu-id="e5333-137">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="e5333-138">Mutabakat dosyasını normalde yaptığınız gibi indirin.</span><span class="sxs-lookup"><span data-stu-id="e5333-138">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="e5333-139">Power BI örneğini indirin, yükleyin ve açın.</span><span class="sxs-lookup"><span data-stu-id="e5333-139">Download, install, and open an instance of Power BI.</span></span>
3. <span data-ttu-id="e5333-140">Power BI **giriş** sekmesinde **veri al**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="e5333-140">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="e5333-141">**Ortak veri kaynakları** listesinde **metin/CSV**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="e5333-141">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="e5333-142">İstendiğinde, keşfi dosyanızı açın.</span><span class="sxs-lookup"><span data-stu-id="e5333-142">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="e5333-143">Excel Pivot tablosunda bir keşfi dosyası açma</span><span class="sxs-lookup"><span data-stu-id="e5333-143">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="e5333-144">Mutabakat dosyasını normalde yaptığınız gibi indirin.</span><span class="sxs-lookup"><span data-stu-id="e5333-144">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="e5333-145">Microsoft Excel'de yeni bir dosya açın.</span><span class="sxs-lookup"><span data-stu-id="e5333-145">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="e5333-146">Veri sekmesinde **Veri al'ı** seçin, **Dosyadan'ı ve ardından** **Metin/CSV'yi seçin.** </span><span class="sxs-lookup"><span data-stu-id="e5333-146">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="e5333-147">İstendiğinde, mutabakat dosyanızı açın.</span><span class="sxs-lookup"><span data-stu-id="e5333-147">When prompted, open your recon file.</span></span> <span data-ttu-id="e5333-148">Verileriniz görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="e5333-148">Your data will appear.</span></span>
5. <span data-ttu-id="e5333-149">Yükle **açılan menüsünde,** Üzerine **yükle'yi ve ardından** Tamam'ı **seçin.**</span><span class="sxs-lookup"><span data-stu-id="e5333-149">In the **Load** dropdown menu, select **Load to**, and then **OK**.</span></span>
6. <span data-ttu-id="e5333-150">Verilerinizi İçeri **Aktar iletişim** kutusunda **PivotTable Raporu'nı seçerek** dosyanızı açın.</span><span class="sxs-lookup"><span data-stu-id="e5333-150">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="e5333-151">Negatif tutar görüntülenir</span><span class="sxs-lookup"><span data-stu-id="e5333-151">Negative amount displayed</span></span>

<span data-ttu-id="e5333-152">Mutabakat dosyanız negatif bir tutar görebilir.</span><span class="sxs-lookup"><span data-stu-id="e5333-152">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="e5333-153">Bu sorun büyük olasılıkla aşağıdakilerden biri nedeniyle oluşur:</span><span class="sxs-lookup"><span data-stu-id="e5333-153">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="e5333-154">Kısa süre önce lisanslarınızı iptal etti veya azalttınız</span><span class="sxs-lookup"><span data-stu-id="e5333-154">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="e5333-155">Hizmet lisans sözleşmesi (SLA) veya Azure tüketimi için kredi aldınız</span><span class="sxs-lookup"><span data-stu-id="e5333-155">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="e5333-156">Bu işlem hakkında daha fazla bilgi edinmek için mutabakat dosyanızda işlemin ödeme türü özniteliğini gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="e5333-156">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="e5333-157">Vergileri veya KDV'yi eşleme</span><span class="sxs-lookup"><span data-stu-id="e5333-157">Map taxes or VAT</span></span>

<span data-ttu-id="e5333-158">Vergileri veya katma değerli vergileri (KDV) faturanıza eşlemek için:</span><span class="sxs-lookup"><span data-stu-id="e5333-158">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="e5333-159">Lisans **tabanlı** dosyadan Vergi sütununu toplama.</span><span class="sxs-lookup"><span data-stu-id="e5333-159">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="e5333-160">Kullanım tabanlı **dosyadan TaxAmount** sütununu toplama.</span><span class="sxs-lookup"><span data-stu-id="e5333-160">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="e5333-161">Mutabakat dosyalarını iş ortağına göre öğeleştirme</span><span class="sxs-lookup"><span data-stu-id="e5333-161">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="e5333-162">Dolaylı modelde **iş ortakları,** bu ek alanları hem lisans tabanlı hem de kullanım tabanlı mutabakat dosyalarında kullanarak dosyaları kurumsal bayiye göre öğe hale kullanabilir.</span><span class="sxs-lookup"><span data-stu-id="e5333-162">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="e5333-163">MPN Kimliği</span><span class="sxs-lookup"><span data-stu-id="e5333-163">MPN ID</span></span> | <span data-ttu-id="e5333-164">Description</span><span class="sxs-lookup"><span data-stu-id="e5333-164">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="e5333-165">MPN Kimliği</span><span class="sxs-lookup"><span data-stu-id="e5333-165">MPN ID</span></span> | <span data-ttu-id="e5333-166">Microsoft İş Ortağı Ağı (CSP) iş ortağının Bulut Çözümü Sağlayıcısı (MPN) tanımlayıcısını (doğrudan veya dolaylı).</span><span class="sxs-lookup"><span data-stu-id="e5333-166">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="e5333-167">Kurumsal Bayi MPN Kimliği</span><span class="sxs-lookup"><span data-stu-id="e5333-167">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="e5333-168">Aboneliğin [kaydının kurumsal bayisinde MPN tanımlayıcısı.](#reseller-mpn-id)</span><span class="sxs-lookup"><span data-stu-id="e5333-168">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="e5333-169">Bu alan, belirli bir abonelik için listelenen kurumsal bayi kimliğine karşılık İş Ortağı Merkezi.</span><span class="sxs-lookup"><span data-stu-id="e5333-169">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="e5333-170">Yalnızca dolaylı modeldeki iş ortakları için mutabakat dosyaları üzerinde görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="e5333-170">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="e5333-171">Satıcı MPN KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="e5333-171">Reseller MPN ID</span></span>

<span data-ttu-id="e5333-172">Bir CSP iş ortağı aboneliği doğrudan müşteriye satmışsa **MPN kimliği** , hem **MPN kimliği** hem de **satıcı MPN kimliği** olarak iki kez listelenir.</span><span class="sxs-lookup"><span data-stu-id="e5333-172">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="e5333-173">Bir CSP iş ortağının **MPN kimliği** olmayan bir satıcısı varsa, bu değer bunun yerine ortağın **MPN kimliğine** ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="e5333-173">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="e5333-174">CSP iş ortağı bir **satıcı MPN kimliğini** kaldırdığında bu değer *-1* olarak ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="e5333-174">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="e5333-175">**Satıcı MPN kimliğini** görüntülemek veya güncelleştirmek için:</span><span class="sxs-lookup"><span data-stu-id="e5333-175">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="e5333-176">İş Ortağı Merkezi'nde oturum açın.</span><span class="sxs-lookup"><span data-stu-id="e5333-176">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="e5333-177">Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="e5333-177">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="e5333-178">Listeden müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="e5333-178">Choose the customer from the list.</span></span>
4. <span data-ttu-id="e5333-179">Müşteri menüsünde **abonelikler**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="e5333-179">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="e5333-180">Listeden aboneliği seçin.</span><span class="sxs-lookup"><span data-stu-id="e5333-180">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="e5333-181">**Satıcıdan (MPN kimliği)** değiştirmek için **Güncelleştir** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="e5333-181">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e5333-182">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="e5333-182">Next steps</span></span>

- [<span data-ttu-id="e5333-183">Faturanız & keşfi dosyanızı okuma</span><span class="sxs-lookup"><span data-stu-id="e5333-183">How to read your bill & recon file</span></span>](read-your-bill.md) 