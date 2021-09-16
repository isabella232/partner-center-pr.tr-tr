---
title: Müşterinizin CSP programına yapılan Microsoft Müşteri Sözleşmesi onaylayın
description: Bulut Çözümü Sağlayıcısı (CSP) iş ortaklarının, müşteriler için sipariş Microsoft Müşteri Sözleşmesi önce müşterinin Microsoft hizmetleri onaylaması gerekir.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: 205de1c852d263e79978358229f1365852872232
ms.sourcegitcommit: 986573bc4382b803bf4d641df6dd1e37c3af1955
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/16/2021
ms.locfileid: "127872314"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a>Müşterinizin CSP programına yapılan Microsoft Müşteri Sözleşmesi onaylayın

**Uygun roller:** Yönetici aracısı | Satış aracısı


Müşterilerin, müşteri kabul etme seçenekleri iki Microsoft Müşteri Sözleşmesi.

**1.** Seçenek: İş ortağı müşteri kabulü için iş ortağı, API/SDK'İş Ortağı Merkezi veya İş Ortağı Merkezi onaylayabilir.

**2.** Seçenek: Müşteri doğrudan kabulü - İş ortağı, Müşteri Merkezi'nde anlaşmayı gözden geçirmek ve kabul etmek için bir URL Microsoft 365 Yönetici davet eder.

## <a name="access-microsoft-customer-agreement-template"></a>Erişim Microsoft Müşteri Sözleşmesi şablonu

