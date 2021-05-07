---
title: İş ortağı hesabınızdaki konumları yönetin
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Yeni bir konum ekleme ve bilgisayar, CSP iş, abonelik ve diğer işlemlerde MPN KIMLIĞI 'nin nasıl kullanıldığını öğrenin.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a2b4fa8b204b10d5d45c0e1409ab4bc463e272f
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702901"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a>MPN hesap konumlarını yönetme ve konum ekleme (silme)


**Uygun roller**

- Genel yönetici
- Hesap yöneticisi

MPN KIMLIĞI konumu, şirketinizin her belirli bir konumunu tanımlar. MPN KIMLIK konumunu kullanarak, uygulamaları, Transact bulut çözümü sağlayıcısı (CSP) işletme ve diğer iş işlemlerine, teşvik etmek için kullanabilirsiniz. Genel MPN KIMLIĞI, destek istekleri gibi işlem olmayan etkinlikler için kullanılır.

## <a name="the-following-scenario-is-typical"></a>Aşağıdaki senaryo tipik bir davranıştır:

Contoso, UK 'teki ortak genel hesabına (PGA) sahiptir. PGA, kayıtlı yasal işletmektir ve tüm işlemsel olmayan işleri yönetmek için Global MPN KIMLIĞI kullanılır. Contoso Ayrıca, UK, Fransa ve ABD 'de başka bir konumdaki yan kuruluşlar veya bölümler için Iş ortağı konum hesapları (PLA) ile eşdeğerdir. MPN hesap yapısında, bu PLAs 'ler benzersiz konum MPN kimlikleri olarak gösterilir. PLAs 'ler, CSP veya teşvikleri programları gibi işlem işleri için kullanılır. Ödemeler belirli konumlara bağlıdır. 

>[!NOTE]
>CSP kiracısı ve MPN konum KIMLIĞI arasında bir 1-1 ilişkisi vardır.

:::image type="content" source="images/locations/locations1.png" alt-text="MPN konumlarının yapısı":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>CSP iş için yeni bir hesap eklemek için Önkoşullar

Yeni bir CSP iş hesabı eklemek için önkoşulları karşıladığından emin olarak başlayın.

1. CSP iş yapmak istediğiniz ülkede MPN KIMLIĞI 'ne sahip olmanız gerekir. Yeni bir MPN konumu oluşturmak için aşağıdaki "MPN konum Ekle" bölümünü okuyun.
  
1. Yeni bir CSP dolaylı satıcı kaydı oluşturmak için, [dolaylı sağlayıcılarla iş](indirect-reseller-tasks-in-partner-center.md#get-started) bölümünü okuyun 

>[!NOTE] 
 >**Yeni** CSP hesabının **Yeni** kimlik bilgileriyle oturum açmayı unutmayın. Mevcut kimlik bilgilerinizi, Iş Ortağı Merkezi zaten bir hesap varmış gibi tanıyacak şekilde kullanmayacaktır.

2. Microsoft Iş ortağı sözleşmesi 'Ni kabul edin ve hesabı etkinleştirin.

1. Doğrudan fatura ortağı olarak kaydolmak istiyorsanız, [doğrudan fatura ortakları Için gereksinimleri](direct-partner-new-requirements.md) okuyun

## <a name="view-and-update-your-mpn-locations"></a>MPN konumlarınızı görüntüleyin ve güncelleştirin

1. MPN hesabı kimlik bilgilerinizle Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard/home) oturum açın. (MPN kimlik bilgileriniz CSP kimlik bilgilerinizle farklı olabilir) 
 
1. **Ayarlar** simgesinden **Hesap ayarları**, **kuruluş profili**, **yasal**' ı seçin. 

1. **Iş ortağı** sekmesinde, GEÇIRILEN konumları PMC 'den düzelmenizi isteyen bir başlık hata iletisi bulunmadığını doğrulayın.  Konumlarınız PMC 'de doğru şekilde ayarlanmamışsa ve henüz BILGISAYARA geçirilmediyse, bu konumları güncelleştirmeniz gerekir.

:::image type="content" source="images/locations/location-two.png" alt-text="Screencap, konumun nasıl güncelleştirilmesini gösterir.":::
 
4.  **PMC konumlarını gözden geçir** ekranında **Güncelleştir**' i seçin.
Aşağıdaki alanları güncelleştirin:

- **Ad alanı**: Şirket konumunun adının doğru olduğundan emin olun. Yinelenen bir hata görüntüleniyorsa, örneğin contoso-contoso, Inc. arasında değişiklik yapmayı deneyin.

- **Yasal varlık alanı**: konumun bağlı olduğu yasal varlığı seçtiğinizden emin olun

- **Adres satırı 1 & 2 alan**: adresin doğru olduğundan emin olun

- **Şehir & Eyalet/İl alanları**: City ve eyalet/eyalet arasındaki birleşimin doğru olduğundan emin olun. Eyalet/bölge ' yi seçmek için açılan menünün uygulanacağı ve diğer ülkelerde alanın el ile eklenmesi gereken ülkeler vardır.

- **ZIP/posta kodu alanı**: ZIP kodu alanının belirttiğiniz ülke, bölge, şehir veya adresle aynı olduğundan emin olun.

- **Birincil iletişim bilgileri alanları**: ilk ve son ad alanlarının doldurulduğundan ve belirtilen e-posta adresinin kişisel bir e-posta adresi (örneğin,, @outlook.com @live.com vb.) olduğundan emin olun.

