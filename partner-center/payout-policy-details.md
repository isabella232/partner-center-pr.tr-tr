---
title: Ödeme zamanlamaları ve süreçleri
description: Ödeme zamanlamaları ve diğer işlemler için ödeme zamanlamaları ve yeniden ödeme işlemleri gibi ödeme ve Azure Market hakkında bilgi öğrenin.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 05/25/2021
ms.openlocfilehash: 417421ad51c30d067ce3eb2189534a391b2951a2
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114845015"
---
# <a name="payout-schedules-and-processes"></a>Ödeme zamanlamaları ve süreçleri

**Uygun roller:** Hesap yöneticisi | Genel yönetici

Bu makalede Microsoft'un ödeme zamanlaması, ödemenin durumu nerede bulunacak ve ödemesi olmayan müşterinin işlemi ele alır.

## <a name="payment-schedules"></a>Ödeme zamanlamaları

Aşağıdaki bölümlerde, Kurumsal Anlaşma ve csP **işlemleri Microsoft Müşteri Sözleşmesi** **işlemleri için ödeme işlemimiz** açıklanmaktadır.

### <a name="transactions-when-customer-has-an-enterprise-agreement"></a>Müşterinin bir iş Kurumsal Anlaşma

Bir müşteri, mevcut Microsoft Microsoft AppSource'Azure Market işlemleri için Kurumsal Anlaşma ürün satın aldı mı, sonraki ödeme döngüsünde müşteri faturasından sonraki 30 gün içinde ödemeleri biz tutarız. Müşterinin kredi kartı kullandığı işlemlerin ödemeden önce 30 günlük tutma süresi vardır.

