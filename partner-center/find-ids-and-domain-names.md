---
title: Kiracı kimliğini, etki alanı adını, kullanıcı nesne kimliğini bulma
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Kuruluşun Azure AD kiracı kimliği Azure portal etki alanı adı veya belirli bir kullanıcı nesnesi kimliği gibi kimlikleri nasıl bulamıyorum? Bazı görevler bu bilgilere ihtiyaç gösterir.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: db730436e88118c24aa966c1023ffeeadd20548a
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960544"
---
# <a name="locate-important-ids-for-a-user"></a>Bir kullanıcı için önemli kimlikleri bulma

**Uygun roller:** Genel yönetici

Bu makalede, bir kullanıcıya Azure portal [bilgileri](https://portal.azure.com/) bulmak için Azure portal nasıl kullanabileceğiniz açıklanmıştır:

- Kullanıcının Microsoft Azure Active Directory kuruluşuna veya şirketin kiracı kimliğine (Azure AD) göre

- Azure AD kiracısı ile ilişkili kuruluşun veya şirketin birincil etki alanı adı

- Kullanıcı nesnesi kimliği

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Kiracı kimliğini Microsoft Azure AD birincil etki alanı adını bulma

Azure AD kiracı kimliğini veya etki alanı içindeki birincil etki alanı adını bulmak için bu Azure portal. (Kiracı kimliğini program aracılığıyla bulmak için bkz. [PowerShell](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell)veya CLI ile kiracı kimliğini bulma.)

> [!NOTE]
> Kiracı kimliği, farklı uygulamalarda veya kaynaklarda farklı adlar olarak çağrıl olabilir. Örneğin, kiracı kimliğine dizin kimliği, Azure Active Directory (Azure AD) kiracısı, Microsoft kimliği veya belirli raporlar için, hatta kiracı tarafından yönlendirilen olarak *başvurul olabilir.*

1. [Azure Portal](https://portal.azure.com/)’ında oturum açın.

2. Menüden **Azure Active Directory'yi** seçin.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Menüde Azure portal seçerek Azure Active Directory seçeneğini gösterir.":::

3. Bir Azure Active Directory **Genel Bakış** sayfası görüntülenir. Azure AD kiracı kimliğini veya birincil etki alanı adını bulmak için Kiracı Kimliği **alanını ve** Birincil etki **alanı alanını** bulun. Bu alanlar Kiracı bilgileri bölümünde görünür.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Kiracı kimliği ve birincil etki alanı adı olmak için vurgulanmış iki alanla Genel Bakış sayfasını gösterir.":::

4. Kiracı kimliğini kiracı Azure portal birkaç şekilde bulabilirsiniz. Menüden **Azure Active Directory'yi** seçin. Ardından, menüde **Yönet bölümünü** bulun ve Özellikler'i **seçin.**

   Özellikler sayfasında kullanıcının ilişkili Kiracı Kimliği de görüntülenir.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Vurgulanmış Kiracı Kimliği alanıyla Özellikler sayfasını gösterir.":::

## <a name="find-the-user-object-id"></a>Kullanıcı nesnesi kimliğini bulma

Yalnızca etki alanı adını ve kiracı kimliğini bulmak her zaman yeterli olabilir. Ayrıca, bir kullanıcıya atanan belirli nesne kimliğini de bulmanız gerekir. Kullanıcının nesne kimliğini aşağıdaki adımlarda bulmak için aşağıdaki adımları Azure portal:

1. [Azure Portal](https://portal.azure.com/)’ında oturum açın.

2. Menüden **Azure Active Directory'yi** seçin.

3. Menüde **Yönet bölümünü** bulun ve Kullanıcılar'ı **seçin.**

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Kullanıcılar Azure Active Directory vurgulanmış Bir Menüyü gösterir.":::

4. Kullanıcılar sayfasında, arama kutusuna kullanıcının adını yazın.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Belirli bir kullanıcı için arama yapmak için arama kutusunu gösteren Kullanıcılar sayfasını gösterir.":::

5. Listede göründüğü yerde kullanıcının adını seçin.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Aranan kullanıcı için bir satır görüntüleyen Kullanıcı sayfasını gösterir.":::

6. Kullanıcının Profil sayfasında Kimlik bölümünü bulun. Nesne Kimliği alanı burada kullanıcının benzersiz nesne kimliğiyle görünür.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Kimlik bölümü ve Nesne Kimliği için vurgulanmış bir alan ile Kullanıcı Profili sayfasını gösterir.":::

## <a name="next-steps"></a>Sonraki adımlar

- [PowerShell veya CLI ile program aracılığıyla kiracı kimliğinizi bulma](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [Azure Active Directory'de kullanıcı profilleri hakkında daha fazla bilgi Azure Active Directory](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [İş ortaklarının müşteri ayrıntılarını nasıl göreceğini veya dışarı aktara İş Ortağı Merkezi](see-your-customer-list.md)

