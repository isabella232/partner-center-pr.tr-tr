---
title: IOT İş Ortakları için Bağlan Satış Temsilcisinden (PSC) geçiş
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: Microsoft IOT iş ortaklarının İş Ortağı Satış Hizmetleri'nden (PSC) Bağlan satış anlaşması İş Ortağı Merkezi satış anlaşması oluşturma veya yönetmeye nasıl yardımcı olduğunu öğrenin.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/07/2021
ms.openlocfilehash: 1850ffe388349cdb7e4c685e5db0004d74735e80
ms.sourcegitcommit: 90bf27df911b428b1222f483c32ba6367870e7c5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/04/2021
ms.locfileid: "115101659"
---
# <a name="guide-to-create-and-manage-iot-deals-in-partner-center-pc-for-iot-partners-migrating-from-partner-sales-connect-psc"></a>İş Ortağı Satış anlaşmasından (PSC) İş Ortağı Merkezi IOT iş ortakları için IOT anlaşmaları oluşturma ve yönetme Bağlan kılavuzu

**Uygun roller:** Hesap yöneticisi | Referans yöneticisi | İş Ortağı Bağlan (PSC) satıcısı | İş Ortağı Bağlan (PSC) yönetici | İş Ortağı Bağlan (PSC) anlaşma yöneticisi

Bu makale, iş ortağı satış anlaşmaları oluşturma ve yönetmeye devam etmek için İş Ortağı Satışları Bağlan'den (PSC) İş Ortağı Merkezi'a (PC) İş Ortağı Merkezi.

>[!Note]
> Bu kılavuz yalnızca **anlaşmalarını PSC'de yöneten IOT** iş ortakları için geçerlidir.

