---
title: CSP bölgesel yetkilendirme kiracı birleştirmesi
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Farklı ülkeler/bölgeler için kiracılar birleştirmek üzere bu yönergeleri kullanın. Bu, müşteri hesaplarını ve müşteri aboneliklerini geçirmeye yönelik adımları içerir.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 923f07c51611670023ef58e4ed340d9cee49b804d784e702ae775c06893ba4bd
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115690265"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>CSP bölgesel yetkilendirme kiracı birleştirme yönergeleri

**Uygulama hedefi**: Iş Ortağı Merkezi | Microsoft Cloud for US Government için iş ortağı Merkezi

**Uygun roller**: genel yönetici | Yönetim Aracısı

\[Bazı bilgiler, ticari olarak yayınlanmadan önce önemli ölçüde değiştirilebilecek, önceden yayınlanan ürünle ilgilidir. Burada verilen bilgilerle ilgili olarak Microsoft açık veya zımni hiçbir garanti vermez.\]

İş için kiracılar birleştirebilirsiniz. Farklı ülkeler/bölgeler için kiracılar birleştirmek üzere bu yönergeleri kullanın.

>[!NOTE]  
>Geçiş yaptığınız hesapta müşterilerinizin her biri için sağlanan aboneliklerin ve lisans sayılarının tümünün farkında olmanız gerekir. Geçiş işleminin bir parçası olarak, yeni merkezi CSP hesabı altında aynı lisans sayılarıyla aynı tam abonelikleri yeniden hazırlayacaksınız. Merkezi kiracıya geçiş yapılacak müşterilerin bir listesini oluşturmaya yardımcı olması için listeyi dışarı aktar özelliğini kullanın.  Birleştirme işlemi tamamlandıktan sonra önceki kiracı durumuna geri döndüremezsiniz. Müşteri eylemi de gerekebilir.

## <a name="prepare-for-migration"></a>Geçiş için hazırlanma

- Geçiş **hesabını (** yeni hesaba geçigeçiizin) kullanarak **iş ortağı merkezi** 'nde oturum açın ve tüm müşterileri ve bu müşteriler için sağlanan tüm hizmetleri gözden geçirin.

- Bu hesabın oturumunu kapatın.

## <a name="migrate-customer-accounts"></a>Müşteri hesaplarını geçirme

1. Geçiş (yeni) hesabıyla **Iş Ortağı Merkezi**  'nde oturum **açın (müşterileri** geçiş yaptığınız bir hesap).

2. **Müşteriler**’i seçin.

3. **Satıcı Ilişkisi iste**' yi seçin. Müşterilerinize göndermek için varsayılan bir e-posta iletisi sunulur. Bu ileti, yeni Iş Ortağı Merkezi hesabınıza özel kuruluş KIMLIĞINE sahip bir URL içerir.

4. **Müşteri eylemi:** Geçirmek istediğiniz her bir etkin müşterilerin bu URL 'YI ziyaret etmesini sağlayın. URL 'yi açarken, müşterinin Office 365 portalında oturum açması istenir. müşteri, Azure ve Office 365 yönetim portallarına erişmek için kullandıkları aynı kuruluş kimliğini kullanarak oturum açar.

5. Oturum açtıktan sonra, **müşteri hesabına** ait genel YÖNETICININ yeni CSP hesabına yönetici ayrıcalıkları sağlayan bir anlaşma göndermesi istenir. Kabul ederse, müşteri onay kutusunu seçer ve ilişkiye izin vermeyi kabul eder.

Müşteriler, sözleşmeyi gönderdikten sonra iş ortağının müşteri listesinde görünür.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Office 365 ve Azure olmayan kullanım tabanlı abonelikleri geçirme

1. Müşterinizin Sözleşmesi imzalandıktan sonra, kendi aboneliklerini merkezi Iş ortağı kiracınız altında yeniden oluşturabilirsiniz.

2. **Iş Ortağı Merkezi**'nden **müşteriler**' i seçin.

3. Geçirmek istediğiniz müşterinin şirket adını açın.

4. **Abonelik Ekle**' yi seçin.

5. Katalogdan doğru abonelikleri ve lisans sayılarını ekleyin. **İş ortağı** hesaplarından geçiş sırasında belirtilen bilgilerle doğrulayın.

   :::image type="content" source="images/regionalcustomer2.png" alt-text="Müşteri listesi.":::

6. Gönder ' i seçin **.**

   Hizmetler artık **müşteriye iş ortağı** hesabına geçiş üzerinden sağlanır.

