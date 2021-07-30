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
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114838130"
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

   a. İş Ortağı Merkezi Web Kancası Kaydı (Insider Önizlemesi)
   
   b. [Özelleştirme] Dynamics 365 akışından Ayrıntıları Oluşturma veya Al
   
   c. Ortak Satış Referansı Oluşturma – Dynamics 365 -İş Ortağı Merkezi (Insider Önizleme)
   
   d. İş Ortağı Merkezi Dynamics 365 - Yardımcı (Insider Önizlemesi)
   
   e. İş Ortağı Merkezi Microsoft'un Dynamics 365'e Ortak Satış Referans Güncelleştirmeleri (Insider Önizlemesi)
   
   f. İş Ortağı Merkezi Dynamics 365'e (Insider Önizleme)
   
   örneğin: Dynamics 365 -İş Ortağı Merkezi (Insider Önizleme)
   
   h. Dynamics 365 Opportunity to İş Ortağı Merkezi (Insider Preview)
   
   i. Dynamics 365 Microsoft Solutions to İş Ortağı Merkezi (Insider Preview)
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Kaynak değişikliği olaylarını kaydetmek için web kancası API'lerini kullanma

Kaynak değişikliği olaylarını İş Ortağı Merkezi için web kancası API'lerini kullanabilirsiniz. Bu değişiklik olayları URL'nize HTTP gönderileri olarak gönderilir.

1. **Dynamics 365 İş Ortağı Merkezi (Insider Preview) öğesini seçin.**

2. Düzenle **simgesini seçin** ve HTTP **isteği geldiğinde'yi seçin.**

3. Sağlanan  HTTP POST URL'sini kopyalamak için Kopyala simgesini seçin.

   :::image type="content" source="images/webhook-video.gif" alt-text="Kaynak değişikliklerini kaydetmek için web kancalarını kullanmayı gösteren ekran görüntüsü.":::

4. Web **Kancası İş Ortağı Merkezi (Insider Preview)** Power Automate'ı ve ardından Çalıştır'ı **seçin.**

5. Akışı çalıştır **penceresinin sağ** bölmede açıldığından emin olduktan sonra Devam'ı **seçin.**

6. Şu ayrıntıları girin:

   - **Http Tetikleyici Uç** Noktası: Bu URL önceki bir adımdan kopyalandı.
   - **Kaydedilebilecek Olaylar:** Tüm kullanılabilir olayları seçin (**referans oluşturuldu,** **referans güncelleştirildi,** **ilgili-referans oluşturuldu** ve **ilgili-referans-güncelleştirildi).**
   - **Mevcut tetikleyici uç noktalarının üzerine yaz?**: Evet. Bir web kancası olayı için yalnızca bir URL kaydedebilirsiniz.

7. Akışı **çalıştır'ı** ve ardından **Bitti'yi seçin.**

Web kancası artık olayları dinlemek, oluşturmak ve güncelleştirmek için kullanabilir.

## <a name="customize-synchronization-steps"></a>Eşitleme adımlarını özelleştirme

CRM sistemleri yüksek oranda özelleştirilmiştir ve CRM kurulum Power Automate özelleştirilebilir. Ortak satış referansları İş Ortağı Merkezi CRM sisteminiz arasında eşitlenmişse, İş Ortağı Merkezi pc'de eşitlenen alanlar Özel alan eşleme [kılavuzunda listelenir.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)

Alan eşleme kılavuzunu izleyin ve **gerekirse [Özelleştir] Dynamics 365** akışından veya ortam değişkenlerinden Ayrıntıları Al'da uygun değişiklikleri yapın. Gelecekteki çözüm yükseltmelerini etkileye Power Automate diğer akışları güncelleştirin.

Aşağıdaki özelleştirmeler kullanılabilir:

