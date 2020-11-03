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
ms.date: 05/20/2020
ms.openlocfilehash: 1bfcb4de27233283b6188903b3e1f6bbdf67698c
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/14/2020
ms.locfileid: "92531943"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="67f23-103">CSP iş ortağı sistemlerini Iş Ortağı Merkezi API 'Leriyle tümleştirmenize yardımcı olmak için Denetim Masası satıcısı olarak kaydetme</span><span class="sxs-lookup"><span data-stu-id="67f23-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>

<span data-ttu-id="67f23-104">**Uygulama hedefi**</span><span class="sxs-lookup"><span data-stu-id="67f23-104">**Applies to**</span></span>

- <span data-ttu-id="67f23-105">İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="67f23-105">Partner Center</span></span>

<span data-ttu-id="67f23-106">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="67f23-106">**Appropriate roles**</span></span>

- <span data-ttu-id="67f23-107">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="67f23-107">Global admin</span></span>

<span data-ttu-id="67f23-108">Bir denetim masası satıcısı (CPV), bulut çözümü sağlayıcısı (CSP) iş ortakları tarafından sistemlerini Iş Ortağı Merkezi API 'Leri ile tümleştirmelerini sağlamak üzere uygulamalar geliştiren bağımsız bir yazılım satıcıdır.</span><span class="sxs-lookup"><span data-stu-id="67f23-108">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="67f23-109">Bir denetim masası satıcısı, Iş Ortağı Merkezi panosuna veya Iş Ortağı Merkezi API 'Lerine doğrudan erişimli bir CSP Iş ortağı değildir.</span><span class="sxs-lookup"><span data-stu-id="67f23-109">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="67f23-110">Microsoft iş ortaklarıyla çalışmak isteyen geçerli bir denetim masası satıcısı (CPV) veya yeni bir CPV olun, Microsoft artık uygulamalarınızı kaydetmek ve bulut çözümü sağlayıcısı iş ortaklarını desteklemek için Iş Ortağı Merkezi 'ne kaydolmanızı gerektirir.</span><span class="sxs-lookup"><span data-stu-id="67f23-110">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="67f23-111">Bir hesap oluşturmak için, bir CPV iş ortağı mevcut bir CSP iş ortağı kiracısı veya mevcut bir CPV kiracısı kullanabilir ya da ekleme sürecinin bir parçası olarak yeni bir kiracı oluşturabilir.</span><span class="sxs-lookup"><span data-stu-id="67f23-111">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="67f23-112">CPV iş ortağı mevcut CSP kiracısını kullanmayı seçerse, ayrı bir çok kiracılı uygulamalar oluşturmalı ve bunları CPV etkinlikleri için Iş Ortağı Merkezi 'ne kaydetmeleri gerekir.</span><span class="sxs-lookup"><span data-stu-id="67f23-112">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="67f23-113">Bir uygulama hem CSP hem de CPV uygulaması olarak kaydedilemez.</span><span class="sxs-lookup"><span data-stu-id="67f23-113">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="67f23-114">Iş Ortağı Merkezi 'ne kaydolduktan ve uygulamalarınızı kaydettirdikten sonra, Iş Ortağı Merkezi API 'Lerine erişebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="67f23-114">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="67f23-115">Microsoft, korumalı alan bilgileriniz ile bir Iş Ortağı Merkezi bildirimi aracılığıyla sizinle iletişim kuracaktır.</span><span class="sxs-lookup"><span data-stu-id="67f23-115">Microsoft will contact you via a Partner Center notification with your sandbox information.</span></span> <span data-ttu-id="67f23-116">Zaten bir korumalı alan hesabınız varsa, bu hesabı kullanmaya devam edin.</span><span class="sxs-lookup"><span data-stu-id="67f23-116">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="67f23-117">Yeni bir korumalı alana ihtiyacınız olmayacaktır.</span><span class="sxs-lookup"><span data-stu-id="67f23-117">You won't need a new sandbox.</span></span>

<span data-ttu-id="67f23-118">[Microsoft Denetim Masası satıcı sözleşmesini](https://go.microsoft.com/fwlink/?linkid=2055198) gözden geçirin</span><span class="sxs-lookup"><span data-stu-id="67f23-118">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="67f23-119">Iş Ortağı Merkezi 'nde çalışma</span><span class="sxs-lookup"><span data-stu-id="67f23-119">Working in Partner Center</span></span>
<span data-ttu-id="67f23-120">Iş Ortağı Merkezi CPV deneyimine kaydolduktan ve CPV sözleşmesini kabul etmeniz durumunda şunları yapabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="67f23-120">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="67f23-121">Çok kiracılı uygulamaları yönetme (Iş Ortağı Merkezi 'nde uygulamaları Azure portal, kaydetmek ve kayıt silmek için uygulama ekleme).</span><span class="sxs-lookup"><span data-stu-id="67f23-121">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="67f23-122">Iş Ortağı Merkezi API 'Lerine yetki almak için, CPVs 'in uygulamalarını Iş Ortağı Merkezi 'ne kaydetmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="67f23-122">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="67f23-123">Uygulamaları tek başına Azure portal eklemek, Iş Ortağı Merkezi API 'Leri için CPV uygulamalarına yetki vermez.</span><span class="sxs-lookup"><span data-stu-id="67f23-123">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="67f23-124">CPV profilinizi görüntüleyin ve yönetin</span><span class="sxs-lookup"><span data-stu-id="67f23-124">View and manage your CPV profile</span></span> 

- <span data-ttu-id="67f23-125">CPV özelliklerine erişmesi gereken kullanıcılarınızı görüntüleyin ve yönetin.</span><span class="sxs-lookup"><span data-stu-id="67f23-125">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="67f23-126">Genel yönetici, bir CPV 'nin sahip olduğu tek roldür.</span><span class="sxs-lookup"><span data-stu-id="67f23-126">Global admin is the only role a CPV can have.</span></span>


