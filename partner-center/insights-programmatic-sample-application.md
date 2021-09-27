---
title: Örnek Uygulama
ms.topic: article
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: İş ortağı içgörüleri verilerine program aracılığıyla erişmek üzere kendi uygulamanızı oluşturmak için örnek uygulamayı kullanın.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e763fd5182489d68e788e88e0f8f1522dac6aba4
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129075358"
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

- Uygulamayı hızlı bir şekilde çalıştırmak için appsettings içinde istemci kimliğini ve istemci gizli **kimliğini güncelleştirin. Development.json**

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="Uygulama sıfırlama geliştirme json'larını":::

Uygulamayı çalıştırarak yerel bir web sunucusu açılır ve bir sayfa açılır ( `https://localhost:44365/ProgrammaticExportSampleApp/sample` ).
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="Örnek uygulamanın kullanıcı arabirimini örnekleme":::

Bu sayfa, yerel makinede çalışan web sunucusuna API çağrıları yapacak ve bu da gerçek programlı erişim API'si çağrılarını yapacaktır.

## <a name="code-snippets"></a>Kod Parçacıkları

Programlı erişim API'si çağrılarını yapmak için C# kodunun temel yapısı aşağıdaki gibidir:
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Kod parçacığını illustrating":::

## <a name="next-steps"></a>Sonraki adımlar

[İş ortağı içgörüleri analiz verilerine erişmek için API'ler](insights-programmatic-analytics-available-api.md)
