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
ms.openlocfilehash: 0ae61db0ca040afe67faa3a0883ea033b8f67562
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/22/2020
ms.locfileid: "92531566"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="80898-103">Yeni cihazlarda Windows Otomatik Pilot profillerini kullanarak müşterinin kullanıma hazır deneyimini özelleştirme</span><span class="sxs-lookup"><span data-stu-id="80898-103">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="80898-104">**Uygulama hedefi**</span><span class="sxs-lookup"><span data-stu-id="80898-104">**Applies to**</span></span>

- <span data-ttu-id="80898-105">CSP doğrudan fatura ortakları, dolaylı sağlayıcılar ve dolaylı satıcılar</span><span class="sxs-lookup"><span data-stu-id="80898-105">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="80898-106">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="80898-106">**Appropriate roles**</span></span>

- <span data-ttu-id="80898-107">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="80898-107">Admin agent</span></span>
- <span data-ttu-id="80898-108">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="80898-108">Global admin</span></span>
- <span data-ttu-id="80898-109">Satış Aracısı</span><span class="sxs-lookup"><span data-stu-id="80898-109">Sales agent</span></span>
- <span data-ttu-id="80898-110">Kullanıcı Yönetimi Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="80898-110">User management admin</span></span>

<span data-ttu-id="80898-111">Müşteri cihazlarını yönetiyorsanız, müşterinin kullanıcıları için hazır olmayan deneyimi (OOBE) özelleştirmeniz gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="80898-111">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="80898-112">Cihazları müşterilere teslim etmeden önce Windows Autopilot profilleriyle yeni cihazları önceden yapılandırabilir ve müşterilerin zaten satın almış olduğu cihazlara yeni profiller uygulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="80898-112">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="80898-113">OEM 'Lerin, cihazın **ürün anahtarı kimliğini (PKıD)** gösteren Autopilot cihaz kutusunun dışında bir sevkiyat etiketi de dahil başlatıldığını unutmayın.</span><span class="sxs-lookup"><span data-stu-id="80898-113">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)** .</span></span>  <span data-ttu-id="80898-114">Bu 1 boyutlu, okunabilir bir barkod, cihazların bir listesini kaldırmak zorunda kalmadan ve cihaz KIMLIĞINI alternatif yollarla ayırarak Autopilot için cihazları kaydetmek için bir yol ile aşağı akış ortakları sağlar.</span><span class="sxs-lookup"><span data-stu-id="80898-114">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="80898-115">Bu makalede, Autopilot profillerinin Iş Ortağı Merkezi 'nde cihazlara nasıl oluşturulacağı ve uygulanacağı açıklanır.</span><span class="sxs-lookup"><span data-stu-id="80898-115">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="80898-116">Zaten Autopilot hakkında bilgi sahibi değilseniz, bu makalelerdeki bilgileri gözden geçirin:</span><span class="sxs-lookup"><span data-stu-id="80898-116">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="80898-117">Windows Autopilot 'e genel bakış</span><span class="sxs-lookup"><span data-stu-id="80898-117">Overview of Windows Autopilot</span></span>](/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="80898-118">Autopilot dağıtım başvurusu Kılavuzu</span><span class="sxs-lookup"><span data-stu-id="80898-118">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="80898-119">Genel Bakış</span><span class="sxs-lookup"><span data-stu-id="80898-119">Overview</span></span>

