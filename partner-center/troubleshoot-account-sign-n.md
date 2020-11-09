---
title: Iş Ortağı Merkezi hesabınızı veya MPN yenileme sorunlarını ayarlamayla ilgili sorunları giderin
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Iş Ortağı Merkezi 'ne kaydolmaya çalışırken sorun giderin. Ödeme yöntemleriyle ilgili adres sorunlarını yanıtlar, parolaları öğrenme ve daha fazlasını yapın.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6bf3e3af8e0d1d87a63f86e892d8bddcd74b6460
ms.sourcegitcommit: 0e142b4fbb044fe8dd2dbc7d13ab70a1a91b9f60
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/09/2020
ms.locfileid: "94381418"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="bf384-104">Hesap kurulumu veya MPN yenileme sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="bf384-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="bf384-105">**Şunlara uygulanır**</span><span class="sxs-lookup"><span data-stu-id="bf384-105">**Applies to**</span></span>

- <span data-ttu-id="bf384-106">İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="bf384-106">Partner Center</span></span>
 
<span data-ttu-id="bf384-107">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="bf384-107">**Appropriate roles**</span></span>

- <span data-ttu-id="bf384-108">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="bf384-108">Global admin</span></span>
- <span data-ttu-id="bf384-109">MPN iş ortağı Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="bf384-109">MPN partner admin</span></span> 
 
<span data-ttu-id="bf384-110">Iş Ortağı Merkezi hesabınızı ayarlarken ortaya çıkan yaygın sorunları gidermeye yönelik bazı öneriler aşağıda verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="bf384-110">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="bf384-111">Iş ortağı üyelik merkezinden geçiş yapıyorsanız ve herhangi bir şirket bilgisi alanını düzenleyemezsiniz ne olur?</span><span class="sxs-lookup"><span data-stu-id="bf384-111">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="bf384-112">Şirketinizin zaten Iş Ortağı Merkezi 'nde (CSP hesabı söyleyin) mevcut olduğu durumlarda, salt okunurdur bir ekran gösterilir.</span><span class="sxs-lookup"><span data-stu-id="bf384-112">In cases where your company already has a presence in Partner Center (say CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="bf384-113">Bu ekranda, Iş Ortağı Merkezi 'nde olduğu gibi şirketiniz hakkındaki tüm bilgiler görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="bf384-113">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="bf384-114">Bu ekrandaki ayrıntıları değiştiremezsiniz.</span><span class="sxs-lookup"><span data-stu-id="bf384-114">You can't change the details on this screen.</span></span> <span data-ttu-id="bf384-115">Bu, tasarım ve bir hata değildir.</span><span class="sxs-lookup"><span data-stu-id="bf384-115">This is by design and not an error.</span></span>

<span data-ttu-id="bf384-116">**Kabul et** ' i seçin ve devam **edin** .</span><span class="sxs-lookup"><span data-stu-id="bf384-116">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="bf384-117">BT departmanı **Iş Ortağı Merkezi 'ne kaydolma** özelliğini devre dışı bıraktı.</span><span class="sxs-lookup"><span data-stu-id="bf384-117">If the IT department has turned off **sign up for Partner Center**.</span></span>

<span data-ttu-id="bf384-118">Bu iletiyi, viral kullanıcıları devre dışı bırakıldığı veya Azure AD kiracısında viral kaydolma devre dışı bırakıldığı için görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="bf384-118">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="bf384-119">Azure AD hesabınız için genel yönetici, aşağıdaki PowerShell komutunu çalıştırarak gerekli özellikleri etkinleştirebilir:</span><span class="sxs-lookup"><span data-stu-id="bf384-119">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="bf384-120">**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-Allowadhocabonelikleri $true**</span><span class="sxs-lookup"><span data-stu-id="bf384-120">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="bf384-121">Daha fazla bilgi için, [self servis kaydolma](/azure/active-directory/users-groups-roles/directory-self-service-signup) makalesini okuyun</span><span class="sxs-lookup"><span data-stu-id="bf384-121">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="bf384-122">Parolanızı unuttum</span><span class="sxs-lookup"><span data-stu-id="bf384-122">You forgot your password</span></span>

<span data-ttu-id="bf384-123">Parolanızı unuttuysanız, oturum açma sayfasında **hesabınıza erişemiyor musunuz?** bağlantısına tıklayın.</span><span class="sxs-lookup"><span data-stu-id="bf384-123">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="bf384-124">Bu seçenek, parolanızı sıfırlamanızı veya genel yöneticinizden size yeni kimlik bilgileri atamasını ister.</span><span class="sxs-lookup"><span data-stu-id="bf384-124">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="bf384-125">"Şirketiniz hakkında bize söyleyin" ekranında, "bir sorun oluştu" hatası alıyorsunuz</span><span class="sxs-lookup"><span data-stu-id="bf384-125">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="bf384-126">Bu hata iletisi genellikle şirket telefon numaranız için yanlışlıkla özel karakter, boşluk veya ülke kodu kullanıyorsanız görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="bf384-126">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="bf384-127">Telefon numarası alanına girilen değer yalnızca en fazla 10 karakter içerebilir.</span><span class="sxs-lookup"><span data-stu-id="bf384-127">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="bf384-128">Kredi kartı satın alma işlemi, "Siparişiniz reddedildi" iletisini bildiren bir hata mesajı alıyor.</span><span class="sxs-lookup"><span data-stu-id="bf384-128">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="bf384-129">Lütfen bilgilerinizi doğrulayın "</span><span class="sxs-lookup"><span data-stu-id="bf384-129">Please verify your information”</span></span>


<span data-ttu-id="bf384-130">Her zaman yasal varlığınızdan değil kredi kartınıza karşılık gelen adresi kullanın.</span><span class="sxs-lookup"><span data-stu-id="bf384-130">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="bf384-131">Ayrıca, ZIP kodunun doğru olduğundan ve kullandığınız adrese karşılık geldiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="bf384-131">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="bf384-132">Çevrimdışı ödeme 'den çevrimiçi ödeme yöntemine geçmek istiyorsunuz</span><span class="sxs-lookup"><span data-stu-id="bf384-132">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="bf384-133">Tercih edilen ödeme yöntemini kullanarak orijinal siparişi ve işlem yeniden Al işlemlerini iptal etmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="bf384-133">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="bf384-134">Bir siparişi iptal etmek için:</span><span class="sxs-lookup"><span data-stu-id="bf384-134">To cancel an order:</span></span>

1. <span data-ttu-id="bf384-135">Panoda **Üyelik teklifleri** sekmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="bf384-135">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="bf384-136">**Siparişi Iptal et** ' i seçin</span><span class="sxs-lookup"><span data-stu-id="bf384-136">Select **Cancel order**</span></span>

3. <span data-ttu-id="bf384-137">Bir onay penceresi görünür ve ilk siparişi iptal etmek için onaylamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="bf384-137">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="bf384-138">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="bf384-138">Next steps</span></span>

- [<span data-ttu-id="bf384-139">İş Ortağı Merkezi hesabınızı yönetme</span><span class="sxs-lookup"><span data-stu-id="bf384-139">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="bf384-140">Faturanızı ve keşfi dosyanızı okuma</span><span class="sxs-lookup"><span data-stu-id="bf384-140">How to read your bill and recon file</span></span>](read-your-bill.md)
