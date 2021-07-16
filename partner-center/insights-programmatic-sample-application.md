---
title: Örnek uygulama
ms.topic: article
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ortak Öngörüler verilerine programlı bir şekilde erişmek üzere kendi uygulamanızı derlemek için örnek uygulamayı kullanın.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: 6f334b9047c38e8b7763a4ba96d21d987c252682
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376942"
---
# <a name="sample-application"></a><span data-ttu-id="c68d5-103">Örnek uygulama</span><span class="sxs-lookup"><span data-stu-id="c68d5-103">Sample Application</span></span>

<span data-ttu-id="c68d5-104">Örnek uygulamalar C# ve JAVA dillerinde oluşturulur ve [GitHub](https://github.com/partneranalytics) kullanılabilir</span><span class="sxs-lookup"><span data-stu-id="c68d5-104">Sample applications are created in C# and JAVA languages and are available on [GitHub](https://github.com/partneranalytics)</span></span>

- [<span data-ttu-id="c68d5-105">C# örnek uygulaması</span><span class="sxs-lookup"><span data-stu-id="c68d5-105">C# Sample Application</span></span>](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [<span data-ttu-id="c68d5-106">JAVA örnek uygulaması</span><span class="sxs-lookup"><span data-stu-id="c68d5-106">JAVA Sample Application</span></span>](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

<span data-ttu-id="c68d5-107">Örnek uygulamadan alma ve kendi uygulamanızı dilediğiniz dilde oluşturma seçeneğini belirleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c68d5-107">You can choose to take inspiration from the sample application and build your own application in any language.</span></span>

<span data-ttu-id="c68d5-108">Örnek uygulama aşağıdaki hedeflere ulaşır:</span><span class="sxs-lookup"><span data-stu-id="c68d5-108">The sample application achieves the following objectives:</span></span>

- <span data-ttu-id="c68d5-109">Azure Active Directory (Azure AD) belirteci oluşturur.</span><span class="sxs-lookup"><span data-stu-id="c68d5-109">Generates an Azure Active Directory (Azure AD) Token.</span></span>
- <span data-ttu-id="c68d5-110">Kullanılabilir veri kümelerini alır.</span><span class="sxs-lookup"><span data-stu-id="c68d5-110">Gets available datasets.</span></span>
- <span data-ttu-id="c68d5-111">Kullanıcı tanımlı sorgular oluşturur.</span><span class="sxs-lookup"><span data-stu-id="c68d5-111">Creates user defined queries.</span></span>
- <span data-ttu-id="c68d5-112">Kullanıcı tanımlı ve sistem sorgularını alır.</span><span class="sxs-lookup"><span data-stu-id="c68d5-112">Gets user defined and system queries.</span></span>
- <span data-ttu-id="c68d5-113">Bir raporu zamanlar.</span><span class="sxs-lookup"><span data-stu-id="c68d5-113">Schedules a report.</span></span>

<span data-ttu-id="c68d5-114">Örnek uygulama, diğer işlevlere yönelik API 'Leri çağırma yöntemini kapsamaz.</span><span class="sxs-lookup"><span data-stu-id="c68d5-114">The sample application doesn't cover the method of calling APIs for other functionalities.</span></span> <span data-ttu-id="c68d5-115">Ancak, diğer API 'Leri çağırma işlemi yukarıda özetlenen ile aynı kalır.</span><span class="sxs-lookup"><span data-stu-id="c68d5-115">However, the process of calling other APIs remains the same as outlined above.</span></span>

## <a name="how-to-run-the-application"></a><span data-ttu-id="c68d5-116">Uygulamayı çalıştırma</span><span class="sxs-lookup"><span data-stu-id="c68d5-116">How to run the application</span></span>

- <span data-ttu-id="c68d5-117">Şu komutu kullanarak depoyu yerel sisteme kopyalayın:</span><span class="sxs-lookup"><span data-stu-id="c68d5-117">Clone the repository to a local system using this command:</span></span>

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> <span data-ttu-id="c68d5-118">daha fazla yönerge için GitHub [deposundaki](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)ProgrammaticExportSampleAppMPN/README. md dosyasına bakın.</span><span class="sxs-lookup"><span data-stu-id="c68d5-118">For more instructions, refer to the ProgrammaticExportSampleAppMPN/README.md file in the GitHub [repository](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java).</span></span>

- <span data-ttu-id="c68d5-119">Uygulamayı hızlı bir şekilde çalıştırmak için, **üzerindeappsettings.Development.js** istemci kimliğini ve istemci gizli anahtarını güncelleştirin</span><span class="sxs-lookup"><span data-stu-id="c68d5-119">To quickly run the app, update the client id and client secret in the **appsettings.Development.json**</span></span>

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="AppSetting geliştirme JSON 'u":::

<span data-ttu-id="c68d5-121">Uygulamanın çalıştırılması, yerel bir Web sunucusu başlatır ve bir sayfa ( `https://localhost:44365/ProgrammaticExportSampleApp/sample` ) açılır.</span><span class="sxs-lookup"><span data-stu-id="c68d5-121">Running the app will start a local web server and a page will open (`https://localhost:44365/ProgrammaticExportSampleApp/sample`).</span></span>
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="Örnek uygulamanın kullanıcı arabirimini gösteren":::

<span data-ttu-id="c68d5-123">Bu sayfa, yerel makinede çalışan Web sunucusuna API çağrıları yapar, bu da gerçek programlı erişim API 'SI çağrılarını yapar.</span><span class="sxs-lookup"><span data-stu-id="c68d5-123">This page will make API calls to the webserver running on the local machine, which in turn will make the actual programmatic access API calls.</span></span>

## <a name="code-snippets"></a><span data-ttu-id="c68d5-124">Kod Parçacıkları</span><span class="sxs-lookup"><span data-stu-id="c68d5-124">Code Snippets</span></span>

<span data-ttu-id="c68d5-125">Programlı erişim API 'SI çağrıları yapmak için C# kodunun temel yapısı aşağıdaki gibidir:</span><span class="sxs-lookup"><span data-stu-id="c68d5-125">The basic structure of the C# code for doing the programmatic access API calls is as follows:</span></span>
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Kod parçacığını gösteren":::

## <a name="next-steps"></a><span data-ttu-id="c68d5-127">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="c68d5-127">Next steps</span></span>

[<span data-ttu-id="c68d5-128">Partner Insights Analytics verilerine erişim için API 'Ler</span><span class="sxs-lookup"><span data-stu-id="c68d5-128">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)
