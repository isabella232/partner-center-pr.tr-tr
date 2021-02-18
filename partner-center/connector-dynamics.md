---
title: Dynamics 365 CRM Iş Ortağı Merkezi için ortak satış Bağlayıcısı
ms.topic: how-to
ms.date: 02/16/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ürün ortağı merkezindeki başvuruları, Dynamics 365 CRM için ortak satış Bağlayıcınız ile eşitler. Satıcılar daha sonra CRM sistemlerinizden Microsoft ile ortak bir şekilde satıtabilecekleri.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: e465130b96886cf2bb77bcd94f56c1a12545a5d5
ms.sourcegitcommit: 64243caed029ffe40e2bbc369f4ee96f4f0ca26f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/18/2021
ms.locfileid: "100645847"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>Dynamics 365 CRM için ortak satış Bağlayıcısı – genel bakış

### <a name="appropriate-roles"></a>Uygun roller

- Başvuru Yöneticisi
- CRM 'de Sistem Yöneticisi veya sistem özelleştiricisi

İş Ortağı Merkezi ortak satış Bağlayıcısı, satıcılarınızın CRM sistemlerinizden Microsoft ile ortak satıtabmasını sağlar. Ortak satış kurdukları anlaşmaları yönetmek için Iş Ortağı Merkezi 'ni kullanmaya eğitilmeleri gerekmez. Ortak satış bağlayıcılarını kullanarak Microsoft satıcı 'ya yönelik yeni bir ortak satış başvurusu oluşturun, Microsoft satıcı 'dan başvurular alın, başvuruları kabul edin/reddedin, işlem değeri gibi işlem verilerini değiştirin ve kapanış tarihi. Ayrıca, bu ortak satış konusunda Microsoft satıcılarından herhangi bir güncelleştirme de alabilirsiniz. Tüm başvurularınızı iş ortağı Merkezi yerine tercih ettiğiniz CRM 'de yönetebilirsiniz. 

Çözüm, Microsoft Power otomatikleştir çözümüne dayalıdır ve Iş Ortağı Merkezi API 'Lerini kullanır.

## <a name="before-you-install---pre-requisites"></a>Yüklemeden önce önkoşulları

