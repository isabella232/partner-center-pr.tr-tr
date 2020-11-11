---
title: Karşılaştırma dosyalarınızı kullanın
ms.topic: article
ms.date: 06/08/2020
description: Iş Ortağı Merkezi 'nde mutabakat dosyaları ve belirli bir faturalandırma döngüsünün ücretlendirdiği ayrıntılı, satır öğesi görünümlerinin nasıl yorumlanacağı hakkında bilgi edinin.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d09c1e57d16937c5656579f3932e9c8feb3ecf24
ms.sourcegitcommit: 95a5afdf68d88b6be848729830dcd114e3fb0c0f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/11/2020
ms.locfileid: "94488101"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="6834f-103">Iş Ortağı Merkezi mutabakatı dosyalarınızda satır öğelerini okumayı öğrenin</span><span class="sxs-lookup"><span data-stu-id="6834f-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="6834f-104">Aşağıdakiler cihazlar için geçerlidir:</span><span class="sxs-lookup"><span data-stu-id="6834f-104">Applies to:</span></span>

- <span data-ttu-id="6834f-105">İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="6834f-105">Partner Center</span></span>
- <span data-ttu-id="6834f-106">Microsoft Cloud for US Government için İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="6834f-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="6834f-107">Bir fatura döngüsündeki her bir ücret için ayrıntılı, satır öğesi görünümü için Iş Ortağı Merkezi ' nden mutabakat dosyalarınızı indirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6834f-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="6834f-108">Satır öğesi ayrıntıları, her bir müşterinin aboneliğine ilişkin ücretleri ve ayrıntılı olayları (bir aboneliğe yönelik bir abonelik için orta dönem ekleme gibi) içerir.</span><span class="sxs-lookup"><span data-stu-id="6834f-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="6834f-109">Uygun roller:</span><span class="sxs-lookup"><span data-stu-id="6834f-109">Appropriate roles:</span></span>

- <span data-ttu-id="6834f-110">Faturalama yöneticisi</span><span class="sxs-lookup"><span data-stu-id="6834f-110">Billing admin</span></span>
- <span data-ttu-id="6834f-111">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="6834f-111">Global admin</span></span>

