---
title: Kullanıcılarınız için çok faktörlü kimlik doğrulaması ayarlama
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: MFA ile çalışanlarınızı ayarlamayı öğrenin
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 37373c032dc34315c0e3274987805d7518d0b595
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276612"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="94cd6-103">Kullanıcılarınız için çok faktörlü kimlik doğrulaması ayarlama</span><span class="sxs-lookup"><span data-stu-id="94cd6-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="94cd6-104">**Uygun roller:** Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="94cd6-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="94cd6-105">Daha fazla gizlilik koruması ve güvenlik, en önemli önceliklerimiz arasında yer almaktadır.</span><span class="sxs-lookup"><span data-stu-id="94cd6-105">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="94cd6-106">En iyi savunmanın önleme olduğunu ve en zayıf bağlantımız kadar güçlü olduğunu biliyoruz.</span><span class="sxs-lookup"><span data-stu-id="94cd6-106">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="94cd6-107">İşte bu nedenle ekosistemimiz içinde herkesin harekete geçsin ve uygun güvenlik korumalarının hazır olduğundan emin olasın.</span><span class="sxs-lookup"><span data-stu-id="94cd6-107">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="94cd6-108">Tüm iş ortaklarının, iş ortağı kiracılarında kullanıcıları için çok faktörlü kimlik doğrulamasını (MFA) etkinleştirmesini kesinlikle öneririz.</span><span class="sxs-lookup"><span data-stu-id="94cd6-108">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="94cd6-109">Kullanıcılarınız için çok faktörlü kimlik doğrulaması ekleme</span><span class="sxs-lookup"><span data-stu-id="94cd6-109">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="94cd6-110">Bu görevi tamamlamak için şirketinizin genel yöneticisi olmak gerekir.</span><span class="sxs-lookup"><span data-stu-id="94cd6-110">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="94cd6-111">Kullanıcılarınız için MFA'yi Azure AD kiracınıza eklerken etkinleştirmek en kolay yöntemdir.</span><span class="sxs-lookup"><span data-stu-id="94cd6-111">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="94cd6-112">Oturum Azure portal [ve](https://portal.azure.com) ardından Kullanıcı **yönetimi'ne gidin.**</span><span class="sxs-lookup"><span data-stu-id="94cd6-112">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="94cd6-113">Çok **faktörlü kimlik doğrulaması'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="94cd6-113">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="94cd6-114">Etkinleştirmek istediğiniz kullanıcıyı seçin ve ardından **Etkinleştir'i seçin.**</span><span class="sxs-lookup"><span data-stu-id="94cd6-114">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="94cd6-115">Bu, bu kullanıcı için MFA'ya olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="94cd6-115">This will enable MFA for this user.</span></span> <span data-ttu-id="94cd6-116">Etkin, kullanıcının ilk kez oturum a açması için MFA doğrulamasını ayarlaması istenecek anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="94cd6-116">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="94cd6-117">Bundan sonra, oturum açmalarında, e-posta veya kısa mesaj aracılığıyla (ayarlanacaklarına bağlı olarak) onlara gönderilen bir kod sağlamaları istenecek.</span><span class="sxs-lookup"><span data-stu-id="94cd6-117">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Doğrulamayı belirtin.":::

>[!NOTE]
><span data-ttu-id="94cd6-119">Yukarıdaki **adımların** aynısını kullanarak ve Zorla'ya seçerek kullanıcılarınızı MFA kullanmaya **zorabilirsiniz.**</span><span class="sxs-lookup"><span data-stu-id="94cd6-119">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="94cd6-120">Daha fazla bilgi edinmek için oturum [açma olaylarının güvenliğini sağlamak için kullanıcı başına Azure Multi-Factor Authentication'a etkinleştirme makalelerini okuyun.](/azure/active-directory/authentication/howto-mfa-userstates)</span><span class="sxs-lookup"><span data-stu-id="94cd6-120">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="94cd6-121">Tüm kullanıcılar Devre Dışı olarak **başlar.**</span><span class="sxs-lookup"><span data-stu-id="94cd6-121">All users start out **Disabled**.</span></span> <span data-ttu-id="94cd6-122">Multi-Factor Authentication'da kullanıcıları kullanıcı Azure Active Directory kaydedip durumu Etkin olarak **değişir.**</span><span class="sxs-lookup"><span data-stu-id="94cd6-122">When you enroll users in per-user Azure Active Directory Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="94cd6-123">Etkinleştirildiğinde kullanıcılar oturum atayarak kayıt işlemini tamamlar ve durumları Zorlanan **olarak değişir.**</span><span class="sxs-lookup"><span data-stu-id="94cd6-123">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="94cd6-124">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="94cd6-124">Next steps</span></span>

- [<span data-ttu-id="94cd6-125">Kullanıcılara rol ve izin atama</span><span class="sxs-lookup"><span data-stu-id="94cd6-125">Assign roles and permissions to users</span></span>](permissions-overview.md)