- **Fırsat adı içinde onay işaretini görüntüle:** Varsayılan olarak, İş Ortağı Merkezi ve Dynamics 365 CRM arasındaki eşitlemenin başarıyla tamam olduğunu belirtmek için fırsat adının yanında bir onay işareti görüntülenir. Benzer şekilde, eşitleme başarısız olursa bir çapraz işaret görüntülenir. Fırsat adına onay veya çapraz işaret eklemekten kaçınmak için fırsat adı ortam değişkensinde Görünen onay işaretinin geçerli **değerini** Hayır olarak ayarlayın.
- **Satış anlaşması** değeri: Varsayılan olarak, İş Ortağı Merkezi crm'de ile arasında `estimatedvalue` eşitlenen satış anlaşması değeri. CRM'de eşitlenen satış anlaşması değeri için farklı bir alanınız varsa:

  - Dynamics  365 ortam değişkeninin Satış değeri alan adını CRM'nin alan adıyla güncelleştirin. Alanın görünen adını değil, adının sağ olduğundan emin olun.
  - **Düzenle [Özelleştirme] Dynamics 365** akışından Ayrıntılar oluşturun  veya Alın ve CRM'de fırsat  oluşturma veya güncelleştirme'ye gidin, Yeni fırsat oluştur ve Mevcut fırsat eylemlerini güncelleştir'i güncelleştirin ve **DealValue** değerini CRM'de doğru alana atacak şekilde güncelleştirin.  Ayrıca Tahmini Gelir **alanından DealValue** **atamayı kaldırın.**

- **Müşteri Hesabı Ülke Kodu:** Yeni bir referans oluşturmak için iki harfli ülke kodu (ISO 3166) sağlayabilirsiniz. Varsayılan olarak, ülke kodu CRM'de hesabın address1_country **eşitler.** CRM'de ülke kodunun eşitley için farklı bir alanınız varsa:

  - Hesapta iki harfli kod içeren birlookup olmayan ülke kodu alanı için Dynamics 365 ortam değişkeninin Müşteri Hesabı **Ülke** Kodu alan adını CRM'nin alan adıyla güncelleştirin. Alanın görünen adını değil, adının sağ olduğundan emin olun. Düzenle **[Özelleştirme] Dynamics 365** akışından Ayrıntılar oluşturun  veya Alın ve CRM'de doğru  alana ülke değeri atamak için CRM eylemde müşteri hesabı oluşturma veya al'a gidin. Ayrıca Adres  **1: Ülke/Bölge alanından Ülke değeri atamayı** kaldırın.

  - Hesapta arama tabanlı bir ülke kodu alanı için hesaba yeni bir özel alan ekleyin ve bu alanı arama tabanlı alanda seçilen değere göre (ISO 3166) iki harfli ülke koduyla (ISO 3166) otomatik olarak ekleyin. CRM'den yeni bir özel alanı şirket içi ve dışına eşitlemek için, sonraki adımları izleyin ve bu alandan İş Ortağı Merkezi.

- **Fırsat alanları:** **Fırsat'ta** doldurulması gereken zorunlu alanlar varsa **[ Özelleştirme] Dynamics 365** akışından  Oluşturma veya Ayrıntıları Al'a  gidin, CRM'de fırsat oluşturma veya güncelleştirme'ye gidin ve İş gereksinimlerinize göre zorunlu alanlara değer atamak için Yeni bir fırsat eylemi oluştur'a gidin.
- **Müşteri adayı** alanları: Müşteri adayı  alanında doldurulması gereken zorunlu alanlar varsa **[Özelleştirme] Dynamics 365**  akışından Oluşturma veya Ayrıntıları  Al'a gidin, CRM'de müşteri adayı oluşturma veya güncelleştirme'ye gidin ve İş gereksinimlerinize göre zorunlu alanlara değer atamak için Yeni müşteri adayı eylemi oluştur'a gidin.
- **Müşteri hesabı:** İş Ortağı Merkezi'den CRM'ye yeni bir referans eşitlen olduğunda, Power Automate çözümü müşteri şirket adını ve posta kodunu kullanarak CRM'de mevcut bir hesabı aramaya çalışır. Bir hesap bulamazsa CRM'de yeni bir müşteri hesabı oluşturulur. Arama ölçütlerini ve yeni hesap oluşturma ayrıntılarını güncelleştirmek için  **[Özelleştirme] Dynamics 365** akışından Ayrıntıları Oluştur veya Al'a gidin ve CRM'de müşteri hesabı oluşturma veya al ve Müşteri hesabı oluştur **eylemine gidin.**

## <a name="update-environment-variable"></a>Ortam değişkenlerini güncelleştirme

