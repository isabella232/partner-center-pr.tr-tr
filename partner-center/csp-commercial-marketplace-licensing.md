---
title: Market tekliflerini lisanslama yönetme
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: ISV ticari market tekliflerinizi lisanslama ayarlamayı ve yönetmeyi öğrenin.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2d8464b93f6f3215043775496baacc8c6abd907bf614db78725814c9bea59229
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115690911"
---
# <a name="manage-licensing-in-marketplace-offers"></a>Market tekliflerini lisanslama yönetme

**Uygun roller:** Genel yönetici | Hesap yöneticisi

Bu makalede teklif ayarlama, İş Ortağı Merkezi'da kullanılabilir hale Microsoft AppSource ve ardından bu teklifin lisanslarını yönetme işlemi açıklanmıştır.  

>[!IMPORTANT]
>Bu makaledeki özellikler şu anda Genel Önizleme'dedir.

## <a name="before-you-begin"></a>Başlamadan önce

### <a name="commercial-marketplace-basics"></a>Ticari market temelleri

Bu işleme başlamadan önce ticari marketin temellerini tanımanız gerekir. Aşağıdaki tabloda yer alan makaleler, başlamanıza yardımcı olacaktır. 

| Konu  | Makale  |
|-------|--------|
|Ticari market planları | [Ticari market teklifleri için planlar ve fiyatlandırma](/azure/marketplace/plans-pricing)    |
|Ticari market teklifleri  | [Listeleme türleri](/azure/marketplace/determine-your-listing-type)    |
|Ticari market hesapları |  [İş Ortağı Merkezi'de ticari market hesabı oluşturma](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a>Teklif Kimliğinizi belirleme

Aşağıdaki yordamlarda teklif kimliği girmeniz istenir. Uygun bir Teklif Kimliği bulmak için şu noktaları göz atarak biraz zaman atabilirsiniz:

- Bu kimlik, market teklifinin web adresi ve varsa Azure Resource Manager müşteriler tarafından görülebilir.
- Teklif Kimliği, teklif kimliğiyle Publisher 40 karakterden kısa olmalıdır.
- Yalnızca küçük harfleri ve rakamları kullanın. Teklif Kimliği kısa çizgi ve alt çizgi içerebilir ancak boşluk içermez. Örneğin, Publisher kimliğiniz ise `testpublisherid` ve `test-offer-1` girersiniz, teklif web adresi `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` olur.
- Oluştur'ı seçdikten sonra bu kimlik **değiştirilemez.**

### <a name="determine-your-offer-alias"></a>Teklif diğer adını belirleme

Teklif diğer adı, teklifte teklif için kullanılan İş Ortağı Merkezi. Ayrıca aşağıdaki yönergelere uygun bir Teklif diğer adı da gerekir:

- Bu ad markette kullanılmamaktadır ve müşterilere gösterilen teklif adı ile diğer değerlerden farklıdır.
- Oluştur'ı seçdikten sonra bu ad değiştirilemez.

## <a name="create-your-offer"></a>Teklifinizi oluşturma

Lisanslama sürecinin ilk adımı ticari market teklifinizi oluşturmaktır. 

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

Bu adımlarda teklifiniz için etkinleştirmek istediğiniz planı veya planları tanımlayabilirsiniz.

1. Sol gezinti menüsünde Plan'a genel **bakış'ı ve** ardından Yeni plan **oluştur'a tıklayın.**
2. Bir Plan **Kimliği ve** Plan adı **girin ve** oluştur'a **basın.**
3. Plan **listeleme sayfasında** Plan açıklamanızı **girin.**
4. Açıklamayı kaydetmek ve daha sonra tamamlamak için Taslağı **kaydet'i seçin.**

5. Bitirdikten sonra Gözden geçir ve **yayımla'yı seçin.** Plan bilgileri artık teklif listesi (planlar appsource.microsoft.com bölümünde görüntülenir.

6. Bu teklif için tüm planları oluşturduktan sonra, her planın Hizmet Kimliğini kopyalamanız gerekir. Plan **listeleme sayfasının** üst kısmında Plana genel bakış'ı seçin. Her planın Hizmet Kimliğini güvenli bir konuma kopyalayın.

## <a name="add-service-ids-to-your-solution"></a>Çözümünüze Hizmet Kimlikleri ekleme

Sonraki adım, az önce kopyalanan her plan için Hizmet Kimliklerini ekleyerek çözümlerinizi güncelleştirmektir. Bu kılavuz için [bkz. Çözümünüz için AppSource Paketi oluşturma.](/powerapps/developer/data-platform/create-package-app-appsource)

## <a name="upload-your-package-and-publish-your-offer"></a>Upload paketinizi yayımlama ve teklifinizi yayımlama

1. Sol gezinti bölmesinde Ticari **Market'i ve ardından** Teknik **yapılandırma'ı seçin.**
2. Temel **Lisans Modeli'nin altında** Kullanıcı'ya **seçin.**
3. **CRM Paketi'nin** altına paket konumunun URL'sini girin.
4. Gerekli diğer bilgileri girmek için sol gezinti bölmesindeki diğer sekmeleri kullanın. Bitirerek Gözden geçir ve **yayımla'yı seçin.**

Teklifi yayımladikten sonra, bilginizi gözden geçirdikten ve doğrulayana kadar devam ederiz. Bu işlemle ilgili herhangi bir sorun varsa size bildiracağız. Tüm sorunlar çözümlendi mi, teklifinizin AppSource'ta kullanılabilir olduğunu size bildirecek. Bu noktada canlı hale siniz.

## <a name="make-your-offer-live-in-partner-center"></a>Teklifinizi İş Ortağı Merkezi'da canlı hale İş Ortağı Merkezi

Aşağıdaki yordamda teklifinizi AppSource'ta canlı hale uygulama işlemi açıklanmıştır. Bu işlem hakkında daha fazla bilgi edinmek için [bkz. Listeleme seçeneklerine giriş.](/azure/marketplace/determine-your-listing-type)

>[!NOTE]
>Teklifinizi yayımlamanız 4-6 saat sürer.

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.
2. Sol gezinti menüsünde Ticari **Market/Genel Bakış'ı seçin.**
3. Genel **Bakış** sayfasında, istediğiniz teklifi bulun. Yayımlanacak olan tekliflerin Durumu Önizleme **olur.** Teklifi seçin.
4. Teklife **genel bakış sayfasında** Canlı yayına **git'i seçin.**
Teklif 4-6 saat içinde canlı olarak yayınlanacak.
5. Teklif listenizi AppSource'ta görmek için Teklife genel bakış sayfasının en altındaki **AppSource** **bağlantısını** seçin.

    - **Lisans özellikli teklifler için:** Teklifiniz bir lisans denetimi gerektiriyorsa, kullanıcılar yalnızca Benimle İletişime Geç'e tıklayarak müşteri adayı girebilirsiniz, böylece onlarla iletişim kurabilirsiniz.

    - **Ücretsiz yükleme seçeneğine sahip lisans** özellikli teklifler için: Teklifiniz için lisans  denetimi gerekli yoksa, yönetici kullanıcılar Benimle İletişime Geçin'e ek olarak bir Şimdi Al düğmesini **de görebilir.** Ücretsiz yükleme seçeneğinizi denemek isteyen kullanıcıların Şimdi Al'a tıklaması gerekir. Bu seçenek, teklifi Yönetim Merkezi'Power Platform yüklemelerini sağlar. Kullanıcılar, soruları **varsa veya** ücretli bir plana yükseltmek için Benimle İletişime Geçin'i kullanmaya devam ediyor.

## <a name="register-isv-connect-deal-in-deal-registration"></a>Anlaşma Kaydı'Bağlan ISV kayıt anlaşması

Bir müşteriye lisans atamadan önce, her satışın bir müşteriye İş Ortağı Merkezi. Bunu yapmak için [bkz. Anlaşmalarınızı kaydetme.](register-deals.md)

## <a name="invite-the-customer"></a>Müşteriyi davet etme

Müşteriyi bu satış anlaşmasına katılmaya davet etmek için aşağıdaki yordamı kullanın.  

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.
2. Sol gezinti menüsünde Ticari **Market/Genel Bakış'ı seçin.**
3. Sol gezinti menüsünde Referanslar'ı **ve ardından** Anlaşma **Kaydı'ı seçin.**
4. Gönderilen **anlaşmalar için** filtrele, **Devam Ediyor sekmesini** ve ardından istediğiniz anlaşmayı seçin.
5. Bu anlaşmanın genel bakış sayfasında Lisansları **yönet'i seçin.**
6. Lisansları **yönet penceresinde** Müşteri ayrıntıları açılan **listesinden müşteriyi** seçin. Müşteri ilişkisi henüz yoksa onay için +Yeni müşteri **davet et'i seçin.**
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