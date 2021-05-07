---
title: İş ortağı hesabınızdaki konumları yönetin
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Yeni bir konum ekleme ve bilgisayar, CSP iş, abonelik ve diğer işlemlerde MPN KIMLIĞI 'nin nasıl kullanıldığını öğrenin.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a2b4fa8b204b10d5d45c0e1409ab4bc463e272f
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702901"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="b348f-103">MPN hesap konumlarını yönetme ve konum ekleme (silme)</span><span class="sxs-lookup"><span data-stu-id="b348f-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="b348f-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="b348f-104">**Appropriate roles**</span></span>

- <span data-ttu-id="b348f-105">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="b348f-105">Global admin</span></span>
- <span data-ttu-id="b348f-106">Hesap yöneticisi</span><span class="sxs-lookup"><span data-stu-id="b348f-106">Account admin</span></span>

<span data-ttu-id="b348f-107">MPN KIMLIĞI konumu, şirketinizin her belirli bir konumunu tanımlar.</span><span class="sxs-lookup"><span data-stu-id="b348f-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="b348f-108">MPN KIMLIK konumunu kullanarak, uygulamaları, Transact bulut çözümü sağlayıcısı (CSP) işletme ve diğer iş işlemlerine, teşvik etmek için kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b348f-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="b348f-109">Genel MPN KIMLIĞI, destek istekleri gibi işlem olmayan etkinlikler için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="b348f-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="b348f-110">Aşağıdaki senaryo tipik bir davranıştır:</span><span class="sxs-lookup"><span data-stu-id="b348f-110">The following scenario is typical:</span></span>

<span data-ttu-id="b348f-111">Contoso, UK 'teki ortak genel hesabına (PGA) sahiptir.</span><span class="sxs-lookup"><span data-stu-id="b348f-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="b348f-112">PGA, kayıtlı yasal işletmektir ve tüm işlemsel olmayan işleri yönetmek için Global MPN KIMLIĞI kullanılır.</span><span class="sxs-lookup"><span data-stu-id="b348f-112">The PGA is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="b348f-113">Contoso Ayrıca, UK, Fransa ve ABD 'de başka bir konumdaki yan kuruluşlar veya bölümler için Iş ortağı konum hesapları (PLA) ile eşdeğerdir.</span><span class="sxs-lookup"><span data-stu-id="b348f-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="b348f-114">MPN hesap yapısında, bu PLAs 'ler benzersiz konum MPN kimlikleri olarak gösterilir.</span><span class="sxs-lookup"><span data-stu-id="b348f-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="b348f-115">PLAs 'ler, CSP veya teşvikleri programları gibi işlem işleri için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="b348f-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="b348f-116">Ödemeler belirli konumlara bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="b348f-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="b348f-117">CSP kiracısı ve MPN konum KIMLIĞI arasında bir 1-1 ilişkisi vardır.</span><span class="sxs-lookup"><span data-stu-id="b348f-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="MPN konumlarının yapısı":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="b348f-119">CSP iş için yeni bir hesap eklemek için Önkoşullar</span><span class="sxs-lookup"><span data-stu-id="b348f-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="b348f-120">Yeni bir CSP iş hesabı eklemek için önkoşulları karşıladığından emin olarak başlayın.</span><span class="sxs-lookup"><span data-stu-id="b348f-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="b348f-121">CSP iş yapmak istediğiniz ülkede MPN KIMLIĞI 'ne sahip olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="b348f-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="b348f-122">Yeni bir MPN konumu oluşturmak için aşağıdaki "MPN konum Ekle" bölümünü okuyun.</span><span class="sxs-lookup"><span data-stu-id="b348f-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="b348f-123">Yeni bir CSP dolaylı satıcı kaydı oluşturmak için, [dolaylı sağlayıcılarla iş](indirect-reseller-tasks-in-partner-center.md#get-started) bölümünü okuyun</span><span class="sxs-lookup"><span data-stu-id="b348f-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="b348f-124">**Yeni** CSP hesabının **Yeni** kimlik bilgileriyle oturum açmayı unutmayın.</span><span class="sxs-lookup"><span data-stu-id="b348f-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="b348f-125">Mevcut kimlik bilgilerinizi, Iş Ortağı Merkezi zaten bir hesap varmış gibi tanıyacak şekilde kullanmayacaktır.</span><span class="sxs-lookup"><span data-stu-id="b348f-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="b348f-126">Microsoft Iş ortağı sözleşmesi 'Ni kabul edin ve hesabı etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="b348f-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="b348f-127">Doğrudan fatura ortağı olarak kaydolmak istiyorsanız, [doğrudan fatura ortakları Için gereksinimleri](direct-partner-new-requirements.md) okuyun</span><span class="sxs-lookup"><span data-stu-id="b348f-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-and-update-your-mpn-locations"></a><span data-ttu-id="b348f-128">MPN konumlarınızı görüntüleyin ve güncelleştirin</span><span class="sxs-lookup"><span data-stu-id="b348f-128">View and update your MPN locations</span></span>

1. <span data-ttu-id="b348f-129">MPN hesabı kimlik bilgilerinizle Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard/home) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="b348f-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="b348f-130">(MPN kimlik bilgileriniz CSP kimlik bilgilerinizle farklı olabilir)</span><span class="sxs-lookup"><span data-stu-id="b348f-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="b348f-131">**Ayarlar** simgesinden **Hesap ayarları**, **kuruluş profili**, **yasal**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="b348f-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="b348f-132">**Iş ortağı** sekmesinde, GEÇIRILEN konumları PMC 'den düzelmenizi isteyen bir başlık hata iletisi bulunmadığını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="b348f-132">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="b348f-133">Konumlarınız PMC 'de doğru şekilde ayarlanmamışsa ve henüz BILGISAYARA geçirilmediyse, bu konumları güncelleştirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="b348f-133">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="Screencap, konumun nasıl güncelleştirilmesini gösterir.":::
 
