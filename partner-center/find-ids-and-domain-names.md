---
title: Kiracı KIMLIĞINI, etki alanı adını, Kullanıcı nesne KIMLIĞINI bulun
ms.topic: how-to
ms.date: 09/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure portal-bir kuruluşun Azure AD kiracı KIMLIĞI, etki alanı adı veya belirli bir kullanıcı nesne KIMLIĞINDE kimlik bulmayı öğrenin. Bazı görevlerde bu bilgiler gereklidir.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 4a3695079a9d5b0b3c66b7c2eda52a31888a6660
ms.sourcegitcommit: 3158b0de261539694e37e433c763afa4067e36fb
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/17/2020
ms.locfileid: "92531462"
---
# <a name="locate-important-ids-for-a-user"></a>Bir kullanıcı için önemli kimlikleri bulma

Bu makalede, bir kullanıcı için aşağıdaki bilgileri bulmak üzere [Azure Portal](https://portal.azure.com/) nasıl kullanılacağı açıklanır:

- Kullanıcının kuruluşunun veya şirketinin Microsoft Azure Active Directory (Azure AD) kiracı KIMLIĞI

- Azure AD kiracısı ile ilişkili kuruluşun veya şirketin birincil etki alanı adı

- Kullanıcı nesnesi KIMLIĞI

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Microsoft Azure AD kiracı KIMLIĞINI ve birincil etki alanı adını bulun

Azure portal içinde Azure AD kiracı KIMLIĞINI veya birincil etki alanı adını bulmak için bu adımları izleyin.

> [!NOTE]
> Kiracı KIMLIĞINE farklı uygulamalarda veya kaynaklarda farklı adlar adı verilir. Örneğin, kiracı KIMLIĞI, dizin KIMLIĞI, Azure Active Directory (Azure AD) kiracısı, Microsoft KIMLIĞI veya belirli raporlar için, hatta *tenantguıd* olarak adlandırılır.

1. [Azure portalında](https://portal.azure.com/) oturum açın.

2. Menüden **Azure Active Directory** seçin.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Menüden Azure Active Directory seçeneğini seçen Azure portal gösterir.":::

3. Azure Active Directory **genel bakış** sayfası görüntülenir. Azure AD kiracı KIMLIĞINI veya birincil etki alanı adını bulmak için **KIRACı kimliği** alanını ve **birincil etki alanı** alanını bulun. Bu alanlar, kiracı bilgileri bölümünde görüntülenir.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Menüden Azure Active Directory seçeneğini seçen Azure portal gösterir.":::

4. Kiracı KIMLIĞINI Azure portal birkaç farklı yolla bulabilirsiniz. Menüden **Azure Active Directory** seçin. Ardından, menüdeki **Yönet** bölümünü bulun ve **Özellikler** ' i seçin.

   Özellikler sayfası kullanıcının ilişkili kiracı KIMLIĞINI de görüntüler.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Menüden Azure Active Directory seçeneğini seçen Azure portal gösterir.":::

## <a name="find-the-user-object-id"></a>Kullanıcı nesne KIMLIĞINI bul

Yalnızca etki alanı adını ve kiracı KIMLIĞINI bulmanın her zaman yeterli olmayabilir. Ayrıca, bir kullanıcıya atanan belirli nesne KIMLIĞINI de bulmanız gerekebilir. Azure portal kullanıcının nesne KIMLIĞINI bulmak için şu adımları izleyin:

1. [Azure portalında](https://portal.azure.com/) oturum açın.

2. Menüden **Azure Active Directory** seçin.

3. Menüdeki **Yönet** bölümünü bulun ve ardından **Kullanıcılar** ' ı seçin.

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Menüden Azure Active Directory seçeneğini seçen Azure portal gösterir.":::

4. Kullanıcılar sayfasında, arama kutusuna kullanıcının adını yazın.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Menüden Azure Active Directory seçeneğini seçen Azure portal gösterir.":::

5. Listede göründüğü kullanıcının adını seçin.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Menüden Azure Active Directory seçeneğini seçen Azure portal gösterir.":::

6. Kullanıcının profil sayfasında kimlik bölümünü bulun. Nesne KIMLIĞI alanı, kullanıcının benzersiz nesne KIMLIĞIYLE birlikte görüntülenir.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Menüden Azure Active Directory seçeneğini seçen Azure portal gösterir.":::

## <a name="next-steps"></a>Sonraki adımlar

- [Azure Active Directory 'de Kullanıcı profilleri hakkında daha fazla bilgi edinin](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [İş ortaklarının Iş Ortağı Merkezi 'nde müşteri ayrıntılarını nasıl görebileceğine veya dışa verebileceğine öğrenin](see-your-customer-list.md)