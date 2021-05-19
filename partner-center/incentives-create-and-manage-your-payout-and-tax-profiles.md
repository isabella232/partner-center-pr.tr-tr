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
ms.openlocfilehash: b167b0e65f3339a29f0227f6135ed70931300d8e
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152163"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a>Iş Ortağı Merkezi 'nde teşvikleri ödeme ve vergi profilleri oluşturma ve yönetme

**Uygun roller**: teşvikleri admin | Hesap Yöneticisi | Genel yönetici

Belirli bir MPN konumuna ilişkin teşvik programlarınızda ödeme alabilmeniz için önce geçerli bir ödeme ve vergi profilini programla ve MPN konumuyla ilişkilendirerek kaydınızı tamamlamanız gerekir. Microsoft ödemeleri yapmak için bu ödeme ve vergi profilini kullanacaktır. Teşvik programının kurallarına bağlı olarak ödeme için elektronik banka transferi veya alacak dekontu kullanmanıza izin verilebilir. 

## <a name="roles-currencies-and-multiple-microsoft-incentive-programs"></a>Roller, para birimleri ve birden çok Microsoft özenli program

Ödeme ve vergi profiliniz ile çalışmaya başlamadan önce aşağıdaki bilgileri anlamanız önemlidir.

### <a name="roles-and-permissions"></a>Roller ve izinler

Teşvik ödemeleri için banka ve vergi bilgilerini girmek üzere bir teşvikleri yöneticisi olmanız gerekir. MPN/Account yöneticisiyseniz, kendinizi ve/veya iş arkadaşını teşvikleri Yöneticisi olacak şekilde atayabilirsiniz.

Teşvikleri yönetici izinleri istemeniz gerekiyorsa MPN yöneticinizle veya genel yöneticinizle iletişime geçin. [Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/)oturum açarak şirketinizde kimlerin bu rolleri olduğunu bulabilirsiniz. Sağ üst köşedeki **Ayarlar** simgesinden **Kullanıcı yönetimi** ' ni seçin ve ardından Genel yönetici ' ye filtre uygulayın.

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