4.  <span data-ttu-id="b348f-135">**PMC konumlarını gözden geçir** ekranında **Güncelleştir**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="b348f-135">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="b348f-136">Aşağıdaki alanları güncelleştirin:</span><span class="sxs-lookup"><span data-stu-id="b348f-136">Update the following fields:</span></span>

- <span data-ttu-id="b348f-137">**Ad alanı**: Şirket konumunun adının doğru olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="b348f-137">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="b348f-138">Yinelenen bir hata görüntüleniyorsa, örneğin contoso-contoso, Inc. arasında değişiklik yapmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="b348f-138">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="b348f-139">**Yasal varlık alanı**: konumun bağlı olduğu yasal varlığı seçtiğinizden emin olun</span><span class="sxs-lookup"><span data-stu-id="b348f-139">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="b348f-140">**Adres satırı 1 & 2 alan**: adresin doğru olduğundan emin olun</span><span class="sxs-lookup"><span data-stu-id="b348f-140">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="b348f-141">**Şehir & Eyalet/İl alanları**: City ve eyalet/eyalet arasındaki birleşimin doğru olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="b348f-141">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="b348f-142">Eyalet/bölge ' yi seçmek için açılan menünün uygulanacağı ve diğer ülkelerde alanın el ile eklenmesi gereken ülkeler vardır.</span><span class="sxs-lookup"><span data-stu-id="b348f-142">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="b348f-143">**ZIP/posta kodu alanı**: ZIP kodu alanının belirttiğiniz ülke, bölge, şehir veya adresle aynı olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="b348f-143">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="b348f-144">**Birincil iletişim bilgileri alanları**: ilk ve son ad alanlarının doldurulduğundan ve belirtilen e-posta adresinin kişisel bir e-posta adresi (örneğin,, @outlook.com @live.com vb.) olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="b348f-144">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="b348f-145">**Telefon numarası alanı**: telefon numarasının özel karakterler, boşluklar veya ülke kodu içermediğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="b348f-145">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="b348f-146">Telefon numarası alanına girilen değer her zaman en fazla 10 karakter içerir.</span><span class="sxs-lookup"><span data-stu-id="b348f-146">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="b348f-147">Bir hata mesajı yoksa,  **Ayarlar**' dan  **Hesap ayarları**, **kuruluş profili**, **tanımlayıcılar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="b348f-147">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="b348f-148">"Location" türünde, bu CSP hesabının ülkesiyle eşleşen MPN KIMLIĞINI bulun ve ilişkilendirmeyi gerçekleştirmek için onu kullanın.</span><span class="sxs-lookup"><span data-stu-id="b348f-148">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="b348f-149">Kullanmak istediğiniz CSP hesabıyla eşleşen MPN KIMLIĞI konumunu bulamazsanız yeni bir MPN KIMLIĞI oluşturacak yeni bir konum ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b348f-149">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="b348f-150">Aşağıda **BIR MPN konumu ekleme** bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="b348f-150">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="b348f-151">MPN konumu ekleme</span><span class="sxs-lookup"><span data-stu-id="b348f-151">Add an MPN location</span></span>

