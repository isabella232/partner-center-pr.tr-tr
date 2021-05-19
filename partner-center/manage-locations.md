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
ms.openlocfilehash: 13d6e7dc4722227035be2b24df48427f2008bb14
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151789"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="2ad45-103">MPN hesap konumlarını yönetme ve konum ekleme (silme)</span><span class="sxs-lookup"><span data-stu-id="2ad45-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="2ad45-104">**Uygun roller**: genel yönetici | Hesap Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="2ad45-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="2ad45-105">MPN KIMLIĞI konumu, şirketinizin her belirli bir konumunu tanımlar.</span><span class="sxs-lookup"><span data-stu-id="2ad45-105">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="2ad45-106">MPN KIMLIK konumunu kullanarak, uygulamaları, Transact bulut çözümü sağlayıcısı (CSP) işletme ve diğer iş işlemlerine, teşvik etmek için kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="2ad45-106">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="2ad45-107">Genel MPN KIMLIĞI, destek istekleri gibi işlem olmayan etkinlikler için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="2ad45-107">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="2ad45-108">Aşağıdaki senaryo tipik bir davranıştır:</span><span class="sxs-lookup"><span data-stu-id="2ad45-108">The following scenario is typical:</span></span>

<span data-ttu-id="2ad45-109">Contoso, UK 'teki ortak genel hesabına (PGA) sahiptir.</span><span class="sxs-lookup"><span data-stu-id="2ad45-109">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="2ad45-110">PGA, kayıtlı yasal işletmektir ve tüm hareketsel olmayan işleri yönetmek için genel MPN KIMLIĞI kullanılır.</span><span class="sxs-lookup"><span data-stu-id="2ad45-110">The PGA is their registered legal business, and its global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="2ad45-111">Contoso Ayrıca, UK, Fransa ve ABD 'de başka bir konumdaki yan kuruluşlar veya bölümler için Iş ortağı konum hesapları (PLA) ile eşdeğerdir.</span><span class="sxs-lookup"><span data-stu-id="2ad45-111">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="2ad45-112">MPN hesap yapısında, bu PLAs 'ler benzersiz konum MPN kimlikleri olarak gösterilir.</span><span class="sxs-lookup"><span data-stu-id="2ad45-112">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="2ad45-113">PLAs 'ler, CSP veya teşvikleri programları gibi işlem işleri için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="2ad45-113">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="2ad45-114">Ödemeler belirli konumlara bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="2ad45-114">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="2ad45-115">CSP kiracısı ve MPN konum KIMLIĞI arasında bir 1-1 ilişkisi vardır.</span><span class="sxs-lookup"><span data-stu-id="2ad45-115">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="MPN konumlarının yapısı":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="2ad45-117">CSP iş için yeni bir hesap eklemek için Önkoşullar</span><span class="sxs-lookup"><span data-stu-id="2ad45-117">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="2ad45-118">Yeni bir CSP iş hesabı eklemek için önkoşulları karşıladığından emin olarak başlayın.</span><span class="sxs-lookup"><span data-stu-id="2ad45-118">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="2ad45-119">CSP iş yapmak istediğiniz ülkede MPN KIMLIĞI 'ne sahip olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="2ad45-119">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="2ad45-120">Yeni bir MPN konumu oluşturmak için aşağıdaki "MPN konum Ekle" bölümünü okuyun.</span><span class="sxs-lookup"><span data-stu-id="2ad45-120">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="2ad45-121">Yeni bir kayıt CSP Indirect Reseller için Dolaylı [sağlayıcılarla çalışma makalesi](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="2ad45-121">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="2ad45-122">Yeni CSP hesabı için **yeni** kimlik bilgileriyle **oturum** açmayı unutmayın.</span><span class="sxs-lookup"><span data-stu-id="2ad45-122">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="2ad45-123">Mevcut kimlik bilgilerinizi, sizi zaten bir İş Ortağı Merkezi olarak tanıyacak şekilde kullanmayın.</span><span class="sxs-lookup"><span data-stu-id="2ad45-123">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="2ad45-124">Hesabı Microsoft İş Ortağı Sözleşmesi hesabı etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="2ad45-124">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="2ad45-125">Doğrudan Fatura iş ortağı olarak kaydolmak için, Doğrudan Fatura iş [ortakları için gereksinimler makaleyi okuyun](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="2ad45-125">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-and-update-your-mpn-locations"></a><span data-ttu-id="2ad45-126">MPN konumlarınızı görüntüleme ve güncelleştirme</span><span class="sxs-lookup"><span data-stu-id="2ad45-126">View and update your MPN locations</span></span>

