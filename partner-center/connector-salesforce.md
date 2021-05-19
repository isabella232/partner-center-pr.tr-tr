---
title: Salesforce CRM Iş Ortağı Merkezi için ortak satış Bağlayıcısı
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Iş ortağı merkezindeki başvurularınızı Salesforce CRM 'niz ile eşitler. Satıcılar daha sonra CRM sistemlerinizden Microsoft ile ortak bir şekilde satıtabilecekleri.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: fa9b35343e1251cfce5caff107de8dff344f4e68
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148423"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Salesforce için ortak satış Bağlayıcısı CRM-genel bakış

**Uygun roller**: başvuru Yöneticisi | CRM 'de Sistem Yöneticisi veya sistem özelleştiricisi

İş Ortağı Merkezi ortak satış Bağlayıcısı, satıcılarınızın CRM sistemlerinizden Microsoft ile ortak satıtabmasını sağlar. Ortak satış kurdukları anlaşmaları yönetmek için Iş Ortağı Merkezi 'ni kullanmaya eğitilmeleri gerekmez. Ortak satış bağlayıcılarını kullanarak, Microsoft satıcı 'ya yönelik yeni bir ortak satış başvurusu oluşturabilir, Microsoft satıcı ile başvuruları alabilir, başvuruları kabul edebilir/reddedebilir, anlaşma değeri gibi işlem verilerini değiştirebilir ve kapanış tarihi gibi işlemleri yapabilirsiniz.  Ayrıca, bu ortak satış konusunda Microsoft satıcılarından herhangi bir güncelleştirme de alabilirsiniz. İş Ortağı Merkezi yerine tercih ettiğiniz CRM 'de çalışırken tüm başvurularınızı yapabilirsiniz. 

Çözüm, Microsoft Power otomatikleştir çözümüne dayalıdır ve Iş Ortağı Merkezi API 'Lerini kullanır.

## <a name="before-you-install---pre-requisites"></a>Yüklemeden önce önkoşulları

