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
ms.openlocfilehash: 13d6e7dc4722227035be2b24df48427f2008bb14
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151789"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a>MPN hesap konumlarını yönetme ve konum ekleme (silme)


**Uygun roller**: genel yönetici | Hesap Yöneticisi

MPN KIMLIĞI konumu, şirketinizin her belirli bir konumunu tanımlar. MPN KIMLIK konumunu kullanarak, uygulamaları, Transact bulut çözümü sağlayıcısı (CSP) işletme ve diğer iş işlemlerine, teşvik etmek için kullanabilirsiniz. Genel MPN KIMLIĞI, destek istekleri gibi işlem olmayan etkinlikler için kullanılır.

## <a name="the-following-scenario-is-typical"></a>Aşağıdaki senaryo tipik bir davranıştır:

Contoso, UK 'teki ortak genel hesabına (PGA) sahiptir. PGA, kayıtlı yasal işletmektir ve tüm hareketsel olmayan işleri yönetmek için genel MPN KIMLIĞI kullanılır. Contoso Ayrıca, UK, Fransa ve ABD 'de başka bir konumdaki yan kuruluşlar veya bölümler için Iş ortağı konum hesapları (PLA) ile eşdeğerdir. MPN hesap yapısında, bu PLAs 'ler benzersiz konum MPN kimlikleri olarak gösterilir. PLAs 'ler, CSP veya teşvikleri programları gibi işlem işleri için kullanılır. Ödemeler belirli konumlara bağlıdır. 

>[!NOTE]
>CSP kiracısı ve MPN konum KIMLIĞI arasında bir 1-1 ilişkisi vardır.

:::image type="content" source="images/locations/locations1.png" alt-text="MPN konumlarının yapısı":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>CSP iş için yeni bir hesap eklemek için Önkoşullar

Yeni bir CSP iş hesabı eklemek için önkoşulları karşıladığından emin olarak başlayın.

1. CSP iş yapmak istediğiniz ülkede MPN KIMLIĞI 'ne sahip olmanız gerekir. Yeni bir MPN konumu oluşturmak için aşağıdaki "MPN konum Ekle" bölümünü okuyun.
  
