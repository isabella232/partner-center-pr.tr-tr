---
title: CSP'ler için Cloudyn'in sunduğu Azure Maliyet Yönetimi
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure kullanımı ve maliyetlerini izlemek üzere uygulamayı kullanabilmeniz için Cloudyn Web uygulamasını nasıl kaydedeceğinizi ve Iş Ortağı Merkezi 'nde BT için gizli anahtar nasıl kullanacağınızı öğrenin.
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: defa691a3bc70cbda45f01cb447d89364a49e3b8
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96535007"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a><span data-ttu-id="0afd8-103">CSP iş ortakları için Azure maliyet yönetimi uygulaması ile müşteri Azure kullanımını ve maliyetlerini izleyin</span><span class="sxs-lookup"><span data-stu-id="0afd8-103">Track customer Azure usage and costs with the Azure cost management app for CSP partners</span></span>  

<span data-ttu-id="0afd8-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="0afd8-104">**Appropriate roles**</span></span>

- <span data-ttu-id="0afd8-105">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="0afd8-105">Global admin</span></span>
- <span data-ttu-id="0afd8-106">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="0afd8-106">Admin agent</span></span>

[<span data-ttu-id="0afd8-107">Azure maliyet yönetimi hakkında daha fazla bilgi alın</span><span class="sxs-lookup"><span data-stu-id="0afd8-107">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="0afd8-108">Başlamadan önce</span><span class="sxs-lookup"><span data-stu-id="0afd8-108">Before you begin</span></span>
<span data-ttu-id="0afd8-109">Azure maliyet yönetimi 'ni kullanabilmek için aşağıdaki gereksinimleri karşıladığınızdan emin olun:</span><span class="sxs-lookup"><span data-stu-id="0afd8-109">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="0afd8-110">Bulut çözümü sağlayıcısı programındaki bir iş ortağıyım.</span><span class="sxs-lookup"><span data-stu-id="0afd8-110">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="0afd8-111">Bir Iş Ortağı Merkezi API web uygulaması oluşturma olanağınız vardır.</span><span class="sxs-lookup"><span data-stu-id="0afd8-111">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="0afd8-112">Genel bakış</span><span class="sxs-lookup"><span data-stu-id="0afd8-112">Overview</span></span>

<span data-ttu-id="0afd8-113">Cloudyn, müşterilerinizin Azure 'un ne kadarını kullandığını ve bu kullanımın maliyetlerini izlemenize ve yönetmenize olanak tanıyan bir Web uygulamasıdır.</span><span class="sxs-lookup"><span data-stu-id="0afd8-113">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="0afd8-114">Bunu Iş Ortağı Merkezi API 'SI aracılığıyla kullanırsınız.</span><span class="sxs-lookup"><span data-stu-id="0afd8-114">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="0afd8-115">Web uygulamanızı Iş Ortağı Merkezi 'ne kaydetme</span><span class="sxs-lookup"><span data-stu-id="0afd8-115">Register your web app in the Partner Center</span></span>
<span data-ttu-id="0afd8-116">Iş Ortağı Merkezi 'ne bir Azure Active Directory Web uygulaması kaydettiğinizde, Iş Ortağı Merkezi API 'sine erişim sağlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0afd8-116">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="0afd8-117">[Genel yönetici veya yönetici aracı hesabı](create-user-accounts-and-set-permissions.md)kullanarak [iş ortağı merkezi](https://partnercenter.microsoft.com/pcv/dashboard/overview) ' nde oturum açın.</span><span class="sxs-lookup"><span data-stu-id="0afd8-117">Sign into [Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="0afd8-118">**İş ortağı merkezi**' nden **Hesap ayarları** &gt; **[uygulama yönetimi](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**' ni seçin.</span><span class="sxs-lookup"><span data-stu-id="0afd8-118">From **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="0afd8-119">**Web uygulaması** bölümünde **Yeni Web uygulaması Ekle**' ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="0afd8-119">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="0afd8-120">**Note**: daha önce bir Web uygulaması oluşturduysanız adım 3 ' ü atlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0afd8-120">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="0afd8-121">Web uygulamanız için **TICARET kimliği** GUID 'Ini ve **uygulama kimliği** GUID 'ini kopyalayın ve kaydedin.</span><span class="sxs-lookup"><span data-stu-id="0afd8-121">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="0afd8-122">Azure maliyet yönetimi uygulamasının 30 günlük ücretsiz deneme sürümünü kullanabilmeniz için her iki kimlik de gereklidir.</span><span class="sxs-lookup"><span data-stu-id="0afd8-122">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="0afd8-123">Uygulamanıza gizli anahtar ekleme</span><span class="sxs-lookup"><span data-stu-id="0afd8-123">Add a secret key to your app</span></span>
1. <span data-ttu-id="0afd8-124">**Anahtar Ekle** düğmesinin yanındaki açılan kutuda 1 veya 2 yıl bir süre seçin.</span><span class="sxs-lookup"><span data-stu-id="0afd8-124">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="0afd8-125">**Anahtar Ekle**' ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="0afd8-125">Click **Add key**.</span></span> 
3. <span data-ttu-id="0afd8-126">Gizli anahtar değerini kopyalayın ve kaydedin.</span><span class="sxs-lookup"><span data-stu-id="0afd8-126">Copy and save the secret key value.</span></span> <span data-ttu-id="0afd8-127">30 günlük ücretsiz deneme için buna ihtiyacınız olacaktır.</span><span class="sxs-lookup"><span data-stu-id="0afd8-127">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="0afd8-128">Uygulama gizli anahtarı, daha uzun süre sonu tarihleri olan parolalar gibidir.</span><span class="sxs-lookup"><span data-stu-id="0afd8-128">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="0afd8-129">Lütfen daha sonra kullanmak için anahtar değerini güvenli bir konuma kaydedin.</span><span class="sxs-lookup"><span data-stu-id="0afd8-129">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="0afd8-130">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="0afd8-130">Next steps</span></span>
<span data-ttu-id="0afd8-131">[30 günlük ücretsiz deneme sürümü](https://go.microsoft.com/fwlink/?linkid=857895)başlatın.</span><span class="sxs-lookup"><span data-stu-id="0afd8-131">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="0afd8-132">Denemeyi başlatmak için aşağıdaki ayrıntılara ihtiyacınız vardır:</span><span class="sxs-lookup"><span data-stu-id="0afd8-132">You need the following details to start the trial:</span></span>
- <span data-ttu-id="0afd8-133">İş Ortağı Merkezi oturum açma kimlik bilgileri</span><span class="sxs-lookup"><span data-stu-id="0afd8-133">Partner Center sign in credentials</span></span>
- <span data-ttu-id="0afd8-134">Ticaret KIMLIĞI GUID 'SI</span><span class="sxs-lookup"><span data-stu-id="0afd8-134">Commerce ID GUID</span></span>
- <span data-ttu-id="0afd8-135">Uygulama KIMLIĞI GUID 'SI</span><span class="sxs-lookup"><span data-stu-id="0afd8-135">App ID GUID</span></span>
- <span data-ttu-id="0afd8-136">Uygulama gizli anahtarı değeri</span><span class="sxs-lookup"><span data-stu-id="0afd8-136">Application secret key value</span></span>
