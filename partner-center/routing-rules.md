---
title: Gelen fırsat yönlendirme kuralları oluşturma ve yönetme
ms.topic: article
ms.date: 08/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft satıcılarından gelen ortak satış fırsatlarının nasıl yönlendirildiklerine karar vermek için, şirketiniz kurallar oluşturabilir.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: efb76953b05bfb10a18657155349e267ee84f456
ms.sourcegitcommit: 42238e2ce36725631f542887c9112593d701ca9c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/20/2021
ms.locfileid: "122621709"
---
# <a name="create-and-manage-inbound-opportunities-routing-rules"></a>Gelen fırsat yönlendirme kuralları oluşturma ve yönetme

**Uygun roller:** Referans yöneticisi | Referans kullanıcısı

> [!IMPORTANT]
> **Yönlendirme kuralları oluşturmak isteğe bağlıdır.** Yalnızca dünyanın farklı yerlerinden varlığı olan daha büyük şirketler için veya referans yönetiminin müşteri pazarlarına ve çözümlerine göre belirli bir konum düzeyinde gerçekleştirilecek karmaşık bir MPN hiyerarşisi olması önerilir.

## <a name="introduction"></a>Giriş

Bu belgede açıklanan işlevsellik, microsoft satıcılarının gönderdiği Ortak satış fırsatlarını istediğiniz MPN konumlarına yönlendirmeye yardımcı olan kuralların yapılandırılması konusunda şirketinize yardımcı olur. Varsayılan olarak, Microsoft satıcısının referansları fırsata dahil edilen Ortak satış çözümüyle ilişkili MPN konuma gönderilir. Oluşturulduktan sonra yönlendirme kuralları, şirketinizin varsayılan yönlendirmeyi geçersiz kılmıştır. Yönlendirme [**kurallarını yalnızca**](permissions-overview.md#manage-referrals) tüm kuruluş kapsamına sahip referans yöneticisi oluşturabilir ve düzenleyebilir. Referans kullanıcı [**rolüne**](permissions-overview.md#manage-referrals) sahip iş ortakları yalnızca referansların şirket içinde nasıl yönlendirildiklerini anlamak için yönlendirme kurallarını görüntülemeye devam ediyor.

Kurallar geçmişe dönük olarak uygulanmaz. Geçmişte veya yönlendirme kuralının daha eski bir yapılandırmasıyla oluşturulan referanslar güncelleştirilmez. Kurallarda yapılan tüm değişiklikler anında uygulanabilir.

Herhangi bir kural için üç ana özet vardır.

- **Müşteri pazarı** - Müşteri şirketinin bulunduğu pazar

- **Çözüm** - OCP GTM portalı veya ticari market aracılığıyla şirketiniz tarafından yayımlanan çözümler

- **MPN** konumu - Referansın yönlendiril olduğu MPN konumu

Her kural şu şekilde okunabilir: Şirketimin çözümlerini kullanarak Microsoft satıcılarının gönderdiği referanslar için bunları bu **MPN konuma yönlendirin**

> [!Note]
> Gelen yönlendirme kuralları yalnızca Microsoft satıcılarının şirketinize gönderdiği Ortak satış fırsatları için geçerlidir.

## <a name="navigation"></a>Gezinti

Yönlendirme kurallarını Hesap ayarları sayfasının **altındaki Referanslar** **sekmesinde oluşturabilirsiniz.** Sayfaya gitmek için sağ üst köşedeki kullanıcı simgesinin yanındaki ayarlar simgesini ve  ardından sol gezinti panelinde Referanslar sekmesini seçin.

## <a name="initial-setup"></a>İlk kurulum

**Yönlendirme kurallarının yapılandırılması zorunlu değildir.** Şirketiniz yönlendirme mantığının avantajını kullanmak için yönlendirme kurallarını kullanmaya karar veriyorsa, referans yönetim sisteminin referansları yönlendirmek için kullandığı varsayılan kuralları içeri aktararak başlayabilirsiniz. Geçerli mantık, müşteri ülkesi ne olursa olsun Microsoft satıcılarından gelen tüm referansları yönlendirmek için çözümle ilişkilendirilmiş MPN kimliğini kullanır. Bunlar başvuru için kullanılabilir ve **yönlendirme kuralları olarak tek tıklamayla** içe aktarabilirsiniz. İçeri aktarma eylemi tamamlandıktan sonra, Microsoft satıcılarının gönderdiği tüm yeni referanslar için kurallar uygulanır. Şirketiniz mevcut kuralları düzenleyebilir veya silebilir ve gerekirse yeni kurallar oluşturabilir. Kuralları [**yalnızca genel**](permissions-overview.md#manage-referrals) kapsamda referans yöneticisi içeri aktar olabilir. Yönlendirme kurallarında yapılan sonraki değişiklikler için de aynı izin gereklidir.

> [!IMPORTANT]
> **E-posta bildirim mantığında değişiklikler vardır.** Kurallar içe aktarılmaz, ticari marketteki Ortak satış  sekmesine yüklenen çözüm kişilerine daha önce gönderilen e-postalar artık gönderilmez. **Yalnızca [ortak satış](permissions-overview.md#manage-referrals)** fırsatının gönderildiği MPN konumunun referans yöneticilerine bildirilecek.

## <a name="override-rules"></a>Kuralları geçersiz kılma

İki tür kuralı geçersiz kılmıştır ve varsayılan kuralın belirli bir koşullarını geçersiz kılarak. Varsayılan kuralda, yalnızca referansların yönlendirilen MPN konumunu değiştirebilirsiniz. Geçersiz kılarak geçersiz kıly bildiğiniz diğer iki kural türü, Tüm çözümler **ve Kurallarda** koşullar **olarak** Tüm pazarlar olan türlerdir.

**Tüm pazarlar** geçersiz kılınıyor - Tüm müşteri pazarları ve belirli bir çözüm A için referansları MPN konumu M1'e yönlendiren bir kural oluşturduğunuz varsayarak. Belirli bir pazar ve aynı çözüm bileşimiyle bu tür bir kuralı geçersiz kılarak. Örnek geçersiz kılma , "Birleşik Krallık pazar ve çözüm A'dan müşteri içeren referanslar için, bunu MPN konumu M2'ye yönlendirin.

**Tüm çözümleri geçersiz** kılma - Tüm çözümler ve belirli bir pazar MKT1 için referansları MPN konumu M1'e yönlendiren bir kural oluşturduğunuz varsayarak. Belirli bir çözüm ve aynı pazar birleşimiyle bu tür bir kuralı geçersiz kılarak. Örnek geçersiz kılma , "market MKT1 ve çözüm B'den müşteri içeren referanslar için, bunu MPN konumu M2'ye yönlendirin.

Aşağıdaki tabloda geçersiz kılabilirsiniz çözüm türlerinin özeti gösterilmiştir

| **Tür** | **Geçersiz k musunuz?** |
|-------|-------|
|Varsayılan| No |
|Tüm pazarlar| Yes|
|Tüm çözümler| Yes|
|Belirli bir çözüm ve belirli pazarlar bileşimi| No|

> [!Note]
> Bu kuralda başka hiçbir şeyi değiştiremiyor olsa bile varsayılan kuralın MPN konumunu değiştirebilirsiniz.

## <a name="rules-evaluation"></a>Kural değerlendirmesi

Şirketinizin bir senaryo için uygulan uyan birden çok kuralı varsa, kullanılan değerlendirme ölçütlerinin altında.

- İlk denetim, belirli bir çözüm ve pazar bileşimine sahip olan ve gelen fırsatta olan bir kurala yöneliktir. Bu tür bir kuralla doğrudan eşleşme, diğer tüm kurallara göre önceliklidir.
- İlk denetim başarısız olursa, referansta belirtilen çözümü içeren ve tüm pazarlar olarak ayarlanmış pazar koşuluna sahip bir kural olup ola bir kural olup o değildir.
- İkinci denetim başarısız olursa, tüm çözümlerin belirli bir pazar için çözüm ölçütü olarak belirtildiği herhangi bir kural olup o zaman kontrol ederiz.
- Üçüncü denetim de başarısız olursa Varsayılan kuralı kullanıruz.

> [!Note]
> Belirli bir konum ve çözüm düzeyinde diğer kurallarla çakışan bir kural oluşturamazsiniz. Çakışan bir kural oluşturmayı denersiniz, kullanıcı arabirimi, yapılandırmanız ile çakışan kuralın adıyla bir hata verir.

## <a name="example"></a>Örnek

Gelen yönlendirme kuralları, Contoso Corporation için oluşturulan yönlendirme kuralları yardımıyla açıklanmıştır. Kuralların nasıl uygulanacaklarını anlamadan önce Contoso Corporation'da MPN hiyerarşisini ve kullanıcı ayarlamayı anlayın.

#### <a name="mpn-hierarchy-of-contoso-corporation"></a>Contoso Corporation'ın MPN hiyerarşisi

| **MPN Kimliği** | **Tür** | **Adres** |
|-------|-------|-------|
|999999| Genel| One Contoso way, **Redmond, Birleşik Devletler of America**|
|555555| Konum| One Contoso way, **Londra, Birleşik Krallık**|
|666666| Konum| Tek Contoso yolu, **Singapur, Singapur**|
|777777| Konum| Tek Contoso yolu, **Bengaluru, Hindistan**|

#### <a name="sellers-from-contoso-corporation"></a>Contoso Corporation'dan Satıcılar

Contoso Corporation'da ilgili referans rollerine ve kapsamına sahip satış satıcıları aşağıda verilmiştir.

| **Ad** | **Role** | **Kapsam** |
|-------|-------|-------|
|Satıcı Bir|Referans yöneticisi|Tüm Kuruluş|
|Satıcı İki|Referans yöneticisi|Bengaluru|
|Satıcı Üç|Referans kullanıcısı|Londra|
|Dördüncü Satıcı|Referans kullanıcısı|Singapur|

#### <a name="inbound-routing-rules-for-contoso-corporation"></a>Contoso Corporation için gelen yönlendirme kuralları

Contoso Corporation için Satıcı 1 tarafından aşağıdaki kural kümesi oluşturulmuş olduğunu varsayalım. Kuralları **oluşturmak ve** düzenlemek için tüm kuruluş kapsamında referans [yöneticisi](permissions-overview.md#manage-referrals) gerektiğinden bu kuralları yalnızca Satıcı Kişisi oluşturabilir.

| **Piyasa** | **Çözümler** | **MPN konumu** | **Yönlendirme kuralı adı** |
|-------|-------|-------|-------|
|Tüm pazarlar|Tüm çözümler|Redmond|Varsayılan|
|Birleşik Krallık|Tüm çözümler|Londra|Birleşik Krallık tüm çözümleri|
|Tüm pazarlar|Sol-ABC|Singapur|Sol-ABC tüm pazarlar|
|Hindistan|Sol-PQR|Bengaluru|Hindistan-Sol-PQR|

#### <a name="summary-of-routing-for-various-scenarios-based-on-the-rules-for-contoso-corporation"></a>Contoso Corporation kurallarına göre çeşitli senaryolar için yönlendirmenin özeti

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
