---
title: Iş ortağı satış bağlantısı 'ndan (PSC) geçiş
ms.topic: article
ms.date: 08/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft iş ortaklarının iş ortağı satış Connect 'ten (PSC) iş ortağı merkezi 'ne nasıl geçirebileceğini ve Microsoft satıcıları tarafından gönderilen anlaşmalar oluşturma veya yönetme hakkında bilgi edinin.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc131991826a6428d613aa34e2e99c19e3efde05
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/22/2020
ms.locfileid: "92531547"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>İş ortağı satış bağlantısı (PSC) üzerinden geçiş yapan iş ortakları için Iş Ortağı Merkezi 'nde (PC) ortak satış ile ilgili kılavuz

**Uygulama hedefi**

- İş Ortağı Merkezi

**Uygun roller**

- Hesap yöneticisi
- Başvuru Yöneticisi
- İş ortağı satış bağlantısı (PSC) satıcı
- İş ortağı Sales Connect (PSC) Yöneticisi
- İş ortağı Sales Connect (PSC) anlaşma Yöneticisi

Siz bildiğiniz gibi şirketiniz, 31 Aralık 2020 ' e kadar PSC 'ye erişimi kaybedecektir. Bununla birlikte, ortak satış anlaşmaları oluşturmak, anlaşmaları yönetmek ve Iş Ortağı Merkezi 'nde size Microsoft satıcıları tarafından gönderilen anlaşmalar için işlem yapmak istediğiniz her şeyi bulacaksınız. Bununla birlikte farklar vardır ve aşağıdaki kılavuz, Iş Ortağı Merkezi 'ne geçişinizi daha yumuşak ve sorunsuz bir şekilde yapmanıza yardımcı olur.

>[!Important]
> Buradan geçiş hakkında PSC 'de bir başlık gördüğünüz için doğru yerde olursunuz. Bu kılavuz, PSC 'de anlaşmalar yöneten çözüm değerlendirmesi (SA) ve OEM ıOT iş ortakları için geçerli değildir.

## <a name="before-you-move-things-you-need-to-know"></a>Taşımadan önce bilmeniz gereken şeyler

### <a name="if-you-are-psc-admin"></a>PSC yöneticisiyseniz

