---
title: Iş Ortağı Merkezi 'nde müşteri abonelikleri oluşturma
ms.topic: how-to
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Microsoft tarafından yayımlanan ürünlerin yanı sıra üçüncü taraf ISV 'Ler tarafından yayımlanan SaaS ürünleri için müşterilerinize abonelik satma hakkında bilgi edinin.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 199e3dc42a0aa46c3e743e9e6fcb0ed585cd0303
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114838028"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Müşteri aboneliklerini oluşturma, askıya alma veya iptal etme

**Uygulama hedefi**: Iş Ortağı Merkezi | Microsoft Cloud for US Government için iş ortağı Merkezi

**Uygun roller**: yönetici Aracısı | Faturalandırma Yöneticisi | Genel yönetici | Yardım Masası Aracısı | Satış Aracısı

Iş Ortağı Merkezi 'nde müşterinizin bir kaydını oluşturduktan sonra, bu abonelikleri katalogdaki ürünlere satabilirsiniz. Bu, üçüncü taraf bağımsız yazılım satıcıları (ISV 'Ler) tarafından [ticari Market](https://azuremarketplace.microsoft.com/marketplace)'e yayımlanan Microsoft ve hizmet olarak yazılım (SaaS) ürünleri tarafından yayımlanan ürünleri içerir.

Bazı teklifler müşteri başına bir abonelikle sınırlıdır. Hangi tekliflerin kısıtlı olduğunu görmek için Iş Ortağı Merkezi fiyatlandırma ve teklifleri sayfasını ziyaret edin.

>[!IMPORTANT]
> CSP programındaki bir iş ortağı olarak, Iş Ortağı Merkezi 'nde ISV yayımcılarından **Lisans tabanlı** veya **ölçülen** SaaS abonelikleri satın alabilirsiniz. Bu, tüm **Lisans tabanlı** veya **tarifeli** SaaS tekliflerini, erişiminiz olan [özel TEKLIFLER](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) de dahil olmak üzere ISV yayımcısı kullanımınıza sunabileceğiniz anlamına gelir. ISV 'lerden diğer, ticari Market tekliflerini satın almak veya yönetmek için (Azure uygulamaları, kapsayıcılar veya VM 'Leri içeren Kullanım tabanlı teklifler gibi) [Azure Portal](https://portal.azure.com/)gitmeniz gerekir.

>[!NOTE]
>Iş Ortağı Merkezi 'nde tüm tarihler ve saatler, evrensel saat Eşgüdümlü (UTC) zaman standardına göre verilmiştir. Bu, yerel saatinizden 24 saate kadar farklılık gösterebilir.

## <a name="create-a-new-subscription"></a>Yeni abonelik oluştur

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard) oturum açın.

2. Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve listeden bir müşteri seçin.

3. **Abonelik Ekle**' yi seçin. **Çevrimiçi hizmetler** sekmesinde, tüm kullanılabilir Market SaaS teklifleri gösterilir.

4. Yalnızca belirli abonelik türlerini görmek için, kullanılabilir filtrelerdeki seçimleri yapın:
   - **Publisher**: ısv 'ler tarafından yayımlanan ticari market ürünlerini görmek için microsoft 'un yalnızca microsoft 'un veya **iş ortağının** tekliflerini görmek üzere **microsoft** 'u seçin.
   - **Faturalandırma türü**: kullanmak istediğiniz abonelik faturalandırması türünü seçin: **Lisans** veya **kullanım**. Aylık ve yıllık faturalandırma sıklığıyla ilgili karar vermenize yardımcı olacak bilgiler için [Lisans tabanlı faturalandırma](license-based-billing.md) konusuna bakın.
   - **kategori**: **Enterprise**, **küçük işletme** veya **deneme**' yı seçin. Deneme abonelikleri hakkında bilgi için bkz. [Microsoft ürünlerine yönelik müşterilerinizin deneme sürümlerini sunma](offer-your-customers-trials-of-microsoft-products.md).

5. Müşteriniz için satın almak istediğiniz ürün aboneliklerini seçin. Gördüğünüz ürünler, müşteri segmentinin (eğitim, Kamu, vb.) ve uyguladığınız filtrelerin türüne bağlıdır. Market 'te gösterilen bazı teklifler, belirli bir müşteri veya belirli bir CSP iş ortağı tarafından her zaman kullanılabilir olmayabilir. Bunun nedeni şu olabilir:

   - Müşterinin zaten bu ürüne yönelik bir aboneliği var ve yalnızca bir tane kullanılabilir

   - Müşterinin aboneliği askıya alınmış olabilir (Bu durumda, yeni bir tane satın almak yerine aboneliği yeniden etkinleştirebilirsiniz.)

   - ISV SaaS teklifleri için teklifin satın alma için sunulmamasının birkaç nedeni olabilir: ISV müşterinin fatura ülkesini veya bölgesini desteklemiyor olabilir; ISV, teklifi CSP programı aracılığıyla kullanılabilir hale getirmek için seçilmiş olabilir; ya da ISV, teklifi yalnızca belirli CSP iş ortakları için [özel](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) olarak yapmış olabilir. ISV teklifi Ayrıca Iş Ortağı Merkezi (örneğin, kapsayıcılar veya bazı kullanım tabanlı teklifler) üzerinden transactable de olmayabilir.  

6. Eklemek istediğiniz her abonelik için, lisansların (gerekirse) sayısını girin ve **Sepete Ekle**' yi seçin.

7. Abonelik eklemeyi bitirdiğinizde, **gözden geçir** ' i seçin ve siparişinizi gözden geçirin.

8. Siparişlerinizi gözden geçirdikten ve bu abonelikleri satın almaya hazırladıktan sonra **satın al**' ı seçin.

9. Bir müşteri için abonelik satın aldıktan sonra aşağıdakiler gerçekleşir:

    - Bu müşterinin **abonelikler** sayfasından abonelik adı ' nı seçerek aboneliği gözden geçirebilir veya düzenleyebilirsiniz. Buradan, varsa eklenti lisanslarını seçebilirsiniz, lisans miktarını değiştirebilir veya aboneliği askıya alabilirsiniz.

    **ISV SaaS (lisans tabanlı ve tarifeli) abonelikler için:**
    - ISV yayımcısının sitesine bir bağlantı alacaksınız. Bu bağlantı, müşterinin aboneliğine ait dağıtım veya hesap kurulumunu tamamlamanıza yardımcı olmalıdır.
      
    >[!NOTE]
    > Ne siz ne de müşteriniz bu tür ISV aboneliği için kurulumu/sağlamayı tamamlamaya yönelik yönergeleri içeren bir e-posta alacaksınız.)

    - Aboneliğiniz 30 günlük ücretsiz deneme sürümü ile birlikte geliyorsa, ücretsiz deneme süresi otomatik olarak uygulanır. CSP programındaki bir iş ortağı olarak, müşteriler için satın aldığınız tekliflerle ilgili ücretsiz deneme süresini beklenemez. Ücretsiz deneme süresi sona erdiğinde, abonelik dönemi başlar ve abonelik, ücretli duruma dönüştürülür. Abonelik daha sonra aynı zamanlamaya göre otomatik olarak yenilenecek.
   
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

