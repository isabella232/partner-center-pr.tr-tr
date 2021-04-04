---
title: Mart 2021 duyuruları
description: Yeni yetenekler, promosyonlar, teklifler, pazarlar veya mevcut tekliflerle ilgili değişiklikler dahil olmak üzere Microsoft Iş Ortağı Merkezi için Mart 2021 duyuruları.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 5b8c5f52207a7b9a49d07885a36b61486be45497
ms.sourcegitcommit: 60bbb8f4056120264b769f94431f84d86984c2e9
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/03/2021
ms.locfileid: "106280879"
---
# <a name="march-2021-announcements"></a><span data-ttu-id="fcd31-103">Mart 2021 duyuruları</span><span class="sxs-lookup"><span data-stu-id="fcd31-103">March 2021 announcements</span></span>

<span data-ttu-id="fcd31-104">Bu sayfada Mart 2021 için Microsoft Iş Ortağı Merkezi duyuruları sağlanmaktadır.</span><span class="sxs-lookup"><span data-stu-id="fcd31-104">This page provides the announcements for Microsoft Partner Center for March 2021.</span></span>

________________
## <a name="updated-csp-customer-address-validation-api-now-available-for-testing"></a><a name="18"></a><span data-ttu-id="fcd31-105">Güncelleştirilmiş CSP müşteri adresi doğrulama API 'SI artık test için kullanılabilir</span><span class="sxs-lookup"><span data-stu-id="fcd31-105">Updated CSP customer address validation API now available for testing</span></span>

### <a name="categories"></a><span data-ttu-id="fcd31-106">Kategoriler</span><span class="sxs-lookup"><span data-stu-id="fcd31-106">Categories</span></span>

- <span data-ttu-id="fcd31-107">Tarih: 2021-03-31</span><span class="sxs-lookup"><span data-stu-id="fcd31-107">Date: 2021-03-31</span></span>
- <span data-ttu-id="fcd31-108">Özellikler</span><span class="sxs-lookup"><span data-stu-id="fcd31-108">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="fcd31-109">Özet</span><span class="sxs-lookup"><span data-stu-id="fcd31-109">Summary</span></span>

<span data-ttu-id="fcd31-110">İş ortakları ve müşterilerin işletmelerini temel alarak işlerini çalıştırmasına yardımcı olma taahhüdünün bir parçası olarak, dünyanın her yerindeki ortakları, bu değişiklikleri ValidateAddress API 'sinde test edecek şekilde davet edeceğiz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-110">As part of our commitment to help partners and customers run their business based on trust, we will be inviting partners worldwide to test the changes to the ValidateAddress API.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcd31-111">Etkilenen hedef kitle</span><span class="sxs-lookup"><span data-stu-id="fcd31-111">Impacted audience</span></span>

<span data-ttu-id="fcd31-112">Tüm CSP doğrudan fatura ortakları ve yeni bir Kullanıcı oluşturan veya mevcut müşteri adresi ayrıntılarını güncelleştiren dolaylı sağlayıcılar</span><span class="sxs-lookup"><span data-stu-id="fcd31-112">All CSP direct bill partners and indirect providers who create new or update existing customer address details</span></span>

### <a name="details"></a><span data-ttu-id="fcd31-113">Ayrıntılar</span><span class="sxs-lookup"><span data-stu-id="fcd31-113">Details</span></span>

<span data-ttu-id="fcd31-114">Microsoft, güvende çalışır.</span><span class="sxs-lookup"><span data-stu-id="fcd31-114">Microsoft runs on trust.</span></span> <span data-ttu-id="fcd31-115">CSP programında deneyimidir müşteri abonelikleri için müşteri adresi doğrulama göndermek için uyumlu, güvenli ve güvenli bir yöntem sağlamayı taahhüt ediyoruz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-115">We’re committed to providing a compliant, safe, and secure method of submitting customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="fcd31-116">31 Mart 2021 ' de bugün, Haziran 2021 ' deki değişikliklerle çalışmaya başlamadan önce, test etmeyi davet etmek istediğimiz ValidateAddress API 'sinde değişiklikler yaptık.</span><span class="sxs-lookup"><span data-stu-id="fcd31-116">Today, March 31, 2021, we have introduced changes to the ValidateAddress API that we’d like to invite you to test, prior to going live with the changes in June 2021.</span></span> 

<span data-ttu-id="fcd31-117">Bu değişikliklerin yalnızca ValidateAddress API 'sini etkilediğini unutmayın.</span><span class="sxs-lookup"><span data-stu-id="fcd31-117">Note that these changes affect the ValidateAddress API only.</span></span> <span data-ttu-id="fcd31-118">CreateCustomer ve UpdateBillingProfile API 'Leri etkilenmez.</span><span class="sxs-lookup"><span data-stu-id="fcd31-118">CreateCustomer and UpdateBillingProfile APIs are not affected.</span></span>

<span data-ttu-id="fcd31-119">Yanıt aşağıdaki durum iletilerinden birini döndürür:</span><span class="sxs-lookup"><span data-stu-id="fcd31-119">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="fcd31-120">Durum</span><span class="sxs-lookup"><span data-stu-id="fcd31-120">Status</span></span> | <span data-ttu-id="fcd31-121">Açıklama</span><span class="sxs-lookup"><span data-stu-id="fcd31-121">Description</span></span> | <span data-ttu-id="fcd31-122">Döndürülen önerilen adreslerin sayısı</span><span class="sxs-lookup"><span data-stu-id="fcd31-122">Number of suggested addresses returned</span></span> |
|----------|-------------|-------------------|
| <span data-ttu-id="fcd31-123">VerifiedShippable</span><span class="sxs-lookup"><span data-stu-id="fcd31-123">VerifiedShippable</span></span> | <span data-ttu-id="fcd31-124">Adres doğrulanır ve sevk edilebilir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-124">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="fcd31-125">Tek</span><span class="sxs-lookup"><span data-stu-id="fcd31-125">Single</span></span> |
| <span data-ttu-id="fcd31-126">Doğrulanamayan</span><span class="sxs-lookup"><span data-stu-id="fcd31-126">Verified</span></span> | <span data-ttu-id="fcd31-127">Adres doğrulandı.</span><span class="sxs-lookup"><span data-stu-id="fcd31-127">Address is verified.</span></span> | <span data-ttu-id="fcd31-128">Tek</span><span class="sxs-lookup"><span data-stu-id="fcd31-128">Single</span></span> |
| <span data-ttu-id="fcd31-129">Interactionrequired</span><span class="sxs-lookup"><span data-stu-id="fcd31-129">InteractionRequired</span></span> | <span data-ttu-id="fcd31-130">Önerilen adresler önemli ölçüde değiştirilmiştir ve kullanıcı onayı gerekir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-130">Suggested address(es) has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="fcd31-131">Tek</span><span class="sxs-lookup"><span data-stu-id="fcd31-131">Single</span></span> |
| <span data-ttu-id="fcd31-132">StreetPartial</span><span class="sxs-lookup"><span data-stu-id="fcd31-132">StreetPartial</span></span> | <span data-ttu-id="fcd31-133">Adreste verilen cadde kısmi ve daha fazla bilgi gerekiyor.</span><span class="sxs-lookup"><span data-stu-id="fcd31-133">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="fcd31-134">Birden çok — en fazla üç</span><span class="sxs-lookup"><span data-stu-id="fcd31-134">Multiple—maximum of three</span></span>|
| <span data-ttu-id="fcd31-135">PremisesPartial</span><span class="sxs-lookup"><span data-stu-id="fcd31-135">PremisesPartial</span></span> | <span data-ttu-id="fcd31-136">Verilen şirket içi (bina numarası, paket numarası, vb.) kısmi ve daha fazla bilgi gerektirir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-136">The given premises (building number, suite number, etc.) is partial and needs more info.</span></span> | <span data-ttu-id="fcd31-137">Birden çok — en fazla üç</span><span class="sxs-lookup"><span data-stu-id="fcd31-137">Multiple—maximum of three</span></span> |
| <span data-ttu-id="fcd31-138">Birden çok</span><span class="sxs-lookup"><span data-stu-id="fcd31-138">Multiple</span></span> | <span data-ttu-id="fcd31-139">Adreste kısmi olan birden çok alan vardır (büyük olasılıkla StreetPartial ve PremisesPartial de dahil).</span><span class="sxs-lookup"><span data-stu-id="fcd31-139">There are multiple fields that are partial in the address (potentially also including StreetPartial and PremisesPartial).</span></span> | <span data-ttu-id="fcd31-140">Birden çok — en fazla üç</span><span class="sxs-lookup"><span data-stu-id="fcd31-140">Multiple—maximum of three</span></span> |
| <span data-ttu-id="fcd31-141">Yok</span><span class="sxs-lookup"><span data-stu-id="fcd31-141">None</span></span> | <span data-ttu-id="fcd31-142">Adres yanlış.</span><span class="sxs-lookup"><span data-stu-id="fcd31-142">Address is incorrect.</span></span> | <span data-ttu-id="fcd31-143">Yok</span><span class="sxs-lookup"><span data-stu-id="fcd31-143">None</span></span> |
| <span data-ttu-id="fcd31-144">Notdoðrulanmış</span><span class="sxs-lookup"><span data-stu-id="fcd31-144">NotValidated</span></span> | <span data-ttu-id="fcd31-145">Adres, doğrulama işlemi aracılığıyla gönderilemedi.</span><span class="sxs-lookup"><span data-stu-id="fcd31-145">Address was not able to be sent through the validation process.</span></span>  | <span data-ttu-id="fcd31-146">Yok</span><span class="sxs-lookup"><span data-stu-id="fcd31-146">None</span></span> |

<span data-ttu-id="fcd31-147">Bir adres, ValidateAddress API aracılığıyla doğrulanacak şekilde gönderildikten sonra, aşağıdaki yanıt şeması döndürülür:</span><span class="sxs-lookup"><span data-stu-id="fcd31-147">Once an address has been submitted to be validated via the ValidateAddress API, the following response schema will be returned:</span></span>

```csharp

// <summary>
/// Object represents the address validation response.
/// </summary>

public class AddressValidationResponse
{
   /// <summary>
   /// Gets or sets the original address
   /// </summary>
   /// <value>
   /// Original Address
   /// </value>
   public Address OriginalAddress { get; set; }

   /// <summary>
   /// Gets or sets the suggested addresses
   /// </summary>
   /// <value>
   /// Suggested Addresses
   /// </value>
   public List<Address> SuggestedAddresses { get; set; }

   /// <summary>
   /// Gets or sets the validation status
   /// </summary>
   /// <value>
   /// Status
   /// </value>
   public string Status { get; set; }

   /// <summary>
   /// Gets or sets the validation message
   /// </summary>
   /// <value>
   /// Validation Message
   /// </value>
   public string ValidationMessage { get; set; }
   ```

<span data-ttu-id="fcd31-148">Bu örnek yanıta göz atın.</span><span class="sxs-lookup"><span data-stu-id="fcd31-148">Take a look at this sample response.</span></span> <span data-ttu-id="fcd31-149">ABD için, posta kodu için yalnızca beş basamak girerseniz, yanıt posta kodu satırı için dört basamaklı ek bir sonek döndürdüğüne göz önünde koyun.</span><span class="sxs-lookup"><span data-stu-id="fcd31-149">Note that for the US, the response will return an additional four-digit suffix for the postal code line if you only enter five digits for the zip code.</span></span>

```csharp
// IAggregatePartner partnerOperations;
// string customerId;
// s{
"suggested_address": {
    "Country": "US",
    "region": "WA",
    "city": "Redmond",
    "address_line1": "1 Microsoft Way",
    "postal_Code": "98052-8300"
},
"original_address": {
    "Country": "US",
    "region": "WA",
    "city": "Redmond",
    "address_line1": "1 Micro Way",
    "postal_Code": "98052"
},
"status":  "InteractionRequired",
"validation_message": "Address field invalid for property: ‘Street’"
}
```

### <a name="next-steps"></a><span data-ttu-id="fcd31-150">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="fcd31-150">Next steps</span></span>

- <span data-ttu-id="fcd31-151">Güncelleştirme için hazırlamaya başlayabilmeniz için, korumalı alan kiracı KIMLIĞINIZI konu uzmanı uzmanlığımızı (SME), Ali Haki 'yı test uçuşla birlikte paylaşabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-151">Share your sandbox tenant ID with our subject matter expert (SME), Ali Khaki, to be included in the test flight, so that you can begin preparing for the update.</span></span>

- <span data-ttu-id="fcd31-152">Bir denetim masası satıcısı (CPV) çözümü kullanıyorsanız, CPV 'nize başvurun.</span><span class="sxs-lookup"><span data-stu-id="fcd31-152">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="fcd31-153">Sorularınız mı var?</span><span class="sxs-lookup"><span data-stu-id="fcd31-153">Questions?</span></span>

<span data-ttu-id="fcd31-154">Microsoft ile işlemlerinizin herhangi bir sorunuz varsa veya sizin için destek gerekiyorsa, iş ortağı destek Yammer grubuna ulaşın.</span><span class="sxs-lookup"><span data-stu-id="fcd31-154">If you have any questions or need support for your operations with Microsoft, reach out to your partner support Yammer group.</span></span>

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a><span data-ttu-id="fcd31-155">Yeni Exchange Yönetim Merkezi (EAC) deneyimi</span><span class="sxs-lookup"><span data-stu-id="fcd31-155">New Exchange admin center (EAC) experience</span></span>

### <a name="categories"></a><span data-ttu-id="fcd31-156">Kategoriler</span><span class="sxs-lookup"><span data-stu-id="fcd31-156">Categories</span></span>

- <span data-ttu-id="fcd31-157">Tarih: 2021-03-29</span><span class="sxs-lookup"><span data-stu-id="fcd31-157">Date: 2021-03-29</span></span>
- <span data-ttu-id="fcd31-158">Özellikler</span><span class="sxs-lookup"><span data-stu-id="fcd31-158">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="fcd31-159">Özet</span><span class="sxs-lookup"><span data-stu-id="fcd31-159">Summary</span></span>

<span data-ttu-id="fcd31-160">27 Nisan 2021 ' den itibaren, Exchange Yönetim Merkezi (EAC), kullanıcılar için günlük verimliliği artıran yeni bir deneyim çıkarır.</span><span class="sxs-lookup"><span data-stu-id="fcd31-160">Starting April 27, 2021, the Exchange admin center (EAC) will roll out a new experience that will improve day-to-day efficiency for users.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcd31-161">Etkilenen hedef kitle</span><span class="sxs-lookup"><span data-stu-id="fcd31-161">Impacted audience</span></span>

<span data-ttu-id="fcd31-162">Iş Ortağı Merkezi aracılığıyla Exchange 'e erişen yönetici temsilcileri</span><span class="sxs-lookup"><span data-stu-id="fcd31-162">Delegated admins accessing Exchange through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="fcd31-163">Ayrıntılar</span><span class="sxs-lookup"><span data-stu-id="fcd31-163">Details</span></span>

<span data-ttu-id="fcd31-164">27 Nisan 2021 ' den itibaren, Iş Ortağı Merkezi aracılığıyla Exchange 'e gitten iş ortakları yeni EAC 'ya yönlendirilir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-164">Starting April 27, 2021, partners who navigate to Exchange through Partner Center will be redirected to the new EAC.</span></span>

<span data-ttu-id="fcd31-165">Bu yeni deneyim Şu anda önizleme olarak sunulmaktadır ve Yöneticiler, klasik EAC içinde sağ üst köşedeki geçişi seçerek bu deneyimi etkinleştirebilir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-165">This new experience is currently available as a preview, and admins can activate this experience by selecting the toggle on the top right corner within the classic EAC.</span></span> <span data-ttu-id="fcd31-166">Ayrıca, tüm sayfalarda görüntülenen "Şimdi deneyin" başlığını seçerek yeni duyak 'e gidebilir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-166">They can also navigate to the new EAC by selecting the “Try it now” banner that’s displayed on all the pages.</span></span>

<span data-ttu-id="fcd31-167">Yeni EAC 'nin avantajları şunlardır:</span><span class="sxs-lookup"><span data-stu-id="fcd31-167">Benefits of the new EAC include:</span></span>

- <span data-ttu-id="fcd31-168">Posta akışı ile ilgili sorunlar için Öngörüler, raporlar ve uyarı mekanizmaları eklendi.</span><span class="sxs-lookup"><span data-stu-id="fcd31-168">Added insights, reports, and alert mechanisms for mail flow–related issues.</span></span> 

- <span data-ttu-id="fcd31-169">Üretkenliği artırmak için kişiselleştirilmiş panolar.</span><span class="sxs-lookup"><span data-stu-id="fcd31-169">Personalized dashboards to increase productivity.</span></span>

