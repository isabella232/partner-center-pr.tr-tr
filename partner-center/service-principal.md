---
title: Azure AD hizmet sorumlusu
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure AD kiracınıza hizmet sorumlusu ekleme hakkında bilgi edinin. Bunun yapılması, Iş Ortağı Merkezi 'ne bir Azure AD uygulaması (hizmet sorumlusu) ekleme anlamına gelir.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 21ef2aaa46359570bbf13c12c5fb6c1f5eab080a
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2020
ms.locfileid: "92531218"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Iş Ortağı Merkezi 'ne bir Azure AD uygulaması (hizmet sorumlusu) ekleme

**Uygulama hedefi**

- İş Ortağı Merkezi

**Uygun roller**

- Genel yönetici

Iş Ortağı Merkezi 'ndeki ticari Market programında artık Iş Ortağı Merkezi hesabınıza bir kullanıcı olarak bir Azure AD uygulaması (hizmet sorumlusu) ekleyebileceksiniz. (Bunu daha önce Bulut İş Ortağı Portalı veya CPP, hesabınızda de yapabileceksiniz. Artık Iş Ortağı Merkezi 'ne geçirdiniz, CPP hesabı salt okunurdur.)
 
>[!Note] 
>Hizmet sorumlusu, Azure AD uygulaması ile eşanlamlıdır.

## <a name="add-an-azure-ad-application-service-principal"></a>Azure AD uygulaması ekleme (hizmet sorumlusu)

1. Iş Ortağı Merkezi panosundan **Ayarlar** ' ı seçin ve ardından **Geliştirici ayarları** ' nı seçin.

2. **Kullanıcıları** seçin ve ardından **Azure AD uygulamaları Ekle** ' yi seçin.

3. Mevcut bir Azure AD uygulaması seçin veya yeni bir tane oluşturun.

4. Yeni bir Azure AD uygulaması oluşturursanız, aşağıdaki bilgileri ekleyin:  

   - **Yanıt URL 'si** : KULLANıCıLARıN Azure AD uygulamanızı kullanmak için oturum açabilecekleri URL.

   - **Uygulama kimliği URI 'si** : Azure AD 'ye yönelik çoklu oturum açma isteği gönderdiğinde sunulan Azure AD uygulaması için mantıksal tanımlayıcı.

   - **Güvenlik rolleri** : roller **Yöneticisi** (cpp ' deki ' Owner ' rolüyle aynı) ve **Geliştirici** (cpp ' de ' katkıda bulunan ' rolüyle aynı), iş ortağı merkezi 'nde ticari Market programına uygulanır ve bu Azure AD uygulamasıyla ilişkilendirilebilir.  

## <a name="next-steps"></a>Sonraki adımlar

- [Iş Ortağı Merkezi 'nde ticari Market 'e genel bakış](csp-commercial-marketplace-overview.md)