1. <span data-ttu-id="2ad45-127">MPN hesabı İş Ortağı Merkezi [kimlik](https://partner.microsoft.com/dashboard/home) bilgilerinizle panoda oturum açın.</span><span class="sxs-lookup"><span data-stu-id="2ad45-127">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="2ad45-128">(MPN kimlik bilgileriniz CSP kimlik bilgilerinizden farklı olabilir)</span><span class="sxs-lookup"><span data-stu-id="2ad45-128">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="2ad45-129">Ayarlar **simgesinden** Hesap ayarları, **Kuruluş profili**, **Yasal'ı** **seçin.**</span><span class="sxs-lookup"><span data-stu-id="2ad45-129">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="2ad45-130">İş **Ortağı sekmesinde,** PMC'den geçirilen konumları düzeltmenizi isteyen bir başlık hata iletisi olmadığını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="2ad45-130">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="2ad45-131">Konumlarınız PMC'de doğru şekilde ayarlanmadıysa ve henüz PC'ye geçiş yapılmadıysa, bu konumları güncelleştirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="2ad45-131">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="Ekran kapsülde konumun nasıl güncelleştiril olduğu gösterilir.":::
 
4.  <span data-ttu-id="2ad45-133">**PMC konumlarını gözden geçir ekranında** Güncelleştir'i **seçin.**</span><span class="sxs-lookup"><span data-stu-id="2ad45-133">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="2ad45-134">Aşağıdaki alanları güncelleştirin:</span><span class="sxs-lookup"><span data-stu-id="2ad45-134">Update the following fields:</span></span>

- <span data-ttu-id="2ad45-135">**Ad alanı:** Şirket konumunun adının doğru olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="2ad45-135">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="2ad45-136">Yinelenen bir hata görüntülenirse, örneğin Contoso'dan Contoso, Inc.</span><span class="sxs-lookup"><span data-stu-id="2ad45-136">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="2ad45-137">**Yasal Varlık alanı:** Konumun bağlı olduğu yasal varlığı seçtiğinizden emin olun</span><span class="sxs-lookup"><span data-stu-id="2ad45-137">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="2ad45-138">**1. adres & 2 alanı içerir:** Adresin doğru olduğundan emin olun</span><span class="sxs-lookup"><span data-stu-id="2ad45-138">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="2ad45-139">**Şehir & Eyalet/İl alanları:** Şehir ile eyalet/il arasındaki birleşimin doğru olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="2ad45-139">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="2ad45-140">Eyalet/İl seçimi için açılan menenin geçerli olduğu ve diğer ülkelerde bu alanın el ile eklenmek zorunda olduğu ülkeler vardır.</span><span class="sxs-lookup"><span data-stu-id="2ad45-140">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="2ad45-141">**ZIP/posta kodu alanı**: ZIP kodu alanının belirttiğiniz ülke, bölge, şehir veya adresle aynı olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="2ad45-141">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="2ad45-142">**Birincil iletişim bilgileri alanları**: ilk ve son ad alanlarının doldurulduğundan ve belirtilen e-posta adresinin kişisel bir e-posta adresi (örneğin,, @outlook.com @live.com vb.) olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="2ad45-142">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="2ad45-143">**Telefon numarası alanı**: telefon numarasının özel karakterler, boşluklar veya ülke kodu içermediğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="2ad45-143">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="2ad45-144">Telefon numarası alanına girilen değer her zaman en fazla 10 karakter içerir.</span><span class="sxs-lookup"><span data-stu-id="2ad45-144">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="2ad45-145">Bir hata mesajı yoksa,  **Ayarlar**' dan  **Hesap ayarları**, **kuruluş profili**, **tanımlayıcılar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="2ad45-145">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="2ad45-146">"Location" türünde, bu CSP hesabının ülkesiyle eşleşen MPN KIMLIĞINI bulun ve ilişkilendirmeyi gerçekleştirmek için onu kullanın.</span><span class="sxs-lookup"><span data-stu-id="2ad45-146">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="2ad45-147">Kullanmak istediğiniz CSP hesabıyla eşleşen MPN KIMLIĞI konumunu bulamazsanız yeni bir MPN KIMLIĞI oluşturacak yeni bir konum ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="2ad45-147">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="2ad45-148">Aşağıda **BIR MPN konumu ekleme** bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="2ad45-148">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="2ad45-149">MPN konumu ekleme</span><span class="sxs-lookup"><span data-stu-id="2ad45-149">Add an MPN location</span></span>

1. <span data-ttu-id="2ad45-150">Iş Ortağı Merkezi 'nde MPN hesabını kullanarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="2ad45-150">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="2ad45-151">(MPN kimlik bilgileriniz CSP kimlik bilgilerinizle farklı olabilir.) MPN hesabının genel yönetici veya hesap yönetici ayrıcalıklarına sahip olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="2ad45-151">(Your MPN credentials may be different from your CSP credentials.) The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="2ad45-152">**Ayarlar simgesinden** **Hesap ayarları** ' nı seçin ve ardından **kuruluş profili**' ni seçin.</span><span class="sxs-lookup"><span data-stu-id="2ad45-152">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="2ad45-153">**Yasal** ' ı seçin ve sonra iş **ortağı** sekmesinde **iş konumları '** nı seçin ve **Konum Ekle** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="2ad45-153">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and select **Add a location.**</span></span>

3. <span data-ttu-id="2ad45-154">Şirketinize eklemek istediğiniz konum için iş adı, adres ve ilgili kişi dahil olmak üzere gerekli ayrıntıları sağlayın.</span><span class="sxs-lookup"><span data-stu-id="2ad45-154">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="2ad45-155">**Konum Ekle**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="2ad45-155">Select **Add location**.</span></span> <span data-ttu-id="2ad45-156">Bu, CSP işlemleri ve teşvikleri için kullanabileceğiniz yeni konum için yeni bir MPN KIMLIĞI oluşturur.</span><span class="sxs-lookup"><span data-stu-id="2ad45-156">This will create a new MPN ID for the new location that you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Yeni bir yasal iş ekleyin":::

> [!NOTE]
> <span data-ttu-id="2ad45-158">Iş Ortağı Merkezi 'ne bir konum eklendikten sonra kaldıramazsınız.</span><span class="sxs-lookup"><span data-stu-id="2ad45-158">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="2ad45-159">Oturum açmak için doğru MPN KIMLIĞINI kullandıysanız, **MPN** 'Yi Iş Ortağı Merkezi 'nin sol menüsünde görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="2ad45-159">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="add-the-registration-number-id"></a><span data-ttu-id="2ad45-160">Kayıt numarası KIMLIĞINI ekleyin</span><span class="sxs-lookup"><span data-stu-id="2ad45-160">Add the registration number ID</span></span>

<span data-ttu-id="2ad45-161">Dolaylı sağlayıcı, Doğrudan fatura iş ortağı veya Dolaylı kurumsal bayiysiniz ve aşağıdaki ülkelerdeki yeni veya mevcut müşterilerle iş yapıyorsanız işletmeniz için kayıt kimliği numaralarını sağlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="2ad45-161">If you are an Indirect provider, Direct bill partner, or Indirect reseller and you are doing business with new or existing customers in the following countries, you need to provide registration ID numbers for your business.</span></span> <span data-ttu-id="2ad45-162">İş yapmakta olduğu ülke aşağıda listelenmiyorsa kayıt kimliği isteğe bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="2ad45-162">If the country you are doing business in is not listed below, the registration ID is optional.</span></span>

- <span data-ttu-id="2ad45-163">Ermenistan</span><span class="sxs-lookup"><span data-stu-id="2ad45-163">Armenia</span></span> 
- <span data-ttu-id="2ad45-164">Azerbaycan</span><span class="sxs-lookup"><span data-stu-id="2ad45-164">Azerbaijan</span></span> 
- <span data-ttu-id="2ad45-165">Belarus</span><span class="sxs-lookup"><span data-stu-id="2ad45-165">Belarus</span></span> 
- <span data-ttu-id="2ad45-166">Brezilya</span><span class="sxs-lookup"><span data-stu-id="2ad45-166">Brazil</span></span> 
- <span data-ttu-id="2ad45-167">Macaristan</span><span class="sxs-lookup"><span data-stu-id="2ad45-167">Hungary</span></span> 
- <span data-ttu-id="2ad45-168">Hindistan</span><span class="sxs-lookup"><span data-stu-id="2ad45-168">India</span></span> 
- <span data-ttu-id="2ad45-169">Irak</span><span class="sxs-lookup"><span data-stu-id="2ad45-169">Iraq</span></span> 
- <span data-ttu-id="2ad45-170">Kazakistan</span><span class="sxs-lookup"><span data-stu-id="2ad45-170">Kazakhstan</span></span> 
- <span data-ttu-id="2ad45-171">Kırgızistan</span><span class="sxs-lookup"><span data-stu-id="2ad45-171">Kyrgyzstan</span></span> 
- <span data-ttu-id="2ad45-172">Moldova</span><span class="sxs-lookup"><span data-stu-id="2ad45-172">Moldova</span></span> 
- <span data-ttu-id="2ad45-173">Myanmar</span><span class="sxs-lookup"><span data-stu-id="2ad45-173">Myanmar</span></span> 
- <span data-ttu-id="2ad45-174">Polonya</span><span class="sxs-lookup"><span data-stu-id="2ad45-174">Poland</span></span> 
- <span data-ttu-id="2ad45-175">Rusya</span><span class="sxs-lookup"><span data-stu-id="2ad45-175">Russia</span></span> 
- <span data-ttu-id="2ad45-176">Suudi Arabistan</span><span class="sxs-lookup"><span data-stu-id="2ad45-176">Saudi Arabia</span></span> 
- <span data-ttu-id="2ad45-177">Güney Afrika</span><span class="sxs-lookup"><span data-stu-id="2ad45-177">South Africa</span></span> 
- <span data-ttu-id="2ad45-178">Güney Sudan</span><span class="sxs-lookup"><span data-stu-id="2ad45-178">South Sudan</span></span>  
- <span data-ttu-id="2ad45-179">Tacikistan</span><span class="sxs-lookup"><span data-stu-id="2ad45-179">Tajikistan</span></span> 
- <span data-ttu-id="2ad45-180">Tayland</span><span class="sxs-lookup"><span data-stu-id="2ad45-180">Thailand</span></span>
- <span data-ttu-id="2ad45-181">Türkiye</span><span class="sxs-lookup"><span data-stu-id="2ad45-181">Turkey</span></span> 
- <span data-ttu-id="2ad45-182">Ukrayna</span><span class="sxs-lookup"><span data-stu-id="2ad45-182">Ukraine</span></span> 
- <span data-ttu-id="2ad45-183">Birleşik Arap Emirlikleri</span><span class="sxs-lookup"><span data-stu-id="2ad45-183">United Arab Emirates</span></span> 
- <span data-ttu-id="2ad45-184">Özbekistan</span><span class="sxs-lookup"><span data-stu-id="2ad45-184">Uzbekistan</span></span> 
- <span data-ttu-id="2ad45-185">Venezuela</span><span class="sxs-lookup"><span data-stu-id="2ad45-185">Venezuela</span></span>
- <span data-ttu-id="2ad45-186">Vietnam</span><span class="sxs-lookup"><span data-stu-id="2ad45-186">Vietnam</span></span> 


<span data-ttu-id="2ad45-187">Daha fazla bilgi için Kayıt [Kimliği numarası bilgilerini okuyun](reg-number-id.md)</span><span class="sxs-lookup"><span data-stu-id="2ad45-187">For more information, read [Registration ID number information](reg-number-id.md)</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="2ad45-188">Konum silme</span><span class="sxs-lookup"><span data-stu-id="2ad45-188">Delete a location</span></span>

<span data-ttu-id="2ad45-189">Bir konumu hesabınızla silmek için İş Ortağı Desteği'ne [başvurabilirsiniz.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b)</span><span class="sxs-lookup"><span data-stu-id="2ad45-189">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="2ad45-190">Bu eylemin etkisini anlayasınız.</span><span class="sxs-lookup"><span data-stu-id="2ad45-190">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="2ad45-191">Silinen konumlar alınamaz ve bu MPN kimliğine bağlı herhangi bir şey artık tanınmaz veya şirket için etkin olmaz.</span><span class="sxs-lookup"><span data-stu-id="2ad45-191">Deleted locations cannot be retrieved and anything tied to that specific MPN ID will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="2ad45-192">İş ortağı genel hesabının ülkesini değiştirme</span><span class="sxs-lookup"><span data-stu-id="2ad45-192">Change country of Partner global account</span></span> 

1. <span data-ttu-id="2ad45-193">MpN hesabını kullanarak oturum açın ve İş Ortağı Merkezi.</span><span class="sxs-lookup"><span data-stu-id="2ad45-193">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="2ad45-194">(MPN kimlik bilgileriniz CSP kimlik bilgilerinizden farklı olabilir.) MPN hesabının Genel Yönetici veya Hesap Yöneticisi ayrıcalıkları olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="2ad45-194">(Your MPN credentials may be different from your CSP credentials.) The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="2ad45-195">İş **Ortağı** sekmesinde İş **konumları'ne gidin** ve konum listesini kontrol edin ve yasal varlığınız olarak istediğiniz konumun listelenmiş olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="2ad45-195">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="2ad45-196">Konum eklemek için Konum ekle'ye tıklayın ve iş adı, adres ve şirket için eklemek istediğiniz konumun birincil ilgili kişisi gibi gerekli ayrıntıları girin.</span><span class="sxs-lookup"><span data-stu-id="2ad45-196">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="2ad45-197">**Ülke/bölge açılan** listesinin **yanındaki Ülkenizi** değiştir'i seçin ve adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="2ad45-197">Select **Change your country** next to the **Country/region** drop-down list and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Yasal iş profili verileri çıkar":::

5. <span data-ttu-id="2ad45-199">**Kaydet**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="2ad45-199">Select **Save**.</span></span>

6. <span data-ttu-id="2ad45-200">MPN genel hesap ülkesi, yeni yasal ülke olarak değiştirilir.</span><span class="sxs-lookup"><span data-stu-id="2ad45-200">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="2ad45-201">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="2ad45-201">Next steps</span></span>

- <span data-ttu-id="2ad45-202">Doğrulama işlemi hakkında [bilgi edinin.](verification-responses.md)</span><span class="sxs-lookup"><span data-stu-id="2ad45-202">Learn about the [verification process](verification-responses.md).</span></span>
