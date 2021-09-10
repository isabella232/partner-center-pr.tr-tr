---
title: Salesforce CRM için ortak satış bağlayıcısı İş Ortağı Merkezi
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: Şirket içinde referanslarınızı Salesforce CRM İş Ortağı Merkezi ile eşitler. Bundan sonra satış satıcıları CRM sistemlerinizin içinde Microsoft ile ortak satışlar da kullanabilir.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 06/28/2021
ms.openlocfilehash: 4a98bd2e98aa1533806205179812af6507b2a2af
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960334"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Salesforce CRM için ortak satış bağlayıcısı - genel bakış

**Uygun roller:** Referans yöneticisi | CRM'de sistem yöneticisi veya sistem özelleştiricisi

İş Ortağı Merkezi ortak satış bağlayıcısı, satış satıcılarının CRM sistemlerinizin içinde Microsoft ile ortak satışlar oluşturmalarını sağlar. Ortak satış anlaşmalarını yönetmek için İş Ortağı Merkezi kullanmak üzere eğitilmaları gerek olmayacaktır. Ortak satış bağlayıcılarını kullanarak, bir Microsoft satıcısıyla etkileşime geçen, Microsoft satıcısından referanslar almak, referansları kabul etmek/reddetmek, satış anlaşması değeri ve kapanış tarihi gibi satış verilerini değiştirmek için yeni bir Ortak satış referansı oluşturabilirsiniz.  Bu Ortak satış anlaşmaları hakkında Microsoft satıcılarından güncelleştirmeleri de edinirsiniz. Tüm referanslarınızı iş yerine kendi tercihli CRM'de çalışırken İş Ortağı Merkezi.

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

İş Ortağı Merkezi ve Salesforce CRM'de referansları eşitlemek için Power Automate çözümünün Microsoft'a özgü referans alanlarını net bir şekilde tanımlaması gerekir. Bu karar, iş ortağı satıcı ekiplerine ortak satış için Microsoft ile paylaşmak istediğiniz referansları verme olanağı sağlar.

