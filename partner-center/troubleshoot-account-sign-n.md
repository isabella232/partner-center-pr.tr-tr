---
title: Iş Ortağı Merkezi hesabınızı veya MPN yenileme sorunlarını ayarlamayla ilgili sorunları giderin
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Iş Ortağı Merkezi 'ne kaydolmaya çalışırken sorun giderin. Ödeme yöntemleriyle ilgili adres sorunlarını yanıtlar, parolaları öğrenme ve daha fazlasını yapın.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9622f02039360e8ab39f459c9a2fe082ec70c854
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756747"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Hesap kurulumu veya MPN yenileme sorunlarını giderme


**Uygun roller**

- Genel yönetici
- MPN iş ortağı Yöneticisi 
 
Iş Ortağı Merkezi hesabınızı ayarlarken ortaya çıkan yaygın sorunları gidermeye yönelik bazı öneriler aşağıda verilmiştir.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Iş ortağı üyelik merkezinden geçiş yapıyorsanız ve herhangi bir şirket bilgisi alanını düzenleyemezsiniz ne olur?

Şirketinizin zaten Iş Ortağı Merkezi 'nde (CSP hesabı söyleyin) mevcut olduğu durumlarda, salt okunurdur bir ekran gösterilir. Bu ekranda, Iş Ortağı Merkezi 'nde olduğu gibi şirketiniz hakkındaki tüm bilgiler görüntülenir.

Bu ekrandaki ayrıntıları değiştiremezsiniz. Bu, tasarım ve bir hata değildir.

**Kabul et** ' i seçin ve devam **edin** .


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>BT departmanı **Iş Ortağı Merkezi 'ne kaydolma** özelliğini devre dışı bıraktı.

Bu iletiyi, viral kullanıcıları devre dışı bırakıldığı veya Azure AD kiracısında viral kaydolma devre dışı bırakıldığı için görürsünüz. Azure AD hesabınız için genel yönetici, aşağıdaki PowerShell komutunu çalıştırarak gerekli özellikleri etkinleştirebilir:

**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-Allowadhocabonelikleri $true**

Daha fazla bilgi için, [self servis kaydolma](/azure/active-directory/users-groups-roles/directory-self-service-signup) makalesini okuyun

## <a name="you-forgot-your-password"></a>Parolanızı unuttum

Parolanızı unuttuysanız, oturum açma sayfasında **hesabınıza erişemiyor musunuz?** bağlantısına tıklayın. Bu seçenek, parolanızı sıfırlamanızı veya genel yöneticinizden size yeni kimlik bilgileri atamasını ister.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>"Şirketiniz hakkında bize söyleyin" ekranında, "bir sorun oluştu" hatası alıyorsunuz

Bu hata iletisi genellikle şirket telefon numaranız için yanlışlıkla özel karakter, boşluk veya ülke kodu kullanıyorsanız görüntülenir. Telefon numarası alanına girilen değer yalnızca en fazla 10 karakter içerebilir.


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>Kredi kartı satın alma işlemi, "Siparişiniz reddedildi" iletisini bildiren bir hata mesajı alıyor. Lütfen bilgilerinizi doğrulayın "


Her zaman yasal varlığınızdan değil kredi kartınıza karşılık gelen adresi kullanın. Ayrıca, ZIP kodunun doğru olduğundan ve kullandığınız adrese karşılık geldiğinden emin olun.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Çevrimdışı ödeme 'den çevrimiçi ödeme yöntemine geçmek istiyorsunuz 

Tercih edilen ödeme yöntemini kullanarak orijinal siparişi ve işlem yeniden Al işlemlerini iptal etmeniz gerekir.

Bir siparişi iptal etmek için:

1. Panoda **Üyelik teklifleri** sekmesini seçin.

2. **Siparişi Iptal et** ' i seçin

3. Bir onay penceresi görünür ve ilk siparişi iptal etmek için onaylamanız gerekir.

## <a name="next-steps"></a>Sonraki adımlar

- [İş Ortağı Merkezi hesabınızı yönetme](partner-center-account-setup.md)
- [Faturanızı ve keşfi dosyanızı okuma](read-your-bill.md)
