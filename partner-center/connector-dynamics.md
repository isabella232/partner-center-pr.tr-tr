---
title: Dynamics 365 CRM Iş Ortağı Merkezi için ortak satış Bağlayıcısı
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Iş ortağı merkezindeki başvurularınızı Dynamics 365 CRM için ortak satış Bağlayıcınız ile senkronize edin. Satıcılar daha sonra CRM sistemlerinizden Microsoft ile ortak bir şekilde satıtabilecekleri.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: c92938bbb4ffa6875419d06a9bbf23010ee60724
ms.sourcegitcommit: 7e32544cf91f932cbeb053c9de506ba9ee773fe2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/20/2020
ms.locfileid: "94947824"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>Dynamics 365 CRM için ortak satış Bağlayıcısı – genel bakış

### <a name="appropriate-roles"></a>Uygun roller

- Başvuru Yöneticisi
- CRM 'de Sistem Yöneticisi veya sistem özelleştiricisi

İş Ortağı Merkezi ortak satış Bağlayıcısı, satıcılarınızın CRM sistemlerinizden Microsoft ile ortak satıtabmasını sağlar. Ortak satış kurdukları anlaşmaları yönetmek için Iş Ortağı Merkezi 'ni kullanmaya eğitilmeleri gerekmez. Ortak satış bağlayıcılarını kullanarak Microsoft satıcı 'ya yönelik yeni bir ortak satış başvurusu oluşturun, Microsoft satıcı 'dan başvurular alın, başvuruları kabul edin/reddedin, işlem değeri gibi işlem verilerini değiştirin ve kapanış tarihi. Ayrıca, bu ortak satış konusunda Microsoft satıcılarından herhangi bir güncelleştirme de alabilirsiniz. Tüm başvurularınızın iş ortağı Merkezi yerine tercih ettiğiniz CRM 'de çalışmasını sağlayabilirsiniz. 

Çözüm, Microsoft Power otomatikleştir çözümüne dayalıdır ve Iş Ortağı Merkezi API 'Lerini kullanır.

## <a name="before-you-install---pre-requisites"></a>Yüklemeden önce önkoşulları

