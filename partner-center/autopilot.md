---
title: Bir cihazın kullanıma hazır deneyimini özelleştirme
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Müşterinin yeni cihazını teslim etmeden önce, Windows Autopilot profillerini kullanarak cihazın kullanıma hazır deneyimini (OOBE) özelleştirebilir veya önceden yapılandırabilirsiniz.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 12057d50e4456dd2450ff497e00c89a9afa5dc4d
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96535006"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="b77a4-103">Yeni cihazlarda Windows Otomatik Pilot profillerini kullanarak müşterinin kullanıma hazır deneyimini özelleştirme</span><span class="sxs-lookup"><span data-stu-id="b77a4-103">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="b77a4-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="b77a4-104">**Appropriate roles**</span></span>

- <span data-ttu-id="b77a4-105">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="b77a4-105">Admin agent</span></span>
- <span data-ttu-id="b77a4-106">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="b77a4-106">Global admin</span></span>
- <span data-ttu-id="b77a4-107">Satış Aracısı</span><span class="sxs-lookup"><span data-stu-id="b77a4-107">Sales agent</span></span>
- <span data-ttu-id="b77a4-108">Kullanıcı Yönetimi Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="b77a4-108">User management admin</span></span>

<span data-ttu-id="b77a4-109">Müşteri cihazlarını yönetiyorsanız, müşterinin kullanıcıları için hazır olmayan deneyimi (OOBE) özelleştirmeniz gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="b77a4-109">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="b77a4-110">Cihazları müşterilere teslim etmeden önce Windows Autopilot profilleriyle yeni cihazları önceden yapılandırabilir ve müşterilerin zaten satın almış olduğu cihazlara yeni profiller uygulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b77a4-110">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="b77a4-111">OEM 'Lerin, cihazın **ürün anahtarı kimliğini (PKıD)** gösteren Autopilot cihaz kutusunun dışında bir sevkiyat etiketi de dahil başlatıldığını unutmayın.</span><span class="sxs-lookup"><span data-stu-id="b77a4-111">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="b77a4-112">Bu 1 boyutlu, okunabilir bir barkod, cihazların bir listesini kaldırmak zorunda kalmadan ve cihaz KIMLIĞINI alternatif yollarla ayırarak Autopilot için cihazları kaydetmek için bir yol ile aşağı akış ortakları sağlar.</span><span class="sxs-lookup"><span data-stu-id="b77a4-112">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="b77a4-113">Bu makalede, Autopilot profillerinin Iş Ortağı Merkezi 'nde cihazlara nasıl oluşturulacağı ve uygulanacağı açıklanır.</span><span class="sxs-lookup"><span data-stu-id="b77a4-113">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="b77a4-114">Zaten Autopilot hakkında bilgi sahibi değilseniz, bu makalelerdeki bilgileri gözden geçirin:</span><span class="sxs-lookup"><span data-stu-id="b77a4-114">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="b77a4-115">Windows Autopilot’a genel bakış</span><span class="sxs-lookup"><span data-stu-id="b77a4-115">Overview of Windows Autopilot</span></span>](/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="b77a4-116">Autopilot dağıtım başvurusu Kılavuzu</span><span class="sxs-lookup"><span data-stu-id="b77a4-116">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="b77a4-117">Genel bakış</span><span class="sxs-lookup"><span data-stu-id="b77a4-117">Overview</span></span>

