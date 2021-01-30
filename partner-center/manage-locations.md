---
title: İş ortağı hesabınızdaki konumları yönetin
ms.topic: how-to
ms.date: 01/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Yeni bir konum ekleme ve bilgisayar, CSP iş, abonelik ve diğer işlemlerde MPN KIMLIĞI 'nin nasıl kullanıldığını öğrenin.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 21d82fc3ec4470d4941d3ca7436089d3e892439e
ms.sourcegitcommit: 81017727107a907bf1f3246097b51667d7c5fb18
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/30/2021
ms.locfileid: "99098899"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="0413d-103">MPN hesap konumlarını yönetin ve yeni bir konum ekleyin</span><span class="sxs-lookup"><span data-stu-id="0413d-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="0413d-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="0413d-104">**Appropriate roles**</span></span>

- <span data-ttu-id="0413d-105">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="0413d-105">Global admin</span></span>
- <span data-ttu-id="0413d-106">Hesap yöneticisi</span><span class="sxs-lookup"><span data-stu-id="0413d-106">Account admin</span></span>

<span data-ttu-id="0413d-107">MPN KIMLIĞI konumu, şirketinizin her belirli bir konumunu tanımlar.</span><span class="sxs-lookup"><span data-stu-id="0413d-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="0413d-108">MPN KIMLIK konumunu kullanarak, uygulamaları, Transact bulut çözümü sağlayıcısı (CSP) işletme ve diğer iş işlemlerine, teşvik etmek için kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0413d-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="0413d-109">Genel MPN KIMLIĞI, destek istekleri gibi işlem olmayan etkinlikler için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="0413d-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="0413d-110">Tipik bir senaryo aşağıda verilmiştir:</span><span class="sxs-lookup"><span data-stu-id="0413d-110">The following is a typical scenario:</span></span>

<span data-ttu-id="0413d-111">Contoso, UK 'teki ortak genel hesabına (PGA) sahiptir.</span><span class="sxs-lookup"><span data-stu-id="0413d-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="0413d-112">Bu, kayıtlı yasal işletmektir ve tüm işlemsel olmayan işleri yönetmek için Global MPN KIMLIĞI kullanılır.</span><span class="sxs-lookup"><span data-stu-id="0413d-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="0413d-113">Contoso Ayrıca, UK, Fransa ve ABD 'de başka bir konumdaki yan kuruluşlar veya bölümler için Iş ortağı konum hesapları (PLA) ile eşdeğerdir.</span><span class="sxs-lookup"><span data-stu-id="0413d-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="0413d-114">MPN hesap yapısında, bu PLAs 'ler benzersiz konum MPN kimlikleri olarak gösterilir.</span><span class="sxs-lookup"><span data-stu-id="0413d-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="0413d-115">PLAs 'ler, CSP veya teşvikleri programları gibi işlem işleri için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="0413d-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="0413d-116">Ödemeler belirli konumlara bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="0413d-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="0413d-117">CSP kiracısı ve MPN konum KIMLIĞI arasında bir 1-1 ilişkisi vardır.</span><span class="sxs-lookup"><span data-stu-id="0413d-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="MPN konumlarının yapısı":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="0413d-119">CSP iş için yeni bir hesap eklemek için Önkoşullar</span><span class="sxs-lookup"><span data-stu-id="0413d-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="0413d-120">Yeni bir CSP iş hesabı eklemek için önkoşulları karşıladığından emin olarak başlayın.</span><span class="sxs-lookup"><span data-stu-id="0413d-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="0413d-121">CSP iş yapmak istediğiniz ülkede MPN KIMLIĞI 'ne sahip olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="0413d-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="0413d-122">Yeni bir MPN konumu oluşturmak için aşağıdaki "MPN konum Ekle" bölümünü okuyun.</span><span class="sxs-lookup"><span data-stu-id="0413d-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="0413d-123">Yeni bir CSP dolaylı satıcı kaydı oluşturmak için, [dolaylı sağlayıcılarla iş](indirect-reseller-tasks-in-partner-center.md#get-started) bölümünü okuyun</span><span class="sxs-lookup"><span data-stu-id="0413d-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="0413d-124">**Yeni** CSP hesabının **Yeni** kimlik bilgileriyle oturum açmayı unutmayın.</span><span class="sxs-lookup"><span data-stu-id="0413d-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="0413d-125">Mevcut kimlik bilgilerinizi, Iş Ortağı Merkezi zaten bir hesap varmış gibi tanıyacak şekilde kullanmayacaktır.</span><span class="sxs-lookup"><span data-stu-id="0413d-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="0413d-126">Microsoft Iş ortağı sözleşmesi 'Ni kabul edin ve hesabı etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="0413d-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="view-your-mpn-locations"></a><span data-ttu-id="0413d-127">MPN konumlarınızı görüntüleyin</span><span class="sxs-lookup"><span data-stu-id="0413d-127">View your MPN locations</span></span>

1. <span data-ttu-id="0413d-128">MPN hesabı kimlik bilgilerinizle Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard/home) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="0413d-128">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="0413d-129">(MPN kimlik bilgileriniz CSP kimlik bilgilerinizle farklı olabilir)</span><span class="sxs-lookup"><span data-stu-id="0413d-129">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="0413d-130">**Ayarlar** simgesinden **Hesap ayarları**, **kuruluş profili**, **yasal**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="0413d-130">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="0413d-131">**Iş ortağı** sekmesinde, GEÇIRILEN konumları PMC 'den düzelmenizi isteyen bir başlık hata iletisi bulunmadığını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="0413d-131">On the **Partner** tab verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span> <span data-ttu-id="0413d-132">Varsa, yönergeleri izleyin ve bu konumları onarın.</span><span class="sxs-lookup"><span data-stu-id="0413d-132">If there is, follow instructions and fix those locations.</span></span> 

