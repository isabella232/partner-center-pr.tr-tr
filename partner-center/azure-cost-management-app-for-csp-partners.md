---
title: CSP'ler için Cloudyn'in sunduğu Azure Maliyet Yönetimi
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure kullanımı ve maliyetlerini izlemek üzere uygulamayı kullanabilmeniz için Cloudyn Web uygulamasını nasıl kaydedeceğinizi ve Iş Ortağı Merkezi 'nde BT için gizli anahtar nasıl kullanacağınızı öğrenin.
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: defa691a3bc70cbda45f01cb447d89364a49e3b8
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96535007"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a>CSP iş ortakları için Azure maliyet yönetimi uygulaması ile müşteri Azure kullanımını ve maliyetlerini izleyin  

**Uygun roller**

- Genel yönetici
- Yönetim Aracısı

[Azure maliyet yönetimi hakkında daha fazla bilgi alın](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>Başlamadan önce
Azure maliyet yönetimi 'ni kullanabilmek için aşağıdaki gereksinimleri karşıladığınızdan emin olun:

- Bulut çözümü sağlayıcısı programındaki bir iş ortağıyım.
- Bir Iş Ortağı Merkezi API web uygulaması oluşturma olanağınız vardır.

## <a name="overview"></a>Genel bakış

Cloudyn, müşterilerinizin Azure 'un ne kadarını kullandığını ve bu kullanımın maliyetlerini izlemenize ve yönetmenize olanak tanıyan bir Web uygulamasıdır. Bunu Iş Ortağı Merkezi API 'SI aracılığıyla kullanırsınız.

## <a name="register-your-web-app-in-the-partner-center"></a>Web uygulamanızı Iş Ortağı Merkezi 'ne kaydetme
Iş Ortağı Merkezi 'ne bir Azure Active Directory Web uygulaması kaydettiğinizde, Iş Ortağı Merkezi API 'sine erişim sağlayabilirsiniz. 
1.  [Genel yönetici veya yönetici aracı hesabı](create-user-accounts-and-set-permissions.md)kullanarak [iş ortağı merkezi](https://partnercenter.microsoft.com/pcv/dashboard/overview) ' nde oturum açın.
2.  **İş ortağı merkezi**' nden **Hesap ayarları** &gt; **[uygulama yönetimi](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**' ni seçin.
3.  **Web uygulaması** bölümünde **Yeni Web uygulaması Ekle**' ye tıklayın.
<br> **Note**: daha önce bir Web uygulaması oluşturduysanız adım 3 ' ü atlayabilirsiniz.
4.  Web uygulamanız için **TICARET kimliği** GUID 'Ini ve **uygulama kimliği** GUID 'ini kopyalayın ve kaydedin. Azure maliyet yönetimi uygulamasının 30 günlük ücretsiz deneme sürümünü kullanabilmeniz için her iki kimlik de gereklidir.

## <a name="add-a-secret-key-to-your-app"></a>Uygulamanıza gizli anahtar ekleme
1. **Anahtar Ekle** düğmesinin yanındaki açılan kutuda 1 veya 2 yıl bir süre seçin.
2. **Anahtar Ekle**' ye tıklayın. 
3. Gizli anahtar değerini kopyalayın ve kaydedin. 30 günlük ücretsiz deneme için buna ihtiyacınız olacaktır.<br>
   > [!NOTE]  
   > Uygulama gizli anahtarı, daha uzun süre sonu tarihleri olan parolalar gibidir. Lütfen daha sonra kullanmak için anahtar değerini güvenli bir konuma kaydedin.

## <a name="next-steps"></a>Sonraki adımlar
[30 günlük ücretsiz deneme sürümü](https://go.microsoft.com/fwlink/?linkid=857895)başlatın.
Denemeyi başlatmak için aşağıdaki ayrıntılara ihtiyacınız vardır:
- İş Ortağı Merkezi oturum açma kimlik bilgileri
- Ticaret KIMLIĞI GUID 'SI
- Uygulama KIMLIĞI GUID 'SI
- Uygulama gizli anahtarı değeri
