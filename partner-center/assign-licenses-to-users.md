---
title: Müşteri hesapları için kullanıcıları yönetme
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: İş Ortağı Merkezi'da müşterileriniz için kullanıcıları yönetme- kullanıcı hesapları oluşturun, kullanıcı lisansları ekleyin veya kaldırın, parolaları sıfırlayın ve kullanıcı hesaplarını silin veya geri yükleme.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc896ec3ce16ab0f05a8131de14f573ad96a8141
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149902"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a>Müşteri hesapları için kullanıcıları ve kullanıcı lisanslarını yönetme 

**Uygun roller:** Genel yönetici | Kullanıcı yönetimi yönetici | Yönetici aracısı


Müşterinin hesabında yeni kullanıcılar oluşturabilir ve silebilirsiniz. Daha önce sildikten sonra 30 gün içinde silmiş olduğunu bir veya daha fazla kullanıcı hesabını da geri yükleyebilirsiniz. Kullanıcının önceki abonelik atamaları da geri yüklenir (önceki ayırmalarının kullanılabilir olduğu varsayıldı).

Bir müşteri için yeni abonelikler satın alırsanız, müşteri size hesap, kullanıcı izinleri ve her kullanıcının hangi hizmetlere ihtiyacı olacak olan tüm kullanıcıların listesini versin.  

>[!NOTE]
>Müşteri **sekmesinin Kullanıcılar**  ve lisanslar bölümünde, başka bir CSP iş ortağından veya başka bir satın alma kanalından satın alınan lisanslara sahip kullanıcılar da dahil olmak üzere belirli bir müşterinin kiracısı içinde oluşturulan tüm kullanıcılar görüntülenir.

Excel ile [uyumlu bir](bulk-license-provisioning-for-multiple-users.md) .csv elektronik tablo dosyası kullanarak adları içeri aktararak birden çok kullanıcıya [abonelik atabilirsiniz.](adding-multiple-users-to-a-customer-account.md)

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>Müşteri için kullanıcı hesapları oluşturma

1. İş Ortağı Merkezi [oturum açın.](https://partner.microsoft.com/dashboard)

2. Yeni İş Ortağı Merkezi **Müşteriler'i** ve ardından listeden bir müşteri seçin.

3. Müşteri menüsünde Kullanıcılar ve **lisanslar'ı seçin.**

4. Ekleyilen her kullanıcı için Abonelik **ekle'yi** seçin ve ardından izinler ve lisanslar dahil olmak üzere bilgileri doldurun. **Değişikliklerinizi** kaydedin.

5. Kullanıcıya göndermek için kullanıcı adını ve geçici parolayı kaydetmeyi emin olun.

6. Bir defada birden çok kullanıcı ekliyorsanız Başka bir kullanıcı **ekle'yi kullanın.**

7. Excel ile uyumlu bir .csv elektronik tablo [dosyasını içeri aktararak aynı anda birden çok kullanıcı abilirsiniz.](adding-multiple-users-to-a-customer-account.md) Onay ekranından adları ve parolaları e-posta ile göndermeden veya yazdırmadan önce tüm kümeyi tamamlaya kadar bekleyebilirsiniz.

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>Müşteri için kullanıcı lisanslarını ekleme veya kaldırma

Aşağıdaki adımlar, Microsoft ürünleri için kullanıcı lisansları eklemek veya kaldırmak için geçerlidir. Ticari Market 'teki lisans tabanlı SaaS aboneliklerine yönelik kullanıcı lisanslarını eklemek veya kaldırmak için bkz. [SaaS aboneliği için lisans ekleme veya kaldırma](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).

1. Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.

2. Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve listeden bir müşteri seçin.

3. Müşteri menüsünde, **Kullanıcılar ve lisanslar**' ı seçin.

4. Listeden bir veya birden fazla kullanıcı seçin. Örneğin, müşteri yeni lisanslar satın almış ve bunları henüz sahip olmayan kişilere atamak istediğinizde, doğru grubu bulmak için **kullanıcıları filtreleme...** seçeneğini kullanabilirsiniz.

5. **Lisansları Yönet**’i seçin. Değişikliklerinizi yapın ve **kaydedin**.

> [!NOTE]
> [Azure Market ürünleri](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)için lisans atama ve etkinleştirme, ürünü yayımlayan bağımsız yazılım SATıCıSı (ISV) üzerinden yönetilir.

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a>Kullanıcının bir müşterinin parolasını sıfırlama

1. İş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard) oturum açın.

2. Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve listeden bir müşteri seçin.

3. Müşteri menüsünde, **Kullanıcılar ve lisanslar**' ı seçin. Listeden kullanıcıyı seçin.

4. Ekranın alt kısmındaki **Parolayı Sıfırla**' yı seçin. 

5. Yeni geçici parolayı kullanıcıya gönderin.

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a>Müşterinin Kullanıcı hesaplarını silme

1. **Iş Ortağı Merkezi** menüsünde **müşteriler**' i seçin. Listeden müşteriyi seçin.

2. Müşteri menüsünde, **Kullanıcılar ve lisanslar**' ı seçin. Listeden kullanıcıyı seçin.

3. Ekranın alt kısmındaki **Kullanıcı hesabını Sil**' i seçin.

Bu hesabı geri yüklemeniz gerekiyorsa, müşterinin **Kullanıcılar ve lisanslar** listesinin **silinen kullanıcılar** sekmesinde bulabilirsiniz. Silinen bir kullanıcıyı geri yüklemek için 30 gününüz vardır.

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a>Silinen kullanıcı hesaplarını geri yükleme

1. **Iş Ortağı Merkezi** menüsünde **müşteriler**' i seçin ve ardından listeden müşteriyi seçin.

2. **Kullanıcılar ve lisanslar ' ı** seçin.

3. **Silinen kullanıcılar ()** sekmesini seçin. Geri yüklenebilecek silinen kullanıcılar varsa, **(1)** veya daha büyük bir bilgi almalıdır.

4. Silinen kullanıcıların onay kutularından bir veya daha fazlasını seçin ve ardından **geri yükle**' yi seçin.

    Tüm seçili kullanıcı hesapları, **Kullanıcılar ve lisanslar** sayfasında yeniden görüntülenir.

## <a name="next-steps"></a>Sonraki adımlar

- [Birden fazla kullanıcıya lisans atama veya atanmış lisansları iptal etme](bulk-license-provisioning-for-multiple-users.md)

- [Müşteri hesabı için birden çok Kullanıcı oluşturma](adding-multiple-users-to-a-customer-account.md)