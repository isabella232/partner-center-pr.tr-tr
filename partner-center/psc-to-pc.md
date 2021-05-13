---
title: İş Ortağı Satış Bağlantısı'dan (PSC) geçiş
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft iş ortaklarının İş Ortağı Satış Bağlantısı'dan (PSC) İş Ortağı Merkezi ve Microsoft satıcılarının gönderdiği anlaşmaları oluşturma veya yönetme hakkında bilgi.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 12/07/2020
ms.openlocfilehash: 584f8a7f2794cb64be49fe7f790904eff50c4c26
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855123"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>İş Ortağı Satış Bağlantısı'İş Ortağı Merkezi (PSC) iş ortakları için İş Ortağı Merkezi 'de ortak satış kılavuzu

**Uygun roller:** Hesap yöneticisi | Referans yöneticisi | İş Ortağı Satış Bağlantısı (PSC) satıcısı | İş Ortağı Satış Bağlantısı (PSC) yönetici | İş Ortağı Satış Bağlantısı (PSC) anlaşma yöneticisi

Bu makalede İş Ortağı Satış Bağlantısı'İş Ortağı Merkezi ortak satış anlaşmaları oluşturma ve yönetmeye devam etmek için İş Ortağı Satış Bağlantısı'İş Ortağı Merkezi.

>[!Note]
> PsC'de geçişle ilgili bir başlık gördüğü için buradasanız doğru yerdesinizdir. Bu kılavuz, PSC'de anlaşmalarını yöneten Çözüm Değerlendirmesi (SA) ve OEM lisanslama iş ortakları için geçerli değildir.

