---
title: İş Ortağı Merkezi'ndeki ödeme ve vergi profilleri
ms.topic: how-to
ms.date: 11/12/2020
description: Teşvikleri çalışmanız için ödeme yapabilmeniz için ödeme ve vergi profilinizi oluşturun ve yönetin. Farklı profillerin oluşturulmasını, yönetilmesini ve kullanılmasını içerir.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: 66177c6e3cd0091081866e1508d28346f49ec713
ms.sourcegitcommit: bfc9e6f6476766cf10ba714f03ca2e96560003b1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/14/2020
ms.locfileid: "94626040"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a>Iş Ortağı Merkezi 'nde teşvikleri ödeme ve vergi profilleri oluşturma ve yönetme

**Uygulama hedefi:**

- İş Ortağı Merkezi

**Uygun roller:**

- Teşvikleri Yöneticisi
- Hesap yöneticisi
- Genel yönetici

Belirli bir MPN konumuna ilişkin teşvik programlarınızda ödeme alabilmeniz için önce geçerli bir ödeme ve vergi profilini programla ve MPN konumuyla ilişkilendirerek kaydınızı tamamlamanız gerekir. Microsoft ödemeleri yapmak için bu ödeme ve vergi profilini kullanacaktır. Teşvik programının kurallarına bağlı olarak ödeme için elektronik banka transferi veya alacak dekontu kullanmanıza izin verilebilir. 

## <a name="roles-currencies-and-other-microsoft-programs"></a>Roller, para birimleri ve diğer Microsoft programları

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
>Iş Ortağı Merkezi 'nde ödeme profilleri oluşturmak veya yönetmek için bir teşvik yöneticisi olmanız gerekir. Her bir teşvik programı altındaki her bir MPN konumuna bir rol atanması gerekir. Iş Ortağı Merkezi 'ne teşvik yöneticileri ekleme hakkında daha fazla bilgi için bkz. [Kullanıcı hesapları oluşturma](create-user-accounts-and-set-permissions.md).

## <a name="access-the-payout-and-tax-section-in-partner-center"></a>Iş Ortağı Merkezi 'nde ödeme ve vergi kısmına erişin

