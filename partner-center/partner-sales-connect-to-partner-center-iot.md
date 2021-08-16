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
ms.openlocfilehash: 4daf26a962d317da9eac3b2351f42c04546533d4
ms.sourcegitcommit: 815760499700bf2c947550524cbddd091622081f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "121914658"
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
    - Ad, soyadı, e-posta kimliği ve telefon numarası gibi tüm ayrıntıları içeren en az bir ekip üyesi
    - Anlaşma değeri
    - Tahmini satış kapanış tarihi
    - İş ortağı notları

PsC'de toplu indirme ve karşıya yükleme özelliklerini kullanarak tüm uygun anlaşmalara ilişkin eksik ayrıntıları anlaşmaya indirebilirsiniz.

>[!Note]
> Yukarıdaki önkullar karşılanmazsa bile anlaşma geçişi başarılı olur. Ancak, yukarıdaki belirtilen gerekli alanlardan herhangi biri kullanılabilir durumda yoksa İş Ortağı Merkezi değiştiremezsiniz. Ardından, üzerinde çalışmaya başlamak için anlaşmalarda eksik olan tüm İş Ortağı Merkezi bilgileri girmeniz gerekir. **Uygun anlaşmaları İş Ortağı Merkezi'a başlamadan önce PSC'de temizlemeniz önemle tavsiye İş Ortağı Merkezi.**

Geçiş anlaşması İş Ortağı Merkezi tek tıklama deneyimi olarak yerleşiktir. Tek ihtiyacınız olan, şirket uygun anlaşmaları geçirmek için hazır olduğunda **"Anlaşmaları geçir"** düğmesine tıklamaktır. **PSC'den geçirmek istediğiniz anlaşmaları seçesiniz. Anlaşmaları geçişe geçirmek istemiyorsanız İş Ortağı Merkezi başlamadan önce bunları PSC'de kapalı durumuna taşımanız gerekir.**

>[!Note]
> Geçiş başlatıldıktan sonra, **anlaşmaların geçişi 24 saat kadar sürebilir.**

Geçiş tamamlandıktan sonra başlık iletisi, geçiş raporunun bağlantısıyla tamamlanacak şekilde değişir. PSC'den İş Ortağı Merkezi'a geçirilen anlaşmaların ayrıntılarını görüntülemek için raporu İş Ortağı Merkezi.

Rapor aşağıdaki ayrıntıları içerir.

- **İş Ortağı Merkezi kimliği** - Bir etkileşimde İş Ortağı Merkezi anlaşmaların benzersiz tanımlayıcısı. İki satış anlaşması vardır: biri iş ortağı, biri de Microsoft için ortak satış anlaşmasında İş Ortağı Merkezi.
- **İş Ortağı Merkezi kimliği** - İş ortağına ait İş Ortağı Merkezi için geçerli olan benzersiz tanımlayıcı.
- **Anlaşma adı** - PSC'de anlaşmaya verilen tanımlayıcı.
- **PSC anlaşma kimliği** - Anlaşma için PSC'deki benzersiz tanımlayıcı.
- **Hatalar** - belirli bir anlaşmadan başka bir anlaşmayı alırken hata olup olamay olduğunu belirtmek için.

Başarıyla geçirilen tüm anlaşmalar PSC'de görünmez. Geçiş yapılan anlaşmalar üzerinde çalışmaya devam İş Ortağı Merkezi.

PSC'den geçirilen anlaşmalar Ortak satış fırsatları sayfasının Giden sekmesinde kullanılabilir. Tüm anlaşmalar İş ortağı tarafından oluşturulan anlaşmalar olarak oluşturulur. Bunlar Microsoft satıcılarının kullanımına açık.