>[!Important]
> 15 Ağustos 2021'den itibaren, şirketiniz PSC'de anlaşma oluşturabilecek veya anlaşmaları düzenleyemez. **PSC'de toplu dışarı aktarma özelliğini kullanarak mevcut anlaşma verilerini indirmeye devam edersiniz. Açık anlaşmaları [psC'den](partner-sales-connect-to-partner-center-iot.md#psc-deals-migration) bu tarihten sonra İş Ortağı Merkezi da geçirilir.**

Bildiğiniz gibi, **şirketiniz 30 Ağustos 2021'den sonra PSC'ye erişimi kaybeder.** Ancak anlaşma oluşturma ve yönetme gibi tüm İş Ortağı Merkezi yine de bulabilirsiniz.

Ancak farklar da vardır. Aşağıdaki kılavuz, geçiş sürecinizin daha sorunsuz ve İş Ortağı Merkezi yardımcı olabilir.

## <a name="before-you-move-things-you-need-to-know"></a>Taşımadan önce, bilmek gerekenler

### <a name="if-you-are-a-psc-admin"></a>PSC yöneticisiyseniz

- İş Ortağı Merkezi'da oturum a almak için bir [iş e-postası gerekir.](https://partner.microsoft.com/)
- Hesap yöneticisinin yardımıyla İş Ortağı Merkezi [ayarlayın.](permissions-overview.md)
- Bu belgeyi okuyarak IOT anlaşmalarını İş Ortağı Merkezi yönetmeyi öğrenin.
- Tüm PSC kullanıcılarınız (İş Ortağı Merkezi, Satış yöneticisi ve Satıcı rolleri) için bir hesapta kullanıcı hesapları ayarlayın ve bu kullanıcılara referans yöneticisi veya referans [kullanıcı rolleri atfı gerçekleştirin.](permissions-overview.md)

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>PSC satış yöneticisi veya satıcıysanız

- Panoda oturum alasınız için bir iş e-İş Ortağı Merkezi [gerekir.](https://partner.microsoft.com/dashboard)
- PSC'de iş dışı bir hesap kullanıyorsanız veya iş e-postanız iş ortağı şirketten farklı bir şirkete yönelikse, hesap ayarlama yardımı için PSC yöneticinize ulaşın.
- PSC'de oturum a İş Ortağı Merkezi hesap ne olursa olsun, hesap ayarlama işleminin tamam olup İş Ortağı Merkezi PSC yöneticinize sorun.
- İş Ortağı Merkezi ve Referanslar bölümüne erişiminiz olduğunu doğrulayın.
- İş akışlarını ve iş akışlarında yapılan değişiklikleri anlamak için bu İş Ortağı Merkezi.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>PSC'de yönetici olarak sonraki adımlarınız bunlardır

Sol İş Ortağı Merkezi menüsünden Referanslar **seçeneğini** belirleyin. Ortak satış fırsatları sayfasına erişebilirsiniz.

  >[!Note]
  > Referanslar sayfalarına erişmek İş Ortağı Merkezi kimlik bilgilerinizi yenilemek için oturum açmanız ve oturum açmanız gerekebilirsiniz.

İş Ortağı Merkezi menüsünde veya Referanslarla ilgili sayfalarda Referanslar seçeneğini görmüyorsanız, şirketin hesap yöneticisine [](permissions-overview.md) başvurarak Referanslar seçeneğine ve  ilgili alana erişmenizi ister. 

Şirketinizin hesap yöneticisini bulmak için:

1. Panonun **sağ** üst köşesindeki dişli simgesinden Hesap ayarları'İş Ortağı Merkezi seçin.

1. İkinci **düzey,** sol gezinti menüsünden Kullanıcı yönetimi'ni seçin.

1. Kullanıcı listesinin üst kısmında Filtre **açılan** menüsünü seçin. Seçeneğini Hesap yöneticisi **olarak değiştirme.**

   Sayfada ilgili e-posta adresleriyle birlikte tüm hesap yöneticileri görüntülenir. Bunlardan birini e-postayla gönderin ve iş hesabınız için referans yöneticisi rolünü atamasını sorun.

  :::image type="content" source="images/pscmigration/account-admin.gif" alt-text="İş ortağı ayarları kullanıcı yönetimi sayfasında hesap yöneticilerini gösteren resim.":::

>[!Important]
>- Rolünüz yalnızca PSC'de kullanıcıları yönetmeyi içeriyorsa, şirketinizin hesap [](permissions-overview.md#manage-mpn-membership-and-your-company) yöneticisinin size şirket ilkesine göre İş Ortağı Merkezi yönetici rolünü atamasını sorun.
>- Rolünüz iot anlaşmalarını yönetmeyi de içerirse, referans yöneticisine veya referans kullanıcı rolüne uygun [şekilde atanmalarını](permissions-overview.md#manage-referrals) iste.
> - PSC yöneticileri arasında bir değişiklik yönetimi adayı da göstermeniz iyi bir fikirdir. Bunu yapmak, tüm PSC yöneticilerinin hesap yöneticilerine tek tek İş Ortağı Merkezi engel olur. Bunun yerine değişiklik yönetimi müşteri adayı, hesap yöneticisiyle İş Ortağı Merkezi kişi olabilir.

## <a name="user-migration"></a>Kullanıcı geçişi

Şirket içinde hesabınız İş Ortağı Merkezi, ortak satış fırsatları sayfasındaki kullanıcı geçiş sihirbazını kullanarak şirket çalışanlarınıza İş Ortağı Merkezi rollerini otomatik olarak atfın.

>[!Note]
> Kullanıcı geçişi yalnızca şirketinizin [hesap yöneticileri](permissions-overview.md#manage-mpn-membership-and-your-company) tarafından yapılabilir. Hesap yöneticisi rolüne sahip değilseniz, kullanıcı geçiş sihirbazının yardımıyla kullanıcı hesaplarını ayarlamaya yardımcı olacak bir hesap yöneticisi bulun.

:::image type="content" source="images/pscmigration/user-migration.gif" alt-text="Kullanıcı geçiş sihirbazını gösteren görüntü.":::

Hesap yöneticileri, referans kılavuzunun yanındaki ortak satış fırsatları sayfasında psC kullanıcı geçiş sihirbazı bağlantısını görebilir. Bağlantıyı seçerek kullanıcı geçişini başlatabilirsiniz. Yöneticiler, kullanıcı geçişini başlatmak için bağlantıyı seçin. Bu kullanıcı geçişi adımını, tüm kullanıcılara rol atamadan önce birden çok kez İş Ortağı Merkezi.

Kullanıcı geçiş tablosunda aşağıdaki ayrıntılar yer alır:

- Kullanıcı hesabı - Çalışanın e-posta kimliği
- PSC iş ortağı hesabı - Çalışanın PSC'de ilişkili olduğu hesap
- PSC kullanıcı rolü - PSC'de atanan üç rolden biri.
- PC MPN konumu - Kullanıcıya uygun rol (PC) İş Ortağı Merkezi verilecek konum. PSC iş ortağı hesabı MPN'i, izin atamak için İş Ortağı Merkezi MPN konumunu bulmak için kullanılır. Kuruluşun tamamı vOrg MPN kimliğini ifade ediyor.
- BILGISAYAR kullanıcı rolü - Çalışanlara PSC kullanıcı rollerine göre roller atanır. PSC'de yöneticiye, yönetici rolünde Referans yöneticisi İş Ortağı Merkezi. Satışcıya kaynaklarda referans kullanıcı rolü İş Ortağı Merkezi. Bu rollerle ilgili İş Ortağı Merkezi ve bu rollere sahip kullanıcıların bu rollerle neler İş Ortağı Merkezi [buradan öğrenebilirsiniz](permissions-overview.md#manage-referrals)
- PC AAD Kiracısı - Microsoft Azure Active Directory 'de kullanıcıların atandığı kiracı (Azure AD) İş Ortağı Merkezi
- Durum - Geçişin durumu için üç olası durum vardır
    - **Geçirilmez** - Kullanıcıya herhangi bir İş Ortağı Merkezi referans rolü atanmamış
    - **Geçirildi** - Kullanıcı tabloda gösterildiği gibi ilgili rol atanmış şekilde başarıyla geçirildi
    - **Hata** - Bazı hata nedeniyle geçiş tamamlanmadı

Bazen geçiş başarısız olabilir ve hatalara neden olabilir. Geçişin hataya neden olabileceğinin birkaç nedeni ve sorunu çözmenin bazı yolları:

1. PSC kullanıcıları iş dışı bir hesap kullanıyor olabilir.

2. PSC kullanıcısı, etki alanındaki hesaplardan farklı bir hesap kullanıyor olabilir ve İş Ortağı Merkezi.

   1. ve 2. senaryolarla ilgili hataları çözmek için kullanıcıdan Azure AD kiracınıza İş Ortağı Merkezi iş hesabını kullanarak oturum açmasını sorun. Genel [yöneticiniz yardımcı](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) olabilir.
   
   Genel yöneticinizi bulmak için: 
   1. Panoda İş Ortağı Merkezi [ve](https://partner.microsoft.com/dashboard) sağ **üst köşesindeki** dişli simgesinden Hesap ayarları'ı seçin.
   2. İkinci **düzey,** sol gezinti çubuğundan Kullanıcı yönetimi'ni seçin.
   3. Kullanıcı listesinin üst kısmında Filtre  açılan menüsünü seçin ve seçeneğini Genel yönetici **olarak belirleyin.** Ardından sayfada ilgili e-posta adresleriyle birlikte tüm genel yöneticiler görüntülenir. İş hesabınız için referans yöneticisi rolünü atamasını istemek için bunlardan birini sorun.
   
      Genel yönetici, Azure AD kiracınız içinde yeni bir kullanıcı hesabı oluşturabilir veya diğer etki alanı hesabı kullanıcılarına konuk kullanıcı erişimi atayabilirsiniz. Tüm PSC anlaşma yöneticileri ve kullanıcıları için hesaplar ayarlanmaz, İş Ortağı Merkezi'da oturum açmaları, sol gezinti menüsünden Referanslar'ı seçmeleri ve Referanslar sayfasını görene kadar onayları gerekir. 

3. Kullanıcının zaten bu rolde atanmış bir referans İş Ortağı Merkezi.
    - Kullanıcının mevcut rolünü doğrularsanız. Uygulamanın sağ üst köşesinde, İş Ortağı Merkezi **(dişli simgesi) Ayarlar'ı** ve ardından Hesap **ayarları'ı seçin.** İkinci bir sol gezinti menüsü gördüğünüzde Kullanıcı **yönetimi'ni seçin** ve kullanıcı için arama yapabilirsiniz.

## <a name="psc-deals-migration"></a>PSC Anlaşmaları geçişi

Kullanıcı geçişini tamamlandıktan sonra ortak satış fırsatları sayfasındaki satış anlaşmaları geçiş sihirbazını kullanarak PSC'den tüm uygun açık anlaşmaları İş Ortağı Merkezi. **Anlaşmalar geçiş bağlantısı yalnızca tüm kuruluş kapsamına sahip referans yöneticileri tarafından İş Ortağı Merkezi.** Ortak satış fırsatları sayfasının sağ üst kısmında **"PSC anlaşmaları geçişi"** adlı bir bağlantı olacak ve bu bağlantı satış anlaşması geçiş sihirbazını açacaktır.

Anlaşma geçişini başlatmadan önce bu bölümü okuyun.

**Geçiş için uygun**

PsC'den İş Ortağı Merkezi'a geçiş için yalnızca bazı anlaşmalar İş Ortağı Merkezi. Bu geçiş sihirbazı, iş ortaklarının anlaşmalarını anlaşmaları İş Ortağı Merkezi müşterileri ile etkin bir şekilde çalışarak anlaşmaları kapatmalarına yardımcı olmak için oluşturulur. **Yalnızca geçerli iş ortağı hesabı ayrıntılarıyla (geçerli MPN Kimliği) 1 Ocak 2020'den itibaren oluşturulan açık durumdaki anlaşmalar geçiş için uygundur.**

## <a name="pre-requisites-for-deal-migration"></a>Anlaşma geçişi için önkullar

İş Ortağı Merkezi'den anlaşma geçişini başlatmadan önce, başarılı bir geçiş için PSC'de anlaşmaları ayarlamak için aşağıdaki yönergeleri izleyin.

- Şirketinizin açık anlaşmalar üzerinde çalışan tüm satış ekibi üyeleri bu geçiş hakkında bilgi sahibidir.
- Satış ekibi üyeleri, anlaşma yönetimi için İş Ortağı Merkezi üzere eğitildi.
- Anlaşmalar, aşağıda açıklandığı gibi tüm gerekli bilgileri içerir.
    - Ad ve adres de dahil olmak üzere müşteri şirketi ayrıntıları
    - En az bir çözüm
    - Tüm ayrıntıları içeren en az bir takım üyesi-ad, soyadı, e-posta KIMLIĞI ve telefon numarası
    - Anlaşma değeri
    - Tahmini anlaşma kapanış tarihi
    - İş ortağı notları

Tüm uygun anlaşmalar için anlaşmayla ilgili tüm eksik ayrıntıları eklemek üzere PSC 'deki toplu indirme ve karşıya yükleme yeteneklerini kullanabilirsiniz.

>[!Note]
> Yukarıdaki ön koşullar karşılanmadığında bile dağıtım geçişi başarılı olur. Ancak, Iş Ortağı Merkezi 'nde yukarıda bahsedilen gerekli alanlardan herhangi biri kullanılabilir değilse, anlaşma durumunu değiştiremezsiniz. Daha sonra, Iş ortağı merkezindeki anlaşmalar üzerinde çalışmaya başlamak için gerekli tüm bilgileri girmeniz gerekir. **Iş Ortağı Merkezi 'ne geçirmeden önce PSC 'deki uygun anlaşmaları temizlemeniz önemle tavsiye edilir.**

Iş Ortağı Merkezi ' nde anlaşma geçişi tek tıklamayla deneyim olarak oluşturulmuştur. Tüm yapmanız gereken, şirketiniz uygun anlaşmaları geçirmeye hazırsa **"anlaşmaları geçir"** düğmesine tıklayın. **PSC 'den geçiş yapmak istediğiniz anlaşmaları seçemezsiniz. Iş Ortağı Merkezi 'ne herhangi bir anlaşmayla geçiş yapmak istemiyorsanız, Geçişe başlamadan önce onları PSC 'de Kapalı durumuna taşıyın.**

>[!Note]
> Geçişi başlattıktan sonra, **yapılan anlaşmalar için 24 saate kadar sürebilir**.

Geçiş tamamlandıktan sonra, başlık iletisinin durumu geçiş raporuna yönelik bir bağlantıyla tamamlandı olarak değiştirilir. PSC 'den Iş Ortağı Merkezi 'ne geçirilen anlaşmalar hakkındaki ayrıntıları görüntülemek için raporu indirin.

Rapor aşağıdaki ayrıntıları içerir.

- **Iş Ortağı Merkezi KATıLıM kimliği** -bir görevlendirmede tüm anlaşmalar Için Iş ortağı merkezindeki benzersiz tanımlayıcı. İş ortağı için iki adet anlaşmalar vardır ve bir iş ortağı merkezi 'nde ortak satış katılımında Microsoft için bir görevlendirme vardır.
- **Iş ortağı merkezi başvuru kimliği** -iş ortağına ait olan Işlem Için Iş Ortağı Merkezi 'nde benzersiz tanımlayıcı.
- **Anlaşma adı** -PSC 'de ele verilen tanımlayıcı.
- **PSC anlaşma kimliği** -anlaşma için PSC içindeki benzersiz tanımlayıcı.
- **Hatalar** -belirli bir anlaşmayı geçirirken herhangi bir hata olup olmadığını gösterir.

Başarılı bir şekilde geçirilmiş tüm anlaşmalar PSC içinde görünür olmayacaktır. İş Ortağı Merkezi 'nde geçirilmiş anlaşmalar üzerinde çalışmaya devam edebilirsiniz.

PSC 'den geçirilen anlaşmalar, ortak satış fırsatları sayfasının giden sekmesinde kullanılabilir. Tüm anlaşmalar Iş ortağı tarafından ele alınır. Bunlar Microsoft satıcıları tarafından görülebilir.

>[!Important]
> Bazı anlaşmalar geçirilmemiş olması nedeniyle herhangi bir hata oluşursa, **"anlaşmaları geçir" düğmesine tıklayarak anlaşma geçişini yeniden başlatabilirsiniz**. Yalnızca bazı uygun anlaşmalar varsa etkinleştirilecek. Bu Ayrıca, anlaşma geçişi başlatıldıktan sonra bazı yeni anlaşmalar için PSC 'de oluşturulan geçiş aşamasındaysanız de yararlı olacaktır.

Tüm anlaşmalar başarıyla geçirildikten sonra, " **anlaşmaları geçir** " düğmesi **devre dışı** olarak **"geçirilecek anlaşmalar yok** " adlı başlık görüntülenir.

## <a name="next-steps"></a>Sonraki adımlar

Iş Ortağı Merkezi 'nde ıOT anlaşmaları oluşturmayı ve yönetmeyi öğrenin.
Bu önemli bir adımdır ve Iş Ortağı Merkezi 'nde ıOT anlaşma yönetimi için hazırlanmanıza yardımcı olur. Anlaşmaları etkin bir şekilde oluşturup yönetebilmeniz için iş akışlarını ve iş ortağı merkezindeki değişiklikleri anlayın. Bu belgeyi tamamen okuyarak başlayın.

## <a name="differences-between-psc-and-pc-workflows"></a>PSC ve PC iş akışları arasındaki farklılıklar

|**Senaryo**|**iş ortağı satışları Bağlan**|**İş Ortağı Merkezi**|
|-----|:-----|:-----|
|Kullanıcı rolleri|PSC 'in yönetici, anlaşma Yöneticisi ve satıcı rolleri vardır.|İş Ortağı Merkezi, [Referans Yöneticisi ve](permissions-overview.md#manage-referrals) konum kapsamına bağlı olarak hem okuma hem de yazma izni veren kullanıcı rollerini içerir.|
|Microsoft satıcı ayrıntıları|Bir anlaşma oluşturulduktan hemen sonra görünür.|Anlaşma türü iş ortağı olarak olduğu için Microsoft satıcı ayrıntıları iş ortakları tarafından görülemez.
|Çözümler|Anlaşma için herhangi bir sayıda çözüm eklenebilir.|İş ortağı, en fazla 50 çözümü ele ekleyebilir.
|Anlaşma ataması|Yalnızca atanan satıcı, anlaşmaları görüntüleyebilir ve üzerinde işlem yapabilir.|Bir anlaşmayı takım bölümüne eklenen başvuru kullanıcıları, anlaşmayı görüntüleyebilir ve üzerinde işlem yapabilir. Çalışma 'nin oluşturulduğu MPN konumu için başvuru yöneticileri, anlaşmayı görüntüleyebilir ve üzerinde işlem yapabilir.|
|Müşteri kuruluşu|Serbest form metin girişi.|Yalnızca birkaç karakter yazarak [Müşteri kuruluşunda](manage-co-sell-opportunities.md#select-your-customer) [D&B veritabanına](https://www.dnb.com/) göre arama yapabilirsiniz. Yasal ad ve adres seçime göre otomatik olarak doldurulur.|

## <a name="moving-from-psc-to-pc---faq"></a>PSC 'den PC 'ye geçme-SSS

Aşağıdaki bölümlerde geçişle ilgili sık sorulan sorular yanıtlanacaktır.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1-Iş Ortağı Merkezi 'ne erişimi yoksa ne yapmam gerekir?

Atanan rolleri almak için, "erişim yok" sayfasında listelenen yöneticilerinize başvurabilirsiniz. Başvurular bölümünde okuma ve yazma izni için [başvuru Yöneticisi](permissions-overview.md#manage-referrals) rolüne ihtiyacınız olacak. Yalnızca iş profillerini yönetiyorsanız iş profili yönetici rolüne iş ortağı Merkezi ' nde ihtiyacınız olacaktır.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Iş Ortağı Merkezi 'nde erişim deneyimi olmadığını gösteren resim.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2-Who iş ortağı merkezi 'ndeki referanslar bölümüne erişim izni verebilir mi?

[Hesap yöneticiniz](permissions-overview.md#manage-mpn-membership-and-your-company) , başvurular sekmesine erişim izni verebilir. Hesap yöneticinize ulaşmak için, Iş Ortağı Merkezi [panosunun](https://partner.microsoft.com/dashboard)sağ üst tarafındaki dişli simgesinden **Hesap ayarları** ' nı seçin. Ardından, ikinci düzey, sol gezinti çubuğundan **Kullanıcı yönetimi** ' ni seçin. Kullanıcı listesinin en üstünde, **filtre** açılan menüsünü seçin ve **Hesap Yöneticisi** seçeneğini belirleyin. Bu sayfada, tüm hesap yöneticileri ilgili e-posta adresleriyle görüntülenir. İş hesabınız için bir başvuru Yöneticisi rolü atamasını isteyin.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3-hesabım için + yeni anlaşma düğmesi gri değildir. Anlaşmalar oluşturmaya başlamak için ne yapmam gerekir?

Bu yalnızca hesabınızla ilişkilendirilen MPN KIMLIĞI, ıOT anlaşmaları oluşturmak için etkinleştirilmemişse gerçekleşir. Eğitim oturumlarında sağlanan e-postadaki ıOT iş ekibine başvurun veya MPN KIMLIĞINIZI ıOT anlaşmaları için etkin bir şekilde sağlamak üzere bir destek bileti oluşturun. "

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4-belirli bir kişiye, PSC gibi kuruluşumuza yönelik anlaşmalar atayabilir miyim?

Takım üyelerini belirli bir anlaşmayı atayabilirsiniz. Diğer başvuru yöneticilerinin bu anlaşmaları görüntülemesini veya bu anlaşmalar üzerinde hareket etmalarını engellemez.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5-bana atanan tüm anlaşmalar için bir görünüm var mı?

Kullanıcı düzeyi sekmesi olan Sık Kullanılanlar özelliğini kullanabilirsiniz. Bu anlaşmalar için hızlı bir erişim sağlamak üzere size atanan tüm anlaşmaları sık kullanılanlar olarak işaretleyebilirsiniz.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6-anlaşmalar için salt okunurdur bir görünüm var mı?

Hayır, başvurular bölümünde anlaşmalar için salt okuma görünümü yoktur.

### <a name="7---is-adding-a-customer-organization-mandatory"></a>7-bir müşteri kuruluşu zorunlu mi ekliyor?

Evet, [Müşteri kuruluşu](./manage-co-sell-opportunities.md#select-your-customer) eklemek Iş Ortağı Merkezi 'nde zorunludur. İlk olarak, müşterinin konumun bulunduğu konumu arayarak başlayın. Sahip olduğunuz ayrıntılara göre; tam yapı adı da dahil olmak üzere belirli ayrıntıları ekleyebilir veya yalnızca şehir ayrıntıları verebilirsiniz. Kuruluş araması, girdiğiniz adla eşleşen tüm yasal varlıkları getirecek, böylece herhangi bir adres ayrıntısı girmenize gerek kalmaz. Tüm ayrıntılar, seçilen kuruluşa göre otomatik olarak doldurulur.

### <a name="8---are-customer-contact-details-mandatory"></a>8-müşteri iletişim ayrıntıları zorunludur mi?

Evet, müşteri iletişim ayrıntıları ıOT anlaşmaları oluşturmak için zorunludur.

### <a name="9---how-many-solutions-can-i-add-to-a-deal"></a>9-bir dağıtmaya kaç çözüm ekleyebilirim?

En fazla 50 çözüm ekleyebilirsiniz (PSC 'de ' Ürünler ' öğesine benzer), bir anlaşma. Çözümler için hem miktar hem de tahmini kapanış tarihi zorunludur ve çözüm ayrıntıları bölümünde tahmini kapanış tarihi, tahmini kapanış tarihinden önce olmalıdır.

### <a name="10---where-can-i-find-the-opportunity-id"></a>10-fırsat KIMLIĞINI nerede bulabilirim?

PSC 'deki fırsat KIMLIĞI, Iş Ortağı Merkezi 'ndeki referans KIMLIĞIYLE aynıdır. Herhangi bir anlaşmayı açtığınızda anlaşma adının yanına başvuru KIMLIĞINI bulabilirsiniz.