- **Telefon numarası alanı**: telefon numarasının özel karakterler, boşluklar veya ülke kodu içermediğinden emin olun. Telefon numarası alanına girilen değer her zaman en fazla 10 karakter içerir.

5. Bir hata mesajı yoksa,  **Ayarlar**' dan  **Hesap ayarları**, **kuruluş profili**, **tanımlayıcılar**' ı seçin.

6. "Location" türünde, bu CSP hesabının ülkesiyle eşleşen MPN KIMLIĞINI bulun ve ilişkilendirmeyi gerçekleştirmek için onu kullanın.

7. Kullanmak istediğiniz CSP hesabıyla eşleşen MPN KIMLIĞI konumunu bulamazsanız yeni bir MPN KIMLIĞI oluşturacak yeni bir konum ekleyebilirsiniz. Aşağıda **BIR MPN konumu ekleme** bölümüne bakın.

## <a name="add-an-mpn-location"></a>MPN konumu ekleme

1. Iş Ortağı Merkezi 'nde MPN hesabını kullanarak oturum açın. (MPN kimlik bilgileriniz CSP kimlik bilgilerinizle farklı olabilir). MPN hesabının genel yönetici veya hesap yönetici ayrıcalıklarına sahip olması gerekir. 

1. **Ayarlar simgesinden** **Hesap ayarları** ' nı seçin ve ardından **kuruluş profili**' ni seçin.

2. **Yasal** ' ı seçin ve sonra iş **ortağı** sekmesinde **iş konumları** ' nı seçin ve **Konum Ekle** ' ye tıklayın.

3. Şirketinize eklemek istediğiniz konum için iş adı, adres ve ilgili kişi dahil olmak üzere gerekli ayrıntıları sağlayın.
 
1. **Konum Ekle**' ye tıklayın. Bu, yeni konum için CSP işlemleri ve teşvikleri için kullanabileceğiniz yeni bir MPN KIMLIĞI oluşturur.

:::image type="content" source="images/legal-biz.png" alt-text="Yeni bir yasal iş ekleyin":::

> [!NOTE]
> Iş Ortağı Merkezi 'ne bir konum eklendikten sonra kaldıramazsınız. Oturum açmak için doğru MPN KIMLIĞINI kullandıysanız, **MPN** 'Yi Iş Ortağı Merkezi 'nin sol menüsünde görürsünüz.

## <a name="add-the-registration-number-id"></a>Kayıt numarası KIMLIĞINI ekleyin

Dolaylı bir Sağlayıcıysanız, doğrudan faturanız veya dolaylı satıcısıysanız ve aşağıdaki ülkelerde yeni veya mevcut müşterilerle iş yapıyorsanız, işletmeniz için kayıt KIMLIĞI numaraları sağlamanız gerekir. İş yapmakta olduğunuz ülke aşağıda listelenmiyorsa kayıt KIMLIĞI isteğe bağlıdır.

- Ermenistan 
- Azerbaycan 
- Belarus 
- Brezilya 
- Macaristan 
- Hindistan 
- Irak 
- Kazakistan 
- Kırgızistan 
- Moldova 
- Myanmar 
- Polonya 
- Rusya 
- Suudi Arabistan 
- Güney Afrika 
- Güney Sudan  
- Tacikistan 
- Tayland
- Türkiye 
- Ukrayna 
- Birleşik Arap Emirlikleri 
- Özbekistan 
- Venezuela
- Vietnam 


Daha fazla bilgi için [kayıt kimliği numarası bilgilerini](reg-number-id.md) okuyun

## <a name="delete-a-location"></a>Konum silme

Hesabınızdan bir konum silmek için [Iş ortağı desteğine](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b)başvurmanız gerekecektir. Bu eylemin sahip olduğu etkiyi anladığınızdan emin olun. Silinen konumlar alınamaz ve söz konusu MPN kimliğine bağlı olan herhangi bir şey artık şirketiniz için tanınmayacak veya etkin olmayacak.

## <a name="change-country-of-partner-global-account"></a>Ortak genel hesap ülkesini değiştirin 

1. Iş Ortağı Merkezi 'nde MPN hesabını kullanarak oturum açın. (MPN kimlik bilgileriniz CSP kimlik bilgilerinizle farklı olabilir). MPN hesabının genel yönetici veya hesap yönetici ayrıcalıklarına sahip olması gerekir. 

2. Iş **ortakları** sekmesinde **iş konumları** ' na gidin ve yasal varlığınız olarak istediğiniz konumun listelendiğinden emin olmak için konumların listesini kontrol edin. 
 
1. Konum eklemek için, **Konum Ekle**' ye tıklayın ve kullanıma hazır olarak, şirketinizde eklemek istediğiniz konum için iş adı, adres ve birincil kişi dahil olmak üzere gerekli ayrıntıları sağlayın. 
 
1. **Ülke/bölge** açılır seçeneğinin yanındaki **ülkenizi değiştirin** ' i seçin ve adımları izleyin. 

:::image type="content" source="images/lbp.png" alt-text="Yasal iş profili verileri kullanıma hazır":::

5. **Kaydet**’e tıklayın.

6. MPN küresel hesap ülkesi, yeni yasal ülkeyle değiştirilecektir.
  
## <a name="next-steps"></a>Sonraki adımlar

- [Doğrulama süreci](verification-responses.md)hakkında bilgi edinin.