uygulamanın en [son sürümünü el ile Microsoft Müşteri Sözleşmesi.](https://aka.ms/customeragreement) Bu Microsoft Müşteri Sözleşmesi ülkeye özgü bir veridir. Uygulama şablonu Microsoft Müşteri Sözleşmesi, müşterinin konumunu temel alarak doğru ülkeyi seçmeyi emin olun.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>1. Seçenek: Müşteri kabulünü İş Ortağı Merkezi

Doğrudan fatura iş ortakları yeni ve mevcut müşteriler için Microsoft Müşteri Sözleşmesi İş Ortağı Merkezi kabul etmelerini onaylayabilir. Dolaylı kurumsal bayiler, müşterileri adına doğrulayamaz ve dolaylı sağlayıcılarla birlikte çalışarak doğrulantıyı tamamlamış olması gerekir.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Yeni müşteriler için müşteri kabulünü onaylama

İş Ortağı Merkezi'de yeni bir müşteri kiracısı oluşturduklarında, müşterinin kiracıyı kabul etme onay Microsoft Müşteri Sözleşmesi. Bu adımları gerçekleştirmek için Yönetici aracısı veya Satış aracısı olmak gerekir.

1. **Müşteriler'i** ve ardından Yeni **müşteri'yi seçin.**

2. Hesap **bilgileri'nin** altında, şirket ve birincil ilgili kişisi için bilgileri girin.

3. **Microsoft sözleşmesi'nin** altında, müşterinin müşteri tarafından kabul edilmeyi kabul etmiş olduğunu Microsoft Müşteri Sözleşmesi.

4. Sözleşme **kabul tarihi'nin** altında uygun tarihi girin. Bunu gelecekteki bir tarihe ayaramazsiniz.

5. Birincil kullanıcı iletişim bilgisinin doğru görüntülendiğinden emin olun. Yanlışsa Güncelleştir'i **seçin** ve sözleşmeyi kabul eden kişi için doğru bilgileri girin.

6. Müşteri **kiracısı** oluşturmaya devam etmek için Sonraki'yi seçin.

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Yeni müşteri.":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Mevcut müşteriler için müşteri kabulünü onaylama

Bunu yapmak için Yönetici aracısı veya Satış aracısı olmak gerekir:

1. **Müşteriler**’i seçin. Müşteriyi bulun ve seçin.

2. Hesap **bilgileri'ne tıklayın.**

3. Öğesinin **Microsoft Müşteri Sözleşmesi** Güncelleştir'i **seçin.**

4. Sözleşmeyi **kabul eden** kişinin **Ad,** Soyadı, **E Telefon** ve kimlik numarasını (isteğe bağlı) girin.  Sözleşme **kabul tarihi'nin** altında uygun tarihi girin. Bunu gelecekteki bir tarihe ayaramazsiniz.

5. Kaydet **ve devam'ı** seçin.

   :::image type="content" source="images/mcua2-update2.png" alt-text="Mevcut müşteri.":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Müşteri kabulü onay alma

Mevcut bir müşterinin mevcut müşteri tarafından kabul edile Microsoft Müşteri Sözleşmesi için aşağıdaki adımları kullanın. Bunu yapmak için Yönetici aracısı veya Satış aracısı olmak gerekir.

1. **Müşteriler'i** seçin ve ardından görmek istediğiniz müşteriyi bulun ve seçin.

2. Hesap **bilgileri'ne tıklayın.**

3. **Microsoft müşteri sözleşmesi altında,** bu müşteri tarafından onay sağlandı veya sağlandı mı?

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>API/SDK kullanarak İş Ortağı Merkezi onaylayın

Api/SDK İş Ortağı Merkezi müşteri kabulünü onaylamak için api/SDK Microsoft Müşteri Sözleşmesi. API/SDK hakkında ayrıntılı bilgi için bkz:

- [Microsoft Müşteri Sözleşmesi için anlaşma meta verilerini alma](/partner-center/develop/get-customer-agreement-metadata)

- [Microsoft Müşteri Sözleşmesinin müşteri kabulünü onaylama](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Microsoft Müşteri Sözleşmesinin müşteri kabulünün onayını alma](/partner-center/develop/get-confirmation-of-customer-agreement)

- [Microsoft Müşteri Sözleşmesi şablonu için indirme bağlantısı oluşturma](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>2. Seçenek: Microsoft 365 Yönetici Center'da müşteri kabulü

İş ortakları, Microsoft 365 Yönetici Center'da anlaşmayı gözden geçirmek ve kabul etmek için URL aracılığıyla yeni ve mevcut müşterileri Microsoft 365 Yönetici davet eder. Sonraki birkaç bölümde şunların nasıl olduğu gösterildi:

- Yeni bir müşteri oluşturun ve müşteriyi sözleşmeyi gözden geçirmesi ve kabul etmeye davet etme.

- Kurumsal bayi ilişkisini ve anlaşmasını gözden geçirmek ve kabul etmek için yeni bir müşteri davet edin.

- Mevcut bir müşteriyi sözleşmeyi gözden geçirmesi ve kabul etmeleri için davet etme.

>[!NOTE]
> Bir müşterinin İş Ortağı Merkezi kabul durumunu almak için [API/SDK'yı](/partner-center/develop/get-direct-sign-status-of-customer-agreement) Microsoft Müşteri Sözleşmesi.  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Yeni bir müşteri oluşturun ve müşteriyi sözleşmeyi gözden geçirmesi ve kabul etmeye davet etme

İş Ortağı Merkezi Center'da yeni bir müşteri oluşturmak ve Microsoft Müşteri Sözleşmesi kabul etmek üzere davet etmek için aşağıdaki Microsoft 365 Yönetici kullanın.

1. İş Ortağı Merkezi'nin Müşteriler sekmesinde Müşteri **ekle'yi seçin.** 

2. Hesap **Bilgileri'nin** altına, yeni müşteriyle ilgili bilgileri müşterinin şirket adı ve birincil ilgili kişisi dahil olmak üzere tüm gerekli alanlara girin.

3. Müşteri **Sözleşmesi'nin** altında **Müşteri'nin Merkezi'nde Microsoft Müşteri Sözleşmesi kabul Microsoft 365 Yönetici istenecek.** Sayfada gerekli diğer tüm alanları doldurun.

4. Sonraki: **Gözden geçir'i** seçin ve ardından müşteri kiracısı oluşturma adımlarına devam edin. 

>[!NOTE] 
>Yeni müşteriler, satın alma teklifini kabul edene kadar Microsoft Müşteri Sözleşmesi.  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Yeni müşteri oluşturun.":::

5. Yeni müşteri iş **akışında** Onay ekranına ulaşıyorsanız müşteri kimlik bilgilerini kaydedin. Bu kimlik bilgilerini daha sonra müşterinize verebilirsiniz.

6. Bu İş Ortağı Merkezi, müşteriyi Microsoft Müşteri Sözleşmesi Center'da hesabı kabul etmeye davet eden bir e-Microsoft 365 Yönetici gönderin. E-postaya şu öğeleri dahil edin:

   - Bu [URL'nin bağlantısı](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Oturum açma gereklidir)

   - Müşterinin 5. Adımda kaydedilen kimlik bilgileri.

7. Müşteri daha sonra iş ortağından e-posta daveti alır ve URL'sini [seçer.](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement)

8. Müşteri, Microsoft 365 Yönetici kimlik bilgilerini kullanarak Microsoft 365 Yönetici Center'da oturum açma.

9. Müşteri, Microsoft Müşteri sözleşmesi kabul etmek için kutuyu kontrol eder.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Kurumsal bayi ilişkisini ve kurumsal bayi ilişkisini gözden geçirmek ve kabul etmek için yeni bir müşteri Microsoft Müşteri Sözleşmesi 

Yeni bir müşteriyi kurumsal bayi ilişkisini ve kurumsal bayi ilişkisini gözden geçirmesi ve kabul etmeye davet etmek için aşağıdaki adımları Microsoft Müşteri Sözleşmesi. 

1. İş Ortağı Merkezi'nin Müşteriler sekmesinden Bayi **ilişkisi isteği bağlantısı'ı** seçin.  

2. Metni ve müşteriyi Microsoft 365 Yönetici Center'a yönlendiren parametreli BIR URL dahil olmak üzere otomatik bir e-posta şablonu oluşturulur.

3. Otomatik olarak oluşturulan e-posta şablonunu özelleştirilebilir ve ardından Panoya kopyala veya **E-postada** **aç'ı seçin.**

4. Bu e-posta şablonunu kullanarak müşteriyi kurumsal bayi ilişkisi isteğini **kabul etmeye davet** Microsoft Müşteri Sözleşmesi.  (Not: E-posta daveti sırasında iş ortağının otomatik olarak sağlanan URL'yi ve kısa süre önce oluşturulan müşteri kimlik bilgilerini de içerip dahil etmeyebilirsiniz.)

   :::image type="content" source="images/mca/createrelationship.png" alt-text="bir ilişki oluşturun.":::

5. Müşteri daveti e-postayla alır ve parametreli URL'ye tıklar. 

6. Müşteri, e-posta içinde sağ istediğiniz kimlik bilgilerini kullanarak Microsoft 365 Yönetici kullanır.

7. Müşteri, kurumsal bayi ilişkisini kabul etmek **için kutuyu Microsoft Müşteri Sözleşmesi.** 

8. Aynı URL'de müşteri birlikte çalıştığı farklı iş ortaklarının birleştirilmiş listesini görebilir. Ayrıntıları görmek için bir iş ortağını seçerek.

   :::image type="content" source="images/mca/accept.jpg" alt-text="Sözleşmeyi kabul etme.":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Mevcut bir müşteriyi sözleşmeyi gözden geçirmesi ve kabul etmeleri için davet etme

Mevcut bir müşteriyi değerlendirmeye ve kabul etmeye davet etmek için aşağıdaki adımları Microsoft Müşteri Sözleşmesi. 

1. Ekli URL ile müşteri e-postası oluşturun ve müşterinizi bu e-posta adresini Microsoft Müşteri Sözleşmesi.

2. Müşteriniz daveti e-postayla alır ve [URL'ye tıklar.](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) 

3. Müşteri, kimlik bilgilerini Microsoft 365 Yönetici Center'a girer.

4. Müşteriniz, onay kutusunu işaret Microsoft Müşteri Sözleşmesi. 

5. Müşteri aynı URL'de birlikte çalıştığı farklı iş ortaklarının birleştirilmiş listesini görebilir. Ayrıntıları görmek için bir iş ortağını seçerek.

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Müşteri.":::

>[!NOTE]
>Bazı senaryolarda, müşteriler doğrudan bu senaryoyu kabul Microsoft Müşteri Sözleşmesi. Bu durumlar hakkında daha fazla bilgi edinmek için aşağıdaki İki senaryoyu okuyun: Müşteriniz adına test etmek için gereken iki senaryo.

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a>Müşterinizin adına test etmeniz gereken iki senaryo

müşterilerin, Microsoft müşteri anlaşmasını Microsoft 365 Yönetici merkezi 'nde doğrudan kabul edebilecekleri iki senaryo vardır.

**Senaryo 1**: mevcut bir müşteri, mevcut bir iş ortağı ilişkisi aracılığıyla aşağıdakilerden birini satın aldı: teklifler, yazılım veya yazılım abonelikleri, ayrılmış örnekler veya Azure planı. Müşteri artık yeni satın alma işlemi gerçekleştirmeye çalışıyor (otomatik yenileme hariç). Bu müşteri URL 'YI tıklattığında, "Microsoft Müşteri anlaşmasını kabul etmek için lütfen Iş ortağınıza ulaşın" iletisini alırlar.  

**Çözümlemek için**: müşteri adına test etmeniz gerekir.

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Microsoft müşteri sözleşmesinin kabul edildiğini onaylamak için iş ortağınıza ulaşmanızı isteyen Microsoft 365 Yönetici Center sayfasının ekran görüntüsü.":::

**Senaryo 2**: mevcut bir müşteri, aşağıdaki tekliflerden, yazılım ve yazılım aboneliklerinden, ayrılmış örneklerden ve Azure planından herhangi birini satın almış. Müşteri artık yeni bir iş ortağıyla yeni satın alma yapmaya çalışıyor.

müşteri yeni iş ortağı ilişkisini ve sözleşmeyi kabul etmek için Microsoft 365 Yönetici Center URL 'sini tıkladığında, "Microsoft müşteri sözleşmesi 'ni kabul etmiş olduğunuz için iş ortağınıza ulaşın" iletisini alırlar.  

**Çözümlemek için**: müşteri adına test etmeniz gerekir.  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a>Müşterinin sözleşmeyi kabul ettiğini onaylama

Daha önce teyit edilmemiş mevcut bir müşteri için yeni bir sipariş oluşturmayı denerseniz, onayı tamamlamaya yönelik bir istem alırsınız. Bunu yapmak için aşağıdaki yordamı kullanın.

1. sözleşmeyi kabul eden kullanıcının **adını**, **soyadını**, **e-posta adresini** ve **Telefon numarasını** (isteğe bağlı) girin.

2. **Sözleşme kabul tarihi** altında, uygun tarihi girin. Bunu gelecekteki bir tarihle ayarlayamazsınız.

3. **Kaydet ve devam et**’i seçin. 

## <a name="next-steps"></a>Sonraki adımlar

- [Şirket profili bilgilerini doğrulama veya güncelleştirme](update-your-partner-profile.md)
- [Microsoft Müşteri Sözleşmeleri (bölgeye, dile göre)](Agreements.md)
