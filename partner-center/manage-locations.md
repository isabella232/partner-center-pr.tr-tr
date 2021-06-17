---
title: İş ortağı hesabınızla konumları yönetme
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Teşvik programlarında, CSP işlerde, aboneliklerde ve diğer işlemlerde yeni konum ve konum MPN kimliğinin nasıl kullanılabı hakkında bilgi edinin.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3d30f250d6635758f3bef8e06c6f57ba0a0be744
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276833"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a>MPN hesap konumlarınızı yönetme ve konum ekleme (silme)


**Uygun roller:** Genel yönetici | Hesap yöneticisi

Konum MPN Kimliği, şirketinizin belirli her konumunu tanımlar. Teşvik programlarına kaydolmak, iş (CSP) ve diğer iş Bulut Çözümü Sağlayıcısı için konum MPN Kimliğini kullanırsiniz. Genel MPN Kimliği, destek istekleri gibi işlem dışı etkinlikler için kullanılır.

## <a name="the-following-scenario-is-typical"></a>Aşağıdaki senaryo tipiktir:

Contoso'da İş Ortağı genel hesabı (PGA) var. PGA, kayıtlı yasal işletmedir ve genel MPN kimliği tüm işlem dışı işletmeleri yönetmek için kullanılır. Contoso ayrıca Birleşik Krallık, Fransa ve ABD'deki başka bir konumdaki yan kuruluş veya bölümlere eşdeğer İş Ortağı konum hesaplarına (PLA) sahiptir. MPN Hesabı yapısında, bu PLA'lar benzersiz konum MPN kimlikleri olarak temsil edildi. PLA'lar CSP veya teşvik programları gibi işlem işletmeleri için kullanılır. Ödemeler belirli konumlara bağlanır. 

>[!NOTE]
>CSP kiracısı ile MPN konum kimliği arasında 1-1 ilişkisi vardır.

:::image type="content" source="images/locations/locations1.png" alt-text="MPN konumlarının yapısı.":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>CSP işletmesi için yeni bir hesap eklemek için önkoşullar

Yeni bir CSP iş hesabı eklemek için önkoşulları yerine getirmenize yardımcı olun.

1. CSP iş yapmak istediğiniz ülkede bir konum MPN Kimliğine sahipsiniz. Yeni bir MPN konumu oluşturmak için aşağıdaki "MPN konumu ekleme" makalesi'ne bakın.
  
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

- **ZIP/ Posta kodu alanı:** Posta Kodu alanında belirtilen Ülke, Bölge, Şehir veya Adres ile eş olduğundan emin olun.

- **Birincil iletişim bilgileri alanları:** Ad ve soyadı alanlarının doldurul olduğundan ve belirtilen e-posta adresinin kişisel bir adres (örneğin, @outlook.com , vb.) değil iş e-posta adresi @live.com olduğundan emin olun

- **Telefon numarası alanı:** Telefon numarası'nın özel karakterler, boşluklar veya ülke kodu içermeyerin. Telefon Numarası alanına girilen değer her zaman en fazla 10 karakter içerir.

5. Hata iletisi yoksa Ayarlar'dan Hesap **Ayarları,** Kuruluş profili **,** **Tanımlayıcılar'ı** **seçin.**

6. Bu CSP hesabının ülkesiyle eşleşen "Konum" Türüne sahip MPN Kimliğini bulun ve ilişkilendirmeyi tamamlamak için kullanın.

7. Kullanmak istediğiniz CSP hesabıyla eşleşen konum MPN Kimliğini bulamazsanız, yeni bir konum ekleyebilir ve bu da yeni bir MPN kimliği oluşturabilir. Aşağıdaki **MPN konumu eklemeye** bakın.

## <a name="add-an-mpn-location"></a>MPN konumu ekleme

1. MpN hesabını kullanarak oturum açın ve İş Ortağı Merkezi. (MPN kimlik bilgileriniz CSP kimlik bilgilerinizden farklı olabilir.) MPN hesabının Genel Yönetici veya Hesap Yöneticisi ayrıcalıkları olmalıdır. 

1. Ayarlar **simgesinden Hesap** **ayarları'nın ve ardından Kuruluş** **profili'nin seçin.**

2. **Yasal'ı** seçin ve ardından **İş Ortağı** sekmesinde İş **konumları'nın ardından Konum** **ekle'yi seçin.**

3. Şirketinize eklemek istediğiniz konum için iş adı, adres ve iletişim gibi gerekli ayrıntıları girin.
 
1. Konum **ekle'yi seçin.** Bu, CSP işlemleri ve teşvikleri için kullanabileceğiniz yeni konum için yeni bir MPN kimliği oluşturacak.

:::image type="content" source="images/legal-biz.png" alt-text="Yeni bir yasal işletme ekleyin.":::

> [!NOTE]
> Bir konum İş Ortağı Merkezi kaldıramazsiniz. Oturum açma için **doğru MPN** kimliğini kullandıysanız İş Ortağı Merkezi menüsünde MPN'i görünür.

## <a name="add-the-registration-number-id"></a>Kayıt numarası kimliğini ekleme

Dolaylı sağlayıcı, Doğrudan fatura iş ortağı veya Dolaylı kurumsal bayiysiniz ve aşağıdaki ülkelerdeki yeni veya mevcut müşterilerle iş yapıyorsanız işletmeniz için kayıt kimliği numaralarını sağlayabilirsiniz. İş yapmakta olduğunuz ülke aşağıda listelenmiyorsa kayıt kimliği isteğe bağlıdır.

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

:::image type="content" source="images/lbp.png" alt-text="Yasal iş profili verileri çıkar.":::

5. **Kaydet**’i seçin.

6. MPN genel hesap ülkesi, yeni yasal ülke olarak değiştirilir.
  
## <a name="next-steps"></a>Sonraki adımlar

- Doğrulama işlemi hakkında [bilgi edinin.](verification-responses.md)
