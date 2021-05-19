---
title: Ödeme zamanlamaları ve süreçleri
description: Ticari market ve diğer işlemler için ödeme zamanlamaları ve yeniden ödeme işlemleri gibi ödemeler ve işlemler hakkında bilgi alın.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 12/04/2020
ms.openlocfilehash: f2ba8132677eb0a0368021b6d7065f5202589f24
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146961"
---
# <a name="payout-schedules-and-processes"></a>Ödeme zamanlamaları ve süreçleri

**Uygun roller:** Hesap yöneticisi | Genel yönetici

Bu makalede Microsoft'un ödeme zamanlaması, ödemenin durumu nerede bulunacak ve ödemesi olmayan müşterinin işlemi ele alır.

## <a name="payment-schedules"></a>Ödeme zamanlamaları

Aşağıdaki bölümlerde, kredi **kartı/fatura** işlemleri için **Kurumsal Anlaşma** işlemlerimiz açıklanmaktadır.

### <a name="enterprise-agreement-transactions"></a>Kurumsal Anlaşma işlemleri

Müşteri mevcut Microsoft Kurumsal Anlaşma'sini kullanarak Microsoft AppSource veya Azure Market ürün satın aldı mı, sonraki ödeme döngüsünde ödemeleri 30 günlük müşteri faturasından sonra biz öderiz. Müşterinin kredi kartı kullandığı işlemlerin ödemeden önce 30 günlük tutma süresi vardır.