1. Azure Active Directory (Azure AD) hesabınızı (Şirket hesabı) veya atanmış bir e-posta adresini kullanarak [Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.

   - Birden çok etki alanı, bir Azure AD hesabında kaydedilebilir. Hangi etki alanlarının ilişkilendirildiğini öğrenmek için genel yöneticinizle iletişime geçin.
   - Yalnızca etki alanı ile oturum açabiliyor @onmicrosoft.com ve ek etki alanlarına ihtiyacınız varsa, Azure AD hesabına ek etki alanları eklemek Için hesap yöneticinize başvurun.
   - **İş veya okul hesabı** ya da **kişisel hesap**' i seçmeniz istenirse **iş veya okul hesabı**' nı seçin.

2. Dişli simgesini seçerek **Ayarlar** menüsünü açın ve **Hesap ayarları**' nı seçin.

3. **Hesap ayarları** menüsünde, **ödeme ve vergi**' ı seçin.

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a>Ayrı programlara ödeme ve vergi profilleri atama

1. [Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/)oturum açın ve sonra da dişli simgesini seçerek **Ayarlar** menüsünü açın. 

2. **Hesap ayarları**' nı seçin, **ödeme ve vergi bölümünü** genişletin ve ardından **ödeme ve vergi profili ataması**' nı seçin. 
   
   Programlarınızın bir listesi görüntülenir. Profil ayrıntılarını görmek için bir programın yanındaki oku seçin. 

3. **Vergi profili** açılan menüsünde istediğiniz vergi profilini seçin veya yeni bir profil oluşturma seçeneğini belirleyin. Yeni bir profil oluşturma seçeneğini belirlediğinizde uygun şekilde yeniden yönlendirilirsiniz.  Açılır pencerede **devam** ' ı seçin. Yeni bir vergi profili oluşturma işlemi aşağıda verilmiştir.

4. **Ödeme yöntemini** seçin.

   - Ödeme yönteminiz **olarak Elektronik banka aktarımı'ı** seçtiyseniz, istediğiniz ödeme profilini seçin veya yeni profil oluşturma seçeneğini belirleyin. Yeni profil oluşturma seçeneğini belirtirseniz, uygun şekilde yeniden yönlendirilmesi gerekir. Açılan pencerede Devam'ı seçin. Yeni ödeme profili oluşturma işlemi aşağıda verilmiştir.

   - Ödeme yönteminiz olarak **Kredi Notu'seçin,** ardından doğrulamayı tamamlarsanız. Bu, başvurulan SAP numarasının kuruluşa ait olduğunu onaylar.

    >[!NOTE]
    >Listelenen birden çok Microsoft iş varlığı varsa, her varlık için bir ödeme profili seçmeniz gerekir.

    >[!NOTE]
    >Ödeme yöntemi kullanılabilirliği teşvik programının kurallarına bağlıdır.

    - Konum MPN Kimliğiniz belirli bir teşvik programı için yerel bir Microsoft yan kuruluşu tarafından ödeniyorsa ve ödeme yöntemi olarak LRD (sınırlı risk dağıtımcı) kredi faturasına izin verdiyse, ödeme profiliniz LRD Kredi Notu ödeme yöntemiyle önceden doldurulur. İlgili teşvik programı ve konum MPN Kimliği için LRD kredi notu  ödeme  yöntemi satırlarında, ödeme profili bölümünde durum olarak Onaylandı veya Doğrulama Gerekiyor'a bakabilirsiniz.
    
       Kredi **notu ödemesi** almak için KONUM MPN'si ve ödeme yöntemi ile ilişkili CSP kiracı kimliği ayrıntılarını onaylamak ve doğrulamak için Doğrulama gerekiyor'a tıklayın. Kredi Notu **Ayrıntıları iletişim** kutusunda CSP Kiracı Kimliği ve sağlanan ayrıntıların doğru olduğunu gözden geçirip doğrulayın. Birden fazla kiracı kimliğiyle karşısanız, ödeme almak istediğiniz CSP kiracı kimliğini dikkatle seçin. Ardından, şirket **ayrıntılarınızı** doğru kabul etmek için Onayla'ya tıklayın ve teşvik ödemesi seçtiğiniz CSP kiracı kimliğine yapılacaktır.
 
      Durum Onaylandı **olarak gösteriyorsa** CSP kiracı kimliğinin ataması tamamlandı ve başka bir eylem gerekmez. Yine de atamanın ayrıntılarını görmek için Onaylandı'ya tıklayın.
   
      İş ortaklarının bir vergi muafiyeti uygulama isteğine açık bir şekilde ihtiyacı olan ülkelerde, bir vergi muafiyeti ' nin yanına,, teşvik programı ve konum MPN 'nin vergi profili bölümünde vergi profilinin yanına uygulanması için bir seçenek olacaktır. Bu kutunun işaretlenmesi, bu kredi notunuza vergi muafiyet avantajları uygular. 
   
      Şu anda, LRD Kredi dekontu ödeme yöntemi yalnızca Avustralya, Yeni Zelanda ve Microsoft ticaret teşvik programı için Kanada iş ortakları için kullanılabilir. Bu üç ülkede MCI programına kaydolmuş olan doğrudan bir Bill partner veya dolaylı sağlayıcısıysanız ve uygun ödeme yöntemi olarak LRD kredi dekontunu görmüyorsanız, kiracı KIMLIĞINIZIN ilgili iş ortağı MPN konum hesabıyla ilişkilendirildiğini doğrulayın. Bu konuda daha fazla bilgi edinmek için [kuruluş profilinizi güncelleştirme](update-your-partner-profile.md)makalesini okuyun.

    
5. **Para birimini** seçin.

6. Ödeme alanlarını tamamladıktan sonra **Gönder**' i seçin.

## <a name="set-up-a-default-bank-profile"></a>Varsayılan bir banka profili ayarlama

Varsayılan banka profillerinin kurulumunu yapabilir ve bunları MPN konumlarına atayabilirsiniz. Bu varsayılan profiller, Microsoft tarafından bu MPN konumu için sonraki kayıtlar için kullanılacaktır. 

1. [Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/)oturum açın ve sonra da dişli simgesini seçerek **Ayarlar**   menüsünü açın. 

2.  **Hesap ayarları**' nı seçin, **ödeme ve vergi** bölümünü genişletin ve ardından **ödeme ve vergi profilleri**' ni seçin. 

3. **Ödeme profilleri** bölümünde **varsayılan profilleri Yönet** ' i seçin. 

4. Varsayılan bir banka profili oluşturmak için **varsayılan bir banka profili Ekle**' yi seçin. 

5. Şirketinizin kullanılabilir banka profilleri listesinden bir banka profili seçin, bu banka profiliyle kullanılacak para birimini seçin ve ardından bu varsayılan profilin uygulanmasını istediğiniz MPN konumlarının listesini seçin.

6. Seçimleri tamamladıktan sonra **bitti** ' yi seçin. Tüm gerekli alanlar tamamlanana kadar bitti düğmesi tıklatılabilir olmaz. 

>[!NOTE]
>Aynı banka ve para birimi eşleştirmesi birden fazla konuma uygulanabilir. Konuma MPN'ye bir kez varsayılan profil ve para birimi birleşimi atandıktan sonra, gelecekteki varsayılan profil atamaları için konum açılan listesinde görünmez. Varsayılan seçim silinirse, konum MPN'i gelecekteki varsayılan profil atamaları için yeniden kullanılır. Her banka profili ve para birimi birleşimi benzersiz, düzenlenebilir bir satır olarak eklenir.

7. Gerekli tüm değişiklikler eklendiktan sonra Kaydet'i **seçin.**  

## <a name="create-your-bank-profile"></a>Banka profilinizi oluşturma

Banka profilleri şirket düzeyinde oluşturulur. Bu, bir şirket içindeki birden çok MPN kimliği ve teşvik programı arasında bir banka profilinin atanmalarına olanak sağlar. Farklı bankacılık ve vergi kuralları geçerli olduğu için, bankacılık profilini farklı ülkelere uygularken özel durumlar olabilir.

>[!NOTE]
>Aşağıdaki sayfalarda yıldız işareti olan alanlar gereklidir. Alanın ne olduğunu bilmiyorsanız bilgi simgesini seçin. 

1. Ayrıntılar **sayfasında şu** alanları doldurun: Profil **adı:** Bu ödeme profilini tanımlamak için benzersiz bir ad girin.
    **Banka hesabı konumu:** Şirketinizin bankasının bulunduğu ülke.
    **Ödeme yöntemi:** Bu hesap için tercih edilen ödeme İş Ortağı Merkezi elektronik banka aktarımıdır.

2. **İleri**’yi seçin.

3. Banka **hesabı sayfasında,** bilginizi girin. Bu sayfada gösterilen alanlar ülkeye göre değişiklik gösterir. 

4. **İleri**’yi seçin.

5. Yararlanıcı **sayfasında** uygun bilgileri girin. Yararlanıcı, şirketinizin bankanın hesabınızla ilgili olarak görüşmesi gerekirse iletişim kuracak kişidir.

6. Alanlar tamamlandığında Son'a tıklayın **ve** ardından **Onayla'ya seçerek** banka profilinizi oluşturun.

Ödeme ve vergi profilleri **sayfasına yeniden yönlendirilmesi** gerekir. Doğrulama tamamlanana kadar yeni **profilinizin durumu Bekleyen Microsoft** doğrulamasını yansıtacak. Bu işlem 48 saate kadar sürebilir. Doğrulama tamamlandıktan sonra profil durumunuz Onaylı veya **Eylem** gerekiyor **durumunu yansıtacak.** Eylem **Gerekli ise,** gerekli bilgileri sağlayarak yukarıdaki adımları tekrarlayın. 

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

5. Ek belgeler **sayfasında** gerekli alanlar'ı seçin ve Ardından'ı **seçin.** 

6. Ülkeniz **veya** bölgeniz için gerekli tüm belgeleri karşıya yüklemek için Gözat'ı seçin. Belge adı gösterildiğinde Karşıya Yükle'yi **seçin.** 

7. Belgeyi kaldırmanız gerekirse **Kaldır**' ı seçin.

8. Kaydetmek ve devam etmek için **son**' u seçin.

9. Açılan iletide **Onayla** ' yı seçin. **Ödeme ve vergi kurulumu** sayfasına geri yönlendirilirsiniz.
 
## <a name="update-expired-tax-profiles"></a>Vadesi geçen vergi profillerini Güncelleştir

1. [Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/)oturum açın ve sonra da dişli simgesini seçerek **Ayarlar** menüsünü açın.

1. **Hesap ayarları**' nı seçin, **ödeme ve vergi** bölümünü genişletin ve ardından **ödeme ve vergi profili**' ni seçin.

1. **Vergi profilini** seçin.

1. Sütun **sona erme tarihini** denetleyin ve süresi dolan veya süresi dolacak olan vergi profiline gidin.

1. **Düzenle**'yi seçin.

1. Vergi formu bölümünde, yeni ayrıntıları sağlayarak vergi formlarını güncelleştirin. 

## <a name="next-steps"></a>Sonraki adımlar

- [Ödemeler ve vergiler hakkında sık sorulan sorular](payout-faq.md)