>[!Important]
> Bazı anlaşmaların geçirilenemleri nedeniyle herhangi bir hata varsa, "Anlaşmaları geçir" düğmesine tıklayarak anlaşma **geçişini yeniden başlatabilirsiniz.** Yalnızca henüz geçirilemeyen bazı uygun anlaşmalar varsa etkinleştirilir. Bu, anlaşma geçişi başladıktan sonra PSC'de bazı yeni anlaşmaların oluşturulacak olduğu geçiş aşamasında da yararlı olacaktır.

Tüm anlaşmalar başarıyla geçirildiktan sonra , **"Anlaşmaları geçir"** düğmesinin devre dışı bırakıldığında "Geçirılacak anlaşma **yok"** ifadesini gösteren bir başlık **vardır.**

## <a name="next-steps"></a>Sonraki adımlar

IOT anlaşmaları oluşturma ve yönetme hakkında bilgi İş Ortağı Merkezi.
Bu önemli bir adımdır ve bu adım, IOT anlaşma yönetimi için hazırlık İş Ortağı Merkezi. Anlaşmaları etkili bir şekilde oluşturmak ve yönetmek İş Ortağı Merkezi iş akışlarını ve iş akışlarını anlama. Bu belgeyi tamamen okuyarak başlayabilirsiniz.

## <a name="differences-between-psc-and-pc-workflows"></a>PSC ile PC iş akışları arasındaki farklar

