---
title: Salesforce CRM Iş Ortağı Merkezi için ortak satış Bağlayıcısı
ms.topic: how-to
ms.date: 09/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Iş ortağı merkezindeki başvurularınızı Salesforce CRM 'niz ile eşitler. Satıcılar daha sonra CRM sistemlerinizden Microsoft ile ortak bir şekilde satıtabilecekleri.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 4b3817dafbd05edf0c50b062b52ac4814c767d04
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/14/2020
ms.locfileid: "92531894"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Salesforce için ortak satış Bağlayıcısı CRM-genel bakış

### <a name="appropriate-roles"></a>Uygun roller

- Başvuru Yöneticisi
- CRM 'de Sistem Yöneticisi veya sistem özelleştiricisi

İş Ortağı Merkezi ortak satış Bağlayıcısı, satıcılarınızın CRM sistemlerinizden Microsoft ile ortak satıtabmasını sağlar. Ortak satış kurdukları anlaşmaları yönetmek için Iş Ortağı Merkezi 'ni kullanmaya eğitilmeleri gerekmez. Ortak satış bağlayıcılarını kullanarak, Microsoft satıcı 'ya yönelik yeni bir ortak satış başvurusu oluşturabilir, Microsoft satıcı ile başvuruları alabilir, başvuruları kabul edebilir/reddedebilir, anlaşma değeri gibi işlem verilerini değiştirebilir ve kapanış tarihi gibi işlemleri yapabilirsiniz.  Ayrıca, bu ortak satış konusunda Microsoft satıcılarından herhangi bir güncelleştirme de alabilirsiniz. İş Ortağı Merkezi yerine tercih ettiğiniz CRM 'de çalışırken tüm başvurularınızı yapabilirsiniz. 

Çözüm, Microsoft Power otomatikleştir çözümüne dayalıdır ve Iş Ortağı Merkezi API 'Lerini kullanır.

## <a name="before-you-install---pre-requisites"></a>Yüklemeden önce önkoşulları

