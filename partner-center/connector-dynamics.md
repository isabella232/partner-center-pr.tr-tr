---
title: Dynamics 365 CRM Iş Ortağı Merkezi için ortak satış Bağlayıcısı
description: Ürün ortağı merkezindeki başvuruları, Dynamics 365 CRM için ortak satış Bağlayıcınız ile eşitler. Daha sonra CRM sisteminizin içinden Microsoft ile ortak satış yapabilirsiniz.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: 798a8a7d26480e8a1fc23bca3af45bd6a0e44778
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960305"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>Dynamics 365 için ortak satış Bağlayıcısı CRM 'ye Genel Bakış

**Uygun roller**: başvuru Yöneticisi | CRM 'de Sistem Yöneticisi veya sistem özelleştiricisi

İş Ortağı Merkezi ortak satış bağlayıcıları, satıcılarınızın müşteri ilişkisi sistemi (CRM) sistemlerinizden Microsoft ile ortak satıtabmasını sağlar. Ortak satış kurdukları anlaşmaları yönetmek için Iş Ortağı Merkezi 'ni kullanmaya eğitilmeleri gerekmez. Ortak satış bağlayıcılarını kullanarak yeni bir ortak satış referansı oluşturun:

- Microsoft satıcı ile iletişim kurun
- Microsoft satıcı 'dan başvuruları alma
- Başvuruları kabul etme veya reddetme
- Anlaşma değeri ve kapanış tarihi gibi işlem verilerini değiştirme 
 
Ayrıca, bu ortak satış konusunda Microsoft satıcılarından herhangi bir güncelleştirme de alabilirsiniz. Tüm başvurularınızı iş ortağı Merkezi yerine tercih ettiğiniz CRM 'de yönetebilirsiniz.

çözüm Power Automate tabanlıdır ve iş ortağı merkezi apı 'lerini kullanır.

## <a name="prerequisites"></a>Önkoşullar

Çözümü yüklemeden önce, aşağıdaki önkoşulları karşıladığınızdan emin olun.

