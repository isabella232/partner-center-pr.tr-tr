---
title: Azure AD hizmet sorumlusu
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure AD kiracınıza hizmet sorumlusu ekleme hakkında bilgi edinin. Bunun için azure ad uygulaması (hizmet sorumlusu) İş Ortağı Merkezi.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 3698032a632384e8416664c9564819d7c4da9c38
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551563"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Azure AD uygulaması (hizmet sorumlusu) İş Ortağı Merkezi

**Uygun roller:** Genel yönetici

İş Ortağı Merkezi'daki Ticari Market programında artık Microsoft Azure Active Directory (Azure AD) uygulamasını (hizmet sorumlusu) kullanıcı olarak İş Ortağı Merkezi. (Daha önce Bulut İş Ortağı Portalı (CPP) hesabınızla bunu yapasınız. İş Ortağı Merkezi'a geçiş İş Ortağı Merkezi CPP hesabı salt okunur olur.)
 
>[!Note] 
>Hizmet sorumlusu, Azure AD uygulamasıyla eş anlamlıdır.

## <a name="add-an-azure-ad-application-service-principal"></a>Azure AD uygulaması ekleme (hizmet sorumlusu)

1. Panodan İş Ortağı Merkezi'yi ve **ardından** Geliştirici **ayarları'ı seçin.**

2. **Kullanıcılar'ı** ve ardından **Azure AD Uygulamaları Ekle'yi seçin.**

3. Mevcut bir Azure AD uygulamasını seçin veya yeni bir uygulama oluşturun.

4. Yeni bir Azure AD uygulaması sanız aşağıdaki bilgileri dahil edin:  

   - **Yanıt URL'si:** Kullanıcıların Azure AD uygulamalarınızı kullanmak için oturum açmasını istediğiniz URL.

   - **Uygulama Kimliği URI'si:** Azure AD'ye çoklu oturum açma isteği gönderdiği zaman sunulan Azure AD uygulaması için mantıksal tanımlayıcı.

   - **Güvenlik rolleri:** Rol **Yöneticisi** (CPP'de 'Sahip' rolüyle aynı) ve **Geliştirici** (CPP'de 'Katkıda Bulunan' rolüyle aynı) İş Ortağı Merkezi'daki Ticari Market programı için geçerlidir ve bu Azure AD Uygulaması ile ilişkilendirilebilir.  

## <a name="next-steps"></a>Sonraki adımlar

- [İş Ortağı Merkezi'da ticari markete genel bakış](csp-commercial-marketplace-overview.md)