|**Konu başlıkları**   |**Ayrıntılar**   |**Bağlantılar**   |
|--------------|--------------------|------|
|Microsoft İş Ortağı Ağı KIMLIĞI |Geçerli bir MPN KIMLIĞI gerekir|[MPN](https://partner.microsoft.com/) 'ye katılması için|
|Ortak satış hazırlanıyor|IP/hizmet çözümünüz ortak satış için hazırlık olmalıdır.|[Microsoft ile satış](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|İş Ortağı Merkezi hesabı|Iş Ortağı Merkezi kiracısı ile ilişkili MPN KIMLIĞI, ortak satış çözümünüz ile ilişkili MPN KIMLIĞIYLE aynı olmalıdır. Bağlayıcıları dağıtmadan önce Iş Ortağı Merkezi portalındaki ortak satış başvurularınızı görebildiğinizi doğrulayın.|[Hesabınızı yönetme](create-user-accounts-and-set-permissions.md)|
|İş Ortağı Merkezi Kullanıcı rolleri|Bağlayıcıları yükleyecek ve kullanacak çalışana bir başvuru Yöneticisi olmalıdır|[Kullanıcı rollerini ve izinlerini atama](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|CRM Kullanıcı rolü, Sistem Yöneticisi veya sistem özelleştiricisi|[Salesforce CRM 'de rol atama](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Güç otomatikleştirme akış hesabı|CRM Sistem Yöneticisi veya sistem özelleştirici için etkin bir [Güç otomatikleştirme](https://flow.microsoft.com) hesabı. Bu kullanıcının, yüklemeden önce en az bir kez [Power otomatikleştirmek](https://flow.microsoft.com) için oturum açması gerekir.|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Microsoft özel alanları için Salesforce paketi yüklemesi 

Iş ortağı merkezi ve Salesforce CRM arasındaki başvuruları eşleştirmek için, Power otomatikleştir çözümünün Microsoft 'a özgü başvuru alanlarını açıkça tanımlaması gerekir. Bu düzenleme, iş ortağı satıcı ekiplerine ortak satış için Microsoft ile hangi başvuruları paylaşacağına karar verme olanağı sunar.

1. Salesforce 'ta **notları** etkinleştirin ve fırsatlar ilgili listesine ekleyin. 
[Başvuru](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. Aşağıdaki adımları izleyerek **fırsat ekiplerini** etkinleştirin: 
    - Kurulum 'da, fırsat ekibi ayarlarını bulmak için **hızlı bul** kutusunu kullanın.
    - Ayarları gerektiği gibi tanımlayın.
[Başvuru](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. Salesforce 'ta, aşağıdaki paket yükleyicisi 'ni kullanarak özel alanlar ve nesneler yükleme.
  
Paketi herhangi bir şirkete yüklemek için [buraya](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) gidin:


Note: bir korumalı alana yüklüyorsanız, URL 'nin başlangıçtaki bölümünü ile değiştirmelisiniz http://test.salesforce.com

4. Salesforce. Microsoft çözümlerini **fırsatla** ilgili listeye ekleyin. Eklendikten sonra, **wrancon** simgesine ve güncelleştirme özelliklerine tıklayın

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

4. Üstteki menüde **AppSource aç** bağlantısına tıklayın.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource 'u aç":::

5. Açılır ekranda **Salesforce Için Iş Ortağı Merkezi başvuruları bağlayıcıları** arayın.  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="AppSource 'u aç":::

6. **Şimdi al** düğmesine tıklayın ve ardından **devam edin** .

7. Bu, uygulamayı yüklemek için Salesforce CRM ortamını seçebileceğiniz sayfayı açar.  Hüküm ve koşulları kabul edin.

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="AppSource 'u aç" na gidin. **Yükleme zamanlandı** , Iş Ortağı Merkezi başvuruları çözümünün yanında görünmelidir. Yükleme, 10-15 dakika sürer.

9. Yükleme tamamlandıktan sonra [Power otomatikleştirmeye](https://flow.microsoft.com) dönün ve sol gezinti alanından **çözümler** ' i seçin. **Salesforce Için Iş Ortağı Merkezi başvuruları** , çözümler listesinden kullanılabilir olduğuna dikkat edin.

10. **Salesforce Için Iş Ortağı Merkezi başvuruları eşitlemesini** seçin. Aşağıdaki güç otomatikleşme akışları ve varlıkları mevcuttur:

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="AppSource 'u aç":::



## <a name="configure-the-solution"></a>Çözümü yapılandırma

1. Çözümü CRM Örneğinizde yükledikten sonra [Power otomatikleştirmek](https://flow.microsoft.com/)' a geri gidin.

2. Sağ üst köşedeki **ortamlar** açılan penceresinden, Power otomatikleştir çözümünü yüklediğiniz CRM örneğini seçin.
3. Üç Kullanıcı hesabını ilişkilendiren bağlantılar oluşturmanız gerekir:
    - Ortak Merkezi Kullanıcı başvuruları yönetici kimlik bilgileri
    - İş Ortağı Merkezi Etkinlikleri
    - Çözüm içindeki Power otomatikleştirmede CRM Yöneticisi.
4. Sol gezinti çubuğundan **Bağlantılar** ' ı seçin ve listeden "Iş Ortağı Merkezi başvuruları" çözümünü seçin.

5. **Bağlantı oluştur** ' a tıklayarak bir bağlantı oluşturun.

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="AppSource 'u aç":::

- Sağ üst köşedeki arama çubuğunda Iş Ortağı Merkezi başvurularını (Önizleme) arayın.

- Iş Ortağı Merkezi kullanıcılarınız için, başvuru yöneticisinin kimlik bilgileri rolüyle bir bağlantı oluşturun.

-  Daha sonra, Iş Ortağı Merkezi kullanıcılarınız için, referanslar yöneticisinin kimlik bilgileriyle bir Iş Ortağı Merkezi olaylar bağlantısı oluşturun.

- CRM yönetici kullanıcısı için Common Data Service (geçerli ortam) bağlantısı oluşturun.

-  Tüm bağlantılar eklendikten sonra ortamınızda aşağıdaki bağlantıları görmeniz gerekir:

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="AppSource 'u aç":::

### <a name="edit-the-connections"></a>Bağlantıları düzenleme

1. Çözümler sayfasına dönün ve **Varsayılan çözüm** ' ı seçin.  **Tüm** ' a tıklayarak **Bağlantı başvurusunu (Önizleme)** seçin.
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="AppSource 'u aç":::

2. Üç nokta simgesini seçerek bağlantıların her birini tek tek düzenleyin. İlgili bağlantıları ekleyin.

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="AppSource 'u aç":::

3. Akışları aşağıdaki sırada açın:

- İş Ortağı Merkezi Web kancası kaydı (Insider Preview)
- Ortak satış başvurusu oluşturma-Salesforce 'a Iş Ortağı Merkezi 'ne (Insider Preview)
- İş Ortağı Merkezi Microsoft ortak-başvuru güncelleştirmelerini Salesforce 'a satma (Insider Preview)
- İş ortağı merkezini Salesforce 'a (Insider Preview)
- Salesforce-Iş Ortağı Merkezi (Insider Preview)
- Salesforce Iş Ortağı Merkezi (Insider Preview)
- Salesforce Microsoft çözümlerini Iş Ortağı Merkezi 'ne (Insider Preview)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Kaynak değişikliği olaylarına kaydolmak için Web kancası API 'Lerini kullanma

Iş Ortağı Merkezi Web kancası API 'Leri, kaynak değişiklik olaylarına kaydolmanızı sağlar. Bu değişiklik olayları, URL 'nize HTTP gönderileri olarak gönderilir.

1. URL 'nizi kaydetmek için **Iş Ortağı Merkezi Web kancası kaydı (Insider Preview)** güç otomatikleştirme akışı ' nı seçin.

2. (A.) Iş Ortağı Merkezi kullanıcısına, aşağıdaki vurgulanmış şekilde, başvuru Yöneticisi kimlik bilgileri (b.) Iş Ortağı Merkezi etkinliklerine yönelik bağlantılar ekleyin

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="AppSource 'u aç":::

3. Bu güncelleştirmeleri yaptığınızda şunu görürsünüz:

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="AppSource 'u aç":::

4. Değişikliklerinizi kaydedin ve **Aç '** ı seçin.

   Iş Ortağı Merkezi Web kancalarını olay değişikliklerini dinleyecek şekilde etkinleştirmek için aşağıdaki adımları uygulayın:

5. **Iş ortağı merkezini SALESFORCE CRM 'ye (Insider Preview)** seçin.

6. **Düzenle** simgesini seçin ve **bir http isteği alındığında** öğesini seçin.

7. Belirtilen HTTP POST URL 'sini kopyalamak için **Kopyala** simgesini seçin.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="AppSource 'u aç"

    3. Varsa **var olan tetikleyici uç noktalarının üzerine yaz** : Evet (Bu, mevcut tüm uç noktaların üzerine yazar.)

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

2. Olay oluşturma için CRM alan eşlemelerini özelleştirmek için, **Yeni paylaşılan fırsat ' ı seçin ve ardından** . **Evet ise** alt adımı seçin ve ardından **CRM 'de yeni fırsat oluşturma** ' yı genişletin. Bu bölümdeki eşlemeleri alan eşleme kılavuzunu kullanarak düzenleyebilirsiniz.

   1. Güncelleştirme olayları için CRM alan eşlemelerini özelleştirmek için "(kapsam) müşteri adayını veya fırsatı eşitlemeyi" adımına tıklayın.

   2. Bir **fırsata yönelik güncelleştirme olup olmadığını seçin, sonra** . **Evet ise** alt adımı seçin ve ardından **iş ortağı merkezi ve CRM 'deki fırsat nesneleri arasında fark olursa** öğesini genişletin.  

   3. **Mevcut fırsatı Güncelleştir** ' in ardından **Evet** ' i seçin

3. CRM için alanları güncelleştirme olayları için başvuru eşitlemesine göre özelleştirmek için:

   1. Power otomatikleştir akışını düzenlemek/özelleştirmek için **Düzenle**  ' yi seçin.

   2. **Fırsatı (kapsam) eşitlemeyi** seçin.

   3. Güncelleştirme olayları için CRM alan eşlemelerini özelleştirmek için (alan eşlemeleri kılavuzuna göre), **Iş ortağı merkezi ve CRM 'deki lider nesneleri arasında fark olup olmadığını** seçin.

   4. **Evet ise** alt adımı seçin ve ardından **fırsat verileriyle bir başvuruyu güncelleştir** adımını genişletin.

   Bu bölümdeki eşlemeleri alan eşleme kılavuzuna göre düzenleyebilirsiniz.

4. CRM için alanları, oluşturma olayları için bir BILGISAYAR başvurusu eşitlemesine göre özelleştirmek için?

   1. Power otomatikleştir akışını düzenlemek/özelleştirmek için **Düzenle**  ' yi seçin.

   2. **Başvuruları eşitleme (kapsam)** seçeneğini belirleyin.

   3. Olay oluşturma için CRM alan eşlemelerini özelleştirmek için (alan eşlemeleri kılavuzuna göre) **Microsoft başvurusu oluştur** ' u seçin.

Bu bölümdeki eşlemeleri alan eşleme kılavuzuna göre düzenleyebilirsiniz.


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Uçtan uca iki yönlü ortak satış başvuru eşitlemesi

Power otomatikleştir çözümünü yükledikten, yapılandırdıktan ve özelleştirdikten sonra Salesforce CRM ve Iş ortağı merkezi arasında ortak satış başvuruları eşitlemesini test edebilirsiniz.

### <a name="pre-requisites"></a>Ön koşullar

Iş ortağı merkezi ve Salesforce CRM genelindeki başvuruları senkronize etmek için, Power otomatikleştir çözümünün Microsoft 'a özgü başvuru alanlarını açıkça ortadan kaldırma ihtiyacı vardır. Bu kimlik, satıcı ekiplerinizi, ortak satış için Microsoft ile hangi referansları paylaşmak istediğlerine karar vermenize olanak sağlar.

Bir dizi özel alan, Salesforce CRM çözümü **fırsat** varlığı Için Iş Ortağı Merkezi başvuruları eşitlemesinin bir parçası olarak kullanılabilir. Bir CRM yönetici kullanıcısının **fırsat** özel alanlarıyla ayrı bir CRM bölümü oluşturması gerekir.

Aşağıdaki özel alanlar CRM bölümünün bir parçası olmalıdır:

- **Iş Ortağı Merkezi Ile Eşitle** : fırsatın Microsoft Iş Ortağı Merkezi ile eşitlenmeyeceğini belirtir

- **Başvuru tanımlayıcısı** : Microsoft Iş Ortağı Merkezi başvurusu için salt okunurdur bir tanımlayıcı alanı

- **Başvuru bağlantısı** : Microsoft Iş Ortağı Merkezi 'nde başvuruya yönelik salt okunurdur bir bağlantı

- **Microsoft 'un yardımı** : başvuru için Microsoft 'un gerekli yardımı

- **Ürünler** : Bu fırsatla ilişkili ürünlerin listesi

- **Denetim** : Iş Ortağı Merkezi başvurularına eşitleme için salt okunurdur bir denetim izi

### <a name="scenarios"></a>LARLA

1. CRM 'de başvuru oluşturulduğunda veya güncelleştirilirken ve Iş Ortağı Merkezi 'nde eşitlendiğinde başvuru eşitlemesi:

   1. CRM 'nin **fırsat** bölümünde görünürlük olan KULLANıCıYLA Salesforce CRM ortamınızda oturum açın.

   2. Salesforce CRM ortamında "yeni fırsat" oluşturduğunuzda aşağıdaki bölümün mevcut olduğundan emin olun.

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="AppSource 'u aç" seçeneğine tıklayarak Iş Ortağı Merkezi 'nden yeni bir ortak satış başvurusu oluşturun.

    4. Salesforce CRM ortamınızda oturum açın.

    5. **Açık fırsatlara** gidin. Microsoft Iş Ortağı Merkezi 'nde oluşturulan başvuru artık Salesforce CRM 'de eşitlendi.

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="AppSource 'u aç":::

    6. Eşitlenmiş bir başvuruyu seçtiğinizde, kart Görünümü ayrıntıları doldurulur.

## <a name="next-steps"></a>Sonraki adımlar

- [Müşteri adaylarını yönetme](manage-leads.md)

- [Ortak satış fırsatlarını yönetme](manage-co-sell-opportunities.md)

- [İş Ortağı Merkezi Web kancaları](/partner-center/develop/partner-center-webhooks)