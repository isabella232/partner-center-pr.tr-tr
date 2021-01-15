---
title: Power BI için Iş ortağı merkezi analizi 'Ni yükler
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Power BI (doğrudan CSP 'deki iş ortakları için) Iş ortağı merkezi analizi uygulamasını yüklemek ve önizlemek için bu makaledeki adımları izleyin.
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 754b3310918df9b38129cf1374ae3731d9d8062e
ms.sourcegitcommit: 1a0c83e2089cb58221bdb24525127378f5197ea8
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/14/2021
ms.locfileid: "98215858"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="328ad-103">Microsoft Power BI için İş Ortağı Merkezi Analizi uygulamasını yükleme ve önizleme</span><span class="sxs-lookup"><span data-stu-id="328ad-103">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>


<span data-ttu-id="328ad-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="328ad-104">**Appropriate roles**</span></span>
-   <span data-ttu-id="328ad-105">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="328ad-105">Global admin</span></span>
-   <span data-ttu-id="328ad-106">Kullanıcı yöneticisi</span><span class="sxs-lookup"><span data-stu-id="328ad-106">User admin</span></span>
-   <span data-ttu-id="328ad-107">Satış Aracısı</span><span class="sxs-lookup"><span data-stu-id="328ad-107">Sales agent</span></span>
-   <span data-ttu-id="328ad-108">Yönetim Aracısı</span><span class="sxs-lookup"><span data-stu-id="328ad-108">Admin agent</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="328ad-109">Başlamadan önce</span><span class="sxs-lookup"><span data-stu-id="328ad-109">Before you begin</span></span>

<span data-ttu-id="328ad-110">Aşağıdaki kullanılabilir Power BI uygulamalar listesinden işletmeniz için en uygun uygulamayı seçin:</span><span class="sxs-lookup"><span data-stu-id="328ad-110">Select the application that is most relevant to your business from the following list of available Power BI apps:</span></span>
- [<span data-ttu-id="328ad-111">Doğrudan sağlayıcı</span><span class="sxs-lookup"><span data-stu-id="328ad-111">Direct Provider</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [<span data-ttu-id="328ad-112">Dolaylı sağlayıcı</span><span class="sxs-lookup"><span data-stu-id="328ad-112">Indirect Provider</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [<span data-ttu-id="328ad-113">Dolaylı satıcı</span><span class="sxs-lookup"><span data-stu-id="328ad-113">Indirect Reseller</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

<span data-ttu-id="328ad-114">Iş ortağı merkezi analizi uygulama Önizleme sürümünü yüklemeden önce, aşağıdaki gereksinimleri karşıladığınızdan emin olun.</span><span class="sxs-lookup"><span data-stu-id="328ad-114">Before you install the Partner Center Analytics app preview version, be sure that you meet the following requirements.</span></span>

- <span data-ttu-id="328ad-115">İşletmeniz için doğru Power BI uygulamayı seçebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="328ad-115">You pick the correct Power BI app for your business.</span></span>

- <span data-ttu-id="328ad-116">Power BI Pro lisansına sahipsiniz.</span><span class="sxs-lookup"><span data-stu-id="328ad-116">You have a Power BI pro license.</span></span>

- <span data-ttu-id="328ad-117">Kiracınıza şablon uygulamaları yüklemek için izinleriniz var.</span><span class="sxs-lookup"><span data-stu-id="328ad-117">You have permissions to install template apps on your tenant.</span></span>

- <span data-ttu-id="328ad-118">Power BI oturum açabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="328ad-118">You can sign in to Power BI.</span></span>

- <span data-ttu-id="328ad-119">[Şirketinizin Azure Active Directory (Azure AD) kiracısında](azure-active-directory-tenants-and-partner-center.md)genel yönetici, yönetici Aracısı veya faturalandırma Yöneticisi olarak oturum açabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="328ad-119">You can sign in as a global admin, admin agent, or billing admin to [your company's Azure Active Directory (Azure AD) tenant](azure-active-directory-tenants-and-partner-center.md).</span></span>

## <a name="to-install-the-app"></a><span data-ttu-id="328ad-120">Uygulamayı yüklemek için</span><span class="sxs-lookup"><span data-stu-id="328ad-120">To install the app</span></span>

1. <span data-ttu-id="328ad-121">Yukarıdaki bölümde verilen uygulama kaynağı bağlantısına (doğrudan sağlayıcı/dolaylı sağlayıcı/dolaylı satıcı) tıklayın.</span><span class="sxs-lookup"><span data-stu-id="328ad-121">Click on the app source link given (Direct Provider/Indirect Provider/Indirect Reseller) in the above section.</span></span>

2. <span data-ttu-id="328ad-122">**Şimdi al**'a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="328ad-122">Click on **GET IT NOW**.</span></span> 

3. <span data-ttu-id="328ad-123">**Devam**' a tıklayarak hüküm ve koşulları kabul edin.</span><span class="sxs-lookup"><span data-stu-id="328ad-123">Agree terms and conditions by clicking **Continue**.</span></span>

4. <span data-ttu-id="328ad-124">Zaten bir hesabınız var mı? **oturum aç '** ı seçin.</span><span class="sxs-lookup"><span data-stu-id="328ad-124">Under Already have an account? select **Sign In**.</span></span>

5. <span data-ttu-id="328ad-125">Sonraki sayfada, Power BI Kullanıcı adınızı ve parolanızı girip oturum aç ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="328ad-125">On the next page, enter your Power BI user name and password and then select Sign In.</span></span>

6. <span data-ttu-id="328ad-126">Çalışma alanı adını sağlayarak çalışma alanını yükler.</span><span class="sxs-lookup"><span data-stu-id="328ad-126">Install the workspace by providing the workspace name.</span></span>

7. <span data-ttu-id="328ad-127">Uygulamalar bölümünde yüklü şablon uygulamalarını bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="328ad-127">You can find the template apps installed under Apps Section.</span></span>

8. <span data-ttu-id="328ad-128">Uygulamalar ' a tıklayın ve yüklü uygulamaları seçin.</span><span class="sxs-lookup"><span data-stu-id="328ad-128">Click on Apps and choose the installed apps.</span></span>

9. <span data-ttu-id="328ad-129">Yeni uygulama ekranınızı açılarak kullanmaya başlayın.</span><span class="sxs-lookup"><span data-stu-id="328ad-129">Get Started with your new app screen opens.</span></span>

10. <span data-ttu-id="328ad-130">Verilere bağlanmak için **Bağlan**' a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="328ad-130">To connect to the data Click **Connect**.</span></span>

11. <span data-ttu-id="328ad-131">**Iş Ortağı Merkezi Analytics** açılır penceresinde, **kimlik doğrulama yönteminin** **oAuth2** olarak ayarlandığını doğrulayın veya listede değilse listeden **oAuth2** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="328ad-131">On the **Connect to Partner Center Analytics** pop-up window, verify that the **Authentication method** is set to **oAuth2** or select **oAuth2** from the list if it's not.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="328ad-132">Bu pencerenin görünmesi birkaç dakika sürebilir.</span><span class="sxs-lookup"><span data-stu-id="328ad-132">This window may take a few minutes to appear.</span></span>

12. <span data-ttu-id="328ad-133">**Iş Ortağı Merkezi Analytics Bağlayıcısı** sayfasında, ŞIRKETINIZIN Azure AD kiracısı için genel yönetici, yönetici Aracısı veya faturalandırma Yöneticisi kimlik bilgileriyle oturum açın ve **oturum aç**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="328ad-133">On the **Partner Center Analytics Connector** page, sign in with global admin, admin agent, or billing admin credentials for your company's Azure AD tenant, and then select **Sign In**.</span></span>
 
13. <span data-ttu-id="328ad-134">Erişim istendiğinde **kabul et**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="328ad-134">When prompted for access, select **Accept**.</span></span> 

<span data-ttu-id="328ad-135">Iş ortağı merkezi analizi hizmeti Power BI bağlandığında, veriler yüklenmeye başlayacaktır.</span><span class="sxs-lookup"><span data-stu-id="328ad-135">Once the Partner Center Analytics service is connected to Power BI, data will begin to load.</span></span> <span data-ttu-id="328ad-136">Veri miktarına bağlı olarak, bu işlem 10 dakikaya kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="328ad-136">Depending on the amount of data, this can take up to 10 minutes.</span></span> 

<span data-ttu-id="328ad-137">Verilerin yüklenmesi tamamlandıktan sonra, Power BI ' de Iş ortağı merkezi analizi uygulama panosunu ve raporlarını kullanmaya başlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="328ad-137">After the data finishes loading, you can start using the Partner Center Analytics app dashboard and reports in Power BI.</span></span>

## <a name="next-steps"></a><span data-ttu-id="328ad-138">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="328ad-138">Next steps</span></span>

[<span data-ttu-id="328ad-139">İş verilerinizi Microsoft için Partner Center Analytics uygulaması ile görüntüleyin Power BI</span><span class="sxs-lookup"><span data-stu-id="328ad-139">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-use.md)
