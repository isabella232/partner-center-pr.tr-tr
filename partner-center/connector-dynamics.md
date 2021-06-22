---
title: Dynamics 365 CRM için ortak satış bağlayıcısı İş Ortağı Merkezi
description: Şirket içinde İş Ortağı Merkezi Dynamics 365 CRM için ortak satış bağlayıcınız ile eşitler. Daha sonra CRM sisteminizin içinde Microsoft ile ortak satışlar da kullanabilirsiniz.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: e656f728789bf5b13dd09732b0b2f5ef30de760a
ms.sourcegitcommit: b7203f1393c3d8f8db4683acdebd09a89e086c3c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/21/2021
ms.locfileid: "112425111"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>Dynamics 365 CRM için ortak satış bağlayıcısı genel bakış

**Uygun roller:** Referans yöneticisi | CRM'de sistem yöneticisi veya sistem özelleştiricisi

İş Ortağı Merkezi ortak satış bağlayıcıları, satış satıcılarının CRM sistemlerinizin içinde Microsoft ile ortak satışlar oluşturmalarını sağlar. Ortak satış anlaşmalarını yönetmek için bu İş Ortağı Merkezi kullanmak üzere eğitilmaları gerek olmayacaktır. Ortak satış bağlayıcılarını kullanarak bir Microsoft satıcısıyla etkileşime geçen, Microsoft satıcısından referanslar alan, referansları kabul eden veya reddeden ve satış anlaşması değeri ve kapanış tarihi gibi satış verilerini değiştirmek için yeni bir ortak satış referansı oluşturun. Ayrıca bu ortak satış anlaşmaları hakkında Microsoft satıcılarından da güncelleştirmeler edinirsiniz. Tüm referanslarınızı yönetmek yerine kendi tercihlerinizi CRM'de İş Ortağı Merkezi.

Çözüm, api'leri Power Automate temel İş Ortağı Merkezi kullanır.

## <a name="prerequisites"></a>Önkoşullar

Çözümü yüklemeden önce aşağıdaki önkoşullara uygun olduğundan emin olun.

