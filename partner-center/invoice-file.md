---
title: Fatura İş Ortağı Merkezi anlama
ms.topic: article
ms.date: 05/18/2020
description: Fatura dosyanız için fatura dosyasındaki alanları İş Ortağı Merkezi olun. Tüm fatura alanları ve tek ücret alanları için alanlar ve tanımlar dahildir.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c741caa6993a5da415d3a94d541bf10c21470889
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114840085"
---
# <a name="understand-partner-center-billing-invoice-fields"></a>Fatura İş Ortağı Merkezi alanlarını anlama

**Uygun roller:** Genel yönetici | Kullanıcı yönetimi yönetici | Faturalama yöneticisi | Yardım masası aracısı

Fatura dosyalarında yer alan alanları anlamak için aşağıdaki İş Ortağı Merkezi kullanabilirsiniz.

## <a name="invoice-file-fields"></a>Fatura dosyası alanları

Fatura dosyalarında aşağıdaki alanlar görünür.

| Alan | Tanım |
| ----- | ---------- |
| US FEIN | Federal İşveren Kimlik Numaranız (FEIN). Bu, Birleşik Devletler vergi numarasıdır. |
| Müşteri numarası | Müşteri numaranız. |
| Fatura adresi | Faturanızı gönder adresi. Şirket adı ve adresinizi faturalama profilinde İş Ortağı Merkezi değiştirebilirsiniz. |
| Lisans tabanlı ücretler | Satın aldığınız kullanım tabanlı lisansların aylık veya yıllık sabit ücretleri, hizmet öncesinde faturalandırıldı. Bu sayı, lisans tabanlı mutabakat **dosyanızdaki Alt toplam** sütunundaki **(sütun T)** tüm ücretlerin toplamıdır. |
| Kullanım tabanlı ücretler | Azure kullanımınız. Bu, faturalama döneminde etkin ve kullanılan yeni hizmetleri veya uygulamaları içerir. Bu sayı, kullanım tabanlı mutabakat dosyanız içinde **PretaxCharges** sütunundaki **(sütun Z)** tüm ücretlerin toplamıdır. |
| İndirimler | Müşterinin aboneliğin normal fiyatından aldığı indirim. Bu sayı birim veya *lisans başına fiyat* olarak değil sabit bir miktar olarak gösterilir. |
| Krediler | Aboneliklerde yapılan değişiklikler (örneğin lisans artışları veya düşüşleri) için krediler veya düzeltmeler. |
| Ara toplam | Vergiler ve vergiye özel ücretler ile kredilerden önce toplam. |
| Vergi | Faturanın 2. sayfasından itibaren Ayrıntılar bölümünde **toplam** olarak geçerli ücretlerinizin toplam vergisi. Bu sayı, kullanım tabanlı mutabakat dosyanız **içinde TaxAmount** sütunundaki **(AA** sütunu)  ve lisans tabanlı mutabakat dosyanız içinde Vergi sütunu **(sütun U)** olan tüm ücretlerin toplamıdır. |
| Diğer krediler | Vergiye özel krediler. |
| Toplam geçerli ücretler | Faturalama dönemi için faturalama para biriminize bağlı olan tutar. Bu ücretler ödemenin son tarihine göredir. |
| Ödeme yönergeleri | Bölgenize göre faturanızı ödemenin açıklaması. *Ödeme yaparken her zaman fatura numaranızı dahil etmek için emin olun.* |
| Fatura no | Faturanın numarası. |
| Faturalama dönemi | Fatura tarihine kadar olan aylık dönem. Bu süre, kullanım tabanlı hizmetlerin tüketildiği ve lisans tabanlı hizmetlerin tüm kredi ayarlamaları veya lisans sayısı değişiklikleri için mu mutabakata varılacağı dönemdir. |
| Fatura tarihi | Faturanın her ay oluşturulacak faturalama tarihi veya yıldönümü tarihi. |
| Ödeme koşulları | Ödeme dönemi. Tek seferlik satın almalar için bu süre her zaman 60 gün olur. |
| Ödeme son tarihi | Ödemenizin alın aldığı tarih. |
| Müşteri Po | Satın alma numarası siparişiniz. |
| Müşteri hizmetleri | Müşteri hizmetine erişebilirsiniz web sitesi adresi. |
| Hizmet alıcısı | Hizmetin kullandığı adres. (Bu, şirket bilgileriyle ilişkili yasal şirket adresidir.) |

## <a name="one-time-charges-fields"></a>Tek seferlik ücretler alanları

Aşağıdaki alanlar yalnızca bir yıllık **ücretlerde** İş Ortağı Merkezi:

| Alan | Tanım |
| ----- | ---------- |
| Tarih | Satın alma tarihi. |
| Description | Ürün adı. |
| Miktar | Satın alınan ürün sayısı (rezervasyonlar gibi). |
| Birim fiyat | Ürün başına fiyat (rezervasyon gibi). |
| İndirimler | Geçerli indirimler. |
| Vergi öncesi tutar | Vergilerden önce yapılan satın almaların alt toplamları. |
| Satış vergisi | Vergi tutarı. |
| Toplam | Toplam ödeme tutarı. |
