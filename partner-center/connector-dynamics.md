---
title: Dynamics 365 CRM için ortak satış bağlayıcısı İş Ortağı Merkezi
description: Şirket içinde İş Ortağı Merkezi Dynamics 365 CRM ortak satış bağlayıcınız ile eşitler. Daha sonra CRM sisteminizin içinde Microsoft ile ortak satışlar da kullanabilirsiniz.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: 035a819020097ddee2230b5541e1b477d4b34c14
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148474"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>Dynamics 365 CRM için ortak satış bağlayıcısı genel bakış

**Uygun roller:** Referans yöneticisi | CRM'de sistem yöneticisi veya sistem özelleştiricisi

İş Ortağı Merkezi ortak satış bağlayıcıları, satış satıcılarının CRM sistemlerinizin içinde Microsoft ile ortak satışlar oluşturmalarını sağlar. Ortak satış anlaşmalarını yönetmek için İş Ortağı Merkezi eğitime sahip olması gerek yok. Ortak satış bağlayıcılarını kullanarak bir Microsoft satıcısıyla etkileşime geçen, Microsoft satıcısından referanslar alan, referansları kabul eden veya reddeden ve satış anlaşması değeri ve kapanış tarihi gibi satış verilerini değiştirmek için yeni bir ortak satış referansı oluşturun. Ayrıca bu ortak satış anlaşmaları hakkında Microsoft satıcılarından da güncelleştirmeler edinirsiniz. Tüm referanslarınızı yönetmek yerine kendi tercihlerinizi CRM'de İş Ortağı Merkezi.

Çözüm, api'leri Power Automate temel İş Ortağı Merkezi kullanır.

## <a name="prerequisites"></a>Önkoşullar

Çözümü yüklemeden önce aşağıdaki önkoşullara uygun olduğundan emin olun.

