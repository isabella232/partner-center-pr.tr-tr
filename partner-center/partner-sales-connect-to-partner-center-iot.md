---
title: IOT İş Ortakları için Bağlan Satış Temsilcisinden (PSC) geçiş
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: Microsoft IOT iş ortaklarının İş Ortağı Satış hizmetleri'nden (PSC) Bağlan satış anlaşması İş Ortağı Merkezi satış anlaşması oluşturma veya yönetme hakkında bilgi.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/07/2021
ms.openlocfilehash: 2b05046118c83c0d398272da68054a8a0c9c48e4
ms.sourcegitcommit: 23ba623b50b06c866703fd876f1b40f3a49ce504
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/22/2021
ms.locfileid: "128074640"
---
# <a name="guide-to-create-and-manage-iot-deals-in-partner-center-pc-for-iot-partners-migrating-from-partner-sales-connect-psc"></a>İş Ortağı Satış anlaşmasından (PSC) geçen IOT iş ortakları için İş Ortağı Merkezi (PC) içinde IOT anlaşmaları oluşturma ve yönetme Bağlan kılavuzu

**Uygun roller:** Hesap yöneticisi | Referans yöneticisi | İş Ortağı Bağlan (PSC) satıcısı | İş Ortağı Bağlan (PSC) yönetici | İş Ortağı Bağlan (PSC) anlaşma yöneticisi

Bu makalede, iş ortağı satış anlaşmalarını oluşturma ve yönetmeye devam etmek için İş Ortağı Satışları Bağlan'den (PSC) İş Ortağı Merkezi'ye (PC) İş Ortağı Merkezi.

>[!Note]
> Bu kılavuz yalnızca **anlaşmalarını PSC'de yöneten IOT** iş ortakları için geçerlidir.

