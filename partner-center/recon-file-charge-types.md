---
title: Mutabakat dosya ücreti türleri
ms.topic: article
ms.date: 06/05/2020
description: Mutabakat dosyalarında ücret türlerini (lisans tabanlı, kullanım tabanlı ve bir kez), kredileri ve indirimleri İş Ortağı Merkezi keşfedin.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8e41210f6eedbea36e72d5d4408fd102e7f7d3289f3f1a7c0ee635fe226aa427
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115688905"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a>Mutabakat dosyalarında farklı ücret İş Ortağı Merkezi anlama

**Için geçerlidir:** İş Ortağı Merkezi | İş Ortağı Merkezi için Microsoft Cloud for US Government

**Uygun roller:** Yönetici aracısı | Faturalama yöneticisi | Genel yönetici

Bu makalede, mutabakat dosyanız üzerinde yer alan fatura bölümü ve ilişkili ücret türleri arasındaki eşlemeler açıklanmıştır. Faturanız ücretlerin özetini sağlar. Mutabakat dosyanız, ücret türleri de dahil olmak üzere satır öğesi işlemlerinin ayrıntılı dökümünü sağlar. Mutabakat dosyaları hakkında daha fazla bilgi için [bkz. mutabakat dosyalarını kullanma.](use-the-reconciliation-files.md)

Hem [kullanım tabanlı mutabakat dosyaları hem](usage-based-recon-files.md) de lisans tabanlı mutabakat [dosyaları](license-based-recon-files.md) yalnızca kullanımla ilgili işlemleri ve ücretleri (tüketilen birimler ve ilgili ücretler) gösterir.

> [!NOTE]
> Düzeltmeler olarak faturada görünen tekli krediler, **indirimler** veya para iadeleri mutabakat dosyasında gösterilmez.

## <a name="map-charge-types-to-invoice-charges"></a>Ücret türlerini fatura ücretleriyle eşleme

Fatura ve mutabakat dosyanız arasındaki ücret tutarlarına çapraz başvuru yapmak için, fatura ve mutabakat Microsoft Excel. Mutabakat dosyanız üzerinde ücret türlerine göre filtreleerek fatura ücretlerini mutabakat dosyasındaki bir ücret dökümleri kümesiyle eşler.

## <a name="license-based-charges"></a>Lisans tabanlı ücretler

Bu lisans tabanlı ücretleri faturanıza eşlemek için, lisans **tabanlı** dosyadaki Tutar sütununu topla.

| Ücret açıklaması (mutabakat dosyasında ChargeType sütunu) | Ücret açıklaması |
| ------------------------------------------------------------- | ------------------ |
| Etkinleştirme ücreti | Satın alma sonrasında aboneliği kullanan müşteriye tahsil edilecek tutar. |
| Ücreti iptal etme | İlişkili lisanslar değiştiriken müşteriye iade edilecek, proratlı ücretler. |
| Örnek prorate işlemini iptal etme | Aylık aboneliği olan müşterinin aboneliği askıya alındı ve ilişkili lisanslar aynı ay içinde değişti. |
| Döngü ücreti | Bir abonelik için düzenli ücretler. |
| Döngü örneği hızı | İlişkili lisanslar değiştiriken müşteri tarafından değerlendirilen prorated ücretler. |
| İptal edilirken ücretlerin prorate işlemi | İptalin ardından hizmetin kullanılmayan kısmı için prorated para iadesi. |
| Geçerli tekliften dönüştürülürken ücretlerin prorate (prorate) | Geçerli aylık abonelikten yıllık aboneliğe dönüştürüldikten sonra prorated ücretler. |
| Yeni bir teklife dönüştüren ücretlerin prorate (prorate) | Aylık abonelik yeni bir yıllık aboneliğe dönüştürüldikten sonra prorated ücretler. |
| Satın almada ücret prorate | Aylık veya yıllık faturalama kullanırken aboneliğin ücret türü. |
| Yenilemede prorate ücreti | Abonelik yenilemesi sırasında prorated ücretler. |
| Ücreti yenileme | Aboneliği yenileme ücreti |
| Etkinleştiren ücretler için prorate (prorate) | Etkinleştirmeden faturalama döneminin sonuna kadar protratılmış ücretler. |

## <a name="one-time-charges"></a>Tek seferlik ücretler

Bu tek seferlik ücretleri faturanıza eşlemek için lisans tabanlı **dosyadan** Amount sütununu topla.

| Ücret açıklaması (mutabakat dosyasında ChargeType sütunu) | Ücret açıklaması |
| ------------------------------------------------------------- | ------------------ |
| new | Yeni bir satın alma oluşturulduğunda kullanılır. |
| yenileme | Bir abonelik, süre sona erdikten sonra yenilendikten sonra kullanılır. |
| addQuantity | Hem özgün satın alma para iadesi hem de artış sonrasında yeni miktar için kullanılır. |
| removeQuantity | Hem özgün satın alma para iadesi hem de düşüş sonrasında yeni miktar için kullanılır. |
| cancelImmediate | Abonelik iptal edilirken kullanılır. |
| dönüştürme | Bir lisans yükseltilirken kullanılır. |
| customerCredit | Bir işlem için krediler (örneğin Azure, SLA vb.) verildiklerde kullanılır. |

## <a name="usage-charges"></a>Kullanım ücretleri

Bu kullanım ücretlerini faturanıza eşlemek için kullanım tabanlı dosyadan **PretaxCharges** sütununu toplamanız gerekir.

| Ücret açıklaması (mutabakat dosyasında ChargeType sütunu) | Ücret açıklaması |
| ------------------------------------------------------------- | ------------------ |
| İptal edilirken kullanım ücretini değerlendirme | Geçerli faturalama dönemi boyunca ödenmemiş kullanım için iptalten sonra kullanım ücretine erişin. |
| Geçerli döngü için kullanım ücretini değerlendirme | Geçerli faturalama dönemi için kullanım ücretine erişin. |

### <a name="credits"></a>Krediler

Bu kredileri faturanıza eşlemek için:

- Lisans tabanlı **dosyadan TotalForCustomer'ı** toplama.
- Kullanım tabanlı **dosyadan PostTaxTotal** sütununu toplama.

| Ücret açıklaması (mutabakat dosyasında ChargeType sütunu) | Ücret açıklaması |
| ------------------------------------------------------------- | ------------------ |
| Bir satır öğesini kaydırma | Vergiler dahil olmak üzere bir satır öğesi için kısmi veya tam para iadesi. |

### <a name="usage-based-discounts"></a>Kullanım tabanlı indirimler

Bu kullanım tabanlı indirimleri faturanıza eşlemek için, kullanım tabanlı dosyadan **PretaxCharges** sütununu toplamanız gerekir.

| Ücret açıklaması (mutabakat dosyasında ChargeType sütunu) | Ücret açıklaması |
| ------------------------------------------------------------- | ------------------ |
| Etkinleştirme indirimi | Abonelik etkinleştirildiğinde uygulanan indirim. |
| Döngü indirimi | Düzenli ücretlere uygulanan indirim. |
| İndirimi yenileme | Abonelik yenilendiklerinde uygulanan indirim. |
| İndirimi iptal etme | İndirimler iptal edilirken uygulanan ücretler. |

### <a name="license-based-discounts"></a>Lisans tabanlı indirimler

Lisans tabanlı indirimleri faturanıza eşlemek için, lisans tabanlı dosyadan **TotalOtherDiscount** sütununu toplamanız gerekir.

*Lisans tabanlı indirimler birden çok ücret türüne uygulanabilir.*
