---
title: İş Ortağı Merkezi veya MPN yenileme sorunlarınızı giderme
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: İş Ortağı Merkezi'a kaydolmaya çalışırken ortaya İş Ortağı Merkezi. Ödeme yöntemleri, parolaları unutma ve daha fazlası ile ilgili zorlukların yanıtlarını verir.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4fc1a43b4d525d9221ac7e4db56f5f278404e3f5
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431762"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Hesap kurulumu veya MPN yenileme sorunlarını giderme

**Uygun roller:** Genel yönetici | MPN iş ortağı yöneticisi
 
Burada, İş Ortağı Merkezi hesabınız ayarlarken ortaya çıkan yaygın sorunları gidermek için İş Ortağı Merkezi edinebilirsiniz.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Şirket dışından Partner Membership Center şirket bilgileri alanlarını düzenleyemeyebilirsiniz

Şirket içinde zaten bir İş Ortağı Merkezi (Bulut Çözümü Sağlayıcısı (CSP) hesabı) olduğu durumlarda, salt okunur bir ekran gösterilir. Bu ekranda, şirketle ilgili tüm bilgiler şirket içinde mevcut İş Ortağı Merkezi.

Bu ekranda ayrıntıları değiştiremezsiniz. Bu bir hata değil, tasarıma göredir.

Devam etmek için Kabul **Et'i** ve ardından Devam'ı **seçin.**


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>IT departmanı Kayıt için **kaydolmayı İş Ortağı Merkezi**

Bu iletiyi, virüslü kullanıcılar devre dışı bırakıldıklarında veya Virüslü Kayıt Azure Active Directory (AD) kiracıda devre dışı bırakılmıştır. Azure AD hesabınıza yönelik Genel yönetici, aşağıdaki PowerShell komutunu çalıştırarak gerekli özellikleri etkinleştirebilirsiniz:

**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**

Daha fazla bilgi için [self servis kaydolma makalelerini okuyun.](/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>Parolanızı unuttunız

Parolanızı unuttuysanız oturum açma sayfasında Hesabınıza erişe **miyim? öğesini seçin.** Bu seçenek parolanızı sıfırlamanıza veya Genel yöneticinizden size yeni kimlik bilgileri atamasını istemenize olanak sağlar.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>"Bize şirketinizi söyleyin" ekranında "Bir sorun oluştu" hatasını alısınız

Bu hata iletisi genellikle şirket telefon numaranıza yanlışlıkla özel karakterler, boşluklar veya ülke kodu kullanıyorsanız ortaya çıktı. Telefon Numarası alanına girilen değer yalnızca en fazla 10 karakter içerebilir.


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>Kredi kartı satın alma sırasında "Siparişiniz reddedildi. Lütfen bilginizi doğrulayın"


Yasal varlığınız yerine her zaman kredi kartınıza karşılık gelen adresi kullanın. Ayrıca posta kodunun doğru olduğundan ve kullanmakta olduğunuz adrese karşılık gelen bir adres olduğundan emin olun.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Çevrimdışı ödemeden çevrimiçi ödeme yöntemine geçmek istiyorsanız 

Özgün siparişi iptal etmeniz ve tercih edilen ödeme yöntemini kullanarak yeniden satın alasanız gerekir.

Siparişi iptal etmek için:

1. Yeni İş Ortağı Merkezi Üyelik Teklifleri **sekmesini** seçin.

2. Siparişi **iptal et'i seçin**

3. Bir onay penceresi görüntülenir ve ilk siparişi iptal etmek için onaylamanız gerekir.

## <a name="next-steps"></a>Sonraki adımlar

- [İş Ortağı Merkezi hesabınızı yönetme](partner-center-account-setup.md)
- [Faturanızı ve mutabakat dosyanızı okuma](read-your-bill.md)
