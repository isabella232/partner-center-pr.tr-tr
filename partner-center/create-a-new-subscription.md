---
title: Iş Ortağı Merkezi 'nde müşteri abonelikleri oluşturma
ms.topic: how-to
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft tarafından yayımlanan ürünlerin yanı sıra üçüncü taraf ISV 'Ler tarafından yayımlanan SaaS ürünleri için müşterilerinize abonelik satma hakkında bilgi edinin.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 9052954c81ef55a2bfa06778ace651c9d0f9b26f
ms.sourcegitcommit: e0444145d7720df948b9d02ae2469206db48dba5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110201417"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Müşteri aboneliklerini oluşturma, askıya alma veya iptal etme

**Uygulama hedefi**: Iş Ortağı Merkezi | ABD kamu için Microsoft Bulut iş ortağı Merkezi

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
   - **Yayımcı:** Yalnızca **Microsoft'un** tekliflerini  görmek için Microsoft'u veya ISV'ler tarafından yayımlanan ticari market ürünlerini görmek için İş Ortağı'ı seçin.
   - **Faturalama türü:** Kullanmak istediğiniz abonelik faturalama türünü seçin: **Lisans veya** **Kullanım.** Aylık [ve yıllık faturalama sıklığı](license-based-billing.md) arasında karar alamanıza yardımcı olacak bilgiler için bkz. Lisans tabanlı faturalama.
   - **Kategori:** Kurumsal, **Küçük** **işletme veya** Deneme'yi **seçin.** Deneme abonelikleri hakkında bilgi için [bkz. Müşterilerinize Microsoft ürünlerinin denemelerini teklif edin.](offer-your-customers-trials-of-microsoft-products.md)

5. Müşteriniz için satın almak istediğiniz ürün aboneliklerini seçin. Gördüğünüz ürünler, müşteri segmenti türüne (eğitim, kamu vb.) ve sizin uyguladık filtrelere bağlıdır. Market'te gösterilen bazı teklifler belirli bir müşteri veya belirli bir CSP iş ortağı tarafından her zaman kullanılabilir olabilir. Bunun nedeni:

   - Müşterinin zaten bu ürüne bir aboneliği vardır ve yalnızca bir ürüne izin verilir

   - Müşterinin aboneliği askıya alınmış olabilir (Bu durumda yeni bir abonelik satın almak yerine aboneliği yeniden etkinleştirebilirsiniz.)

   - ISV SaaS tekliflerinin satın alınamama nedenlerinden birkaçı olabilir: ISV müşterinin fatura ülkesi veya bölgesi için destek sunmayabiliyor olabilir; ISV, teklifi CSP programı aracılığıyla kullanılabilir halememiş olabilir; veya ISV teklifi yalnızca belirli CSP [iş](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) ortaklarına özel yapmış olabilir. ISV teklifi, kapsayıcılar veya kullanım tabanlı İş Ortağı Merkezi gibi) aracılığıyla işlem gerçekleştirilebilir de değildir.  

6. Eklemek istediğiniz her abonelik için lisans sayısını girin (gerekirse) ve Sepete **ekle'yi seçin.**

7. Abonelik eklemeyi bitirdikten sonra Siparişinizi gözden **geçir'i** seçin.

8. Siparişlerinizi gözden geçirerek bu abonelikleri satın almaya hazır olduktan sonra Satın Al'ı **seçin.**

9. Bir müşteri için abonelik satın alırsınız, aşağıdakiler gerçekleşir:

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

İş ortakları, müşteri tarafından talep edilmesi ya da ödememe veya sahtekarlık durumlarında aboneliği askıya alabilir veya iptal edebilir.

### <a name="suspend-a-subscription"></a>Bir aboneliği askıya alma

Aboneliğin durumunu Askıya Alındı olarak **değiştirebilirsiniz.** Kullanıcılar oturum alamiyor veya hizmetlere erişemiyor.

1. İş Ortağı Merkezi [oturum açın.](https://partner.microsoft.com/dashboard)

2. Yeni İş Ortağı Merkezi **Müşteriler'i** ve ardından listeden bir müşteri seçin.

3. Yönetmek istediğiniz aboneliği seçin.

4. **Durum** bölümünde **Askıya Alındı**'yı seçin. Sonra **Gönder** ile yaptığınız değişiklikleri gönderin.

5. Abonelik 90 gün veya 90 gün içinde yeniden etkinleştirildiği sürece tüm veriler silinir ve hesabın açılmasıyla ilk faturalama dönemi (en fazla 120 gün) arasındaki gün sayısına ek olarak bu süreye dahil olur.

Bir aboneliği askıya alırsanız, Askıya Alınmış düğmesinin altında gördüğünüz tarih, aboneliği yeniden etkinleştirmezsanız aboneliğin süresinin otomatik olarak ne zaman dol olacağını gösterir.  

>[!NOTE]
>CSP abonelikleri, hizmetlerin çalışmaya devam eder ancak abonelik herhangi bir faturalama ücreti oluşturmazken süresi dolmuş bir süreye (doğrudan web abonelikleri gibi) sahip değildir. CSP abonelikleri etkin veya askıya alınmış (veya tamamen silinmiş).

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

- [Müşterileriniz için ticari market ürünlerini yönetme](csp-commercial-marketplace-manage.md)

- [Ticari markete genel bakış](csp-commercial-marketplace-overview.md)