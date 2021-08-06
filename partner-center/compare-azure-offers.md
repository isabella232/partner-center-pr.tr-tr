---
title: CSP iş ortakları için Azure tekliflerini karşılaştırma
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Bulut Çözümü Sağlayıcısı (CSP) programı kapsamındaki iş ortakları için yeni Microsoft ticaret deneyiminde yer alan teklifler arasındaki temel farkları karşılaştırın.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 42d3597e9c91fcc448289a673aae2c672df6869c004e7162efd5d6235259db09
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115679895"
---
# <a name="compare-differences-between-azure-offers-in-the-csp-program"></a>CSP programında Azure teklifleri arasındaki farkları karşılaştırma

**Uygun roller:** Yönetici aracısı | Faturalama yöneticisi | Genel yönetici | Yardım masası aracısı | Satış aracısı

Bu makalede, Bulut Çözümü Sağlayıcısı (CSP) programı kapsamındaki Azure teklifleri arasındaki temel farklar açıklanmıştır.

## <a name="overview-of-key-differences-between-azure-offers"></a>Azure teklifleri arasındaki temel farklara genel bakış

Aşağıdaki tabloda, yeni Microsoft ticaret deneyiminin bir parçası olan CSP programı teklifleri arasındaki temel farklılıklara genel bir bakış yer alır.

|**Teklif**| **Azure planı**|**Üçüncü taraf market teklifleri**|**Azure Rezervasyonlar**|**CSP aracılığıyla satılan Sunucu Abonelikleri**|**Lisans tabanlı teklifler**|
|-------------------|:------|:-----|:---------|:--------------|:---------|
|Faturalandırma|Aylık|Değişken (teklife bağımlı)|Son müşteri|Tam dönem veya 3 yıllık dönem için ön|Aylık veya Yıllık|
|Lisans sahibi|Son müşteri|Değişken (teklife bağımlı)|Son müşteri| Son müşteri|Son müşteri|
|Kapsam Dönemi|İptal edilene kadar etkin|Değişken (teklife bağımlı)|Teklif açıklamasına bakın|Tüm Azure Rezervasyonları kendi benzersiz kapsam dönemine sahip olur. Tüm Sunucu Abonelikleri kendi benzersiz kapsam dönemine sahip olur.|   Ek lisanslar mevcut kapsam dönemine yaslıtacak|
|Otomatik Yenileme|Yes|Yes|Hayır| Hayır|Yes|
|Çoklu Para Birimi|Müşteri konumunu/para birimini temel alan fatura|Müşteri konumunu/para birimini temel alan fatura|Müşteri konumunu/para birimini temel alan fatura|Müşteri konumunu/para birimini temel alan fatura|İş ortağı konumu para birimine göre| 
|Mutabakat & fatura|Her müşteri konumu para birimi için ayrı fatura ve Mutabakat dosyası.  Ayrıca günlük olarak derecelendirilmiş kullanım dosyaları da (hem fatura hem de faturalanmamış bölümler için) sağlanıyor |Her müşteri konumu para birimi için ayrı fatura ve Mutabakat dosyası|Her müşteri konumu para birimi için ayrı fatura ve Mutabakat dosyası|Her müşteri konumu para birimi için ayrı fatura ve Mutabakat dosyası|Tek bir fatura ve Mutabakat dosyasındaki tüm siparişler|
|Teklif Matrisi & Listesi|Aylık yayımlanan ve ABD doları olarak fiyatlandı*|Market teklifleri ve fiyatlandırması, başlangıçtan itibaren gerçek zamanlı CSV dosya biçimine aktarabilirsiniz.|Tüm fiyatlandırma ve teklif ayrıntılarının dahil olduğu ayrı, tek dosya. Ayrı bir Teklif Matrisi dosyası yoktur||Tüm fiyatlandırma ve teklif ayrıntılarının dahil olduğu ayrı, tek dosya. Ayrı bir Teklif Matrisi yoktur.| 
|Değişimleri & döndürür|Geçerli değildir. Azure planının satın alma eylemlerinde ticari işlem yoktur|Bir aylık ve 12 aylık lisans tabanlı tekliflerin yanı sıra kullanım tabanlı teklifler arasında değişiklik gösterir.|Sipariş tarihini takip etmek için 5 gün içinde %100 kredi alır. Sipariş tarihini 5 gün sonra döndürürse, pro-rated kredisi ve pro-rated kredinin %12'si erken sonlandırma ücreti alır; Müşteri başına yıllık 50.000 ABD doları (veya yerel para birimi eşdeğeri) sınırı|Sipariş tarihini takip etmek için 60 gün içinde %100 kredi lisans anahtarları devre dışı bırakılır. Kısmi dönüşler kabul edilmeyecektir.|   30 günlük askıya almalar/iptaller %100 kredi alır; 30 günlük askıya almalar/iptaller için prot derecelendirmeli bir kredi alırsınız.|
|Coğrafi Kullanılabilirlik|139 ülke - Bu ülkelerin tam listesi burada mevcuttur.|Yeni Ticaret Teklifleri Ülke Kullanılabilirliği ve Müşteri Para Birimi Matrisi, bu tekliflerin iş ortağı tarafından CSP'de kullanılabilir yapmak için uygun olduğu kapsamı gösterir.|Tüm ayrıntılar için bkz. Yeni Ticaret Teklifleri Ülke Kullanılabilirliği ve Müşteri Para Birimi Matrisi. Aynı çıkış zamanlaması tüm yeni ticari teklifler için geçerlidir.|Tüm ayrıntılar için bkz. Yeni Ticaret Teklifleri Ülke Kullanılabilirliği ve Müşteri Para Birimi Matrisi.  Aynı çıkış zamanlaması tüm yeni ticari teklifler için geçerlidir.|247 ülke|
|Destek gereksinimleri|Standart CSP destek gereksinimleri.|Teklif yayımlama şirketi teknik desteklerden sorumludur.  CSP İş Ortağı satış öncesi etkinliklerden, işlemden ve faturalama desteğinden sorumludur.|Standart CSP destek gereksinimleri.|Standart CSP destek gereksinimleri.|Standart CSP destek gereksinimleri.|

*Microsoft, Azure ölçüm fiyatlarına program aracılığıyla gerçek zamanlı erişim için Q4'te fiyat listesi API'leri sağlar.

## <a name="next-steps"></a>Sonraki adımlar

- [Azure planına taşıma - çalışmaya başlama](azure-plan-get-started.md)

- [Azure planı satın alma](purchase-azure-plan.md)

- [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)