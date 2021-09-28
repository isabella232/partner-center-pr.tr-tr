---
title: Iş Ortağı Merkezi hesabınızı veya MPN yenileme sorunlarını ayarlamayla ilgili sorunları giderin
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
description: Iş Ortağı Merkezi 'ne kaydolmaya çalışırken sorun giderin. Ödeme yöntemleriyle ilgili adres sorunlarını yanıtlar, parolaları öğrenme ve daha fazlasını yapın.
author: ParthP
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d57cec763db2c22b08ec7cc5ae1b6f39c697811f
ms.sourcegitcommit: e1da62b36420d78bf44e3962358d0af65ebc3402
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129088527"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Hesap kurulumu veya MPN yenileme sorunlarını giderme

**Uygun roller**: genel yönetici | MPN iş ortağı Yöneticisi

Iş Ortağı Merkezi hesabınızı ayarlarken ortaya çıkan yaygın sorunları gidermeye yönelik bazı öneriler aşağıda verilmiştir.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Iş ortağı üyelik merkezinden geçiş yapıyorsanız ve herhangi bir şirket bilgisi alanını düzenleyemezsiniz ne olur?

şirketinizin zaten iş ortağı merkezi 'nde (örneğin, bir Bulut Çözümü Sağlayıcısı (CSP) bir hesabı) sahip olduğu durumlarda, salt okunurdur bir ekran gösterilir. Bu ekranda, Iş Ortağı Merkezi 'nde olduğu gibi şirketiniz hakkındaki tüm bilgiler görüntülenir.

Bu ekrandaki ayrıntıları değiştiremezsiniz. Bu, tasarım ve bir hata değildir.

Devam etmek için **kabul et**' i ve sonra **devam**' ı seçin.

### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>BT departmanı **Iş Ortağı Merkezi 'Ne kaydolma** işlemi kapalıysa

bu iletiyi, viral kullanıcıları devre dışı bırakıldığı veya Azure Active Directory (AD) kiracısında viral kaydolma devre dışı bırakıldığı için görürsünüz. Azure AD hesabınız için genel yönetici, aşağıdaki PowerShell komutunu çalıştırarak gerekli özellikleri etkinleştirebilir:

**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-Allowadhocabonelikleri $true**

Daha fazla bilgi için [self servis kaydolun](/azure/active-directory/users-groups-roles/directory-self-service-signup)makalesini okuyun.

## <a name="you-forgot-your-password"></a>Parolanızı unuttum

Parolanızı unuttuysanız, oturum açma sayfasında **hesabınıza erişemiyor musunuz?** seçeneğini belirleyin. Bu seçenek, parolanızı sıfırlamanızı veya genel yöneticinizden size yeni kimlik bilgileri atamasını ister.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>"Şirketiniz hakkında bize söyleyin" ekranında, "bir sorun oluştu" hatası alıyorsunuz

Bu hata iletisi genellikle şirket telefon numaranız için yanlışlıkla özel karakter, boşluk veya ülke kodu kullanıyorsanız görüntülenir. Telefon Number alanına girilen değer yalnızca en fazla 10 karakter içerebilir.

### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>Kredi kartı satın alma işlemi, "Siparişiniz reddedildi" iletisini bildiren bir hata mesajı alıyor. Lütfen bilgilerinizi doğrulayın "

Her zaman yasal varlığınızdan değil kredi kartınıza karşılık gelen adresi kullanın. Ayrıca, ZIP kodunun doğru olduğundan ve kullandığınız adrese karşılık geldiğinden emin olun.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Çevrimdışı ödeme 'den çevrimiçi ödeme yöntemine geçmek istiyorsunuz

Tercih edilen ödeme yöntemini kullanarak orijinal siparişi ve işlem yeniden Al işlemlerini iptal etmeniz gerekir.

Bir siparişi iptal etmek için:

> [!NOTE]
> Çalışma alanları arabirimi hakkında daha fazla bilgi edinmek için bkz. [Iş ortağı merkezini alma](get-around-partner-center.md#turn-workspaces-on-and-off).

#### <a name="workspaces-view"></a>[Çalışma alanları görünümü](#tab/workspaces-view)

1. [Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard) **Üyelik** kutucuğunu seçin.

2. **Üyelik tekliflerini** seçin ve **siparişi iptal edin**.

3. Bir onay penceresi görünür ve ilk siparişi iptal etmek için onaylamanız gerekir.

#### <a name="current-view"></a>[Geçerli görünüm](#tab/current-view)

1. [Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard) **Üyelik teklifleri** sekmesini seçin.

2. **Siparişi Iptal et**' i seçin.

3. Bir onay penceresi görünür ve ilk siparişi iptal etmek için onaylamanız gerekir.

* * *

## <a name="next-steps"></a>Sonraki adımlar

- [İş Ortağı Merkezi hesabınızı yönetme](partner-center-account-setup.md)
- [Faturanızı ve keşfi dosyanızı okuma](read-your-bill.md)
