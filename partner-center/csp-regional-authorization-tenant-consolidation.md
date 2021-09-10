---
title: CSP bölgesel yetkilendirme kiracı birleştirmesi
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Farklı ülke/bölgeler için kiracıları birleştirmek için bu yönergeleri kullanın. Bu, müşteri hesaplarını ve müşteri aboneliklerini geçirme adımlarını içerir.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: f4df62bddba501552eafe2142f4c0656b8eefc7c
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961315"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>CSP bölgesel yetkilendirme kiracı birleştirme yönergeleri

**Uygulama:** İş Ortağı Merkezi | İş Ortağı Merkezi için Microsoft Cloud for US Government

**Uygun roller:** Genel yönetici | Yönetici aracısı

\[Bazı bilgiler, ticari olarak yayımlanmadan önce önemli ölçüde değiştirilabilecek, önceden yayımlanan ürünle ilgilidir. Burada verilen bilgilerle ilgili olarak Microsoft açık veya zımni hiçbir garanti vermez.\]

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

4. **Müşteri Eylemi:** Geçirmek istediğiniz etkin müşterilerin her biri bu URL'yi ziyaret eder. URL'yi a açması için müşteriden Office 365 istenir. Müşteri, Azure'a erişmek ve yönetim portallarını kullanmak için Office 365 oturumlar.

5. Oturum açmanın ardından, müşteri  hesabının Genel Yöneticisi'nin yeni CSP hesabına yönetici temsilcisi ayrıcalıkları veren bir sözleşme göndermesi istenir. Kabul ederse müşteri onay kutusunu seçer ve ilişkiyi yetkilendirmeyi kabul eder.

Müşteriler, anlaşma gönderildikten sonra iş ortağının müşteri listesinde tek tek görünür.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Azure'Office 365 olmayan abonelikleri ve kullanım tabanlı olmayan abonelikleri Office 365

1. Müşteriniz anlaşmayı imzaladığı zaman aboneliklerini Merkezi İş Ortağı Kiracınız altında yeniden oluşturabilirsiniz.

2. Bu **İş Ortağı Merkezi** Müşteriler'i **seçin.**

3. Geçirmek istediğiniz müşterinin şirket adını açın.

4. Abonelik **ekle'yi seçin.**

5. Katalogdan doğru abonelikleri ve lisans sayılarını ekleyin. İş ortağı hesaplarından **Geçiş'te sağlanan bilgilerle** doğrulayın.

   :::image type="content" source="images/regionalcustomer2.png" alt-text="müşteri listesi.":::

6. **Gönder'i seçin.**

   Hizmetler artık müşteriye İş Ortağı hesabına **geçişten** sağlanıyor.

7. Tüm ek müşteriler için abonelikleri geçirmek için bu adımları tekrarlayın.

Sonraki bölüme devam etmeden önce İş ortağı  hesaplarından geçiş bölümünde var olan tüm müşteri abonelikleri, İş ortağı hesabına geçiş bölümünde **yeniden** sağlandığından emin olun.

> [!NOTE]
> İş ortaklarının,  İş Ortağı Merkezi'daki İş Ortağı Kiracı hesabından Geçiş'te abonelikleri askıya alması  ve çift faturalamanın oluşmaması için bu aboneliklerin İş Ortağı Merkezi kiracıda İş Ortağı Kiracısına Geçiş hesabı altında ayarladığı gün askıya alması gerekir. Aboneliklerden Geçiş doğru şekilde devre dışı bırakılamayarak oluşan faturalama çakışmaları nedeniyle krediler için **destek istekleri reddedilir.**

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>İş ortağı hesabından Office 365 abonelikleri devre dışı bırakma

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

CsP Office 365 aksine, Azure'ın kullanım tabanlı CSP aboneliklerini el ile geçirmesi gerekmez. Microsoft Azure Destek, Azure aboneliklerini ve dağıtılan tüm hizmetleri veya kaynakları **CSP** kurumsal bayi hesaplarından **CSP** kurumsal bayi hesabına geçişten geçirir. Bu geçiş sırasında müşteriye hizmet kesintisi yaşanmaz.

