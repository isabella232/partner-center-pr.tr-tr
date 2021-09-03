---
title: İş Ortağı SatışLarı Bağlan (PSC)
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: Microsoft iş ortaklarının İş Ortağı Satışları Bağlan (PSC) İş Ortağı Merkezi Microsoft satıcılarının gönderdiği anlaşmaları oluşturma veya yönetme işlemlerini nasıl yönettiklerini öğrenin.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 12/07/2020
ms.openlocfilehash: d75f268b93d0a9c864bd6daeff3276810be7e928
ms.sourcegitcommit: 09d2c10491244775e656b48fce35b5648262ce59
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/03/2021
ms.locfileid: "123458061"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>İş Ortağı Satışları (PSC) İş Ortağı Merkezi (PSC) iş ortakları için Bağlan satış kılavuzu

**Uygun roller:** Hesap yöneticisi | Referans yöneticisi | İş Ortağı Bağlan (PSC) satıcısı | İş Ortağı Bağlan (PSC) yönetici | İş Ortağı Bağlan (PSC) anlaşma yöneticisi

Bu makalede, iş ortaklarının iş ortağı satış anlaşmaları oluşturma ve yönetmeye devam etmek için İş Ortağı Satışları Bağlan'den İş Ortağı Merkezi'ye (PC) İş Ortağı Merkezi.

>[!Note]
> PsC'de geçişle ilgili bir başlık gördüğü için buradasanız doğru yerdesinizdir. Bu kılavuz, PSC'de anlaşmalarını yöneten Çözüm Değerlendirmesi (SA) ve OEM lisanslama iş ortakları için geçerli değildir.

