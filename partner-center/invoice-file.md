---
title: Fatura İş Ortağı Merkezi anlama
ms.topic: article
ms.date: 05/18/2020
description: Fatura dosyanız için fatura dosyasındaki alanları İş Ortağı Merkezi olun. Tüm fatura alanları ve tek ücret alanları için alanlar ve tanımlar dahildir.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5cb60c775bd8de38b8d7ca69c4dd97cf11b919fd
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146621"
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
| Krediler | Aboneliklerde yapılan değişiklikler için krediler veya düzeltmeler (örneğin, lisans artışları veya düşüşleri). |
| Ara toplam | Vergiler ve vergiye özel ücretler ile kredilerden önce toplam. |
| Vergi | Faturanın 2. sayfasından itibaren Ayrıntılar bölümünde **toplam** olarak geçerli ücretlerinizin toplam vergisi. Bu sayı, kullanım tabanlı mutabakat dosyanız **içinde TaxAmount** sütunundaki **(AA** sütunu)  ve lisans tabanlı mutabakat dosyanız içinde Vergi sütunu **(sütun U)** olan tüm ücretlerin toplamıdır. |
| Diğer krediler | Vergiye özel krediler. |
| Toplam geçerli ücretler | Faturalama dönemi için faturalama para biriminize bağlı olan tutar. Bu ücretler ödemenin son tarihine göredir. |
| Ödeme yönergeleri | Bölgenize göre faturanızı ödemenin açıklaması. *Ödeme yaparken her zaman fatura numaranızı dahil etmek için emin olun.* |
| Fatura no | Faturanın numarası. |
| Faturalama dönemi | Fatura tarihine kadar olan aylık dönem. Bu süre, kullanım tabanlı hizmetlerin tüketildiği ve lisans tabanlı hizmetlerin tüm kredi ayarlamaları veya lisans sayısı değişiklikleri için mu mutabakata varılacağı dönemdir. |
| Fatura tarihi | Faturanın her ay oluşturulacak faturalama tarihi veya yıldönümü tarihi. |
| Ödeme koşulları | Ödeme dönemi. Tek seferlik satın alımlarda bu, her zaman 60 gün olur. |
| Ödeme bitiş tarihi | Ödemenizin alınması gereken tarih. |
| Müşteri PO 'su | Satın alma numaranız siparişiniz. |
| Müşteri hizmetleri | Müşteri hizmetine erişebileceğiniz Web sitesi adresi. |
| Hizmet alıcısı | Hizmetin kullanıldığı adres. (Bu, şirket tarafından mücadele ile ilişkili yasal Şirket adresidir.) |

## <a name="one-time-charges-fields"></a>Tek seferlik ücretler alanları

Aşağıdaki alanlar yalnızca Iş ortağı merkezindeki **tek seferlik ücretler** için geçerlidir:

| Alan | Tanım |
| ----- | ---------- |
| Tarih | Satın alma tarihi. |
| Description | Ürün adı. |
| Miktar | Satın alınan ürünlerin (rezervasyonlar gibi) sayısı. |
| Birim fiyat | Ürün başına fiyat (örneğin, bir ayırma). |
| İndirimler | Geçerli iskontolar. |
| Vergi öncesi tutar | Vergi öncesi satın alımlarınızın alt toplamı. |
| Satış vergisi | Vergi tutarı. |
| Toplam | Toplam ödeme tutarı. |
