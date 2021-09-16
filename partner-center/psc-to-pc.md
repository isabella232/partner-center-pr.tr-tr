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
ms.sourcegitcommit: 90c87bd5e63a8af932ece5696267ea715fea6a01
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/16/2021
ms.locfileid: "127900449"
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

En üstteki PSC ekran görüntüsü ile Iş Ortağı Merkezi ekran görüntüsü arasındaki eşleşen, numaralandırılmış daireleri karşılaştırın. Eşleşen sayılar, Iş Ortağı Merkezi 'nde PSC ile ilgili özelliği veya özniteliği nerede bulabileceğinizi gösterir. Kırmızı daireler eşleşen Iş Ortağı Merkezi alanını gösterir.  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="iş ortağı satış Bağlan giriş sayfası ve iş ortağı merkezi 'nde ortak satış fırsatlarını varsayılan görünümü arasındaki alan eşlemelerini gösteren resim." lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>2-Iş Ortağı Merkezi anlaşma görünümüyle eşleştirilmiş olan PSC ızgara görünümü

En üstteki PSC ekran görüntüsü ile Iş Ortağı Merkezi ekran görüntüsü arasındaki eşleşen, numaralandırılmış daireleri karşılaştırın. Eşleşen sayılar, Iş Ortağı Merkezi 'nde PSC ile ilgili özelliği veya özniteliği nerede bulabileceğinizi gösterir. Kırmızı daireler eşleşen Iş Ortağı Merkezi alanını gösterir.  

> [!NOTE]
> Ekran görüntülerinin altında diğer konular görüntülenir.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="iş ortağı Sales Bağlan (PSC) kılavuz görünümü ve iş ortağı merkezi anlaşma görünümü arasındaki alan eşlemelerini gösteren resim." lightbox="images/pscmigration/grid-view-expanded.png":::

**Özel hususlar:**

- Iş Ortağı Merkezi 'nde PSC gibi bir liste görünümü yoktur.  Tüm anlaşmalar, müşteri bilgilerini ve anlaşma türünü içeren en son alınan veya oluşturulan tarihe göre listelenir. Görünümdeki ilk işlem varsayılan olarak seçilidir. PSC tablosu biçiminde görüntülenen değerlerin çoğu, Iş Ortağı Merkezi 'nde anlaşma ayrıntı görünümünde kullanılabilir.
- Anlaşma rolü Iş Ortağı Merkezi 'nde gerekli bir alan değil. İş akışlarının hiçbirinde gösterilmez veya yakalanmaz. Microsoft satıcı tarafında, başa eklenen çözümlere göre otomatik olarak türetilir.
- Son değiştirilme tarihi, Iş Ortağı Merkezi 'nin başvuru ayrıntıları sayfasında gösterilmez. İş ortakları, son güncelleme tarihine göre anlaşmaları sıralamak için sıralama işlevini kullanabilir.

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3-PSC anlaşma Ayrıntıları görünümü Iş Ortağı Merkezi ile eşlendi

En üstteki (PSC) ekran görüntüsündeki eşleşen, numaralandırılmış daireler, ortak merkez ekran görüntüsü ile karşılaştırın. Eşleşen sayılar, Iş Ortağı Merkezi 'nde PSC ile ilgili özelliği veya özniteliği nerede bulabileceğinizi gösterir. Kırmızı daireler, Iş Ortağı Merkezi 'nde eşleşen alan veya alan olmadığını gösterir.

> [!NOTE]
> Ekran görüntülerinin altında diğer konular görüntülenir.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="iş ortağı Sales Bağlan (PSC) anlaşma ayrıntıları görünümü ve iş ortağı merkezi anlaşma ayrıntıları görünümü arasındaki alan eşlemelerini gösteren resim." lightbox="images/pscmigration/deal-details-expanded.png":::

**Özel hususlar:**

- İş ortakları, iş ortağı anlaşma ayrıntısı görünümündeki Düzenle düğmesini seçerek bir anlaşmayı düzenleyebilir (6). Düzenle düğmesi seçildikten sonra tüm alanlar düzenlenebilir hale gelir. Daha sonra, anlaşma için yapılan düzenlemeleri kaydetme veya iptal etme seçeneğiniz vardır.
- Iş Ortağı Merkezi 'nde Yineleneni kapatma seçeneği yoktur.
- Müşteri sonucu Iş Ortağı Merkezi 'nde kullanılamaz. Müşteri etkileşimlerine ilişkin tüm ayrıntılar, Iş Ortağı Merkezi ' nde Notlar bölümünde güncelleştirilebilen olabilir.
- Tahmini çözüm kapatma tarihi yalnızca Iş Ortağı Merkezi 'nde OEM ıOT anlaşmaları için kullanılabilir. Bu bilgiler diğer hiçbir anlaşma türü için görüntülenmez.
- Lisanslama programı Iş Ortağı Merkezi 'nde gerekli değildir. Bu bilgiler, işlem sırasında seçilen çözümlere göre otomatik olarak algılanır.