1. <span data-ttu-id="b348f-152">Iş Ortağı Merkezi 'nde MPN hesabını kullanarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="b348f-152">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="b348f-153">(MPN kimlik bilgileriniz CSP kimlik bilgilerinizle farklı olabilir).</span><span class="sxs-lookup"><span data-stu-id="b348f-153">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="b348f-154">MPN hesabının genel yönetici veya hesap yönetici ayrıcalıklarına sahip olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="b348f-154">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="b348f-155">**Ayarlar simgesinden** **Hesap ayarları** ' nı seçin ve ardından **kuruluş profili**' ni seçin.</span><span class="sxs-lookup"><span data-stu-id="b348f-155">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="b348f-156">**Yasal** ' ı seçin ve sonra iş **ortağı** sekmesinde **iş konumları** ' nı seçin ve **Konum Ekle** ' ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="b348f-156">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="b348f-157">Şirketinize eklemek istediğiniz konum için iş adı, adres ve ilgili kişi dahil olmak üzere gerekli ayrıntıları sağlayın.</span><span class="sxs-lookup"><span data-stu-id="b348f-157">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="b348f-158">**Konum Ekle**' ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="b348f-158">Click **Add location**.</span></span> <span data-ttu-id="b348f-159">Bu, yeni konum için CSP işlemleri ve teşvikleri için kullanabileceğiniz yeni bir MPN KIMLIĞI oluşturur.</span><span class="sxs-lookup"><span data-stu-id="b348f-159">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Yeni bir yasal iş ekleyin":::

> [!NOTE]
> <span data-ttu-id="b348f-161">Iş Ortağı Merkezi 'ne bir konum eklendikten sonra kaldıramazsınız.</span><span class="sxs-lookup"><span data-stu-id="b348f-161">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="b348f-162">Oturum açmak için doğru MPN KIMLIĞINI kullandıysanız, **MPN** 'Yi Iş Ortağı Merkezi 'nin sol menüsünde görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="b348f-162">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="add-the-registration-number-id"></a><span data-ttu-id="b348f-163">Kayıt numarası KIMLIĞINI ekleyin</span><span class="sxs-lookup"><span data-stu-id="b348f-163">Add the registration number ID</span></span>

<span data-ttu-id="b348f-164">Dolaylı bir Sağlayıcıysanız, doğrudan faturanız veya dolaylı satıcısıysanız ve aşağıdaki ülkelerde yeni veya mevcut müşterilerle iş yapıyorsanız, işletmeniz için kayıt KIMLIĞI numaraları sağlamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="b348f-164">If you are an Indirect provider, Direct bill partner, or Indirect reseller and you are doing business with new or existing customers in the following countries, you need to provide registration ID numbers for your business.</span></span> <span data-ttu-id="b348f-165">İş yapmakta olduğunuz ülke aşağıda listelenmiyorsa kayıt KIMLIĞI isteğe bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="b348f-165">If the country you are doing business in is not listed below, the registration ID is optional.</span></span>

- <span data-ttu-id="b348f-166">Ermenistan</span><span class="sxs-lookup"><span data-stu-id="b348f-166">Armenia</span></span> 
- <span data-ttu-id="b348f-167">Azerbaycan</span><span class="sxs-lookup"><span data-stu-id="b348f-167">Azerbaijan</span></span> 
- <span data-ttu-id="b348f-168">Belarus</span><span class="sxs-lookup"><span data-stu-id="b348f-168">Belarus</span></span> 
- <span data-ttu-id="b348f-169">Brezilya</span><span class="sxs-lookup"><span data-stu-id="b348f-169">Brazil</span></span> 
- <span data-ttu-id="b348f-170">Macaristan</span><span class="sxs-lookup"><span data-stu-id="b348f-170">Hungary</span></span> 
- <span data-ttu-id="b348f-171">Hindistan</span><span class="sxs-lookup"><span data-stu-id="b348f-171">India</span></span> 
- <span data-ttu-id="b348f-172">Irak</span><span class="sxs-lookup"><span data-stu-id="b348f-172">Iraq</span></span> 
- <span data-ttu-id="b348f-173">Kazakistan</span><span class="sxs-lookup"><span data-stu-id="b348f-173">Kazakhstan</span></span> 
- <span data-ttu-id="b348f-174">Kırgızistan</span><span class="sxs-lookup"><span data-stu-id="b348f-174">Kyrgyzstan</span></span> 
- <span data-ttu-id="b348f-175">Moldova</span><span class="sxs-lookup"><span data-stu-id="b348f-175">Moldova</span></span> 
- <span data-ttu-id="b348f-176">Myanmar</span><span class="sxs-lookup"><span data-stu-id="b348f-176">Myanmar</span></span> 
- <span data-ttu-id="b348f-177">Polonya</span><span class="sxs-lookup"><span data-stu-id="b348f-177">Poland</span></span> 
- <span data-ttu-id="b348f-178">Rusya</span><span class="sxs-lookup"><span data-stu-id="b348f-178">Russia</span></span> 
- <span data-ttu-id="b348f-179">Suudi Arabistan</span><span class="sxs-lookup"><span data-stu-id="b348f-179">Saudi Arabia</span></span> 
- <span data-ttu-id="b348f-180">Güney Afrika</span><span class="sxs-lookup"><span data-stu-id="b348f-180">South Africa</span></span> 
- <span data-ttu-id="b348f-181">Güney Sudan</span><span class="sxs-lookup"><span data-stu-id="b348f-181">South Sudan</span></span>  
- <span data-ttu-id="b348f-182">Tacikistan</span><span class="sxs-lookup"><span data-stu-id="b348f-182">Tajikistan</span></span> 
- <span data-ttu-id="b348f-183">Tayland</span><span class="sxs-lookup"><span data-stu-id="b348f-183">Thailand</span></span>
- <span data-ttu-id="b348f-184">Türkiye</span><span class="sxs-lookup"><span data-stu-id="b348f-184">Turkey</span></span> 
- <span data-ttu-id="b348f-185">Ukrayna</span><span class="sxs-lookup"><span data-stu-id="b348f-185">Ukraine</span></span> 
- <span data-ttu-id="b348f-186">Birleşik Arap Emirlikleri</span><span class="sxs-lookup"><span data-stu-id="b348f-186">United Arab Emirates</span></span> 
- <span data-ttu-id="b348f-187">Özbekistan</span><span class="sxs-lookup"><span data-stu-id="b348f-187">Uzbekistan</span></span> 
- <span data-ttu-id="b348f-188">Venezuela</span><span class="sxs-lookup"><span data-stu-id="b348f-188">Venezuela</span></span>
- <span data-ttu-id="b348f-189">Vietnam</span><span class="sxs-lookup"><span data-stu-id="b348f-189">Vietnam</span></span> 


