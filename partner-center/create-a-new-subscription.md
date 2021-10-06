---
title: Iş Ortağı Merkezi 'nde müşteri abonelikleri oluşturma
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Microsoft tarafından yayımlanan ürünlerin yanı sıra üçüncü taraf ISV 'Ler tarafından yayımlanan SaaS ürünleri için müşterilerinize abonelik satma hakkında bilgi edinin.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: c42e2e8dbc98bdf9ed0e2994bfb7ad49848aad76
ms.sourcegitcommit: b78e85a0bc62e3536b067417cb3db7899cda4f97
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/06/2021
ms.locfileid: "129565340"
---
# <a name="manage-customer-subscriptions"></a>Müşteri aboneliklerini yönetme

**Uygulama hedefi**: Iş Ortağı Merkezi | Microsoft Cloud for US Government için iş ortağı Merkezi

**Uygun roller**: yönetici Aracısı | Faturalandırma Yöneticisi | Genel yönetici | Yardım Masası Aracısı | Satış Aracısı

Iş Ortağı Merkezi 'nde müşterinizin bir kaydını oluşturduktan sonra, bu abonelikleri katalogdaki ürünlere satabilirsiniz. Bu, üçüncü taraf bağımsız yazılım satıcıları (ISV 'Ler) tarafından [ticari Market](https://azuremarketplace.microsoft.com/marketplace)'e yayımlanan Microsoft ve hizmet olarak yazılım (SaaS) ürünleri tarafından yayımlanan ürünleri içerir.

Bazı teklifler müşteri başına bir abonelikle sınırlıdır. Hangi tekliflerin kısıtlı olduğunu görmek için Iş Ortağı Merkezi **Fiyat listeleri** sayfasını ziyaret edin.

> [!IMPORTANT]
> CSP programındaki bir iş ortağı olarak, Iş Ortağı Merkezi 'nde ISV yayımcılarından **Lisans tabanlı** veya **ölçülen** SaaS abonelikleri satın alabilirsiniz. Bu, tüm **Lisans tabanlı** veya **tarifeli** SaaS tekliflerini, erişiminiz olan [özel TEKLIFLER](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) de dahil olmak üzere ISV yayımcısı kullanımınıza sunabileceğiniz anlamına gelir. ISV 'lerden diğer, ticari Market tekliflerini satın almak veya yönetmek için (Azure uygulamaları, kapsayıcılar veya VM 'Leri içeren Kullanım tabanlı teklifler gibi) [Azure Portal](https://portal.azure.com/)gitmeniz gerekir.

> [!NOTE]
> Iş Ortağı Merkezi 'nde tüm tarihler ve saatler, evrensel saat Eşgüdümlü (UTC) zaman standardına göre verilmiştir. Bu, yerel saatinizden 24 saate kadar farklılık gösterebilir.

## <a name="create-a-new-subscription"></a>Yeni abonelik oluştur

> [!NOTE]
> Çalışma alanları arabirimi hakkında daha fazla bilgi edinmek için bkz. [Iş ortağı merkezini alma](get-around-partner-center.md#turn-workspaces-on-and-off).

#### <a name="workspaces-view"></a>[Çalışma alanları görünümü](#tab/workspaces-view)

1. [Iş Ortağı Merkezi panosundan](https://partner.microsoft.com/dashboard) **müşteriler** kutucuğunu seçin ve müşteri listesinden müşteriyi seçin.

2. **Abonelik Ekle**' yi seçin. **Çevrimiçi hizmetler** sekmesinde, tüm kullanılabilir Market SaaS teklifleri gösterilir.

3. Yalnızca belirli abonelik türlerini görmek için, kullanılabilir filtrelerdeki seçimleri yapın:
   - **Publisher**: ısv 'ler tarafından yayımlanan ticari market ürünlerini görmek için microsoft 'un yalnızca microsoft 'un veya **iş ortağının** tekliflerini görmek üzere **microsoft** 'u seçin.
   - **Faturalandırma türü**: kullanmak istediğiniz abonelik faturalandırması türünü seçin: **Lisans** veya **kullanım**. Aylık ve yıllık faturalandırma sıklığıyla ilgili karar vermenize yardımcı olacak bilgiler için [Lisans tabanlı faturalandırma](license-based-billing.md) konusuna bakın.
   - **kategori**: **Enterprise**, **küçük işletme** veya **deneme**' yı seçin. Deneme abonelikleri hakkında bilgi için bkz. [Microsoft ürünlerine yönelik müşterilerinizin deneme sürümlerini sunma](offer-your-customers-trials-of-microsoft-products.md).

4. Müşteriniz için satın almak istediğiniz ürün aboneliklerini seçin. Gördüğünüz ürünler, müşteri segmentinin (eğitim, Kamu, vb.) ve uyguladığınız filtrelerin türüne bağlıdır. Market 'te gösterilen bazı teklifler, belirli bir müşteri veya belirli bir CSP iş ortağı tarafından her zaman kullanılabilir olmayabilir. Bunun nedeni şu olabilir:
   - Müşterinin zaten bu ürüne yönelik bir aboneliği var ve yalnızca bir tane kullanılabilir
   - Müşterinin aboneliği askıya alınmış olabilir (Bu durumda, yeni bir tane satın almak yerine aboneliği yeniden etkinleştirebilirsiniz.)
   - ISV SaaS teklifleri için teklifin satın alma için sunulmamasının birkaç nedeni olabilir: ISV müşterinin fatura ülkesini veya bölgesini desteklemiyor olabilir; ISV, teklifi CSP programı aracılığıyla kullanılabilir hale getirmek için seçilmiş olabilir; ya da ISV, teklifi yalnızca belirli CSP iş ortakları için [özel](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) olarak yapmış olabilir. ISV teklifi Ayrıca Iş Ortağı Merkezi (örneğin, kapsayıcılar veya bazı kullanım tabanlı teklifler) üzerinden transactable de olmayabilir.  

5. Eklemek istediğiniz her abonelik için, lisansların (gerekirse) sayısını girin ve **Sepete Ekle**' yi seçin.

6. Abonelik eklemeyi bitirdiğinizde, **gözden geçir** ' i seçin ve siparişinizi gözden geçirin.

7. Siparişlerinizi gözden geçirdikten ve bu abonelikleri satın almaya hazırladıktan sonra **satın al**' ı seçin.

8. Bir müşteri için abonelik satın aldıktan sonra aşağıdakiler gerçekleşir:

    - Bu müşterinin **abonelikler** sayfasından abonelik adı ' nı seçerek aboneliği gözden geçirebilir veya düzenleyebilirsiniz. Buradan, varsa eklenti lisanslarını seçebilirsiniz, lisans miktarını değiştirebilir veya aboneliği askıya alabilirsiniz.

    **ISV SaaS (lisans tabanlı ve tarifeli) abonelikler için:**
    - ISV yayımcısının sitesine bir bağlantı alacaksınız. Bu bağlantı, müşterinin aboneliğine ait dağıtım veya hesap kurulumunu tamamlamanıza yardımcı olmalıdır.

    > [!NOTE]
    > Ne siz ne de müşteriniz bu tür ISV aboneliği için kurulumu/sağlamayı tamamlamaya yönelik yönergeleri içeren bir e-posta alacaksınız.)

    - Aboneliğiniz 30 günlük ücretsiz deneme sürümü ile birlikte geliyorsa, ücretsiz deneme süresi otomatik olarak uygulanır. CSP programındaki bir iş ortağı olarak, müşteriler için satın aldığınız tekliflerle ilgili ücretsiz deneme süresini beklenemez. Ücretsiz deneme süresi sona erdiğinde, abonelik dönemi başlar ve abonelik, ücretli duruma dönüştürülür. Abonelik daha sonra aynı zamanlamaya göre otomatik olarak yenilenecek.

#### <a name="current-view"></a>[Geçerli görünüm](#tab/current-view)

1. [Iş Ortağı Merkezi panosundan](https://partner.microsoft.com/dashboard) **müşteriler**' i seçin ve müşteri listesinden müşteriyi seçin.

2. **Abonelik Ekle**' yi seçin. **Çevrimiçi hizmetler** sekmesinde, tüm kullanılabilir Market SaaS teklifleri gösterilir.

3. Yalnızca belirli abonelik türlerini görmek için, kullanılabilir filtrelerdeki seçimleri yapın:
   - **Publisher**: ısv 'ler tarafından yayımlanan ticari market ürünlerini görmek için microsoft 'un yalnızca microsoft 'un veya **iş ortağının** tekliflerini görmek üzere **microsoft** 'u seçin.
   - **Faturalandırma türü**: kullanmak istediğiniz abonelik faturalandırması türünü seçin: **Lisans** veya **kullanım**. Aylık ve yıllık faturalandırma sıklığıyla ilgili karar vermenize yardımcı olacak bilgiler için [Lisans tabanlı faturalandırma](license-based-billing.md) konusuna bakın.
   - **kategori**: **Enterprise**, **küçük işletme** veya **deneme**' yı seçin. Deneme abonelikleri hakkında bilgi için bkz. [Microsoft ürünlerine yönelik müşterilerinizin deneme sürümlerini sunma](offer-your-customers-trials-of-microsoft-products.md).

4. Müşteriniz için satın almak istediğiniz ürün aboneliklerini seçin. Gördüğünüz ürünler, müşteri segmentinin (eğitim, Kamu, vb.) ve uyguladığınız filtrelerin türüne bağlıdır. Market 'te gösterilen bazı teklifler, belirli bir müşteri veya belirli bir CSP iş ortağı tarafından her zaman kullanılabilir olmayabilir. Bunun nedeni şu olabilir:
   - Müşterinin zaten bu ürüne yönelik bir aboneliği var ve yalnızca bir tane kullanılabilir
   - Müşterinin aboneliği askıya alınmış olabilir (Bu durumda, yeni bir tane satın almak yerine aboneliği yeniden etkinleştirebilirsiniz.)
   - ISV SaaS teklifleri için teklifin satın alma için sunulmamasının birkaç nedeni olabilir: ISV müşterinin fatura ülkesini veya bölgesini desteklemiyor olabilir; ISV, teklifi CSP programı aracılığıyla kullanılabilir hale getirmek için seçilmiş olabilir; ya da ISV, teklifi yalnızca belirli CSP iş ortakları için [özel](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) olarak yapmış olabilir. ISV teklifi Ayrıca Iş Ortağı Merkezi (örneğin, kapsayıcılar veya bazı kullanım tabanlı teklifler) üzerinden transactable de olmayabilir.  

5. Eklemek istediğiniz her abonelik için, lisansların (gerekirse) sayısını girin ve **Sepete Ekle**' yi seçin.

6. Abonelik eklemeyi bitirdiğinizde, **gözden geçir** ' i seçin ve siparişinizi gözden geçirin.

7. Siparişlerinizi gözden geçirdikten ve bu abonelikleri satın almaya hazırladıktan sonra **satın al**' ı seçin.

8. Bir müşteri için abonelik satın aldıktan sonra aşağıdakiler gerçekleşir:

    - Bu müşterinin **abonelikler** sayfasından abonelik adı ' nı seçerek aboneliği gözden geçirebilir veya düzenleyebilirsiniz. Buradan, varsa eklenti lisanslarını seçebilirsiniz, lisans miktarını değiştirebilir veya aboneliği askıya alabilirsiniz.

    **ISV SaaS (lisans tabanlı ve tarifeli) abonelikler için:**
    - ISV yayımcısının sitesine bir bağlantı alacaksınız. Bu bağlantı, müşterinin aboneliğine ait dağıtım veya hesap kurulumunu tamamlamanıza yardımcı olmalıdır.

    > [!NOTE]
    > Ne siz ne de müşteriniz bu tür ISV aboneliği için kurulumu/sağlamayı tamamlamaya yönelik yönergeleri içeren bir e-posta alacaksınız.)

    - Aboneliğiniz 30 günlük ücretsiz deneme sürümü ile birlikte geliyorsa, ücretsiz deneme süresi otomatik olarak uygulanır. CSP programındaki bir iş ortağı olarak, müşteriler için satın aldığınız tekliflerle ilgili ücretsiz deneme süresini beklenemez. Ücretsiz deneme süresi sona erdiğinde, abonelik dönemi başlar ve abonelik, ücretli duruma dönüştürülür. Abonelik daha sonra aynı zamanlamaya göre otomatik olarak yenilenecek.

* * *

## <a name="update-subscriptions-with-add-ons"></a>Eklentilerle abonelikleri güncelleştirme

Bir eklenti satın almak için müşterinin öncelikle etkin bir temel aboneliği olmalıdır.  Eklentileri katalog aracılığıyla satın alamazsınız.

1. Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.

2. Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve listeden bir müşteri seçin.

3. Yönetmek istediğiniz aboneliği seçin.

4. **Durum** bölümünün altında, abonelik Için kullanılabilen eklentilerin bir listesi bulunur.  

5. Gerekli her eklenti için lisans miktarını güncelleştirin. Sonra **Gönder** ile yaptığınız değişiklikleri gönderin.

Iş Ortağı Merkezi aracılığıyla eklenti satın alma özelliği yalnızca doğrudan fatura ve dolaylı sağlayıcılar için kullanılabilir.
Temel gereksinimlere ve bölgesel kullanılabilirliğe göre yalnızca uygun eklentiler görüntülenir. Fiyatlandırma ve teklifler hakkında daha fazla bilgi için bkz. Cloud Bayi teklif matrisi. Temel abonelik askıya alındığında ilişkili tüm eklentiler de askıya alınır.

Eklentilerin başlangıç tarihleri temel abonelikle uyumludur; ücretler Ücret başlangıç tarihi ile Ücret bitiş tarihi kullanılarak hesaplanır ve ilk faturaya orantılı bir ücret uygulanır. Daha fazla bilgi için bkz. [Lisans tabanlı faturalandırma](license-based-billing.md).


## <a name="suspend-or-cancel-a-subscription"></a>Aboneliği askıya alma veya iptal etme

İş ortakları, müşteri tarafından isteniyorsa veya ödeme veya sahtekarlık durumlarında bir aboneliği askıya alabilir veya iptal edebilir.

### <a name="suspend-a-subscription"></a>Bir aboneliği askıya alma

Aboneliğin durumunu **askıya alındı** olarak değiştirdiğinizde, kullanıcılar oturum açamaz veya hizmetlere erişemez.

1. Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.

2. Yeni İş Ortağı Merkezi **Müşteriler'i ve** ardından listeden bir müşteri seçin.

3. Yönetmek istediğiniz aboneliği seçin.

4. **Durum** bölümünde **Askıya Alındı**'yı seçin. Sonra **Gönder** ile yaptığınız değişiklikleri gönderin.

5. Abonelik 90 gün veya 90 gün içinde yeniden etkinleştirildiği sürece tüm veriler silinir ve hesabın açılmasıyla ilk faturalama dönemi (en fazla 120 gün) arasındaki gün sayısı.

Bir aboneliği askıya alırsanız, Askıya Alınmış düğmesinin altında gördüğünüz tarih, aboneliği yeniden etkinleştirmezsanız aboneliğin süresinin otomatik olarak ne zaman dol olacağını gösterir.  

> [!NOTE]
> CSP abonelikleri, hizmetlerin çalışmaya devam eder ancak abonelik herhangi bir faturalama ücreti oluşturmazken süresi dolmuş bir süreye (doğrudan web abonelikleri gibi) sahip değildir. CSP abonelikleri etkin veya askıya alınmış (veya tamamen silinmiş).

> [!NOTE]
> Yeni Ticaret değişiklikleri şu anda yalnızca Microsoft 365/Dynamics 365 yeni ticaret deneyimi teknik önizlemesinde yer alan iş ortakları tarafından kullanılabilir.

Yeni ticari abonelikleri askıya almak veya askıya alınmış yeni ticari abonelikleri yeniden etkinleştirmek için bir hizmet isteği oluşturun ve de destekle iletişime geçin.


### <a name="cancel-a-subscription"></a>Aboneliği iptal etme

Lisans tabanlı SaaS aboneliklerini ticari market içindeki üçüncü taraf ISV yayımcılarından İş Ortağı Merkezi [edebilirsiniz.](csp-commercial-marketplace-overview.md) İptal süresi içinde iptal edersiniz, tam para iadesi alırsınız.

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

2. Yeni İş Ortağı Merkezi **Müşteriler'i ve** ardından listeden bir müşteri seçin.

3. İptal etmek istediğiniz aboneliği bulun.

4. Durum sütununda **İptal'i** **seçin.** Sonra **Gönder** ile yaptığınız değişiklikleri gönderin.

5. İletişim kutusu görüntülenirse ilgili ayrıntıları doldurun ve Gönder'i **seçin.**

6. İptali onaylamak için Evet, iptal **et'i seçin.**

> [!NOTE]
> Api'leri kullanarak bir Azure Market aboneliğini iptal edebilirsiniz. Bunu yapmak için [bkz. Azure Market aboneliğini iptal etme.](/partner-center/develop/cancel-an-azure-marketplace-subscription)

## <a name="suspend-or-cancel-a-new-commerce-subscription"></a>Yeni bir ticari aboneliği askıya alma veya iptal etme

### <a name="suspend-a-new-commerce-subscription"></a>Yeni bir ticari aboneliği askıya alma

> [!NOTE]
> Yeni Ticaret değişiklikleri şu anda yalnızca Microsoft 365/Dynamics 365 yeni ticaret deneyimi teknik önizlemesinde yer alan iş ortakları tarafından kullanılabilir.

Müşteriden ödeme almama durumunda (bazen "engelleme senaryosu" olarak da adlandırılır) iş ortakları, müşterinin aboneliğin hizmetlerine erişimini hemen engellemek için aboneliğini duraklatabilir ve sürdürebilirsiniz.

İş ortakları aboneliği iptal etmeden herhangi bir zamanda duraklatabilir ve sürdürebilirsiniz. Ancak, iş ortağı faturalaması askıya alma sırasında devam eder. 

Müşterinin aboneliklerini duraklatma, aboneliği devam ettirilene kadar oturum açma ve hizmetlerini kullanma becerisini devre dışı bırakacak. Abonelik 90 gün içinde yeniden etkinleştirildiği sürece abonelikle ilgili tüm veriler silinir.

Aboneliği duraklatmak için şu İş Ortağı Merkezi:

1. Müşterinin abonelik sayfasına gidin ve duraklatmak istediğiniz aboneliği seçin.

2. Askıya **al radyo** düğmesini seçin.

3. Açılan iletişim kutusunda Tamam'ı **seçin.**

4. Abonelik artık duraklatılmış durumda olur ve iş ortağı abonelik için faturalandırılır.

Duraklatma işlemi, kullanıcının İş Ortağı Merkezi api'leri aracılığıyla geri alınarak müşterinin aboneliğin hizmetlerine erişimini hemen geri yükleyebilirsiniz.

> [!IMPORTANT]
> Aboneliği duraklatma, tüm otomatik yenileme ayarlarını devre dışı çevirir ve mevcut zamanlanmış değişiklikleri kaldırır. Aboneliği duraklatmak yalnızca müşterinin hizmet erişimini etkiler ve iş ortağı faturalaması duraklatılmış durumdayken devam eder.

### <a name="cancel-a-new-commerce-subscription"></a>Yeni bir ticari aboneliği iptal etme

> [!Note] 
> Yeni Ticaret değişiklikleri şu anda yalnızca Microsoft 365/Dynamics 365 yeni ticaret deneyimi teknik önizlemesinde yer alan iş ortakları tarafından kullanılabilir.

Yeni ticari teklifler için, iş ortakları herhangi bir dönem için ilk **72** saat içinde (günlük olarak **proration hesaplanan) proratlı** para iadesi ile aboneliğini iptal edebilir.  

72 saat sonra iptal artık kullanılamaz ve müşteri için ödeme yapmayı durdursa veya aboneliği kullanmayı durdursa bile (herhangi bir faturalama planı için geçerlidir) iş ortağı tam dönem için faturalandırılır.

İptal işlemi tamamlandığında müşteri hizmete erişimi hemen kaybeder ve hizmet geri yüklenebilir. Aboneliğin durumu kurtarılamaz.  

Lisanslar orta dönemde eklenirse, aynı 72 saatlik ilke ek lisansların azaltılması için de geçerlidir. Eklenen lisansların azaltılması, destek istekleri **aracılığıyla yapılması gerekir.**

## <a name="subscription-renewals"></a>Abonelik yenilemeleri

> [!NOTE]
> Yeni Ticaret değişiklikleri şu anda yalnızca Microsoft 365/Dynamics 365 yeni ticaret deneyimi teknik önizlemesinde yer alan iş ortakları tarafından kullanılabilir.

Etkin abonelikler varsayılan olarak abonelik süresi sona erdiğinde otomatik olarak yenilenecek şekilde ayarlanır. Ticari [market ürünlerine veya yeni](csp-commercial-marketplace-overview.md)ticari aboneliklere yönelik abonelikler için isteğe bağlı olarak aboneliği otomatik olarak yenilemeyi seçebilirsiniz.

Etkin bir ticari market aboneliğinin veya yeni ticari aboneliklerin otomatik olarak yenilenmesini durdurmak için:

1. İş Ortağı Merkezi [oturum açın.](https://partner.microsoft.com/dashboard)

2. Yeni İş Ortağı Merkezi **Müşteriler'i ve** ardından listeden bir müşteri seçin.

3. **Abonelikler**'i seçin. Bu, müşteri için satın aldığınız tüm lisans tabanlı abonelikleri listeler.

4. Abonelik **sütununda** değiştirmek istediğiniz aboneliği seçin.

5. Abonelik ayrıntıları sayfasında Durum bölümünü **bulun ve** Otomatik yenile **kutusunun işaretini** kaldırın.

6. **Gönder**’i seçin.

### <a name="manage-new-commerce-renewals-with-scheduled-changes"></a>Zamanlanmış değişikliklerle yeni ticari yenilemeleri yönetme

> [!NOTE]
> Yeni Ticaret değişiklikleri şu anda yalnızca Microsoft 365/Dynamics 365 yeni ticaret deneyimi teknik önizlemesinde yer alan iş ortakları tarafından kullanılabilir.

Aboneliklerde bazı değişiklikler yalnızca bir süre sonunda olabilir. Bu değişiklikler, terimin sonunda rahatça uygulanarak zamanlanmış olabilir. Zamanlanmış olması gereken değişiklik örnekleri:

- lisans azaltmaları
- Faturalama dönemi değişiklikleri
- Faturalama sıklığında yapılan değişiklikler

Dönem boyunca yükseltmeler veya lisans artışları gibi diğer değişiklikler uygulanabilir.

Zaman çizelgesi değişiklikleri, abonelik bir sonraki dönem için yenilendikleri yenileme sırasında gerçekleşir.

Zamanlanmış değişiklikler için önkullar:

- Abonelik etkin 
- Otomatik yenileme açık
- SKU'nun yükseltme için uygun olması gerekir

Yenileme sırasında yapılacak yeni bir değişiklik zamanlaması için:

1. Panoda İş Ortağı Merkezi açın.

2. Müşteri **listesinden** bir müşteri seçin.

3. Yönetmek istediğiniz aboneliği seçin.

4. Yenilemeleri **Yönet'i seçin.**

5. SKU, miktar, terim veya faturalama sıklığı için farklı bir Değere değiştir'i seçin:

   - **Geçerli,** aboneliğin geçerli değeridir

   - **değerini** olarak değiştir, yeni abonelik için yenilemede uygulanması istediğiniz son kayıtlı değerdir

6. **Gönder**’i seçin.

7. Değişiklikler yenileme sırasında gerçekleşir.

İş ortakları, mevcut **zamanlanmış değişikliği görüntülemek,** güncelleştirmek veya kaldırmak için Yenilemeleri Yönet'e erişim sağlar.

> [!NOTE]
> - Denemeler varsayılan olarak deneme döneminin sonunda ücretli eşdeğer SKU'ya dönüştürülür.
> - Zamanlanmış SKU yükseltmelerinde, lisans miktarı değişmezse, kullanıcı lisansı yeniden ataması otomatik olur, aksi takdirde el ile yapılması gerekir.
> - Abonelikte ara dönem güncelleştirmeleri yapılırsa kaydedilen zamanlanmış değişiklikler silinir.

Kaydedilen zamanlanmış değişiklikler, aşağıdaki orta dönem değişiklikleri gerçekleştirdiğinde silinir:  

- Otomatik yenileme kapalı 
- Miktar değiştirildi 
- Abonelik iptal edildi 
- SKU yükseltildi 
- Deneme dönüştürüldü 

## <a name="upgrades-in-new-commerce-subscriptions"></a>Yeni ticaret aboneliklerinde yükseltmeler

Yeni Ticaret için, yükseltme, ücretli bir abonelikten başka ücretli aboneliğe kadar bir ücretden gelmektedir. Yeni ticari ödemeli yükseltmeler, müşterinin geçerli SKU 'sundan, eklenen hizmetlere kadar anında yükseltmelerini sağlar. 

İş ortakları, lisans sayılarını yapılandırırken hangi aboneliğin yükseltmek istediğinizi seçebilir. İş ortakları, yükseltme için uygun olması halinde **Yeni** bir abonelik seçebilir veya **mevcut** bir aboneliği seçebilir. 

Yükseltmeler iki türden oluşabilir: **tam yükseltme** ve **kısmi yükseltme**.

> [!NOTE]
> - Yükseltmeler, bir dönem sonunda gerçekleşecek şekilde zamanlanabilir veya orta ölçekli bir dönem için kullanılabilir.
> - Orta ölçekli bir yükseltmeyi başlatmak, var olan zamanlanmış yükseltmeleri kaldırır.
> - Yükseltmeler yalnızca **etkin** durumdaki aboneliklerden başlatılabilir.

### <a name="full-upgrades"></a>Tam yükseltmeler

Tam yükseltme, tüm veya daha fazla lisansın yükseltilmekte olduğu anlamına gelen yerinde bir yükseltmeye sahiptir. Bu durumda, abonelik KIMLIĞI aynı kalır ve lisanslar otomatik olarak atanır. Ancak, müşterinin zaten başka bir iş ortağından veya kanaldan daha eski olan hedef SKU 'yu satın almış olması durumunda el ile atama gerekecektir. El ile atama gerekliyse, iş ortağı merkezi 'nde lisansların el ile atanması gerektiğini belirten bir uyarı iletisi görür. 

### <a name="partial-upgrades"></a>Kısmi yükseltmeler

Kısmi yükseltmeler, bir iş ortağının bir SKU 'dan diğerine bazı lisanslar belirlemesini sağlar. Geleneksel lisans tabanlı aboneliklerdeki önceki yükseltme işlevselliği yalnızca yükseltilecek tüm lisansların etkinleştirilmesini sağlar. Yeni ticaret, bir ortağın bazı lisansları kolay bir şekilde taşımasına olanak sağlar. Bu, iş ortağının yükseltmeleri yönetme konusunda daha fazla denetime sahip olmasını sağlar ve bu sayede bazı kullanıcıları, bunları taşımadan yeni bir SKU 'ya taşımasına olanak tanır.

Kısmi yükseltme ayrıntıları:

- Yükseltme lisansı sayısı ilk aboneliğin boyutundan küçükse kısmi olarak tanımlanır.
- Kısmen yükseltirken, yükseltmenin kaynaklandığı abonelikle aynı dönem bitiş tarihlerine sahip olacağı yeni bir abonelik oluşturulur.

## <a name="increasing-and-reducing-licenses-in-new-commerce-subscriptions"></a>Yeni ticaret aboneliklerindeki lisansları artırma ve azaltma

Bir abonelikteki lisans sayısı, faturalama ayarlamaları bir sonraki faturaya ve mutabakat dosyasına yansımış olacak şekilde herhangi bir zamanda **artırılabilir** . 

Bir abonelikteki lisans sayısı **azaltılabilir**:
- Yalnızca abonelik siparişi **ilk kez yerleştirildiğinde veya yenilendiğinde** ilk 72 saat içinde. 
- **Orta terime eklenen** lisanslar için 72 saat içinde müşteri desteği aracılığıyla

Bir abonelik döneminin ilk 72 saati içinde (ilk satın alma veya yenileme sonrasında) bir lisans sayısı azalması, Iş Ortağı Merkezi 'nde veya API aracılığıyla self servis aracılığıyla yapılabilir.

Orta dönemde eklenen lisanslar için lisans sayısı azalması, yalnızca ilk 72 saat içinde müşteri desteği aracılığıyla yapılabilir.

Lisans azaltma her iki durumda da,    aboneliği kullandığınız günler için eşit miktarda (günde bir **hesaplanan gün)** toplam miktarı iade edersiniz. 

Abonelik siparişi yerleştirildiğinden veya ek lisanslar eklendikten sonra **72 saatten fazla** süre geçtikten sonra, yenileme sırasında bir sonraki iptal penceresine kadar lisans sayısı **azaltılamıyor** .

## <a name="switching-billing-plans"></a>Faturalandırma planlarını değiştirme

İş ortağının faturalandırma planını ve faturalandırma terimini birlikte değiştirme esnekliği vardır. Ayrıca, faturalandırma terimini tamamen sıfırlamadan yalnızca faturalandırma planının orta dönem olarak değiştirilmesi seçeneği de vardır.

### <a name="just-changing-billing-frequency-scheduled-change"></a>Yalnızca faturalandırma sıklığını değiştirme (zamanlanan değişiklik)

İş ortakları yalnızca birkaç adımda Iş Ortağı Merkezi aracılığıyla yalnızca faturalandırma planını değiştirebilir ve bu da bir sonraki fatura döngüsünün yürürlüğe girer:

1. Müşterinin abonelik sayfasına gidin ve değiştirmek istediğiniz aboneliği seçin.

2. **Faturalandırma sıklığını Yönet** bağlantısını seçin.

3. Geçerli faturalandırma sıklığını ve sıklığı değiştirme seçeneklerini içeren bir açılan menüyü görüntüleyen bir yan panel açılır.

4. Yeni bir değer seçildikten sonra yeni faturalandırma değişiklikleri bir **sonraki fatura döngüsüne** (anında değişiklik değil) uygulanır.

### <a name="changing-billing-frequency-along-with-billing-term-and-other-fields-immediate-change"></a>Faturalama sıklığının yanı sıra fatura şartı ve diğer alanları değiştirme (anında değişiklik)

İş ortağı, faturalama sıklığını ve aynı zamanda Iş Ortağı Merkezi aracılığıyla diğer alanları ve bir değişikliği tetikleyecek şekilde değiştirebilir:

1. Müşterinin abonelik sayfasına gidin ve değiştirmek istediğiniz aboneliği seçin.

2. Süre içinde, açılan menüdeki bir seçeneği belirleyerek dönem süresini değiştirin. Bu, fatura sıklığını değiştirmek için başka bir açılan menü açar.

3. Açılan listeden farklı bir faturalandırma sıklığı seçin.

4. Değişiklikleri yaptıktan ve Gönder ' i tıklatmanızdan sonra yeni faturalandırma değişiklikleri **hemen** gerçekleşir.

## <a name="next-steps"></a>Sonraki adımlar

- [Müşterileriniz için ticari Market ürünleri satın alın](csp-commercial-marketplace-purchase.md)

- [Müşterileriniz için ticari Market ürünlerini yönetme](csp-commercial-marketplace-manage.md)

- [Ticari markete genel bakış](csp-commercial-marketplace-overview.md)
