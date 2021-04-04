---
title: Teşviklerle ilgili müşteri ilişkilendirme sorunları
description: Talep edilen kayıt ortağı (CPOR) müşteri ilişkilendirmeleriyle çalışırken ortaya çıkan sorunları nasıl ele alabileceğinizi öğrenin.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.date: 09/11/2020
ms.openlocfilehash: 30639725c0a852046251e83c3791f56d788931c1
ms.sourcegitcommit: 6498c57e75aa097861523b206dc142f789deeb36
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "106179232"
---
# <a name="issues-with-claimed-partner-of-record-cpor-customer-associations"></a>Talep edilen kayıt Iş ortağı (CPOR) müşteri ilişkilendirmeleri ile ilgili sorunlar

**Uygun roller**

- Faturalama yöneticisi
- Genel yönetici
- Teşvikleri Yöneticisi

Aşağıdaki içerik, müşteri ilişkilendirmeleriyle çalışırken gelebileceğiniz sorunları çözmenize yardımcı olur.

## <a name="domain-tenant-mismatch"></a>Etki alanı kiracı uyumsuzluğu

Istenen kayıt Iş ortağı (CPOR) ilişki talep akışı içinde, müşteri kiracı KIMLIĞI ve alt etki alanı sağlamanız istenecektir. Bunların eşleşmediğini belirten bir hata alırsanız, doğru ayrıntılara sahip olduğunuzdan emin olmak için müşteri ile iletişim kurun.

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a>CPOR ilişkilendirme talep akışındaki abonelik hataları

CPOR ilişkilendirme talep akışında, Business Applications (Dynamics 365) aracılığıyla talep kurmaya çalıştığınız bir ürün için abonelik sağlamanız istenebilir. Ürünün ve aboneliğin, için talep edilen kiracıya ait olduğunu dinamik olarak denetliyoruz, aboneliği soruyoruz. Ayrıca aboneliğin etkin/yetkisiz kullanım durumunda olduğunu denetliyoruz.

Hatayı alırsanız bunun çeşitli nedenleri olabilir:

- Seçilen ürün müşterinin kiracısında mevcut değildir
- Dynamics için belirtilen abonelik
- Sağlanan abonelik CSP içindir
- Müşteri henüz bu abonelik için ürünleri etkinleştirmedi/sağladı
- Abonelik zaten alınmıştır
- Girilen tanımlayıcı bir abonelik KIMLIĞI değil

Aboneliğinizin doğruluğu hakkında sorularınız varsa, aboneliğin doğru olduğundan ve doğru kiracı KIMLIĞINI kullandığınızdan emin olmak için müşterunuzla birlikte çalışın.

Bu yol sorununuzu çözümlemezse [desteğe](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)başvurun.

## <a name="when-subscriptions-will-be-available-to-claim"></a>Abonelikler talep için kullanılabilir olacaktır

Abonelik için işlem gerçekleştirirken abonelik henüz sağlanmadıysa bir hata alırsınız. Aboneliğin, abonelik veya platformun bu uygulamayı seçmesini ve talep etmek için kullanılabilir hale gelmesi için yapması gereken birkaç adım vardır. Abonelik talep edilmeye çalışılırken bir hata alıyorsanız, sağlanmış olduğundan ve istediğiniz aboneliğin doğru olduğundan emin olmak için müşteri ile iletişim kurun. Bu yolu zaten aldıysanız, [desteğe](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)başvurun.

## <a name="which-activity-do-i-choose"></a>Hangi etkinliği seçeceğim?

CPOR istek çözümü platformu, Business Applications ve Microsoft 365 çözüm alanlarıyla ilgili CPOR ilişki taleplerine izin verir. Her çözüm alanı için geçerli olan etkinlikler aşağıda verilmiştir. Gelecekte geri kazanmak zorunda kalmamak için açıklamalara göre doğru etkinliği seçin. Yanlış bir etkinlikle Sonuçlama, eksik uygunluk ve bir kazanç elde edilmesine yol açabilir.


