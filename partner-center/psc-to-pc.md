---
title: iş ortağı Sales Bağlan (PSC) geçirme
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: microsoft iş ortaklarının iş ortağı Bağlan satışlarından (PSC) iş ortağı merkezi 'ne nasıl geçirebileceğini ve microsoft satıcıları tarafından gönderilen anlaşmalar oluşturma veya yönetme hakkında bilgi edinin.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.date: 09/27/2021
ms.openlocfilehash: 7631c85d9bf8f9e63f377fd9bdd28f42162a9bfa
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129070346"
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

> [!IMPORTANT]
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

  > [!NOTE]
  > Iş Ortağı Merkezi oturumunuzu kapatıp başvuru sayfalarına erişim için kimlik bilgilerinizi yenilemek üzere yeniden oturum açmanız gerekebilir.

Iş Ortağı Merkezi menüsünde veya başvurularda ilişkili sayfalarda **Başvurular** seçeneğini görmüyorsanız, şirketinizin [hesap yöneticisine](permissions-overview.md) başvurarak, **Başvurular** seçeneğine ve ilgili alana erişim vermesini isteyin.

Şirketinizin hesap yöneticisini bulmak için:

1. [iş ortağı merkezi panosundan](https://partner.microsoft.com/dashboard)Ayarlar dişli simgesini ve ardından **hesap ayarlarını** seçin.

2. **Kullanıcı yönetimi**' ni seçin.

3. Kullanıcı listesinin en üstünde, **filtre** açılan menüsünü seçin. **Hesap Yöneticisi** seçeneğini değiştirin.

   Bu sayfada, tüm hesap yöneticileri ilgili e-posta adresleriyle görüntülenir. Bunlardan birine e-posta gönderin ve iş hesabınız için başvuru Yöneticisi rolünü atamasını isteyin.

  :::image type="content" source="images/pscmigration/account-admin.gif" alt-text="İş ortağı ayarları Kullanıcı Yönetimi sayfasında hesap yöneticileri 'ni gösteren resim.":::

> [!IMPORTANT]
> - Rolünüz yalnızca PSC 'deki kullanıcıları yönetmeyi içeriyorsa, şirketinizin hesap yöneticisinden Iş Ortağı Merkezi 'nde [Hesap Yöneticisi](permissions-overview.md#manage-mpn-membership-and-your-company) rolünü atamasını isteyin. 
> - Rolünüzde ortak satış fırsatlarını yönetme de varsa, [Başvurular yönetici](permissions-overview.md#manage-referrals) rolü atanmasını isteyin.
> - Aynı zamanda PSC yöneticileri arasında bir değişiklik yönetimi liderine aday bir fikir elde etmek iyi bir fikirdir. Bunun yapılması, tüm PSC yöneticilerinin Iş ortağı merkezi hesap yöneticilerine ayrı olarak ulaşmasını önler. Bunun yerine, değişiklik Yönetimi lideri daha sonra Iş ortağı merkezi hesap yöneticisi ile çalışan birincil kişidir.

## <a name="user-migration"></a>Kullanıcı geçişi

Iş Ortağı Merkezi 'nde hesabınızı ayarladıktan sonra, iş ortağı merkezi rollerini şirketinizin çalışanlarına otomatik olarak atamak için ortak satış fırsatları sayfasında Kullanıcı Geçiş Sihirbazı 'nı kullanın.

> [!NOTE]
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

- PSC kullanıcıları iş dışı bir hesap kullanıyor olabilir.

- PSC kullanıcısı, Iş Ortağı Merkezi 'nde kullandığınız bir etki alanından farklı bir hesap kullanıyor olabilir.

   1 ve 2 senaryolarıyla ilgili hataları gidermek için kullanıcıdan Azure AD kiracınıza bağlı iş hesabını kullanarak iş ortağı merkezi 'Nde oturum açmasını isteyin. [Genel yöneticiniz](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) yardımcı olabilir.
   
   Genel yöneticinize ulaşmak için: 
   - Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard) oturum açın ve sağ üst köşedeki dişli simgesinden **Hesap ayarları** ' nı seçin.
   - İkinci düzey, sol gezinti çubuğundan **Kullanıcı yönetimi** ' ni seçin.
   - Kullanıcı listesinin en üstünde, **filtre** açılan menüsünü seçin ve seçeneğini **genel yönetici** olarak değiştirin. Daha sonra sayfa, tüm genel yöneticileri ilgili e-posta adresleriyle birlikte görüntüler. İş hesabınız için bir başvuru Yöneticisi rolü atamasını isteyin.
   
      Genel yönetici, Azure AD kiracınızda yeni bir kullanıcı hesabı oluşturabilir ya da diğer etki alanı hesabı kullanıcılarına Konuk Kullanıcı erişimi atayabilir. Tüm PSC anlaşma yöneticileri ve kullanıcıları için hesaplar kurulduktan sonra, Iş Ortağı Merkezi 'nde oturum açması, sol gezinti menüsünden **başvuruları** seçmeniz ve başvurular sayfasını görebilecekleri onaylanır.

- Kullanıcının Iş Ortağı Merkezi 'ne atanmış bir başvuru rolü zaten var.
    - Kullanıcının var olan rolünü doğrulayabilirsiniz. iş ortağı merkezi 'nin sağ üst köşesinde **Ayarlar** (dişli simgesi) ve ardından **hesap ayarları**' nı seçin. İkinci bir sol gezinti menüsünü gördüğünüzde **Kullanıcı yönetimi** ' ni seçin ve Kullanıcı için arama yapın.

## <a name="psc-deals-migration"></a>PSC anlaşmalar geçişi

Kullanıcı geçişini tamamladıktan sonra, PSC 'den Iş Ortağı Merkezi 'ne uygun tüm açık anlaşmaları getirmek için ortak satış fırsatları sayfasında anlaşmalar Geçiş Sihirbazı 'nı kullanın. **Anlaşmalar geçiş bağlantısı yalnızca ortak merkezindeki tüm kuruluş kapsamına sahip olan, yalnızca görünür başvuru yöneticileri olacaktır.** Ortak satış fırsatları sayfasının sağ üst kısmında **"PSC anlaşmaları geçişi"** adlı bir bağlantı olacak ve bu bağlantı satış anlaşması geçiş sihirbazını açacaktır.

Anlaşma geçişini başlatmadan önce bu bölümü okuyun.

**Geçişe uygun**

Yalnızca bazı anlaşmalar PSC 'den Iş Ortağı Merkezi 'ne geçişe uygundur. Bu Geçiş Sihirbazı, iş ortaklarının, BT 'nin müşterileri ile çalışmaya devam ettikleri Iş Ortağı Merkezi 'ne anlaşmalar getirmelerini sağlamak için oluşturulmuştur. **Yalnızca geçerli iş ortağı hesabı ayrıntıları (geçerli MPN ID) ile 1 Ocak 2020 ' den oluşturulan ve açık durumda olan anlaşmalar geçiş için uygun değildir.**

**Geçiş için uygun değil**

- Çözüm değerlendirme anlaşmaları anlaşma geçişi için uygun değil
- OEM lisanslama iş anlaşmaları, anlaşma geçişi için uygun değil
- PSC'de kazanildi olarak işaretlenen anlaşmalar geçiş için uygun değildir. Kazandı olarak işaretlenen anlaşmalar için uygunsa anlaşma kaydı PSC'de tamamlanır.

## <a name="pre-requisites-for-deal-migration"></a>Anlaşma geçişi için önkullar

İş Ortağı Merkezi'dan anlaşma geçişini başlatmadan önce, başarılı bir geçiş için PSC'de anlaşmaları ayarlamak için aşağıdaki yönergeleri izleyin.

1. Şirketinizin açık anlaşmalar üzerinde çalışan tüm satış ekibi üyeleri bu geçiş hakkında bilgi sahibidir.
2. Satış ekibi üyeleri, anlaşma yönetimi için İş Ortağı Merkezi üzere eğitildi.
3. Anlaşmalar, aşağıda açıklandığı gibi tüm gerekli bilgileri içerir.
    - Ad ve adres de dahil olmak üzere müşteri şirketi ayrıntıları
    - Ortak satış anlaşması ise müşterinin iletişim ayrıntıları
    - En az bir çözüm
    - Ad, soyadı, e-posta kimliği ve telefon numarası gibi tüm ayrıntıları içeren en az bir ekip üyesi
    - Anlaşma değeri
    - Tahmini satış kapanış tarihi
    - İş ortağı notları

PsC'de toplu indirme ve karşıya yükleme özelliklerini kullanarak tüm uygun anlaşmaların anlaşmada eksik olan tüm ayrıntılarını indirebilirsiniz.

> [!NOTE]
> Yukarıdaki önkullar karşılanmazsa bile anlaşma geçişi başarılı olur. Ancak, yukarıdaki belirtilen gerekli alanlardan herhangi biri kullanılabilir durumda yoksa İş Ortağı Merkezi değiştiremezsiniz. Ardından, üzerinde çalışmaya başlamak için anlaşmalarda eksik olan tüm İş Ortağı Merkezi bilgileri girmeniz gerekir. **PsC'de uygun anlaşmaları, İş Ortağı Merkezi'a İş Ortağı Merkezi.**

Geçiş anlaşması İş Ortağı Merkezi tek tıklama deneyimi olarak yerleşiktir. Tek ihtiyacınız olan, şirket uygun anlaşmaları geçirmek için hazır olduğunda **"Anlaşmaları geçir"** düğmesini seçmektir. **PSC'den geçirmek istediğiniz anlaşmaları seçesiniz. Geçişe herhangi bir anlaşma İş Ortağı Merkezi, geçişe başlamadan önce bunları PSC'de kapalı durumuna taşımanız gerekir.**

> [!NOTE]
> Geçiş başlatıldıktan sonra, **anlaşmaların geçişi 24 saat kadar sürebilir.**

Geçiş tamamlandıktan sonra başlık iletisi, geçiş raporunun bağlantısıyla tamamlanacak şekilde değişir. PSC'den İş Ortağı Merkezi'a geçirilen anlaşmaların ayrıntılarını görüntülemek için raporu İş Ortağı Merkezi.

Rapor aşağıdaki ayrıntıları içerir.

- **İş Ortağı Merkezi kimliği** - Bir etkileşimde İş Ortağı Merkezi anlaşmaların benzersiz tanımlayıcısı. İki satış anlaşması vardır: biri iş ortağı, biri de Microsoft için ortak satış anlaşmasında İş Ortağı Merkezi.
- **İş Ortağı Merkezi kimliği** - İş ortağına ait İş Ortağı Merkezi için geçerli olan benzersiz tanımlayıcı.
- **Anlaşma adı** - PSC'de anlaşmaya verilen tanımlayıcı.
- **PSC anlaşma kimliği** - Anlaşma için PSC'deki benzersiz tanımlayıcı.
- **Hatalar** - belirli bir anlaşmadan başka bir anlaşmayı alırken herhangi bir hata olup olamay olduğunu belirtmek için.

Başarıyla geçirilen tüm anlaşmalar PSC'de görünmez. Geçiş yapılan anlaşmalar üzerinde çalışmaya devam İş Ortağı Merkezi anlaşma kaydını İş Ortağı Merkezi. Ortak satış anlaşmaları için Microsoft satıcılarının etkileşimleri üzerinde değişiklik olmayacaktır.

PSC'den geçirilen anlaşmalar, satış anlaşması kaynağına bağlı olarak Gelen ve Giden sekmelerinde kullanılabilir. Şirket tarafından paylaşılan tüm satış anlaşmaları Giden sekmesinde, Microsoft tarafından başlatılan satış anlaşmaları ise şirket içinde İş Ortağı Merkezi. Geçiş sonrası oluşturulacak iki tür anlaşma vardır.

- **Ortak satış anlaşmaları** - PSC'de ortak satış olarak işaretlenen satış anlaşmaları, psc'de ortak satış anlaşması olarak İş Ortağı Merkezi.
- **İş ortağı tarafından yapılan anlaşmalar** - Ortak satış olarak işaretlenen anlaşmalar, ortak satış anlaşması olarak İş Ortağı Merkezi. İş ortağı tarafından yönlendirilen satış anlaşmaları Microsoft satıcılarının kullanımına açıktır ve terminal durumuna ulaşmadan önce ortak satış anlaşmalarına yükseltilebilir (kazanıldı, kaybedildi). Ayrıca, anlaşmada teşvike uygun bir çözüm varsa, iş ortağı tarafından yönlendiren anlaşmalar anlaşma kaydı için uygun olur.

> [!IMPORTANT]
> Bazı anlaşmaların geçirilenemleri nedeniyle herhangi bir hata varsa, "Anlaşmaları geçir" düğmesine tıklayarak anlaşma **geçişini yeniden başlatabilirsiniz.** Yalnızca henüz geçirilemeyen bazı uygun anlaşmalar varsa etkinleştirilir. Bu, anlaşma geçişi başladıktan sonra PSC'de bazı yeni anlaşmaların oluşturulacak olduğu geçiş aşamasında da yararlı olacaktır.

Tüm anlaşmalar başarıyla geçirildiktan sonra , **"Anlaşmaları geçir"** düğmesinin devre dışı bırakıldığında "Geçirılacak anlaşma **yok"** ifadesini gösteren bir başlık **vardır.**

Kullanıcı geçişini ve/veya anlaşma geçişini tamamladıktan sonra, geçiş stratejisine karar vermek için aşağıdaki kılavuzu kullanın:

Şirketinizin bir İş Ortağı Geliştirme Yöneticisi (PDM) varsa - İş Ortağı Merkezi hesabınız ayar olduğunda ve kullanıcılarınız başka bir yere taşındığında ve rollere ve izinlere sahip olduğunda, Ortak Satış etkinliklerinizi İş Ortağı Merkezi. PdM'yi geçiş işleminin son tarihine kadar beklemek yerine geçişi yapmaları konusunda bilgilendirin. Bu, tüm yeni anlaşmaların geçişe İş Ortağı Merkezi.

> [!NOTE]
> Bu anahtarı kullandıktan sonra yalnızca PSC'de mevcut Etkin anlaşmalar üzerinde eyleme geçabileceksiniz. PSC'de Microsoft satıcılarından yeni anlaşmalar oluşturasınız veya satış anlaşması alamaysınız.

Şirkette PDM yoksa - Tüm kullanıcı hesaplarının ayarlandığından ve tüm kullanıcılar tarafından doğrulandığından emin olun. Bir e-posta ve PSC'de, satışa ilk olarak ortak satış yapmaya başlayacağınız tam tarihle ilgili bir başlık İş Ortağı Merkezi. PSC'de mevcut etkin anlaşmaları yönetmeye devam etmek zorunda olduğunu unutmayın.

> [!IMPORTANT]
> Kazanildi olarak işaretlenen anlaşmaları kaydetmek için 30 Nisan 2021'e kadar devam edilecektir.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>PSC yöneticileri, PSC anlaşma yöneticileri ve PSC satıcıları için sonraki adımlar

İş Ortağı Merkezi'da ortak satış yapmayı İş Ortağı Merkezi.
Bu önemli bir adımdır ve bu adım, satış ve satış için hazırlık İş Ortağı Merkezi. Hemen ortak satış yapmak için İş Ortağı Merkezi iş akışlarını ve değişiklikleri anlıyoruz. Bu belgeyi tamamen okuyarak başlayabilirsiniz. ortak satış deneyimi galerisinde de [iyi bir kaynak kümesi mevcuttur.](https://aka.ms/cosellexperience)

## <a name="major-differences-between-psc-and-partner-center-workflows"></a>PSC ile iş akışları arasındaki İş Ortağı Merkezi farklar

|**Senaryo**|**İş Ortağı Satış Bağlan**|**İş Ortağı Merkezi**|
|-----|:-----|:-----|
|Kullanıcı rolleri|PSC'de yönetici, satış anlaşması yöneticisi ve satıcı rolleri vardır.|İş Ortağı Merkezi yalnızca tüm [anlaşmalar](permissions-overview.md#manage-referrals) için okuma ve yazma izni veren referans yöneticisi rolüne sahip olur.|
|Ortak satış anlaşması için Microsoft'u davet etme|Microsoft satıcısı tarafından başlatılan bu işlem, iş ortağı tarafından açık bir şekilde sorulmaz.|Anlaşma için bir Microsoft [satıcısının yardımı gerekirse](manage-co-sell-opportunities.md#add-solutions) iş ortağının açık bir istekte yerması gerekir. Microsoft Seller'ın isteği reddetme seçeneği vardır.|
|Süre sonu|Anlaşma süresinin dolması kavramı yoktur.|İş ortağı tarafından kabul edilmediğinde iş ortağı gelen anlaşmaların süresi 14 gün içinde dolar. Aynı durum, Microsoft satıcısının 14 gün içinde eyleme geçene kadar süresi dolan iş ortağı giden satış anlaşmalarında da geçerli olur.|
|Microsoft satıcı ayrıntıları|Anlaşma oluşturulur oluşturulmaz görünür.|Microsoft Satıcı ayrıntıları yalnızca satıcı iş ortağından ortak satış davetini açıkça kabul ederse İş Ortağı ile paylaşılır.|
|[Özel işlem hattı](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Kullanılamıyor.|İş ortakları, Microsoft satıcılarına görünürlük vermeden işlem hatlarını paylaşabilir.|
|Çözümler|Bir satış anlaşmasına yalnızca bir fiyat listesine ait çözümler eklenebilir.|İş ortağı aşağıdaki [listelere](manage-co-sell-opportunities.md#add-solutions) ait çözümler ekleyebilir. a) Kendi çözümleri b) Microsoft birinci taraf kataloğundan çözümler (PSC'de İşlem Anlaşması rolüne benzer) ve c) Diğer üçüncü taraf iş ortaklarının ortak satış çözümleri (PSC'de ISV Anlaşması rolüne benzer).|
|Anlaşma ataması|Anlaşmaları yalnızca atanan satıcı görüntülemeli ve üzerinde eylemde davranabilir.|Anlaşma üzerinde çalışan insanları belirtmek için bir satış anlaşmasına ekip üyeleri eklenebilir; diğer referans yöneticilerinin bu anlaşmaları görüntülemesini veya bu anlaşmalara göre hareketlerini engellemesi engellenmez.|
|Müşteri kuruluşu|Serbest biçimli metin girişi.|Yalnızca birkaç karakter [yazarak](manage-co-sell-opportunities.md#select-your-customer) [müşteri kuruluşunda D&B](https://www.dnb.com/) veritabanında arama edebilirsiniz. Yasal ad ve adres, seçime göre otomatik olarak doldurulur.|
|Müşteri ilgili kişisi|Zorunlu değildir.|Özel işlem hattı paylaşımı için zorunlu değildir. Microsoft satıcısı ortak satış isteğine katılmak için davet edildiyse gereklidir.|
|Genel API|Kullanılamıyor.|[Referansları](/partner/develop/referrals) program aracılığıyla yönetmek için İş Ortağı Merkezi API.|

## <a name="map-the-fields-in-psc-to-the-corresponding-fields-in-partner-center"></a>PSC'de alanları, psc'de karşılık gelen İş Ortağı Merkezi

Bu bölüm, PSC için gösterilen seçili ekran görüntülerini ortak satış fırsatları bölümündeki ilgili görünümle İş Ortağı Merkezi karşılar.

Her ekran görüntüsü çifti üzerinde numaralı, sarı veya kırmızı daireler görebilirsiniz:

- **Sarı daireler ne anlama geliyor?** Numaralı, sarı daireler her PSC ekran görüntüsünde ilk olarak görünür. Daha sonra, altında aynı İş Ortağı Merkezi bir ekran görüntüsüyle birlikte bir yardımcı ekran görüntüsü bulabilirsiniz.

   PSC'de her bir alanın veya özniteliğin İş Ortağı Merkezi ilgili iki ekran görüntüsünde numaralı dairelerle nasıl eş olduğunu görebilirsiniz. Örneğin, birincide numaralı, sarı "1"i, PSC ekran görüntüsünü numaralı, ikincisinde sarı "1" ile, altta İş Ortağı Merkezi ekran görüntüsüyle eşleyebilirsiniz.

- **Kırmızı daire ne anlama geliyor?** Bir ekran görüntüsünde kırmızı bir daire görüyorsanız, PSC alanı bu ekran görüntüsünde İş Ortağı Merkezi.

PSC'den İş Ortağı Merkezi alan eşlemeleri aşağıdaki alanlar için gösterilir:

- Ortak satış fırsatları varsayılan görünümüne İş Ortağı Merkezi PSC giriş sayfası
- İş Ortağı Merkezi anlaşma görünümüyle eşlenen PSC kılavuz görünümü
- PsC anlaşma ayrıntıları görünümü, İş Ortağı Merkezi ayrıntıları görünümüyle eşlenmiş
- Çözüm ekle görünümüne eşlenen PSC İş Ortağı Merkezi Görünümü
- Kullanıcı yönetimi görünümüyle eşlenen PSC İş Ortağı Merkezi yönetimi görünümü
- PsC kullanıcı rolü atama görünümü, İş Ortağı Merkezi atama görünümüyle eşlenmiş
- Bildirim görünümüyle eşlenen PSC İş Ortağı Merkezi görünümü

### <a name="psc-home-page-mapped-to-the-partner-center-co-sell-opportunities-default-view"></a>Ortak satış fırsatları varsayılan görünümüne İş Ortağı Merkezi PSC giriş sayfası

Üst PSC ekran görüntüsü ile altındaki ekran görüntüsü arasındaki eşleşen, İş Ortağı Merkezi daireleri karşılaştırın. Eşleşen sayılar, PSC ile ilgili özelliği veya özniteliğini aşağıdaki İş Ortağı Merkezi. Kırmızı daireler, alanla eşleşen bir İş Ortağı Merkezi işaret ediyor.  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="İş Ortağı Satışları sayfasının giriş sayfası ile Bağlan ortak satış fırsatlarının varsayılan görünümü arasındaki alan eşlemelerini gösteren İş Ortağı Merkezi." lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="psc-grid-view-mapped-to-the-partner-center-deal-view"></a>İş Ortağı Merkezi anlaşma görünümüyle eşlenen PSC kılavuz görünümü

Üst PSC ekran görüntüsü ile altındaki ekran görüntüsü arasındaki eşleşen, İş Ortağı Merkezi daireleri karşılaştırın. Eşleşen sayılar, PSC ile ilgili özelliği veya özniteliğini aşağıdaki İş Ortağı Merkezi. Kırmızı daireler, alanla eşleşen bir İş Ortağı Merkezi işaret ediyor.  

> [!NOTE]
> Ekran görüntülerinin altında dikkat edilmesi gereken diğer noktalar da yer almaktadır.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="İş Ortağı Satışları (PSC) kılavuz görünümü ile Bağlan satış anlaşması görünümü arasındaki alan İş Ortağı Merkezi gösteren görüntü." lightbox="images/pscmigration/grid-view-expanded.png":::

#### <a name="special-considerations"></a>Dikkat edilmesi gereken özel noktalar

- PsC'ninki gibi İş Ortağı Merkezi liste görünümü yoktur.  Tüm anlaşmalar, müşteri bilgileri ve satış anlaşması türüyle birlikte en son alınan veya oluşturulma tarihine göre listelenir. Görünümde ilk anlaşma varsayılan olarak seçilidir. PSC tablo biçiminde görüntülenen değerlerin çoğu, satış anlaşması ayrıntı görünümünde İş Ortağı Merkezi.
- Anlaşma rolü, bir rol için gerekli İş Ortağı Merkezi. İş akışlarının hiçbirsinde görüntülenmez veya yakalanmaz. Satış anlaşmasına eklenen çözümlere göre Microsoft satıcı tarafında otomatik olarak türetilir.
- Son değiştirme tarihi, son değiştirme tarihi İş Ortağı Merkezi. İş ortakları, anlaşmaları son güncelleştirme tarihine göre sıralamak için sıralama işlevini kullanabilir.

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3 - PsC Anlaşma ayrıntıları görünümü, İş Ortağı Merkezi

Üst (PSC) ekran görüntüsünde eşleşen, numaralı daireleri, altındaki İş Ortağı Merkezi ekran görüntüsüyle karşılaştırın. Eşleşen sayılar, PSC ile ilgili özelliği veya özniteliğini aşağıdaki İş Ortağı Merkezi. Kırmızı daireler, verilerde eşleşen alan veya alan İş Ortağı Merkezi.

> [!NOTE]
> Ekran görüntülerinin altında dikkat edilmesi gereken diğer noktalar da yer almaktadır.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="İş Ortağı Satışları ve (PSC) satış Bağlan görünümü ile satış anlaşması ayrıntıları görünümü arasındaki alan İş Ortağı Merkezi gösteren görüntü." lightbox="images/pscmigration/deal-details-expanded.png":::

#### <a name="special-considerations"></a>Dikkat edilmesi gereken özel noktalar

- İş ortakları, iş ortağı anlaşması ayrıntı görünümünde düzenle düğmesini seçerek bir anlaşmayı düzenleyebilir (6). Düzenle düğmesi seçildikten sonra tüm alanlar düzenlenebilir hale gelecektir. Ardından anlaşmada yapılan düzenlemeleri kaydetme veya iptal etme seçeneğiniz vardır.
- Anlaşmayı aynı anlaşmada yinelenen olarak kapatma seçeneği İş Ortağı Merkezi.
- Müşteri Sonucu, İş Ortağı Merkezi. Müşteri etkileşimleri ile ilgili tüm ayrıntılar, İş Ortağı Merkezi.
- Tahmini çözüm kapatma tarihi yalnızca aynı anda yalnızca OEM IOT anlaşmaları İş Ortağı Merkezi. Bu bilgiler diğer hiçbir anlaşma türü için görüntülenmez.
- Lisanslama programı, lisanslama İş Ortağı Merkezi. Bu bilgiler, anlaşmada seçilen çözümlere göre otomatik olarak görüntülenir.

> [!NOTE]
> Kazanıldı veya kaybedildi olarak işaretlenen anlaşmalar daha sonra düzenlenemez. Anlaşmaları bu terminal durumları içine alırken dikkatli olun.

### <a name="psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>'Çözüm ekle' görünümüne eşlenen PSC 'İş Ortağı Merkezi' görünümü

Üst (PSC) ekran görüntüsünde eşleşen, numaralı daireleri, altındaki İş Ortağı Merkezi ekran görüntüsüyle karşılaştırın. Eşleşen sayılar, PSC ile ilgili özelliği veya özniteliğini aşağıdaki İş Ortağı Merkezi. Kırmızı daireler, verilerde eşleşen alan veya alan İş Ortağı Merkezi.
  
:::image type="content" source="images/pscmigration/products.png" alt-text="İş Ortağı Satışları (PSC) ürün Bağlan görünümü ile çözüm ekleme görünümü arasındaki alan İş Ortağı Merkezi gösteren görüntü." lightbox="images/pscmigration/products-expanded.png":::

### <a name="user-management-in-psc-versus-partner-center"></a>PSC'de kullanıcı yönetimi ile İş Ortağı Merkezi

Üst (PSC) ekran görüntüsünde eşleşen, numaralı daireleri, altındaki İş Ortağı Merkezi ekran görüntüsüyle karşılaştırın. Eşleşen sayılar, PSC ile ilgili özelliği veya özniteliğini aşağıdaki İş Ortağı Merkezi. Kırmızı daireler, verilerde eşleşen alan veya alan İş Ortağı Merkezi.  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="İş Ortağı Satışları (PSC) kullanıcı Bağlan giriş sayfası ile Hesap ayarları alanında İş Ortağı Merkezi Kullanıcı yönetimi sayfası görünümü arasındaki alan eşlemelerini gösteren görüntü."  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="user-role-assignment-in-psc-versus-partner-center"></a>PSC'de kullanıcı rolü ataması ile İş Ortağı Merkezi

Üst (PSC) ekran görüntüsünde eşleşen, numaralı daireleri, altındaki İş Ortağı Merkezi ekran görüntüsüyle karşılaştırın. Eşleşen sayılar, PSC ile ilgili özelliği veya özniteliğini aşağıdaki İş Ortağı Merkezi. Kırmızı daireler, verilerde eşleşen alan veya alan İş Ortağı Merkezi.  

:::image type="content" source="images/pscmigration/roles.png" alt-text="İş Ortağı Satışları (PSC) rol atama görünümü Bağlan rol atama görünümü arasındaki alan eşlemelerini İş Ortağı Merkezi görüntüsü." lightbox="images/pscmigration/roles-expanded.png":::

#### <a name="special-considerations"></a>Dikkat edilmesi gereken özel noktalar

- PSC yöneticisinin eşdeğer rolü, hesap yöneticisi rolü İş Ortağı Merkezi.
- Ortak satış anlaşması yönetimi için İş Ortağı Merkezi rol vardır. Bu rol, referans yöneticisi rolüdir.

### <a name="7---notifications-in-psc-versus-partner-center"></a>7 - PSC ile İş Ortağı Merkezi arasındaki bildirimler

Üst (PSC) ekran görüntüsünde eşleşen, numaralı daireleri, altındaki İş Ortağı Merkezi ekran görüntüsüyle karşılaştırın. Eşleşen sayılar, PSC ile ilgili özelliği veya özniteliğini aşağıdaki İş Ortağı Merkezi. Kırmızı daireler, verilerde eşleşen alan veya alan İş Ortağı Merkezi.  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="İş Ortağı Satışları ve (PSC) Bağlan eşlemesini ve İş Ortağı Merkezi gösteren görüntü."  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>PSC'den İş Ortağı Merkezi - Sık sorulan sorular

Aşağıdaki bölümlerde geçişle ilgili sık sorulan sorular yanıtlanmaktadır.

### <a name="what-should-i-do-if-i-dont-have-access-to-partner-center"></a>Erişim iznim yoksa ne İş Ortağı Merkezi?

Atanmış rolleri almak için "Erişim yok" sayfasında listelenen yöneticilerinize başvurabilirsiniz. Referanslar bölümünde [okuma ve](permissions-overview.md#manage-referrals) yazma izni için referans yöneticisi rolüne ihtiyacınız olacak. Yalnızca iş profillerini yönetiyorsanız, iş profili yöneticisi rolünüz İş Ortağı Merkezi.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="İş Ortağı Merkezi'da erişim yok deneyimini gösteren görüntü.":::

### <a name="who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>Who bölümündeki Referanslar bölümüne erişim izni İş Ortağı Merkezi?

Hesap [yöneticiniz Referanslar](permissions-overview.md#manage-mpn-membership-and-your-company) sekmesine erişmenizi sağlar. Hesap yöneticinizi bulmak için **panonun** sağ üst köşesindeki dişli simgesinden Hesap ayarları'İş Ortağı Merkezi [seçin.](https://partner.microsoft.com/dashboard) Ardından, ikinci **düzey,** sol gezinti çubuğundan Kullanıcı yönetimi'ni seçin. Kullanıcı listesinin üst kısmında Filtre  açılan menüsünü seçin ve seçeneğini hesap yöneticisi **olarak belirleyin.** Sayfada ilgili e-posta adresleriyle birlikte tüm hesap yöneticileri görüntülenir. İş hesabınız için referans yöneticisi rolünü atamasını istemek için bunlardan birini sorun.

### <a name="the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>+yeni anlaşma düğmesi, hesabımız için gri renkte gösterilir. Anlaşma oluşturmaya başlamak için ne yapabilirim?

Bu durum yalnızca mpN kuruluşuna bağlı ortak satışa hazır çözüm yoksa ve bu çözümde İş Ortağı Merkezi. Çözümlerinizin MPN kimliğinin düzeltilmesi için PDM'nize başvurun veya sorundan bahsederek bir destek bileti oluşturun: "PSC geçişi sonrasında yeni satış anlaşması düğmesi gri."

### <a name="can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>PSC gibi kuruluştan belirli bir kişiye satış anlaşması atay musunuz?

Takım üyelerini belirli bir satış anlaşmasına at attayarak. Diğer referans yöneticilerinin bu anlaşmaları görüntülemesini veya bu anlaşmalara göre hareket etmelerini engellemez.

### <a name="is-there-a-view-of-all-the-deals-assigned-to-me"></a>Bana atanan tüm anlaşmaların bir görünümü var mı?

Kullanıcı düzeyinde bir sekme olan sık kullanılanlar özelliğini kullanabilirsiniz. Anlaşmalara hızlı erişim elde etmek için size sık kullanılanlar olarak atanan tüm anlaşmaları işaretlebilirsiniz.

### <a name="is-there-a-read-only-view-for-the-deals"></a>Anlaşmalar için salt okunur bir görünüm var mı?

Hayır, referanslar bölümünde anlaşmaların salt okunur bir görünümü yoktur. Tüm referans yöneticileri tüm anlaşmalara tam okuma ve yazma erişimine sahip olur.

### <a name="how-can-i-register-a-deal-after-marking-it-as-won"></a>Anlaşmayı won olarak işaretledikten sonra nasıl kayıt olabilirim?

Anlaşma aşağıdaki ölçütleri karşılarsa, anlaşma kaydını başlatmak için bir açılır [pencere görüntülenir.](./register-deals.md)

- Anlaşmada teşvike uygun bir çözüm vardır.
- Microsoft satıcısı satış anlaşmasına katılmak için davet edildi veya sizi satış anlaşmasına davet etti.
- Microsoft kartı, İş Ortağı Merkezi'da Kabul Edildi veya Kazanıldı İş Ortağı Merkezi.

### <a name="i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>Anlaşma Kaydı bölümünde "+Yeni anlaşma kaydı" düğmesini seçerek hata iletisi alıyorum. Anlaşmalarımı nasıl kaydederim?

**+Yeni satış anlaşması** kaydı düğmesi yalnızca ISV bağlantı programına kayıtlı olan iş ortakları tarafından satış anlaşmasına karşılık gelen ortak satış fırsatı olmayan bir satış anlaşması kaydetmek için İş Ortağı Merkezi. Ortak satış fırsatıyla anlaşmaları kaydetmek için, anlaşma kazanildi olarak işaretlendiğinde ve anlaşma kaydı ölçütlerini karşılarsa bir açılır pencere görüntülenir.

### <a name="is-adding-a-customer-organization-mandatory"></a>Müşteri kuruluşu eklemek zorunlu mu?

Evet, müşteri [kuruluşuna ekleme](./manage-co-sell-opportunities.md#select-your-customer) zorunludur İş Ortağı Merkezi. İlk olarak müşterinin bulunduğu konumu arayarak başlayalım. Sahip olduğunuz ayrıntılara göre; Tam bina adı dahil olmak üzere belirli olabilir veya yalnızca şehir ayrıntılarını veabilirsiniz. Kuruluş araması, herhangi bir adres ayrıntısı girmek zorunda olmadığınız adla eşleşen tüm yasal varlıkları getirir. Tüm ayrıntılar seçilen kuruluşa göre otomatik olarak doldurulur.

### <a name="are-customer-contact-details-mandatory"></a>Müşteri iletişim bilgileri zorunlu mu?

Oluşturmakta [olduğunu anlaşma türüne](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) bağlıdır. Yalnızca işlem hattınızı paylaşıyorsanız ve Microsoft satış kuruluşundan herhangi bir yardıma gerek yoksa, müşteri iletişim bilgilerini vermeyebilirsiniz. Microsoft satıcısından etkin bir şekilde yardım almak için ortak satışlar yaptıysanız müşteri iletişim bilgilerini de sağlayabilirsiniz. Bir ortak satış isteği oluşturmadan önce müşteriden açık bir onay İş Ortağı Merkezi.

### <a name="how-many-solutions-can-i-add-to-a-deal"></a>Bir anlaşmaya kaç çözüm ekleyebilirim?

Bir satış anlaşmasına en fazla 50 çözüm (PSC'de 'ürünler' ile benzer) eklersiniz. PSC'den farklı olarak, ortak satışa uygun çözümleriniz, Microsoft birinci taraf SKÜ'ler ve diğer üçüncü taraf ortak satış uygun çözümlerinden çözümlerinizi karma olarak kullanabilirsiniz. Bu rolde seçilecek veya kullanılabilir bir satış İş Ortağı Merkezi. Microsoft SKU'ları için isteğe bağlı olarak satış anlaşmasına eklenen her SKU için miktar ve fiyat eklenmiştir.

### <a name="when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>Satış anlaşması oluşturduk sonra Microsoft satıcısının ayrıntılarını ne zaman bulasınız?

Microsoft satıcılarına yalnızca Microsoft tarafında ilgili satıcı kişisi ile satış anlaşması oluşturulurken belirtilen tam yardım gereksinimi eşledikten sonra atanır. Atamadan sonra bile Microsoft satıcıları ortak satış davetini kabul etme veya reddetme seçeneğine sahip olur. Yalnızca bir satıcı tarafından ortak satış daveti kabul edilirse, anlaşma Microsoft satıcı iletişim bilgileriyle güncelleştirilir. Microsoft satıcılarının satış anlaşmasına göre hareket etmek için SLA'sı 14 gündür. İş ortaklarının süresi dolmuş durumuna gelmeden önce anlaşma üzerinde hareket etmek zorunda olduğu SLA'dır.

### <a name="where-can-i-find-the-opportunity-id"></a>Fırsat kimliğini nerede bulamıyorum?

PSC'deki Fırsat Kimliği, İş Ortağı Merkezi. Herhangi bir anlaşmayı a açmak için anlaşma adının yanında anlaşma kimliğini bulabilirsiniz.

### <a name="how-can-my-pdm-get-access-to-partner-center"></a>PDM'm İş Ortağı Merkezi?

İş Ortağı Merkezi PSC'den farklı olarak PDM'ler tarafından erişilemez. Bu özelliği etkinleştirmek için aşağıda belirtilen birden çok seçenek vardır.

- OCP Analizler - PDM'ler yalnızca anlaşmaları ve onlarla ilgili ilerlemeleri görüntülüyorsa, kuruluş görünümünü elde etmek için Tek Ticari İş Ortağı (OCP) Analizler portalını kullanabilirler. Bu bir iç araçtır ve yalnızca PDM'ler için kullanılabilir. OCP içgörüleri, şirket kullanıcıları için kullanılamaz.
- İş Ortağı Merkezi konuk kullanıcı - PDM hesabını İş Ortağı Merkezi bir konuk kullanıcı olarak ekleyebilir ve referansları görüntüleysin ve bunlar üzerinde eyleme geçsin diye onlara referans yöneticisi @microsoft.com rolü atabilirsiniz.
- Kiracınız [içinde yeni](./create-user-accounts-and-set-permissions.md#add-a-new-user) kullanıcı oluşturma - Kendi kiracınız içinde yeni bir kullanıcı oluşturabilir ve bu ayrıntıları PDM ile paylaşarak, hesabın diğer referans kullanıcılarına benzer referansları görüntülemelerini ve bu kullanıcılara göre hareketlerini gerçekleştirebilirsiniz.

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>PSC'deki hesabınız geçerli bir MPN ile ilişkili değilse doğru MPN kimliğini bulma

PSC'de 'PSC geçersiz MPN ID ilişkilendirme sorunu' başlığıyla ilgili bir başlık gördükten dolayı buradaysanız, doğru yerdesiniz demektir. Hesabınız aşağıdaki nedenlerden dolayı geçersiz bir MPN kimliğine bağlanmış olabilir

- Şirketinizin bir İş Ortağı Merkezi yok.
- PDM'niz, PSC hesabınızla İş Ortağı Merkezi (MPN ID) arasında bağlantı olan dahili sistemlerde hesabınız MPN kimliğini girerken bir hata yaptı.
- Şirket, Partner Membership Center(PMC) İş Ortağı Merkezi.

İlk olarak aşağıdaki adımları takip edin ve doğru MPN kimliğini bulun.

1. İş Ortağı Merkezi oturum [açın.](https://partner.microsoft.com/dashboard)
2. MPN kimliğini bulmak [için hesap ayarları belgelerinde](./partner-center-account-setup.md#locate-your-mpn-id) verilen kılavuzu kullanın.

Aşağıda, mpN kimliğiniz için tam olarak hangi konumda İş Ortağı Merkezi ekran görüntüsü verilmiştir.

:::image type="content" source="images/pscmigration/finding-mpnid.png" alt-text="İş ortağının MPN kimliğini bularak hesap ayarlarını gösteren resim."  lightbox="images/pscmigration/finding-mpnid.png":::

- PDM'niz varsa, mpN kimliğinizin hesaptan doğru MPN kimliğiyle düzeltilmesini İş Ortağı Merkezi.
- PDM'niz yoksa, PSC başlığında gösterilen PSC hesap bilgilerini ve psc hesabınızdan doğru MPN kimliğini içeren PSC başlığında verilen adrese bir e-İş Ortağı Merkezi gönderin.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Satış anlaşmalarınızı oluşturmanıza ve yönetmenize yardımcı olacak İş Ortağı Merkezi

Ortak satış yardım konularını henüz okumadısanız, aşağıdaki kaynaklar satış anlaşmalarını yönetmeye İş Ortağı Merkezi.

|**Bunu yapmak için**   |**Bunu okuyun**   |
|-----------------------|:-----------------------|
|Ortak satış fırsatları sayfasındaki sekmeleri ve gezintiyi anlama|[Ortak satış bölümünde gezinme](./manage-co-sell-opportunities.md)|
|D&B listesinden bir müşteri kuruluşu seçme |[Müşterinizi seçin](./manage-co-sell-opportunities.md#select-your-customer)|
|Anlaşma ayrıntıları bölümündeki alanları değiştirme|[Anlaşma ayrıntıları](./manage-co-sell-opportunities.md#deal-details)|
|Anlaşma ekibine takım üyelerinizi ekleme|[Çalışanlarınızı ekleme](./manage-co-sell-opportunities.md#add-team-members)|
|Ortak satış anlaşmasına yanıt verme|[Ortak satış anlaşmalarını yönetme](./manage-co-sell-opportunities.md#respond-to-a-co-sell-opportunity)
|İş Ortağı Merkezi'de kazandnız anlaşmaları İş Ortağı Merkezi |[Yeni bir anlaşma kaydetme](./register-deals.md)
|Referans içgörüleri alın ve referansların nasıl olduğunu öğrenin |[Referans içgörüleri](./referral-insights.md)
|İş profili oluşturma ve yönetme|[İş profilini yönetme](./create-a-marketing-profile.md)
|İş profiliniz için müşteri adaylarını yönetme |[Müşteri adaylarını yönetme](./manage-leads.md)|

## <a name="next-steps"></a>Sonraki adımlar

- [İş ortağı Bağlan](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) çalışma İş Ortağı Merkezi çalışma kitabı aracılığıyla iş ortaklarının satış işlemlerini ve rollerini yeni satış süreçleriyle hizalamak için İş Ortağı Merkezi ve İş Ortağı Satışları Bağlan.
- [İş Ortağı Merkezi ortak satış](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) çalışma kılavuzu - müşteri adaylarını veya ortak satış fırsatlarını yönetmek ve anlaşmaları kaydetmek için İş Ortağı Merkezi aracılığıyla bir operasyon modelini belirlemeye yönelik kılavuz.
- [Referans yönetimi destesi](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) - Müşteri adaylarını ve ortak satış fırsatlarını yönetmeye ve müşteri adaylarına müşteri adayı İş Ortağı Merkezi.
- [Ticari markette yayımlama](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) ve yönetme: Ticari markette teklif oluşturma, yönetme ve yayımlamaya yönelik İş Ortağı Merkezi adım adım talimatlar.