---
title: Analiz verilerine program aracılığıyla erişmek için önkoşullar
description: Analiz verilerine program aracılığıyla erişmek için önkoşullar
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 9359cb25fee113ee166c7ce407ed70f319f3e6b6
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129071095"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a>Analiz verilerine program aracılığıyla erişmek için önkoşullar

**Uygun roller:** Genel yönetici | MPN yöneticisi

İş ortağı içgörüleri analiz verilerine program aracılığıyla erişmeden önce aşağıdaki gereksinimleri karşılamanız gerekir.

## <a name="mpn-program-enrollment"></a>MPN Programı kaydı

İş ortağı içgörüleri analiz verilerine program aracılığıyla erişmek için MPN programına kaydolmanız ve bir hesap İş Ortağı Merkezi gerekir. Nasıl olduğunu öğrenmek için [bkz. İş Ortağı Merkezi'da MPN hesabı oluşturma](mpn-create-a-partner-center-account.md)

## <a name="create-azure-active-directory-aad-application"></a>Azure Active Directory (AAD) uygulaması oluşturma

İş Ortağı ve Analiz verilerine program aracılığıyla erişmek için normal Analizler bilgileri kullanılamaz. Program Azure Active Directory erişim API'lerine erişmek için gizli bir (uygulama + kullanıcı erişimi) ile birlikte bir Azure Active Directory (AAD) uygulaması oluşturularak. AAD uygulaması ve gizli bilgi oluşturma hakkında bilgi edinmek için bkz. Hızlı Başlangıç: Uygulama kaydetme [Microsoft kimlik platformu.](/azure/active-directory/develop/quickstart-register-app)   Microsoft Partner API'a erişmek için izin gereklidir. İzin ekleme hakkında bilgi edinmek için bkz. [Partner API kimlik doğrulaması - İş Ortağı](/partner/develop/api-authentication#application-and-user-access)

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a>Kullanıcıya Yönetici Rapor Görüntüleyicisi (ERV) rolü atama

İş ortağı içgörüleri analiz verilerine program aracılığıyla erişmek için Yönetici Rapor Görüntüleyicisi'ne (ERV) sahipsiniz. Kullanıcıya ERV rolü atama hakkında bilgi edinmek için [bkz. İş Ortağı Merkezi Analizler tabanlı erişim - İş Ortağı Merkezi](insights-roles.md)

## <a name="generate-an-aad-token"></a>AAD belirteci oluşturma

Uygulama (istemci) kimliğini, istemci gizli parolasını, kullanıcı kimliğini ve parolanızı kullanarak bir AAD belirteci oluşturabilirsiniz.   [AAD](insights-programmatic-first-api-call.md#token-generation) belirteci oluşturma adımları için buraya göz atabilirsiniz.

> [!Note]
> Belirteç bir saat boyunca geçerlidir.

## <a name="next-steps"></a>Sonraki adımlar
[Programlı erişim paradigması](insights-programmatic-access-paradigm.md)