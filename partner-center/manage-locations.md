---
title: İş ortağı hesabınızdaki konumları yönetme
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Yeni bir konum ekleme ve bilgisayar, CSP iş, abonelik ve diğer işlemlerde MPN KIMLIĞI 'nin nasıl kullanıldığını öğrenin.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b994d4dc483e030586ea615b5835afbc7555cabe
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129075849"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a>MPN hesap konumlarını yönetme ve konum ekleme (silme)

**Uygun roller**: genel yönetici | Hesap Yöneticisi

MPN KIMLIĞI konumu, şirketinizin her belirli bir konumunu tanımlar. mpn kimlik konumunu,, transact Bulut Çözümü Sağlayıcısı (CSP) işletmeye ve diğer iş işlemlerine teşvik etmek için kullanabilirsiniz. Genel MPN KIMLIĞI, destek istekleri gibi işlem olmayan etkinlikler için kullanılır.

## <a name="the-following-scenario-is-typical"></a>Aşağıdaki senaryo tipik bir davranıştır:

Contoso, UK 'teki ortak genel hesabına (PGA) sahiptir. PGA, kayıtlı yasal işletmektir ve tüm hareketsel olmayan işleri yönetmek için genel MPN KIMLIĞI kullanılır. Contoso Ayrıca, UK, Fransa ve ABD 'de başka bir konumdaki yan kuruluşlar veya bölümler için Iş ortağı konum hesapları (PLA) ile eşdeğerdir. MPN hesap yapısında, bu PLAs 'ler benzersiz konum MPN kimlikleri olarak gösterilir. PLAs 'ler, CSP veya teşvikleri programları gibi işlem işleri için kullanılır. Ödemeler belirli konumlara bağlıdır.

> [!NOTE]
> CSP kiracısı ve MPN konum KIMLIĞI arasında bire bir ilişki vardır.

:::image type="content" source="images/locations/locations1.png" alt-text="MPN konumlarının yapısı.":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>Bir CSP işletmesi için yeni bir hesap ekleme konusunda ön koşullar

Yeni bir CSP iş hesabı eklemek için önkoşulları karşıladığından emin olarak başlayın.

1. CSP iş yapmak istediğiniz ülkede MPN KIMLIĞI 'ne sahip olmanız gerekir. Yeni bir MPN konumu oluşturmak için aşağıdaki "MPN konum Ekle" bölümünü okuyun.
  
