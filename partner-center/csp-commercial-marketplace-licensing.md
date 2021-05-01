---
title: Market teklifte lisanslamayı yönetme
ms.topic: how-to
ms.date: 04/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: ISV ticari Market tekliflerinizi için lisanslamayı ayarlamayı ve yönetmeyi öğrenin.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3b2281696a2fe69253cd033eb2a7eef7fb3046f3
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284894"
---
# <a name="manage-licensing-in-marketplace-offers"></a>Market teklifte lisanslamayı yönetme

**Uygun roller**

- Genel yönetici
- Hesap yöneticisi

Bu makalede, Iş Ortağı Merkezi 'nde bir teklif ayarlama, Microsoft AppSource ' de kullanılabilir hale getirme ve ardından bu teklifin lisanslarını yönetme sürecinde size yol gösterilir.  

>[!IMPORTANT]
>Bu makaledeki yetenekler Şu anda genel önizlemededir.

## <a name="before-you-begin"></a>Başlamadan önce

Bu işleme başlamadan önce, aşağıdaki bilgileri öğrenmeniz gerekir.

### <a name="review-the-azure-marketplace-documentation"></a>Azure Marketi belgelerini gözden geçirin

Aşağıdaki makalelerde, devam etmeden önce bilmeniz gereken bilgiler yer almalıdır. 

