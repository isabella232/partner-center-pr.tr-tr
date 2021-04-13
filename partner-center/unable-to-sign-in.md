---
title: Iş Ortağı Merkezi 'nde oturum açılamıyor
ms.topic: troubleshooting
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Olası nedenlerde sorun giderin ve Iş Ortağı Merkezi 'nde oturum açamıyorum çözümler hakkında bilgi edinin. parolaları sıfırlama, rolleri denetleme ve kimlik bilgilerini denetleme hakkında daha fazla bilgi edinin.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 17087727afcaf3dbcf47801f8668388c370758e7
ms.sourcegitcommit: 9b04509f3830462628c1bb6af2ca41ed68b52619
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/09/2021
ms.locfileid: "107266580"
---
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a><span data-ttu-id="c399a-103">Iş Ortağı Merkezi için oturum açma sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="c399a-103">Troubleshoot sign-in issues for Partner Center</span></span>

<span data-ttu-id="c399a-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="c399a-104">**Appropriate roles**</span></span>

- <span data-ttu-id="c399a-105">Iş Ortağı Merkezi ile ilgilenen tüm iş ortakları</span><span class="sxs-lookup"><span data-stu-id="c399a-105">All partners interested in Partner Center</span></span>

<span data-ttu-id="c399a-106">Bu makale, Iş Ortağı Merkezi için ortak oturum açma sorunlarına yönelik çözümler içerir.</span><span class="sxs-lookup"><span data-stu-id="c399a-106">This article contains solutions for common sign-in issues for Partner Center.</span></span>

## <a name="youve-forgotten-your-password-for-partner-center"></a><span data-ttu-id="c399a-107">Iş Ortağı Merkezi için parolanızı unuttunuz</span><span class="sxs-lookup"><span data-stu-id="c399a-107">You've forgotten your password for Partner Center</span></span>

<span data-ttu-id="c399a-108">Parolanızı unuttuysanız ve Iş Ortağı Merkezi 'Nde oturum açamıyor, desteğe başvurun.</span><span class="sxs-lookup"><span data-stu-id="c399a-108">If you have forgotten your password and can't sign into Partner Center, contact Support.</span></span> <span data-ttu-id="c399a-109">[Iş ürünleri Için desteğe](/microsoft-365/admin/contact-support-for-business-products)uygun kişiyi bulun.</span><span class="sxs-lookup"><span data-stu-id="c399a-109">Find the appropriate contact at [Support for Business Products](/microsoft-365/admin/contact-support-for-business-products).</span></span>

<span data-ttu-id="c399a-110">Bir MPN iş ortağıysanız, genel yöneticinizden sizin için yeni bir parola oluşturmasını isteyin.</span><span class="sxs-lookup"><span data-stu-id="c399a-110">If you're an MPN partner, ask your Global admin to create a new password for you.</span></span> <span data-ttu-id="c399a-111">Bir CSP dolaylı satıcısıysanız, dolaylı sağlayıcınızı Azure AD kiracınızda sizin için yeni bir genel yönetici oluşturmasını isteyin veya Temsilcili yönetici ayrıcalıklarını kullanarak sizin için yeni bir parola oluşturun.</span><span class="sxs-lookup"><span data-stu-id="c399a-111">If you're a CSP Indirect reseller, ask your Indirect provider to create a new Global admin for you on your Azure AD tenant or create a new password for you using their delegated admin privileges.</span></span>

<span data-ttu-id="c399a-112">Parolanızı nasıl sıfırlayabileceğinizi ve iş hesabınıza yeniden erişiminizi geri kazanmak için [güvenlik bilgilerini kullanarak iş veya okul parolanızı sıfırlayın](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password)makalesini okuyun.</span><span class="sxs-lookup"><span data-stu-id="c399a-112">To learn more about how you can reset your password and regain access to your work account, read [Reset your work or school password using security info](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password).</span></span>

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a><span data-ttu-id="c399a-113">Iş Ortağı Merkezi 'nde beklenen sayfaları veya özellikleri görüntüleyemez veya yönetemezsiniz</span><span class="sxs-lookup"><span data-stu-id="c399a-113">You can't view or manage the expected pages or capabilities in Partner Center</span></span>

<span data-ttu-id="c399a-114">Iş Ortağı Merkezi 'ndeki sayfalara erişim, atadığınız roller tarafından denetlenir.</span><span class="sxs-lookup"><span data-stu-id="c399a-114">Access to pages in Partner Center is controlled by the roles that you're assigned.</span></span> <span data-ttu-id="c399a-115">Hangi rollerin atandığını denetlemek için Iş Ortağı Merkezi ' nde ayarlar simgesini seçin, **Hesap ayarları**' nı seçin ve ardından hesap ayarları ' nda **Kullanıcı yönetimi**' ni seçin.</span><span class="sxs-lookup"><span data-stu-id="c399a-115">To check which roles you're assigned, in Partner Center select the Settings icon, select **Account settings**, and then in Account settings, select **User management**.</span></span> <span data-ttu-id="c399a-116">Ara alanına adınızı yazın ve ardından sonuçları görüntüleyin.</span><span class="sxs-lookup"><span data-stu-id="c399a-116">In Search, type your name and then view the results.</span></span>