>[!Important]
> 15 Ağustos 2021'den itibaren, şirketiniz PSC'de anlaşma oluşturabilecek veya anlaşmaları düzenleyemez. **PSC'de toplu dışarı aktarma özelliğini kullanarak mevcut anlaşma verilerini indirmeye devam edersiniz. Açık anlaşmaları [PSC'den bu](partner-sales-connect-to-partner-center-iot.md#psc-deals-migration) tarihten sonra İş Ortağı Merkezi da geçirsiniz.**

Bildiğiniz gibi, **şirketiniz 30 Ağustos 2021'den sonra PSC'ye erişimi kaybeder.** Ancak anlaşma oluşturma ve yönetme gibi tüm İş Ortağı Merkezi yine de bulabilirsiniz.

Ancak farklar da vardır. Aşağıdaki kılavuz, geçiş sürecinizin daha sorunsuz ve İş Ortağı Merkezi yardımcı olabilir.

## <a name="before-you-move-things-you-need-to-know"></a>Taşımadan önce, bilmek gerekenler

### <a name="if-you-are-a-psc-admin"></a>PSC yöneticisiyseniz

- İş Ortağı Merkezi.'de oturum a açması için bir [iş e-postası gerekir.](https://partner.microsoft.com/)
- Hesap yöneticisinin yardımıyla İş Ortağı Merkezi [ayarlayın.](permissions-overview.md)
- Bu belgeyi okuyarak IOT anlaşmalarını İş Ortağı Merkezi yönetmeyi öğrenin.
- Tüm PSC kullanıcılarınız (İş Ortağı Merkezi, Satış yöneticisi ve Satıcı rolleri) için hesaplarda kullanıcı hesapları ayarlayın ve referans yöneticisi veya referans kullanıcı [rolleri atfı gerçekleştirin.](permissions-overview.md)

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>PSC satış yöneticisi veya satıcıysanız

- İş Ortağı Merkezi panosunda oturum a İş Ortağı Merkezi [gerekir.](https://partner.microsoft.com/dashboard)
- PSC'de iş dışı bir hesap kullanıyorsanız veya iş e-postanız iş ortağı şirketten farklı bir şirkete yönelikse, hesap ayarlama yardımı için PSC yöneticinize ulaşın.
- PSC'de oturum a İş Ortağı Merkezi hesap ne olursa olsun, hesap ayarlama işleminin tamam olup İş Ortağı Merkezi PSC yöneticinize sorun.
- İş Ortağı Merkezi ve Referanslar bölümüne erişiminizin olduğunu doğrulayın.
- İş akışlarını ve iş akışlarında yapılan değişiklikleri anlamak için bu İş Ortağı Merkezi.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>PSC'de yönetici olarak, sonraki adımlarınız bunlardır

Sol İş Ortağı Merkezi menüsünden Referanslar **seçeneğini** belirleyin. Ortak satış fırsatları sayfasına erişebilirsiniz.

  >[!Note]
  > Referanslar sayfalarına erişmek İş Ortağı Merkezi kimlik bilgilerinizi yenilemek için oturum açma ve oturum açma işlemlerinizi yeniden imzalamanız gerekir.

İş Ortağı Merkezi menüsünde veya Referanslarla ilgili sayfalarda Referanslar seçeneğini görmüyorsanız, şirketin hesap yöneticisine [](permissions-overview.md) başvurarak Referanslar seçeneğine ve  ilgili alana erişmenizi istemelerini sorun. 

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

Hesap yöneticileri, referans kılavuzunun yanındaki ortak satış fırsatları sayfasında psC kullanıcı geçiş sihirbazı bağlantısını görebilir. Bağlantıyı seçerek kullanıcı geçişini başlatabilirsiniz. Yöneticiler, kullanıcı geçişini başlatmak için bağlantıyı seçin. Bu kullanıcı geçişi adımını, tüm kullanıcılara rol atamaya uygun roller atanana kadar birden çok İş Ortağı Merkezi.

Kullanıcı geçiş tablosunda aşağıdaki ayrıntılar yer alır:

- Kullanıcı hesabı - Çalışanın e-posta kimliği
- PSC iş ortağı hesabı - Çalışanın PSC'de ilişkili olduğu hesap
- PSC kullanıcı rolü - PSC'de atanan üç rolden biri.
- PC MPN konumu - Kullanıcıya ilgili rol (PC) İş Ortağı Merkezi verilecek konum. PSC iş ortağı hesabı MPN'i, izin atamak için İş Ortağı Merkezi MPN konumunu bulmak için kullanılır. Kuruluşun tamamı vOrg MPN kimliğini ifade ediyor.
- BILGISAYAR kullanıcı rolü - Çalışanlara PSC kullanıcı rollerine göre roller atanır. PSC'de yöneticiye, yönetici rolünde Referans yöneticisi İş Ortağı Merkezi. Satıcıya kaynaklarda referans kullanıcı rolü İş Ortağı Merkezi. Şirket rollerini İş Ortağı Merkezi ve bu rollere sahip kullanıcıların neler yapaları hakkında daha fazla bilgi edinmek için Şu konuda daha fazla bilgi [İş Ortağı Merkezi.](permissions-overview.md#manage-referrals)
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
   1. Panoda oturum İş Ortağı Merkezi [sağ](https://partner.microsoft.com/dashboard) **üst köşesindeki** dişli simgesinden Hesap ayarları'ı seçin.
   2. İkinci **düzey,** sol gezinti çubuğundan Kullanıcı yönetimi'ni seçin.
   3. Kullanıcı listesinin üst kısmında Filtre  açılan menüsünü seçin ve seçeneğini Genel yönetici **olarak belirleyin.** Ardından sayfada ilgili e-posta adresleriyle birlikte tüm genel yöneticiler görüntülenir. İş hesabınız için referans yöneticisi rolünü atamasını istemek için bunlardan birini sorun.
   
      Genel yönetici, Azure AD kiracınız içinde yeni bir kullanıcı hesabı oluşturabilir veya diğer etki alanı hesabı kullanıcılarına konuk kullanıcı erişimi atayabilirsiniz. Tüm PSC anlaşma yöneticileri ve kullanıcıları için hesaplar ayarlanmaz, İş Ortağı Merkezi'da oturum açmaları, sol gezinti menüsünden Referanslar'ı seçmeleri ve Referanslar sayfasını görene kadar onayları gerekir. 

3. Kullanıcının zaten bu rolde atanmış bir referans İş Ortağı Merkezi.
    - Kullanıcının mevcut rolünü doğrularsanız. Uygulamanın sağ üst köşesinde, İş Ortağı Merkezi **(dişli simgesi) Ayarlar'yi** ve ardından Hesap **ayarları'ı seçin.** İkinci bir sol gezinti menüsü gördüğünüzde Kullanıcı **yönetimi'ni seçin** ve kullanıcı için arama yapabilirsiniz.

## <a name="psc-deals-migration"></a>PSC Anlaşmaları geçişi

Kullanıcı geçişini tamamlandıktan sonra, uygun tüm açık anlaşmaları PSC'den ortak satış fırsatlarına getirmek için ortak satış fırsatları sayfasındaki anlaşmalar geçiş sihirbazını İş Ortağı Merkezi. **Anlaşmalar geçiş bağlantısı yalnızca tüm kuruluş kapsamına sahip referans yöneticileri tarafından İş Ortağı Merkezi.** Ortak satış fırsatları sayfasının sağ üst kısmında **"PSC anlaşmaları geçişi"** adlı bir bağlantı olacak ve bu bağlantı satış anlaşması geçiş sihirbazını açacaktır.

Anlaşma geçişini başlatmadan önce bu bölümü okuyun.

**Geçiş için uygun**

Yalnızca bazı anlaşmalar PSC'den İş Ortağı Merkezi. Bu geçiş sihirbazı, iş ortaklarının anlaşmalarını anlaşmaları İş Ortağı Merkezi müşterileri ile etkin bir şekilde çalışarak anlaşmaları kapatmalarına yardımcı olmak için oluşturulur. **Yalnızca geçerli iş ortağı hesabı ayrıntılarıyla (geçerli MPN Kimliği) 1 Ocak 2020'den itibaren oluşturulan açık durumdaki anlaşmalar geçiş için uygundur.**

## <a name="pre-requisites-for-deal-migration"></a>Anlaşma geçişi için önkullar

İş Ortağı Merkezi'den anlaşma geçişini başlatmadan önce, başarılı bir geçiş için PSC'de anlaşmaları ayarlamak için aşağıdaki yönergeleri izleyin.

- Şirketinizin açık anlaşmalar üzerinde çalışan tüm satış ekibi üyeleri bu geçiş hakkında bilgi sahibidir.
- Satış ekibi üyeleri, anlaşma yönetimi için İş Ortağı Merkezi üzere eğitildi.
- Anlaşmalar, aşağıda açıklandığı gibi tüm gerekli bilgileri içerir.
    - Ad ve adres de dahil olmak üzere müşteri şirketi ayrıntıları
    - En az bir çözüm
    - Ad, soyadı, e-posta kimliği ve telefon numarası gibi tüm ayrıntıları içeren en az bir ekip üyesi
    - Anlaşma değeri
    - Tahmini satış kapanış tarihi
    - İş ortağı notları

PsC'de toplu indirme ve karşıya yükleme özelliklerini kullanarak tüm uygun anlaşmaların anlaşmada eksik olan tüm ayrıntılarını indirebilirsiniz.

>[!Note]
> Yukarıdaki önkullar karşılanmazsa bile anlaşma geçişi başarılı olur. Ancak, yukarıdaki belirtilen gerekli alanlardan herhangi biri kullanılabilir durumda değilse İş Ortağı Merkezi değiştiremezsiniz. Ardından, üzerinde çalışmaya başlamak için anlaşmalarda eksik olan tüm İş Ortağı Merkezi bilgileri girmeniz gerekir. **PsC'de uygun anlaşmaları, İş Ortağı Merkezi'a İş Ortağı Merkezi.**

Geçiş anlaşması İş Ortağı Merkezi tek tıklama deneyimi olarak yerleşiktir. Tek gereken, şirket uygun anlaşmaları geçirmek için hazır olduğunda **"Anlaşmaları geçir"** düğmesine tıklamaktır. **PSC'den geçirmek istediğiniz anlaşmaları seçesiniz. Geçişe herhangi bir anlaşma İş Ortağı Merkezi, geçişe başlamadan önce bunları PSC'de kapalı durumuna taşımanız gerekir.**

>[!Note]
> Geçiş başlatıldıktan sonra, **anlaşmaların geçişi 24 saat kadar sürebilir.**

Geçiş tamamlandıktan sonra başlık iletisi, geçiş raporunun bağlantısıyla tamamlanacak şekilde değişir. PSC'den İş Ortağı Merkezi'a geçirilen anlaşmaların ayrıntılarını görüntülemek için raporu İş Ortağı Merkezi.

Rapor aşağıdaki ayrıntıları içerir.

- **İş Ortağı Merkezi kimliği** - Bir etkileşimde İş Ortağı Merkezi anlaşmaların benzersiz tanımlayıcısı. İki satış anlaşması vardır: biri iş ortağı, biri de Microsoft için ortak satış anlaşmasında İş Ortağı Merkezi.
- **İş Ortağı Merkezi kimliği** - İş ortağına ait İş Ortağı Merkezi için geçerli olan benzersiz tanımlayıcı.
- **Anlaşma adı** - PSC'de anlaşmaya verilen tanımlayıcı.
- **PSC anlaşma kimliği** - Anlaşma için PSC'deki benzersiz tanımlayıcı.
- **Hatalar** - belirli bir anlaşmadan başka bir anlaşmayı alırken herhangi bir hata olup olamay olduğunu belirtmek için.

Başarıyla geçirilen tüm anlaşmalar PSC'de görünmez. Geçiş yapılan anlaşmalar üzerinde çalışmaya devam İş Ortağı Merkezi.

PSC'den geçirilen anlaşmalar Ortak satış fırsatları sayfasının Giden sekmesinde kullanılabilir. Tüm anlaşmalar İş ortağı tarafından yapılan anlaşmalar olarak oluşturulur. Bunlar Microsoft satıcılarının kullanımına açık.

>[!Important]
> Bazı anlaşmaların geçirilenemleri nedeniyle herhangi bir hata varsa, "Anlaşmaları geçir" düğmesine tıklayarak anlaşma **geçişini yeniden başlatabilirsiniz.** Yalnızca henüz geçirilemeyen bazı uygun anlaşmalar varsa etkinleştirilir. Bu, anlaşma geçişi başladıktan sonra PSC'de bazı yeni anlaşmaların oluşturulacak olduğu geçiş aşamasında da yararlı olacaktır.

Tüm anlaşmalar başarıyla geçirildiktan sonra , **"Anlaşmaları geçir"** düğmesinin devre dışı bırakıldığında "Geçirılacak anlaşma **yok"** ifadesini gösteren bir başlık **vardır.**

## <a name="next-steps"></a>Sonraki adımlar

IOT anlaşmaları oluşturma ve yönetme hakkında bilgi İş Ortağı Merkezi.
Bu önemli bir adımdır ve bu adım, IOT anlaşma yönetimi için hazırlık İş Ortağı Merkezi. Anlaşmaları etkili bir şekilde oluştur İş Ortağı Merkezi yönetebilirsiniz. Bu belgeyi tamamen okuyarak başlayabilirsiniz.

## <a name="differences-between-psc-and-pc-workflows"></a>PSC ile PC iş akışları arasındaki farklar

|**Senaryo**|**İş Ortağı Satış Bağlan**|**İş Ortağı Merkezi**|
|-----|:-----|:-----|
|Kullanıcı rolleri|PSC'de yönetici, satış anlaşması yöneticisi ve satıcı rolleri vardır.|İş Ortağı Merkezi, konum [kapsamına göre hem](permissions-overview.md#manage-referrals) okuma hem de yazma izni veren referans yöneticisi ve referans kullanıcı rollerine sahiptir.|
|Microsoft satıcı ayrıntıları|Anlaşma oluşturulur oluşturulmaz görünür.|Satış anlaşması türü iş ortağı tarafından yönlendirildiklarından Microsoft Satıcı ayrıntıları iş ortaklarının kullanımına açık değildir.
|Çözümler|Anlaşmaya herhangi bir sayıda çözüm eklenebilir.|İş ortağı anlaşmaya en fazla 50 çözüm ekleyebilir.
|Anlaşma ataması|Anlaşmaları yalnızca atanan satıcı görüntülemeli ve üzerinde eylemde davranabilir.|Bir anlaşmanın takıma eklenen referans kullanıcıları anlaşmayı görüntüp buna göre hareket ediyor olabilir. Anlaşmanın oluşturulacak MPN konumu için referans yöneticileri, anlaşmayı görüntüp üzerinde eylem gerçekleştirebilirsiniz.|
|Müşteri kuruluşu|Serbest biçimli metin girişi.|Yalnızca birkaç karakter [yazarak](manage-co-sell-opportunities.md#select-your-customer) [müşteri kuruluşunda D&B](https://www.dnb.com/) veritabanında arama edebilirsiniz. Yasal ad ve adres, seçime göre otomatik olarak doldurulur.|

## <a name="moving-from-psc-to-pc---faq"></a>PSC'den PC'ye Taşıma - SSS

Aşağıdaki bölümlerde geçişle ilgili sık sorulan sorular yanıtlanmaktadır.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1 - Erişim iznim yoksa ne İş Ortağı Merkezi?

Atanmış rolleri almak için "Erişim yok" sayfasında listelenen yöneticilerinize başvurabilirsiniz. Referanslar bölümünde [okuma ve](permissions-overview.md#manage-referrals) yazma izni için referans yöneticisi rolüne ihtiyacınız olacak. Yalnızca iş profillerini yönetiyorsanız, iş profili yöneticisi rolünüz İş Ortağı Merkezi.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Veri erişim yok deneyimini gösteren İş Ortağı Merkezi.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2 - Who bölümündeki Referanslar bölümüne erişim izni İş Ortağı Merkezi?

Hesap [yöneticiniz Referanslar](permissions-overview.md#manage-mpn-membership-and-your-company) sekmesine erişmenizi sağlar. Hesap yöneticinizi bulmak için **panonun** sağ üst köşesindeki dişli simgesinden Hesap ayarları'İş Ortağı Merkezi [seçin.](https://partner.microsoft.com/dashboard) Ardından, ikinci **düzey,** sol gezinti çubuğundan Kullanıcı yönetimi'ni seçin. Kullanıcı listesinin üst kısmında Filtre  açılan menüsünü seçin ve seçeneğini hesap yöneticisi **olarak belirleyin.** Sayfada ilgili e-posta adresleriyle birlikte tüm hesap yöneticileri görüntülenir. İş hesabınız için referans yöneticisi rolünü atamasını istemek için bunlardan birini sorun.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3 - Hesabımız için +yeni anlaşma düğmesi gridir. Anlaşma oluşturmaya başlamak için ne yapabilirim?

Bu yalnızca hesabınızla ilişkili MPN Kimliği IOT anlaşmaları oluşturmak için etkinleştirilmediyse gerçekleşir. Eğitim oturumları sırasında sağlanan e-postada IOT iş ekibine başvurun veya IOT anlaşmaları için MPN id'nizi etkinleştirecek bir destek bileti oluşturun."

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4 - PSC gibi kuruluştan belirli bir kişiye satış anlaşması atay musunuz?

Takım üyelerini belirli bir satış anlaşmasına at attayarak. Diğer referans yöneticilerinin bu anlaşmaları görüntülemesini veya bu anlaşmalara göre hareket etmelerini engellemez.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5 - Bana atanan tüm anlaşmaların bir görünümü var mı?

Kullanıcı düzeyinde bir sekme olan sık kullanılanlar özelliğini kullanabilirsiniz. Anlaşmalara hızlı erişim elde etmek için size sık kullanılanlar olarak atanan tüm anlaşmaları işaretlebilirsiniz.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6 - Anlaşmalar için salt okunur bir görünüm var mı?

Hayır, referanslar bölümünde anlaşmaların salt okunur bir görünümü yoktur.

### <a name="7---is-adding-a-customer-organization-mandatory"></a>7 - Müşteri kuruluşu eklemek zorunlu mu?

Evet, müşteri [kuruluşuna yeni](./manage-co-sell-opportunities.md#select-your-customer) bir kuruluş eklemek İş Ortağı Merkezi. İlk olarak müşterinin bulunduğu konumu arayarak başlayalım. Sahip olduğunuz ayrıntılara göre; Tam bina adı dahil olmak üzere belirli ayrıntıları ekleyebilir veya yalnızca şehir ayrıntılarını veabilirsiniz. Kuruluş araması, herhangi bir adres ayrıntısı girmek zorunda olmadığınız adla eşleşen tüm yasal varlıkları getirir. Tüm ayrıntılar seçilen kuruluşa göre otomatik olarak doldurulur.

### <a name="8---are-customer-contact-details-mandatory"></a>8 - Müşteri iletişim bilgileri zorunlu mu?

Evet, müşteri iletişim ayrıntıları IOT anlaşmaları oluşturmak için zorunludur.

### <a name="9---how-many-solutions-can-i-add-to-a-deal"></a>9 - Bir anlaşmaya kaç çözüm ekleyebilirim?

Bir satış anlaşmasına en fazla 50 çözüm (PSC'de 'ürünler' ile benzer) eklersiniz. Çözümler için hem miktar hem de tahmini kapanış tarihi zorunludur ve çözümlerin tahmini kapanış tarihi anlaşma ayrıntıları bölümündeki tahmini kapanış tarihinden daha erken olmalıdır.

### <a name="10---where-can-i-find-the-opportunity-id"></a>10 - Fırsat kimliğini nerede bulamıyorum?

PSC'deki Fırsat Kimliği, İş Ortağı Merkezi. Herhangi bir anlaşmayı a açmak için anlaşma adının yanında Referans Kimliğini bulabilirsiniz.