>[!Note]
>Kazanıldı veya kaybedildi olarak işaretlenen herhangi bir anlaşma daha sonra düzenlenemez. Bir anlaşmayı bu Terminal durumlarından birine taşırken dikkatli olun.

### <a name="4---psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>4-' çözüm ekleme ' görünümü Iş Ortağı Merkezi 'ne eşlenmiş ' ürün Ekle ' görünümü

En üstteki (PSC) ekran görüntüsündeki eşleşen, numaralandırılmış daireler, ortak merkez ekran görüntüsü ile karşılaştırın. Eşleşen sayılar, Iş Ortağı Merkezi 'nde PSC ile ilgili özelliği veya özniteliği nerede bulabileceğinizi gösterir. Kırmızı daireler, Iş Ortağı Merkezi 'nde eşleşen alan veya alan olmadığını gösterir.
  
:::image type="content" source="images/pscmigration/products.png" alt-text="ortak satış Bağlan (PSC) ürün ekleme görünümü ve iş ortağı merkezi çözüm ekleme görünümü arasındaki alan eşlemelerini gösteren resim." lightbox="images/pscmigration/products-expanded.png":::

### <a name="5---user-management-in-psc-versus-partner-center"></a>5-PSC ve Iş Ortağı Merkezi 'nde Kullanıcı Yönetimi

En üstteki (PSC) ekran görüntüsündeki eşleşen, numaralandırılmış daireler, ortak merkez ekran görüntüsü ile karşılaştırın. Eşleşen sayılar, Iş Ortağı Merkezi 'nde PSC ile ilgili özelliği veya özniteliği nerede bulabileceğinizi gösterir. Kırmızı daireler, Iş Ortağı Merkezi 'nde eşleşen alan veya alan olmadığını gösterir.  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="iş ortağı Sales Bağlan (PSC) kullanıcı yönetimi ana ve hesap ayarları alanındaki iş ortağı merkezi kullanıcı yönetimi sayfa görünümü arasındaki alan eşlemelerini gösteren resim."  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="6---user-role-assignment-in-psc-versus-partner-center"></a>6-PSC ve Iş Ortağı Merkezi 'nde Kullanıcı rolü ataması

En üstteki (PSC) ekran görüntüsündeki eşleşen, numaralandırılmış daireler, ortak merkez ekran görüntüsü ile karşılaştırın. Eşleşen sayılar, Iş Ortağı Merkezi 'nde PSC ile ilgili özelliği veya özniteliği nerede bulabileceğinizi gösterir. Kırmızı daireler, Iş Ortağı Merkezi 'nde eşleşen alan veya alan olmadığını gösterir.  

:::image type="content" source="images/pscmigration/roles.png" alt-text="iş ortağı Sales Bağlan (PSC) rol atama görünümü ve iş ortağı merkezi rolü atama görünümü arasındaki alan eşlemelerini gösteren resim." lightbox="images/pscmigration/roles-expanded.png":::

**Özel hususlar:**

- PSC Yöneticisi için eşdeğer rol, Iş Ortağı Merkezi ' nde Hesap Yöneticisi rolüdür.
- Ortak satış anlaşma yönetimi için Iş Ortağı Merkezi 'nde yalnızca bir rol vardır. Bu rol, başvuru Yöneticisi rolüdür.

### <a name="7---notifications-in-psc-versus-partner-center"></a>7-PSC ve Iş Ortağı Merkezi 'nde bildirimler

En üstteki (PSC) ekran görüntüsündeki eşleşen, numaralandırılmış daireler, ortak merkez ekran görüntüsü ile karşılaştırın. Eşleşen sayılar, Iş Ortağı Merkezi 'nde PSC ile ilgili özelliği veya özniteliği nerede bulabileceğinizi gösterir. Kırmızı daireler, Iş Ortağı Merkezi 'nde eşleşen alan veya alan olmadığını gösterir.  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="ortak satış Bağlan (PSC) bildirimleri ve iş ortağı merkezi bildirimleri görünümü arasındaki eşlemeyi gösteren resim."  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>PSC 'den Iş Ortağı Merkezi 'ne geçme-sık sorulan sorular

Aşağıdaki bölümlerde geçişle ilgili sık sorulan sorular yanıtlanacaktır.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1-Iş Ortağı Merkezi 'ne erişimi yoksa ne yapmam gerekir?

