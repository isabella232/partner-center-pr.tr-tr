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
ms.openlocfilehash: 1a7d5f3169c4b338a07475a7e246e87841b8dcfb
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431565"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="eb402-103">Veri mutabakat dosyalarında satır öğelerini İş Ortağı Merkezi öğrenin</span><span class="sxs-lookup"><span data-stu-id="eb402-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="eb402-104">**Uygun roller:** Faturalama yöneticisi | Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="eb402-104">**Appropriate roles**: Billing admin | Global admin</span></span>

<span data-ttu-id="eb402-105">Bir faturalama döngüsünde her bir İş Ortağı Merkezi ayrıntılı ve satır öğesi görünümü için mutabakat dosyalarınızı bir hesaptan indirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="eb402-105">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="eb402-106">Satır öğesi ayrıntıları, her müşterinin aboneliklerinin ücretlerini ve ayrıntılı olayları (bir aboneliğe lisansların orta dönem eklemesi gibi) içerir.</span><span class="sxs-lookup"><span data-stu-id="eb402-106">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="eb402-107">Faturanızı okuma hakkında bilgi için **bkz.** [Faturanızı okuma.](read-your-bill.md)</span><span class="sxs-lookup"><span data-stu-id="eb402-107">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="eb402-108">Mutabakat dosyası alanlarını anlama</span><span class="sxs-lookup"><span data-stu-id="eb402-108">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="eb402-109">Lisans tabanlı mutabakat dosyası alanları</span><span class="sxs-lookup"><span data-stu-id="eb402-109">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="eb402-110">Kullanım tabanlı mutabakat dosyası alanları</span><span class="sxs-lookup"><span data-stu-id="eb402-110">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="eb402-111">Günlük fiyatlandırılan kullanım mutabakat dosyası alanları</span><span class="sxs-lookup"><span data-stu-id="eb402-111">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="eb402-112">Tek sefer satın alma CSP mutabakat dosyası alanları</span><span class="sxs-lookup"><span data-stu-id="eb402-112">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="eb402-113">Mutabakat dosyalarında ücret türlerini anlama</span><span class="sxs-lookup"><span data-stu-id="eb402-113">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="eb402-114">Mutabakat dosyalarında **(ChargeType** sütunu) ücret türlerini anlamak için [bkz. Mutabakat dosyası ücret türleri.](recon-file-charge-types.md)</span><span class="sxs-lookup"><span data-stu-id="eb402-114">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="eb402-115">Biçimlendirme sorunlarını düzeltme</span><span class="sxs-lookup"><span data-stu-id="eb402-115">Fix formatting issues</span></span>

<span data-ttu-id="eb402-116">Bazen bir mutabakat dosyası biçimlendirme sorunları içerebilir.</span><span class="sxs-lookup"><span data-stu-id="eb402-116">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="eb402-117">Örneğin, en-US yerel yereli kullanılmazsa bu sorun oluşabilir.</span><span class="sxs-lookup"><span data-stu-id="eb402-117">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="eb402-118">Mutabakat dosyalarınıza ilişkin biçimlendirme sorunlarını düzeltmek için şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="eb402-118">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="eb402-119">Mutabakat dosyasını (.csv biçiminde) Microsoft Excel'de açın.</span><span class="sxs-lookup"><span data-stu-id="eb402-119">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="eb402-120">Dosyadaki ilk sütunu seçin.</span><span class="sxs-lookup"><span data-stu-id="eb402-120">Select the first column in the file.</span></span>
3. <span data-ttu-id="eb402-121">Metni **Sütunlara Dönüştürme Sihirbazı'nı açın.**</span><span class="sxs-lookup"><span data-stu-id="eb402-121">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="eb402-122">Şeritte Veri'yi **ve ardından** Metinden **Sütunlar'a'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="eb402-122">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="eb402-123">Sihirbazda Sınırlandırılmış **dosya türü'ne tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="eb402-123">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="eb402-124">Ardından, **Sonraki'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="eb402-124">Then, select **Next**.</span></span>
5. <span data-ttu-id="eb402-125">**Sınırlayıcılar alanında Virgül'i** **seçin.**</span><span class="sxs-lookup"><span data-stu-id="eb402-125">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="eb402-126">(Sekme **zaten** seçiliyse, bu seçeneği seçili bırakın.) Ardından, **Sonraki'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="eb402-126">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="eb402-127">Sütun veri biçimi alanında **Tarih:MDY'yi seçin.** </span><span class="sxs-lookup"><span data-stu-id="eb402-127">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="eb402-128">Ardından, **Sonraki'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="eb402-128">Then, select **Next**.</span></span>
7. <span data-ttu-id="eb402-129">Sütun veri **biçimi alanında tüm** tutar sütunları için **Metin'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="eb402-129">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="eb402-130">Ardından **Son**'u seçin.</span><span class="sxs-lookup"><span data-stu-id="eb402-130">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="eb402-131">Mutabakat dosyalarını program aracılığıyla indirme</span><span class="sxs-lookup"><span data-stu-id="eb402-131">Download reconciliation files programmatically</span></span>

