---
title: Iş ortağı satış bağlantısı 'ndan (PSC) geçiş
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft iş ortaklarının iş ortağı satış Connect 'ten (PSC) iş ortağı merkezi 'ne nasıl geçirebileceğini ve Microsoft satıcıları tarafından gönderilen anlaşmalar oluşturma veya yönetme hakkında bilgi edinin.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 12/07/2020
ms.openlocfilehash: bbd2d1035bdcde691b0db620949d0e973667627b
ms.sourcegitcommit: 351c7ff4e6ebbb615a00190b2310156381f9cf03
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/07/2020
ms.locfileid: "96776923"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>İş ortağı satış bağlantısı (PSC) üzerinden geçiş yapan iş ortakları için Iş Ortağı Merkezi 'nde (PC) ortak satış ile ilgili kılavuz

**Uygun roller**

- Hesap yöneticisi
- Başvuru Yöneticisi
- İş ortağı satış bağlantısı (PSC) satıcı
- İş ortağı Sales Connect (PSC) Yöneticisi
- İş ortağı Sales Connect (PSC) anlaşma Yöneticisi

Bu makalede iş ortağı satışları iş ortağı merkezi 'ne geçiş yapan iş ortakları, iş ortağı merkezi 'nde ortak satış anlaşmaları oluşturmaya ve yönetmeye devam edebilirler.

Bildiğiniz gibi şirketiniz, 31 Mart 2021 ' den sonra PSC 'ye erişimi kaybedecektir. Bununla birlikte, Iş Ortağı Merkezi 'nde yapmak istediğiniz her şeyi, ortak satış anlaşmaları oluşturma, anlaşmaları yönetme ve Microsoft satıcıları tarafından size gönderilen anlaşmalar üzerinde işlem yapacak şekilde bulacaksınız.

Ancak farklılıklar olacaktır. Aşağıdaki kılavuz, Iş Ortağı Merkezi 'ne geçişinizi daha sorunsuz ve daha basit hale getirmenize yardımcı olabilir.

>[!Important]
> Buradan geçiş hakkında PSC 'de bir başlık gördüğünüz için doğru yerde olursunuz. Bu kılavuz, PSC 'de anlaşmalar yöneten çözüm değerlendirmesi (SA) ve OEM ıOT iş ortakları için geçerli değildir.

## <a name="before-you-move-things-you-need-to-know"></a>Taşımadan önce bilmeniz gereken şeyler

### <a name="if-you-are-a-psc-admin"></a>Bir PSC yöneticisiyseniz

