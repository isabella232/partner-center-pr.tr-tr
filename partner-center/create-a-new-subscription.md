---
title: İş Ortağı Merkezi'de müşteri abonelikleri oluşturma
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Microsoft tarafından yayımlanan ürünler ve üçüncü taraf ISV'ler tarafından yayımlanan SaaS ürünleri için müşterilerinize abonelik satmayı öğrenin.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: f959dfad32fbe1f4f5f71d3dcbdc64f07ee5b901
ms.sourcegitcommit: e1da62b36420d78bf44e3962358d0af65ebc3402
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129089819"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Müşteri aboneliklerini oluşturma, askıya alma veya iptal etme

**Uygulama:** İş Ortağı Merkezi | İş Ortağı Merkezi için Microsoft Cloud for US Government

**Uygun roller:** Yönetici aracısı | Faturalama yöneticisi | Genel yönetici | Yardım masası aracısı | Satış aracısı

Müşterinizin kaydını İş Ortağı Merkezi katalogda ürünlere satabilirsiniz. Bu, üçüncü taraf Bağımsız Yazılım Satıcıları (ISV) tarafından ticari markette yayımlanan Microsoft ve Hizmet Olarak Yazılım (SaaS) ürünleri [tarafından yayımlanan ürünleri içerir.](https://azuremarketplace.microsoft.com/marketplace)

Bazı teklifler müşteri başına bir abonelikle sınırlıdır. Hangi tekliflerin kısıtlanmış olduğunu görmek için Fiyatlandırma ve Teklifler İş Ortağı Merkezi sayfasını ziyaret edin.

> [!IMPORTANT]
> CSP programında bir iş ortağı olarak, lisans tabanlı veya tarifeli **SaaS** aboneliklerini iş ortağınız içindeki ISV yayımcılarından İş Ortağı Merkezi.  Bu, ISV **yayımcının** sizin için sunduğu lisans tabanlı veya tarifeli **SaaS** tekliflerini, erişiminiz olan özel teklifler de dahil olmak üzere satın almak anlamına gelir. [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) ISV'lerden (Azure uygulamaları, Kapsayıcılar veya VM'ler içeren kullanım tabanlı teklifler gibi) diğer ticari market tekliflerini satın almak veya yönetmek için [Azure portal.](https://portal.azure.com/)

> [!NOTE]
> Tüm tarihler ve İş Ortağı Merkezi Evrensel Saat Eşgüdümli (UTC) saat standardını kullanır. Bu, yerel saatle 24 saat arasında farklılık gösterebilir.

## <a name="create-a-new-subscription"></a>Yeni abonelik oluşturma

> [!NOTE]
> Çalışma alanları arabirimi hakkında daha fazla bilgi edinmek için [bkz. İş Ortağı Merkezi.](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Çalışma alanları görünümü](#tab/workspaces-view)

1. Panodan [İş Ortağı Merkezi](https://partner.microsoft.com/dashboard)Müşteri **kutucuğunu** ve ardından Müşteri listesinden müşteriyi seçin.

2. Abonelik **ekle'yi seçin.** Çevrimiçi **Hizmetler sekmesinde** tüm kullanılabilir Market SaaS teklifleri görüntülenir.

3. Yalnızca belirli abonelik türlerini görmek için kullanılabilir filtrelerde seçimler yapın:
   - **Publisher:** Yalnızca **Microsoft'un tekliflerini** görmek için  Microsoft'u veya ISV'ler tarafından yayımlanan ticari market ürünlerini görmek için İş Ortağı'ı seçin.
   - **Faturalama türü:** Kullanmak istediğiniz abonelik faturalama türünü seçin: **Lisans veya** **Kullanım.** Aylık [ve yıllık faturalama sıklığı](license-based-billing.md) arasında karar alamanıza yardımcı olacak bilgiler için bkz. Lisans tabanlı faturalama.
   - **Kategori:** **Enterprise,** **Küçük işletme veya** Deneme'yi **seçin.** Deneme abonelikleri hakkında bilgi için [bkz. Müşterilerinize Microsoft ürünlerinin denemelerini teklif edin.](offer-your-customers-trials-of-microsoft-products.md)

4. Müşteriniz için satın almak istediğiniz ürün aboneliklerini seçin. Gördüğünüz ürünler, müşteri segmenti türüne (eğitim, kamu vb.) ve sizin uyguladık filtrelere bağlıdır. Market'te gösterilen bazı teklifler belirli bir müşteri veya belirli bir CSP iş ortağı tarafından her zaman kullanılabilir olabilir. Bunun nedeni:
   - Müşterinin zaten bu ürüne bir aboneliği vardır ve yalnızca bir aboneliğe izin verilir
   - Müşterinin aboneliği askıya alınmış olabilir (Bu durumda yeni bir abonelik satın almak yerine aboneliği yeniden etkinleştirebilirsiniz.)
   - ISV SaaS tekliflerinin satın alınamama nedenlerinden birkaçı olabilir: ISV müşterinin fatura ülkesi veya bölgesi için destek sunmayabiliyor olabilir; ISV, teklifi CSP programı aracılığıyla kullanılabilir halememiş olabilir; veya ISV teklifi yalnızca belirli CSP [iş](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) ortaklarına özel yapmış olabilir. ISV teklifi, kapsayıcılar veya kullanım tabanlı İş Ortağı Merkezi gibi) aracılığıyla işlem gerçekleştirilebilir de değildir.  

5. Eklemek istediğiniz her abonelik için lisans sayısını girin (gerekirse) ve Sepete **ekle'yi seçin.**

6. Abonelik eklemeyi bitirdikten sonra Siparişinizi gözden **geçir'i** seçin.

7. Siparişlerinizi gözden geçirerek bu abonelikleri satın almaya hazır olduktan sonra Satın Al'ı **seçin.**

8. Bir müşteri için abonelik satın alırsınız, aşağıdakiler gerçekleşir:

    - Müşterinin Abonelikler sayfasından abonelik adını seçerek aboneliği gözden geçirebilirsiniz veya **düzenleyebilirsiniz.** Buradan, varsa eklenti lisanslarını seçin, lisans miktarını değiştirebilir veya aboneliği askıya alın.

    **ISV SaaS (lisans tabanlı ve tarifeli) abonelikler için:**
    - ISV yayımcısı sitesine bir bağlantı alırsınız. Bu bağlantı, müşterinin aboneliğinin dağıtımını veya hesap kurulumunu tamamlamanıza yardımcı olur.

    > [!NOTE]
    > Bu tür bir ISV aboneliği için hesap ayarlamayı/sağlamayı tamamlama yönergelerini içeren bir e-posta ne siz ne de müşteriniz tarafından gönderilir.)

    - Aboneliğiniz 30 günlük ücretsiz deneme sürümüyle geliyorsa, ücretsiz deneme süresi otomatik olarak uygulanır. CSP programında iş ortağı olarak, müşteriler için satın aldığınız tekliflerde ücretsiz deneme süresinden feragatamazsiniz. Ücretsiz deneme süresi sona erdiğinde abonelik dönemi başlar ve abonelik ücretli durumuna dönüştürülür. Abonelik daha sonra aynı zaman çizelgesine göre otomatik olarak yenilenecektir.

#### <a name="current-view"></a>[Geçerli görünüm](#tab/current-view)

1. Panodan [İş Ortağı Merkezi Müşteriler'i](https://partner.microsoft.com/dashboard) ve ardından Müşteri listesinden müşteriyi seçin.

2. Abonelik **ekle'yi seçin.** Çevrimiçi **Hizmetler sekmesinde** tüm kullanılabilir Market SaaS teklifleri görüntülenir.

3. Yalnızca belirli abonelik türlerini görmek için kullanılabilir filtrelerde seçimler yapın:
   - **Publisher:** Yalnızca **Microsoft'un tekliflerini** görmek için  Microsoft'u veya ISV'ler tarafından yayımlanan ticari market ürünlerini görmek için İş Ortağı'ı seçin.
   - **Faturalama türü:** Kullanmak istediğiniz abonelik faturalama türünü seçin: **Lisans veya** **Kullanım.** Aylık [ve yıllık faturalama sıklığı](license-based-billing.md) arasında karar alamanıza yardımcı olacak bilgiler için bkz. Lisans tabanlı faturalama.
   - **Kategori:** **Enterprise,** **Küçük işletme veya** Deneme'yi **seçin.** Deneme abonelikleri hakkında bilgi için [bkz. Müşterilerinize Microsoft ürünlerinin denemelerini teklif edin.](offer-your-customers-trials-of-microsoft-products.md)

4. Müşteriniz için satın almak istediğiniz ürün aboneliklerini seçin. Gördüğünüz ürünler, müşteri segmenti türüne (eğitim, kamu vb.) ve sizin uyguladık filtrelere bağlıdır. Market'te gösterilen bazı teklifler belirli bir müşteri veya belirli bir CSP iş ortağı tarafından her zaman kullanılabilir olabilir. Bunun nedeni:
   - Müşterinin zaten bu ürüne bir aboneliği vardır ve yalnızca bir aboneliğe izin verilir
   - Müşterinin aboneliği askıya alınmış olabilir (Bu durumda yeni bir abonelik satın almak yerine aboneliği yeniden etkinleştirebilirsiniz.)
   - ISV SaaS tekliflerinin satın alınamama nedenlerinden birkaçı olabilir: ISV müşterinin fatura ülkesi veya bölgesi için destek sunmayabiliyor olabilir; ISV, teklifi CSP programı aracılığıyla kullanılabilir halememiş olabilir; veya ISV teklifi yalnızca belirli CSP [iş](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) ortaklarına özel yapmış olabilir. ISV teklifi, kapsayıcılar veya kullanım tabanlı İş Ortağı Merkezi gibi) aracılığıyla işlem gerçekleştirilebilir de değildir.  

5. Eklemek istediğiniz her abonelik için lisans sayısını girin (gerekirse) ve Sepete **ekle'yi seçin.**

6. Abonelik eklemeyi bitirdikten sonra Siparişinizi gözden **geçir'i** seçin.

7. Siparişlerinizi gözden geçirerek bu abonelikleri satın almaya hazır olduktan sonra Satın Al'ı **seçin.**

8. Bir müşteri için abonelik satın alırsınız, aşağıdakiler gerçekleşir:

    - Müşterinin Abonelikler sayfasından abonelik adını seçerek aboneliği gözden geçirebilirsiniz veya **düzenleyebilirsiniz.** Buradan, varsa eklenti lisanslarını seçin, lisans miktarını değiştirebilir veya aboneliği askıya alın.

    **ISV SaaS (lisans tabanlı ve tarifeli) abonelikler için:**
    - ISV yayımcısı sitesine bir bağlantı alırsınız. Bu bağlantı, müşterinin aboneliğinin dağıtımını veya hesap kurulumunu tamamlamanıza yardımcı olur.

    > [!NOTE]
    > Bu tür bir ISV aboneliği için hesap ayarlamayı/sağlamayı tamamlama yönergelerini içeren bir e-posta ne siz ne de müşteriniz tarafından gönderilir.)

    - Aboneliğiniz 30 günlük ücretsiz deneme sürümüyle geliyorsa, ücretsiz deneme süresi otomatik olarak uygulanır. CSP programında iş ortağı olarak, müşteriler için satın aldığınız tekliflerde ücretsiz deneme süresinden feragatamazsiniz. Ücretsiz deneme süresi sona erdiğinde abonelik dönemi başlar ve abonelik ücretli durumuna dönüştürülür. Abonelik daha sonra aynı zaman çizelgesine göre otomatik olarak yenilenecektir.

