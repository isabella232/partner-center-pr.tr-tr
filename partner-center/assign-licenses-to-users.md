---
title: Kullanıcıları müşteri hesaplarına göre yönetme
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Iş Ortağı Merkezi 'nde müşterileriniz için kullanıcıları yönetme-Kullanıcı hesapları oluşturma, kullanıcı lisansları ekleme veya kaldırma, parolaları sıfırlama ve Kullanıcı hesaplarını silme veya geri yükleme.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1c346e5e680fdd0b0b82715160b238e1e6b6a9a9
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248356"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a>Müşteri hesapları için kullanıcıları ve kullanıcı lisanslarını yönetme 

**Uygun roller**: genel yönetici | Kullanıcı Yönetimi Yöneticisi | Yönetim Aracısı


Müşterinin hesabındaki yeni kullanıcıları oluşturabilir ve silebilirsiniz. Ayrıca, silmenin 30 gün içinde daha önce sildiğiniz bir veya daha fazla kullanıcı hesabını geri yükleyebilirsiniz. Kullanıcının önceki abonelik atamaları da geri yüklenecektir (önceki ayırmaların kullanılabildiği varsayılarak).

Bir müşteri için yeni abonelikler satın aldığınızda, müşteri size hesap, Kullanıcı izinleri ve her kullanıcının ihtiyacı olan hizmetlere sahip olan tüm kullanıcıların bir listesini vermelidir.  

>[!NOTE]
>**Müşteri** sekmesinin **Kullanıcılar ve lisanslar** bölümü, belirli bir müşterinin kiracısında oluşturulan, başka bir CSP ortağından veya başka bir satın alma kanalından satın alınmış lisanslardan oluşan kullanıcılar dahil olmak üzere tüm kullanıcıları gösterir.

[Excel uyumlu bir .csv elektronik tablo dosyası](adding-multiple-users-to-a-customer-account.md)kullanarak adları içeri aktararak aynı anda [birden fazla kullanıcıya abonelik atayabilirsiniz](bulk-license-provisioning-for-multiple-users.md) .

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>Müşteri için kullanıcı hesapları oluşturma

1. Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.

2. Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve listeden bir müşteri seçin.

3. Müşteri menüsünde, **Kullanıcılar ve lisanslar**' ı seçin.

4. Eklediğiniz her kullanıcı için **Abonelik Ekle**' yi seçin ve ardından izinler ve lisanslar dahil olmak üzere bilgileri doldurun. Değişikliklerinizi **kaydedin** .

5. Kullanıcıya göndermek için Kullanıcı adını ve geçici parolayı kaydettiğinizden emin olun.

6. Birden çok kullanıcıyı aynı anda ekliyorsanız, **başka bir Kullanıcı Ekle** öğesini kullanın.

7. ayrıca, [Excel uyumlu bir .csv elektronik tablo dosyasını içeri aktararak](adding-multiple-users-to-a-customer-account.md)aynı anda birden fazla kullanıcı ekleyebilirsiniz. Onay ekranından adları ve parolaları göndermeden veya yazdırmadan önce tüm küme ile işiniz tamamlanana kadar bekleyebilirsiniz.

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>Müşteri için kullanıcı lisanslarını ekleme veya kaldırma

Aşağıdaki adımlar, Microsoft ürünlerine yönelik kullanıcı lisanslarını eklemek veya kaldırmak için geçerlidir. Ticari Market 'teki lisans tabanlı SaaS aboneliklerine yönelik kullanıcı lisanslarını eklemek veya kaldırmak için bkz. [SaaS aboneliği için lisans ekleme veya kaldırma](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).

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