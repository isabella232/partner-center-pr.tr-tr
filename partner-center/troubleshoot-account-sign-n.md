---
title: İş Ortağı Merkezi veya MPN yenileme sorunlarınızı giderme
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: İş Ortağı Merkezi'a kaydolmaya çalışırken ortaya İş Ortağı Merkezi. Ödeme yöntemleriyle ilgili zorlukları, parolaları unutmayı ve daha fazlasını yanıtlar.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a5e8a292ad8593dc0b94179d5f0ee418344ef9af
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854698"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Hesap kurulumu veya MPN yenileme sorunlarını giderme

**Uygun roller:** Genel yönetici | MPN iş ortağı yöneticisi
 
Burada, İş Ortağı Merkezi hesabınız ayarlarken ortaya çıkan yaygın sorunları gidermeye yönelik İş Ortağı Merkezi vardır.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Şirket dışından Partner Membership Center şirket bilgileri alanlarını düzenleyemeyebilirsiniz

Şirket içinde zaten bir İş Ortağı Merkezi (csP hesabı gibi) olduğu durumlarda, salt okunur bir ekran gösterilir. Bu ekranda, şirketle ilgili tüm bilgiler şirket içinde mevcut İş Ortağı Merkezi.

Bu ekranda ayrıntıları değiştiremezsiniz. Bu bir hata değil, tasarıma göredir.

Devam etmek **için Kabul** Et ve **Devam Et'i** seçin.


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>IT departmanı Kayıt için **kaydolmayı İş Ortağı Merkezi**

Bu iletiyi, virüslü kullanıcılar devre dışı bırakıldıklarında veya Azure AD kiracısı üzerinde Viral Kayıt devre dışı bırakıldıklarında görüyorsunuz. Azure AD hesabınıza yönelik Genel yönetici, aşağıdaki PowerShell komutunu çalıştırarak gerekli özellikleri etkinleştirebilirsiniz:

**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**

Daha fazla bilgi için [self servis kaydolma makalelerini okuyun.](/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>Parolanızı unuttunız

Parolanızı unuttuysanız oturum açma **sayfasındaki Hesabınıza erişe miyim?** bağlantısını seçin. Bu seçenek parolanızı sıfırlamanıza veya Genel yöneticinizden size yeni kimlik bilgileri atamasını istemenize olanak sağlar.

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
