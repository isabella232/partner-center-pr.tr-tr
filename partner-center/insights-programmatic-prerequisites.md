---
title: Analiz verilerine program aracılığıyla erişmek için önkoşullar
description: Analiz verilerine program aracılığıyla erişmek için önkoşullar
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 12c466cce37ac252fedf5f72ef90e390bb1af256
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960824"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a>Analiz verilerine program aracılığıyla erişmek için önkoşullar

**Uygun roller:** Genel yönetici | MPN yöneticisi

İş ortağı içgörüleri analiz verilerine program aracılığıyla erişmeden önce aşağıdaki gereksinimleri karşılamanız gerekir.

## <a name="mpn-program-enrollment"></a>MPN Programı kaydı

İş ortağı içgörüleri analiz verilerine program aracılığıyla erişmek için MPN programına kaydolmanız ve bir İş Ortağı Merkezi gerekir. Nasıl olduğunu öğrenmek için [bkz. İş Ortağı Merkezi'de MPN hesabı oluşturma](mpn-create-a-partner-center-account.md)

## <a name="create-azure-active-directory-aad-application"></a>Azure Active Directory (AAD) uygulaması oluşturma

İş Ortağı ve Analiz verilerine program aracılığıyla erişmek için normal Analizler bilgileri kullanılamaz. Program Azure Active Directory erişim API'lerine erişmek için gizli bir (uygulama + kullanıcı erişimi) ile birlikte bir Azure Active Directory (AAD) uygulamasının da oluşturulacak olması gerekir. AAD uygulaması ve gizli bilgi oluşturma hakkında bilgi edinmek için bkz. Hızlı Başlangıç: Uygulama kaydetme [Microsoft kimlik platformu.](/azure/active-directory/develop/quickstart-register-app)   Microsoft Partner API'a erişmek için izin gereklidir. İzin ekleme hakkında bilgi edinmek için bkz. [Partner API kimlik doğrulaması - İş Ortağı](/partner/develop/api-authentication#application-and-user-access)

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a>Kullanıcıya Yönetici Rapor Görüntüleyicisi (ERV) rolü atama

İş ortağı içgörüleri analiz verilerine program aracılığıyla erişmek için Yönetici Rapor Görüntüleyicisi'ne (ERV) sahipsiniz. Kullanıcıya ERV rolü atamayı öğrenmek için [bkz. İş Ortağı Merkezi Analizler tabanlı erişim - İş Ortağı Merkezi](insights-roles.md)

## <a name="generate-an-aad-token"></a>AAD belirteci oluşturma

Uygulama (istemci) kimliğini, istemci gizli parolasını, kullanıcı kimliğini ve parolanızı kullanarak bir AAD belirteci oluşturmanız gerekir.   [AAD](insights-programmatic-first-api-call.md#token-generation) belirteci oluşturma adımları için buraya göz atabilirsiniz.

> [!Note]
> Belirteç bir saat boyunca geçerlidir.

## <a name="next-steps"></a>Sonraki adımlar
[Programlı erişim paradigması](insights-programmatic-access-paradigm.md)