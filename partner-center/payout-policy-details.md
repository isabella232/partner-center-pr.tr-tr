---
title: Ödeme zamanlamaları ve süreçleri
description: Ticari Market ve diğer işlemler için ödeme zamanlamaları ve çıkış işlemleri gibi ödemeler ve işlemler hakkında bilgi edinin.
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 12/04/2020
ms.openlocfilehash: f4d31a5cf0752d03248b0efddb98ce621f9174f9
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/31/2021
ms.locfileid: "106086184"
---
# <a name="payout-schedules-and-processes"></a>Ödeme zamanlamaları ve süreçleri

**Uygun roller**

- Hesap yöneticisi
- Genel yönetici

Bu makalede, Microsoft 'un ödeme zamanlaması açıklanır. bu durum, bir ödeyen durumunun nerede bulunacağını ve müşterinin ödeme yapılmadığı süreci anlatmaktadır.

## <a name="payment-schedules"></a>Ödeme zamanlamaları

Aşağıdaki bölümlerde, **Kurumsal Anlaşma** ve **kredi kartı/fatura** işlemleri için ödeme sürecimiz açıklanır.

### <a name="enterprise-agreement-transactions"></a>Kurumsal Anlaşma işlemler

Bir müşteri, mevcut Microsoft Kurumsal Anlaşma işlemler için kullanarak Microsoft AppSource veya Azure Marketi 'nden bir ürün satın aldığında, bir sonraki ödeme ömrü 30 günlük Müşteri faturasında ödemeler yayınlarız. Müşterinin kredi kartı kullandığı işlemler, ödemesinden önce 30 günlük bir bekleme süresi sağlar.

Bir ödeme genellikle Microsoft 'un müşteriden ödeme toplamasından önce meydana gelir. Müşteri Microsoft 'a ödeme yapdığımızda, ancak zaten bir ödeme yapmış olduğumuz eylemler için aşağıdaki [Müşteri ödemesiz işleme](#process-for-customer-non-payment) ' ya bakın.

| Olay | Description | Raporlama görünürlüğü | Zaman |
| --- | --- | --- | --- |
| İşlemin kullanımı veya ayı | Müşteri bir hizmeti kullanır veya satın alarak. | [Kullanım](/azure/marketplace/partner-center-portal/usage-dashboard) veya [sıralama](/azure/marketplace/partner-center-portal/orders-dashboard) panosu | **Ay 1** |
| Microsoft fatura tutarını hesaplar | Toplam kullanımı belirleme, toplam işlem | [Kullanım](/azure/marketplace/partner-center-portal/usage-dashboard) veya [sıralama](/azure/marketplace/partner-center-portal/orders-dashboard) panosu | **Ay 2** |
| Ödeme gönderildi | Ajantı ücretini ve ödeme kazançlarını belirleme | [Ödeme bildiriminde](payout-statement.md) Işlem geçmişinde işlenmemiş olarak işaretlendi | **Ay 3 (1 hafta)** |
| Ödeme hazırlığı | Kazançlar aylık ödeme için hazırlandı | [Ödeme bildiriminde](payout-statement.md) Işlem geçmişinde yakında çıkacak şekilde işaretlendi | **Ay 3 (1 hafta)** |
| **Ödeme gönderildi** | **Ödeme, yayımcıya gönderilir** | **Işlem geçmişinde ve ödeme [bildiriminin](payout-statement.md) ödemeler bölümünde gönderildi olarak işaretlendi** | **3. ay (15 ' ten sonra değil)** |
| Müşteriye göre ödenen fatura | Microsoft müşteriden ödeme toplar | düzeltme sınıfı, | **Ay 4 ila 12** |
|

\* Ödeme tarihi Pasifik standart saatine (PST) göre yapılır.

:::image type="content" source="images/payouts/timeline-enterprise.png" alt-text="Kurumsal Anlaşma müşterileri için ödemelerin zaman çizelgesi.":::

### <a name="transactions-with-credit-card-or-invoice-checkwire"></a>Kredi kartı veya fatura ile işlemler (Çek/tel)

Kredi kartına veya aylık faturaya sahip tüm satın alımlarda, müşteri üzerinden fon toplandığından emin olmak için 30 günlük bir bekleme süresi bulunur.

| Olay | Description | Raporlama görünürlüğü | Zaman |
| --- | --- | --- | --- |
| İşlemin kullanımı veya ayı | Müşteri bir hizmeti kullanır veya satın alarak. | [Kullanım](/azure/marketplace/partner-center-portal/usage-dashboard) veya [sıralama](/azure/marketplace/partner-center-portal/orders-dashboard) panosu | **Ay 1** |
| Müşteriye göre ödenen fatura | Toplam kullanımı, toplam işlem değerini ve müşterinin ödediği faturayı belirleme | [Kullanım](/azure/marketplace/partner-center-portal/usage-dashboard) veya [sıralama](/azure/marketplace/partner-center-portal/orders-dashboard) panosu | **Ay 2** |
| Ödeme gönderildi | Ajantı ücretini ve ödeme kazançlarını belirleme | [Ödeme bildiriminde](payout-statement.md) Işlem geçmişinde işlenmemiş olarak işaretlendi | **Ay 2** |
| 30 günlük tutulduğu dönem | Fonların toplanması, olası geri göndermeler ve geri ödeme istekleri olduğundan emin olun | [Ödeme bildiriminde](payout-statement.md) Işlem geçmişinde işlenmemiş olarak işaretlendi | **Ay 3** |
| Ödeme hazırlığı | Kazançlar aylık ödeme için hazırlandı | [Ödeme bildiriminde](payout-statement.md) Işlem geçmişinde yakında çıkacak şekilde işaretlendi | **Ay 4 (1 hafta)** |
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
| Örnek ödeme tarihi | 10/15/2020 | Ödeme panosundaki Işlem geçmişi ve ödemeler bölümünde **gönderildi** olarak işaretlendi |
| <font color="red">Müşteri Microsoft 'a ödeme yapmasa da</font> | 12/2/2020 – 12/5/2020 | Değişiklik yok, yukarıdaki ile aynı |
| Müşteri ilk geç ödeme e-postasını alır | 12/6/2020 | Yok |
| Müşteri, artan aciliyet e-postalarını alır | 12/7/2020 – 1/31/2021 | Yok |
| Yayımcı, yazma işlemi için büyük olasılıkla | 1/7/2021 | Müşteriye henüz ödeme gönderilmemiş olan e-posta bildirimi gönderilir. İşlem KIMLIĞI ve dolar miktarı dahil edilir. |
| Müşteri sonlandırma bildirimini alır | 2/1/2021 | Yok |
| Toplama işleminin bitişi/fonları yazılır | 2/15/2021 | Fonların yazıldığı yayımcıya gönderilen e-posta bildirimi. İşlem KIMLIĞI ve dolar miktarı dahil edilir. |
| Ödeme kesinti | 01.03.2021 | Yayımcı, Iş Ortağı Merkezi ödeme bildiriminde negatif işlem görür |
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
