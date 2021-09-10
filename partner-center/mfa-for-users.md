---
title: Kullanıcılarınız için çok faktörlü kimlik doğrulaması ayarlama
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: MFA ile çalışanlarınızı ayarlamayı öğrenin
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 4ff0aa89224c13eddcc6b935c8494188298aeb12
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961424"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>Kullanıcılarınız için çok faktörlü kimlik doğrulaması ayarlama

**Uygun roller:** Genel yönetici

Daha fazla gizlilik koruması ve güvenlik, en önemli önceliklerimiz arasında yer almaktadır. En iyi savunmanın önleme olduğunu ve en zayıf bağlantımız kadar güçlü olduğunu biliyoruz. İşte bu nedenle ekosistemimiz içinde herkesin harekete geçsin ve uygun güvenlik korumalarının hazır olduğundan emin oisun. Tüm iş ortaklarının, iş ortağı kiracılarında kullanıcıları için çok faktörlü kimlik doğrulamasını (MFA) etkinleştirmesini kesinlikle öneririz. 

## <a name="add-multi-factor-authentication-for-your-users"></a>Kullanıcılarınız için çok faktörlü kimlik doğrulaması ekleme

Bu görevi tamamlamak için şirketinizin genel yöneticisi olmak gerekir.

Kullanıcılarınız için MFA'yi Azure AD kiracınıza eklerken etkinleştirmek en kolay yöntemdir.

1. Oturum Azure portal [ve](https://portal.azure.com) ardından Kullanıcı **yönetimi'ne gidin.**
1. Çok **faktörlü kimlik doğrulaması'ı seçin.**
1. Etkinleştirmek istediğiniz kullanıcıyı seçin ve ardından **Etkinleştir'i seçin.**

Bu, bu kullanıcı için MFA'ya olanak sağlar. Etkin, kullanıcının ilk kez oturum a açması için MFA doğrulamasını ayarlaması istenecek anlamına gelir. Bundan sonra, oturum açmalarında, e-posta veya kısa mesaj yoluyla (ayarlanacaklarına bağlı olarak) onlara gönderilen bir kod sağlamaları istenecek.  

:::image type="content" source="images/multi-factor-authentication/security-verification.png" alt-text="Doğrulamayı belirtin.":::

>[!NOTE]
>Yukarıdaki **adımların** aynısını kullanarak ve Zorla'ya seçerek kullanıcılarınızı MFA kullanmaya **zorabilirsiniz.** Daha fazla bilgi edinmek için oturum [açma olaylarının güvenliğini sağlamak için kullanıcı başına Azure Multi-Factor Authentication'a etkinleştirme makalelerini okuyun.](/azure/active-directory/authentication/howto-mfa-userstates) 

Tüm kullanıcılar Devre Dışı olarak **başlar.** Multi-Factor Authentication için kullanıcıları kullanıcı başına Azure Active Directory, durumları Etkin olarak **değişir.** Etkinleştirildiğinde kullanıcılar oturum atayarak kayıt işlemini tamamlar ve durumları Zorlanan **olarak değişir.** 

## <a name="next-steps"></a>Sonraki adımlar

- [Kullanıcılara rol ve izin atama](permissions-overview.md)