|**Konu başlıkları**   |**Ayrıntılar**   |**Bağlantılar**   |
|--------------|--------------------|------|
|Microsoft İş Ortağı Ağı (MPN) Kimliği |Geçerli bir MPN kimliğine ihtiyacınız vardır.|[İş Ortağı ağına katılma](https://partner.microsoft.com/)|
|Ortak satışa hazır|IP/Hizmetler çözümünüz ortak satışa hazır olmalı.|[Microsoft ile satış](https://partner.microsoft.com/membership/sell-with-microsoft)|
|İş Ortağı Merkezi hesabı|Kiracıyla ilişkilendirilmiş MPN İş Ortağı Merkezi ortak satış çözümünüzle ilişkili MPN Kimliği ile aynı olması gerekir. Bağlayıcıları dağıtmadan önce ortak satış referanslarınızı İş Ortağı Merkezi portalında gördüğünüzü doğrulayın.|[Hesabınızı yönetme](create-user-accounts-and-set-permissions.md)|
|İş Ortağı Merkezi rollerini atama|Bağlayıcıları yükecek ve kullanacak olan çalışanın Referans yöneticisi olması gerekir.|[Kullanıcı rollerini ve izinlerini atama](create-user-accounts-and-set-permissions.md)|
|Dynamics 365 CRM|CRM kullanıcı rolü Sistem yöneticisi veya Sistem özelleştiricisi'dir.|[Dynamics 365'te rol atama](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Power Automate akış hesabı|Test, hazırlama ve üretim için veritabanıyla yeni bir üretim ortamı oluşturun. Veritabanına sahip mevcut bir üretim ortamınız varsa bu ortam yeniden kullanılabilir. Bağlayıcı çözümünü yükleyen kullanıcının bu ortama Power Automate bir lisansa sahip olması gerekir. Yükleme başarısız olursa ilerleme durumunu izleyebilir ve Power Automate [daha](https://flow.microsoft.com/) fazla bilgi edinebilirsiniz. Çözümler **altında Geçmişi gör'i** **seçin.**|[Ortam oluşturma veya yönetme](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Dynamics 365 İş Ortağı Merkezi Referans eşitlemesini yükleme (Power Automate çözümü)

1. Power Automate [gidin](https://flow.microsoft.com)ve sağ **üst** köşedeki Ortamlar'ı seçin. Bu adım size kullanılabilir CRM örneklerini gösterir.

1. Sağ üst köşedeki açılan listeden uygun CRM örneğini seçin.

1. Sol **tarafta** Çözümler'i seçin.

1. Üst **menüden AppSource'ı** Aç bağlantısını seçin.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource'a Aç'ın ekran görüntüsü.":::

1. Açılan **İş Ortağı Merkezi Dynamics 365** için Referans Bağlayıcıları araması gerçekleştirin.  

1. Şimdi **al düğmesini ve** ardından Devam'ı **seçin.**

1. Uygulamayı yüklemek için CRM (Dynamics 365) ortamını seçerek bir sayfa görüntülenir. Hüküm ve koşulları kabul etmek.

1. İlerleme durumunu izleyebilirsiniz ve yükleme başarısız olursa Çözümler'in altında Geçmişi Power Automate'yi seçerek daha **fazla** ayrıntıya **inebilirsiniz.**

1. Yükleme tamamlandıktan sonra, Power Automate geri [dönüp](https://flow.microsoft.com) **Çözümler'i** seçin. **İş Ortağı Merkezi Dynamics 365** için Referans Eşitlemesi artık Çözümler **listesinde** kullanılabilir.

1. **Dynamics 365 İş Ortağı Merkezi Referans Eşitleme'yi seçin.** Aşağıdaki Power Automate ve varlıklar kullanılabilir.

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Kullanılabilir CRM'leri gösteren ekran görüntüsü.":::

## <a name="test-before-you-go-live"></a>Canlı yayına başlamadan önce test

Üretim ortamında bir Power Automate çözümü yüklemeden, yapılandırmadan ve özelleştirmeden önce, çözümü hazırlama CRM örneğinde test etmek için emin olun. Şunları yapmak gerekir:

- Hazırlama Power Automate CRM örneğine uygulama çözümünü yükleyin.
- Hazırlama ortamında Power Automate yapılandırma ve özelleştirme.
- Çözümü hazırlama CRM örneğinde test etmek.
- Başarılı bir test sonrasında yönetilen çözüm olarak üretim örneğine aktarın.

## <a name="configure-the-solution"></a>Çözümü yapılandırma

1. Çözümü CRM örneğine yükledikten sonra [Power Automate.](https://flow.microsoft.com/)

1. Sağ **üst** köşedeki Ortamlar açılan listesinden, Power Automate çözümünü yüklemiş olduğunuz CRM Power Automate seçin.

1. Üç kullanıcı hesabını ilişkilendirilen bağlantılar oluşturmanız gerekir:

   - İş Ortağı Merkezi yönetici kimlik bilgilerine sahip bir kullanıcı
   - İş Ortağı Merkezi Etkinlikleri
   - Çözümde akış Power Automate CRM yöneticisi

   1. Sol **tarafta** Bağlantılar'ı seçin ve **İş Ortağı Merkezi Referanslar** çözümünü seçin.

   1. Bağlantı oluştur'a **seçerek bağlantı oluşturun.**

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Bağlantı oluştur'ları gösteren ekran görüntüsü.":::

   1. Sağ **İş Ortağı Merkezi arama çubuğunda Referanslar (önizleme)** araması gerçekleştirin.

   1. Referans yöneticisinin kimlik bilgileri İş Ortağı Merkezi kullanıcınız için bir bağlantı oluşturun.

   1. Ardından, Referanslar İş Ortağı Merkezi kimlik bilgileriyle İş Ortağı Merkezi kullanıcınız için bir Olay bağlantısı oluşturun.

   1. CRM yönetici kullanıcısı için Common Data Service (geçerli ortam) için bir bağlantı oluşturun.
     
   1. Tüm bağlantıları ekledikten sonra ortamınıza aşağıdaki bağlantıları görüyor gerekir.

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Bağlantıları gösteren ekran görüntüsü.":::

## <a name="edit-the-connections"></a>Bağlantıları düzenleme

1. Çözümler sayfasına geri **dönüp** Varsayılan **Çözüm'i seçin.** Tüm **'i seçerek Bağlantı Başvurusu (önizleme)** **öğesini seçin.**

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Bağlantıları düzenlemeyi gösteren ekran görüntüsü.":::

1. Üç nokta simgesini seçerek bağlantıların her bir öğesini tek tek düzenleyin. İlgili bağlantıları ekleyin.

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Listelenen bağlantıları gösteren ekran görüntüsü.":::

1. Çözümler sayfasına **geri** dönüp **Dynamics 365** için İş Ortağı Merkezi Referans Eşitlemesi'ne tıklayın ve aşağıdaki sırayla her akışın yanındaki üç nokta simgesini seçerek akışı açabilirsiniz. Akışı açma sırasında herhangi bir sorunla karşılaşırsanız bkz. Özelleştirme [adımları ve Sorun](connector-dynamics.md#customize-synchronization-steps) giderme [adımları.](connectors-troubleshoot.md)

Akışları aşağıdaki sırayla aç:

- İş Ortağı Merkezi Web Kancası Kaydı (Insider Önizlemesi)
- Ortak Satış Referansı Oluşturma – Dynamics 365 -İş Ortağı Merkezi (Insider Önizleme)
- [Özelleştirme] Dynamics 365 akışından Ayrıntıları Oluşturma veya Al
- İş Ortağı Merkezi dynamics 365 - Helper (Insider Preview)
- İş Ortağı Merkezi Microsoft'un Dynamics 365'e Ortak Satış Referans Güncelleştirmeleri (Insider Önizlemesi)
- İş Ortağı Merkezi Dynamics 365'e (Insider Önizleme)
- Dynamics 365 -İş Ortağı Merkezi (Insider Önizleme)
- Dynamics 365 Opportunity to İş Ortağı Merkezi (Insider Preview)
- Dynamics 365 Microsoft Solutions to İş Ortağı Merkezi (Insider Preview)
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Kaynak değişikliği olaylarını kaydetmek için web kancası API'lerini kullanma

Kaynak değişikliği olaylarını İş Ortağı Merkezi için web kancası API'lerini kullanabilirsiniz. Bu değişiklik olayları URL'nize HTTP gönderileri olarak gönderilir.

1. **Dynamics 365 İş Ortağı Merkezi (Insider Preview) öğesini seçin.**

1. Düzenle **simgesini seçin** ve HTTP **isteği geldiğinde seçeneğini seçin.**

1. Sağlanan  HTTP POST URL'sini kopyalamak için Kopyala simgesini seçin.

   :::image type="content" source="images/webhook-video.gif" alt-text="Kaynak değişikliklerini kaydetmek için web kancalarını kullanmayı gösteren ekran görüntüsü.":::

1. Web **Kancası İş Ortağı Merkezi (Insider Preview)** Power Automate'ı ve ardından Çalıştır'ı **seçin.**

1. Akışı çalıştır **penceresinin sağ** bölmede açıldığından emin olduktan sonra Devam'ı **seçin.**

1. Şu ayrıntıları girin:

   - **Http Tetikleyici Uç** Noktası: Bu URL önceki bir adımdan kopyalandı.
   - **Kaydedilebilecek Olaylar:** Tüm kullanılabilir olayları seçin (**referans oluşturuldu,** **referans güncelleştirildi,** **ilgili-referans oluşturuldu** ve **ilgili-referans-güncelleştirildi).**
   - **Mevcut tetikleyici uç noktalarının üzerine yaz?**: Evet. Bir web kancası olayı için yalnızca bir URL kaydedebilirsiniz.

1. Akışı **çalıştır'ı** ve ardından **Bitti'yi seçin.**

Web kancası artık olayları dinlemek, oluşturmak ve güncelleştirmek için kullanabilir.

## <a name="customize-synchronization-steps"></a>Eşitleme adımlarını özelleştirme

CRM sistemleri yüksek oranda özelleştirilmiştir ve CRM kurulum Power Automate özelleştirilebilir. Ortak satış referansları İş Ortağı Merkezi CRM sisteminiz arasında eşitlenmişse, İş Ortağı Merkezi pc'de eşitlenen alanlar Özel alan eşleme [kılavuzunda listelenir.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)

Alan eşleme kılavuzunu izleyin ve **gerekirse [Özelleştir] Dynamics 365** akışından veya ortam değişkenlerinden Ayrıntıları Al'da uygun değişiklikleri yapın. Gelecekteki çözüm yükseltmelerini etkileye Power Automate diğer akışları güncelleştirin.

Aşağıdaki özelleştirmeler kullanılabilir:

- **Fırsat adı içinde onay işaretini görüntüle:** Varsayılan olarak, İş Ortağı Merkezi ile Dynamics 365 CRM arasında eşitlemenin başarıyla devam ediyor olduğunu belirtmek için fırsat adının yanında bir onay işareti görüntülenir. Benzer şekilde, eşitleme başarısız olursa bir çapraz işaret görüntülenir. Fırsat adına bir onay veya çapraz işaret eklemekten kaçınmak için fırsat adı ortam değişkensinde Görünen onay işaretinin geçerli **değerini** Hayır olarak ayarlayın.
- **Satış anlaşması** değeri: Varsayılan olarak, İş Ortağı Merkezi CRM'de tahmini değer **ile** eşitlenir. CRM'de eşitlenen satış anlaşması değeri için farklı bir alanınız varsa:

  - Dynamics  365 ortam değişkeninin Satış değeri alan adını CRM'nin alan adıyla güncelleştirin. Alanın görünen adını değil, adının sağ olduğundan emin olun.
  - **Düzenle [Özelleştirme] Dynamics 365** akışından Ayrıntılar oluşturun  veya Alın ve CRM'de fırsat  oluşturma veya güncelleştirme'ye gidin ve Yeni fırsat oluştur ve Mevcut fırsat eylemlerini güncelleştir'i güncelleştirin ve **DealValue** değerini CRM'de doğru alana atacak şekilde güncelleştirin.  Ayrıca Tahmini Gelir **alanından DealValue** **atamayı kaldırın.**

- **Müşteri Hesabı Ülke Kodu:** Yeni bir referans sanız iki harfli ülke kodu (ISO 3166) sağlamak zorunludur. Varsayılan olarak, ülke kodu CRM'de hesabın address1_country **eşitler.** CRM'de ülke kodunun eşitley için farklı bir alanınız varsa:

  - Hesapta iki harfli kod içeren birarama dışı ülke kodu alanı için:
    - Dynamics 365 **ortam** değişkeninin Müşteri Hesabı Ülke Kodu alan adını CRM'nin alan adıyla güncelleştirin. Alanın görünen adını değil, adının sağ olduğundan emin olun.
    - Düzenle **[Özelleştirme] Dynamics 365** akışından Ayrıntılar oluşturun  veya Alın ve CRM'de doğru  alana ülke değeri atamak için CRM eylemde müşteri hesabı oluşturma veya al'a gidin. Ayrıca Adres  **1: Ülke/Bölge alanından Ülke değeri atamayı** kaldırın.

  - Hesapta arama tabanlı ülke kodu alanı için:
    - Hesaba yeni bir özel alan ekleyin ve arama tabanlı alanda seçilen değere göre (veya tam tersi) iki harfli ülke koduyla (ISO 3166) otomatik olarak doldurmak.
    - CRM'den yeni bir özel alanı şirket içi ve dışına eşitlemek için, sonraki adımları takip edin İş Ortağı Merkezi.

- **Fırsat alanları:** **Fırsat'ta** doldurulması gereken zorunlu alanlar varsa **[Özelleştirme] Dynamics 365** akışından Oluşturma  veya Ayrıntıları Al'a  gidin, CRM'de fırsat oluşturma veya güncelleştirme'ye gidin ve İş gereksinimlerinize göre zorunlu alanlara değer atamak için Yeni fırsat eylemi oluştur'a gidin.
- **Müşteri adayı** alanları: Müşteri adayı  alanında doldurulması gereken zorunlu alanlar varsa **[Özelleştirme] Dynamics 365**  akışından Oluşturma veya Ayrıntıları  Al'a gidin, CRM'de müşteri adayı oluşturma veya güncelleştirme'ye gidin ve İş gereksinimlerinize göre zorunlu alanlara değer atamak için Yeni müşteri adayı eylemi oluştur'a gidin.
- **Müşteri hesabı:** İş Ortağı Merkezi'den CRM'ye yeni bir referans eşitlen olduğunda, Power Automate çözümü müşteri şirket adını ve posta kodunu kullanarak CRM'de mevcut bir hesabı aramaya çalışır. Bir hesap bulamazsa CRM'de yeni bir müşteri hesabı oluşturulur. Arama ölçütlerini ve yeni hesap oluşturma ayrıntılarını güncelleştirmek için  **[Özelleştirme] Dynamics 365** akışından Ayrıntıları Oluştur veya Al'a gidin ve CRM'de müşteri hesabı oluşturma veya al ve Müşteri hesabı oluştur **eylemine gidin.**

## <a name="update-environment-variable"></a>Ortam değişkenlerini güncelleştirme

Ortam değişkeni değerini güncelleştirmek için:

1. Çözümler sayfasına **gidin ve** Varsayılan **Çözüm'i seçin.** Tüm **'i seçerek** Ortam Değişkeni'ne **seçin.**

1. Güncelleştirilmiş olması gereken değer için ortam değişkenlerini seçin ve üç **nokta** simgesini kullanarak Düzenle'yi seçin.

1. Yeni **değer seçeneğini** kullanarak ve değeri sağlayarak **Geçerli** Değeri güncelleştirin (Varsayılan **Değeri** güncelleştirin). Değerin değişkenin veri türüyle eşleşmesi gerekir. Örneğin, Evet veya Hayır veri türü Evet veya Hayır değerini kabul eder.

   :::image type="content" source="images/environment-variables-video.gif" alt-text="Ortam değişkenlerini güncelleştir'i gösteren ekran görüntüsü.":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>4-2 2 yönlü ortak satış referans eşitlemesi

Power Automate çözümünü yükledikten, yapılandırıp özelleştirdikten sonra Dynamics 365 ile İş Ortağı Merkezi arasında ortak satış referans eşitlemesini test İş Ortağı Merkezi.

### <a name="prerequisites"></a>Önkoşullar

İş Ortağı Merkezi dynamics 365 CRM'de referansları eşitlemek için, Power Automate microsoft'a özgü referans alanlarını açıkça sınırlar. Bu kimlik, satıcı ekiplerinize ortak satış için Microsoft ile hangi referansları paylaşmak istediğinize karar verme olanağı verir.

Çözüm yüklemesi kapsamında bir dizi özel alan ve nesne eklenecektir. CRM yönetici kullanıcısnın Fırsat özel alanlarıyla ayrı bir CRM **bölümü oluşturması** gerekir.

Aşağıdaki özel alanlar CRM bölümünün bir parçası olması gerekir:

- **İş Ortağı Merkezi ile eşitleme:** Fırsatın İş Ortağı Merkezi. Varsayılan olarak, bu alanın değeri Hayır'dır ve Satıcınız tarafından Microsoft ile bir fırsat paylaşmak için açıkça Evet olarak ayar yapılması gerekir. İş Ortağı Merkezi CRM'ye paylaşılan yeni referanslarda bu alan değeri Evet olarak ayarlanır.
- **Referans Tanımlayıcısı:** Referans başvurusu için salt İş Ortağı Merkezi alanı.
- **Referans Bağlantısı:** Referansta referansın salt okunur İş Ortağı Merkezi.
- **Microsoft nasıl yardımcı olabilir?**: Referans için Microsoft'tan yardım gerekir. Ortak satış referansı oluşturmak için Microsoft'tan gereken uygun yardımı seçin. Ortak satış referansı oluşturma fırsatıyla bir müşteri ilgili kişisi ilişkili olması gerekir. Ortak satış dışı bir referans oluşturmak için bu alanı seçmeyin. Ortak satış olmayan bir referans, uygun yardım gerekli seçeneği seçerek ortak satış referansı olarak dönüştürmek için kullanılabilir.
- **Microsoft İş Ortağı Merkezi Referans Görünürlüğü:** Referans için İş Ortağı Merkezi seçin. Bunu Microsoft satıcılarının kullanımına açık hale dönüştürerek ortak satış olmayan bir referans ortak satışa dönüştürülmüş olabilir. Microsoft yardımı gerektiğinde referans varsayılan olarak Microsoft satıcılarının kullanımına açıktır. Bu alan görünür olarak işaretlendikten sonra geri döndürülmeyebilir.
- **Microsoft CRM Tanımlayıcısı:** Ortak satış referansı oluşturulduğunda ve Microsoft tarafından kabul edilirken, bu alan Microsoft'un CRM tanımlayıcısıyla doldurulur.
- **Ürünler: Eski:** Bu alanı kullanma veya CRM bölümüne ekleme. Yalnızca geriye dönük uyumluluk için kullanılabilir. Bunun İş Ortağı Merkezi çözümlerini kullanın.
- **Denetim:** Referanslarla eşitlemek için salt okunur bir İş Ortağı Merkezi izi.
- **Microsoft İş Ortağı Merkezi Çözümleri:** Ortak satışa hazır çözümleri veya Microsoft çözümlerini fırsatla ilişkilendirmek için özel bir nesne. Fırsattan bir veya daha fazla çözüm eklenebilir veya kaldırılabilir. Microsoft ile paylaşmadan önce fırsata en az bir ortak satışa hazır veya Microsoft çözümü eklemek zorunludur. Bu nesneyi fırsatla ilişkilendirmek için **CRM'de Fırsat** formunu güncelleştirin.

  Fırsat formunda uygun **sekmeyi seçin** ve burada gösterildiği gibi bir alt ızgara ekleyin.

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Fırsat formunu gösteren ekran görüntüsü.":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Microsoft Solutions'u gösteren ekran görüntüsü.":::

- Microsoft çözümlerini ekledikten sonra ortak satışa hazır çözüm ayrıntılarını önceden doldurularak satış satıcılarının bunları eklemelerine gerek yok. Yeni bir çözüm ayrıntısı eklemek için CRM'de Microsoft  Çözüm Ayrıntıları nesnesine gidin ve Kayıt Ekle'yi seçerek tek bir giriş ekleyin veya Birden çok giriş eklemek için **Excel karşıya** yükleme'yi kullanın.

  :::image type="content" source="images/cosellconnectors/dynamics-solution-1.png" alt-text="Yeni Microsoft Çözümü Ayrıntılarını gösteren ekran görüntüsü.":::

### <a name="scenarios"></a>Senaryolar

1. Referans CRM'de oluşturulduğunda veya güncelleştirildiğinde ve referansta eşitlendi İş Ortağı Merkezi:

   1. CRM'nin Fırsat bölümünde görünürlüğü olan kullanıcıyla Dynamics 365 CRM **ortamında** oturum açma.

   1. Dynamics 365 İş Ortağı Merkezi yeni bir fırsat oluşturdukta **Microsoft** İş Ortağı Merkezi bölümünün mevcut olduğundan emin olmak.

      :::image type="content" source="images/cosellconnectors/dynamics-solution-2.png" alt-text="Yeni fırsat'ın ekran görüntüsü.":::

   1. Bu fırsatı İş Ortağı Merkezi eşitlemek için, kart görünümünde aşağıdaki alanları ayar

      - **Microsoft nasıl yardımcı olabilir?**: Ortak satış referansı oluşturmak için uygun bir yardım seçeneği belirleyin.

         :::image type="content" source="images/cosellconnectors/dynamics-solution-3.png" alt-text="Kart görünümünde uygun alanların nasıl alınacaklarını gösteren ekran görüntüsü.":::

      - **Müşteriyle** iletişim: Ortak satış referansı oluşturmak için fırsata bir müşteri ilgili kişisi ekleyin.
      - **Iş Ortağı Merkezi Ile Eşitle**: Evet.
      - **Microsoft çözümleri**: bir başvuruyu Microsoft ile paylaşmak için, fırsata geçerli bir ortak satış veya Microsoft çözümü ekleyin.

        :::image type="content" source="images/cosellconnectors/dynamics-solution-4.png" alt-text="Çözüm KIMLIĞINI gösteren ekran görüntüsü.":::

   1. İş **Ortağı Merkezi Ile Eşitle** seçeneği Evet olarak ayarlandığında Dynamics 365 ' de fırsat oluşturulduktan sonra 10 dakika bekleyin. Sonra Iş Ortağı Merkezi hesabınızda oturum açın. Başvurularınız, Dynamics 365 ve **başvuru tanımlayıcısıyla** eşitlenir. **Başvuru bağlantısı** doldurulacak. Bir hata oluşursa, **Denetim** alanı hata bilgileriyle doldurulur.

      1. Benzer şekilde, **Iş Ortağı Merkezi Ile Eşitle** seçeneği Evet olarak ayarlanmış bir fırsat Için, DYNAMICS 365 CRM 'de fırsatı güncelleştirirseniz değişiklikler Iş Ortağı Merkezi hesabınızda eşitlenir.

      1. Iş Ortağı Merkezi ile başarıyla eşitlenen fırsatlar, Dynamics 365 ' de ✔ simgesiyle tanımlanır.

1. Iş Ortağı Merkezi 'nde başvuru oluşturulduğunda veya güncelleştirilirken ve Dynamics 365 ortamında eşitlendiğinde başvuru eşitlemesi:

   1. Iş Ortağı Merkezi [panonuzda](https://partner.microsoft.com/dashboard/home)oturum açın.

   1. Sol menüden **referanslar** ' ı seçin.

   1. **Yeni anlaşma** seçeneğini belirleyerek Iş Ortağı Merkezi 'nden yeni bir ortak satış başvurusu oluşturun.

   1. Dynamics 365 CRM ortamınızda oturum açın.

   1. **Açık fırsatlara** gidin. Iş Ortağı Merkezi 'nde oluşturulan başvuru artık Dynamics 365 CRM 'de eşitlenir.

   1. Eşitlenmiş bir başvuruyu seçtiğinizde, kart Görünümü ayrıntıları doldurulur.

## <a name="next-steps"></a>Sonraki adımlar

- [Müşteri adaylarını yönetme](manage-leads.md)
- [Ortak satış fırsatlarını yönetme](manage-co-sell-opportunities.md)
- [Microsoft Power otomatikleştir platformu hakkında daha fazla bilgi](/power-automate/)
- [İş Ortağı Merkezi web kancaları](/partner-center/develop/partner-center-webhooks)