1. Azure Active Directory (Azure AD) hesabınızı (Şirket hesabı) veya atanmış bir e-posta adresini kullanarak [Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.

   - Birden çok etki alanı, bir Azure AD hesabında kaydedilebilir. Hangi etki alanlarının ilişkilendirildiğini öğrenmek için genel yöneticinizle iletişime geçin.
   - Yalnızca etki alanı ile oturum açabiliyor @onmicrosoft.com , Azure AD hesabına ek etki alanları eklemek Için hesap yöneticinize başvurun.
   - **İş veya okul hesabı** ya da **kişisel hesap** ' i seçmeniz istenirse **iş veya okul hesabı** ' nı seçin.

2. Dişli simgesini seçerek **Ayarlar** menüsünü açın ve ardından **iş ortağı ayarları** ' nı seçin.

3. **Hesap ayarları** menüsünde, **ödeme ve vergi** ' ı seçin. 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a>Ayrı programlara ödeme ve vergi profilleri atama

1. [Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/)oturum açın ve sonra da dişli simgesini seçerek **Ayarlar** menüsünü açın. 

2. **Iş ortağı ayarları** ' nı seçin, **ödeme ve vergi bölümünü** genişletin ve ardından **ödeme ve vergi profili ataması** ' nı seçin. 
   
   Programlarınızın bir listesi görüntülenir. Profil ayrıntılarını görmek için bir programın yanındaki oku seçin. 

3. **Vergi profili** açılan menüsünde istediğiniz vergi profilini seçin veya yeni bir profil oluşturma seçeneğini belirleyin. Yeni bir profil oluşturma seçeneğini belirlediğinizde uygun şekilde yeniden yönlendirilirsiniz.  Açılır pencerede devam ' ı seçin. Yeni bir vergi profili oluşturma işlemi aşağıda verilmiştir.

4. **Ödeme yöntemini** seçin.

   - Ödeme yönteminiz olarak **elektronik banka aktarımı** ' nı seçtiyseniz, istediğiniz ödeme profilini seçin veya yeni bir profil oluşturma seçeneğini belirleyin. Yeni bir profil oluşturma seçeneğini belirlediğinizde uygun şekilde yeniden yönlendirilirsiniz. Açılır pencerede devam ' ı seçin. Yeni bir ödeme profili oluşturma işlemi aşağıda verilmiştir.

   - Ödeme yönteminiz olarak **kredi dekontunu** seçtiyseniz doğrulamayı tamamlayabilirsiniz. Bu, başvurulan SAP numarasının kuruluşunuza ait olduğunu onaylar.

    >[!NOTE]
    >Listelenen birden fazla Microsoft iş varlığı varsa, her varlık için bir ödeme profili seçmeniz gerekir.

    >[!NOTE]
    >Ödeme yöntemi kullanılabilirliği, teşvik programının kurallarına bağlıdır.
    
5. **Para birimini** seçin.

6. Ödeme alanlarını tamamladıktan sonra **Gönder** ' i seçin.

## <a name="create-your-bank-profile"></a>Banka profilinizi oluşturma

Banka profilleri bir kuruluş düzeyinde oluşturulur. Bu, bir banka profilinin bir kuruluştaki birden fazla MPN KIMLIĞI ile atanmasını ve bu programları teşvik etmesine olanak tanır. Farklı bankacılık ve vergi kuralları uygulanabildiği için bankacılık profili farklı ülkelere uygulanırken özel durumlar olabilir.

>[!NOTE]
>Aşağıdaki sayfalarda, yıldız işareti olan alanlar gereklidir. Bir alanın ne olduğunu bilmiyorsanız, bilgi simgesini seçin. 

1. **Ayrıntılar** sayfasında, şu alanları doldurun: **profil adı:** bu ödeme profilini tanımlamak için benzersiz bir ad girin.
    **Banka hesabı konumu:** Şirketinizin bankasının bulunduğu ülke.
    **Ödeme yöntemi:** Iş Ortağı Merkezi için tercih edilen ödeme yöntemi elektronik banka aktarmasıdır.

2. **İleri** ’yi seçin.

3. **Banka hesabı** sayfasında, bilgilerinizi girin. Bu sayfada gösterilen alanlar ülkeye göre farklılık gösterecektir. 

4. **İleri** ’yi seçin.

5. **Lehdar** sayfasında, ilgili bilgileri girin. Lehdar, şirketinizdeki kişiden, hesabınızı tartışmaları gerektiğinde bankanın iletişim kurabildikleri kişidir.

6. Alanlar tamamlandığında, **son** ' u seçin ve ardından banka profilinizi oluşturmak için **Onayla** ' yı seçin.

**Ödeme ve vergi profilleri** sayfasına yönlendirilirsiniz. Yeni profilinizin durumu, doğrulama tamamlanana kadar **bekleyen Microsoft doğrulamasını** yansıtır. Bu işlem, 48 saate kadar sürebilir. Doğrulama tamamlandıktan sonra, profil durumunuz **onaylanan** veya **eylem gereken eylemi** yansıtır. **Eylem gerekliyse** , gerekli bilgileri sağlamak için yukarıdaki adımları tekrarlayın. 

## <a name="create-your-tax-profile"></a>Vergi profilinizi oluşturma

Microsoft 'un kuruluşunuz için gereken vergi bilgilerini sağlamak için aşağıdaki yordamı kullanın. Bu bölümdeki sayfalar dinamiktir ve ülkeniz ya da bölgenize göre değişir. Doğru vergi bilgilerini tanımlamaya yönelik yardıma ihtiyacınız varsa, ülkenizde uygun kamu kaynaklarıyla iletişim kurun.

Kuzey iş ortağı şirketleri için, W8 veya W9 formlarını tamamlamada bilgi almanız gerekiyorsa, aşağıdaki adresler size ıRS sitesine götürür:

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> Şirketiniz için yalnızca ayrıntıları girin. Kişisel ayrıntıları hiçbir şekilde girmeyin.

1. **Iş profili** sayfasında, gerekli alanları tamamlayıp **İleri** ' yi seçin. 

2. **Kurulum** sayfasında, şirketiniz için geçerli olan seçeneği belirleyin.

   - Şirketiniz yalnızca Birleşik Devletler veya bu profil bir bireyin varsa, sol taraftaki seçeneği belirleyin.
   - Şirketinizin Birleşik Devletler dışına dahil olması durumunda sağ taraftaki seçeneği seçin ve ardından listeden bulunduğunuz ülkeyi/bölgenizi seçin.

3. **İleri** ’yi seçin. 

4. **Vergi durumu** sayfasında, gerekli bilgileri girin ve ardından **İleri** ' yi seçin. Bu sayfadaki alanlar ülkeye göre değişiklik gösterecektir. ayrıntılarınız. 

5. **Ek belgeler** sayfasında gerekli alanlar ' ı seçin ve **İleri** ' yi seçin. 

6. Ülkeniz veya bölgeniz için gereken tüm belgeleri karşıya yüklemek için **Araştır** ' ı seçin. Belge adı gösterildiğinde **karşıya yükle** ' yi seçin. 

7. Belgeyi kaldırmanız gerekirse **Kaldır** ' ı seçin.

8. Kaydetmek ve devam etmek için **son** ' u seçin.

9. Açılan iletide **Onayla** ' yı seçin. **Ödeme ve vergi kurulumu** sayfasına geri yönlendirilirsiniz.

## <a name="next-steps"></a>Sonraki adımlar

- [Teşvikleri ödeme ve vergi profili SSS](incentives-payout-tax-profile-faqs.md)