- [Dynamics 365 for Customer Engagement ve PowerApps teklifi oluşturma](https://docs.microsoft.com/azure/marketplace/dynamics-365-customer-engage-offer-setup)
- [Iş Ortağı Merkezi 'nde ticari Market hesabı oluşturma](https://docs.microsoft.com/azure/marketplace/create-account)

### <a name="create-your-offer-id"></a>Teklif KIMLIĞINIZI oluşturma

Aşağıdaki yordamlarda bir teklif KIMLIĞI girmeniz istenir. Aşağıdaki noktaları göz önünde bulundurarak uygun bir teklif KIMLIĞIYLE karşılaşmaya biraz zaman atın:

- Bu KIMLIK, varsa Market teklifi ve Azure Resource Manager şablonları için Web adresinde müşteriler tarafından görülebilir.
- Yayımcı KIMLIĞIYLE birleştirilmiş teklif KIMLIĞI, 40 karakter uzunluğunda olmalıdır.
- Yalnızca küçük harfleri ve rakamları kullanın. Teklif KIMLIĞI, kısa çizgiler ve alt çizgiler içerebilir ancak boşluk içeremez. Örneğin, yayımcı KIMLIĞINIZ testpublisherıd ise ve test-teklif-1 girerseniz, teklif Web adresi olur https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1 .
- Bu KIMLIK, **Oluştur**' u seçtikten sonra değiştirilemez.

### <a name="create-your-offer-alias"></a>Teklif diğer adınızı oluşturma

Teklif diğer adı, Iş Ortağı Merkezi 'nde teklif için kullanılan addır. Ayrıca, aşağıdaki yönergeleri takip eden uygun bir teklif diğer adına ihtiyacınız olacaktır:

- Bu ad Market 'te kullanılmıyor ve teklif adından ve müşterilere gösterilen diğer değerlerden farklı.
- Bu ad, Oluştur ' u seçtikten sonra değiştirilemez.

## <a name="create-your-offer"></a>Teklifinizi oluşturma

Lisanslama sürecinin ilk adımı, ticari Market teklifinizi oluşturmaktır. 

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.
2. Sol gezinti menüsünde **ticari Market/genel bakış**' ı seçin.
3. Genel Bakış sayfasının üst kısmında, **yeni teklif**' i seçin ve ardından Dynamics 365 ' i seçerek **& PowerApps**' i seçin.
4. Daha önce oluşturduğunuz **TEKLIF kimliği** ve **teklif diğer adını** girin.
5. Teklifi oluşturmak için **Oluştur** ' u seçin ve devam edin.
6. Lisanslama seçeneklerinizi belirleyin.

    - Teklifiniz için lisans yönetimini etkinleştirmek üzere **Microsoft aracılığıyla uygulama lisans yönetimini etkinleştir**' i seçin. Bu bir kerelik bir ayardır ve teklifiniz yayımlandıktan sonra bu ayarı değiştiremezsiniz.

    - Ayrıca, müşterilerin bir lisans olmadan uygulamanızın temel işlevselliğini çalıştırmasına ve bir lisans satın aldıktan sonra Premium özellikleri çalıştırmasına olanak sağlayabilirsiniz. Bunu yapmak için, **lisanslar atanmasa bile müşterilerin uygulamamı yüklemesine Izin ver**' i seçin.

    - Teklifinizin lisans yönetimi 'nin etkinleştirilmesini istemiyorsanız, **Şimdi al (ücretsiz)**, **ücretsiz deneme** veya **benimle iletişim kurun**' i seçin.

## <a name="create-your-plan"></a>Planınızı oluşturma

Bu adımlarda, teklifiniz için etkinleştirmek istediğiniz planı veya planları tanımlayacaksınız.

1. Sol gezinti menüsünde **plana genel bakış**' ı seçin ve ardından **Yeni plan oluştur**' u seçin.
2. Bir **plan kimliği** ve **Plan adı** girin ve ardından **Oluştur**' u seçin.
3. **Plan listeleme** sayfasında **plan açıklamanızı** girin.
4. Açıklamayı kaydetmek ve daha sonra sona ermesini sağlamak için **Taslağı kaydet**' i seçin.

5. İşiniz bittiğinde, **gözden geçir ve Yayımla**' yı seçin. Plan bilgileri artık teklif listesi (planlar bölümü) altında appsource.microsoft.com üzerinde görüntülenir.

6. Bu teklif için tüm planları oluşturduktan sonra, her planın hizmet KIMLIĞINI kopyalamanız gerekir. Plan listesi sayfasının en üstünde **plana genel bakış ' ı** seçin. Her planın hizmet KIMLIĞINI güvenli bir konuma kopyalayın.

## <a name="add-service-ids-to-your-solution"></a>Çözümünüze hizmet kimlikleri ekleyin

Bir sonraki adım, yeni kopyaladığınız her plana ait hizmet kimliklerini ekleyerek çözümünüzü güncelleştirmedir. Bunun hakkında yönergeler için bkz. [çözümünüz Için AppSource paketi oluşturma](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).

## <a name="upload-your-package-and-publish-your-offer"></a>Paketinizi karşıya yükleyin ve teklifinizi yayımlayın

1. Sol gezinti bölmesinde, **ticari Market**' i seçin ve ardından **Teknik yapılandırma**' yı seçin.
2. **Temel lisans modeli** altında **Kullanıcı**' yı seçin.
3. **CRM paketi** altında, paket KONUMLARıNıZıN URL 'sini girin.
4. Diğer gerekli bilgileri girmek için sol gezinti bölmesindeki diğer sekmeleri kullanın. İşiniz bittiğinde, **gözden geçir ve Yayımla**' yı seçin.

Teklifi yayımladıktan sonra bilgilerinizi gözden geçireceğiz ve doğrulayacağız. Bu işlemle ilgili herhangi bir sorun varsa sizi bilgilendireceğiz. Tüm sorunlar çözümlendikten sonra teklifinizin AppSource 'ta kullanılabildiğini belirten bir bildirim alırsınız. Bu noktada, onu canlı hale getirebilirsiniz.

## <a name="make-your-offer-live-in-partner-center"></a>Teklifinizi Iş Ortağı Merkezi 'nde canlı hale getirin

Aşağıdaki yordam, teklifinizi AppSource 'ta canlı hale getirme sürecinde size yol gösterir. Bu işlem hakkında daha fazla bilgi edinmek için bkz. [listeye giriş seçenekleri](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).

>[!NOTE]
>Teklifinizi yayımladıktan sonra, bu işlem 4-6 saat sürer.

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.
2. Sol gezinti menüsünde **ticari Market/genel bakış**' ı seçin.
3. **Genel bakış** sayfasında, aradığınız teklifi bulun. Yayımlanmaya hazırlanma teklifleri **Önizleme** durumuna sahip olur. Teklifi seçin.
4. **Teklifin genel bakış** sayfasında **canlı git**' i seçin.
Teklif 4-6 saat içinde etkin olacaktır.
5. AppSource 'ta teklif listelemeyi görmek için, **teklif genel bakış** sayfasının alt kısmındaki **appsource** bağlantısını seçin.

    - **Lisans etkin teklifler için**: teklifiniz bir lisans denetimi gerektiriyorsa, kullanıcılar bu kişilerle iletişim kurabilmesi Için yalnızca **benimle iletişim** kuracak bir müşteri adayı girebilecektir.

    - **Ücretsiz yükleme seçeneğiyle lisans etkin teklifler için**: teklifiniz bir lisans denetimi gerektirmiyorsa, yönetici kullanıcılar **bana başvurmaya** ek olarak **Şimdi bir şimdi al** düğmesine sahip olur. Ücretsiz yükleme seçeneğinizi denemek isteyen kullanıcılar **Şimdi al**' a tıklamalıdır, bu, teklifi Power platform yönetim merkezine yüklemeye getirir. Kullanıcılar, herhangi bir sorunuz varsa veya ücretli bir plana yükseltmek istediklerinde **benimle Iletişim kurma** 'yı kullanmaya devam edebilir.

## <a name="register-isv-connect-deal-in-dealreg"></a>Satıcılarla ilgili ISV bağlantısı anlaşmayı Kaydet

Bir sonraki adım, anlaşmayı kaydetmenizi sağlar. Bunu yapmak için bkz. [anlaşmaları kaydetme](https://docs.microsoft.com/partner-center/register-deals).

## <a name="invite-the-customer"></a>Müşteriyi davet etme

Müşteriyi bu başa katılmaya davet etmek için aşağıdaki yordamı kullanın.  

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.
2. Sol gezinti menüsünde **ticari Market/genel bakış**' ı seçin.
3. **Gönderilen** anlaşmalar için filtre uygulayın, **devam eden** sekmesini seçin ve ardından istediğiniz anlaşmayı seçin.
4. Bu anlaşma için genel bakış sayfasında **Lisansları Yönet**' i seçin.
5. **Lisansları Yönet** penceresinde müşteri **ayrıntıları** açılır listesinden müşteriyi seçin. Müşteri ilişkisi henüz yoksa, **+ Yeni müşteriyi onay olarak davet et**' i seçin.
6. Görüntülenen bağlantıyı kopyalayın.
7. Bu bağlantıyı, müşterinizin faturalandırma Yöneticisi veya genel yöneticisine e-posta ile gönderin ve bu bağlantıyı admin.microsoft.com erişmek ve oluşturduğunuz ilişkiyi kabul etmek ve yetkilendirmek için kullanın.

    >[!NOTE]
    >Müşteri bu adımı gerçekleştirene kadar ilişki kurulmayacak.

## <a name="activate-manage-and-remove-your-licenses"></a>Lisanslarınızı etkinleştirin, yönetin ve kaldırın

Müşteriniz kurulduktan sonra, teklifinizden planlar eklemeye başlayabilir ve her plana lisans atayabilirsiniz.

1. Bu anlaşma için Lisansları Yönet penceresinde **+ plan Ekle**' yi seçin.
2. **Bu çözüm Için planları** ve lisans alanı **sayısını** tamamlayıp **Lisansları Güncelleştir**' i seçin. Lisanslar, müşteriler tarafından yönetilecek ve çalışanlara atanacak admin.microsoft.com adresinde kullanılabilir.

    - Mevcut bir planın lisans sayısını değiştirmek için, **Lisans sayısı** alanına yeni sayıyı girin ve ardından **Lisansları Güncelleştir**' i seçin.

    - Bir anlaşma için lisansları devre dışı bırakmak veya kaldırmak için, **Eylemler** alanındaki çöp kutusu simgesini seçin ve ardından **Lisansları Güncelleştir**' i seçin.