<span data-ttu-id="b77a4-118">Iş Ortağı Merkezi 'ndeki Windows Autopilot özelliği ile müşteri cihazlarına uygulanacak özel profiller oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b77a4-118">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="b77a4-119">Aşağıdaki profil ayarları, bu makalenin yayımlandığı sırada mevcuttur:</span><span class="sxs-lookup"><span data-stu-id="b77a4-119">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="b77a4-120">Gizlilik ayarlarını atlayın.</span><span class="sxs-lookup"><span data-stu-id="b77a4-120">Skip privacy settings.</span></span> <span data-ttu-id="b77a4-121">Bu isteğe bağlı Autopilot profili ayarı, kuruluşların OOBE işlemi sırasında gizlilik ayarlarını istememesini sağlar.</span><span class="sxs-lookup"><span data-stu-id="b77a4-121">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="b77a4-122">Cihazda yerel yönetici hesabı oluşturmayı devre dışı bırakın.</span><span class="sxs-lookup"><span data-stu-id="b77a4-122">Disable local admin account creation on the device.</span></span> <span data-ttu-id="b77a4-123">Kuruluşlar, işlem tamamlandıktan sonra cihazı ayarlamaya yönelik kullanıcının yönetici erişimine sahip olup olmadığına karar verebilir.</span><span class="sxs-lookup"><span data-stu-id="b77a4-123">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="b77a4-124">Cihazı iş veya okul için otomatik olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="b77a4-124">Automatically set up device for work or school.</span></span> <span data-ttu-id="b77a4-125">Autopilot ile kaydedilen tüm cihazlar otomatik olarak iş veya okul cihazları olarak kabul edilir. bu nedenle, bu soru, OOBE işlemi sırasında istenmez.</span><span class="sxs-lookup"><span data-stu-id="b77a4-125">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="b77a4-126">Cortana, OneDrive ve OEM kayıt kurulum sayfalarını atlayın.</span><span class="sxs-lookup"><span data-stu-id="b77a4-126">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="b77a4-127">Autopilot ile kaydedilen tüm cihazlar, kullanıma hazır deneyim (OOBE) işlemi sırasında bu sayfaları otomatik olarak atlar.</span><span class="sxs-lookup"><span data-stu-id="b77a4-127">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="b77a4-128">Son Kullanıcı Lisans Sözleşmesi 'Ni (EULA) atlayın.</span><span class="sxs-lookup"><span data-stu-id="b77a4-128">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="b77a4-129">Kuruluşlar, Windows 10 sürüm 1709 ' den başlayarak, OOBE işlemi sırasında sunulan EULA sayfasını atlamaya karar verebilir.</span><span class="sxs-lookup"><span data-stu-id="b77a4-129">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="b77a4-130">Windows kurulumu sırasında EULA sayfasını atlamayı göz önünde bulundurmanız gereken önemli bilgiler için bkz. [Windows AUTOPILOT EULA](#windows-autopilot-eula-dismissal)</span><span class="sxs-lookup"><span data-stu-id="b77a4-130">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="b77a4-131">Aşağıdaki profil ve cihaz yönetim izinleri ve sınırlamaları geçerlidir:</span><span class="sxs-lookup"><span data-stu-id="b77a4-131">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="b77a4-132">CSP iş ortakları aralarında bayi ilişkileri olan mevcut müşteriler için, müşteri iş ortağının temsilci yönetim ayrıcalıklarını kaldırmış olsa bile, Otomatik Pilot profillerini yönetmeye devam edebilir.</span><span class="sxs-lookup"><span data-stu-id="b77a4-132">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="b77a4-133">Müşterilerinizin eklediği mevcut cihazları müşterileriniz için yönetebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b77a4-133">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="b77a4-134">Müşterinizin Microsoft Store İş'e veya Microsoft Intune Portalına yüklediği cihazları yönetemezsiniz.</span><span class="sxs-lookup"><span data-stu-id="b77a4-134">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="b77a4-135">Autopilot profillerini Iş Ortağı Merkezi 'nde oluşturma ve yönetme</span><span class="sxs-lookup"><span data-stu-id="b77a4-135">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="b77a4-136">Iş Ortağı Merkezi 'nde, Windows Autopilot dağıtım profilleri oluşturabilir ve bunları cihazlara uygulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b77a4-136">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="b77a4-137">Yalnızca yönetici aracıları profil oluşturabilir ve uygulayabilir.</span><span class="sxs-lookup"><span data-stu-id="b77a4-137">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="b77a4-138">Yeni bir Autopilot profili oluşturun</span><span class="sxs-lookup"><span data-stu-id="b77a4-138">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="b77a4-139">Iş Ortağı Merkezi menüsünden **müşteriler** ' i seçin ve ardından Autopilot profilini oluşturduğunuz müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="b77a4-139">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="b77a4-140">Müşterinin ayrıntı sayfasında **cihazlar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="b77a4-140">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="b77a4-141">**Windows Autopilot profilleri** altında **Yeni profil ekle**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="b77a4-141">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="b77a4-142">Profilin adını ve açıklamasını girip OOBE ayarlarını yapılandırın.</span><span class="sxs-lookup"><span data-stu-id="b77a4-142">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="b77a4-143">Aşağıdakilerden birini seçin:</span><span class="sxs-lookup"><span data-stu-id="b77a4-143">Choose from:</span></span>  

   - <span data-ttu-id="b77a4-144">Kurulum 'da gizlilik ayarlarını atla</span><span class="sxs-lookup"><span data-stu-id="b77a4-144">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="b77a4-145">Kurulumda yerel yönetici hesabını devre dışı bırak</span><span class="sxs-lookup"><span data-stu-id="b77a4-145">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="b77a4-146">Kurulum 'da sayfaları otomatik olarak atla</span><span class="sxs-lookup"><span data-stu-id="b77a4-146">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="b77a4-147">( *İş veya okul için kurulumu otomatik olarak seçme* ve *Cortana, OneDrive ve OEM kayıt kurulum sayfalarını atlama* dahil)</span><span class="sxs-lookup"><span data-stu-id="b77a4-147">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="b77a4-148">Son Kullanıcı Lisans Sözleşmesi 'ni (EULA) atla</span><span class="sxs-lookup"><span data-stu-id="b77a4-148">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="b77a4-149">Windows kurulumu sırasında EULA sayfasını atlamayı göz önünde bulundurmanız gereken önemli bilgiler için bkz. [Windows AUTOPILOT EULA](#windows-autopilot-eula-dismissal)</span><span class="sxs-lookup"><span data-stu-id="b77a4-149">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="b77a4-150">Bittiğinde **Gönder** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="b77a4-150">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="b77a4-151">Müşteri cihazlarına bir Autopilot profili uygulama</span><span class="sxs-lookup"><span data-stu-id="b77a4-151">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="b77a4-152">Aşağıdaki yönergelerde, müşterinin cihazlarını Iş Ortağı Merkezi 'ne eklediğiniz ve cihaz listesine erişebileceğiniz varsayılmaktadır.</span><span class="sxs-lookup"><span data-stu-id="b77a4-152">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="b77a4-153">Müşterinin cihazlarını henüz eklemediyseniz, [müşterinin hesabına cihaz ekleme](#add-devices-to-a-customers-account) ' deki yönergeleri izleyin ve ardından aşağıdaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="b77a4-153">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="b77a4-154">Bir müşteri için Autopilot profili oluşturduktan sonra, bunu müşterinin cihazlarına uygulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b77a4-154">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="b77a4-155">Iş Ortağı Merkezi menüsünden **müşteriler** ' i seçin ve ardından Autopilot profilini oluşturduğunuz müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="b77a4-155">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="b77a4-156">Müşterinin ayrıntı sayfasında **cihazlar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="b77a4-156">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="b77a4-157">**Cihazları cihazlara Uygula** altında, profil eklemek istediğiniz cihazları veya cihaz gruplarını seçin ve ardından **profili Uygula**' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="b77a4-157">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="b77a4-158">Yeni uyguladığınız profil **profil** sütununda görünür.</span><span class="sxs-lookup"><span data-stu-id="b77a4-158">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="b77a4-159">Profilin cihaza başarıyla uygulanacağını doğrulamak için aşağıdaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="b77a4-159">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="b77a4-160">a.</span><span class="sxs-lookup"><span data-stu-id="b77a4-160">a.</span></span>  <span data-ttu-id="b77a4-161">Bir cihazı ağa bağlayın ve açın.</span><span class="sxs-lookup"><span data-stu-id="b77a4-161">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="b77a4-162">b.</span><span class="sxs-lookup"><span data-stu-id="b77a4-162">b.</span></span>  <span data-ttu-id="b77a4-163">Uygun OOBE ekranlarının (varsa) göründüğünü doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="b77a4-163">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="b77a4-164">c.</span><span class="sxs-lookup"><span data-stu-id="b77a4-164">c.</span></span>  <span data-ttu-id="b77a4-165">OOBE işlemi durdurulduğunda, yeni bir kullanıcı için hazırlamak üzere cihazı fabrika varsayılan ayarlarına sıfırlayın.</span><span class="sxs-lookup"><span data-stu-id="b77a4-165">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="b77a4-166">Bir Autopilot profilini müşterinin cihazından kaldırma</span><span class="sxs-lookup"><span data-stu-id="b77a4-166">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="b77a4-167">Iş Ortağı Merkezi menüsünden **müşteriler** ' i seçin ve ardından Autopilot profilini oluşturduğunuz müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="b77a4-167">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="b77a4-168">Müşterinin ayrıntı sayfasında **cihazlar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="b77a4-168">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="b77a4-169">**Cihazlara profilleri Uygula** altında, profili kaldırmak istediğiniz cihazları seçin ve ardından **Profili Kaldır**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="b77a4-169">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="b77a4-170">Bir cihazın cihazdan kaldırılması, profili listenizden silmez.</span><span class="sxs-lookup"><span data-stu-id="b77a4-170">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="b77a4-171">Bir profili silmek istiyorsanız, [Autopilot profilini güncelleştirme veya silme](#update-or-delete-an-autopilot-profile)bölümündeki yönergeleri izleyin.</span><span class="sxs-lookup"><span data-stu-id="b77a4-171">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="b77a4-172">Autopilot profilini güncelleştirme veya silme</span><span class="sxs-lookup"><span data-stu-id="b77a4-172">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="b77a4-173">Müşteriler cihazları gönderdikten sonra, kullanıma hazır deneyimini değiştirmek isterse, Iş Ortağı Merkezi ' nde profili değiştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b77a4-173">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="b77a4-174">Müşterinin cihazı internet 'e bağlandığı zaman, OOBE işlemi sırasında en son profil sürümünü indirir.</span><span class="sxs-lookup"><span data-stu-id="b77a4-174">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="b77a4-175">Ayrıca, bir müşteri bir cihazı fabrika varsayılan ayarlarına geri yüklediğinde, bu cihaz, OOBE işlemi sırasında en son profil sürümünü yeniden indirir.</span><span class="sxs-lookup"><span data-stu-id="b77a4-175">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="b77a4-176">Iş Ortağı Merkezi menüsünden **müşteriler** ' i seçin ve ardından bir Autopilot profilini değiştirmenizi isteyen müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="b77a4-176">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="b77a4-177">Müşterinin ayrıntı sayfasında **cihazlar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="b77a4-177">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="b77a4-178">**Windows Autopilot profilleri** altında güncelleştirmeniz gereken profili seçin.</span><span class="sxs-lookup"><span data-stu-id="b77a4-178">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="b77a4-179">Gerekli değişiklikleri yapıp **Gönder**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="b77a4-179">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="b77a4-180">Bu profili silmek için sayfanın sağ üst köşesinden **Profili Sil** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="b77a4-180">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="b77a4-181">Müşterinin hesabına cihaz ekleme</span><span class="sxs-lookup"><span data-stu-id="b77a4-181">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="b77a4-182">Satış aracıları ve yönetici aracıları, bir müşterinin hesabına cihaz ekleyebilir.</span><span class="sxs-lookup"><span data-stu-id="b77a4-182">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="b77a4-183">Müşteri cihazlarına özel Autopilot profilleri uygulayabilmeniz için önce müşterinin cihaz listesine erişebiliyor olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="b77a4-183">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="b77a4-184">OEM adı, seri numarası ve model birleşimini kullanmayı planlıyorsanız, bu sınırlamalara dikkat edin:</span><span class="sxs-lookup"><span data-stu-id="b77a4-184">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="b77a4-185">Bu tanımlama grubu yalnızca daha yeni cihazlar (örneğin, 4k karmaları) için geçerlidir ve 128b karmaları (RS2 ve önceki cihazlar) için desteklenmez.</span><span class="sxs-lookup"><span data-stu-id="b77a4-185">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="b77a4-186">Demet kaydı, büyük/küçük harfe duyarlıdır; bu nedenle, dosyadaki verilerin, OEM sağlayıcısı (donanım sağlayıcısı) tarafından sağlandığı gibi, model ve üretici adlarıyla \**_tam_* _ ile eşleşmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="b77a4-186">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names \**_exactly_* _ as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="b77a4-187">Iş Ortağı Merkezi 'nde bir müşterinin hesabına cihaz eklemek için aşağıdaki yönergeleri izleyin.</span><span class="sxs-lookup"><span data-stu-id="b77a4-187">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="b77a4-188">Iş Ortağı Merkezi menüsünde _ *Customers*\* öğesini seçin ve ardından cihazlarını yönetmek istediğiniz müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="b77a4-188">Select _ *Customers*\* from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="b77a4-189">Müşterinin ayrıntı sayfasında **cihazlar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="b77a4-189">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="b77a4-190">**Cihazlara profil Uygula** altında **Cihaz Ekle**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="b77a4-190">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="b77a4-191">Cihaz listesi için bir ad girin ve ardından, müşteri listesini (. csv dosyası biçiminde) Iş Ortağı Merkezi 'ne yüklemek için **Gözden** geçirme ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="b77a4-191">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="b77a4-192">Bu. csv dosyasını cihazınızın satın alımından almış olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="b77a4-192">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="b77a4-193">Bir. csv dosyası almadıysanız, [Windows Autopilot 'a cihaz ekleme](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)adımlarını izleyerek kendiniz bir tane oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b77a4-193">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="b77a4-194">. Csv dosyasını karşıya yükleyin ve ardından **Kaydet**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="b77a4-194">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="b77a4-195">Bir .csv dosyasını karşıya yüklemeye çalışırken hata iletisi alıyorsanız, dosyanın biçimini denetleyin.</span><span class="sxs-lookup"><span data-stu-id="b77a4-195">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="b77a4-196">Yalnızca donanım karmasını veya OEM adı, seri numarası ve model (bu sütun sırasıyla) veya Windows Ürün Kimliğini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b77a4-196">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="b77a4-197">Cihaz listesi oluşturmak için cihaz **Ekle** ' nin yanındaki bağlantıdan sunulan Sample. csv dosyasını da kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b77a4-197">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="b77a4-198">. Csv dosyanız şuna benzer görünmelidir:</span><span class="sxs-lookup"><span data-stu-id="b77a4-198">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="b77a4-199">**Cihaz seri numarası, Windows ürün KIMLIĞI, donanım karması, üretici adı, cihaz modeli**</span><span class="sxs-lookup"><span data-stu-id="b77a4-199">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="b77a4-200">**{serialNumber},,, Microsoft Corporation, Surface dizüstü bilgisayar**</span><span class="sxs-lookup"><span data-stu-id="b77a4-200">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="b77a4-201">"Üretici adı" ve "cihaz modeli" büyük/küçük harfe duyarlıdır.</span><span class="sxs-lookup"><span data-stu-id="b77a4-201">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="b77a4-202">Üretici adı ve cihaz modeli için hangi değeri koyacağınızı bilmiyorsanız, doğru değerleri toplamak için bunu cihazda çalıştırabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="b77a4-202">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="b77a4-203">Windows Autopilot EULA</span><span class="sxs-lookup"><span data-stu-id="b77a4-203">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="b77a4-204">ÖNEMLI BILGILER</span><span class="sxs-lookup"><span data-stu-id="b77a4-204">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="b77a4-205">Windows Autopilot, müşterileriniz için yönettiğiniz cihazlarda özelleştirilmiş Windows yüklemelerini yapılandırmanıza olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="b77a4-205">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="b77a4-206">Müşteri tarafından bu şekilde yetkilendirilirse, EULA (Son Kullanıcı Lisans Sözleşmesi) kabul ekranı dahil olmak üzere Windows 'u ayarlarken kullanıcılara sunulan belirli kurulum ekranlarını göstermez veya gizleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b77a4-206">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="b77a4-207">Bu işlevi kullanarak, kullanıcılara bildirim veya koşulların kabul etmesini sağlamak için tasarlanan tüm ekranları gizlemeyi veya gizlemeyi kabul etmiş olursunuz. koşulları, müşterinizin adına (bir kuruluşun veya bireysel kullanıcı gibi), herhangi bir uyarıyı onaylamak ve müşteriniz için geçerli olan koşulları kabul etmek için müşterinize yeterli izin ve yetkilendirme elde ettiğinizi kabul edersiniz.</span><span class="sxs-lookup"><span data-stu-id="b77a4-207">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="b77a4-208">Bu, lisans hüküm ve koşullarına yönelik anlaşmayı ve bu aracı kullanarak gizlemeyin veya gizleyemediyseniz kullanıcıya sunulacak bildirimi içerir.</span><span class="sxs-lookup"><span data-stu-id="b77a4-208">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="b77a4-209">Müşteri, Microsoft 'tan veya lisanslı dağıtıcılarından yazılım için geçerli bir lisans almadıysanız, müşteriniz bu cihazlarda Windows yazılımlarını kullanmayabilir.</span><span class="sxs-lookup"><span data-stu-id="b77a4-209">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>