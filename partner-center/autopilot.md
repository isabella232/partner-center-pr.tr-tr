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
ms.openlocfilehash: 5294495403be729adecb5a7814ade4f9d454a0f6
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149834"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="d1660-103">Yeni cihazlarda Windows Otomatik Pilot profillerini kullanarak müşterinin kullanıma hazır deneyimini özelleştirme</span><span class="sxs-lookup"><span data-stu-id="d1660-103">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="d1660-104">**Uygun roller**: yönetici Aracısı | Genel yönetici | Satış Aracısı | Kullanıcı Yönetimi Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="d1660-104">**Appropriate roles**: Admin agent | Global admin | Sales agent | User management admin</span></span>

<span data-ttu-id="d1660-105">Müşteri cihazlarını yönetiyorsanız, müşterinin kullanıcıları için hazır olmayan deneyimi (OOBE) özelleştirmeniz gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="d1660-105">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="d1660-106">Cihazları müşterilere teslim etmeden önce Windows Autopilot profilleriyle yeni cihazları önceden yapılandırabilir ve müşterilerin zaten satın almış olduğu cihazlara yeni profiller uygulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d1660-106">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="d1660-107">OEM 'Lerin, cihazın **ürün anahtarı kimliğini (PKıD)** gösteren Autopilot cihaz kutusunun dışında bir sevkiyat etiketi de dahil başlatıldığını unutmayın.</span><span class="sxs-lookup"><span data-stu-id="d1660-107">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="d1660-108">Bu 1 boyutlu, okunabilir bir barkod, cihazların bir listesini kaldırmak zorunda kalmadan ve cihaz KIMLIĞINI alternatif yollarla ayırarak Autopilot için cihazları kaydetmek için bir yol ile aşağı akış ortakları sağlar.</span><span class="sxs-lookup"><span data-stu-id="d1660-108">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="d1660-109">Bu makalede, Autopilot profillerinin Iş Ortağı Merkezi 'nde cihazlara nasıl oluşturulacağı ve uygulanacağı açıklanır.</span><span class="sxs-lookup"><span data-stu-id="d1660-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="d1660-110">Zaten Autopilot hakkında bilgi sahibi değilseniz, bu makalelerdeki bilgileri gözden geçirin:</span><span class="sxs-lookup"><span data-stu-id="d1660-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="d1660-111">Windows Autopilot’a genel bakış</span><span class="sxs-lookup"><span data-stu-id="d1660-111">Overview of Windows Autopilot</span></span>](/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="d1660-112">Autopilot dağıtım başvurusu Kılavuzu</span><span class="sxs-lookup"><span data-stu-id="d1660-112">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="d1660-113">Genel Bakış</span><span class="sxs-lookup"><span data-stu-id="d1660-113">Overview</span></span>