|**Senaryo**|**İş Ortağı Satış Bağlan**|**İş Ortağı Merkezi**|
|-----|:-----|:-----|
|Kullanıcı rolleri|PSC'de yönetici, satış yöneticisi ve satıcı rolleri vardır.|İş Ortağı Merkezi, [konum kapsamına göre hem](permissions-overview.md#manage-referrals) okuma hem de yazma izni veren referans yöneticisi ve referans kullanıcı rollerine sahiptir.|
|Microsoft satıcı ayrıntıları|Anlaşma oluşturulur oluşturulmaz görünür.|Anlaşma türü iş ortağı tarafından yönlendirilen Microsoft Satıcı ayrıntıları iş ortaklarının kullanımına açık değildir.
|Çözümler|Anlaşmaya herhangi bir sayıda çözüm eklenebilir.|İş ortağı anlaşmaya en fazla 50 çözüm ekleyebilir.
|Anlaşma ataması|Anlaşmaları yalnızca atanan satıcı görüntülemeli ve üzerinde eylemde davranabilir.|Bir anlaşmanın takıma eklenen referans kullanıcıları anlaşmayı görüntüp üzerinde eyleme geçebilirsiniz. Anlaşmanın oluşturulmuş olduğu MPN konumu için referans yöneticileri, anlaşmayı görüntüp üzerinde eylem gerçekleştirebilirsiniz.|
|Müşteri kuruluşu|Serbest biçimli metin girişi.|Yalnızca birkaç karakter [yazarak](manage-co-sell-opportunities.md#select-your-customer) [müşteri kuruluşunda D&B](https://www.dnb.com/) veritabanında arama edebilirsiniz. Yasal ad ve adres, seçime göre otomatik olarak doldurulur.|

## <a name="moving-from-psc-to-pc---faq"></a>PSC'den PC'ye Taşıma - SSS

Aşağıdaki bölümlerde geçişle ilgili sık sorulan sorular yanıtlanmaktadır.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1 - Erişim iznim yoksa ne İş Ortağı Merkezi?

Atanmış rolleri almak için "Erişim yok" sayfasında listelenen yöneticilerinize başvurabilirsiniz. Referanslar bölümünde [okuma ve](permissions-overview.md#manage-referrals) yazma izni için referans yöneticisi rolüne ihtiyacınız olacak. Yalnızca iş profillerini yönetiyorsanız, iş profili yöneticisi rolünüz İş Ortağı Merkezi.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="İş Ortağı Merkezi'da erişim yok deneyimini gösteren görüntü.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2 - Who bölümündeki Referanslar bölümüne erişim izni İş Ortağı Merkezi?

Hesap [yöneticiniz,](permissions-overview.md#manage-mpn-membership-and-your-company) Referanslar sekmesine erişmenizi sağlar. Hesap yöneticinizi bulmak için **panonun** sağ üst köşesindeki dişli simgesinden Hesap ayarları'İş Ortağı Merkezi [seçin.](https://partner.microsoft.com/dashboard) Ardından, ikinci **düzey,** sol gezinti çubuğundan Kullanıcı yönetimi'ni seçin. Kullanıcı listesinin üst kısmında Filtre  açılan menüsünü seçin ve seçeneğini hesap yöneticisi **olarak belirleyin.** Sayfada tüm hesap yöneticileri ilgili e-posta adresleriyle birlikte görüntülenir. İş hesabınız için referans yöneticisi rolünü atamasını istemek için bunlardan birini sorun.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3 - Hesabımız için +yeni anlaşma düğmesi gridir. Anlaşma oluşturmaya başlamak için ne yapabilirim?

Bu yalnızca hesabınızla ilişkili MPN Kimliği IOT anlaşmaları oluşturmak için etkinleştirilmediyse gerçekleşir. Eğitim oturumları sırasında sağlanan e-postada IOT iş ekibine başvurun veya IOT anlaşmaları için MPN id'nizi etkinleştirecek bir destek bileti oluşturun."

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4 - PSC gibi kuruluştan belirli bir kişiye anlaşma atay musunuz?

Takım üyelerini belirli bir satış anlaşmasına atdırarak. Diğer referans yöneticilerinin bu anlaşmaları görüntülemesini veya bu anlaşmalara göre hareket etmelerini engellemez.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5 - Bana atanan tüm anlaşmaların bir görünümü var mı?

Kullanıcı düzeyinde bir sekme olan sık kullanılanlar özelliğini kullanabilirsiniz. Anlaşmalara hızlı erişim elde etmek için size atanan tüm anlaşmaları sık kullanılanlara ekleyebilirsiniz.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6 - Anlaşmalar için salt okunur bir görünüm var mı?

Hayır, referanslar bölümünde anlaşmaların salt okunur bir görünümü yoktur.

### <a name="7---is-adding-a-customer-organization-mandatory"></a>7 - Müşteri kuruluşu eklemek zorunlu mu?

Evet, müşteri [kuruluşuna yeni](./manage-co-sell-opportunities.md#select-your-customer) bir kuruluş eklemek İş Ortağı Merkezi. İlk olarak müşterinin bulunduğu konumu arayarak başlayalım. Sahip olduğunuz ayrıntılara göre; Tam bina adı dahil olmak üzere belirli ayrıntıları ekleyebilir veya yalnızca şehir ayrıntılarını veabilirsiniz. Kuruluş araması, herhangi bir adres ayrıntısı girmeniz gerekmayacak şekilde, girersiniz adla eşleşen tüm yasal varlıkları getirir. Tüm ayrıntılar seçilen kuruluşa göre otomatik olarak doldurulur.

### <a name="8---are-customer-contact-details-mandatory"></a>8 - Müşteri iletişim bilgileri zorunlu mu?

Evet, müşteri iletişim ayrıntıları IOT anlaşmaları oluşturmak için zorunludur.

### <a name="9---how-many-solutions-can-i-add-to-a-deal"></a>9 - Bir anlaşmaya kaç çözüm ekleyebilirim?

Bir satış anlaşmasına en fazla 50 çözüm (PSC'de 'ürünler' ile benzer) eklersiniz. Çözümler için hem miktar hem de tahmini kapanış tarihi zorunludur ve çözümlerin tahmini kapanış tarihi, anlaşma ayrıntıları bölümündeki tahmini kapanış tarihinden önceki olmalıdır.

### <a name="10---where-can-i-find-the-opportunity-id"></a>10 - Fırsat kimliğini nerede bulamıyorum?

PSC'deki Fırsat Kimliği, İş Ortağı Merkezi. Herhangi bir anlaşmayı a açmak için anlaşma adının yanında Referans Kimliğini bulabilirsiniz.
