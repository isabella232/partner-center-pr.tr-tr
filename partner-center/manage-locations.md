---
title: İş ortağı hesabınızla konumları yönetme
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Teşvik programlarında, CSP işlerde, aboneliklerde ve diğer işlemlerde yeni konum ve konum MPN kimliğinin nasıl kullanılabı hakkında bilgi edinin.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3d30f250d6635758f3bef8e06c6f57ba0a0be744
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276833"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="85505-103">MPN hesap konumlarınızı yönetme ve konum ekleme (silme)</span><span class="sxs-lookup"><span data-stu-id="85505-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="85505-104">**Uygun roller:** Genel yönetici | Hesap yöneticisi</span><span class="sxs-lookup"><span data-stu-id="85505-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="85505-105">Konum MPN Kimliği, şirketinizin belirli her konumunu tanımlar.</span><span class="sxs-lookup"><span data-stu-id="85505-105">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="85505-106">Teşvik programlarına kaydolmak, iş (CSP) ve diğer iş Bulut Çözümü Sağlayıcısı için konum MPN Kimliğini kullanırsiniz.</span><span class="sxs-lookup"><span data-stu-id="85505-106">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="85505-107">Genel MPN Kimliği, destek istekleri gibi işlem dışı etkinlikler için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="85505-107">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="85505-108">Aşağıdaki senaryo tipiktir:</span><span class="sxs-lookup"><span data-stu-id="85505-108">The following scenario is typical:</span></span>

<span data-ttu-id="85505-109">Contoso'da İş Ortağı genel hesabı (PGA) var.</span><span class="sxs-lookup"><span data-stu-id="85505-109">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="85505-110">PGA, kayıtlı yasal işletmedir ve genel MPN kimliği tüm işlem dışı işletmeleri yönetmek için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="85505-110">The PGA is their registered legal business, and its global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="85505-111">Contoso ayrıca Birleşik Krallık, Fransa ve ABD'deki başka bir konumdaki yan kuruluş veya bölümlere eşdeğer İş Ortağı konum hesaplarına (PLA) sahiptir.</span><span class="sxs-lookup"><span data-stu-id="85505-111">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="85505-112">MPN Hesabı yapısında, bu PLA'lar benzersiz konum MPN kimlikleri olarak temsil edildi.</span><span class="sxs-lookup"><span data-stu-id="85505-112">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="85505-113">PLA'lar CSP veya teşvik programları gibi işlem işletmeleri için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="85505-113">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="85505-114">Ödemeler belirli konumlara bağlanır.</span><span class="sxs-lookup"><span data-stu-id="85505-114">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="85505-115">CSP kiracısı ile MPN konum kimliği arasında 1-1 ilişkisi vardır.</span><span class="sxs-lookup"><span data-stu-id="85505-115">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="MPN konumlarının yapısı.":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="85505-117">CSP işletmesi için yeni bir hesap eklemek için önkoşullar</span><span class="sxs-lookup"><span data-stu-id="85505-117">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="85505-118">Yeni bir CSP iş hesabı eklemek için önkoşulları yerine getirmenize yardımcı olun.</span><span class="sxs-lookup"><span data-stu-id="85505-118">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="85505-119">CSP iş yapmak istediğiniz ülkede bir konum MPN Kimliğine sahipsiniz.</span><span class="sxs-lookup"><span data-stu-id="85505-119">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="85505-120">Yeni bir MPN konumu oluşturmak için aşağıdaki "MPN konumu ekleme" makalesi'ne bakın.</span><span class="sxs-lookup"><span data-stu-id="85505-120">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="85505-121">Yeni bir kayıt CSP Indirect Reseller için Dolaylı [sağlayıcılarla çalışma makalesi](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="85505-121">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="85505-122">Yeni CSP hesabı için **yeni** kimlik bilgileriyle **oturum** açmayı unutmayın.</span><span class="sxs-lookup"><span data-stu-id="85505-122">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="85505-123">Mevcut kimlik bilgilerinizi, sizi zaten bir İş Ortağı Merkezi olarak tanıyacak şekilde kullanmayın.</span><span class="sxs-lookup"><span data-stu-id="85505-123">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="85505-124">Hesabı Microsoft İş Ortağı Sözleşmesi hesabı etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="85505-124">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="85505-125">Doğrudan Fatura iş ortağı olarak kaydolmak için, Doğrudan Fatura iş [ortakları için gereksinimler makaleyi okuyun](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="85505-125">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-and-update-your-mpn-locations"></a><span data-ttu-id="85505-126">MPN konumlarınızı görüntüleme ve güncelleştirme</span><span class="sxs-lookup"><span data-stu-id="85505-126">View and update your MPN locations</span></span>

