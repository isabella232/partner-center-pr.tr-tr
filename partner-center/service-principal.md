---
title: Azure AD hizmet sorumlusu
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
description: Azure AD kiracınıza hizmet sorumlusu ekleme hakkında bilgi edinin. Bunun için azure ad uygulaması (hizmet sorumlusu) İş Ortağı Merkezi.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: a7851d270ad51a5a06ebc7d7725a2ae5c803419b
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248580"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Azure AD uygulaması (hizmet sorumlusu) İş Ortağı Merkezi

**Uygun roller:** Genel yönetici

İş Ortağı Merkezi'daki Ticari Market programında artık Microsoft Azure Active Directory (Azure AD) uygulamasını (hizmet sorumlusu) kullanıcı olarak İş Ortağı Merkezi. (Daha önce Bulut İş Ortağı Portalı (CPP) hesabınızla bunu yapasınız. İş Ortağı Merkezi'ye geçiş İş Ortağı Merkezi CPP hesabı salt okunur olur.)
 
>[!Note] 
>Hizmet sorumlusu, Azure AD uygulamasıyla eş anlamlıdır.

## <a name="add-an-azure-ad-application-service-principal"></a>Azure AD uygulaması ekleme (hizmet sorumlusu)

1. Uygulama panosundan İş Ortağı Merkezi'yi **ve Ayarlar'yi** seçin.

2. **Kullanıcılar'ı** ve ardından **Azure AD Uygulamaları Ekle'yi seçin.**

3. Mevcut bir Azure AD uygulamasını seçin veya yeni bir uygulama oluşturun.

4. Yeni bir Azure AD uygulaması sanız aşağıdaki bilgileri dahil edin:  

   - **Yanıt** URL'si: Kullanıcıların Azure AD uygulamalarınızı kullanmak için oturum açmasını istediğiniz URL.

   - **Uygulama Kimliği URI'si:** Azure AD'ye çoklu oturum açma isteği gönderdiği zaman sunulan Azure AD uygulaması için mantıksal tanımlayıcı.

   - **Güvenlik rolleri:** Rol **Yöneticisi** (CPP'de 'Sahip' rolüyle aynı) ve **Geliştirici** (CPP'de 'Katkıda Bulunan' rolüyle aynı) İş Ortağı Merkezi'daki Ticari Market programı için geçerlidir ve bu Azure AD Uygulaması ile ilişkilendirilebilir.  

## <a name="next-steps"></a>Sonraki adımlar

- [İş Ortağı Merkezi'da ticari markete genel bakış](csp-commercial-marketplace-overview.md)