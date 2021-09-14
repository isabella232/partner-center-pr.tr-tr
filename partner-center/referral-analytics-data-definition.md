---
title: Başvuru Analizi veri tanımları
ms.topic: article
ms.date: 08/10/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: Belge, başvuru Analizi sayfalarından indirebileceğiniz çeşitli raporlar ve veri tanımlarını listeler.
author: v-sausharma
ms.author: v-sausharma
ms.localizationpriority: medium
ms.openlocfilehash: e2409dcbfd2a9de677ef4ec79bf8749072859325
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248453"
---
# <a name="referral-analytics-export--data-definitions"></a>Başvuru Analizi dışarı aktarma – veri tanımları

**Uygun roller**: başvuru Yöneticisi

## <a name="introduction"></a>Giriş

Müşteri adayı ve ortak satış analizi sayfasındaki dışarı aktar düğmesini kullanarak ham veri kümelerini dışarı aktarabilirsiniz.

Veri tanımlarıyla birlikte indirebileceğiniz çeşitli raporlar aşağıdaki tablolarda listelenmiştir:

## <a name="leads-export"></a>Müşteri adaylarını dışarı aktarma

|   Sütun adı |   Veri açıklaması    |
|----|----|
|   Referans kimliği |   Başvuru için benzersiz KIMLIK  |
|   Müşteri ülkesi    |   Müşterinin ülkesi |
|   Müşteri Adı   |   Müşterinin adı    |
|   Başvuru oluşturma tarihi  |   Başvurunun Oluşturulma tarihi   |
|   Başvuru kaynağı |   Başvurunun kaynağı: nitelenmiş, Market  |
|   Başvuru türü   |   Müşteri adayının türü    |
|   Lider yönü  |   Müşteri adayının yönü   |
|   Lider para birimi   |   Müşteri adayının para birimi    |
|   Lider değeri  |   İş ortağı tarafından sunulan tahmini lider değeri    |
|   Lider değeri (USD)    |   İş ortağı tarafından ABD Doları cinsinden sunulan tahmini lider değeri |
|   Durum      |   Başvurunun en son durumu   |
|   Durum Nedeni   |   Durumun açıklamaları veya nedeni    |
|       |       |


## <a name="co-sell-export"></a>Ortak satış dışa aktarma

|   Sütun adı |   Veri açıklaması    |
|    ----    |    ----    |
|   Referans kimliği |   Başvuru için benzersiz KIMLIK  |
|   Müşteri ülkesi    |   Müşterinin ülkesi |
|   Müşteri şehri   |   Müşterinin şehri    |
|   Müşteri Adı   |   Müşterinin adı    |
|   Başvuru oluşturma tarihi  |   Başvurunun Oluşturulma tarihi   |
|   Anlaşma türü   |   Anlaşma türü: ortak satış, iş ortağı LED, özel |
|   Anlaşma yönü  |   İşlem yönü: gelen ve giden    |
|   Anlaşma para birimi   |   Anlaşma para birimi    |
|   Tahmini anlaşma değeri    |   İş ortağı tarafından sunulan tahmini anlaşma değeri    |
|   Tahmini anlaşma değeri (USD)  |   İş ortağı tarafından ABD Doları cinsinden sunulan tahmini anlaşma değeri |
|   Çözüm Kimliği     |   Çözüm KIMLIĞI listesi |
|   Çözüm Adı   |   Çözüm adları listesi  |
|   MPN Kimliği  |   İş ortağının Microsoft iş ortağı ağı KIMLIĞI |
|   İş ortağı adı    |   Ortağın adı |
|   Anlaşma kimliği |   Anlaşma KIMLIĞI  |
|   Katılım KIMLIĞI   |   Benzersiz katılım KIMLIĞI    |
|   Microsoft MSX KIMLIĞI    |   MSX-anlaşma KIMLIĞI  |
|   Microsoft başvurusu oluşturma tarihi    |   Microsoft 'a başvuru oluşturma tarihi |
|   Kayıtlı kişi adı soyadı   |   Anlaşma kaydı sırasında belirtilen iş ortağı kişisinin adı |
|   Kayıtlı kişi soyadı    |   Anlaşma kaydı sırasında belirtilen iş ortağı kişisinin soyadı  |
|   Kayıtlı iletişim e-postası    |   Anlaşma kaydı sırasında belirtilen iş ortağı kişisinin e-postası  |
|   Kayıtlı iletişim telefon numarası |   anlaşma kaydı sırasında belirtilen iş ortağı kişisinin Telefon sayısı   |
|   Sözleşme para birimi   |   Anlaşma kaydı sırasında belirtilen sözleşmenin para birimi  |
|   Sözleşme değeri  |   Anlaşma kaydı sırasında belirtilen toplam sözleşme değeri. Bu yazılım ve hizmet ücretlerini içerir ancak donanım maliyetlerini içermez  |
|   Sözleşme değeri (USD)    |   Anlaşma kaydı sırasında belirtilen ABD Doları cinsinden toplam sözleşme değeri   |
|   Sözleşme başlangıç tarihi |   Anlaşma kaydı sırasında belirtilen sözleşmenin başlangıç tarihi    |
|   Sözleşme bitiş tarihi   |   Anlaşma kaydı sırasında belirtilen sözleşmenin bitiş tarihi  |
|   Sözleşme Imza tarihi  |   Anlaşma kaydı sırasında belirtilen sözleşmenin imza tarihi |
|   Anlaşma türü   |   Sözleşmenin türü    |
|   Kayıtlı anlaşma çözüm KIMLIĞI |   Anlaşma kaydı için çözümün KIMLIĞI    |
|   Kayıtlı anlaşma çözümü adı   |   Anlaşma kaydı çözümünün adı  |
|   Kayıtlı anlaşma çözümü para birimi   |   Anlaşma kaydı sırasında sağlanan çözüm için para birimi |
|   Kayıtlı anlaşma çözümü değeri  |   Anlaşma kaydı sırasında sağlanan çözüm değeri. Genel olarak, bu toplam sözleşme değeri yinelenen olmayan uygulama ücretlerinin altındadır.   |
|   Kayıtlı anlaşma çözümü değeri (USD)    |   Anlaşma kaydı sırasında sağlanan ABD doları değerindeki çözüm değeri |
|   Dağıtıldı |   Çözümün Azure'da mı yoksa Diğerlerinde mi dağıtıldığından gösterir    |
|   Birincil Dağıtım   |   Çözümün Müşteri Kiracısına mı yoksa İş Ortağı Kiracısına mı dağıtıldıklarını gösterir  |
|   Anlaşma Oluşturma Tarihi  |   Anlaşma kaydının oluşturma tarihi  |
|   Anlaşma Gönderme Tarihi     |   Anlaşma kaydının gönderilme tarihi |
|   Anlaşma Onaylı/Reddedilen Tarih     |   Onaylandı/reddedilen tarihle ilgili anlaşma. Bu durum sütunuyla eşlenmiş. |
|   ABD Federal Anlaşması |   Bunun bir ABD federal anlaşması olup olmayacağını gösterir    |
|   Market Işlem Yapılan Anlaşma mı?  |   Bunun bir Market işlemli anlaşması olup olduğunu gösterir    |
|   Market işlem tarihi    |   Satış anlaşması markette işlem yapılan market işlem tarihi|
|   Durum      |   Referansların en son durumu   |
|   Durum Nedeni   |   Açıklamalar veya durum açıklaması    |
|       |       |