|**Konu başlıkları**   |**Ayrıntılar**   |**Bağlantılar**   |
|--------------|--------------------|------|
|Microsoft İş Ortağı Ağı KIMLIĞI |Geçerli bir MPN KIMLIĞI gerekir|[MPN](https://partner.microsoft.com/) 'ye katılması için|
|Cosatışı hazırlanıyor|IP/hizmet çözümünüz ortak satış için hazırlık olmalıdır.|[Microsoft ile satış](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|İş Ortağı Merkezi hesabı|Iş Ortağı Merkezi kiracısı ile ilişkili MPN KIMLIĞI, ortak satış çözümünüz ile ilişkili MPN KIMLIĞIYLE aynı olmalıdır. Bağlayıcıları dağıtmadan önce Iş Ortağı Merkezi portalındaki ortak satış başvurularınızı görebildiğinizi doğrulayın.|[Hesabınızı yönetme](create-user-accounts-and-set-permissions.md)|
|İş Ortağı Merkezi Kullanıcı rolleri|Bağlayıcıları yükleyecek ve kullanacak çalışana bir başvuru Yöneticisi olmalıdır|[Kullanıcı rollerini ve izinlerini atama](create-user-accounts-and-set-permissions.md)| 
|Dynamics 365 CRM|CRM Kullanıcı rolü, Sistem Yöneticisi veya sistem özelleştiricisi|[Dynamics 365 ' de rol atama](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Güç otomatikleştirme akış hesabı|Test/hazırlama ve üretim için veritabanı ile yeni üretim ortamı oluşturun. Veritabanına sahip mevcut bir üretim ortamınız varsa, yeniden kullanılabilir. Bağlayıcı çözümünü yükleyecek olan kullanıcının, bu ortama yönelik lisansa otomatik hale getirmesi ve erişimi olması gerekir. İlerlemeyi izleyebilir ve daha fazla ayrıntı edinebilirsiniz. çözüm altında geçmişi gör ' e tıklayarak yüklemenin [Power otomatikleştirmede](https://flow.microsoft.com/) başarısız olması gerekir.|[Ortam oluşturma veya yönetme](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Dynamics 365 için Iş Ortağı Merkezi başvuruları eşitlemesini (Power otomatikleştir çözümü) yükler

1. [Power otomatikleştirir](https://flow.microsoft.com) ' a gidin ve sağ üst köşedeki **ortamlar** ' ı seçin. Bu adımda, kullanılabilir CRM örnekleri gösterilir.

2. Sağ üst köşedeki açılan listeden uygun CRM örneğini seçin.

3. Sol gezinti çubuğunda **çözümler** ' i seçin.

4. Üstteki menüde **AppSource aç** bağlantısına tıklayın.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource 'u aç":::

5. Açılır ekranda **Dynamics365 Için Iş Ortağı Merkezi başvuruları bağlayıcıları** aratın.  

6. **Şimdi al** düğmesine tıklayın ve ardından **devam edin**.

7. Bu, uygulamayı yüklemek için CRM (Dynamics 365) ortamını seçebileceğiniz sayfayı açar.  Hüküm ve koşulları kabul edin.

8. İlerlemeyi izleyebilir ve daha fazla ayrıntı edinebilirsiniz. **çözüm** altında **Geçmişi gör** ' e tıklayarak yüklemenin Power otomatikleştirmede başarısız olması gerekir.
 

9. Yükleme tamamlandıktan sonra [Power otomatikleştirmeye](https://flow.microsoft.com) dönün ve sol gezinti alanından **çözümler** ' i seçin. **Dynamics 365 Için Iş Ortağı Merkezi başvuruları** , çözümler listesinden kullanılabilir olduğuna dikkat edin.

10. **Dynamics 365 Için Iş Ortağı Merkezi başvuruları eşitlemesini** seçin. Aşağıdaki güç otomatikleşme akışları ve varlıkları mevcuttur:

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Kullanılabilir CRMS 'ler":::

## <a name="best-practice-test-before-you-go-live"></a>En iyi yöntem: canlı çalışmadan önce test edin

Üretim ortamında güç otomatikleştirme çözümünü yüklemeden, yapılandırmadan ve özelleştirebilmeniz için, çözümü bir hazırlama CRM örneğinde test ettiğinizden emin olun.

- Microsoft Power otomatikleştir çözümünü hazırlama ortamına/CRM örneğine yükler.
- Hazırlama ortamında Microsoft Power otomatikleştirmek çözümünü yapılandırın ve özelleştirin.
- Çözümü bir hazırlama/CRM örneğinde test edin. 
- Başarılı sayfasında, üretim örneğine yönetilen çözüm olarak içeri aktarın. 

## <a name="configure-the-solution"></a>Çözümü yapılandırma

1. Çözümü CRM Örneğinizde yükledikten sonra [Power otomatikleştirmek](https://flow.microsoft.com/)' a geri gidin.


2. Sağ üst köşedeki **ortamlar** açılan penceresinden, Power otomatikleştir çözümünü yüklediğiniz CRM örneğini seçin.

3. Üç Kullanıcı hesabını ilişkilendiren bağlantılar oluşturmanız gerekir:

   - Ortak Merkezi Kullanıcı başvuruları yönetici kimlik bilgileri

   - İş Ortağı Merkezi Etkinlikleri

   - Çözüm içindeki Power otomatikleştirmede CRM Yöneticisi.

      1. Sol gezinti çubuğundan **Bağlantılar** ' ı seçin ve listeden "Iş Ortağı Merkezi başvuruları" çözümünü seçin.

      2. **Bağlantı oluştur**' a tıklayarak bir bağlantı oluşturun.

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Bağlantı oluşturma":::

      3. Sağ üst köşedeki arama çubuğunda **Iş Ortağı Merkezi başvurularını (Önizleme)** arayın.

      4. Iş Ortağı Merkezi kullanıcılarınız için, başvuru yöneticisinin kimlik bilgileri rolüyle bir bağlantı oluşturun.

      5. Daha sonra, Iş Ortağı Merkezi kullanıcılarınız için, referanslar yöneticisinin kimlik bilgileriyle bir Iş Ortağı Merkezi olaylar bağlantısı oluşturun.

      6. CRM yönetici kullanıcısı için Common Data Service (geçerli ortam) bağlantısı oluşturun.
     
      7. Tüm bağlantılar eklendikten sonra ortamınızda aşağıdaki bağlantıları görmeniz gerekir:

:::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Bağlantılar":::
   
## <a name="edit-the-connections"></a>Bağlantıları düzenleme

1. **Çözümler** sayfasına dönün ve **Varsayılan çözüm**' ı seçin. **Tüm**' a tıklayarak **Bağlantı başvurusunu (Önizleme)** seçin.

:::image type="content" source="images/cosellconnectors/dynamics-3.png" alt-text="Bağlan":::

2. Üç nokta simgesini seçerek bağlantıların her birini tek tek düzenleyin. İlgili bağlantıları ekleyin.

:::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Listelenen bağlantılar"::: 

3.  Çözümler sayfasına dönün, Dynamics 365 için Iş Ortağı Merkezi başvuruları eşitlemesini seçin ve aşağıdaki dizide yer alan her akışın yanındaki üç nokta simgesine tıklayarak akışı etkinleştirin. Akışı açmak için herhangi bir sorunla karşılaşırsanız, [özelleştirme adımları](connector-dynamics.md#customize-synchronization-steps) ve [sorun giderme adımları](connectors-troubleshoot.md)bölümüne bakın. 

Akışları aşağıdaki sırada açın:

- İş Ortağı Merkezi Web kancası kaydı (Insider Preview)
- Ortak satış başvurusu oluşturma – Dynamics 365-Iş Ortağı Merkezi (Insider Preview)
- Kişiselleştirin Dynamics 365 akışından ayrıntılar oluşturun veya alın 
- İş Ortağı Merkezi-Dynamics 365-Yardımcısı (Insider Preview)
- İş Ortağı Merkezi Microsoft ortak satış başvuruları Dynamics 365 'a (Insider Preview)
- İş Ortağı Merkezi-Dynamics 365 (Insider Preview)
- Dynamics 365-Iş Ortağı Merkezi (Insider Preview)
- Dynamics 365 Iş Ortağı Merkezi (Insider Preview) fırsatı
- Dynamics 365 Microsoft Solutions for Partner Center (Insider Preview)
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Kaynak değişikliği olaylarına kaydolmak için Web kancası API 'Lerini kullanma

Iş Ortağı Merkezi Web kancası API 'Leri, kaynak değişiklik olaylarına kaydolmanızı sağlar. Bu değişiklik olayları, URL 'nize HTTP gönderileri olarak gönderilir.

1. **Iş Ortağı Merkezi 'Ni Dynamics 365 'e (Insider Preview)** seçin.

2. **Düzenle** simgesini seçin ve **bir http isteği alındığında** öğesini seçin.

3. Belirtilen HTTP POST URL 'sini kopyalamak için **Kopyala** simgesini seçin.

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="URL'yi Kopyala":::

4. Şimdi "Iş Ortağı Merkezi Web kancası kaydı 'nı (Insider Preview)" Power otomatikleştirmeyi seçin ve **Çalıştır**' ı seçin.

5. Sağ bölmede "akış Çalıştır" penceresinin açık olduğundan emin olun ve **devam**' a tıklayın.

6. Şu ayrıntıları girin:

   - **Http tetikleyici uç noktası**: önceki adımdan kopyalanmış URL

   - **Kayıt yapılacak olaylar**: tüm kullanılabilir olayları seçin ("başvuru oluşturma", "başvuru-güncelleştirilmiş", "ilgili-başvuru-oluşturulan", "ilgili-başvuru-güncelleştirilmiş")

   -Varsa **, var olan tetikleyici uç noktalarının üzerine yaz**: Evet, belirli bir Web kancası olayı için yalnızca bir URL kaydedileyebileceğine dikkat etmek önemlidir. Yalnızca bir URL 'nin belirli bir Web kancası olayı için kaydedileceği unutulmamalıdır. 

7. **Çalıştır** ' ı seçin ve **bitti** ' yi seçin.

Web kancası artık olayları oluşturmak ve güncelleştirmek için dinleme yapabilir.

## <a name="customize-synchronization-steps"></a>Eşitleme adımlarını özelleştirme

CRM sistemleri büyük ölçüde özelleştirilir ve CRM kurulumunuzu temel alarak Power otomatikleştir çözümünü özelleştirebilirsiniz.  Ortak satış başvuruları Iş ortağı merkezi ve CRM sisteminiz arasında eşitlendiğinde, Iş Ortağı Merkezi BILGISAYAR üzerinde eşitlenen alanlar [özel alan eşleme kılavuzunda](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)listelenir.

Alan eşleme kılavuzunu izleyin ve gerekirse, [özelleştirme] bölümünde uygun değişiklikleri yapın **Dynamics 365 Flow veya ortam değişkenlerinden ayrıntılar oluşturun veya alın**  . Daha sonraki çözüm yükseltmelerini etkileyebileceğinden, Power otomatikleştir çözümünde diğer akışların güncelleştirilmesi önerilmez. 

Kullanılabilir özelleştirmeler şunlardır:

- Fırsat adı onay işareti: varsayılan olarak, iş ortağı merkezi ve Dynamics 365 CRM arasındaki eşitlemenin başarıyla gerçekleştiği anlamına gelen fırsat adı ' nın yanında bir onay işareti görüntülenir. Benzer şekilde, eşitleme başarısız olursa bir çapraz işaret görüntülenir. Fırsat adında denetim veya çapraz işaret eklemeyi önlemek için, fırsat adı ortam değişkeninde Şu anki görüntüleme onay işareti değerini Hayır olarak ayarlayın.

- Anlaşma değeri: varsayılan olarak, Iş Ortağı Merkezi 'nden anlaşma değeri, CRM 'de **estimatedvalue** kaynağından ve bu değerden eşitlenecek. CRM 'de dağıtılacak değer için farklı bir alanınız varsa:

    a.    Dynamics 365 ortam değişkeninde, CRM 'nin alan adı ile anlaşma değeri alan adını güncelleştirin. Alanın adını, görünen adı değil, belirtmeniz gerektiğini unutmayın.

    b.    Düzenleme **[özelleştirme] Dynamics 365 akışından ayrıntı oluşturma veya güncelleştirme hakkında bilgi alın** ve CRM 'de fırsat **Oluştur veya Güncelleştir** ' e gidin ve CRM 'de doğru alana **satıcılarla değer** değeri atamak için **Yeni bir fırsat oluştur** ve **Mevcut fırsat eylemlerini Güncelleştir** ' i güncelleştirin. Ayrıca, **tahmini gelir** alanından **satıcılarla değer atamasını** kaldırın.

- Müşteri hesabı ülke kodu: yeni bir başvuru oluştururken iki harfli bir ülke kodu (ISO 3166) sağlamak zorunludur. Ülke kodu, varsayılan olarak, CRM 'de hesap address1_country alanından ve bu alandan eşitlenecek. CRM 'de şu kaynaktan eşitlenecek ülke kodu için farklı bir alanınız varsa:

   a.    Hesapta, iki harfli kod içeren arama olmayan bir ülke kodu alanı için:

   - Dynamics 365 ortam değişkenindeki müşteri hesabı ülke kodu alan adını, CRM 'nin alan adıyla güncelleştirin. Alanın adını, görünen adı değil, belirtmeniz gerektiğini unutmayın.

   - Düzenleme **[özelleştirme] Dynamics 365 akışından ayrıntılar oluşturun veya alın**  ve CRM 'de doğru alana ülke değeri atamak için CRM 'de müşteri hesabı oluştur veya Al ' a gidin. Ayrıca, Adres 1 ' den ülke değeri atamasını Kaldır: ülke/bölge alanı.

   b.    Hesabındaki arama temelli bir ülke kodu alanı için:

   - Hesapta yeni bir özel alan ekleyin ve arama tabanlı alanda seçilen değere göre iki harfli ülke kodu (ISO 3166) ile otomatik olarak doldurun ve tam tersi de geçerlidir.

   - Yeni özel alanı CRM 'den ve Iş Ortağı Merkezi ' nden eşitlemek için arama dışı ülke kodu alanı için yukarıdaki adımları izleyin.

- Fırsat alanları: fırsatta doldurulması gereken zorunlu alanlar varsa, düzenleme **[özelleştirme] Dynamics 365 akışından ayrıntıları oluşturun veya alın**  ve CRM 'de **fırsat oluştur veya Güncelleştir** ' i ve güncelleştirme ' ye giderek, iş gereksinimlerinize göre zorunlu alanlara değer atamak Için **Yeni bir fırsat oluşturma eylemi oluşturun** .

- Lider alanları: müşteri adayıyla doldurulması gereken zorunlu alanlar varsa, düzenleme **[özelleştirme] Dynamics 365 akışından ayrıntı oluşturma veya güncelleştirme hakkında bilgi edinmek**  ve CRM 'de **müşteri adayı oluştur veya Güncelleştir** ' i ve güncelleştirme ' ye giderek, iş gereksinimlerinize göre zorunlu alanlara değer atamak için **Yeni bir müşteri adayı eylemi oluşturma** ' ya gidin.

- Müşteri hesabı: Iş Ortağı Merkezi 'nden CRM 'ye yeni bir başvuru eşitlendiğinde, Power otomatikleştir çözümü müşteri şirket adı ve posta kodu kullanarak CRM 'de mevcut bir hesabı aramaya çalışır. Bir tane bulamazsa, CRM 'de yeni bir müşteri hesabı oluşturulur. Arama ölçütünü ve yeni hesap oluşturma ayrıntılarını güncelleştirmek için, düzenleme **[özelleştirme] Dynamics 365 akışından ayrıntılar oluşturun veya alın** ve CRM 'de **müşteri hesabı oluştur veya Al** ve **müşteri hesabı oluştur eylemi**' ne gidin.

## <a name="update-environment-variable"></a>Ortam değişkenini Güncelleştir

Bir ortam değişken değerini güncelleştirmek için:

1. **Çözümler** sayfasına gidin ve **Varsayılan çözüm**' ı seçin. Tümü ' ne tıklayarak **ortam değişkenini** seçin.

2. Güncelleştirilmesi gereken değer için ortam değişkenini seçin ve üç nokta simgesini kullanarak **Düzenle** ' ye tıklayın.

3. **Yeni değer** seçeneğini kullanarak **geçerli değeri** güncelleştirin (varsayılan değeri güncelleştirmeyin) ve değeri sağlayın. Değer, değişkenin veri türüyle eşleşmelidir; Örneğin, Evet/Hayır veri türü Evet veya Hayır değerini kabul eder.

:::image type="content" source="images/cosellconnectors/dynamics-5.png" alt-text="Varsayılan değerler için düzenleme kutusu":::

- Uçtan uca iki yönlü ortak satış başvuru eşitlemesi

Power otomatikleştir çözümünü yükledikten, yapılandırdıktan ve özelleştirdikten sonra, Dynamics 365 ve Iş ortağı merkezi arasında ortak satış başvuruları eşitlemesini test edebilirsiniz.

### <a name="pre-requisites"></a>Ön koşullar

Iş ortağı merkezi ve Dynamics 365 CRM arasındaki başvuruları eşleştirmek için, Power otomatikleştir çözümü, Microsoft 'a özgü başvuru alanlarını açıkça ortadan kaldırır. Bu kimlik, satıcı ekiplerine ortak satış için Microsoft ile hangi referansları paylaşmak istediğini belirleme olanağı sağlar.

Bir dizi özel alan ve nesne, çözüm yüklemesinin parçası olarak eklenir. Bir CRM yönetici kullanıcısının **fırsat** özel alanlarıyla ayrı bir CRM bölümü oluşturması gerekir.

Aşağıdaki özel alanlar CRM bölümünün bir parçası olmalıdır:

- **Iş Ortağı Merkezi Ile Eşitle**: fırsatın Microsoft Iş Ortağı Merkezi ile eşitlenmeyeceğini belirtir. Varsayılan olarak, bu alanın değeri Hayır ' dır ve Microsoft ile bir fırsat paylaşmak için satıcı tarafından açıkça Evet olarak ayarlanması gerekir. Iş Ortağı Merkezi 'nden CRM 'ye paylaşılan yeni başvurular, bu alan değeri Evet olarak ayarlanmıştır.

- **Başvuru tanımlayıcısı**: Microsoft Iş Ortağı Merkezi başvurusu için salt okunurdur bir tanımlayıcı alanı

- **Başvuru bağlantısı**: Microsoft Iş Ortağı Merkezi 'nde başvuruya yönelik salt okunurdur bir bağlantı
- **Microsoft nasıl yardım edebilir?**: başvuru için Microsoft 'un gerekli olduğu yardım. Ortak satış başvurusu oluşturmak için Microsoft 'tan gerekli uygun yardımı seçin. Ortak satış başvurusu oluşturmak için bir müşteri kişisinin fırsatla ilişkilendirilmesi gerekir. Ortak satış olmayan bir başvuru oluşturmak için bu alanı seçili değil olarak bırakın. Ortak satış olmayan bir başvuru, uygun yardım gerekli seçeneği belirlenerek her zaman ortak satış bir başvuruya dönüştürülebilir.

- **Microsoft Iş ortağı merkezi başvuru görünürlüğü**: Microsoft Iş Ortağı Merkezi başvurusu için görünürlük ' i seçin. Ortak satış olmayan bir başvuru, Microsoft satıcıları için görünür hale getirerek ortak satış olarak dönüştürülebilir. Microsoft Yardım gerektiğinde, başvuru varsayılan olarak Microsoft satıcılarıyla görülebilir. Görünür olarak işaretlendikten sonra bu alan geri döndürülemez.

- **MICROSOFT CRM tanımlayıcısı**: Microsoft tarafından bir ortak satış başvurusu oluşturulup kabul edildiğinde, bu alan MICROSOFT 'un CRM tanımlayıcısı ile doldurulur.

- **Ürünler: kullanılmıyor** – bu alanı KULLANMAYıN veya CRM bölümüne ekleyin, yalnızca geriye dönük uyumluluk için kullanılabilir. Bunun yerine Microsoft Iş Ortağı Merkezi çözümlerini kullanın.

- **Denetim**: Iş Ortağı Merkezi başvurularına eşitleme için salt okunurdur bir denetim izi

- **Microsoft Iş ortağı merkezi çözümleri**: ortak satış için hazırlanma çözümlerini veya Microsoft çözümlerini fırsatla ilişkilendirmek için özel bir nesne. Bir veya daha fazla çözüm eklenebilir ve/veya fırsata kaldırılabilir. Microsoft ile paylaşmadan önce fırsata en az bir ortak satış veya Microsoft çözümü eklenmesi zorunludur. Bu nesneyi fırsatla ilişkilendirmek için CRM 'de fırsat formunu güncelleştirin:

  Fırsat formu ' nda uygun sekmesini seçin ve aşağıda gösterildiği gibi bir alt ızgara ekleyin:

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Fırsat formu":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="{alternatif-metin}":::



- Microsoft çözümlerini ekledikten sonra, satıcılarınızın onları eklemesi gerekmiyorsa, ortak satış için kullanıma yönelik kullanıma yönelik çözüm ayrıntılarını önceden doldurabilirsiniz. Yeni bir çözüm ayrıntısı eklemek için, CRM 'de Microsoft çözüm ayrıntıları nesnesi ' ne gidin ve bir giriş eklemek için **kayıt Ekle** ' ye tıklayın veya birden çok giriş eklemek için **Excel karşıya yüklemeyi** kullanın.

:::image type="content" source="images/dynamic-1a.png" alt-text="Çözüm ayrıntıları":::

### <a name="scenarios"></a>LARLA

1. CRM 'de başvuru oluşturulduğunda veya güncelleştirilirken ve Iş Ortağı Merkezi 'nde eşitlendiğinde başvuru eşitlemesi:

   1. Dynamics 365 CRM ortamınızda, CRM 'nin **fırsat** bölümünde görünürlük olan kullanıcıyla oturum açın.

   2. Dynamics 365 ortamında "yeni fırsat" oluşturduğunuzda Microsoft Iş Ortağı Merkezi bölümünün mevcut olduğundan emin olun.

   :::image type="content" source="images/dynamic-2a.png" alt-text="Yeni fırsat"::: 

   3. Bu fırsatı Iş Ortağı Merkezi ile eşleştirmek için, kart görünümünde aşağıdaki alanları ayarlamış olduğunuzdan emin olun:

      - **Microsoft nasıl yardım edebilir?**: ortak satış başvurusu oluşturmak için uygun bir yardım seçeneği belirleyin.

         :::image type="content" source="images/dynamic-3a.png" alt-text="Kart görünümünde uygun alanları alma":::

      - **Müşteri iletişim**: ortak satış başvurusu oluşturmak için fırsata bir müşteri kişisi ekleyin.
      - **Iş Ortağı Merkezi Ile Eşitle**: Evet

      - Microsoft Solutions: bir başvuruyu Microsoft ile paylaşmak Için, fırsata geçerli bir ortak satış veya Microsoft çözümü ekleyin.
       
      
      :::image type="content" source="images/dynamic-4a.png" alt-text="Çözüm Kimliği":::

   4. Fırsat Dynamics 365 ' de Iş Ortağı Merkezi ile Eşitle seçeneği Evet olarak ayarlandığında, 10 dakika bekleyin ve ardından Iş Ortağı Merkezi hesabınızda oturum açın. Başvurularınız, Dynamics 365 ve başvuru tanımlayıcısıyla eşitlenir. Başvuru bağlantısı doldurulacak. Bir hata olması durumunda, denetim alanı hata bilgileriyle doldurulur.
     
    5. Benzer şekilde, "Partner Center ile eşitleme" seçeneği "Evet" olarak ayarlanmış bir fırsat için, Dynamics 365 CRM 'de fırsatı güncelleştirirseniz değişiklikler Iş Ortağı Merkezi hesabınızda eşitlenir.

    6. Iş Ortağı Merkezi ile başarıyla eşitlenen fırsatlar, Dynamics 365 ' de ✔ simgesiyle tanımlanır.

2. Microsoft Iş Ortağı Merkezi 'nde başvuru oluşturulduğunda veya güncelleştirilirken ve Dynamics 365 ortamında eşitlendiğinde başvuru eşitlemesi:

   1. Iş Ortağı Merkezi [panonuzda](https://partner.microsoft.com/dashboard/home)oturum açın.

   2. Sol taraftaki menüden **referanslar** ' ı seçin.

   3. **Yeni anlaşma** seçeneğini belirleyerek Iş Ortağı Merkezi 'nden yeni bir ortak satış başvurusu oluşturun.

   4. Dynamics 365 CRM ortamınızda oturum açın.

   5. **Açık fırsatlara** gidin. Microsoft Iş Ortağı Merkezi 'nde oluşturulan başvuru artık Dynamics 365 CRM 'de eşitlendi.

   6. Eşitlenmiş bir başvuruyu seçtiğinizde, kart Görünümü ayrıntıları doldurulur.

## <a name="next-steps"></a>Sonraki adımlar

- [Müşteri adaylarını yönetme](manage-leads.md)

- [Ortak satış fırsatlarını yönetme](manage-co-sell-opportunities.md)

- [Microsoft Power otomatikleştir platformu hakkında daha fazla bilgi](/power-automate/)

- [İş Ortağı Merkezi web kancaları](/partner-center/develop/partner-center-webhooks)