1. Salesforce'ta **Notlar'ı** etkinleştirin ve fırsatlarla ilgili listeye ekleyin. [Başvuru](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

1. Aşağıdaki **adımları kullanarak** Fırsat ekiplerini etkinleştirin:
    - Kurulum'da Hızlı Bul **kutusunu kullanarak** Opportunity Team Ayarlar.
    - Ayarları gereken şekilde tanımlayın. [Başvuru](https://help.salesforce.com/articleView?id=sf.opp_team_manage.htm&type=5)

1. Salesforce'ta, paket yükleyicisini kullanarak özel alanlar ve [nesneler yükleyin.](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV) Paketi herhangi bir şirkete yüklemek için bu yükleyiciyi kullanın.

    >[!NOTE]
    >Korumalı alanı yüklüyorsanız URL'nin ilk bölümünü ile değiştirmeniz `http://test.salesforce.com` gerekir.

1. Salesforce'ta Microsoft Solutions'u **Fırsatla ilgili listesine** ekleyin. Eklendiktan sonra, İngiliz anahtarı **simgesini** seçin ve özellikleri güncelleştirin

## <a name="best-practice-test-before-you-go-live"></a>En İyi Yöntem: Canlı yayına başlamadan önce test

Üretim ortamında bir çözüm yüklemeden, Power Automate ve özelleştirmeden önce, çözümü hazırlama CRM örneğinde test etmek için emin olun.

- Hazırlama Power Automate/CRM örneğine Microsoft Power Automate çözümünü yükleyin.

- Çözümün bir kopyasını kopyalayın, yapılandırmanızı çalıştırın ve Power Automate akış özelleştirmelerini hazırlama ortamında çalıştırın.

- Çözümü hazırlama/CRM örneğinde test edin.

- Başarıyla, yönetilen bir çözüm olarak üretim örneğine aktarın.

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

1. Ardından Çözümlerinizi yönetme sayfasına **yönlendirildiniz.**  Sayfanın alt İş Ortağı Merkezi ok düğmelerini kullanarak "İş Ortağı Merkezi Referanslar" sayfasına gidin. **Zamanlanan yükleme,** Referanslar çözümünün İş Ortağı Merkezi görüntü gerekir. Yükleme 10-15 dakika sürer.

1. Yükleme tamamlandıktan sonra çalışma alanına geri Power Automate [sol](https://flow.microsoft.com) gezinti **alanında Çözümler'i** seçin. **Salesforce İş Ortağı Merkezi Referans Eşitlemesi'nin çözümler** listesinde kullanılabilir olduğunu fark edin.

1. **Salesforce İş Ortağı Merkezi Referans Eşitleme'yi seçin.** Aşağıdaki Power Automate ve varlıklar kullanılabilir:

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

        :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Bağlantı oluştur'ları gösteren ekran görüntüsü.":::

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

1. Üç nokta simgesini seçerek her bir bağlantıyı tek tek düzenleyin. İlgili bağlantıları ekleyin.

   :::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Ekran görüntüsü atht bağlayıcıları nasıl düzenleyileceğini gösterir.":::

1. Akışları aşağıdaki sırada açın:
   - İş Ortağı Merkezi Web kancası kaydı (Insider Preview)
   - Kişiselleştirin Salesforce ile ayrıntılar oluşturun veya alın
   - Iş Ortağı Merkezi 'ne ortak satış Referral-Salesforce oluşturma (Insider Preview)
   - İş Ortağı Merkezi Microsoft ortak-başvuru güncelleştirmelerini Salesforce 'a satma (Insider Preview)  
   - İş ortağı merkezini Salesforce 'a (Insider Preview)
   - Salesforce-Iş Ortağı Merkezi (Insider Preview)
   - Salesforce Iş Ortağı Merkezi (Insider Preview)
   - Salesforce Microsoft çözümlerini Iş Ortağı Merkezi 'ne (Insider Preview)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Kaynak değişikliği olaylarına kaydolmak için Web kancası API 'Lerini kullanma

Kaynak değiştirme olaylarına kaydolmak için Iş Ortağı Merkezi Web kancası API 'Lerini kullanabilirsiniz. Bu değişiklik olayları, URL 'nize HTTP gönderileri olarak gönderilir.

1. **Iş ortağı merkezini SALESFORCE CRM 'ye (Insider Preview)** seçin.

1. **Düzenle simgesini** seçin ve **bir http isteği alındığında** öğesini seçin.

1. Belirtilen **http post URL 'sini** kopyalamak için **Kopyala** simgesini seçin.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="URL 'nin nasıl kopyalanacağını gösteren ekran görüntüsü.":::

1. **iş ortağı merkezi web kancası kaydı (ınsider preview)** Power Automate akışı ' nı seçin ve ardından **çalıştır**' ı seçin.

1. **Akış Çalıştır** penceresinin sağ bölmede açıldığından emin olun ve **devam**' ı seçin.

1. Şu ayrıntıları girin:

   - **Http tetikleyici uç noktası**: Bu URL önceki bir adımdan kopyalanmış.
   - **Kaydolmak Için olaylar**: kullanılabilir tüm olayları (**başvuru-oluşturulan**, **başvuru-güncelleştirilmiş**, **ilişkili-başvuru-oluşturma** ve **ilgili-başvuru-güncelleştirilmiş**) seçin.
   - Varsa **var olan tetikleyici uç noktalarının üzerine yaz**: Evet. Belirli bir Web kancası olayı için yalnızca bir URL kaydedilebilir.

1. **Akış Çalıştır**' ı seçin ve **bitti**' yi seçin.

Web kancası artık olayları dinleyebilir, oluşturabilir ve güncelleştirebilir.

## <a name="customize-synchronization-steps"></a>Eşitleme adımlarını özelleştirme

crm sistemleri büyük ölçüde özelleştirilir ve Power Automate çözümünü, crm kurulumunuzu temel alarak özelleştirebilirsiniz. Ortak satış başvuruları Iş ortağı merkezi ve CRM sisteminiz arasında eşitlendiğinde, Iş Ortağı Merkezi BILGISAYAR üzerinde eşitlenen alanlar [özel alan eşleme kılavuzunda](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)listelenir.

Alan eşleme kılavuzunu izleyin ve gerekirse, [özelleştirme] içinde uygun değişiklikleri yapın Salesforce veya ortam değişkenlerinden **Ayrıntılar oluşturun veya alın** . gelecekteki çözüm yükseltmelerini etkileyebileceğinden Power Automate çözümdeki diğer akışları güncelleştirmeyin.

Aşağıdaki özelleştirmeler kullanılabilir:

- **Fırsat adında onay Işareti göster**: varsayılan olarak, Iş ortağı merkezi ve Salesforce CRM arasındaki eşitlemenin başarıyla gerçekleştiği anlamına gelen fırsat adının yanında bir onay işareti görüntülenir. Benzer şekilde, eşitleme başarısız olursa bir çapraz işaret görüntülenir. Fırsat adına bir denetim veya çapraz işaret eklemekten kaçınmak için, **fırsat adı ortam değişkeninde görünen onay işaretinin** geçerli değerini Hayır olarak ayarlayın.

- **Aşama adı**:

  - **Etkin aşama adı**: Bu, fırsatın Salesforce 'taki satış işlem hattının aşamasıdır.  Etkin bir aşamayı temsil eder ve Iş Ortağı Merkezi 'nde kabul edilen durumdaki bir başvuruya eşdeğerdir. Bu işlem, satış işlem hattının bir sonraki aşaması ile, bekletme aşamasından sonra olabilir. Fırsatın satış aşamasını, bekletme aşamasından etkin aşamasına taşımak, Iş Ortağı Merkezi 'ndeki başvuruyu kabul eder ve değişiklikler eşitlemeye başlar.

  - **Tutan aşama adı**: bir fırsatın Salesforce 'daki satış Işlem hattındaki aşamasının adı. Bir açık bekleme aşamasını temsil eder. Henüz kabul edilmeyen Microsoft 'tan paylaşılan yeni ortak satış başvuruları, Salesforce 'ta bu aşamaya ayarlanır. Bir fırsatta yapılan herhangi bir değişiklik, bir bekleme aşamasıdır ve Iş Ortağı Merkezi ile eşitlenmez. Fırsatın satış aşamasını bu açık bekleme aşamasından çıkarmak, Iş Ortağı Merkezi 'ndeki başvuruyu kabul eder ve değişiklikler eşitlemeye başlar.

- **Müşteri hesabı ülke kodu**: yeni bir başvuru oluştururken iki harfli bir ülke kodu (ISO 3166) sağlamak zorunludur. Varsayılan olarak, ülke kodu Salesforce 'daki firmanın **bilme ülkesi** alanından ve bu alandan eşitlenir. Salesforce 'ta eşitlenecek ülke kodunun farklı bir alanına sahipseniz:

  - Hesapta iki harfli bir kod içeren arama olmayan ülke kodu alanı için:

    - Salesforce ortam değişkenindeki **müşteri hesabı ülke kodu** alan adını, CRM 'nin alan adıyla güncelleştirin. Alanın adını, görünen adını değil, sağladığınızdan emin olun.

    - Düzenle **[özelleştirme] Salesforce 'Tan ayrıntılar oluşturun veya alın** ve CRM 'de doğru alana bir **ülke** değeri atamak için **CRM 'de müşteri hesabı oluştur veya Al** ' a gidin. Ayrıca, **Billingcountry**'den **ülke** değeri atamasını kaldırın.

  - Hesaptaki arama temelli bir ülke kodu alanı için:

    - Hesaba yeni bir özel alan ekleyin ve arama tabanlı alanda seçilen değere göre iki harfli bir ülke kodu (ISO 3166) ile otomatik olarak doldurun ve tam tersi de geçerlidir.

    - Yeni bir özel alanı CRM 'den ve Iş Ortağı Merkezi 'nden eşitlemek için, arama dışı ülke kodu alanına yönelik önceki adımları izleyin.

- **Anlaşma değeri**: varsayılan olarak, Iş Ortağı Merkezi ' nden anlaşma DEĞERI, CRM 'deki tutardan ve bu **miktardan** eşitlenecek. CRM 'de eşitlenmek üzere anlaşma değeri için farklı bir alanınız varsa:

  - Salesforce ortam değişkeninde, CRM 'nin alan adı ile **işlem değeri** alan adını güncelleştirin. Alanın adını, görünen adını değil, sağladığınızdan emin olun.

  - Düzenle **[özelleştirme] Salesforce 'Tan ayrıntılar oluşturun veya** GÜNCELLEŞTIRIN ve CRM 'de **fırsat oluştur veya Güncelleştir** ' e gidin ve her ikisi de **Yeni bir fırsat oluşturun** ve **Mevcut fırsat eylemlerini güncelleştirin** . 

- **Anlaşma değeri para birimi kodu**: Salesforce 'daki anlaşma değeri para birimi kodu alanının adı. Bu alan API adı, Microsoft Iş Ortağı Merkezi 'nde başvuru oluştururken veya güncelleştirirken fırsatın anlaşma değeri para birimi kodunu almak için kullanılacaktır. Anlaşma değeri para birimi kodu alanı varsayılan alan **CurrencyIsoCode** değerinden farklıysa, bu ortam değişkeninin geçerli değerini güncelleştirin.

  - Salesforce ortam değişkeninde, CRM 'nin alan adı ile **işlem değeri para birimi** alan adını güncelleştirin. Alanın adını, görünen adını değil, sağladığınızdan emin olun.

  - Düzenle **[özelleştirme] Salesforce 'Tan ayrıntılar oluşturun veya** GÜNCELLEŞTIRIN ve CRM 'de **fırsat oluştur veya Güncelleştir** ' e gidin ve **güncelleştirme, her** ikisi de **Yeni bir fırsat oluştur** ve **var olan fırsatı Güncelleştir** eylemlerini Salesforce 'daki doğru alana atamak için güncelleştirin.

- **Ortak satış fırsatlarını Eşitle**: **Evet** olarak ayarlanırsa, iş ortağı merkezinden Salesforce 'a yalnızca ortak satış ve işlem hattı paylaşma olanakları eşitlenir. **Hayır** olarak ayarlanırsa, müşteri adayları, ortak satış ve işlem hattı paylaşma fırsatları Iş Ortağı Merkezi 'nden Salesforce 'a eşitlenir. Bu değişkenin Salesforce 'tan Iş Ortağı Merkezi 'ne eşitlenen fırsatları üzerinde hiçbir etkisi yoktur.

## <a name="update-environment-variable"></a>Ortam değişkenini Güncelleştir

Bir ortam değişken değerini güncelleştirmek için:

1. **Çözümler** sayfasına gidin ve **Varsayılan çözüm**' ı seçin. **Tümü**' nü seçerek **ortam değişkenini** seçin.

1. Güncelleştirilmesi gereken değer için ortam değişkenini seçin ve üç nokta simgesini kullanarak **Düzenle** ' yi seçin.

1. **Yeni değer** seçeneğini kullanarak ve değeri sağlayarak **geçerli değeri** güncelleştirin ( **varsayılan değeri** güncelleştirmeyin). Değerin, değişkenin veri türüyle eşleşmesi gerekir. Örneğin, Evet veya Hayır veri türü Evet ya da Hayır değerini kabul eder.

   :::image type="content" source="images/cosellconnectors/environment-variables-video.gif" alt-text="Ortam değişkenlerini güncelleştirme ' nin gösterildiği ekran görüntüsü.":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Uçtan uca iki yönlü ortak satış başvuru eşitlemesi

Power Automate çözümünü yükledikten, yapılandırdıktan ve özelleştirdikten sonra Salesforce CRM ve iş ortağı merkezi arasında ortak satış başvuruları eşitlemesini test edebilirsiniz.

### <a name="pre-requisites"></a>Ön koşullar

iş ortağı merkezi ve Salesforce CRM genelindeki başvuruları senkronize etmek için Power Automate çözümü, Microsoft 'a özgü başvuru alanlarını açıkça ortadan kaldırır. Bu kimlik, satıcı ekiplerinizi, ortak satış için Microsoft ile hangi referansları paylaşmak istediğlerine karar vermenize olanak sağlar.

Bir dizi özel alan, Salesforce CRM çözümü **fırsat** varlığı Için Iş Ortağı Merkezi başvuruları eşitlemesinin bir parçası olarak kullanılabilir. Bir CRM yönetici kullanıcısının **fırsat** özel alanlarıyla ayrı bir CRM bölümü oluşturması gerekir.

Aşağıdaki özel alanlar CRM bölümünün bir parçası olmalıdır:

- **Iş Ortağı Merkezi Ile Eşitle**: fırsatın Iş Ortağı Merkezi ile eşitlenmeyeceğini belirtir. Varsayılan olarak, bu alanın değeri Hayır ' dır ve Microsoft ile bir fırsat paylaşmak için satıcı tarafından açıkça Evet olarak ayarlanması gerekir. Iş Ortağı Merkezi 'nden CRM 'ye paylaşılan yeni başvurular, bu alan değeri Evet olarak ayarlanmıştır.

- **Başvuru tanımlayıcısı**: Microsoft Iş Ortağı Merkezi başvurusu için salt okunurdur bir tanımlayıcı alanı.

- **Başvuru bağlantısı**: Microsoft Iş Ortağı Merkezi ' nde başvurunun salt okunurdur bağlantısı.

- **Microsoft Yardımı**: başvuru için Microsoft 'un gerekli yardımı. Ortak satış başvurusu oluşturmak için, Microsoft 'tan gereken uygun yardımı seçin. Ortak satış başvurusu oluşturmak için bir müşteri kişisinin fırsatla ilişkilendirilmesi gerekir. Ortak satış olmayan bir başvuru oluşturmak için bu alanı seçmeyin. Ortak satış olmayan bir başvuru, uygun yardım-gerekli seçeneği belirlenerek her zaman ortak satış başvuruya dönüştürülebilir.

- **Microsoft Iş ortağı merkezi başvuru görünürlüğü**: Iş Ortağı Merkezi başvurusu için görünürlük ' i seçin. Ortak satış olmayan bir başvuru, Microsoft satıcıları için görünür hale getirerek ortak satış olarak dönüştürülebilir. Microsoft Yardım gerektiğinde, başvuru varsayılan olarak Microsoft satıcılarıyla görülebilir. Bu alan görünür olarak işaretlendikten sonra geri döndürülemez.

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
