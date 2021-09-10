---
title: Faturalama - lisans tabanlı SaaS işlemleri
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Lisans tabanlı, hizmet olarak İş Ortağı Merkezi (SaaS) işlemleri için yaygın faturalama senaryoları hakkında bilgi alın.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9568a014de926682dd89dd9d06d1c6ca5b98ac71
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960065"
---
# <a name="common-billing-scenarios-for-license-based-saas-transactions-in-partner-center"></a>İş Ortağı Merkezi'de lisans tabanlı SaaS işlemleri için yaygın faturalama İş Ortağı Merkezi

**Uygun roller:** Yönetici aracısı | Faturalama yöneticisi | Yardım masası aracısı | Satış aracısı


Bu örnek [yaygın faturalama senaryoları,](common-billing-scenarios.md) hizmet olarak lisans tabanlı yazılım (SaaS) abonelikleri için İş Ortağı Merkezi.

## <a name="convert-a-free-trial-saas-subscription-to-a-paid-subscription"></a>Ücretsiz deneme SaaS aboneliğini ücretli aboneliğe dönüştürme

Bu senaryoda, lisans tabanlı ücretsiz deneme SaaS aboneliğinin yenilenmesi için faturalama açıklanıyor. Yenileme işlemi, ücretsiz denemeyi ücretsiz deneme döneminin sonunda ücretli aboneliğe dönüştürür.

Bu örnekte, 10 Haziran'da lisans tabanlı SaaS (hizmet olarak yazılım) aboneliğinin ücretsiz deneme sürümü satın aldınız. Bu ücretsiz deneme sürümü, ücretsiz deneme süresi sona erdiğinde ücretli abonelik olarak otomatik olarak yenilenir.

Mutabakat dosyaları aşağıdaki ücretleri içerir:

| Satın alma tarihi | Ücret başlangıç tarihi | Ücret bitiş tarihi | Birim fiyat | Birim miktarı | Toplam tutar | Ücret türü | Abonelik açıklaması |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 USD | 1 | 0 USD | Yeni | Ücretsiz deneme sürümü |
| 07/10/2019 | 07/10/2019 | 08/09/2019 | 2 ABD doları | 1 | 2 ABD doları | Yenile | Ücretli abonelik |

## <a name="cancel-a-free-trial-saas-subscription"></a>Ücretsiz deneme SaaS aboneliğini iptal etme

> [!TIP]
> Ücretsiz deneme süresi boyunca bile lisans tabanlı ücretsiz deneme SaaS aboneliğini istediğiniz zaman iptal edebilirsiniz.

Bu senaryoda, 1 Temmuz'da lisans tabanlı ücretsiz deneme SaaS aboneliği satın aldınız ve daha sonra bu aboneliği hemen İş Ortağı Merkezi.

Mutabakat dosyası aşağıdaki ücretleri içerir:

| Satın alma tarihi | Ücret başlangıç tarihi | Ücret bitiş tarihi | Birim fiyat | Birim miktarı | Toplam tutar | Ücret türü | Abonelik açıklaması |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 USD | 11 | 0 USD | Yeni | Ücretsiz deneme sürümü |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 USD | 11 | 0 USD | İptal | Ücretsiz deneme sürümü |

## <a name="convert-custom-meter-saas-subscription-to-another-sku"></a>Özel ölçüm SaaS aboneliğini başka bir SKU'ya dönüştürme

Bu senaryoda, aynı tarihte bir özel ölçüm SaaS aboneliğinin bir stok tutma biriminden (SKU) aynı ürün için başka bir SKU'ya nasıl dönüştürülmesi açıkmektedir.

Bu senaryoda, bir ürün altında bir SKU (Silver) satın aldı ve aynı tarihte bu ürünün altında başka bir kullanılabilir SKU'ya (Bronz) dönüştürtün.

Mutabakat dosyası aşağıdaki ücretleri içerir:

| Satın alma tarihi | SKU | Ücret başlangıç tarihi | Ücret bitiş tarihi | Birim fiyat | Birim miktarı | Toplam tutar | Ücret türü | Abonelik açıklaması |
| ------------- | ----------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Silver | 06/10/2019 | 06/10/2019 | 20 USD | 1 | 20 USD | Yeni | Özel ölçüm SaaS aboneliği |
| 06/10/2019 | Silver | 06/10/2019 | 06/10/2019 | 20 USD | 1 | -20 ABD doları | Dönüştür | Özel ölçüm SaaS aboneliği için prorated rebill |
| 06/10/2019 | Bronz | 06/10/2019 | 06/10/2019 | 10$ | 1 | 10$ | Dönüştür | Özel ölçüm SaaS aboneliği |

## <a name="purchase-and-cancel-a-customer-meter-saas-subscription-on-same-date"></a>Aynı tarihte müşteri ölçüm SaaS aboneliği satın alma ve iptal etme

Bu senaryoda, aynı tarihte satın aldığınız ve iptal edilen bir müşteri ölçüm SaaS Azure portal faturalaması açıklandı.

Bu senaryoda, özel bir ölçüm SaaS aboneliği satın Azure portal. Ardından aboneliği aynı tarihte iptal ettiniz.

| Satın alma tarihi | SKU | Ücret başlangıç tarihi | Ücret bitiş tarihi | Birim fiyat | Birim miktarı | Toplam tutar | Ücret türü | Abonelik açıklaması |
| ------------- | ------------- |----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Bronz | 06/10/2019 | 06/10/2019 | 10$ | 1 | 10$ | Yeni | Özel ölçüm SaaS aboneliği |
| 06/10/2019 | Bronz | 06/10/2019 | 06/10/2019 | 10$ | 1 | -10 ABD doları | CancelImmediate | Özel ölçüm SaaS aboneliği |
