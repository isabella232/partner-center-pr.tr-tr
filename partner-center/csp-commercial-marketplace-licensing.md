---
title: Market teklifte lisanslamayı yönetme
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: ISV ticari Market tekliflerinizi için lisanslamayı ayarlamayı ve yönetmeyi öğrenin.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c128b99b034564bcaa100ca975253f8b1bad7a42
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147964"
---
# <a name="manage-licensing-in-marketplace-offers"></a>Market teklifte lisanslamayı yönetme

**Uygun roller**: genel yönetici | Hesap Yöneticisi

Bu makalede, Iş Ortağı Merkezi 'nde bir teklif ayarlama, Microsoft AppSource ' de kullanılabilir hale getirme ve ardından bu teklifin lisanslarını yönetme sürecinde size yol gösterilir.  

>[!IMPORTANT]
>Bu makaledeki yetenekler Şu anda genel önizlemededir.

## <a name="before-you-begin"></a>Başlamadan önce

### <a name="commercial-marketplace-basics"></a>Ticari Market temelleri

Bu işleme başlamadan önce, ticari Market 'in temelleri hakkında bilgi almalısınız. Aşağıdaki tablodaki makaleler başlamanıza yardımcı olur. 

| Konu  | Makale  |
|-------|--------|
|Ticari Market planları | [Ticari Market teklifleri için planlar ve fiyatlandırma](/azure/marketplace/plans-pricing)    |
|Ticari Market teklifleri  | [Liste türleri](/azure/marketplace/determine-your-listing-type)    |
|Ticari Market hesapları |  [Iş Ortağı Merkezi 'nde ticari Market hesabı oluşturma](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a>Teklif KIMLIĞINIZI belirleme

Aşağıdaki yordamlarda bir teklif KIMLIĞI girmeniz istenir. Aşağıdaki noktaları göz önünde bulundurarak uygun bir teklif KIMLIĞIYLE karşılaşmaya biraz zaman atın:

- Bu KIMLIK, varsa Market teklifi ve Azure Resource Manager şablonları için Web adresinde müşteriler tarafından görülebilir.
- Yayımcı KIMLIĞIYLE birleştirilmiş teklif KIMLIĞI, 40 karakter uzunluğunda olmalıdır.
- Yalnızca küçük harfleri ve rakamları kullanın. Teklif Kimliği kısa çizgi ve alt çizgi içerebilir ancak boşluk içermez. Örneğin, Yayımcı Kimliğiniz ise ve `testpublisherid` `test-offer-1` girersiniz, teklif web adresi `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` olur.
- Oluştur'ı seçdikten sonra bu kimlik **değiştirilemez.**

### <a name="determine-your-offer-alias"></a>Teklif diğer adını belirleme

Teklif diğer adı, teklifte teklif için kullanılan İş Ortağı Merkezi. Ayrıca aşağıdaki yönergelere uygun bir Teklif diğer adı da gerekir:

- Bu ad markette kullanılmamaktadır ve müşterilere gösterilen teklif adı ile diğer değerlerden farklıdır.
- Oluştur'ı seçdikten sonra bu ad değiştirilemez.

## <a name="create-your-offer"></a>Teklifinizi oluşturma

Lisanslama sürecinin ilk adımı, ticari market teklifinizi oluşturmaktır. 

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.
2. Sol gezinti menüsünde Ticari **Market/Genel Bakış'ı seçin.**
3. Genel Bakış sayfasının üst kısmında Yeni **teklif'i** seçin ve ardından **Dynamics 365 for Customer Engagement & PowerApps'i seçin.**
4. Daha önce **oluşturduğunuz Teklif** Kimliği ve **Teklif diğer** adını girin.
5. Teklifi **oluşturmak ve** devam etmek için Oluştur'a seçin.
6. Lisanslama seçeneklerinizi belirleyin.

    - Teklifiniz için lisans yönetimini etkinleştirmek için Microsoft aracılığıyla **uygulama lisans yönetimini etkinleştir'i seçin.** Bu tek seferlik bir ayardır ve teklifiniz yayımlandıktan sonra bunu değiştiremezsiniz.

    - Ayrıca, müşterilerin uygulama temel işlevselliğini lisans olmadan çalıştırmasını ve lisans satın alan premium özellikleri çalıştırmasını da sebilirsiniz. Bunu yapmak için Lisans **atanmasa bile müşterilerin uygulamamı yüklemesine izin ver'i seçin.**

    - Teklifinizin lisans yönetiminin etkinleştirilmesi istemiyorsanız Şimdi al **(Ücretsiz)** **,** Ücretsiz deneme veya Bana ulaşın'ı **seçin.**

## <a name="create-your-plan"></a>Planınızı oluşturma

Bu adımlarda, teklifiniz için etkinleştirmek istediğiniz planı veya planları tanımlayacaksınız.

1. Sol gezinti menüsünde **plana genel bakış**' ı seçin ve ardından **Yeni plan oluştur**' u seçin.
2. Bir **plan kimliği** ve **Plan adı** girin ve ardından **Oluştur**' u seçin.
3. **Plan listeleme** sayfasında **plan açıklamanızı** girin.
4. Açıklamayı kaydetmek ve daha sonra sona ermesini sağlamak için **Taslağı kaydet**' i seçin.

5. İşiniz bittiğinde, **gözden geçir ve Yayımla**' yı seçin. Plan bilgileri artık teklif listesi (planlar bölümü) altında appsource.microsoft.com üzerinde görüntülenir.

6. Bu teklif için tüm planları oluşturduktan sonra, her planın hizmet KIMLIĞINI kopyalamanız gerekir. Plan listesi sayfasının en üstünde **plana genel bakış ' ı** seçin. Her planın hizmet KIMLIĞINI güvenli bir konuma kopyalayın.

## <a name="add-service-ids-to-your-solution"></a>Çözümünüze hizmet kimlikleri ekleyin

Bir sonraki adım, yeni kopyaladığınız her plana ait hizmet kimliklerini ekleyerek çözümünüzü güncelleştirmedir. Bunun hakkında yönergeler için bkz. [çözümünüz Için AppSource paketi oluşturma](/powerapps/developer/data-platform/create-package-app-appsource).

## <a name="upload-your-package-and-publish-your-offer"></a>Paketinizi karşıya yükleyin ve teklifinizi yayımlayın

1. Sol gezinti bölmesinde, **ticari Market**' i seçin ve ardından **Teknik yapılandırma**' yı seçin.
2. **Temel lisans modeli** altında **Kullanıcı**' yı seçin.
3. **CRM paketi** altında, paket KONUMLARıNıZıN URL 'sini girin.
4. Diğer gerekli bilgileri girmek için sol gezinti bölmesindeki diğer sekmeleri kullanın. İşiniz bittiğinde, **gözden geçir ve Yayımla**' yı seçin.

Teklifi yayımladıktan sonra bilgilerinizi gözden geçireceğiz ve doğrulayacağız. Bu işlemle ilgili herhangi bir sorun varsa sizi bilgilendireceğiz. Tüm sorunlar çözümlendikten sonra teklifinizin AppSource 'ta kullanılabildiğini belirten bir bildirim alırsınız. Bu noktada, onu canlı hale getirebilirsiniz.

## <a name="make-your-offer-live-in-partner-center"></a>Teklifinizi Iş Ortağı Merkezi 'nde canlı hale getirin

Aşağıdaki yordam, teklifinizi AppSource 'ta canlı hale getirme sürecinde size yol gösterir. Bu işlem hakkında daha fazla bilgi edinmek için bkz. [listeye giriş seçenekleri](/azure/marketplace/determine-your-listing-type).

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

## <a name="register-isv-connect-deal-in-deal-registration"></a>ISV Connect 'in anlaşmayı kayda kaydetme

Bir müşteriye lisans atayabilmeniz için önce her satışın Iş Ortağı Merkezi 'ne kaydedilmesi gerekir. Bunu yapmak için [bkz. Anlaşmalarınızı kaydetme.](register-deals.md)

## <a name="invite-the-customer"></a>Müşteriyi davet etme

Müşteriyi bu satış anlaşmasına katılmaya davet etmek için aşağıdaki yordamı kullanın.  

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.
2. Sol gezinti menüsünde Ticari **Market/Genel Bakış'ı seçin.**
3. Sol gezinti menüsünde Referanslar'ı **ve ardından** Anlaşma **Kaydı'ı seçin.**
4. Gönderilen **anlaşmalar için** filtrele, **Devam Ediyor sekmesini** ve ardından istediğiniz anlaşmayı seçin.
5. Bu anlaşmayı genel bakış sayfasında Lisansları **yönet'i seçin.**
6. Lisansları **yönet penceresinde** Müşteri ayrıntıları açılan **listesinden** müşteriyi seçin. Müşteri ilişkisi henüz yoksa onay için +Yeni müşteri **davet et'i seçin.**
7. Görüntülenen bağlantıyı kopyalayın.
8. Bu bağlantıyı müşterinizin faturalama yöneticisine veya genel yöneticisine e-posta ile gönderin ve bu bağlantıyı kullanarak admin.microsoft.com ilişkileri kabul etmelerini ve yetkilendirmelerini snın.

    >[!NOTE]
    >Müşteri bu adımı gerçekleştirene kadar ilişki kurulmayacak.

## <a name="activate-manage-and-remove-your-licenses"></a>Lisanslarınızı etkinleştirme, yönetme ve kaldırma

Müşteriniz size ilişkinin yetkilerini verdiktan sonra teklifinizin planlarını eklemeye ve her plana lisans atamaya başlayabilirsiniz.

1. Bu anlaşma için Lisansları yönet penceresinde **+Plan ekle'yi seçin.**
2. Bu çözüm **için planlar ve Lisans** sayısı alanlarını **doldurun** ve ardından Lisansları **güncelleştir'i seçin.** Lisanslar, müşterilerin admin.microsoft.com atanmalarını sağlamak için şirket içinde kullanılabilir.

    - Mevcut bir planın lisans sayısını değiştirmek için Lisans sayısı  alanına yeni numarayı girin ve Lisansları **güncelleştir'i seçin.**

    - Bir anlaşma için lisansları devre dışı bırakmak veya kaldırmak için Eylemler alanında çöp kutusu **simgesini ve** ardından Lisansları **güncelleştir'i seçin.**

## <a name="next-steps"></a>Sonraki adımlar

[Lisanslama kaynakları](support-resources-licensing.md)