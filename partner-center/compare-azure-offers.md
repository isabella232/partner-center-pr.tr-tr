---
title: CSP iş ortakları için Azure tekliflerini karşılaştırın
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Bulut çözümü sağlayıcısı (CSP) programındaki iş ortakları için yeni Microsoft ticaret deneyimindeki teklifler arasındaki önemli farkları karşılaştırın.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: d1544333cd2251dd26223bebf20ef08723e976fb
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148542"
---
# <a name="compare-differences-between-azure-offers-in-the-csp-program"></a>CSP programındaki Azure teklifleri arasındaki farkları karşılaştırın

**Uygun roller**: yönetici Aracısı | Faturalandırma Yöneticisi | Genel yönetici | Yardım Masası Aracısı | Satış Aracısı

Bu makalede, bulut çözümü sağlayıcısı (CSP) programındaki Azure teklifleri arasındaki temel farklılıklar açıklanır.

## <a name="overview-of-key-differences-between-azure-offers"></a>Azure teklifleri arasındaki önemli farklılıklara genel bakış

Aşağıdaki tabloda, yeni Microsoft ticaret deneyiminin bir parçası olan CSP program teklifleri arasındaki önemli farklılıklara genel bakış sunulmaktadır.

|**Teklif**| **Azure planı**|**Üçüncü taraf Market teklifleri**|**Azure Rezervasyonlar**|**CSP aracılığıyla satılan sunucu abonelikleri**|**Lisans tabanlı teklifler**|
|-------------------|:------|:-----|:---------|:--------------|:---------|
|Faturalandırma|Aylık|Değişken (teklif bağımlı)|Son müşteri|Tam terim veya 3 yıllık dönem için önde|Aylık veya yıllık|
|Lisans bkz.|Son müşteri|Değişken (teklif bağımlı)|Son müşteri| Son müşteri|Son müşteri|
|Kapsam terimi|İptal edilene kadar etkin|Değişken (teklife bağımlı)|Teklif açıklamasına bakın|Tüm Azure Rezervasyonları kendi benzersiz kapsam dönemine sahip olur. Tüm Sunucu Abonelikleri kendi benzersiz kapsam dönemine sahip olur.|   Ek lisanslar mevcut kapsam dönemine yaslıtacak|
|Otomatik Yenileme|Yes|Yes|Hayır| Hayır|Yes|
|Çoklu Para Birimi|Müşteri konumunu/para birimini temel alan fatura|Müşteri konumunu/para birimini temel alan fatura|Müşteri konumunu/para birimini temel alan fatura|Müşteri konumunu/para birimini temel alan fatura|İş ortağı konumu para birimine göre| 
|Mutabakat & fatura|Her müşteri konumu para birimi için ayrı fatura ve Mutabakat dosyası.  Ayrıca günlük olarak derecelendirilmiş kullanım dosyaları da (hem fatura hem de faturalanmamış bölümler için) sağlanıyor |Her müşteri konumu para birimi için ayrı fatura ve Mutabakat dosyası|Her müşteri konumu para birimi için ayrı fatura ve Mutabakat dosyası|Her müşteri konumu para birimi için ayrı fatura ve Mutabakat dosyası|Tek bir fatura ve Mutabakat dosyasındaki tüm siparişler|
|Fiyat listesi & teklif matrisi|Aylık olarak yayımlanmış ve ABD Doları cinsinden fiyatlandırılır *|Market teklifleri ve fiyatlandırma, gerçek zamanlı olarak CSV dosya biçimine aktarılabilir.|Tümü fiyatlandırma ve teklif ayrıntıları dahil ayrı, tek bir dosya. Ayrı bir teklif matrisi dosyası yok||Tümü fiyatlandırma ve teklif ayrıntıları dahil ayrı, tek bir dosya. Ayrı bir teklif matrisi yoktur.| 
|& değiş tokuş döndürür|Geçerli değildir. Azure planının satın alma eyleminde ticari bir işlem yoktur|Bir aylık ve 12 aylık lisans tabanlı tekliflerin yanı sıra kullanım tabanlı tekliflerin arasında farklılık gösterir.|Sipariş tarihi %100 kredisi alacak şekilde 5 günden daha az bir değer döndürür. Sipariş tarihi, eşit olarak 5 günden daha uzun bir süre sonra, Pro dereceli kredide %12 erken sonlandırma ücreti alacak. Yıllık aylık $50.000 ABD Doları (veya yerel para birimi eşdeğeri)|Sipariş tarihinden itibaren 60 günden az bir değer döndürür %100 kredi lisans anahtarları devre dışı bırakılır. Kısmi dönüşler kabul edilmez.|   30 günden az getirilmesi/iptaller, %100 kredi alır; 30 günden büyük getirilmesi/iptaller, bir Pro-dereceli kredi alır.|
|Coğrafi kullanılabilirlik|139 ülkeler-bu ülkelerin tam listesi burada bulunabilir.|Yeni ticaret ülke kullanılabilirliği ve müşteri para birimi matrisi, bu tekliflerin iş ortağı tarafından CSP 'de kullanılabilir hale getirilme kapsamını gösterir.|Tüm ayrıntılar için bkz. yeni ticaret teklifleri ülke kullanılabilirliği ve müşteri para birimi matrisi. Aynı piyasaya çıkma zamanlaması tüm yeni ticari teklifler için geçerlidir.|Tüm ayrıntılar için bkz. Yeni Ticaret Teklifleri Ülke Kullanılabilirliği ve Müşteri Para Birimi Matrisi.  Aynı çıkış zamanlaması tüm yeni ticari teklifler için geçerlidir.|247 ülke|
|Destek gereksinimleri|Standart CSP destek gereksinimleri.|Teklif yayımlama şirketi teknik desteklerden sorumludur.  CSP İş Ortağı satış öncesi etkinliklerden, işlemden ve faturalama desteğinden sorumludur.|Standart CSP destek gereksinimleri.|Standart CSP destek gereksinimleri.|Standart CSP destek gereksinimleri.|

*Microsoft, Azure ölçüm fiyatlarına program aracılığıyla gerçek zamanlı erişim için Q4'te fiyat listesi API'leri sağlar.

## <a name="next-steps"></a>Sonraki adımlar

- [Azure planına taşıma - çalışmaya başlama](azure-plan-get-started.md)

- [Azure planı satın alma](purchase-azure-plan.md)

- [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)