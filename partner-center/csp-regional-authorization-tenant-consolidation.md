---
title: CSP bölgesel yetkilendirme kiracı birleştirmesi
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Farklı ülke/bölgeler için kiracıları birleştirmek için bu yönergeleri kullanın. Bu, müşteri hesaplarını ve müşteri aboneliklerini geçirme adımlarını içerir.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: d2168dcd60b8675a21960918dab49b778025fa51
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147590"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>CSP bölgesel yetkilendirme kiracı birleştirme yönergeleri

**Uygulama:** İş Ortağı Merkezi | İş Ortağı Merkezi için Microsoft Cloud for US Government

**Uygun roller:** Genel yönetici | Yönetici aracısı

\[Bazı bilgiler, ticari olarak yayınlanmadan önce önemli ölçüde değiştirilabilecek, önceden yayımlanan ürünle ilgilidir. Burada verilen bilgilerle ilgili olarak Microsoft açık veya zımni hiçbir garanti vermez.\]

İşletmeniz için kiracıları birleştirin. Farklı ülke/bölgeler için kiracıları birleştirmek için bu yönergeleri kullanın.

>[!NOTE]  
>Geçişte olduğunuz hesapta yer alan müşterilerin her biri için sağlanan tüm aboneliklerin ve lisans sayılarının farkında olmak gerekir. Geçiş işleminin bir parçası olarak yeni merkezi CSP hesabı altında aynı lisans sayılarını tam olarak aynı abonelikleri yeniden sağlarsınız. Merkezi kiracıya taşınarak müşterilerin listesini oluşturmanıza yardımcı olmak için dışarı aktarma listesi özelliğini kullanın.  Birleştirme tamamlandıktan sonra önceki kiracı durumuna geri dönebilirsiniz. Müşteri eylemi de gerekli olabilir.

## <a name="prepare-for-migration"></a>Geçiş için hazırlanma

- Geçiş **İş Ortağı Merkezi** (yeni hesaba  geçiş yapmak için) kullanarak oturum açın ve tüm müşterileri ve bu müşteriler için sağlanan tüm hizmetleri gözden geçirin.

- Bu hesabın oturumlarını açın.

## <a name="migrate-customer-accounts"></a>Müşteri hesaplarını geçirme

