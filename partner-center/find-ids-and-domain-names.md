---
title: Kiracı kimliğini, etki alanı adını, kullanıcı nesne kimliğini bulma
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Bir kuruluşun Azure AD kiracı kimliği Azure portal etki alanı adı veya belirli kullanıcı nesnesi kimliği gibi kimlikleri nasıl bulamıyorum? Bazı görevler bu bilgilere ihtiyaç gösterir.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 643b1eeb96a47ee4c438f733efe3be22234d02ff
ms.sourcegitcommit: e462f562e7f26b7d6870c22638a2a841499109d6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/11/2021
ms.locfileid: "109740293"
---
# <a name="locate-important-ids-for-a-user"></a>Bir kullanıcı için önemli kimlikleri bulma

**Uygun roller**

- Genel yönetici

Bu makalede, bir kullanıcıya Azure portal [bilgileri](https://portal.azure.com/) bulmak için Azure portal nasıl kullanabileceğiniz açıklanmıştır:

- Kullanıcının Microsoft Azure Active Directory kuruluşuna veya şirketin kiracı kimliğine (Azure AD) göre

- Azure AD kiracısı ile ilişkili kuruluşun veya şirketin birincil etki alanı adı

- Kullanıcı nesnesi kimliği

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Kiracı kimliğini Microsoft Azure AD birincil etki alanı adını bulma

Azure AD kiracı kimliğini veya etki alanı içindeki birincil etki alanı adını bulmak için bu Azure portal. (Kiracı kimliğini program aracılığıyla bulmak için bkz. [PowerShell](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell)veya CLI ile kiracı kimliğini bulma.)

> [!NOTE]
> Kiracı kimliği, farklı uygulamalarda veya kaynaklarda farklı adlar olarak çağrıl olabilir. Örneğin, kiracı kimliğine dizin kimliği, Azure Active Directory (Azure AD) kiracısı, Microsoft kimliği veya belirli raporlar için, hatta kiracı tarafından yönlendirilen olarak *başvurul olabilir.*

1. [Azure portalında](https://portal.azure.com/) oturum açın.

2. Menüden **Azure Active Directory'yi** seçin.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Menüden Azure portal seçerek Azure Active Directory seçeneğini gösterir.":::

3. Bir Azure Active Directory **Genel Bakış** sayfası görüntülenir. Azure AD kiracı kimliğini veya birincil etki alanı adını bulmak için Kiracı Kimliği **alanını ve** Birincil etki **alanı alanını** bulun. Bu alanlar Kiracı bilgileri bölümünde görünür.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Kiracı kimliği ve birincil etki alanı adı olmak için vurgulanmış iki alanla Genel Bakış sayfasını gösterir.":::

4. Kiracı KIMLIĞINI Azure portal birkaç farklı yolla bulabilirsiniz. Menüden **Azure Active Directory** seçin. Ardından, menüdeki **Yönet** bölümünü bulun ve **Özellikler**' i seçin.

   Özellikler sayfası kullanıcının ilişkili kiracı KIMLIĞINI de görüntüler.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Vurgulanan kiracı KIMLIĞI alanıyla birlikte Özellikler sayfasını gösterir.":::

## <a name="find-the-user-object-id"></a>Kullanıcı nesne KIMLIĞINI bul

Yalnızca etki alanı adını ve kiracı KIMLIĞINI bulmanın her zaman yeterli olmayabilir. Ayrıca, bir kullanıcıya atanan belirli nesne KIMLIĞINI de bulmanız gerekebilir. Azure portal kullanıcının nesne KIMLIĞINI bulmak için şu adımları izleyin:

1. [Azure portalında](https://portal.azure.com/) oturum açın.

2. Menüden **Azure Active Directory** seçin.

3. Menüdeki **Yönet** bölümünü bulun ve ardından **Kullanıcılar**' ı seçin.

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Vurgulanan, kullanıcılar seçeneğiyle birlikte Azure Active Directory menüsünü gösterir.":::

4. Kullanıcılar sayfasında, arama kutusuna kullanıcının adını yazın.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Belirli bir kullanıcıyı aramak için arama kutusuyla birlikte kullanıcılar sayfasını gösterir.":::

5. Listede göründüğü kullanıcının adını seçin.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Aranan Kullanıcı için bir satır görüntüleyen Kullanıcı sayfasını gösterir.":::

6. Kullanıcının profil sayfasında kimlik bölümünü bulun. Nesne KIMLIĞI alanı, kullanıcının benzersiz nesne KIMLIĞIYLE birlikte görüntülenir.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Kimlik bölümü ve nesne KIMLIĞI için vurgulanmış bir alan olan kullanıcı profili sayfasını gösterir.":::

## <a name="next-steps"></a>Sonraki adımlar

- [PowerShell veya CLı ile program aracılığıyla kiracı KIMLIĞINIZI bulun](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [Azure Active Directory'de kullanıcı profilleri hakkında daha fazla bilgi Azure Active Directory](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [İş ortaklarının müşteri ayrıntılarını nasıl göreceğini veya dışarı aktara İş Ortağı Merkezi](see-your-customer-list.md)