Ödeme genellikle Microsoft müşteriden ödeme toplamadan önce gerçekleşir. Müşterinin [Microsoft'a ödemesi başarısız](#process-for-customer-non-payment) olduğunda ancak ödemesi zaten yapılan işlemler için aşağıdaki Müşterinin ödemesi olmayan ödeme işlemi'ne bakın.

| Olay | Description | Raporlama Görünürlüğü | Zamanlama* |
| --- | --- | --- | --- |
| Kullanım veya işlem ayı | Müşteri bir hizmet kullanır veya satın alır. | [Kullanım](/azure/marketplace/partner-center-portal/usage-dashboard) veya [Sipariş](/azure/marketplace/partner-center-portal/orders-dashboard) Panosu | **1. Ay** |
| Microsoft faturalama tutarını hesaplar | Toplam kullanımı, toplam işlemleri belirleme | [Kullanım](/azure/marketplace/partner-center-portal/usage-dashboard) veya [Sipariş](/azure/marketplace/partner-center-portal/orders-dashboard) Panosu | **2. Ay** |
| Ödeme gönderildi | Ajans ücretini ve ödeme kazançlarını belirleme | Ödeme deyiminde İşlem Geçmişinde İşlenmemiş [olarak işaretlendi](payout-statement.md) | **3. ay (1. hafta)** |
| Ödeme hazırlama | Kazançlar aylık ödeme için hazırlanır | Ödeme hesap hesaplarında İşlem Geçmişi'ne Gelecek [olarak işaretlendi](payout-statement.md) | **3. ay (1. hafta)** |
| **Gönderilen ödeme** | **Ödeme yayımcıya gönderilir** | **İşlem Geçmişinde ve ödeme deyiminin Ödemeler bölümünde Gönderildi [olarak işaretlendi](payout-statement.md)** | **3. Ay (en geç 15. ay)** |
| Müşteri tarafından ödenen fatura | Microsoft müşteriden ödeme toplar | düzeltme sınıfı, | **4. ay ile 12. ay** |
|

\* Ödeme tarihi Pasifik Standart Saati'ne (PST) göredir.

:::image type="content" source="images/payouts/timeline-enterprise.png" alt-text="Kurumsal anlaşma müşterileri için ödemelerin zaman çizelgesi.":::

### <a name="transactions-when-customer-has-a-microsoft-customer-agreement-or-csp"></a>Müşterinin bir Microsoft Müşteri Sözleşmesi veya CSP'ye sahip olduğu işlemler

Kredi kartı veya aylık fatura ile yapılan tüm satın almaların müşteriden fon toplanmış olduğundan emin olmak için 30 günlük tutma süresi vardır.

| Olay | Description | Raporlama Görünürlüğü | Zamanlama* |
| --- | --- | --- | --- |
| Kullanım veya işlem ayı | Müşteri bir hizmet kullanır veya satın alır. | [Kullanım](/azure/marketplace/partner-center-portal/usage-dashboard) veya [Sipariş](/azure/marketplace/partner-center-portal/orders-dashboard) Panosu | **1. Ay** |
| Müşteri tarafından ödenen fatura | Toplam kullanımı, toplam işlem değerini ve müşteri ödeme faturasını belirleme | [Kullanım](/azure/marketplace/partner-center-portal/usage-dashboard) veya [Sipariş](/azure/marketplace/partner-center-portal/orders-dashboard) Panosu | **2. Ay** |
| Ödeme gönderildi | Ajans ücretini ve ödeme kazançlarını belirleme | Ödeme deyiminde İşlem Geçmişinde İşlenmemiş [olarak işaretlendi](payout-statement.md) | **2. Ay** |
| 30 günlük tutma süresi | Fon toplama, olası geri ödeme ve para iadesi isteklerinin top olduğundan emin olmak | Ödeme deyiminde İşlem Geçmişinde İşlenmemiş [olarak işaretlendi](payout-statement.md) | **3. Ay** |
| Ödeme hazırlama | Kazançlar aylık ödeme için hazırlanır | Ödeme hesap hesaplarında İşlem Geçmişi'ne Gelecek [olarak işaretlendi](payout-statement.md) | **4. ay (1. hafta)** |
| **Gönderilen ödeme** | **Ödeme yayımcıya gönderilir** | **İşlem Geçmişinde ve ödeme deyiminin Ödemeler bölümünde Gönderildi [olarak işaretlendi](payout-statement.md)** | **4. Ay (en geç 15. ay)** |
|

\* Ödeme tarihi Pasifik Standart Saati'ne (PST) göredir.

:::image type="content" source="images/payouts/timeline-credit-card-invoice.png" alt-text="Kredi kartı ve fatura müşterileri için ödemelerin zaman çizelgesi.":::

## <a name="process-for-customer-non-payment"></a>Ödemesi olmayan müşteri için işlem

Microsoft, nadiren ticari market satın almaları için müşterilerden ödeme topamıyor. Müşteri faturalama zaman çizelgesine göre Microsoft'a ödemesi başarısız olduğunda koleksiyonlar işlemini başlatacağız. Bu işlem yaklaşık dört ay sürer ve Microsoft'tan kalıcı iletişim gerektirir. Bu işlem sonunda ödeme alınamazsa Microsoft, fonlarını toplaması mümkün olmayan bir şekilde yazar.

Burada ifade etmek gerekirken Microsoft, sonunda toplaması kabul edilemez olan yayımcılara (sizin) fonlar ödemiş olabilir. Bu nedenle, bu miktarları mu mutabakata varmak için bir sürecimiz vardır.

Microsoft, aşağıdaki yöntemlerden birini kullanarak size zaten ödenen tüm ödemelerin ücretlerini karşılar: (1) Microsoft, ödenmemiş tutarları gelecekteki ödemelerden çıkarır; Örneğin, ödemelerde 1.000 ABD doları atıf yapılmaz ve yazılabilir olarak kabul edilirse, 1.000 ABD doları kurtarılana kadar gelecekteki ödemeniz geri alınmayacak veya (2) Microsoft, ödenmemiş tutarlar için para iadesi veya fatura yayımcıları talep edilebilir.

Aşağıdaki zamanlama bir örnektir:

| Olay | Yaklaşık tarih* | İş ortağı görünürlüğü |
| --- | --- | --- |
| Örnek ödeme tarihi | 10/15/2020 | İşlem **Geçmişinde** ve Ödeme Panosu'nın Ödemeler bölümünde Gönderildi olarak işaretlendi |
| <font color="red">Müşteri Microsoft'a ödemezse</font> | 12/2/2020 – 12/5/2020 | Yukarıdakiyle aynı şekilde değişiklik yok |
| Müşteri ilk geç ödeme e-postası alır | 12/6/2020 | Hiçbiri |
| Müşteri artan aciliyet e-postalarını alıyor | 12/7/2020 – 1/31/2021 | Hiçbiri |
| Publisher büyük olasılıkla kapalı olduğu bildirildi | 1/7/2021 | - |
| Müşteri sonlandırma bildirimini alır | 2/1/2021 | Hiçbiri |
| Toplama işleminin bitişi/fonları yazılır | 2/15/2021 | Fonların yazıldığı yayımcıya gönderilen e-posta bildirimi. |
| Ödeme kesinti | 01.03.2021 | Publisher, iş ortağı merkezi ödeme deyimindeki negatif işlem görür |
| Ödeme stopaj uygulanan | 3/15/2021 | Gelecekteki ödemeler, Iş Ortağı Merkezi ödeme bildiriminde gösterilir. Publisher, bakiye artık negatif olmayacak şekilde ödeme almaz.  |
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
