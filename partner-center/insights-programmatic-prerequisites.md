---
title: Analiz verilerine programlı olarak erişim önkoşulları
description: Analiz verilerine programlı olarak erişim önkoşulları
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d4c39025aa3804435dd4d2359b93cd4a2e13ccc4
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376953"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a>Analiz verilerine programlı olarak erişim önkoşulları

**Uygun roller:** Genel yönetici | MPN Yöneticisi

İş ortağı öngörüleri analiz verilerine programlı bir şekilde erişebilmeniz için aşağıdaki gereksinimleri karşılamanız gerekir.

## <a name="mpn-program-enrollment"></a>MPN program kaydı

İş ortağı öngörüleri Analizi verilerine programlı bir şekilde erişmek için MPN programına kaydolduktan ve bir Iş Ortağı Merkezi hesabına sahip olmanız gerekir. Nasıl yapılacağını öğrenmek için bkz. [Iş Ortağı Merkezi 'nde MPN hesabı oluşturma](mpn-create-a-partner-center-account.md)

## <a name="create-azure-active-directory-aad-application"></a>Azure Active Directory (AAD) uygulaması oluşturma

düzenli kullanıcı kimlik bilgileri, iş ortağı Analizler analiz verilerine programlı erişim için kullanılamaz. programlı erişim apı 'lerine erişmek için bir Azure Active Directory (AAD) uygulamasının bir gizli anahtar (uygulama + kullanıcı erişimi) ile birlikte oluşturulması gerekir. AAD uygulaması ve gizli dizi oluşturmayı öğrenmek için bkz [. hızlı başlangıç: Microsoft kimlik platformu bir uygulamayı kaydetme.](/azure/active-directory/develop/quickstart-register-app)   Microsoft Iş ortağı API 'sine erişmek için izin gerekir. İzin ekleme hakkında bilgi edinmek için bkz. [Iş ortağı API kimlik doğrulaması-Iş ortağı](/partner/develop/api-authentication#application-and-user-access)

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a>Kullanıcıya Executive Report Viewer (ERV) rolü atama

İş ortağı öngörüleri Analizi verilerine programlı bir şekilde erişmek için, Executive Report Viewer (ERV) olmalıdır. kullanıcıya erv rolü atamayı öğrenmek için bkz. [partner center Analizler rol tabanlı erişim-iş ortağı merkezi](insights-roles.md)

## <a name="generate-an-aad-token"></a>AAD belirteci oluşturma

Uygulama (istemci) KIMLIĞI, istemci parolası, Kullanıcı KIMLIĞINIZ ve parolanızı kullanarak bir AAD belirteci oluşturmanız gerekir. AAD belirteci oluşturma adımları için   [buraya bakın](insights-programmatic-first-api-call.md#token-generation) .

> [!Note]
> Belirteç bir saat için geçerlidir.

## <a name="next-steps"></a>Sonraki adımlar
[Programlı erişim paradigması](insights-programmatic-access-paradigm.md)