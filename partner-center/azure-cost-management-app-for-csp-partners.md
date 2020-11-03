---
title: CSP 'Ler için Cloudyn ile Azure maliyet yönetimi
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure kullanımı ve maliyetlerini izlemek üzere uygulamayı kullanabilmeniz için Cloudyn Web uygulamasını nasıl kaydedeceğinizi ve Iş Ortağı Merkezi 'nde BT için gizli anahtar nasıl kullanacağınızı öğrenin.
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4ea156ef0932fe1af20f3e3c4b9be1a5f931cdde
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/17/2020
ms.locfileid: "92530995"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a><span data-ttu-id="1ece9-103">CSP iş ortakları için Azure maliyet yönetimi uygulaması ile müşteri Azure kullanımını ve maliyetlerini izleyin</span><span class="sxs-lookup"><span data-stu-id="1ece9-103">Track customer Azure usage and costs with the Azure cost management app for CSP partners</span></span>  

<span data-ttu-id="1ece9-104">**Uygulama hedefi**</span><span class="sxs-lookup"><span data-stu-id="1ece9-104">**Applies to**</span></span>

- <span data-ttu-id="1ece9-105">İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="1ece9-105">Partner Center</span></span>
- <span data-ttu-id="1ece9-106">Bulut çözümü sağlayıcısı program iş ortakları</span><span class="sxs-lookup"><span data-stu-id="1ece9-106">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="1ece9-107">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="1ece9-107">**Appropriate roles**</span></span>

- <span data-ttu-id="1ece9-108">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="1ece9-108">Global admin</span></span>
- <span data-ttu-id="1ece9-109">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="1ece9-109">Admin agent</span></span>