Ödeme genellikle Microsoft müşteriden ödeme toplamadan önce gerçekleşir. Müşterinin [Microsoft'a ödemesi başarısız](#process-for-customer-non-payment) olduğunda ancak ödemesi zaten yapılan işlemler için aşağıdaki Müşterinin ödemesi olmayan ödeme işlemi'ne bakın.

| Olay | Description | Raporlama Görünürlüğü | Zamanlama* |
| --- | --- | --- | --- |
| Kullanım veya işlem ayı | Müşteri bir hizmet kullanır veya satın alır. | [Kullanım](/azure/marketplace/partner-center-portal/usage-dashboard) veya [Sipariş](/azure/marketplace/partner-center-portal/orders-dashboard) Panosu | **1. Ay** |
| Microsoft faturalama tutarını hesaplar | Toplam kullanımı, toplam işlemleri belirleme | [Kullanım](/azure/marketplace/partner-center-portal/usage-dashboard) veya [Sipariş](/azure/marketplace/partner-center-portal/orders-dashboard) Panosu | **2. Ay** |
| Ödeme gönderildi | Ajantı ücretini ve ödeme kazançlarını belirleme | [Ödeme bildiriminde](payout-statement.md) Işlem geçmişinde işlenmemiş olarak işaretlendi | **Ay 3 (1 hafta)** |
| Ödeme hazırlığı | Kazançlar aylık ödeme için hazırlandı | [Ödeme bildiriminde](payout-statement.md) Işlem geçmişinde yakında çıkacak şekilde işaretlendi | **Ay 3 (1 hafta)** |
| **Ödeme gönderildi** | **Ödeme, yayımcıya gönderilir** | **Işlem geçmişinde ve ödeme [bildiriminin](payout-statement.md) ödemeler bölümünde gönderildi olarak işaretlendi** | **3. ay (15 ' ten sonra değil)** |
| Müşteriye göre ödenen fatura | Microsoft müşteriden ödeme toplar | düzeltme sınıfı, | **Ay 4 ila 12** |
|

\* Ödeme tarihi Pasifik standart saatine (PST) göre yapılır.

:::image type="content" source="images/payouts/timeline-enterprise.png" alt-text="Kurumsal Anlaşma müşterileri için ödemelerin zaman çizelgesi.":::

### <a name="transactions-with-credit-card-or-invoice-checkwire"></a>Kredi kartı veya fatura ile işlemler (Çek/tel)

Kredi kartına veya aylık faturaya sahip tüm satın alımlarda, müşteri üzerinden fon toplandığından emin olmak için 30 günlük bir bekleme süresi bulunur.

| Olay | Description | Raporlama görünürlüğü | Zamanlama* |
| --- | --- | --- | --- |
| Kullanım veya işlem ayı | Müşteri bir hizmet kullanır veya satın alır. | [Kullanım](/azure/marketplace/partner-center-portal/usage-dashboard) veya [Sipariş](/azure/marketplace/partner-center-portal/orders-dashboard) Panosu | **1. Ay** |
| Müşteri tarafından ödenen fatura | Toplam kullanımı, toplam işlem değerini ve müşteri ödeme faturasını belirleme | [Kullanım](/azure/marketplace/partner-center-portal/usage-dashboard) veya [Sipariş](/azure/marketplace/partner-center-portal/orders-dashboard) Panosu | **2. Ay** |
| Ödeme gönderildi | Ajans ücretini ve ödeme kazançlarını belirleme | Ödeme deyiminde İşlem Geçmişinde İşlenmemiş [olarak işaretlendi](payout-statement.md) | **2. Ay** |
| 30 günlük tutma süresi | Fon toplama, olası geri ödeme ve para iadesi isteklerinin top olduğundan emin olmak | Ödeme deyiminde İşlem Geçmişinde İşlenmemiş [olarak işaretlendi](payout-statement.md) | **3. Ay** |
| Ödemeyi hazırlama | Kazançlar aylık ödeme için hazırlanır | Ödeme hesap hesaplarında İşlem Geçmişi'ne Gelecek [olarak işaretlendi](payout-statement.md) | **Ay 4 (1 hafta)** |
| **Ödeme gönderildi** | **Ödeme, yayımcıya gönderilir** | **Işlem geçmişinde ve ödeme [bildiriminin](payout-statement.md) ödemeler bölümünde gönderildi olarak işaretlendi** | **4. ay (15. günden sonra değil)** |
|

\* Ödeme tarihi, Pasifik Standart Saati (PST) olarak belirlenir.

:::image type="content" source="images/payouts/timeline-credit-card-invoice.png" alt-text="Kredi kartı ve fatura müşterileri için ödemelerin zaman çizelgesi.":::

## <a name="process-for-customer-non-payment"></a>Müşteri ödemesiz işlem

Nadir durumlarda Microsoft, ticari Market satın alımları için müşterilerden ödeme toplayamamaktadır. Bir müşteri Microsoft 'un faturalandırma zamanlamalarına göre ödeme yapamazsa koleksiyonlar işlemine başlayacağız. Bu işlem yaklaşık dört ay sürer ve Microsoft 'tan kalıcı iletişim içerir. Ödeme bu işlemin sonuna kadar alınmadıysa, Microsoft fonları toplanabilir olmayan bir tablo olarak yazar.

Bu işlem için, Microsoft, bu işlemin sonunda, son olarak toplanabilir bir tablo olan yayımcılar 'a (siz) zaten ücret ödemüş olabilir. Bu nedenle, bu miktarları mutabık kılma sürecimiz vardır. (Zaten alınmış) ödemenin uzlaştırılabileceğini belirten bir uyarı olduğundan emin olmak için, bir müşteri koleksiyonlar sürecinde olduğunda ve satın alımlarınızın kapalı olma olasılığı varsa size bildirilir.

Microsoft, aşağıdaki yöntemlerden birini kullanarak zaten ücretli olan tüm ödemeler için ödeme yapacaktır: (1) Microsoft, ödenmemiş miktarları gelecekteki ödemeler üzerinden çıkartabilir; Örneğin, ödemelerden $1.000, toplanmamış tablo olarak kabul edilir ve bu durum devre dışı bırakılırsa, gelecekteki ödemelerden bazıları $1.000 kurtarılana veya (2) Microsoft, toplanan herhangi bir miktar için bir para iadesi veya fatura yayımcıları isteyebileceği için,

Aşağıdaki zamanlama bir örnektir:

| Olay | Yaklaşık Tarih * | İş ortağı görünürlüğü |
| --- | --- | --- |
| Örnek ödeme tarihi | 10/15/2020 | İşlem **Geçmişinde** ve Ödeme Panosu'nın Ödemeler bölümünde Gönderildi olarak işaretlendi |
| <font color="red">Müşteri Microsoft'a ödemezse</font> | 12/2/2020 – 12/5/2020 | Yukarıdakiyle aynı şekilde değişiklik yok |
| Müşteri ilk geç ödeme e-postası alır | 12/6/2020 | Hiçbiri |
| Müşteri artan aciliyet e-postalarını alıyor | 12/7/2020 – 1/31/2021 | Hiçbiri |
| Yayımcıya büyük olasılıkla kapalı yazma bildirildi | 1/7/2021 | Yayımcıya, müşterilerinin henüz ödeme göndermemiş olduğu e-posta bildirimi gönderilir. İşlem kimliği ve dolar tutarı dahil edilir. |
| Müşteri sonlandırma bildirimi alır | 2/1/2021 | Hiçbiri |
| Toplama işlemi sona erer / fonlar yazılır | 2/15/2021 | Fonlar yazılıp yayımcıya gönderilen e-posta bildirimi. İşlem kimliği ve dolar tutarı dahil edilir. |
| Ödeme düşüldüğü | 01.03.2021 | Yayımcı, Iş Ortağı Merkezi ödeme bildiriminde negatif işlem görür |
| Ödeme stopaj uygulanan | 3/15/2021 | Gelecekteki ödemeler, Iş Ortağı Merkezi ödeme bildiriminde gösterilir. Bu, bakiye artık negatif olmadığından, ödeme ödemeyi almaz.  |
|||

\* Ödeme tarihi, Pasifik Standart Saati (PST) olarak belirlenir.

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Ödemelerin bir ödeme hesabına ulaşması için geçen gün sayısı

Genellikle söz konusu ayın 15. gününde belirli bir ay boyunca herhangi bir ödeme gönderiyoruz, ancak ödemenin hesabınıza ulaşması için başka bir zaman alır. Gün sayısı, aşağıda açıklandığı gibi, hesabınız için kullandığımız ödeme yöntemine bağlıdır.

> [!NOTE]
> Aşağıda gösterilen günler yaklaşık değerlerdir; herhangi bir ödemenin hesabınıza ulaşması daha fazla veya daha az zaman alabilir.

| Ödeme yöntemi     | Ödeme hesabına ulaşma gün sayısı     |
|--------------------|--------------------------------------------|
| PayPal             | 1 iş günü                             |
| ACH/SEPA           | 2-3 iş günü                          |
| Tel aktarım      | 7-10 iş günü                         |
|

## <a name="next-steps"></a>Sonraki adımlar

- [Vergi ayrıntıları](tax-details-marketplace.md)