| Çözüm alanı | Etkinlik | İçin geçerlidir |
| ------ | ----------- | ----------- |
| İş uygulamaları      | Satış öncesi   | Uygun bir ürünün satın almasını etkileyenler ve satış öncesi teşvikleri için uygulama kullanmak istiyorsanız seçin. Bu seçenek yalnızca müşteri bu ürünleri toplu lisanslama sözleşmesi veya Web-Direct aracılığıyla satın aldıysa geçerlidir. |
|    |  Kullanım  | Uygun bir iş yükünün benimseme ve kullanımını ve kullanım teşvikleri için uygulamak istediğinizi seçin. Bu seçenek yalnızca müşteri bu ürünleri toplu lisanslama sözleşmesi veya Web-Direct aracılığıyla satın aldıysa geçerlidir. |
|    | Gelir ilişkisi   | Uygun bir ürünün seçimini bir Iş etkileyen olarak etkileyenler ' i seçin. Bu seçenek yalnızca gelir ilişkilendirmesi amaçlıdır, bu ödemeleri teşvik etmek için değildir. Bu seçenek yalnızca müşteri bu ürünleri toplu lisanslama sözleşmesi veya Web-Direct aracılığıyla satın aldıysa geçerlidir.   |
| Microsoft 365   | Kullanım   | Uygun bir iş yükünün benimseme ve kullanımını ve kullanım teşvikleri için uygulamak istediğinizi seçin. |

## <a name="which-mpn-do-i-choose"></a>Hangi MPN 'yi seçeceğim?

CPOR ilişkilendirme talep akışında, son Müşterideki için yaptığınız iş ile ilişkilendirilmesi gereken bir şirket MPN seçmeniz istenir. Şirketiniz, bir kısmı bir veya daha fazla bilgisayar ve FRP FastTrack gibi bir iş ortağı türüyle ilişkili birçok MPNs olabilir. CPOR ilişkilendirme talep akışı, bir bir bir bir bir bir bir bir bir bir iş ortağı türü olarak hangi MPNs 'nin kaydedildiğini belirler, ancak belirli bir iş ortağı türü olan MPN olduğunu söylemez. İleride geri kazanmak zorunda kalmamak için doğru MPN 'yi seçmeniz önemlidir. Yanlış MPN ile Sonuçlama, eksik uygunluk ve teşvik kazanmına yol açabilir.

Hangi MPN kullanacağınızı görmüyorsanız, genel yöneticinizle iletişime geçin.

Kullanmak istediğiniz MPN, kayıtlı değilse, [teşvikleri Genel Bakış sekmesinde](https://partner.microsoft.com/dashboard/incentives/enrollment/summary) (oturum açma gerekir) bunu yönetebilirsiniz.

## <a name="choosing-a-product-vs-entering-a-subscription"></a>Bir ürün seçme ve abonelik girme

Bir Dynamics ürün talep edildiğinde ve onaylandığında, iş ortağı, abonelik KIMLIĞINI CPOR ilişkilendirme talebi içinde görüntüleyebilir. Bu abonelik talep edildiğinde, etkin veya yetkisiz kullanım durumunda olur, ancak aboneliğin bittiği bir zaman olabilir ve yeni aboneliklerin ayrı bir CPOR ilişkilendirme talebinde talep edilmesine gerek olacaktır.

## <a name="competing-claims"></a>Rekabet talepleri

Zaten başka bir iş ortağıyla ilişkili olan bir müşteri ve ürünleri için bir CPOR ilişki talebi oluşturuyorsanız, talep yönetimi şu şekilde olur:

1. Yeni müşteri ilişkilendirmesini oluşturduktan sonra Microsoft doğruluğundan emin olmak için sağladığınız ilişkilendirmenin ve yürütme kanıtının ayrıntılarını doğrular.

2. Siz ve başka bir iş ortağı aynı müşteri ve ürün/iş yükünü talep ederseniz, Microsoft hangi ortağın onaylanacağını öğrenmek için her ortağın yürütme belgelerini gözden geçirir.

3. Her iki iş ortağının da ek bilgiler istenebilir ve bu da ilişkilendirme isteğinizi işlerken gecikmelere neden olabilir.

4. Bu süre, daha uzun bir süre boyunca _Gözden geçirme altında_ kalabilse de, cpor ilişki talepiniz beş iş günü içinde incelenmeye devam edecektir. Bu senaryo, Microsoft şu anda ürüne/iş yüküne sahip olan iş ortağıyla birlikte çalışıyorsa meydana gelebilir. Bu durumda, talebin açıklamalar bölümünde bildirim alırsınız. 

>[!IMPORTANT]
>CPVEYA ilişkilendirme yürütmesinin (PoE) doğrulanması için ek bilgilere ihtiyaç duyuyorsanız, CPOR ilişkilendirme talep açıklamaları bölümü aracılığıyla sizinle iletişim kuracağız.

## <a name="next-steps"></a>Sonraki adımlar

- [Teşviklerle çalışmaya başlama](incentives-get-started-intro.md)