Ortam değişkeni değerini güncelleştirmek için:

1. Çözümler sayfasına **gidin ve** Varsayılan **Çözüm'i seçin.** Tüm **'i seçerek** Ortam Değişkeni'ne **seçin.**

2. Güncelleştirilmiş olması gereken değer için ortam değişkenlerini seçin ve üç **nokta** simgesini kullanarak Düzenle'yi seçin.

3. Yeni **değer seçeneğini** kullanarak ve değeri sağlayarak **Geçerli** Değeri güncelleştirin (Varsayılan **Değeri** güncelleştirin). Değerin değişkenin veri türüyle eşleşmesi gerekir. Örneğin, Evet veya Hayır veri türü Evet veya Hayır değerini kabul eder.

   :::image type="content" source="images/cosellconnectors/environment-variables-video.gif" alt-text="Ortam değişkenlerini güncelleştir'i gösteren ekran görüntüsü.":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>4-24 çift yönlü ortak satış referans eşitlemesi

Power Automate çözümünü yükledikten, yapılandırıp özelleştirdikten sonra Dynamics 365 ile İş Ortağı Merkezi arasında ortak satış referans eşitlemesini test İş Ortağı Merkezi.

### <a name="prerequisites"></a>Önkoşullar

Power Automate çözümü, İş Ortağı Merkezi Dynamics 365 CRM'de referansları eşitlemek için Microsoft'a özgü referans alanlarını açıkça sınırlar. Bu kimlik, satıcı ekiplerinize ortak satış için Microsoft ile hangi referansları paylaşmak istediğinize karar verme olanağı verir.

Çözüm yüklemesi kapsamında bir dizi özel alan ve nesne eklenecektir. CRM yönetici kullanıcısnın Fırsat özel alanlarıyla ayrı bir CRM **bölümü** oluşturması gerekir.

Aşağıdaki özel alanlar CRM bölümünün bir parçası olması gerekir:

- **İş Ortağı Merkezi ile eşitleme:** Fırsatın İş Ortağı Merkezi. Varsayılan olarak, bu alanın değeri Hayır'dır ve Satıcınız tarafından Microsoft ile bir fırsat paylaşmak için açıkça Evet olarak ayar yapılması gerekir. İş Ortağı Merkezi CRM'ye paylaşılan yeni referanslarda bu alan değeri Evet olarak ayarlanır.
- **Referans Tanımlayıcısı:** Referans başvurusu için salt İş Ortağı Merkezi alanı.
- **Referans Bağlantısı:** Referansta referansın salt okunur İş Ortağı Merkezi.
- **Microsoft nasıl yardımcı olabilir?**: Referans için Microsoft'tan yardım gerekir. Ortak satış referansı oluşturmak için Microsoft'tan gereken uygun yardımı seçin. Ortak satış referansı oluşturma fırsatıyla bir müşteri ilgili kişisi ilişkili olması gerekir. Ortak satış dışı bir referans oluşturmak için bu alanı seçmeyin. Ortak satış olmayan bir referans, uygun yardım gerekli seçeneği seçerek ortak satış referansı olarak dönüştürmek için kullanılabilir.
- **Microsoft İş Ortağı Merkezi Referans Görünürlüğü:** Referans için İş Ortağı Merkezi seçin. Bunu Microsoft satış satıcılarının kullanımına açık hale dönüştürerek ortak satış olmayan bir referans ortak satışa dönüştürülmüş olabilir. Microsoft yardımı gerektiğinde referans varsayılan olarak Microsoft satıcılarının kullanımına açıktır. Bu alan görünür olarak işaretlendikten sonra geri döndürülmeyebilir.
- **Microsoft CRM:** Ortak satış referansı oluşturulduğunda ve Microsoft tarafından kabul edilirken, bu alan Microsoft'un CRM tanımlayıcısıyla doldurulur.
- **Ürünler: Eski:** Bu alanı kullanma veya CRM bölümüne ekleme. Yalnızca geriye dönük uyumluluk için kullanılabilir. Bunun İş Ortağı Merkezi çözümlerini kullanın.
- **Denetim:** Referanslarla eşitlemek için salt okunur bir İş Ortağı Merkezi izi.
- **Microsoft İş Ortağı Merkezi Çözümleri:** Ortak satışa hazır çözümleri veya Microsoft çözümlerini fırsatla ilişkilendirmek için özel bir nesne. Fırsattan bir veya daha fazla çözüm eklenebilir veya kaldırılabilir. Microsoft ile paylaşmadan önce fırsata en az bir ortak satışa hazır veya Microsoft çözümü eklemek zorunludur. Bu nesneyi fırsatla ilişkilendirmek için **CRM'de Fırsat** formunu güncelleştirin.

  Fırsat formunda uygun **sekmeyi seçin** ve burada gösterildiği gibi bir alt ızgara ekleyin.

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Fırsat formunu gösteren ekran görüntüsü.":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Microsoft Çözümleri'nin ekran görüntüsü.":::