Atanan rolleri almak için, "erişim yok" sayfasında listelenen yöneticilerinize başvurabilirsiniz. Başvurular bölümünde okuma ve yazma izni için [başvuru Yöneticisi](permissions-overview.md#manage-referrals) rolüne ihtiyacınız olacak. Yalnızca iş profillerini yönetiyorsanız iş profili yönetici rolüne iş ortağı Merkezi ' nde ihtiyacınız olacaktır.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Iş Ortağı Merkezi 'nde erişim deneyimi olmadığını gösteren resim.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2-Who iş ortağı merkezi 'ndeki referanslar bölümüne erişim izni verebilir mi?

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

Oluşturmakta olduğunuz [işlem türüne](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) bağlıdır. Yalnızca işlem hattınızı paylaşıyorsanız ve Microsoft satış kuruluştan herhangi bir yardım gerektirmiyorsa, müşteri iletişim ayrıntılarını vermemesini seçebilirsiniz. Microsoft satıcı 'dan etkin bir şekilde yardım Aradığınız yerde ortak satıyor olmanız durumunda müşteri iletişim ayrıntılarını sağlamanız gerekir. Iş Ortağı Merkezi 'nde ortak satış isteği oluşturmadan önce müşteriden açık onay almalısınız.

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11-bir dağıtmaya kaç çözüm ekleyebilirim?

En fazla 50 çözüm ekleyebilirsiniz (PSC 'de ' Ürünler ' öğesine benzer), bir anlaşma. PSC 'nin aksine, kendi ortak satış uygun çözümlerinizde, Microsoft ilk taraf SKU 'Lardan ve diğer üçüncü taraf ortak satış özellikli çözümlerle çözümler karıştırabilirsiniz. Iş Ortağı Merkezi 'nde seçilecek veya kullanılabilecek bir anlaşma rolü yok. Microsoft SKU 'Ları için, isteğe bağlı olarak, başa eklenen her SKU için miktar ve fiyat ekleyebilirsiniz.

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12-bir anlaşma oluşturduktan sonra Microsoft satıcı ayrıntılarını öğrenmem gerekir mi?

Microsoft satıcıları, Microsoft tarafındaki ilgili satıcı ile ilgilenirken belirtilen tam yardım gereksinimini eşleştirdikten sonra atanır. Atamadan sonra bile Microsoft satıcıları, ortak satış davetini kabul etme veya reddetme seçeneğine sahip olacaktır. Yalnızca bir satıcı tarafından bir ortak satış daveti kabul edilirse, bu anlaşma Microsoft satıcı iletişim ayrıntıları ile güncelleştirilir. Microsoft satıcıları için SLA, anlaşma üzerinde işlem yapması için 14 gündür. Bu, iş ortaklarının, zaman aşımına uğramadan önce anlaşma üzerinde işlem yapması gereken SLA 'dır.

### <a name="13---where-can-i-find-the-opportunity-id"></a>13-fırsat KIMLIĞINI nerede bulabilirim?

PSC 'deki fırsat KIMLIĞI, Iş ortağı merkezindeki anlaşma KIMLIĞIYLE aynıdır. Herhangi bir anlaşmayı açtığınızda anlaşma adının yanında anlaşma KIMLIĞINI bulabilirsiniz.

### <a name="14---how-can-my-pdm-get-access-to-partner-center"></a>14-PDM nasıl Iş Ortağı Merkezi 'ne erişebilirim?

İş Ortağı Merkezi 'Ne doğrudan PSC 'nin aksine, PDMs 'niz tarafından erişilemez. Bu özelliği etkinleştirmek için aşağıda bahsedilen birden çok seçenek vardır.

- OCP Analizler-pdms yalnızca bunlarla ilgili anlaşmaları ve ilerlemeyi görüntülüyorsanız, kuruluşunuzun görünümünü almak için tek bir ticari iş ortağı (OCP) Analizler portalını kullanabilirler. Bu bir iç araçtır ve yalnızca PDMs için kullanılabilir. OCP Insights, şirketinizin kullanıcıları için kullanılamaz.
- Iş Ortağı Merkezi 'nde Konuk Kullanıcı-PDM @microsoft.com Hesabınızı, Iş Ortağı Merkezi 'nde Konuk Kullanıcı olarak ekleyebilir ve başvuruları görüntüleyebilmek ve bunlarla işlem yapabilmesi için başvuru Yöneticisi rolü atayabilirsiniz.
- Kiracınızda [Yeni bir Kullanıcı](./create-user-accounts-and-set-permissions.md#add-a-new-user) oluşturma-kendi kiracınızda yeni bir kullanıcı oluşturabilir ve bu ayrıntıları PDM ile paylaşabilir ve bu sayede hesabınızdaki diğer başvuru kullanıcılarına benzer başvuruları görüntüleyebilir ve bunlarla işlem yapabilir.

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>PSC 'deki hesabınız geçerli bir MPN ile ilişkili değilse, doğru MPN KIMLIĞINI bulma

Burada, PSC 'nin ' PSC geçersiz MPN KIMLIĞI ilişkilendirme sorunu ' içinde bir başlık gördüğünüz için doğru yerde olursunuz. Aşağıdaki nedenlerden dolayı hesabınız geçersiz bir MPN KIMLIĞINE bağlanmış olabilir

- Şirketinizde bir Iş Ortağı Merkezi hesabı yok.
- PDM 'niz, PSC hesabınızı Iş Ortağı Merkezi hesabınıza (MPN KIMLIĞI) bağlayan iç sistemlere hesabınızın MPN KIMLIĞINI girerken bir hata yaptı.
- Şirketiniz Iş ortağı üyeliği merkezinden (PMC) Iş Ortağı Merkezi 'ne geçişi tamamlamadı.

İlk olarak, aşağıdaki adımları izleyerek doğru MPN KIMLIĞINI bulun.

1. [Iş Ortağı Merkezi hesabınızda](https://partner.microsoft.com/dashboard)oturum açın.
2. MPN KIMLIĞINI bulmak için [Hesap ayarları belgelerinde](./partner-center-account-setup.md#locate-your-mpn-id) verilen kılavuzu kullanın.

Aşağıda, Iş Ortağı Merkezi MPN KIMLIĞINIZI bulabileceğiniz tam konumu gösteren ekran görüntüsü verilmiştir.

:::image type="content" source="images/pscmigration/finding-mpn-id.png" alt-text="İş ortağının MPN KIMLIĞINI bulabileceği hesap ayarlarını gösteren resim."  lightbox="images/pscmigration/finding-mpn-id.png":::

- Bir PDM varsa, Iş Ortağı Merkezi hesabınızdaki doğru MPN KIMLIĞIYLE MPN KIMLIĞINIZI düzeltmesini isteyin.
- Bir PDM yoksa, PSC ana başlığında verilen adrese, hem PSC başlığında hem de Iş Ortağı Merkezi hesabınızdaki doğru MPN KIMLIĞINE sahip bir e-posta gönderin.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Iş Ortağı Merkezi 'nde anlaşmalar oluşturmanıza ve yönetmenize yardımcı olacak kaynaklar

Ortak satış yardım konularını henüz okumadıysanız, aşağıdaki kaynaklar Iş ortağı merkezindeki anlaşmaları yönetmenize yardımcı olur.

|**Bunu yapmak için**   |**Bunu okuyun**   |
|-----------------------|:-----------------------|
|Ortak satış fırsatları sayfasında sekmeleri ve gezintiyi anlama|[Ortak satış bölümünde gezinme](./manage-co-sell-opportunities.md)|
|D&B listesinden bir müşteri organizasyonu seçme |[Müşteriyi seçin](./manage-co-sell-opportunities.md#select-your-customer)|
|Anlaşma ayrıntıları bölümündeki alanları değiştirme|[Anlaşma ayrıntıları](./manage-co-sell-opportunities.md#deal-details)|
|Ekip üyelerinizi bir anlaşma ekibine ekleme|[Çalışanlarınızı ekleyin](./manage-co-sell-opportunities.md#add-team-members)|
|Ortak satış bir anlaşmayı yanıtlama|[Ortak satış anlaşmalar yönetme](./manage-co-sell-opportunities.md#respond-to-a-co-sell-opportunity)
|Iş Ortağı Merkezi 'nde kazandığı anlaşmaları kaydetme |[Yeni bir anlaşma Kaydet](./register-deals.md)
|Başvuru öngörülerini edinin ve başvurularınızın nasıl çalıştığını öğrenin |[Referans içgörüleri](./referral-insights.md)
|İş profili oluşturma ve yönetme|[İş profilini yönetme](./create-a-marketing-profile.md)
|İş profiliniz için müşteri adaylarını yönetme |[Müşteri adaylarını yönetme](./manage-leads.md)|

## <a name="next-steps"></a>Sonraki adımlar


- iş ortağı satışları iş ortağı [merkezi çalışma kitabına](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) , iş ortaklarının satış süreçlerini ve rollerini iş ortağı merkezi ile iş ortağı satış Bağlan ile yeni satış süreçleriyle hizalamak için çalışma kitabı. Bağlan
- [Iş Ortağı Merkezi ortak satış çalışma kılavuzu](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) -müşteri adaylarını yönetmek Için Iş Ortağı Merkezi aracılığıyla bir işletim modelini belirlemek için bir iş modeli veya ortak satış fırsatları ve anlaşmaları kaydetme.
- [Başvuru yönetimi destesi](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) -müşteri adaylarını yönetmek için görselleştirilen adım adım yönergeler ve Iş Ortağı Merkezi aracılığıyla ortak satış fırsatları.
- [Ticari Market 'Te yayımlama ve yönetme](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) -ticari Market 'Teki Iş Ortağı Merkezi aracılığıyla teklifler oluşturmak, yönetmek ve yayımlamak için görselleştirilen adım adım yönergeler.
