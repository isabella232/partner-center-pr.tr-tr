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
ms.openlocfilehash: 64467ec608c2ca87dbc2b7d5dfb02adb08f13c18
ms.sourcegitcommit: 0a6b1e6d845391539f54213efff00af4d23f028c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/14/2020
ms.locfileid: "92530955"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Microsoft Power BI için İş Ortağı Merkezi Analizi uygulamasını yükleme ve önizleme

**Uygulama hedefi**

- İş Ortağı Merkezi

**Uygun roller**
-   Genel yönetici
-   Kullanıcı yöneticisi
-   Satış Aracısı
-   Yönetim Aracısı

## <a name="before-you-begin"></a>Başlamadan önce

Aşağıdaki kullanılabilir Power BI uygulamalar listesinden işletmeniz için en uygun uygulamayı seçin:
- [Doğrudan sağlayıcı](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [Dolaylı sağlayıcı](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [Dolaylı satıcı](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

Iş ortağı merkezi analizi uygulama Önizleme sürümünü yüklemeden önce, aşağıdaki gereksinimleri karşıladığınızdan emin olun.

- İşletmeniz için doğru Power BI uygulamayı seçebilirsiniz.

- Power BI Pro lisansına sahipsiniz.

- Kiracınıza şablon uygulamaları yüklemek için izinleriniz var.

- Power BI oturum açabilirsiniz.

- [Şirketinizin Azure Active Directory (Azure AD) kiracısında](azure-active-directory-tenants-and-partner-center.md)genel yönetici, yönetici Aracısı veya faturalandırma Yöneticisi olarak oturum açabilirsiniz.

## <a name="to-install-the-app"></a>Uygulamayı yüklemek için

1. Yukarıdaki bölümde verilen uygulama kaynağı bağlantısına (doğrudan sağlayıcı/dolaylı sağlayıcı/dolaylı satıcı) tıklayın.

2. **Şimdi al** 'a tıklayın. 

3. **Devam** ' a tıklayarak hüküm ve koşulları kabul edin.

4. Zaten bir hesabınız var mı? **oturum aç '** ı seçin.

5. Sonraki sayfada, Power BI Kullanıcı adınızı ve parolanızı girip oturum aç ' ı seçin.

6. Çalışma alanı adını sağlayarak çalışma alanını yükler.

7. Uygulamalar bölümünde yüklü şablon uygulamalarını bulabilirsiniz.

8. Uygulamalar ' a tıklayın ve yüklü uygulamaları seçin.

9. Yeni uygulama ekranınızı açılarak kullanmaya başlayın.

10. Verilere bağlanmak için **Bağlan** ' a tıklayın.

11. **Iş Ortağı Merkezi Analytics** açılır penceresinde, **kimlik doğrulama yönteminin** **oAuth2** olarak ayarlandığını doğrulayın veya listede değilse listeden **oAuth2** ' yi seçin. 

> [!NOTE]  
>  Bu pencerenin görünmesi birkaç dakika sürebilir.

12. **Iş Ortağı Merkezi Analytics Bağlayıcısı** sayfasında, ŞIRKETINIZIN Azure AD kiracısı için genel yönetici, yönetici Aracısı veya faturalandırma Yöneticisi kimlik bilgileriyle oturum açın ve **oturum aç** ' ı seçin.
 
13. Erişim istendiğinde **kabul et** ' i seçin. 

Iş ortağı merkezi analizi hizmeti Power BI bağlandığında, veriler yüklenmeye başlayacaktır. Veri miktarına bağlı olarak, bu işlem 10 dakikaya kadar sürebilir. 

Verilerin yüklenmesi tamamlandıktan sonra, Power BI ' de Iş ortağı merkezi analizi uygulama panosunu ve raporlarını kullanmaya başlayabilirsiniz.

## <a name="next-steps"></a>Sonraki adımlar

[İş verilerinizi Microsoft için Partner Center Analytics uygulaması ile görüntüleyin Power BI](power-bi-app-for-direct-partners-use.md)
