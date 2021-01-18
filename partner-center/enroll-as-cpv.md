---
title: Denetim Masası satıcısı olarak kaydetme
description: CSP iş ortağı sistemlerini Iş Ortağı Merkezi API 'Leriyle daha iyi tümleştirebilmeniz için Iş Ortağı Merkezi 'nde bir denetim masası satıcısı (CPV) olarak nasıl kaydolacağınızı öğrenin.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 01/15/2021
ms.openlocfilehash: 5fd2267d53641fe4a0b6181217a35f0470e5bbe5
ms.sourcegitcommit: 7681c6fc51e78cba106c46a52f6bb27e1a5c1c6b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/18/2021
ms.locfileid: "98560519"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="73a59-103">CSP iş ortağı sistemlerini Iş Ortağı Merkezi API 'Leriyle tümleştirmenize yardımcı olmak için Denetim Masası satıcısı olarak kaydetme</span><span class="sxs-lookup"><span data-stu-id="73a59-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>


<span data-ttu-id="73a59-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="73a59-104">**Appropriate roles**</span></span>

- <span data-ttu-id="73a59-105">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="73a59-105">Global admin</span></span>

<span data-ttu-id="73a59-106">Bir denetim masası satıcısı (CPV), bulut çözümü sağlayıcısı (CSP) iş ortakları tarafından sistemlerini Iş Ortağı Merkezi API 'Leri ile tümleştirmelerini sağlamak üzere uygulamalar geliştiren bağımsız bir yazılım satıcıdır.</span><span class="sxs-lookup"><span data-stu-id="73a59-106">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="73a59-107">Bir denetim masası satıcısı, Iş Ortağı Merkezi panosuna veya Iş Ortağı Merkezi API 'Lerine doğrudan erişimli bir CSP Iş ortağı değildir.</span><span class="sxs-lookup"><span data-stu-id="73a59-107">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="73a59-108">Microsoft iş ortaklarıyla çalışmak isteyen geçerli bir denetim masası satıcısı (CPV) veya yeni bir CPV olun, Microsoft artık uygulamalarınızı kaydetmek ve bulut çözümü sağlayıcısı iş ortaklarını desteklemek için Iş Ortağı Merkezi 'ne kaydolmanızı gerektirir.</span><span class="sxs-lookup"><span data-stu-id="73a59-108">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="73a59-109">Bir hesap oluşturmak için, bir CPV iş ortağı mevcut bir CSP iş ortağı kiracısı veya mevcut bir CPV kiracısı kullanabilir ya da ekleme sürecinin bir parçası olarak yeni bir kiracı oluşturabilir.</span><span class="sxs-lookup"><span data-stu-id="73a59-109">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="73a59-110">CPV iş ortağı mevcut CSP kiracısını kullanmayı seçerse, ayrı bir çok kiracılı uygulamalar oluşturmalı ve bunları CPV etkinlikleri için Iş Ortağı Merkezi 'ne kaydetmeleri gerekir.</span><span class="sxs-lookup"><span data-stu-id="73a59-110">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="73a59-111">Bir uygulama hem CSP hem de CPV uygulaması olarak kaydedilemez.</span><span class="sxs-lookup"><span data-stu-id="73a59-111">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="73a59-112">Iş Ortağı Merkezi 'ne kaydolduktan ve uygulamalarınızı kaydettirdikten sonra, Iş Ortağı Merkezi API 'Lerine erişebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="73a59-112">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="73a59-113">Bir sandbox hesabına ihtiyacınız varsa Microsoft Desteği isteğiyle Microsoft ile iletişim kurun.</span><span class="sxs-lookup"><span data-stu-id="73a59-113">Contact Microsoft through a Microsoft Support request if you need a sandbox account.</span></span> <span data-ttu-id="73a59-114">Zaten bir korumalı alan hesabınız varsa, bu hesabı kullanmaya devam edin.</span><span class="sxs-lookup"><span data-stu-id="73a59-114">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="73a59-115">Yeni bir korumalı alan gerekmez</span><span class="sxs-lookup"><span data-stu-id="73a59-115">You won't need a new sandbox</span></span>

<span data-ttu-id="73a59-116">[Microsoft Denetim Masası satıcı sözleşmesini](https://go.microsoft.com/fwlink/?linkid=2055198) gözden geçirin</span><span class="sxs-lookup"><span data-stu-id="73a59-116">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="73a59-117">Iş Ortağı Merkezi 'nde çalışma</span><span class="sxs-lookup"><span data-stu-id="73a59-117">Working in Partner Center</span></span>

<span data-ttu-id="73a59-118">Iş Ortağı Merkezi CPV deneyimine kaydolduktan ve CPV sözleşmesini kabul etmeniz durumunda şunları yapabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="73a59-118">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="73a59-119">Çok kiracılı uygulamaları yönetme (Iş Ortağı Merkezi 'nde uygulamaları Azure portal, kaydetmek ve kayıt silmek için uygulama ekleme).</span><span class="sxs-lookup"><span data-stu-id="73a59-119">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="73a59-120">Iş Ortağı Merkezi API 'Lerine yetki almak için, CPVs 'in uygulamalarını Iş Ortağı Merkezi 'ne kaydetmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="73a59-120">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="73a59-121">Uygulamaları tek başına Azure portal eklemek, Iş Ortağı Merkezi API 'Leri için CPV uygulamalarına yetki vermez.</span><span class="sxs-lookup"><span data-stu-id="73a59-121">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="73a59-122">CPV profilinizi görüntüleyin ve yönetin</span><span class="sxs-lookup"><span data-stu-id="73a59-122">View and manage your CPV profile</span></span> 

- <span data-ttu-id="73a59-123">CPV özelliklerine erişmesi gereken kullanıcılarınızı görüntüleyin ve yönetin.</span><span class="sxs-lookup"><span data-stu-id="73a59-123">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="73a59-124">Genel yönetici, bir CPV 'nin sahip olduğu tek roldür.</span><span class="sxs-lookup"><span data-stu-id="73a59-124">Global admin is the only role a CPV can have.</span></span>

## <a name="next-steps"></a><span data-ttu-id="73a59-125">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="73a59-125">Next steps</span></span>

<span data-ttu-id="73a59-126">-[Iş Ortağı Merkezi hesabınıza ek kiracılar ekleyin](multi-tenant-account.md)</span><span class="sxs-lookup"><span data-stu-id="73a59-126">-[Add additional tenants to your Partner Center account](multi-tenant-account.md)</span></span>