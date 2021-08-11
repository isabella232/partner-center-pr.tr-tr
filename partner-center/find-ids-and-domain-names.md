---
title: Kiracı KIMLIĞINI, etki alanı adını, Kullanıcı nesne KIMLIĞINI bulun
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Azure portal-bir kuruluşun Azure AD kiracı KIMLIĞI, etki alanı adı veya belirli bir kullanıcı nesne KIMLIĞINDE kimlik bulmayı öğrenin. Bazı görevlerde bu bilgiler gereklidir.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 6f701d3f1b69add9b5ca6691f36f018b00414aa1309fa08351158bdb06e02a87
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115683982"
---
# <a name="locate-important-ids-for-a-user"></a>Bir kullanıcı için önemli kimlikleri bulma

**Uygun roller**: genel yönetici

Bu makalede, bir kullanıcı için aşağıdaki bilgileri bulmak üzere [Azure Portal](https://portal.azure.com/) nasıl kullanılacağı açıklanır:

- kullanıcının kuruluşunun veya şirketinin Microsoft Azure Active Directory (Azure AD) kiracı kimliği

- Azure AD kiracısı ile ilişkili kuruluşun veya şirketin birincil etki alanı adı

- Kullanıcı nesnesi KIMLIĞI

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Microsoft Azure AD kiracı kimliğini ve birincil etki alanı adını bulun

Azure portal içinde Azure AD kiracı KIMLIĞINI veya birincil etki alanı adını bulmak için bu adımları izleyin. (Bir kiracı KIMLIĞINI programlı bir şekilde bulmak istiyorsanız bkz. [PowerShell veya CLI ile KIRACı kimliğini bulma](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)

> [!NOTE]
> Kiracı KIMLIĞINE farklı uygulamalarda veya kaynaklarda farklı adlar adı verilir. örneğin, kiracı kimliği, dizin kimliği, Azure Active Directory (Azure AD) kiracısı, Microsoft kimliği veya belirli raporlar için, hatta *tenantguıd* olarak adlandırılır.

1. [Azure Portal](https://portal.azure.com/)’ında oturum açın.

2. menüden **Azure Active Directory** seçin.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="menüden Azure Active Directory seçeneğini seçen Azure portal gösterir.":::

3. Azure Active Directory **genel bakış** sayfası görüntülenir. Azure AD kiracı KIMLIĞINI veya birincil etki alanı adını bulmak için **KIRACı kimliği** alanını ve **birincil etki alanı** alanını bulun. Bu alanlar, kiracı bilgileri bölümünde görüntülenir.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="İki Vurgulanan alan, kiracı KIMLIĞI ve birincil etki alanı adı içeren genel bakış sayfasını gösterir.":::

4. Kiracı KIMLIĞINI Azure portal birkaç farklı yolla bulabilirsiniz. menüden **Azure Active Directory** seçin. Ardından, menüdeki **Yönet** bölümünü bulun ve **Özellikler**' i seçin.

   Özellikler sayfası kullanıcının ilişkili kiracı KIMLIĞINI de görüntüler.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Vurgulanan kiracı KIMLIĞI alanıyla birlikte Özellikler sayfasını gösterir.":::

## <a name="find-the-user-object-id"></a>Kullanıcı nesne KIMLIĞINI bul

Yalnızca etki alanı adını ve kiracı KIMLIĞINI bulmanın her zaman yeterli olmayabilir. Ayrıca, bir kullanıcıya atanan belirli nesne KIMLIĞINI de bulmanız gerekebilir. Azure portal kullanıcının nesne KIMLIĞINI bulmak için şu adımları izleyin:

1. [Azure Portal](https://portal.azure.com/)’ında oturum açın.

2. menüden **Azure Active Directory** seçin.

3. Menüdeki **Yönet** bölümünü bulun ve ardından **Kullanıcılar**' ı seçin.

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="vurgulanan, kullanıcılar seçeneğiyle birlikte Azure Active Directory menüsünü gösterir.":::

4. Kullanıcılar sayfasında, arama kutusuna kullanıcının adını yazın.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Belirli bir kullanıcıyı aramak için arama kutusuyla birlikte kullanıcılar sayfasını gösterir.":::

5. Listede göründüğü kullanıcının adını seçin.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Aranan Kullanıcı için bir satır görüntüleyen Kullanıcı sayfasını gösterir.":::

6. Kullanıcının profil sayfasında kimlik bölümünü bulun. Nesne KIMLIĞI alanı, kullanıcının benzersiz nesne KIMLIĞIYLE birlikte görüntülenir.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Kimlik bölümü ve nesne KIMLIĞI için vurgulanmış bir alan olan kullanıcı profili sayfasını gösterir.":::

## <a name="next-steps"></a>Sonraki adımlar

- [PowerShell veya CLı ile program aracılığıyla kiracı KIMLIĞINIZI bulun](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [Azure Active Directory 'de Kullanıcı profilleri hakkında daha fazla bilgi edinin](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [İş ortaklarının Iş Ortağı Merkezi 'nde müşteri ayrıntılarını nasıl görebileceğine veya dışa verebileceğine öğrenin](see-your-customer-list.md)

