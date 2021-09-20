---
title: iş ortağı Sales Bağlan (PSC) geçirme
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: microsoft iş ortaklarının iş ortağı Bağlan satışlarından (PSC) iş ortağı merkezi 'ne nasıl geçirebileceğini ve microsoft satıcıları tarafından gönderilen anlaşmalar oluşturma veya yönetme hakkında bilgi edinin.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.date: 09/08/2021
ms.openlocfilehash: 96106dd84d4889c9165daf41385d1092361101c4
ms.sourcegitcommit: 731a5e2725a72ecdae40189a3f52ab6b4a4c8058
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/20/2021
ms.locfileid: "128007278"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>iş ortağı satışları Bağlan (PSC) ile geçiş için iş ortağı merkezi 'nde (PC) ortak satış ile ilgili kılavuz

**Uygun roller**: Hesap Yöneticisi | Başvuru Yöneticisi | iş ortağı satışları Bağlan (PSC) satıcı | iş ortağı satışları Bağlan (PSC) yöneticisi | iş ortağı Sales Bağlan (PSC) anlaşma yöneticisi

bu makalede ortak satış Bağlan (PSC) ile iş ortağı merkezi 'ne (PC) geçiş yapan iş ortakları, iş ortağı merkezi 'nde ortak satış anlaşmaları oluşturmaya ve yönetmeye devam edebilmeleri için kılavuzluk sağlar.

> [!NOTE]
> Buradan geçiş hakkında PSC 'de bir başlık gördüğünüz için doğru yerde olursunuz. Bu kılavuz, PSC 'de anlaşmalar yöneten çözüm değerlendirmesi (SA) ve OEM lisanslama iş ortakları için geçerli değildir.

