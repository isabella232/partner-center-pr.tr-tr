---
title: Satıcı ilişkisini bir müşteriyle kaldır
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft doğrudan iş ortaklarının müşterileri kendi listesinden nasıl kaldırabileceğini, yönetici ayrıcalıkları temsilcilerin nasıl kaldırılacağını ve bir müşterinin desteğini veya satın almayı durdurmasını öğrenin.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 83259f2f895be9ef34c55db5613ccfe6891a4424
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551478"
---
# <a name="how-to-remove-a-reseller-relationship-with-a-customer-in-partner-center"></a><span data-ttu-id="e562b-103">İş Ortağı Merkezi'nde müşteriyle kurumsal bayi ilişkisini kaldırma</span><span class="sxs-lookup"><span data-stu-id="e562b-103">How to remove a reseller relationship with a customer in Partner Center</span></span>

<span data-ttu-id="e562b-104">**Uygun roller**: genel yönetici</span><span class="sxs-lookup"><span data-stu-id="e562b-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="e562b-105">Bu makalede, Iş Ortağı Merkezi 'nde müşteri ile satıcı ilişkisinin nasıl kaldırılacağı açıklanır.</span><span class="sxs-lookup"><span data-stu-id="e562b-105">This article describes how to remove a reseller relationship with a customer in Partner Center.</span></span>

<span data-ttu-id="e562b-106">Doğrudan iş ortakları veya dolaylı sağlayıcılar: bir müşteriyle artık deneyimidir, Iş Ortağı Merkezi ' nde ilişkiyi kaldırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="e562b-106">Direct partners or Indirect providers: if you're no longer transacting with a customer, you can remove the relationship in Partner Center.</span></span>

<span data-ttu-id="e562b-107">İlişkinin kaldırılması şu sonuçları doğurur:</span><span class="sxs-lookup"><span data-stu-id="e562b-107">Removing a relationship has the following consequences:</span></span>

- <span data-ttu-id="e562b-108">Müşteriyi, İş Ortağı Merkezi'ndeki müşteri listenizden kaldırır</span><span class="sxs-lookup"><span data-stu-id="e562b-108">Removes the customer from your list of customers in Partner Center</span></span>
- <span data-ttu-id="e562b-109">Müşteriniz için [kullanılabilir destek kişileri listesinden](assign-support-contacts.md) sizi kaldırır</span><span class="sxs-lookup"><span data-stu-id="e562b-109">Removes you from the [list of available support contacts](assign-support-contacts.md) for your customer</span></span>
- <span data-ttu-id="e562b-110">Müşteri için temsilci yönetici ayrıcalıklarınızı kaldırır</span><span class="sxs-lookup"><span data-stu-id="e562b-110">Removes your delegation admin privileges for the customer</span></span>
- <span data-ttu-id="e562b-111">Müşteri için ileride satın alma işlemleri yapmanızı engeller</span><span class="sxs-lookup"><span data-stu-id="e562b-111">Prevents you from making future purchases for the customer</span></span>

## <a name="how-to-remove-a-relationship"></a><span data-ttu-id="e562b-112">İlişkiyi kaldırma</span><span class="sxs-lookup"><span data-stu-id="e562b-112">How to remove a relationship</span></span>

<span data-ttu-id="e562b-113">İlişkiyi kaldırmak için, Azure ayrılmış örnek (RI) ayırmalarını iptal etmeniz, yazılım satın alımlarını iptal etmeniz ve kalan tüm etkin abonelikleri askıya almanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="e562b-113">To remove the relationship, you'll need to cancel Azure reserved instance (RI) reservations, cancel software purchases, and suspend any remaining active subscriptions first.</span></span>

1. <span data-ttu-id="e562b-114">**Etkin abonelikleri askıya alın.**</span><span class="sxs-lookup"><span data-stu-id="e562b-114">**Suspend any active subscriptions.**</span></span>

   1. <span data-ttu-id="e562b-115">Iş ortağı merkezinden **müşteriler** ' e gidin ve müşteri seçin</span><span class="sxs-lookup"><span data-stu-id="e562b-115">From the Partner Center, go to **Customers** and select a customer</span></span>

   2. <span data-ttu-id="e562b-116">**Abonelikler**' in altında bir abonelik seçin.</span><span class="sxs-lookup"><span data-stu-id="e562b-116">Under **Subscriptions**, select a subscription.</span></span>

   3. <span data-ttu-id="e562b-117">**Askıya alındı** seçin</span><span class="sxs-lookup"><span data-stu-id="e562b-117">Select **Suspended**</span></span>

   4. <span data-ttu-id="e562b-118">Her etkin abonelik için bu adımları tekrarlayın.</span><span class="sxs-lookup"><span data-stu-id="e562b-118">Repeat these steps for each active subscription.</span></span>

2. <span data-ttu-id="e562b-119">**Iş Ortağı Merkezi 'nde ilişkiyi kaldırın:**</span><span class="sxs-lookup"><span data-stu-id="e562b-119">**Remove the relationship in Partner Center:**</span></span>

   <span data-ttu-id="e562b-120">a.</span><span class="sxs-lookup"><span data-stu-id="e562b-120">a.</span></span> <span data-ttu-id="e562b-121">Iş Ortağı Merkezi ' nden **müşteriler** ' e gidin ve bir müşteri seçin.</span><span class="sxs-lookup"><span data-stu-id="e562b-121">From the Partner Center, go to **Customers** and select a customer.</span></span>

   <span data-ttu-id="e562b-122">b.</span><span class="sxs-lookup"><span data-stu-id="e562b-122">b.</span></span> <span data-ttu-id="e562b-123">**Hesabı** seçin.</span><span class="sxs-lookup"><span data-stu-id="e562b-123">Select the **Account**.</span></span>

   <span data-ttu-id="e562b-124">c.</span><span class="sxs-lookup"><span data-stu-id="e562b-124">c.</span></span> <span data-ttu-id="e562b-125">**Satıcı Ilişkisini kaldır**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="e562b-125">Select **Remove reseller relationship**.</span></span>

   > [!NOTE]
   > <span data-ttu-id="e562b-126">Herhangi bir abonelik hala etkinse, **satıcı Ilişkisini kaldır** bağlantısı devre dışı bırakılır.</span><span class="sxs-lookup"><span data-stu-id="e562b-126">If any subscriptions are still active, the **Remove reseller relationship** link will be inactive.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e562b-127">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="e562b-127">Next steps</span></span>

- [<span data-ttu-id="e562b-128">Müşteriyle ilişki isteme veya yeniden oluşturma</span><span class="sxs-lookup"><span data-stu-id="e562b-128">Request or re-establish a relationship with a customer</span></span>](request-a-relationship-with-a-customer.md)