<span data-ttu-id="80898-120">Iş Ortağı Merkezi 'ndeki Windows Autopilot özelliği ile müşteri cihazlarına uygulanacak özel profiller oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="80898-120">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="80898-121">Aşağıdaki profil ayarları, bu makalenin yayımlandığı sırada mevcuttur:</span><span class="sxs-lookup"><span data-stu-id="80898-121">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="80898-122">Gizlilik ayarlarını atlayın.</span><span class="sxs-lookup"><span data-stu-id="80898-122">Skip privacy settings.</span></span> <span data-ttu-id="80898-123">Bu isteğe bağlı Autopilot profili ayarı, kuruluşların OOBE işlemi sırasında gizlilik ayarlarını istememesini sağlar.</span><span class="sxs-lookup"><span data-stu-id="80898-123">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="80898-124">Cihazda yerel yönetici hesabı oluşturmayı devre dışı bırakın.</span><span class="sxs-lookup"><span data-stu-id="80898-124">Disable local admin account creation on the device.</span></span> <span data-ttu-id="80898-125">Kuruluşlar, işlem tamamlandıktan sonra cihazı ayarlamaya yönelik kullanıcının yönetici erişimine sahip olup olmadığına karar verebilir.</span><span class="sxs-lookup"><span data-stu-id="80898-125">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="80898-126">Cihazı iş veya okul için otomatik olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="80898-126">Automatically set up device for work or school.</span></span> <span data-ttu-id="80898-127">Autopilot ile kaydedilen tüm cihazlar otomatik olarak iş veya okul cihazları olarak kabul edilir. bu nedenle, bu soru, OOBE işlemi sırasında istenmez.</span><span class="sxs-lookup"><span data-stu-id="80898-127">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="80898-128">Cortana, OneDrive ve OEM kayıt kurulum sayfalarını atlayın.</span><span class="sxs-lookup"><span data-stu-id="80898-128">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="80898-129">Autopilot ile kaydedilen tüm cihazlar, kullanıma hazır deneyim (OOBE) işlemi sırasında bu sayfaları otomatik olarak atlar.</span><span class="sxs-lookup"><span data-stu-id="80898-129">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="80898-130">Son Kullanıcı Lisans Sözleşmesi 'Ni (EULA) atlayın.</span><span class="sxs-lookup"><span data-stu-id="80898-130">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="80898-131">Kuruluşlar, Windows 10 sürüm 1709 ' den başlayarak, OOBE işlemi sırasında sunulan EULA sayfasını atlamaya karar verebilir.</span><span class="sxs-lookup"><span data-stu-id="80898-131">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="80898-132">Windows kurulumu sırasında EULA sayfasını atlamayı göz önünde bulundurmanız gereken önemli bilgiler için bkz. [Windows AUTOPILOT EULA](#windows-autopilot-eula-dismissal)</span><span class="sxs-lookup"><span data-stu-id="80898-132">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="80898-133">Aşağıdaki profil ve cihaz yönetim izinleri ve sınırlamaları geçerlidir:</span><span class="sxs-lookup"><span data-stu-id="80898-133">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="80898-134">CSP iş ortakları aralarında bayi ilişkileri olan mevcut müşteriler için, müşteri iş ortağının temsilci yönetim ayrıcalıklarını kaldırmış olsa bile, Otomatik Pilot profillerini yönetmeye devam edebilir.</span><span class="sxs-lookup"><span data-stu-id="80898-134">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="80898-135">Müşterilerinizin eklediği mevcut cihazları müşterileriniz için yönetebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="80898-135">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="80898-136">Müşterinizin Microsoft Store İş'e veya Microsoft Intune Portalına yüklediği cihazları yönetemezsiniz.</span><span class="sxs-lookup"><span data-stu-id="80898-136">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="80898-137">Autopilot profillerini Iş Ortağı Merkezi 'nde oluşturma ve yönetme</span><span class="sxs-lookup"><span data-stu-id="80898-137">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="80898-138">Iş Ortağı Merkezi 'nde, Windows Autopilot dağıtım profilleri oluşturabilir ve bunları cihazlara uygulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="80898-138">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="80898-139">Yalnızca yönetici aracıları profil oluşturabilir ve uygulayabilir.</span><span class="sxs-lookup"><span data-stu-id="80898-139">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="80898-140">Yeni bir Autopilot profili oluşturun</span><span class="sxs-lookup"><span data-stu-id="80898-140">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="80898-141">Iş Ortağı Merkezi menüsünden **müşteriler** ' i seçin ve ardından Autopilot profilini oluşturduğunuz müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="80898-141">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="80898-142">Müşterinin ayrıntı sayfasında **cihazlar** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="80898-142">On the customer's detail page, select **Devices** .</span></span>

3. <span data-ttu-id="80898-143">**Windows Autopilot profilleri** altında **Yeni profil ekle** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="80898-143">Under **Windows Autopilot profiles** select **Add new profile** .</span></span>

