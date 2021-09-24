---
title: ıot iş ortakları için iş ortağı Sales Bağlan (PSC) geçişi
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: Microsoft ıot iş ortaklarının iş ortağı Bağlan satışlarından (PSC) iş ortağı merkezi 'ne nasıl geçirebileceğini ve anlaşmalar oluşturma veya yönetme hakkında bilgi edinin.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/07/2021
ms.openlocfilehash: 2b05046118c83c0d398272da68054a8a0c9c48e4
ms.sourcegitcommit: fb9ca808f6362e81d65a6ba5770dc8820834a0ed
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/24/2021
ms.locfileid: "128360211"
---
# <a name="guide-to-create-and-manage-iot-deals-in-partner-center-pc-for-iot-partners-migrating-from-partner-sales-connect-psc"></a>iş ortağı Sales Bağlan (PSC) geçiş iş ortakları için iş ortağı merkezi 'nde (PC) ıot anlaşmaları oluşturma ve yönetme kılavuzu

**Uygun roller**: Hesap Yöneticisi | Başvuru Yöneticisi | iş ortağı satışları Bağlan (PSC) satıcı | iş ortağı satışları Bağlan (PSC) yöneticisi | iş ortağı Sales Bağlan (PSC) anlaşma yöneticisi

bu makale, iş ortağı merkezi 'nde anlaşmalar oluşturmaya ve yönetmeye devam edebilmeleri için ortak satış Bağlan (PSC) tarafından iş ortağı merkezi 'ne (PC) geçiş yapmak üzere ıot iş ortakları için rehberlik sağlar.

>[!Note]
> Bu kılavuz yalnızca PSC 'de anlaşmalar yöneten **IoT iş ortakları için geçerlidir** .

