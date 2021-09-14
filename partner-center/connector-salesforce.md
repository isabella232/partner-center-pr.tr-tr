---
title: Salesforce CRM için ortak satış bağlayıcısı İş Ortağı Merkezi
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: Şirket içinde referanslarınızı Salesforce CRM İş Ortağı Merkezi ile eşitler. Satış satıcıları daha sonra CRM sistemlerinizin içinde Microsoft ile ortak satışlar da kullanabilir.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 06/28/2021
ms.openlocfilehash: 4a98bd2e98aa1533806205179812af6507b2a2af
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248530"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Salesforce CRM için ortak satış bağlayıcısı - genel bakış

**Uygun roller:** Referans yöneticisi | CRM'de sistem yöneticisi veya sistem özelleştiricisi

İş Ortağı Merkezi ortak satış bağlayıcısı, satış satıcılarının CRM sistemlerinizin içinde Microsoft ile ortak satışlar oluşturmalarını sağlar. Ortak satış anlaşmalarını yönetmek için bu İş Ortağı Merkezi için eğitilmaları gerek olmayacaktır. Ortak satış bağlayıcılarını kullanarak, bir Microsoft satıcısıyla etkileşime geçen, Microsoft satıcısından referanslar almak, referansları kabul etmek/reddetmek, satış anlaşması değeri ve kapanış tarihi gibi satış verilerini değiştirmek için yeni bir Ortak satış referansı oluşturabilirsiniz.  Bu Ortak satış anlaşmaları hakkında Microsoft satıcılarından güncelleştirmeleri de edinirsiniz. Tüm referanslarınızı iş yerine kendi tercihli CRM'de çalışırken İş Ortağı Merkezi.

Çözüm, Microsoft Power Automate Çözümü'İş Ortağı Merkezi kullanır.

## <a name="before-you-install---pre-requisites"></a>Yüklemeden önce - önkullar

