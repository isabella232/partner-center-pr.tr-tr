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
ms.openlocfilehash: 416bf2804eeb796109f538c109f8087006d7c9da
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129072326"
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
> İş Ortağı Merkezi önizleme arabirimi, mantıksal olarak gruplu çalışma alanları aracılığıyla daha verimli ve üretken bir kullanıcı deneyimi sağlar. Çalışma alanları arabirimi ve bu arabirimi açma hakkında daha fazla bilgi edinmek için [bkz. İş Ortağı Merkezi.](get-around-partner-center.md#turn-workspaces-on-and-off)

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

2. Yeni İş Ortağı Merkezi Müşteriler'i **ve** ardından listeden bir müşteri seçin.

3. Yönetmek istediğiniz aboneliği seçin.

4. **Durum** bölümünde **Askıya Alındı**'yı seçin. Sonra **Gönder** ile yaptığınız değişiklikleri gönderin.

5. Abonelik 90 gün veya 90 gün içinde yeniden etkinleştirildiği sürece tüm veriler silinir ve hesabın açılmasıyla ilk faturalama dönemi (en fazla 120 gün) arasındaki gün sayısı.

Bir aboneliği askıya alırsanız, Askıya Alındı düğmesinin altında gördüğünüz tarih, aboneliği yeniden etkinleştirmezsanız aboneliğin süresinin otomatik olarak ne zaman dol olacağını gösterir.  

>[!NOTE]
>CSP abonelikleri, hizmetlerin çalışmaya devam eder ancak abonelik herhangi bir faturalama ücreti oluşturmazken süresi dolmuş bir süreye (doğrudan web abonelikleri gibi) sahip değildir. CSP abonelikleri etkin veya askıya alınmış (veya tamamen silinmiş).

### <a name="cancel-a-subscription"></a>Aboneliği iptal etme

Ticari market içindeki üçüncü taraf ISV yayımcılarından lisans tabanlı SaaS aboneliklerini İş Ortağı Merkezi [edebilirsiniz.](csp-commercial-marketplace-overview.md) İptal süresi içinde iptal edersiniz, tam para iadesi alırsınız.

Aylık olarak faturalandırılan ISV teklifleri için:

- Siparişi verdikten 24 saatten az bir süre sonra iptal edersiniz, sonraki faturada tam kredi alırsınız.

- Siparişi verdikten 24 saat sonra iptal edersiniz, iptal işlemi yenileme sırasında yapılacak şekilde zamanlanmış olur.

Yıllık olarak faturalandırılan teklifler için:

- Siparişi verdikten 14 gün sonra iptal edersiniz, sonraki faturada tam kredi alırsınız.

- Siparişi verdikten 14 gün sonra iptal edersiniz, iptal işlemi yenileme sırasında yapılacak şekilde zamanlanmış olur.

Bu süreler sona erdikten sonra aboneliği iptal etme seçeneğini artık göremeyeceksiniz.

> [!NOTE]
> Kullanım tabanlı ve tarifeli, üçüncü taraf ISV hizmetleri (örneğin, sanal makineleri veya kapsayıcıları kullananlar) iade için uygun değildir. Kullanım tabanlı hizmetler bir iptal yöntemi olarak kullanımdan silindi. Ücretler kullanımdan sonra faturalandırılana bu hizmetler para iadesi için uygun değildir.

Lisans tabanlı bir SaaS aboneliğini ISV yayımcısından iptal etmek için aşağıdakileri yapın:

1. İş Ortağı Merkezi [oturum açın.](https://partner.microsoft.com/dashboard)

2. Yeni İş Ortağı Merkezi Müşteriler'i **ve** ardından listeden bir müşteri seçin.

3. İptal etmek istediğiniz aboneliği bulun.

4. Durum sütununda **İptal'i** **seçin.** Sonra **Gönder** ile yaptığınız değişiklikleri gönderin.

5. İletişim kutusu görüntülenirse ilgili ayrıntıları doldurun ve Gönder'i **seçin.**

6. İptali onaylamak için Evet, iptal **et'i seçin.**

> [!NOTE]
> Api'leri kullanarak bir Azure Market aboneliğini iptal edebilirsiniz. Bunu yapmak için [bkz. Azure Market aboneliğini iptal etme.](/partner-center/develop/cancel-an-azure-marketplace-subscription)

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>Ticari market aboneliğinin otomatik olarak yenilenip yenilenmayacaklarını seçme

Etkin abonelikler varsayılan olarak abonelik süresi sona erdiğinde otomatik olarak yenilenecek şekilde ayarlanır. Ticari [market ürünlerine abonelikler için](csp-commercial-marketplace-overview.md)isteğe bağlı olarak aboneliği otomatik olarak yenilemeyi seçebilirsiniz.

Etkin bir ticari market aboneliğinin otomatik olarak yenilenmesini durdurmak için:

1. İş Ortağı Merkezi [oturum açın.](https://partner.microsoft.com/dashboard)

2. Yeni İş Ortağı Merkezi Müşteriler'i **ve** ardından listeden bir müşteri seçin.

3. **Abonelikler**'i seçin. Bu, müşteri için satın aldığınız lisans tabanlı abonelikleri listeler.

4. Abonelik **sütununda** değiştirmek istediğiniz aboneliği seçin.

5. Abonelik ayrıntıları sayfasında Durum bölümünü **bulun ve** Otomatik yenile **kutusunun işaretini** kaldırın.

6. **Gönder**’i seçin.

## <a name="next-steps"></a>Sonraki adımlar

- [Müşterileriniz için ticari market ürünleri satın alma](csp-commercial-marketplace-purchase.md)

- [Müşterileriniz için ticari market ürünlerini yönetme](csp-commercial-marketplace-manage.md)

- [Ticari markete genel bakış](csp-commercial-marketplace-overview.md)