7. Tüm ek müşterilerin aboneliklerini geçirmek için bu adımları tekrarlayın.

Bir sonraki bölüme geçmeden önce **, iş ortağı** hesaplarından geçiş altında bulunan tüm müşteri aboneliklerinin **iş ortağı hesabına** geçiş altında yeniden sağlandığını doğrulayın.

> [!NOTE]
> İş ortakları, iş ortağı Merkezi **'nde iş ortağı** kiracı hesabından geçiş sırasında abonelikleri askıya almalıdır. bu abonelikler, Çift faturalandırma işleminin gerçekleşmemesini sağlamak için Iş Ortağı Merkezi 'nde **iş ortağı kiracı** hesabı altına geçirilir ve ayarlanır. Aboneliklerden geçiş işleminin doğru şekilde devre dışı bırakılmasından kaynaklanan bir çakışma nedeniyle, destek istekleri krediler için  reddedilir.

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>iş ortağı hesabından geçilen Office 365 aboneliklerini devre dışı bırakma

**İş ortağı** hesaplarından GEÇIŞ altında CSP aboneliğini devre dışı bırakmak gelecekteki faturalandırmayı durduruyor. Azure abonelikleri, geçiş işlemi sırasında otomatik olarak devre dışı bırakıldığından Azure aboneliklerini el ile devre dışı bırakmanız gerekmez.

1. **CSP hesabından** geçiş yaparken **iş ortağı merkezi** ' nde oturum açın ve müşteri listesine gidin.

2. Devre dışı bırakmak için abonelikleri olan müşteriyi açın ve ardından devre dışı bırakılacak ilk teklifi seçin.

3. Aboneliği **askıya alındı** olarak ayarlayın ve ardından **Gönder**' i seçin.

   >[!Note]
   >Aboneliğin askıya alınması, iki faturalandırma gerçekleşmemesini sağlar.

   Abonelik, abonelikler listesinde **askıya alındı** olarak gösterilir.

4. Müşterinin altındaki tüm abonelikler için bu adımları tekrarlayın. Tüm Show askıda olduğunu doğrulayın **.**

5. Listede bir sonraki müşteriyi seçin ve tüm abonelikleri devre dışı bırakma işlemini tekrarlayın.

## <a name="migrating-azure-usage-based-subscriptions"></a>Azure kullanım tabanlı abonelikleri geçirme

Office 365 CSP aboneliklerinden farklı olarak, Azure, kullanım tabanlı CSP aboneliklerinin el ile geçirilmesi gerekmez. Microsoft Azure Destek, Azure aboneliklerini ve dağıtılan tüm hizmet veya kaynakları **, CSP satıcı** hesaplarından geçiş **aşamasından CSP satıcı hesabına geçme durumuna** geçirmeye yönelik olarak geçirilir. Bu geçiş sırasında müşteriye hizmet kesintisi olmaz.

1. Azure abonelikleri 'nin geçirileceği müşteri hesaplarının, yeni CSP hesabına **geçme** ile ilişkilendirilecek anlaşmayı kabul ettiğinden emin olun.

2. Microsoft 'un hangi müşteri hesaplarının geçirmeye hazırlanmaya yönelik olduğunu bilgilendirirsiniz ve bu müşterinin şirket adlarını sağlayabilirsiniz.

3. Microsoft, Azure kullanım tabanlı abonelikleri geçirir ve geçiş tamamlandığında size bildirir.

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

**Dışarı aktarma işlevini** kullanarak, yeni birleştirilmiş yapınıza kullanmanız gereken abonelikleri yakalayabilirsiniz:

1. Müşterilerin listesini görmek için Iş Ortağı Merkezi ' nde **müşteriler** ' i seçin. 

2. İstenen müşteri adını açın.

3. **abonelikler sayfasında,** aboneliklerin ayrıntılarını bir Excel dosyasına dışarı aktarmak için **abonelikleri dışarı aktar** ' ı seçin.

4. Yeni birleştirilmiş kiracınızdaki abonelikleri yeniden oluşturmak için bu listeyi kullanın.

### <a name="api-registration"></a>API kaydı

API kaydı hakkında daha fazla bilgi için bkz. [Iş Ortağı Merkezi 'NDE API erişimi ayarlama](/partner-center/develop/set-up-api-access-in-partner-center).

## <a name="next-steps"></a>Sonraki adımlar

- [CSP teklifleri satın oluşturabileceğiniz Bulut Çözümü Sağlayıcısı program bölgesel pazarlar ve para birimleri](regional-authorization-overview.md)