|**Konu başlıkları**|**Ayrıntılar**|**Bağlantılar**|
|--------------|--------------------|------|
|Microsoft İş Ortağı Ağı kimliği |Geçerli bir MPN kimliğine ihtiyacınız var|[MPN'ye katılmak için](https://partner.microsoft.com/)|
|Ortak satışa hazır|IP/Hizmetler çözümünüz ortak satışa hazır olmalı.|[Microsoft ile satış](https://partner.microsoft.com/membership/sell-with-microsoft)|
|İş Ortağı Merkezi hesabı|Kiracıyla ilişkilendirilmiş MPN İş Ortağı Merkezi Ortak satış çözümünüzle ilişkili MPN Kimliği ile aynı olması gerekir. Bağlayıcıları dağıtmadan önce ortak satış referanslarınızı İş Ortağı Merkezi portalında gördüğünüzü doğrulayın.|[Hesabınızı yönetme](create-user-accounts-and-set-permissions.md)|
|İş Ortağı Merkezi rollerini atama|Bağlayıcıları yükecek ve kullanacak olan çalışanın Referans yöneticisi olması gerekir|[Kullanıcı rollerini ve izinlerini atama](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|CRM kullanıcı rolü Sistem yöneticisi veya Sistem özelleştiricisi|[Salesforce CRM'de rol atama](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Power Automate Flow Hesabı|Test, hazırlama ve üretim için veritabanıyla yeni bir üretim ortamı oluşturun. Veritabanına sahip mevcut bir üretim ortamınız varsa bu ortam yeniden kullanılabilir. Bağlayıcı çözümünü yükleyen kullanıcının bu ortama Power Automate bir lisansa sahip olması gerekir. Yükleme başarısız olursa ilerleme durumunu izleyebilir ve Power Automate [daha](https://flow.microsoft.com/) fazla bilgi edinebilirsiniz. Çözümler **altında Geçmişi gör'i** **seçin.**|[Ortam oluşturma veya yönetme](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Microsoft Özel Alanları için Salesforce Paketini Yükleme

İş Ortağı Merkezi ve Salesforce CRM genelinde referansları eşitlemek için Power Automate çözümünün Microsoft'a özgü referans alanlarını net bir şekilde tanımlaması gerekir. Bu karar, iş ortağı satıcı ekiplerine ortak satış için Microsoft ile paylaşmak istediğiniz referansları verme olanağı sağlar.

1. Salesforce'ta **Notlar'ı** etkinleştirin ve fırsatlarla ilgili listeye ekleyin. [Başvuru](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

1. Aşağıdaki **adımları kullanarak** Fırsat ekiplerini etkinleştirin:
    - Kurulum'da Hızlı Bul **kutusunu kullanarak** Opportunity Team Ayarlar.
    - Ayarları gereken şekilde tanımlayın. [Başvuru](https://help.salesforce.com/articleView?id=sf.opp_team_manage.htm&type=5)

1. Salesforce'ta, paket yükleyicisini kullanarak özel alanlar ve [nesneler yükleyin.](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV) Paketi herhangi bir şirkete yüklemek için bu yükleyiciyi kullanın.

    >[!NOTE]
    >Korumalı alanı yüklüyorsanız URL'nin ilk bölümünü ile değiştirmeniz `http://test.salesforce.com` gerekir.

1. Salesforce'ta Microsoft Solutions'u **Fırsatla ilgili listesine** ekleyin. Eklendiktan sonra, İngiliz **anahtarı simgesini** seçin ve özellikleri güncelleştirin

## <a name="best-practice-test-before-you-go-live"></a>En İyi Yöntem: Canlı yayına başlamadan önce test

Üretim ortamında bir Power Automate çözümü yüklemeden, yapılandırmadan ve özelleştirmeden önce, çözümü hazırlama CRM örneğinde test etmek için emin olun.

- Hazırlama Power Automate/CRM örneğine Microsoft Power Automate çözümünü yükleyin.

- Çözümün bir kopyasını kopyalayın, yapılandırmanızı çalıştırın ve Power Automate akış özelleştirmelerini hazırlama ortamında çalıştırın.

- Çözümü hazırlama/CRM örneğinde test edin.

- Başarıyla, yönetilen bir çözüm olarak üretim örneğine içeri aktarın.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Salesforce CRM İş Ortağı Merkezi Referans Eşitlemesini Yükleme

1. Çalışma [Power Automate](https://flow.microsoft.com) sağ üst **köşedeki** Ortamlar'ı seçin. Bu size kullanılabilir CRM örneklerini gösterir.

1. Sağ üst köşedeki açılan listeden uygun CRM örneğini seçin.

1. Sol **gezinti** çubuğunda Çözümler'i seçin.

1. Üst **menüden AppSource'ı** Aç bağlantısını seçin.

   :::image type="content" source="images/cosellconnectors/open-appsource.png" alt-text="AppSource'i açın.":::

1. Açılan **İş Ortağı Merkezi Salesforce için Referans** Bağlayıcıları araması gerçekleştirin.  

   :::image type="content" source="images/salesforce/salesforce-get-it-now.png" alt-text="Şimdi Al'ın ekran görüntüsü.":::

1. Şimdi **al düğmesini ve** ardından Devam'ı **seçin.**

1. Sonraki sayfada, uygulamayı yüklemek için Salesforce CRM ortamını seçin. Hüküm ve koşulları kabul etmek.

1. Ardından Çözümlerinizi yönetme sayfasına **yönlendirildiniz.**  Sayfanın alt İş Ortağı Merkezi ok düğmelerini kullanarak "İş Ortağı Merkezi Referanslar" sayfasına gidin. **Zamanlanan yükleme,** Referanslar çözümünün İş Ortağı Merkezi görün gerekir. Yükleme 10-15 dakika sürer.

1. Yükleme tamamlandıktan sonra çalışma alanına geri [Power Automate](https://flow.microsoft.com) sol gezinti **alanında Çözümler'i** seçin. **Salesforce İş Ortağı Merkezi Referans Eşitlemesi'nin çözümler** listesinde kullanılabilir olduğunu fark edin.

1. **Salesforce İş Ortağı Merkezi Referans Eşitleme'yi seçin.** Aşağıdaki Power Automate akışlar ve varlıklar kullanılabilir:

   :::image type="content" source="images/cosellconnectors/partner-center-referrals-synchronization.png" alt-text="Salesforce akışları.":::

## <a name="configure-the-solution"></a>Çözümü yapılandırma

1. Çözümü CRM örneğine yükledikten sonra, [Power Automate.](https://flow.microsoft.com/)

1. Sağ **üst** köşedeki Ortamlar açılan listesinden, Power Automate çözümünü yüklemiş Power Automate seçin.

1. Üç kullanıcı hesabını ilişkilendirilen bağlantılar oluşturmanız gerekir:

   - İş Ortağı Merkezi yönetici kimlik bilgilerine sahip bir kullanıcı
   - İş Ortağı Merkezi Etkinlikleri
   - Çözümde akış Power Automate CRM yöneticisi

   1. Sol **gezinti** çubuğundan Bağlantılar'ı seçin ve **İş Ortağı Merkezi Referanslar** çözümünü seçin.

   1. Bağlantı oluştur'a **seçerek bağlantı oluşturun.**

        :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Bağlantı oluştur'a tıklayın.":::

   1. Sağ **İş Ortağı Merkezi arama çubuğunda Referanslar (önizleme)** araması gerçekleştirin.

   1. Referans yöneticisinin kimlik bilgileri İş Ortağı Merkezi kullanıcınız için bir bağlantı oluşturun.

   1. Ardından, Referanslar İş Ortağı Merkezi kimlik bilgileriyle İş Ortağı Merkezi kullanıcınız için bir Olay bağlantısı oluşturun.

   1. CRM yönetici kullanıcısı için Salesforce için bir bağlantı oluşturun.
  
   1. CRM yönetici kullanıcısı için Microsoft Dataverse bağlantısı oluşturun.

   1. Tüm Bağlantıları ekledikten sonra ortamınıza aşağıdaki bağlantıları görüyor gerekir:

        :::image type="content" source="images/cosellconnectors/salesforce-connections.png" alt-text="Bağlantıları gözlemleyi gösteren ekran görüntüsü.":::

### <a name="edit-the-connections"></a>Bağlantıları düzenleme

1. Çözümler sayfasına **geri dönüp** Varsayılan **Çözüm'i seçin.** Tüm **'e tıklayarak Bağlantı Başvurusu (önizleme)** **öğesini seçin.**

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Bağlantıları düzenlemeyi gösteren ekran görüntüsü.":::

1. Üç nokta simgesini seçerek Bağlantılar'ın her bir öğesini tek tek düzenleyin. İlgili bağlantıları ekleyin.

   :::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Bağlayıcıları düzenlemeyi gösteren atht'nin ekran görüntüsü.":::

1. Akışları aşağıdaki sırayla aç:
   - İş Ortağı Merkezi Web Kancası Kaydı (Insider Önizlemesi)
   - [Özelleştirme] Salesforce'tan Ayrıntılar Oluşturma veya Ayrıntıları Al
   - İş Ortağı Merkezi için ortak Referral-Salesforce oluşturma (Insider Önizleme)
   - İş Ortağı Merkezi Microsoft Ortak Satış Referans Güncelleştirmelerini Salesforce'a (Insider Önizleme) yükleme  
   - İş Ortağı Merkezi'a (Insider Önizleme)
   - Salesforce'tan İş Ortağı Merkezi 'a (Insider Önizleme)
   - Salesforce Opportunity to İş Ortağı Merkezi (Insider Preview)
   - İş Ortağı Merkezi için Salesforce Microsoft Solutions (Insider Önizleme)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Kaynak değişikliği olaylarını kaydetmek için Web Kancası API'lerini kullanma

Kaynak değişikliği olaylarını İş Ortağı Merkezi için web kancası API'lerini kullanabilirsiniz. Bu değişiklik olayları URL'nize HTTP gönderileri olarak gönderilir.

1. **Salesforce CRM İş Ortağı Merkezi (Insider Preview) seçeneğini kullanın.**

1. Düzenle simgesini **seçin ve** Bir HTTP **isteği geldiğinde'yi seçin.**

1. Sağlanan  HTTP POST URL'sini kopyalamak için **Kopyala simgesini seçin.**

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="URL'yi kopyalamayı gösteren ekran görüntüsü.":::

1. Web **kancası İş Ortağı Merkezi (Insider Preview)** Power Automate çalıştır'ı **seçin.**

1. Akışı çalıştır **penceresinin sağ** bölmede açıldığından emin olduktan sonra Devam'ı **seçin.**

1. Şu ayrıntıları girin:

   - **Http Tetikleyici Uç** Noktası: Bu URL önceki bir adımdan kopyalandı.
   - **Kaydedilebilecek Olaylar:** Tüm kullanılabilir olayları seçin (**referans oluşturuldu,** **referans güncelleştirildi,** **ilgili-referans oluşturuldu** ve **ilgili-referans-güncelleştirildi).**
   - **Mevcut tetikleyici uç noktalarının üzerine yaz?**: Evet. Bir web kancası olayı için yalnızca bir URL kaydedebilirsiniz.

1. Akışı **çalıştır'ı** ve ardından **Bitti'yi seçin.**

Web kancası artık olayları dinlemek, oluşturmak ve güncelleştirmek için kullanabilir.

## <a name="customize-synchronization-steps"></a>Eşitleme adımlarını özelleştirme

CRM sistemleri yüksek oranda özelleştirilmiştir ve CRM kurulum Power Automate özelleştirilebilir. Ortak satış referansları İş Ortağı Merkezi CRM sisteminiz arasında eşitlenmişse, İş Ortağı Merkezi pc'de eşitlenen alanlar Özel alan eşleme [kılavuzunda listelenir.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)

Alan eşleme kılavuzunu izleyin ve **gerekirse [Özelleştir] Salesforce** veya ortam değişkenlerinden Ayrıntılar Oluşturma veya Ayrıntıları Al içinde uygun değişiklikleri yapın. Gelecekteki çözüm yükseltmelerini etkileye Power Automate diğer akışları güncelleştirin.

Aşağıdaki özelleştirmeler kullanılabilir:

- **Fırsat adı içinde onay işaretini görüntüle:** Varsayılan olarak, İş Ortağı Merkezi ve Salesforce CRM arasındaki eşitlemenin başarılı olduğunu belirtmek için fırsat adının yanında bir onay işareti görüntülenir. Benzer şekilde, eşitleme başarısız olursa bir çapraz işaret görüntülenir. Fırsat adına onay veya çapraz işaret eklemekten kaçınmak için fırsat adı ortam değişkensinde Görünen onay işaretinin geçerli **değerini** Hayır olarak ayarlayın.

- **Aşama adı:**

  - **Etkin aşama adı:** Salesforce'ta bir fırsatın satış işlem hattında yer alan aşamadır.  Etkin bir aşamayı temsil eder ve kabul edilen durumdaki bir referansla eşdeğerdir ve İş Ortağı Merkezi. Bu, satış işlem hattında, tutma aşamasından sonraki aşama olabilir. Opportunity'in satış aşamasının etkin aşamaya taşınması, referansta referansı kabul eder İş Ortağı Merkezi değişiklikler eşitlenmeye başlar.

  - **Tutma aşaması adı:** Salesforce'ta bir fırsatın satış işlem hattında yer alan aşamanın adı. Bir tutma aşamayı temsil eder. Microsoft'tan paylaşılan ve henüz kabul edilmemiş olan yeni ortak satış referansları Salesforce'ta bu aşamaya ayarlanır. Bir fırsatta, tutma aşamasında yapılan tüm değişiklikler, bir fırsatta yapılan tüm değişiklikler İş Ortağı Merkezi. Opportunity'in satış aşamalarının bu tutma aşamasından dışarı taşınması, referansta referansı kabul İş Ortağı Merkezi değişiklikler eşitlenmeye başlar.

- **Müşteri Hesabı Ülke Kodu:** Yeni bir referans sanız iki harfli ülke kodu (ISO 3166) sağlamak zorunludur. Varsayılan olarak ülke kodu, hesabın Salesforce'daki **BillingCountry** alanına ve bu alandan eşitler. Salesforce'ta eşitlenen ülke kodu için farklı bir alanı varsa:

  - Hesapta iki harfli kod içeren birarama dışı ülke kodu alanı için:

    - Salesforce **ortam değişkensinde** Müşteri Hesabı Ülke Kodu alan adını CRM'nin alan adıyla güncelleştirin. Alanın görünen adını değil, adının sağ olduğundan emin olun.

    - **[Özelleştirme] Salesforce'tan** Ayrıntıları Oluştur veya Al'a gidin ve **CRM'de** doğru alana ülke değeri atamak için CRM eylemde müşteri hesabı oluşturma veya al'a gidin.  Ayrıca, BillingCountry'den  Ülke değeri **atamayı kaldırın.**

  - Hesapta arama tabanlı ülke kodu alanı için:

    - Hesaba yeni bir özel alan ekleyin ve arama tabanlı alanda seçilen değere göre (veya tam tersi) iki harfli ülke koduyla (ISO 3166) otomatik olarak doldurmak.

    - CRM'den yeni bir özel alanı şirket içi ve dışına eşitlemek için, sonraki adımları takip edin ve bu alandan İş Ortağı Merkezi.

- **Satış anlaşması** değeri: Varsayılan olarak, İş Ortağı Merkezi crm'de Tutar ile  eşitlenir. CRM'de eşitlenecek satış anlaşması değeri için farklı bir alanınız varsa:

  - Salesforce **ortam değişkeninin** Satış değeri alanı adını CRM'nin alan adıyla güncelleştirin. Alanın görünen adını değil, adının sağ olduğundan emin olun.

  - Düzenle **[Özelleştirme] Salesforce'tan** Ayrıntılar oluşturun  veya Alın ve CRM'de fırsat oluşturma  veya güncelleştirme'ye gidin ve Hem Yeni fırsat oluştur hem de Mevcut fırsat eylemlerini **güncelleştir'i Güncelleştir'i** Güncelleştir'i Salesforce'ta doğru alana atamak için güncelleştirin. 

- **Satış anlaşması değeri para birimi** kodu: Salesforce'ta satış anlaşması değeri para birimi kodu alanı adı. Bu alan API'si adı, Microsoft İş Ortağı Merkezi'da referans oluşturulurken veya güncelleştirilerek Fırsat'ın satış anlaşması değeri para birimi kodunu almak için İş Ortağı Merkezi. Satış anlaşması değeri para birimi kodu alanı **currencyIsoCode** varsayılan alanından farklı ise, bu ortam değişkeninin geçerli değerini güncelleştirin.

  - Salesforce **ortam değişkeninin** Satış değeri para birimi alan adını CRM'nin alan adıyla güncelleştirin. Alanın görünen adını değil, adının sağ olduğundan emin olun.

  - Düzenle **[Özelleştirme] Salesforce'tan** Ayrıntılar oluşturun  veya Alın ve CRM'de fırsat oluşturma  veya güncelleştirme'ye gidin ve Hem Yeni fırsat oluştur hem de Mevcut fırsat eylemlerini güncelleştir'i güncelleştirin ve **DealValueCurrency'yi** Salesforce'ta doğru alana at uygun alana at uygun şekilde güncelleştirin. 

- **Ortak satış fırsatı eşitleme:** Evet olarak **ayarlanırsa,** yalnızca ortak satış ve işlem hattı paylaşım fırsatları İş Ortağı Merkezi Salesforce'a eşitlenir. Hayır olarak **ayarlanırsa** müşteri adayları, ortak satış ve işlem hattı paylaşım fırsatları İş Ortağı Merkezi Salesforce'a eşitlenir. Bu değişkenin Salesforce'tan İş Ortağı Merkezi'a eşitlenen fırsatlar üzerinde hiçbir etkisi İş Ortağı Merkezi.

## <a name="update-environment-variable"></a>Ortam değişkenlerini güncelleştirme

Ortam değişkeni değerini güncelleştirmek için:

1. Çözümler sayfasına **gidin ve** Varsayılan **Çözüm'i seçin.** Tüm **'i seçerek** Ortam Değişkeni'ne **seçin.**

1. Güncelleştirilmiş olması gereken değer için ortam değişkenlerini seçin ve üç **nokta** simgesini kullanarak Düzenle'yi seçin.

1. Yeni **değer seçeneğini** kullanarak ve değeri sağlayarak **Geçerli** Değeri güncelleştirin (Varsayılan **Değeri** güncelleştirin). Değerin değişkenin veri türüyle eşleşmesi gerekir. Örneğin, Evet veya Hayır veri türü Evet veya Hayır değerini kabul eder.

   :::image type="content" source="images/cosellconnectors/environment-variables-video.gif" alt-text="Ortam değişkenlerini güncelleştir'i gösteren ekran görüntüsü.":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>4- uç çift yönlü ortak satış referans eşitlemesi

Power Automate çözümünü yükledikten, yapılandırıp özelleştirdikten sonra Salesforce CRM ile İş Ortağı Merkezi arasında ortak satış referans eşitlemesi için test İş Ortağı Merkezi.

### <a name="pre-requisites"></a>Ön koşullar

İş Ortağı Merkezi ve Salesforce CRM'de referansları eşitlemek için Power Automate çözümünün Microsoft'a özgü referans alanlarını net bir şekilde geri yüklemesi gerekir. Bu kimlik, satış ekibinize ortak satış için Microsoft ile paylaşmak istediğiniz referansları belirleme olanağı sağlar.

Salesforce CRM çözümü Fırsat varlığı için Referans eşitleme İş Ortağı Merkezi bir dizi özel **alan** mevcuttur. CRM yönetici kullanıcısnın Fırsat özel alanlarıyla ayrı bir CRM **bölümü** oluşturması gerekir.

Aşağıdaki özel alanlar CRM bölümünün bir parçası olması gerekir:

- **İş Ortağı Merkezi ile eşitleme:** Fırsatın İş Ortağı Merkezi. Varsayılan olarak, bu alanın değeri Hayır'dır ve Satıcınız tarafından Microsoft ile bir fırsat paylaşmak için açıkça Evet olarak ayar yapılması gerekir. İş Ortağı Merkezi CRM'e paylaşılan yeni referanslarda bu alan değeri Evet olarak ayarlanır.

- **Referans Tanımlayıcısı:** Microsoft'un referans için salt İş Ortağı Merkezi alanı.

- **Referans Bağlantısı:** Microsoft İş Ortağı Merkezi'de referansın salt okunur bağlantısı.

- **Microsoft nasıl yardımcı olabilir:** Referans için Microsoft'tan gereken yardım. Ortak satış referansı oluşturmak için Microsoft'tan gereken uygun yardımı seçin. Ortak satış referansı oluşturma fırsatıyla bir müşteri ilgili kişisi ilişkili olması gerekir. Ortak satış dışı bir referans oluşturmak için bu alanı seçmeyin. Ortak satış olmayan bir referans, uygun yardım gerekli seçeneği seçerek ortak satış referansı olarak dönüştürmek için kullanılabilir.

- **Microsoft İş Ortağı Merkezi Referans Görünürlüğü:** Referans için İş Ortağı Merkezi seçin. Ortak satış olmayan bir başvuru, Microsoft satıcıları için görünür hale getirerek ortak satış olarak dönüştürülebilir. Microsoft Yardım gerektiğinde, başvuru varsayılan olarak Microsoft satıcılarıyla görülebilir. Bu alan görünür olarak işaretlendikten sonra geri döndürülemez.

- **Microsoft CRM tanımlayıcı**: microsoft tarafından bir ortak satış başvurusu oluşturulup kabul edildiğinde, bu alan microsoft 'un CRM tanımlayıcısı ile doldurulur.

- **Microsoft Iş ortağı merkezi çözümleri**: ortak satış için hazırlanma çözümlerini veya Microsoft çözümlerini fırsatla ilişkilendirmek için özel bir nesne. Fırsatta bir veya daha fazla çözüm eklenebilir veya kaldırılabilir. Microsoft ile paylaşmadan önce fırsata en az bir ortak satış veya Microsoft çözümü eklemek zorunludur. Bu nesneyi fırsatla ilişkilendirmek için CRM 'de **fırsat** formunu güncelleştirin.

- **Denetim**: Iş Ortağı Merkezi başvurularına eşitleme için salt okunurdur bir denetim izi

### <a name="scenarios"></a>LARLA

1. CRM 'de başvuru oluşturulduğunda veya güncelleştirilirken ve Iş Ortağı Merkezi 'nde eşitlendiğinde başvuru eşitlemesi:

   1. CRM 'nin **fırsat** bölümünde görünürlük olan KULLANıCıYLA Salesforce CRM ortamınızda oturum açın.

   1. Salesforce CRM ortamında **Yeni bir fırsat** oluşturduğunuzda **Microsoft iş ortağı merkezi** 'nin mevcut olduğundan emin olun.

   1. Iş Ortağı Merkezi ile başarıyla eşitlenen fırsatlar, Salesforce CRM 'de ✔ simgesiyle tanımlanır.
      :::image type="content" source="images/salesforce/salesforce-environment.png" alt-text="Salesforce ortamının ekran görüntüsü.":::

   1. Bu fırsatı Microsoft Iş Ortağı Merkezi ile eşleştirmek için, kart görünümünde aşağıdaki alanları ayarlamış olduğunuzdan emin olun:

      - **Microsoft nasıl yardım edebilir?**: ortak satış başvurusu oluşturmak için uygun bir yardım seçeneği belirleyin.

        :::image type="content" source="images/salesforce/salesforce-help-option.png" alt-text="Kart görünümünde uygun alanların nasıl alınacağını gösteren ekran görüntüsü.":::

      - **Iş Ortağı Merkezi Ile Eşitle**: Evet
      - **Müşteri iletişim**: ortak satış başvurusu oluşturmak için, fırsata bir müşteri kişisi ekleyin.
      - **Microsoft çözümleri**: bir başvuruyu Microsoft ile paylaşmak için, fırsata geçerli bir ortak satış veya Microsoft çözümü ekleyin.

   1. **Iş Ortağı Merkezi ile fırsat eşitlemesi** seçeneğini **Evet** olarak ayarladıktan sonra, 10 dakika bekleyin, iş ortağı Merkezi hesabınızda oturum açın. Başvurularınız Salesforce CRM ile eşitlenecek ve başvuru bağlantısı doldurulacak. Bir hata oluşursa, denetim alanı hata bilgileriyle doldurulur.

   1. Benzer şekilde, **Iş Ortağı Merkezi Ile Eşitle** seçeneği **Evet** olarak AYARLANDıĞıNDA, fırsatı Salesforce CRM 'de güncelleştirirseniz değişiklikler iş ortağı merkezi hesabınızla eşitlenir.

2. Microsoft Iş Ortağı Merkezi 'nde başvuru oluşturulduğunda veya güncelleştirilirken ve Salesforce CRM ortamında eşitlendiğinde başvuru eşitlemesi:

    1. Iş Ortağı Merkezi [panonuzda](https://partner.microsoft.com/dashboard/home)oturum açın.

    1. Sol taraftaki menüden **referanslar** ' ı seçin.

    1. "Yeni anlaşma" seçeneğine tıklayarak Iş Ortağı Merkezi 'nden yeni bir ortak satış başvurusu oluşturun.

    1. Salesforce CRM ortamınızda oturum açın.

    1. **Açık fırsatlara** gidin. Microsoft Iş Ortağı Merkezi 'nde oluşturulan başvuru artık Salesforce CRM 'de eşitlendi.

    1. Eşitlenmiş bir başvuruyu seçtiğinizde, kart Görünümü ayrıntıları doldurulur.

       :::image type="content" source="images/salesforce/salesforce-casino.png" alt-text="Salesforce fırsat sayfasının ekran görüntüsü.":::

>[!NOTE]
>**Dağıtım ile ilgili yardıma mı ihtiyacınız var?**
>Ortak satış referans bağlayıcı dağıtımınız hakkında yardım almak için Iş ortağı teknik danışmanına sahip olabilirsiniz. Dağıtım yardımı ve başarılı bir uygulama için en iyi uygulamalar sağlayabilir.
>
>Daha fazla bilgi için bkz. [Teknik satış öncesi ve Dağıtım Hizmetleri Isteği gönderme](technical-benefits.md)

## <a name="next-steps"></a>Sonraki adımlar

- [Müşteri adaylarını yönetme](manage-leads.md)

- [Ortak satış fırsatlarını yönetme](manage-co-sell-opportunities.md)

- [İş Ortağı Merkezi web kancaları](/partner-center/develop/partner-center-webhooks)
