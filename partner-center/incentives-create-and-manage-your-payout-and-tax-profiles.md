---
title: İş Ortağı Merkezi'ndeki ödeme ve vergi profilleri
ms.topic: how-to
ms.date: 04/15/2021
description: Teşvikleri çalışmanız için ödeme yapabilmeniz için ödeme ve vergi profilinizi oluşturun ve yönetin. Farklı profillerin oluşturulmasını, yönetilmesini ve kullanılmasını içerir.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: 35210907bfdb45c491cf08c531543b2ea91a2d214bbab085aa1d367e3168ff2a
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115695382"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a>Iş Ortağı Merkezi 'nde teşvikleri ödeme ve vergi profilleri oluşturma ve yönetme

**Uygun roller**: teşvikleri admin | Hesap Yöneticisi | Genel yönetici

Belirli bir MPN konumuna ilişkin teşvik programlarınızda ödeme alabilmeniz için önce geçerli bir ödeme ve vergi profilini programla ve MPN konumuyla ilişkilendirerek kaydınızı tamamlamanız gerekir. Microsoft ödemeleri yapmak için bu ödeme ve vergi profilini kullanacaktır. Teşvik programının kurallarına bağlı olarak ödeme için elektronik banka transferi veya alacak dekontu kullanmanıza izin verilebilir. 

## <a name="roles-currencies-and-multiple-microsoft-incentive-programs"></a>Roller, para birimleri ve birden çok Microsoft özenli program

Ödeme ve vergi profiliniz ile çalışmaya başlamadan önce aşağıdaki bilgileri anlamanız önemlidir.

### <a name="roles-and-permissions"></a>Roller ve izinler

Teşvik ödemeleri için banka ve vergi bilgilerini girmek üzere bir teşvikleri yöneticisi olmanız gerekir. MPN/Account yöneticisiyseniz, kendinizi ve/veya iş arkadaşını teşvikleri Yöneticisi olacak şekilde atayabilirsiniz.

Teşvikleri yönetici izinleri istemeniz gerekiyorsa MPN yöneticinizle veya genel yöneticinizle iletişime geçin. [Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/)oturum açarak şirketinizde kimlerin bu rolleri olduğunu bulabilirsiniz. sağ üst köşedeki **Ayarlar** simgesinden **kullanıcı yönetimi** ' ni seçin ve ardından genel yönetici ' ye filtre uygulayın.

Teşvikleri kullanıcılar, teşvik kazanç ve ödeme ayrıntılarını ve raporlarını görüntüleyebilir, ancak banka ve vergi ayrıntılarını düzenleyemez.

### <a name="choose-your-disbursement-currency"></a>Tediye para birimini seçin

Ödemeler, ödeme profilinizi ayarlarken seçtiğiniz para birimiyle yapılır. Ödemeler, Microsoft tarafından aylık olarak ayarlanan bir döviz kuru kullanılarak hesaplanır. Seçilen para birimi nedeniyle, değerde yapılan değişikliklerden sorumlu olacaksınız.

### <a name="using-different-profiles-for-different-microsoft-programs"></a>Farklı Microsoft programları için farklı profiller kullanma

Şirketiniz birden çok teşvik programında kaydedildiyse, hepsi için aynı ödeme hesabını kullanabilir veya farklı programlar için farklı ödeme hesapları kullanmayı tercih edebilirsiniz.

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a>Iş Ortağı Merkezi 'nde ödeme ve vergi profilleri oluşturma ve yönetme

Aşağıdaki bölümler, Iş Ortağı Merkezi 'nde ödeme ve vergi profilleri oluşturma ve yönetme sürecinde size yol gösterecektir.

>[!IMPORTANT]
>Iş Ortağı Merkezi 'nde ödeme ve vergi profilleri oluşturmak veya yönetmek için bir Özenisiz yönetici olmanız gerekir. Her bir teşvik programı altındaki her bir MPN konumuna bir rol atanması gerekir. Iş Ortağı Merkezi 'ne teşvik yöneticileri ekleme hakkında daha fazla bilgi için bkz. [Kullanıcı hesapları oluşturma](create-user-accounts-and-set-permissions.md).

## <a name="access-the-payout-and-tax-section-in-partner-center"></a>Iş Ortağı Merkezi 'nde ödeme ve vergi kısmına erişin

