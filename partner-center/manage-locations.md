---
title: İş ortağı hesabınızdaki konumları yönetin
ms.topic: how-to
ms.date: 02/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Yeni bir konum ekleme ve bilgisayar, CSP iş, abonelik ve diğer işlemlerde MPN KIMLIĞI 'nin nasıl kullanıldığını öğrenin.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 41ffaeaf0fb46659142949872295523546bb91c1
ms.sourcegitcommit: 5768f10cd122a20fe3df3062ea34e7096d99f639
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/09/2021
ms.locfileid: "100005917"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="8152b-103">MPN hesap konumlarını yönetme ve konum ekleme (silme)</span><span class="sxs-lookup"><span data-stu-id="8152b-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="8152b-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="8152b-104">**Appropriate roles**</span></span>

- <span data-ttu-id="8152b-105">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="8152b-105">Global admin</span></span>
- <span data-ttu-id="8152b-106">Hesap yöneticisi</span><span class="sxs-lookup"><span data-stu-id="8152b-106">Account admin</span></span>

<span data-ttu-id="8152b-107">MPN KIMLIĞI konumu, şirketinizin her belirli bir konumunu tanımlar.</span><span class="sxs-lookup"><span data-stu-id="8152b-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="8152b-108">MPN KIMLIK konumunu kullanarak, uygulamaları, Transact bulut çözümü sağlayıcısı (CSP) işletme ve diğer iş işlemlerine, teşvik etmek için kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8152b-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="8152b-109">Genel MPN KIMLIĞI, destek istekleri gibi işlem olmayan etkinlikler için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="8152b-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="8152b-110">Tipik bir senaryo aşağıda verilmiştir:</span><span class="sxs-lookup"><span data-stu-id="8152b-110">The following is a typical scenario:</span></span>

<span data-ttu-id="8152b-111">Contoso, UK 'teki ortak genel hesabına (PGA) sahiptir.</span><span class="sxs-lookup"><span data-stu-id="8152b-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="8152b-112">Bu, kayıtlı yasal işletmektir ve tüm işlemsel olmayan işleri yönetmek için Global MPN KIMLIĞI kullanılır.</span><span class="sxs-lookup"><span data-stu-id="8152b-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="8152b-113">Contoso Ayrıca, UK, Fransa ve ABD 'de başka bir konumdaki yan kuruluşlar veya bölümler için Iş ortağı konum hesapları (PLA) ile eşdeğerdir.</span><span class="sxs-lookup"><span data-stu-id="8152b-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="8152b-114">MPN hesap yapısında, bu PLAs 'ler benzersiz konum MPN kimlikleri olarak gösterilir.</span><span class="sxs-lookup"><span data-stu-id="8152b-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="8152b-115">PLAs 'ler, CSP veya teşvikleri programları gibi işlem işleri için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="8152b-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="8152b-116">Ödemeler belirli konumlara bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="8152b-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="8152b-117">CSP kiracısı ve MPN konum KIMLIĞI arasında bir 1-1 ilişkisi vardır.</span><span class="sxs-lookup"><span data-stu-id="8152b-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="MPN konumlarının yapısı":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="8152b-119">CSP iş için yeni bir hesap eklemek için Önkoşullar</span><span class="sxs-lookup"><span data-stu-id="8152b-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="8152b-120">Yeni bir CSP iş hesabı eklemek için önkoşulları karşıladığından emin olarak başlayın.</span><span class="sxs-lookup"><span data-stu-id="8152b-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="8152b-121">CSP iş yapmak istediğiniz ülkede MPN KIMLIĞI 'ne sahip olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="8152b-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="8152b-122">Yeni bir MPN konumu oluşturmak için aşağıdaki "MPN konum Ekle" bölümünü okuyun.</span><span class="sxs-lookup"><span data-stu-id="8152b-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="8152b-123">Yeni bir CSP dolaylı satıcı kaydı oluşturmak için, [dolaylı sağlayıcılarla iş](indirect-reseller-tasks-in-partner-center.md#get-started) bölümünü okuyun</span><span class="sxs-lookup"><span data-stu-id="8152b-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="8152b-124">**Yeni** CSP hesabının **Yeni** kimlik bilgileriyle oturum açmayı unutmayın.</span><span class="sxs-lookup"><span data-stu-id="8152b-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="8152b-125">Mevcut kimlik bilgilerinizi, Iş Ortağı Merkezi zaten bir hesap varmış gibi tanıyacak şekilde kullanmayacaktır.</span><span class="sxs-lookup"><span data-stu-id="8152b-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="8152b-126">Microsoft Iş ortağı sözleşmesi 'Ni kabul edin ve hesabı etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="8152b-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="8152b-127">Doğrudan fatura ortağı olarak kaydolmak istiyorsanız, [doğrudan fatura ortakları Için gereksinimleri](direct-partner-new-requirements.md) okuyun</span><span class="sxs-lookup"><span data-stu-id="8152b-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-your-mpn-locations"></a><span data-ttu-id="8152b-128">MPN konumlarınızı görüntüleyin</span><span class="sxs-lookup"><span data-stu-id="8152b-128">View your MPN locations</span></span>

1. <span data-ttu-id="8152b-129">MPN hesabı kimlik bilgilerinizle Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard/home) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="8152b-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="8152b-130">(MPN kimlik bilgileriniz CSP kimlik bilgilerinizle farklı olabilir)</span><span class="sxs-lookup"><span data-stu-id="8152b-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="8152b-131">**Ayarlar** simgesinden **Hesap ayarları**, **kuruluş profili**, **yasal**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="8152b-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="8152b-132">**Iş ortağı** sekmesinde, GEÇIRILEN konumları PMC 'den düzelmenizi isteyen bir başlık hata iletisi bulunmadığını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="8152b-132">On the **Partner** tab verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span> <span data-ttu-id="8152b-133">Varsa, yönergeleri izleyin ve bu konumları onarın.</span><span class="sxs-lookup"><span data-stu-id="8152b-133">If there is, follow instructions and fix those locations.</span></span> 

