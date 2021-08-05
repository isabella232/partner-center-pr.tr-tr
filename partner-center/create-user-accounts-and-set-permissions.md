---
title: Kullanıcı hesapları oluşturma ve rol atama
description: Her çalışana erişim izni olmadan önce bir rol İş Ortağı Merkezi. Kullanıcı hesapları oluşturma, rol atama ve izinleri ayarlama hakkında bilgi.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-account
ms.custom: contperf-fy21q2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 71a330356b6c4b3792086f1bc2823e0e067e04ae
ms.sourcegitcommit: 90bf27df911b428b1222f483c32ba6367870e7c5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/04/2021
ms.locfileid: "115101282"
---
# <a name="create-user-accounts"></a>Kullanıcı hesapları oluşturma  

**Uygun roller:** Hesap yöneticisi | Genel yönetici | Kullanıcı yönetimi yöneticisi

Şirket hesabına erişmesi gereken çalışanlar için kullanıcı İş Ortağı Merkezi. Bu görevlerin kullanıcı yönetimi yöneticisi, hesap yöneticisi veya genel yönetici tarafından yapılması gerekir. Bu görevleri gerçekleştiren kullanıcıya Kullanıcı yöneticisi veya Azure Active Directory (AAD) rolü de Genel yönetici. AAD rolleri hakkında daha fazla bilgi için [bkz.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)Azure Active Directory.

## <a name="add-a-new-user"></a>Yeni kullanıcı ekleme

1. Uygulamanın **Ayarlar** sağ üst köşesindeki Simge simgesinden Hesap **İş Ortağı Merkezi'yi ve** ardından Kullanıcı **yönetimi'ne tıklayın.**

2. **Kullanıcı ekle**'yi seçin.

3. Kullanıcının tam adını ve benzersiz e-posta adresini girin.

4. Aracı türünü ve/veya kullanıcıya atamak istediğiniz yönetici türünü seçin. İş Ortağı Merkezi rol tabanlıdır, bu nedenle kullanıcının görünümünü yalnızca kullanıcının belirli görevleri tamamlaması için gereken özellikleri gösterecek şekilde özelleştirmek için izinler atabilirsiniz.  Kullanıcılar rol ataması yapmak isterse, Kullanıcı yönetimi'ne  gidip genel yöneticiyi filtreleerek genel yöneticilerin iletişim kuracaklarını bulabilirler.

5. Kullanıcı hesabını oluşturmak için **Ekle**'yi seçin. Sonraki sayfada kullanıcının ayrıntılarını onaylayın.

> [!IMPORTANT]  
> Bu sayfada görüntülenen yeni kullanıcının oturum açma bilgilerini not edin. Bu bilgileri kopyalayıp yeni kullanıcıya gönderebilirsiniz çünkü daha sonra bu bilgilere yeniden erişesiniz. 

Kullanıcının kullanıcı adı ve geçici parolayla İş Ortağı Merkezi oturum açması gerekir. Kullanıcı, İş Ortağı Merkezi kez oturum açınca parolasını değiştirmesi istenir.

## <a name="assign-user-roles"></a>Kullanıcı rolleri atama

Bu rolde İş Ortağı Merkezi için atanmış bir rolünüz olması gerekir.  Şu anda roller kiracı Azure Active Directory, Bulut Çözümü Sağlayıcısı (CSP) rolleri ve AAD dışı şirket rolleridir. Tek bir şirketin tüm bu rollere ihtiyacı olabilir.

>[!Important]
>Kişilerin kiracınıza erişmek için kiracınıza İş Ortağı Merkezi. Rol atamaları ek erişim sağlar.

## <a name="next-steps"></a>Sonraki adımlar

- [Şirket içinde çalışması gereken çalışanlar için kullanıcı rollerini ve izinlerini İş Ortağı Merkezi](permissions-overview.md)
