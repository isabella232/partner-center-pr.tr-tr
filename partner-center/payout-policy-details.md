---
title: Ödeme zamanlamaları ve ilke ayrıntıları-Azure Marketi
description: Zamanlamalar ve engel dahil olmak üzere ticari Market ödeme ilkelerine ilişkin ayrıntılar hakkında bilgi edinin.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: mingshen-ms
ms.author: mingshen
ms.date: 11/06/2020
ms.openlocfilehash: 8986ef1d2a16d939530ed49875a21c13b0b97868
ms.sourcegitcommit: 0e142b4fbb044fe8dd2dbc7d13ab70a1a91b9f60
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/09/2020
ms.locfileid: "94381401"
---
# <a name="payout-schedules-and-policy-details"></a>Ödeme zamanlamaları ve ilke ayrıntıları

Bu makalede, Microsoft 'un ödeme süreci, ödeme zamanlaması, bir ödeme durumunun nerede bulunacağı ve müşteri ödemesiz için işlem ele alınmaktadır.

## <a name="payment-schedules"></a>Ödeme zamanlamaları

Aşağıdaki bölümlerde, **Kurumsal Anlaşma** ve **kredi kartı/fatura** işlemleri için ödeme sürecimiz açıklanır.

### <a name="enterprise-agreement-transactions"></a>Kurumsal Anlaşma işlemler

Bir müşteri, mevcut Microsoft Kurumsal Anlaşma işlemler için kullanarak Microsoft AppSource veya Azure Marketi 'nden bir ürün satın aldığında, bir sonraki ödeme ömrü 30 günlük Müşteri faturasında ödemeler yayınlarız. Müşterinin kredi kartı kullandığı işlemler, ödemesinden önce 30 günlük bir bekleme süresi sağlar.