>[!Important]
> 15 Ağustos 'Tan itibaren 2021, şirketinizin PSC 'de anlaşmalar oluşturamayacak veya düzenleyemeyecek. **Aynı zamanda PSC içindeki toplu dışa aktarma özelliğini kullanarak mevcut anlaşmalar verilerini indirebilirsiniz. Ayrıca, bu tarihten sonra PSC 'den Iş Ortağı Merkezi 'ne [Açık anlaşmalar geçirebilirsiniz](partner-sales-connect-to-partner-center-iot.md#psc-deals-migration) .**

Bildiğiniz gibi şirketiniz, **30 ağustos 2021 ' den sonra PSC 'ye erişimi kaybedecektir**. Ancak, Iş Ortağı Merkezi 'nde yapmak istediğiniz her şeyi (örneğin, anlaşmalar oluşturma ve yönetme) de bulabilirsiniz.

Ancak farklılıklar olacaktır. Aşağıdaki kılavuz, Iş Ortağı Merkezi 'ne geçişinizi daha sorunsuz ve daha basit hale getirmenize yardımcı olabilir.

## <a name="before-you-move-things-you-need-to-know"></a>Taşımadan önce bilmeniz gereken şeyler

### <a name="if-you-are-a-psc-admin"></a>Bir PSC yöneticisiyseniz

- İş [Ortağı Merkezi](https://partner.microsoft.com/)'nde oturum açmak için bir iş e-postasına ihtiyacınız vardır.
- Iş Ortağı Merkezi [hesap yöneticisinin](permissions-overview.md)yardımıyla hesabınızı ayarlayın.
- Bu belgeyi okuyarak Iş Ortağı Merkezi 'nde ıOT anlaşmaları oluşturmayı ve yönetmeyi öğrenin.
- Tüm PSC kullanıcılarınız (yönetici, anlaşma Yöneticisi ve satıcı rolleri) için Iş Ortağı Merkezi 'nde Kullanıcı hesapları kurun ve bunlara [başvuru Yöneticisi veya başvuru Kullanıcı rolleri](permissions-overview.md)atayın.

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>Bir PSC anlaşma Yöneticisi veya satıcı

- İş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açmak için bir iş e-postasına ihtiyacınız vardır.
- PSC 'de iş dışı bir hesap kullanıyorsanız veya iş e-postanız iş ortağı şirketten farklı bir şirkette kullanılıyorsa, hesap kurulumu için PSC yöneticinizle iletişime geçin.
- PSC 'de oturum açmak için kullandığınız hesap ne olursa olsun, Iş ortağı merkezi hesap ayarlanmanız durumunda PSC yöneticinizle görüşün.
- Iş Ortağı Merkezi 'ne ve başvurular bölümüne erişiminiz olup olmadığını doğrulayın.
- İş akışlarını ve iş ortağı merkezindeki değişiklikleri anlamak için bu belgeyi okuyun.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>PSC 'de yönetici olarak, bunlar sonraki adımlardır

Iş ortağı merkezi sol gezinti menüsünde, **Başvurular** seçeneğini belirleyin. Ortak satış fırsatları sayfasına erişebildiğinizden emin olun.

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
>- Rolünüz yalnızca PSC 'deki kullanıcıları yönetmeyi içeriyorsa, şirketinizin hesap yöneticisinden şirketinizin ilkesi uyarınca Iş Ortağı Merkezi ' nde [Hesap Yöneticisi](permissions-overview.md#manage-mpn-membership-and-your-company) rolünü atamasını isteyin.
>- Rolünüz IoT anlaşmalar yönetimini de içeriyorsa, uygun şekilde [başvuru Yöneticisi veya başvurular Kullanıcı](permissions-overview.md#manage-referrals) rolü atanmasını isteyin.
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
- BILGISAYAR Kullanıcı rolü-çalışanlar, PSC Kullanıcı rollerine göre rollere atanır. PSC 'deki yöneticiye, Iş Ortağı Merkezi 'nde referanslar yönetici rolleri atanır. Satıcı, Iş Ortağı Merkezi 'nde başvuru Kullanıcı rolüne atanır. İş Ortağı Merkezi rolleri ve bu rollere sahip olan kullanıcıların, iş  [Ortağı Merkezi 'nde çalışması gereken bir şirketin kullanıcıları için Kullanıcı rolleri ve Izinleri atama](permissions-overview.md#manage-referrals)konusunda daha fazla bilgi edinin.
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
   1. Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard) oturum açın ve sağ üst köşedeki dişli simgesinden **Hesap ayarları** ' nı seçin.
   2. İkinci düzey, sol gezinti çubuğundan **Kullanıcı yönetimi** ' ni seçin.
   3. Kullanıcı listesinin en üstünde, **filtre** açılan menüsünü seçin ve seçeneğini **genel yönetici** olarak değiştirin. Daha sonra sayfa, tüm genel yöneticileri ilgili e-posta adresleriyle birlikte görüntüler. İş hesabınız için bir başvuru Yöneticisi rolü atamasını isteyin.
   
      Genel yönetici, Azure AD kiracınızda yeni bir kullanıcı hesabı oluşturabilir ya da diğer etki alanı hesabı kullanıcılarına Konuk Kullanıcı erişimi atayabilir. Tüm PSC anlaşma yöneticileri ve kullanıcıları için hesaplar kurulduktan sonra, Iş Ortağı Merkezi 'nde oturum açması, sol gezinti menüsünden **başvuruları** seçmeniz ve başvurular sayfasını görebilecekleri onaylanır.

3. Kullanıcının Iş Ortağı Merkezi 'ne atanmış bir başvuru rolü zaten var.
    - Kullanıcının var olan rolünü doğrulayabilirsiniz. iş ortağı merkezi 'nin sağ üst köşesinde **Ayarlar** (dişli simgesi) ve ardından **hesap ayarları**' nı seçin. İkinci bir sol gezinti menüsünü gördüğünüzde **Kullanıcı yönetimi** ' ni seçin ve Kullanıcı için arama yapın.

## <a name="psc-deals-migration"></a>PSC anlaşmalar geçişi

Kullanıcı geçişini tamamladıktan sonra, PSC 'den Iş Ortağı Merkezi 'ne uygun tüm açık anlaşmaları getirmek için ortak satış fırsatları sayfasında anlaşmalar Geçiş Sihirbazı 'nı kullanın. **Anlaşmalar geçiş bağlantısı yalnızca Iş Ortağı Merkezi 'ndeki tüm kuruluş kapsamına sahip başvuru yöneticileri için görünür olacaktır.** Ortak satış fırsatları sayfasının sağ üst kısmında **"PSC anlaşmaları geçişi"** adlı bir bağlantı olacak ve bu bağlantı satış anlaşması geçiş sihirbazını açacaktır.

Anlaşma geçişini başlatmadan önce bu bölümü okuyun.

**Geçişe uygun**

Yalnızca bazı anlaşmalar PSC 'den Iş Ortağı Merkezi 'ne geçişe uygundur. Bu Geçiş Sihirbazı, iş ortaklarının, BT 'nin müşterileri ile çalışmaya devam ettikleri Iş Ortağı Merkezi 'ne anlaşmalar getirmelerini sağlamak için oluşturulmuştur. **Yalnızca geçerli iş ortağı hesabı ayrıntıları (geçerli MPN ID) ile 1 Ocak 2020 ' den oluşturulan açık durumdaki anlaşmalar geçişe uygundur.**

## <a name="pre-requisites-for-deal-migration"></a>Anlaşma geçişi için önkoşulların önkoşulları

Iş Ortağı Merkezi 'nden anlaşma geçişini başlatmadan önce, başarılı bir geçiş için PSC 'deki anlaşmaları ayarlamak üzere aşağıdaki yönergeleri izleyin.

- Şirketinizde açık anlaşmalar üzerinde çalışan tüm satış ekibi üyeleri bu geçiş hakkında bilgi sahibi.
- Satış ekibi üyeleri, anlaşma yönetimi için Iş Ortağı Merkezi 'ni kullanmaya eğitim sağlar.
- Bu anlaşmalar, aşağıda açıklandığı gibi gerekli tüm bilgilere sahiptir.
    - Ad ve adres dahil müşteri Şirket ayrıntıları
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