<span data-ttu-id="eb402-132">Mutabakat dosyaları çok büyük olabilir ve bazen indirmek zordur.</span><span class="sxs-lookup"><span data-stu-id="eb402-132">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="eb402-133">Mutabakat dosyalarını program aracılığıyla indirmek için bkz. [Fatura satırı öğelerini al.](/partner-center/develop/get-invoiceline-items)</span><span class="sxs-lookup"><span data-stu-id="eb402-133">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="eb402-134">Dosyanız Excel'de satır sınırını aşarsa</span><span class="sxs-lookup"><span data-stu-id="eb402-134">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="eb402-135">Mutabakat dosyasını indire ancak Microsoft Excel'de açamıyorsanız, dosya büyük olasılıkla Excel'in izin ver alanından daha fazla satır içerdiği anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="eb402-135">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="eb402-136">Bu durumda, dosyayı açmak için aşağıdaki yordamlardan birini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="eb402-136">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="eb402-137">Bir mutabakat dosyasını Power BI</span><span class="sxs-lookup"><span data-stu-id="eb402-137">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="eb402-138">Mutabakat dosyasını normalde olduğu gibi indirin.</span><span class="sxs-lookup"><span data-stu-id="eb402-138">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="eb402-139">Microsoft Power BI'nin bir örneğini indirin, yükleyin ve açın.</span><span class="sxs-lookup"><span data-stu-id="eb402-139">Download, install, and open an instance of Microsoft Power BI.</span></span>
3. <span data-ttu-id="eb402-140">Giriş Power BI **Veri** al'ı **seçin.**</span><span class="sxs-lookup"><span data-stu-id="eb402-140">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="eb402-141">Ortak veri kaynakları listesinde **Metin/CSV'yi seçin.** </span><span class="sxs-lookup"><span data-stu-id="eb402-141">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="eb402-142">İstendiğinde, mutabakat dosyanızı açın.</span><span class="sxs-lookup"><span data-stu-id="eb402-142">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="eb402-143">Excel özet tablosunda mutabakat dosyası açma</span><span class="sxs-lookup"><span data-stu-id="eb402-143">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="eb402-144">Mutabakat dosyasını normalde olduğu gibi indirin.</span><span class="sxs-lookup"><span data-stu-id="eb402-144">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="eb402-145">Microsoft Excel'de yeni bir dosya açın.</span><span class="sxs-lookup"><span data-stu-id="eb402-145">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="eb402-146">Veri sekmesinde **Veri al'ı** seçin, **Dosyadan'ı ve ardından** **Metin/CSV'yi seçin.** </span><span class="sxs-lookup"><span data-stu-id="eb402-146">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="eb402-147">İstendiğinde, mutabakat dosyanızı açın.</span><span class="sxs-lookup"><span data-stu-id="eb402-147">When prompted, open your recon file.</span></span> <span data-ttu-id="eb402-148">Verileriniz görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="eb402-148">Your data will appear.</span></span>
5. <span data-ttu-id="eb402-149">Yükle açılan **menüsünde,** Üzerine **yükle'yi ve ardından** Tamam'ı **seçin.**</span><span class="sxs-lookup"><span data-stu-id="eb402-149">In the **Load** dropdown menu, select **Load to**, and then select **OK**.</span></span>
6. <span data-ttu-id="eb402-150">Verilerinizi İçeri **Aktar iletişim** kutusunda **PivotTable Raporu'nı seçerek** dosyanızı açın.</span><span class="sxs-lookup"><span data-stu-id="eb402-150">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="eb402-151">Negatif tutar görüntülenir</span><span class="sxs-lookup"><span data-stu-id="eb402-151">Negative amount displayed</span></span>

<span data-ttu-id="eb402-152">Mutabakat dosyanız negatif bir tutar görebilir.</span><span class="sxs-lookup"><span data-stu-id="eb402-152">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="eb402-153">Bu sorun büyük olasılıkla aşağıdakilerden biri nedeniyle oluşur:</span><span class="sxs-lookup"><span data-stu-id="eb402-153">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="eb402-154">Kısa süre önce lisanslarınızı iptal etti veya azalttınız</span><span class="sxs-lookup"><span data-stu-id="eb402-154">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="eb402-155">Hizmet lisans sözleşmesi (SLA) veya Azure tüketimi için kredi aldınız</span><span class="sxs-lookup"><span data-stu-id="eb402-155">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="eb402-156">Bu işlem hakkında daha fazla bilgi edinmek için mutabakat dosyanızda işlemin ödeme türü özniteliğini gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="eb402-156">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="eb402-157">Vergileri veya KDV'yi eşleme</span><span class="sxs-lookup"><span data-stu-id="eb402-157">Map taxes or VAT</span></span>