<span data-ttu-id="c399a-117">İstediğiniz Uzmanlıklar, müşteriler, teşvikleri veya kullanıcıları görüntüleyebilmemişse veya yönetebiliyorsanız, aşağıdaki çözümleri deneyin:</span><span class="sxs-lookup"><span data-stu-id="c399a-117">If you aren't able to view or manage the competencies, customers, incentives, or users that you expect, try the following solutions:</span></span>

- <span data-ttu-id="c399a-118">MPN, CSP ve başvuruların özelliklerine erişim için, genel yönetici veya hesap yöneticinizle görüşün. Roller ve Iş Ortağı Merkezi 'nde etkinleştirildikleri görevler hakkında daha fazla bilgi edinmek için bkz. [kullanıcılara rol & Izinleri atama](permissions-overview.md).</span><span class="sxs-lookup"><span data-stu-id="c399a-118">For access to the capabilities of MPN, CSP, and Referrals, contact your Global admin or Account admin. To learn more about roles and the tasks they enable in Partner Center, see [Assign roles & permissions to users](permissions-overview.md).</span></span>
- <span data-ttu-id="c399a-119">Ticari Market ve Windows & Xbox, Office Mağazası, Microsoft Edge ve donanım geliştirici programlarının özelliklerine erişim için kuruluşunuzdaki sahip veya yönetici rolünde bulunan kişiyle iletişim kurun.</span><span class="sxs-lookup"><span data-stu-id="c399a-119">For access to the capabilities of the Commercial Marketplace and the Windows & Xbox, Office Store, Microsoft Edge, and Hardware developer programs, contact the person in the Owner or Manager role in your organization.</span></span> <span data-ttu-id="c399a-120">Roller ve izinler hakkında daha fazla bilgi edinmek için bkz. [Microsoft Iş Ortağı Merkezi 'nde ticari Market hesabını yönetme](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions).</span><span class="sxs-lookup"><span data-stu-id="c399a-120">To learn more about roles and permissions, see [How to manage a commercial marketplace account in Microsoft Partner Center](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions).</span></span>

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a><span data-ttu-id="c399a-121">Iş Ortağı Merkezi 'nde teklifinizi veya avantajlarınızı göremezsiniz</span><span class="sxs-lookup"><span data-stu-id="c399a-121">You can’t see your offer or benefits in Partner Center</span></span>

<span data-ttu-id="c399a-122">Oturum açmak için doğru kimlik bilgilerini kullandığınızı onaylayın.</span><span class="sxs-lookup"><span data-stu-id="c399a-122">Confirm that you are using the correct credentials to sign in.</span></span> <span data-ttu-id="c399a-123">Örneğin, çalışmanız ve kişisel hesaplarınız aynı görünebilir (gibi abc@contoso.com ), ancak birisi sizin oluşturduğunuz bir kişisel hesap olabilir ve sizin adınıza bir iş hesabı olabilir.</span><span class="sxs-lookup"><span data-stu-id="c399a-123">For example, your work and personal accounts may look the same (such as abc@contoso.com), but one may be a personal account that you created and another may be a business account set up on your behalf.</span></span> <span data-ttu-id="c399a-124">Bu durumda, oturum açtıysanız ancak MPN, CSP, ticari Market ile ilgili beklenen özellikleri görüntüleyemiyorsa, iş hesabınızı seçmeyi deneyin.</span><span class="sxs-lookup"><span data-stu-id="c399a-124">In this case, if you are signed in, but are unable to view expected capabilities related to MPN, CSP, Commercial Marketplace, try selecting your work account.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c399a-125">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="c399a-125">Next steps</span></span>

- [<span data-ttu-id="c399a-126">Hesap bilgilerinizi doğrulama</span><span class="sxs-lookup"><span data-stu-id="c399a-126">Verify your account information</span></span>](verification-responses.md)
- [<span data-ttu-id="c399a-127">Parolamı sıfırlama</span><span class="sxs-lookup"><span data-stu-id="c399a-127">Reset my password</span></span>](reset-my-pasword.md)
- [<span data-ttu-id="c399a-128">Kullanıcı parolasını sıfırlama</span><span class="sxs-lookup"><span data-stu-id="c399a-128">Reset a user password</span></span>](reset-a-user-password.md)