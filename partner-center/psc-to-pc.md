---
title: iş ortağı Sales Bağlan (PSC) geçirme
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: microsoft iş ortaklarının iş ortağı Bağlan satışlarından (PSC) iş ortağı merkezi 'ne nasıl geçirebileceğini ve microsoft satıcıları tarafından gönderilen anlaşmalar oluşturma veya yönetme hakkında bilgi edinin.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 12/07/2020
ms.openlocfilehash: 754a41716575dbc03dc0a6c384753ad35c4d187ae302b7bcd2feefa5d5bb133e
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115684471"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>iş ortağı satışları Bağlan (PSC) ile geçiş için iş ortağı merkezi 'nde (PC) ortak satış ile ilgili kılavuz

**Uygun roller**: Hesap Yöneticisi | Başvuru Yöneticisi | iş ortağı satışları Bağlan (PSC) satıcı | iş ortağı satışları Bağlan (PSC) yöneticisi | iş ortağı Sales Bağlan (PSC) anlaşma yöneticisi

bu makalede ortak satış Bağlan (PSC) ile iş ortağı merkezi 'ne (PC) geçiş yapan iş ortakları, iş ortağı merkezi 'nde ortak satış anlaşmaları oluşturmaya ve yönetmeye devam edebilmeleri için kılavuzluk sağlar.

>[!Note]
> Buradan geçiş hakkında PSC 'de bir başlık gördüğünüz için doğru yerde olursunuz. Bu kılavuz, PSC 'de anlaşmalar yöneten çözüm değerlendirmesi (SA) ve OEM lisanslama iş ortakları için geçerli değildir.