3. <span data-ttu-id="0413d-133">Bir hata mesajı yoksa,  **Ayarlar**' dan  **Hesap ayarları**, **kuruluş profili**, **tanımlayıcılar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="0413d-133">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

4. <span data-ttu-id="0413d-134">"Location" türünde, bu CSP hesabının ülkesiyle eşleşen MPN KIMLIĞINI bulun ve bunu aşağıda aramak ve ilişkilendirilmesi için kullanmak üzere kullanın.</span><span class="sxs-lookup"><span data-stu-id="0413d-134">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to search below and complete association.</span></span>

5. <span data-ttu-id="0413d-135">Kullanmak istediğiniz CSP hesabıyla eşleşen MPN KIMLIĞI konumunu bulamazsanız yeni bir MPN KIMLIĞI oluşturacak yeni bir konum ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0413d-135">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location which will create a new MPN ID.</span></span> <span data-ttu-id="0413d-136">Aşağıda **BIR MPN konumu ekleme** bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="0413d-136">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="0413d-137">MPN konumu ekleme</span><span class="sxs-lookup"><span data-stu-id="0413d-137">Add an MPN location</span></span>

1. <span data-ttu-id="0413d-138">Iş Ortağı Merkezi 'nde MPN hesabını kullanarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="0413d-138">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="0413d-139">(MPN kimlik bilgileriniz CSP kimlik bilgilerinizle farklı olabilir).</span><span class="sxs-lookup"><span data-stu-id="0413d-139">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="0413d-140">MPN hesabının genel yönetici veya hesap yönetici ayrıcalıklarına sahip olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="0413d-140">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="0413d-141">**Ayarlar simgesinden** **Hesap ayarları** ' nı seçin ve ardından **kuruluş profili**' ni seçin.</span><span class="sxs-lookup"><span data-stu-id="0413d-141">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="0413d-142">**Yasal** ' ı seçin ve sonra iş **ortağı** sekmesinde **iş konumları** ' nı seçin ve **Konum Ekle** ' ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="0413d-142">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="0413d-143">Şirketinize eklemek istediğiniz konum için iş adı, adres ve ilgili kişi dahil olmak üzere gerekli ayrıntıları sağlayın.</span><span class="sxs-lookup"><span data-stu-id="0413d-143">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="0413d-144">**Konum Ekle**' ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="0413d-144">Click **Add location**.</span></span> <span data-ttu-id="0413d-145">Bu, yeni konum için CSP işlemleri ve teşvikleri için kullanabileceğiniz yeni bir MPN KIMLIĞI oluşturur.</span><span class="sxs-lookup"><span data-stu-id="0413d-145">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Yeni bir yasal iş ekleyin":::

> [!NOTE]
> <span data-ttu-id="0413d-147">Iş Ortağı Merkezi 'ne bir konum eklendikten sonra kaldırılamaz.</span><span class="sxs-lookup"><span data-stu-id="0413d-147">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="0413d-148">Oturum açmak için doğru MPN KIMLIĞINI kullandıysanız, **MPN** 'Yi Iş Ortağı Merkezi 'nin sol menüsünde görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="0413d-148">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="0413d-149">Ortak genel hesap ülkesini değiştirin</span><span class="sxs-lookup"><span data-stu-id="0413d-149">Change country of Partner global account</span></span> 

1. <span data-ttu-id="0413d-150">Iş Ortağı Merkezi 'nde MPN hesabını kullanarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="0413d-150">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="0413d-151">(MPN kimlik bilgileriniz CSP kimlik bilgilerinizle farklı olabilir).</span><span class="sxs-lookup"><span data-stu-id="0413d-151">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="0413d-152">MPN hesabının genel yönetici veya hesap yönetici ayrıcalıklarına sahip olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="0413d-152">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="0413d-153">Iş **ortakları** sekmesinde **iş konumları** ' na gidin ve yasal varlığınız olarak istediğiniz konumun listelendiğinden emin olmak için konumların listesini kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="0413d-153">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="0413d-154">Konum eklemek için, **Konum Ekle**' ye tıklayın ve kullanıma hazır olarak, şirketinizde eklemek istediğiniz konum için iş adı, adres ve birincil kişi dahil olmak üzere gerekli ayrıntıları sağlayın.</span><span class="sxs-lookup"><span data-stu-id="0413d-154">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="0413d-155">**Ülke/bölge** açılır seçeneğinin yanındaki **ülkenizi değiştirin** ' i seçin ve adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="0413d-155">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Yasal iş profili verileri kullanıma hazır":::

5. <span data-ttu-id="0413d-157">**Kaydet**’e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="0413d-157">Click **Save**.</span></span>

6. <span data-ttu-id="0413d-158">MPN küresel hesap ülkesi, yeni yasal ülkeyle değiştirilecektir.</span><span class="sxs-lookup"><span data-stu-id="0413d-158">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="0413d-159">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="0413d-159">Next steps</span></span>

- <span data-ttu-id="0413d-160">[Doğrulama süreci](verification-responses.md)hakkında bilgi edinin.</span><span class="sxs-lookup"><span data-stu-id="0413d-160">Learn about the [verification process](verification-responses.md).</span></span>