1. Azure Active Directory (Azure AD) hesabınızı (şirket hesabı) veya atanmış bir e-posta adresini kullanarak [iş ortağı merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.

   - Birden çok etki alanı, bir Azure AD hesabında kaydedilebilir. Hangi etki alanlarının ilişkilendirildiğini öğrenmek için genel yöneticinizle iletişime geçin.
   - Yalnızca etki alanı ile oturum açabiliyor @onmicrosoft.com ve ek etki alanlarına ihtiyacınız varsa, Azure AD hesabına ek etki alanları eklemek Için hesap yöneticinize başvurun.
   - **İş veya okul hesabı** ya da **kişisel hesap**' i seçmeniz istenirse **iş veya okul hesabı**' nı seçin.

2. **Ayarlar** menüsünü açmak için dişli simgesini seçin ve ardından **hesap ayarları**' nı seçin.

3. **Hesap ayarları** menüsünde, **ödeme ve vergi**' ı seçin.

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a>Ayrı programlara ödeme ve vergi profilleri atama

1. [iş ortağı merkezi panosunda](https://partner.microsoft.com/dashboard/)oturum açın ve ardından **Ayarlar** menüsünü açmak için dişli simgesini seçin. 

2. **Hesap ayarları**' nı seçin, **ödeme ve vergi bölümünü** genişletin ve ardından **ödeme ve vergi profili ataması**' nı seçin. 
   
   Programlarınızın bir listesi görüntülenir. Profil ayrıntılarını görmek için bir programın yanındaki oku seçin. 

3. **Vergi profili** açılan menüsünde istediğiniz vergi profilini seçin veya yeni bir profil oluşturma seçeneğini belirleyin. Yeni bir profil oluşturma seçeneğini belirlediğinizde uygun şekilde yeniden yönlendirilirsiniz.  Açılır pencerede **devam** ' ı seçin. Yeni bir vergi profili oluşturma işlemi aşağıda verilmiştir.

4. **Ödeme yöntemini** seçin.

   - Ödeme yönteminiz olarak **elektronik banka aktarımı** ' nı seçtiyseniz, istediğiniz ödeme profilini seçin veya yeni bir profil oluşturma seçeneğini belirleyin. Yeni bir profil oluşturma seçeneğini belirlediğinizde uygun şekilde yeniden yönlendirilirsiniz. Açılır pencerede devam ' ı seçin. Yeni bir ödeme profili oluşturma işlemi aşağıda verilmiştir.

   - Ödeme yönteminiz olarak **kredi dekontunu** seçtiyseniz doğrulamayı tamamlayabilirsiniz. Bu, başvurulan SAP numarasının kuruluşunuza ait olduğunu onaylar.

    >[!NOTE]
    >Listelenen birden fazla Microsoft iş varlığı varsa, her varlık için bir ödeme profili seçmeniz gerekir.

    >[!NOTE]
    >Ödeme yöntemi kullanılabilirliği, teşvik programının kurallarına bağlıdır.

    - MPN KIMLIĞINIZ, belirli bir bir bir bilgisayar için yerel bir Microsoft yan kuruluşu tarafından ödeniyorsa ve ödeme yöntemi olarak LRD (sınırlı riskli dağıtıcı) kredi faturasına izin veriyorsa ödeme profiliniz, LRD kredi notu ödeme yöntemiyle önceden doldurulur. LRD Kredi dekontu ödeme yöntemi satırında ilgili özeniler programı ve konum MPN KIMLIĞI için, ödeme profili bölümünde durum olarak **onaylama** veya **doğrulama** gerektiğini görürsünüz.
    
       Kredi dekontu ödemesini almak için, konum MPN ve ödeme yöntemiyle ilişkili CSP kiracı KIMLIĞI ayrıntılarını onaylamak ve doğrulamak için **doğrulama gerekiyor** ' u seçin. **Kredi dekontu ayrıntıları** iletişim kutusunda, belirtilen CSP Kiracı kimliği ve ayrıntılarının doğru olduğunu gözden geçirin ve doğrulayın. Birden fazla kiracı KIMLIĞIYLE birlikte sunulursa, ödemeleri almak istediğiniz CSP kiracı KIMLIĞINI dikkatle seçin. Daha sonra, şirket ayrıntılarınızın doğru olduğunu ve seçtiğiniz CSP kiracı KIMLIĞINE özendirme ödemesi gerektiğini onaylamak için **Onayla** ' yı seçin.
 
      Durum **onaylandığını** GÖSTERIYORSA, CSP Kiracı kimliği ataması tamamlanmıştır ve başka bir eylem gerekmez. Atamanın ayrıntılarını görmek için onaylanmış ' i de seçebilirsiniz.
   
      İş ortaklarının bir vergi muafiyeti uygulama isteğine açık bir şekilde ihtiyacı olan ülkelerde, bir vergi muafiyeti ' nin yanına,, teşvik programı ve konum MPN 'nin vergi profili bölümünde vergi profilinin yanına uygulanması için bir seçenek olacaktır. Bu kutunun işaretlenmesi, bu kredi notunuza vergi muafiyet avantajları uygular. 
   
      Şu anda, LRD Kredi dekontu ödeme yöntemi yalnızca Avustralya, Yeni Zelanda ve Microsoft ticaret teşvik programı için Kanada iş ortakları için kullanılabilir. Bu üç ülkede MCI programına kaydolmuş olan doğrudan bir Bill partner veya dolaylı sağlayıcısıysanız ve uygun ödeme yöntemi olarak LRD kredi dekontunu görmüyorsanız, kiracı KIMLIĞINIZIN ilgili iş ortağı MPN konum hesabıyla ilişkilendirildiğini doğrulayın. Bu konuda daha fazla bilgi edinmek için [kuruluş profilinizi güncelleştirme](update-your-partner-profile.md)makalesini okuyun.

    
5. **Para birimini** seçin.

6. Ödeme alanlarını tamamladıktan sonra **Gönder**' i seçin.

## <a name="set-up-a-default-bank-profile"></a>Varsayılan bir banka profili ayarlama

Varsayılan banka profilleri ayarlayabilir ve bunları MPN konumlarına atayabilirsiniz. Bu varsayılan profiller Microsoft tarafından söz konusu MPN konumunda daha sonra yapılan kayıt işlemlerinde kullanılır. 

1. [iş ortağı merkezi panosunda](https://partner.microsoft.com/dashboard/)oturum açın ve ardından **Ayarlar** menüsünü açmak için dişli simgesini seçin   . 

2.  **Hesap ayarları**' nı seçin, **ödeme ve vergi** bölümünü genişletin ve ardından **ödeme ve vergi profilleri**' ni seçin. 

3. **Ödeme profilleri** bölümünde **varsayılan profilleri Yönet** ' i seçin. 

4. Varsayılan bir banka profili oluşturmak için **varsayılan bir banka profili Ekle**' yi seçin. 

5. Şirketinizin kullanılabilir banka profilleri listesinden bir banka profili seçin, bu banka profiliyle kullanılacak para birimini seçin ve ardından bu varsayılan profilin uygulanmasını istediğiniz MPN konumlarının listesini seçin.

6. Seçimleri tamamladıktan sonra **bitti** ' yi seçin. Tüm gerekli alanlar tamamlanana kadar bitti düğmesi tıklatılabilir olmaz. 

>[!NOTE]
>Aynı banka ve para birimi eşleştirmesi birden fazla konuma uygulanabilir. MPN konumuna bir kez varsayılan profil ve para birimi birleşimi atanmışsa, daha sonra varsayılan profil atamaları için Konum açılır listesinde görünmez. Varsayılan seçim silinirse, MPN konumu gelecekteki varsayılan profil atamaları için yeniden görüntülenir. Her banka profili ve para birimi kombinasyonu benzersiz, düzenlenebilir bir satır olarak eklenir.

7. Tüm gerekli değişiklikler eklendikten sonra **Kaydet**' i seçin.  

## <a name="create-your-bank-profile"></a>Banka profilinizi oluşturma

Banka profilleri, bir şirket düzeyinde oluşturulur. Bu, bir banka profilinin bir şirketteki birden çok MPN KIMLIĞI ile atanmasını ve bu programları teşvik etmesine olanak tanır. Farklı bankacılık ve vergi kuralları uygulanabildiği için bankacılık profili farklı ülkelere uygulanırken özel durumlar olabilir.

>[!NOTE]
>Aşağıdaki sayfalarda, yıldız işareti olan alanlar gereklidir. Bir alanın ne olduğunu bilmiyorsanız, bilgi simgesini seçin. 

1. **Ayrıntılar** sayfasında, şu alanları doldurun: **profil adı:** bu ödeme profilini tanımlamak için benzersiz bir ad girin.
    **Banka hesabı konumu:** Şirketinizin bankasının bulunduğu ülke.
    **Ödeme yöntemi:** Iş Ortağı Merkezi için tercih edilen ödeme yöntemi elektronik banka aktarmasıdır.

2. **İleri**’yi seçin.

3. **Banka hesabı** sayfasında, bilgilerinizi girin. Bu sayfada gösterilen alanlar ülkeye göre farklılık gösterecektir. 

4. **İleri**’yi seçin.

5. **Lehdar** sayfasında, ilgili bilgileri girin. Lehdar, şirketinizdeki kişiden, hesabınızı tartışmaları gerektiğinde bankanın iletişim kurabildikleri kişidir.

6. Alanlar tamamlandığında, **son**' u seçin ve ardından banka profilinizi oluşturmak için **Onayla** ' yı seçin.

**Ödeme ve vergi profilleri** sayfasına yönlendirilirsiniz. Doğrulama tamamlanana kadar yeni **profilinizin durumu Bekleyen Microsoft** doğrulamasını yansıtacak. Bu işlem 48 saate kadar sürebilir. Doğrulama tamamlandıktan sonra profil durumunuz Onaylı veya **Eylem** gerekiyor **durumunu yansıtacak.** Eylem **Gerekli ise,** yukarıdaki adımları gerekli bilgileri sağlayarak tekrarlayın. 

## <a name="create-your-tax-profile"></a>Vergi profilinizi oluşturma

Microsoft'a, kuruluş için gereken vergi bilgilerini sağlamak üzere aşağıdaki yordamı kullanın. Bu bölümdeki sayfalar dinamiktir ve ülkenize veya bölgenize göre değişiklik gösterir. Doğru vergi bilgilerini tanımlamayla ilgili yardıma ihtiyacınız varsa, ülkenizin uygun kamu kaynaklarına ulaşın.

Amerika'daki iş ortağı şirketler için, W8 veya W9 formlarını tamamlama hakkında bilgi gerekirse aşağıdaki adresler sizi IRS sitesine alır:

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> Yalnızca şirketinizin ayrıntılarını girin. Kişisel ayrıntıları asla girmeyin.

1. İş **Profili sayfasında** gerekli alanları doldurun ve ardından Sonraki'yi **seçin.** 

2. Kurulum **sayfasında,** şirket için geçerli olan seçeneği belirleyin.

   - Sol tarafta, şirketiniz yalnızca şirket içinde yer Birleşik Devletler veya bu profil bir kişiye yönelikse seçeneğini belirleyin.
   - Şirket, şirket dışı bir şirketse sağ Birleşik Devletler seçin ve sonra listeden ülkenizi/bölgenizi seçin.

3. **İleri**’yi seçin. 

4. Vergi **durumu sayfasında** gerekli bilgileri girin ve ardından Sonraki'yi **seçin.** Bu sayfada yer alan alanlar ülkeye göre değişiklik gösterir. ayrıntılarınızı. 

5. Ek belgeler **sayfasında,** gerekli alanlar ve Ardından'ı **seçin.** 

6. Ülkeniz **veya** bölgeniz için gerekli tüm belgeleri karşıya yüklemek için Gözat'ı seçin. Belge adı gösterildiğinde, belge adını **Upload.** 

7. Belgeyi kaldırmanız gerekirse Kaldır'ı **seçin.**

8. Kaydetmek ve devam etmek için Son'a **tıklayın.**

9. Açılır **iletide** Onayla'ya seçin. Ödeme ve vergi kurulumu **sayfasına geri dönersiniz.**
 
## <a name="update-expired-tax-profiles"></a>Süresi dolan vergi profillerini güncelleştirme

1. Panoda [İş Ortağı Merkezi açın](https://partner.microsoft.com/dashboard/)ve ardından dişli simgesini seçerek Ayarlar **açın.**

1. Hesap **ayarları'ı** seçin, **Ödeme ve vergi bölümünü genişletin** ve sonra Ödeme ve vergi **profili'ne tıklayın.**

1. Vergi **profili'ne tıklayın.**

1. Sona Erme **Tarihi sütununu** kontrol edin ve süresi dolmuş veya süresi dolmak üzere olan vergi profiline gidin.

1. **Düzenle**'yi seçin.

1. Vergi formu bölümünde yeni ayrıntıları sağlayarak vergi formlarını güncelleştirin. 

## <a name="next-steps"></a>Sonraki adımlar

- [Ödeme ve vergiler hakkında sık sorulan sorular](payout-faq.yml)