>[!Important]
> 1 Nisan 2021 ' den itibaren şirketiniz, PSC 'de anlaşmalar oluşturamaz veya düzenleyemez. **Aynı zamanda PSC içindeki toplu dışa aktarma özelliğini kullanarak mevcut anlaşmalar verilerini indirebilirsiniz. Ayrıca, bu tarihten sonra PSC 'den Iş Ortağı Merkezi 'ne [Açık anlaşmalar geçirebilirsiniz](psc-to-pc.md#psc-deals-migration) .** <br><br> Üzerinde etkin olarak çalıştığınız ve IP ortak satışı ile uygun çözümleri içeren anlaşmalar varsa, iki seçeneğiniz vardır: <br><br> 1. "31 Mart 2021 ' dan önce, anlaşmayı Kazanıldı olarak işaretleyin ve <br> 2. [anlaşmaları](psc-to-pc.md#psc-deals-migration) Iş Ortağı Merkezi 'ne geçirin ve böylece anlaşma üzerinde çalışmaya ve anlaşma kaydı başlatmaya daha fazla zaman alırsınız.

Bildiğiniz gibi, **Şirket, 30 nisan 2021 ' den sonra PSC 'ye erişimi kaybedecektir**. Bununla birlikte, Iş Ortağı Merkezi 'nde yapmak istediğiniz her şeyi, ortak satış anlaşmaları oluşturma, anlaşmaları yönetme ve Microsoft satıcıları tarafından size gönderilen anlaşmalar üzerinde işlem yapacak şekilde bulacaksınız.

Ancak farklılıklar olacaktır. Aşağıdaki kılavuz, Iş Ortağı Merkezi 'ne geçişinizi daha sorunsuz ve daha basit hale getirmenize yardımcı olabilir.

## <a name="before-you-move-things-you-need-to-know"></a>Taşımadan önce bilmeniz gereken şeyler

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
- BILGISAYAR Kullanıcı rolü-çalışanlar, PSC Kullanıcı rollerine göre rollere atanır. PSC 'deki yöneticiye, Iş Ortağı Merkezi 'nde referanslar yönetici rolleri atanır. Satıcı, Iş Ortağı Merkezi 'nde başvuru Kullanıcı rolüne atanır. Iş Ortağı Merkezi rolleri ve bu rollerin bulunduğu kullanıcıların Iş [Ortağı Merkezi 'nde](permissions-overview.md#manage-referrals) neler yapabileceğini öğrenin
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

Yalnızca bazı anlaşmalar PSC 'den Iş Ortağı Merkezi 'ne geçişe uygundur. Bu Geçiş Sihirbazı, iş ortaklarının, BT 'nin müşterileri ile çalışmaya devam ettikleri Iş Ortağı Merkezi 'ne anlaşmalar getirmelerini sağlamak için oluşturulmuştur. **Yalnızca geçerli iş ortağı hesabı ayrıntılarıyla (geçerli MPN KIMLIĞI) 1 Ocak 2020'den itibaren oluşturulan ve anlaşma kaydından geçen açık durumdaki anlaşmalar geçiş için uygundur.**

**Geçiş için uygun değil**

- Çözüm değerlendirme anlaşmaları anlaşma geçişi için uygun değil
- OEM lisanslama iş anlaşmaları, anlaşma geçişi için uygun değil
- PSC'de kazanildi olarak işaretlenen anlaşmalar geçiş için uygun değildir. Kazandı olarak işaretlenen anlaşmalar için uygunsa anlaşma kaydı PSC'de tamamlanır.

## <a name="pre-requisites-for-deal-migration"></a>Anlaşma geçişi için önkullar

İş Ortağı Merkezi'den anlaşma geçişini başlatmadan önce, başarılı bir geçiş için PSC'de anlaşmaları ayarlamak için aşağıdaki yönergeleri izleyin.

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

>[!Note]
> Yukarıdaki önkullar karşılanmazsa bile anlaşma geçişi başarılı olur. Ancak, yukarıdaki belirtilen gerekli alanlardan herhangi biri kullanılabilir durumda değilse İş Ortağı Merkezi durumunu değiştiremezsiniz. Ardından, üzerinde çalışmaya başlamak için anlaşmalarda eksik olan tüm İş Ortağı Merkezi bilgileri girmeniz gerekir. **PsC'de uygun anlaşmaları, İş Ortağı Merkezi'a İş Ortağı Merkezi.**

Geçiş anlaşması İş Ortağı Merkezi tek tıklama deneyimi olarak yerleşiktir. Tek ihtiyacınız olan, şirket uygun anlaşmaları geçirmek için hazır olduğunda **"Anlaşmaları geçir"** düğmesini seçmektir. **PSC'den geçirmek istediğiniz anlaşmaları seçesiniz. Herhangi bir anlaşmayı İş Ortağı Merkezi psC'de kapalı durumuna geçirmeniz gerekir.**

>[!Note]
> Geçiş başlatıldıktan sonra, **anlaşmaların geçişi 24 saat kadar sürebilir.**

Geçiş tamamlandıktan sonra başlık iletisi, geçiş raporunun bağlantısıyla tamamlanacak şekilde değişir. PSC'den İş Ortağı Merkezi'a geçirilen anlaşmaların ayrıntılarını görüntülemek için raporu İş Ortağı Merkezi.

Rapor aşağıdaki ayrıntıları içerir.

1. **İş Ortağı Merkezi kimliği** - Bir etkileşimde İş Ortağı Merkezi anlaşmaların benzersiz tanımlayıcısı. İki satış anlaşması vardır: biri iş ortağı, biri de Microsoft için ortak satış anlaşmasında İş Ortağı Merkezi.
2. **İş Ortağı Merkezi referans kimliği** - İş ortağına ait İş Ortağı Merkezi için geçerli olan benzersiz tanımlayıcı.
3. **Anlaşma adı** - PSC'de anlaşmaya verilen tanımlayıcı.
4. **PSC anlaşma kimliği** - Anlaşma için PSC'deki benzersiz tanımlayıcı.
5. **Hatalar** - belirli bir anlaşmadan başka bir anlaşmayı alırken herhangi bir hata olup olamay olduğunu belirtmek için.

Başarıyla geçirilen tüm anlaşmalar PSC'de görünmez. Geçiş yapılan anlaşmalar üzerinde çalışmaya devam İş Ortağı Merkezi anlaşma kaydını İş Ortağı Merkezi. Ortak satış anlaşmaları için Microsoft satıcılarının etkileşimleri üzerinde değişiklik olmayacaktır.

PSC'den geçirilen anlaşmalar, satış anlaşması kaynağına bağlı olarak Gelen ve Giden sekmelerinde kullanılabilir. Şirket tarafından paylaşılan tüm satış anlaşmaları Giden sekmesinde, Microsoft tarafından başlatılan satış anlaşmaları ise şirket içinde İş Ortağı Merkezi. Geçiş sonrası oluşturulacak iki tür anlaşma vardır.

1. **Ortak satış anlaşmaları** - PSC'de ortak satış olarak işaretlenen satış anlaşmaları, psc'de ortak satış anlaşması olarak İş Ortağı Merkezi.
2. **İş ortağı tarafından yapılan anlaşmalar** - Ortak satış olarak işaretlenen anlaşmalar, ortak satış anlaşması olarak İş Ortağı Merkezi. İş ortağı tarafından yönlendirilen satış anlaşmaları Microsoft satıcılarının kullanımına açıktır ve terminal durumuna ulaşmadan önce ortak satış anlaşmalarına yükseltilebilir (kazanıldı, kaybedildi). Ayrıca, anlaşmada teşvike uygun bir çözüm varsa, iş ortağı tarafından yönlendiren anlaşmalar anlaşma kaydı için uygun olur.

>[!Important]
> Bazı anlaşmaların geçirilenemleri nedeniyle herhangi bir hata varsa, "Anlaşmaları geçir" düğmesine tıklayarak anlaşma **geçişini yeniden başlatabilirsiniz.** Yalnızca henüz geçirilemeyen bazı uygun anlaşmalar varsa etkinleştirilir. Bu, anlaşma geçişi başladıktan sonra PSC'de bazı yeni anlaşmaların oluşturulacak olduğu geçiş aşamasında da yararlı olacaktır.

Tüm anlaşmalar başarıyla geçirildiktan sonra , **"Anlaşmaları geçir"** düğmesinin devre dışı bırakıldığında "Geçirilir anlaşma **yok"** ifadesini gösteren bir başlık **vardır.**

Kullanıcı geçişini ve/veya anlaşma geçişini tamamladıktan sonra, geçiş stratejisine karar vermek için aşağıdaki kılavuzu kullanın:

Şirketinizin bir İş Ortağı Geliştirme Yöneticisi (PDM) varsa - İş Ortağı Merkezi hesabınız ayar olduğunda ve kullanıcılarınız başka bir yere taşındığında ve rollere ve izinlere sahip olduğunda, Ortak Satış etkinliklerinizi İş Ortağı Merkezi. PdM'yi geçiş işleminin son tarihine kadar beklemek yerine geçişi yapmaları konusunda bilgilendirin. Bu, tüm yeni anlaşmaların geçişe İş Ortağı Merkezi.

>[!Note]
>Bu anahtarı kullandıktan sonra yalnızca PSC'de mevcut Etkin anlaşmalar üzerinde eyleme geçabileceksiniz. PSC'de Microsoft satıcılarından yeni anlaşmalar oluşturasınız veya satış anlaşması alamaysınız.

Şirkette PDM yoksa - Tüm kullanıcı hesaplarının ayarlandığından ve tüm kullanıcılar tarafından doğrulandığından emin olun. Bir e-posta ve PSC'de, satışa ilk başlanmaz tarihle ilgili bir başlık ve e-posta İş Ortağı Merkezi. PSC'de mevcut etkin anlaşmaları yönetmeye devam etmek zorunda olduğunu unutmayın.

>[!Important]
> Kazanildi olarak işaretlenen anlaşmaları kaydetmek için 30 Nisan 2021'e kadar devam edilecektir.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>PSC yöneticileri, PSC anlaşma yöneticileri ve PSC satıcıları için sonraki adımlar

İş Ortağı Merkezi'da ortak satış yapmayı İş Ortağı Merkezi.
Bu önemli bir adımdır ve bu adım, satış ve satış için hazırlık İş Ortağı Merkezi. Hemen ortak satış yapmak için İş Ortağı Merkezi iş akışlarını ve değişiklikleri anlıyoruz. Bu belgeyi tamamen okuyarak başlayabilirsiniz. ortak satış deneyimi galerisinde de [iyi bir kaynak kümesi mevcuttur.](https://aka.ms/cosellexperience)

## <a name="major-differences-between-psc-and-partner-center-workflows"></a>PSC ile iş akışları arasındaki İş Ortağı Merkezi farklar

|**Senaryo**|**İş Ortağı Satış Bağlan**|**İş Ortağı Merkezi**|
|-----|:-----|:-----|
|Kullanıcı rolleri|PSC'de yönetici, satış anlaşması yöneticisi ve satıcı rolleri vardır.|İş Ortağı Merkezi yalnızca tüm [anlaşmalar](permissions-overview.md#manage-referrals) için okuma ve yazma izni veren referans yöneticisi rolüne sahip olur.|
|Ortak satış anlaşması için Microsoft'u davet etme|Microsoft satıcısı tarafından başlatılan bu işlem, iş ortağı tarafından açık bir şekilde sorulmamasıdır.|Anlaşma için bir Microsoft [satıcısının yardımı gerekirse](manage-co-sell-opportunities.md#add-solutions) iş ortağının açık bir istekte yerması gerekir. Microsoft Seller'ın isteği reddetme seçeneği vardır.|
|Süre sonu|Anlaşma süresinin dolması kavramı yoktur.|İş ortağı tarafından kabul edilmediğinde iş ortağı gelen anlaşmaların süresi 14 gün içinde dolar. Aynı durum, Microsoft satıcısının 14 gün içinde eyleme geçene kadar süresi dolan iş ortağı giden satış anlaşmalarında da geçerli olur.|
|Microsoft satıcı ayrıntıları|Anlaşma oluşturulur oluşturulmaz görünür.|Microsoft Satıcı ayrıntıları yalnızca satıcı iş ortağından ortak satış davetini açıkça kabul ederse İş Ortağı ile paylaşılır.|
|[Özel işlem hattı](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Kullanılamıyor.|İş ortakları, Microsoft satıcılarına görünürlük vermeden işlem hatlarını paylaşabilir.|
|Çözümler|Bir satış anlaşmasına yalnızca bir fiyat listesine ait çözümler eklenebilir.|İş ortağı aşağıdaki [listelere](manage-co-sell-opportunities.md#add-solutions) ait çözümler ekleyebilir. a) Kendi çözümleri b) Microsoft birinci taraf kataloğundan çözümler (PSC'de İşlem Anlaşması rolüne benzer) ve c) Diğer üçüncü taraf iş ortaklarının ortak satış çözümleri (PSC'de ISV Anlaşması rolüne benzer).|
|Anlaşma ataması|Anlaşmaları yalnızca atanan satıcı görüntülemeli ve üzerinde eylemde davranabilir.|Ekip üyeleri bir satış anlaşması üzerinde çalışan insanları belirtmek için bir satış anlaşmasına eklenebilir; diğer referans yöneticilerinin bu anlaşmaları görüntülemesini veya bu anlaşmalara göre hareketlerini engellemesi engellenmez.|
|Müşteri kuruluşu|Serbest biçimli metin girişi.|Yalnızca birkaç karakter [yazarak](manage-co-sell-opportunities.md#select-your-customer) [müşteri kuruluşunda D&B](https://www.dnb.com/) veritabanında arama edebilirsiniz. Yasal ad ve adres, seçime göre otomatik olarak doldurulur.|
|Müşteri ilgili kişisi|Zorunlu değildir.|Özel işlem hattı paylaşımı için zorunlu değildir. Microsoft satıcısı ortak satış isteğine katılmak için davet edildiyse gereklidir.|
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
1. Kullanıcı yönetimi görünümüne eşlenmiş PSC İş Ortağı Merkezi yönetimi görünümü
1. Kullanıcı rolü atama görünümüyle eşlenen PSC İş Ortağı Merkezi atama görünümü
1. Bildirim görünümüyle eşlenen PSC İş Ortağı Merkezi görünümü

### <a name="1---psc-home-page-mapped-to-the-partner-center-co-sell-opportunities-default-view"></a>1 - Ortak satış fırsatları varsayılan görünümüne İş Ortağı Merkezi PSC giriş sayfası

Üst PSC ekran görüntüsü ile altındaki ekran görüntüsü arasındaki eşleşen İş Ortağı Merkezi daireleri karşılaştırın. Eşleşen sayılar, PSC ile ilgili özelliği veya özniteliğini aşağıdaki İş Ortağı Merkezi. Kırmızı daireler, alanda eşleşen bir İş Ortağı Merkezi işaret ediyor.  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="İş Ortağı Satışları sayfasının giriş sayfası ile Bağlan'daki Ortak satış fırsatlarının varsayılan görünümü arasındaki alan eşlemelerini İş Ortağı Merkezi." lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>2 - İş Ortağı Merkezi anlaşma görünümüne eşlenmiş PSC kılavuz görünümü

Üst PSC ekran görüntüsü ile altındaki ekran görüntüsü arasındaki eşleşen İş Ortağı Merkezi daireleri karşılaştırın. Eşleşen sayılar, PSC ile ilgili özelliği veya özniteliğini aşağıdaki İş Ortağı Merkezi. Kırmızı daireler, alanda eşleşen bir İş Ortağı Merkezi işaret ediyor.  

> [!NOTE]
> Ekran görüntülerinin altında dikkat edilmesi gereken diğer noktalar da yer almaktadır.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="İş Ortağı Satışları (PSC) kılavuz görünümü ile Bağlan satış anlaşması görünümü arasındaki alan İş Ortağı Merkezi gösteren görüntü." lightbox="images/pscmigration/grid-view-expanded.png":::

**Dikkat edilmesi gereken özel noktalar:**

- PsC'ninki gibi İş Ortağı Merkezi liste görünümü yoktur.  Tüm anlaşmalar, müşteri bilgileri ve satış anlaşması türüyle birlikte alınan veya oluşturulan en son tarihe göre listelenir. Görünümde ilk anlaşma varsayılan olarak seçilidir. PSC tablo biçiminde görüntülenen değerlerin çoğu, satış anlaşması ayrıntı görünümünde İş Ortağı Merkezi.
- Anlaşma rolü, rol için gerekli bir İş Ortağı Merkezi. İş akışlarının hiçbirsinde görüntülenmez veya yakalanmaz. Satış anlaşmasına eklenen çözümlere göre Microsoft satıcı tarafında otomatik olarak türetilir.
- Son değiştirme tarihi, başvuru ayrıntıları sayfasında İş Ortağı Merkezi. İş ortakları, anlaşmaları son güncelleştirme tarihine göre sıralamak için sıralama işlevini kullanabilir.

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3 - PsC Anlaşma ayrıntıları görünümü, İş Ortağı Merkezi

Üst (PSC) ekran görüntüsünde eşleşen, numaralı daireleri, altındaki İş Ortağı Merkezi ekran görüntüsüyle karşılaştırın. Eşleşen sayılar, PSC ile ilgili özelliği veya özniteliğini aşağıdaki İş Ortağı Merkezi. Kırmızı daireler, verilerde eşleşen alan veya alan İş Ortağı Merkezi.

> [!NOTE]
> Ekran görüntülerinin altında dikkat edilmesi gereken diğer noktalar da yer almaktadır.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="İş Ortağı Satışları (PSC) anlaşma ayrıntıları görünümü Bağlan satış anlaşması ayrıntıları görünümü arasındaki alan İş Ortağı Merkezi gösteren görüntü." lightbox="images/pscmigration/deal-details-expanded.png":::

**Dikkat edilmesi gereken özel noktalar:**

- İş ortakları, iş ortağı anlaşması ayrıntı görünümünde düzenle düğmesini seçerek bir anlaşmayı düzenleyebilir (6). Düzenle düğmesi seçildikten sonra tüm alanlar düzenlenebilir hale gelecektir. Ardından anlaşmada yapılan düzenlemeleri kaydetme veya iptal etme seçeneğiniz vardır.
- Anlaşmayı aynı anlaşmada yinelenen olarak kapatma seçeneği İş Ortağı Merkezi.
- Müşteri Sonucu, İş Ortağı Merkezi. Müşteri etkileşimleri ile ilgili tüm ayrıntılar, İş Ortağı Merkezi.
- Tahmini çözüm kapatma tarihi yalnızca aynı anda yalnızca OEM IOT anlaşmaları İş Ortağı Merkezi. Bu bilgiler diğer hiçbir anlaşma türü için görüntülenmez.
- Lisanslama programı, lisanslama İş Ortağı Merkezi. Bu bilgiler, anlaşmada seçilen çözümlere göre otomatik olarak görüntülenir.

>[!Note]
>Kazanıldı veya kaybedildi olarak işaretlenen anlaşmalar daha sonra düzenlenemez. Anlaşmaları bu terminal durumları içine alırken dikkatli olun.

### <a name="4---psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>4 - 'Çözüm ekle' görünümüyle eşlenen PSC 'İş Ortağı Merkezi' görünümü

Üst (PSC) ekran görüntüsünde eşleşen, numaralı daireleri, altındaki İş Ortağı Merkezi ekran görüntüsüyle karşılaştırın. Eşleşen sayılar, PSC ile ilgili özelliği veya özniteliğini aşağıdaki İş Ortağı Merkezi. Kırmızı daireler, verilerde eşleşen alan veya alan İş Ortağı Merkezi.
  
:::image type="content" source="images/pscmigration/products.png" alt-text="İş Ortağı Satışları (PSC) ürün Bağlan görünümü ile çözüm ekleme görünümü arasındaki alan İş Ortağı Merkezi gösteren görüntü." lightbox="images/pscmigration/products-expanded.png":::

### <a name="5---user-management-in-psc-versus-partner-center"></a>5 - PSC'de kullanıcı yönetimi ile İş Ortağı Merkezi

Üst (PSC) ekran görüntüsünde eşleşen, numaralı daireleri, altındaki İş Ortağı Merkezi ekran görüntüsüyle karşılaştırın. Eşleşen sayılar, PSC ile ilgili özelliği veya özniteliğini aşağıdaki İş Ortağı Merkezi. Kırmızı daireler, verilerde eşleşen alan veya alan İş Ortağı Merkezi.  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="İş Ortağı Satışları (PSC) kullanıcı Bağlan giriş sayfası ile Hesap ayarları alanında İş Ortağı Merkezi Yönetim sayfası görünümü arasındaki alan eşlemelerini gösteren görüntü."  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="6---user-role-assignment-in-psc-versus-partner-center"></a>6 - PSC'de kullanıcı rolü ataması ile İş Ortağı Merkezi

Üst (PSC) ekran görüntüsünde eşleşen, numaralı daireleri, altındaki İş Ortağı Merkezi ekran görüntüsüyle karşılaştırın. Eşleşen sayılar, PSC ile ilgili özelliği veya özniteliğini aşağıdaki İş Ortağı Merkezi. Kırmızı daireler, verilerde eşleşen alan veya alan İş Ortağı Merkezi.  

:::image type="content" source="images/pscmigration/roles.png" alt-text="İş Ortağı Satışları (PSC) rol atama görünümü Bağlan rol atama görünümü arasındaki alan eşlemelerini İş Ortağı Merkezi görüntüsü." lightbox="images/pscmigration/roles-expanded.png":::

**Dikkat edilmesi gereken özel noktalar:**

- PSC yöneticisinin eşdeğer rolü, İş Ortağı Merkezi.
- Ortak satış anlaşması yönetimi için İş Ortağı Merkezi rol vardır. Bu rol, referans yöneticisi rolüdir.

### <a name="7---notifications-in-psc-versus-partner-center"></a>7 - PSC ile İş Ortağı Merkezi arasındaki bildirimler

Üst (PSC) ekran görüntüsünde eşleşen, numaralı daireleri, altındaki İş Ortağı Merkezi ekran görüntüsüyle karşılaştırın. Eşleşen sayılar, PSC ile ilgili özelliği veya özniteliğini aşağıdaki İş Ortağı Merkezi. Kırmızı daireler, verilerde eşleşen alan veya alan İş Ortağı Merkezi.  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="İş Ortağı SatışLarı ve (PSC) Bağlan eşlemesini ve İş Ortağı Merkezi görünümünü gösteren görüntü."  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>PSC'den İş Ortağı Merkezi - Sık sorulan sorular

Aşağıdaki bölümlerde geçişle ilgili sık sorulan sorular yanıtlanmaktadır.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1 - Erişim iznim yoksa ne İş Ortağı Merkezi?

Atanmış rolleri almak için "Erişim yok" sayfasında listelenen yöneticilerinize başvurabilirsiniz. Referanslar bölümünde [okuma ve](permissions-overview.md#manage-referrals) yazma izni için referans yöneticisi rolüne ihtiyacınız olacak. Yalnızca iş profillerini yönetiyorsanız, iş profili yöneticisi rolünüz İş Ortağı Merkezi.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="İş Ortağı Merkezi'da erişim yok deneyimini gösteren görüntü.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2 - Who bölümündeki Referanslar bölümüne erişim izni İş Ortağı Merkezi?

Hesap [yöneticiniz,](permissions-overview.md#manage-mpn-membership-and-your-company) Referanslar sekmesine erişmenizi sağlar. Hesap yöneticinizi bulmak için **panonun** sağ üst köşesindeki dişli simgesinden Hesap ayarları'İş Ortağı Merkezi [seçin.](https://partner.microsoft.com/dashboard) Ardından, ikinci **düzey,** sol gezinti çubuğundan Kullanıcı yönetimi'ni seçin. Kullanıcı listesinin üst kısmında Filtre  açılan menüsünü seçin ve seçeneğini hesap yöneticisi **olarak belirleyin.** Sayfada ilgili e-posta adresleriyle birlikte tüm hesap yöneticileri görüntülenir. İş hesabınız için referans yöneticisi rolünü atamasını istemek için bunlardan birini sorun.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3 - Hesabımız için +yeni anlaşma düğmesi gridir. Anlaşma oluşturmaya başlamak için ne yapabilirim?

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

İlk olarak, aşağıdaki adımları izleyerek doğru MPN KIMLIĞINI bulun

- Iş Ortağı Merkezi hesabınızda oturum açın
- MPN KIMLIĞINI bulmak için [Hesap ayarları belgelerinde](./partner-center-account-setup.md#locate-your-mpn-id) verilen kılavuzu kullanın.

Aşağıda, Iş Ortağı Merkezi MPN KIMLIĞINIZI bulabileceğiniz tam konumu gösteren ekran görüntüsü yer alabilir

:::image type="content" source="images/pscmigration/findingMPNID.png" alt-text="İş ortağının MPN KIMLIĞINI bulabileceği hesap ayarlarını gösteren resim."  lightbox="images/pscmigration/findingMPNID.png":::

seçin

- Bir PDM varsa, Iş Ortağı Merkezi hesabınızdaki doğru MPN KIMLIĞIYLE MPN KIMLIĞINIZI düzeltmesini isteyin.
- Bir PDM yoksa, PSC ana başlığında verilen adrese, hem PSC başlığında hem de Iş Ortağı Merkezi hesabınızdaki doğru MPN KIMLIĞINE sahip bir e-posta gönderin.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Iş Ortağı Merkezi 'nde anlaşmalar oluşturmanıza ve yönetmenize yardımcı olacak kaynaklar

Ortak satış yardım konularını henüz okumadıysanız, aşağıdaki kaynaklar Iş ortağı merkezindeki anlaşmaları yönetmenize yardımcı olur.

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


- iş ortağı satışları iş ortağı [merkezi çalışma kitabına](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) , iş ortaklarının satış süreçlerini ve rollerini iş ortağı merkezi ile iş ortağı satış Bağlan ile yeni satış süreçleriyle hizalamak için çalışma kitabı. Bağlan
- [Iş Ortağı Merkezi ortak satış çalışma kılavuzu](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) -müşteri adaylarını yönetmek Için Iş Ortağı Merkezi aracılığıyla bir işletim modelini belirlemek için bir iş modeli veya ortak satış fırsatları ve anlaşmaları kaydetme.
- [Başvuru yönetimi destesi](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) -müşteri adaylarını yönetmek için görselleştirilen adım adım yönergeler ve Iş Ortağı Merkezi aracılığıyla ortak satış fırsatları.
- [Ticari Market 'Te yayımlama ve yönetme](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) -ticari Market 'Teki Iş Ortağı Merkezi aracılığıyla teklifler oluşturmak, yönetmek ve yayımlamak için görselleştirilen adım adım yönergeler.