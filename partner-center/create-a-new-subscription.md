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
ms.openlocfilehash: 1a2e13bf45b10bebe6ab0492ac059dc1d6a6c0ca
ms.sourcegitcommit: 462d6026287b85c9feea602af5bcdf924f3e6976
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/05/2021
ms.locfileid: "129452422"
---
# <a name="manage-customer-subscriptions"></a>Müşteri aboneliklerini yönetme

**Uygulama hedefi**: Iş Ortağı Merkezi | Microsoft Cloud for US Government için iş ortağı Merkezi

**Uygun roller**: yönetici Aracısı | Faturalandırma Yöneticisi | Genel yönetici | Yardım Masası Aracısı | Satış Aracısı

Iş Ortağı Merkezi 'nde müşterinizin bir kaydını oluşturduktan sonra, bu abonelikleri katalogdaki ürünlere satabilirsiniz. Bu, üçüncü taraf bağımsız yazılım satıcıları (ISV 'Ler) tarafından [ticari Market](https://azuremarketplace.microsoft.com/marketplace)'e yayımlanan Microsoft ve hizmet olarak yazılım (SaaS) ürünleri tarafından yayımlanan ürünleri içerir.

Bazı teklifler müşteri başına bir abonelikle sınırlıdır. Hangi tekliflerin kısıtlı olduğunu görmek için Iş Ortağı Merkezi fiyatlandırma ve teklifleri sayfasını ziyaret edin.

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

2. Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve listeden bir müşteri seçin.

3. Yönetmek istediğiniz aboneliği seçin.

4. **Durum** bölümünde **Askıya Alındı**'yı seçin. Sonra **Gönder** ile yaptığınız değişiklikleri gönderin.

5. Abonelik 90 gün içinde yeniden etkinleştirilmediği veya 90 gün ile hesabın açıldığı zaman arasındaki gün sayısı ile ilk fatura dönemi (maksimum 120 gün) arasında tüm veriler silinir.

Bir aboneliği askıya aldığınızda, **askıya alınmış** düğmesinin altında gördüğünüz Tarih, yeniden etkinleştirmezseniz aboneliğin otomatik olarak ne zaman dolacağını gösterir. 

> [!NOTE]
> CSP aboneliklerinin süresi, hizmetin hala çalıştığı ancak aboneliğin fatura ücreti üretmeyen süresi olmayan bir döneme (Web-Direct aboneliklerinin yapması) sahip değildir. CSP abonelikleri etkin veya askıya alındı (ya da tamamen silinmiş).

> [!NOTE]
> yeni ticaret değişiklikleri şu anda yalnızca Microsoft 365/dynamics 365 yeni ticaret deneyimi technical preview 'ın parçası olan iş ortakları tarafından kullanılabilir.

Yeni ticari abonelikleri askıya almak veya askıya alınmış yeni ticari abonelikleri yeniden etkinleştirmek için bir hizmet isteği oluşturun ve desteğe başvurun.


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

## <a name="suspend-or-cancel-a-new-commerce-subscription"></a>Yeni bir ticari aboneliği askıya alma veya iptal etme

### <a name="suspend-a-new-commerce-subscription"></a>Yeni bir ticari aboneliği askıya al

> [!NOTE]
> yeni ticaret değişiklikleri şu anda yalnızca Microsoft 365/dynamics 365 yeni ticaret deneyimi technical preview 'ın parçası olan iş ortakları tarafından kullanılabilir.

Müşteri ödemesiz "hatırlatarak senaryosu" olarak da adlandırılır. iş ortakları, müşterinin aboneliğin Hizmetlerine erişimini hemen engellemek için aboneliğini duraklatabilir ve sürdürebilir.

İş ortakları bir aboneliği iptal etmeden duraklatabilir ve devam edebilir. Ancak, iş ortağı faturalandırma askıya alma sırasında devam eder. 

Müşterinin aboneliklerinin duraklatılması, abonelikleri sürdürülene kadar oturum açma ve hizmetlerini kullanma imkanlarını devre dışı bırakacaktır. Abonelik 90 gün içinde yeniden etkinleştirilmediği takdirde abonelikle ilgili tüm veriler silinir.

Iş Ortağı Merkezi 'ni kullanarak bir aboneliği duraklatabilirsiniz:

1. Müşterinin abonelik sayfasına gidin ve duraklatmak istediğiniz aboneliği seçin.

2. Radyoyu **beklet** düğmesini seçin.

3. Açılır iletişim kutusunda **Tamam**' ı seçin.

4. Abonelik artık duraklatılmış durumda olacak ve iş ortağı abonelik için faturalandırılmaya devam edecek.

Duraklatma, Iş Ortağı Merkezi kullanıcı arabirimi veya API 'Ler aracılığıyla bir müşterinin bir aboneliğin Hizmetlerine erişimini anında geri yükler.

> [!IMPORTANT]
> Bir aboneliğin duraklatılması, otomatik yenileme ayarlarını devre dışı bırakır ve var olan zamanlanmış değişiklikleri kaldırır. Bir aboneliğin duraklatılması yalnızca müşterinin hizmet erişimini etkiler ve duraklama durumunda iş ortağı faturalandırmaya devam eder.

### <a name="cancel-a-new-commerce-subscription"></a>Yeni bir ticari aboneliği iptal et

> [!Note] 
> yeni ticaret değişiklikleri şu anda yalnızca Microsoft 365/dynamics 365 yeni ticaret deneyimi technical preview 'ın parçası olan iş ortakları tarafından kullanılabilir.

Yeni ticaret teklifleri için, iş ortakları, her dönem için ilk **72 saat** içinde eşit olarak dağıtılmış bir geri ödeme ile aboneliğini iptal edebilir **(günde eşit olarak hesaplanır)**.  

72 saat sonra, iptal artık kullanılamaz ve müşteri için ödeme ve abonelik (herhangi bir faturalandırma planına uygulanabilir) olsa bile, iş ortağı tam dönem için faturalandırılır.

İptal işlemi tamamlandığında, müşteri hizmete erişimi hemen kaybedecektir ve hizmet geri yüklenemez. Aboneliğin durumu kurtarılamaz olacaktır.  

Lisanslar orta dönemde eklenirse, ek lisansların her azalmasıyla aynı 72 saat ilkesi uygulanır. Eklenen lisansların azaltılması, **destek istekleri** aracılığıyla yapılmalıdır.

## <a name="subscription-renewals"></a>Abonelik yenilemeleri

> [!NOTE]
> yeni ticaret değişiklikleri şu anda yalnızca Microsoft 365/dynamics 365 yeni ticaret deneyimi technical preview 'ın parçası olan iş ortakları tarafından kullanılabilir.

Etkin abonelikler varsayılan olarak abonelik süresi sona erdiğinde otomatik olarak yenilenecek şekilde ayarlanır. [Ticari Market ürünlerine](csp-commercial-marketplace-overview.md)veya yeni ticaret aboneliklerine yönelik abonelikler için, isteğe bağlı olarak, aboneliği otomatik olarak yenilemeyi seçebilirsiniz.

Etkin bir ticari Market aboneliğini veya yeni ticari abonelikleri otomatik olarak yenilemeyi durdurmak için:

1. Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.

2. Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve listeden bir müşteri seçin.

3. **Abonelikler**'i seçin. Bu, müşteri için satın aldığınız lisans tabanlı abonelikleri listeler.

4. **Abonelik** sütununda, değiştirmek istediğiniz aboneliği seçin.

5. Abonelik Ayrıntıları sayfasında, **durum** bölümünü bulun ve **Otomatik Yenile** kutusunun işaretini kaldırın.

6. **Gönder**’i seçin.

### <a name="manage-new-commerce-renewals-with-scheduled-changes"></a>Zamanlanan değişikliklerle yeni ticaret yenilemeleri yönetme

> [!NOTE]
> yeni ticaret değişiklikleri şu anda yalnızca Microsoft 365/dynamics 365 yeni ticaret deneyimi technical preview 'ın parçası olan iş ortakları tarafından kullanılabilir.

Aboneliklerde yapılan bazı değişiklikler yalnızca bir terimin sonunda gerçekleşebilir. Bu değişiklikler, terimin sonunda kolayca uygulanabilmeleri için zamanlanabilir. Zamanlanması gereken değişikliklere örnek olarak şunlar verilebilir:

- Lisans indirimleri
- Fatura terimiyle yapılan değişiklikler
- Faturalandırma sıklığında yapılan değişiklikler

Yükseltmeler veya lisans artışları gibi diğer değişiklikler, dönem sırasında uygulanabilir.

Zaman çizelgesi, abonelik bir sonraki dönem için yenilendiğinde yenileme sırasında meydana gelir.

Zamanlanan değişiklikler için önkoşulların önkoşulları:

- Abonelik etkin 
- Otomatik yenileme açık
- SKU 'nun yükseltme için uygun olması gerekir

Yenileme sırasında yeni bir değişikliği zamanlamak için:

1. Iş Ortağı Merkezi panosunda oturum açın.

2. Müşteri listesinden bir **Müşteri** seçin.

3. Yönetmek istediğiniz aboneliği seçin.

4. **Yenilemeleri Yönet**' i seçin.

5. SKU, miktar, dönem veya faturalandırma sıklığı için farklı bir değer değişikliği seçin:

   - **Geçerli** , aboneliğin geçerli değeridir

   - Olarak **Değiştir** , yeni abonelik için yenilemeye uygulanmasını istediğiniz son kayıtlı değerdir

6. **Gönder**’i seçin.

7. Değişiklikler yenilemeyle yapılır.

İş ortakları, var olan zamanlanmış değişikliği görüntülemek, güncelleştirmek veya kaldırmak için **yenilemeler yönetme** erişimi sağlayabilir.

> [!NOTE]
> - Varsayılan olarak, denemeler deneme süresinin sonunda ücretli eşdeğer SKU 'ya dönüştürülür.
> - Zamanlanan SKU yükseltmeleri için, lisans miktarı değişmezse Kullanıcı Lisans yeniden ataması otomatik olarak yapılır, aksi takdirde el ile yapılmalıdır.
> - Abonelikte orta dönem güncelleştirmeler yapılırsa, kaydedilen zamanlanan değişiklikler silinir.

Kaydedilen zamanlanan değişiklikler aşağıdaki orta dönemli değişiklikler yapıldığında silinir:  

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