> [!IMPORTANT]
> 1 Nisan 2021 itibariyle, şirketiniz PSC içinde anlaşmalar oluşturamaz veya düzenleyemeyecektir. **Aynı zamanda PSC içindeki toplu dışa aktarma özelliğini kullanarak mevcut anlaşmalar verilerini indirebilirsiniz. Ayrıca, bu tarihten sonra PSC 'den Iş Ortağı Merkezi 'ne [Açık anlaşmalar geçirebilirsiniz](psc-to-pc.md#psc-deals-migration) .**
> 
> Üzerinde etkin olarak çalıştığınız ve IP ortak satışı ile uygun çözümleri içeren anlaşmalar varsa, iki seçeneğiniz vardır:
> 
> 1. "31 Mart 2021 tarihinden önce,
> 2. İş ortağı [Merkezi 'ne çalışarak, anlaşma](psc-to-pc.md#psc-deals-migration) üzerinde çalışmayı ve anlaşma kaydı başlatmayı daha fazla zaman alırsınız.

Şirketiniz, 30 Nisan 2021 ' den sonra PSC 'ye erişimi kaybederse de Iş Ortağı Merkezi 'nde, ortak satış anlaşmaları oluşturma, anlaşmaları yönetme ve Microsoft satıcıları tarafından size gönderilen anlaşmalar için işlem yapmaya yönelik her şeyi bulabilirsiniz.

Ancak farklılıklar olacaktır. Aşağıdaki kılavuz, Iş Ortağı Merkezi 'ne geçişinizi daha sorunsuz ve daha basit hale getirmenize yardımcı olabilir.

## <a name="things-to-know-before-moving"></a>Taşınmadan önce bilmeniz gerekenler

### <a name="if-you-are-a-psc-admin"></a>Bir PSC yöneticisiyseniz

- İş [Ortağı Merkezi](https://partner.microsoft.com/)'nde oturum açmak için bir iş e-postasına ihtiyacınız vardır.
- Iş Ortağı Merkezi [hesap yöneticisinin](permissions-overview.md)yardımıyla hesabınızı ayarlayın.
- Bu belgeyi okuyarak Iş Ortağı Merkezi 'nde ortak satışı yapmayı öğrenin.
- Tüm PSC kullanıcılarınız (yönetici, anlaşma Yöneticisi ve satıcı rolleri) için Iş Ortağı Merkezi 'nde Kullanıcı hesapları ayarlayın ve bunlara [referans yönetici rolleri](permissions-overview.md)atayın.

>[!IMPORTANT]
> PSC başlığında gösterilen Microsoft İş Ortağı Ağı (MPN) KIMLIĞININ Iş Ortağı Merkezi 'nde MPN konumları listesinde bulunduğundan emin olun.

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="İş ortaklarının MPN KIMLIĞINI bulabileceği PSC başlığını gösteren resim.":::

 mpn kimliğinin bir iş ortağı merkezi mpn konumu olarak göründüğünü doğrulamak için, iş ortağı merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın, ardından ekranın sağ üst kısmındaki **Ayarlar** (dişli simgesi) ve ardından **Account Ayarlar**' ı seçin. İkinci düzey, sol gezinti menüsünde, Iş Ortağı Merkezi hesabıyla ilişkili tüm MPN kimliklerinin ve konumların listesini görmek için **konumlar** ' ı seçin.

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

  :::image type="content" source="images/pscmigration/account-admin.gif" alt-text="İş ortağı ayarları Kullanıcı Yönetimi sayfasında hesap yöneticileri 'ni gösteren resim.":::

>[!Important]
>- Rolünüz yalnızca PSC 'deki kullanıcıları yönetmeyi içeriyorsa, şirketinizin hesap yöneticisinden Iş Ortağı Merkezi 'nde [Hesap Yöneticisi](permissions-overview.md#manage-mpn-membership-and-your-company) rolünü atamasını isteyin. 
>- Rolünüzde ortak satış fırsatlarını yönetme de varsa, [Başvurular yönetici](permissions-overview.md#manage-referrals) rolü atanmasını isteyin.
> - Aynı zamanda PSC yöneticileri arasında bir değişiklik yönetimi liderine aday bir fikir elde etmek iyi bir fikirdir. Bunun yapılması, tüm PSC yöneticilerinin Iş ortağı merkezi hesap yöneticilerine ayrı olarak ulaşmasını önler. Bunun yerine, değişiklik Yönetimi lideri daha sonra Iş ortağı merkezi hesap yöneticisi ile çalışan birincil kişidir.

## <a name="user-migration"></a>Kullanıcı geçişi

Iş Ortağı Merkezi 'nde hesabınızı ayarladıktan sonra, iş ortağı merkezi rollerini şirketinizin çalışanlarına otomatik olarak atamak için ortak satış fırsatları sayfasında Kullanıcı Geçiş Sihirbazı 'nı kullanın.

>[!Note]
> Kullanıcı geçişi yalnızca, şirketinizin [hesap yöneticileri](permissions-overview.md#manage-mpn-membership-and-your-company) tarafından gerçekleştirilebilir. Hesap Yöneticisi rolüne sahip değilseniz, Kullanıcı geçiş sihirbazının yardımıyla Kullanıcı hesaplarını ayarlamaya yardımcı olabilecek bir hesap yöneticisi bulun.

:::image type="content" source="images/pscmigration/user-migration.gif" alt-text="Kullanıcı Geçiş Sihirbazı 'nı gösteren resim.":::

Hesap yöneticileri, referanslar kılavuzunun yanındaki ortak satış fırsatları sayfasında bir PSC Kullanıcı Geçiş Sihirbazı bağlantısı görür. Bağlantıyı seçerek Kullanıcı geçişini başlatabilirler. Kullanıcı geçişini başlatmak için Yöneticiler bağlantıyı seçebilir. Tüm kullanıcılara Iş Ortağı Merkezi 'nde uygun roller atanıncaya kadar, bu kullanıcı geçiş adımını birden çok kez gerçekleştirebilirler.

Kullanıcı geçiş tablosu aşağıdaki ayrıntılara sahiptir:

- Kullanıcı hesabı-çalışanın e-posta KIMLIĞI
- PSC iş ortağı hesabı-çalışanın PSC içinde ilişkilendirildiği hesap
- PSC Kullanıcı rolü-PSC içinde öğesine atanan üç rolden biridir.
- BILGISAYAR MPN konumu-kullanıcıya ilgili Iş Ortağı Merkezi (PC) rolleri verilecek konum. PSC iş ortağı hesabı MPN, izin atamak üzere Iş Ortağı Merkezi 'nde eşdeğer MPN konumunu bulmak için kullanılır. Kuruluşun tamamı, vOrg MPN KIMLIĞINI gösterir.
- BILGISAYAR Kullanıcı rolü-çalışanlar, PSC Kullanıcı rollerine göre rollere atanır. PSC 'deki yöneticiye, Iş Ortağı Merkezi 'nde referanslar yönetici rolleri atanır. Satıcı, Iş Ortağı Merkezi 'nde başvuru Kullanıcı rolüne atanır. İş Ortağı Merkezi rolleri ve bu rollere sahip olan kullanıcılar, iş ortağı [Merkezi 'nde çalışması gereken bir şirketin kullanıcılarına Kullanıcı rolleri ve Izinleri atama](permissions-overview.md#manage-referrals)konusunun Iş Ortağı Merkezi 'Nde Iş Ortağı Merkezi 'nde neler yapabileceğini öğrenin.
- bilgisayar AAD kiracısı-kullanıcıların iş ortağı merkezi 'nde atandığı Microsoft Azure Active Directory (Azure AD) kiracısı
- Durum-geçiş durumunun üç olası durumu vardır
    - **Geçirilmedi** -kullanıcıya hiçbir Iş ortağı merkezi başvuru rolü atanmamış
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
    - Kullanıcının var olan rolünü doğrulayabilirsiniz. iş ortağı merkezi 'nin sağ üst köşesinde **Ayarlar** (dişli simgesi) ve ardından **hesap ayarları**' nı seçin. İkinci bir sol gezinti menüsünü gördüğünüzde **Kullanıcı yönetimi** ' ni seçin ve Kullanıcı için arama yapın.

## <a name="psc-deals-migration"></a>PSC anlaşmalar geçişi

Kullanıcı geçişini tamamladıktan sonra, PSC 'den Iş Ortağı Merkezi 'ne uygun tüm açık anlaşmaları getirmek için ortak satış fırsatları sayfasında anlaşmalar Geçiş Sihirbazı 'nı kullanın. **Anlaşmalar geçiş bağlantısı yalnızca ortak merkezindeki tüm kuruluş kapsamına sahip olan, yalnızca görünür başvuru yöneticileri olacaktır.** Ortak satış fırsatları sayfasının sağ üst kısmında **"PSC anlaşmaları geçişi"** adlı bir bağlantı olacak ve bu bağlantı satış anlaşması geçiş sihirbazını açacaktır.

Anlaşma geçişini başlatmadan önce bu bölümü okuyun.

**Geçişe uygun**

Yalnızca bazı anlaşmalar PSC 'den Iş Ortağı Merkezi 'ne geçişe uygundur. Bu Geçiş Sihirbazı, iş ortaklarının, BT 'nin müşterileri ile çalışmaya devam ettikleri Iş Ortağı Merkezi 'ne anlaşmalar getirmelerini sağlamak için oluşturulmuştur. **Yalnızca geçerli iş ortağı hesabı ayrıntıları (geçerli MPN ID) ile 1 Ocak 2020 ' den oluşturulan ve açık durumda olan anlaşmalar geçiş için uygun değildir.**

**Geçiş için uygun değil**

- Çözüm değerlendirmesi anlaşmaları, anlaşma geçişi için uygun değildir
- OEM lisanslama iş anlaşmaları, anlaşma geçişi için uygun değildir
- PSC 'de Kazanıldı olarak işaretlenen tüm bir anlaşma geçiş için uygun değildir. Kazanıldı olarak işaretlenen anlaşmalar için uygun olursa, kayıt işlemi yapın.

## <a name="pre-requisites-for-deal-migration"></a>Anlaşma geçişi için önkoşulların önkoşulları

Iş Ortağı Merkezi 'nden anlaşma geçişini başlatmadan önce, başarılı bir geçiş için PSC 'deki anlaşmaları ayarlamak üzere aşağıdaki yönergeleri izleyin.

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

Tüm uygun anlaşmalar için anlaşmayla ilgili tüm eksik ayrıntıları eklemek üzere PSC 'deki toplu indirme ve karşıya yükleme yeteneklerini kullanabilirsiniz.

>[!Note]
> Yukarıdaki ön koşullar karşılanmadığında bile dağıtım geçişi başarılı olur. Ancak, Iş Ortağı Merkezi 'nde yukarıda bahsedilen gerekli alanlardan herhangi biri kullanılabilir değilse, anlaşma durumunu değiştiremezsiniz. Daha sonra, Iş ortağı merkezindeki anlaşmalar üzerinde çalışmaya başlamak için gerekli tüm bilgileri girmeniz gerekir. **Iş Ortağı Merkezi 'ne geçirmeden önce PSC 'deki uygun anlaşmaları temizlemeniz önemle tavsiye edilir.**

Iş Ortağı Merkezi ' nde anlaşma geçişi tek tıklamayla deneyim olarak oluşturulmuştur. Tüm yapmanız gereken, şirketiniz uygun anlaşmaları geçirmeye hazırsa **"anlaşmaları geçir"** düğmesini seçin. **PSC 'den geçiş yapmak istediğiniz anlaşmaları seçemezsiniz. Iş Ortağı Merkezi 'ne herhangi bir anlaşmayla geçiş yapmak istemiyorsanız, Geçişe başlamadan önce onları PSC 'de Kapalı durumuna taşıyın.**

>[!Note]
> Geçişi başlattıktan sonra, **yapılan anlaşmalar için 24 saate kadar sürebilir**.

Geçiş tamamlandıktan sonra, başlık iletisinin durumu geçiş raporuna yönelik bir bağlantıyla tamamlandı olarak değiştirilir. PSC 'den Iş Ortağı Merkezi 'ne geçirilen anlaşmalar hakkındaki ayrıntıları görüntülemek için raporu indirin.

Rapor aşağıdaki ayrıntıları içerir.

1. **Iş Ortağı Merkezi KATıLıM kimliği** -bir görevlendirmede tüm anlaşmalar Için Iş ortağı merkezindeki benzersiz tanımlayıcı. İş ortağı için iki adet anlaşmalar vardır ve bir iş ortağı merkezi 'nde ortak satış katılımında Microsoft için bir görevlendirme vardır.
2. **Iş ortağı merkezi başvuru kimliği** -iş ortağına ait olan Işlem Için Iş Ortağı Merkezi 'nde benzersiz tanımlayıcı.
3. **Anlaşma adı** -PSC 'de ele verilen tanımlayıcı.
4. **PSC anlaşma kimliği** -anlaşma için PSC içindeki benzersiz tanımlayıcı.
5. **Hatalar** -belirli bir anlaşmayı geçirirken herhangi bir hata olup olmadığını gösterir.

Başarılı bir şekilde geçirilmiş tüm anlaşmalar PSC içinde görünür olmayacaktır. İş Ortağı Merkezi 'nde anlaşma kaydını tamamlama dahil, iş ortağı Merkezi ' nde geçirilen anlaşmalar üzerinde çalışmaya devam edebilirsiniz. Ortak satış anlaşmaları için Microsoft satıcıları ile etkileşimlerde hiçbir değişiklik olmayacaktır.

PSC 'den geçirilen anlaşmalar, gelen ve giden sekmelerinde, anlaşma kaynağına bağlı olarak kullanılabilir. Şirketiniz tarafından paylaşılan tüm anlaşmalar giden sekmesinde kullanıma sunulacaktır ve Microsoft tarafından başlatılan anlaşmalar Iş Ortağı Merkezi 'nin gelen sekmesinde kullanıma sunulacaktır. Geçiş sonrası oluşturulacak iki tür anlaşmalar olacaktır.

1. Ortak satış **anlaşmaları** -PSC içinde ortak satış olarak işaretlenen anlaşmalar, Iş Ortağı Merkezi 'nde ortak satış anlaşmaları olarak oluşturulur.
2. **Ortak satış** olarak işaretlenmemiş anlaşmalar, Iş Ortağı Merkezi 'nde ortak çalışan anlaşmalar olarak oluşturulur. İş ortağı olarak çalışan anlaşmalar, Microsoft satıcılarına görünür ve Terminal durumuna (kazanıldı, kaybedildi) ulaşmadan önce ortak satış anlaşmaları olarak yükseltilebilir. Ayrıca, anlaşmadan uygun bir çözüm varsa, iş ortağı ile ilgili anlaşmalar, anlaşma kaydı için uygun olur.

>[!Important]
> Bazı anlaşmalar geçirilmemiş olması nedeniyle herhangi bir hata oluşursa, **"anlaşmaları geçir" düğmesine tıklayarak anlaşma geçişini yeniden başlatabilirsiniz**. Yalnızca bazı uygun anlaşmalar varsa etkinleştirilecek. Bu Ayrıca, anlaşma geçişi başlatıldıktan sonra bazı yeni anlaşmalar için PSC 'de oluşturulan geçiş aşamasındaysanız de yararlı olacaktır.

Tüm anlaşmalar başarıyla geçirildikten sonra, " **anlaşmaları geçir** " düğmesi **devre dışı** olarak **"geçirilecek anlaşmalar yok** " adlı başlık görüntülenir.

Kullanıcı geçişini ve/veya geçiş işlemini tamamladıktan sonra, geçiş stratejisine karar vermek için aşağıdaki kılavuzu kullanın:

Şirketinizde bir Iş ortağı Geliştirme Yöneticisi (PDM) varsa-Iş Ortağı Merkezi hesabınız ayarlandığında ve kullanıcılarınız üzerine taşınır ve roller ve izinler varsa, ortak satış etkinliklerinizi Iş Ortağı Merkezi 'ne taşıyabilirsiniz. Geçiş tamamlanma son tarihine kadar beklemek yerine PDM, tüm yeni anlaşmalarınızın Iş Ortağı Merkezi 'ne akmasını sağlayan bir anahtar yapmasını bildirin.

>[!Note]
>Bu anahtarı yaptıktan sonra, yalnızca PSC 'deki mevcut etkin anlaşmalar üzerinde işlem yapabilirsiniz. Yeni anlaşmalar oluşturmayabilir veya PSC 'de Microsoft satıcılarından herhangi bir anlaşmalar alamazsınız.

Şirketiniz bir PDM içermiyorsa, tüm Kullanıcı hesaplarının tüm kullanıcılar tarafından ayarlandığından ve doğrulandığından emin olun. Iş Ortağı Merkezi 'nde ortak satış ile başlayabilmeniz için, bir e-posta ile ve PSC 'deki bir başlık aracılığıyla bildirimde bulunacaktır. PSC 'deki mevcut etkin anlaşmaları hala yönetmeniz gerektiğini unutmayın.

>[!Important]
> Kazanıldı olarak işaretlenen anlaşmaları kaydetmek için 30 Nisan 2021 tarihine kadar olursunuz.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>PSC yöneticileri, PSC anlaşma yöneticileri ve PSC satıcıları için sonraki adımlar

Iş Ortağı Merkezi 'nde ortak satışı yapmayı öğrenin.
Bu önemli bir adımdır ve Iş Ortağı Merkezi 'nde ortak satış için hazırlıklı olmanıza yardımcı olur. Verimli bir şekilde işbirliği yapabilmeniz için iş akışlarını ve iş ortağı merkezindeki değişiklikleri anlayın. Bu belgeyi tamamen okuyarak başlayın. [Ortak satış deneyimi galerisinde](https://aka.ms/cosellexperience)uygun bir kaynak kümesi de mevcuttur.

## <a name="major-differences-between-psc-and-partner-center-workflows"></a>PSC ve Iş ortağı merkezi iş akışları arasındaki önemli farklılıklar

|**Senaryo**|**iş ortağı satışları Bağlan**|**İş Ortağı Merkezi**|
|-----|:-----|:-----|
|Kullanıcı rolleri|PSC 'in yönetici, anlaşma Yöneticisi ve satıcı rolleri vardır.|İş ortağı merkezi yalnızca tüm anlaşmalar için hem okuma hem de yazma izni veren [başvuru Yöneticisi](permissions-overview.md#manage-referrals) rolüne sahiptir.|
|Ortak satış için Microsoft 'a davet etme|Microsoft satıcı tarafından başlatılan, iş ortağı tarafından açık bir sorun yoktur.|Bir Microsoft satıcı yardımı bir anlaşma için gerekliyse iş ortağının [açık bir istek](manage-co-sell-opportunities.md#add-solutions) yapması gerekir. Microsoft satıcının isteği reddetme seçeneği vardır.|
|Süre sonu|Bir anlaşma süre sonu kavramı yoktur.|İş ortağı tarafından kabul edilmediyse iş ortağı gelen anlaşmalar 14 gün içinde sona erer. Ayrıca, iş ortağı giden anlaşmalar, Microsoft satıcı bunları 14 gün içinde işlem yapmaz.|
|Microsoft satıcı ayrıntıları|Bir anlaşma oluşturulduktan hemen sonra görünür.|Microsoft satıcı ayrıntıları, yalnızca satıcı iş ortağından ortak satış davetini kabul ettiğinde ortak olarak paylaşılır.|
|[Özel işlem hattı](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Kullanılamıyor.|İş ortakları, Microsoft satıcıları için görünürlük vermeden kendi işlem hatlarını paylaşabilir.|
|Çözümler|Yalnızca bir fiyat listesine ait olan çözümler bir başa eklenebilir.|İş ortağı, aşağıdaki listelere ait [çözümler](manage-co-sell-opportunities.md#add-solutions) ekleyebilir. a) Microsoft 'un ilk taraf kataloğundan (PSC 'deki Işlem anlaşma rolüne benzer) ve c) çözümleri, diğer üçüncü taraf iş ortaklarından (PSC 'deki ISV anlaşma rolüne benzer şekilde) ortak satış çözümleri sağlar.|
|Anlaşma ataması|Yalnızca atanan satıcı, anlaşmaları görüntüleyebilir ve üzerinde işlem yapabilir.|Ekip üyeleri bir anlaşma üzerinde çalışan kişileri belirtmek için bir anlaşmaya eklenebilir, diğer başvuru yöneticilerinin bu anlaşmalar üzerinde görüntülenmesini veya bu anlaşmaları üzerinde hareket etmesinin engellenmesi yoktur.|
|Müşteri kuruluşu|Serbest form metin girişi.|Yalnızca birkaç karakter yazarak [Müşteri kuruluşunda](manage-co-sell-opportunities.md#select-your-customer) [D&B veritabanına](https://www.dnb.com/) göre arama yapabilirsiniz. Yasal ad ve adres seçime göre otomatik olarak doldurulur.|
|Müşteri iletişim|Zorunlu değildir.|Özel işlem hattı paylaşımı için zorunlu değildir. Microsoft satıcı, ortak satış isteğine katılmaya davet edildiyseniz gereklidir.|
|Genel API|Kullanılamıyor.|[Referansları](/partner/develop/referrals) program aracılığıyla yönetmek için İş Ortağı Merkezi API.|

## <a name="map-the-fields-in-psc-to-the-corresponding-fields-in-partner-center"></a>PSC'de alanları ilgili alanlara eşleme İş Ortağı Merkezi

Bu bölüm, PSC için gösterilen seçili ekran görüntülerini ortak satış fırsatları bölümündeki ilgili görünümle İş Ortağı Merkezi karşılar.

Her ekran görüntüsü çifti üzerinde numaralı, sarı veya kırmızı daireler görebilirsiniz:

- **Sarı daireler ne anlama geliyor?** Numaralı, sarı daireler her PSC ekran görüntüsünde ilk olarak görünür. Ardından, altında aynı İş Ortağı Merkezi bir yardımcı ekran görüntüsü bulabilirsiniz.

   PSC'de her bir alanın veya özniteliğin İş Ortağı Merkezi eşle eşle olduğunu görmek için, ilgili iki ekran görüntüsünde numaralı daireleri birlikte eşler. Örneğin, birincide numaralı, sarı "1"i, PSC ekran görüntüsünü numaralı, ikincisinde sarı "1" ile, altta İş Ortağı Merkezi ekran görüntüsüyle eşleyebilirsiniz.

- **Kırmızı daire ne anlama geliyor?** Bir ekran görüntüsünde kırmızı daire görüyorsanız, PSC alanı bir ekran görüntüsünde İş Ortağı Merkezi.

PSC'den İş Ortağı Merkezi alan eşlemeleri aşağıdaki alanlar için gösterilir:

1. Ortak satış fırsatları varsayılan görünümüyle İş Ortağı Merkezi PSC giriş sayfası
1. İş Ortağı Merkezi anlaşma görünümüne eşlenmiş PSC kılavuz görünümü
1. PsC anlaşma ayrıntıları görünümü, İş Ortağı Merkezi ayrıntıları görünümüyle eşlenmiş
1. Çözüm ekle görünümüne eşlenen PSC İş Ortağı Merkezi Görünümü
1. Kullanıcı yönetimi görünümüyle eşlenen PSC İş Ortağı Merkezi yönetimi görünümü
1. Kullanıcı rolü atama görünümüyle eşlenen PSC İş Ortağı Merkezi atama görünümü
1. PsC bildirimleri görünümü, İş Ortağı Merkezi görünümüyle eşlenmiş

### <a name="1---psc-home-page-mapped-to-the-partner-center-co-sell-opportunities-default-view"></a>1 - Ortak satış fırsatları varsayılan görünümüne İş Ortağı Merkezi PSC giriş sayfası

Üst PSC ekran görüntüsü ile altındaki ekran görüntüsü arasındaki eşleşen, İş Ortağı Merkezi daireleri karşılaştırın. Eşleşen sayılar, PSC ile ilgili özelliği veya özniteliğini farklı bir İş Ortağı Merkezi. Kırmızı daireler, alanla eşleşen bir İş Ortağı Merkezi işaret ediyor.  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="İş Ortağı Satışları sayfasının giriş sayfası ile Bağlan ortak satış fırsatlarının varsayılan görünümü arasındaki alan eşlemelerini gösteren İş Ortağı Merkezi." lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>2 - İş Ortağı Merkezi anlaşma görünümüne eşlenmiş PSC kılavuz görünümü

Üst PSC ekran görüntüsü ile altındaki ekran görüntüsü arasındaki eşleşen, İş Ortağı Merkezi daireleri karşılaştırın. Eşleşen sayılar, PSC ile ilgili özelliği veya özniteliğini farklı bir İş Ortağı Merkezi. Kırmızı daireler, alanla eşleşen bir İş Ortağı Merkezi işaret ediyor.  

> [!NOTE]
> Ekran görüntülerinin altında dikkat edilmesi gereken diğer noktalar da yer almaktadır.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="İş Ortağı Satışları (PSC) kılavuz görünümü ile Bağlan satış anlaşması görünümü arasındaki alan İş Ortağı Merkezi gösteren görüntü." lightbox="images/pscmigration/grid-view-expanded.png":::

**Dikkat edilmesi gereken özel noktalar:**

- PsC'nin İş Ortağı Merkezi liste görünümü yoktur.  Tüm anlaşmalar, müşteri bilgileri ve satış anlaşması türüyle birlikte en son alınan veya oluşturulma tarihine göre listelenir. Görünümde ilk anlaşma varsayılan olarak seçilidir. PSC tablo biçiminde görüntülenen değerlerin çoğu, satış anlaşması ayrıntı görünümünde İş Ortağı Merkezi.
- Anlaşma rolü, rol için gerekli bir İş Ortağı Merkezi. İş akışlarının hiçbirsinde görüntülenmez veya yakalanmaz. Satış anlaşmasına eklenen çözümlere göre Microsoft satıcı tarafında otomatik olarak türetilir.
- Son değiştirme tarihi, başvuru ayrıntıları sayfasında İş Ortağı Merkezi. İş ortakları, anlaşmaları son güncelleştirme tarihine göre sıralamak için sıralama işlevini kullanabilir.

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3 - PsC Anlaşma ayrıntıları görünümü, İş Ortağı Merkezi

Üst (PSC) ekran görüntüsünde eşleşen, numaralı daireleri, altındaki İş Ortağı Merkezi ekran görüntüsüyle karşılaştırın. Eşleşen sayılar, PSC ile ilgili özelliği veya özniteliğini farklı bir İş Ortağı Merkezi. Kırmızı daireler, verilerde eşleşen alan veya alan İş Ortağı Merkezi.

> [!NOTE]
> Ekran görüntülerinin altında dikkat edilmesi gereken diğer noktalar da yer almaktadır.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="İş Ortağı Satışları ve (PSC) satış Bağlan görünümü ile satış anlaşması ayrıntıları görünümü arasındaki alan İş Ortağı Merkezi gösteren görüntü." lightbox="images/pscmigration/deal-details-expanded.png":::

**Dikkat edilmesi gereken özel noktalar:**

- İş ortakları, iş ortağı anlaşması ayrıntı görünümünde düzenle düğmesini seçerek bir anlaşmayı düzenleyebilir (6). Düzenle düğmesi seçildikten sonra tüm alanlar düzenlenebilir hale gelecektir. Ardından anlaşmada yapılan düzenlemeleri kaydetme veya iptal etme seçeneğiniz vardır.
- Anlaşmayı aynı anlaşmada yinelenen olarak kapatma seçeneği İş Ortağı Merkezi.
- Müşteri Sonucu şu anda İş Ortağı Merkezi. Müşteri etkileşimleri ile ilgili tüm ayrıntılar, İş Ortağı Merkezi.
- Tahmini çözüm kapatma tarihi yalnızca aynı anda OEM IOT anlaşmaları İş Ortağı Merkezi. Bu bilgiler diğer hiçbir anlaşma türü için görüntülenmez.
- Lisanslama programı, lisanslama İş Ortağı Merkezi. Bu bilgiler, anlaşmada seçilen çözümlere göre otomatik olarak görüntülenir.

>[!Note]
>Kazanıldı veya kaybedildi olarak işaretlenen anlaşmalar daha sonra düzenlenemez. Anlaşmaları bu terminal durumları içine alırken dikkatli olun.

### <a name="4---psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>4 - 'Çözüm ekle' görünümüyle eşlenen PSC 'İş Ortağı Merkezi' görünümü

Üst (PSC) ekran görüntüsünde eşleşen, numaralı daireleri, altındaki İş Ortağı Merkezi ekran görüntüsüyle karşılaştırın. Eşleşen sayılar, PSC ile ilgili özelliği veya özniteliğini farklı bir İş Ortağı Merkezi. Kırmızı daireler, verilerde eşleşen alan veya alan İş Ortağı Merkezi.
  
:::image type="content" source="images/pscmigration/products.png" alt-text="İş Ortağı Satışları (PSC) ürün Bağlan görünümü ile çözüm ekleme görünümü arasındaki alan İş Ortağı Merkezi gösteren görüntü." lightbox="images/pscmigration/products-expanded.png":::

### <a name="5---user-management-in-psc-versus-partner-center"></a>5 - PSC'de kullanıcı yönetimi ile İş Ortağı Merkezi

Üst (PSC) ekran görüntüsünde eşleşen, numaralı daireleri, altındaki İş Ortağı Merkezi ekran görüntüsüyle karşılaştırın. Eşleşen sayılar, PSC ile ilgili özelliği veya özniteliğini farklı bir İş Ortağı Merkezi. Kırmızı daireler, verilerde eşleşen alan veya alan İş Ortağı Merkezi.  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="İş Ortağı Satışları (PSC) kullanıcı Bağlan giriş sayfası ile Hesap ayarları alanında İş Ortağı Merkezi Yönetim sayfası görünümü arasındaki alan eşlemelerini gösteren görüntü."  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="6---user-role-assignment-in-psc-versus-partner-center"></a>6 - PSC'de kullanıcı rolü ataması ile İş Ortağı Merkezi

Üst (PSC) ekran görüntüsünde eşleşen, numaralı daireleri, altındaki İş Ortağı Merkezi ekran görüntüsüyle karşılaştırın. Eşleşen sayılar, PSC ile ilgili özelliği veya özniteliğini farklı bir İş Ortağı Merkezi. Kırmızı daireler, verilerde eşleşen alan veya alan İş Ortağı Merkezi.  

:::image type="content" source="images/pscmigration/roles.png" alt-text="İş Ortağı Satışları (PSC) rol Bağlan görünümü ile rol atama görünümü arasındaki alan İş Ortağı Merkezi gösteren görüntü." lightbox="images/pscmigration/roles-expanded.png":::

**Dikkat edilmesi gereken özel noktalar:**

- PSC yöneticisinin eşdeğer rolü, hesap yöneticisi rolü İş Ortağı Merkezi.
- Ortak satış anlaşması yönetimi için İş Ortağı Merkezi rol vardır. Bu rol, referans yöneticisi rolüdir.

### <a name="7---notifications-in-psc-versus-partner-center"></a>7 - PSC'de bildirimler ve İş Ortağı Merkezi

Üst (PSC) ekran görüntüsünde eşleşen, numaralı daireleri, altındaki İş Ortağı Merkezi ekran görüntüsüyle karşılaştırın. Eşleşen sayılar, PSC ile ilgili özelliği veya özniteliğini farklı bir İş Ortağı Merkezi. Kırmızı daireler, verilerde eşleşen alan veya alan İş Ortağı Merkezi.  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="İş Ortağı SatışLarı ve (PSC) Bağlan eşlemesini ve İş Ortağı Merkezi gösteren görüntü."  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>PSC'den İş Ortağı Merkezi - Sık sorulan sorular

Aşağıdaki bölümlerde geçişle ilgili sık sorulan sorular yanıtlanmaktadır.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1 - Erişim iznim yoksa ne İş Ortağı Merkezi?

Atanmış rolleri almak için "Erişim yok" sayfasında listelenen yöneticilerinize başvurabilirsiniz. Referanslar bölümünde [okuma ve](permissions-overview.md#manage-referrals) yazma izni için referans yöneticisi rolüne ihtiyacınız olacak. Yalnızca iş profillerini yönetiyorsanız, iş profili yöneticisi rolünüz İş Ortağı Merkezi.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="İş Ortağı Merkezi'da erişim yok deneyimini gösteren görüntü.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2 - Who bölümündeki Referanslar bölümüne erişim izni İş Ortağı Merkezi?

Hesap [yöneticiniz Referanslar](permissions-overview.md#manage-mpn-membership-and-your-company) sekmesine erişmenizi sağlar. Hesap yöneticinizi bulmak için **panonun** sağ üst köşesindeki dişli simgesinden Hesap ayarları'İş Ortağı Merkezi [seçin.](https://partner.microsoft.com/dashboard) Ardından, ikinci **düzey,** sol gezinti çubuğundan Kullanıcı yönetimi'ni seçin. Kullanıcı listesinin üst kısmında Filtre  açılan menüsünü seçin ve seçeneğini hesap yöneticisi **olarak belirleyin.** Sayfada ilgili e-posta adresleriyle birlikte tüm hesap yöneticileri görüntülenir. İş hesabınız için referans yöneticisi rolünü atamasını istemek için bunlardan birini sorun.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3 - Hesabımız için +yeni anlaşma düğmesi gridir. Anlaşma oluşturmaya başlamak için ne yapabilirim?

Bu yalnızca, mpN kuruluşuna bağlı ortak satışa hazır çözüm yoksa ve bu çözümde İş Ortağı Merkezi. Çözümlerinizin MPN kimliğinin düzeltilmesi için PDM'nize başvurun veya sorundan bahsederek bir destek bileti oluşturun: "PSC geçişi sonrasında yeni satış anlaşması düğmesi gri."

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4 - PSC gibi kuruluştan belirli bir kişiye satış anlaşması atay musunuz?

Takım üyelerini belirli bir satış anlaşmasına at attayarak. Diğer referans yöneticilerinin bu anlaşmaları görüntülemesini veya bu anlaşmalara göre hareket etmelerini engellemez.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5 - Bana atanan tüm anlaşmaların bir görünümü var mı?

Kullanıcı düzeyinde bir sekme olan sık kullanılanlar özelliğini kullanabilirsiniz. Anlaşmalara hızlı erişim elde etmek için size sık kullanılanlar olarak atanan tüm anlaşmaları işaretlebilirsiniz.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6 - Anlaşmalar için salt okunur bir görünüm var mı?

Hayır, referanslar bölümünde anlaşmaların salt okunur bir görünümü yoktur. Tüm referans yöneticileri tüm anlaşmalara tam okuma ve yazma erişimine sahip olur.

### <a name="7---how-can-i-register-a-deal-after-marking-it-as-won"></a>7 - Anlaşmayı kazandı olarak işaretledikten sonra nasıl kayıt olabilirim?

Anlaşma aşağıdaki ölçütleri karşılarsa, anlaşma kaydını başlatmak için bir açılır [pencere görüntülenir.](./register-deals.md)

- Anlaşmada teşvike uygun bir çözüm vardır.
- Microsoft satıcısı satış anlaşmasına katılmak için davet edildi veya sizi satış anlaşmasına davet etti.
- Microsoft kartı, Kabul Edildi veya Kazanıldı İş Ortağı Merkezi.

### <a name="8---i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>8 - Anlaşma Kaydı bölümünde "+Yeni anlaşma kaydı" düğmesini seçerek hata iletisi alıyorum. Anlaşmalarımı nasıl kaydederim?

**+Yeni satış anlaşması** kaydı düğmesi yalnızca ISV bağlantı programına kayıtlı iş ortakları tarafından satış anlaşmasına karşılık gelen ortak satış fırsatı olmayan bir satış anlaşması kaydetmek için İş Ortağı Merkezi. Ortak satış fırsatıyla anlaşmaları kaydetmek için, anlaşma kazanildi olarak işaretlendiğinde ve anlaşma kaydı ölçütlerini karşılarsa bir açılır pencere görüntülenir.

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9 - Müşteri kuruluşu eklemek zorunlu mu?

Evet, müşteri [kuruluşuna yeni](./manage-co-sell-opportunities.md#select-your-customer) bir kuruluş eklemek İş Ortağı Merkezi. İlk olarak müşterinin bulunduğu konumu arayarak başlayalım. Sahip olduğunuz ayrıntılara göre; Tam bina adı dahil olmak üzere belirli olabilir veya yalnızca şehir ayrıntılarını veabilirsiniz. Kuruluş araması, herhangi bir adres ayrıntısı girmek zorunda olmadığınız adla eşleşen tüm yasal varlıkları getirir. Tüm ayrıntılar seçilen kuruluşa göre otomatik olarak doldurulur.

### <a name="10---are-customer-contact-details-mandatory"></a>10 - Müşteri iletişim bilgileri zorunlu mu?

Oluşturmakta [olduğunu anlaşma türüne](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) bağlıdır. Yalnızca işlem hattınızı paylaşıyorsanız ve Microsoft satış kuruluşundan herhangi bir yardıma gerek yoksa, müşteri iletişim bilgilerini vermeyebilirsiniz. Microsoft satıcısından etkin bir şekilde yardım almak için ortak satışlar yaptıysanız müşteri iletişim bilgilerini de sağlayabilirsiniz. Bir ortak satış isteği oluşturmadan önce müşteriden açık bir onay İş Ortağı Merkezi.

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11 - Bir anlaşmaya kaç çözüm ekleyebilirim?

Bir satış anlaşmasına en fazla 50 çözüm (PSC'de 'ürünler' ile benzer) eklersiniz. PSC'den farklı olarak, ortak satışa uygun çözümleriniz, Microsoft birinci taraf SKÜ'ler ve diğer üçüncü taraf ortak satış uygun çözümlerinden çözümlerinizi karma olarak kullanabilirsiniz. Bu rolde seçilecek veya kullanılabilir bir satış İş Ortağı Merkezi. Microsoft SKU'ları için isteğe bağlı olarak satış anlaşmasına eklenen her SKU için miktar ve fiyat eklenmiştir.

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12 - Satış anlaşması oluşturduklarından sonra Microsoft satıcısının ayrıntılarını ne zaman edinecekim?

Microsoft satıcılarına yalnızca Microsoft tarafında ilgili satıcı kişisi ile satış anlaşması oluşturulurken belirtilen tam yardım gereksinimi eşledikten sonra atanır. Atamadan sonra bile Microsoft satıcıları ortak satış davetini kabul etme veya reddetme seçeneğine sahip olur. Yalnızca bir satıcı tarafından ortak satış daveti kabul edilirse, anlaşma Microsoft satıcı iletişim bilgileriyle güncelleştirilir. Microsoft satıcılarının satış anlaşmasına göre hareket etmek için SLA'sı 14 gündür. İş ortaklarının süresi dolmuş durumuna gelmeden önce anlaşma üzerinde hareket etmek zorunda olduğu SLA'dır.

### <a name="13---where-can-i-find-the-opportunity-id"></a>13 - Fırsat kimliğini nerede bulamıyorum?

PSC'deki Fırsat Kimliği, İş Ortağı Merkezi. Herhangi bir anlaşmayı a açmak için anlaşma adının yanında anlaşma kimliğini bulabilirsiniz.

### <a name="14---how-can-my-pdm-get-access-to-partner-center"></a>14 - PDM'm İş Ortağı Merkezi?

İş Ortağı Merkezi PSC'den farklı olarak PDM'ler tarafından erişilemez. Bu özelliği etkinleştirmek için aşağıda belirtilen birden çok seçenek vardır.

- OCP Analizler - PDM'ler yalnızca anlaşmaları ve onlarla ilgili ilerlemeyi görüntülüyorsa, kuruluş görünümünü elde etmek için Tek Ticari İş Ortağı (OCP) Analizler portalını kullanabilirler. Bu bir iç araçtır ve yalnızca PDM'ler için kullanılabilir. OCP içgörüleri, şirket kullanıcıları için kullanılamaz.
- İş Ortağı Merkezi konuk kullanıcı - PDM hesabını İş Ortağı Merkezi bir konuk kullanıcı olarak ekleyebilir ve referansları görüntüleysin ve bunlar üzerinde eyleme geçsin diye onlara referans yöneticisi rolü @microsoft.com atabilirsiniz.
- Kiracınız [içinde yeni](./create-user-accounts-and-set-permissions.md#add-a-new-user) kullanıcı oluşturma - Kendi kiracınız içinde yeni bir kullanıcı oluşturabilir ve bu ayrıntıları PDM ile paylaşarak, hesabın diğer referans kullanıcılarına benzer referansları görüntülemelerini ve bu kullanıcılara göre hareketlerini gerçekleştirebilirsiniz.

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>PSC'deki hesabınız geçerli bir MPN ile ilişkili değilse doğru MPN kimliğini bulma

PSC'de 'PSC geçersiz MPN ID ilişkilendirme sorunu' başlığıyla ilgili bir başlık gördükten dolayı buradaysanız, doğru yerdesiniz demektir. Hesabınız aşağıdaki nedenlerden dolayı geçersiz bir MPN kimliğine bağlanmış olabilir

- Şirketinizin bir İş Ortağı Merkezi yok.
- PDM'niz, PSC hesabınızla İş Ortağı Merkezi hesabınıza (MPN ID) bağlantı olan iç sistemlerde hesabınıza mpN kimliğini girerken bir hata yaptı.
- Şirket, Partner Membership Center(PMC) İş Ortağı Merkezi.

İlk olarak aşağıdaki adımları takip edin ve doğru MPN kimliğini bulun.

1. İş Ortağı Merkezi oturum [açın.](https://partner.microsoft.com/dashboard)
2. MPN kimliğini bulmak [için hesap ayarları belgelerinde](./partner-center-account-setup.md#locate-your-mpn-id) verilen kılavuzu kullanın.

Aşağıda, mpN kimliğiniz için tam olarak hangi konumu İş Ortağı Merkezi ekran görüntüsü verilmiştir.

:::image type="content" source="images/pscmigration/finding-mpn-id.png" alt-text="İş ortağının MPN kimliğini bularak hesap ayarlarını gösteren resim."  lightbox="images/pscmigration/finding-mpn-id.png":::

- PDM'niz varsa, mpN kimliğinizin hesaptan doğru MPN kimliğiyle düzeltilmesini İş Ortağı Merkezi.
- PDM'niz yoksa, PSC başlığında gösterilen PSC hesap bilgilerini ve psc hesabınızdan doğru MPN kimliğini içeren PSC başlığında verilen adrese bir e-İş Ortağı Merkezi gönderin.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Satış anlaşmalarınızı oluşturmanıza ve yönetmenize yardımcı olacak İş Ortağı Merkezi

Ortak satış yardım konularını henüz okumadısanız, aşağıdaki kaynaklar satış anlaşmalarını yönetmeye yardımcı İş Ortağı Merkezi.

|**Bunu yapmak için**   |**Bunu okuyun**   |
|-----------------------|:-----------------------|
|Ortak satış fırsatları sayfasındaki sekmeleri ve gezintiyi anlama|[Ortak satış bölümünde gezinme](./manage-co-sell-opportunities.md)|
|D&B listesinden bir müşteri kuruluşu seçme |[Müşterinizi seçin](./manage-co-sell-opportunities.md#select-your-customer)|
|Anlaşma ayrıntıları bölümündeki alanları değiştirme|[Anlaşma ayrıntıları](./manage-co-sell-opportunities.md#deal-details)|
|Anlaşma ekibine takım üyelerinizi ekleme|[Çalışanlarınızı ekleme](./manage-co-sell-opportunities.md#add-team-members)|
|Ortak satış anlaşmasına yanıt verme|[Ortak satış anlaşmalarını yönetme](./manage-co-sell-opportunities.md#respond-to-a-co-sell-opportunity)
|İş Ortağı Merkezi'de kazanarak kazanarak anlaşmaları İş Ortağı Merkezi |[Yeni bir anlaşma kaydetme](./register-deals.md)
|Referans içgörüleri alın ve referansların nasıl olduğunu öğrenin |[Referans içgörüleri](./referral-insights.md)
|İş profili oluşturma ve yönetme|[İş profilini yönetme](./create-a-marketing-profile.md)
|İş profiliniz için müşteri adaylarını yönetme |[Müşteri adaylarını yönetme](./manage-leads.md)|

## <a name="next-steps"></a>Sonraki adımlar


- [İş Ortağı Bağlan](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) İş Ortağı Merkezi çalışma kitabı - İş Ortağı Merkezi ve İş Ortağı Satışları karşılaştırması aracılığıyla iş ortaklarının satış işlemlerini ve rollerini yeni satış süreçleriyle hizalamak için Bağlan.
- [İş Ortağı Merkezi ortak satış çalışma kılavuzu](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) - müşteri adaylarını veya ortak satış fırsatlarını yönetmek ve anlaşmaları kaydetmek İş Ortağı Merkezi aracılığıyla bir operasyon modelini belirlemeye yönelik kılavuz.
- [Referans yönetimi destesi](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) - Müşteri adaylarını ve ortak satış fırsatlarını yönetmek için adım adım talimatlar görselleştirilmiş İş Ortağı Merkezi.
- [Ticari markette yayımlama](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) ve yönetme - ticari markette teklif oluşturma, yönetme ve yayımlamaya yönelik İş Ortağı Merkezi adım adım yönerge görselleştirildi.