|**Konu başlıkları**   |**Ayrıntılar**   |**Bağlantılar**   |
|--------------|--------------------|------|
|Microsoft İş Ortağı Ağı KIMLIĞI |Geçerli bir MPN KIMLIĞI gerekir|[MPN](https://partner.microsoft.com/) 'ye katılması için|
|Ortak satış hazırlanıyor|IP/hizmet çözümünüz ortak satış için hazırlık olmalıdır.|[Microsoft ile satış](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|İş Ortağı Merkezi hesabı|Iş Ortağı Merkezi kiracısı ile ilişkili MPN KIMLIĞI, ortak satış çözümünüz ile ilişkili MPN KIMLIĞIYLE aynı olmalıdır. Bağlayıcıları dağıtmadan önce Iş Ortağı Merkezi portalındaki ortak satış başvurularınızı görebildiğinizi doğrulayın.|[Hesabınızı yönetme](create-user-accounts-and-set-permissions.md)|
|İş Ortağı Merkezi rollerini atama|Bağlayıcıları yükecek ve kullanacak olan çalışanın Referans yöneticisi olması gerekir|[Kullanıcı rollerini ve izinlerini atama](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|CRM kullanıcı rolü Sistem yöneticisi veya Sistem özelleştiricisi|[Salesforce CRM'de rol atama](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Power Automate Flow Hesabı|CRM [Sistem Power Automate](https://flow.microsoft.com) veya Sistem özelleştiricisi için etkin bir hesap. Bu kullanıcının yüklemeden önce [Power Automate](https://flow.microsoft.com) kez oturum açması gerekir.|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Microsoft Özel Alanları için Salesforce Paketini Yükleme 

İş Ortağı Merkezi ve Salesforce CRM'de referansları eşitlemek için Power Automate çözümün Microsoft'a özgü referans alanlarını net bir şekilde tanımlaması gerekir. Bu karar, iş ortağı satıcı ekiplerine ortak satış için Microsoft ile paylaşmak istediğiniz referansları verme olanağı sağlar.

1. Salesforce'ta **Notlar'ı** etkinleştirin ve fırsatlarla ilgili listeye ekleyin. 
[Başvuru](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. Aşağıdaki **adımları kullanarak** Fırsat ekiplerini etkinleştirin: 
    - Kurulum'da, Fırsat **Ekibi Ayarları'nı** bulmak için Hızlı Bul kutusunu kullanın.
    - Ayarları gereken şekilde tanımlayın.
[Başvuru](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. Salesforce'ta, paket yükleyicisini kullanarak özel alanlar ve [nesneler yükleyin.](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV) Paketi herhangi bir şirkete yüklemek için bunu kullanın.

>[!NOTE]
>Korumalı alanı yüklüyorsanız URL'nin ilk bölümünü ile değiştirmeniz gerekir http://test.salesforce.com

4. Salesforce'ta Microsoft Solutions'u **Fırsatla ilgili listesine** ekleyin. Eklendiktan sonra, İngiliz anahtarı **simgesini** seçin ve özellikleri güncelleştirin

## <a name="best-practice-test-before-you-go-live"></a>En iyi yöntem: canlı çalışmadan önce test edin

Üretim ortamında güç otomatikleştirme çözümünü yüklemeden, yapılandırmadan ve özelleştirebilmeniz için, çözümü bir hazırlama CRM örneğinde test ettiğinizden emin olun.

- Microsoft Power otomatikleştir çözümünü hazırlama ortamına/CRM örneğine yükler.

- Çözümün bir kopyasını oluşturun ve yapılandırma ve Power otomatikleştir akış özelleştirmelerinizi hazırlama ortamında çalıştırın.

- Çözümü bir hazırlama/CRM örneğinde test edin.

- Başarı durumunda, üretim örneğine yönetilen bir çözüm olarak içeri aktarın.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Salesforce CRM için Iş ortağı merkezi başvuru eşitlemesini yükler

1. [Power otomatikleştirir](https://flow.microsoft.com) ' a gidin ve sağ üst köşedeki **ortamlar** ' ı seçin. Bu, size kullanılabilir CRM örneklerini gösterir.

2. Sağ üst köşedeki açılan listeden uygun CRM örneğini seçin.

3. Sol gezinti çubuğunda **çözümler** ' i seçin.

4. Üstteki menüde **AppSource 'U aç** bağlantısını seçin.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource 'u aç":::

5. Açılır ekranda **Salesforce Için Iş Ortağı Merkezi başvuruları bağlayıcıları** arayın.  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. **Şimdi al** düğmesini seçin ve sonra **devam edin**.

7. Bu, uygulamayı yüklemek için Salesforce CRM ortamını seçebileceğiniz sayfayı açar.  Hüküm ve koşulları kabul edin.

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Kullanılabilir CRMS 'ler":::

8. Daha sonra **çözümlerinizi yönetme** sayfasına yönlendirilirsiniz.  Sayfanın alt kısmındaki ok düğmelerini kullanarak "Iş Ortağı Merkezi başvuruları" na gidin. **Zamanlanan yükleme,** Referanslar çözümünün İş Ortağı Merkezi görün gerekir. Yükleme 10-15 dakika sürer.

9. Yükleme tamamlandıktan sonra çalışma alanına geri Power Automate sol [gezinti](https://flow.microsoft.com) **alanında Çözümler'i** seçin. **Salesforce İş Ortağı Merkezi Referans Eşitlemesi'nin** Çözümler listesinde kullanılabilir olduğunu fark edin.

10. **Salesforce İş Ortağı Merkezi Referans Eşitleme'yi seçin.** Aşağıdaki Power Automate ve varlıklar kullanılabilir:

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce akışları":::



## <a name="configure-the-solution"></a>Çözümü yapılandırma

1. Çözümü CRM örneğine yüklekten sonra [Power Automate.](https://flow.microsoft.com/)

2. Sağ **üst** köşedeki Ortamlar açılan listesinden, Power Automate çözümünü yüklemiş Power Automate seçin.
3. Üç kullanıcı hesabını ilişkilendirilen bağlantılar oluşturmanız gerekir:
    - İş Ortağı Merkezi yönetici kimlik bilgilerine sahip bir kullanıcı
    - İş Ortağı Merkezi Etkinlikleri
    - Çözümde akış Power Automate CRM yöneticisi.
4. Sol **gezinti** çubuğundan Bağlantılar'ı seçin ve listeden "İş Ortağı Merkezi Referanslar" çözümünü seçin.

5. Bağlantı oluştur'a **tıklayarak bağlantı oluşturun.**

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Bağlantı oluşturma":::

- Sağ İş Ortağı Merkezi arama çubuğunda Referanslar (önizleme) araması gerçekleştirin.

- Referans yöneticisinin kimlik bilgileri İş Ortağı Merkezi kullanıcınız için bir bağlantı oluşturun.

-  Ardından, referans İş Ortağı Merkezi kimlik bilgileriyle İş Ortağı Merkezi için bir Olay bağlantısı oluşturun.

- CRM yönetici kullanıcısı için Salesforce için bir bağlantı oluşturun.

-  Tüm Bağlantılar eklendiktan sonra, ortamınıza aşağıdaki Bağlantıları görüyor gerekir:

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Bağlantıları gözlemle":::

### <a name="edit-the-connections"></a>Bağlantıları düzenleme

1. Çözümler sayfasına geri dönüp Varsayılan **Çözüm'i seçin.**  Tüm **'e tıklayarak Bağlantı Başvurusu (önizleme)** **öğesini seçin.**
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Bağlayıcı düzenlemeye başlama":::

2. Üç nokta simgesini seçerek Bağlantılar'ın her bir öğesini tek tek düzenleyin. İlgili bağlantıları ekleyin.

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Bağlayıcıları düzenleme":::

3. Akışları aşağıdaki sırayla aç:

- İş Ortağı Merkezi Web Kancası Kaydı (Insider Önizlemesi)
- Ortak Satış Referansı Oluşturma - İş Ortağı Merkezi Salesforce (Insider Önizleme)
- İş Ortağı Merkezi Microsoft Ortak Satış Referans Güncelleştirmelerini Salesforce'a (Insider Önizleme) yönlendirme
- İş Ortağı Merkezi'a (Insider Önizleme)
- Salesforce'tan İş Ortağı Merkezi 'a (Insider Önizleme)
- Salesforce Opportunity to İş Ortağı Merkezi (Insider Preview)
- İş Ortağı Merkezi için Salesforce Microsoft Solutions (Insider Önizleme)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Kaynak değişikliği olaylarını kaydetmek için Web Kancası API'lerini kullanma

Web İş Ortağı Merkezi API'leri, kaynak değişikliği olaylarına kaydolmaya olanak sağlar. Bu değişiklik olayları URL'nize HTTP gönderileri olarak gönderilir.

1. URL'nizi kaydetmek için Web **Kancası İş Ortağı Merkezi (Insider Önizleme) Power Automate** seçin.

2. (A.) Iş Ortağı Merkezi kullanıcısına, aşağıdaki vurgulanmış şekilde, başvuru Yöneticisi kimlik bilgileri (b.) Iş Ortağı Merkezi etkinliklerine yönelik bağlantılar ekleyin

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Tetikleyici":::

3. Bu güncelleştirmeleri yaptığınızda şunu görürsünüz:

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Web Kancaları":::

4. Değişikliklerinizi kaydedin ve **Aç '** ı seçin.

   Iş Ortağı Merkezi Web kancalarını olay değişikliklerini dinleyecek şekilde etkinleştirmek için aşağıdaki adımları uygulayın:

5. **Iş ortağı merkezini SALESFORCE CRM 'ye (Insider Preview)** seçin.

6. **Düzenle** simgesini seçin ve **bir http isteği alındığında** öğesini seçin.

7. Belirtilen HTTP POST URL 'sini kopyalamak için **Kopyala** simgesini seçin.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="URL'yi Kopyala":::

8. Şimdi "Iş Ortağı Merkezi Web kancası kaydı 'nı (Insider Preview)" Power otomatikleştirmeyi seçin ve **Çalıştır**' ı seçin.

9. Sağ bölmede "akış Çalıştır" penceresinin açık olduğundan emin olun ve **devam**' ı seçin.

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

   1. Iş ortağı merkezini Salesforce CRM 'ye (Insider Preview) seçin.

   2. Power otomatikleştir akışını düzenlemek/özelleştirmek için **Düzenle** ' yi seçin.

   3. **Müşteri adayını veya fırsatı eşitlemeyi (kapsam)** seçin.

2. Olay oluşturma için CRM alan eşlemelerini özelleştirmek için, **Yeni paylaşılan fırsat ' ı seçin ve ardından**. **Evet ise** alt adımı seçin ve ardından **CRM 'de yeni fırsat oluşturma**' yı genişletin. Bu bölümdeki eşlemeleri alan eşleme kılavuzunu kullanarak düzenleyebilirsiniz.

   1. Güncelleştirme olayları için CRM alan eşlemelerini özelleştirmek için "(kapsam) müşteri adayını veya fırsatı eşitlemeyi" adımını seçin.

   2. Bir **fırsata yönelik güncelleştirme olup olmadığını seçin, sonra**. **Evet ise** alt adımı seçin ve ardından **iş ortağı merkezi ve CRM 'deki fırsat nesneleri arasında fark olursa** öğesini genişletin.  

   3. **Mevcut fırsatı Güncelleştir** ' in ardından **Evet** ' i seçin

3. CRM için alanları güncelleştirme olayları için başvuru eşitlemesine göre özelleştirmek için:

   1. Power otomatikleştir akışını düzenlemek/özelleştirmek için **Düzenle**  ' yi seçin.

   2. **Fırsatı (kapsam) eşitlemeyi** seçin.

   3. Güncelleştirme olayları için CRM alan eşlemelerini özelleştirmek için (alan eşlemeleri kılavuzuna göre), **Iş ortağı merkezi ve CRM 'deki lider nesneleri arasında fark olup olmadığını** seçin.

   4. **Evet ise** alt adımı seçin ve ardından **fırsat verileriyle bir başvuruyu güncelleştir** adımını genişletin.

   Bu bölümdeki eşlemeleri alan eşleme kılavuzuna göre düzenleyebilirsiniz.

4. CRM için alanları, oluşturma olayları için bir BILGISAYAR başvurusu eşitlemesine göre özelleştirmek için?

   1. Akışı **düzenlemek/özelleştirmek**  için Düzenle'Power Automate seçin.

   2. **(Kapsam) Referansları Eşitle'yi seçin.**

   3. Oluşturma olayları için CRM alan eşlemelerini özelleştirmek için (alan eşlemeleri kılavuzuna göre) **Microsoft Referansı Oluştur'u seçin.**

Bu bölümdeki eşlemeleri Alan Eşleme Kılavuzu'na göre düzenleyebilirsiniz.


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>4- uç çift yönlü ortak satış referans eşitlemesi

Power Automate çözümünü yüklemiş, yapılandırmış ve özelleştirmiş olduktan sonra Salesforce CRM ile İş Ortağı Merkezi arasında ortak satış referans eşitlemesi için test İş Ortağı Merkezi.

### <a name="pre-requisites"></a>Ön koşullar

İş Ortağı Merkezi ve Salesforce CRM'de referansları eşitlemek için Power Automate çözümünün Microsoft'a özgü referans alanlarını net bir şekilde delelenmesi gerekir. Bu kimlik, satış ekibinize ortak satış için Microsoft ile paylaşmak istediğiniz referansları belirleme olanağı sağlar.

Salesforce CRM çözümü fırsat varlığı için Referans Eşitleme İş Ortağı Merkezi bir dizi özel **alan** mevcuttur. CRM yönetici kullanıcısnın Fırsat özel alanlarıyla ayrı bir CRM **bölümü oluşturması** gerekir.

Aşağıdaki özel alanlar CRM bölümünün bir parçası olması gerekir:

- **İş Ortağı Merkezi ile eşitleme:** Fırsatın Microsoft İş Ortağı Merkezi ile eşit İş Ortağı Merkezi

- **Referans Tanımlayıcısı:** Microsoft referans başvurusu için salt İş Ortağı Merkezi alanı

- **Referans Bağlantısı:** Microsoft İş Ortağı Merkezi'de referansın salt okunur bağlantısı

- **Microsoft nasıl yardımcı olabilir:** Referans için Microsoft'tan gereken yardım

- **Ürünler:** Bu fırsatla ilişkili ürünlerin listesi

- **Denetim:** Referanslarla eşitleme için salt okunur bir denetim İş Ortağı Merkezi izi

### <a name="scenarios"></a>Senaryo:

1. Referans CRM'de oluşturulduğunda veya güncelleştirildiğinde ve referansta eşit İş Ortağı Merkezi:

   1. CRM'nin Fırsat bölümünde görünürlüğü olan kullanıcıyla Salesforce CRM **ortamında** oturum açma.

   2. Salesforce CRM ortamında "yeni fırsat" oluşturduğunuzda aşağıdaki bölümün mevcut olduğundan emin olun.

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce ortamı":::

   3. Bu fırsatı Microsoft Iş Ortağı Merkezi ile eşleştirmek için, kart görünümünde aşağıdaki alanları ayarlamış olduğunuzdan emin olun:

       - "Iş Ortağı Merkezi ile Eşitle": Evet
       - "Microsoft nasıl yardım edebilir?": aşağıdaki seçeneklerden seçim yapın:
       - Ürünler: ürünün çözüm kimlikleri

   4. **Iş Ortağı Merkezi ile fırsat eşitlemesi** seçeneğini **Evet** olarak ayarladıktan sonra 10 dakika bekleyin, iş ortağı Merkezi hesabınızda oturum açın. Başvurularınız Salesforce CRM ile eşitlenecek.

   5. "Iş Ortağı Merkezi ile Eşitle" seçeneği "Evet" olarak ayarlandığında, fırsatı Salesforce CRM 'de güncelleştirirseniz, değişiklikler Iş Ortağı Merkezi hesabınızla eşitlenir.

   6. Iş Ortağı Merkezi ile başarıyla eşitlenen fırsatlar, Salesforce CRM 'de ✔ simgesiyle tanımlanır.

2. Microsoft Iş Ortağı Merkezi 'nde başvuru oluşturulduğunda veya güncelleştirilirken ve Salesforce CRM ortamında eşitlendiğinde başvuru eşitlemesi:

    1. Iş Ortağı Merkezi [panonuzda](https://partner.microsoft.com/dashboard/home)oturum açın.

    2. Sol taraftaki menüden **referanslar** ' ı seçin.

    3. "Yeni anlaşma" seçeneğine tıklayarak Iş Ortağı Merkezi 'nden yeni bir ortak satış başvurusu oluşturun.

    4. Salesforce CRM ortamınızda oturum açın.

    5. **Açık fırsatlara** gidin. Microsoft Iş Ortağı Merkezi 'nde oluşturulan başvuru artık Salesforce CRM 'de eşitlendi.

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce fırsat ekranı":::

    6. Eşitlenmiş bir başvuruyu seçtiğinizde, kart Görünümü ayrıntıları doldurulur.

## <a name="next-steps"></a>Sonraki adımlar

- [Müşteri adaylarını yönetme](manage-leads.md)

- [Ortak satış fırsatlarını yönetme](manage-co-sell-opportunities.md)

- [İş Ortağı Merkezi web kancaları](/partner-center/develop/partner-center-webhooks)