<span data-ttu-id="eb402-158">Vergileri veya katma değerli vergileri (KDV) faturanıza eşlemek için:</span><span class="sxs-lookup"><span data-stu-id="eb402-158">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="eb402-159">Lisans **tabanlı** dosyadan Vergi sütununu toplama.</span><span class="sxs-lookup"><span data-stu-id="eb402-159">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="eb402-160">Kullanım tabanlı **dosyadan TaxAmount** sütununu toplama.</span><span class="sxs-lookup"><span data-stu-id="eb402-160">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="eb402-161">Mutabakat dosyalarını iş ortağına göre öğeleştirme</span><span class="sxs-lookup"><span data-stu-id="eb402-161">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="eb402-162">Dolaylı modelde **iş ortakları,** bu ek alanları hem lisans tabanlı hem de kullanım tabanlı mutabakat dosyalarında kullanarak dosyaları kurumsal bayiye göre öğe hale kullanabilir.</span><span class="sxs-lookup"><span data-stu-id="eb402-162">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="eb402-163">MPN Kimliği</span><span class="sxs-lookup"><span data-stu-id="eb402-163">MPN ID</span></span> | <span data-ttu-id="eb402-164">Açıklama</span><span class="sxs-lookup"><span data-stu-id="eb402-164">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="eb402-165">MPN Kimliği</span><span class="sxs-lookup"><span data-stu-id="eb402-165">MPN ID</span></span> | <span data-ttu-id="eb402-166">Microsoft İş Ortağı Ağı (CSP) iş ortağının Bulut Çözümü Sağlayıcısı (MPN) tanımlayıcısını (doğrudan veya dolaylı).</span><span class="sxs-lookup"><span data-stu-id="eb402-166">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="eb402-167">Kurumsal Bayi MPN Kimliği</span><span class="sxs-lookup"><span data-stu-id="eb402-167">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="eb402-168">Aboneliğin [kaydının kurumsal bayisinde MPN tanımlayıcısı.](#reseller-mpn-id)</span><span class="sxs-lookup"><span data-stu-id="eb402-168">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="eb402-169">Bu alan, belirli bir abonelik için listelenen kurumsal bayi kimliğine karşılık İş Ortağı Merkezi.</span><span class="sxs-lookup"><span data-stu-id="eb402-169">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="eb402-170">Yalnızca dolaylı modelde iş ortakları için mutabakat dosyalarında görünür.</span><span class="sxs-lookup"><span data-stu-id="eb402-170">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="eb402-171">Kurumsal Bayi MPN Kimliği</span><span class="sxs-lookup"><span data-stu-id="eb402-171">Reseller MPN ID</span></span>

<span data-ttu-id="eb402-172">CsP iş ortağı aboneliği doğrudan müşteriye satsa **MPN** kimliği iki kez listelenir ve **hem MPN Kimliği** hem de **Kurumsal Bayi MPN Kimliği olarak listelenir.**</span><span class="sxs-lookup"><span data-stu-id="eb402-172">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="eb402-173">CSP iş ortağının **MPN** kimliğine sahip bir kurumsal bayisi varsa, bu değer bunun yerine iş **ortağının MPN kimliğine** ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="eb402-173">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="eb402-174">CSP iş ortağı kurumsal bayi **MPN kimliğini** kaldırırsa bu değer *-1 olarak ayarlanır.*</span><span class="sxs-lookup"><span data-stu-id="eb402-174">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="eb402-175">Kurumsal Bayi MPN Kimliğini **görüntülemek veya güncelleştirmek için:**</span><span class="sxs-lookup"><span data-stu-id="eb402-175">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="eb402-176">İş Ortağı Merkezi'nde oturum açın.</span><span class="sxs-lookup"><span data-stu-id="eb402-176">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="eb402-177">Yeni İş Ortağı Merkezi Müşteriler'i **seçin.**</span><span class="sxs-lookup"><span data-stu-id="eb402-177">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="eb402-178">Listeden müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="eb402-178">Choose the customer from the list.</span></span>
4. <span data-ttu-id="eb402-179">Müşteri menüsünde Abonelikler'i **seçin.**</span><span class="sxs-lookup"><span data-stu-id="eb402-179">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="eb402-180">Listeden aboneliği seçin.</span><span class="sxs-lookup"><span data-stu-id="eb402-180">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="eb402-181">Kurumsal **Bayiyi** **(MPN Kimliği) değiştirmek için güncelleştir'i seçin.**</span><span class="sxs-lookup"><span data-stu-id="eb402-181">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="eb402-182">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="eb402-182">Next steps</span></span>

- [<span data-ttu-id="eb402-183">Mutabakat dosyası için faturanızı & okuma</span><span class="sxs-lookup"><span data-stu-id="eb402-183">How to read your bill & recon file</span></span>](read-your-bill.md) 