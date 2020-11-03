---
title: İş ortağı hesabınızdaki konumları yönetin
ms.topic: article
ms.date: 10/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Yeni bir konum ekleme ve bilgisayar, CSP iş, abonelik ve diğer işlemlerde MPN KIMLIĞI 'nin nasıl kullanıldığını öğrenin.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c6b0fc84636befedbc51aa0672ce19110eb4d9aa
ms.sourcegitcommit: 1719ff11409cd6953602b7798f8cfe821b8ea15e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/15/2020
ms.locfileid: "92531971"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="88351-103">MPN hesap konumlarını yönetin ve yeni bir konum ekleyin</span><span class="sxs-lookup"><span data-stu-id="88351-103">Manage your MPN account locations and add a new location</span></span>

<span data-ttu-id="88351-104">**Uygulama hedefi**</span><span class="sxs-lookup"><span data-stu-id="88351-104">**Applies to**</span></span>

- <span data-ttu-id="88351-105">İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="88351-105">Partner Center</span></span>

<span data-ttu-id="88351-106">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="88351-106">**Appropriate roles**</span></span>

- <span data-ttu-id="88351-107">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="88351-107">Global admin</span></span>
- <span data-ttu-id="88351-108">Hesap yöneticisi</span><span class="sxs-lookup"><span data-stu-id="88351-108">Account admin</span></span>

<span data-ttu-id="88351-109">MPN KIMLIĞI konumu, şirketinizin her belirli bir konumunu tanımlar.</span><span class="sxs-lookup"><span data-stu-id="88351-109">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="88351-110">MPN KIMLIK konumunu kullanarak, uygulamaları, Transact bulut çözümü sağlayıcısı (CSP) işletme ve diğer iş işlemlerine, teşvik etmek için kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="88351-110">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="88351-111">Genel MPN KIMLIĞI, destek istekleri gibi işlem olmayan etkinlikler için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="88351-111">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="88351-112">Tipik bir senaryo aşağıda verilmiştir:</span><span class="sxs-lookup"><span data-stu-id="88351-112">The following is a typical scenario:</span></span>

<span data-ttu-id="88351-113">Contoso, UK 'teki ortak genel hesabına (PGA) sahiptir.</span><span class="sxs-lookup"><span data-stu-id="88351-113">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="88351-114">Bu, kayıtlı yasal işletmektir ve tüm işlemsel olmayan işleri yönetmek için Global MPN KIMLIĞI kullanılır.</span><span class="sxs-lookup"><span data-stu-id="88351-114">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="88351-115">Contoso Ayrıca, UK, Fransa ve ABD 'de başka bir konumdaki yan kuruluşlar veya bölümler için Iş ortağı konum hesapları (PLA) ile eşdeğerdir.</span><span class="sxs-lookup"><span data-stu-id="88351-115">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="88351-116">MPN hesap yapısında, bu PLAs 'ler benzersiz konum MPN kimlikleri olarak gösterilir.</span><span class="sxs-lookup"><span data-stu-id="88351-116">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="88351-117">PLAs 'ler, CSP veya teşvikleri programları gibi işlem işleri için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="88351-117">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="88351-118">Ödemeler belirli konumlara bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="88351-118">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="88351-119">CSP kiracısı ve MPN konum KIMLIĞI arasında bir 1-1 ilişkisi vardır.</span><span class="sxs-lookup"><span data-stu-id="88351-119">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="MPN konumlarının yapısı":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a><span data-ttu-id="88351-121">CSP iş için yeni bir konum eklemek üzere Önkoşullar</span><span class="sxs-lookup"><span data-stu-id="88351-121">Prerequisites in order to add a new location for a CSP business</span></span>

<span data-ttu-id="88351-122">Yeni bir CSP iş konumu eklemek için birkaç önkoşul vardır:</span><span class="sxs-lookup"><span data-stu-id="88351-122">To add a new CSP business location, there are several prerequisites:</span></span>

1. <span data-ttu-id="88351-123">İş yapmak istediğiniz ülkede MPN KIMLIĞI 'ne sahip olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="88351-123">You must have a location MPN ID in the country where you want to do business.</span></span>

1. <span data-ttu-id="88351-124">[İş bölgesinde](regional-authorization-overview.md) zaten CSP 'ye kayıtlı olmayan yeni BIR Azure AD kiracısına sahip olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="88351-124">You need a new Azure AD tenant in the [region of business](regional-authorization-overview.md) which is not already enrolled into CSP.</span></span> <span data-ttu-id="88351-125">CSP 'ye kaydoldığınızda bunu oluşturun.</span><span class="sxs-lookup"><span data-stu-id="88351-125">Create this when you enroll in CSP.</span></span>
 
