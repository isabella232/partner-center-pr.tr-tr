---
title: İş Ortağı Merkezi veya MPN yenileme sorunlarınızı giderme
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: İş Ortağı Merkezi'a kaydolmaya çalışırken ortaya İş Ortağı Merkezi. Ödeme yöntemleriyle ilgili zorlukları, parolaları unutmayı ve daha fazlasını yanıtlar.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a5e8a292ad8593dc0b94179d5f0ee418344ef9af
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854698"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="2d4b4-104">Hesap kurulumu veya MPN yenileme sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="2d4b4-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="2d4b4-105">**Uygun roller:** Genel yönetici | MPN iş ortağı yöneticisi</span><span class="sxs-lookup"><span data-stu-id="2d4b4-105">**Appropriate roles**: Global admin | MPN partner admin</span></span>
 
<span data-ttu-id="2d4b4-106">Burada, İş Ortağı Merkezi hesabınız ayarlarken ortaya çıkan yaygın sorunları gidermeye yönelik İş Ortağı Merkezi vardır.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-106">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="2d4b4-107">Şirket dışından Partner Membership Center şirket bilgileri alanlarını düzenleyemeyebilirsiniz</span><span class="sxs-lookup"><span data-stu-id="2d4b4-107">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="2d4b4-108">Şirket içinde zaten bir İş Ortağı Merkezi (csP hesabı gibi) olduğu durumlarda, salt okunur bir ekran gösterilir.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-108">In cases where your company already has a presence in Partner Center (for example, a CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="2d4b4-109">Bu ekranda, şirketle ilgili tüm bilgiler şirket içinde mevcut İş Ortağı Merkezi.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-109">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="2d4b4-110">Bu ekranda ayrıntıları değiştiremezsiniz.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-110">You can't change the details on this screen.</span></span> <span data-ttu-id="2d4b4-111">Bu bir hata değil, tasarıma göredir.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-111">This is by design and not an error.</span></span>

<span data-ttu-id="2d4b4-112">Devam etmek **için Kabul** Et ve **Devam Et'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-112">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="2d4b4-113">IT departmanı Kayıt için **kaydolmayı İş Ortağı Merkezi**</span><span class="sxs-lookup"><span data-stu-id="2d4b4-113">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="2d4b4-114">Bu iletiyi, virüslü kullanıcılar devre dışı bırakıldıklarında veya Azure AD kiracısı üzerinde Viral Kayıt devre dışı bırakıldıklarında görüyorsunuz.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-114">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="2d4b4-115">Azure AD hesabınıza yönelik Genel yönetici, aşağıdaki PowerShell komutunu çalıştırarak gerekli özellikleri etkinleştirebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="2d4b4-115">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="2d4b4-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="2d4b4-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="2d4b4-117">Daha fazla bilgi için [self servis kaydolma makalelerini okuyun.](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="2d4b4-117">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="2d4b4-118">Parolanızı unuttunız</span><span class="sxs-lookup"><span data-stu-id="2d4b4-118">You forgot your password</span></span>

<span data-ttu-id="2d4b4-119">Parolanızı unuttuysanız oturum açma **sayfasındaki Hesabınıza erişe miyim?** bağlantısını seçin.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-119">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="2d4b4-120">Bu seçenek parolanızı sıfırlamanıza veya Genel yöneticinizden size yeni kimlik bilgileri atamasını istemenize olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-120">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="2d4b4-121">"Şirketiniz hakkında bize söyleyin" ekranında, "bir sorun oluştu" hatası alıyorsunuz</span><span class="sxs-lookup"><span data-stu-id="2d4b4-121">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="2d4b4-122">Bu hata iletisi genellikle şirket telefon numaranız için yanlışlıkla özel karakter, boşluk veya ülke kodu kullanıyorsanız görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-122">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="2d4b4-123">Telefon numarası alanına girilen değer yalnızca en fazla 10 karakter içerebilir.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-123">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="2d4b4-124">Kredi kartı satın alma işlemi, "Siparişiniz reddedildi" iletisini bildiren bir hata mesajı alıyor.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-124">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="2d4b4-125">Lütfen bilgilerinizi doğrulayın "</span><span class="sxs-lookup"><span data-stu-id="2d4b4-125">Please verify your information”</span></span>


<span data-ttu-id="2d4b4-126">Her zaman yasal varlığınızdan değil kredi kartınıza karşılık gelen adresi kullanın.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-126">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="2d4b4-127">Ayrıca, ZIP kodunun doğru olduğundan ve kullandığınız adrese karşılık geldiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-127">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="2d4b4-128">Çevrimdışı ödeme 'den çevrimiçi ödeme yöntemine geçmek istiyorsunuz</span><span class="sxs-lookup"><span data-stu-id="2d4b4-128">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="2d4b4-129">Tercih edilen ödeme yöntemini kullanarak orijinal siparişi ve işlem yeniden Al işlemlerini iptal etmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-129">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="2d4b4-130">Bir siparişi iptal etmek için:</span><span class="sxs-lookup"><span data-stu-id="2d4b4-130">To cancel an order:</span></span>

1. <span data-ttu-id="2d4b4-131">Panoda **Üyelik teklifleri** sekmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-131">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="2d4b4-132">**Siparişi Iptal et** ' i seçin</span><span class="sxs-lookup"><span data-stu-id="2d4b4-132">Select **Cancel order**</span></span>

3. <span data-ttu-id="2d4b4-133">Bir onay penceresi görünür ve ilk siparişi iptal etmek için onaylamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-133">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2d4b4-134">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="2d4b4-134">Next steps</span></span>

- [<span data-ttu-id="2d4b4-135">İş Ortağı Merkezi hesabınızı yönetme</span><span class="sxs-lookup"><span data-stu-id="2d4b4-135">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="2d4b4-136">Faturanızı ve keşfi dosyanızı okuma</span><span class="sxs-lookup"><span data-stu-id="2d4b4-136">How to read your bill and recon file</span></span>](read-your-bill.md)
