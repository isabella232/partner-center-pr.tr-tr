---
title: Ödeme yapılmaması, sahtekarlık veya suistimal durumlarını yönetme
description: Iş Ortağı Merkezi 'nde bu riskleri yönetmek ve azaltmak için çevrimiçi işlemlere ve en iyi yöntemlere dahil olan çeşitli riskler hakkında bilgi edinin.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: 75881544097abdfac8d6f96bde37e9700eb28cf7
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132358"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>Ödeme alınamaması, dolandırıcılık veya kötüye kullanım durumlarını İş Ortağı Merkezi’nde yönetme

Aşağıdakiler cihazlar için geçerlidir:

- Microsoft kamu bulutu için iş ortağı Merkezi

**Uygun roller**

- Genel yönetici
- Kullanıcı Yönetimi Yöneticisi
- Yönetim Aracısı
- Faturalama yöneticisi

Müşterileriniz ve/veya müşterilerin satın alınan hizmetlerin ödemesinden sorumlu satın alma işlemleri için mali olarak sorumlusunuz. Bu nedenle, *sahte önleme ve algılama riski azaltma denetimlerini yerleştirmenizi öneririz*.

Sahte etkinlik veya kötüye kullanımı önlemek için, olası riskleri anlamak ve pozlandırmayı azaltabileceğiniz ilke ve uygulamalar geliştirmek önemlidir.

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a>Microsoft kabul edilebilir kullanım Ilkesi zorlaması

Microsoft, kabul edilen kullanım Ilkesini ihlal ettiğimiz ya da şüpheli olduğunu düşündüğünüz iş ortağı veya müşteri etkinliğini algılarsa, zorlama adımları ele alınacaktır. Müşteri hemen askıya alınabilir. Microsoft tarafından yapılan istekleriniz için zorlama eylemleri hakkında bilgilendirilirsiniz.

## <a name="abuse-of-service-risks"></a>Hizmet riskleri kötüye kullanımı

**Hizmet riskleri kötüye kullanımı,** bulut hizmetlerini Microsoft 'un kabul edilebilir kullanım ilkesi ihlaline neden olan müşteriler anlamına gelir.

### <a name="examples-of-abuse-of-service"></a>Hizmetin kötüye kullanımı örnekleri

Bu Microsoft 'un kabul edilebilir kullanım ilkesi ihlalleri örnekleri şunlar olabilir:

- Yığın posta
- Bilgisayar korsanlığı
- Dağıtılmış hizmet reddi (DDoS) saldırıları
- Bitpara madenciliği
- Kötü amaçlı yazılım dağıtımı
- Korsan aboneliklerin el satımı

## <a name="theft-of-service-risks"></a>Hizmet riskleri hırsızlığı

**Hizmet riskleri hırsızlığı** , tüketilen hizmetler için ödeme yapma amacı olmayan müşteriler anlamına gelir. Bu hırsızlık, çalınmış ödeme araçları 'nı kullanarak, yanlış faturalandırma bilgileri sağlar ve/veya bekleyen bakiyelerde varsayılan değerleri içerir.

### <a name="examples-of-service-theft"></a>Hizmet hırsızlığı örnekleri

Bu çevrimiçi işlem risklerine örnek olarak şunlar verilebilir:

- Kişide olmayan işlemler ("kredi kartı yok" işlemleri)
- Yanlış temsil edilen kimlikler
- İlk ödeme alınmadan önce sağlanan ve kullanılan hizmetler
- Çevrimiçi sahtekarlık için gelişen pazarlar ve/veya yüksek riskli bölgeler
- Hesap oluşturmayı otomatikleştirin ve hatalı aktör yaparak satın alabilirsiniz

## <a name="managing-online-risk"></a>Çevrimiçi riski yönetme

Müşteri ilişkilerinizin yaşam döngülerinde çevrimiçi işlem risklerinin pozlamasını azaltmak üzere ilke ve uygulamalar geliştirmenize yardımcı olması için aşağıdaki önerileri kullanabilirsiniz.

### <a name="onboarding-new-customers"></a>Yeni müşterileri ekleme

Yeni müşterileri ekleme sırasında çevrimiçi riskleri azaltmaya yönelik öneriler şunlardır:

- Mümkün olduğunda müşterilerle kişisel ilişkiler oluşturun (örneğin, müşterilere telefonla iletişim kurun).
- Daha iyi Yöntemler (kredi ofisleri veya iş ticari rapor kuruluşlarını kullanma gibi) sayesinde müşterilerin kimlik bilgilerini ve arka planını doğrulayın.
- Robot hesap oluşturma ve satın alma işlemlerini en aza indirmek için kaydolma sırasında Multi-Factor Authentication (SMS doğrulaması gibi) kullanın.
- Hizmetleri (dijital kimlik hizmetleri gibi) kullanarak kimlikleri yönetin ve izleyin.
- Yoğun kredi kartı sahtekarlık algılama sistemleriyle müşterinin mali gücünü değerlendirin.
- Açık koleksiyonlar ilkesi oluşturun. Koleksiyonlar işleminizi ayrıntılandırın ve aboneliklerde erişim ne zaman ödemesiz olarak etkilenecektir. (Ödeme dışı [bir müşterinin aboneliğini](create-a-new-subscription.md#suspend-a-subscription) devre dışı bırakabilir veya askıya alabilirsiniz.)

### <a name="managing-customer-accounts"></a>Müşteri hesaplarını yönetme

Müşteri hesaplarını yönetme önerileri satın alma sonrası şunları içerir:

- Microsoft bildirimlerini hızlıca alma, gözden geçirme, işlem yapması ve yanıt vermeye yönelik bir işlem uygulayın.
- Ayarlar uygun izleme eşiklerini yaparken, bulut kullanımı iş ihtiyaçlarını anlamak için müşterilerle birlikte çalışın. (Örneğin, Iş Ortağı Merkezi 'nde [aylık bir Azure harcama bütçesi ayarlayabilirsiniz](set-an-azure-spending-budget-for-your-customers.md) . Bu anlama, ay içinde müşteri kullanımını izlemenizi ve müşteriler bütçesine yakın olduğunda bildirim gönderilmesini sağlar.)
- Dolandırıcılığın erken algılanmasına yardımcı olmak için [Müşteri etkinlik günlüklerini](activity-logs.md) düzenli olarak izleyin.
- Şüpheli etkinlikler algılandığında hızlı bir işlem yapın.
- Müşterilerin, risk azaltma denetimlerini uygulamadan aboneliğe tam yönetim erişimi vermekten kaçının.

### <a name="managing-customer-billing"></a>Müşteri faturalandırmasını yönetme

Müşteri faturalandırma sonrası satın alma için öneriler şunları içerir:

- İlk işlem ve faturalandırma öncesinde ön ödeme isteği.
- Yüksek riskli ödeme gereçleri (ön ödemeli kartlar veya depolanan değer kartları gibi) kabul etmeyin.
- Müşteri ödemelerini ve yaşlandırma hesaplarının alacakları izleyin. Geç ödemeler veya ödeme yapılmadığı için standartlaştırılmış hatırlatarak süreçlerini zorlayacağı.

Çevrimiçi riski azaltmaya yönelik daha ayrıntılı stratejiler için [çevrimiçi işlem risk yönetimi kılavuzuna bakın.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)