1. Yeni bir kayıt CSP Indirect Reseller için Dolaylı [sağlayıcılarla çalışma makalesi](indirect-reseller-tasks-in-partner-center.md#get-started) 

>[!NOTE] 
 >Yeni CSP hesabı için **yeni** kimlik bilgileriyle **oturum** açmayı unutmayın. Mevcut kimlik bilgilerinizi, sizi zaten bir İş Ortağı Merkezi olarak tanıyacak şekilde kullanmayın.

2. Hesabı Microsoft İş Ortağı Sözleşmesi hesabı etkinleştirin.

1. Doğrudan Fatura iş ortağı olarak kaydolmak için, Doğrudan Fatura iş [ortakları için gereksinimler makaleyi okuyun](direct-partner-new-requirements.md)

## <a name="view-and-update-your-mpn-locations"></a>MPN konumlarınızı görüntüleme ve güncelleştirme

1. MPN hesabı İş Ortağı Merkezi [kimlik](https://partner.microsoft.com/dashboard/home) bilgilerinizle panoda oturum açın. (MPN kimlik bilgileriniz CSP kimlik bilgilerinizden farklı olabilir) 
 
1. Ayarlar **simgesinden** Hesap ayarları, **Kuruluş profili**, **Yasal'ı** **seçin.** 

1. İş **Ortağı sekmesinde,** PMC'den geçirilen konumları düzeltmenizi isteyen bir başlık hata iletisi olmadığını doğrulayın.  Konumlarınız PMC'de doğru şekilde ayarlanmadıysa ve henüz PC'ye geçiş yapılmadıysa, bu konumları güncelleştirmeniz gerekir.

:::image type="content" source="images/locations/location-two.png" alt-text="Ekran kapsülde konumun nasıl güncelleştiril olduğu gösterilir.":::
 
4.  **PMC konumlarını gözden geçir ekranında** Güncelleştir'i **seçin.**
Aşağıdaki alanları güncelleştirin:

- **Ad alanı:** Şirket konumunun adının doğru olduğundan emin olun. Yinelenen bir hata görüntülenirse, örneğin Contoso'dan Contoso, Inc.

- **Yasal Varlık alanı:** Konumun bağlı olduğu yasal varlığı seçtiğinizden emin olun

- **1. adres & 2 alanı içerir:** Adresin doğru olduğundan emin olun

- **Şehir & Eyalet/İl alanları:** Şehir ile eyalet/il arasındaki birleşimin doğru olduğundan emin olun. Eyalet/İl seçimi için açılan menenin geçerli olduğu ve diğer ülkelerde bu alanın el ile eklenmek zorunda olduğu ülkeler vardır.

- **ZIP/posta kodu alanı**: ZIP kodu alanının belirttiğiniz ülke, bölge, şehir veya adresle aynı olduğundan emin olun.

- **Birincil iletişim bilgileri alanları**: ilk ve son ad alanlarının doldurulduğundan ve belirtilen e-posta adresinin kişisel bir e-posta adresi (örneğin,, @outlook.com @live.com vb.) olduğundan emin olun.

- **Telefon numarası alanı**: telefon numarasının özel karakterler, boşluklar veya ülke kodu içermediğinden emin olun. Telefon numarası alanına girilen değer her zaman en fazla 10 karakter içerir.

5. Bir hata mesajı yoksa,  **Ayarlar**' dan  **Hesap ayarları**, **kuruluş profili**, **tanımlayıcılar**' ı seçin.

6. "Location" türünde, bu CSP hesabının ülkesiyle eşleşen MPN KIMLIĞINI bulun ve ilişkilendirmeyi gerçekleştirmek için onu kullanın.

7. Kullanmak istediğiniz CSP hesabıyla eşleşen MPN KIMLIĞI konumunu bulamazsanız yeni bir MPN KIMLIĞI oluşturacak yeni bir konum ekleyebilirsiniz. Aşağıda **BIR MPN konumu ekleme** bölümüne bakın.

## <a name="add-an-mpn-location"></a>MPN konumu ekleme

1. Iş Ortağı Merkezi 'nde MPN hesabını kullanarak oturum açın. (MPN kimlik bilgileriniz CSP kimlik bilgilerinizle farklı olabilir.) MPN hesabının genel yönetici veya hesap yönetici ayrıcalıklarına sahip olması gerekir. 

1. **Ayarlar simgesinden** **Hesap ayarları** ' nı seçin ve ardından **kuruluş profili**' ni seçin.

2. **Yasal** ' ı seçin ve sonra iş **ortağı** sekmesinde **iş konumları '** nı seçin ve **Konum Ekle** ' yi seçin.

3. Şirketinize eklemek istediğiniz konum için iş adı, adres ve ilgili kişi dahil olmak üzere gerekli ayrıntıları sağlayın.
 
1. **Konum Ekle**' yi seçin. Bu, CSP işlemleri ve teşvikleri için kullanabileceğiniz yeni konum için yeni bir MPN KIMLIĞI oluşturur.

:::image type="content" source="images/legal-biz.png" alt-text="Yeni bir yasal iş ekleyin":::

> [!NOTE]
> Iş Ortağı Merkezi 'ne bir konum eklendikten sonra kaldıramazsınız. Oturum açmak için doğru MPN KIMLIĞINI kullandıysanız, **MPN** 'Yi Iş Ortağı Merkezi 'nin sol menüsünde görürsünüz.

## <a name="add-the-registration-number-id"></a>Kayıt numarası KIMLIĞINI ekleyin

Dolaylı sağlayıcı, Doğrudan fatura iş ortağı veya Dolaylı kurumsal bayiysiniz ve aşağıdaki ülkelerdeki yeni veya mevcut müşterilerle iş yapıyorsanız işletmeniz için kayıt kimliği numaralarını sağlayabilirsiniz. İş yapmakta olduğu ülke aşağıda listelenmiyorsa kayıt kimliği isteğe bağlıdır.

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


Daha fazla bilgi için Kayıt [Kimliği numarası bilgilerini okuyun](reg-number-id.md)

## <a name="delete-a-location"></a>Konum silme

Bir konumu hesabınızla silmek için İş Ortağı Desteği'ne [başvurabilirsiniz.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b) Bu eylemin etkisini anlayasınız. Silinen konumlar alınamaz ve bu MPN kimliğine bağlı herhangi bir şey artık tanınmaz veya şirket için etkin olmaz.

## <a name="change-country-of-partner-global-account"></a>İş ortağı genel hesabının ülkesini değiştirme 

1. MpN hesabını kullanarak oturum açın ve İş Ortağı Merkezi. (MPN kimlik bilgileriniz CSP kimlik bilgilerinizden farklı olabilir.) MPN hesabının Genel Yönetici veya Hesap Yöneticisi ayrıcalıkları olmalıdır. 

2. İş **Ortağı** sekmesinde İş **konumları'ne gidin** ve konum listesini kontrol edin ve yasal varlığınız olarak istediğiniz konumun listelenmiş olduğundan emin olun. 
 
1. Konum eklemek için Konum ekle'ye tıklayın ve iş adı, adres ve şirket için eklemek istediğiniz konumun birincil ilgili kişisi gibi gerekli ayrıntıları girin. 
 
1. **Ülke/bölge açılan** listesinin **yanındaki Ülkenizi** değiştir'i seçin ve adımları izleyin. 

:::image type="content" source="images/lbp.png" alt-text="Yasal iş profili verileri çıkar":::

5. **Kaydet**’i seçin.

6. MPN genel hesap ülkesi, yeni yasal ülke olarak değiştirilir.
  
## <a name="next-steps"></a>Sonraki adımlar

- Doğrulama işlemi hakkında [bilgi edinin.](verification-responses.md)