3. <span data-ttu-id="88351-126">Bölgede CSP programına kaydolmak için yeni AAD kiracısını kullanın.</span><span class="sxs-lookup"><span data-stu-id="88351-126">Use the new AAD tenant to enroll into CSP program in the region.</span></span>
<span data-ttu-id="88351-127">Yasal Şirket adı, adres, birincil iletişim ayrıntıları dahil yasal Şirket ayrıntılarını sağlama.</span><span class="sxs-lookup"><span data-stu-id="88351-127">Providing legal company details including the legal company name, address, primary contact details.</span></span> <span data-ttu-id="88351-128">Bu hesap, doğrulamaya devam edecek, bu nedenle geçerli bilgiler eklediğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="88351-128">This account will undergo verification, so make sure to add valid information.</span></span>

>[!NOTE] 
 ><span data-ttu-id="88351-129">**Yeni** Azure AD kiracısı için **Yeni** kimlik bilgileriyle oturum açmayı unutmayın.</span><span class="sxs-lookup"><span data-stu-id="88351-129">Remember to sign in with the **new** credentials for the **new** Azure AD tenant.</span></span> <span data-ttu-id="88351-130">Mevcut kimlik bilgilerinizi, Iş Ortağı Merkezi zaten bir hesap varmış gibi tanıyacak şekilde kullanmayacaktır.</span><span class="sxs-lookup"><span data-stu-id="88351-130">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

4. <span data-ttu-id="88351-131">Microsoft Iş ortağı sözleşmesi 'Ni kabul edin ve hesabı etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="88351-131">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="88351-132">MPN konumu ekleme</span><span class="sxs-lookup"><span data-stu-id="88351-132">Add an MPN location</span></span>

1. <span data-ttu-id="88351-133">Iş Ortağı Merkezi 'nde MPN hesabını kullanarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="88351-133">Sign in using the MPN account in Partner Center .</span></span> <span data-ttu-id="88351-134">MPN hesabının genel yönetici veya hesap yönetici ayrıcalıklarına sahip olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="88351-134">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="88351-135">**Ayar simgesinden** **iş ortağı ayarları** ' nı seçin.</span><span class="sxs-lookup"><span data-stu-id="88351-135">From the **Setting icon** , select the **Partner settings** .</span></span>

2. <span data-ttu-id="88351-136">**Konum seçin.**</span><span class="sxs-lookup"><span data-stu-id="88351-136">Select **Locations.**</span></span>

3. <span data-ttu-id="88351-137">**Konum Ekle** ' yi seçin ve şirkete eklemek istediğiniz konumun adres ayrıntılarını ve konum için bir birincil kişiyi ekleyin.</span><span class="sxs-lookup"><span data-stu-id="88351-137">Select **Add a location** , and insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="88351-138">Iş Ortağı Merkezi 'ne bir konum eklendikten sonra kaldırılamaz.</span><span class="sxs-lookup"><span data-stu-id="88351-138">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="88351-139">Oturum açmak için doğru MPN KIMLIĞINI kullandıysanız, **MPN** 'Yi Iş Ortağı Merkezi 'nin sol menüsünde görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="88351-139">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-global-partner-account-location"></a><span data-ttu-id="88351-140">Küresel iş ortağı hesabı konumunu değiştir</span><span class="sxs-lookup"><span data-stu-id="88351-140">Change Global partner account location</span></span>

1. <span data-ttu-id="88351-141">**[Konumlar](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)** sayfasında, yasal varlığınız olarak istediğiniz konumun listelendiğinden emin olmak için konumların listesini kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="88351-141">On the **[Locations](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)** page, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="88351-142">Değilse, ekleyin.</span><span class="sxs-lookup"><span data-stu-id="88351-142">If it isn't, add it.</span></span>

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="Tüm geçerli konumların listesini içeren Iş ortağı merkezi hesap konumları sayfasının ekran görüntüsü.":::

2. <span data-ttu-id="88351-144">**Iş ortağı profilini** seçin ve ardından **yasal iş profilini Güncelleştir** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="88351-144">Select **Partner profile** and then select **Update legal business profile**</span></span>

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="Seçilebilir güncelleştirme seçeneğiyle Iş ortağı merkezi hesap ortağı profili bilgilerini gösteren ekran görüntüsü.":::

3. <span data-ttu-id="88351-146">Bölgeyi ve yasal varlığı seçip **gönderebilirsiniz** .</span><span class="sxs-lookup"><span data-stu-id="88351-146">Select the region and legal entity and **Submit** it.</span></span>

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="İş ortağının yasal iş profilini güncelleştirme ekran görüntüsü, ülke veya bölgeyi ve yasal varlığı güncelleştirmek için açılan listeleri gösterir.":::

## <a name="next-steps"></a><span data-ttu-id="88351-148">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="88351-148">Next steps</span></span>

- <span data-ttu-id="88351-149">[Doğrulama süreci](verification-responses.md)hakkında bilgi edinin.</span><span class="sxs-lookup"><span data-stu-id="88351-149">Learn about the [verification process](verification-responses.md).</span></span>
