---
title: Kullanıcılarınız için çok faktörlü kimlik doğrulaması ayarlama
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: MFA ile çalışanlarınızın nasıl ayarlanacağını öğrenin
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f42c97be88a1a505f7e0ae9b8af0d4a9167d8447
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182384"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>Kullanıcılarınız için çok faktörlü kimlik doğrulaması ayarlama

**Uygun roller**

- Genel yönetici

Büyük gizlilik korumaları ve güvenlik, en iyi önceliklerimiz arasındadır. En iyi savunması önleme olduğunu ve yalnızca zayıf bağlantımız kadar güçlü olduğunu biliyoruz. Bu nedenle, ekosistemimizde herkesin işlem yapması ve uygun güvenlik korumalarının yerinde olduğundan emin olunması gerekir. Tüm ortakların kendi iş ortağı kiracılarında kullanıcıları için Multi-Factor Authentication 'ı (MFA) etkinleştirmesine kesinlikle önerilir. 

## <a name="add-multi-factor-authentication-for-your-users"></a>Kullanıcılarınız için Multi-Factor Authentication ekleme

Bu görevi gerçekleştirmek için şirketiniz için genel yönetici olmanız gerekir.

Azure AD kiracınıza eklerken kullanıcılarınız için MFA 'yı etkinleştirmek en kolay yoldur.

1. [Azure Portal](https://portal.azure.com) oturum açın ve ardından **Kullanıcı yönetimi**' ne gidin.
1. **Multi-Factor Authentication**'ı seçin.
1. Etkinleştirmek istediğiniz kullanıcıyı seçin ve ardından **Etkinleştir**' i seçin.

Bu, bu kullanıcı için MFA 'yı etkinleştirir. Etkin, kullanıcıdan ilk kez oturum açtıklarında MFA doğrulamasını ayarlaması istenecektir. Bundan sonra oturum açma sırasında, bunlara e-posta veya kısa mesaj yoluyla (ayarlandıkları bağlı olarak) bir kod vermesi istenir.  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Nasıl doğrulanalınacağını belirtin":::

>[!NOTE]
>Kullanıcılarınıza, yukarıdaki gibi aynı adımları kullanarak ve **Uygula**' yı seçerek MFA 'Yı kullanmaya **zorlayabilirsiniz** . Daha fazla bilgi edinmek için, [oturum açma olaylarını güvenli hale getirmek üzere Kullanıcı başına Azure Multi-Factor Authentication etkinleştirme](/azure/active-directory/authentication/howto-mfa-userstates)makalesini okuyun. 

Tüm kullanıcılar **devre dışı bırakıldı**. Kullanıcıları Kullanıcı başına Azure Multi-Factor Authentication kaydettiğinizde, durumları **etkin** olarak değişir. Etkin kullanıcılar oturum açıp kayıt işlemini tamamladıktan sonra, durumu **Zorlanmış** olarak değişir. 

## <a name="next-steps"></a>Sonraki adımlar

- [Kullanıcılara rol ve izin atama](permissions-overview.md)