---
title: Gelen fırsatları yönlendirme kuralları oluşturma ve yönetme
ms.topic: article
ms.date: 08/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Şirketiniz, Microsoft satıcılarından gelen bir ortak satış fırsatının nasıl yönlendirildiğini belirlemek için kurallar oluşturabilir.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: efb76953b05bfb10a18657155349e267ee84f456
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961475"
---
# <a name="create-and-manage-inbound-opportunities-routing-rules"></a>Gelen fırsatları yönlendirme kuralları oluşturma ve yönetme

**Uygun roller**: başvuru Yöneticisi | Başvuru kullanıcısı

> [!IMPORTANT]
> **Yönlendirme kuralları oluşturma isteğe bağlıdır**. Yalnızca dünyanın dört bir yanındaki büyük şirketler için önerilir veya şirketinizin, başvuru yönetiminin müşteri pazarlarına ve çözümlerine bağlı olarak belirli bir konum düzeyinde yapılması gereken karmaşık bir MPN hiyerarşisi varsa.

## <a name="introduction"></a>Giriş

Bu belgede açıklanan işlevsellik, şirketinizin kuralları yapılandırmasına yardımcı olur. Bu, Microsoft satıcıları tarafından gönderilen ortak satış fırsatlarını tercih ettiğiniz MPN konumlarına yönlendirmenize yardımcı olabilir. Varsayılan olarak, Microsoft satıcı başvuruları, fırsatta birlikte bulunan ortak satış çözümüyle ilişkili MPN konumuna gönderilir. Oluşturulduysa yönlendirme kuralları, şirketinizin varsayılan yönlendirmeyi geçersiz kılmasına yardımcı olur. Yalnızca tüm kuruluş kapsamına sahip [**başvuru Yöneticisi**](permissions-overview.md#manage-referrals) yönlendirme kuralları oluşturabilir ve düzenleyebilir. [**Başvuru Kullanıcı**](permissions-overview.md#manage-referrals) rolüne sahip iş ortakları, yalnızca başvuruların şirket içinde nasıl yönlendirildiğini anlamak için yönlendirme kurallarını görüntüleyebilir.

Kurallar, geriye dönük olarak uygulanmaz. Geçmişte veya daha eski bir yönlendirme kuralı yapılandırması ile oluşturulan tüm başvurular güncellenmez. Kurallarda yapılan tüm değişiklikler uygulanabilir anında.

Her kural için üç ana Özet vardır.

- **Müşteri marketi** -müşteri şirketinin bulunduğu Pazar

- **Çözüm** -şirketiniz tarafından, OCP GTM portalı veya ticari Market aracılığıyla yayınlanan çözümler

- **MPN konumu** -başvurunun yönlendirileceği MPN konumu

Her kural, **şirketimdeki çözümle Microsoft satıcıları tarafından gönderilen başvurular için bu şekilde okunabilir, bu MPN konumuna yönlendirin**

> [!Note]
> Gelen yönlendirme kuralları yalnızca Microsoft satıcıları tarafından şirketiniz tarafından gönderilen ortak satış fırsatları için geçerlidir.

## <a name="navigation"></a>Gezinti

**Hesap ayarları** sayfasında, **referanslar** sekmesinde yönlendirme kuralları oluşturabilirsiniz. Sayfaya gitmek için sağ üst köşedeki Kullanıcı simgesinin yanındaki Ayarlar simgesini seçin ve ardından sol gezinti panelinde **Başvurular** sekmesini seçin.

## <a name="initial-setup"></a>İlk kurulum

**Yönlendirme kurallarını yapılandırma zorunlu değildir**. Şirketiniz yönlendirme mantığının avantajlarından yararlanmak için yönlendirme kurallarını kullanmaya karar verirse, başvuru yönetimi sisteminin, başvuruları yönlendirmek için kullandığı varsayılan kuralları içeri aktararak başlayabilirsiniz. Geçerli mantık, müşteri ülkesinden bağımsız olarak Microsoft satıcılarından gelen tüm başvuruları yönlendirmek için Çözümle ilişkili MPN KIMLIĞINI kullanır. Bunlar, başvurağınız için kullanılabilir ve yönlendirme kuralları olarak **bir tıklama ile içeri aktarılabilir** . İçeri aktarma eylemi tamamlandıktan sonra, kurallar Microsoft satıcıları tarafından gönderilen tüm yeni başvurular için uygulanır. Şirketiniz mevcut kuralları düzenleyebilir, silebilir ve gerekirse yeni kurallar oluşturabilir. Kuralları yalnızca genel kapsama sahip olan [**başvuru Yöneticisi**](permissions-overview.md#manage-referrals) alabilir. Yönlendirme kurallarında sonraki değişiklikler için aynı izin gerekir.

> [!IMPORTANT]
> **E-posta bildirim mantığındaki değişiklikler vardır**. Kurallar içeri aktarıldıkları anda, ticari Market 'teki ortak satış sekmesinde karşıya yüklenen **çözüm kişilerine** daha önce gönderilen e-postalar artık gönderilmez. Yalnızca ortak satış fırsatının gönderildiği MPN konumunun **[başvuru yöneticileri](permissions-overview.md#manage-referrals)** bilgilendirilir.

## <a name="override-rules"></a>Geçersiz kılma kuralları

İki kural türünü geçersiz kılabilir ve varsayılan kuralın belirli bir koşulunu geçersiz kılabilirsiniz. Varsayılan kuralda, yalnızca başvuruların yönlendirileceği MPN konumunu değiştirebilirsiniz. Geçersiz kılabileceğiniz diğer iki kural türü, kurallarda koşullar olarak **Tüm çözümlere** ve **Tüm pazarlara** sahip olanlardır.

**Tüm pazarlar geçersiz kılma** -bir kural oluşturduğunuzu, tüm müşteri pazarları ve belirli bir çözüm a için, başvuruları MPN konumuna yönlendirdiğini kabul ediyor. Bu kuralı belirli bir Pazar ve aynı çözüm birleşimi ile geçersiz kılabilirsiniz. Örnek geçersiz kılma "Pazar Birleşik Krallık ve çözüm A 'dan müşterileri içeren başvurular için, bunu MPN location m2 'e yönlendirebilir.

**Tüm çözümler geçersiz kılınsın** , tüm çözümler ve belirli BIR Pazar MKT1 için, başvuruları MPN konumuna yönlendirdiğini belirten bir kural oluşturduğunuzu kabul edersiniz. Bu kuralı belirli bir çözümle ve aynı Pazar birleşimine sahip olacak şekilde geçersiz kılabilirsiniz. Örnek geçersiz kılma "Pazar MKT1 ve çözüm B 'den müşterileri içeren başvurular için, bunu MPN location m2 'e yönlendirin.

Aşağıdaki tabloda, geçersiz kılabileceğiniz çözüm türlerinin özeti gösterilmektedir

| **Tür** | **Geçersiz kılabilir misiniz?** |
|-------|-------|
|Varsayılan| No |
|Tüm pazarlar| Yes|
|Tüm çözümler| Yes|
|Belirli bir çözüm (ler) ve belirli Pazar (ler) kombinasyonu| No|

> [!Note]
> Bu kuralda başka herhangi bir şeyi değiştiremeseniz de, varsayılan kural için MPN konumunu değiştirebilirsiniz.

## <a name="rules-evaluation"></a>Kural değerlendirmesi

Şirketiniz bir senaryo için uygulanabilecek birden çok kurala sahipse, değerlendirme ölçütlerinin altında kullanılır.

- İlk denetim, gelen fırsatta belirtilen çözüm ve Pazar birleşimine sahip bir kural için olacaktır. Bu tür bir kuralla doğrudan eşleşme, diğer tüm kurallara göre önceliklidir.
- İlk denetim başarısız olursa, piyasa koşulunun tüm pazarlar olarak ayarlandığı başvuruda bahsedilen çözümü içeren kuralların olup olmadığını kontrol ediyoruz.
- İkinci denetim başarısız olursa, tüm çözümlerin belirli bir pazar için çözüm ölçütü olarak bahsedilen kurallar olup olmadığını kontrol ediyoruz.
- Üçüncü denetim de başarısız olursa, varsayılan kuralı kullanırız.

> [!Note]
> Belirli bir konum ve çözüm düzeyindeki diğer kurallarla çakışan bir kural oluşturamazsınız. Kullanıcı arabirimi, çakışan bir kural oluşturmaya çalıştığınızda, yapılandırmanızla çakışan kuralın adıyla bir hata oluşturur.

## <a name="example"></a>Örnek

Gelen yönlendirme kuralları, contoso Corporation için oluşturulan yönlendirme kurallarının yardımıyla açıklanacaktır. Kuralların nasıl uygulanacağını anlamadan önce, contoso Corporation 'da MPN hiyerarşisini ve Kullanıcı kurulumunu anmıza izin verin.

#### <a name="mpn-hierarchy-of-contoso-corporation"></a>Contoso Corporation 'ın MPN hiyerarşisi

| **MPN Kimliği** | **Tür** | **Adres** |
|-------|-------|-------|
|999999| Genel| Tek contoso Way, **Redmond, Birleşik Devletler Amerika**|
|555555| Konum| Tek contoso Way, **Londra, Birleşik Krallık**|
|666666| Konum| Tek contoso yöntemi, **Singapur, Singapur**|
|777777| Konum| Tek contoso Way, **Bengaluru, Hindistan**|

#### <a name="sellers-from-contoso-corporation"></a>Contoso Corporation şirketinin satıcıları

Contoso Corporation 'ın ilgili referans rollerinin ve kapsamındaki satıcılar aşağıda verilmiştir.

| **Ad** | **Role** | **Kapsam** |
|-------|-------|-------|
|Satıcı bir|Başvuru Yöneticisi|Kuruluşun tamamı|
|Ikinci satıcı|Başvuru Yöneticisi|Bengaluru|
|Üçüncü satıcı|Başvuru kullanıcısı|Londra|
|Dördüncü Satıcı|Referans kullanıcısı|Singapur|

#### <a name="inbound-routing-rules-for-contoso-corporation"></a>Contoso Corporation için gelen yönlendirme kuralları

Contoso Corporation için Satıcı 1 tarafından aşağıdaki kural kümesi oluşturulmuş olduğunu varsayalım. Kuralları **oluşturmak ve** düzenlemek için tüm kuruluş kapsamında referans [yöneticisi](permissions-overview.md#manage-referrals) gerektiğinden bu kuralları yalnızca Satıcı Kişisi oluşturabilir.

| **Piyasa** | **Çözümler** | **MPN konumu** | **Yönlendirme kuralı adı** |
|-------|-------|-------|-------|
|Tüm pazarlar|Tüm çözümler|Redmond|Varsayılan|
|Birleşik Krallık|Tüm çözümler|Londra|Birleşik Krallık tüm çözümleri|
|Tüm pazarlar|Sol-ABC|Singapur|Sol-ABC tüm pazarlar|
|Hindistan|Sol-PQR|Bengaluru|Hindistan-Sol-PQR|

#### <a name="summary-of-routing-for-various-scenarios-based-on-the-rules-for-contoso-corporation"></a>Contoso Corporation kurallarına göre çeşitli senaryolar için yönlendirme özeti

| **Hayır** | **Senaryo** | **Müşteri Pazarı** | **Dahil edilen çözümler** |**Yönlendirme kuralı uygulandı** |**MPN ataması** |**Referans erişimi** |
|-----|----------|-------|-------|-------|-------|-----------|
| 1|Belirli bir çözüm ve pazar kuralı eşleşmesi yok|Birleşik Krallık|SOL-PQR|Genel|999999| Seller One, Seller Two, Seller Three (takıma eklenmişse), Seller Four (takıma eklenmişse)|
| 2|Tüm çözümler ve belirli bir pazar kuralı eşleşmesi|Birleşik Krallık|SOL-PQR|Birleşik Krallık tüm çözümleri|555555| Seller One, Seller Three (takıma eklenmişse) |
| 3|Belirli bir çözüm ve tüm pazarlar kural eşleşmesi|Nijerya|SOL-ABC|SOL-ABC tüm pazarlar|666666| Seller One, Seller Four (takıma eklenmişse) |
| 4|Belirli bir çözüm ve pazar kuralı eşleşmesi|Hindistan|SOL-PQR|Hindistan-Sol-PQR|777777| Satıcı Bir, Satıcı İki|
| 5|Şirket sahibi olmadığınız bir çözümle gelen referans|Birleşik Devletler Amerika|SOL-XYZ|Genel|999999| Seller One, Seller Two, Seller Three (takıma eklenmişse), Seller Four (takıma eklenmişse)|

## <a name="next-steps"></a>Sonraki adımlar

- [Ortak Satış Fırsatlarını Yönetme](manage-co-sell-opportunities.md)

- [Dynamics 365 CRM için ortak satış bağlayıcısı alın](connector-dynamics.md)

- [Salesforce CRM için ortak satış bağlayıcısı alın](connector-salesforce.md)