<span data-ttu-id="6834f-112">**Faturanızı** okuma hakkında daha fazla bilgi için bkz. [faturanızı okuyun](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="6834f-112">For information on how to read your **invoice** , see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="6834f-113">Mutabakat dosyası alanlarını anlama</span><span class="sxs-lookup"><span data-stu-id="6834f-113">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="6834f-114">Lisans tabanlı mutabakat dosya alanları</span><span class="sxs-lookup"><span data-stu-id="6834f-114">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="6834f-115">Kullanım tabanlı mutabakat dosya alanları</span><span class="sxs-lookup"><span data-stu-id="6834f-115">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="6834f-116">Günlük olarak derecelendirilen kullanım mutabakatı dosya alanları</span><span class="sxs-lookup"><span data-stu-id="6834f-116">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="6834f-117">Bir kerelik satın alma CSP 'si mutabakatı dosya alanları</span><span class="sxs-lookup"><span data-stu-id="6834f-117">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="6834f-118">Mutabakat dosyalarındaki ücretlendirme türlerini anlama</span><span class="sxs-lookup"><span data-stu-id="6834f-118">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="6834f-119">Mutabakat dosyalarındaki ( **Chargetype** sütunu) ücret türlerini anlamak için bkz. [mutabakatı dosya ücreti türleri](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="6834f-119">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="6834f-120">Biçimlendirme sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="6834f-120">Fix formatting issues</span></span>

<span data-ttu-id="6834f-121">Bazen bir mutabakat dosyasında biçimlendirme sorunları bulunabilir.</span><span class="sxs-lookup"><span data-stu-id="6834f-121">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="6834f-122">Örneğin, en-US yerel ayarı kullanılmazsa bu sorun oluşabilir.</span><span class="sxs-lookup"><span data-stu-id="6834f-122">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="6834f-123">Mutabakat dosyalarınızda biçimlendirme sorunlarını gidermek için aşağıdaki adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="6834f-123">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="6834f-124">Microsoft Excel 'de mutabakat dosyasını (. csv biçiminde) açın.</span><span class="sxs-lookup"><span data-stu-id="6834f-124">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="6834f-125">Dosyadaki ilk sütunu seçin.</span><span class="sxs-lookup"><span data-stu-id="6834f-125">Select the first column in the file.</span></span>
3. <span data-ttu-id="6834f-126">**Metni sütunlara dönüştürme Sihirbazı** ' nı açın.</span><span class="sxs-lookup"><span data-stu-id="6834f-126">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="6834f-127">Şeritte, **veriler** ' i seçin ve **sütunlar** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="6834f-127">On the ribbon, select **Data** , then select **Text to Columns**.</span></span>
4. <span data-ttu-id="6834f-128">Sihirbazda, **ayrılmış dosya türü** ' nü seçin.</span><span class="sxs-lookup"><span data-stu-id="6834f-128">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="6834f-129">Ardından **İleri** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="6834f-129">Then, select **Next**.</span></span>
5. <span data-ttu-id="6834f-130">**Sınırlayıcılar** alanında **virgül** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="6834f-130">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="6834f-131">( **Sekmesi** zaten seçildiyse, bu seçeneği seçili bırakabilirsiniz.) Ardından **İleri** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="6834f-131">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="6834f-132">**Sütun veri biçimi** alanında **Tarih: mdy** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="6834f-132">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="6834f-133">Ardından **İleri** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="6834f-133">Then, select **Next**.</span></span>
7. <span data-ttu-id="6834f-134">**Sütun veri biçimi** alanında, tüm miktar sütunları için **metin** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="6834f-134">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="6834f-135">Ardından **Son** 'u seçin.</span><span class="sxs-lookup"><span data-stu-id="6834f-135">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="6834f-136">Karşılaştırma dosyalarını programlı olarak indir</span><span class="sxs-lookup"><span data-stu-id="6834f-136">Download reconciliation files programmatically</span></span>

<span data-ttu-id="6834f-137">Mutabakat dosyaları çok büyük olabilir ve bazen indirmek zordur.</span><span class="sxs-lookup"><span data-stu-id="6834f-137">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="6834f-138">Karşılaştırma dosyalarını program aracılığıyla indirmek için bkz. [fatura satırı öğelerini Al](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="6834f-138">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="6834f-139">Vergiler veya KDV 'yi eşleştirin</span><span class="sxs-lookup"><span data-stu-id="6834f-139">Map taxes or VAT</span></span>

<span data-ttu-id="6834f-140">Vergiler veya katma değer vergi (KDV) faturanızı eşlemek için:</span><span class="sxs-lookup"><span data-stu-id="6834f-140">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="6834f-141">Lisans tabanlı dosyadaki **vergi** sütununu toplayın.</span><span class="sxs-lookup"><span data-stu-id="6834f-141">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="6834f-142">Kullanım tabanlı dosyadaki **TaxAmount** sütununu toplayın.</span><span class="sxs-lookup"><span data-stu-id="6834f-142">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="6834f-143">İş ortağına göre mutabakat dosyalarını dök</span><span class="sxs-lookup"><span data-stu-id="6834f-143">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="6834f-144">**Dolaylı modeldeki** iş ortakları, bu ek alanları hem lisans tabanlı hem de kullanım tabanlı mutabakat dosyalarında kullanarak dosyaları satıcıya göre silebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6834f-144">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="6834f-145">MPN Kimliği</span><span class="sxs-lookup"><span data-stu-id="6834f-145">MPN ID</span></span> | <span data-ttu-id="6834f-146">Açıklama</span><span class="sxs-lookup"><span data-stu-id="6834f-146">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="6834f-147">MPN Kimliği</span><span class="sxs-lookup"><span data-stu-id="6834f-147">MPN ID</span></span> | <span data-ttu-id="6834f-148">Bulut çözümü sağlayıcısı (CSP) ortağının (doğrudan veya dolaylı) Microsoft İş Ortağı Ağı (MPN) tanımlayıcısı.</span><span class="sxs-lookup"><span data-stu-id="6834f-148">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="6834f-149">Satıcı MPN KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="6834f-149">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="6834f-150">[Abonelik için kayıt satıcısının MPN tanımlayıcısı](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="6834f-150">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="6834f-151">Bu alan, Iş Ortağı Merkezi 'nde belirli bir abonelik için listelenen satıcı KIMLIĞINE karşılık gelir.</span><span class="sxs-lookup"><span data-stu-id="6834f-151">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="6834f-152">Yalnızca dolaylı modeldeki iş ortakları için mutabakat dosyaları üzerinde görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="6834f-152">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="6834f-153">Satıcı MPN KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="6834f-153">Reseller MPN ID</span></span>

<span data-ttu-id="6834f-154">Bir CSP iş ortağı aboneliği doğrudan müşteriye satmışsa **MPN kimliği** , hem **MPN kimliği** hem de **satıcı MPN kimliği** olarak iki kez listelenir.</span><span class="sxs-lookup"><span data-stu-id="6834f-154">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="6834f-155">Bir CSP iş ortağının **MPN kimliği** olmayan bir satıcısı varsa, bu değer bunun yerine ortağın **MPN kimliğine** ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="6834f-155">If a CSP partner has a reseller with no **MPN ID** , this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="6834f-156">CSP iş ortağı bir **satıcı MPN kimliğini** kaldırdığında bu değer *-1* olarak ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="6834f-156">If the CSP partner removes a **Reseller MPN ID** , this value will be set to *-1*.</span></span>

<span data-ttu-id="6834f-157">**Satıcı MPN kimliğini** görüntülemek veya güncelleştirmek için:</span><span class="sxs-lookup"><span data-stu-id="6834f-157">To view or update the **Reseller MPN ID** :</span></span>

1. <span data-ttu-id="6834f-158">İş Ortağı Merkezi'nde oturum açın.</span><span class="sxs-lookup"><span data-stu-id="6834f-158">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="6834f-159">Iş Ortağı Merkezi menüsünde **müşteriler** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="6834f-159">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="6834f-160">Listeden müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="6834f-160">Choose the customer from the list.</span></span>
4. <span data-ttu-id="6834f-161">Müşteri menüsünde **abonelikler** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="6834f-161">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="6834f-162">Listeden aboneliği seçin.</span><span class="sxs-lookup"><span data-stu-id="6834f-162">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="6834f-163">**Satıcıdan (MPN kimliği)** değiştirmek için **Güncelleştir** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="6834f-163">Select **update** to change the **Reseller (MPN ID)**.</span></span>