- İş [Ortağı Merkezi](https://partner.microsoft.com/)'nde oturum açmak için iş e-postasına ihtiyacınız vardır.
- Iş Ortağı Merkezi [Hesap Yöneticisi](permissions-overview.md)yardımıyla hesabınızı ayarlayın.
- Bu belgeyi okuyarak Iş Ortağı Merkezi 'nde ortak satışı yapmayı öğrenin.
- Tüm PSC kullanıcılarınız (yönetici, anlaşma Yöneticisi ve satıcı rolleri) için Iş Ortağı Merkezi 'nde Kullanıcı hesapları kurun ve bunlara [referans yönetici rolleri](permissions-overview.md)atayın.

>[!Important]
> PSC başlığında gösterilen MPN KIMLIĞININ Iş Ortağı Merkezi 'nde MPN konumları listesinde bulunduğundan emin olun. İş Ortağı Merkezi 'nde "hesap ayarları" ve "[konumlar](manage-locations.md)" a giderek iş ortağı merkezi hesabıyla Ilişkili tüm MPNS listesini bulmak için bunu doğrulayabilirsiniz.

 :::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="İş ortaklarının MPN KIMLIĞINI bulabileceği PSC başlığını gösteren resim.":::

### <a name="if-you-are-psc-deal-manager-or-seller"></a>PSC Yöneticisi veya satıcı kullanıyorsanız

- İş [Ortağı Merkezi](https://partner.microsoft.com/)'nde oturum açmak için bir iş e-postasına ihtiyacınız vardır.
- PSC 'de iş dışı bir hesap kullanıyorsanız veya iş e-postanız iş ortağı şirketten farklı bir şirkette kullanılıyorsa, hesap kurulumu için PSC yöneticinizle iletişime geçin.
- PSC 'de oturum açmak için kullandığınız hesap ne olursa olsun, Iş ortağı merkezi hesap ayarlanmanız durumunda PSC yöneticinizle görüşün.
- Iş Ortağı Merkezi 'ne ve başvurular bölümüne erişiminiz olup olmadığını doğrulayın.
- İş akışlarını ve iş ortağı merkezindeki değişiklikleri anlamak için bu belgeyi okuyun.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>PSC 'de yönetici olarak, bunlar sonraki adımlardır

Başvurular sekmesini görmüyorsanız:

- Şirketinizin [genel Yöneticisi](permissions-overview.md) , başvurular sekmesine erişim izni verebilir. Genel yöneticinizle ilgili bilgi edinmek için iş ortağı merkezi 'nin sağ üst tarafındaki dişli simgesine ait Iş ortağı ayarları ' na gidin. Sol gezinti çubuğunun ikinci düzeyindeki Kullanıcı Yönetimi sayfasını seçin. Sayfanın sağ üst kısmındaki "tüm kullanıcılar" ı ve "Genel Yöneticiler" olarak değiştirin açılan listesine tıklayın. Bu sayfada, tüm genel Yöneticiler ilgili e-posta kimlikleriyle birlikte görüntülenir. İş hesabınız için "başvuru Yöneticisi" erişimi almak üzere bunlarla iletişim kurun.

>[!Important]
> Rolünüzün yalnızca PSC 'deki kullanıcıları yönetmesi durumunda, Iş Ortağı Merkezi 'nde [hesap yönetici](permissions-overview.md#manage-mpn-membership-and-your-company) rolü olursunuz. Rolünüzde ortak satış fırsatlarını yönetme de varsa, [başvuruları yönetici](permissions-overview.md#manage-referrals) rolü almalısınız. Ayrıca, aynı zamanda PC 'deki hesap yöneticilerine tek tek ulaşan tüm PSC yöneticileri yerine iş ortağı merkezi hesap yöneticisi ile çalışmak üzere PSC yöneticileri arasında tek bir değişiklik yönetimi liderine aday olun.

 :::image type="content" source="images/pscmigration/accountadmin.png" alt-text="İş ortaklarının MPN KIMLIĞINI bulabileceği PSC başlığını gösteren resim." olarak değiştirin açılan listesine tıklayın.
- Genel yönetici, Azure AD kiracınızda yeni bir kullanıcı hesabı oluşturabilir ya da diğer etki alanı hesabı kullanıcılarına Konuk Kullanıcı erişimi atayabilir.
- Tüm PSC anlaşma yöneticileri ve kullanıcıları için hesaplar kurulduktan sonra, Iş Ortağı Merkezi ' nde oturum açması, sol gezinti bölmesinde başvuru sekmesine gitmeniz ve başvurular sayfasını görebilecekleri konusunda emin olmak gerekir.

Şirketinizde bir PDM varsa-Iş Ortağı Merkezi hesabınız ayarlandığında ve kullanıcılarınız üzerine taşınır ve roller ve izinler varsa, ortak satış etkinliklerinizi Iş Ortağı Merkezi 'ne taşıyabilirsiniz. Geçiş tamamlanma son tarihine kadar beklemek yerine PDM, tüm yeni anlaşmalarınızın Iş Ortağı Merkezi 'ne akmasını sağlayan bir anahtar yapmasını bildirin.
>[!Note]
>Bu anahtarı yaptıktan sonra, yalnızca PSC 'deki mevcut etkin anlaşmalar üzerinde işlem yapabilirsiniz. Yeni anlaşmalar oluşturmayabilir veya PSC 'de Microsoft satıcılarından herhangi bir anlaşmalar alamazsınız.

Şirketiniz bir PDM içermiyorsa, tüm Kullanıcı hesaplarının tüm kullanıcılar tarafından ayarlandığından ve doğrulandığından emin olun. Iş Ortağı Merkezi 'nde ortak satış ile başlayabilmeniz için, bir e-posta ile ve PSC 'deki bir başlık aracılığıyla bildirimde bulunacaktır. PSC 'deki mevcut etkin anlaşmaları hala yönetmeniz gerektiğini unutmayın.

>[!Important]
>Etkin anlaşmalar BILGISAYARA geçirilmeyecektir. 31 Aralık 2020 ' e kadar olan anlaşmaları kapatmak ve kaydetmek için kullanabilirsiniz.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>PSC yöneticileri, PSC anlaşma yöneticileri ve PSC satıcıları için sonraki adımlar

Iş Ortağı Merkezi 'nde ortak satışı yapmayı öğrenin.
Bu önemli bir adımdır ve Iş Ortağı Merkezi 'nde ortak satış için hazırlıklı olmanıza yardımcı olur. İş akışlarını ve iş ortağı merkezindeki değişiklikleri anlamak için, bir günden etkin bir şekilde işbirliği yapabilirsiniz. Bu belgeyi tamamen okuyarak başlayın. [Ortak satış deneyimi galerisinde](https://aka.ms/cosellexperience)uygun bir kaynak kümesi de mevcuttur.

## <a name="major-differences-between-psc-and-pc-workflows"></a>PSC ve PC iş akışları arasındaki önemli farklılıklar

|**Senaryo**|**İş ortağı satışları bağlantısı**|**İş Ortağı Merkezi**|
|-----|:-----|:-----|
|Kullanıcı rolleri|PSC 'in yönetici, anlaşma Yöneticisi ve satıcı rolleri vardır.|BILGISAYAR yalnızca tüm anlaşmalar için hem okuma hem de yazma izni veren [başvuru Yöneticisi](permissions-overview.md#manage-referrals) rolüne sahiptir.|
|Ortak satış için Microsoft 'a davet etme|Microsoft satıcı tarafından başlatılan, iş ortağı tarafından açık bir sorun yoktur.|Bir Microsoft satıcı yardımı bir anlaşma için gerekliyse iş ortağının [açık bir istek](manage-co-sell-opportunities.md#add-solutions) yapması gerekir. Microsoft satıcının isteği reddetme seçeneği vardır.|
|Süre sonu|Bir anlaşma süre sonu kavramı yoktur.|İş ortağı tarafından kabul edilmediyse iş ortağı gelen anlaşmalar 14 gün içinde sona erer. Ayrıca, iş ortağı giden anlaşmalar, Microsoft satıcı bunları 14 gün içinde işlem yapmaz.|
|Microsoft satıcı ayrıntıları|Bir anlaşma oluşturulduktan hemen sonra görünür.|Microsoft satıcı ayrıntıları, yalnızca satıcı iş ortağından ortak satış davetini kabul ettiğinde ortak olarak paylaşılır.|
|[Özel işlem hattı](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Kullanılamıyor.|İş ortakları, Microsoft satıcıları için görünürlük vermeden kendi işlem hatlarını paylaşabilir.|
|Çözümler|Yalnızca bir fiyat listesine ait olan çözümler bir başa eklenebilir.|İş ortağı, aşağıdaki listelere ait [çözümler](manage-co-sell-opportunities.md#add-solutions) ekleyebilir. a) Microsoft 'un ilk taraf kataloğundan (PSC 'deki Işlem anlaşma rolüne benzer) ve c) çözümleri, diğer üçüncü taraf iş ortaklarından (PSC 'deki ISV anlaşma rolüne benzer şekilde) ortak satış çözümleri sağlar.|
|Anlaşma ataması|Yalnızca atanan satıcı, anlaşmaları görüntüleyebilir ve üzerinde işlem yapabilir.|Ekip üyeleri bir anlaşma üzerinde çalışan kişileri belirtmek için bir anlaşmaya eklenebilir, diğer başvuru yöneticilerinin bu anlaşmalar üzerinde görüntülenmesini veya bu anlaşmaları üzerinde hareket etmesinin engellenmesi yoktur.|
|Müşteri kuruluşu|Serbest form metin girişi.|Yalnızca birkaç karakter yazarak [Müşteri kuruluşunda](manage-co-sell-opportunities.md#select-your-customer) [D&B veritabanına](https://www.dnb.com/) göre arama yapabilirsiniz. Yasal ad ve adres seçime göre otomatik olarak doldurulur.|
|Müşteri iletişim|Zorunlu değildir.|Özel işlem hattı paylaşımı için zorunlu değildir. Microsoft satıcı, ortak satış isteğine katılmaya davet edildiyseniz gereklidir.|
|Ortak API|Kullanılamıyor.|Iş Ortağı Merkezi başvurularını programlı bir şekilde yönetmek için [ortak API](/partner/develop/referrals) .|

## <a name="psc-and-partner-center-field-mapping"></a>PSC ve Iş ortağı merkezi alan eşleme

Bu bölüm, PSC ve Iş ortağı merkezi arasındaki özniteliklerin tam eşlemesini gösterir. PSC 'deki her ekran, Iş Ortağı Merkezi ortak satış fırsatları bölümünde ilgili görünüm ile karşılaştırılır. 

>[!Note]
>Iş Ortağı Merkezi 'nde eşdeğer özniteliği bulmak için PSC ekran görüntülerinde sarı kabarcıkların numaralarını izleyin. Kırmızı kabarcıklar, dosyalanmış Iş Ortağı Merkezi 'nde kullanılabilir olmadığını gösterir.

**Iş Ortağı Merkezi 'nde ortak satış fırsatlarının ana sayfası ve varsayılan görünümü**

 :::image type="content" source="images/pscmigration/homepage.png" alt-text="İş ortaklarının MPN KIMLIĞINI bulabileceği PSC başlığını gösteren resim.":::

**PSC Grid görünümü ve Iş ortağı merkezi işlem görünümü**

- Iş Ortağı Merkezi 'nde PSC gibi bir liste görünümü yoktur.  Tüm anlaşmalar, müşteri bilgilerini ve anlaşma türünü içeren en son alınan veya oluşturulan tarihe göre listelenir. Görünümdeki ilk işlem varsayılan olarak seçilidir. PSC tablosu biçiminde görüntülenen değerlerin çoğu, bılgısayar içindeki anlaşma ayrıntı görünümünde kullanılabilir.
- Anlaşma rolü, BILGISAYARıNDA gerekli bir alan değildir. Hiçbir iş akışının hiçbirinde gösterilmez veya yakalanmaz. Microsoft satıcı tarafında, başa eklenen çözümlere göre otomatik olarak türetilir.
- Son değiştirilme tarihi, BILGISAYARDAKI başvuru ayrıntıları sayfasında gösterilmez. İş ortakları, son güncelleme tarihine göre anlaşmaları sıralamak için sıralama işlevini kullanabilir.

 :::image type="content" source="images/pscmigration/gridview.png" alt-text="İş ortaklarının MPN KIMLIĞINI bulabileceği PSC başlığını gösteren resim.":::

**PSC ve Iş Ortağı Merkezi 'nde anlaşma Ayrıntıları görünümü**

- İş ortakları, iş ortağı anlaşma ayrıntısı görünümündeki Düzenle düğmesine tıklayarak bir anlaşmayı düzenleyebilir (6). Düzenle düğmesine tıklandıktan sonra tüm alanlar, anlaşma için yapılan düzenlemeleri kaydetme veya iptal etme seçeneğiyle düzenlenecektir.
- Iş Ortağı Merkezi 'nde Yineleneni kapatma seçeneği yoktur.
- Müşteri sonucu iş ortağı merkezi 'nde kullanılamaz. Müşteri etkileşimlerine ilişkin tüm ayrıntılar, bılgısayar içindeki Notlar bölümünde güncelleştirilemeyebilir.
- Tahmini çözüm kapatma tarihi yalnızca Iş Ortağı Merkezi 'nde OEM ıOT anlaşmaları ile kullanılabilir. Diğer hiçbir anlaşma türü için görüntülenmez.
- Lisanslama programı bılgısayarda gerekli değildir. Bu, işlem sırasında seçilen çözümlere göre otomatik olarak algılanır.

>[!Note]
>Kazanıldı veya kaybedildi olarak işaretlenen herhangi bir anlaşma, bu gönderiyi düzenleyemezsiniz. Bu Terminal durumlarından birine bir anlaşma taşırken dikkatli olun.

 :::image type="content" source="images/pscmigration/dealdetails.png" alt-text="İş ortaklarının MPN KIMLIĞINI bulabileceği PSC başlığını gösteren resim.":::

**PSC ' ürün ekleme ' görünümü ve Iş Ortağı Merkezi ' çözüm Ekle ' görünümü**

 :::image type="content" source="images/pscmigration/products.png" alt-text="İş ortaklarının MPN KIMLIĞINI bulabileceği PSC başlığını gösteren resim.":::

**PSC ve Iş Ortağı Merkezi 'nde Kullanıcı Yönetimi**

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="İş ortaklarının MPN KIMLIĞINI bulabileceği PSC başlığını gösteren resim.":::

**PSC ve Iş Ortağı Merkezi 'nde Kullanıcı rolü ataması**

- PSC Yöneticisi için eşdeğer rol, Iş Ortağı Merkezi ' nde Hesap Yöneticisi rolüdür.
- Iş Ortağı Merkezi 'nde, referans yönetici rolü olan ortak satış anlaşma yönetimi için yalnızca bir rol vardır.

 :::image type="content" source="images/pscmigration/roles.png" alt-text="İş ortaklarının MPN KIMLIĞINI bulabileceği PSC başlığını gösteren resim.":::

**PSC ve Iş ortağı merkezindeki bildirimler**

 :::image type="content" source="images/pscmigration/notifications.png" alt-text="İş ortaklarının MPN KIMLIĞINI bulabileceği PSC başlığını gösteren resim.":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>PSC 'den Iş Ortağı Merkezi 'ne geçme-sık sorulan sorular

**Q1. Iş Ortağı Merkezi 'ne erişim izni yoksa ne yapmam gerekir?**

Atanan rolleri almak için, "erişim yok" sayfasında listelenen yöneticilerinize başvurabilirsiniz. Başvurular bölümünde okuma ve yazma izni için "[başvuru Yöneticisi](permissions-overview.md#manage-referrals)" rolüne ihtiyacınız olacaktır. Yalnızca iş profillerini yönetiyorsanız, iş ortağı merkezi 'nde "Iş profili Yöneticisi" rolüne ihtiyacınız olacaktır.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="İş ortaklarının MPN KIMLIĞINI bulabileceği PSC başlığını gösteren resim." yalnızca ISV Connect programına kayıtlı iş ortakları tarafından, Iş Ortağı Merkezi 'nde ilgili ortak satış fırsatı olmadan bir anlaşma kaydetmek için kullanılır. Bir ortak satış fırsatıyla anlaşmalar kaydettirmek için, anlaşma Kazanıldı olarak işaretlendiğinde ve anlaşma kaydı ölçütlerini karşılıyorsa bir açılır pencere görüntülenir.

**Q9. Bir müşteri kuruluşu zorunlu mi ekliyor?**

Evet, [Müşteri kuruluşu](./manage-co-sell-opportunities.md#select-your-customer) eklemek Iş Ortağı Merkezi 'nde zorunludur. İlk olarak, müşterinin konumun bulunduğu konumu arayarak başlayın. Sahip olduğunuz ayrıntılara göre; tam bina adını dahil edebilir veya yalnızca şehir ayrıntıları verebilirsiniz. Kuruluş araması, girdiğiniz adla eşleşen tüm yasal varlıkları getirecek, böylece herhangi bir adres ayrıntısı girmenize gerek kalmaz. Tüm ayrıntılar, seçilen kuruluşa göre otomatik olarak doldurulur.

**Q10. Müşteri iletişim ayrıntıları zorunludur mi?**

Oluşturmakta olduğunuz [işlem türüne](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) bağlıdır. Yalnızca işlem hattınızı paylaşıyorsanız ve Microsoft satış kuruluştan herhangi bir yardım gerektirmiyorsa, müşteri iletişim ayrıntılarını vermemesini seçebilirsiniz. Microsoft satıcı 'dan etkin bir şekilde yardım Aradığınız yerde ortak satıyor olmanız durumunda müşteri iletişim ayrıntılarını sağlamanız gerekir. İş Ortağı Merkezi 'nde ortak satış isteği oluşturmadan önce müşteriden açık onay almalısınız.

**Q11. Bir dağıtmaya kaç çözüm ekleyebilirim?**

En fazla 50 çözüm ekleyebilirsiniz (PSC 'de ' Ürünler ' öğesine benzer), bir anlaşma. PSC 'nin aksine, kendi ortak satış uygun çözümlerinizde, Microsoft ilk taraf SKU 'Lardan ve diğer üçüncü taraf ortak satış özellikli çözümlerle çözümler karıştırabilirsiniz. İş Ortağı Merkezi 'nde seçilecek veya kullanılabilecek bir anlaşma rolü yok. Microsoft SKU 'Ları için, isteğe bağlı olarak, başa eklenen her SKU için miktar ve fiyat ekleyebilirsiniz.

**Q12. Bir anlaşma oluşturduktan sonra Microsoft satıcı ayrıntılarını ne zaman alabilirim?**

Microsoft satıcıları, Microsoft tarafındaki ilgili satıcı ile ilgilenirken belirtilen tam yardım gereksinimini eşleştirdikten sonra atanır. Atamadan sonra bile Microsoft satıcıları, ortak satış davetini kabul etme veya reddetme seçeneğine sahip olacaktır. Yalnızca bir satıcı tarafından bir ortak satış daveti kabul edilirse, bu anlaşma Microsoft satıcı iletişim ayrıntıları ile güncelleştirilir. Microsoft satıcıları için SLA, anlaşma üzerinde işlem yapması için 14 gündür. Bu, iş ortaklarının, zaman aşımına uğramadan önce anlaşma üzerinde işlem yapması gereken SLA 'dır.

**Q13. Fırsat KIMLIĞINI nerede bulabilirim?**

PSC 'deki fırsat KIMLIĞI, BILGISAYARDAKI anlaşma KIMLIĞIYLE aynıdır. Herhangi bir anlaşmayı açtığınızda anlaşma adının yanında anlaşma KIMLIĞINI bulabilirsiniz.

**Q14. PDM nasıl BILGISAYARA erişebilirim?**

İş Ortağı Merkezi 'Ne doğrudan PSC 'nin aksine, PDMs 'niz tarafından erişilemez. Bu özelliği etkinleştirmek için aşağıda bahsedilen birden çok seçenek vardır.

- OCP Insights-PDMs yalnızca bunlarla ilgili anlaşmalar & ilerlerse, kuruluşunuzun görünümünü almak için OCP Insights portalını kullanabilirler. Bu bir iç araçtır ve yalnızca PDMs için kullanılabilir. OCP öngörülerinin şirketinizin kullanıcıları için sunulmadığını unutmayın.
- Iş Ortağı Merkezi 'nde Konuk Kullanıcı-PDM @microsoft.com Hesabınızı, iş ortağı merkezi 'nde Konuk Kullanıcı olarak ekleyebilir ve başvuruları görüntüleyebilmek ve bunlarla işlem yapabilmesi için başvuru Yöneticisi rolü atayabilirsiniz.
- Kiracınızda [Yeni bir Kullanıcı](./create-user-accounts-and-set-permissions.md#add-a-new-user) oluşturma-kendi kiracınızda yeni bir kullanıcı oluşturabilir ve bu ayrıntıları PDM ile paylaşabilir ve bu sayede hesabınızdaki diğer başvuru kullanıcılarına benzer başvuruları görüntüleyebilir ve bunlarla işlem yapabilir.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Iş Ortağı Merkezi 'nde anlaşmalar oluşturmanıza ve yönetmenize yardımcı olacak kaynaklar

Ortak satış yardım konularını henüz okumadıysanız, aşağıdaki kaynaklar iş ortağı merkezindeki anlaşmaları yönetmenize yardımcı olur.

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

## <a name="additional-resources"></a>Ek kaynaklar

- İş ortağı satışları iş ortağı [Merkezi çalışma kitabına bağlanır](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) -iş ortaklarının satış süreçlerini ve rollerini Iş Ortağı Merkezi Ile Iş ortağı Sales Connect aracılığıyla yeni satış süreçleriyle hizalayın.
- [Iş Ortağı Merkezi ortak satış çalışma kılavuzu](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) -müşteri adaylarını yönetmek Için Iş Ortağı Merkezi aracılığıyla bir işletim modelini belirlemek için bir iş modeli veya ortak satış fırsatları ve anlaşmaları kaydetme.
- [Başvuru yönetimi destesi](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) -müşteri adaylarını yönetmek için görselleştirilen adım adım yönergeler ve Iş Ortağı Merkezi aracılığıyla ortak satış fırsatları.
- [Ticari Market 'Te yayımlama ve yönetme](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) -ticari Market 'Teki Iş Ortağı Merkezi aracılığıyla teklifler oluşturmak, yönetmek ve yayımlamak için görselleştirilen adım adım yönergeler.
