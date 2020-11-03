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
ms.openlocfilehash: 98bfd9a9ce6f03ad62a830f05ba82f9b90268326
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/22/2020
ms.locfileid: "92531582"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="2314c-103">Iş Ortağı Merkezi mutabakatı dosyalarınızda satır öğelerini okumayı öğrenin</span><span class="sxs-lookup"><span data-stu-id="2314c-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="2314c-104">Aşağıdakiler cihazlar için geçerlidir:</span><span class="sxs-lookup"><span data-stu-id="2314c-104">Applies to:</span></span>

- <span data-ttu-id="2314c-105">İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="2314c-105">Partner Center</span></span>
- <span data-ttu-id="2314c-106">ABD kamu için Microsoft Bulut iş ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="2314c-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="2314c-107">Bir fatura döngüsündeki her bir ücret için ayrıntılı, satır öğesi görünümü için Iş Ortağı Merkezi ' nden mutabakat dosyalarınızı indirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="2314c-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="2314c-108">Satır öğesi ayrıntıları, her bir müşterinin aboneliğine ilişkin ücretleri ve ayrıntılı olayları (bir aboneliğe yönelik bir abonelik için orta dönem ekleme gibi) içerir.</span><span class="sxs-lookup"><span data-stu-id="2314c-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="2314c-109">Uygun roller:</span><span class="sxs-lookup"><span data-stu-id="2314c-109">Appropriate roles:</span></span>

- <span data-ttu-id="2314c-110">Faturalama yöneticisi</span><span class="sxs-lookup"><span data-stu-id="2314c-110">Billing admin</span></span>
- <span data-ttu-id="2314c-111">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="2314c-111">Global admin</span></span>

