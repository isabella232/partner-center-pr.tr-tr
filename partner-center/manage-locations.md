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
ms.openlocfilehash: e39f264485e71c5a96916c224c0ea1a85c17a55b
ms.sourcegitcommit: fc1f9cb5a542bdc92d62d2a7e1ab2f4e69903e49
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/28/2021
ms.locfileid: "98925023"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="e89a7-103">MPN hesap konumlarını yönetin ve yeni bir konum ekleyin</span><span class="sxs-lookup"><span data-stu-id="e89a7-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="e89a7-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="e89a7-104">**Appropriate roles**</span></span>

- <span data-ttu-id="e89a7-105">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="e89a7-105">Global admin</span></span>
- <span data-ttu-id="e89a7-106">Hesap yöneticisi</span><span class="sxs-lookup"><span data-stu-id="e89a7-106">Account admin</span></span>

<span data-ttu-id="e89a7-107">MPN KIMLIĞI konumu, şirketinizin her belirli bir konumunu tanımlar.</span><span class="sxs-lookup"><span data-stu-id="e89a7-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="e89a7-108">MPN KIMLIK konumunu kullanarak, uygulamaları, Transact bulut çözümü sağlayıcısı (CSP) işletme ve diğer iş işlemlerine, teşvik etmek için kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="e89a7-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="e89a7-109">Genel MPN KIMLIĞI, destek istekleri gibi işlem olmayan etkinlikler için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="e89a7-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="e89a7-110">Tipik bir senaryo aşağıda verilmiştir:</span><span class="sxs-lookup"><span data-stu-id="e89a7-110">The following is a typical scenario:</span></span>

