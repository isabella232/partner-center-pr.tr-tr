---
title: İş Ortağı Merkezi Analytics'i Power BI
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Uygulama yükleme ve önizlemesini (CSP'de doğrudan Power BI için İş Ortağı Merkezi Analiz uygulaması için) yüklemek ve önizlemek için bu makaledeki adımları izleyin.
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ff95f989ac847bd2c17558d062c86a52110b2ddf
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565058"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="233aa-103">Microsoft Power BI için İş Ortağı Merkezi Analizi uygulamasını yükleme ve önizleme</span><span class="sxs-lookup"><span data-stu-id="233aa-103">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>


<span data-ttu-id="233aa-104">**Uygun roller:** Genel yönetici | Kullanıcı yönetimi yönetici | Satış aracısı | Yönetici aracısı</span><span class="sxs-lookup"><span data-stu-id="233aa-104">**Appropriate roles**: Global admin | User management admin | Sales agent | Admin agent</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="233aa-105">Başlamadan önce</span><span class="sxs-lookup"><span data-stu-id="233aa-105">Before you begin</span></span>

<span data-ttu-id="233aa-106">Aşağıdaki kullanılabilir Microsoft uygulamaları listesinden işletmeniz için en uygun Power BI seçin:</span><span class="sxs-lookup"><span data-stu-id="233aa-106">Select the application that is most relevant to your business from the following list of available Microsoft Power BI apps:</span></span>

- [<span data-ttu-id="233aa-107">Doğrudan Sağlayıcı</span><span class="sxs-lookup"><span data-stu-id="233aa-107">Direct Provider</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [<span data-ttu-id="233aa-108">Dolaylı Sağlayıcı</span><span class="sxs-lookup"><span data-stu-id="233aa-108">Indirect Provider</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [<span data-ttu-id="233aa-109">Dolaylı Kurumsal Bayi</span><span class="sxs-lookup"><span data-stu-id="233aa-109">Indirect Reseller</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

<span data-ttu-id="233aa-110">İş Ortağı Merkezi Analytics uygulama önizleme sürümünü yüklemeden önce, aşağıdaki gereksinimleri karşılasanız emin olun.</span><span class="sxs-lookup"><span data-stu-id="233aa-110">Before you install the Partner Center Analytics app preview version, be sure that you meet the following requirements.</span></span>

- <span data-ttu-id="233aa-111">İşletmeniz için doğru Power BI uygulamayı seçersiniz.</span><span class="sxs-lookup"><span data-stu-id="233aa-111">You pick the correct Power BI app for your business.</span></span>

- <span data-ttu-id="233aa-112">Pro lisansınız Power BI sahipsiniz.</span><span class="sxs-lookup"><span data-stu-id="233aa-112">You have a Power BI pro license.</span></span>

- <span data-ttu-id="233aa-113">Kiracınıza şablon uygulamaları yükleme izinlerine sahipsiniz.</span><span class="sxs-lookup"><span data-stu-id="233aa-113">You have permissions to install template apps on your tenant.</span></span>

- <span data-ttu-id="233aa-114">Bu oturum açma Power BI.</span><span class="sxs-lookup"><span data-stu-id="233aa-114">You can sign in to Power BI.</span></span>

- <span data-ttu-id="233aa-115">Genel yönetici, yönetici aracısı veya faturalama yöneticisi olarak, şirketinizin Azure Active Directory [(Azure AD) kiracısı olarak oturumabilirsiniz.](azure-active-directory-tenants-and-partner-center.md)</span><span class="sxs-lookup"><span data-stu-id="233aa-115">You can sign in as a global admin, admin agent, or billing admin to [your company's Azure Active Directory (Azure AD) tenant](azure-active-directory-tenants-and-partner-center.md).</span></span>

## <a name="to-install-the-app"></a><span data-ttu-id="233aa-116">Uygulamayı yüklemek için</span><span class="sxs-lookup"><span data-stu-id="233aa-116">To install the app</span></span>

1. <span data-ttu-id="233aa-117">Yukarıdaki bölümde verilen uygulama kaynağı bağlantısını (Doğrudan Sağlayıcı/Dolaylı Sağlayıcı/Dolaylı Kurumsal Bayi) seçin.</span><span class="sxs-lookup"><span data-stu-id="233aa-117">Select the app source link given (Direct Provider/Indirect Provider/Indirect Reseller) in the above section.</span></span>

2. <span data-ttu-id="233aa-118">ŞIMDI **AL'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="233aa-118">Select **GET IT NOW**.</span></span> 

3. <span data-ttu-id="233aa-119">Devam'ı seçerek hüküm ve koşulları **kabul edersiniz.**</span><span class="sxs-lookup"><span data-stu-id="233aa-119">Agree terms and conditions by selecting **Continue**.</span></span>

4. <span data-ttu-id="233aa-120">Zaten bir hesabınız mı var? Oturum **Açma'ya seçin.**</span><span class="sxs-lookup"><span data-stu-id="233aa-120">Under Already have an account? select **Sign In**.</span></span>

5. <span data-ttu-id="233aa-121">Sonraki sayfada, kullanıcı adı Power BI parolanızı girin ve ardından **Oturum'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="233aa-121">On the next page, enter your Power BI user name and password and then select **Sign In**.</span></span>

6. <span data-ttu-id="233aa-122">Çalışma alanı adını sağlayarak çalışma alanını yükleyin.</span><span class="sxs-lookup"><span data-stu-id="233aa-122">Install the workspace by providing the workspace name.</span></span>

7. <span data-ttu-id="233aa-123">Yüklü şablon uygulamalarını Uygulamalar Bölümünde bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="233aa-123">You can find the template apps installed under Apps Section.</span></span>

8. <span data-ttu-id="233aa-124">**Uygulamalar'ı** ve yüklü uygulamaları seçin.</span><span class="sxs-lookup"><span data-stu-id="233aa-124">Select **Apps** and choose the installed apps.</span></span>

9. <span data-ttu-id="233aa-125">Başla uygulama ekranınız açılır.</span><span class="sxs-lookup"><span data-stu-id="233aa-125">Get Started with your new app screen opens.</span></span>

10. <span data-ttu-id="233aa-126">Verilere bağlanmak için Bağlan'ı **seçin.**</span><span class="sxs-lookup"><span data-stu-id="233aa-126">To connect to the data, select **Connect**.</span></span>

11. <span data-ttu-id="233aa-127">İş Ortağı Merkezi **Analytics'e** bağlan açılır penceresinde, Kimlik doğrulama  yönteminin oAuth2 olarak ayar olduğunu doğrulayın veya ayarlanmazsa listeden **oAuth2'yi** seçin. </span><span class="sxs-lookup"><span data-stu-id="233aa-127">On the **Connect to Partner Center Analytics** pop-up window, verify that the **Authentication method** is set to **oAuth2** or select **oAuth2** from the list if it's not.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="233aa-128">Bu pencerenin görünmesi birkaç dakika sürebilir.</span><span class="sxs-lookup"><span data-stu-id="233aa-128">This window may take a few minutes to appear.</span></span>

12. <span data-ttu-id="233aa-129">İş Ortağı Merkezi **Analytics Bağlayıcısı** sayfasında, şirketinizin Azure AD kiracısı için genel yönetici, yönetici aracısı veya faturalama yöneticisi kimlik bilgileriyle oturum açma ve ardından Oturum **Açma'ya tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="233aa-129">On the **Partner Center Analytics Connector** page, sign in with global admin, admin agent, or billing admin credentials for your company's Azure AD tenant, and then select **Sign In**.</span></span>
 
13. <span data-ttu-id="233aa-130">Erişim istendiğinde Kabul Et'i **seçin.**</span><span class="sxs-lookup"><span data-stu-id="233aa-130">When prompted for access, select **Accept**.</span></span> 

<span data-ttu-id="233aa-131">İş Ortağı Merkezi Analytics hizmeti Power BI veri yüklenmeye başlar.</span><span class="sxs-lookup"><span data-stu-id="233aa-131">Once the Partner Center Analytics service is connected to Power BI, data will begin to load.</span></span> <span data-ttu-id="233aa-132">Veri miktarına bağlı olarak bu süre 10 dakika kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="233aa-132">Depending on the amount of data, this can take up to 10 minutes.</span></span> 

<span data-ttu-id="233aa-133">Verilerin yüklenmesi tamam olduktan sonra, İş Ortağı Merkezi Analytics uygulama panosu ve raporları Power BI.</span><span class="sxs-lookup"><span data-stu-id="233aa-133">After the data finishes loading, you can start using the Partner Center Analytics app dashboard and reports in Power BI.</span></span>

## <a name="next-steps"></a><span data-ttu-id="233aa-134">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="233aa-134">Next steps</span></span>

[<span data-ttu-id="233aa-135">Microsoft Power BI için İş Ortağı Merkezi Analytics uygulamasıyla iş verilerinizi Power BI</span><span class="sxs-lookup"><span data-stu-id="233aa-135">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-use.md)