1. Geçiş **(yeni İş Ortağı Merkezi** **hesabıyla** (müşterileri geçişte olduğunuz hesap) oturum açın.

2. **Müşteriler**’i seçin.

3. Kurumsal **bayi ilişkisi isteğide bulun seçeneğini seçin.** Müşterilerinize göndermek için size varsayılan bir e-posta iletisi gönderilir. Bu ileti, yeni İş Ortağı Merkezi hesabınız için benzersiz kuruluş kimliğine sahip bir URL içerir.

4. **Müşteri eylemi:** Geçirmek istediğiniz her bir etkin müşterilerin bu URL 'YI ziyaret etmesini sağlayın. URL 'YI açarken, müşterinin Office 365 portalında oturum açması istenir. Müşteri, Azure ve Office 365 yönetim portallarına erişmek için kullandıkları aynı kuruluş KIMLIĞINI kullanarak oturum açar.

5. Oturum açtıktan sonra, **müşteri hesabına** ait genel YÖNETICININ yeni CSP hesabına yönetici ayrıcalıkları sağlayan bir anlaşma göndermesi istenir. Kabul ederse, müşteri onay kutusunu seçer ve ilişkiye izin vermeyi kabul eder.

Müşteriler, sözleşmeyi gönderdikten sonra iş ortağının müşteri listesinde görünür.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Office 365 ve Azure olmayan kullanım tabanlı abonelikleri geçirme

1. Müşterinizin Sözleşmesi imzalandıktan sonra, kendi aboneliklerini merkezi Iş ortağı kiracınız altında yeniden oluşturabilirsiniz.

2. **Iş Ortağı Merkezi**'nden **müşteriler**' i seçin.

3. Geçirmek istediğiniz müşterinin şirket adını açın.

4. **Abonelik Ekle**' yi seçin.

5. Katalogdan doğru abonelikleri ve lisans sayılarını ekleyin. **İş ortağı** hesaplarından geçiş sırasında belirtilen bilgilerle doğrulayın.

   :::image type="content" source="images/regionalcustomer2.png" alt-text="Müşteri listesi":::

6. Gönder ' i seçin **.**

   Hizmetler artık **müşteriye iş ortağı** hesabına geçiş üzerinden sağlanır.

7. Tüm ek müşterilerin aboneliklerini geçirmek için bu adımları tekrarlayın.

Bir sonraki bölüme geçmeden önce **, iş ortağı** hesaplarından geçiş altında bulunan tüm müşteri aboneliklerinin **iş ortağı hesabına** geçiş altında yeniden sağlandığını doğrulayın.

> [!NOTE]
> İş ortakları, iş ortağı Merkezi **'nde iş ortağı** kiracı hesabından geçiş sırasında abonelikleri askıya almalıdır. bu abonelikler, Çift faturalandırma işleminin gerçekleşmemesini sağlamak için Iş Ortağı Merkezi 'nde **iş ortağı kiracı** hesabı altına geçirilir ve ayarlanır. Aboneliklerden Geçiş doğru şekilde devre dışı bırakılamayarak oluşan faturalama çakışmaları nedeniyle krediler için **destek istekleri reddedilir.**

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>İş ortağı hesabından geçiş altında Office 365 aboneliklerini devre dışı bırakma

CSP aboneliğini İş ortağı hesaplarından **Geçiş altında devre** dışı bırakmak gelecekte faturalamayı durdurur. Geçiş işlemi sırasında Azure abonelikleri otomatik olarak devre dışı bırakılana kadar Azure aboneliklerini el ile devre dışı bırakmanız gerekmez.

1. CSP **hesabından İş Ortağı Merkezi** **hesabıyla** oturum açın ve müşteri listesine gidin.

2. Devre dışı bırakmak için müşteriyi aboneliklerle açın ve devre dışı bırakmak için ilk teklifi seçin.

3. Aboneliği askıya alındı **olarak ayarlayın** ve gönder'i **seçin.**

   >[!Note]
   >Aboneliğin askıya alınması, çift faturalamanın oluşmaz.

   Abonelik, **abonelikler listesinde** askıya alınmış olarak görünür.

4. Müşteri altındaki tüm abonelikler için bu adımları tekrarlayın. Tüm show askıya alınmış **olduğunu doğrulayın.**

5. Listeden bir sonraki müşteriyi seçin ve tüm abonelikleri devre dışı bırakma işlemini tekrarlayın.

## <a name="migrating-azure-usage-based-subscriptions"></a>Azure kullanım tabanlı abonelikleri kullanma

Azure, Office 365 CSP abonelikleri'nden farklı olarak kullanım tabanlı CSP aboneliklerini el ile geçirmeniz gerekmez. Microsoft Azure Desteği, Azure aboneliklerini ve dağıtılan tüm hizmetleri veya kaynakları **CSP** kurumsal bayi hesaplarından **CSP** kurumsal bayi hesabına geçişten geçirir. Bu geçiş sırasında müşteriye hizmet kesintisi yaşanmaz.

1. Azure aboneliklerini geçirecek olan müşteri hesaplarının yeni CSP hesabına geçiş ile ilişkilendirilecek **sözleşmeyi kabul etmelerini** sağlar.

2. Microsoft'a hangi müşteri hesaplarının geçişe hazır olduğunu bildirecek ve bu müşterinin şirket adlarını sağlayacaksınız.

3. Microsoft, Azure kullanım tabanlı abonelikleri geçirir ve geçiş tamamlandığında size bilgi sağlar.

4. CSP satıcısı hesabından geçiş altında olan Azure **aboneliğinin, Iş** Ortağı Merkezi 'nde müşteri abonelikleri bölümünde **askıya alındı** olarak işaretlendiğinden emin olmanız gerekir.

5. CSP satıcısı hesabına **geçilen** Azure aboneliğinin, artık müşteri abonelikleri bölümünde Iş Ortağı Merkezi 'nde **etkin** durumunu gösterdiğini doğrulayın.

   >[!Note]
   > Müşterinin altındaki abonelikleri devre dışı bırakmak, müşterinin görünüşünü müşteriler listesinde değiştirmez. Şu anda listedeki müşterileri kaldırma seçeneği yoktur. İş **ortakları, gelecekteki hesaptan gelen** geçiş aşamasından bu müşterilere abonelikleri geri eklemektan kaçınmalıdır.

6. Hesap (ler) **den** geçiş için gelecekteki ücretleri durdurmak üzere tüm müşterileriniz kapsamındaki tüm abonelikler için bu adımları yineleyin. İş ortağı, İptalin günü ile fatura döneminin son günü arasındaki kullanılmamış gün sayısı için krediyle birlikte bir son fatura alacaktır. Son fatura döneminden sonra gelecek fatura üretilecektir.

### <a name="additional-information"></a>Ek bilgiler

- Aboneliği devre dışı bırakmadan önce, CSP hesabından **geçilen** aboneliğin devre dışı bırakılması, **hizmetin CSP hesabından** sağlandığı sürece son müşterinin hizmetini etkilemez.

- Abonelikler müşteri tarafından kullanılamaz ve askıya alındığında veya iptal edildiğinde ücret üretmez.

- Şu anda **müşteriler** listesinden bir müşteriyi tamamen kaldırmanın bir yolu yoktur.
- 
    >[!Note]
    > İş ortakları, iş ortağı merkezi 'nde iş ortağı kiracı hesabından **alınan** abonelikleri askıya almalıdır. bu abonelikler, Çift faturalandırma işleminin gerçekleşmemesini sağlamak **için hesap geçişi** altında hesaba geçirilir ve ayarlanır. Microsoft, **aboneliklerden** askıya alma işleminin askıya alınma durumuna doğru ayarlamamasından kaynaklanan herhangi bir çakışma nedeniyle kredilerin isteklerini desteklemez.

### <a name="simplify-migration-using-export"></a>Dışarı aktarma kullanarak geçişi basitleştirme

Dışarı **Aktarma İşlevini** kullanarak, yeni birleştirilmiş yapıda kullanmak için ihtiyacınız olan abonelikleri yakaabilirsiniz:

1. Müşterilerin **listesini** İş Ortağı Merkezi için İş Ortağı Merkezi'yi seçin. 

2. İstediğiniz müşteri adını açın.

3. Abonelikler **sayfasında Abonelikleri** Dışarı **Aktar'ı** seçerek aboneliklerin ayrıntılarını bir Excel dosyasına aktarın.

4. Yeni birleştirilmiş kiracınıza abonelikleri yeniden oluşturmak için bu listeyi kullanın.

### <a name="api-registration"></a>API kaydı

API kaydı hakkında daha fazla bilgi için [bkz. Api erişimini İş Ortağı Merkezi.](/partner-center/develop/set-up-api-access-in-partner-center)

## <a name="next-steps"></a>Sonraki adımlar

- [Bulut Çözümü Sağlayıcısı CSP tekliflerini satarak bölgesel pazarları ve para birimlerini programla](regional-authorization-overview.md)
