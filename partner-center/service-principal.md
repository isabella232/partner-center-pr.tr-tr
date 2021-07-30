---
title: Azure AD hizmet sorumlusu
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
description: Azure AD kiracınıza hizmet sorumlusu ekleme hakkında bilgi edinin. Bunun yapılması, Iş Ortağı Merkezi 'ne bir Azure AD uygulaması (hizmet sorumlusu) ekleme anlamına gelir.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: a7851d270ad51a5a06ebc7d7725a2ae5c803419b
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114842839"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Iş Ortağı Merkezi 'ne bir Azure AD uygulaması (hizmet sorumlusu) ekleme

**Uygun roller**: genel yönetici

iş ortağı merkezi 'ndeki ticari market programında artık iş ortağı merkezi hesabınıza bir kullanıcı olarak Microsoft Azure Active Directory (Azure AD) uygulaması (hizmet sorumlusu) ekleyebileceksiniz. (Bunu daha önce Bulut İş Ortağı Portalı (CPP) hesabınızda yapabileceksiniz. Artık Iş Ortağı Merkezi 'ne geçirdiniz, CPP hesabı salt okunurdur.)
 
>[!Note] 
>Hizmet sorumlusu, Azure AD uygulaması ile eşanlamlıdır.

## <a name="add-an-azure-ad-application-service-principal"></a>Azure AD uygulaması ekleme (hizmet sorumlusu)

1. iş ortağı merkezi panosundan **Ayarlar** ' yi seçin ve ardından **geliştirici ayarları**' nı seçin.

2. **Kullanıcıları** seçin ve ardından **Azure AD uygulamaları Ekle**' yi seçin.

3. Mevcut bir Azure AD uygulaması seçin veya yeni bir tane oluşturun.

4. Yeni bir Azure AD uygulaması oluşturursanız, aşağıdaki bilgileri ekleyin:  

   - **Yanıt URL 'si**: KULLANıCıLARıN Azure AD uygulamanızı kullanmak için oturum açabilecekleri URL.

   - **Uygulama kimliği URI 'si**: Azure AD 'ye yönelik çoklu oturum açma isteği gönderdiğinde sunulan Azure AD uygulaması için mantıksal tanımlayıcı.

   - **Güvenlik rolleri**: roller **Yöneticisi** (cpp ' deki ' Owner ' rolüyle aynı) ve **Geliştirici** (cpp ' de ' katkıda bulunan ' rolüyle aynı), iş ortağı merkezi 'nde ticari Market programına uygulanır ve bu Azure AD uygulamasıyla ilişkilendirilebilir.  

## <a name="next-steps"></a>Sonraki adımlar

- [Iş Ortağı Merkezi 'nde ticari Market 'e genel bakış](csp-commercial-marketplace-overview.md)