1. <span data-ttu-id="85505-127">MPN hesabı İş Ortağı Merkezi [kimlik](https://partner.microsoft.com/dashboard/home) bilgilerinizle panoda oturum açın.</span><span class="sxs-lookup"><span data-stu-id="85505-127">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="85505-128">(MPN kimlik bilgileriniz CSP kimlik bilgilerinizden farklı olabilir)</span><span class="sxs-lookup"><span data-stu-id="85505-128">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="85505-129">Ayarlar **simgesinden** Hesap ayarları, **Kuruluş profili**, **Yasal'ı** **seçin.**</span><span class="sxs-lookup"><span data-stu-id="85505-129">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="85505-130">İş **Ortağı sekmesinde,** PMC'den geçirilen konumları düzeltmenizi isteyen bir başlık hata iletisi olmadığını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="85505-130">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="85505-131">Konumlarınız PMC'de doğru şekilde ayarlanmadıysa ve henüz PC'ye geçiş yapılmadıysa, bu konumları güncelleştirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="85505-131">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="Ekran kapsülde konumun nasıl güncelleştiril olduğu gösterilir.":::
 
4.  <span data-ttu-id="85505-133">**PMC konumlarını gözden geçir ekranında** Güncelleştir'i **seçin.**</span><span class="sxs-lookup"><span data-stu-id="85505-133">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="85505-134">Aşağıdaki alanları güncelleştirin:</span><span class="sxs-lookup"><span data-stu-id="85505-134">Update the following fields:</span></span>

- <span data-ttu-id="85505-135">**Ad alanı:** Şirket konumunun adının doğru olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="85505-135">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="85505-136">Yinelenen bir hata görüntülenirse, örneğin Contoso'dan Contoso, Inc.</span><span class="sxs-lookup"><span data-stu-id="85505-136">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="85505-137">**Yasal Varlık alanı:** Konumun bağlı olduğu yasal varlığı seçtiğinizden emin olun</span><span class="sxs-lookup"><span data-stu-id="85505-137">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="85505-138">**1. adres & 2 alanı içerir:** Adresin doğru olduğundan emin olun</span><span class="sxs-lookup"><span data-stu-id="85505-138">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="85505-139">**Şehir & Eyalet/İl alanları:** Şehir ile eyalet/il arasındaki birleşimin doğru olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="85505-139">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="85505-140">Eyalet/İl seçimi için açılan menenin geçerli olduğu ve diğer ülkelerde bu alanın el ile eklenmek zorunda olduğu ülkeler vardır.</span><span class="sxs-lookup"><span data-stu-id="85505-140">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="85505-141">**ZIP/ Posta kodu alanı:** Posta Kodu alanında belirtilen Ülke, Bölge, Şehir veya Adres ile eş olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="85505-141">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="85505-142">**Birincil iletişim bilgileri alanları:** Ad ve soyadı alanlarının doldurul olduğundan ve belirtilen e-posta adresinin kişisel bir adres (örneğin, @outlook.com , vb.) değil iş e-posta adresi @live.com olduğundan emin olun</span><span class="sxs-lookup"><span data-stu-id="85505-142">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="85505-143">**Telefon numarası alanı:** Telefon numarası'nın özel karakterler, boşluklar veya ülke kodu içermeyerin.</span><span class="sxs-lookup"><span data-stu-id="85505-143">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="85505-144">Telefon Numarası alanına girilen değer her zaman en fazla 10 karakter içerir.</span><span class="sxs-lookup"><span data-stu-id="85505-144">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="85505-145">Hata iletisi yoksa Ayarlar'dan Hesap **Ayarları,** Kuruluş profili **,** **Tanımlayıcılar'ı** **seçin.**</span><span class="sxs-lookup"><span data-stu-id="85505-145">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="85505-146">Bu CSP hesabının ülkesiyle eşleşen "Konum" Türüne sahip MPN Kimliğini bulun ve ilişkilendirmeyi tamamlamak için kullanın.</span><span class="sxs-lookup"><span data-stu-id="85505-146">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="85505-147">Kullanmak istediğiniz CSP hesabıyla eşleşen konum MPN Kimliğini bulamazsanız, yeni bir konum ekleyebilir ve bu da yeni bir MPN kimliği oluşturabilir.</span><span class="sxs-lookup"><span data-stu-id="85505-147">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="85505-148">Aşağıdaki **MPN konumu eklemeye** bakın.</span><span class="sxs-lookup"><span data-stu-id="85505-148">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="85505-149">MPN konumu ekleme</span><span class="sxs-lookup"><span data-stu-id="85505-149">Add an MPN location</span></span>

1. <span data-ttu-id="85505-150">MpN hesabını kullanarak oturum açın ve İş Ortağı Merkezi.</span><span class="sxs-lookup"><span data-stu-id="85505-150">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="85505-151">(MPN kimlik bilgileriniz CSP kimlik bilgilerinizden farklı olabilir.) MPN hesabının Genel Yönetici veya Hesap Yöneticisi ayrıcalıkları olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="85505-151">(Your MPN credentials may be different from your CSP credentials.) The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="85505-152">Ayarlar **simgesinden Hesap** **ayarları'nın ve ardından Kuruluş** **profili'nin seçin.**</span><span class="sxs-lookup"><span data-stu-id="85505-152">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="85505-153">**Yasal'ı** seçin ve ardından **İş Ortağı** sekmesinde İş **konumları'nın ardından Konum** **ekle'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="85505-153">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and select **Add a location.**</span></span>

3. <span data-ttu-id="85505-154">Şirketinize eklemek istediğiniz konum için iş adı, adres ve iletişim gibi gerekli ayrıntıları girin.</span><span class="sxs-lookup"><span data-stu-id="85505-154">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="85505-155">Konum **ekle'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="85505-155">Select **Add location**.</span></span> <span data-ttu-id="85505-156">Bu, CSP işlemleri ve teşvikleri için kullanabileceğiniz yeni konum için yeni bir MPN kimliği oluşturacak.</span><span class="sxs-lookup"><span data-stu-id="85505-156">This will create a new MPN ID for the new location that you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Yeni bir yasal işletme ekleyin.":::

> [!NOTE]
> <span data-ttu-id="85505-158">Bir konum İş Ortağı Merkezi kaldıramazsiniz.</span><span class="sxs-lookup"><span data-stu-id="85505-158">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="85505-159">Oturum açma için **doğru MPN** kimliğini kullandıysanız İş Ortağı Merkezi menüsünde MPN'i görünür.</span><span class="sxs-lookup"><span data-stu-id="85505-159">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="add-the-registration-number-id"></a><span data-ttu-id="85505-160">Kayıt numarası kimliğini ekleme</span><span class="sxs-lookup"><span data-stu-id="85505-160">Add the registration number ID</span></span>

<span data-ttu-id="85505-161">Dolaylı sağlayıcı, Doğrudan fatura iş ortağı veya Dolaylı kurumsal bayiysiniz ve aşağıdaki ülkelerdeki yeni veya mevcut müşterilerle iş yapıyorsanız işletmeniz için kayıt kimliği numaralarını sağlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="85505-161">If you are an Indirect provider, Direct bill partner, or Indirect reseller and you are doing business with new or existing customers in the following countries, you need to provide registration ID numbers for your business.</span></span> <span data-ttu-id="85505-162">İş yapmakta olduğunuz ülke aşağıda listelenmiyorsa kayıt kimliği isteğe bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="85505-162">If the country you are doing business in is not listed below, the registration ID is optional.</span></span>

- <span data-ttu-id="85505-163">Ermenistan</span><span class="sxs-lookup"><span data-stu-id="85505-163">Armenia</span></span> 
- <span data-ttu-id="85505-164">Azerbaycan</span><span class="sxs-lookup"><span data-stu-id="85505-164">Azerbaijan</span></span> 
- <span data-ttu-id="85505-165">Belarus</span><span class="sxs-lookup"><span data-stu-id="85505-165">Belarus</span></span> 
- <span data-ttu-id="85505-166">Brezilya</span><span class="sxs-lookup"><span data-stu-id="85505-166">Brazil</span></span> 
- <span data-ttu-id="85505-167">Macaristan</span><span class="sxs-lookup"><span data-stu-id="85505-167">Hungary</span></span> 
- <span data-ttu-id="85505-168">Hindistan</span><span class="sxs-lookup"><span data-stu-id="85505-168">India</span></span> 
- <span data-ttu-id="85505-169">Irak</span><span class="sxs-lookup"><span data-stu-id="85505-169">Iraq</span></span> 
- <span data-ttu-id="85505-170">Kazakistan</span><span class="sxs-lookup"><span data-stu-id="85505-170">Kazakhstan</span></span> 
- <span data-ttu-id="85505-171">Kırgızistan</span><span class="sxs-lookup"><span data-stu-id="85505-171">Kyrgyzstan</span></span> 
- <span data-ttu-id="85505-172">Moldova</span><span class="sxs-lookup"><span data-stu-id="85505-172">Moldova</span></span> 
- <span data-ttu-id="85505-173">Myanmar</span><span class="sxs-lookup"><span data-stu-id="85505-173">Myanmar</span></span> 
- <span data-ttu-id="85505-174">Polonya</span><span class="sxs-lookup"><span data-stu-id="85505-174">Poland</span></span> 
- <span data-ttu-id="85505-175">Rusya</span><span class="sxs-lookup"><span data-stu-id="85505-175">Russia</span></span> 
- <span data-ttu-id="85505-176">Suudi Arabistan</span><span class="sxs-lookup"><span data-stu-id="85505-176">Saudi Arabia</span></span> 
- <span data-ttu-id="85505-177">Güney Afrika</span><span class="sxs-lookup"><span data-stu-id="85505-177">South Africa</span></span> 
- <span data-ttu-id="85505-178">Güney Sudan</span><span class="sxs-lookup"><span data-stu-id="85505-178">South Sudan</span></span>  
- <span data-ttu-id="85505-179">Tacikistan</span><span class="sxs-lookup"><span data-stu-id="85505-179">Tajikistan</span></span> 
- <span data-ttu-id="85505-180">Tayland</span><span class="sxs-lookup"><span data-stu-id="85505-180">Thailand</span></span>
- <span data-ttu-id="85505-181">Türkiye</span><span class="sxs-lookup"><span data-stu-id="85505-181">Turkey</span></span> 
- <span data-ttu-id="85505-182">Ukrayna</span><span class="sxs-lookup"><span data-stu-id="85505-182">Ukraine</span></span> 
- <span data-ttu-id="85505-183">Birleşik Arap Emirlikleri</span><span class="sxs-lookup"><span data-stu-id="85505-183">United Arab Emirates</span></span> 
- <span data-ttu-id="85505-184">Özbekistan</span><span class="sxs-lookup"><span data-stu-id="85505-184">Uzbekistan</span></span> 
- <span data-ttu-id="85505-185">Venezuela</span><span class="sxs-lookup"><span data-stu-id="85505-185">Venezuela</span></span>
- <span data-ttu-id="85505-186">Vietnam</span><span class="sxs-lookup"><span data-stu-id="85505-186">Vietnam</span></span> 


<span data-ttu-id="85505-187">Daha fazla bilgi için Kayıt [Kimliği numarası bilgilerini okuyun](reg-number-id.md)</span><span class="sxs-lookup"><span data-stu-id="85505-187">For more information, read [Registration ID number information](reg-number-id.md)</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="85505-188">Konum silme</span><span class="sxs-lookup"><span data-stu-id="85505-188">Delete a location</span></span>

<span data-ttu-id="85505-189">Bir konumu hesabınızla silmek için İş Ortağı Desteği'ne [başvurabilirsiniz.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b)</span><span class="sxs-lookup"><span data-stu-id="85505-189">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="85505-190">Bu eylemin etkisini anlayasınız.</span><span class="sxs-lookup"><span data-stu-id="85505-190">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="85505-191">Silinen konumlar alınamaz ve bu MPN kimliğine bağlı herhangi bir şey artık tanınmaz veya şirket için etkin olmaz.</span><span class="sxs-lookup"><span data-stu-id="85505-191">Deleted locations cannot be retrieved and anything tied to that specific MPN ID will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="85505-192">İş ortağı genel hesabının ülkesini değiştirme</span><span class="sxs-lookup"><span data-stu-id="85505-192">Change country of Partner global account</span></span> 

1. <span data-ttu-id="85505-193">MpN hesabını kullanarak oturum açın ve İş Ortağı Merkezi.</span><span class="sxs-lookup"><span data-stu-id="85505-193">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="85505-194">(MPN kimlik bilgileriniz CSP kimlik bilgilerinizden farklı olabilir.) MPN hesabının Genel Yönetici veya Hesap Yöneticisi ayrıcalıkları olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="85505-194">(Your MPN credentials may be different from your CSP credentials.) The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="85505-195">İş **Ortağı** sekmesinde İş **konumları'ne gidin** ve konum listesini kontrol edin ve yasal varlığınız olarak istediğiniz konumun listelenmiş olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="85505-195">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="85505-196">Konum eklemek için Konum ekle'ye tıklayın ve iş adı, adres ve şirket için eklemek istediğiniz konumun birincil ilgili kişisi gibi gerekli ayrıntıları girin.</span><span class="sxs-lookup"><span data-stu-id="85505-196">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="85505-197">**Ülke/bölge açılan** listesinin **yanındaki Ülkenizi** değiştir'i seçin ve adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="85505-197">Select **Change your country** next to the **Country/region** drop-down list and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Yasal iş profili verileri çıkar.":::

5. <span data-ttu-id="85505-199">**Kaydet**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="85505-199">Select **Save**.</span></span>

6. <span data-ttu-id="85505-200">MPN genel hesap ülkesi, yeni yasal ülke olarak değiştirilir.</span><span class="sxs-lookup"><span data-stu-id="85505-200">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="85505-201">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="85505-201">Next steps</span></span>

- <span data-ttu-id="85505-202">Doğrulama işlemi hakkında [bilgi edinin.](verification-responses.md)</span><span class="sxs-lookup"><span data-stu-id="85505-202">Learn about the [verification process](verification-responses.md).</span></span>