<span data-ttu-id="b348f-190">Daha fazla bilgi için [kayıt kimliği numarası bilgilerini](reg-number-id.md) okuyun</span><span class="sxs-lookup"><span data-stu-id="b348f-190">For more information, read [Registration ID number information](reg-number-id.md)</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="b348f-191">Konum silme</span><span class="sxs-lookup"><span data-stu-id="b348f-191">Delete a location</span></span>

<span data-ttu-id="b348f-192">Hesabınızdan bir konum silmek için [Iş ortağı desteğine](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b)başvurmanız gerekecektir.</span><span class="sxs-lookup"><span data-stu-id="b348f-192">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="b348f-193">Bu eylemin sahip olduğu etkiyi anladığınızdan emin olun.</span><span class="sxs-lookup"><span data-stu-id="b348f-193">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="b348f-194">Silinen konumlar alınamaz ve söz konusu MPN kimliğine bağlı olan herhangi bir şey artık şirketiniz için tanınmayacak veya etkin olmayacak.</span><span class="sxs-lookup"><span data-stu-id="b348f-194">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="b348f-195">Ortak genel hesap ülkesini değiştirin</span><span class="sxs-lookup"><span data-stu-id="b348f-195">Change country of Partner global account</span></span> 

1. <span data-ttu-id="b348f-196">Iş Ortağı Merkezi 'nde MPN hesabını kullanarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="b348f-196">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="b348f-197">(MPN kimlik bilgileriniz CSP kimlik bilgilerinizle farklı olabilir).</span><span class="sxs-lookup"><span data-stu-id="b348f-197">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="b348f-198">MPN hesabının genel yönetici veya hesap yönetici ayrıcalıklarına sahip olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="b348f-198">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="b348f-199">Iş **ortakları** sekmesinde **iş konumları** ' na gidin ve yasal varlığınız olarak istediğiniz konumun listelendiğinden emin olmak için konumların listesini kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="b348f-199">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="b348f-200">Konum eklemek için, **Konum Ekle**' ye tıklayın ve kullanıma hazır olarak, şirketinizde eklemek istediğiniz konum için iş adı, adres ve birincil kişi dahil olmak üzere gerekli ayrıntıları sağlayın.</span><span class="sxs-lookup"><span data-stu-id="b348f-200">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="b348f-201">**Ülke/bölge** açılır seçeneğinin yanındaki **ülkenizi değiştirin** ' i seçin ve adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="b348f-201">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Yasal iş profili verileri kullanıma hazır":::

5. <span data-ttu-id="b348f-203">**Kaydet**’e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="b348f-203">Click **Save**.</span></span>

6. <span data-ttu-id="b348f-204">MPN küresel hesap ülkesi, yeni yasal ülkeyle değiştirilecektir.</span><span class="sxs-lookup"><span data-stu-id="b348f-204">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="b348f-205">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="b348f-205">Next steps</span></span>

- <span data-ttu-id="b348f-206">[Doğrulama süreci](verification-responses.md)hakkında bilgi edinin.</span><span class="sxs-lookup"><span data-stu-id="b348f-206">Learn about the [verification process](verification-responses.md).</span></span>