[<span data-ttu-id="1ece9-110">Azure maliyet yönetimi hakkında daha fazla bilgi alın</span><span class="sxs-lookup"><span data-stu-id="1ece9-110">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="1ece9-111">Başlamadan önce</span><span class="sxs-lookup"><span data-stu-id="1ece9-111">Before you begin</span></span>
<span data-ttu-id="1ece9-112">Azure maliyet yönetimi 'ni kullanabilmek için aşağıdaki gereksinimleri karşıladığınızdan emin olun:</span><span class="sxs-lookup"><span data-stu-id="1ece9-112">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="1ece9-113">Bulut çözümü sağlayıcısı programındaki bir iş ortağıyım.</span><span class="sxs-lookup"><span data-stu-id="1ece9-113">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="1ece9-114">Bir Iş Ortağı Merkezi API web uygulaması oluşturma olanağınız vardır.</span><span class="sxs-lookup"><span data-stu-id="1ece9-114">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="1ece9-115">Genel Bakış</span><span class="sxs-lookup"><span data-stu-id="1ece9-115">Overview</span></span>

<span data-ttu-id="1ece9-116">Cloudyn, müşterilerinizin Azure 'un ne kadarını kullandığını ve bu kullanımın maliyetlerini izlemenize ve yönetmenize olanak tanıyan bir Web uygulamasıdır.</span><span class="sxs-lookup"><span data-stu-id="1ece9-116">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="1ece9-117">Bunu Iş Ortağı Merkezi API 'SI aracılığıyla kullanırsınız.</span><span class="sxs-lookup"><span data-stu-id="1ece9-117">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="1ece9-118">Web uygulamanızı Iş Ortağı Merkezi 'ne kaydetme</span><span class="sxs-lookup"><span data-stu-id="1ece9-118">Register your web app in the Partner Center</span></span>
<span data-ttu-id="1ece9-119">Iş Ortağı Merkezi 'ne bir Azure Active Directory Web uygulaması kaydettiğinizde, Iş Ortağı Merkezi API 'sine erişim sağlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1ece9-119">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="1ece9-120">[Genel yönetici veya yönetici aracı hesabı](create-user-accounts-and-set-permissions.md)kullanarak [iş ortağı merkezinde](https://partnercenter.microsoft.com/pcv/dashboard/overview) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="1ece9-120">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="1ece9-121">**İş ortağı merkezi** ' nden **Hesap ayarları** &gt; **[uygulama yönetimi](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** ' ni seçin.</span><span class="sxs-lookup"><span data-stu-id="1ece9-121">From the **Partner Center** , select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** .</span></span>
3.  <span data-ttu-id="1ece9-122">**Web uygulaması** bölümünde **Yeni Web uygulaması Ekle** ' ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="1ece9-122">In the **Web App** section, click **Add new web app** .</span></span>
<br> <span data-ttu-id="1ece9-123">**Note** : daha önce bir Web uygulaması oluşturduysanız adım 3 ' ü atlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1ece9-123">**Note** : If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="1ece9-124">Web uygulamanız için **TICARET kimliği** GUID 'Ini ve **uygulama kimliği** GUID 'ini kopyalayın ve kaydedin.</span><span class="sxs-lookup"><span data-stu-id="1ece9-124">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="1ece9-125">Azure maliyet yönetimi uygulamasının 30 günlük ücretsiz deneme sürümünü kullanabilmeniz için her iki kimlik de gereklidir.</span><span class="sxs-lookup"><span data-stu-id="1ece9-125">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="1ece9-126">Uygulamanıza gizli anahtar ekleme</span><span class="sxs-lookup"><span data-stu-id="1ece9-126">Add a secret key to your app</span></span>
1. <span data-ttu-id="1ece9-127">**Anahtar Ekle** düğmesinin yanındaki açılan kutuda 1 veya 2 yıl bir süre seçin.</span><span class="sxs-lookup"><span data-stu-id="1ece9-127">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="1ece9-128">**Anahtar Ekle** ' ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="1ece9-128">Click **Add key** .</span></span> 
3. <span data-ttu-id="1ece9-129">Gizli anahtar değerini kopyalayın ve kaydedin.</span><span class="sxs-lookup"><span data-stu-id="1ece9-129">Copy and save the secret key value.</span></span> <span data-ttu-id="1ece9-130">30 günlük ücretsiz deneme için buna ihtiyacınız olacaktır.</span><span class="sxs-lookup"><span data-stu-id="1ece9-130">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="1ece9-131">Uygulama gizli anahtarı, daha uzun süre sonu tarihleri olan parolalar gibidir.</span><span class="sxs-lookup"><span data-stu-id="1ece9-131">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="1ece9-132">Lütfen daha sonra kullanmak için anahtar değerini güvenli bir konuma kaydedin.</span><span class="sxs-lookup"><span data-stu-id="1ece9-132">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1ece9-133">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="1ece9-133">Next steps</span></span>
<span data-ttu-id="1ece9-134">[30 günlük ücretsiz deneme sürümü](https://go.microsoft.com/fwlink/?linkid=857895)başlatın.</span><span class="sxs-lookup"><span data-stu-id="1ece9-134">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="1ece9-135">Denemeyi başlatmak için aşağıdaki ayrıntılara ihtiyacınız vardır:</span><span class="sxs-lookup"><span data-stu-id="1ece9-135">You need the following details to start the trial:</span></span>
- <span data-ttu-id="1ece9-136">İş Ortağı Merkezi oturum açma kimlik bilgileri</span><span class="sxs-lookup"><span data-stu-id="1ece9-136">Partner Center sign in credentials</span></span>
- <span data-ttu-id="1ece9-137">Ticaret KIMLIĞI GUID 'SI</span><span class="sxs-lookup"><span data-stu-id="1ece9-137">Commerce ID GUID</span></span>
- <span data-ttu-id="1ece9-138">Uygulama KIMLIĞI GUID 'SI</span><span class="sxs-lookup"><span data-stu-id="1ece9-138">App ID GUID</span></span>
- <span data-ttu-id="1ece9-139">Uygulama gizli anahtarı değeri</span><span class="sxs-lookup"><span data-stu-id="1ece9-139">Application secret key value</span></span>