>[!Important]
> 1 Nisan 2021'den itibaren, şirketiniz PSC'de anlaşma oluşturabilecek veya anlaşmaları düzenleyemez. **PSC'de toplu dışarı aktarma özelliğini kullanarak mevcut anlaşma verilerini indirmeye devam edersiniz. Açık anlaşmaları [psC'den](psc-to-pc.md#psc-deals-migration) bu tarihten sonra İş Ortağı Merkezi da geçirilir.** <br><br> IP ortak satış teşviki uygun çözümleri içeren etkin bir şekilde üzerinde çalıştığınız anlaşmalar varsa iki seçeneğiniz vardır: <br><br> 1. Anlaşmayı kazanildi olarak işaretle ve 31 Mart 2021'den önce PSC'de anlaşma kaydını tamamla. <br> 2. [Anlaşmaları İş Ortağı Merkezi](psc-to-pc.md#psc-deals-migration) ve anlaşma kaydını başlatmak için daha fazla zaman elde etmek için anlaşmaları geçişe geçirme.

Bildiğiniz gibi şirket, **30 Nisan 2021'den sonra PSC'ye erişimi kaybeder.** Ancak, ortak satış anlaşmaları oluşturma, satış anlaşmalarınızı yönetme ve Microsoft satıcılarının size gönderdiği anlaşmalara göre hareket İş Ortağı Merkezi istediğiniz her şeyi yine de bulabilirsiniz.

Ancak farklar da vardır. Aşağıdaki kılavuz, geçiş sürecinizin daha sorunsuz ve İş Ortağı Merkezi yardımcı olabilir.

## <a name="before-you-move-things-you-need-to-know"></a>Taşımadan önce, bilmek gerekenler

### <a name="if-you-are-a-psc-admin"></a>PSC yöneticisiyseniz

- İş Ortağı Merkezi'da oturum a almak için bir [iş e-postası gerekir.](https://partner.microsoft.com/)
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

1. Panonun **sağ** üst köşesindeki dişli simgesinden Hesap ayarları'İş Ortağı Merkezi seçin.

1. İkinci **düzey,** sol gezinti menüsünden Kullanıcı yönetimi'ni seçin.

1. Kullanıcı listesinin üst kısmında Filtre **açılan** menüsünü seçin. Seçeneğini Hesap yöneticisi **olarak değiştirme.**

   Sayfada ilgili e-posta adresleriyle birlikte tüm hesap yöneticileri görüntülenir. Bunlardan birini e-postayla gönderin ve iş hesabınız için referans yöneticisi rolünü atamasını sorun.

  :::image type="content" source="images/pscmigration/account-admin.gif" alt-text="İş ortağı ayarları kullanıcı yönetimi sayfasında hesap yöneticilerini gösteren resim.":::

>[!Important]
>- Rolünüz yalnızca PSC'de kullanıcıları yönetmeyi içeriyorsa, şirketinizin hesap yöneticisinin size şirket içinde hesap yöneticisi [rolünü](permissions-overview.md#manage-mpn-membership-and-your-company) atamasını İş Ortağı Merkezi. 
>- Rolünüz ortak satış fırsatlarını yönetmeyi de içerirse referans yöneticisi [rolünün atanmasını](permissions-overview.md#manage-referrals) istemeniz gerekir.
> - PSC yöneticileri arasında bir değişiklik yönetimi adayı da göstermeniz iyi bir fikirdir. Bunu yapmak, tüm PSC yöneticilerinin hesap yöneticilerine tek tek İş Ortağı Merkezi engel olur. Bunun yerine değişiklik yönetimi müşteri adayı, hesap yöneticisiyle İş Ortağı Merkezi kişi olabilir.

## <a name="user-migration"></a>Kullanıcı geçişi

Şirket içinde hesabınız İş Ortağı Merkezi, ortak satış fırsatları sayfasındaki kullanıcı geçiş sihirbazını kullanarak şirket çalışanlarınıza İş Ortağı Merkezi rollerini otomatik olarak atfın.

>[!Note]
> Kullanıcı geçişi yalnızca şirketinizin [hesap yöneticileri](permissions-overview.md#manage-mpn-membership-and-your-company) tarafından yapılabilir. Hesap yöneticisi rolüne sahip değilseniz, kullanıcı geçiş sihirbazının yardımıyla kullanıcı hesaplarını ayarlamaya yardımcı olacak bir hesap yöneticisi bulun.

:::image type="content" source="images/pscmigration/user-migration.gif" alt-text="Kullanıcı geçiş sihirbazını gösteren görüntü.":::

Hesap yöneticileri, referans kılavuzunun yanındaki ortak satış fırsatları sayfasında psC kullanıcı geçiş sihirbazı bağlantısını görebilir. Bağlantıyı seçerek kullanıcı geçişini başlatabilirsiniz. Yöneticiler, kullanıcı geçişini başlatmak için bağlantıyı seçin. Tüm kullanıcılara Iş Ortağı Merkezi 'nde uygun roller atanıncaya kadar, bu kullanıcı geçiş adımını birden çok kez gerçekleştirebilirler.

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

2. PSC kullanıcısı, etki alanındaki hesaplardan farklı bir hesap kullanıyor olabilir ve İş Ortağı Merkezi.

   1. ve 2. senaryolarla ilgili hataları çözmek için kullanıcıdan Azure AD kiracınıza İş Ortağı Merkezi iş hesabını kullanarak oturum açmasını sorun. Genel [yöneticiniz yardımcı](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) olabilir.
   
   Genel yöneticinizi bulmak için: 
   - Panoda İş Ortağı Merkezi [ve](https://partner.microsoft.com/dashboard) sağ **üst köşesindeki** dişli simgesinden Hesap ayarları'ı seçin.
   - İkinci **düzey,** sol gezinti çubuğundan Kullanıcı yönetimi'ni seçin.
   - Kullanıcı listesinin üst kısmında Filtre  açılan menüsünü seçin ve seçeneğini Genel yönetici **olarak belirleyin.** Ardından sayfada ilgili e-posta adresleriyle birlikte tüm genel yöneticiler görüntülenir. İş hesabınız için referans yöneticisi rolünü atamasını istemek için bunlardan birini sorun.
   
      Genel yönetici, Azure AD kiracınız içinde yeni bir kullanıcı hesabı oluşturabilir veya diğer etki alanı hesabı kullanıcılarına konuk kullanıcı erişimi atayabilirsiniz. Tüm PSC anlaşma yöneticileri ve kullanıcıları için hesaplar ayarlanmaz, İş Ortağı Merkezi'da oturum açmaları, sol gezinti menüsünden Referanslar'ı seçmeleri ve Referanslar sayfasını görene kadar onayları gerekir. 

3. Kullanıcının zaten bu rolde atanmış bir referans İş Ortağı Merkezi.
    - Kullanıcının mevcut rolünü doğrularsanız. Uygulamanın sağ üst köşesinde ayarlar İş Ortağı Merkezi **'ı** (dişli simgesi) ve ardından Hesap **ayarları'ı seçin.** İkinci bir sol gezinti menüsü gördüğünüzde Kullanıcı **yönetimi'ni seçin** ve kullanıcı için arama yapabilirsiniz.

## <a name="psc-deals-migration"></a>PSC Anlaşmaları geçişi

Kullanıcı geçişini tamamlandıktan sonra, uygun tüm açık anlaşmaları PSC'den PC'ye getirmek için ortak satış fırsatları sayfasındaki anlaşmalar geçiş sihirbazını kullanın. **Anlaşmalar geçiş bağlantısı yalnızca tüm kuruluş kapsamına sahip referans yöneticileri tarafından İş Ortağı Merkezi.** Ortak satış fırsatları sayfasının sağ üst **kısmında "PSC** anlaşma geçişi" adlı bir bağlantı olacak ve satış anlaşması geçiş sihirbazı açılır.

Anlaşma geçişini başlatmadan önce bu bölümü okuyun.

**Geçiş için uygun**

Yalnızca bazı anlaşmalar PSC 'den PC 'ye geçiş için uygun. Bu Geçiş Sihirbazı, iş ortaklarının, BT 'nin müşterileri ile çalışmaya devam ettikleri Iş Ortağı Merkezi 'ne anlaşmalar getirmelerini sağlamak için oluşturulmuştur. **Yalnızca geçerli iş ortağı hesabı ayrıntıları (geçerli MPN ID) ile 1 Ocak 2020 ' den oluşturulan ve açık durumda olan anlaşmalar geçiş için uygun değildir.**

**Geçiş için uygun değil**

- Çözüm değerlendirmesi anlaşmaları, anlaşma geçişi için uygun değildir
- OEM lisanslama iş anlaşmaları, anlaşma geçişi için uygun değildir
- PSC 'de Kazanıldı olarak işaretlenen tüm bir anlaşma geçiş için uygun değildir. Kazanıldı olarak işaretlenen anlaşmalar için uygun olursa, kayıt işlemi yapın.

## <a name="pre-requisites-for-deal-migration"></a>Anlaşma geçişi için önkoşulların önkoşulları

BILGISAYARDAN geçiş geçişini başlatmadan önce, başarılı bir geçiş için PSC 'deki anlaşmaları ayarlamak üzere aşağıdaki yönergeleri izleyin.

1. Şirketinizde açık anlaşmalar üzerinde çalışan tüm satış ekibi üyeleri bu geçiş hakkında bilgi sahibi.
2. Satış ekibi üyeleri, anlaşma yönetimi için Iş Ortağı Merkezi 'ni kullanmaya eğitim sağlar.
3. Bu anlaşmalar, aşağıda açıklandığı gibi gerekli tüm bilgilere sahiptir.
    - Ad ve adres dahil müşteri Şirket ayrıntıları
    - Ortak satış bir anlaşma ise müşteri iletişim ayrıntıları
    - En az bir çözüm
    - Tüm ayrıntıları içeren en az bir takım üyesi-ad, soyadı, e-posta KIMLIĞI ve telefon numarası
    - Anlaşma değeri
    - Tahmini anlaşma kapanış tarihi
    - İş ortağı notları

PsC'de toplu indirme ve karşıya yükleme özelliklerini kullanarak tüm uygun anlaşmaların anlaşmada eksik olan tüm ayrıntılarını indirebilirsiniz.

>[!Note]
> Yukarıdaki önkullar karşılanmazsa bile anlaşma geçişi başarılı olur. Ancak, yukarıdaki belirtilen gerekli alanlardan herhangi biri kullanılabilir durumda değilse İş Ortağı Merkezi durumunu değiştiremezsiniz. Ardından, üzerinde çalışmaya başlamak için anlaşmalarda eksik olan tüm İş Ortağı Merkezi bilgileri girmeniz gerekir. **PsC'de uygun anlaşmaları, İş Ortağı Merkezi'a İş Ortağı Merkezi.**

Geçiş anlaşması İş Ortağı Merkezi tek tıklama deneyimi olarak yerleşiktir. Tek gereken, şirket uygun anlaşmaları geçirmek için hazır olduğunda **"Anlaşmaları geçir"** düğmesine tıklamaktır. **PSC'den geçirmek istediğiniz anlaşmaları seçesiniz. Herhangi bir anlaşmayı İş Ortağı Merkezi psC'de kapalı durumuna geçirmeniz gerekir.**

>[!Note]
> Geçiş başlatıldıktan sonra, **anlaşmaların geçişi 24 saat kadar sürebilir.**

Geçiş tamamlandıktan sonra başlık iletisi, geçiş raporunun bağlantısıyla tamamlanacak şekilde değişir. PSC'den PC'ye geçirilen anlaşmaların ayrıntılarını görüntülemek için raporu indirin.

Rapor aşağıdaki ayrıntıları içerir.

1. **İş Ortağı Merkezi kimliği** - Bir etkileşimde İş Ortağı Merkezi anlaşmaların benzersiz tanımlayıcısı. İki satış anlaşması vardır: biri iş ortağı, biri de Microsoft için ortak satış anlaşmasında İş Ortağı Merkezi.
2. **İş Ortağı Merkezi referans kimliği** - İş ortağına ait İş Ortağı Merkezi için geçerli olan benzersiz tanımlayıcı.
3. **Anlaşma adı** - PSC'de anlaşmaya verilen tanımlayıcı.
4. **PSC anlaşma kimliği** - Anlaşma için PSC'deki benzersiz tanımlayıcı.
5. **Hatalar** - belirli bir anlaşmadan başka bir anlaşmayı alırken herhangi bir hata olup olamay olduğunu belirtmek için.

Başarıyla geçirilen tüm anlaşmalar PSC'de görünmez. Bilgisayardaki anlaşma kaydını tamamlama da dahil olmak üzere BILGISAYARDAKI geçirilmiş anlaşmalar üzerinde çalışmaya devam edebilirsiniz. Ortak satış anlaşmaları için Microsoft satıcıları ile etkileşimlerde hiçbir değişiklik olmayacaktır.

PSC 'den geçirilen anlaşmalar, gelen ve giden sekmelerinde, anlaşma kaynağına bağlı olarak kullanılabilir. Şirketiniz tarafından paylaşılan tüm anlaşmalar giden sekmesinde kullanıma sunulacaktır ve Microsoft tarafından başlatılan anlaşmalar Iş Ortağı Merkezi 'nin gelen sekmesinde kullanıma sunulacaktır. Geçiş sonrası oluşturulacak iki tür anlaşmalar olacaktır.

1. Ortak satış **anlaşmaları** -PSC içinde ortak satış olarak işaretlenen anlaşmalar, Iş Ortağı Merkezi 'nde ortak satış anlaşmaları olarak oluşturulur.
2. **Ortak satış** olarak işaretlenmemiş anlaşmalar, Iş Ortağı Merkezi 'nde ortak çalışan anlaşmalar olarak oluşturulur. İş ortağı olarak çalışan anlaşmalar, Microsoft satıcılarına görünür ve Terminal durumuna (kazanıldı, kaybedildi) ulaşmadan önce ortak satış anlaşmaları olarak yükseltilebilir. Ayrıca, anlaşmadan uygun bir çözüm varsa, iş ortağı ile ilgili anlaşmalar, anlaşma kaydı için uygun olur.

>[!Important]
> Bazı anlaşmalar geçirilmemiş olması nedeniyle herhangi bir hata oluşursa, **"anlaşmaları geçir" düğmesine tıklayarak anlaşma geçişini yeniden başlatabilirsiniz**. Yalnızca bazı uygun anlaşmalar varsa etkinleştirilecek. Bu Ayrıca, anlaşma geçişi başlatıldıktan sonra bazı yeni anlaşmalar için PSC 'de oluşturulan geçiş aşamasındaysanız de yararlı olacaktır.

Tüm anlaşmalar başarıyla geçirildikten sonra, " **anlaşmaları geçir** " düğmesi **devre dışı** olarak **"geçirilecek anlaşmalar yok** " adlı başlık görüntülenir.

Kullanıcı geçişini ve/veya geçiş işlemini tamamladıktan sonra, geçiş stratejisine karar vermek için aşağıdaki kılavuzu kullanın:

Şirketinizde bir Iş ortağı Geliştirme Yöneticisi (PDM) varsa-Iş Ortağı Merkezi hesabınız ayarlandığında ve kullanıcılarınız üzerine taşınır ve roller ve izinler varsa, ortak satış etkinliklerinizi Iş Ortağı Merkezi 'ne taşıyabilirsiniz. PdM'yi geçiş işleminin son tarihine kadar beklemek yerine geçişi yapmaları konusunda bilgilendirin. Bu, tüm yeni anlaşmaların geçişe İş Ortağı Merkezi.

>[!Note]
>Bu anahtarı kullandıktan sonra yalnızca PSC'de mevcut Etkin anlaşmalar üzerinde eyleme geçabileceksiniz. PSC'de Microsoft satıcılarından yeni anlaşmalar oluşturasınız veya satış anlaşması alamaysınız.

Şirkette PDM yoksa - Tüm kullanıcı hesaplarının ayarlandığından ve tüm kullanıcılar tarafından doğrulandığından emin olun. Bir e-posta ve PSC'de, satışa ilk başlanmaz tarihle ilgili bir başlık ve e-posta İş Ortağı Merkezi. PSC'de mevcut etkin anlaşmaları yönetmeye devam etmek zorunda olduğunu unutmayın.

>[!Important]
> Kazanildi olarak işaretlenen anlaşmaları kaydetmek için 30 Nisan 2021'e kadar devam edilecektir.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>PSC yöneticileri, PSC anlaşma yöneticileri ve PSC satıcıları için sonraki adımlar

İş Ortağı Merkezi'da ortak satış yapmayı İş Ortağı Merkezi.
Bu önemli bir adımdır ve bu adım, satış ve satış için hazırlık İş Ortağı Merkezi. Hemen ortak satış yapmak için İş Ortağı Merkezi iş akışlarını ve değişiklikleri anlıyoruz. Bu belgeyi tamamen okuyarak başlayabilirsiniz. ortak satış deneyimi galerisinde de [iyi bir kaynak kümesi mevcuttur.](https://aka.ms/cosellexperience)

## <a name="major-differences-between-psc-and-pc-workflows"></a>PSC ile PC iş akışları arasındaki önemli farklar

|**Senaryo**|**İş Ortağı Satış Bağlantısı**|**İş Ortağı Merkezi**|
|-----|:-----|:-----|
|Kullanıcı rolleri|PSC'de yönetici, satış anlaşması yöneticisi ve satıcı rolleri vardır.|Bilgisayar yalnızca tüm [anlaşmalar](permissions-overview.md#manage-referrals) için hem okuma hem de yazma izni veren referans yöneticisi rolüne sahip.|
|Ortak satış anlaşması için Microsoft'u davet etme|Microsoft satıcısı tarafından başlatılan bu işlem, iş ortağı tarafından açık bir şekilde sorulmamasıdır.|Anlaşma için bir Microsoft [satıcısının yardımı gerekirse](manage-co-sell-opportunities.md#add-solutions) iş ortağının açık bir istekte yerması gerekir. Microsoft satıcının isteği reddetme seçeneği vardır.|
|Süre sonu|Bir anlaşma süre sonu kavramı yoktur.|İş ortağı tarafından kabul edilmediyse iş ortağı gelen anlaşmalar 14 gün içinde sona erer. Ayrıca, iş ortağı giden anlaşmalar, Microsoft satıcı bunları 14 gün içinde işlem yapmaz.|
|Microsoft satıcı ayrıntıları|Bir anlaşma oluşturulduktan hemen sonra görünür.|Microsoft satıcı ayrıntıları, yalnızca satıcı iş ortağından ortak satış davetini kabul ettiğinde ortak olarak paylaşılır.|
|[Özel işlem hattı](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Kullanılamıyor.|İş ortakları, Microsoft satıcıları için görünürlük vermeden kendi işlem hatlarını paylaşabilir.|
|Çözümler|Yalnızca bir fiyat listesine ait olan çözümler bir başa eklenebilir.|İş ortağı, aşağıdaki listelere ait [çözümler](manage-co-sell-opportunities.md#add-solutions) ekleyebilir. a) Microsoft 'un ilk taraf kataloğundan (PSC 'deki Işlem anlaşma rolüne benzer) ve c) çözümleri, diğer üçüncü taraf iş ortaklarından (PSC 'deki ISV anlaşma rolüne benzer şekilde) ortak satış çözümleri sağlar.|
|Anlaşma ataması|Yalnızca atanan satıcı, anlaşmaları görüntüleyebilir ve üzerinde işlem yapabilir.|Ekip üyeleri bir anlaşma üzerinde çalışan kişileri belirtmek için bir anlaşmaya eklenebilir, diğer başvuru yöneticilerinin bu anlaşmalar üzerinde görüntülenmesini veya bu anlaşmaları üzerinde hareket etmesinin engellenmesi yoktur.|
|Müşteri kuruluşu|Serbest form metin girişi.|Yalnızca birkaç karakter yazarak [Müşteri kuruluşunda](manage-co-sell-opportunities.md#select-your-customer) [D&B veritabanına](https://www.dnb.com/) göre arama yapabilirsiniz. Yasal ad ve adres seçime göre otomatik olarak doldurulur.|
|Müşteri iletişim|Zorunlu değildir.|Özel işlem hattı paylaşımı için zorunlu değildir. Microsoft satıcısı ortak satış isteğine katılmak için davet edildiyse gereklidir.|
|Genel API|Kullanılamıyor.|[Referansları](/partner/develop/referrals) program aracılığıyla yönetmek için İş Ortağı Merkezi API.|

## <a name="map-the-fields-in-psc-to-the-corresponding-fields-in-partner-center"></a>PSC'de alanları, psc'de karşılık gelen İş Ortağı Merkezi

Bu bölüm, PSC için gösterilen seçili ekran görüntülerini ortak satış fırsatları bölümündeki ilgili görünümle İş Ortağı Merkezi karşılar.

Her ekran görüntüsü çifti üzerinde numaralı, sarı veya kırmızı daireler görebilirsiniz:

- **Sarı daireler ne anlama geliyor?** Numaralı, sarı daireler her PSC ekran görüntüsünde ilk olarak görünür. Daha sonra, altında aynı İş Ortağı Merkezi bir yardımcı ekran görüntüsü bulabilirsiniz.

   PSC'de her alanın veya özniteliğin İş Ortağı Merkezi eşlemesini görmek için, ilgili iki ekran görüntüsünde numaralı daireleri birlikte eşler. Örneğin, birincide numaralı sarı "1"i, PSC ekran görüntüsünü numaralı, ikincisinde sarı "1" ile, altta İş Ortağı Merkezi ekran görüntüsüyle eşleyebilirsiniz.

- **Kırmızı daire ne anlama geliyor?** Bir ekran görüntüsünde kırmızı bir daire görüyorsanız, PSC alanı bu ekran görüntüsünde İş Ortağı Merkezi.

PSC'den İş Ortağı Merkezi alan eşlemeleri aşağıdaki alanlar için gösterilir:

1. Ortak satış fırsatları varsayılan görünümüyle İş Ortağı Merkezi PSC giriş sayfası
1. İş Ortağı Merkezi anlaşma görünümüyle eşlenen PSC kılavuz görünümü
1. PsC anlaşma ayrıntıları görünümü, İş Ortağı Merkezi ayrıntıları görünümüyle eşlenmiş
1. Çözüm ekle görünümüne eşlenen PSC İş Ortağı Merkezi Görünümü
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
- Anlaşma rolü, BILGISAYARıNDA gerekli bir alan değildir. İş akışlarının hiçbirsinde görüntülenmez veya yakalanmaz. Satış anlaşmasına eklenen çözümlere göre Microsoft satıcı tarafında otomatik olarak türetilir.
- Son değiştirme tarihi, pc'de referans ayrıntıları sayfasında görüntülenmez. İş ortakları, anlaşmaları son güncelleştirme tarihine göre sıralamak için sıralama işlevini kullanabilir.

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3 - PsC Anlaşma ayrıntıları görünümü, İş Ortağı Merkezi

Üst (PSC) ekran görüntüsünde eşleşen, numaralı daireleri, altındaki İş Ortağı Merkezi ekran görüntüsüyle karşılaştırın. Eşleşen sayılar, PSC ile ilgili özelliği veya özniteliğini aşağıdaki İş Ortağı Merkezi. Kırmızı daireler, verilerde eşleşen alan veya alan İş Ortağı Merkezi.

> [!NOTE]
> Ekran görüntülerinin altında dikkat edilmesi gereken diğer noktalar da yer almaktadır.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="İş Ortağı Satış Bağlantısı (PSC) satış anlaşması ayrıntıları görünümü ile satış anlaşması ayrıntıları görünümü arasındaki alan İş Ortağı Merkezi gösteren görüntü." lightbox="images/pscmigration/deal-details-expanded.png":::

**Dikkat edilmesi gereken özel noktalar:**

- İş ortakları, iş ortağı anlaşması ayrıntı görünümünde düzenle düğmesini seçerek bir anlaşmayı düzenleyebilir (6). Düzenle düğmesi seçildikten sonra tüm alanlar düzenlenebilir hale gelecektir. Ardından anlaşmada yapılan düzenlemeleri kaydetme veya iptal etme seçeneğiniz vardır.
- Anlaşmayı aynı anlaşmada yinelenen olarak kapatma seçeneği İş Ortağı Merkezi.
- Müşteri Sonucu, İş Ortağı Merkezi. Müşteri etkileşimleri ile ilgili tüm ayrıntılar pc'nin Notlar bölümünde güncelleştirilebilir.
- Tahmini çözüm kapatma tarihi yalnızca aynı anda yalnızca OEM IOT anlaşmaları İş Ortağı Merkezi. Bu bilgiler diğer hiçbir anlaşma türü için görüntülenmez.
- Pc'de lisans programı gerekli değildir. Bu bilgiler, işlem sırasında seçilen çözümlere göre otomatik olarak algılanır.

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
- Ortak satış anlaşması yönetimi için İş Ortağı Merkezi rol vardır. Bu rol, referans yöneticisi rolüdir.

### <a name="7---notifications-in-psc-versus-partner-center"></a>7 - PSC ile İş Ortağı Merkezi arasındaki bildirimler

Üst (PSC) ekran görüntüsünde eşleşen, numaralı daireleri, altındaki İş Ortağı Merkezi ekran görüntüsüyle karşılaştırın. Eşleşen sayılar, PSC ile ilgili özelliği veya özniteliğini aşağıdaki İş Ortağı Merkezi. Kırmızı daireler, verilerde eşleşen alan veya alan İş Ortağı Merkezi.  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="İş Ortağı Satış Bağlantısı (PSC) bildirimleri ile İş Ortağı Merkezi arasındaki eşlemeyi gösteren görüntü."  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>PSC'den İş Ortağı Merkezi - Sık sorulan sorular

Aşağıdaki bölümlerde geçişle ilgili sık sorulan sorular yanıtlanmaktadır.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1 - Erişim iznim yoksa ne İş Ortağı Merkezi?

Atanmış rolleri almak için "Erişim yok" sayfasında listelenen yöneticilerinize başvurabilirsiniz. Referanslar bölümünde [okuma ve](permissions-overview.md#manage-referrals) yazma izni için referans yöneticisi rolüne ihtiyacınız olacak. Yalnızca iş profillerini yönetiyorsanız, iş ortağı merkezinde iş profili yönetici rolüne ihtiyacınız vardır.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="İş Ortağı Merkezi'da erişim yok deneyimini gösteren görüntü.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2 - Bana, İş Ortağı Merkezi'daki Referanslar bölümüne erişim izni İş Ortağı Merkezi?

Hesap [yöneticiniz,](permissions-overview.md#manage-mpn-membership-and-your-company) Referanslar sekmesine erişmenizi sağlar. Hesap yöneticinizi bulmak için **panonun** sağ üst köşesindeki dişli simgesinden Hesap ayarları'İş Ortağı Merkezi [seçin.](https://partner.microsoft.com/dashboard) Ardından, ikinci **düzey,** sol gezinti çubuğundan Kullanıcı yönetimi'ni seçin. Kullanıcı listesinin üst kısmında Filtre  açılan menüsünü seçin ve seçeneğini hesap yöneticisi **olarak belirleyin.** Sayfada ilgili e-posta adresleriyle birlikte tüm hesap yöneticileri görüntülenir. İş hesabınız için referans yöneticisi rolünü atamasını istemek için bunlardan birini sorun.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3 - Hesabımız için +yeni anlaşma düğmesi gridir. Anlaşmalar oluşturmaya başlamak için ne yapmam gerekir?

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

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9 - Müşteri kuruluşu eklemek zorunlu mu?

Evet, müşteri [kuruluşuna yeni](./manage-co-sell-opportunities.md#select-your-customer) bir kuruluş eklemek İş Ortağı Merkezi. İlk olarak müşterinin bulunduğu konumu arayarak başlayalım. Sahip olduğunuz ayrıntılara göre; Tam bina adı dahil olmak üzere belirli olabilir veya yalnızca şehir ayrıntılarını veabilirsiniz. Kuruluş araması, herhangi bir adres ayrıntısı girmek zorunda olmadığınız adla eşleşen tüm yasal varlıkları getirir. Tüm ayrıntılar seçilen kuruluşa göre otomatik olarak doldurulur.

### <a name="10---are-customer-contact-details-mandatory"></a>10 - Müşteri iletişim bilgileri zorunlu mu?

Oluşturmakta [olduğunu anlaşma türüne](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) bağlıdır. Yalnızca işlem hattınızı paylaşıyorsanız ve Microsoft satış kuruluşundan herhangi bir yardıma gerek yoksa, müşteri iletişim bilgilerini vermeyebilirsiniz. Microsoft satıcısından etkin bir şekilde yardım almak için ortak satışlar yaptıysanız müşteri iletişim bilgilerini de sağlayabilirsiniz. İş ortağı merkezinde ortak satış isteği oluşturmadan önce müşteriden açık onay alasınız.

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11 - Bir anlaşmaya kaç çözüm ekleyebilirim?

Bir satış anlaşmasına en fazla 50 çözüm (PSC'de 'ürünler' ile benzer) eklersiniz. PSC'den farklı olarak, ortak satışa uygun çözümleriniz, Microsoft birinci taraf SKÜ'ler ve diğer üçüncü taraf ortak satışa uygun çözümleriniz çözümlerini karma olarak kullanabilirsiniz. İş ortağı merkezinde seçilecek veya kullanılabilir olacak bir satış anlaşması rolü yoktur. Microsoft SKU'ları için isteğe bağlı olarak satış anlaşmasına eklenen her SKU için miktar ve fiyat eklenmiştir.

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12 - Satış anlaşması oluşturduklarından sonra Microsoft satıcısının ayrıntılarını ne zaman edinecekim?

Microsoft satıcılarına yalnızca Microsoft tarafında ilgili satıcı kişisi ile anlaşma oluşturulurken belirtilen tam yardım gereksinimi eşledikten sonra atanır. Atamadan sonra bile Microsoft satıcıları ortak satış davetini kabul etme veya reddetme seçeneğine sahip olur. Yalnızca bir satıcı tarafından ortak satış daveti kabul edilirse, anlaşma Microsoft satıcı iletişim bilgileriyle güncelleştirilir. Microsoft satıcıları için SLA, anlaşma üzerinde işlem yapması için 14 gündür. Bu, iş ortaklarının, zaman aşımına uğramadan önce anlaşma üzerinde işlem yapması gereken SLA 'dır.

### <a name="13---where-can-i-find-the-opportunity-id"></a>13-fırsat KIMLIĞINI nerede bulabilirim?

PSC 'deki fırsat KIMLIĞI, BILGISAYARDAKI anlaşma KIMLIĞIYLE aynıdır. Herhangi bir anlaşmayı açtığınızda anlaşma adının yanında anlaşma KIMLIĞINI bulabilirsiniz.

### <a name="14---how-can-my-pdm-get-access-to-pc"></a>14-PDM Bilgisayarıma nasıl erişeirim?

İş Ortağı Merkezi 'Ne doğrudan PSC 'nin aksine, PDMs 'niz tarafından erişilemez. Bu özelliği etkinleştirmek için aşağıda bahsedilen birden çok seçenek vardır.

- OCP Insights-PDMs yalnızca bunlarla ilgili anlaşmaları ve ilerlemeyi görüntülüyorsanız, kuruluş görünümünüzü almak için OCP Insights portalını kullanabilirler. Bu bir iç araçtır ve yalnızca PDMs için kullanılabilir. OCP öngörülerinin şirketinizin kullanıcıları için sunulmadığını unutmayın.
- Iş Ortağı Merkezi 'nde Konuk Kullanıcı-PDM @microsoft.com Hesabınızı, iş ortağı merkezi 'nde Konuk Kullanıcı olarak ekleyebilir ve başvuruları görüntüleyebilmek ve bunlarla işlem yapabilmesi için başvuru Yöneticisi rolü atayabilirsiniz.
- Kiracınızda [Yeni bir Kullanıcı](./create-user-accounts-and-set-permissions.md#add-a-new-user) oluşturma-kendi kiracınızda yeni bir kullanıcı oluşturabilir ve bu ayrıntıları PDM ile paylaşabilir ve bu sayede hesabınızdaki diğer başvuru kullanıcılarına benzer başvuruları görüntüleyebilir ve bunlarla işlem yapabilir.

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>PSC 'deki hesabınız geçerli bir MPN ile ilişkili değilse, doğru MPN KIMLIĞINI bulma

Burada, PSC 'nin ' PSC geçersiz MPN KIMLIĞI ilişkilendirme sorunu ' içinde bir başlık gördüğünüz için doğru yerde olursunuz. Aşağıdaki nedenlerden dolayı hesabınız geçersiz bir MPN KIMLIĞINE bağlanmış olabilir

- Şirketinizde bir Iş Ortağı Merkezi hesabı yok.
- PDM 'niz, PSC hesabınızı Iş Ortağı Merkezi hesabınıza (MPNıD) bağlayan iç sistemlere hesabınızın MPN KIMLIĞINI girerken bir hata yaptı.
- Şirketiniz, Iş ortağı üyelik Merkezi 'nden (PMC) BILGISAYARA geçişi tamamlamadı.

İlk olarak, aşağıdaki adımları izleyerek doğru MPN KIMLIĞINI bulun

- İş Ortağı Merkezi oturum açın
- MPN kimliğini bulmak [için hesap ayarları belgelerinde](./partner-center-account-setup.md#locate-your-mpn-id) verilen kılavuzu kullanın.

Aşağıda, MPN kimliğiniz için tam olarak hangi konumda İş Ortağı Merkezi ekran görüntüsü verilmiştir

:::image type="content" source="images/pscmigration/findingMPNID.png" alt-text="İş ortağının MPN kimliğini bularak hesap ayarlarını gösteren resim."  lightbox="images/pscmigration/findingMPNID.png":::

seçin

- PDM'niz varsa, iş ortağı merkezi hesabınızdan MPN kimliğinizin doğru MPN kimliğiyle düzeltilmesini istemelerini sorun.
- PDM'niz yoksa, PSC başlığında gösterilen PSC hesap bilgilerini ve iş ortağı merkezi hesabınızdan doğru MPN kimliğini içeren PSC başlığında verilen adrese bir e-posta gönderin.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Satış anlaşmalarınızı oluşturmanıza ve yönetmenize yardımcı olacak İş Ortağı Merkezi

Ortak satış yardım konularını henüz okumadısanız, aşağıdaki kaynaklar iş ortağı merkezinde satış anlaşmalarını yönetmenize yardımcı olur.

|**Bunu yapmak için**   |**Bunu okuyun**   |
|-----------------------|:-----------------------|
|Ortak satış fırsatları sayfasındaki sekmeleri ve gezintiyi anlama|[Ortak satış bölümünde gezinme](./manage-co-sell-opportunities.md#navigating-the-co-sell-section)|
|D&B listesinden bir müşteri kuruluşu seçme |[Müşterinizi seçin](./manage-co-sell-opportunities.md#select-your-customer)|
|Anlaşma ayrıntıları bölümündeki alanları değiştirme|[Anlaşma ayrıntıları](./manage-co-sell-opportunities.md#deal-details)|
|Anlaşma ekibine takım üyelerinizi ekleme|[Çalışanlarınızı ekleme](./manage-co-sell-opportunities.md#add-team-members)|
|Ortak satış anlaşmasına yanıt verme|[Ortak satış anlaşmalarını yönetme](./manage-co-sell-opportunities.md#responding-to-a-co-sell-opportunity)
|İş Ortağı Merkezi'da kazandnız anlaşmaları İş Ortağı Merkezi |[Yeni bir anlaşma Kaydet](./register-deals.md)
|Başvuru öngörülerini edinin ve başvurularınızın nasıl çalıştığını öğrenin |[Referans içgörüleri](./referral-insights.md)
|İş profili oluşturma ve yönetme|[İş profilini yönetme](./create-a-marketing-profile.md)
|İş profiliniz için müşteri adaylarını yönetme |[Müşteri adaylarını yönetme](./manage-leads.md)|

## <a name="next-steps"></a>Sonraki adımlar


- İş ortağı satışları iş ortağı [Merkezi çalışma kitabına bağlanır](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) -iş ortaklarının satış süreçlerini ve rollerini Iş Ortağı Merkezi Ile Iş ortağı Sales Connect aracılığıyla yeni satış süreçleriyle hizalayın.
- [Iş Ortağı Merkezi ortak satış çalışma kılavuzu](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) -müşteri adaylarını yönetmek Için Iş Ortağı Merkezi aracılığıyla bir işletim modelini belirlemek için bir iş modeli veya ortak satış fırsatları ve anlaşmaları kaydetme.
- [Başvuru yönetimi destesi](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) -müşteri adaylarını yönetmek için görselleştirilen adım adım yönergeler ve Iş Ortağı Merkezi aracılığıyla ortak satış fırsatları.
- [Ticari Market 'Te yayımlama ve yönetme](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) -ticari Market 'Teki Iş Ortağı Merkezi aracılığıyla teklifler oluşturmak, yönetmek ve yayımlamak için görselleştirilen adım adım yönergeler.