3. <span data-ttu-id="8152b-134">Bir hata mesajı yoksa,  **Ayarlar**' dan  **Hesap ayarları**, **kuruluş profili**, **tanımlayıcılar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="8152b-134">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

4. <span data-ttu-id="8152b-135">"Location" türünde, bu CSP hesabının ülkesiyle eşleşen MPN KIMLIĞINI bulun ve bunu aşağıda aramak ve ilişkilendirilmesi için kullanmak üzere kullanın.</span><span class="sxs-lookup"><span data-stu-id="8152b-135">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to search below and complete association.</span></span>

5. <span data-ttu-id="8152b-136">Kullanmak istediğiniz CSP hesabıyla eşleşen MPN KIMLIĞI konumunu bulamazsanız yeni bir MPN KIMLIĞI oluşturacak yeni bir konum ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8152b-136">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location which will create a new MPN ID.</span></span> <span data-ttu-id="8152b-137">Aşağıda **BIR MPN konumu ekleme** bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="8152b-137">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="8152b-138">MPN konumu ekleme</span><span class="sxs-lookup"><span data-stu-id="8152b-138">Add an MPN location</span></span>

1. <span data-ttu-id="8152b-139">Iş Ortağı Merkezi 'nde MPN hesabını kullanarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="8152b-139">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="8152b-140">(MPN kimlik bilgileriniz CSP kimlik bilgilerinizle farklı olabilir).</span><span class="sxs-lookup"><span data-stu-id="8152b-140">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="8152b-141">MPN hesabının genel yönetici veya hesap yönetici ayrıcalıklarına sahip olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="8152b-141">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="8152b-142">**Ayarlar simgesinden** **Hesap ayarları** ' nı seçin ve ardından **kuruluş profili**' ni seçin.</span><span class="sxs-lookup"><span data-stu-id="8152b-142">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="8152b-143">**Yasal** ' ı seçin ve sonra iş **ortağı** sekmesinde **iş konumları** ' nı seçin ve **Konum Ekle** ' ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="8152b-143">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="8152b-144">Şirketinize eklemek istediğiniz konum için iş adı, adres ve ilgili kişi dahil olmak üzere gerekli ayrıntıları sağlayın.</span><span class="sxs-lookup"><span data-stu-id="8152b-144">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="8152b-145">**Konum Ekle**' ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="8152b-145">Click **Add location**.</span></span> <span data-ttu-id="8152b-146">Bu, yeni konum için CSP işlemleri ve teşvikleri için kullanabileceğiniz yeni bir MPN KIMLIĞI oluşturur.</span><span class="sxs-lookup"><span data-stu-id="8152b-146">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Yeni bir yasal iş ekleyin":::