| Konu başlıkları   | Ayrıntılar   | Bağlantılar   |
|--------------|--------------------|------|
| Microsoft İş Ortağı Ağı (MPN) KIMLIĞI |Geçerli bir MPN KIMLIĞI gereklidir. | [Iş ortağı ağına katılarak](https://partner.microsoft.com/) |
| Ortak satış hazırlanıyor|IP/hizmet çözümünüz ortak satış için hazırlık olmalıdır. | [Microsoft ile satış](https://partner.microsoft.com/membership/sell-with-microsoft) |
| İş Ortağı Merkezi hesabı | Iş Ortağı Merkezi kiracısı ile ilişkili MPN KIMLIĞI, ortak satış çözümünüz ile ilişkili MPN KIMLIĞIYLE aynı olmalıdır. Bağlayıcıları dağıtmadan önce ortak satış başvurularınızı Iş Ortağı Merkezi portalında görebildiğinizi doğrulayın. | [Hesabınızı yönetme](create-user-accounts-and-set-permissions.md) |
| İş Ortağı Merkezi Kullanıcı rolleri | Bağlayıcıları yükleyecek ve kullanacak olan çalışanın bir başvuru Yöneticisi olması gerekir.|[Kullanıcı rollerini ve izinlerini atama](create-user-accounts-and-set-permissions.md) |
| Dynamics 365 CRM|CRM Kullanıcı rolü, Sistem Yöneticisi veya sistem özelleştiricisi.|[Dynamics 365 ' de rol atama](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization) |
| Power Automate flow hesabı|Test, hazırlama ve üretim için bir veritabanı ile yeni bir üretim ortamı oluşturun. Bir veritabanı olan bir üretim ortamınız varsa, yeniden kullanılabilir. bağlayıcı çözümünü yükleyecek kullanıcının bu ortama bir Power Automate lisansı ve erişimi olması gerekir. yükleme başarısız olursa ilerleme durumunu izleyebilir ve [Power Automate](https://flow.microsoft.com/) daha fazla bilgi edinebilirsiniz. **Çözümler** altında **geçmişi görüntüle** ' yi seçin. | [Ortam oluşturma veya yönetme](/power-platform/admin/create-environment#create-an-environment-with-a-database) |

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Dynamics 365 için iş ortağı merkezi başvuruları eşitlemesini (Power Automate çözümü) yükler

1. [Power Automate](https://flow.microsoft.com)gidin ve sağ üst köşedeki **ortamlar** ' ı seçin. Bu adımda, kullanılabilir CRM örnekleri gösterilir.

2. Sağ üst köşedeki aşağı açılan listeden uygun CRM örneğini seçin.

3. Sol tarafta **çözümler** ' i seçin.

4. Üstteki menüde **AppSource 'U aç** bağlantısını seçin.

   :::image type="content" source="images/cosellconnectors/open-appsource.png" alt-text="Açık AppSource gösteren ekran görüntüsü.":::

5. Açılır ekranda **Dynamics 365 Için Iş Ortağı Merkezi başvuruları bağlayıcılarını** arayın.  

6. **Şimdi al** düğmesini seçin ve ardından **devam**' ı seçin.

7. Uygulamayı yüklemek için CRM (Dynamics 365) ortamını seçebileceğiniz bir sayfa görüntülenir. Hüküm ve koşulları kabul edin.

8. ilerlemeyi izleyebilir ve yükleme başarısız olursa, **çözümler** altında **geçmişi görüntüle** ' yi seçerek Power Automate daha fazla ayrıntı alabilirsiniz.

9. yükleme tamamlandıktan sonra, [Power Automate](https://flow.microsoft.com) ' ye dönün ve sol taraftaki **çözümler** ' i seçin. **Dynamics 365 Için Iş Ortağı Merkezi başvuruları eşitleme** artık **çözüm** listesinde bulunabilir.

10. **Dynamics 365 Için Iş Ortağı Merkezi başvuruları eşitlemesini** seçin. aşağıdaki Power Automate akışları ve varlıkları kullanılabilir.

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Kullanılabilir CRMs 'yi gösteren ekran görüntüsü.":::

## <a name="test-before-you-go-live"></a>Canlı çalışmadan önce test edin

üretim ortamında Power Automate çözümünü yüklemeden, yapılandırmadan ve özelleştirmadan önce, çözümü bir hazırlama CRM örneğinde test edin. Şunları yapmanız gerekir:

- Power Automate çözümünü bir hazırlama ortamı CRM örneğine yükler.
- Power Automate çözümünü hazırlama ortamında yapılandırın ve özelleştirin.
- Çözümü bir hazırlama CRM örneğinde test edin.
- Başarılı bir testten sonra, üretim örneğine yönetilen bir çözüm olarak içeri aktarın.

## <a name="configure-the-solution"></a>Çözümü yapılandırma

1. Çözümü CRM Örneğinizde yükledikten sonra [Power automate](https://flow.microsoft.com/)' a geri dönün.

2. sağ üst köşedeki **ortamlar** açılan listesinden Power Automate çözümünü yüklediğiniz CRM örneğini seçin.

3. Üç Kullanıcı hesabını ilişkilendiren bağlantılar oluşturmanız gerekir:

   - Ortak Merkezi Kullanıcı başvuruları yönetici kimlik bilgileri
   - İş Ortağı Merkezi Etkinlikleri
   - çözümde Power Automate akışlar ile CRM yöneticisi

   a. Sol taraftaki **Bağlantılar** ' ı seçin ve listeden **Iş Ortağı Merkezi başvuruları** çözümünü seçin.

   b. **Bağlantı oluştur** seçeneğini belirleyerek bir bağlantı oluşturun.

      :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Bağlantı oluştur ' un gösterildiği ekran görüntüsü.":::

   c. Sağ üst köşedeki arama çubuğunda **Iş Ortağı Merkezi başvurularını (Önizleme)** arayın.

   d. Iş Ortağı Merkezi kullanıcılarınız için, başvuru yöneticisinin kimlik bilgileri rolüyle bir bağlantı oluşturun.

   e. Ardından, Iş Ortağı Merkezi kullanıcılarınız için, başvuru Yöneticisi kimlik bilgileri ile bir Iş Ortağı Merkezi olaylar bağlantısı oluşturun.

   f. CRM yönetici kullanıcısı için Common Data Service (geçerli ortam) bağlantısı oluşturun.
     
   örneğin: Tüm bağlantıları ekledikten sonra ortamınızda aşağıdaki bağlantıları görmeniz gerekir.

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Bağlantıları gösteren ekran görüntüsü.":::

## <a name="edit-the-connections"></a>Bağlantıları düzenleme

1. **Çözümler** sayfasına dönün ve **Varsayılan çözüm**' ı seçin. **Tümünü** seçerek **Bağlantı başvurusunu (Önizleme)** seçin.

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Bağlantıların düzenlendiğinin gösterildiği ekran görüntüsü.":::

2. Üç nokta simgesini seçerek her bir bağlantıyı tek tek düzenleyin. İlgili bağlantıları ekleyin.

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Listelenen bağlantıları gösteren ekran görüntüsü.":::

3. **Çözümler** sayfasına dönün, **Dynamics 365 Için Iş Ortağı Merkezi başvuruları eşitlemesini** seçin ve aşağıdaki dizideki her akışın yanındaki üç nokta simgesini seçerek akışı açın. Akışı açtığınızda herhangi bir sorunla karşılaşırsanız, bkz. [özelleştirme adımları](connector-dynamics.md#customize-synchronization-steps) ve [sorun giderme adımları](connectors-troubleshoot.md).

   Akışları aşağıdaki sırada açın:

   a. İş Ortağı Merkezi Web kancası kaydı (Insider Preview)
   
   b. Kişiselleştirin Dynamics 365 akışından ayrıntılar oluşturun veya alın
   
   c. Ortak satış başvurusu oluşturma – Dynamics 365-Iş Ortağı Merkezi (Insider Preview)
   
   d. İş Ortağı Merkezi-Dynamics 365-Yardımcısı (Insider Preview)
   
   e. İş Ortağı Merkezi Microsoft ortak satış başvuruları Dynamics 365 'a (Insider Preview)
   
   f. İş Ortağı Merkezi-Dynamics 365 (Insider Preview)
   
   örneğin: Dynamics 365-Iş Ortağı Merkezi (Insider Preview)
   
   h. Dynamics 365 Iş Ortağı Merkezi (Insider Preview) fırsatı
   
   i. Dynamics 365 Microsoft Solutions for Partner Center (Insider Preview)
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Kaynak değişikliği olaylarına kaydolmak için Web kancası API 'Lerini kullanma

Kaynak değiştirme olaylarına kaydolmak için Iş Ortağı Merkezi Web kancası API 'Lerini kullanabilirsiniz. Bu değişiklik olayları, URL 'nize HTTP gönderileri olarak gönderilir.

1. **Iş Ortağı Merkezi 'Ni Dynamics 365 'e (Insider Preview)** seçin.

2. **Düzenle** simgesini seçin ve **bir http isteği alındığında** öğesini seçin.

3. Belirtilen HTTP POST URL 'sini kopyalamak için **Kopyala** simgesini seçin.

   :::image type="content" source="images/webhook-video.gif" alt-text="Kaynak değişikliklerini kaydetmek için Web kancalarını kullanmayı gösteren ekran görüntüsü.":::

4. **iş ortağı merkezi web kancası kaydı (ınsider preview)** Power Automate akışı ' nı seçin ve ardından **çalıştır**' ı seçin.

5. **Akış Çalıştır** penceresinin sağ bölmede açıldığından emin olun ve **devam**' ı seçin.

6. Şu ayrıntıları girin:

   - **Http tetikleyici uç noktası**: Bu URL önceki bir adımdan kopyalanmış.
   - **Kaydolmak Için olaylar**: kullanılabilir tüm olayları (**başvuru-oluşturulan**, **başvuru-güncelleştirilmiş**, **ilişkili-başvuru-oluşturma** ve **ilgili-başvuru-güncelleştirilmiş**) seçin.
   - Varsa **var olan tetikleyici uç noktalarının üzerine yaz**: Evet. Belirli bir Web kancası olayı için yalnızca bir URL kaydedilebilir.

7. **Akış Çalıştır**' ı seçin ve bitti ' yi seçin **.**

Web kancası artık olayları dinleyebilir, oluşturabilir ve güncelleştirebilir.

## <a name="customize-synchronization-steps"></a>Eşitleme adımlarını özelleştirme

crm sistemleri büyük ölçüde özelleştirilir ve Power Automate çözümünü, crm kurulumunuzu temel alarak özelleştirebilirsiniz. Ortak satış başvuruları Iş ortağı merkezi ve CRM sisteminiz arasında eşitlendiğinde, Iş Ortağı Merkezi BILGISAYAR üzerinde eşitlenen alanlar [özel alan eşleme kılavuzunda](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)listelenir.

Alan eşleme kılavuzunu izleyin ve gerekirse, [özelleştirme] bölümünde uygun değişiklikleri yapın **Dynamics 365 Flow veya ortam değişkenlerinden ayrıntılar oluşturun veya alın** . gelecekteki çözüm yükseltmelerini etkileyebileceğinden Power Automate çözümdeki diğer akışları güncelleştirmeyin.

Aşağıdaki özelleştirmeler kullanılabilir:

- **Fırsat adında onay Işareti göster**: varsayılan olarak, Iş Ortağı Merkezi ile DYNAMICS 365 CRM arasındaki eşitlemenin başarıyla gerçekleştiği anlamına gelen fırsat adının yanında bir onay işareti görüntülenir. Benzer şekilde, eşitleme başarısız olursa bir çapraz işaret görüntülenir. Fırsat adına bir denetim veya çapraz işaret eklemekten kaçınmak için, **fırsat adı ortam değişkeninde görünen onay işaretinin** geçerli değerini Hayır olarak ayarlayın.
- **Anlaşma değeri**: varsayılan olarak, Iş Ortağı Merkezi ' nden anlaşma DEĞERI, CRM 'de ve sürümünden eşitlenir `estimatedvalue` . CRM 'de eşitlenecek anlaşma değeri için farklı bir alanınız varsa:

  - Dynamics 365 ortam değişkeninde, CRM 'nin alan adı ile **anlaşma değeri** alan adını güncelleştirin. Alanın adını, görünen adını değil, sağladığınızdan emin olun.
  - Düzenle **[özelleştirme] Dynamics 365 akışından ayrıntılar oluşturun veya** GÜNCELLEŞTIRIN ve CRM 'de **fırsat oluştur veya Güncelleştir** ' e gidin ve **Yeni bir fırsat oluşturun** ve **Mevcut fırsat eylemlerini güncelleştirin** ve CRM 'de doğru alana **satıcılarla değer** değerini atayın. Ayrıca, **tahmini gelir** alanından **satıcılarla değer** atamasını kaldırın.

- **Müşteri hesabı ülke kodu**: yeni bir başvuru oluştururken iki harfli bir ülke kodu (ISO 3166) sağlamanız gerekir. Ülke kodu, varsayılan olarak, CRM 'deki **address1_country** alanından ve bu hesaba eşitlenir. CRM 'de eşitlenecek ülke kodunun farklı bir alanına sahipseniz:

  - İki harfli bir kod içeren hesapta arama olmayan bir ülke kodu alanı için, Dynamics 365 ortam değişkenindeki **müşteri hesabı ülke kodu** alan adını CRM 'nin alan adı ile güncelleştirin. Alanın adını, görünen adını değil, sağladığınızdan emin olun. Düzenle **[Özelleştir] Dynamics 365 akışından ayrıntılar oluşturun veya bu hesaptan ayrıntıları alın** ve CRM 'de doğru alana bir **ülke** değeri atamak için CRM eyleminde **müşteri hesabı oluştur veya Al** ' a gidin. Ayrıca, **ülke** değeri atamasını **Adres 1: ülke/bölge** alanından kaldırın.

  - Hesaptaki arama temelli bir ülke kodu alanı için, hesapta yeni bir özel alan ekleyin ve arama tabanlı alanda seçilen değere göre iki harfli bir ülke kodu (ISO 3166) ile otomatik olarak doldurun ve tam tersi de geçerlidir. Yeni bir özel alanı CRM 'den ve Iş Ortağı Merkezi 'nden eşitlemek için, arama dışı ülke kodu alanına yönelik önceki adımları izleyin.

- **Fırsat alanları**: **fırsatta** doldurulması gereken zorunlu alanlar varsa, düzenleme **[özelleştirme] Dynamics 365 akışından ayrıntıları oluşturma veya GÜNCELLEŞTIRME hakkında bilgi alın** ve CRM 'de **fırsat oluştur veya Güncelleştir** ' e gidin ve iş gereksinimlerinize göre zorunlu alanlara değer atamak için **Yeni bir fırsat oluşturma eylemi oluşturun** .
- **Lider alanları**: **müşteri adayıyla** doldurulması gereken zorunlu alanlar varsa, **[Özelleştir] Dynamics 365 akışından ayrıntıları oluşturma veya güncelleştirme hakkında bilgi edinmek** Için, CRM 'de **müşteri adayı oluştur veya Güncelleştir** ' i ve güncelleştirme ' ye gidin ve iş gereksinimlerinize göre zorunlu alanlara değer atamak için **Yeni bir müşteri adayı eylemi oluşturun** .
- **müşteri hesabı**: iş ortağı merkezi 'nden CRM 'ye yeni bir başvuru eşitlendiğinde Power Automate çözüm, müşteri şirket adı ve posta kodu kullanarak CRM 'de mevcut bir hesabı aramaya çalışır. Bir tane bulamazsa, CRM 'de yeni bir müşteri hesabı oluşturulur. Arama ölçütünü ve yeni hesap oluşturma ayrıntılarını güncelleştirmek için, düzenleme **[özelleştirme] Dynamics 365 akışından ayrıntılar oluşturun veya alın** ve CRM ve **müşteri hesabı oluşturma eyleminde** **müşteri hesabı oluştur veya Al** ' a gidin.

## <a name="update-environment-variable"></a>Ortam değişkenini Güncelleştir

Bir ortam değişken değerini güncelleştirmek için:

1. **Çözümler** sayfasına gidin ve **Varsayılan çözüm**' ı seçin. **Tümü**' nü seçerek **ortam değişkenini** seçin.

2. Güncelleştirilmesi gereken değer için ortam değişkenini seçin ve üç nokta simgesini kullanarak **Düzenle** ' yi seçin.

3. **Yeni değer** seçeneğini kullanarak ve değeri sağlayarak **geçerli değeri** güncelleştirin ( **varsayılan değeri** güncelleştirmeyin). Değerin, değişkenin veri türüyle eşleşmesi gerekir. Örneğin, Evet veya Hayır veri türü Evet ya da Hayır değerini kabul eder.

   :::image type="content" source="images/cosellconnectors/environment-variables-video.gif" alt-text="Ortam değişkenlerini güncelleştirme ' nin gösterildiği ekran görüntüsü.":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>Uçtan uca çift yönlü ortak satış başvuru eşitlemesi

Power Automate çözümünü yükledikten, yapılandırdıktan ve özelleştirdikten sonra, Dynamics 365 ve iş ortağı merkezi arasında ortak satış başvuruları eşitlemesini test edebilirsiniz.

### <a name="prerequisites"></a>Önkoşullar

iş ortağı merkezi ve Dynamics 365 CRM arasındaki başvuruları eşleştirmek için Power Automate çözümü, Microsoft 'a özgü başvuru alanlarını açıkça ortadan kaldırır. Bu kimlik, satıcı ekiplerine ortak satış için Microsoft ile hangi referansları paylaşmak istediğini belirleme olanağı sağlar.

Bir dizi özel alan ve nesne, çözüm yüklemesinin parçası olarak eklenir. Bir CRM yönetici kullanıcısının **fırsat** özel alanlarıyla ayrı bir CRM bölümü oluşturması gerekir.

Aşağıdaki özel alanlar CRM bölümünün bir parçası olmalıdır:

- **Iş Ortağı Merkezi Ile Eşitle**: fırsatın Iş Ortağı Merkezi ile eşitlenmeyeceğini belirtir. Varsayılan olarak, bu alanın değeri Hayır ' dır ve Microsoft ile bir fırsat paylaşmak için satıcı tarafından açıkça Evet olarak ayarlanması gerekir. Iş Ortağı Merkezi 'nden CRM 'ye paylaşılan yeni başvurular, bu alan değeri Evet olarak ayarlanmıştır.
- **Başvuru tanımlayıcısı**: Iş Ortağı Merkezi başvurusu için salt okunurdur bir tanımlayıcı alanı.
- **Başvuru bağlantısı**: Iş Ortağı Merkezi 'nde başvurunun salt okunurdur bağlantısı.
- **Microsoft nasıl yardım edebilir?**: başvuru için Microsoft 'un gerekli olduğu yardım. Ortak satış başvurusu oluşturmak için, Microsoft 'tan gereken uygun yardımı seçin. Ortak satış başvurusu oluşturmak için bir müşteri kişisinin fırsatla ilişkilendirilmesi gerekir. Ortak satış olmayan bir başvuru oluşturmak için bu alanı seçmeyin. Ortak satış olmayan bir başvuru, uygun yardım-gerekli seçeneği belirlenerek her zaman ortak satış başvuruya dönüştürülebilir.
- **Microsoft Iş ortağı merkezi başvuru görünürlüğü**: Iş Ortağı Merkezi başvurusu için görünürlük ' i seçin. Ortak satış olmayan bir başvuru, Microsoft satıcıları için görünür hale getirerek ortak satış olarak dönüştürülebilir. Microsoft Yardım gerektiğinde, başvuru varsayılan olarak Microsoft satıcılarıyla görülebilir. Bu alan görünür olarak işaretlendikten sonra geri döndürülemez.
- **Microsoft CRM tanımlayıcı**: microsoft tarafından bir ortak satış başvurusu oluşturulup kabul edildiğinde, bu alan microsoft 'un CRM tanımlayıcısı ile doldurulur.
- **Ürünler: kullanılmıyor**: bu alanı KULLANMAYıN veya CRM bölümüne ekleyin. Yalnızca geriye dönük uyumluluk için kullanılabilir. Bunun yerine Iş Ortağı Merkezi çözümlerini kullanın.
- **Denetim**: Iş Ortağı Merkezi başvurularına eşitleme için salt okunurdur bir denetim izi.
- **Microsoft Iş ortağı merkezi çözümleri**: ortak satış için hazırlanma çözümlerini veya Microsoft çözümlerini fırsatla ilişkilendirmek için özel bir nesne. Fırsattan bir veya daha fazla çözüm eklenebilir veya kaldırılabilir. Microsoft ile paylaşmadan önce fırsata en az bir ortak satışa hazır veya Microsoft çözümü eklemek zorunludur. Bu nesneyi fırsatla ilişkilendirmek için **CRM'de Fırsat** formunu güncelleştirin.

  Fırsat formunda uygun **sekmeyi seçin** ve burada gösterildiği gibi bir alt ızgara ekleyin.

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Fırsat formunu gösteren ekran görüntüsü.":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Microsoft Çözümleri'nin ekran görüntüsü.":::

- Microsoft çözümlerini ekledikten sonra ortak satışa hazır çözüm ayrıntılarını önceden doldurularak satış satıcılarının bunları eklemelerine gerek yok. Yeni bir çözüm ayrıntısı eklemek için CRM'de Microsoft  Çözüm Ayrıntıları nesnesine gidin ve Kayıt Ekle'yi seçerek bir giriş ekleyin veya birden çok girdi **eklemek Excel** karşıya yükleme seçeneğini kullanın.

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
      - **İş Ortağı Merkezi** eşitle: Evet.
      - **Microsoft Çözümleri:** Referansı Microsoft ile paylaşmak için fırsata geçerli bir ortak satışa hazır veya Microsoft çözümü ekleyin.

        :::image type="content" source="images/cosellconnectors/dynamics-solution-4.png" alt-text="Çözüm Kimliğini gösteren ekran görüntüsü.":::

   1. Dynamics 365'te Fırsat ile Eşitle seçeneği Evet **İş Ortağı Merkezi** olarak oluşturulduktan sonra 10 dakika bekleyin. Ardından hesap hesabınızla İş Ortağı Merkezi olun. Referanslar Dynamics 365 ve Referans Tanımlayıcısı ile **eşitlenir.** **Referans Bağlantısı** doldurulur. Bir hata varsa Denetim **alanı** hata bilgileriyle doldurulur.

      1. Benzer şekilde, **İş Ortağı Merkezi** ile Eşitle seçeneği Evet olarak ayarlanmış bir fırsat için, Dynamics 365 CRM'de bu fırsatı güncelleştirseniz değişiklikler İş Ortağı Merkezi eşitlenir.

      1. İş Ortağı Merkezi ile başarıyla eşitlenen fırsatlar Dynamics 365'te ✔icon ile tanımlanır.

1. Referans, Dynamics 365 ortamında İş Ortağı Merkezi oluşturulduğunda veya güncelleştirildiğinde referans eşitleme:

   1. Panonuza İş Ortağı Merkezi [açın.](https://partner.microsoft.com/dashboard/home)

   1. Sol **menüden** Referanslar'ı seçin.

   1. Yeni satış anlaşması seçeneğini kullanarak İş Ortağı Merkezi ortak satış **referansı** oluşturun.

   1. Dynamics 365 CRM ortamınıza oturum açma.

   1. Açık **Fırsatlar'a gidin.** İş Ortağı Merkezi oluşturulan referans artık Dynamics 365 CRM'de eşitlenir.

   1. Eşitlenmiş bir referansı seçerek kart görünümü ayrıntıları doldurulur.

## <a name="next-steps"></a>Sonraki adımlar

- [Müşteri adaylarını yönetme](manage-leads.md)
- [Ortak satış fırsatlarını yönetme](manage-co-sell-opportunities.md)
- [Microsoft Power Automate platformu hakkında daha fazla bilgi](/power-automate/)
- [İş Ortağı Merkezi web kancaları](/partner-center/develop/partner-center-webhooks)