- İş [Ortağı Merkezi](https://partner.microsoft.com/)'nde oturum açmak için bir iş e-postasına ihtiyacınız vardır.
- Iş Ortağı Merkezi [hesap yöneticisinin](permissions-overview.md)yardımıyla hesabınızı ayarlayın.
- Bu belgeyi okuyarak Iş Ortağı Merkezi 'nde ortak satışı yapmayı öğrenin.
- Tüm PSC kullanıcılarınız (yönetici, anlaşma Yöneticisi ve satıcı rolleri) için Iş Ortağı Merkezi 'nde Kullanıcı hesapları ayarlayın ve bunlara [referans yönetici rolleri](permissions-overview.md)atayın.

>[!IMPORTANT]
> PSC başlığında gösterilen MPN KIMLIĞININ Iş Ortağı Merkezi 'ndeki MPN konumları listesinde bulunduğundan emin olun.

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="İş ortaklarının MPN KIMLIĞINI bulabileceği PSC başlığını gösteren resim.":::

 MPN KIMLIĞININ bir Iş Ortağı Merkezi MPN konumu olarak göründüğünü doğrulamak için Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın, ardından ekranın sağ üst kısmındaki **Ayarlar** (dişli simgesi) ve ardından **Hesap ayarları**' nı seçin. İkinci düzey, sol gezinti menüsünde, Iş Ortağı Merkezi hesabıyla ilişkili tüm MPN kimliklerinin ve konumların listesini görmek için **konumlar** ' ı seçin.

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>Bir PSC anlaşma Yöneticisi veya satıcı

- İş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açmak için bir iş e-postasına ihtiyacınız vardır.
- PSC 'de iş dışı bir hesap kullanıyorsanız veya iş e-postanız iş ortağı şirketten farklı bir şirkette kullanılıyorsa, hesap kurulumu için PSC yöneticinizle iletişime geçin.
- PSC 'de oturum açmak için kullandığınız hesap ne olursa olsun, Iş ortağı merkezi hesap ayarlanmanız durumunda PSC yöneticinizle görüşün.
- Iş Ortağı Merkezi 'ne ve başvurular bölümüne erişiminiz olup olmadığını doğrulayın.
- İş akışlarını ve iş ortağı merkezindeki değişiklikleri anlamak için bu belgeyi okuyun.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>PSC 'de yönetici olarak, bunlar sonraki adımlardır

Iş ortağı merkezi sol gezinti menüsünde, **Başvurular** seçeneğini belirleyin. Başvuru sayfalarına erişebildiğinizden emin olun.

  >[!Note]
  > Iş Ortağı Merkezi oturumunuzu kapatıp başvuru sayfalarına erişim için kimlik bilgilerinizi yenilemek üzere yeniden oturum açmanız gerekebilir.

Iş Ortağı Merkezi menüsünde veya başvurularda ilişkili sayfalarda **Başvurular** seçeneğini görmüyorsanız, şirketinizin [hesap yöneticisine](permissions-overview.md) başvurarak, **Başvurular** seçeneğine ve ilgili alana erişim vermesini isteyin.

Şirketinizin hesap yöneticisini bulmak için:

1. Iş Ortağı Merkezi panosunun sağ üst tarafındaki dişli simgesinden **Hesap ayarları** ' nı seçin.

1. İkinci düzey, sol gezinti menüsünden **Kullanıcı yönetimi** ' ni seçin.

1. Kullanıcı listesinin en üstünde, **filtre** açılan menüsünü seçin. **Hesap Yöneticisi** seçeneğini değiştirin.

   Bu sayfada, tüm hesap yöneticileri ilgili e-posta adresleriyle görüntülenir. Bunlardan birine e-posta gönderin ve iş hesabınız için başvuru Yöneticisi rolünü atamasını isteyin.

  :::image type="content" source="images/pscmigration/account-admin.png" alt-text="İş ortağı ayarları Kullanıcı Yönetimi sayfasında hesap yöneticileri 'ni gösteren resim.":::

>[!Important]
>- Rolünüz yalnızca PSC 'deki kullanıcıları yönetmeyi içeriyorsa, şirketinizin hesap yöneticisinden Iş Ortağı Merkezi 'nde [Hesap Yöneticisi](permissions-overview.md#manage-mpn-membership-and-your-company) rolünü atamasını isteyin. 
>- Rolünüzde ortak satış fırsatlarını yönetme de varsa, [Başvurular yönetici](permissions-overview.md#manage-referrals) rolü atanmasını isteyin.
> - Aynı zamanda PSC yöneticileri arasında bir değişiklik yönetimi liderine aday bir fikir elde etmek iyi bir fikirdir. Bunun yapılması, tüm PSC yöneticilerinin Iş ortağı merkezi hesap yöneticilerine ayrı olarak ulaşmasını önler. Bunun yerine, değişiklik Yönetimi lideri daha sonra Iş ortağı merkezi hesap yöneticisi ile çalışan birincil kişidir.

## <a name="user-migration"></a>Kullanıcı geçişi

Iş Ortağı Merkezi 'nde hesabınızı ayarladıktan sonra, iş ortağı merkezi rollerini şirketinizin çalışanlarına otomatik olarak atamak için ortak satış fırsatları sayfasında Kullanıcı Geçiş Sihirbazı 'nı kullanın.

>[!Note]
> Kullanıcı geçişi yalnızca, şirketinizin [hesap yöneticileri](permissions-overview.md#manage-mpn-membership-and-your-company) tarafından gerçekleştirilebilir. Hesap Yöneticisi rolüne sahip değilseniz, Kullanıcı geçiş sihirbazının yardımıyla Kullanıcı hesaplarını ayarlamaya yardımcı olabilecek bir hesap yöneticisi bulun. Kullanıcı geçiş işlevi 18 Kasım 2020 tarihinden itibaren kullanılabilir.

:::image type="content" source="images/pscmigration/psc-user-migration.png" alt-text="Kullanıcı Geçiş Sihirbazı 'nı gösteren resim.":::

Hesap yöneticileri, referanslar kılavuzunun yanındaki ortak satış fırsatları sayfasında bir PSC Kullanıcı Geçiş Sihirbazı bağlantısı görür. Bağlantıyı seçerek Kullanıcı geçişini başlatabilirler. Kullanıcı geçişini başlatmak için Yöneticiler bağlantıyı seçebilir. Tüm kullanıcılara Iş Ortağı Merkezi 'nde uygun roller atanıncaya kadar, bu kullanıcı geçiş adımını birden çok kez gerçekleştirebilirler.

Kullanıcı geçiş tablosu aşağıdaki ayrıntılara sahiptir:

- Kullanıcı hesabı-çalışanın e-posta KIMLIĞI
- PSC iş ortağı hesabı-çalışanın PSC içinde ilişkilendirildiği hesap
- PSC Kullanıcı rolü-PSC içinde öğesine atanan üç rolden biridir.
- BILGISAYAR MPN konumu-kullanıcıya ilgili bılgısayar rolleri verilecek konum. PSC iş ortağı hesabı MPN, izin atamak üzere Iş Ortağı Merkezi 'nde eşdeğer MPN konumunu bulmak için kullanılır. Kuruluşun tamamı, vOrg MPN KIMLIĞINI gösterir.
- BILGISAYAR Kullanıcı rolü-çalışanlar, PSC Kullanıcı rollerine göre rollere atanır. PSC 'deki yöneticiye, bılgısayarda başvuru yöneticisi rolleri atanacaktır. Satıcı, bılgısayarda başvuru Kullanıcı rolüne atanır. BILGISAYAR rolleri ve bu rollerin bulunduğu kullanıcılar iş [Ortağı Merkezi 'nde](permissions-overview.md#manage-referrals) neler yapabileceğini öğrenin
- BILGISAYAR AAD kiracısı-kullanıcıların Iş Ortağı Merkezi 'nde atandığı kiracı
- Durum-geçiş durumunun üç olası durumu vardır
    - **Geçirilmedi** -kullanıcıya HERHANGI bir bilgisayar başvuruları rolü atanmamış
    - **Geçirilmiş** -Kullanıcı, tabloda gösterildiği gibi atanan ilgili rolle başarıyla geçirildi
    - **Hata** -bir hata nedeniyle geçiş tamamlanamıyor

Bazen geçiş başarısız olabilir ve hatalara neden olabilir. Bir geçişin hataya neden olabileceği ve sorunu çözmek için bazı yollarla bazı nedenleri aşağıda verilmiştir:

1. PSC kullanıcıları iş dışı bir hesap kullanıyor olabilir.

2. PSC kullanıcısı, Iş Ortağı Merkezi 'nde kullandığınız bir etki alanından farklı bir hesap kullanıyor olabilir.

   1 ve 2 senaryolarıyla ilgili hataları gidermek için kullanıcıdan Azure AD kiracınıza bağlı iş hesabını kullanarak iş ortağı merkezi 'Nde oturum açmasını isteyin. [Genel yöneticiniz](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) yardımcı olabilir.
   
   Genel yöneticinize ulaşmak için: 
   - Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard) oturum açın ve sağ üst köşedeki dişli simgesinden **Hesap ayarları** ' nı seçin.
   - İkinci düzey, sol gezinti çubuğundan **Kullanıcı yönetimi** ' ni seçin.
   - Kullanıcı listesinin en üstünde, **filtre** açılan menüsünü seçin ve seçeneğini **genel yönetici** olarak değiştirin. Daha sonra sayfa, tüm genel yöneticileri ilgili e-posta adresleriyle birlikte görüntüler. İş hesabınız için bir başvuru Yöneticisi rolü atamasını isteyin.
   
      Genel yönetici, Azure AD kiracınızda yeni bir kullanıcı hesabı oluşturabilir ya da diğer etki alanı hesabı kullanıcılarına Konuk Kullanıcı erişimi atayabilir. Tüm PSC anlaşma yöneticileri ve kullanıcıları için hesaplar kurulduktan sonra, Iş Ortağı Merkezi 'nde oturum açması, sol gezinti menüsünden **başvuruları** seçmeniz ve başvurular sayfasını görebilecekleri onaylanır.

3. Kullanıcının Iş Ortağı Merkezi 'ne atanmış bir başvuru rolü zaten var.
    - Kullanıcının var olan rolünü doğrulayabilirsiniz. Iş Ortağı Merkezi 'nin sağ üst köşesinde, **Ayarlar** (dişli simgesi) ve ardından **Hesap ayarları**' nı seçin. İkinci bir sol gezinti menüsünü gördüğünüzde **Kullanıcı yönetimi** ' ni seçin ve Kullanıcı için arama yapın.

Kullanıcı geçişini tamamladıktan sonra, geçiş stratejisine karar vermek için aşağıdaki kılavuzu kullanın:

Şirketinizde bir Iş ortağı Geliştirme Yöneticisi (PDM) varsa-Iş Ortağı Merkezi hesabınız ayarlandığında ve kullanıcılarınız üzerine taşınır ve roller ve izinler varsa, ortak satış etkinliklerinizi Iş Ortağı Merkezi 'ne taşıyabilirsiniz. Geçiş tamamlanma son tarihine kadar beklemek yerine PDM, tüm yeni anlaşmalarınızın Iş Ortağı Merkezi 'ne akmasını sağlayan bir anahtar yapmasını bildirin.

>[!Note]
>Bu anahtarı yaptıktan sonra, yalnızca PSC 'deki mevcut etkin anlaşmalar üzerinde işlem yapabilirsiniz. Yeni anlaşmalar oluşturmayabilir veya PSC 'de Microsoft satıcılarından herhangi bir anlaşmalar alamazsınız.

Şirketiniz bir PDM içermiyorsa, tüm Kullanıcı hesaplarının tüm kullanıcılar tarafından ayarlandığından ve doğrulandığından emin olun. Iş Ortağı Merkezi 'nde ortak satış ile başlayabilmeniz için, bir e-posta ile ve PSC 'deki bir başlık aracılığıyla bildirimde bulunacaktır. PSC 'deki mevcut etkin anlaşmaları hala yönetmeniz gerektiğini unutmayın.

>[!Important]
>Etkin anlaşmalar BILGISAYARA geçirilmeyecektir. 31 Mart 2021 ' e kadar olan anlaşmaları kapatmak ve kaydetmek için kullanabilirsiniz.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>PSC yöneticileri, PSC anlaşma yöneticileri ve PSC satıcıları için sonraki adımlar

Iş Ortağı Merkezi 'nde ortak satışı yapmayı öğrenin.
Bu önemli bir adımdır ve Iş Ortağı Merkezi 'nde ortak satış için hazırlıklı olmanıza yardımcı olur. Verimli bir şekilde işbirliği yapabilmeniz için iş akışlarını ve iş ortağı merkezindeki değişiklikleri anlayın. Bu belgeyi tamamen okuyarak başlayın. [Ortak satış deneyimi galerisinde](https://aka.ms/cosellexperience)uygun bir kaynak kümesi de mevcuttur.

## <a name="major-differences-between-psc-and-pc-workflows"></a>PSC ve PC iş akışları arasındaki önemli farklılıklar

|**Senaryo**|**İş ortağı satışları bağlantısı**|**İş Ortağı Merkezi**|
|-----|:-----|:-----|
|Kullanıcı rolleri|PSC 'in yönetici, anlaşma Yöneticisi ve satıcı rolleri vardır.|BILGISAYAR yalnızca tüm anlaşmalar için hem okuma hem de yazma izni veren [başvuru Yöneticisi](permissions-overview.md#manage-referrals) rolüne sahiptir.|
|Ortak satış için Microsoft 'a davet etme|Microsoft satıcı tarafından başlatılan, iş ortağı tarafından açık bir sorun yoktur.|Bir Microsoft satıcı yardımı bir anlaşma için gerekliyse iş ortağının [açık bir istek](manage-co-sell-opportunities.md#add-solutions) yapması gerekir. Microsoft satıcının isteği reddetme seçeneği vardır.|
|Süre sonu|Bir anlaşma süre sonu kavramı yoktur.|İş ortağı tarafından kabul edilmediyse iş ortağı gelen anlaşmalar 14 gün içinde sona erer. Ayrıca, iş ortağı giden anlaşmalar, Microsoft satıcı bunları 14 gün içinde işlem yapmaz.|
|Microsoft satıcı ayrıntıları|Bir anlaşma oluşturulduktan hemen sonra görünür.|Microsoft satıcı ayrıntıları, yalnızca satıcı iş ortağından ortak satış davetini kabul ettiğinde ortak olarak paylaşılır.|
|[Özel işlem hattı](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Kullanılamıyor.|İş ortakları, Microsoft satıcıları için görünürlük vermeden kendi işlem hatlarını paylaşabilir.|
|Çözümler|Yalnızca bir fiyat listesine ait olan çözümler bir başa eklenebilir.|İş ortağı, aşağıdaki listelere ait [çözümler](manage-co-sell-opportunities.md#add-solutions) ekleyebilir. a) Microsoft 'un ilk taraf kataloğundan (PSC 'deki Işlem anlaşma rolüne benzer) ve c) çözümleri, diğer üçüncü taraf iş ortaklarından (PSC 'deki ISV anlaşma rolüne benzer şekilde) ortak satış çözümleri sağlar.|
|Anlaşma ataması|Yalnızca atanan satıcı, anlaşmaları görüntüleyebilir ve üzerinde işlem yapabilir.|Ekip üyeleri bir anlaşma üzerinde çalışan kişileri belirtmek için bir anlaşmaya eklenebilir, diğer başvuru yöneticilerinin bu anlaşmalar üzerinde görüntülenmesini veya bu anlaşmaları üzerinde hareket etmesinin engellenmesi yoktur.|
|Müşteri kuruluşu|Serbest form metin girişi.|Yalnızca birkaç karakter yazarak [Müşteri kuruluşunda](manage-co-sell-opportunities.md#select-your-customer) [D&B veritabanına](https://www.dnb.com/) göre arama yapabilirsiniz. Yasal ad ve adres seçime göre otomatik olarak doldurulur.|
|Müşteri iletişim|Zorunlu değildir.|Özel işlem hattı paylaşımı için zorunlu değildir. Microsoft satıcı, ortak satış isteğine katılmaya davet edildiyseniz gereklidir.|
|Ortak API|Kullanılamıyor.|Iş Ortağı Merkezi başvurularını programlı bir şekilde yönetmek için [ortak API](/partner/develop/referrals) .|

## <a name="map-the-fields-in-psc-to-the-corresponding-fields-in-partner-center"></a>PSC 'deki alanları Iş Ortağı Merkezi 'ndeki ilgili alanlarla eşleyin

Bu bölüm, Iş Ortağı Merkezi ortak satış fırsatları bölümünde ilgili görünüme karşılık gelen PSC için gösterilen seçili ekran görüntülerini (veya "haritalar") karşılaştırır.

Her ekran görüntüsü çiftinde numaralandırılmış, sarı veya kırmızı daireler görürsünüz:

- **Sarı daireler ne anlama geliyor?** Numaralandırılmış sarı daireler her bir PSC ekran görüntüsünde önce görüntülenir. Daha sonra aynı sayının birçoğu ile birlikte bir yardımcı Iş Ortağı Merkezi ekran görüntüsü bulacaksınız.

   Her bir alanın veya özniteliğin Iş Ortağı Merkezi 'ndeki karşılığına nasıl eşlendiğini görmek için, numaralandırılmış çemberleri iki, ilgili ekran görüntülerinde birlikte eşleştirin. Örneğin, birinci, PSC ekran görüntüsünde numaralandırılmış, sarı "1" ile, ikinci örnekteki Iş Ortağı Merkezi ekran görüntüsünde numaralı

- **Kırmızı bir daire ne anlama geliyor?** Bir ekran görüntüsünde kırmızı bir daire görürseniz, bu, PSC alanının Iş Ortağı Merkezi 'nde kullanılamaz olduğunu gösterir.

PSC-Iş ortağı merkezi alan eşlemeleri aşağıdaki alanlar için gösterilir:

1. Iş Ortağı Merkezi ortak satış fırsatları varsayılan görünümü ile eşlenmiş PSC giriş sayfası
1. Iş Ortağı Merkezi anlaşma görünümü ile eşlenmiş PSC ızgara görünümü
1. PSC anlaşma Ayrıntıları görünümü Iş Ortağı Merkezi anlaşma Ayrıntıları görünümü ile eşlendi
1. Iş Ortağı Merkezi 'ne eşlenmiş PSC ekleme ürünleri görünümü çözüm ekleme görünümü
1. Iş Ortağı Merkezi Kullanıcı yönetimi görünümüne eşlenmiş PSC Kullanıcı yönetimi görünümü
1. Partneruser rolü atama görünümü Iş ortağı merkezi rolü atama görünümüne eşlendi
1. Iş Ortağı Merkezi bildirimleri görünümüne eşlenmiş PSC bildirimleri görünümü

### <a name="1---psc-home-page-mapped-to-the-partner-center-co-sell-opportunities-default-view"></a>1-Iş Ortağı Merkezi ortak satış fırsatları varsayılan görünümü ile eşlenmiş PSC giriş sayfası

En üstteki PSC ekran görüntüsü ile Iş Ortağı Merkezi ekran görüntüsü arasındaki eşleşen, numaralandırılmış daireleri karşılaştırın. Eşleşen sayılar, PSC ile ilgili özelliği veya özniteliği Iş Ortağı Merkezi 'nde nerede bulabileceğinizi gösterir. Kırmızı daireler eşleşen Iş Ortağı Merkezi alanını gösterir.  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="Iş ortağı satış bağlantısı 'nın ana sayfası ve Iş Ortağı Merkezi 'nde ortak satış fırsatlarını varsayılan görünümü arasındaki alan eşlemelerini gösteren resim." lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>2-Iş Ortağı Merkezi anlaşma görünümüyle eşleştirilmiş olan PSC ızgara görünümü

En üstteki PSC ekran görüntüsü ile Iş Ortağı Merkezi ekran görüntüsü arasındaki eşleşen, numaralandırılmış daireleri karşılaştırın. Eşleşen sayılar, Iş Ortağı Merkezi 'nde PSC ile ilgili özelliği veya özniteliği nerede bulabileceğinizi gösterir. Kırmızı daireler eşleşen Iş Ortağı Merkezi alanını gösterir.  

> [!NOTE]
> Ekran görüntülerinin altında diğer konular görüntülenir.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="Iş ortağı Sales Connect (PSC) kılavuz görünümü ve Iş Ortağı Merkezi anlaşma görünümü arasındaki alan eşlemelerini gösteren resim." lightbox="images/pscmigration/grid-view-expanded.png":::

**Özel hususlar:**

- Iş Ortağı Merkezi 'nde PSC gibi bir liste görünümü yoktur.  Tüm anlaşmalar, müşteri bilgilerini ve anlaşma türünü içeren en son alınan veya oluşturulan tarihe göre listelenir. Görünümdeki ilk işlem varsayılan olarak seçilidir. PSC tablosu biçiminde görüntülenen değerlerin çoğu, bılgısayar içindeki anlaşma ayrıntı görünümünde kullanılabilir.
- Anlaşma rolü, BILGISAYARıNDA gerekli bir alan değildir. İş akışlarının hiçbirinde gösterilmez veya yakalanmaz. Microsoft satıcı tarafında, başa eklenen çözümlere göre otomatik olarak türetilir.
- Son değiştirilme tarihi, BILGISAYARDAKI başvuru ayrıntıları sayfasında gösterilmez. İş ortakları, son güncelleme tarihine göre anlaşmaları sıralamak için sıralama işlevini kullanabilir.

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3-PSC anlaşma Ayrıntıları görünümü Iş Ortağı Merkezi ile eşlendi

En üstteki (PSC) ekran görüntüsündeki eşleşen, numaralandırılmış daireler, ortak merkez ekran görüntüsü ile karşılaştırın. Eşleşen sayılar, Iş Ortağı Merkezi 'nde PSC ile ilgili özelliği veya özniteliği nerede bulabileceğinizi gösterir. Kırmızı daireler, Iş Ortağı Merkezi 'nde eşleşen alan veya alan olmadığını gösterir.

> [!NOTE]
> Ekran görüntülerinin altında diğer konular görüntülenir.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Iş ortağı Sales Connect (PSC) anlaşma Ayrıntıları görünümü ve Iş Ortağı Merkezi anlaşma Ayrıntıları görünümü arasındaki alan eşlemelerini gösteren resim." lightbox="images/pscmigration/deal-details-expanded.png":::

**Özel hususlar:**

- İş ortakları, iş ortağı anlaşma ayrıntısı görünümündeki Düzenle düğmesini seçerek bir anlaşmayı düzenleyebilir (6). Düzenle düğmesi seçildikten sonra tüm alanlar düzenlenebilir hale gelir. Daha sonra, anlaşma için yapılan düzenlemeleri kaydetme veya iptal etme seçeneğiniz vardır.
- Iş Ortağı Merkezi 'nde Yineleneni kapatma seçeneği yoktur.
- Müşteri sonucu Iş Ortağı Merkezi 'nde kullanılamaz. Müşteri etkileşimlerine ilişkin tüm ayrıntılar, bılgısayar içindeki Notlar bölümünde güncelleştirilemeyebilir.
- Tahmini çözüm kapatma tarihi yalnızca Iş Ortağı Merkezi 'nde OEM ıOT anlaşmaları için kullanılabilir. Bu bilgiler diğer hiçbir anlaşma türü için görüntülenmez.
- Lisanslama programı bılgısayarda gerekli değildir. Bu bilgiler, işlem sırasında seçilen çözümlere göre otomatik olarak algılanır.

>[!Note]
>Kazanıldı veya kaybedildi olarak işaretlenen herhangi bir anlaşma daha sonra düzenlenemez. Bir anlaşmayı bu Terminal durumlarından birine taşırken dikkatli olun.

### <a name="4---psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>4-' çözüm ekleme ' görünümü Iş Ortağı Merkezi 'ne eşlenmiş ' ürün Ekle ' görünümü

En üstteki (PSC) ekran görüntüsündeki eşleşen, numaralandırılmış daireler, ortak merkez ekran görüntüsü ile karşılaştırın. Eşleşen sayılar, Iş Ortağı Merkezi 'nde PSC ile ilgili özelliği veya özniteliği nerede bulabileceğinizi gösterir. Kırmızı daireler, Iş Ortağı Merkezi 'nde eşleşen alan veya alan olmadığını gösterir.
  
:::image type="content" source="images/pscmigration/products.png" alt-text="Ortak satış bağlantısı (PSC) ürün ekleme görünümü ve Iş Ortağı Merkezi çözüm ekleme görünümü arasındaki alan eşlemelerini gösteren resim." lightbox="images/pscmigration/products-expanded.png":::

### <a name="5---user-management-in-psc-versus-partner-center"></a>5-PSC ve Iş Ortağı Merkezi 'nde Kullanıcı Yönetimi

En üstteki (PSC) ekran görüntüsündeki eşleşen, numaralandırılmış daireler, ortak merkez ekran görüntüsü ile karşılaştırın. Eşleşen sayılar, Iş Ortağı Merkezi 'nde PSC ile ilgili özelliği veya özniteliği nerede bulabileceğinizi gösterir. Kırmızı daireler, Iş Ortağı Merkezi 'nde eşleşen alan veya alan olmadığını gösterir.  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Iş ortağı satış bağlantısı (PSC) Kullanıcı Yönetimi ana ve hesap ayarları alanındaki Iş Ortağı Merkezi Kullanıcı yönetimi sayfa görünümü arasındaki alan eşlemelerini gösteren resim."  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="6---user-role-assignment-in-psc-versus-partner-center"></a>6-PSC ve Iş Ortağı Merkezi 'nde Kullanıcı rolü ataması

En üstteki (PSC) ekran görüntüsündeki eşleşen, numaralandırılmış daireler, ortak merkez ekran görüntüsü ile karşılaştırın. Eşleşen sayılar, Iş Ortağı Merkezi 'nde PSC ile ilgili özelliği veya özniteliği nerede bulabileceğinizi gösterir. Kırmızı daireler, Iş Ortağı Merkezi 'nde eşleşen alan veya alan olmadığını gösterir.  

:::image type="content" source="images/pscmigration/roles.png" alt-text="Iş ortağı Sales Connect (PSC) rol atama görünümü ve Iş ortağı merkezi rolü atama görünümü arasındaki alan eşlemelerini gösteren resim." lightbox="images/pscmigration/roles-expanded.png":::

**Özel hususlar:**

- PSC Yöneticisi için eşdeğer rol, Iş Ortağı Merkezi ' nde Hesap Yöneticisi rolüdür.
- Ortak satış anlaşma yönetimi için Iş Ortağı Merkezi 'nde yalnızca bir rol vardır. Bu rol, başvuru Yöneticisi rolüdür.

### <a name="7---notifications-in-psc-versus-partner-center"></a>7-PSC ve Iş Ortağı Merkezi 'nde bildirimler

En üstteki (PSC) ekran görüntüsündeki eşleşen, numaralandırılmış daireler, ortak merkez ekran görüntüsü ile karşılaştırın. Eşleşen sayılar, Iş Ortağı Merkezi 'nde PSC ile ilgili özelliği veya özniteliği nerede bulabileceğinizi gösterir. Kırmızı daireler, Iş Ortağı Merkezi 'nde eşleşen alan veya alan olmadığını gösterir.  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="Ortak satış bağlantısı (PSC) bildirimleri ve Iş Ortağı Merkezi bildirimleri görünümü arasındaki eşlemeyi gösteren resim."  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>PSC 'den Iş Ortağı Merkezi 'ne geçme-sık sorulan sorular

Aşağıdaki bölümlerde geçişle ilgili sık sorulan sorular yanıtlanacaktır.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1-Iş Ortağı Merkezi 'ne erişimi yoksa ne yapmam gerekir?

Atanan rolleri almak için, "erişim yok" sayfasında listelenen yöneticilerinize başvurabilirsiniz. Başvurular bölümünde okuma ve yazma izni için [başvuru Yöneticisi](permissions-overview.md#manage-referrals) rolüne ihtiyacınız olacak. Yalnızca iş profillerini yönetiyorsanız iş profili yönetici rolüne iş ortağı Merkezi ' nde ihtiyacınız olacaktır.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Iş Ortağı Merkezi 'nde erişim deneyimi olmadığını gösteren resim.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2-Iş Ortağı Merkezi 'ndeki referanslar bölümüne kimler erişebilir?

[Hesap yöneticiniz](permissions-overview.md#manage-mpn-membership-and-your-company) , başvurular sekmesine erişim izni verebilir. Hesap yöneticinize ulaşmak için, Iş Ortağı Merkezi [panosunun](https://partner.microsoft.com/dashboard)sağ üst tarafındaki dişli simgesinden **Hesap ayarları** ' nı seçin. Ardından, ikinci düzey, sol gezinti çubuğundan **Kullanıcı yönetimi** ' ni seçin. Kullanıcı listesinin en üstünde, **filtre** açılan menüsünü seçin ve **Hesap Yöneticisi** seçeneğini belirleyin. Bu sayfada, tüm hesap yöneticileri ilgili e-posta adresleriyle görüntülenir. İş hesabınız için bir başvuru Yöneticisi rolü atamasını isteyin.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3-hesabım için + yeni anlaşma düğmesi gri değildir. Anlaşmalar oluşturmaya başlamak için ne yapmam gerekir?

Bu yalnızca, Iş Ortağı Merkezi 'nde kullandığınız MPN kuruluşuna iliştirilmiş ortak satış için ücretsiz çözüm olmadığında gerçekleşir. Çözümlerinizin MPN KIMLIĞINI bir şekilde düzeltti veya bir destek bileti oluşturmak için PDM ile iletişime geçerek "yeni anlaşma düğmesi, PSC geçişten sonra gri" olarak görüntüleniyor.

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4-belirli bir kişiye, PSC gibi kuruluşumuza yönelik anlaşmalar atayabilir miyim?

Takım üyelerini belirli bir anlaşmayı atayabilirsiniz. Diğer başvuru yöneticilerinin bu anlaşmaları görüntülemesini veya bu anlaşmalar üzerinde hareket etmalarını engellemez.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5-bana atanan tüm anlaşmalar için bir görünüm var mı?

Kullanıcı düzeyi sekmesi olan Sık Kullanılanlar özelliğini kullanabilirsiniz. Bu anlaşmalar için hızlı bir erişim sağlamak üzere size atanan tüm anlaşmaları sık kullanılanlar olarak işaretleyebilirsiniz.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6-anlaşmalar için salt okunurdur bir görünüm var mı?

Hayır, başvurular bölümünde anlaşmalar için salt okuma görünümü yoktur. Tüm başvuru yöneticilerinin tüm anlaşmalar için tam okuma ve yazma erişimi olur.

### <a name="7---how-can-i-register-a-deal-after-marking-it-as-won"></a>7-Kazanıldı olarak işaretlendikten sonra bir anlaşmayı nasıl kaydedebilirim?

Anlaşma aşağıdaki ölçütleri karşılıyorsa, [anlaşmayı](./register-deals.md)başlatmak için bir açılır pencere görüntüleriz.

- Ele uygun bir çözüm vardır.
- Microsoft satıcı, başa katılmaya davet edilir veya sizi ele davet ederler.
- Microsoft kartı, Iş Ortağı Merkezi 'nde kabul edilen veya kazanıldı durumunda.

### <a name="8---i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>8-anlaşma kaydı bölümünde "+ yeni anlaşma kaydı" düğmesini seçdiğimde bir hata mesajı alıyorum. Nasıl anlaşmalar kaydedebilirim?

**+ Yeni anlaşma kaydı** DÜĞMESI yalnızca ISV Connect programına kayıtlı iş ortakları tarafından, Iş Ortağı Merkezi 'Nde ilgili ortak satış fırsatı olmadan bir anlaşma kaydetmek için kullanılır. Bir ortak satış fırsatıyla anlaşmalar kaydettirmek için, anlaşma Kazanıldı olarak işaretlendiğinde ve anlaşma kaydı ölçütlerini karşılıyorsa bir açılır pencere görüntülenir.

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9-bir müşteri kuruluşu zorunlu mi ekliyor?

Evet, [Müşteri kuruluşu](./manage-co-sell-opportunities.md#select-your-customer) eklemek Iş Ortağı Merkezi 'nde zorunludur. İlk olarak, müşterinin konumun bulunduğu konumu arayarak başlayın. Sahip olduğunuz ayrıntılara göre; tam bina adını dahil edebilir veya yalnızca şehir ayrıntıları verebilirsiniz. Kuruluş araması, girdiğiniz adla eşleşen tüm yasal varlıkları getirecek, böylece herhangi bir adres ayrıntısı girmenize gerek kalmaz. Tüm ayrıntılar, seçilen kuruluşa göre otomatik olarak doldurulur.

### <a name="10---are-customer-contact-details-mandatory"></a>10-müşteri iletişim ayrıntıları zorunludur mi?

Oluşturmakta olduğunuz [işlem türüne](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) bağlıdır. Yalnızca işlem hattınızı paylaşıyorsanız ve Microsoft satış kuruluştan herhangi bir yardım gerektirmiyorsa, müşteri iletişim ayrıntılarını vermemesini seçebilirsiniz. Microsoft satıcı 'dan etkin bir şekilde yardım Aradığınız yerde ortak satıyor olmanız durumunda müşteri iletişim ayrıntılarını sağlamanız gerekir. İş Ortağı Merkezi 'nde ortak satış isteği oluşturmadan önce müşteriden açık onay almalısınız.

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11-bir dağıtmaya kaç çözüm ekleyebilirim?

En fazla 50 çözüm ekleyebilirsiniz (PSC 'de ' Ürünler ' öğesine benzer), bir anlaşma. PSC 'nin aksine, kendi ortak satış uygun çözümlerinizde, Microsoft ilk taraf SKU 'Lardan ve diğer üçüncü taraf ortak satış özellikli çözümlerle çözümler karıştırabilirsiniz. İş Ortağı Merkezi 'nde seçilecek veya kullanılabilecek bir anlaşma rolü yok. Microsoft SKU 'Ları için, isteğe bağlı olarak, başa eklenen her SKU için miktar ve fiyat ekleyebilirsiniz.

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12-bir anlaşma oluşturduktan sonra Microsoft satıcı ayrıntılarını öğrenmem gerekir mi?

Microsoft satıcıları, Microsoft tarafındaki ilgili satıcı ile ilgilenirken belirtilen tam yardım gereksinimini eşleştirdikten sonra atanır. Atamadan sonra bile Microsoft satıcıları, ortak satış davetini kabul etme veya reddetme seçeneğine sahip olacaktır. Yalnızca bir satıcı tarafından bir ortak satış daveti kabul edilirse, bu anlaşma Microsoft satıcı iletişim ayrıntıları ile güncelleştirilir. Microsoft satıcıları için SLA, anlaşma üzerinde işlem yapması için 14 gündür. Bu, iş ortaklarının, zaman aşımına uğramadan önce anlaşma üzerinde işlem yapması gereken SLA 'dır.

### <a name="13---where-can-i-find-the-opportunity-id"></a>13-fırsat KIMLIĞINI nerede bulabilirim?

PSC 'deki fırsat KIMLIĞI, BILGISAYARDAKI anlaşma KIMLIĞIYLE aynıdır. Herhangi bir anlaşmayı açtığınızda anlaşma adının yanında anlaşma KIMLIĞINI bulabilirsiniz.

### <a name="14---how-can-my-pdm-get-access-to-pc"></a>14-PDM Bilgisayarıma nasıl erişeirim?

İş Ortağı Merkezi 'Ne doğrudan PSC 'nin aksine, PDMs 'niz tarafından erişilemez. Bu özelliği etkinleştirmek için aşağıda bahsedilen birden çok seçenek vardır.

- OCP Insights-PDMs yalnızca bunlarla ilgili anlaşmaları ve ilerlemeyi görüntülüyorsanız, kuruluş görünümünüzü almak için OCP Insights portalını kullanabilirler. Bu bir iç araçtır ve yalnızca PDMs için kullanılabilir. OCP öngörülerinin şirketinizin kullanıcıları için sunulmadığını unutmayın.
- Iş Ortağı Merkezi 'nde Konuk Kullanıcı-PDM @microsoft.com Hesabınızı, iş ortağı merkezi 'nde Konuk Kullanıcı olarak ekleyebilir ve başvuruları görüntüleyebilmek ve bunlarla işlem yapabilmesi için başvuru Yöneticisi rolü atayabilirsiniz.
- Kiracınızda [Yeni bir Kullanıcı](./create-user-accounts-and-set-permissions.md#add-a-new-user) oluşturma-kendi kiracınızda yeni bir kullanıcı oluşturabilir ve bu ayrıntıları PDM ile paylaşabilir ve bu sayede hesabınızdaki diğer başvuru kullanıcılarına benzer başvuruları görüntüleyebilir ve bunlarla işlem yapabilir.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Iş Ortağı Merkezi 'nde anlaşmalar oluşturmanıza ve yönetmenize yardımcı olacak kaynaklar

Ortak satış yardım konularını henüz okumadıysanız, aşağıdaki kaynaklar iş ortağı merkezindeki anlaşmaları yönetmenize yardımcı olur.

|**Bunu yapmak için**   |**Bunu okuyun**   |
|-----------------------|:-----------------------|
|Ortak satış fırsatları sayfasında sekmeleri ve gezintiyi anlama|[Ortak satış bölümünde gezinme](./manage-co-sell-opportunities.md#navigating-the-co-sell-section)|
|D&B listesinden bir müşteri organizasyonu seçme |[Müşteriyi seçin](./manage-co-sell-opportunities.md#select-your-customer)|
|Anlaşma ayrıntıları bölümündeki alanları değiştirme|[Anlaşma ayrıntıları](./manage-co-sell-opportunities.md#deal-details)|
|Ekip üyelerinizi bir anlaşma ekibine ekleme|[Çalışanlarınızı ekleyin](./manage-co-sell-opportunities.md#add-team-members)|
|Ortak satış bir anlaşmayı yanıtlama|[Ortak satış anlaşmalar yönetme](./manage-co-sell-opportunities.md#responding-to-a-co-sell-opportunity)
|Iş Ortağı Merkezi 'nde kazandığı anlaşmaları kaydetme |[Yeni bir anlaşma Kaydet](./register-deals.md)
|Başvuru öngörülerini edinin ve başvurularınızın nasıl çalıştığını öğrenin |[Referans içgörüleri](./referral-insights.md)
|İş profili oluşturma ve yönetme|[İş profilini yönetme](./create-a-marketing-profile.md)
|İş profiliniz için müşteri adaylarını yönetme |[Müşteri adaylarını yönetme](./manage-leads.md)|

## <a name="next-steps"></a>Sonraki adımlar

Şu ek kaynakları izleyin:

- İş ortağı satışları iş ortağı [Merkezi çalışma kitabına bağlanır](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) -iş ortaklarının satış süreçlerini ve rollerini Iş Ortağı Merkezi Ile Iş ortağı Sales Connect aracılığıyla yeni satış süreçleriyle hizalayın.
- [Iş Ortağı Merkezi ortak satış çalışma kılavuzu](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) -müşteri adaylarını yönetmek Için Iş Ortağı Merkezi aracılığıyla bir işletim modelini belirlemek için bir iş modeli veya ortak satış fırsatları ve anlaşmaları kaydetme.
- [Başvuru yönetimi destesi](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) -müşteri adaylarını yönetmek için görselleştirilen adım adım yönergeler ve Iş Ortağı Merkezi aracılığıyla ortak satış fırsatları.
- [Ticari Market 'Te yayımlama ve yönetme](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) -ticari Market 'Teki Iş Ortağı Merkezi aracılığıyla teklifler oluşturmak, yönetmek ve yayımlamak için görselleştirilen adım adım yönergeler.