<span data-ttu-id="d1660-114">Iş Ortağı Merkezi 'ndeki Windows Autopilot özelliği ile müşteri cihazlarına uygulanacak özel profiller oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d1660-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="d1660-115">Aşağıdaki profil ayarları, bu makalenin yayımlandığı sırada mevcuttur:</span><span class="sxs-lookup"><span data-stu-id="d1660-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="d1660-116">Gizlilik ayarlarını atlayın.</span><span class="sxs-lookup"><span data-stu-id="d1660-116">Skip privacy settings.</span></span> <span data-ttu-id="d1660-117">Bu isteğe bağlı Autopilot profili ayarı, kuruluşların OOBE işlemi sırasında gizlilik ayarlarını istememesini sağlar.</span><span class="sxs-lookup"><span data-stu-id="d1660-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="d1660-118">Cihazda yerel yönetici hesabı oluşturmayı devre dışı bırakın.</span><span class="sxs-lookup"><span data-stu-id="d1660-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="d1660-119">Kuruluşlar, işlem tamamlandıktan sonra cihazı ayarlamaya yönelik kullanıcının yönetici erişimine sahip olup olmadığına karar verebilir.</span><span class="sxs-lookup"><span data-stu-id="d1660-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="d1660-120">Cihazı iş veya okul için otomatik olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="d1660-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="d1660-121">Autopilot ile kaydedilen tüm cihazlar otomatik olarak iş veya okul cihazları olarak kabul edilir. bu nedenle, bu soru, OOBE işlemi sırasında istenmez.</span><span class="sxs-lookup"><span data-stu-id="d1660-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="d1660-122">Cortana, OneDrive ve OEM kayıt kurulum sayfalarını atlayın.</span><span class="sxs-lookup"><span data-stu-id="d1660-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="d1660-123">Autopilot'a kayıtlı tüm cihazlar, ilk deneyim (OOBE) işlemi sırasında bu sayfaları otomatik olarak atlar.</span><span class="sxs-lookup"><span data-stu-id="d1660-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="d1660-124">Son Kullanıcı Lisans Sözleşmesi'ne (EULA) atla.</span><span class="sxs-lookup"><span data-stu-id="d1660-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="d1660-125">1709 Windows 10 başlayarak, kuruluşlar OOBE işlemi sırasında sunulan EULA sayfasını atlamayı karar kabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d1660-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="d1660-126">Windows [Windows Autopilot EULA sayfasını atlama hakkında](#windows-autopilot-eula-dismissal) dikkate alınması gereken önemli bilgiler için aşağıdaki EULA'yı çıkarma sayfasına bakın.</span><span class="sxs-lookup"><span data-stu-id="d1660-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="d1660-127">Aşağıdaki profil ve cihaz yönetim izinleri ve sınırlamaları geçerlidir:</span><span class="sxs-lookup"><span data-stu-id="d1660-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="d1660-128">CSP iş ortakları aralarında bayi ilişkileri olan mevcut müşteriler için, müşteri iş ortağının temsilci yönetim ayrıcalıklarını kaldırmış olsa bile, Otomatik Pilot profillerini yönetmeye devam edebilir.</span><span class="sxs-lookup"><span data-stu-id="d1660-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="d1660-129">Müşterilerinizin eklediği mevcut cihazları müşterileriniz için yönetebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d1660-129">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="d1660-130">Müşterinizin Microsoft Store İş'e veya Microsoft Intune Portalına yüklediği cihazları yönetemezsiniz.</span><span class="sxs-lookup"><span data-stu-id="d1660-130">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="d1660-131">İş Ortağı Merkezi'da Autopilot profilleri oluşturma ve yönetme</span><span class="sxs-lookup"><span data-stu-id="d1660-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="d1660-132">Bu İş Ortağı Merkezi, dağıtım Windows Autopilot oluşturabilir ve bunları cihazlara uygulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d1660-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="d1660-133">Profiller yalnızca yönetici aracıları oluşturabilir ve uygulayabilir.</span><span class="sxs-lookup"><span data-stu-id="d1660-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="d1660-134">Yeni bir Autopilot profili oluşturma</span><span class="sxs-lookup"><span data-stu-id="d1660-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="d1660-135">İş Ortağı Merkezi  menüsünden Müşteriler'i seçin ve ardından Autopilot profilini oluşturmakta olduğunu müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="d1660-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="d1660-136">Müşterinin ayrıntı sayfasında Cihazlar'ı **seçin.**</span><span class="sxs-lookup"><span data-stu-id="d1660-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="d1660-137">Profil **Windows Autopilot altında Yeni profil** **ekle'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="d1660-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="d1660-138">Profilin adını ve açıklamasını girin ve ardından OOBE ayarlarını yapılandırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d1660-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="d1660-139">Aşağıdakilerden birini seçin:</span><span class="sxs-lookup"><span data-stu-id="d1660-139">Choose from:</span></span>  

   - <span data-ttu-id="d1660-140">Kurulumda gizlilik ayarlarını atla</span><span class="sxs-lookup"><span data-stu-id="d1660-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="d1660-141">Kurulumda yerel yönetici hesabını devre dışı bırakma</span><span class="sxs-lookup"><span data-stu-id="d1660-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="d1660-142">Kurulumda sayfaları otomatik olarak atlama</span><span class="sxs-lookup"><span data-stu-id="d1660-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="d1660-143">(İş *veya okul için kurulumu otomatik olarak seçme ve* Cortana, OneDrive ve OEM kayıt kurulum sayfalarını *atla'yı içerir)*</span><span class="sxs-lookup"><span data-stu-id="d1660-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="d1660-144">Son kullanıcı lisans sözleşmelerini (EULA) atla</span><span class="sxs-lookup"><span data-stu-id="d1660-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="d1660-145">Windows [Windows Autopilot EULA sayfasını atlama hakkında](#windows-autopilot-eula-dismissal) dikkate alınması gereken önemli bilgiler için aşağıdaki EULA'yı çıkarma sayfasına bakın.</span><span class="sxs-lookup"><span data-stu-id="d1660-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="d1660-146">Tamamlandığında **Gönder'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="d1660-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="d1660-147">Müşteri cihazlarına Autopilot profili uygulama</span><span class="sxs-lookup"><span data-stu-id="d1660-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="d1660-148">Aşağıdaki yönergelerde, müşterinin cihazlarını Iş Ortağı Merkezi 'ne eklediğiniz ve cihaz listesine erişebileceğiniz varsayılmaktadır.</span><span class="sxs-lookup"><span data-stu-id="d1660-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="d1660-149">Müşterinin cihazlarını henüz eklemediyseniz, [müşterinin hesabına cihaz ekleme](#add-devices-to-a-customers-account) ' deki yönergeleri izleyin ve ardından aşağıdaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="d1660-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="d1660-150">Bir müşteri için Autopilot profili oluşturduktan sonra, bunu müşterinin cihazlarına uygulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d1660-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="d1660-151">Iş Ortağı Merkezi menüsünden **müşteriler** ' i seçin ve ardından Autopilot profilini oluşturduğunuz müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="d1660-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="d1660-152">Müşterinin ayrıntı sayfasında **cihazlar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="d1660-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="d1660-153">**Cihazları cihazlara Uygula** altında, profil eklemek istediğiniz cihazları veya cihaz gruplarını seçin ve ardından **profili Uygula**' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="d1660-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="d1660-154">Yeni uyguladığınız profil **profil** sütununda görünür.</span><span class="sxs-lookup"><span data-stu-id="d1660-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="d1660-155">Profilin cihaza başarıyla uygulanacağını doğrulamak için aşağıdaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="d1660-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="d1660-156">a.</span><span class="sxs-lookup"><span data-stu-id="d1660-156">a.</span></span>  <span data-ttu-id="d1660-157">Bir cihazı ağa bağlayın ve açın.</span><span class="sxs-lookup"><span data-stu-id="d1660-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="d1660-158">b.</span><span class="sxs-lookup"><span data-stu-id="d1660-158">b.</span></span>  <span data-ttu-id="d1660-159">Uygun OOBE ekranlarının (varsa) göründüğünü doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="d1660-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="d1660-160">c.</span><span class="sxs-lookup"><span data-stu-id="d1660-160">c.</span></span>  <span data-ttu-id="d1660-161">OOBE işlemi durdurulduğunda, yeni bir kullanıcı için hazırlamak üzere cihazı fabrika varsayılan ayarlarına sıfırlayın.</span><span class="sxs-lookup"><span data-stu-id="d1660-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="d1660-162">Bir Autopilot profilini müşterinin cihazından kaldırma</span><span class="sxs-lookup"><span data-stu-id="d1660-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="d1660-163">Iş Ortağı Merkezi menüsünden **müşteriler** ' i seçin ve ardından Autopilot profilini oluşturduğunuz müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="d1660-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="d1660-164">Müşterinin ayrıntı sayfasında **cihazlar**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="d1660-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="d1660-165">**Cihazlara profilleri Uygula** altında, profili kaldırmak istediğiniz cihazları seçin ve ardından **Profili Kaldır**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="d1660-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="d1660-166">Bir cihazın cihazdan kaldırılması, profili listenizden silmez.</span><span class="sxs-lookup"><span data-stu-id="d1660-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="d1660-167">Bir profili silmek istiyorsanız, [Autopilot profilini güncelleştirme veya silme](#update-or-delete-an-autopilot-profile)bölümündeki yönergeleri izleyin.</span><span class="sxs-lookup"><span data-stu-id="d1660-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="d1660-168">Autopilot profilini güncelleştirme veya silme</span><span class="sxs-lookup"><span data-stu-id="d1660-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="d1660-169">Müşteriler cihazları gönderdikten sonra, kullanıma hazır deneyimini değiştirmek isterse, Iş Ortağı Merkezi ' nde profili değiştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d1660-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="d1660-170">Müşterinin cihazı internet 'e bağlandığı zaman, OOBE işlemi sırasında en son profil sürümünü indirir.</span><span class="sxs-lookup"><span data-stu-id="d1660-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="d1660-171">Ayrıca, bir müşteri bir cihazı fabrika varsayılan ayarlarına geri yükleyene kadar, OOBE işlemi sırasında cihaz yeniden en son profil sürümünü indirir.</span><span class="sxs-lookup"><span data-stu-id="d1660-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="d1660-172">İş Ortağı Merkezi  menüsünden Müşteriler'i seçin ve ardından Autopilot profilini değiştirmenizi isteyen müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="d1660-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="d1660-173">Müşterinin ayrıntı sayfasında Cihazlar'ı **seçin.**</span><span class="sxs-lookup"><span data-stu-id="d1660-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="d1660-174">**Profiller Windows Autopilot altında** güncelleştirmeniz gereken profili seçin.</span><span class="sxs-lookup"><span data-stu-id="d1660-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="d1660-175">Gerekli değişiklikleri yapın ve gönder'i **seçin.**</span><span class="sxs-lookup"><span data-stu-id="d1660-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="d1660-176">Bu profili silmek için sayfanın **sağ üst** köşesinden Profili sil'i seçin.</span><span class="sxs-lookup"><span data-stu-id="d1660-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="d1660-177">Müşterinin hesabına cihaz ekleme</span><span class="sxs-lookup"><span data-stu-id="d1660-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="d1660-178">Satış temsilcileri ve yönetici temsilcileri, bir müşterinin hesabına cihaz ekleyebilir.</span><span class="sxs-lookup"><span data-stu-id="d1660-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="d1660-179">Müşteri cihazlarına özel Autopilot profilleri uygulayamadan önce müşterinin cihaz listesine erişebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d1660-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="d1660-180">OEM adını, seri numarasını ve model birleşimini kullanmayı planlıyorsanız şu sınırlamalara dikkat edin:</span><span class="sxs-lookup"><span data-stu-id="d1660-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="d1660-181">Bu tuple yalnızca daha yeni cihazlarda (örneğin 4k karmalar) çalışır ve 128b karmalar (RS2 ve önceki cihazlar) için desteklanmaz.</span><span class="sxs-lookup"><span data-stu-id="d1660-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="d1660-182">Kayıt, büyük/büyük/büyük harfe duyarlıdır, bu nedenle dosyada yer alan verilerin, OEM sağlayıcısı (donanım sağlayıcısı) tarafından sağlanan model ve üretici adlarına tam olarak eşleşmesi gerekir. </span><span class="sxs-lookup"><span data-stu-id="d1660-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="d1660-183">Aşağıdaki yönergeleri izleyerek cihazları bir müşterinin hesabıyla İş Ortağı Merkezi.</span><span class="sxs-lookup"><span data-stu-id="d1660-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="d1660-184">İş Ortağı Merkezi  menüsünden Müşteriler'i seçin ve ardından cihazlarını yönetmek istediğiniz müşteriyi seçin.</span><span class="sxs-lookup"><span data-stu-id="d1660-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="d1660-185">Müşterinin ayrıntı sayfasında Cihazlar'ı **seçin.**</span><span class="sxs-lookup"><span data-stu-id="d1660-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="d1660-186">Cihazlara **profil uygula altında Cihaz ekle'yi** **seçin.**</span><span class="sxs-lookup"><span data-stu-id="d1660-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="d1660-187">Cihaz listesi için bir ad  girin ve ardından Gözat'ı seçerek müşterinin listesini (.csv dosya biçiminde) İş Ortağı Merkezi.</span><span class="sxs-lookup"><span data-stu-id="d1660-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="d1660-188">Bu .csv dosyasını cihaz satın alma ile almış olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="d1660-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="d1660-189">Bir .csv dosyası almadıysanız, Bir .csv dosyasına cihaz ekleme'de yer alan [adımları Windows Autopilot.](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="d1660-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="d1660-190">.csv dosyasını karşıya yükleyin ve Kaydet'i **seçin.**</span><span class="sxs-lookup"><span data-stu-id="d1660-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="d1660-191">Bir .csv dosyasını karşıya yüklemeye çalışırken hata iletisi alıyorsanız, dosyanın biçimini denetleyin.</span><span class="sxs-lookup"><span data-stu-id="d1660-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="d1660-192">Yalnızca donanım karmasını veya OEM adı, seri numarası ve model (bu sütun sırasıyla) veya Windows Ürün Kimliğini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d1660-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="d1660-193">Cihaz listesi oluşturmak için cihaz **Ekle** ' nin yanındaki bağlantıdan sunulan Sample. csv dosyasını da kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d1660-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="d1660-194">. Csv dosyanız şuna benzer görünmelidir:</span><span class="sxs-lookup"><span data-stu-id="d1660-194">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="d1660-195">**Cihaz seri numarası, Windows ürün KIMLIĞI, donanım karması, üretici adı, cihaz modeli**</span><span class="sxs-lookup"><span data-stu-id="d1660-195">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="d1660-196">**{serialNumber},,, Microsoft Corporation, Surface dizüstü bilgisayar**</span><span class="sxs-lookup"><span data-stu-id="d1660-196">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="d1660-197">"Üretici adı" ve "cihaz modeli" büyük/küçük harfe duyarlıdır.</span><span class="sxs-lookup"><span data-stu-id="d1660-197">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="d1660-198">Üretici adı ve cihaz modeli için hangi değeri koyacağınızı bilmiyorsanız, doğru değerleri toplamak için bunu cihazda çalıştırabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="d1660-198">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="d1660-199">Windows Autopilot EULA</span><span class="sxs-lookup"><span data-stu-id="d1660-199">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="d1660-200">ÖNEMLI BILGILER</span><span class="sxs-lookup"><span data-stu-id="d1660-200">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="d1660-201">Windows Autopilot, müşterileriniz için yönettiğiniz cihazlarda özelleştirilmiş Windows yüklemelerini yapılandırmanıza olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="d1660-201">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="d1660-202">Müşteri tarafından bu şekilde yetkilendirilirse, EULA (Son Kullanıcı Lisans Sözleşmesi) kabul ekranı dahil olmak üzere Windows 'u ayarlarken kullanıcılara sunulan belirli kurulum ekranlarını göstermez veya gizleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d1660-202">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="d1660-203">Bu işlevi kullanarak, kullanıcılara bildirim veya koşulların kabul etmesini sağlamak için tasarlanan tüm ekranları gizlemeyi veya gizlemeyi kabul etmiş olursunuz. koşulları, müşterinizin adına (bir kuruluşun veya bireysel kullanıcı gibi), herhangi bir uyarıyı onaylamak ve müşteriniz için geçerli olan koşulları kabul etmek için müşterinize yeterli izin ve yetkilendirme elde ettiğinizi kabul edersiniz.</span><span class="sxs-lookup"><span data-stu-id="d1660-203">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="d1660-204">Bu, lisans hüküm ve koşullarına yönelik anlaşmayı ve bu aracı kullanarak gizlemeyin veya gizleyemediyseniz kullanıcıya sunulacak bildirimi içerir.</span><span class="sxs-lookup"><span data-stu-id="d1660-204">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="d1660-205">Müşteri, Microsoft 'tan veya lisanslı dağıtıcılarından yazılım için geçerli bir lisans almadıysanız, müşteriniz bu cihazlarda Windows yazılımlarını kullanmayabilir.</span><span class="sxs-lookup"><span data-stu-id="d1660-205">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>