1. Azure aboneliklerini geçirecek olan müşteri hesaplarının yeni CSP hesabına geçiş ile ilişkilendirilecek **sözleşmeyi kabul etmelerini** sağlar.

2. Microsoft'a hangi müşteri hesaplarının geçişe hazır olduğunu bildirecek ve bu müşterinin şirket adlarını sağlayacaksınız.

3. Microsoft, Azure kullanım tabanlı abonelikleri geçirir ve geçiş tamamlandığında size bilgi sağlar.

4. **CsP** kurumsal bayi hesabından geçiş bölümünde Azure aboneliğinin artık  müşteri abonelikleri bölümünde İş Ortağı Merkezi olarak işaretlenir.

5. CSP kurumsal bayi hesabına geçiş **bölümündeki** Azure aboneliğinin artık  müşteri abonelikleri bölümünde İş Ortağı Merkezi durumunun etkin olduğunu onaylayın.

   >[!Note]
   > Müşterinin altındaki aboneliklerin devre dışı bırakılması, Müşteriler listesinde müşterinin görünümünü değiştirmez. Şu anda listeden müşteri kaldırma seçeneği yoktur. İş ortakları gelecekte bu müşterilere Geçiş Hesabından **abonelik eklemekten** kaçınmalı.

6. Geçiş Hesabı'nın gelecekteki ücretlerini durdurmak için tüm müşterileriniz altındaki tüm abonelikler için **bu adımları** tekrarlayın. İş ortağı, iptal günü ile faturalama döneminin son günü arasındaki kullanılmayan gün sayısı için krediye sahip son bir fatura alır. Bu son faturalama döneminden sonra gelecekteki faturalar oluşturulmaz.

### <a name="additional-information"></a>Ek bilgiler

- Aboneliğin CSP  hesabından Geçişten devre dışı bırakılması, hizmetin aboneliği devre dışı bırakmadan önce **CSP** hesabına geçişten sağlanması şartıyla son müşterinin hizmetini etkilemez.

- Abonelikler müşteri tarafından kullanılamaz ve askıya alındı veya iptal edildiklerde ücret oluşturmaz.

- Şu anda bir müşteriyi Müşteriler listesinden tamamen kaldırmanın bir **yolu** yoktur.
- 
    >[!Note]
    > İş ortaklarının aynı  gün içinde İş ortağı kiracı hesabından geçişini askıya al İş Ortağı Merkezi,  bu abonelikler çift faturalamanın oluşmaması için Geçiş Hesabı altında ayarlanır. Microsoft, Aboneliklerden askıya Alma ayarının doğru şekilde ayarilamama nedeniyle faturalamada oluşan çakışmalar nedeniyle kredi **isteklerini** desteklemez.

### <a name="simplify-migration-using-export"></a>Dışarı Aktarma kullanarak geçişi basitleştirme

Dışarı **Aktarma İşlevini** kullanarak, yeni birleştirilmiş yapıda kullanmak için ihtiyacınız olan abonelikleri yakaabilirsiniz:

1. Müşterilerin **listesini** görmek İş Ortağı Merkezi'da Müşteriler'i seçin. 

2. İstediğiniz müşteri adını açın.

3. Abonelikler **sayfasında Abonelikleri** Dışarı **Aktar'ı** seçerek aboneliklerin ayrıntılarını bir Excel aktarın.

4. Yeni birleştirilmiş kiracıda abonelikleri yeniden oluşturmak için bu listeyi kullanın.

### <a name="api-registration"></a>API kaydı

API kaydı hakkında daha fazla bilgi için [bkz. Api erişimini İş Ortağı Merkezi.](/partner-center/develop/set-up-api-access-in-partner-center)

## <a name="next-steps"></a>Sonraki adımlar

- [Bulut Çözümü Sağlayıcısı CSP tekliflerini satarak bölgesel pazarları ve para birimlerini programla](regional-authorization-overview.md)