|**Konu başlıkları**   |**Ayrıntılar**   |**Bağlantılar**   |
|--------------|--------------------|------|
|Microsoft İş Ortağı Ağı KIMLIĞI |Geçerli bir MPN KIMLIĞI gerekir|[MPN](https://partner.microsoft.com/) 'ye katılması için|
|Cosatışı hazırlanıyor|IP/hizmet çözümünüz ortak satış için hazırlık olmalıdır.|[Microsoft ile satış](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|İş Ortağı Merkezi hesabı|Iş Ortağı Merkezi kiracısı ile ilişkili MPN KIMLIĞI, ortak satış çözümünüz ile ilişkili MPN KIMLIĞIYLE aynı olmalıdır. Bağlayıcıları dağıtmadan önce Iş Ortağı Merkezi portalındaki ortak satış başvurularınızı görebildiğinizi doğrulayın.|[Hesabınızı yönetme](create-user-accounts-and-set-permissions.md)|
|İş Ortağı Merkezi Kullanıcı rolleri|Bağlayıcıları yükleyecek ve kullanacak çalışana bir başvuru Yöneticisi olmalıdır|[Kullanıcı rollerini ve izinlerini atama](create-user-accounts-and-set-permissions.md)| |Dynamics 365 CRM|CRM Kullanıcı rolü, Sistem Yöneticisi veya sistem özelleştiricisi|[Dynamics 365 ' de rol atama](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Güç otomatikleştirme akış hesabı|CRM Sistem Yöneticisi veya sistem özelleştirici için etkin bir [Güç otomatikleştirme](https://flow.microsoft.com) hesabı. Bu kullanıcının, yüklemeden önce en az bir kez [Power otomatikleştirmek](https://flow.microsoft.com) için oturum açması gerekir.|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Dynamics 365 için Iş Ortağı Merkezi başvuruları eşitlemesini (Power otomatikleştir çözümü) yükler

1. [Power otomatikleştirir](https://flow.microsoft.com) ' a gidin ve sağ üst köşedeki **ortamlar** ' ı seçin. Bu adımda, kullanılabilir CRM örnekleri gösterilir.

2. Sağ üst köşedeki açılan listeden uygun CRM örneğini seçin.

3. Sol gezinti çubuğunda **çözümler** ' i seçin.

4. Üstteki menüde **AppSource aç** bağlantısına tıklayın.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource 'u aç":::

5. Açılır ekranda **Dynamics365 Için Iş Ortağı Merkezi başvuruları bağlayıcıları** aratın.  

6. **Şimdi al** düğmesine tıklayın ve ardından **devam edin**.

7. Bu, uygulamayı yüklemek için CRM (Dynamics 365) ortamını seçebileceğiniz sayfayı açar.  Hüküm ve koşulları kabul edin.

8. Daha sonra **çözümlerinizi yönetme** sayfasına yönlendirilirsiniz.  Sayfanın alt kısmındaki ok düğmelerini kullanarak "Iş Ortağı Merkezi başvuruları" na gidin. **Yükleme zamanlandı** , Iş Ortağı Merkezi başvuruları çözümünün yanında görünmelidir. Yükleme, 10-15 dakika sürer. 

9. Yükleme tamamlandıktan sonra [Power otomatikleştirmeye](https://flow.microsoft.com) dönün ve sol gezinti alanından **çözümler** ' i seçin. **Dynamics 365 Için Iş Ortağı Merkezi başvuruları** , çözümler listesinden kullanılabilir olduğuna dikkat edin.

10. **Dynamics 365 Için Iş Ortağı Merkezi başvuruları eşitlemesini** seçin. Aşağıdaki güç otomatikleşme akışları ve varlıkları mevcuttur:

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Kullanılabilir CRMS 'ler":::

## <a name="best-practice-test-before-you-go-live"></a>En iyi yöntem: canlı çalışmadan önce test edin

Üretim ortamında güç otomatikleştirme çözümünü yüklemeden, yapılandırmadan ve özelleştirebilmeniz için, çözümü bir hazırlama CRM örneğinde test ettiğinizden emin olun.

- Microsoft Power otomatikleştir çözümünü hazırlama ortamına/CRM örneğine yükler.
- Çözümün bir kopyasını oluşturun ve yapılandırma ve Power otomatikleştir akış özelleştirmelerinizi hazırlama ortamında çalıştırın.
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

         :::image type="content" source="images/cosellconnectors/dynamics1.png" alt-text="Bağlantı oluşturma":::

      3. Sağ üst köşedeki arama çubuğunda **Iş Ortağı Merkezi başvurularını (Önizleme)** arayın.

      4. Iş Ortağı Merkezi kullanıcılarınız için, başvuru yöneticisinin kimlik bilgileri rolüyle bir bağlantı oluşturun.

      5. Daha sonra, Iş Ortağı Merkezi kullanıcılarınız için, referanslar yöneticisinin kimlik bilgileriyle bir Iş Ortağı Merkezi olaylar bağlantısı oluşturun.

      6. CRM yönetici kullanıcısı için Common Data Service (geçerli ortam) bağlantısı oluşturun.
       
     
      7. Tüm bağlantılar eklendikten sonra ortamınızda aşağıdaki bağlantıları görmeniz gerekir:

:::image type="content" source="images/cosellconnectors/dynamics2.png" alt-text="Bağlantılar":::
   
## <a name="edit-the-connections"></a>Bağlantıları düzenleme

1. **Çözümler** sayfasına dönün ve **Varsayılan çözüm**' ı seçin. **Tüm**' a tıklayarak **Bağlantı başvurusunu (Önizleme)** seçin.

:::image type="content" source="images/cosellconnectors/dynamics3.png" alt-text="Bağlan":::

2. Üç nokta simgesini seçerek bağlantıların her birini tek tek düzenleyin. İlgili bağlantıları ekleyin.

:::image type="content" source="images/cosellconnectors/dynamics4.png" alt-text="Listelenen bağlantılar"::: 

3.  Akışları aşağıdaki sırada açın:
- İş Ortağı Merkezi Web kancası kaydı (Insider Preview)
- Ortak satış başvurusu oluşturma – Dynamics 365-Iş Ortağı Merkezi (Insider Preview)
- İş Ortağı Merkezi Microsoft ortak satış başvuruları Dynamics 365 'a (Insider Preview)
- İş Ortağı Merkezi-Dynamics 365 (Insider Preview)
- Dynamics 365-Iş Ortağı Merkezi (Insider Preview)
- Dynamics 365 Iş Ortağı Merkezi (Insider Preview) fırsatı
- Dynamics 365 Microsoft Solutions for Partner Center (Insider Preview)
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Kaynak değişikliği olaylarına kaydolmak için Web kancası API 'Lerini kullanma

Iş Ortağı Merkezi Web kancası API 'Leri, kaynak değişiklik olaylarına kaydolmanızı sağlar. Bu değişiklik olayları, URL 'nize HTTP gönderileri olarak gönderilir.

1. URL 'nizi kaydetmek için **Iş Ortağı Merkezi Web kancası kaydı (Insider Preview)** güç otomatikleştirme akışı ' nı seçin.

2. (A.) Iş Ortağı Merkezi kullanıcısına, aşağıdaki vurgulanmış şekilde, başvuru Yöneticisi kimlik bilgileri (b.) Iş Ortağı Merkezi etkinliklerine yönelik bağlantılar ekleyin

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Tetikleyici":::

3. Bu güncelleştirmeleri yaptığınızda şunu görürsünüz:

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Web Kancaları":::

4. Değişikliklerinizi kaydedin ve **Aç '** ı seçin.

   Iş Ortağı Merkezi Web kancalarını olay değişikliklerini dinleyecek şekilde etkinleştirmek için aşağıdaki adımları uygulayın:

5. **Iş Ortağı Merkezi 'Ni Dynamics 365 'e (Insider Preview)** seçin.

6. **Düzenle** simgesini seçin ve **bir http isteği alındığında** öğesini seçin.

7. Belirtilen HTTP POST URL 'sini kopyalamak için **Kopyala** simgesini seçin.

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="URL'yi Kopyala":::

8. Şimdi "Iş Ortağı Merkezi Web kancası kaydı 'nı (Insider Preview)" Power otomatikleştirmeyi seçin ve **Çalıştır**' ı seçin.

9. Sağ bölmede "akış Çalıştır" penceresinin açık olduğundan emin olun ve **devam**' a tıklayın.

10. Şu ayrıntıları girin:

    1. **Http tetikleyici uç noktası**: önceki adımdan kopyalanmış URL

    2. **Kaydolmak Için olaylar**: "başvuru oluşturuldu" ve "başvuru-güncelleştirildi"

    3. Varsa **var olan tetikleyici uç noktalarının üzerine yaz**: Evet (Bu, mevcut tüm uç noktaların üzerine yazar.)

11. **Çalıştır** ' ı seçin ve **bitti** ' yi seçin.

Web kancası artık olayları oluşturmak ve güncelleştirmek için dinleme yapabilir.

## <a name="customize-synchronization-steps"></a>Eşitleme adımlarını özelleştirme

Ortak satış başvuruları Iş ortağı merkezi ve CRM sisteminiz arasında eşitlendiğinde, Iş Ortağı Merkezi BILGISAYAR üzerinde eşitlenen alanlar burada listelenir.

Genellikle CRM sistemleri oldukça özelleştirilir. Power otomatikleştir akışlarını özelleştirebilirsiniz. Alan eşleme kılavuzunu izleyin ve gerekirse Power otomatikleştir akışlarının adımlarında uygun değişiklikleri yapın.  CRM eşlemelerine Microsoft Iş ortağı merkezleri sağlanır, ancak CRM ortamınıza göre alanları daha fazla özelleştirmeyi tercih edebilirsiniz.

Her bir güç otomatikleştirme akışının birden çok adımı gereksinimlerinize göre özelleştirilebilir. Aşağıdakiler kullanılabilir özelleştirmeler örneğidir:

1. Iş ortağı merkezindeki oluştur veya Güncelleştir olaylarının CRM başvuru eşitlemesine yönelik alanlarını özelleştirmek için: 

    a. Iş Ortağı Merkezi 'ni Dynamics 365 (Insider Preview) veya Iş Ortağı Merkezi ' ni (Insider Preview) seçin.

    b. Power otomatikleştir akışını düzenlemek/özelleştirmek için **Düzenle** ' yi seçin.

    c. **Müşteri adayını veya fırsatı eşitlemeyi (kapsam)** seçin.

2. Olay oluşturma için CRM alan eşlemelerini (alan eşlemeleri kılavuzuna göre) özelleştirmek için, **Yeni paylaşılan fırsat ' ı seçin ve ardından**. **Evet ise** alt adımı seçin ve ardından **CRM 'de yeni fırsat oluşturma**' yı genişletin. Bu bölümdeki eşlemeleri alan eşleme kılavuzunu kullanarak düzenleyebilirsiniz.

    d. Güncelleştirme olayları için CRM alan eşlemelerini özelleştirmek için (alan eşlemeleri kılavuzuna göre), "(kapsam) müşteri adayını veya fırsatı eşitlemeyi" adımına tıklayın.

    e. Bir **fırsata yönelik güncelleştirme olup olmadığını seçin, sonra**. **Evet ise** alt adımı seçin ve ardından **iş ortağı merkezi ve CRM 'deki fırsat nesneleri arasında fark olursa** öğesini genişletin.  

    f. **Mevcut fırsatı Güncelleştir** ' in ardından **Evet** ' i seçin

3. CRM için alanları güncelleştirme olayları için başvuru eşitlemesine göre özelleştirmek için:

    a. Power otomatikleştir akışını düzenlemek/özelleştirmek için **Düzenle**  ' yi seçin.

    b. **Fırsatı (kapsam) eşitlemeyi** seçin.

    c. Güncelleştirme olayları için CRM alan eşlemelerini özelleştirmek için, **Iş ortağı merkezi ve CRM 'deki lider nesneleri arasında fark olup olmadığını** seçin. 

    d. **Evet ise** alt adımı seçin ve ardından **fırsat verileriyle bir başvuruyu güncelleştir** adımını genişletin.

   Bu bölümdeki eşlemeleri alan eşleme kılavuzuna göre düzenleyebilirsiniz.

4. CRM için alanları, oluşturma olayları için bir BILGISAYAR başvurusu eşitlemesine göre özelleştirmek için?

   a. Power otomatikleştir akışını düzenlemek/özelleştirmek için **Düzenle**  ' yi seçin.

   b. **Başvuruları eşitleme (kapsam)** seçeneğini belirleyin.

   c. Olay oluşturma için CRM alan eşlemelerini özelleştirmek için (alan eşlemeleri kılavuzuna göre) **Microsoft başvurusu oluştur**' u seçin.

   Bu bölümdeki eşlemeleri alan eşleme kılavuzuna göre düzenleyebilirsiniz.

Oluşturulan iki ortam değişkeni vardır:

- Onay işareti: Iş ortağı merkezi ve Dynamics 365 CRM arasında çift yönlü olarak eşitlenen fırsatların yanı sıra onay işareti simgesi gerekip gerekmediğini belirtir.

- Yalnızca ortak satış fırsatlarını eşitleyin: yalnızca ortak satış fırsatlarını eşitlemek isteyip istemediğinizi belirtir.

Ortam değişkenleri için varsayılan değeri düzenlemeyi seçebilirsiniz.

:::image type="content" source="images/cosellconnectors/dynamics5.png" alt-text="Varsayılan değerler için düzenleme kutusu":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Uçtan uca iki yönlü ortak satış başvuru eşitlemesi

Power otomatikleştir çözümünü yükledikten, yapılandırdıktan ve özelleştirdikten sonra, Dynamics 365 ve Iş ortağı merkezi arasında ortak satış başvuruları eşitlemesini test edebilirsiniz.

### <a name="pre-requisites"></a>Ön koşullar

Iş ortağı merkezi ve Dynamics 365 CRM arasındaki başvuruları eşleştirmek için, Power otomatikleştir çözümü, Microsoft 'a özgü başvuru alanlarını açıkça ortadan kaldırır. Bu kimlik, satıcı ekiplerine ortak satış için Microsoft ile hangi referansları paylaşmak istediğini belirleme olanağı sağlar.

**Fırsat** varlığının bir parçası olarak bir dizi özel alan mevcuttur. Bir CRM yönetici kullanıcısının **fırsat** özel alanlarıyla ayrı bir CRM bölümü oluşturması gerekir.

Aşağıdaki özel alanlar CRM bölümünün bir parçası olmalıdır:

- **Iş Ortağı Merkezi Ile Eşitle**: fırsatın Microsoft Iş Ortağı Merkezi ile eşitlenmeyeceğini belirtir

- **Başvuru tanımlayıcısı**: Microsoft Iş Ortağı Merkezi başvurusu için salt okunurdur bir tanımlayıcı alanı

- **Başvuru bağlantısı**: Microsoft Iş Ortağı Merkezi 'nde başvuruya yönelik salt okunurdur bir bağlantı

- **Microsoft nasıl yardım edebilir?**: başvuru için Microsoft 'un gerekli olduğu yardım

- **Ürünler**: Bu fırsatla ilişkili ürünlerin listesi

- **Denetim**: Iş Ortağı Merkezi başvurularına eşitleme için salt okunurdur bir denetim izi

Dynamics 365 CRM 'deki fırsat formunu ürün çözümlerini içerecek şekilde güncelleştirin.

:::image type="content" source="images/cosellconnectors/dynamics6.png" alt-text="Fırsat formu":::

:::image type="content" source="images/cosellconnectors/dynamics7.png" alt-text="{alternatif-metin}":::

### <a name="scenarios"></a>LARLA

1. CRM 'de başvuru oluşturulduğunda veya güncelleştirilirken ve Iş Ortağı Merkezi 'nde eşitlendiğinde başvuru eşitlemesi:

   1. Dynamics 365 CRM ortamınızda, CRM 'nin **fırsat** bölümünde görünürlük olan kullanıcıyla oturum açın.

   2. Dynamics 365 ortamında "yeni fırsat" oluşturduğunuzda aşağıdaki bölümün mevcut olduğundan emin olun.

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Dynamics 365 ' de Microsoft Iş Ortağı Merkezi bilgilerini gösteren örnek fırsat bölümü.":::

   3. Bu fırsatı Microsoft Iş Ortağı Merkezi ile eşleştirmek için, kart görünümünde aşağıdaki alanları ayarlamış olduğunuzdan emin olun:

      - **Iş Ortağı Merkezi Ile Eşitle**: Evet

      - **Microsoft nasıl yardım edebilir?**: aşağıdakilerden seçim yapın:

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Dynamics 365 ' de, Microsoft 'un nasıl yardım edebilir adlı bir alanın yanında Microsoft Iş Ortağı Merkezi yardım seçeneklerini gösteren örnek fırsat bölümü.":::

      - **Ürünler**: ürünün çözüm kimlikleri

   4. Fırsat Dynamics 365 ' de **Iş Ortağı Merkezi Ile Eşitle** seçeneği **Evet** olarak ayarlandığında, 10 dakika bekleyin ve ardından iş ortağı Merkezi hesabınızda oturum açın. Başvurularınız Dynamics 365 ile eşitlenir.

   5. Benzer şekilde, "Partner Center ile eşitleme" seçeneği "Evet" olarak ayarlanmış bir fırsat için, Dynamics 365 CRM 'de fırsatı güncelleştirirseniz değişiklikler Iş Ortağı Merkezi hesabınızda eşitlenir.

   6. Iş Ortağı Merkezi ile başarıyla eşitlenen fırsatlar, Dynamics 365 ' de ✔ simgesiyle tanımlanır.

2. Microsoft Iş Ortağı Merkezi 'nde başvuru oluşturulduğunda veya güncelleştirilirken ve Dynamics 365 ortamında eşitlendiğinde başvuru eşitlemesi:

   1. Iş Ortağı Merkezi [panonuzda](https://partner.microsoft.com/dashboard/home)oturum açın.

   2. Sol taraftaki menüden **referanslar** ' ı seçin.

   3. "Yeni anlaşma" seçeneğine tıklayarak Iş Ortağı Merkezi 'nden yeni bir ortak satış başvurusu oluşturun.

   4. Dynamics 365 CRM ortamınızda oturum açın.

   5. **Açık fırsatlara** gidin. Microsoft Iş Ortağı Merkezi 'nde oluşturulan başvuru artık Dynamics 365 CRM 'de eşitlendi.

   6. Eşitlenmiş bir başvuruyu seçtiğinizde, kart Görünümü ayrıntıları doldurulur.

## <a name="next-steps"></a>Sonraki adımlar

- [Müşteri adaylarını yönetme](manage-leads.md)

- [Ortak satış fırsatlarını yönetme](manage-co-sell-opportunities.md)

- [Microsoft Power otomatikleştir platformu hakkında daha fazla bilgi](/power-automate/)

- [İş Ortağı Merkezi Web kancaları](/partner-center/develop/partner-center-webhooks)