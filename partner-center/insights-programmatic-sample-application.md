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
# <a name="sample-application"></a>Örnek uygulama

Örnek uygulamalar C# ve JAVA dillerinde oluşturulur ve [GitHub](https://github.com/partneranalytics) kullanılabilir

- [C# örnek uygulaması](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [JAVA örnek uygulaması](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

Örnek uygulamadan alma ve kendi uygulamanızı dilediğiniz dilde oluşturma seçeneğini belirleyebilirsiniz.

Örnek uygulama aşağıdaki hedeflere ulaşır:

- Azure Active Directory (Azure AD) belirteci oluşturur.
- Kullanılabilir veri kümelerini alır.
- Kullanıcı tanımlı sorgular oluşturur.
- Kullanıcı tanımlı ve sistem sorgularını alır.
- Bir raporu zamanlar.

Örnek uygulama, diğer işlevlere yönelik API 'Leri çağırma yöntemini kapsamaz. Ancak, diğer API 'Leri çağırma işlemi yukarıda özetlenen ile aynı kalır.

## <a name="how-to-run-the-application"></a>Uygulamayı çalıştırma

- Şu komutu kullanarak depoyu yerel sisteme kopyalayın:

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> daha fazla yönerge için GitHub [deposundaki](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)ProgrammaticExportSampleAppMPN/README. md dosyasına bakın.

- Uygulamayı hızlı bir şekilde çalıştırmak için, **üzerindeappsettings.Development.js** istemci kimliğini ve istemci gizli anahtarını güncelleştirin

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="AppSetting geliştirme JSON 'u":::

Uygulamanın çalıştırılması, yerel bir Web sunucusu başlatır ve bir sayfa ( `https://localhost:44365/ProgrammaticExportSampleApp/sample` ) açılır.
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="Örnek uygulamanın kullanıcı arabirimini gösteren":::

Bu sayfa, yerel makinede çalışan Web sunucusuna API çağrıları yapar, bu da gerçek programlı erişim API 'SI çağrılarını yapar.

## <a name="code-snippets"></a>Kod Parçacıkları

Programlı erişim API 'SI çağrıları yapmak için C# kodunun temel yapısı aşağıdaki gibidir:
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Kod parçacığını gösteren":::

## <a name="next-steps"></a>Sonraki adımlar

[Partner Insights Analytics verilerine erişim için API 'Ler](insights-programmatic-analytics-available-api.md)
