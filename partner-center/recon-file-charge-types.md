---
title: Mutabakat dosya ücreti türleri
ms.topic: article
ms.date: 06/05/2020
description: Iş Ortağı Merkezi mutabakatı dosyalarındaki ücret türlerini (örneğin, lisans tabanlı, kullanım tabanlı ve tek seferlik), kredilerin ve indirimlerle bulun.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5a1f45de59fc9dac6a443bb8a14c3a80b36ba3f7
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855888"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a>Iş Ortağı Merkezi mutabakatı dosyalarındaki farklı ücret türlerini anlayın

**Uygulama hedefi**: Iş Ortağı Merkezi | ABD kamu için Microsoft Bulut iş ortağı Merkezi

**Uygun roller**: yönetici Aracısı | Faturalandırma Yöneticisi | Genel yönetici

Bu makalede, bir fatura bölümü ve mutabakat dosyanızda olabilecek ilişkili ücret türleri arasındaki eşlemeler açıklanır. Faturanızda ücretler özeti sağlanmaktadır. Mutabakat dosyanız, ücret türleri dahil olmak üzere satır öğesi işlemlerinin ayrıntılı bir dökümünü sağlar. Karşılaştırma dosyaları hakkında daha fazla bilgi için bkz. [karşılaştırma dosyalarını kullanma](use-the-reconciliation-files.md).

Hem [Kullanım tabanlı](usage-based-recon-files.md) hem de [Lisans tabanlı mutabakat dosyaları](license-based-recon-files.md) yalnızca kullanımla ilgili işlemler ve ücretler (tüketilen birimler ve ilgili ücretler) gösterir.

> [!NOTE]
> Tek kapalı krediler, faturada görüntülenen iskontolar veya para iadesi, mutabakat dosyasında  gösterilmez.

## <a name="map-charge-types-to-invoice-charges"></a>Ücret türlerini fatura ücretlerine eşleyin

Fatura ve mutabakat dosyanız arasında çapraz başvuru ücret miktarları için, Microsoft Excel 'deki filtre seçeneklerini kullanın. Mutabakat dosyasındaki ücretlendirme türlerine göre filtreleme yaparak fatura ücretlerini mutabakat dosyasındaki bir dizi ücret dökümü ile eşleyin.

## <a name="license-based-charges"></a>Lisans tabanlı ücretler

Bu lisans tabanlı ücretleri faturanızda eşlemek için, lisans tabanlı dosyadaki **tutar** sütununu toplayın.

| Ücretlendirme açıklaması (mutabakat dosyasındaki ChargeType sütunu) | Ücret açıklaması |
| ------------------------------------------------------------- | ------------------ |
| Etkinleştirme ücreti | Satın alma işleminden sonra aboneliği kullandıklarında müşteriye ücretlendirilen miktar. |
| Ücreti iptal et | İlişkili lisanslar değiştiriken müşteriye iade edilecek, proratlı ücretler. |
| Örnek prorate işlemini iptal etme | Aylık aboneliği olan müşterinin aboneliği askıya alındı ve ilişkili lisanslar aynı ay içinde değişti. |
| Döngü ücreti | Bir abonelik için düzenli ücretler. |
| Döngü örneği hızı | İlişkili lisanslar değiştiriken müşteri tarafından değerlendirilen, proratılmış ücretler. |
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
| Yeni | Yeni bir satın alma oluşturulduğunda kullanılır. |
| addQuantity | Hem özgün satın alma para iadesi hem de artış sonrasında yeni miktar için kullanılır. |
| removeQuantity | Hem özgün satın alma para iadesi hem de düşüş sonrasında yeni miktar için kullanılır. |
| İptal | Abonelik iptal edilirken kullanılır. |
| Dönüştür | Bir lisans yükseltilirken, ancak lisans sayısı değişmeden kalır. |

## <a name="usage-charges"></a>Kullanım ücretleri

Bu kullanım ücretlerini faturanıza eşlemek için kullanım tabanlı dosyadan **PretaxCharges** sütununu toplamanız gerekir.

| Ücret açıklaması (mutabakat dosyasında ChargeType sütunu) | Ücret açıklaması |
| ------------------------------------------------------------- | ------------------ |
| İptal edilirken kullanım ücretini değerlendirme | Geçerli faturalama dönemi boyunca ödenmemiş kullanım iptali sırasında kullanım ücretine erişin. |
| Geçerli döngü için kullanım ücretini değerlendirme | Geçerli faturalama dönemi için kullanım ücretine erişin. |

### <a name="credits"></a>Krediler

Bu kredileri faturanıza eşlemek için:

- Lisans tabanlı dosyadan **Totalforcustomer** toplamını toplayın.
- Kullanım tabanlı dosyadaki **Posttaxtotal** sütununu toplayın.

| Ücretlendirme açıklaması (mutabakat dosyasındaki ChargeType sütunu) | Ücret açıklaması |
| ------------------------------------------------------------- | ------------------ |
| Bir satır öğesinin sapmasını | Vergiler dahil olmak üzere bir satır öğesine kısmi veya tam para iadesi. |

### <a name="usage-based-discounts"></a>Kullanım tabanlı indirimler

Bu kullanım tabanlı indirimleri faturanızda eşlemek için, kullanım tabanlı dosyadaki **Pretaxcharges** sütununu toplayın.

| Ücretlendirme açıklaması (mutabakat dosyasındaki ChargeType sütunu) | Ücret açıklaması |
| ------------------------------------------------------------- | ------------------ |
| Etkinleştirme indirimi | Abonelik etkinleştirildiğinde uygulanan indirim. |
| Devir indirimi | Düzenli ücretlere uygulanan indirim. |
| İndirimi Yenile | Abonelik yenilendiğinde uygulanan indirim. |
| İndirimi iptal et | İndirimler iptal edildiğinde uygulanan ücretler. |

### <a name="license-based-discounts"></a>Lisans tabanlı indirimler

Lisans tabanlı indirimleri faturanızda eşlemek için, **TotalOtherDiscount** sütununu lisans tabanlı dosyadan toplayın.

*Lisans tabanlı indirimler, birden çok ücret türüne uygulanabilir.*
