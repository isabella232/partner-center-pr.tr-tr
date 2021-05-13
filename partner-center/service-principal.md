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
ms.openlocfilehash: 7d12bb66574e6bcee60b2a1df1673dc9171fbee2
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854936"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Azure AD uygulaması (hizmet sorumlusu) İş Ortağı Merkezi

**Uygun roller:** Genel yönetici

İş Ortağı Merkezi'daki Ticari Market programında artık bir Azure AD uygulamasını (hizmet sorumlusu) kullanıcı olarak İş Ortağı Merkezi. (Daha önce Bulut İş Ortağı Portalı veya CPP hesapta bunu yapasınız. İş Ortağı Merkezi'a geçiş İş Ortağı Merkezi CPP hesabı salt okunur olur.)
 
>[!Note] 
>Hizmet sorumlusu, Azure AD uygulamasıyla eş anlamlıdır.

## <a name="add-an-azure-ad-application-service-principal"></a>Azure AD uygulaması ekleme (hizmet sorumlusu)

1. Panodan İş Ortağı Merkezi'yi ve **ardından** Geliştirici **ayarları'ı seçin.**

2. **Kullanıcılar'ı** ve ardından **Azure AD Uygulamaları Ekle'yi seçin.**

3. Mevcut bir Azure AD uygulamasını seçin veya yeni bir uygulama oluşturun.

4. Yeni bir Azure AD Uygulaması sanız aşağıdaki bilgileri dahil edin:  

   - **Yanıt URL'si:** Kullanıcıların Azure AD uygulamalarınızı kullanmak için oturum açmasını istediğiniz URL.

   - **Uygulama Kimliği URI'si:** Azure AD'ye çoklu oturum açma isteği gönderdiği zaman sunulan Azure AD uygulaması için mantıksal tanımlayıcı.

   - **Güvenlik rolleri:** Rol **Yöneticisi** (CPP'de 'Sahip' rolüyle aynı) ve **Geliştirici** (CPP'de 'Katkıda Bulunan' rolüyle aynı) İş Ortağı Merkezi'daki Ticari Market programı için geçerlidir ve bu Azure AD Uygulaması ile ilişkilendirilebilir.  

## <a name="next-steps"></a>Sonraki adımlar

- [İş Ortağı Merkezi'da ticari markete genel bakış](csp-commercial-marketplace-overview.md)