<span data-ttu-id="fcd31-170">Yeni deneyimin içinde gezinmenize yardımcı olmak için, yeni EAC deneyiminde **eğitim & Kılavuzu** bölümünde videolar bulunur.</span><span class="sxs-lookup"><span data-stu-id="fcd31-170">To help you navigate through the new experience, videos are available within the **Training & Guide** section on the new EAC experience.</span></span> <span data-ttu-id="fcd31-171">Bu, size yeni portalı en iyi şekilde nasıl kullanabileceğinizi gösteren bir genel bakış sunar.</span><span class="sxs-lookup"><span data-stu-id="fcd31-171">These will give you an overview of how you can best use the new portal.</span></span>

>[!NOTE]
><span data-ttu-id="fcd31-172">Bu değişiklik ile klasik EAC deneyimi kullanım dışı olmayacaktır.</span><span class="sxs-lookup"><span data-stu-id="fcd31-172">With this change, the classic EAC experience will not be deprecated.</span></span> <span data-ttu-id="fcd31-173">Herhangi bir değişiklik uygulanmadan önce iyi bir bildirim alırsınız.</span><span class="sxs-lookup"><span data-stu-id="fcd31-173">You will be notified well in advance before any change is implemented.</span></span>

### <a name="next-steps"></a><span data-ttu-id="fcd31-174">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="fcd31-174">Next steps</span></span>

- <span data-ttu-id="fcd31-175">Yeni deneyimin ekran görüntülerini görüntüleyebileceğiniz [Bu konuyla ilgili kaynaklara](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/)göz atın.</span><span class="sxs-lookup"><span data-stu-id="fcd31-175">Check out the [resources about this topic](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), where you can view screenshots of the new experience.</span></span>

- <span data-ttu-id="fcd31-176">Bu bilgileri, kuruluşunuzdaki uygun paydaşlarla paylaşabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-176">Share this information with the appropriate stakeholders in your organization.</span></span> 

### <a name="questions"></a><span data-ttu-id="fcd31-177">Sorularınız mı var?</span><span class="sxs-lookup"><span data-stu-id="fcd31-177">Questions?</span></span>

<span data-ttu-id="fcd31-178">Bu değişiklikler hakkında herhangi bir soru için ilgili Yammer topluluklarınızı kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="fcd31-178">For any questions about these changes, check your relevant Yammer communities.</span></span>

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a><span data-ttu-id="fcd31-179">Microsoft Işlemleri: ürün başlatma takvimini tanıtma</span><span class="sxs-lookup"><span data-stu-id="fcd31-179">Microsoft Operations: Introducing the product launch calendar</span></span>

### <a name="categories"></a><span data-ttu-id="fcd31-180">Kategoriler</span><span class="sxs-lookup"><span data-stu-id="fcd31-180">Categories</span></span>

- <span data-ttu-id="fcd31-181">Tarih: 2021-03-25</span><span class="sxs-lookup"><span data-stu-id="fcd31-181">Date: 2021-03-25</span></span>
- <span data-ttu-id="fcd31-182">Teklifler | Modern çalışma alanı</span><span class="sxs-lookup"><span data-stu-id="fcd31-182">Offers | Modern Workplace</span></span>

### <a name="summary"></a><span data-ttu-id="fcd31-183">Özet</span><span class="sxs-lookup"><span data-stu-id="fcd31-183">Summary</span></span>

<span data-ttu-id="fcd31-184">İş ortağı geri bildirimlerine yanıt olarak, Microsoft Işlemleri ürün başlatma ile ilgili iletişimleri kolaylaştıracaktır.</span><span class="sxs-lookup"><span data-stu-id="fcd31-184">In response to partner feedback, Microsoft Operations will streamline communications for product launches.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcd31-185">Etkilenen hedef kitle</span><span class="sxs-lookup"><span data-stu-id="fcd31-185">Impacted audience</span></span>

<span data-ttu-id="fcd31-186">Bulut çözümü sağlayıcısı (CSP) iş ortakları</span><span class="sxs-lookup"><span data-stu-id="fcd31-186">Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="fcd31-187">Ayrıntılar</span><span class="sxs-lookup"><span data-stu-id="fcd31-187">Details</span></span>

<span data-ttu-id="fcd31-188">Microsoft, iş ortağı deneyimlerini sürekli olarak geliştirmeye kararlıdır.</span><span class="sxs-lookup"><span data-stu-id="fcd31-188">Microsoft is committed to continually improving partner experiences.</span></span> <span data-ttu-id="fcd31-189">Microsoft 'tan çok fazla iletişim aldığınızı ve ürün başlatma için tekrarlanan Duyurular dahil ettiğimiz hakkında geri bildirimde bulunduk.</span><span class="sxs-lookup"><span data-stu-id="fcd31-189">We’ve had feedback from you that you’ve been receiving too many communications from Microsoft, including duplicate announcements for product launches.</span></span>

<span data-ttu-id="fcd31-190">Microsoft, geri bildiriminiz doğrultusunda, yeni ve mevcut tekliflerle ilgili ürün için hazırlık deneyimini kolaylaştırmıştır.</span><span class="sxs-lookup"><span data-stu-id="fcd31-190">In response to your feedback, Microsoft has streamlined the readiness experience for product launches for new and existing offers.</span></span>

<span data-ttu-id="fcd31-191">Artık, Işlem hazırlık kaynağı galerisinde yayınlanan ürünün tek bir aylık görünümünü sunuyoruz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-191">We now provide you with a single monthly view of product launches, published in the Operations readiness resource gallery.</span></span> <span data-ttu-id="fcd31-192">Bu aylık [ürün başlatma takvimi görünümü](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) , işlem hazırlık kaynağı galerisindeki ve Iş Ortağı Merkezi bildirilerinde tek tek ürün başlatma iletişimlerinin yerini alır.</span><span class="sxs-lookup"><span data-stu-id="fcd31-192">This monthly [product launch calendar view](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) will replace individual product launch communications in the Operations readiness resource gallery and in Partner Center announcements.</span></span>

