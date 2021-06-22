---
title: İş Ortağı Merkezi veya MPN yenileme sorunlarınızı giderme
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: İş Ortağı Merkezi'a kaydolmaya çalışırken ortaya İş Ortağı Merkezi. Ödeme yöntemleri, parolaları unutma ve daha fazlası ile ilgili zorlukların yanıtlarını verir.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4fc1a43b4d525d9221ac7e4db56f5f278404e3f5
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431762"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="54bf3-104">Hesap kurulumu veya MPN yenileme sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="54bf3-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="54bf3-105">**Uygun roller:** Genel yönetici | MPN iş ortağı yöneticisi</span><span class="sxs-lookup"><span data-stu-id="54bf3-105">**Appropriate roles**: Global admin | MPN partner admin</span></span>
 
<span data-ttu-id="54bf3-106">Burada, İş Ortağı Merkezi hesabınız ayarlarken ortaya çıkan yaygın sorunları gidermek için İş Ortağı Merkezi edinebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="54bf3-106">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="54bf3-107">Şirket dışından Partner Membership Center şirket bilgileri alanlarını düzenleyemeyebilirsiniz</span><span class="sxs-lookup"><span data-stu-id="54bf3-107">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="54bf3-108">Şirket içinde zaten bir İş Ortağı Merkezi (Bulut Çözümü Sağlayıcısı (CSP) hesabı) olduğu durumlarda, salt okunur bir ekran gösterilir.</span><span class="sxs-lookup"><span data-stu-id="54bf3-108">In cases where your company already has a presence in Partner Center (for example, a Cloud Solution Provider (CSP) account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="54bf3-109">Bu ekranda, şirketle ilgili tüm bilgiler şirket içinde mevcut İş Ortağı Merkezi.</span><span class="sxs-lookup"><span data-stu-id="54bf3-109">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="54bf3-110">Bu ekranda ayrıntıları değiştiremezsiniz.</span><span class="sxs-lookup"><span data-stu-id="54bf3-110">You can't change the details on this screen.</span></span> <span data-ttu-id="54bf3-111">Bu bir hata değil, tasarıma göredir.</span><span class="sxs-lookup"><span data-stu-id="54bf3-111">This is by design and not an error.</span></span>

<span data-ttu-id="54bf3-112">Devam etmek için Kabul **Et'i** ve ardından Devam'ı **seçin.**</span><span class="sxs-lookup"><span data-stu-id="54bf3-112">To proceed, select **Accept**, and then select **Continue**.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="54bf3-113">IT departmanı Kayıt için **kaydolmayı İş Ortağı Merkezi**</span><span class="sxs-lookup"><span data-stu-id="54bf3-113">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="54bf3-114">Bu iletiyi, virüslü kullanıcılar devre dışı bırakıldıklarında veya Virüslü Kayıt Azure Active Directory (AD) kiracıda devre dışı bırakılmıştır.</span><span class="sxs-lookup"><span data-stu-id="54bf3-114">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure Active Directory (AD) tenant.</span></span> <span data-ttu-id="54bf3-115">Azure AD hesabınıza yönelik Genel yönetici, aşağıdaki PowerShell komutunu çalıştırarak gerekli özellikleri etkinleştirebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="54bf3-115">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="54bf3-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="54bf3-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="54bf3-117">Daha fazla bilgi için [self servis kaydolma makalelerini okuyun.](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="54bf3-117">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="54bf3-118">Parolanızı unuttunız</span><span class="sxs-lookup"><span data-stu-id="54bf3-118">You forgot your password</span></span>

<span data-ttu-id="54bf3-119">Parolanızı unuttuysanız oturum açma sayfasında Hesabınıza erişe **miyim? öğesini seçin.**</span><span class="sxs-lookup"><span data-stu-id="54bf3-119">If you have forgotten your password, on the sign-in page, select **Can't access your account?**.</span></span> <span data-ttu-id="54bf3-120">Bu seçenek parolanızı sıfırlamanıza veya Genel yöneticinizden size yeni kimlik bilgileri atamasını istemenize olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="54bf3-120">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="54bf3-121">"Bize şirketinizi söyleyin" ekranında "Bir sorun oluştu" hatasını alısınız</span><span class="sxs-lookup"><span data-stu-id="54bf3-121">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="54bf3-122">Bu hata iletisi genellikle şirket telefon numaranıza yanlışlıkla özel karakterler, boşluklar veya ülke kodu kullanıyorsanız ortaya çıktı.</span><span class="sxs-lookup"><span data-stu-id="54bf3-122">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="54bf3-123">Telefon Numarası alanına girilen değer yalnızca en fazla 10 karakter içerebilir.</span><span class="sxs-lookup"><span data-stu-id="54bf3-123">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="54bf3-124">Kredi kartı satın alma sırasında "Siparişiniz reddedildi.</span><span class="sxs-lookup"><span data-stu-id="54bf3-124">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="54bf3-125">Lütfen bilginizi doğrulayın"</span><span class="sxs-lookup"><span data-stu-id="54bf3-125">Please verify your information”</span></span>


<span data-ttu-id="54bf3-126">Yasal varlığınız yerine her zaman kredi kartınıza karşılık gelen adresi kullanın.</span><span class="sxs-lookup"><span data-stu-id="54bf3-126">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="54bf3-127">Ayrıca posta kodunun doğru olduğundan ve kullanmakta olduğunuz adrese karşılık gelen bir adres olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="54bf3-127">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="54bf3-128">Çevrimdışı ödemeden çevrimiçi ödeme yöntemine geçmek istiyorsanız</span><span class="sxs-lookup"><span data-stu-id="54bf3-128">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="54bf3-129">Özgün siparişi iptal etmeniz ve tercih edilen ödeme yöntemini kullanarak yeniden satın alasanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="54bf3-129">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="54bf3-130">Siparişi iptal etmek için:</span><span class="sxs-lookup"><span data-stu-id="54bf3-130">To cancel an order:</span></span>

1. <span data-ttu-id="54bf3-131">Yeni İş Ortağı Merkezi Üyelik Teklifleri **sekmesini** seçin.</span><span class="sxs-lookup"><span data-stu-id="54bf3-131">In the Partner Center dashboard, select the **Membership Offers** tab.</span></span>

2. <span data-ttu-id="54bf3-132">Siparişi **iptal et'i seçin**</span><span class="sxs-lookup"><span data-stu-id="54bf3-132">Select **Cancel order**</span></span>

3. <span data-ttu-id="54bf3-133">Bir onay penceresi görüntülenir ve ilk siparişi iptal etmek için onaylamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="54bf3-133">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="54bf3-134">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="54bf3-134">Next steps</span></span>

- [<span data-ttu-id="54bf3-135">İş Ortağı Merkezi hesabınızı yönetme</span><span class="sxs-lookup"><span data-stu-id="54bf3-135">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="54bf3-136">Faturanızı ve mutabakat dosyanızı okuma</span><span class="sxs-lookup"><span data-stu-id="54bf3-136">How to read your bill and recon file</span></span>](read-your-bill.md)
