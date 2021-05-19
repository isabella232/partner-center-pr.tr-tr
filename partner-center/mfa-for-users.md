---
title: Kullanıcılarınız için çok faktörlü kimlik doğrulaması ayarlama
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: MFA ile çalışanlarınızın kurulumunu öğrenin
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 5173526d0f65623311d5cd3a1061e8b9e93e9bb9
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151636"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="ec51c-103">Kullanıcılarınız için çok faktörlü kimlik doğrulaması ayarlama</span><span class="sxs-lookup"><span data-stu-id="ec51c-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="ec51c-104">**Uygun roller**: genel yönetici</span><span class="sxs-lookup"><span data-stu-id="ec51c-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="ec51c-105">Büyük gizlilik korumaları ve güvenlik, en iyi önceliklerimiz arasındadır.</span><span class="sxs-lookup"><span data-stu-id="ec51c-105">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="ec51c-106">En iyi savunması önleme olduğunu ve yalnızca zayıf bağlantımız kadar güçlü olduğunu biliyoruz.</span><span class="sxs-lookup"><span data-stu-id="ec51c-106">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="ec51c-107">Bu nedenle, ekosistemimizde herkesin işlem yapması ve uygun güvenlik korumalarının yerinde olduğundan emin olunması gerekir.</span><span class="sxs-lookup"><span data-stu-id="ec51c-107">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="ec51c-108">Tüm ortakların kendi iş ortağı kiracılarında kullanıcıları için Multi-Factor Authentication 'ı (MFA) etkinleştirmesine kesinlikle önerilir.</span><span class="sxs-lookup"><span data-stu-id="ec51c-108">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="ec51c-109">Kullanıcılarınız için Multi-Factor Authentication ekleme</span><span class="sxs-lookup"><span data-stu-id="ec51c-109">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="ec51c-110">Bu görevi gerçekleştirmek için şirketiniz için genel yönetici olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="ec51c-110">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="ec51c-111">Azure AD kiracınıza eklerken kullanıcılarınız için MFA 'yı etkinleştirmek en kolay yoldur.</span><span class="sxs-lookup"><span data-stu-id="ec51c-111">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="ec51c-112">[Azure Portal](https://portal.azure.com) oturum açın ve ardından **Kullanıcı yönetimi**' ne gidin.</span><span class="sxs-lookup"><span data-stu-id="ec51c-112">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="ec51c-113">**Multi-Factor Authentication**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="ec51c-113">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="ec51c-114">Etkinleştirmek istediğiniz kullanıcıyı seçin ve ardından **Etkinleştir**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="ec51c-114">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="ec51c-115">Bu, bu kullanıcı için MFA 'yı etkinleştirir.</span><span class="sxs-lookup"><span data-stu-id="ec51c-115">This will enable MFA for this user.</span></span> <span data-ttu-id="ec51c-116">Etkin, kullanıcıdan ilk kez oturum açtıklarında MFA doğrulamasını ayarlaması istenecektir.</span><span class="sxs-lookup"><span data-stu-id="ec51c-116">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="ec51c-117">Bundan sonra oturum açma sırasında, bunlara e-posta veya kısa mesaj yoluyla (ayarlandıkları bağlı olarak) bir kod vermesi istenir.</span><span class="sxs-lookup"><span data-stu-id="ec51c-117">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Nasıl doğrulanalınacağını belirtin":::

>[!NOTE]
><span data-ttu-id="ec51c-119">Kullanıcılarınıza, yukarıdaki gibi aynı adımları kullanarak ve **Uygula**' yı seçerek MFA 'Yı kullanmaya **zorlayabilirsiniz** .</span><span class="sxs-lookup"><span data-stu-id="ec51c-119">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="ec51c-120">Daha fazla bilgi edinmek için, [oturum açma olaylarını güvenli hale getirmek üzere Kullanıcı başına Azure Multi-Factor Authentication etkinleştirme](/azure/active-directory/authentication/howto-mfa-userstates)makalesini okuyun.</span><span class="sxs-lookup"><span data-stu-id="ec51c-120">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="ec51c-121">Tüm kullanıcılar **devre dışı bırakıldı**.</span><span class="sxs-lookup"><span data-stu-id="ec51c-121">All users start out **Disabled**.</span></span> <span data-ttu-id="ec51c-122">Kullanıcıları Kullanıcı başına Azure Active Directory Multi-Factor Authentication kaydettiğinizde, durumları **etkin** olarak değişir.</span><span class="sxs-lookup"><span data-stu-id="ec51c-122">When you enroll users in per-user Azure Active Directory Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="ec51c-123">Etkinleştirildiğinde kullanıcılar oturum atayarak kayıt işlemini tamamlar ve durumları Zorlanan **olarak değişir.**</span><span class="sxs-lookup"><span data-stu-id="ec51c-123">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="ec51c-124">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="ec51c-124">Next steps</span></span>

- [<span data-ttu-id="ec51c-125">Kullanıcılara rol ve izin atama</span><span class="sxs-lookup"><span data-stu-id="ec51c-125">Assign roles and permissions to users</span></span>](permissions-overview.md)