|**Konu başlıkları**   |**Ayrıntılar**   |**Bağlantılar**   |
|--------------|--------------------|------|
|Microsoft İş Ortağı Ağı (MPN) Kimliği |Geçerli bir MPN kimliğine ihtiyacınız vardır.|[İş Ortağı ağına katılma](https://partner.microsoft.com/)|
|Ortak satışa hazır|IP/Hizmetler çözümünüz ortak satışa hazır olmalı.|[Microsoft ile satış](https://partner.microsoft.com/membership/sell-with-microsoft)|
|İş Ortağı Merkezi hesabı|Kiracıyla ilişkilendirilmiş MPN İş Ortağı Merkezi ortak satış çözümünüzle ilişkili MPN Kimliği ile aynı olması gerekir. Bağlayıcıları dağıtmadan önce ortak satış referanslarınızı İş Ortağı Merkezi portalında gördüğünüzü doğrulayın.|[Hesabınızı yönetme](create-user-accounts-and-set-permissions.md)|
|İş Ortağı Merkezi Kullanıcı rolleri|Bağlayıcıları yükleyecek ve kullanacak olan çalışanın bir başvuru Yöneticisi olması gerekir.|[Kullanıcı rollerini ve izinlerini atama](create-user-accounts-and-set-permissions.md)|
|Dynamics 365 CRM|CRM Kullanıcı rolü, Sistem Yöneticisi veya sistem özelleştiricisi.|[Dynamics 365 ' de rol atama](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Güç otomatikleştirme akış hesabı|Test, hazırlama ve üretim için bir veritabanı ile yeni bir üretim ortamı oluşturun. Bir veritabanı olan bir üretim ortamınız varsa, yeniden kullanılabilir. Bağlayıcı çözümünü yüklemeye devam eden kullanıcının bu ortama yönelik bir güç otomatikleştirme lisansı ve erişimi olmalıdır. İlerleme durumunu izleyebilir ve yükleme başarısız olursa [Power otomatikleştirmede](https://flow.microsoft.com/) daha fazla bilgi edinebilirsiniz. **Çözümler** altında **geçmişi görüntüle** ' yi seçin.|[Ortam oluşturma veya yönetme](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Dynamics 365 için Iş Ortağı Merkezi başvuruları eşitlemesini (Power otomatikleştir çözümü) yükler

1. [Power otomatikleştirir](https://flow.microsoft.com)' a gidin ve sağ üst köşedeki **ortamlar** ' ı seçin. Bu adımda, kullanılabilir CRM örnekleri gösterilir.

1. Sağ üst köşedeki aşağı açılan listeden uygun CRM örneğini seçin.

1. Sol tarafta **çözümler** ' i seçin.

1. Üstteki menüde **AppSource 'U aç** bağlantısını seçin.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Açık AppSource gösteren ekran görüntüsü.":::

1. Açılır ekranda **Dynamics 365 Için Iş Ortağı Merkezi başvuruları bağlayıcılarını** arayın.  

1. **Şimdi al** düğmesini seçin ve ardından **devam**' ı seçin.

1. Uygulamayı yüklemek için CRM (Dynamics 365) ortamını seçebileceğiniz bir sayfa görüntülenir. Hüküm ve koşulları kabul edin.

1. İlerlemeyi izleyebilir ve yükleme başarısız olursa, **çözüm** altında **geçmişi göster** ' i seçerek Power otomatikleştirmede daha fazla bilgi edinebilirsiniz.

1. Yükleme tamamlandıktan sonra [Power otomatikleştirmeye](https://flow.microsoft.com) dönün ve sol taraftaki **çözümler** ' i seçin. **Dynamics 365 Için Iş Ortağı Merkezi başvuruları eşitleme** artık **çözüm** listesinde bulunabilir.

1. **Dynamics 365 Için Iş Ortağı Merkezi başvuruları eşitlemesini** seçin. Aşağıdaki güç otomatikleşme akışları ve varlıkları kullanılabilir.

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Kullanılabilir CRMs 'yi gösteren ekran görüntüsü.":::

## <a name="test-before-you-go-live"></a>Canlı çalışmadan önce test edin

Üretim ortamında güç otomatikleştirme çözümünü yüklemeden, yapılandırmadan ve özelleştirebilmeniz için, çözümü bir hazırlama CRM örneğinde test ettiğinizden emin olun. Şunları yapmanız gerekir:

- Güç otomatikleştirme çözümünü bir hazırlama ortamı CRM örneğine yükler.
- Güç otomatikleştirme çözümünü hazırlama ortamında yapılandırın ve özelleştirin.
- Çözümü bir hazırlama CRM örneğinde test edin.
- Başarılı bir testten sonra, üretim örneğine yönetilen bir çözüm olarak içeri aktarın.

## <a name="configure-the-solution"></a>Çözümü yapılandırma

1. Çözümü CRM Örneğinizde yükledikten sonra [Power otomatikleştirmeye](https://flow.microsoft.com/)geri dönün.

1. Sağ üst köşedeki **ortamlar** açılan listesinden, Power otomatikleştir çözümünü yüklediğiniz CRM örneğini seçin.

1. Üç Kullanıcı hesabını ilişkilendiren bağlantılar oluşturmanız gerekir:

   - İş Ortağı Merkezi yönetici kimlik bilgilerine sahip bir kullanıcı
   - İş Ortağı Merkezi Etkinlikleri
   - Çözümde akış Power Automate CRM yöneticisi

   1. Sol **tarafta** Bağlantılar'ı seçin ve **İş Ortağı Merkezi Referanslar** çözümünü seçin.

   1. Bağlantı oluştur'a **seçerek bağlantı oluşturun.**

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Bağlantı oluştur'a tıklayın.":::

   1. Sağ **İş Ortağı Merkezi arama çubuğunda Referanslar (önizleme)** araması gerçekleştirin.

   1. Referans yöneticisinin kimlik bilgileri İş Ortağı Merkezi kullanıcınız için bir bağlantı oluşturun.

   1. Ardından, Referanslar İş Ortağı Merkezi kimlik bilgileriyle İş Ortağı Merkezi kullanıcınız için bir Olay bağlantısı oluşturun.

   1. CRM yönetici kullanıcısı için Common Data Service (geçerli ortam) için bir bağlantı oluşturun.
     
   1. Tüm bağlantıları ekledikten sonra ortamınıza aşağıdaki bağlantıları görüyor gerekir.

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Bağlantıları gösteren ekran görüntüsü.":::

## <a name="edit-the-connections"></a>Bağlantıları düzenleme

1. Çözümler sayfasına **geri dönüp** Varsayılan **Çözüm'i seçin.** Tüm **'i seçerek Bağlantı Başvurusu (önizleme)** **öğesini seçin.**

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Bağlantıları düzenlemeyi gösteren ekran görüntüsü.":::

1. Üç nokta simgesini seçerek bağlantıların her bir öğesini tek tek düzenleyin. İlgili bağlantıları ekleyin.

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Listelenen bağlantıları gösteren ekran görüntüsü.":::

1.  Çözümler sayfasına **geri** dönüp **Dynamics 365** için İş Ortağı Merkezi Referans Eşitlemesi'ne tıklayın ve aşağıdaki sırayla her akışın yanındaki üç nokta simgesini seçerek akışı açabilirsiniz. Akışı açma sırasında herhangi bir sorunla karşılaşırsanız, bkz. [Özelleştirme adımları ve](connector-dynamics.md#customize-synchronization-steps) Sorun giderme [adımları.](connectors-troubleshoot.md)

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

1. Düzenle **simgesini seçin** ve HTTP **isteği geldiğinde'yi seçin.**

1. Sağlanan  HTTP POST URL'sini kopyalamak için Kopyala simgesini seçin.

   :::image type="content" source="images/webhook-video.gif" alt-text="Kaynak değişikliklerini kaydetmek için web kancalarını kullanmayı gösteren ekran görüntüsü.":::

1. Web **Kancası İş Ortağı Merkezi (Insider Preview)** Power Automate'ı ve ardından Çalıştır'ı **seçin.**

1. Akışı çalıştır **penceresinin sağ** bölmede açıldığından emin olduktan sonra Devam'ı **seçin.**

1. Şu ayrıntıları girin:

   - **Http Tetikleyici Uç** Noktası: Bu URL önceki bir adımdan kopyalandı.
   - **Kaydolmak Için olaylar**: kullanılabilir tüm olayları (**başvuru-oluşturulan**, **başvuru-güncelleştirilmiş**, **ilişkili-başvuru-oluşturma** ve **ilgili-başvuru-güncelleştirilmiş**) seçin.
   - Varsa **var olan tetikleyici uç noktalarının üzerine yaz**: Evet. Belirli bir Web kancası olayı için yalnızca bir URL kaydedilebilir.

1. **Akış Çalıştır**' ı seçin ve bitti ' yi seçin **.**

Web kancası artık olayları dinleyebilir, oluşturabilir ve güncelleştirebilir.

## <a name="customize-synchronization-steps"></a>Eşitleme adımlarını özelleştirme

CRM sistemleri büyük ölçüde özelleştirilir ve CRM kurulumunuzu temel alarak Power otomatikleştir çözümünü özelleştirebilirsiniz. Ortak satış başvuruları Iş ortağı merkezi ve CRM sisteminiz arasında eşitlendiğinde, Iş Ortağı Merkezi BILGISAYAR üzerinde eşitlenen alanlar [özel alan eşleme kılavuzunda](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)listelenir.

Alan eşleme kılavuzunu izleyin ve gerekirse, [özelleştirme] bölümünde uygun değişiklikleri yapın **Dynamics 365 Flow veya ortam değişkenlerinden ayrıntılar oluşturun veya alın** . Daha sonraki çözüm yükseltmelerini etkileyebileceğinden, Power otomatikleştir çözümündeki diğer akışları güncelleştirmeyin.

Aşağıdaki özelleştirmeler kullanılabilir:

- **Fırsat adında onay Işareti göster**: varsayılan olarak, Iş Ortağı Merkezi ile DYNAMICS 365 CRM arasındaki eşitlemenin başarıyla gerçekleştiği anlamına gelen fırsat adının yanında bir onay işareti görüntülenir. Benzer şekilde, eşitleme başarısız olursa bir çapraz işaret görüntülenir. Fırsat adına bir denetim veya çapraz işaret eklemekten kaçınmak için, **fırsat adı ortam değişkeninde görünen onay işaretinin** geçerli değerini Hayır olarak ayarlayın.
- **Anlaşma değeri**: varsayılan olarak, Iş Ortağı Merkezi 'nden anlaşma DEĞERI, CRM 'deki **estimatedvalue** ile ve bu değerden eşitlenecek. CRM 'de eşitlenecek anlaşma değeri için farklı bir alanınız varsa:

  - Dynamics 365 ortam değişkeninde, CRM 'nin alan adı ile **anlaşma değeri** alan adını güncelleştirin. Alanın adını, görünen adını değil, sağladığınızdan emin olun.
  - Düzenle **[özelleştirme] Dynamics 365 akışından ayrıntılar oluşturun veya** GÜNCELLEŞTIRIN ve CRM 'de **fırsat oluştur veya Güncelleştir** ' e gidin ve **Yeni bir fırsat oluşturun** ve **Mevcut fırsat eylemlerini güncelleştirin** ve CRM 'de doğru alana **satıcılarla değer** değerini atayın. Ayrıca, **tahmini gelir** alanından **satıcılarla değer** atamasını kaldırın.

- **Müşteri hesabı ülke kodu**: yeni bir başvuru oluştururken iki harfli bir ülke kodu (ISO 3166) sağlamanız zorunludur. Ülke kodu, varsayılan olarak, CRM 'deki **address1_country** alanından ve bu hesaba eşitlenir. CRM 'de eşitlenecek ülke kodunun farklı bir alanına sahipseniz:

   - Hesapta iki harfli bir kod içeren arama olmayan ülke kodu alanı için:
     - Dynamics 365 ortam değişkenindeki **müşteri hesabı ülke kodu** alan adını, CRM 'nin alan adıyla güncelleştirin. Alanın adını, görünen adını değil, sağladığınızdan emin olun.
     - Düzenle **[Özelleştir] Dynamics 365 akışından ayrıntılar oluşturun veya bu hesaptan ayrıntıları alın** ve CRM 'de doğru alana bir **ülke** değeri atamak için CRM eyleminde **müşteri hesabı oluştur veya Al** ' a gidin. Ayrıca, **ülke** değeri atamasını **Adres 1: ülke/bölge** alanından kaldırın.

   - Hesaptaki arama temelli bir ülke kodu alanı için:
     - Hesaba yeni bir özel alan ekleyin ve arama tabanlı alanda seçilen değere göre iki harfli bir ülke kodu (ISO 3166) ile otomatik olarak doldurun ve tam tersi de geçerlidir.
     - Yeni bir özel alanı CRM 'den ve Iş Ortağı Merkezi 'nden eşitlemek için, arama dışı ülke kodu alanına yönelik önceki adımları izleyin.

- **Fırsat alanları**: **fırsatta** doldurulması gereken zorunlu alanlar varsa, düzenleme **[özelleştirme] Dynamics 365 akışından ayrıntıları oluşturma veya GÜNCELLEŞTIRME hakkında bilgi alın** ve CRM 'de **fırsat oluştur veya Güncelleştir** ' e gidin ve iş gereksinimlerinize göre zorunlu alanlara değer atamak için **Yeni bir fırsat oluşturma eylemi oluşturun** .
- **Lider alanları**: **müşteri adayıyla** doldurulması gereken zorunlu alanlar varsa, **[Özelleştir] Dynamics 365 akışından ayrıntıları oluşturma veya güncelleştirme hakkında bilgi edinmek** Için, CRM 'de **müşteri adayı oluştur veya Güncelleştir** ' i ve güncelleştirme ' ye gidin ve iş gereksinimlerinize göre zorunlu alanlara değer atamak için **Yeni bir müşteri adayı eylemi oluşturun** .
- **Müşteri hesabı**: Iş ortağı MERKEZI 'nden CRM 'ye yeni bir başvuru eşitlendiğinde, Power otomatikleştir çözümü müşterinin Şirket adı ve posta kodunu kullanarak CRM 'de mevcut bir hesabı aramaya çalışır. Bir tane bulamazsa, CRM 'de yeni bir müşteri hesabı oluşturulur. Arama ölçütünü ve yeni hesap oluşturma ayrıntılarını güncelleştirmek için, düzenleme **[özelleştirme] Dynamics 365 akışından ayrıntılar oluşturun veya alın** ve CRM ve **müşteri hesabı oluşturma eyleminde** **müşteri hesabı oluştur veya Al** ' a gidin.

## <a name="update-environment-variable"></a>Ortam değişkenini Güncelleştir

Bir ortam değişken değerini güncelleştirmek için:

1. **Çözümler** sayfasına gidin ve **Varsayılan çözüm**' ı seçin. **Tümü**' nü seçerek **ortam değişkenini** seçin.

1. Güncelleştirilmesi gereken değer için ortam değişkenini seçin ve üç nokta simgesini kullanarak **Düzenle** ' yi seçin.

1. **Yeni değer** seçeneğini kullanarak ve değeri sağlayarak **geçerli değeri** güncelleştirin ( **varsayılan değeri** güncelleştirmeyin). Değerin, değişkenin veri türüyle eşleşmesi gerekir. Örneğin, Evet veya Hayır veri türü Evet ya da Hayır değerini kabul eder.

   :::image type="content" source="images/environment-variables-video.gif" alt-text="Ortam değişkenlerini güncelleştirme ' nin gösterildiği ekran görüntüsü.":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>Uçtan uca çift yönlü ortak satış başvuru eşitlemesi

Power otomatikleştir çözümünü yükledikten, yapılandırdıktan ve özelleştirdikten sonra, Dynamics 365 ve Iş ortağı merkezi arasında ortak satış başvuruları eşitlemesini test edebilirsiniz.

### <a name="prerequisites"></a>Önkoşullar

Iş ortağı merkezi ve Dynamics 365 CRM arasındaki başvuruları eşleştirmek için, Power otomatikleştir çözümü, Microsoft 'a özgü başvuru alanlarını açıkça ortadan kaldırır. Bu kimlik, satıcı ekiplerine ortak satış için Microsoft ile hangi referansları paylaşmak istediğini belirleme olanağı sağlar.

Bir dizi özel alan ve nesne, çözüm yüklemesinin parçası olarak eklenir. Bir CRM yönetici kullanıcısının **fırsat** özel alanlarıyla ayrı bir CRM bölümü oluşturması gerekir.

Aşağıdaki özel alanlar CRM bölümünün bir parçası olmalıdır:

- **Iş Ortağı Merkezi Ile Eşitle**: fırsatın Iş Ortağı Merkezi ile eşitlenmeyeceğini belirtir. Varsayılan olarak, bu alanın değeri Hayır ' dır ve Microsoft ile bir fırsat paylaşmak için satıcı tarafından açıkça Evet olarak ayarlanması gerekir. Iş Ortağı Merkezi 'nden CRM 'ye paylaşılan yeni başvurular, bu alan değeri Evet olarak ayarlanmıştır.
- **Başvuru tanımlayıcısı**: Iş Ortağı Merkezi başvurusu için salt okunurdur bir tanımlayıcı alanı.
- **Başvuru bağlantısı**: Iş Ortağı Merkezi 'nde başvurunun salt okunurdur bağlantısı.
- **Microsoft nasıl yardım edebilir?**: başvuru için Microsoft 'un gerekli olduğu yardım. Ortak satış başvurusu oluşturmak için, Microsoft 'tan gereken uygun yardımı seçin. Ortak satış başvurusu oluşturmak için bir müşteri kişisinin fırsatla ilişkilendirilmesi gerekir. Ortak satış olmayan bir başvuru oluşturmak için bu alanı seçmeyin. Ortak satış olmayan bir başvuru, uygun yardım-gerekli seçeneği belirlenerek her zaman ortak satış başvuruya dönüştürülebilir.
- **Microsoft Iş ortağı merkezi başvuru görünürlüğü**: Iş Ortağı Merkezi başvurusu için görünürlük ' i seçin. Ortak satış olmayan bir başvuru, Microsoft satıcıları için görünür hale getirerek ortak satış olarak dönüştürülebilir. Microsoft Yardım gerektiğinde, başvuru varsayılan olarak Microsoft satıcılarıyla görülebilir. Bu alan görünür olarak işaretlendikten sonra geri döndürülemez.
- **MICROSOFT CRM tanımlayıcısı**: Microsoft tarafından bir ortak satış başvurusu oluşturulup kabul edildiğinde, bu alan MICROSOFT 'un CRM tanımlayıcısı ile doldurulur.
- **Ürünler: kullanılmıyor**: bu alanı KULLANMAYıN veya CRM bölümüne ekleyin. Yalnızca geriye dönük uyumluluk için kullanılabilir. Bunun yerine Iş Ortağı Merkezi çözümlerini kullanın.
- **Denetim**: Iş Ortağı Merkezi başvurularına eşitleme için salt okunurdur bir denetim izi.
- **Microsoft Iş ortağı merkezi çözümleri**: ortak satış için hazırlanma çözümlerini veya Microsoft çözümlerini fırsatla ilişkilendirmek için özel bir nesne. Fırsatta bir veya daha fazla çözüm eklenebilir veya kaldırılabilir. Microsoft ile paylaşmadan önce fırsata en az bir ortak satış veya Microsoft çözümü eklemek zorunludur. Bu nesneyi fırsatla ilişkilendirmek için CRM 'de **fırsat** formunu güncelleştirin.

  **Fırsat** formunda uygun sekmesini seçin ve burada gösterildiği gibi bir alt ızgara ekleyin.

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Fırsat formunu gösteren ekran görüntüsü.":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Microsoft çözümlerini gösteren ekran görüntüsü.":::

- Microsoft çözümlerini ekledikten sonra, satıcılarınızın bunları eklemek zorunda kalmaması için ortak satış için kullanılabilir çözüm ayrıntılarını önceden girebilirsiniz. Yeni bir çözüm ayrıntısı eklemek için, CRM 'deki Microsoft çözüm ayrıntıları nesnesine gidin ve bir giriş eklemek için **kayıt Ekle** ' yi seçin veya birden çok giriş eklemek için **Excel karşıya yüklemeyi** kullanın.

  :::image type="content" source="images/dynamic-1a.png" alt-text="Yeni Microsoft çözüm ayrıntılarını gösteren ekran görüntüsü.":::

### <a name="scenarios"></a>Senaryolar

1. CRM 'de başvuru oluşturulduğunda veya güncelleştirilirken ve Iş Ortağı Merkezi 'nde eşitlendiğinde başvuru eşitlemesi:

   1. Dynamics 365 CRM ortamınızda, CRM 'nin **fırsat** bölümünde görünürlük olan kullanıcıyla oturum açın.

   1. Dynamics 365 ortamında yeni bir fırsat oluşturduğunuzda **Microsoft Iş Ortağı Merkezi** bölümünün mevcut olduğundan emin olun.

      :::image type="content" source="images/dynamic-2a.png" alt-text="Yeni fırsat gösteren ekran görüntüsü.":::

   1. Bu fırsatı Iş Ortağı Merkezi ile eşleştirmek için, kart görünümünde aşağıdaki alanları ayarlamış olduğunuzdan emin olun:

      - **Microsoft nasıl yardımcı olabilir?**: Ortak satış referansı oluşturmak için uygun bir yardım seçeneği belirleyin.

         :::image type="content" source="images/dynamic-3a.png" alt-text="Kart görünümünde uygun alanların nasıl alınacaklarını gösteren ekran görüntüsü.":::

      - **Müşteriyle** iletişim: Ortak satış referansı oluşturmak için fırsata bir müşteri ilgili kişisi ekleyin.
      - **İş Ortağı Merkezi** ile eşitle: Evet.
      - **Microsoft Çözümleri:** Referansı Microsoft ile paylaşmak için fırsata geçerli bir ortak satışa hazır veya Microsoft çözümü ekleyin.
      
        :::image type="content" source="images/dynamic-4a.png" alt-text="Çözüm Kimliğini gösteren ekran görüntüsü.":::

   1. Dynamics 365'te Fırsat ile Eşitle seçeneği Evet **İş Ortağı Merkezi** olarak oluşturulduktan sonra 10 dakika bekleyin. Ardından hesap hesabınızla İş Ortağı Merkezi olun. Referanslar Dynamics 365 ve Referans Tanımlayıcısı ile **eşitlenir.** **Referans Bağlantısı** doldurulur. Bir hata varsa Denetim **alanı** hata bilgileriyle doldurulur.
     
    1. Benzer şekilde, **İş Ortağı Merkezi** ile Eşitle seçeneği Evet olarak ayarlanmış bir fırsat için, Dynamics 365 CRM'de bu fırsatı güncelleştirseniz değişiklikler İş Ortağı Merkezi eşitlenir.

    1. İş Ortağı Merkezi ile başarıyla eşitlenen fırsatlar Dynamics 365'te ✔icon ile tanımlanır.

1. Referans, Dynamics 365 ortamında İş Ortağı Merkezi veya güncelleştirildiğinde referans eşitleme:

   1. Panonuza İş Ortağı Merkezi [açın.](https://partner.microsoft.com/dashboard/home)

   1. Sol **menüden** Referanslar'ı seçin.

   1. Yeni satış anlaşması seçeneğini kullanarak İş Ortağı Merkezi ortak satış **referansı** oluşturun.

   1. Dynamics 365 CRM ortamınıza oturum açma.

   1. Açık **Fırsatlar'a gidin.** İş Ortağı Merkezi oluşturulan referans artık Dynamics 365 CRM'de eşitlenir.

   1. Eşitlenmiş bir başvuruyu seçtiğinizde, kart Görünümü ayrıntıları doldurulur.

## <a name="next-steps"></a>Sonraki adımlar

- [Müşteri adaylarını yönetme](manage-leads.md)
- [Ortak satış fırsatlarını yönetme](manage-co-sell-opportunities.md)
- [Microsoft Power otomatikleştir platformu hakkında daha fazla bilgi](/power-automate/)
- [İş Ortağı Merkezi web kancaları](/partner-center/develop/partner-center-webhooks)