Bir ödeme genellikle Microsoft 'un müşteriden ödeme toplamasından önce meydana gelir. Müşteri Microsoft 'a ödeme yapdığımızda, ancak zaten bir ödeme yapmış olduğumuz eylemler için aşağıdaki [Müşteri ödemesiz işleme](#process-for-customer-non-payment) ' ya bakın.

| Olay | Açıklama | Raporlama görünürlüğü | Zaman |
| --- | --- | --- | --- |
| Işlemin kullanımı veya ayı | Müşteri bir hizmeti kullanır veya satın alarak. | [Kullanım](/azure/marketplace/partner-center-portal/usage-dashboard) veya [sıralama](/azure/marketplace/partner-center-portal/orders-dashboard) panosu | **Ay 1** |
| Satınalma siparişi oluşturuldu | Toplam kullanımı belirleme, toplam işlem | [Kullanım](/azure/marketplace/partner-center-portal/usage-dashboard) veya [sıralama](/azure/marketplace/partner-center-portal/orders-dashboard) panosu | **Ay 2** |
| ISV ödeme Işitme oluşturuldu | Ajantı ücretini ve ödeme kazançlarını belirleme | Ödeme bildiriminde Işlem geçmişinde Işlenmemiş olarak işaretlendi | **Ay 3 (1 hafta)** |
| Ödeme hazırlığı | Kazançlar aylık ödeme için hazırlandı | Ödeme bildiriminde Işlem geçmişinde yakında çıkacak şekilde işaretlendi | **Ay 3 (1 hafta)** |
| **Ödeme tarihi** | **Ödeme, yayımcıya gönderilir** | **Işlem geçmişinde ve ödeme bildiriminin ödemeler bölümünde gönderildi olarak işaretlendi** | **3. ay (15 ' ten sonra değil)** |
| Müşteriye göre ödenen fatura | Microsoft müşteriden ödeme toplar | düzeltme sınıfı, | **Ay 4 ila 12** |
|

\* Ödeme tarihi Pasifik standart saatine (PST) göre yapılır.

### <a name="customers-who-pay-using-credit-card-or-invoice"></a>Kredi kartı veya fatura kullanarak ödeme yapan müşteriler

Kredi kartına veya aylık faturaya sahip tüm satın alımlarda, müşteri üzerinden fon toplandığından emin olmak için 30 günlük bir bekleme süresi bulunur.

| Olay | Açıklama | Raporlama görünürlüğü | Zaman |
| --- | --- | --- | --- |
| Işlemin kullanımı veya ayı | Müşteri bir hizmeti kullanır veya satın alarak. | [Kullanım](/azure/marketplace/partner-center-portal/usage-dashboard) veya [sıralama](/azure/marketplace/partner-center-portal/orders-dashboard) panosu | **Ay 1** |
| Müşteriye göre ödenen fatura | Toplam kullanımı, toplam işlem değerini ve müşterinin ödediği faturayı belirleme | [Kullanım](/azure/marketplace/partner-center-portal/usage-dashboard) veya [sıralama](/azure/marketplace/partner-center-portal/orders-dashboard) panosu | **Ay 2** |
| ISV ödeme Işitme oluşturuldu | Ajantı ücretini ve ödeme kazançlarını belirleme | Ödeme bildiriminde Işlem geçmişinde Işlenmemiş olarak işaretlendi | **Ay 2** |
| 30 günlük tutma dönemi | Fonların toplanması, olası geri ödeme ve iade isteklerinin yapıldığından emin olun | Ödeme bildiriminde Işlem geçmişinde Işlenmemiş olarak işaretlendi | **Ay 3** |
| Ödeme hazırlığı | Kazançlar aylık ödeme için hazırlandı | Ödeme bildiriminde Işlem geçmişinde yakında çıkacak şekilde işaretlendi | **Ayın ilk haftası 4** |
| **Ödeme tarihi** | **Ödeme, yayımcıya gönderilir** | **Işlem geçmişinde ve ödeme bildiriminin ödemeler bölümünde gönderildi olarak işaretlendi** | **4. ay (15. günden sonra değil)** |
|

\* Ödeme tarihi, Pasifik Standart Saati (PST) olarak belirlenir.

## <a name="process-for-customer-non-payment"></a>Müşteri ödemesiz işlem

Nadir durumlarda Microsoft, ticari Market satın alımları için müşterilerden ödeme toplayamamaktadır. Bir müşteri Microsoft 'un faturalandırma zamanlamalarına göre ödeme yapamazsa koleksiyonlar işlemine başlayacağız. Bu işlem yaklaşık dört ay sürer ve Microsoft 'tan kalıcı iletişim içerir. Ödeme bu işlemin sonuna kadar alınmıyorsa, Microsoft fonları toplanabilir olmayan bir tablo olarak yazar.

Bu işlem için, Microsoft, bu işlemin sonunda, son olarak toplanabilir bir tablo olan yayımcılar 'a (siz) zaten ücret ödemüş olabilir. Bu nedenle, bu miktarları mutabık kılma sürecimiz vardır. (Zaten alınmış) ödemenin uzlaştırılabileceğini belirten bir uyarı olduğundan emin olmak için, bir müşteri koleksiyonlar sürecinde olduğunda ve satın alımlarınızın kapalı olma olasılığı varsa size bildirilir.

Microsoft, aşağıdaki yöntemlerden birini kullanarak zaten ücretli olan tüm ödemeler için ödeme yapacaktır: (1) Microsoft, ödenmemiş miktarları gelecekteki ödemeler üzerinden çıkartabilir; Örneğin, ödemelerden $1.000, toplanmamış tablo olarak kabul edilir ve bu durum devre dışı bırakılırsa, gelecekteki ödemelerden bazıları $1.000 kurtarılana veya (2) Microsoft, toplanan herhangi bir miktar için bir para iadesi veya fatura yayımcıları isteyebileceği için,

Örnek zamanlama aşağıda verilmiştir:

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

Genellikle söz konusu ayın 15. gününde belirli bir ay boyunca herhangi bir ödeme gönderiyoruz, ancak ödemenin hesabınıza ulaşması daha fazla zaman alır. Gün sayısı, aşağıda açıklandığı gibi, hesabınız için kullandığımız ödeme yöntemine bağlıdır.

> [!NOTE]
> Aşağıda gösterilen günler yaklaşık değerlerdir; Tüm ödemeler hesabınıza ulaşmak için daha uzun veya daha kısa bir süre alabilir.

| Ödeme yöntemi     | Ödeme hesabına ulaşma gün sayısı     |
|--------------------|--------------------------------------------|
| PayPal             | 1 iş günü                             |
| ACH/SEPA           | 2-3 iş günü                          |
| Tel aktarım      | 7-10 iş günü                         |
|

## <a name="next-steps"></a>Sonraki adımlar

[Vergi ayrıntıları](tax-details-marketplace.md)hakkında bilgi edinin.
