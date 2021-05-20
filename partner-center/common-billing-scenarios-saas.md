---
title: Faturalandırma-lisans tabanlı SaaS işlemleri
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lisans tabanlı, hizmet olarak yazılım (SaaS) işlemleri için Iş Ortağı Merkezi 'nde ortak faturalandırma senaryoları hakkında bilgi edinin.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 764d5a3cb0dc6f409e5272d4119424396caff53b
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148644"
---
# <a name="common-billing-scenarios-for-license-based-saas-transactions-in-partner-center"></a>Iş Ortağı Merkezi 'nde lisans tabanlı SaaS işlemleri için genel faturalandırma senaryoları

**Uygun roller**: yönetici Aracısı | Faturalandırma Yöneticisi | Yardım Masası Aracısı | Satış Aracısı


Bu örnek [genel faturalandırma senaryoları](common-billing-scenarios.md) , Iş Ortağı Merkezi 'nde lisans tabanlı yazılım hizmeti (SaaS) abonelikleri için geçerlidir.

## <a name="convert-a-free-trial-saas-subscription-to-a-paid-subscription"></a>Ücretsiz deneme SaaS aboneliğini ücretli aboneliğe dönüştürme

Bu senaryo, lisans tabanlı ücretsiz deneme SaaS aboneliğinin yenilenmesi için faturalandırmayı açıklar. Yenileme, ücretsiz denemeyi ücretsiz deneme süresi sonunda ücretli bir aboneliğe dönüştürür.

Bu örnekte, 10 Haziran 'da lisans tabanlı SaaS (hizmet olarak yazılım) aboneliği için ücretsiz bir deneme satın aldınız. Ücretsiz deneme süresi sona erdiğinde bu ücretsiz deneme, ücretli bir abonelik olarak otomatik olarak yenilenir.

Keşfi dosyaları aşağıdaki ücretleri içerir:

| Satın alma tarihi | Ücret başlangıç tarihi | Ücretlendirme bitiş tarihi | Birim fiyat | Birim miktarı | Toplam tutar | Ücret türü | Abonelik açıklaması |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 USD | 1 | 0 USD | Yeni | Ücretsiz deneme sürümü |
| 07/10/2019 | 07/10/2019 | 08/09/2019 | $2 | 1 | $2 | Yenile | Ücretli abonelik |

## <a name="cancel-a-free-trial-saas-subscription"></a>Ücretsiz deneme SaaS aboneliğini iptal etme

> [!TIP]
> Ücretsiz deneme süresi boyunca bile lisans tabanlı ücretsiz deneme SaaS aboneliğini dilediğiniz zaman iptal edebilirsiniz.

Bu senaryoda, 1 Temmuz 'da lisans tabanlı ücretsiz deneme SaaS aboneliğini satın almış ve sonra Iş Ortağı Merkezi ' nde hemen iptal etmiş olursunuz.

Keşfi dosyası aşağıdaki ücretleri içerir:

| Satın alma tarihi | Ücret başlangıç tarihi | Ücretlendirme bitiş tarihi | Birim fiyat | Birim miktarı | Toplam tutar | Ücret türü | Abonelik açıklaması |
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
| 06/10/2019 | Bronz | 06/10/2019 | 06/10/2019 | 10$ | 1 | 10$ | Dönüştür | Özel Ölçüm SaaS aboneliği |

## <a name="purchase-and-cancel-a-customer-meter-saas-subscription-on-same-date"></a>Müşteri ölçer SaaS aboneliğini aynı tarihte satın alıp iptal etme

Bu senaryo, satın aldığınız ve aynı tarihte Azure portal aracılığıyla iptal ettiğiniz bir müşteri ölçümü SaaS aboneliğine yönelik faturalandırma işlemini açıklar.

Bu senaryoda, Azure portal bir özel ölçüm SaaS aboneliği satın aldınız. Daha sonra, aynı tarihte aboneliği iptal etmiş olursunuz.

| Satın alma tarihi | SKU | Ücret başlangıç tarihi | Ücretlendirme bitiş tarihi | Birim fiyat | Birim miktarı | Toplam tutar | Ücret türü | Abonelik açıklaması |
| ------------- | ------------- |----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Bronz | 06/10/2019 | 06/10/2019 | 10$ | 1 | 10$ | Yeni | Özel Ölçüm SaaS aboneliği |
| 06/10/2019 | Bronz | 06/10/2019 | 06/10/2019 | 10$ | 1 | -10 ABD doları | CancelImmediate | Özel ölçüm SaaS aboneliği |
