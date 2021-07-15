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
ms.openlocfilehash: 10438ba30c6eb5ba5b1daef1ad16521f1f8e77c6
ms.sourcegitcommit: 70b8ebbe0d431c7a13529f9eabd1b24f40108a46
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/14/2021
ms.locfileid: "113989783"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a>Iş Ortağı Merkezi mutabakatı dosyalarındaki farklı ücret türlerini anlayın

**Uygulama hedefi**: Iş Ortağı Merkezi | Microsoft Cloud for US Government için iş ortağı Merkezi

**Uygun roller**: yönetici Aracısı | Faturalandırma Yöneticisi | Genel yönetici

Bu makalede, bir fatura bölümü ve mutabakat dosyanızda olabilecek ilişkili ücret türleri arasındaki eşlemeler açıklanır. Faturanızda ücretler özeti sağlanmaktadır. Mutabakat dosyanız, ücret türleri dahil olmak üzere satır öğesi işlemlerinin ayrıntılı bir dökümünü sağlar. Karşılaştırma dosyaları hakkında daha fazla bilgi için bkz. [karşılaştırma dosyalarını kullanma](use-the-reconciliation-files.md).

Hem [Kullanım tabanlı](usage-based-recon-files.md) hem de [Lisans tabanlı mutabakat dosyaları](license-based-recon-files.md) yalnızca kullanımla ilgili işlemler ve ücretler (tüketilen birimler ve ilgili ücretler) gösterir.

> [!NOTE]
> Tek kapalı krediler, faturada görüntülenen iskontolar veya para iadesi, mutabakat dosyasında  gösterilmez.

## <a name="map-charge-types-to-invoice-charges"></a>Ücret türlerini fatura ücretlerine eşleyin

Fatura ve mutabakat dosyanız arasında çapraz başvuru ücret miktarları için Microsoft Excel ' deki filtre seçeneklerini kullanın. Mutabakat dosyasındaki ücretlendirme türlerine göre filtreleme yaparak fatura ücretlerini mutabakat dosyasındaki bir dizi ücret dökümü ile eşleyin.

## <a name="license-based-charges"></a>Lisans tabanlı ücretler

Bu lisans tabanlı ücretleri faturanızda eşlemek için, lisans tabanlı dosyadaki **tutar** sütununu toplayın.

| Ücretlendirme açıklaması (mutabakat dosyasındaki ChargeType sütunu) | Ücret açıklaması |
| ------------------------------------------------------------- | ------------------ |
| Etkinleştirme ücreti | Satın alma işleminden sonra aboneliği kullandıklarında müşteriye ücretlendirilen miktar. |
| Ücreti iptal et | İlişkili lisanslar değiştirildiğinde müşteriye eşit olarak dağıtılmış ücretler müşteriye iade edildi. |
| Örnek eşit olarak iptal et | Aylık aboneliğe sahip müşteri, abonelik askıya alındı ve ilişkili lisanslar aynı ay içinde değiştiği zaman eşit olarak dağıtılmış ücretler iptal edilir. |
| Bisiklet ücreti | Bir abonelik için dönemsel ücretler. |
| Bisiklet örneği eşit | İlişkili lisanslar değiştirildiğinde müşteriden alınan eşit oranda dağıtılmış ücretler. |
| İptal edildiğinde eşit ücret ücretleri | İptal sonrasında hizmetin kullanılmayan bölümü için eşit olarak dağıtılmış para iadesi. |
| Geçerli sunumdan uzakta değişiklik yaparken eşit ücretler | Geçerli aylık abonelikten bir yıllık aboneliğe dönüştürmeden sonra eşit olarak dağıtılmış ücretler. |
| Yeni bir teklife dönüştürülürken eşit ücretler ücretleri | Aylık bir aboneliği yeni bir yıllık aboneliğe dönüştürdükten sonra eşit olarak dağıtılmış ücretler. |
| Satın alma sırasında ücretleri eşit oranda artır | Aylık veya yıllık faturalandırma kullanılırken bir abonelik için ücret türü. |
| Yenileme sırasında eşit ücret ücreti | Abonelik yenileme sonrasında eşit olarak dağıtılmış ücretler. |
| Ücretleri Yenile | Abonelik yenileme ücreti |
| Etkinleştirmede eşit ücretler | Faturalandırma döneminin sonuna kadar etkinleştirilmesinin eşit olarak dağıtılmış ücretleri. |

## <a name="one-time-charges"></a>Tek seferlik ücretler

Bu tek seferlik ücretleri faturanızda eşlemek için, **tutar** sütununu lisans tabanlı dosyadan toplayın.

| Ücretlendirme açıklaması (mutabakat dosyasındaki ChargeType sütunu) | Ücret açıklaması |
| ------------------------------------------------------------- | ------------------ |
| new | Yeni bir satın alma oluşturulduğunda kullanılır. |
| yenileme | Dönem sonundan sonra bir abonelik yenilendiğinde kullanılır. |
| addQuantity | Hem orijinal satınalmanın para iadesi hem de bir artmadan sonraki yeni miktarın kullanıldığı. |
| removeQuantity | Orijinal satınalmanın para iadesi ve yeni miktarın bir azalmadan sonraki aşamasında kullanılır. |
| cancelImmediate | Abonelik iptal edildiğinde kullanılır. |
| dönüştürme | Bir lisans yükseltildiğinde kullanılır. |
| Müşterinin kredisi | Kredi (örn. Azure, SLA, vb.) bir işleme göre verildiğinde kullanılır. |

## <a name="usage-charges"></a>Kullanım ücretleri

Bu kullanım ücretlerini faturanızda eşlemek için, kullanım tabanlı dosyadaki **Pretaxcharges** sütununu toplayın.

| Ücretlendirme açıklaması (mutabakat dosyasındaki ChargeType sütunu) | Ücret açıklaması |
| ------------------------------------------------------------- | ------------------ |
| İptal edildiğinde kullanım ücretini değerlendir | Geçerli fatura döneminde ücretsiz kullanım için İptalden sonra kullanım ücretini erişin. |
| Geçerli döngüyle ilgili kullanım ücretini değerlendir | Geçerli fatura dönemi için kullanım ücretine erişin. |

### <a name="credits"></a>Krediler

Bu kredileri faturanızda eşlemek için:

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