<span data-ttu-id="fcd31-193">Bu [ürün başlatma takvimine](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) [topluluk koleksiyonları](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [Takvim görünümleri](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated)ve [CSP bültenleri](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)' nden de erişebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-193">You can also access this [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) from [community collections](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [calendar views](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated), and [CSP newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span></span> <span data-ttu-id="fcd31-194">Her ayın ürün başlatma takvimini, Işlem hazırlık kaynağı galerisinde bir duyuru ile yayımladığımızda sizi bilgilendireceğiz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-194">We’ll notify you when we publish each month’s product launch calendar with an announcement in the Operations readiness resource gallery.</span></span>

<span data-ttu-id="fcd31-195">Fiyat listesi önizlemesi ve fiyat listesi değişiklik günlüklerinde ve ürün bloglarında, lisanslama kılavuzlarında ve ürün pazarlama sayfalarında yeni ve mevcut tekliflerle ilgili bilgiler bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-195">You can still find information regarding new and existing offers in the price list preview and price list change logs, as well as in product blogs, licensing guides, and product marketing pages.</span></span>

<span data-ttu-id="fcd31-196">Değişiklik, aşağıdaki ürünler için başlatılır.</span><span class="sxs-lookup"><span data-stu-id="fcd31-196">The change will apply to launches for the following products:</span></span>

- <span data-ttu-id="fcd31-197">Dynamics şirket içi</span><span class="sxs-lookup"><span data-stu-id="fcd31-197">Dynamics on-premises</span></span>
- <span data-ttu-id="fcd31-198">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="fcd31-198">Microsoft 365</span></span>
- <span data-ttu-id="fcd31-199">Microsoft Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="fcd31-199">Microsoft Dynamics 365</span></span>
- <span data-ttu-id="fcd31-200">Windows</span><span class="sxs-lookup"><span data-stu-id="fcd31-200">Windows</span></span>
- <span data-ttu-id="fcd31-201">Sunucu</span><span class="sxs-lookup"><span data-stu-id="fcd31-201">Server</span></span>  
- <span data-ttu-id="fcd31-202">Araçlar</span><span class="sxs-lookup"><span data-stu-id="fcd31-202">Tools</span></span>
- <span data-ttu-id="fcd31-203">Takımlar ve Telco</span><span class="sxs-lookup"><span data-stu-id="fcd31-203">Teams and Telco</span></span>

<span data-ttu-id="fcd31-204">Işlem hazırlığı ayrıntıları gerektiren ürün başlatma için özel duyurular gönderilmeye devam edeceğiz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-204">We’ll continue to send specific announcements for product launches that require Operations readiness details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="fcd31-205">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="fcd31-205">Next steps</span></span>

<span data-ttu-id="fcd31-206">Bu konuyla ilgili kaynakları gözden geçirin ve bu bilgileri kuruluşunuzdaki uygun hissedarlarla paylaşabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-206">Review the resources about this topic and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="fcd31-207">Sorularınız mı var?</span><span class="sxs-lookup"><span data-stu-id="fcd31-207">Questions?</span></span>

<span data-ttu-id="fcd31-208">Bu teklifler hakkında daha fazla soru için ilgili Yammer topluluklarınızı kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="fcd31-208">For any further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a><span data-ttu-id="fcd31-209">CSP müşteri ekleme gereksinimlerinde yapılan değişiklikler</span><span class="sxs-lookup"><span data-stu-id="fcd31-209">Changes to CSP customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="fcd31-210">Kategoriler</span><span class="sxs-lookup"><span data-stu-id="fcd31-210">Categories</span></span>

- <span data-ttu-id="fcd31-211">Tarih: 2021-03-25</span><span class="sxs-lookup"><span data-stu-id="fcd31-211">Date: 2021-03-25</span></span>
- <span data-ttu-id="fcd31-212">Özellikler</span><span class="sxs-lookup"><span data-stu-id="fcd31-212">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="fcd31-213">Özet</span><span class="sxs-lookup"><span data-stu-id="fcd31-213">Summary</span></span>

<span data-ttu-id="fcd31-214">İş ortakları ve müşterilerin işlerini güvenle çalıştırmasına yardımcı olma çabamız kapsamında, 25 Mart 2021 ' den itibaren geçerli olan ek müşteri bilgileri isteyeceğiz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-214">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcd31-215">Etkilenen hedef kitle</span><span class="sxs-lookup"><span data-stu-id="fcd31-215">Impacted audience</span></span>

<span data-ttu-id="fcd31-216">Bulut çözümü sağlayıcısı (CSP) doğrudan fatura ortakları ve sonraki bölümde listelenen ülkelerde yeni veya mevcut müşterileri olan dolaylı sağlayıcılar</span><span class="sxs-lookup"><span data-stu-id="fcd31-216">Cloud Solution Provider (CSP) direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="fcd31-217">Ayrıntılar</span><span class="sxs-lookup"><span data-stu-id="fcd31-217">Details</span></span>

<span data-ttu-id="fcd31-218">Microsoft, güvende çalışır.</span><span class="sxs-lookup"><span data-stu-id="fcd31-218">Microsoft runs on trust.</span></span> <span data-ttu-id="fcd31-219">CSP programında deneyimidir müşteri abonelikleri için uyumlu, güvenli ve güvenli bir müşteri doğrulama yöntemi sağlamayı taahhüt ediyoruz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-219">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="fcd31-220">25 Mart 2021 ' de, aşağıdaki ölçütlerin her ikisini de karşılayan iş ortaklarını etkileyecek Iş Ortağı Merkezi API 'SI ve Kullanıcı arabirimi (UI) geliştirmeleri sunacağız:</span><span class="sxs-lookup"><span data-stu-id="fcd31-220">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

1. <span data-ttu-id="fcd31-221">İş ortağı Microsoft ile doğrudan faturalandırma ilişkisine sahiptir (Bu, ortağın doğrudan bir fatura ortağı veya dolaylı bir sağlayıcı olduğu anlamına gelir).</span><span class="sxs-lookup"><span data-stu-id="fcd31-221">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

2. <span data-ttu-id="fcd31-222">İş ortağı aşağıdaki ülkelerde yeni veya mevcut müşteriler ile iş yapar:</span><span class="sxs-lookup"><span data-stu-id="fcd31-222">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="fcd31-223">Tayland</span><span class="sxs-lookup"><span data-stu-id="fcd31-223">Thailand</span></span>
    - <span data-ttu-id="fcd31-224">Vietnam</span><span class="sxs-lookup"><span data-stu-id="fcd31-224">Vietnam</span></span>
    - <span data-ttu-id="fcd31-225">Türkiye</span><span class="sxs-lookup"><span data-stu-id="fcd31-225">Turkey</span></span>
    - <span data-ttu-id="fcd31-226">Polonya</span><span class="sxs-lookup"><span data-stu-id="fcd31-226">Poland</span></span>
    - <span data-ttu-id="fcd31-227">Güney Afrika</span><span class="sxs-lookup"><span data-stu-id="fcd31-227">South Africa</span></span>
    - <span data-ttu-id="fcd31-228">Hindistan</span><span class="sxs-lookup"><span data-stu-id="fcd31-228">India</span></span>
    - <span data-ttu-id="fcd31-229">Brezilya</span><span class="sxs-lookup"><span data-stu-id="fcd31-229">Brazil</span></span>
    - <span data-ttu-id="fcd31-230">Irak</span><span class="sxs-lookup"><span data-stu-id="fcd31-230">Iraq</span></span>
    - <span data-ttu-id="fcd31-231">Myanmar</span><span class="sxs-lookup"><span data-stu-id="fcd31-231">Myanmar</span></span>
    - <span data-ttu-id="fcd31-232">Güney Sudan</span><span class="sxs-lookup"><span data-stu-id="fcd31-232">South Sudan</span></span>
    - <span data-ttu-id="fcd31-233">Suudi Arabistan</span><span class="sxs-lookup"><span data-stu-id="fcd31-233">Saudi Arabia</span></span>
    - <span data-ttu-id="fcd31-234">Birleşik Arap Emirlikleri</span><span class="sxs-lookup"><span data-stu-id="fcd31-234">United Arab Emirates</span></span>
    - <span data-ttu-id="fcd31-235">Venezuela</span><span class="sxs-lookup"><span data-stu-id="fcd31-235">Venezuela</span></span>

<span data-ttu-id="fcd31-236">Ölçütlere uyan iş ortaklarının, yeni müşterileri eklerken veya mevcut müşteri ayrıntılarını değiştirirken müşterinin **Şirket kayıt kimliği** 'ni (müşterinin **kuruluş** adı olarak da bilinir) ve **telefon numarasını** göndermesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-236">Partners who meet the criteria will have to submit a customer's **company registration ID** (also known as the customer's **organization INN**) and **phone number** when they onboard new customers or modify existing customer details.</span></span> <span data-ttu-id="fcd31-237">Ayrıca bu iş ortakları müşteri için isteğe bağlı bir **ikinci ad** da girebilir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-237">These partners can also enter an optional **middle name** for the customer.</span></span>

<span data-ttu-id="fcd31-238">Şirket kayıt KIMLIĞINIZI eklediğinizde müşterinin kişisel KIMLIĞINI değil iş vergi KIMLIĞINIZI kullanmanız gerektiğini unutmayın.</span><span class="sxs-lookup"><span data-stu-id="fcd31-238">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="fcd31-239">Aşağıdaki ülkelerde yeni veya mevcut müşteriler ile iş yapan iş ortakları, Kasım 2020 ' de daha önceki bir sürüm ile zaten eklendi.</span><span class="sxs-lookup"><span data-stu-id="fcd31-239">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="fcd31-240">Ermenistan</span><span class="sxs-lookup"><span data-stu-id="fcd31-240">Armenia</span></span>
- <span data-ttu-id="fcd31-241">Azerbaycan</span><span class="sxs-lookup"><span data-stu-id="fcd31-241">Azerbaijan</span></span>
- <span data-ttu-id="fcd31-242">Belarus</span><span class="sxs-lookup"><span data-stu-id="fcd31-242">Belarus</span></span>
- <span data-ttu-id="fcd31-243">Macaristan</span><span class="sxs-lookup"><span data-stu-id="fcd31-243">Hungary</span></span>
- <span data-ttu-id="fcd31-244">Kazakistan</span><span class="sxs-lookup"><span data-stu-id="fcd31-244">Kazakhstan</span></span>
- <span data-ttu-id="fcd31-245">Kırgızistan</span><span class="sxs-lookup"><span data-stu-id="fcd31-245">Kyrgyzstan</span></span>
- <span data-ttu-id="fcd31-246">Moldova</span><span class="sxs-lookup"><span data-stu-id="fcd31-246">Moldova</span></span>
- <span data-ttu-id="fcd31-247">Rusya</span><span class="sxs-lookup"><span data-stu-id="fcd31-247">Russia</span></span>
- <span data-ttu-id="fcd31-248">Tacikistan</span><span class="sxs-lookup"><span data-stu-id="fcd31-248">Tajikistan</span></span>
- <span data-ttu-id="fcd31-249">Ukrayna</span><span class="sxs-lookup"><span data-stu-id="fcd31-249">Ukraine</span></span>
- <span data-ttu-id="fcd31-250">Özbekistan</span><span class="sxs-lookup"><span data-stu-id="fcd31-250">Uzbekistan</span></span>

<span data-ttu-id="fcd31-251">Dünyanın geri kalanında müşterilere sahip olan iş ortakları 25 Mart 2021 ' de, müşteriler için isteğe bağlı ayrıntılar olarak **Şirket kayıt kimliği**, **telefon numarası** ve **Orta adı** girme olanağına sahip olur.</span><span class="sxs-lookup"><span data-stu-id="fcd31-251">Partners with customers in the rest of the world will have the ability on March 25, 2021 to enter the **company registration ID**, **phone number**, and **middle name** for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="fcd31-252">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="fcd31-252">Next steps</span></span>

- <span data-ttu-id="fcd31-253">Daha ayrıntılı rehberlik için, [adanmış iş ortağı koleksiyonundaki](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) teknik belgeleri ve sık sorulan soruları gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="fcd31-253">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>

- <span data-ttu-id="fcd31-254">Iş Ortağı Merkezi API 'sini ve Web kullanıcısı deneyimini kullanarak değişiklikleri içerecek şekilde hazırlayın.</span><span class="sxs-lookup"><span data-stu-id="fcd31-254">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> <span data-ttu-id="fcd31-255">API/SDK 'lar test için kullanılabilir olacak.</span><span class="sxs-lookup"><span data-stu-id="fcd31-255">API/SDKs will be available for testing.</span></span>

- <span data-ttu-id="fcd31-256">Yeni müşterileri eklerken veya mevcut müşteri ayrıntılarını değiştirirken ek verileri gönderdiğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="fcd31-256">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>

- <span data-ttu-id="fcd31-257">Bir denetim masası satıcısı (CPV) çözümü kullanıyorsanız, CPV 'nize başvurun.</span><span class="sxs-lookup"><span data-stu-id="fcd31-257">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="fcd31-258">Sorularınız mı var?</span><span class="sxs-lookup"><span data-stu-id="fcd31-258">Questions?</span></span>

<span data-ttu-id="fcd31-259">Yasal tanımlayıcıyla (ıNN veya tın olarak da bilinir) ilgili sorularınız varsa vergi danışmanınıza veya yerel vergi ofisine başvurun.</span><span class="sxs-lookup"><span data-stu-id="fcd31-259">Contact your tax advisor or local tax office if you have any questions related to the legal identifier (also called INN or TIN).</span></span> <span data-ttu-id="fcd31-260">Microsoft, vergi konusunda önemli yönergeler sağlayamaz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-260">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="fcd31-261">Microsoft ile işlemlerinde desteğe ihtiyacınız varsa, [bir hizmet isteği açın](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="fcd31-261">If you need support in your operations with Microsoft, [open a service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a><span data-ttu-id="fcd31-262">1 Mart 2021 ' de yapılan düzeltmeler kalıcı yazılım fiyat listesi</span><span class="sxs-lookup"><span data-stu-id="fcd31-262">Corrections made to March 1, 2021 perpetual software price list</span></span>

### <a name="categories"></a><span data-ttu-id="fcd31-263">Kategoriler</span><span class="sxs-lookup"><span data-stu-id="fcd31-263">Categories</span></span>

- <span data-ttu-id="fcd31-264">Tarih: 2021-03-23</span><span class="sxs-lookup"><span data-stu-id="fcd31-264">Date: 2021-03-23</span></span>
- <span data-ttu-id="fcd31-265">Teklifler/Pazarlar</span><span class="sxs-lookup"><span data-stu-id="fcd31-265">Offers/Markets</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcd31-266">Etkilenen hedef kitle</span><span class="sxs-lookup"><span data-stu-id="fcd31-266">Impacted audience</span></span>

<span data-ttu-id="fcd31-267">Bulut çözüm sağlayıcısı programında dolaylı sağlayıcılar ve doğrudan fatura ortakları deneyimidir kalıcı yazılım</span><span class="sxs-lookup"><span data-stu-id="fcd31-267">Indirect providers and direct bill partners transacting perpetual software in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="fcd31-268">Ayrıntılar</span><span class="sxs-lookup"><span data-stu-id="fcd31-268">Details</span></span>

<span data-ttu-id="fcd31-269">1 Mart 2021 ' de gönderilen kalıcı yazılım için fiyat listesi, orada olmaması gereken pazarlara dahil değildir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-269">The price list for perpetual software posted on March 1, 2021 included markets that should not have been there.</span></span> <span data-ttu-id="fcd31-270">Kalıcı yazılım fiyat listesi, düzeltmeler ile 17 Mart 2021 ' de güncelleştirildi.</span><span class="sxs-lookup"><span data-stu-id="fcd31-270">The perpetual software price list was updated on March 17, 2021 with the corrections.</span></span> <span data-ttu-id="fcd31-271">Bu düzeltmeler yalnızca için geçerlidir:</span><span class="sxs-lookup"><span data-stu-id="fcd31-271">These corrections were only applicable to:</span></span>

- <span data-ttu-id="fcd31-272">Ürün KIMLIĞI: DF77X4D43RKT</span><span class="sxs-lookup"><span data-stu-id="fcd31-272">Product ID: DF77X4D43RKT</span></span> 
- <span data-ttu-id="fcd31-273">Ürün adı: Microsoft 365 İş için Windows 10 Home-Pro yükseltmesi</span><span class="sxs-lookup"><span data-stu-id="fcd31-273">Product name: Windows 10 Home to Pro Upgrade for Microsoft 365 Business</span></span>
- <span data-ttu-id="fcd31-274">Kaldırılan veya desteklenmeyen pazarlar: AE, AF, AL, har, AO, BA, BB, BD, BH, BM, mılyar TL, BO, BR, BS, siyah beyaz, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, çn, d, IN,, KN, KZ, LB, , Nı, NP, OM, PA, PE, PH, PK, PR, INER, QA, RS, RU, RW, SG, SN, ZF, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YS, ZM, ZW</span><span class="sxs-lookup"><span data-stu-id="fcd31-274">Removed or unsupported markets: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW</span></span>

<span data-ttu-id="fcd31-275">Bu değişiklikler yalnızca yukarıdaki ürün için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-275">These changes only apply to the above product.</span></span> <span data-ttu-id="fcd31-276">Diğer ürünlerin bir düzeltme yoktur.</span><span class="sxs-lookup"><span data-stu-id="fcd31-276">Other products had no corrections.</span></span> 

### <a name="next-steps-and-resources"></a><span data-ttu-id="fcd31-277">Sonraki adımlar ve kaynaklar</span><span class="sxs-lookup"><span data-stu-id="fcd31-277">Next steps and resources</span></span>

- <span data-ttu-id="fcd31-278">Transact kalıcı yazılım kullanan iş ortakları en son kalıcı yazılım fiyat listesini indirmelidir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-278">Partners who transact perpetual software should download the latest perpetual software price list.</span></span>
- <span data-ttu-id="fcd31-279">Ülkelerinden oluşan iki harfli kısaltmayı kolay bir şekilde eşlemek için [bölge ülke kodlarına](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) başvurun.</span><span class="sxs-lookup"><span data-stu-id="fcd31-279">Consult the [region country codes](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) for a friendly mapping of the two letter abbreviation to countries.</span></span>
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> <span data-ttu-id="fcd31-280">.NET Standard SDK sürümü (v 1.17.0)</span><span class="sxs-lookup"><span data-stu-id="fcd31-280">SDK Release on .NET Standard (v1.17.0)</span></span>

### <a name="categories"></a><span data-ttu-id="fcd31-281">Kategoriler</span><span class="sxs-lookup"><span data-stu-id="fcd31-281">Categories</span></span>

- <span data-ttu-id="fcd31-282">Tarih: 2021-03-23</span><span class="sxs-lookup"><span data-stu-id="fcd31-282">Date: 2021-03-23</span></span>

- <span data-ttu-id="fcd31-283">Özellikler</span><span class="sxs-lookup"><span data-stu-id="fcd31-283">Capabilities</span></span>
 
### <a name="impacted-audience"></a><span data-ttu-id="fcd31-284">Etkilenen hedef kitle</span><span class="sxs-lookup"><span data-stu-id="fcd31-284">Impacted audience</span></span>

<span data-ttu-id="fcd31-285">Iş ortağı merkezi .NET SDK 'sını kullanan CSP programına katılan doğrudan fatura ortakları ve dolaylı sağlayıcılar.</span><span class="sxs-lookup"><span data-stu-id="fcd31-285">Direct Bill partners and Indirect Providers participating in the CSP program who are using the Partner Center .NET SDK.</span></span>

### <a name="details"></a><span data-ttu-id="fcd31-286">Ayrıntılar</span><span class="sxs-lookup"><span data-stu-id="fcd31-286">Details</span></span>

<span data-ttu-id="fcd31-287">23 2020 Mart itibariyle Iş ortakları, [Microsoftpartnercenter. NETSDK (NuGet Galerisi |) sürümünü indirmeye başlayabilir. Microsoft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), güncelleştirilmiş ortak Iş ortağı MERKEZI SDK [GitHub örnekleri](https://github.com/Microsoft/Partner-Center-DotNet-Samples)ile birlikte.</span><span class="sxs-lookup"><span data-stu-id="fcd31-287">As of March 23 2020, Partners can start downloading the version of [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), along with updated public Partner Center SDK [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples).</span></span> <span data-ttu-id="fcd31-288">Bu sürüm aşağıdaki yöntemlerin güncelleştirmelerini içerir:</span><span class="sxs-lookup"><span data-stu-id="fcd31-288">This version includes updates to the following methods:</span></span>

#### <a name="audit-updated-new-operation-types"></a><span data-ttu-id="fcd31-289">Denetim güncelleştirildi: yeni işlem türleri</span><span class="sxs-lookup"><span data-stu-id="fcd31-289">Audit Updated: New operation types</span></span>

<span data-ttu-id="fcd31-290">Müşterinin ne zaman onayladığı ve sonlandırıldığı hakkında bilinmesi için yeni [işlem türleri](https://docs.microsoft.com/partner-center/develop/auditing-resources) eklendi.</span><span class="sxs-lookup"><span data-stu-id="fcd31-290">Added new [operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for knowing when the customer approved and terminated DAP.</span></span>

- <span data-ttu-id="fcd31-291">DapAdminRelationshipApproved</span><span class="sxs-lookup"><span data-stu-id="fcd31-291">DapAdminRelationshipApproved</span></span>

- <span data-ttu-id="fcd31-292">Dapadminrelationshipsonlandırılan</span><span class="sxs-lookup"><span data-stu-id="fcd31-292">DapAdminRelationshipTerminated</span></span>

#### <a name="audit-updated-new-resource-and-operation-types"></a><span data-ttu-id="fcd31-293">Denetim güncelleştirildi: yeni kaynak ve işlem türleri</span><span class="sxs-lookup"><span data-stu-id="fcd31-293">Audit Updated: New resource and operation types</span></span>

<span data-ttu-id="fcd31-294">Müşteri dizin rolü senaryosunu desteklemek için yeni [kaynak ve işlem türleri](https://docs.microsoft.com/partner-center/develop/auditing-resources) eklendi.</span><span class="sxs-lookup"><span data-stu-id="fcd31-294">Added new [resource and operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for supporting the customer directory role scenario.</span></span>

- <span data-ttu-id="fcd31-295">Yeni kaynak türü "CustomerDirectoryRole"</span><span class="sxs-lookup"><span data-stu-id="fcd31-295">New resource type “CustomerDirectoryRole”</span></span>

- <span data-ttu-id="fcd31-296">"AddUserMember" ve "RemoveUserMember" işlem türleri</span><span class="sxs-lookup"><span data-stu-id="fcd31-296">Operation types “AddUserMember” and “RemoveUserMember”</span></span>

#### <a name="sdk-updates-to-customer-accounts"></a><span data-ttu-id="fcd31-297">Müşteri hesaplarına SDK güncelleştirmeleri</span><span class="sxs-lookup"><span data-stu-id="fcd31-297">SDK Updates to customer accounts</span></span>

- <span data-ttu-id="fcd31-298">GET/customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus desteği</span><span class="sxs-lookup"><span data-stu-id="fcd31-298">Support for GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span></span>

- <span data-ttu-id="fcd31-299">/Customers/{Customer-Tenant-ID}/nitelikler al</span><span class="sxs-lookup"><span data-stu-id="fcd31-299">GET /customers/{customer-tenant-id}/qualifications</span></span>

- <span data-ttu-id="fcd31-300">/Customers/{customer_id}/nitelikler SONRASı? Code = {validationCode}</span><span class="sxs-lookup"><span data-stu-id="fcd31-300">POST /customers/{customer_id}/qualifications?code={validationCode}</span></span>

#### <a name="additional-changes"></a><span data-ttu-id="fcd31-301">Ek değişiklikler</span><span class="sxs-lookup"><span data-stu-id="fcd31-301">Additional changes</span></span>

<span data-ttu-id="fcd31-302">Aşağıdaki değişiklikler yeni ticaret 'nin bir parçası olarak sunulmuştur ve şu anda yalnızca M365/D365 yeni ticaret deneyimi Technical Preview 'ın parçası olan iş ortakları tarafından kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-302">The following changes are introduced as part of New Commerce, and are currently available by invitation only to partners who are part of the M365/D365 New Commerce experience technical preview.</span></span> <span data-ttu-id="fcd31-303">Yeni ticaret Technical Preview kapsamında olmayan iş ortakları, etkileri fark etmez ve geriye dönük olarak uyumlu olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="fcd31-303">Partners who are not part of the New Commerce technical preview should not notice impacts and should be backward compatible.</span></span>

- <span data-ttu-id="fcd31-304">Katalog değişiklikleri:</span><span class="sxs-lookup"><span data-stu-id="fcd31-304">Catalog Changes:</span></span>

  - <span data-ttu-id="fcd31-305">/Products/{product-id}/SKUs/{SKU-id} al</span><span class="sxs-lookup"><span data-stu-id="fcd31-305">GET /products/{product-id}/skus/{sku-id}</span></span>

- <span data-ttu-id="fcd31-306">Satın alın ve yönetin:</span><span class="sxs-lookup"><span data-stu-id="fcd31-306">Purchase and Manage:</span></span>
  - <span data-ttu-id="fcd31-307">/Customers/{CustomerID}/abonelikleri al</span><span class="sxs-lookup"><span data-stu-id="fcd31-307">GET /customers/{customerId}/subscriptions</span></span>
  - <span data-ttu-id="fcd31-308">/Customers/{CustomerID}/Subscriptions/{SubscriptionID} al</span><span class="sxs-lookup"><span data-stu-id="fcd31-308">GET /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="fcd31-309">PATCH/Customers/{CustomerID}/Subscriptions/{SubscriptionID}</span><span class="sxs-lookup"><span data-stu-id="fcd31-309">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="fcd31-310">/Customers/{CustomerID}/Subscriptions/{SubscriptionID}/geçişli tioneligılıklara al</span><span class="sxs-lookup"><span data-stu-id="fcd31-310">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span></span>
  - <span data-ttu-id="fcd31-311">/Customers/{CustomerID}/Subscriptions/{SubscriptionID}/geçişlerini al</span><span class="sxs-lookup"><span data-stu-id="fcd31-311">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>
  - <span data-ttu-id="fcd31-312">POST/Customers/{CustomerID}/Subscriptions/{SubscriptionID}/geçişlerin</span><span class="sxs-lookup"><span data-stu-id="fcd31-312">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>

### <a name="next-steps"></a><span data-ttu-id="fcd31-313">Sonraki Adımlar</span><span class="sxs-lookup"><span data-stu-id="fcd31-313">Next Steps</span></span>

- <span data-ttu-id="fcd31-314">En son [Microsoftpartnercenter. NETSDK sürümünü indirin (NuGet Galerisi | Microsoft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span><span class="sxs-lookup"><span data-stu-id="fcd31-314">Download the latest version [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span></span>
- <span data-ttu-id="fcd31-315">[GitHub örneklerini](https://github.com/Microsoft/Partner-Center-DotNet-Samples) indirme ve gözden geçirme</span><span class="sxs-lookup"><span data-stu-id="fcd31-315">Download and review the [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span></span>

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a><span data-ttu-id="fcd31-316">Uygun teklifler için CSP ticari Market teklifi ve FY21 CSP teşvikleri</span><span class="sxs-lookup"><span data-stu-id="fcd31-316">CSP commercial marketplace offer and FY21 CSP incentives for eligible offers</span></span>

### <a name="categories"></a><span data-ttu-id="fcd31-317">Kategoriler</span><span class="sxs-lookup"><span data-stu-id="fcd31-317">Categories</span></span>

- <span data-ttu-id="fcd31-318">Tarih: 2021-03-18</span><span class="sxs-lookup"><span data-stu-id="fcd31-318">Date: 2021-03-18</span></span>
- <span data-ttu-id="fcd31-319">Özellikler</span><span class="sxs-lookup"><span data-stu-id="fcd31-319">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcd31-320">Etkilenen hedef kitle</span><span class="sxs-lookup"><span data-stu-id="fcd31-320">Impacted audience</span></span>

<span data-ttu-id="fcd31-321">Bulut çözüm sağlayıcısı programındaki dolaylı sağlayıcılar ve doğrudan fatura ortakları</span><span class="sxs-lookup"><span data-stu-id="fcd31-321">Indirect providers and direct bill partners in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="fcd31-322">Ayrıntılar</span><span class="sxs-lookup"><span data-stu-id="fcd31-322">Details</span></span>

<span data-ttu-id="fcd31-323">Bulut çözümü sağlayıcısı programındaki dolaylı sağlayıcılar ve doğrudan fatura ortakları, üçüncü taraf teklifler satmanıza ve Iş ortağı merkezi veya Azure portal işlenen her bir uygun üçüncü taraf teklifi için bir indirim teşvik elde edebilir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-323">Indirect providers and direct bill partners in the Cloud Solution Provider program can sell third party offers and earn a rebate incentive for each eligible third-party offer transacted in Partner Center or the Azure portal.</span></span> <span data-ttu-id="fcd31-324">Bu öneriler, uygun tekliflerle ilgili olarak faturalandırılan satış hakkında indirim biçiminde olacaktır ve **30 haziran 2021 ' ye kadar kullanılabilir**.</span><span class="sxs-lookup"><span data-stu-id="fcd31-324">The incentive will be in the form of a rebate on billed sales for the eligible offers and is **available until June 30, 2021**.</span></span>  

<span data-ttu-id="fcd31-325">Aşağıdaki CSP ticari marketi teklifi hakkında bilgi edinmeye devam edin ve müşterilerin devam ettirme başarısını ve dijital dönüşümünü etkinleştirmeye yönelik doğru teklifleri belirlemek için müşterilerinizle iletişim kurun.</span><span class="sxs-lookup"><span data-stu-id="fcd31-325">Continue learning about this CSP Commercial Marketplace Offer incentive below and contact your customers today to identify the right offers to enable their continued success and digital transformation.</span></span>

<span data-ttu-id="fcd31-326">En son IaaS ve SaaS çözümlerini Microsoft müşterilerine pazarlamak için bağımsız yazılım satıcıları (ISV 'Ler) ile iş ortaklıyoruz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-326">We partner with Independent Software Vendors (ISVs) to bring the latest IaaS and SaaS solutions to market for Microsoft customers.</span></span> <span data-ttu-id="fcd31-327">ISV yayımcıları, Microsoft iş ortağı kanalı aracılığıyla tekliflerinden satışları etkinleştirme seçeneğine sahiptir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-327">ISV publishers have the option of enabling sales of their offers through the Microsoft partner channel.</span></span> <span data-ttu-id="fcd31-328">Özendiğimiz tekliflerimiz iki kategoride yer almalıdır:</span><span class="sxs-lookup"><span data-stu-id="fcd31-328">Our incentive-eligible offers fall into two categories:</span></span>

- <span data-ttu-id="fcd31-329">Azure IP ortak satış incentivized durumu ile SaaS ve IaaS üçüncü taraf tekliflerini seçin.</span><span class="sxs-lookup"><span data-stu-id="fcd31-329">Select SaaS and IaaS third-party offers with Azure IP co-sell incentivized status.</span></span> 

- <span data-ttu-id="fcd31-330">Ekipler ile tümleştirilmiş SaaS uygulamaları veya PowerPoint, Word, Excel, Outlook veya SharePoint gibi en az iki Microsoft 365 üretkenlik uygulaması.</span><span class="sxs-lookup"><span data-stu-id="fcd31-330">SaaS applications integrated with Teams or at least two Microsoft 365 productivity apps, such as PowerPoint, Word, Excel, Outlook, or SharePoint.</span></span>

### <a name="next-steps-and-resources"></a><span data-ttu-id="fcd31-331">Sonraki adımlar ve kaynaklar</span><span class="sxs-lookup"><span data-stu-id="fcd31-331">Next steps and resources</span></span>

- <span data-ttu-id="fcd31-332">Uygun Market uygulamaları satmaya uygun olan uygulamaları teşvik etmek için [Iş ortağı teşvikleri](https://partner.microsoft.com/membership/partner-incentives) hakkında bilgi edinin.</span><span class="sxs-lookup"><span data-stu-id="fcd31-332">Learn about earning [Partner Incentives](https://partner.microsoft.com/membership/partner-incentives) for selling eligible marketplace apps the incentive eligible apps.</span></span> <span data-ttu-id="fcd31-333">Yeni teklifler aylık olarak eklenir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-333">New offers are added monthly.</span></span>  
- [<span data-ttu-id="fcd31-334">Bulut çözümü sağlayıcısı doğrudan fatura ortağı özendirme kaynakları</span><span class="sxs-lookup"><span data-stu-id="fcd31-334">Cloud Solution Provider direct bill partner incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [<span data-ttu-id="fcd31-335">Bulut çözümü sağlayıcısı dolaylı sağlayıcı, kaynakları teşvik edin</span><span class="sxs-lookup"><span data-stu-id="fcd31-335">Cloud Solution Provider indirect provider incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- <span data-ttu-id="fcd31-336">Ticari market uygulamalarını satma hakkında daha fazla bilgi edinmek için bu [sunuyu](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="fcd31-336">Review this [presentation](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) to learn more about selling the commercial marketplace apps.</span></span> <span data-ttu-id="fcd31-337">Ek kaynaklara [buradan](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/)göz atın.</span><span class="sxs-lookup"><span data-stu-id="fcd31-337">Check out additional resources [here](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span></span> 
- <span data-ttu-id="fcd31-338">[Iş Ortağı Merkezi](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) veya [Azure Portal](https://ms.portal.azure.com/#home) ticari Market kataloğunu keşfet</span><span class="sxs-lookup"><span data-stu-id="fcd31-338">Explore the commercial marketplace catalog in [Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) or [Azure portal](https://ms.portal.azure.com/#home)</span></span>
- <span data-ttu-id="fcd31-339">Uygulamaları şirketinizin marketi ile bütünleştirmek için [API 'leri](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) kullanma</span><span class="sxs-lookup"><span data-stu-id="fcd31-339">Use [APIs](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) to integrate apps into your company’s marketplace</span></span>
- <span data-ttu-id="fcd31-340">İş yaparken ilgilendiğiniz ISV 'lere ulaşın</span><span class="sxs-lookup"><span data-stu-id="fcd31-340">Reach out to ISVs you are interested in doing business with</span></span>
- <span data-ttu-id="fcd31-341">Dolaylı sağlayıcıların, hangi uygulamaların satmaya yönelik API 'Leri ve kılavuz satıcılarını kullanarak tümleştirmeleri gerekir</span><span class="sxs-lookup"><span data-stu-id="fcd31-341">Indirect providers need to integrate using APIs and guide resellers on which apps to sell</span></span>

### <a name="questions"></a><span data-ttu-id="fcd31-342">Sorularınız mı var?</span><span class="sxs-lookup"><span data-stu-id="fcd31-342">Questions?</span></span>  

<span data-ttu-id="fcd31-343">Iş Ortağı Merkezi 'nde ticari Market 'e genel bakış için [Bu makaleye](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) başvurun.</span><span class="sxs-lookup"><span data-stu-id="fcd31-343">Refer to [this article](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) for an overview of the commercial marketplace in Partner Center.</span></span>

<span data-ttu-id="fcd31-344">Daha fazla yardıma ihtiyacınız varsa, Iş Ortağı Merkezi 'nde bir destek isteği oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-344">If you need additional assistance you can create a support request in Partner Center.</span></span> <span data-ttu-id="fcd31-345">Daha fazla bilgi edinin [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .</span><span class="sxs-lookup"><span data-stu-id="fcd31-345">Learn more at [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).</span></span>

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a><span data-ttu-id="fcd31-346">Power BI Premium teklif adlandırma ve önkoşul güncelleştirme</span><span class="sxs-lookup"><span data-stu-id="fcd31-346">Power BI Premium offer naming and prerequisite update</span></span>

### <a name="categories"></a><span data-ttu-id="fcd31-347">Kategoriler</span><span class="sxs-lookup"><span data-stu-id="fcd31-347">Categories</span></span>

- <span data-ttu-id="fcd31-348">Tarih: 2021-03-18</span><span class="sxs-lookup"><span data-stu-id="fcd31-348">Date: 2021-03-18</span></span>
- <span data-ttu-id="fcd31-349">Özellikler</span><span class="sxs-lookup"><span data-stu-id="fcd31-349">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="fcd31-350">Özet</span><span class="sxs-lookup"><span data-stu-id="fcd31-350">Summary</span></span>

<span data-ttu-id="fcd31-351">1 Nisan 2021 son fiyat listesi, Kullanıcı başına Power BI Premium için adlandırma ve/veya önkoşul bilgilerine açıklık eklemek üzere güncelleştirilir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-351">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcd31-352">Etkilenen hedef kitle</span><span class="sxs-lookup"><span data-stu-id="fcd31-352">Impacted audience</span></span>

<span data-ttu-id="fcd31-353">Bulut çözümü sağlayıcısı (CSP) doğrudan ve dolaylı iş ortakları</span><span class="sxs-lookup"><span data-stu-id="fcd31-353">Cloud Solution Provider (CSP) direct and indirect partners</span></span>

### <a name="details"></a><span data-ttu-id="fcd31-354">Ayrıntılar</span><span class="sxs-lookup"><span data-stu-id="fcd31-354">Details</span></span>

<span data-ttu-id="fcd31-355">1 Nisan 2021 son fiyat listesi, Kullanıcı başına Power BI Premium için adlandırma ve/veya önkoşul bilgilerine açıklık eklemek üzere güncelleştirilir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-355">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

<span data-ttu-id="fcd31-356">Son fiyat listesi güncelleştirilene kadar, bu bölümdeki bilgileri kullanarak doğru ürünün düzenli olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="fcd31-356">Until the final price list is updated, use the information in this section to ensure that the correct product is ordered.</span></span>

<span data-ttu-id="fcd31-357">Aşağıdaki ayrıntılar etkilenen SKU ve önkoşul ayrıntılarını göstermektedir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-357">The following details show the affected SKU and prerequisite details.</span></span>

| <span data-ttu-id="fcd31-358">1 Mart 'ta bir görünen ad teklif listesi önizlemesi</span><span class="sxs-lookup"><span data-stu-id="fcd31-358">Offer display name on March 1 price list preview</span></span> |  <span data-ttu-id="fcd31-359">1 Nisan 'ın son fiyat listesindeki teklif görünen adı güncelleştirildi</span><span class="sxs-lookup"><span data-stu-id="fcd31-359">Updated offer display name on April 1 final price list</span></span>| <span data-ttu-id="fcd31-360">Teklif Kimliği</span><span class="sxs-lookup"><span data-stu-id="fcd31-360">Offer ID</span></span> |
| ------ | ----------- | ----------- |
| <span data-ttu-id="fcd31-361">Kullanıcı başına Power BI Premium Add-On (kar amacı gütmeyen personel fiyatlandırması)</span><span class="sxs-lookup"><span data-stu-id="fcd31-361">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="fcd31-362">Kullanıcı başına Power BI Premium Add-On **(Office)** (kar amacı gütmeyen personel fiyatlandırması)</span><span class="sxs-lookup"><span data-stu-id="fcd31-362">Power BI Premium Per User Add-On **(Office)** (Nonprofit Staff Pricing)</span></span>   | <span data-ttu-id="fcd31-363">31c03289-47AB-4AB0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="fcd31-363">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span>   |

<span data-ttu-id="fcd31-364">Müşterilerin bu teklifi satın almak için aşağıdaki önkoşulların herhangi birine sahip olması gerekir:</span><span class="sxs-lookup"><span data-stu-id="fcd31-364">Customers are required to have any one of the following prerequisites to purchase this offer:</span></span>

| <span data-ttu-id="fcd31-365">Teklif görünen adı</span><span class="sxs-lookup"><span data-stu-id="fcd31-365">Offer display name</span></span> | <span data-ttu-id="fcd31-366">Teklif Kimliği</span><span class="sxs-lookup"><span data-stu-id="fcd31-366">Offer ID</span></span> |
| ------ | ----------- |
| <span data-ttu-id="fcd31-367">Microsoft 365 E5 (kar amacı gütmeyen personel fiyatlandırması)</span><span class="sxs-lookup"><span data-stu-id="fcd31-367">Microsoft 365 E5 (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="fcd31-368">31bedf01-9e57-4ece-a53a-d3656a563931</span><span class="sxs-lookup"><span data-stu-id="fcd31-368">31bedf01-9e57-4ece-a53a-d3656a563931</span></span>   |
|   <span data-ttu-id="fcd31-369">Ses konferansı olmadan E5 Microsoft 365 (kar amacı gütmeyen personel fiyatlandırması)</span><span class="sxs-lookup"><span data-stu-id="fcd31-369">Microsoft 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="fcd31-370">b456810a-c414-4e07-98fc-ef74e8175a09</span><span class="sxs-lookup"><span data-stu-id="fcd31-370">b456810a-c414-4e07-98fc-ef74e8175a09</span></span>|
|   <span data-ttu-id="fcd31-371">Office 365 E5 (kar amacı gütmeyen personel fiyatlandırması)</span><span class="sxs-lookup"><span data-stu-id="fcd31-371">Office 365 E5 (Nonprofit Staff Pricing)</span></span>| <span data-ttu-id="fcd31-372">ce139fe5-8bd5-47ED-a5be-07c286f8b9e</span><span class="sxs-lookup"><span data-stu-id="fcd31-372">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span></span>    |
|   <span data-ttu-id="fcd31-373">Office 365 E5 (kar amacı gütmeyen personel fiyatlandırma) denemesi</span><span class="sxs-lookup"><span data-stu-id="fcd31-373">Office 365 E5 (Nonprofit Staff Pricing) Trial</span></span>|  <span data-ttu-id="fcd31-374">2f192efe-608a-4C9C-9d19-2b0b70b0962e</span><span class="sxs-lookup"><span data-stu-id="fcd31-374">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span></span>|
|   <span data-ttu-id="fcd31-375">Office 365 E5 ses konferansı olmadan (kar amacı gütmeyen personel fiyatlandırması)</span><span class="sxs-lookup"><span data-stu-id="fcd31-375">Office 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="fcd31-376">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span><span class="sxs-lookup"><span data-stu-id="fcd31-376">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span></span>|

<span data-ttu-id="fcd31-377">Aşağıdaki Power BI Premium teklifi satın alma için gereken bir önkoşula sahiptir:</span><span class="sxs-lookup"><span data-stu-id="fcd31-377">The following Power BI Premium offer has a prerequisite required for purchase:</span></span>

| <span data-ttu-id="fcd31-378">Teklif görünen adı</span><span class="sxs-lookup"><span data-stu-id="fcd31-378">Offer display name</span></span> | <span data-ttu-id="fcd31-379">Teklif Kimliği</span><span class="sxs-lookup"><span data-stu-id="fcd31-379">Offer ID</span></span> |
| ------ | ----------- |
|   <span data-ttu-id="fcd31-380">Kullanıcı başına Power BI Premium Add-On (kar amacı gütmeyen personel fiyatlandırması)</span><span class="sxs-lookup"><span data-stu-id="fcd31-380">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="fcd31-381">ef0b895b-681b-4026-a5b1-dda182a57d40</span><span class="sxs-lookup"><span data-stu-id="fcd31-381">ef0b895b-681b-4026-a5b1-dda182a57d40</span></span> |

<span data-ttu-id="fcd31-382">Müşterilerin bu teklifi satın alması için bu önkoşulu olması gerekir:</span><span class="sxs-lookup"><span data-stu-id="fcd31-382">Customers are required to have this prerequisite to purchase this offer:</span></span>

| <span data-ttu-id="fcd31-383">Teklif görünen adı</span><span class="sxs-lookup"><span data-stu-id="fcd31-383">Offer display name</span></span> | <span data-ttu-id="fcd31-384">Teklif Kimliği</span><span class="sxs-lookup"><span data-stu-id="fcd31-384">Offer ID</span></span> |
| ------ |----------|
| <span data-ttu-id="fcd31-385">Power BI Pro (kar amacı gütmeyen personel fiyatlandırması)</span><span class="sxs-lookup"><span data-stu-id="fcd31-385">Power BI Pro (Nonprofit Staff Pricing)</span></span>  |   <span data-ttu-id="fcd31-386">cabdfc93-5786-4224-bfd3-35d58f833b35</span><span class="sxs-lookup"><span data-stu-id="fcd31-386">cabdfc93-5786-4224-bfd3-35d58f833b35</span></span> |

### <a name="next-steps"></a><span data-ttu-id="fcd31-387">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="fcd31-387">Next steps</span></span>

<span data-ttu-id="fcd31-388">Bu konuyla ilgili kaynakları gözden geçirin ve bu bilgileri kuruluşunuzdaki uygun hissedarlarla paylaşabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-388">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="fcd31-389">Sorularınız mı var?</span><span class="sxs-lookup"><span data-stu-id="fcd31-389">Questions?</span></span>

<span data-ttu-id="fcd31-390">Bu tekliflerle ilgili herhangi bir soru için ilgili Yammer topluluklarınızı kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="fcd31-390">For any questions about these offers, check your relevant Yammer communities.</span></span> 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> <span data-ttu-id="fcd31-391">Microsoft 365 F3 için Mart fiyat güncelleştirmeleri</span><span class="sxs-lookup"><span data-stu-id="fcd31-391">March price updates for Microsoft 365 F3</span></span>

### <a name="categories"></a><span data-ttu-id="fcd31-392">Kategoriler</span><span class="sxs-lookup"><span data-stu-id="fcd31-392">Categories</span></span>

- <span data-ttu-id="fcd31-393">Tarih: 2021-03-16</span><span class="sxs-lookup"><span data-stu-id="fcd31-393">Date: 2021-03-16</span></span>
- <span data-ttu-id="fcd31-394">Teklifler/Pazarlar</span><span class="sxs-lookup"><span data-stu-id="fcd31-394">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="fcd31-395">Özet</span><span class="sxs-lookup"><span data-stu-id="fcd31-395">Summary</span></span>

<span data-ttu-id="fcd31-396">Microsoft 365 F3 Ingiliz Sterlini (GBP) ve Euro (EUR) için yanlış Mart 2021 fiyatlandırması düzeltildi.</span><span class="sxs-lookup"><span data-stu-id="fcd31-396">Incorrect March 2021 pricing has been corrected for Microsoft 365 F3 British Pound (GBP) and Euro (EUR).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcd31-397">Etkilenen hedef kitle</span><span class="sxs-lookup"><span data-stu-id="fcd31-397">Impacted audience</span></span>

<span data-ttu-id="fcd31-398">İş ortakları, 1 Mart 'ta Microsoft 365 F3 veya bulut çözümü sağlayıcısı (CSP) programı aracılığıyla 1 Mart 2021 arasında bir EUR Satın alma.</span><span class="sxs-lookup"><span data-stu-id="fcd31-398">Partners purchasing Microsoft 365 F3 in GBP or EUR between March 1 and March 17, 2021 through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="fcd31-399">Ayrıntılar</span><span class="sxs-lookup"><span data-stu-id="fcd31-399">Details</span></span>

<span data-ttu-id="fcd31-400">Microsoft, Microsoft 365 F3 için yanlış fiyatlandırmayı çözümledi.</span><span class="sxs-lookup"><span data-stu-id="fcd31-400">Microsoft has resolved incorrect pricing for Microsoft 365 F3.</span></span> <span data-ttu-id="fcd31-401">Yanlış fiyatlar GBP ve EUR için ve yalnızca 1 Mart, 17 Mart 2021 arasında satın alınan tekliflere yöneliktir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-401">The incorrect prices were for GBP and EUR and only for offers purchased between March 1 and March 17, 2021.</span></span> <span data-ttu-id="fcd31-402">Etkilenen teklifler ve para birimleri aşağıda listelenmiştir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-402">The impacted offers and currencies are listed below.</span></span> 

| <span data-ttu-id="fcd31-403">Teklif adı</span><span class="sxs-lookup"><span data-stu-id="fcd31-403">Offer name</span></span> | <span data-ttu-id="fcd31-404">Para Birimi</span><span class="sxs-lookup"><span data-stu-id="fcd31-404">Currency</span></span> | <span data-ttu-id="fcd31-405">Teklif Kimliği</span><span class="sxs-lookup"><span data-stu-id="fcd31-405">Offer ID</span></span> | <span data-ttu-id="fcd31-406">Malzeme KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="fcd31-406">Material ID</span></span> |
| ------ |----------- |----------- |----------- |
| <span data-ttu-id="fcd31-407">Microsoft 365 F3 (Hayır)</span><span class="sxs-lookup"><span data-stu-id="fcd31-407">Microsoft 365 F3 (Charity)</span></span> | <span data-ttu-id="fcd31-408">GBP</span><span class="sxs-lookup"><span data-stu-id="fcd31-408">GBP</span></span> | <span data-ttu-id="fcd31-409">57b722c2-c435-4bfb-9bc8-80509213a13a</span><span class="sxs-lookup"><span data-stu-id="fcd31-409">57b722c2-c435-4bfb-9bc8-80509213a13a</span></span> | <span data-ttu-id="fcd31-410">AAD-11626</span><span class="sxs-lookup"><span data-stu-id="fcd31-410">AAD-11626</span></span> |
| <span data-ttu-id="fcd31-411">Microsoft 365 F3 (ticari)</span><span class="sxs-lookup"><span data-stu-id="fcd31-411">Microsoft 365 F3 (Commercial)</span></span> | <span data-ttu-id="fcd31-412">EUR</span><span class="sxs-lookup"><span data-stu-id="fcd31-412">EUR</span></span>| <span data-ttu-id="fcd31-413">3451a3b0-8cdav-44a7-bad7-c30be81c4aaa</span><span class="sxs-lookup"><span data-stu-id="fcd31-413">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span></span> | <span data-ttu-id="fcd31-414">AAA-89898</span><span class="sxs-lookup"><span data-stu-id="fcd31-414">AAA-89898</span></span> |
 
<span data-ttu-id="fcd31-415">Mart ve Nisan Preview lisansı-temel fiyat listeleri, 16 Mart 5PM Pasifik standart saati ile güncelleştirildi.</span><span class="sxs-lookup"><span data-stu-id="fcd31-415">The March and April preview license-base price lists were updated March 16, 5PM pacific standard time.</span></span>

### <a name="next-steps"></a><span data-ttu-id="fcd31-416">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="fcd31-416">Next steps</span></span>

- <span data-ttu-id="fcd31-417">İş ortakları, her ikisi de Mart ve Nisan önizlemesi olmak üzere geçerli lisans tabanlı fiyat listelerini, varsa bu fiyat düzeltmelerini yeniden indirmelidir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-417">Partners should redownload the current license-based price lists, both March and the April preview, with these price corrections if applicable.</span></span>  
- <span data-ttu-id="fcd31-418">Microsoft, etkilenen işlemleri düzeltme ile ilgili sonraki adımlar hakkında bilgi almak için, önümüzdeki haftalarda, gelecek haftalarda bulunan iş ortakları ile iletişim kuracaktır.</span><span class="sxs-lookup"><span data-stu-id="fcd31-418">Microsoft will be contacting impacted partners in the coming weeks via email to inform them of next steps related to correcting affected transactions.</span></span>

### <a name="questions"></a><span data-ttu-id="fcd31-419">Sorularınız mı var?</span><span class="sxs-lookup"><span data-stu-id="fcd31-419">Questions?</span></span>

<span data-ttu-id="fcd31-420">Diğer sorular için lütfen ilgili CSP Yammer topluluklarınızı denetleyin.</span><span class="sxs-lookup"><span data-stu-id="fcd31-420">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> <span data-ttu-id="fcd31-421">Iş Ortağı Merkezi aracılığıyla yasal şirket adını güncelleştirme</span><span class="sxs-lookup"><span data-stu-id="fcd31-421">Update a legal company name through Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="fcd31-422">Kategoriler</span><span class="sxs-lookup"><span data-stu-id="fcd31-422">Categories</span></span>

- <span data-ttu-id="fcd31-423">Tarih: 2021-03-16</span><span class="sxs-lookup"><span data-stu-id="fcd31-423">Date: 2021-03-16</span></span>
- <span data-ttu-id="fcd31-424">Sürücü verimliliği & ölçeği</span><span class="sxs-lookup"><span data-stu-id="fcd31-424">Drive Efficiency & Scale</span></span>

### <a name="summary"></a><span data-ttu-id="fcd31-425">Özet</span><span class="sxs-lookup"><span data-stu-id="fcd31-425">Summary</span></span>

<span data-ttu-id="fcd31-426">2021 Mart 'tan başlayarak, Microsoft İş Ortağı Ağı (MPN) iş ortakları ve bulut çözümü sağlayıcısı (CSP) dolaylı satıcıları, Iş Ortağı Merkezi aracılığıyla yasal şirket adlarını güncelleştirebilir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-426">Starting March 2021, Microsoft Partner Network (MPN) partners and Cloud Solution Provider (CSP) indirect resellers can update their legal company name through Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcd31-427">Etkilenen hedef kitle</span><span class="sxs-lookup"><span data-stu-id="fcd31-427">Impacted audience</span></span>

<span data-ttu-id="fcd31-428">MPN iş ortakları ve CSP dolaylı satıcıları (CSP doğrudan fatura ortakları için geçerli değildir)</span><span class="sxs-lookup"><span data-stu-id="fcd31-428">MPN partners and CSP indirect resellers (not applicable to CSP direct bill partners)</span></span>

### <a name="details"></a><span data-ttu-id="fcd31-429">Ayrıntılar</span><span class="sxs-lookup"><span data-stu-id="fcd31-429">Details</span></span>

<span data-ttu-id="fcd31-430">2021 Mart 'tan itibaren, MPN iş ortakları ve CSP dolaylı satıcıları, Iş Ortağı Merkezi aracılığıyla uyumlu ve kendi kendine bir şekilde yasal şirket adını güncelleştirebilir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-430">Starting March 2021, MPN partners and CSP indirect resellers can update their legal company name through Partner Center in a compliant, self-serve manner.</span></span> <span data-ttu-id="fcd31-431">Bu yeni özellik sayesinde, iş ortaklarının şirket adlarını güncelleştirmek için Iş ortağı merkezi destek bileti göndermesi artık gerekmez.</span><span class="sxs-lookup"><span data-stu-id="fcd31-431">With this new feature, partners will no longer need to submit a Partner Center support ticket to update their company name.</span></span> <span data-ttu-id="fcd31-432">Bu işlem, bu etkinlikleri gerçekleştirirken iş ortakları için önemli miktarda zaman kazandırır.</span><span class="sxs-lookup"><span data-stu-id="fcd31-432">This will save a significant amount of time for partners when performing these activities.</span></span> 

<span data-ttu-id="fcd31-433">Daha fazla bilgi için bkz. [yasal iş profilinizi güncelleştirme](../update-your-partner-profile.md#update-your-legal-business-profile).</span><span class="sxs-lookup"><span data-stu-id="fcd31-433">To learn more, see [Update your legal business profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

>[!NOTE]
><span data-ttu-id="fcd31-434">Yasal iş profilinizde bulunan şirket adının yazım hatası ve kısaltmalarının olmadığından ve resmi şirket iş kaydı kayıtlarınızda tam olarak eşleştiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="fcd31-434">Ensure that the company name in your legal business profile is free of spelling errors and abbreviations, and exactly matches your formal company business registration records.</span></span> <span data-ttu-id="fcd31-435">Kuruluş profilinizi güncelleştirme hakkında daha fazla bilgi için bkz. [kuruluş profilinizi doğrulama](../update-your-partner-profile.md#update-your-legal-business-profile).</span><span class="sxs-lookup"><span data-stu-id="fcd31-435">For more information on updating your organization profile, refer to [Verify your organization profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

### <a name="next-steps"></a><span data-ttu-id="fcd31-436">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="fcd31-436">Next steps</span></span>

<span data-ttu-id="fcd31-437">Uygun ekibin süreçlerini gözden geçirebilmesi ve güncelleştirebilmesi için bu bilgileri kuruluşunuz dahilinde paylaşabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-437">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="fcd31-438">Sorularınız mı var?</span><span class="sxs-lookup"><span data-stu-id="fcd31-438">Questions?</span></span>

<span data-ttu-id="fcd31-439">Diğer sorular için lütfen ilgili CSP Yammer topluluklarınızı denetleyin.</span><span class="sxs-lookup"><span data-stu-id="fcd31-439">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> <span data-ttu-id="fcd31-440">Bulut çözümü sağlayıcısı (CSP) program evrimi ve açık lisans programı değişikliklerinde Güncelleştir</span><span class="sxs-lookup"><span data-stu-id="fcd31-440">Update to Cloud Solution Provider (CSP) program evolution and Open License program changes</span></span>

### <a name="categories"></a><span data-ttu-id="fcd31-441">Kategoriler</span><span class="sxs-lookup"><span data-stu-id="fcd31-441">Categories</span></span>

- <span data-ttu-id="fcd31-442">Tarih: 2021-03-15</span><span class="sxs-lookup"><span data-stu-id="fcd31-442">Date: 2021-03-15</span></span>
- <span data-ttu-id="fcd31-443">Özellikler</span><span class="sxs-lookup"><span data-stu-id="fcd31-443">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="fcd31-444">Özet</span><span class="sxs-lookup"><span data-stu-id="fcd31-444">Summary</span></span>

<span data-ttu-id="fcd31-445">Yeni ticari ve kamu sektörü kalıcı yazılım teklifleri, açık lisanslama programındaki değişikliklerle birlikte bulut çözümü sağlayıcısı (CSP) programına geliyor.</span><span class="sxs-lookup"><span data-stu-id="fcd31-445">New commercial and public sector perpetual software offers are coming to the Cloud Solution Provider (CSP) program along with changes to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcd31-446">Etkilenen hedef kitle</span><span class="sxs-lookup"><span data-stu-id="fcd31-446">Impacted audience</span></span>

<span data-ttu-id="fcd31-447">Açık lisans programı ile satılan ticari dağıtımcılar ve yönetilen satıcılar ve tüm CSP iş ortakları deneyimidir kalıcı yazılım</span><span class="sxs-lookup"><span data-stu-id="fcd31-447">Commercial distributors and managed resellers selling through the Open License program, as well as all CSP partners transacting perpetual software</span></span>

### <a name="details"></a><span data-ttu-id="fcd31-448">Ayrıntılar</span><span class="sxs-lookup"><span data-stu-id="fcd31-448">Details</span></span>

<span data-ttu-id="fcd31-449">Microsoft, Eylül 2020 ' de, iş ortakları için şirket içi yazılımın kullanılabilirliği de dahil olmak üzere, CSP programındaki iş ortaklarına yönelik fırsatları genişletmek için dijital dönüşümde yolculukta bir dizi adım [duyurmuştur](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) .</span><span class="sxs-lookup"><span data-stu-id="fcd31-449">In September 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) a series of steps in our digital transformation journey to expand opportunities to partners in the CSP program, including the availability of on-premises software for partners.</span></span> <span data-ttu-id="fcd31-450">Bu değişiklikler, iş ortaklarının, CSP 'deki yazılım lisanslarını kullanarak işlerini büyütmesine ve bunların erişimini genişletmesine imkan tanır.</span><span class="sxs-lookup"><span data-stu-id="fcd31-450">These changes enable partners to grow their business and extend their reach by leveraging software licenses in CSP, positioning them for success in today’s cloud-first world.</span></span> <span data-ttu-id="fcd31-451">Ayrıca, müşterilerin buluta geçişini güçlendirin ve iş ortaklarına müşteri hibrit bulut ortamları için gereken esnekliği sunar.</span><span class="sxs-lookup"><span data-stu-id="fcd31-451">They also empower customers’ transitions to the cloud and give partners the flexibility needed for customer hybrid cloud environments.</span></span>

<span data-ttu-id="fcd31-452">Bu dijital dönüşüme devam eden aşağıdaki değişiklikleri duyuruyoruz:</span><span class="sxs-lookup"><span data-stu-id="fcd31-452">In continuation of this digital transformation, we are announcing the following changes:</span></span>

- <span data-ttu-id="fcd31-453">1 Temmuz 2021: açık lisans programı fiyat listesine yeni SKU 'Lar, ürünler veya promosyonlar eklenmeyecektir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-453">July 1, 2021:  No new SKUs, products, or promotions will be added to the Open License program price list.</span></span>

- <span data-ttu-id="fcd31-454">7 Temmuz 2021: Iki ticari teklif, orijinal Windows ve Visual Studio Professional edinme ve kamu sektörü teklifleri (kamu, eğitim ve kar amacı: [duyuru](./2020-december.md#9)), CSP kalıcı yazılım fiyat listesine eklenecektir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-454">July 7, 2021:  Two commercial offers, Get Genuine Windows and Visual Studio Professional, and public sector offers (government, education and nonprofit – see [announcement](./2020-december.md#9)) will be added to the CSP perpetual software price list.</span></span>  <span data-ttu-id="fcd31-455">Fiyat listesi, Iş Ortağı Merkezi 'nde [satış > fiyatlandırma & teklifleri](https://partnercenter.microsoft.com/pcv/sales) sayfasının yazılımlar bölümünde bulunabilir ve bu tarihte yeniden yayımlanmak üzere olur.</span><span class="sxs-lookup"><span data-stu-id="fcd31-455">The price list can be found in the Software section of the [Sell > Pricing & Offers](https://partnercenter.microsoft.com/pcv/sales) page in Partner Center and will be republished on this date.</span></span>

<span data-ttu-id="fcd31-456">CSP program evrimi ve açık lisans programı değişiklikleriyle ilgili tüm ayrıntılar için lütfen aşağıdaki **sonraki adımlara** bakın.</span><span class="sxs-lookup"><span data-stu-id="fcd31-456">For full details regarding the CSP program evolution and Open License program changes, please see **Next Steps** below.</span></span>

### <a name="next-steps"></a><span data-ttu-id="fcd31-457">Sonraki Adımlar:</span><span class="sxs-lookup"><span data-stu-id="fcd31-457">Next Steps:</span></span>

- <span data-ttu-id="fcd31-458">CSP program evrimi: [bulut çözümü sağlayıcısı program](https://partner.microsoft.com/resources/collection/software-in-csp#/) hazırlık malzemelerinden kalıcı yazılımı gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="fcd31-458">CSP Program evolution:  Review the [Perpetual software in the Cloud Solution Provider program](https://partner.microsoft.com/resources/collection/software-in-csp#/) readiness materials.</span></span> <span data-ttu-id="fcd31-459">Rolünüzün doğru bilgilerini hızlı bir şekilde bulmak için bu [hazırlık haritasını](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) kullanın.</span><span class="sxs-lookup"><span data-stu-id="fcd31-459">Use this [readiness map](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

- <span data-ttu-id="fcd31-460">Lisans programı değişikliklerini aç: [CSP program evrimini gözden geçirin ve açık lisans programı değişiklikleri](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) hazırlık malzemelerini inceleyin.</span><span class="sxs-lookup"><span data-stu-id="fcd31-460">Open License program changes:  Review the [CSP program evolution and Open License program changes](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) readiness materials.</span></span> <span data-ttu-id="fcd31-461">Rolünüzün doğru bilgilerini hızlı bir şekilde bulmak için bu [hazırlık haritasını](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) kullanın.</span><span class="sxs-lookup"><span data-stu-id="fcd31-461">Use this [readiness map](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

### <a name="questions"></a><span data-ttu-id="fcd31-462">Sorular</span><span class="sxs-lookup"><span data-stu-id="fcd31-462">Questions</span></span>

<span data-ttu-id="fcd31-463">Diğer sorular için lütfen ilgili CSP Yammer topluluklarınızı denetleyin.</span><span class="sxs-lookup"><span data-stu-id="fcd31-463">For any further questions please check your relevant CSP Yammer communities.</span></span>

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a><span data-ttu-id="fcd31-464">Önceki bir duyuruya güncelleştirme: Premium değerlendirmeler, uyumluluk Yöneticisi eklentisi</span><span class="sxs-lookup"><span data-stu-id="fcd31-464">Update to a previous announcement: Premium Assessments, an add-on to Compliance Manager</span></span>

### <a name="categories"></a><span data-ttu-id="fcd31-465">Kategoriler</span><span class="sxs-lookup"><span data-stu-id="fcd31-465">Categories</span></span>

- <span data-ttu-id="fcd31-466">Tarih: 2021-03-15</span><span class="sxs-lookup"><span data-stu-id="fcd31-466">Date: 2021-03-15</span></span>
- <span data-ttu-id="fcd31-467">İşlerinizi büyütme</span><span class="sxs-lookup"><span data-stu-id="fcd31-467">Grow your business</span></span>

### <a name="summary"></a><span data-ttu-id="fcd31-468">Özet</span><span class="sxs-lookup"><span data-stu-id="fcd31-468">Summary</span></span>

<span data-ttu-id="fcd31-469">Deneme teklifleri fiyat listesinde listelenmemelidir ve kaldırılacak.</span><span class="sxs-lookup"><span data-stu-id="fcd31-469">The trial offers shouldn’t have been listed on the price list and will be removed.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcd31-470">Etkilenen hedef kitle</span><span class="sxs-lookup"><span data-stu-id="fcd31-470">Impacted audience</span></span>

<span data-ttu-id="fcd31-471">Bulut çözüm sağlayıcısı aracılığıyla iş ortakları deneyimidir</span><span class="sxs-lookup"><span data-stu-id="fcd31-471">Partners transacting through Cloud Solution Provider</span></span>

### <a name="details"></a><span data-ttu-id="fcd31-472">Ayrıntılar</span><span class="sxs-lookup"><span data-stu-id="fcd31-472">Details</span></span>

<span data-ttu-id="fcd31-473">Deneme teklifleri fiyat listesine dahil edilmemelidir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-473">The trial offers shouldn’t have been included in the price list.</span></span> <span data-ttu-id="fcd31-474">Bunlar 1 Mayıs 2021 fiyat listesinden kaldırılacak.</span><span class="sxs-lookup"><span data-stu-id="fcd31-474">These will be removed from the May 1, 2021 price list.</span></span>

<span data-ttu-id="fcd31-475">Özgün duyuru [burada](./2021-february.md#4)bulunur.</span><span class="sxs-lookup"><span data-stu-id="fcd31-475">The original announcement is [here](./2021-february.md#4).</span></span>

### <a name="additional-resources"></a><span data-ttu-id="fcd31-476">Ek kaynaklar</span><span class="sxs-lookup"><span data-stu-id="fcd31-476">Additional resources</span></span>

- [<span data-ttu-id="fcd31-477">Microsoft 365 E5 güvenlik ve uyumluluk</span><span class="sxs-lookup"><span data-stu-id="fcd31-477">Microsoft 365 E5 security and compliance</span></span>](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [<span data-ttu-id="fcd31-478">Microsoft Uyumluluk Yöneticisi-Microsoft 365 uyumluluğu 'nda değerlendirme oluşturma ve yönetme</span><span class="sxs-lookup"><span data-stu-id="fcd31-478">Build and manage assessments in Microsoft Compliance Manager - Microsoft 365 Compliance</span></span>](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a><span data-ttu-id="fcd31-479">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="fcd31-479">Next steps</span></span>

<span data-ttu-id="fcd31-480">Bu konuyla ilgili kaynakları gözden geçirin ve bu bilgileri kuruluşunuzdaki uygun hissedarlarla paylaşabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-480">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="fcd31-481">Sorularınız mı var?</span><span class="sxs-lookup"><span data-stu-id="fcd31-481">Questions?</span></span>

<span data-ttu-id="fcd31-482">Bu tekliflerle ilgili sorular için ilgili Yammer topluluklarınızı kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="fcd31-482">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> <span data-ttu-id="fcd31-483">Çözümlerinizi bir ticari Iş ortağından (OCP) Microsoft ticari Market 'e (GTM) taşıma</span><span class="sxs-lookup"><span data-stu-id="fcd31-483">Migrate your solutions from One Commercial Partner (OCP) go-to market (GTM) to the Microsoft commercial marketplace</span></span>

### <a name="categories"></a><span data-ttu-id="fcd31-484">Kategoriler</span><span class="sxs-lookup"><span data-stu-id="fcd31-484">Categories</span></span>

- <span data-ttu-id="fcd31-485">Tarih: 2021-03-12</span><span class="sxs-lookup"><span data-stu-id="fcd31-485">Date: 2021-03-12</span></span>
- <span data-ttu-id="fcd31-486">Özellikler</span><span class="sxs-lookup"><span data-stu-id="fcd31-486">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="fcd31-487">Özet</span><span class="sxs-lookup"><span data-stu-id="fcd31-487">Summary</span></span>

<span data-ttu-id="fcd31-488">29 Mart 2021 ' den itibaren, sınırlı bir ticari Iş ortağı (OCP) go-to market (GTM) özelliği ile karşılaşırsınız.</span><span class="sxs-lookup"><span data-stu-id="fcd31-488">From March 29, 2021, you will begin to experience limited One Commercial Partner (OCP) go-to market (GTM) capabilities.</span></span> <span data-ttu-id="fcd31-489">Çözümlerinizi Iş Ortağı Merkezi ' nde ticari Market 'e geçirmenizi öneririz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-489">We encourage you to migrate your solutions to the commercial marketplace in Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcd31-490">Etkilenen hedef kitle</span><span class="sxs-lookup"><span data-stu-id="fcd31-490">Impacted audience</span></span>

<span data-ttu-id="fcd31-491">OCP GTM 'de çözümlerle ortak satış kurumları</span><span class="sxs-lookup"><span data-stu-id="fcd31-491">Organizations co-selling with solutions in OCP GTM</span></span>

### <a name="details"></a><span data-ttu-id="fcd31-492">Ayrıntılar</span><span class="sxs-lookup"><span data-stu-id="fcd31-492">Details</span></span>

<span data-ttu-id="fcd31-493">Aralık 2020 ' de, Microsoft OCP GTM aracından gelen yolculuğumuzu Iş Ortağı Merkezi 'nde Microsoft Commercial Market 'e başladık.</span><span class="sxs-lookup"><span data-stu-id="fcd31-493">In December 2020, we started our journey from the Microsoft OCP GTM tool to the Microsoft commercial marketplace in Partner Center.</span></span> <span data-ttu-id="fcd31-494">Bu geçiş ticari Market 'in yeteneklerini genişleterek, çözümlerinizi milyonlarca müşteriye göre sergilemenize, diğer Microsoft ve iş ortağı satıcılarıyla fırsatları daha da paylaşabilir ve yenilikçi çözümleri ortaklaşa satabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-494">This transition expands the capabilities of the commercial marketplace where you can showcase your solutions to millions of customers, bidirectionally share opportunities with other Microsoft and partner sellers, and jointly sell innovative solutions.</span></span>

<span data-ttu-id="fcd31-495">Geçişin sonraki kilometre taşı, 29 Mart 2021 ' de gerçekleşmeyecektir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-495">The next milestone in the transition will take place on March 29, 2021.</span></span> <span data-ttu-id="fcd31-496">Diğer bir deyişle, bazı alanlar salt okunurdur, sınırlı OCP GTM özelliklerine karşılaşmak için başlarsınız.</span><span class="sxs-lookup"><span data-stu-id="fcd31-496">That’s when you’ll begin to experience limited OCP GTM capabilities, with some fields becoming read-only.</span></span> <span data-ttu-id="fcd31-497">Şu anda OCP GTM 'deki çözümlerle ortak satıyorsanız, kendi özelliklerinden faydalanmak ve yayımlama deneyiminizi basitleştirmek için çözümlerinizi ticari Market 'e geçirmenizi öneririz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-497">If you’re currently co-selling with solutions in OCP GTM, we encourage you to migrate your solutions to the commercial marketplace to take advantage of its capabilities and simplify your publishing experience.</span></span> 

<span data-ttu-id="fcd31-498">Ticari Market 'e geçiş yapmak Iş Ortağı Merkezi 'ni ortak satış yayımlama deneyiminin birincil hedefine getirir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-498">Moving to the commercial marketplace makes Partner Center the primary destination for the co-sell publishing experience.</span></span> <span data-ttu-id="fcd31-499">Çözümlerinizi, Microsoft ürünleri için kullandığımız aynı kanallar ve ürün içi deneyimler aracılığıyla paylaşılan müşterilerimiz ile bağlayarak işinizi büyütmeye devam edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-499">It’s where you can continue to grow your business by connecting your solutions with our shared customers through the same channels and in-product experiences that we use for Microsoft products.</span></span> <span data-ttu-id="fcd31-500">[Ticari Market hakkında daha fazla bilgi edinin](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span><span class="sxs-lookup"><span data-stu-id="fcd31-500">[Learn more about the commercial marketplace](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span></span>

### <a name="next-steps"></a><span data-ttu-id="fcd31-501">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="fcd31-501">Next steps</span></span>

- <span data-ttu-id="fcd31-502">Çözümlerinizi henüz taşıdıysanız, geçiş [kılavuzunda](/azure/marketplace/co-sell-solution-migration) açıklanan yönergeleri izleyin veya tüm geçiş etkinliklerini tamamlayıp, ticari markette çözümünüzü yayımlamaya başlamak için [adım adım video öğreticisini](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) görüntüleyin.</span><span class="sxs-lookup"><span data-stu-id="fcd31-502">If you have not yet moved your solutions, follow the instructions detailed in the [transition guide](/azure/marketplace/co-sell-solution-migration) or view the [step-by-step video tutorial](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) to complete all migration activities and start publishing your solution(s) in the commercial marketplace.</span></span>

- <span data-ttu-id="fcd31-503">OCP GTM 'deki sınırlı yetenek deneyimiyle ilgili sorularınız için, [Microsoft ticari Market SSS 'de yayımlanacak ortak satış gereksinimlerini](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf)görüntüleyin.</span><span class="sxs-lookup"><span data-stu-id="fcd31-503">For questions regarding the limited capability experience in OCP GTM, view the [Co-sell requirements to publish in the Microsoft commercial marketplace FAQ](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span></span> <span data-ttu-id="fcd31-504">(29 Mart 2021 ' i Başlatan "OCP GTM Limited yetenekler" bölümüne bakın.)</span><span class="sxs-lookup"><span data-stu-id="fcd31-504">(See the section “OCP GTM limited capabilities starting March 29, 2021.”)</span></span>

### <a name="questions"></a><span data-ttu-id="fcd31-505">Sorularınız mı var?</span><span class="sxs-lookup"><span data-stu-id="fcd31-505">Questions?</span></span>

<span data-ttu-id="fcd31-506">Sorularınız varsa veya daha fazla bilgiye ihtiyacınız varsa [desteğe](https://partner.microsoft.com/support/?stage=1) başvurun.</span><span class="sxs-lookup"><span data-stu-id="fcd31-506">Contact [Support](https://partner.microsoft.com/support/?stage=1) if you have any questions or need more information.</span></span>

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a><span data-ttu-id="fcd31-507">Azure için bulut çözümü sağlayıcısı (CSP) programında yeni ticaret deneyimini Rusya 'ya genişletme</span><span class="sxs-lookup"><span data-stu-id="fcd31-507">Expanding the new commerce experience in the Cloud Solution Provider (CSP) program for Azure to Russia</span></span>

### <a name="categories"></a><span data-ttu-id="fcd31-508">Kategoriler</span><span class="sxs-lookup"><span data-stu-id="fcd31-508">Categories</span></span>

- <span data-ttu-id="fcd31-509">Tarih: 2021-03-10</span><span class="sxs-lookup"><span data-stu-id="fcd31-509">Date: 2021-03-10</span></span>
- <span data-ttu-id="fcd31-510">Özellikler</span><span class="sxs-lookup"><span data-stu-id="fcd31-510">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcd31-511">Etkilenen hedef kitle</span><span class="sxs-lookup"><span data-stu-id="fcd31-511">Impacted audience</span></span>

<span data-ttu-id="fcd31-512">Rusya 'daki tüm iş ortakları bulut çözümü sağlayıcısı (CSP) programı üzerinden deneyimidir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-512">All partners in Russia transacting through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="fcd31-513">Ayrıntılar</span><span class="sxs-lookup"><span data-stu-id="fcd31-513">Details</span></span>

<span data-ttu-id="fcd31-514">10 2021 Mart 'tan itibaren, **Rusya 'Da Azure IÇIN CSP 'de yeni ticaret deneyiminin** kullanılabilirliğini duyurmaktan mutluluk duyuyoruz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-514">Starting March 10 2021, we’re excited to announce the availability of the **new commerce experience in CSP for Azure in Russia**.</span></span> <span data-ttu-id="fcd31-515">Bu deneyim, müşterilerin Azure hizmetlerini satın alıp tüketme yöntemini kolaylaştırır ve geliştirir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-515">This experience will streamline and improve the way customers buy and consume Azure services.</span></span> <span data-ttu-id="fcd31-516">Ayrıca, CSP programındaki iş ortaklarına satış momalları genelinde Azure fiyatlandırması için tutarlı bir görünüm, genel tutarlılık için ABD Doları fiyatlandırması, faturalandırma tarihi hizalaması ve Azure maliyet yönetimine erişim hakkı verecektir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-516">It will also give partners in the CSP program a consistent view of Azure pricing across sales motions, USD pricing for global consistency, billing date alignment, and access to Azure Cost Management.</span></span>

### <a name="next-steps"></a><span data-ttu-id="fcd31-517">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="fcd31-517">Next steps</span></span>

<span data-ttu-id="fcd31-518">Yeni Azure ticari deneyimine giriş ve ek bilgi sağlama gibi birkaç kaynak mevcuttur.</span><span class="sxs-lookup"><span data-stu-id="fcd31-518">There are several resources available introducing the new Azure commerce experience and providing additional information.</span></span> <span data-ttu-id="fcd31-519">[CSP program güncelleştirmeleri kaynak galerisinde](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/)en son SSS, Decks, video ve daha fazlasını bulun.</span><span class="sxs-lookup"><span data-stu-id="fcd31-519">Find the latest FAQs, decks, video and more in the [CSP Program Updates Resource Gallery](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span></span>

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a><span data-ttu-id="fcd31-520">İş Ortağı Merkezi Yazılım lisans anahtarı ve indirme karşılama</span><span class="sxs-lookup"><span data-stu-id="fcd31-520">Partner Center software license key and download fulfillment</span></span>

### <a name="categories"></a><span data-ttu-id="fcd31-521">Kategoriler</span><span class="sxs-lookup"><span data-stu-id="fcd31-521">Categories</span></span>

- <span data-ttu-id="fcd31-522">Tarih: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="fcd31-522">Date: 2021-03-04</span></span>
- <span data-ttu-id="fcd31-523">Özellikler</span><span class="sxs-lookup"><span data-stu-id="fcd31-523">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="fcd31-524">Özet</span><span class="sxs-lookup"><span data-stu-id="fcd31-524">Summary</span></span>

<span data-ttu-id="fcd31-525">Iş Ortağı Merkezi yazılım indirme ve lisans anahtarı karşılama özelliği yeniden belirtilmiştir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-525">The Partner Center software download and license key fulfillment capability has been reinstated.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcd31-526">Etkilenen hedef kitle</span><span class="sxs-lookup"><span data-stu-id="fcd31-526">Impacted audience</span></span>

<span data-ttu-id="fcd31-527">Tüm bulut çözümü sağlayıcısı (CSP) iş ortakları, kalıcı ve sunucu aboneliği yazılım siparişlerinin Iş Ortağı Merkezi aracılığıyla deneyimidir</span><span class="sxs-lookup"><span data-stu-id="fcd31-527">All Cloud Solution Provider (CSP) partners transacting perpetual and server subscription software orders through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="fcd31-528">Ayrıntılar</span><span class="sxs-lookup"><span data-stu-id="fcd31-528">Details</span></span>

<span data-ttu-id="fcd31-529">İş ortağı geri bildirimlerine yanıt olarak, kalıcı ve sunucu aboneliği yazılım siparişleri için yazılım ve lisans anahtarları almak üzere Iş Ortağı Merkezi 'ni karşılama özelliğini sunuyoruz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-529">In response to partner feedback, we’re reinstating the Partner Center fulfillment capability to obtain software and license keys for perpetual and server subscription software orders.</span></span> <span data-ttu-id="fcd31-530">19 Ocak 2021 ' de kaldırılmadan önce önceki durumuna geri yüklenecek.</span><span class="sxs-lookup"><span data-stu-id="fcd31-530">It will be restored to its previous state prior to being removed on January 19, 2021.</span></span> <span data-ttu-id="fcd31-531">( [Duyuruya](2020-september.md#17)bakın.)</span><span class="sxs-lookup"><span data-stu-id="fcd31-531">(See the [announcement](2020-september.md#17).)</span></span>

<span data-ttu-id="fcd31-532">Yazılım lisans anahtarlarının ve indirme bağlantılarının, fikri mülkiyet varlıklarından sonra değerli ve yüksek oranda aranan olduğunu unutmayın.</span><span class="sxs-lookup"><span data-stu-id="fcd31-532">Note that software license keys and download links are valuable and highly sought-after intellectual property assets.</span></span> <span data-ttu-id="fcd31-533">Sızmış ise, etkinleştirme sınırlarının tükenmesine ve olumsuz bir müşteri ve iş ortağı deneyimine neden olabilir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-533">If leaked, they can quickly be depleted of their activation limits and cause a negative customer and partner experience.</span></span>

### <a name="next-steps"></a><span data-ttu-id="fcd31-534">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="fcd31-534">Next steps</span></span>

<span data-ttu-id="fcd31-535">Kullanım yönergeleri ve yazılım anahtarı dağıtımı hakkında önemli yönergeler için aşağıdaki kaynakları gözden geçirin:</span><span class="sxs-lookup"><span data-stu-id="fcd31-535">Review the following resources for usage instructions and important guidance on software key distribution:</span></span>

- [<span data-ttu-id="fcd31-536">CSP programı aracılığıyla şirket içi yazılım satma</span><span class="sxs-lookup"><span data-stu-id="fcd31-536">Sell on-premises software through the CSP program</span></span>](../csp-on-premise-software.md)
- <span data-ttu-id="fcd31-537">[Iş Ortağı Merkezi yeni ticaret Işlemleri Kılavuzu](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) ( **yazılım anahtarı dağıtımı hakkında rehberlik** bölümüne bakın.)</span><span class="sxs-lookup"><span data-stu-id="fcd31-537">[Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (See the **Guidance on Software Key Distribution** section.)</span></span>

### <a name="questions"></a><span data-ttu-id="fcd31-538">Sorularınız mı var?</span><span class="sxs-lookup"><span data-stu-id="fcd31-538">Questions?</span></span>

<span data-ttu-id="fcd31-539">Bu bildirimde ilgili başka sorularınız varsa ilgili Yammer topluluklarınızı kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="fcd31-539">If you have any further questions about this notice, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a><span data-ttu-id="fcd31-540">Iş ortağı satış bağlantısı (PSC) üzerinden Iş Ortağı Merkezi 'ne anlaşmalar geçirin</span><span class="sxs-lookup"><span data-stu-id="fcd31-540">Migrate your deals from Partner Sales Connect (PSC) to Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="fcd31-541">Kategoriler</span><span class="sxs-lookup"><span data-stu-id="fcd31-541">Categories</span></span>

- <span data-ttu-id="fcd31-542">Tarih: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="fcd31-542">Date: 2021-03-04</span></span>
- <span data-ttu-id="fcd31-543">Özellikler</span><span class="sxs-lookup"><span data-stu-id="fcd31-543">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="fcd31-544">Özet</span><span class="sxs-lookup"><span data-stu-id="fcd31-544">Summary</span></span>

<span data-ttu-id="fcd31-545">İş ortağı satış bağlantısı (PSC), 31 Mart 2021 ' den itibaren salt okunurdur. bu nedenle, PSC 'lerden Iş ortağı merkezine geçişlerinizi geçirmeye başlamanızı başlıyoruz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-545">Partner Sales Connect (PSC) will move to read-only access starting March 31, 2021, so we urge you to begin migrating your deals from PSC to Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcd31-546">Etkilenen hedef kitle</span><span class="sxs-lookup"><span data-stu-id="fcd31-546">Impacted audience</span></span>

<span data-ttu-id="fcd31-547">PSC 'de anlaşmalar olan iş ortakları</span><span class="sxs-lookup"><span data-stu-id="fcd31-547">Partners with deals in PSC</span></span>

### <a name="details"></a><span data-ttu-id="fcd31-548">Ayrıntılar</span><span class="sxs-lookup"><span data-stu-id="fcd31-548">Details</span></span>

<span data-ttu-id="fcd31-549">Paylaşılan büyüme taahhüdünün bir parçası olarak **Microsoft ile ortak satış** , keşfedilmesi için kullanabileceğiniz yoldur **, uzmanlığınızı sunun ve olumlu müşteri sonuçları için müşteri parmak izini genişletmenizi** sağlar.</span><span class="sxs-lookup"><span data-stu-id="fcd31-549">As part of our shared commitment to growth, **co-sell with Microsoft** is the path for you to **be discovered, deliver your expertise, and expand your customer footprint** for positive customer outcomes.</span></span> <span data-ttu-id="fcd31-550">Normalden **3,5 kat daha hızlı** bir ortalama Işlem olan Iş Ortağı Merkezi 'nde ortak satış deneyiminizi yönetmek, doğrudan müşteri, iş ortağı ve Microsoft satıcı kanallarından satış yapmanıza ve tüm başvuru işlem hattınızı tek bir konumda yönetmenize olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="fcd31-550">With an average deal that’s **3.5 times faster** than normal, managing your co-sell experience in Partner Center allows you to sell across the direct customer, partner, and Microsoft seller channels, and manage your entire referral pipeline in one location.</span></span>

<span data-ttu-id="fcd31-551">**PSC** , **31 Mart 2021**' den itibaren **salt okuma erişimine** geçer, bu nedenle iş ortağı merkezi 'ne taşıma ve bu özellik geliştirmelerini erişme hakkında bilgi alırız:</span><span class="sxs-lookup"><span data-stu-id="fcd31-551">**PSC** will move to **read-only access** starting **March 31, 2021**, so we urge you to start your move to Partner Center and access these capability improvements:</span></span> 

- <span data-ttu-id="fcd31-552">Microsoft ile paylaştığınız anlaşmalar, ihtiyacınız olan yardım türüne göre doğru satıcı için **daha doğru bir şekilde yönlendirilmenizi** sağlar.</span><span class="sxs-lookup"><span data-stu-id="fcd31-552">**More accurate routing** of the deals that you share with Microsoft to the right seller, based on the type of assistance you need.</span></span>
- <span data-ttu-id="fcd31-553">Mücadele için uygun çözümler ve ISV Connect program ölçütlerini karşılamak için, onay işlemini ve nihai yürütme (POE) kanıtlamayı basitleştirecek olan **ön ödemeli uygunluk doğrulaması** .</span><span class="sxs-lookup"><span data-stu-id="fcd31-553">**Upfront deal eligibility validation** for incentive-eligible solutions and to meet the ISV Connect program criteria, simplifying the approval process and final proof of execution (POE) attestation.</span></span>
- <span data-ttu-id="fcd31-554">Tüm ortak satış fırsatlarınızı ve satış nitelikli müşteri adaylarını tek bir yerde yönetmek için **sorunsuz Kullanıcı deneyimi** .</span><span class="sxs-lookup"><span data-stu-id="fcd31-554">**Seamless user experience** to manage all your co-sell opportunities and sales qualified leads in one place.</span></span>

<span data-ttu-id="fcd31-555">Ayrıca, taşınmasında yardımcı olması için Iş Ortağı Merkezi 'nde yeni özellikler ekledik:</span><span class="sxs-lookup"><span data-stu-id="fcd31-555">We’ve also recently added new features in Partner Center to assist in your move:</span></span>

- [<span data-ttu-id="fcd31-556">Ortak satış fırsatları için toplu işlemler</span><span class="sxs-lookup"><span data-stu-id="fcd31-556">Bulk operations for co-sell opportunities</span></span>](../bulk-operations.md)
- <span data-ttu-id="fcd31-557">[Geçiş özelliğini dağıt](../psc-to-pc.md) ( **PSC anlaşmalar geçiş** bölümüne bakın.)</span><span class="sxs-lookup"><span data-stu-id="fcd31-557">[Deal migration feature](../psc-to-pc.md) (See the **PSC Deals migration** section.)</span></span>

<span data-ttu-id="fcd31-558">Iş Ortağı Merkezi 'nde ortak satış deneyimini kullanarak, satış ekipleriniz, bu müşteri adaylarına ve fırsatlara odaklanmak, anlaşmaları kapatmak ve müşteri ilişkileri oluşturmak için daha fazla zaman alır.</span><span class="sxs-lookup"><span data-stu-id="fcd31-558">Using the co-sell experience in Partner Center, your sales teams will have more time to focus on nurturing leads and opportunities, closing deals, and creating lasting customer relationships.</span></span>

### <a name="next-steps"></a><span data-ttu-id="fcd31-559">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="fcd31-559">Next steps</span></span>

<span data-ttu-id="fcd31-560">Iş Ortağı Merkezi [geçiş kılavuzunu](../psc-to-pc.md) kullanarak, PSC 'Lerden Iş ortağı merkezine anlaşmalar geçirme adımlarında size yol gösterir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-560">Use the Partner Center [transition guide](../psc-to-pc.md) to walk you through the steps to migrate your deals from PSC to Partner Center.</span></span>

### <a name="questions"></a><span data-ttu-id="fcd31-561">Sorularınız mı var?</span><span class="sxs-lookup"><span data-stu-id="fcd31-561">Questions?</span></span>

<span data-ttu-id="fcd31-562">Daha fazla soru için [desteğe](https://partner.microsoft.com/support/?stage=1)başvurun.</span><span class="sxs-lookup"><span data-stu-id="fcd31-562">For any further questions, contact [Support](https://partner.microsoft.com/support/?stage=1).</span></span>

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a><span data-ttu-id="fcd31-563">Yeni Microsoft Dynamics 365 ürünleri ve 1 Nisan 2021 ' de sunulan teklifler</span><span class="sxs-lookup"><span data-stu-id="fcd31-563">New Microsoft Dynamics 365 products and offers available on April 1, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="fcd31-564">Kategoriler</span><span class="sxs-lookup"><span data-stu-id="fcd31-564">Categories</span></span>

- <span data-ttu-id="fcd31-565">Tarih: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="fcd31-565">Date: 2021-03-04</span></span>
- <span data-ttu-id="fcd31-566">Özellikler</span><span class="sxs-lookup"><span data-stu-id="fcd31-566">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="fcd31-567">Özet</span><span class="sxs-lookup"><span data-stu-id="fcd31-567">Summary</span></span>

<span data-ttu-id="fcd31-568">Microsoft, 1 Nisan 2021 ' de, bulut çözümü sağlayıcısı (CSP) programı için birkaç yeni ürün ve teklif başlatacaktır.</span><span class="sxs-lookup"><span data-stu-id="fcd31-568">On April 1, 2021, Microsoft will be launching several new products and offers for the Cloud Solution Provider (CSP) program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcd31-569">Etkilenen hedef kitle</span><span class="sxs-lookup"><span data-stu-id="fcd31-569">Impacted audience</span></span>

<span data-ttu-id="fcd31-570">Tüm iş ortakları bulut çözümü sağlayıcısı (CSP) programı üzerinden deneyimidir</span><span class="sxs-lookup"><span data-stu-id="fcd31-570">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="fcd31-571">Ayrıntılar</span><span class="sxs-lookup"><span data-stu-id="fcd31-571">Details</span></span>

<span data-ttu-id="fcd31-572">Microsoft, 1 Nisan 2021 ' de aşağıdaki yeni ürünleri ve şunları sunuyor:</span><span class="sxs-lookup"><span data-stu-id="fcd31-572">On April 1, 2021, Microsoft will be launching the following new products and offers:</span></span>

- <span data-ttu-id="fcd31-573">Kullanıcı başına Power BI Premium</span><span class="sxs-lookup"><span data-stu-id="fcd31-573">Power BI Premium Per User</span></span>
- <span data-ttu-id="fcd31-574">Müşteri ses ve pazarlama USL coğrafi ve segment genişletme</span><span class="sxs-lookup"><span data-stu-id="fcd31-574">Customer Voice and Marketing USL geo and segment expansion</span></span>

<span data-ttu-id="fcd31-575">**Kullanıcı başına Power BI Premium**</span><span class="sxs-lookup"><span data-stu-id="fcd31-575">**Power BI Premium Per User**</span></span>

<span data-ttu-id="fcd31-576">Microsoft, ilk Kullanıcı başına Power BI Premium tekliflerini tanıtacaktır.</span><span class="sxs-lookup"><span data-stu-id="fcd31-576">Microsoft will introduce the first per-user Power BI Premium offers.</span></span> <span data-ttu-id="fcd31-577">Power BI Premium Şu anda yalnızca bir kapasite yapısında satılabilir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-577">Power BI Premium is currently sold only in a capacity construct.</span></span> <span data-ttu-id="fcd31-578">Kullanıcı başına Power BI Premium kurumsal iş zekası (BI) ve analiz özelliklerine erişim sağlar.</span><span class="sxs-lookup"><span data-stu-id="fcd31-578">Power BI Premium Per User provides access to enterprise business intelligence (BI) and analytics capabilities.</span></span> <span data-ttu-id="fcd31-579">Esnek bireysel bilgisayar lisanslama, küçük ve orta ölçekli işletmeler için.</span><span class="sxs-lookup"><span data-stu-id="fcd31-579">Its flexible individual seat licensing caters to small and medium-sized businesses.</span></span>

<span data-ttu-id="fcd31-580">Bu teklif hakkında daha fazla bilgi edinmek için [Power BI sürüm ayrıntılarını](/power-platform-release-plan/2020wave2/power-bi/planned-features) gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="fcd31-580">Review the [Power BI release details](/power-platform-release-plan/2020wave2/power-bi/planned-features) to learn more about this offer.</span></span>


<span data-ttu-id="fcd31-581">**Teklif Ayrıntıları**</span><span class="sxs-lookup"><span data-stu-id="fcd31-581">**Offer details**</span></span>

<span data-ttu-id="fcd31-582">Teklif adının fiyat listesi önizlemeden biraz farklı olduğunu unutmayın.</span><span class="sxs-lookup"><span data-stu-id="fcd31-582">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="fcd31-583">Teklif adı</span><span class="sxs-lookup"><span data-stu-id="fcd31-583">Offer name</span></span> | <span data-ttu-id="fcd31-584">Teklif Kimliği</span><span class="sxs-lookup"><span data-stu-id="fcd31-584">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="fcd31-585">Kullanıcı başına Power BI Premium</span><span class="sxs-lookup"><span data-stu-id="fcd31-585">Power BI Premium Per User</span></span> | <span data-ttu-id="fcd31-586">9c810018-9356-4903-95ab-eeb956289290</span><span class="sxs-lookup"><span data-stu-id="fcd31-586">9c810018-9356-4903-95ab-eeb956289290</span></span> | 
| <span data-ttu-id="fcd31-587">Fakülteler için Kullanıcı başına Power BI Premium</span><span class="sxs-lookup"><span data-stu-id="fcd31-587">Power BI Premium Per User for Faculty</span></span> | <span data-ttu-id="fcd31-588">3afc44f-f372-4ad5-8657-aadd9574fce0</span><span class="sxs-lookup"><span data-stu-id="fcd31-588">3affc44f-f372-4ad5-8657-aadd9574fce0</span></span> | 
| <span data-ttu-id="fcd31-589">Öğrenciler için Kullanıcı başına Power BI Premium</span><span class="sxs-lookup"><span data-stu-id="fcd31-589">Power BI Premium Per User for Students</span></span> | <span data-ttu-id="fcd31-590">657eea87-d0b0-4c89-8c8e-9b04395bd940</span><span class="sxs-lookup"><span data-stu-id="fcd31-590">657eea87-d0b0-4c89-8c8e-9b04395bd940</span></span> | 
| <span data-ttu-id="fcd31-591">Kullanıcı başına Power BI Premium (kar personeli olmayan personel fiyatlandırması)</span><span class="sxs-lookup"><span data-stu-id="fcd31-591">Power BI Premium Per User (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="fcd31-592">7a0a856c-059f-45dd-9d26-ae27992e706a</span><span class="sxs-lookup"><span data-stu-id="fcd31-592">7a0a856c-059f-45dd-9d26-ae27992e706a</span></span> | 
| <span data-ttu-id="fcd31-593">Kullanıcı başına Power BI Premium Add-On</span><span class="sxs-lookup"><span data-stu-id="fcd31-593">Power BI Premium Per User Add-On</span></span> | <span data-ttu-id="fcd31-594">244ff87e-5925-44a0-BF31-gizlenir 189719b58</span><span class="sxs-lookup"><span data-stu-id="fcd31-594">244ff87e-5925-44a0-bf31-cea189719b58</span></span> | 
| <span data-ttu-id="fcd31-595">Fakülteler için Kullanıcı başına Power BI Premium Add-On</span><span class="sxs-lookup"><span data-stu-id="fcd31-595">Power BI Premium Per User Add-On for Faculty</span></span> | <span data-ttu-id="fcd31-596">5dad849bd-b8f7-4340-b4f4-3a9eaeb8987e</span><span class="sxs-lookup"><span data-stu-id="fcd31-596">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span></span> | 
| <span data-ttu-id="fcd31-597">Öğrenciler için Kullanıcı başına Add-On Power BI Premium</span><span class="sxs-lookup"><span data-stu-id="fcd31-597">Power BI Premium Per User Add-On for Students</span></span> | <span data-ttu-id="fcd31-598">cf62d70d-5af5-422a-bda8-97936402ac8e</span><span class="sxs-lookup"><span data-stu-id="fcd31-598">cf62d70d-5af5-422a-bda8-97936402ac8e</span></span> | 
| <span data-ttu-id="fcd31-599">Kullanıcı başına Power BI Premium Add-On (kar amacı gütmeyen personel fiyatlandırması)</span><span class="sxs-lookup"><span data-stu-id="fcd31-599">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="fcd31-600">31c03289-47AB-4AB0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="fcd31-600">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span> | 

<span data-ttu-id="fcd31-601">**Müşteri ses ve pazarlama USL coğrafi ve segment genişletme**</span><span class="sxs-lookup"><span data-stu-id="fcd31-601">**Customer Voice and Marketing USL geo and segment expansion**</span></span>

<span data-ttu-id="fcd31-602">Aralık 2020 başlatmaya yönelik bir izleme olarak Dynamics 365 müşteri Voice ve Marketing USL teklifleri, yeni ülkeler ve daha fazla kar ve eğitim SKU 'Ları eklemek üzere değiştirilmiştir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-602">As a follow-up to the December 2020 launch, Dynamics 365 Customer Voice and Marketing USL offers have been changed to add new countries and more nonprofit and educational SKUs.</span></span>

| <span data-ttu-id="fcd31-603">Teklif adı</span><span class="sxs-lookup"><span data-stu-id="fcd31-603">Offer name</span></span> | <span data-ttu-id="fcd31-604">Teklif Kimliği</span><span class="sxs-lookup"><span data-stu-id="fcd31-604">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="fcd31-605">Dynamics 365 müşteri sesi USL (kar amacı gütmeyen personel fiyatlandırması)</span><span class="sxs-lookup"><span data-stu-id="fcd31-605">Dynamics 365 Customer Voice USL (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="fcd31-606">7a8642a5-481e-4906-a642-b56dbeeb62a0</span><span class="sxs-lookup"><span data-stu-id="fcd31-606">7a8642a5-481e-4906-a642-b56dbeeb62a0</span></span> |
| <span data-ttu-id="fcd31-607">Fakülteler için Dynamics 365 müşteri sesi USL</span><span class="sxs-lookup"><span data-stu-id="fcd31-607">Dynamics 365 Customer Voice USL for Faculty</span></span> | <span data-ttu-id="fcd31-608">85162d70-9676-4CF6-A4BC-a0d6672f2657</span><span class="sxs-lookup"><span data-stu-id="fcd31-608">85162d70-9676-4cf6-a4bc-a0d6672f2657</span></span> |

<span data-ttu-id="fcd31-609">Bu teklifler hakkında daha fazla bilgi edinmek için aşağıdaki sayfaları ziyaret edin:</span><span class="sxs-lookup"><span data-stu-id="fcd31-609">Visit the following pages to find out more about these offers:</span></span>

- [<span data-ttu-id="fcd31-610">Dynamics 365 müşteri hizmeti sesli giriş sayfası</span><span class="sxs-lookup"><span data-stu-id="fcd31-610">Dynamics 365 Customer Service Voice home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)
- [<span data-ttu-id="fcd31-611">Dynamics 365 pazarlama ana sayfası</span><span class="sxs-lookup"><span data-stu-id="fcd31-611">Dynamics 365 Marketing home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a><span data-ttu-id="fcd31-612">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="fcd31-612">Next steps</span></span>

<span data-ttu-id="fcd31-613">Bu konudaki kaynakları gözden geçirin ve bu bilgileri kuruluşunuzdaki uygun hissedarlarla paylaşabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-613">Review the resources on this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="fcd31-614">Sorularınız mı var?</span><span class="sxs-lookup"><span data-stu-id="fcd31-614">Questions?</span></span>

<span data-ttu-id="fcd31-615">Bu tekliflerle ilgili herhangi bir soru için ilgili Yammer topluluklarınızı kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="fcd31-615">For any questions about these offers, check your relevant Yammer communities.</span></span> 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> <span data-ttu-id="fcd31-616">Microsoft Evrensel Yazdırma artık bazı paketlerde kullanılabilir</span><span class="sxs-lookup"><span data-stu-id="fcd31-616">Microsoft Universal Print now available in some suites</span></span>

### <a name="categories"></a><span data-ttu-id="fcd31-617">Kategoriler</span><span class="sxs-lookup"><span data-stu-id="fcd31-617">Categories</span></span>

- <span data-ttu-id="fcd31-618">Tarih: 2021-03-33</span><span class="sxs-lookup"><span data-stu-id="fcd31-618">Date: 2021-03-33</span></span>
- <span data-ttu-id="fcd31-619">Özellikler</span><span class="sxs-lookup"><span data-stu-id="fcd31-619">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="fcd31-620">Özet</span><span class="sxs-lookup"><span data-stu-id="fcd31-620">Summary</span></span>

<span data-ttu-id="fcd31-621">Microsoft Evrensel Yazdırma, 1 Mart 2021 ' den bağımsız bir eklenti olarak, select Microsoft 365 paketleri ve tek başına eklenti olarak Transact tarafından kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-621">Microsoft Universal Print will be available to transact within select Microsoft 365 suites and as a standalone add-on from March 1, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcd31-622">Etkilenen hedef kitle</span><span class="sxs-lookup"><span data-stu-id="fcd31-622">Impacted audience</span></span>

<span data-ttu-id="fcd31-623">Tüm iş ortakları bulut çözümü sağlayıcısı (CSP) programı üzerinden deneyimidir</span><span class="sxs-lookup"><span data-stu-id="fcd31-623">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="fcd31-624">Ayrıntılar</span><span class="sxs-lookup"><span data-stu-id="fcd31-624">Details</span></span>

<span data-ttu-id="fcd31-625">[Evrensel Yazdırma](https://aka.ms/universalprint) , şirket içi yazdırma sunucuları gereksinimini ortadan kaldıran ve Windows cihazlarının Azure 'a kayıtlı yazıcılara yazdırmasını sağlayan bir Microsoft 365 yazdırma hizmetidir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-625">[Universal Print](https://aka.ms/universalprint) is a Microsoft 365 print service that removes the need for on-premises print servers, and enables Windows devices to print to Azure-registered printers.</span></span> <span data-ttu-id="fcd31-626">Bu, 1 Mart 2021 ' den itibaren Transact tarafından kullanılabilir olacaktır.</span><span class="sxs-lookup"><span data-stu-id="fcd31-626">It will be available to transact from March 1, 2021.</span></span>

<span data-ttu-id="fcd31-627">Çalışanlar, daha az yazdırma, kolay konum tabanlı yazıcı bulma ve öğrenme eğrisi olmadan sezgisel bir yazdırma deneyiminden yararlanır.</span><span class="sxs-lookup"><span data-stu-id="fcd31-627">Workers benefit from driverless printing, streamlined location-based printer discovery, and an intuitive printing experience with no learning curve.</span></span> <span data-ttu-id="fcd31-628">Azure Active Directory (Azure AD) 'ye katılmış olan cihazlar, güvenli bir şekilde yazdırmak için mevcut Azure AD kimlik bilgilerini kullanır.</span><span class="sxs-lookup"><span data-stu-id="fcd31-628">Devices that are joined to Azure Active Directory (Azure AD) use existing Azure AD credentials to print securely.</span></span> <span data-ttu-id="fcd31-629">Yöneticiler, Azure portal kullanarak yazdırmayı yönetir ve Evrensel Yazdırma için yerel destekle kolayca yazıcılara bağlanabilir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-629">Administrators manage printing by using the Azure portal, and can easily connect printers with native support for Universal Print.</span></span> <span data-ttu-id="fcd31-630">Evrensel Yazdırma, Evrensel Yazdırma Bağlayıcısı yazılımı kullanılarak uyumlu olmayan yazıcılarla dağıtılabilir.</span><span class="sxs-lookup"><span data-stu-id="fcd31-630">Universal Print can be deployed with non-compatible printers by using Universal Print connector software.</span></span>

<span data-ttu-id="fcd31-631">Evrensel Yazdırma, Windows E3, a3, E5 ve A5, ve Microsoft 365 BP, F3, E3, a3, E5 ve a5 ' a başlayacak şekilde geri doldurulacak.</span><span class="sxs-lookup"><span data-stu-id="fcd31-631">Universal Print will be backfilled at launch to Windows E3, A3, E5, and A5, and Microsoft 365 BP, F3, E3, A3, E5, and A5.</span></span>  

<span data-ttu-id="fcd31-632">**Teklif Ayrıntıları**</span><span class="sxs-lookup"><span data-stu-id="fcd31-632">**Offer details**</span></span>

<span data-ttu-id="fcd31-633">Teklif adının fiyat listesi önizlemeden biraz farklı olduğunu unutmayın.</span><span class="sxs-lookup"><span data-stu-id="fcd31-633">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="fcd31-634">Teklif adı</span><span class="sxs-lookup"><span data-stu-id="fcd31-634">Offer name</span></span> | <span data-ttu-id="fcd31-635">Teklif Kimliği</span><span class="sxs-lookup"><span data-stu-id="fcd31-635">Offer ID</span></span> | <span data-ttu-id="fcd31-636">Malzeme KIMLIĞI</span><span class="sxs-lookup"><span data-stu-id="fcd31-636">Material ID</span></span> |
| ------ |----------- |----------- |  
| <span data-ttu-id="fcd31-637">Evrensel yazdırma birimi eklentisi (500 iş)-Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="fcd31-637">Universal Print volume add-on (500 jobs) - Microsoft 365</span></span>  | <span data-ttu-id="fcd31-638">cb131356-45ee-4ae2-8537-873b706c8e75</span><span class="sxs-lookup"><span data-stu-id="fcd31-638">cb131356-45ee-4ae2-8537-873b706c8e75</span></span>     | <span data-ttu-id="fcd31-639">9 Bı-00004</span><span class="sxs-lookup"><span data-stu-id="fcd31-639">9BI-00004</span></span>   |
| <span data-ttu-id="fcd31-640">Fakülteler için Evrensel yazdırma birimi eklentisi (500 işleri)-Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="fcd31-640">Universal Print volume add-on (500 jobs) for faculty - Microsoft 365</span></span>   | <span data-ttu-id="fcd31-641">477bee81-9872-43d6-91d3-c72390bfcf49</span><span class="sxs-lookup"><span data-stu-id="fcd31-641">477bee81-9872-43d6-91d3-c72390bfcf49</span></span>   | <span data-ttu-id="fcd31-642">9BK-00004</span><span class="sxs-lookup"><span data-stu-id="fcd31-642">9BK-00004</span></span>   |
| <span data-ttu-id="fcd31-643">Evrensel yazdırma birimi eklentisi (500 iş)-Windows</span><span class="sxs-lookup"><span data-stu-id="fcd31-643">Universal Print volume add-on (500 jobs) - Windows</span></span>    | <span data-ttu-id="fcd31-644">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span><span class="sxs-lookup"><span data-stu-id="fcd31-644">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span></span>   | <span data-ttu-id="fcd31-645">9 Bı-00002</span><span class="sxs-lookup"><span data-stu-id="fcd31-645">9BI-00002</span></span>   |
| <span data-ttu-id="fcd31-646">Fakülte için Evrensel yazdırma birimi eklentisi (500 işleri)-Windows</span><span class="sxs-lookup"><span data-stu-id="fcd31-646">Universal Print volume add-on (500 jobs) for faculty - Windows</span></span>   |  <span data-ttu-id="fcd31-647">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span><span class="sxs-lookup"><span data-stu-id="fcd31-647">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span></span>  | <span data-ttu-id="fcd31-648">9BK-00002</span><span class="sxs-lookup"><span data-stu-id="fcd31-648">9BK-00002</span></span>   |

### <a name="next-steps"></a><span data-ttu-id="fcd31-649">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="fcd31-649">Next steps</span></span>

<span data-ttu-id="fcd31-650">Fiyat listesi ve [evrensel yazdırmaya genel bakış hakkında bilgi](/universal-print/fundamentals/universal-print-whatis)edinin.</span><span class="sxs-lookup"><span data-stu-id="fcd31-650">Familiarize yourself with the price list and the [Universal Print overview](/universal-print/fundamentals/universal-print-whatis).</span></span> <span data-ttu-id="fcd31-651">Bu bilgileri kuruluşunuzdaki ilgili tüm kişilerle paylaşabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fcd31-651">Share this information with all appropriate contacts in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="fcd31-652">Sorularınız mı var?</span><span class="sxs-lookup"><span data-stu-id="fcd31-652">Questions?</span></span>

<span data-ttu-id="fcd31-653">Bu tekliflerle ilgili herhangi bir soru için ilgili Yammer topluluklarınızı kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="fcd31-653">For any questions about these offers, check your relevant Yammer communities.</span></span>