* * *

## <a name="update-subscriptions-with-add-ons"></a>Eklentilerle abonelikleri güncelleştirme

Eklenti satın almak için müşterinin önce etkin bir temel aboneliği olması gerekir.  Eklentileri katalog aracılığıyla satın alamazsınız.

1. İş Ortağı Merkezi [oturum açın.](https://partner.microsoft.com/dashboard)

2. Yeni İş Ortağı Merkezi **Müşteriler'i** ve ardından listeden bir müşteri seçin.

3. Yönetmek istediğiniz aboneliği seçin.

4. Durum **bölümünün** altında, abonelik için kullanılabilir Eklentilerin listesi yer almaktadır.  

5. Gerekli her Eklenti için lisans miktarını güncelleştirin. Sonra **Gönder** ile yaptığınız değişiklikleri gönderin.

Yalnızca doğrudan fatura ve dolaylı sağlayıcılar İş Ortağı Merkezi eklenti satın alma özelliğine sahip olabilir.
Yalnızca uygun eklentiler temel gereksinimlere ve bölgesel kullanılabilirlik durumuna göre görüntülenir. Fiyatlandırma ve teklifler hakkında daha fazla bilgi için Bulut Kurumsal Bayi teklif matrisi'ne bakın. Temel abonelik askıya alındığında ilişkili tüm eklentiler de askıya alınır.

Eklentilerin başlangıç tarihleri temel abonelikle uyumludur; ücretler Ücret başlangıç tarihi ile Ücret bitiş tarihi kullanılarak hesaplanır ve ilk faturaya orantılı bir ücret uygulanır. Daha fazla bilgi için [bkz. Lisans tabanlı faturalama.](license-based-billing.md)


## <a name="suspend-or-cancel-a-subscription"></a>Aboneliği askıya alma veya iptal etme

İş ortakları, müşteri tarafından talep edilmesi ya da ödememe veya sahtekarlık durumlarında aboneliği askıya alabilir veya iptal edebilir.

### <a name="suspend-a-subscription"></a>Bir aboneliği askıya alma

Aboneliğin durumunu Askıya Alındı olarak **değiştirebilirsiniz.** Kullanıcılar oturum alamiyor veya hizmetlere erişemiyor.

1. İş Ortağı Merkezi [oturum açın.](https://partner.microsoft.com/dashboard)

2. Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve listeden bir müşteri seçin.

3. Yönetmek istediğiniz aboneliği seçin.

4. **Durum** bölümünde **Askıya Alındı**'yı seçin. Sonra **Gönder** ile yaptığınız değişiklikleri gönderin.

5. Abonelik 90 gün içinde yeniden etkinleştirilmediği veya 90 gün ile hesabın açıldığı zaman arasındaki gün sayısı ile ilk fatura dönemi (maksimum 120 gün) arasında tüm veriler silinir.

Bir aboneliği askıya aldığınızda, **askıya alınmış** düğmesinin altında gördüğünüz Tarih, yeniden etkinleştirmezseniz aboneliğin otomatik olarak ne zaman dolacağını gösterir. 

>[!NOTE]
>CSP aboneliklerinin süresi, hizmetin hala çalıştığı ancak aboneliğin fatura ücreti üretmeyen süresi olmayan bir döneme (Web-Direct aboneliklerinin yapması) sahip değildir. CSP abonelikleri etkin veya askıya alındı (ya da tamamen silinmiş).

### <a name="cancel-a-subscription"></a>Aboneliği iptal et

Iş Ortağı Merkezi [ticari marketi](csp-commercial-marketplace-overview.md)kapsamındaki üçüncü taraf ISV yayımcılarından lisans tabanlı SaaS aboneliklerini iptal edebilirsiniz. İptal dönemi içinde iptal ettiğiniz sürece, tam bir para iadesi alırsınız.

Aylık olarak faturalandırılan ISV teklifleri için:

- Siparişi yerleştirdikten sonra 24 saatten az iptal ederseniz bir sonraki faturada bir tam kredi alacaksınız.

- Siparişi yerleştirdikten sonra 24 saatten sonra iptal ederseniz, iptal etme, yenileme sırasında gerçekleşecek şekilde zamanlanır.

Yıllık olarak faturalandırılan teklifler için:

- Siparişi girdikten sonra 14 günden daha az bir süre sonra iptal ederseniz, sonraki faturada bir tam kredi alırsınız.

- Siparişi girdikten sonra 14 günden daha sonra iptal ederseniz iptali, yenileme sırasında gerçekleşecek şekilde zamanlanır.

Bu dönemler bittikten sonra, aboneliği iptal etme seçeneğini artık göremezsiniz.

> [!NOTE]
> Kullanım tabanlı ve tarifeli, üçüncü taraf ISV Hizmetleri (örneğin, sanal makineleri veya kapsayıcıları kullanan), return için uygun değildir. Kullanım tabanlı hizmetler, iptal yöntemi olarak geçersiz bir şekilde sağlanabilir. Ücretler kullanım sonrasında faturalandırıladıklarından, bu hizmetler para iadesi için uygun değildir.

Lisans tabanlı bir SaaS aboneliğini ISV yayımcısından iptal etmek için aşağıdakileri yapın:

1. Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.

2. Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve listeden bir müşteri seçin.

3. İptal etmek istediğiniz aboneliği bulun.

4. **Durum** sütununda **iptal**' i seçin. Sonra **Gönder** ile yaptığınız değişiklikleri gönderin.

5. Bir iletişim kutusu görüntülenirse, ilgili ayrıntıları doldurun ve **Gönder**' i seçin.

6. İptali onaylamak için **Evet, iptal**' i seçin.

> [!NOTE]
> Ayrıca API 'Leri kullanarak bir Azure Marketi aboneliğini iptal etmeyi seçebilirsiniz. Bunu yapmak için bkz. [Azure Marketi aboneliğini Iptal etme](/partner-center/develop/cancel-an-azure-marketplace-subscription).

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>Bir ticari Market aboneliğinin otomatik olarak yenilenip yenilenmeyeceğini seçin

Etkin abonelikler varsayılan olarak abonelik süresi sona erdiğinde otomatik olarak yenilenecek şekilde ayarlanır. [Ticari Market ürünlerine yönelik abonelikler](csp-commercial-marketplace-overview.md)için, isteğe bağlı olarak, aboneliği otomatik olarak yenilemeyi seçebilirsiniz.

Etkin bir ticari Market aboneliğini otomatik olarak yenilemeyi durdurmak için:

1. Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.

2. Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve listeden bir müşteri seçin.

3. **Abonelikler**'i seçin. Bu, müşteri için satın aldığınız lisans tabanlı abonelikleri listeler.

4. **Abonelik** sütununda, değiştirmek istediğiniz aboneliği seçin.

5. Abonelik Ayrıntıları sayfasında, **durum** bölümünü bulun ve **Otomatik Yenile** kutusunun işaretini kaldırın.

6. **Gönder**’i seçin.

## <a name="next-steps"></a>Sonraki adımlar

- [Müşterileriniz için ticari Market ürünleri satın alın](csp-commercial-marketplace-purchase.md)

- [Müşterileriniz için ticari Market ürünlerini yönetme](csp-commercial-marketplace-manage.md)

- [Ticari markete genel bakış](csp-commercial-marketplace-overview.md)