>[!Important]
> 1 Nisan 2021'den itibaren, şirketiniz PSC'de anlaşma oluşturabilecek veya anlaşmaları düzenleyemez. **PSC'de toplu dışarı aktarma özelliğini kullanarak mevcut anlaşma verilerini indirmeye devam edersiniz. Ayrıca açık [anlaşmaları PSC'den](psc-to-pc.md#psc-deals-migration) bu tarihten sonra İş Ortağı Merkezi geçişe de geçirilir.** <br><br> IP ortak satış teşviki için uygun çözümler içeren etkin bir şekilde üzerinde çalıştığınız anlaşmalar varsa iki seçeneğiniz vardır: <br><br> 1. Anlaşmayı kazanildi olarak işaretle ve 31 Mart 2021'den önce PSC'de anlaşma kaydını tamamla. <br> 2. [Anlaşmaları İş Ortağı Merkezi](psc-to-pc.md#psc-deals-migration) daha fazla zaman elde etmek ve anlaşma kaydını başlatmak için geçiş.

Bildiğiniz gibi şirket, **30 Nisan 2021'den sonra PSC'ye erişimi kaybeder.** Ancak, ortak satış anlaşmaları oluşturma, anlaşmalarınızı yönetme ve Microsoft satıcılarının size gönderdiği anlaşmalara göre hareket İş Ortağı Merkezi istediğiniz her şeyi yine de bulabilirsiniz.

Ancak farklar vardır. Aşağıdaki kılavuz, geçiş sürecinizin daha sorunsuz ve İş Ortağı Merkezi yardımcı olabilir.

## <a name="before-you-move-things-you-need-to-know"></a>Taşımadan önce, bilmek gerekenler

### <a name="if-you-are-a-psc-admin"></a>PSC yöneticisiyseniz

- İş Ortağı Merkezi'da oturum a almak için bir iş [e-postası gerekir.](https://partner.microsoft.com/)
- Hesap yöneticisinin yardımıyla İş Ortağı Merkezi [ayarlayın.](permissions-overview.md)
- Bu belgeyi okuyarak İş Ortağı Merkezi satış yapmayı öğrenin.
- Tüm PSC kullanıcılarınız (İş Ortağı Merkezi, Satış yöneticisi ve Satıcı rolleri) için hesaplarda kullanıcı hesapları ayarlayın ve bu kullanıcılara [referans yöneticisi rolleri atfı gerçekleştirin.](permissions-overview.md)

>[!IMPORTANT]
> PSC başlığında Microsoft İş Ortağı Ağı (MPN) kimliğinin, İş Ortağı Merkezi'deki MPN konumları listesinde kullanılabilir olduğundan emin İş Ortağı Merkezi.

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="İş ortaklarının MPN kimliğini bularak PSC başlıklarını gösteren resim.":::

 MPN Kimliğinin İş Ortağı Merkezi MPN konumu olarak görüntülendiğinden emin olmak için İş Ortağı Merkezi panosunda oturum [açın,](https://partner.microsoft.com/dashboard)ardından ekranın sağ üst köşesindeki **Ayarlar** (Dişli simgesi) öğesini ve ardından **Hesap** Ayarlar. İkinci düzey, sol gezinti menüsünde Konumlar'ı seçerek hesap hesabıyla ilişkili tüm MPN kimliklerinin ve konumların İş Ortağı Merkezi seçin. 

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>PSC satış yöneticisi veya satıcıysanız

- Panoda oturum alasınız için bir iş e-İş Ortağı Merkezi [gerekir.](https://partner.microsoft.com/dashboard)
- PSC'de iş dışı bir hesap kullanıyorsanız veya iş e-postanız iş ortağı şirketten farklı bir şirkete yönelikse, hesap ayarlama yardımı için PSC yöneticinize ulaşın.
- PSC'de oturum a İş Ortağı Merkezi hesap ne olursa olsun hesap ayarlama işleminin tamamlandıktan sonra PSC yöneticinize sorun.
- İş Ortağı Merkezi ve Referanslar bölümüne erişiminiz olduğunu doğrulayın.
- İş akışlarını ve iş akışlarında yapılan değişiklikleri anlamak için bu İş Ortağı Merkezi.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>PSC'de yönetici olarak, sonraki adımlarınız bunlardır

Sol İş Ortağı Merkezi menüsünden Referanslar **seçeneğini** belirleyin. Referanslar sayfalarına erişebilirsiniz.

  >[!Note]
  > Referanslar sayfalarına erişim İş Ortağı Merkezi kimlik bilgilerinizi yenilemek için oturum açma ve oturum açma işlemlerinizi yeniden açmanız gerekir.

İş Ortağı Merkezi menüsünde veya Referanslarla ilgili sayfalarda Referanslar seçeneğini görmüyorsanız, şirketin hesap yöneticisine [](permissions-overview.md) başvurarak Referanslar seçeneğine ve  ilgili alana erişmenizi istemelerini sorun. 

Şirketinizin hesap yöneticisini bulmak için:

1. Panonun **sağ** üst köşesindeki dişli simgesinden Hesap ayarları'İş Ortağı Merkezi seçin.

1. İkinci **düzey,** sol gezinti menüsünden Kullanıcı yönetimi'ni seçin.

1. Kullanıcı listesinin üst kısmında Filtre **açılan** menüsünü seçin. Seçeneğini Hesap yöneticisi **olarak değiştirme.**

   Sayfada ilgili e-posta adresleriyle birlikte tüm hesap yöneticileri görüntülenir. Bunlardan birini e-postayla gönderin ve iş hesabınız için referans yöneticisi rolünü atamasını sorun.

  :::image type="content" source="images/pscmigration/account-admin.gif" alt-text="İş ortağı ayarları kullanıcı yönetimi sayfasında hesap yöneticilerini gösteren resim.":::

>[!Important]
>- Rolünüz yalnızca PSC'de kullanıcıları yönetmeyi içeriyorsa, şirketinizin hesap yöneticisinin şirket içinde hesap yöneticisi rolünü [size](permissions-overview.md#manage-mpn-membership-and-your-company) atamasını İş Ortağı Merkezi. 
>- Rolünüz ortak satış fırsatlarını yönetmeyi de içerirse referans yöneticisi [rolünün atanmasını](permissions-overview.md#manage-referrals) istemeniz gerekir.
> - PSC yöneticileri arasında bir değişiklik yönetimi adayı da göstermeniz iyi bir fikirdir. Bunu yapmak, tüm PSC yöneticilerinin hesap yöneticilerine tek tek İş Ortağı Merkezi engel olur. Bunun yerine değişiklik yönetimi müşteri adayı, hesap yöneticisiyle İş Ortağı Merkezi kişi olabilir.

## <a name="user-migration"></a>Kullanıcı geçişi

İş Ortağı Merkezi'da hesabınız İş Ortağı Merkezi ortak satış fırsatları sayfasındaki kullanıcı geçiş sihirbazını kullanarak şirket çalışanlarınıza İş Ortağı Merkezi rollerini otomatik olarak atfın.

>[!Note]
> Kullanıcı geçişi yalnızca şirketinizin [hesap yöneticileri](permissions-overview.md#manage-mpn-membership-and-your-company) tarafından yapılabilir. Hesap yöneticisi rolüne sahip değilseniz, kullanıcı geçiş sihirbazının yardımıyla kullanıcı hesaplarını ayarlamaya yardımcı olacak bir hesap yöneticisi bulun.

:::image type="content" source="images/pscmigration/user-migration.gif" alt-text="Kullanıcı geçiş sihirbazını gösteren görüntü.":::

Hesap yöneticileri, referans kılavuzunun yanındaki ortak satış fırsatları sayfasında psC kullanıcı geçiş sihirbazı bağlantısını görebilir. Bağlantıyı seçerek kullanıcı geçişini başlatabilirsiniz. Yöneticiler, kullanıcı geçişini başlatmak için bağlantıyı seçerek. Bu kullanıcı geçişi adımını, tüm kullanıcılarAsneden kullanıcıya uygun roller atanana kadar birden çok İş Ortağı Merkezi.

Kullanıcı geçiş tablosunda aşağıdaki ayrıntılar yer alır:

- Kullanıcı hesabı - Çalışanın e-posta kimliği
- PSC iş ortağı hesabı - Çalışanın PSC'de ilişkili olduğu hesap
- PSC kullanıcı rolü - PSC'de atanan üç rolden biri.
- PC MPN konumu - Kullanıcıya ilgili rol (PC) İş Ortağı Merkezi verilecek konum. PSC iş ortağı hesabı MPN'i, izin atamak için İş Ortağı Merkezi mpN konumunu bulmak için kullanılır. Kuruluşun tamamı vOrg MPN kimliğini ifade ediyor.
- BILGISAYAR kullanıcı rolü - Çalışanlara PSC kullanıcı rollerine göre roller atanır. PSC'de yöneticiye, yönetici rolünde Referans yöneticisi İş Ortağı Merkezi. Satıcıya kaynaklarda referans kullanıcı rolü İş Ortağı Merkezi. Bu rollerle ilgili İş Ortağı Merkezi ve bu rollere sahip kullanıcıların bu rollerle neler İş Ortağı Merkezi [buradan öğrenebilirsiniz](permissions-overview.md#manage-referrals)
- PC AAD Kiracısı - Microsoft Azure Active Directory 'de kullanıcıların atandığı kiracı (Azure AD) İş Ortağı Merkezi
- Durum - Geçişin durumu için üç olası durum vardır
    - **Geçirilmez** - Kullanıcıya herhangi bir İş Ortağı Merkezi referans rolü atanmamış
    - **Geçirildi** - Kullanıcı tabloda gösterildiği gibi ilgili rol atanmış şekilde başarıyla geçirildi
    - **Hata** - Bazı hata nedeniyle geçiş tamamlanmadı

Bazen geçiş başarısız olabilir ve hatalara neden olabilir. Geçişin hataya neden olabileceğinin birkaç nedeni ve sorunu çözmenin bazı yolları:

1. PSC kullanıcıları iş dışı bir hesap kullanıyor olabilir.

2. PSC kullanıcısı, etki alanındaki hesaplardan farklı bir hesap kullanıyor olabilir İş Ortağı Merkezi.

   Senaryo 1 ve 2 ile ilgili hataları çözmek için kullanıcıdan Azure AD kiracınıza İş Ortağı Merkezi iş hesabını kullanarak oturum açmasını sorun. Genel [yöneticiniz yardımcı](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) olabilir.
   
   Genel yöneticinizi bulmak için: 
   - Panoda oturum İş Ortağı Merkezi [sağ](https://partner.microsoft.com/dashboard) **üst köşesindeki** dişli simgesinden Hesap ayarları'ı seçin.
   - İkinci **düzey,** sol gezinti çubuğundan Kullanıcı yönetimi'ni seçin.
   - Kullanıcı listesinin üst kısmında Filtre  açılan menüsünü seçin ve seçeneğini Genel yönetici **olarak belirleyin.** Ardından sayfada ilgili e-posta adresleriyle birlikte tüm genel yöneticiler görüntülenir. İş hesabınız için referans yöneticisi rolünü atamasını istemek için bunlardan birini sorun.
   
      Genel yönetici, Azure AD kiracınız içinde yeni bir kullanıcı hesabı oluşturabilir veya diğer etki alanı hesabı kullanıcılarına konuk kullanıcı erişimi atayabilirsiniz. Hesaplar tüm PSC anlaşma yöneticileri ve kullanıcıları için ayar olduktan sonra, İş Ortağı Merkezi'de  oturum açmaları, sol gezinti menüsünden Referanslar'ı seçmeleri ve Referanslar sayfasını görene kadar onaylamaları gerekir.

3. Kullanıcının zaten bu rolde atanmış bir referans rolü İş Ortağı Merkezi.
    - Kullanıcının mevcut rolünü doğrularsanız. Uygulamanın sağ üst köşesinde, İş Ortağı Merkezi **(dişli simgesi) Ayarlar'ı** ve ardından Hesap **ayarları'ı seçin.** İkinci bir sol gezinti menüsü gördüğünüzde Kullanıcı **yönetimi'ni seçin** ve kullanıcı için arama yapabilirsiniz.

## <a name="psc-deals-migration"></a>PSC Anlaşmaları geçişi

Kullanıcı geçişini tamamlandıktan sonra ortak satış fırsatları sayfasındaki satış anlaşmaları geçiş sihirbazını kullanarak PSC'den tüm uygun açık anlaşmaları İş Ortağı Merkezi. **Anlaşmalar geçiş bağlantısı yalnızca tüm kuruluş kapsamına sahip referans yöneticileri tarafından İş Ortağı Merkezi.** Ortak satış fırsatları sayfasının sağ üst kısmında **"PSC anlaşmaları geçişi"** adlı bir bağlantı olacak ve bu bağlantı satış anlaşması geçiş sihirbazını açacaktır.

Anlaşma geçişini başlatmadan önce bu bölümü okuyun.

**Geçiş için uygun**

PsC'den İş Ortağı Merkezi'a geçiş için yalnızca bazı anlaşmalar İş Ortağı Merkezi. Bu geçiş sihirbazı, iş ortaklarının anlaşmalarını anlaşmaları İş Ortağı Merkezi müşterileri ile etkin bir şekilde çalışarak anlaşmaları kapatmalarına yardımcı olmak için oluşturulur. **Yalnızca geçerli iş ortağı hesabı ayrıntılarıyla (geçerli MPN KIMLIĞI) 1 Ocak 2020'den itibaren oluşturulan ve anlaşma kaydından geçen açık durumdaki anlaşmalar geçiş için uygundur.**

**Geçiş için uygun değil**

- Çözüm değerlendirme anlaşmaları anlaşma geçişi için uygun değil
- OEM lisanslama iş anlaşmaları, anlaşma geçişi için uygun değildir
- PSC'de kazanildi olarak işaretlenen anlaşmalar geçiş için uygun değildir. Kazandı olarak işaretlenen anlaşmalar için uygunsa anlaşma kaydı PSC'de tamamlanır.

## <a name="pre-requisites-for-deal-migration"></a>Anlaşma geçişi için önkullar

İş Ortağı Merkezi'dan anlaşma geçişini başlatmadan önce, başarılı bir geçiş için PSC'de anlaşmaları ayarlamak için aşağıdaki yönergeleri izleyin.

1. Şirketinizin açık anlaşmalar üzerinde çalışan tüm satış ekibi üyeleri bu geçiş hakkında bilgi sahibidir.
2. Satış ekibi üyeleri, anlaşma yönetimi için İş Ortağı Merkezi için eğitilmiş.
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
> Yukarıdaki önkullar karşılanmazsa bile anlaşma geçişi başarılı olur. Ancak, yukarıdaki belirtilen gerekli alanlardan herhangi biri kullanılabilir durumda yoksa İş Ortağı Merkezi değiştiremezsiniz. Ardından, üzerinde çalışmaya başlamak için anlaşmalarda eksik olan tüm İş Ortağı Merkezi bilgileri girmeniz gerekir. **Uygun anlaşmaları İş Ortağı Merkezi'a başlamadan önce PSC'de temizlemeniz önemle tavsiye İş Ortağı Merkezi.**

Geçiş anlaşması İş Ortağı Merkezi tek tıklama deneyimi olarak yerleşiktir. Tek ihtiyacınız olan, şirket uygun anlaşmaları geçirmek için hazır olduğunda **"Anlaşmaları geçir"** düğmesini seçmektir. **PSC'den geçirmek istediğiniz anlaşmaları seçesiniz. Herhangi bir anlaşmayı geçişe geçirmek istemiyorsanız İş Ortağı Merkezi başlamadan önce bunları PSC'de kapalı durumuna taşımanız gerekir.**

>[!Note]
> Geçiş başlatıldıktan sonra, **anlaşmaların geçişi 24 saat kadar sürebilir.**

Geçiş tamamlandıktan sonra başlık iletisi, geçiş raporunun bağlantısıyla tamamlanacak şekilde değişir. PSC'den İş Ortağı Merkezi'a geçirilen anlaşmaların ayrıntılarını görüntülemek için raporu İş Ortağı Merkezi.

Rapor aşağıdaki ayrıntıları içerir.

1. **İş Ortağı Merkezi kimliği** - Bir etkileşimde İş Ortağı Merkezi anlaşmaların benzersiz tanımlayıcısı. İki satış anlaşması vardır: biri iş ortağı, biri de Microsoft için ortak satış anlaşmasında İş Ortağı Merkezi.
2. **İş Ortağı Merkezi kimliği** - İş ortağına ait İş Ortağı Merkezi için geçerli olan benzersiz tanımlayıcı.
3. **Anlaşma adı** - PSC'de anlaşmaya verilen tanımlayıcı.
4. **PSC anlaşma kimliği** - Anlaşma için PSC'deki benzersiz tanımlayıcı.
5. **Hatalar** - belirli bir anlaşmadan başka bir anlaşmayı alırken herhangi bir hata olup olamay olduğunu belirtmek için.

Başarıyla geçirilen tüm anlaşmalar PSC'de görünmez. Geçiş yapılan anlaşmalar üzerinde İş Ortağı Merkezi devam İş Ortağı Merkezi. Ortak satış anlaşmaları için Microsoft satıcılarının etkileşimleri üzerinde değişiklik olmayacaktır.

PSC'den geçirilen anlaşmalar, satış anlaşması kaynağına bağlı olarak Gelen ve Giden sekmelerinde kullanılabilir. Şirket tarafından paylaşılan tüm satış anlaşmaları Giden sekmesinde, Microsoft tarafından başlatılan satış anlaşmaları ise şirket içinde İş Ortağı Merkezi. Geçiş sonrası oluşturulacak iki tür anlaşma vardır.

1. **Ortak satış anlaşmaları** - PSC'de ortak satış olarak işaretlenen satış anlaşmaları, psc'de ortak satış anlaşması olarak İş Ortağı Merkezi.
2. **İş ortağı tarafından yapılan anlaşmalar** - Ortak satış olarak işaretlenen anlaşmalar, ortak satış anlaşması olarak İş Ortağı Merkezi. İş ortağı tarafından yönlendirilen satış anlaşmaları Microsoft satıcılarının kullanımına açıktır ve terminal durumuna ulaşmadan önce ortak satış anlaşmalarına yükseltilebilir (kazanıldı, kaybedildi). Ayrıca, anlaşmada teşvike uygun bir çözüm varsa, iş ortağı tarafından yönlendiren anlaşmalar anlaşma kaydı için uygun olur.

>[!Important]
> Bazı anlaşmaların geçirilenemleri nedeniyle herhangi bir hata varsa, "Anlaşmaları geçir" düğmesine tıklayarak anlaşma **geçişini yeniden başlatabilirsiniz.** Yalnızca henüz geçirilemeyen bazı uygun anlaşmalar varsa etkinleştirilir. Bu, anlaşma geçişi başladıktan sonra PSC'de bazı yeni anlaşmaların oluşturulacak olduğu geçiş aşamasında da yararlı olacaktır.

Tüm anlaşmalar başarıyla geçirildiktan sonra , **"Anlaşmaları geçir"** düğmesinin devre dışı bırakıldığında "Geçirılacak anlaşma **yok"** ifadesini gösteren bir başlık **vardır.**

Kullanıcı geçişini ve/veya anlaşma geçişini tamamladıktan sonra, geçiş stratejisine karar vermek için aşağıdaki kılavuzu kullanın:

Şirketinizin bir İş Ortağı Geliştirme Yöneticisi (PDM) varsa - İş Ortağı Merkezi hesabınız ayar olduğunda ve kullanıcılarınız başka bir yere taşındığında ve rollere ve izinlere sahip olduğunda, Ortak Satış etkinliklerinizi İş Ortağı Merkezi. PdM'yi geçiş işleminin son tarihine kadar beklemek yerine geçişi yapmaları konusunda bilgilendirin. Bu, tüm yeni anlaşmaların geçişe İş Ortağı Merkezi.

>[!Note]
>Bu anahtarı kullandıktan sonra yalnızca PSC'de mevcut Etkin anlaşmalar üzerinde eyleme geçesiniz. PSC'de Microsoft satıcılarından yeni anlaşmalar oluşturasınız veya satış anlaşması alamaysınız.

Şirkette PDM yoksa - Tüm kullanıcı hesaplarının ayarlandığından ve tüm kullanıcılar tarafından doğrulandığından emin olun. Bir e-posta ve PSC'de, satışa ilk başlanmaz tarihi içeren bir başlık ile size İş Ortağı Merkezi. PSC'de mevcut etkin anlaşmaları yönetmeye devam etmek zorunda olduğunu unutmayın.

>[!Important]
> Kazanildi olarak işaretlenen anlaşmaları kaydetmek için 30 Nisan 2021'e kadar devam edilecektir.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>PSC yöneticileri, PSC anlaşma yöneticileri ve PSC satıcıları için sonraki adımlar

İş Ortağı Merkezi'da ortak satış yapmayı İş Ortağı Merkezi.
Bu önemli bir adımdır ve bu adım, satış ve satış için hazırlık İş Ortağı Merkezi. Hemen ortak satış yapmak için İş Ortağı Merkezi iş akışlarını ve değişiklikleri anlıyoruz. Bu belgeyi tamamen okuyarak başlayabilirsiniz. ortak satış deneyimi galerisinde de [iyi bir kaynak kümesi mevcuttur.](https://aka.ms/cosellexperience)

## <a name="major-differences-between-psc-and-partner-center-workflows"></a>PSC ile iş akışları arasındaki İş Ortağı Merkezi farklar

|**Senaryo**|**İş Ortağı Satış Bağlan**|**İş Ortağı Merkezi**|
|-----|:-----|:-----|
|Kullanıcı rolleri|PSC'de yönetici, satış yöneticisi ve satıcı rolleri vardır.|İş Ortağı Merkezi yalnızca tüm [anlaşmalar](permissions-overview.md#manage-referrals) için okuma ve yazma izni veren referans yöneticisi rolüne sahip olur.|
|Ortak satış anlaşması için Microsoft'u davet etme|Microsoft satıcısı tarafından başlatılan bu işlem, iş ortağı tarafından açık bir şekilde sorulmaz.|Anlaşma için bir Microsoft [satıcısının yardımı gerekirse](manage-co-sell-opportunities.md#add-solutions) iş ortağının açık bir istekte yerması gerekir. Microsoft Seller'ın isteği reddetme seçeneği vardır.|
|Süre sonu|Anlaşma süresinin dolması kavramı yoktur.|İş ortağı tarafından kabul edilmediğinde iş ortağı gelen anlaşmaların süresi 14 gün içinde dolar. Aynı durum, Microsoft satıcısının 14 gün içinde eyleme geçene kadar süresi dolan iş ortağı giden satış anlaşmalarında da geçerli olur.|
|Microsoft satıcı ayrıntıları|Anlaşma oluşturulur oluşturulmaz görünür.|Microsoft Satıcı ayrıntıları yalnızca satıcı iş ortağından ortak satış davetini açıkça kabul ederse İş Ortağı ile paylaşılır.|
|[Özel işlem hattı](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Kullanılamıyor.|İş ortakları, Microsoft satıcılarına görünürlük vermeden işlem hatlarını paylaşabilir.|
|Çözümler|Bir satış anlaşmasına yalnızca bir fiyat listesine ait çözümler eklenebilir.|İş ortağı aşağıdaki [listelere](manage-co-sell-opportunities.md#add-solutions) ait çözümler ekleyebilir. a) Kendi çözümleri b) Microsoft birinci taraf kataloğundan çözümler (PSC'de İşlem Anlaşması rolüne benzer) ve c) Diğer üçüncü taraf iş ortaklarının ortak satış çözümleri (PSC'de ISV Anlaşması rolüne benzer).|
|Anlaşma ataması|Anlaşmaları yalnızca atanan satıcı görüntülemeli ve üzerinde eylemde davranabilir.|Anlaşma üzerinde çalışan insanları belirtmek için bir satış anlaşmasına ekip üyeleri eklenebilir; diğer referans yöneticilerinin bu anlaşmaları görüntülemesini veya bu anlaşmalara göre hareketlerini engellemesi engellenmez.|
|Müşteri kuruluşu|Serbest biçimli metin girişi.|Yalnızca birkaç karakter [yazarak](manage-co-sell-opportunities.md#select-your-customer) [müşteri kuruluşunda D&B](https://www.dnb.com/) veritabanında arama edebilirsiniz. Yasal ad ve adres, seçime göre otomatik olarak doldurulur.|
|Müşteri ilgili kişisi|Zorunlu değildir.|Özel işlem hattı paylaşımı için zorunlu değildir. Microsoft satıcı, ortak satış isteğine katılmaya davet edildiyseniz gereklidir.|
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

Bu durum yalnızca mpN kuruluşuna bağlı ortak satışa hazır çözüm yoksa ve bu çözümde İş Ortağı Merkezi. Çözümlerinizin MPN kimliğinin düzeltilmesi için PDM'nize başvurun veya sorundan bahsederek bir destek bileti oluşturun: "PSC geçişi sonrasında yeni satış anlaşması düğmesi gri."

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4 - PSC gibi kuruluştan belirli bir kişiye anlaşma atay musunuz?

Takım üyelerini belirli bir satış anlaşmasına at attayarak. Diğer referans yöneticilerinin bu anlaşmaları görüntülemesini veya bu anlaşmalara göre hareket etmelerini engellemez.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5 - Bana atanan tüm anlaşmaların bir görünümü var mı?

Kullanıcı düzeyinde bir sekme olan sık kullanılanlar özelliğini kullanabilirsiniz. Anlaşmalara hızlı erişim elde etmek için size sık kullanılanlar olarak atanan tüm anlaşmaları işaretlebilirsiniz.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6 - Anlaşmalar için salt okunur bir görünüm var mı?

Hayır, referanslar bölümünde anlaşmaların salt okunur bir görünümü yoktur. Tüm referans yöneticileri tüm anlaşmalara tam okuma ve yazma erişimine sahip olur.

### <a name="7---how-can-i-register-a-deal-after-marking-it-as-won"></a>7 - Anlaşmayı won olarak işaretledikten sonra nasıl kayıt olabilirim?

Anlaşma aşağıdaki ölçütleri karşılarsa, anlaşma kaydını başlatmak için bir açılır [pencere görüntülenir.](./register-deals.md)

- Anlaşmada teşvike uygun bir çözüm vardır.
- Microsoft satıcısı satış anlaşmasına katılmak için davet edildi veya sizi satış anlaşmasına davet etti.
- Microsoft kartı, İş Ortağı Merkezi'da Kabul Edildi veya Kazanıldı İş Ortağı Merkezi.

### <a name="8---i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>8 - Anlaşma Kaydı bölümünde "+Yeni anlaşma kaydı" düğmesini seçerek hata iletisi alıyorum. Anlaşmalarımı nasıl kaydederim?

**+Yeni satış anlaşması** kaydı düğmesi yalnızca ISV bağlantı programına kayıtlı olan iş ortakları tarafından satış anlaşmasına karşılık gelen ortak satış fırsatı olmayan bir satış anlaşması kaydetmek için İş Ortağı Merkezi. Ortak satış fırsatıyla anlaşmaları kaydetmek için, anlaşma kazanildi olarak işaretlendiğinde ve anlaşma kaydı ölçütlerini karşılarsa bir açılır pencere görüntülenir.

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9 - Müşteri kuruluşu eklemek zorunlu mu?

Evet, bir müşteri [kuruluşuna](./manage-co-sell-opportunities.md#select-your-customer) yeni bir kuruluş eklemek İş Ortağı Merkezi. İlk olarak müşterinin bulunduğu konumu arayarak başlayalım. Sahip olduğunuz ayrıntılara göre; Tam bina adı dahil olmak üzere belirli olabilir veya yalnızca şehir ayrıntılarını veabilirsiniz. Kuruluş araması, herhangi bir adres ayrıntısı girmek zorunda olmadığınız adla eşleşen tüm yasal varlıkları getirir. Tüm ayrıntılar seçilen kuruluşa göre otomatik olarak doldurulur.

### <a name="10---are-customer-contact-details-mandatory"></a>10 - Müşteri iletişim bilgileri zorunlu mu?

Oluşturmakta [olduğunu anlaşma türüne](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) bağlıdır. Yalnızca işlem hattınızı paylaşıyorsanız ve Microsoft satış kuruluşundan herhangi bir yardıma gerek yoksa, müşteri iletişim bilgilerini vermeyebilirsiniz. Microsoft satıcısından etkin bir şekilde yardım almak için ortak satışlar yaptıysanız müşteri iletişim bilgilerini de sağlayabilirsiniz. Bir ortak satış isteği oluşturmadan önce müşteriden açık onay İş Ortağı Merkezi.

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11 - Bir anlaşmaya kaç çözüm ekleyebilirim?

Bir satış anlaşmasına en fazla 50 çözüm (PSC'de 'ürünler' ile benzer) eklersiniz. PSC'den farklı olarak, ortak satışa uygun çözümleriniz, Microsoft birinci taraf SKÜ'ler ve diğer üçüncü taraf ortak satışa uygun çözümleriniz çözümlerini karma olarak kullanabilirsiniz. Bu rolde seçilecek veya kullanılabilir bir satış İş Ortağı Merkezi. Microsoft SKU'ları için isteğe bağlı olarak satış anlaşmasına eklenen her SKU için miktar ve fiyat eklenmiştir.

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12 - Satış anlaşması oluşturduklarından sonra Microsoft satıcısının ayrıntılarını ne zaman edinecekim?

Microsoft satıcılarına yalnızca Microsoft tarafında ilgili satıcı kişisi ile anlaşma oluşturulurken belirtilen tam yardım gereksinimi eşledikten sonra atanır. Atamadan sonra bile Microsoft satıcıları ortak satış davetini kabul etme veya reddetme seçeneğine sahip olur. Yalnızca bir satıcı ortak satış daveti kabul edilirse satış anlaşması Microsoft satıcı iletişim bilgileriyle güncelleştirilir. Microsoft satıcılarının satış anlaşmasına göre hareket etmek için SLA'sı 14 gündür. İş ortaklarının süresi dolmuş durumuna gelmeden önce anlaşma üzerinde hareket etmek zorunda olduğu SLA'dır.

### <a name="13---where-can-i-find-the-opportunity-id"></a>13 - Fırsat kimliğini nerede bulamıyorum?

PSC'deki Fırsat Kimliği, İş Ortağı Merkezi. Herhangi bir anlaşmayı a açmak için anlaşma adının yanında anlaşma kimliğini bulabilirsiniz.

### <a name="14---how-can-my-pdm-get-access-to-partner-center"></a>14 - PDM'm İş Ortağı Merkezi?

İş Ortağı Merkezi PSC'den farklı olarak PDM'ler tarafından erişilemez. Bu özelliği etkinleştirmek için aşağıda belirtilen birden çok seçenek vardır.

- OCP Analizler - PDM'ler yalnızca anlaşmaları ve ilgili ilerlemeleri görüntülüyorsa, kuruluş görünümlerinizi almak için One Ticari İş Ortağı (OCP) Analizler portalını kullanabilirler. Bu bir iç araçtır ve yalnızca PDM'ler için kullanılabilir. OCP içgörüleri, şirket kullanıcıları için kullanılamaz.
- İş Ortağı Merkezi konuk kullanıcı - PDM hesabını İş Ortağı Merkezi bir konuk kullanıcı olarak ekleyebilir ve referansları görüntüleysin ve bunlar üzerinde eylem gerçekleştireb için onlara referans yöneticisi @microsoft.com rolü atabilirsiniz.
- Kiracınız [içinde yeni](./create-user-accounts-and-set-permissions.md#add-a-new-user) bir kullanıcı oluşturma - Kendi kiracınız içinde yeni bir kullanıcı oluşturabilir ve bu ayrıntıları PDM ile paylaşarak, hesabın diğer referans kullanıcılarına benzer referansları görüntülemelerini ve bu kullanıcılara göre hareketlerini gerçekleştirebilirsiniz.

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>PSC'deki hesabınız geçerli bir MPN ile ilişkili değilse doğru MPN kimliğini bulma

PSC'de 'PSC geçersiz MPN ID ilişkilendirme sorunu' başlığıyla ilgili bir başlık gördükten dolayı buradaysanız, doğru yerdesiniz demektir. Hesabınız aşağıdaki nedenlerden dolayı geçersiz bir MPN kimliğine bağlanmış olabilir

- Şirketinizin bir İş Ortağı Merkezi yok.
- PDM'niz, PSC hesabınızla İş Ortağı Merkezi hesabınıza (MPN ID) bağlantı olan dahili sistemlerde hesabınıza mpN kimliğini girerken bir hata yaptı.
- Şirket, Partner Membership Center(PMC) İş Ortağı Merkezi.

İlk olarak, aşağıdaki adımları izleyin ve doğru MPN kimliğini bulun

- İş Ortağı Merkezi oturum açın
- MPN kimliğini bulmak [için hesap ayarları belgelerinde](./partner-center-account-setup.md#locate-your-mpn-id) verilen kılavuzu kullanın.

Aşağıda, mpN kimliğiniz için tam olarak hangi konumda İş Ortağı Merkezi ekran görüntüsü verilmiştir

:::image type="content" source="images/pscmigration/finding-mpn-id.png" alt-text="İş ortağının MPN kimliğini bularak hesap ayarlarını gösteren resim."  lightbox="images/pscmigration/finding-mpn-id.png":::

seçin

- PDM'niz varsa, mpN kimliğinizin hesaptan doğru MPN kimliğiyle düzeltilmesini İş Ortağı Merkezi.
- PDM'niz yoksa, PSC başlığında gösterilen PSC hesap bilgilerini ve psc hesabınızdan doğru MPN kimliğini içeren PSC başlığında verilen adrese bir e-posta İş Ortağı Merkezi.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Satış anlaşmalarınızı oluşturmanıza ve yönetmenize yardımcı olacak kaynaklar İş Ortağı Merkezi

Ortak satış yardım konularını henüz okumadısanız, aşağıdaki kaynaklar satış anlaşmalarını yönetmeye yardımcı İş Ortağı Merkezi.

|**Bunu yapmak için**   |**Bunu okuyun**   |
|-----------------------|:-----------------------|
|Ortak satış fırsatları sayfasındaki sekmeleri ve gezintiyi anlama|[Ortak satış bölümünde gezinme](./manage-co-sell-opportunities.md#navigating-the-co-sell-section)|
|D&B listesinden bir müşteri kuruluşu seçme |[Müşterinizi seçin](./manage-co-sell-opportunities.md#select-your-customer)|
|Anlaşma ayrıntıları bölümündeki alanları değiştirme|[Anlaşma ayrıntıları](./manage-co-sell-opportunities.md#deal-details)|
|Anlaşma ekibine takım üyelerinizi ekleme|[Çalışanlarınızı ekleme](./manage-co-sell-opportunities.md#add-team-members)|
|Ortak satış anlaşmasına yanıt verme|[Ortak satış anlaşmalarını yönetme](./manage-co-sell-opportunities.md#responding-to-a-co-sell-opportunity)
|İş Ortağı Merkezi'de kazandnız anlaşmaları İş Ortağı Merkezi |[Yeni bir anlaşma kaydetme](./register-deals.md)
|Referans içgörüleri alın ve referansların nasıl olduğunu öğrenin |[Referans içgörüleri](./referral-insights.md)
|İş profili oluşturma ve yönetme|[İş profilini yönetme](./create-a-marketing-profile.md)
|İş profiliniz için müşteri adaylarını yönetme |[Müşteri adaylarını yönetme](./manage-leads.md)|

## <a name="next-steps"></a>Sonraki adımlar


- [İş Ortağı Bağlan İş Ortağı Merkezi](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) çalışma kitabı - İş Ortağı Merkezi ve İş Ortağı Satışları karşılaştırması aracılığıyla iş ortaklarının satış işlemlerini ve rollerini yeni satış süreçleriyle hizalamak için Bağlan.
- [İş Ortağı Merkezi ortak satış](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) çalışma kılavuzu - müşteri adaylarını veya ortak satış fırsatlarını yönetmeye ve anlaşmaları kaydetmeye İş Ortağı Merkezi aracılığıyla bir operasyon modelini belirlemeye yönelik kılavuz.
- [Referans yönetimi destesi](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) - Müşteri adaylarını ve ortak satış fırsatlarını yönetmek için adım adım talimatlar görselleştirilmiş İş Ortağı Merkezi.
- [Ticari markette yayımlama](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) ve yönetme : Ticari markette teklif oluşturma, yönetme ve yayımlamaya yönelik İş Ortağı Merkezi adım adım talimatlar.