<span data-ttu-id="e89a7-111">Contoso, UK 'teki ortak genel hesabına (PGA) sahiptir.</span><span class="sxs-lookup"><span data-stu-id="e89a7-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="e89a7-112">Bu, kayıtlı yasal işletmektir ve tüm işlemsel olmayan işleri yönetmek için Global MPN KIMLIĞI kullanılır.</span><span class="sxs-lookup"><span data-stu-id="e89a7-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="e89a7-113">Contoso Ayrıca, UK, Fransa ve ABD 'de başka bir konumdaki yan kuruluşlar veya bölümler için Iş ortağı konum hesapları (PLA) ile eşdeğerdir.</span><span class="sxs-lookup"><span data-stu-id="e89a7-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="e89a7-114">MPN hesap yapısında, bu PLAs 'ler benzersiz konum MPN kimlikleri olarak gösterilir.</span><span class="sxs-lookup"><span data-stu-id="e89a7-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="e89a7-115">PLAs 'ler, CSP veya teşvikleri programları gibi işlem işleri için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="e89a7-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="e89a7-116">Ödemeler belirli konumlara bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="e89a7-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="e89a7-117">CSP kiracısı ve MPN konum KIMLIĞI arasında bir 1-1 ilişkisi vardır.</span><span class="sxs-lookup"><span data-stu-id="e89a7-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="MPN konumlarının yapısı":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="e89a7-119">CSP iş için yeni bir hesap eklemek için Önkoşullar</span><span class="sxs-lookup"><span data-stu-id="e89a7-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="e89a7-120">Yeni bir CSP iş hesabı eklemek için önkoşulları karşıladığından emin olarak başlayın.</span><span class="sxs-lookup"><span data-stu-id="e89a7-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="e89a7-121">CSP iş yapmak istediğiniz ülkede MPN KIMLIĞI 'ne sahip olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="e89a7-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="e89a7-122">Yeni bir MPN konumu oluşturmak için aşağıdaki "MPN konum Ekle" bölümünü okuyun.</span><span class="sxs-lookup"><span data-stu-id="e89a7-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="e89a7-123">Yeni bir CSP dolaylı satıcı kaydı oluşturmak için, [dolaylı sağlayıcılarla iş](indirect-reseller-tasks-in-partner-center.md#get-started) bölümünü okuyun</span><span class="sxs-lookup"><span data-stu-id="e89a7-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="e89a7-124">**Yeni** CSP hesabının **Yeni** kimlik bilgileriyle oturum açmayı unutmayın.</span><span class="sxs-lookup"><span data-stu-id="e89a7-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="e89a7-125">Mevcut kimlik bilgilerinizi, Iş Ortağı Merkezi zaten bir hesap varmış gibi tanıyacak şekilde kullanmayacaktır.</span><span class="sxs-lookup"><span data-stu-id="e89a7-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="e89a7-126">Microsoft Iş ortağı sözleşmesi 'Ni kabul edin ve hesabı etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="e89a7-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="e89a7-127">MPN konumu ekleme</span><span class="sxs-lookup"><span data-stu-id="e89a7-127">Add an MPN location</span></span>

1. <span data-ttu-id="e89a7-128">Iş Ortağı Merkezi 'nde MPN hesabını kullanarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="e89a7-128">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="e89a7-129">(MPN kimlik bilgileriniz CSP kimlik bilgilerinizle farklı olabilir).</span><span class="sxs-lookup"><span data-stu-id="e89a7-129">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="e89a7-130">MPN hesabının genel yönetici veya hesap yönetici ayrıcalıklarına sahip olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="e89a7-130">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="e89a7-131">**Ayarlar simgesinden** **Hesap ayarları** ' nı seçin ve ardından **kuruluş profili**' ni seçin.</span><span class="sxs-lookup"><span data-stu-id="e89a7-131">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="e89a7-132">**Yasal** ' ı seçin ve sonra iş **ortağı** sekmesinde **iş konumları** ' nı seçin ve **Konum Ekle** ' ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="e89a7-132">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="e89a7-133">Şirketinize eklemek istediğiniz konum için iş adı, adres ve ilgili kişi dahil olmak üzere gerekli ayrıntıları sağlayın.</span><span class="sxs-lookup"><span data-stu-id="e89a7-133">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="e89a7-134">**Konum Ekle**' ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="e89a7-134">Click **Add location**.</span></span> <span data-ttu-id="e89a7-135">Bu, yeni konum için CSP işlemleri ve teşvikleri için kullanabileceğiniz yeni bir MPN KIMLIĞI oluşturur.</span><span class="sxs-lookup"><span data-stu-id="e89a7-135">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Yeni bir yasal iş ekleyin":::

> [!NOTE]
> <span data-ttu-id="e89a7-137">Iş Ortağı Merkezi 'ne bir konum eklendikten sonra kaldırılamaz.</span><span class="sxs-lookup"><span data-stu-id="e89a7-137">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="e89a7-138">Oturum açmak için doğru MPN KIMLIĞINI kullandıysanız, **MPN** 'Yi Iş Ortağı Merkezi 'nin sol menüsünde görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="e89a7-138">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="e89a7-139">Ortak genel hesap ülkesini değiştirin</span><span class="sxs-lookup"><span data-stu-id="e89a7-139">Change country of Partner global account</span></span> 

1. <span data-ttu-id="e89a7-140">Iş Ortağı Merkezi 'nde MPN hesabını kullanarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="e89a7-140">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="e89a7-141">(MPN kimlik bilgileriniz CSP kimlik bilgilerinizle farklı olabilir).</span><span class="sxs-lookup"><span data-stu-id="e89a7-141">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="e89a7-142">MPN hesabının genel yönetici veya hesap yönetici ayrıcalıklarına sahip olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="e89a7-142">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="e89a7-143">Iş **ortakları** sekmesinde **iş konumları** ' na gidin ve yasal varlığınız olarak istediğiniz konumun listelendiğinden emin olmak için konumların listesini kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="e89a7-143">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="e89a7-144">Konum eklemek için, **Konum Ekle**' ye tıklayın ve kullanıma hazır olarak, şirketinizde eklemek istediğiniz konum için iş adı, adres ve birincil kişi dahil olmak üzere gerekli ayrıntıları sağlayın.</span><span class="sxs-lookup"><span data-stu-id="e89a7-144">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="e89a7-145">**Ülke/bölge** açılır seçeneğinin yanındaki **ülkenizi değiştirin** ' i seçin ve adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="e89a7-145">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Yasal iş profili verileri kullanıma hazır":::

5. <span data-ttu-id="e89a7-147">**Kaydet**’e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="e89a7-147">Click **Save**.</span></span>

6. <span data-ttu-id="e89a7-148">MPN küresel hesap ülkesi, yeni yasal ülkeyle değiştirilecektir.</span><span class="sxs-lookup"><span data-stu-id="e89a7-148">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="e89a7-149">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="e89a7-149">Next steps</span></span>

- <span data-ttu-id="e89a7-150">[Doğrulama süreci](verification-responses.md)hakkında bilgi edinin.</span><span class="sxs-lookup"><span data-stu-id="e89a7-150">Learn about the [verification process](verification-responses.md).</span></span>