> [!NOTE]
> <span data-ttu-id="8152b-148">Iş Ortağı Merkezi 'ne bir konum eklendikten sonra kaldıramazsınız.</span><span class="sxs-lookup"><span data-stu-id="8152b-148">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="8152b-149">Oturum açmak için doğru MPN KIMLIĞINI kullandıysanız, **MPN** 'Yi Iş Ortağı Merkezi 'nin sol menüsünde görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="8152b-149">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="8152b-150">Konum silme</span><span class="sxs-lookup"><span data-stu-id="8152b-150">Delete a location</span></span>

<span data-ttu-id="8152b-151">Hesabınızdan bir konum silmek için [Iş ortağı desteğine](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b)başvurmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="8152b-151">To delete a location from your account you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="8152b-152">Bu eylemin sahip olduğu etkiyi anladığınızdan emin olun.</span><span class="sxs-lookup"><span data-stu-id="8152b-152">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="8152b-153">Silinen konumlar alınamaz ve söz konusu MPN kimliğine bağlı olan herhangi bir şey artık şirketiniz için tanınmayacak veya etkin olmayacak.</span><span class="sxs-lookup"><span data-stu-id="8152b-153">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="8152b-154">Ortak genel hesap ülkesini değiştirin</span><span class="sxs-lookup"><span data-stu-id="8152b-154">Change country of Partner global account</span></span> 

1. <span data-ttu-id="8152b-155">Iş Ortağı Merkezi 'nde MPN hesabını kullanarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="8152b-155">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="8152b-156">(MPN kimlik bilgileriniz CSP kimlik bilgilerinizle farklı olabilir).</span><span class="sxs-lookup"><span data-stu-id="8152b-156">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="8152b-157">MPN hesabının genel yönetici veya hesap yönetici ayrıcalıklarına sahip olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="8152b-157">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="8152b-158">Iş **ortakları** sekmesinde **iş konumları** ' na gidin ve yasal varlığınız olarak istediğiniz konumun listelendiğinden emin olmak için konumların listesini kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="8152b-158">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="8152b-159">Konum eklemek için, **Konum Ekle**' ye tıklayın ve kullanıma hazır olarak, şirketinizde eklemek istediğiniz konum için iş adı, adres ve birincil kişi dahil olmak üzere gerekli ayrıntıları sağlayın.</span><span class="sxs-lookup"><span data-stu-id="8152b-159">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="8152b-160">**Ülke/bölge** açılır seçeneğinin yanındaki **ülkenizi değiştirin** ' i seçin ve adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="8152b-160">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Yasal iş profili verileri kullanıma hazır":::

5. <span data-ttu-id="8152b-162">**Kaydet**’e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="8152b-162">Click **Save**.</span></span>

6. <span data-ttu-id="8152b-163">MPN küresel hesap ülkesi, yeni yasal ülkeyle değiştirilecektir.</span><span class="sxs-lookup"><span data-stu-id="8152b-163">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="8152b-164">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="8152b-164">Next steps</span></span>

- <span data-ttu-id="8152b-165">[Doğrulama süreci](verification-responses.md)hakkında bilgi edinin.</span><span class="sxs-lookup"><span data-stu-id="8152b-165">Learn about the [verification process](verification-responses.md).</span></span>