- Microsoft çözümlerini ekledikten sonra ortak satışa hazır çözüm ayrıntılarını önceden doldurularak satış satıcılarının bunları eklemelerine gerek yok. Yeni bir çözüm ayrıntısı eklemek için CRM'de Microsoft  Çözüm Ayrıntıları nesnesine gidin ve Kayıt Ekle'yi seçerek bir girdi ekleyin veya birden çok girdi **eklemek Excel** karşıya yükleme seçeneğini kullanın.

  :::image type="content" source="images/cosellconnectors/dynamics-solution-1.png" alt-text="Yeni Microsoft Çözümü Ayrıntılarını gösteren ekran görüntüsü.":::

### <a name="scenarios"></a>Senaryolar

1. Referans CRM'de oluşturulduğunda veya güncelleştirildiğinde ve referansta eşitlendi İş Ortağı Merkezi:

   1. CRM'nin Fırsat bölümünde görünürlüğü olan kullanıcıyla Dynamics 365 CRM **ortamında** oturum açma.

   1. Dynamics 365 İş Ortağı Merkezi yeni bir fırsat oluşturdukta **Microsoft** İş Ortağı Merkezi bölümünün mevcut olduğundan emin olmak.

      :::image type="content" source="images/cosellconnectors/dynamics-solution-2.png" alt-text="Yeni fırsat'ın ekran görüntüsü.":::

   1. Bu fırsatı İş Ortağı Merkezi eşitlemek için, kart görünümünde aşağıdaki alanları ayar

      - **Microsoft nasıl yardımcı olabilir?**: Ortak satış referansı oluşturmak için uygun yardım seçeneğini belirleyin.

         :::image type="content" source="images/cosellconnectors/dynamics-solution-3.png" alt-text="Kart görünümünde uygun alanların nasıl alınacaklarını gösteren ekran görüntüsü.":::

      - **Müşteriyle** iletişim: Ortak satış referansı oluşturmak için fırsata bir müşteri ilgili kişisi ekleyin.
      - **İş Ortağı Merkezi** ile eşitle: Evet.
      - **Microsoft Çözümleri:** Referansı Microsoft ile paylaşmak için fırsata geçerli bir ortak satışa hazır veya Microsoft çözümü ekleyin.

        :::image type="content" source="images/cosellconnectors/dynamics-solution-4.png" alt-text="Çözüm Kimliğini gösteren ekran görüntüsü.":::

   1. Dynamics 365'te Fırsatla Eşitle seçeneği Evet **İş Ortağı Merkezi** olarak oluşturulduktan sonra 10 dakika bekleyin. Ardından hesap hesabınızla İş Ortağı Merkezi olun. Referanslar Dynamics 365 ve Referans Tanımlayıcısı ile **eşitlenir.** **Referans Bağlantısı** doldurulur. Bir hata varsa Denetim **alanı** hata bilgileriyle doldurulur.

      1. Benzer şekilde, **İş Ortağı Merkezi** ile Eşitle seçeneği Evet olarak ayarlanmış bir fırsat için, Dynamics 365 CRM'de bu fırsatı güncelleştirseniz değişiklikler İş Ortağı Merkezi eşitlenir.

      1. İş Ortağı Merkezi ile başarıyla eşitlenen fırsatlar Dynamics 365'✔icon ile tanımlanır.

1. Referans, Dynamics 365 ortamında İş Ortağı Merkezi veya güncelleştirildiğinde referans eşitleme:

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
