---
title: Satıcı olarak Denetim Masası kaydetme
description: CSP iş ortağı sistemlerini Denetim Masası API'lerle daha iyi tümleştire İş Ortağı Merkezi bir Satıcı (CPV) İş Ortağı Merkezi öğrenin.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 01/15/2021
ms.openlocfilehash: edc0ea8f0fda58f23cbce82bc7023a3277517cc3
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147148"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="8158f-103">CSP iş ortağı sistemlerini Denetim Masası API'lerle tümleştirin ve satıcı olarak İş Ortağı Merkezi olun</span><span class="sxs-lookup"><span data-stu-id="8158f-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>


<span data-ttu-id="8158f-104">**Uygun roller:** Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="8158f-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="8158f-105">Bir Denetim Masası Satıcısı (CPV), Bulut Çözümü Sağlayıcısı (CSP) iş ortakları tarafından sistemlerini İş Ortağı Merkezi API'lerle tümleştirerek kullanmaları için uygulamalar geliştiren bağımsız bir yazılım satıcısıdır.</span><span class="sxs-lookup"><span data-stu-id="8158f-105">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="8158f-106">Bir Denetim Masası satıcı, İş Ortağı Merkezi panosuna veya İş Ortağı Merkezi ERIŞIMI olan bir CSP İş Ortağı Merkezi değildir.</span><span class="sxs-lookup"><span data-stu-id="8158f-106">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="8158f-107">İster mevcut bir Denetim Masası Satıcısı (CPV) ister Microsoft iş ortaklarıyla çalışmak isteyen yeni bir CPV olun, Microsoft artık uygulamalarınızı kaydetmek ve iş ortaklarını desteklemek için İş Ortağı Merkezi'a kaydolmanızı Bulut Çözümü Sağlayıcısı gerektirir.</span><span class="sxs-lookup"><span data-stu-id="8158f-107">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="8158f-108">Bir hesap oluşturmak için, CPV iş ortağı var olan bir CSP iş ortağı kiracısını veya mevcut CPV kiracısını kullanabilir ya da ekleme işleminin bir parçası olarak yeni bir kiracı oluşturabilir.</span><span class="sxs-lookup"><span data-stu-id="8158f-108">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="8158f-109">CPV iş ortağı mevcut CSP kiracıyı kullanmayı seçerse, ayrı çok kiracılı uygulamalar oluşturmaları ve bunları CPV etkinlikleri için İş Ortağı Merkezi kaydetmeleri gerekir.</span><span class="sxs-lookup"><span data-stu-id="8158f-109">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="8158f-110">Bir uygulama hem CSP hem de CPV uygulaması olarak kaydedilene.</span><span class="sxs-lookup"><span data-stu-id="8158f-110">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="8158f-111">Uygulamanıza kaydolarak İş Ortağı Merkezi uygulamalarınızı kaydettikten sonra, uygulama API'lerine İş Ortağı Merkezi olur.</span><span class="sxs-lookup"><span data-stu-id="8158f-111">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="8158f-112">Korumalı alan hesabına ihtiyacınız varsa Microsoft Desteği isteğiyle Microsoft'a ulaşın.</span><span class="sxs-lookup"><span data-stu-id="8158f-112">Contact Microsoft through a Microsoft Support request if you need a sandbox account.</span></span> <span data-ttu-id="8158f-113">Zaten bir korumalı alan hesabınız varsa, bunu kullanmaya devam edersiniz.</span><span class="sxs-lookup"><span data-stu-id="8158f-113">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="8158f-114">Yeni bir korumalı alana ihtiyacınız olmayacak</span><span class="sxs-lookup"><span data-stu-id="8158f-114">You won't need a new sandbox</span></span>

<span data-ttu-id="8158f-115">Microsoft [Denetim Masası Satıcı sözleşmesini gözden geçirme](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="8158f-115">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="8158f-116">İş Ortağı Merkezi'da çalışma</span><span class="sxs-lookup"><span data-stu-id="8158f-116">Working in Partner Center</span></span>

<span data-ttu-id="8158f-117">İş Ortağı Merkezi CPV deneyimine kaydolarak CPV anlaşmasını kabul edin:</span><span class="sxs-lookup"><span data-stu-id="8158f-117">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="8158f-118">Çok kiracılı uygulamaları yönetme (uygulamalarınızı Azure portal, kaydetme ve uygulama kaydını İş Ortağı Merkezi).</span><span class="sxs-lookup"><span data-stu-id="8158f-118">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="8158f-119">Iş Ortağı Merkezi API 'Lerine yetki almak için, CPVs 'in uygulamalarını Iş Ortağı Merkezi 'ne kaydetmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="8158f-119">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="8158f-120">Uygulamaları tek başına Azure portal eklemek, Iş Ortağı Merkezi API 'Leri için CPV uygulamalarına yetki vermez.</span><span class="sxs-lookup"><span data-stu-id="8158f-120">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="8158f-121">CPV profilinizi görüntüleyin ve yönetin</span><span class="sxs-lookup"><span data-stu-id="8158f-121">View and manage your CPV profile</span></span> 

- <span data-ttu-id="8158f-122">CPV özelliklerine erişmesi gereken kullanıcılarınızı görüntüleyin ve yönetin.</span><span class="sxs-lookup"><span data-stu-id="8158f-122">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="8158f-123">Genel yönetici, bir CPV 'nin sahip olduğu tek roldür.</span><span class="sxs-lookup"><span data-stu-id="8158f-123">Global admin is the only role a CPV can have.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8158f-124">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="8158f-124">Next steps</span></span>

<span data-ttu-id="8158f-125">-[Iş Ortağı Merkezi hesabınıza ek kiracılar ekleyin](multi-tenant-account.md)</span><span class="sxs-lookup"><span data-stu-id="8158f-125">-[Add additional tenants to your Partner Center account](multi-tenant-account.md)</span></span>