<span data-ttu-id="2314c-112">**Faturanızı** okuma hakkında daha fazla bilgi için bkz. [faturanızı okuyun](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="2314c-112">For information on how to read your **invoice** , see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="2314c-113">Mutabakat dosyası alanlarını anlama</span><span class="sxs-lookup"><span data-stu-id="2314c-113">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="2314c-114">Lisans tabanlı mutabakat dosya alanları</span><span class="sxs-lookup"><span data-stu-id="2314c-114">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="2314c-115">Kullanım tabanlı mutabakat dosya alanları</span><span class="sxs-lookup"><span data-stu-id="2314c-115">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="2314c-116">Günlük olarak derecelendirilen kullanım mutabakatı dosya alanları</span><span class="sxs-lookup"><span data-stu-id="2314c-116">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="2314c-117">Mutabakat dosyalarındaki ücretlendirme türlerini anlama</span><span class="sxs-lookup"><span data-stu-id="2314c-117">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="2314c-118">Mutabakat dosyalarındaki ( **Chargetype** sütunu) ücret türlerini anlamak için bkz. [mutabakatı dosya ücreti türleri](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="2314c-118">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="2314c-119">Biçimlendirme sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="2314c-119">Fix formatting issues</span></span>

<span data-ttu-id="2314c-120">Bazen bir mutabakat dosyasında biçimlendirme sorunları bulunabilir.</span><span class="sxs-lookup"><span data-stu-id="2314c-120">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="2314c-121">Örneğin, en-US yerel ayarı kullanılmazsa bu sorun oluşabilir.</span><span class="sxs-lookup"><span data-stu-id="2314c-121">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="2314c-122">Mutabakat dosyalarınızda biçimlendirme sorunlarını gidermek için aşağıdaki adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="2314c-122">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="2314c-123">Microsoft Excel 'de mutabakat dosyasını (. csv biçiminde) açın.</span><span class="sxs-lookup"><span data-stu-id="2314c-123">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="2314c-124">Dosyadaki ilk sütunu seçin.</span><span class="sxs-lookup"><span data-stu-id="2314c-124">Select the first column in the file.</span></span>
3. <span data-ttu-id="2314c-125">**Metni sütunlara dönüştürme Sihirbazı** ' nı açın.</span><span class="sxs-lookup"><span data-stu-id="2314c-125">Open the **Convert Text to Columns Wizard** .</span></span> <span data-ttu-id="2314c-126">Şeritte, **veriler** ' i seçin ve **sütunlar** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="2314c-126">On the ribbon, select **Data** , then select **Text to Columns** .</span></span>
4. <span data-ttu-id="2314c-127">Sihirbazda, **ayrılmış dosya türü** ' nü seçin.</span><span class="sxs-lookup"><span data-stu-id="2314c-127">In the wizard, select **Delimited file type** .</span></span> <span data-ttu-id="2314c-128">Ardından **İleri** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="2314c-128">Then, select **Next** .</span></span>
5. <span data-ttu-id="2314c-129">**Sınırlayıcılar** alanında **virgül** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="2314c-129">In the **Delimiters** field, select **Comma** .</span></span> <span data-ttu-id="2314c-130">( **Sekmesi** zaten seçildiyse, bu seçeneği seçili bırakabilirsiniz.) Ardından **İleri** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="2314c-130">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next** .</span></span>
6. <span data-ttu-id="2314c-131">**Sütun veri biçimi** alanında **Tarih: mdy** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="2314c-131">In the **Column data format** field, select **Date:MDY** .</span></span> <span data-ttu-id="2314c-132">Ardından **İleri** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="2314c-132">Then, select **Next** .</span></span>
7. <span data-ttu-id="2314c-133">**Sütun veri biçimi** alanında, tüm miktar sütunları için **metin** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="2314c-133">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="2314c-134">Ardından **Son** 'u seçin.</span><span class="sxs-lookup"><span data-stu-id="2314c-134">Then, select **Finish** .</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="2314c-135">Karşılaştırma dosyalarını programlı olarak indir</span><span class="sxs-lookup"><span data-stu-id="2314c-135">Download reconciliation files programmatically</span></span>

<span data-ttu-id="2314c-136">Mutabakat dosyaları çok büyük olabilir ve bazen indirmek zordur.</span><span class="sxs-lookup"><span data-stu-id="2314c-136">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="2314c-137">Karşılaştırma dosyalarını program aracılığıyla indirmek için bkz. [fatura satırı öğelerini Al](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="2314c-137">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="2314c-138">Vergiler veya KDV 'yi eşleştirin</span><span class="sxs-lookup"><span data-stu-id="2314c-138">Map taxes or VAT</span></span>

<span data-ttu-id="2314c-139">Vergiler veya katma değer vergi (KDV) faturanızı eşlemek için:</span><span class="sxs-lookup"><span data-stu-id="2314c-139">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="2314c-140">Lisans tabanlı dosyadaki **vergi** sütununu toplayın.</span><span class="sxs-lookup"><span data-stu-id="2314c-140">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="2314c-141">Kullanım tabanlı dosyadaki **TaxAmount** sütununu toplayın.</span><span class="sxs-lookup"><span data-stu-id="2314c-141">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="2314c-142">İş ortağına göre mutabakat dosyalarını dök</span><span class="sxs-lookup"><span data-stu-id="2314c-142">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="2314c-143">**Dolaylı modeldeki** iş ortakları, bu ek alanları hem lisans tabanlı hem de kullanım tabanlı mutabakat dosyalarında kullanarak dosyaları satıcıya göre silebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="2314c-143">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="2314c-144">MPN Kimliği</span><span class="sxs-lookup"><span data-stu-id="2314c-144">MPN ID</span></span> | <span data-ttu-id="2314c-145">Açıklama</span><span class="sxs-lookup"><span data-stu-id="2314c-145">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="2314c-146">MPN Kimliği</span><span class="sxs-lookup"><span data-stu-id="2314c-146">MPN ID</span></span> | <span data-ttu-id="2314c-147">Bulut çözümü sağlayıcısı (CSP) ortağının (doğrudan veya dolaylı) Microsoft İş Ortağı Ağı (MPN) tanımlayıcısı.</span><span class="sxs-lookup"><span data-stu-id="2314c-147">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="2314c-148">Satıcı MPN KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="2314c-148">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="2314c-149">[Abonelik için kayıt satıcısının MPN tanımlayıcısı](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="2314c-149">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="2314c-150">Bu alan, Iş Ortağı Merkezi 'nde belirli bir abonelik için listelenen satıcı KIMLIĞINE karşılık gelir.</span><span class="sxs-lookup"><span data-stu-id="2314c-150">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="2314c-151">Yalnızca dolaylı modeldeki iş ortakları için mutabakat dosyaları üzerinde görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="2314c-151">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="2314c-152">Satıcı MPN KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="2314c-152">Reseller MPN ID</span></span>

<span data-ttu-id="2314c-153">Bir CSP iş ortağı aboneliği doğrudan müşteriye satmışsa **MPN kimliği** , hem **MPN kimliği** hem de **satıcı MPN kimliği** olarak iki kez listelenir.</span><span class="sxs-lookup"><span data-stu-id="2314c-153">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID** .</span></span>

<span data-ttu-id="2314c-154">Bir CSP iş ortağının **MPN kimliği** olmayan bir satıcısı varsa, bu değer bunun yerine ortağın **MPN kimliğine** ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="2314c-154">If a CSP partner has a reseller with no **MPN ID** , this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="2314c-155">CSP iş ortağı bir **satıcı MPN kimliğini** kaldırdığında bu değer *-1* olarak ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="2314c-155">If the CSP partner removes a **Reseller MPN ID** , this value will be set to *-1* .</span></span>

<span data-ttu-id="2314c-156">**Satıcı MPN kimliğini** görüntülemek veya güncelleştirmek için:</span><span class="sxs-lookup"><span data-stu-id="2314c-156">To view or update the **Reseller MPN ID** :</span></span>

1. <span data-ttu-id="2314c-157">İş Ortağı Merkezi'nde oturum açın.</span><span class="sxs-lookup"><span data-stu-id="2314c-157">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="2314c-158">Iş Ortağı Merkezi menüsünde **müşteriler** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="2314c-158">In the Partner Center menu, select **Customers** .</span></span>
3. <span data-ttu-id="2314c-159">Listeden müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="2314c-159">Choose the customer from the list.</span></span>
4. <span data-ttu-id="2314c-160">Müşteri menüsünde **abonelikler** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="2314c-160">In the customer menu, select **Subscriptions** .</span></span>
5. <span data-ttu-id="2314c-161">Listeden aboneliği seçin.</span><span class="sxs-lookup"><span data-stu-id="2314c-161">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="2314c-162">**Satıcıdan (MPN kimliği)** değiştirmek için **Güncelleştir** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="2314c-162">Select **update** to change the **Reseller (MPN ID)** .</span></span>