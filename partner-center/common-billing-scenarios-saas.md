---
title: Faturalandırma-lisans tabanlı SaaS işlemleri
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Lisans tabanlı, hizmet olarak yazılım (SaaS) işlemleri için Iş Ortağı Merkezi 'nde ortak faturalandırma senaryoları hakkında bilgi edinin.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 85b5b4c33226236b7fcc3ce6b4833c3d58aba58ebb281b80576c9f26d04ecfe3
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115682258"
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

## <a name="convert-custom-meter-saas-subscription-to-another-sku"></a>Özel Ölçüm SaaS aboneliğini başka bir SKU 'ya Dönüştür

Bu senaryoda, bir özel ölçüm SaaS aboneliğinin aynı ürün için aynı ürüne ait bir stok tutma biriminden (SKU) başka bir SKU 'ya nasıl dönüştürüleceği açıklanır.

Bu senaryoda, bir ürün altında bir SKU (Gümüş) satın aldınız ve bu ürünün altında bulunan başka bir SKU 'ya (Bronz) aynı tarihte dönüştürüyoruz.

Keşfi dosyası aşağıdaki ücretleri içerir:

| Satın alma tarihi | SKU | Ücret başlangıç tarihi | Ücretlendirme bitiş tarihi | Birim fiyat | Birim miktarı | Toplam tutar | Ücret türü | Abonelik açıklaması |
| ------------- | ----------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Silver | 06/10/2019 | 06/10/2019 | 20 USD | 1 | 20 USD | Yeni | Özel Ölçüm SaaS aboneliği |
| 06/10/2019 | Silver | 06/10/2019 | 06/10/2019 | 20 USD | 1 | -$20 | Dönüştür | Özel Ölçüm SaaS aboneliği için eşit olarak dağıtılmış yeniden faturalandırılır |
| 06/10/2019 | Bronz | 06/10/2019 | 06/10/2019 | 10$ | 1 | 10$ | Dönüştür | Özel ölçüm SaaS aboneliği |

## <a name="purchase-and-cancel-a-customer-meter-saas-subscription-on-same-date"></a>Aynı tarihte müşteri ölçüm SaaS aboneliği satın alma ve iptal etme

Bu senaryoda, aynı tarihte satın aldığınız ve abonelikten iptal edilen bir müşteri ölçüm SaaS Azure portal faturalaması açıklandı.

Bu senaryoda, özel bir ölçüm SaaS aboneliği satın Azure portal. Ardından aboneliği aynı tarihte iptal ettiniz.

| Satın alma tarihi | SKU | Ücret başlangıç tarihi | Ücret bitiş tarihi | Birim fiyat | Birim miktarı | Toplam tutar | Ücret türü | Abonelik açıklaması |
| ------------- | ------------- |----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Bronz | 06/10/2019 | 06/10/2019 | 10$ | 1 | 10$ | Yeni | Özel ölçüm SaaS aboneliği |
| 06/10/2019 | Bronz | 06/10/2019 | 06/10/2019 | 10$ | 1 | -10 ABD doları | CancelImmediate | Özel ölçüm SaaS aboneliği |