Etkin abonelikler varsayılan olarak abonelik süresi sona erdiğinde otomatik olarak yenilenecek şekilde ayarlanır. Ticari [market ürünlerine abonelikler için](csp-commercial-marketplace-overview.md)isteğe bağlı olarak aboneliği otomatik olarak yenilemeyi seçebilirsiniz.

Etkin bir ticari market aboneliğinin otomatik olarak yenilenmesini durdurmak için:

1. İş Ortağı Merkezi [oturum açın.](https://partner.microsoft.com/dashboard)

2. Yeni İş Ortağı Merkezi **Müşteriler'i** ve ardından listeden bir müşteri seçin.

3. **Abonelikler**'i seçin. Bu, müşteri için satın aldığınız lisans tabanlı abonelikleri listeler.

4. Abonelik **sütununda** değiştirmek istediğiniz aboneliği seçin.

5. Abonelik ayrıntıları sayfasında Durum bölümünü **bulun ve** Otomatik yenile **kutusunun işaretini** kaldırın.

6. **Gönder**’i seçin.

## <a name="next-steps"></a>Sonraki adımlar

- [Müşterileriniz için ticari market ürünleri satın alma](csp-commercial-marketplace-purchase.md)

- [Müşterileriniz için ticari market ürünlerini yönetme](csp-commercial-marketplace-manage.md)

- [Ticari markete genel bakış](csp-commercial-marketplace-overview.md)