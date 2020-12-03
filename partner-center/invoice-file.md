---
title: Iş ortağı merkezi faturalama faturalarını anlama
ms.topic: article
ms.date: 05/18/2020
description: Iş Ortağı Merkezi faturalaması için fatura dosyanızdaki alanları anlayın. Dahil edilen alanlar ve tanımlar tüm fatura alanları ve tek seferlik ücret alanları için kullanılır.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3e9eb392279c0a09b5e30395b38ab7030bfa87d4
ms.sourcegitcommit: 147813ba322653c989df5afe0b3bf0c252523a92
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/03/2020
ms.locfileid: "96556302"
---
# <a name="understand-partner-center-billing-invoice-fields"></a>Iş ortağı merkezi faturalama faturası alanlarını anlayın

**Uygun roller**

- Genel yönetici
- Kullanıcı yöneticisi
- Faturalama yöneticisi
- Yardım Masası Aracısı

Iş ortağı merkezi fatura dosyalarındaki alanları anlamak için aşağıdaki tabloları kullanabilirsiniz.

## <a name="invoice-file-fields"></a>Fatura dosyası alanları

Fatura dosyalarınızda aşağıdaki alanlar görüntülenir.

| Alan | Tanım |
| ----- | ---------- |
| BIZE FEDA | Federal Işveren kimlik numaranız (FEIN). Bu Birleşik Devletler federal vergi tanımlayıcı numarasıdır. |
| Müşteri numarası | Müşteri numaranız. |
| Fatura adresi | Faturanızı gönderdiğimiz adres. Şirket adınızı ve/veya adresinizi Iş ortağı merkezi faturalama profilinizde değiştirebilirsiniz. |
| Lisans tabanlı ücretler | Satın alınan kullanım tabanlı lisanslarınız için aylık veya yıllık ücretler, hizmette önceden faturalandırılır. Bu sayı, lisans tabanlı mutabakat dosyanızdaki **alt toplam** sütunundaki (sütun **T**) tüm ücretlerin toplamıdır. |
| Kullanım tabanlı ücretler | Azure kullanımınız. Bu, faturalama döneminde etkinleştirilen ve kullanılan yeni hizmetleri veya uygulamaları içerir. Bu sayı, kullanım tabanlı mutabakat dosyanızdaki **Pretaxcharges** sütunundaki ( **Z** sütunu) tüm ücretlerin toplamıdır. |
| İndirimler | Müşterinin aboneliğin normal fiyatından aldığı indirim. Bu sayı, birim veya lisans başına fiyat olarak değil, *sabit bir tutar* olarak gösterilir. |
| Krediler | Aboneliklerde yapılan değişiklikler için krediler veya Ayarlamalar (örneğin, lisans artar veya azalır). |
| Ara toplam | Vergiler ve vergi dışlamalı ücretler ve kredilerin toplam sayısı. |
| Vergi | Faturanızda sayfa 2 ' den itibaren **Ayrıntılar** bölümünde toplanan geçerli ücretler için toplam vergi. Bu sayı, kullanım tabanlı mutabakat dosyanızdaki **TaxAmount** sütunundaki (sütun **AA**) tüm giderlerin toplamıdır ve lisans tabanlı mutabakat dosyanızdaki **vergi** sütunu (sütun **U**). |
| Diğer krediler | Vergi dışlamalı krediler. |
| Toplam geçerli ücret | Fatura dönemi için faturalandırma para biriminiz için gereken miktar. Bu ücretler, ödeme bitiş tarihi ile kaynaklanmaktadır. |
| Ödeme yönergeleri | Bölgenize göre faturanızı nasıl ödeyabileceğinize ilişkin açıklama. *Ödeme yaparken her zaman fatura numaranızı eklediğinizden emin olun.* |
| Fatura No | Faturanızda bulunan sayı. |
| Faturalama dönemi | Aylık dönem, fatura tarihine kadar önde gelen. Bu, kullanım tabanlı hizmetlerin kullanıldığı ve lisans sayımında yapılan kredi ayarlamaları ya da değişiklikler için lisans tabanlı hizmetlerin Uzlaştırılmakta olduğu dönemdir. |
| Fatura tarihi | Faturanızda her ay oluşturulan faturalandırma tarihi veya yıldönümü tarihi. |
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
| Açıklama | Ürün adı. |
| Miktar | Satın alınan ürünlerin (rezervasyonlar gibi) sayısı. |
| Birim fiyat | Ürün başına fiyat (örneğin, bir ayırma). |
| İndirimler | Geçerli iskontolar. |
| Vergi öncesi tutar | Vergi öncesi satın alımların alt toplamı. |
| Satış vergisi | Vergi tutarı. |
| Toplam | Ödenecek toplam miktar. |
