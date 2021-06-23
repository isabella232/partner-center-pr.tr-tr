---
title: Mutabakat dosyası için faturanızı & okuma
ms.topic: article
ms.date: 06/05/2020
description: Mutabakat dosyalarınız hakkında & öğrenin. Faturanız, İş Ortağı Merkezi dönem boyunca program, ürünler ve müşteriler için geçerli olan ücretleri gösterir.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bbdf85d20e15841189191d6b415b54c26378850e
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551206"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>Faturanızı ve mutabakat dosyanızı anlama - bunları nasıl bu İş Ortağı Merkezi


**Uygun roller:** Genel yönetici | Faturalama yöneticisi | Yönetici aracısı


**Faturanız,** tüm **fatura ücretlerinizin İş Ortağı Merkezi** (program genelinde, tüm ürünler ve tüm müşteriler) özetini içerir. 

## <a name="find-your-bill-and-reconciliation-file"></a>Fatura ve mutabakat dosyanızı bulma 

Faturanızı panonun Faturalama sayfasında bulabilirsiniz İş Ortağı Merkezi. Bu sayfada faturalama geçmişinizi, harcama eğilimlerinizi ve mutabakat dosyalarınızı da bulabilirsiniz. 

1. İş Ortağı Merkezi [oturum açın.](https://partner.microsoft.com/dashboard/home) 

2. Sol menüde Faturalama'ya **tıklayın.** 

3. Faturalama durumu sayfasında daha ayrıntılı bilgi görüntülemek için bir fatura veya mutabakat dosyası seçin. 

Sayfanın en üstünde son fatura tarihine göre Hesap bakiyesi'nin altında en son faturanıza bir bağlantı bulabilirsiniz. 

Önceki faturaları Faturalama geçmişi bölümünde bulabilirsiniz. Uygun yılı seçin ve ardından uygun Faturalama döneminin yanındaki açılan oku seçin. Dönemin faturasını indirmek için Faturalar (.pdf) öğesinin yanındaki bağlantıyı seçin. 

## <a name="invoice-types"></a>Fatura türleri

Microsoft tüm lisans tabanlı ücretler (Office 365 gibi) ve kullanım tabanlı ücretler (Azure gibi) için bir fatura ve tek kullanımlık ücretler (Azure RI, Market veya Azure planı gibi) için ayrı bir fatura sunar.

Örneğin,  

**Senaryo 1 [Tek Para Birimi]**: İş ortağının 145P teklifi ve Office 365 lisansları için satın almaları vardır,  

- İş ortağı hem Office 365 hem de Azure (145p) ücretleri kapsayan bir fatura PDF dosyası ve iki mutabakat dosyası alır.  

**Senaryo 2 [Tek Para Birimi]**: İş ortağının 145p satın alma ile birlikte Azure RI, Market ve/veya Azure planı için satın almaları vardır.

- İş ortağı, Azure ücretlerini kapsayan bir fatura PDF dosyası ve bir mutabakat dosyası (145p) alır. 

- İş ortağı, Azure ayrılmış örneği (RI), Market ve Azure planı ücretlerini kapsayan başka bir fatura PDF dosyası ve bir mutabakat dosyası alır. 

**Senaryo 3 [Çok** Para Birimi] : İş ortağının DKK'de Azure RI için satın almaları ve EUR cinsinden Azure planı ile EUR cinsinden 145p satın almaları vardır.

- İş ortağı, DKK'de Azure RI ücretlerini kapsayan bir fatura PDF ve bir mutabakat dosyası alır. 

- İş ortağı, EUR olarak Azure planı ücretlerini kapsayan bir fatura PDF dosyası ve bir mutabakat dosyası alır. 

- İş ortağı, 145p teklife (veya iş ortağı faturalama para birimine) yönelik ücretlerini kapsayan başka bir fatura PDF dosyası ve bir mutabakat dosyası alır. 


## <a name="understanding-invoice-pdf"></a>Fatura PDF'lerini anlama 

**Kullanım faturaları ve lisans** tabanlı ücretler: Office 365 ve Azure gibi hizmetlerin ücretlerine göre faturalar, seçtiğiniz faturalama tarihini [UTC] takip etmeden itibaren iki (2) gün içinde kullanılabilir.  

**Bir kezlik ve yinelenen** ücretler için faturalar: Azure RI, Azure planı, Market gibi hizmetlerin ücretlerine göre faturalar her ayın sekizden sonra kullanılamaz.  

Fatura PDF belgesinde yer alan önemli alanlardan bazıları aşağıda verilmiştir:

**Fatura numarası:** İlgili faturalama dönemi için oluşturulan fatura belgesinin benzersiz tanımlayıcısı. 

**Faturalama dönemi:** Bu süre, kullanım ve lisans tabanlı hizmetlere sahip olduğunuz dönemdir. 

**Fatura tarihi:** Faturanın her ay oluşturulacak faturalama tarihi veya yıldönümü tarihi. 

**Ödeme son tarihi:** Ödemenizin alın aldığı tarih. 

**Ücretler:** İlgili faturalama dönemi için faturalama para biriminize bağlı olan tutar. 

**Krediler:** Krediler (hizmet düzeyi sözleşmesi (SLA) gibi) veya aboneliklerde yapılan değişikliklere (örneğin, lisans artışları veya düşüşleri) yönelik düzeltmeler. 

**Ödeme yönergeleri:** Bölgenize göre faturanızı ödemenin açıklaması. Ödeme yaparken her zaman fatura numaranızı dahil etmek için emin olun. 

Fatura dosyanız (tek defalık ücretlere ilişkin alanlar dahil) tüm alanların ayrıntılı açıklaması için [bkz. Fatura dosyası alanları.](invoice-file.md) 

## <a name="understand-reconciliation-files"></a>Mutabakat dosyalarını anlama

 Ücretlerinizin detaya gitme/öğe ayrıntılarını sağlayan mutabakat dosyaları, Fatura PDF'sine ek olarak indirilebilir. Mutabakat dosyaları müşteri faturalarını oluşturmak için kullanabileceğiniz müşteri tanımlayıcılarını ve abonelik tanımlayıcılarını içerir. Mutabakat dosyaları hakkında daha fazla bilgi için [bkz. Mutabakat dosyalarını kullanma.](use-the-reconciliation-files.md) 

## <a name="next-steps"></a>Sonraki adımlar

- [Mutabakat dosyalarını kullanma](use-the-reconciliation-files.md)