4. <span data-ttu-id="80898-144">Profilin adını ve açıklamasını girip OOBE ayarlarını yapılandırın.</span><span class="sxs-lookup"><span data-stu-id="80898-144">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="80898-145">Aşağıdakilerden birini seçin:</span><span class="sxs-lookup"><span data-stu-id="80898-145">Choose from:</span></span>  

   - <span data-ttu-id="80898-146">Kurulum 'da gizlilik ayarlarını atla</span><span class="sxs-lookup"><span data-stu-id="80898-146">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="80898-147">Kurulumda yerel yönetici hesabını devre dışı bırak</span><span class="sxs-lookup"><span data-stu-id="80898-147">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="80898-148">Kurulum 'da sayfaları otomatik olarak atla</span><span class="sxs-lookup"><span data-stu-id="80898-148">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="80898-149">( *İş veya okul için kurulumu otomatik olarak seçme* ve *Cortana, OneDrive ve OEM kayıt kurulum sayfalarını atlama* dahil)</span><span class="sxs-lookup"><span data-stu-id="80898-149">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages* )</span></span>
  
   - <span data-ttu-id="80898-150">Son Kullanıcı Lisans Sözleşmesi 'ni (EULA) atla</span><span class="sxs-lookup"><span data-stu-id="80898-150">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="80898-151">Windows kurulumu sırasında EULA sayfasını atlamayı göz önünde bulundurmanız gereken önemli bilgiler için bkz. [Windows AUTOPILOT EULA](#windows-autopilot-eula-dismissal)</span><span class="sxs-lookup"><span data-stu-id="80898-151">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="80898-152">Bittiğinde **Gönder** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="80898-152">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="80898-153">Müşteri cihazlarına bir Autopilot profili uygulama</span><span class="sxs-lookup"><span data-stu-id="80898-153">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="80898-154">Aşağıdaki yönergelerde, müşterinin cihazlarını Iş Ortağı Merkezi 'ne eklediğiniz ve cihaz listesine erişebileceğiniz varsayılmaktadır.</span><span class="sxs-lookup"><span data-stu-id="80898-154">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="80898-155">Müşterinin cihazlarını henüz eklemediyseniz, [müşterinin hesabına cihaz ekleme](#add-devices-to-a-customers-account) ' deki yönergeleri izleyin ve ardından aşağıdaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="80898-155">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="80898-156">Bir müşteri için Autopilot profili oluşturduktan sonra, bunu müşterinin cihazlarına uygulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="80898-156">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="80898-157">Iş Ortağı Merkezi menüsünden **müşteriler** ' i seçin ve ardından Autopilot profilini oluşturduğunuz müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="80898-157">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="80898-158">Müşterinin ayrıntı sayfasında **cihazlar** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="80898-158">On the customer's detail page, select **Devices** .</span></span>

3. <span data-ttu-id="80898-159">**Cihazları cihazlara Uygula** altında, profil eklemek istediğiniz cihazları veya cihaz gruplarını seçin ve ardından **profili Uygula** ' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="80898-159">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile** .</span></span> <span data-ttu-id="80898-160">Yeni uyguladığınız profil **profil** sütununda görünür.</span><span class="sxs-lookup"><span data-stu-id="80898-160">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="80898-161">Profilin cihaza başarıyla uygulanacağını doğrulamak için aşağıdaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="80898-161">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="80898-162">a.</span><span class="sxs-lookup"><span data-stu-id="80898-162">a.</span></span>  <span data-ttu-id="80898-163">Bir cihazı ağa bağlayın ve açın.</span><span class="sxs-lookup"><span data-stu-id="80898-163">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="80898-164">b.</span><span class="sxs-lookup"><span data-stu-id="80898-164">b.</span></span>  <span data-ttu-id="80898-165">Uygun OOBE ekranlarının (varsa) göründüğünü doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="80898-165">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="80898-166">c.</span><span class="sxs-lookup"><span data-stu-id="80898-166">c.</span></span>  <span data-ttu-id="80898-167">OOBE işlemi durdurulduğunda, yeni bir kullanıcı için hazırlamak üzere cihazı fabrika varsayılan ayarlarına sıfırlayın.</span><span class="sxs-lookup"><span data-stu-id="80898-167">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="80898-168">Bir Autopilot profilini müşterinin cihazından kaldırma</span><span class="sxs-lookup"><span data-stu-id="80898-168">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="80898-169">Iş Ortağı Merkezi menüsünden **müşteriler** ' i seçin ve ardından Autopilot profilini oluşturduğunuz müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="80898-169">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="80898-170">Müşterinin ayrıntı sayfasında **cihazlar** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="80898-170">On the customer's detail page, select **Devices** .</span></span>

3. <span data-ttu-id="80898-171">**Cihazlara profilleri Uygula** altında, profili kaldırmak istediğiniz cihazları seçin ve ardından **Profili Kaldır** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="80898-171">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile** .</span></span>

   >[!NOTE]
   ><span data-ttu-id="80898-172">Bir cihazın cihazdan kaldırılması, profili listenizden silmez.</span><span class="sxs-lookup"><span data-stu-id="80898-172">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="80898-173">Bir profili silmek istiyorsanız, [Autopilot profilini güncelleştirme veya silme](#update-or-delete-an-autopilot-profile)bölümündeki yönergeleri izleyin.</span><span class="sxs-lookup"><span data-stu-id="80898-173">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="80898-174">Autopilot profilini güncelleştirme veya silme</span><span class="sxs-lookup"><span data-stu-id="80898-174">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="80898-175">Müşteriler cihazları gönderdikten sonra, kullanıma hazır deneyimini değiştirmek isterse, Iş Ortağı Merkezi ' nde profili değiştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="80898-175">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="80898-176">Müşterinin cihazı internet 'e bağlandığı zaman, OOBE işlemi sırasında en son profil sürümünü indirir.</span><span class="sxs-lookup"><span data-stu-id="80898-176">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="80898-177">Ayrıca, bir müşteri bir cihazı fabrika varsayılan ayarlarına geri yüklediğinde, bu cihaz, OOBE işlemi sırasında en son profil sürümünü yeniden indirir.</span><span class="sxs-lookup"><span data-stu-id="80898-177">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="80898-178">Iş Ortağı Merkezi menüsünden **müşteriler** ' i seçin ve ardından bir Autopilot profilini değiştirmenizi isteyen müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="80898-178">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="80898-179">Müşterinin ayrıntı sayfasında **cihazlar** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="80898-179">On the customer's detail page, select **Devices** .</span></span>

3. <span data-ttu-id="80898-180">**Windows Autopilot profilleri** altında güncelleştirmeniz gereken profili seçin.</span><span class="sxs-lookup"><span data-stu-id="80898-180">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="80898-181">Gerekli değişiklikleri yapıp **Gönder** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="80898-181">Make the required changes and then select **Submit** .</span></span>

<span data-ttu-id="80898-182">Bu profili silmek için sayfanın sağ üst köşesinden **Profili Sil** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="80898-182">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="80898-183">Müşterinin hesabına cihaz ekleme</span><span class="sxs-lookup"><span data-stu-id="80898-183">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="80898-184">Satış aracıları ve yönetici aracıları, bir müşterinin hesabına cihaz ekleyebilir.</span><span class="sxs-lookup"><span data-stu-id="80898-184">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="80898-185">Müşteri cihazlarına özel Autopilot profilleri uygulayabilmeniz için önce müşterinin cihaz listesine erişebiliyor olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="80898-185">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="80898-186">OEM adı, seri numarası ve model birleşimini kullanmayı planlıyorsanız, bu sınırlamalara dikkat edin:</span><span class="sxs-lookup"><span data-stu-id="80898-186">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="80898-187">Bu tanımlama grubu yalnızca daha yeni cihazlar (örneğin, 4k karmaları) için geçerlidir ve 128b karmaları (RS2 ve önceki cihazlar) için desteklenmez.</span><span class="sxs-lookup"><span data-stu-id="80898-187">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="80898-188">Demet kaydı, büyük/küçük harfe duyarlıdır, bu nedenle dosyadaki verilerin, ***tam*** olarak OEM sağlayıcısı (donanım sağlayıcısı) tarafından sağlandığı şekilde model ve üretici adlarıyla eşleşmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="80898-188">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="80898-189">Iş Ortağı Merkezi 'nde bir müşterinin hesabına cihaz eklemek için aşağıdaki yönergeleri izleyin.</span><span class="sxs-lookup"><span data-stu-id="80898-189">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="80898-190">Iş Ortağı Merkezi menüsünden **müşteriler** ' i seçin ve ardından cihazlarını yönetmek istediğiniz müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="80898-190">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="80898-191">Müşterinin ayrıntı sayfasında **cihazlar** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="80898-191">On the customer's detail page, select **Devices** .</span></span>

3. <span data-ttu-id="80898-192">**Cihazlara profil Uygula** altında **Cihaz Ekle** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="80898-192">Under **Apply profiles to devices** select **Add devices** .</span></span>

4. <span data-ttu-id="80898-193">Cihaz listesi için bir ad girin ve ardından, müşteri listesini (. csv dosyası biçiminde) Iş Ortağı Merkezi 'ne yüklemek için **Gözden** geçirme ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="80898-193">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="80898-194">Bu. csv dosyasını cihazınızın satın alımından almış olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="80898-194">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="80898-195">Bir. csv dosyası almadıysanız, [Windows Autopilot 'a cihaz ekleme](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)adımlarını izleyerek kendiniz bir tane oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="80898-195">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="80898-196">. Csv dosyasını karşıya yükleyin ve ardından **Kaydet** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="80898-196">Upload the .csv file and then select **Save** .</span></span>

<span data-ttu-id="80898-197">Bir .csv dosyasını karşıya yüklemeye çalışırken hata iletisi alıyorsanız, dosyanın biçimini denetleyin.</span><span class="sxs-lookup"><span data-stu-id="80898-197">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="80898-198">Yalnızca donanım karmasını veya OEM adı, seri numarası ve model (bu sütun sırasıyla) veya Windows Ürün Kimliğini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="80898-198">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="80898-199">Cihaz listesi oluşturmak için cihaz **Ekle** ' nin yanındaki bağlantıdan sunulan Sample. csv dosyasını da kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="80898-199">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="80898-200">. Csv dosyanız şuna benzer görünmelidir:</span><span class="sxs-lookup"><span data-stu-id="80898-200">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="80898-201">**Cihaz seri numarası, Windows ürün KIMLIĞI, donanım karması, üretici adı, cihaz modeli**</span><span class="sxs-lookup"><span data-stu-id="80898-201">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="80898-202">**{serialNumber},,, Microsoft Corporation, Surface dizüstü bilgisayar**</span><span class="sxs-lookup"><span data-stu-id="80898-202">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="80898-203">"Üretici adı" ve "cihaz modeli" büyük/küçük harfe duyarlıdır.</span><span class="sxs-lookup"><span data-stu-id="80898-203">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="80898-204">Üretici adı ve cihaz modeli için hangi değeri koyacağınızı bilmiyorsanız, doğru değerleri toplamak için bunu cihazda çalıştırabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="80898-204">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="80898-205">Windows Autopilot EULA</span><span class="sxs-lookup"><span data-stu-id="80898-205">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="80898-206">ÖNEMLI BILGILER</span><span class="sxs-lookup"><span data-stu-id="80898-206">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="80898-207">Windows Autopilot, müşterileriniz için yönettiğiniz cihazlarda özelleştirilmiş Windows yüklemelerini yapılandırmanıza olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="80898-207">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="80898-208">Müşteri tarafından bu şekilde yetkilendirilirse, EULA (Son Kullanıcı Lisans Sözleşmesi) kabul ekranı dahil olmak üzere Windows 'u ayarlarken kullanıcılara sunulan belirli kurulum ekranlarını göstermez veya gizleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="80898-208">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="80898-209">Bu işlevi kullanarak, kullanıcılara bildirim veya koşulların kabul etmesini sağlamak için tasarlanan tüm ekranları gizlemeyi veya gizlemeyi kabul etmiş olursunuz. koşulları, müşterinizin adına (bir kuruluşun veya bireysel kullanıcı gibi), herhangi bir uyarıyı onaylamak ve müşteriniz için geçerli olan koşulları kabul etmek için müşterinize yeterli izin ve yetkilendirme elde ettiğinizi kabul edersiniz.</span><span class="sxs-lookup"><span data-stu-id="80898-209">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="80898-210">Bu, lisans hüküm ve koşullarına yönelik anlaşmayı ve bu aracı kullanarak gizlemeyin veya gizleyemediyseniz kullanıcıya sunulacak bildirimi içerir.</span><span class="sxs-lookup"><span data-stu-id="80898-210">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="80898-211">Müşteri, Microsoft 'tan veya lisanslı dağıtıcılarından yazılım için geçerli bir lisans almadıysanız, müşteriniz bu cihazlarda Windows yazılımlarını kullanmayabilir.</span><span class="sxs-lookup"><span data-stu-id="80898-211">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>