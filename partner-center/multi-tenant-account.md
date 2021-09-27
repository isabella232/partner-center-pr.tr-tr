---
title: İş Ortağı Merkezi hesabınıza kiracı ekleme
ms.topic: article
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: İş Ortağı Merkezi hesabınıza birden çok Azure AD kiracısı ekleme, birleştirme veya yönetme hakkında bilgi edinin ve bunu neden yapmak istemeyebilirsiniz?
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c1e116a6d7aa17cd01a0dfb0342c6f76ad78c448
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129073658"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Hesap hesabınıza birden çok kiracı ekleme ve İş Ortağı Merkezi yönetme


**Uygun roller:** Genel yönetici | Hesap yöneticisi

Bu makalede, birden çok şirket Azure Active Directory (Azure AD) kiracılarını birleştirme ve bunları şirket hesabınıza ekleme ve İş Ortağı Merkezi ele alır. Bunu yapmak için birçok neden vardır. Örnek:

- Contoso adlı bir şirket olan Fabrikam adlı başka bir şirket edindi. İki şirketin ayrı kalmasını, ancak yeni çalışanların şirket içinde İş Ortağı Merkezi. Bu durumda, yeni şirketin Azure AD kiracısı ile İş Ortağı genel hesabınız (PGA) ilişkilendirmeniz gerekir. Bu ilişki, her iki şirkette de kullanıcıların şirket içinde İş Ortağı Merkezi.

- İşletmenizi birden fazla kiracıyla *(örneğin, contoso.com*, *contoso.uk* ve *contoso.in)* çalıştırdısanız, çok kiracılı kiracıyı kullanarak bunları aynı bilgisayar hesabında grupabilirsiniz.

- Birleşme ve satın alma yönergeleri her iki şirketin kiracıları ile çalışmanız gerektirse, hem şirket içinde hem de şirket *constoso.com* *fabrikam.com* gerekir.

- Kiracılardan herhangi bir kullanıcının şunları mümkün olması gerekir:
    * Eğitim İş Ortağı Merkezi, dijital indirmeler veya Microsoft Sertifikalı Professional (MCP) ilişkilendirmesi için erişim bilgileri.
    * Bir İş Ortağı Merkezi (MPN) Microsoft İş Ortağı Ağı teşvik yöneticisi gibi farklı roller atanabilir.

## <a name="add-an-azure-ad-tenant-to-your-account"></a>Hesabınıza Azure AD kiracısı ekleme

1. Genel yönetici olarak [İş Ortağı Merkezi oturum](https://partner.microsoft.com/dashboard) açın.

2. Ayarlar dişli simgesini ve ardından **Hesap ayarları 'ı ve** ardından Kiracılar'ı **seçin.**
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Azure AD Profili bölmesindeki İş ortağı düğmesinin ekran görüntüsü.":::

3. **İşle'yi** seçin ve ilişkilendirmek istediğiniz kiracıyı seçin.

4. İstendiğinde, ilişkilendirmek istediğiniz kiracıda genel yönetici olarak oturum açın ve Onayla'ya **seçin.**

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Yeni Azure AD ilişkilendirmesi onaylayın bölmesindeki Onayla düğmesinin ekran görüntüsü.":::

   İlişkiyi onaylandıktan sonra Tüm **ayarlamalar iletisi** görüntülenir. Yeni eklenen kiracıyı görüntülemek için Kiracı yönetimine **geri dön seçeneğini seçin.**

> [!NOTE]
> Zaten başka bir kiracı hesabıyla ilişkilendirilmişse kiracıyı bir hesapla İş Ortağı Merkezi.

## <a name="remove-a-tenant-from-your-account"></a>Bir kiracıyı hesabınızdan kaldırma

1. Microsoft'ta genel yönetici olarak [oturum İş Ortağı Merkezi.](https://partner.microsoft.com/dashboard)

2. Ayarlar dişli simgesini ve ardından **Hesap ayarları 'ı ve** ardından Kiracılar'ı **seçin.**

3. **İş ortağı** sekmesini seçin.

4. **İlişkilerini** kaldırmak istediğiniz kiracının yanındaki Kaldır'ı seçin.

   :::image type="content" source="images/disassociate.png" alt-text="Geçerli kiracı ilişkilendirmelerinin ve bunların Kaldır bağlantılarının ekran görüntüsü.":::

   Önceki ekran görüntüsünde gösterildiği  gibi, Birincil kiracı ve o anda oturum asanız kiracı dışında tüm ilişkili kiracılar için Kaldır bağlantıları etkinleştirilir.

   > [!NOTE]
   > Bir kiracıyı kaldırsanız, kiracı üzerindeki kullanıcılar artık İş Ortağı Merkezi erişimine sahip olmaz ve kaldırma işlemi yetkinliklerinizi etkileyene sahip olabilir.

## <a name="next-steps"></a>Sonraki adımlar

- [Kullanıcı hesapları oluşturma](create-user-accounts-and-set-permissions.md)
