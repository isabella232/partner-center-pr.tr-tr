---
title: Örnek Uygulama
ms.topic: article
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: İş ortağı içgörüleri verilerine program aracılığıyla erişmek üzere kendi uygulamanızı oluşturmak için örnek uygulamayı kullanın.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: c558852b7c2af7243187a856067d17a2137cfac867149b80e9c852a1d08d780a
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115683804"
---
# <a name="sample-application"></a>Örnek Uygulama

Örnek uygulamalar C# ve JAVA dillerinde oluşturulur [](https://github.com/partneranalytics) ve GitHub

- [C# Örnek Uygulaması](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [JAVA Örnek Uygulaması](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

Örnek uygulamadan ilham alıp istediğiniz dilde kendi uygulamanızı derlemeyi seçebilirsiniz.

Örnek uygulama aşağıdaki hedeflere ulaşıyor:

- Bir Azure Active Directory (Azure AD) Belirteci üretir.
- Kullanılabilir veri kümelerini alır.
- Kullanıcı tanımlı sorgular oluşturur.
- Kullanıcı tanımlı ve sistem sorgularını alır.
- Bir rapor zamanlar.

Örnek uygulama, diğer işlevler için API'leri çağırma yöntemini kapsıyor. Ancak, diğer API'leri çağırma işlemi yukarıda özetlenenle aynı kalır.

## <a name="how-to-run-the-application"></a>Uygulamayı çalıştırma

- Bu komutu kullanarak depoyu yerel bir sisteme klonlama:

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> Daha fazla yönergeler için, GitHub deposundaki ProgrammaticExportSampleAppMPN/README.md [dosyasına bakın.](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

- Uygulamayı hızlı bir şekilde çalıştırmak için, istemci kimliğini ve istemci gizliappsettings.Development.js **güncelleştirin**

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="Uygulama sıfırlama geliştirme json'larını":::

Uygulamayı çalıştırarak yerel bir web sunucusu başlar ve bir sayfa açılır ( `https://localhost:44365/ProgrammaticExportSampleApp/sample` ).
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="Örnek uygulamanın kullanıcı arabirimini örnekleme":::

Bu sayfa, yerel makinede çalışan web sunucusuna API çağrıları yapacak ve bu da gerçek programlı erişim API'si çağrılarını yapacaktır.

## <a name="code-snippets"></a>Kod Parçacıkları

Programlı erişim API'si çağrılarını yapmak için C# kodunun temel yapısı aşağıdaki gibidir:
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Kod parçacığını illustrating":::

## <a name="next-steps"></a>Sonraki adımlar

[İş ortağı içgörüleri analiz verilerine erişmek için API'ler](insights-programmatic-analytics-available-api.md)