2. Yeni bir CSP dolaylı satıcı kaydı oluşturmak için, [dolaylı sağlayıcılarla iş](indirect-reseller-tasks-in-partner-center.md#get-started)makalesini okuyun.

> [!NOTE]
> **Yeni** CSP hesabının **Yeni** kimlik bilgileriyle oturum açmayı unutmayın. Mevcut kimlik bilgilerinizi, Iş Ortağı Merkezi zaten bir hesap varmış gibi tanıyacak şekilde kullanmayacaktır.

3. Microsoft Iş ortağı sözleşmesi 'Ni kabul edin ve hesabı etkinleştirin.

4. Doğrudan fatura ortağı olarak kaydolmak istiyorsanız, [doğrudan fatura ortakları Için gereksinimleri](direct-partner-new-requirements.md) okuyun

## <a name="view-and-update-your-mpn-locations"></a>MPN konumlarınızı görüntüleyin ve güncelleştirin

1. MPN hesabı kimlik bilgilerinizle [Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard) oturum açın. (MPN kimlik bilgileriniz CSP kimlik bilgilerinizle farklı olabilir.)

2. Ayarlar dişli simgesini seçin ve ardından **hesap Ayarlar**, sonra **yasal**' ı seçin.

3. **Iş ortağı** sekmesinde, GEÇIRILEN konumları PMC 'den düzelmenizi isteyen bir başlık hata iletisi bulunmadığını doğrulayın.  Konumlarınız PMC 'de doğru şekilde ayarlanmamışsa ve henüz BILGISAYARA geçirilmediyse, bu konumları güncelleştirmeniz gerekir.

:::image type="content" source="images/locations/location-two.png" alt-text="Screencap, konumun nasıl güncelleştirilmesini gösterir.":::

4. **PMC konumlarını gözden geçir** ekranında **Güncelleştir**' i seçin.
Aşağıdaki alanları güncelleştirin:

- **Ad alanı**: Şirket konumunun adının doğru olduğundan emin olun. Yinelenen bir hata görüntüleniyorsa, örneğin contoso-contoso, Inc. arasında değişiklik yapmayı deneyin.

- **Yasal varlık alanı**: konumun bağlı olduğu yasal varlığı seçtiğinizden emin olun

- **Adres satırı 1 & 2 alan**: adresin doğru olduğundan emin olun

- **Şehir & Eyalet/İl alanları**: City ve eyalet/eyalet arasındaki birleşimin doğru olduğundan emin olun. Eyalet/bölge ' yi seçmek için açılan menünün uygulanacağı ve diğer ülkelerde alanın el ile eklenmesi gereken ülkeler vardır.

- **ZIP/posta kodu alanı**: ZIP kodu alanının belirttiğiniz ülke, bölge, şehir veya adresle aynı olduğundan emin olun.

- **Birincil iletişim bilgileri alanları**: ilk ve son ad alanlarının doldurulduğundan ve belirtilen e-posta adresinin kişisel bir e-posta adresi (örneğin,, @outlook.com @live.com vb.) olduğundan emin olun.

- **Telefon numarası alanı**: Telefon numarasının özel karakterler, boşluklar veya ülke kodu içermediğinden emin olun. Telefon Number alanına girilen değer her zaman en fazla 10 karakter içerir.

5. bir hata mesajı yoksa **Ayarlar**'den **hesap Ayarlar**, **kuruluş profili**, **tanımlayıcılar**' ı seçin.

6. "Location" türünde, bu CSP hesabının ülkesiyle eşleşen MPN KIMLIĞINI bulun ve ilişkilendirmeyi gerçekleştirmek için onu kullanın.

7. Kullanmak istediğiniz CSP hesabıyla eşleşen MPN KIMLIĞI konumunu bulamazsanız yeni bir MPN KIMLIĞI oluşturacak yeni bir konum ekleyebilirsiniz. Aşağıda **BIR MPN konumu ekleme** bölümüne bakın.

## <a name="add-an-mpn-location"></a>MPN konumu ekleme

1. Iş Ortağı Merkezi 'nde MPN hesabını kullanarak oturum açın. (MPN kimlik bilgileriniz CSP kimlik bilgilerinizle farklı olabilir.) MPN hesabının genel yönetici veya hesap yönetici ayrıcalıklarına sahip olması gerekir.

2. Ayarlar dişli simgesini, sonra **hesap Ayarlar** ve ardından **kuruluş profili**' ni seçin.

3. **Yasal** ' ı seçin ve sonra iş **ortağı** sekmesinde **iş konumları '** nı seçin ve **Konum Ekle** ' yi seçin.

4. Şirketinize eklemek istediğiniz konum için iş adı, adres ve ilgili kişi dahil olmak üzere gerekli ayrıntıları sağlayın.

5. **Konum Ekle**' yi seçin. Bu, CSP işlemleri ve teşvikleri için kullanabileceğiniz yeni konum için yeni bir MPN KIMLIĞI oluşturur.

:::image type="content" source="images/legal-biz.png" alt-text="Yeni bir hukuk işi ekleyin.":::

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

Hesabınızdan bir konum silmek için [Iş ortağı desteğine](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b)başvurmanız gerekecektir. Bu eylemin sonuçlarını anladığınızdan emin olun. Silinen konumlar alınamaz ve söz konusu MPN KIMLIğINE bağlı olan herhangi bir şey artık şirketiniz için tanınmayacak veya etkin olmayacak.

## <a name="change-country-of-partner-global-account"></a>Ortak genel hesap ülkesini değiştirin

1. Iş Ortağı Merkezi 'nde MPN hesabını kullanarak oturum açın. (MPN kimlik bilgileriniz CSP kimlik bilgilerinizle farklı olabilir.) MPN hesabının genel yönetici veya hesap yönetici ayrıcalıklarına sahip olması gerekir.

2. Ayarlar dişli simgesini seçin, sonra **hesap Ayarlar**. Iş **ortakları** sekmesinde **iş konumları** ' na gidin ve yasal varlığınız olarak istediğiniz konumun listelendiğinden emin olmak için konumların listesini kontrol edin.

3. Konum eklemek için, **Konum Ekle**' ye tıklayın ve kullanıma hazır olarak, şirketinizde eklemek istediğiniz konum için iş adı, adres ve birincil kişi dahil olmak üzere gerekli ayrıntıları sağlayın.

4. Ülke **/bölge** açılır listesinin yanındaki **ülkenizi değiştirin** ' i seçin ve adımları izleyin.

:::image type="content" source="images/lbp.png" alt-text="Yasal iş profili verileri kullanıma hazır.":::

5. **Kaydet**’i seçin.

6. MPN küresel hesap ülkesi, yeni yasal ülkeyle değiştirilecektir.
  
## <a name="next-steps"></a>Sonraki adımlar

- [Doğrulama süreci](verification-responses.md)hakkında bilgi edinin.
