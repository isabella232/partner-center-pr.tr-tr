---
title: Kullanıcı hesapları oluşturma ve rol atama
description: Iş Ortağı Merkezi 'Ne erişebilmek için her çalışana bir rol atanması gerekir. Kullanıcı hesapları oluşturma, rol atama ve izinleri ayarlama hakkında bilgi edinin.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperf-fy21q2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: c8fad4432f9aabba69877d80038ec9e2665c639d
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2020
ms.locfileid: "97492543"
---
# <a name="create-user-accounts"></a>Kullanıcı hesapları oluşturma  

**Uygun roller**

- Hesap yöneticisi
- Genel yönetici
- Kullanıcı Yönetimi Yöneticisi

Iş Ortağı Merkezi 'ne erişmesi gereken çalışanlar için Kullanıcı hesapları oluşturun. Bu görevlerin Kullanıcı Yönetimi Yöneticisi, hesap yöneticisi veya genel yönetici tarafından yapılması gerekir. Bu görevleri gerçekleştiren kullanıcıya ayrıca Kullanıcı Yöneticisi veya genel yönetici Azure Active Directory (AAD) rolleri atanmalıdır. AAD rolleri hakkında daha fazla bilgi için [Azure Active Directory Içindeki yönetici rolü izinleri](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)bölümüne bakın.

## <a name="add-a-new-user"></a>Yeni kullanıcı ekleme

1. Iş Ortağı Merkezi 'nin sağ üst köşesindeki **Ayarlar** simgesinden **Hesap ayarları** ' nı seçin ve ardından **Kullanıcı yönetimi**' ni seçin.

2. **Kullanıcı ekle**'yi seçin.

3. Kullanıcının tam adını ve benzersiz e-posta adresini girin.

4. Aracının türünü ve/veya kullanıcıya atamak istediğiniz yönetici türünü seçin. İş ortağı merkezi erişimi rol tabanlıdır, bu nedenle kullanıcının görünümünü yalnızca kullanıcının belirli görevleri tamamlaması için ihtiyaç duyacağı özellikleri gösterecek şekilde özelleştirmek için izinler atayabilirsiniz.  Kullanıcılar bir rol ataması istiyorlarsa, genel yöneticilerle **Kullanıcı yönetimine** ve filtrelemeye geçerek genel yöneticileri iletişim kurmak üzere bulabilir.

5. Kullanıcı hesabını oluşturmak için **Ekle**'yi seçin. Sonraki sayfada kullanıcının ayrıntılarını onaylayın.

> [!IMPORTANT]  
> Yeni kullanıcının oturum açma bilgilerini bu sayfada bir yere unutmayın. Daha sonra tekrar erişemeyeceksiniz, bu bilgileri kopyalayıp yeni kullanıcıya gönderdiğinizden emin olun. 

Kullanıcının Iş Ortağı Merkezi 'nde Kullanıcı adı ve geçici parola ile oturum açması gerekir. Kullanıcı Iş Ortağı Merkezi 'ne ilk kez oturum açtığında, kullanıcıların parolalarını değiştirmesi istenir.

## <a name="assign-user-roles"></a>Kullanıcı rolleri atama

İş Ortağı Merkezi 'nde çalışmak için atanmış bir role sahip olmanız gerekir.  Şu anda, roller Azure Active Directory kiracı rolleri, bulut çözümü sağlayıcısı (CSP) rolleri ve AAD olmayan şirket rollerini içerir. Tek bir şirketin bu rollerin tümüne ihtiyacı olabilir.

>[!Important]
>Iş Ortağı Merkezi 'ne erişmek için kişisel kişilerin kiracınızda listelenmesi gerekir. Rol atamaları ek erişim sağlar.

## <a name="next-steps"></a>Sonraki adımlar

- [İş Ortağı Merkezi 'nde çalışması gereken çalışanlar için Kullanıcı rolleri ve izinleri atama](permissions-overview.md)
