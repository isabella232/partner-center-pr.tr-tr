---
title: Faturanız & keşfi dosyanızı okuma
ms.topic: article
ms.date: 06/05/2020
description: Faturanızda & mutabakat dosyaları hakkında bilgi edinin. Faturanızda, bu aylık dönem için program, ürün ve müşteriler genelinde Iş Ortağı Merkezi ücretleri gösterilmektedir.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 839f6f76e7efde4f0ad51375ceb5801f925c2510
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961054"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>Faturanızı ve mutabakat dosyanızı anlayın-bunları Iş Ortağı Merkezi 'nde nasıl bulacağınızı öğrenin


**Uygun roller**: genel yönetici | Faturalandırma Yöneticisi | Yönetim Aracısı


**Faturanızda** **tüm iş ortağı merkezi ücretlerinizin** (program, tüm ürünler ve tüm müşteriler) bir özeti yer alınmaktadır. 

## <a name="find-your-bill-and-reconciliation-file"></a>Faturanızı ve mutabakat dosyanızı bulun 

Faturanızı, Iş Ortağı Merkezi ' nde panonun faturalama sayfasında bulabilirsiniz. Bu sayfada faturalandırma geçmişinizi, harcama eğilimlerini ve mutabakatı dosyalarını da bulabilirsiniz. 

1. Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard/home)oturum açın. 

2. Sol taraftaki menüde **faturalandırma**' i seçin. 

3. Faturalama durumu sayfasında daha ayrıntılı bilgi görüntülemek için bir fatura veya mutabakat dosyası seçin. 

En son faturanızda bir bağlantıyı, son fatura tarihinden itibaren hesap bakiyesi altında sayfanın en üstünde bulabilirsiniz. 

Önceki faturaları faturalandırma geçmişi bölümünde bulabilirsiniz. Uygun yılı seçin ve ardından uygun fatura döneminin yanındaki aşağı açılan oku seçin. Bu dönemin faturasını indirmek için faturalar ' ın yanındaki bağlantıyı (.pdf) seçin. 

## <a name="invoice-types"></a>Fatura türleri

Microsoft, lisans tabanlı ücretler (Office 365 gibi) ve kullanım tabanlı ücretler (azure gibi) için bir fatura ve tek seferlik ücretler (azure rı, market veya azure planı gibi) için ayrı bir fatura yayımlayacak.

Örneğin,  

**senaryo 1 [tek para birimi]**: iş ortağının 145p teklifi ve Office 365 lisansları için satın alma işlemleri vardır.  

- iş ortağı, hem Office 365 hem de Azure (145p) ile ilgili ücretleri kapsayan bir fatura PDF 'si ve iki mutabakat dosyası alır.  

**Senaryo 2 [tek para birimi]**: iş ortağı, 145p satın alımlarıyla bırlıkte Azure RI, Market ve/veya Azure planına yönelik satın alımları içerir

- İş ortağı bir fatura PDF 'si ve Azure ücretlerini kapsayan tek bir mutabakat dosyası alır (145p). 

- İş ortağı, Azure ayrılmış örneği (RI), Market, Azure planına ait ücretleri kapsayan başka bir fatura PDF ve bir mutabakat dosyası alır. 

**Senaryo 3 [çoklu para birimi]**: Iş ortağı DKK 'de Azure RI ve EUR 'deki 145p satın alımlarıyla birlikte satın alma işlemleri içerir.

- İş ortağı, DKK içindeki Azure RI ücretlerini kapsayan bir fatura PDF ve tek bir mutabakat dosyası alır. 

- İş ortağı, EUR 'deki Azure planına yönelik ücretleri kapsayan bir fatura PDF ve tek bir mutabakat dosyası alır. 

- İş ortağı başka bir fatura PDF 'si ve bir mutabakat dosyası alırlar (veya iş ortağı faturalandırma para birimi) 145p teklifi ücretini kapsayan bir 


## <a name="understanding-invoice-pdf"></a>Fatura PDF 'sini anlama 

**kullanım ve lisans tabanlı ücretler için faturalar**: Office 365 ve Azure gibi hizmetlerin ücretlerine yönelik faturalar, seçtiğiniz faturalandırma tarihinin iki (2) günü içinde (UTC]) kullanılabilir.  

**Kerelik ve tekrarlayan ücretler için faturalar**: Azure RI, Azure planı, Market gibi hizmetler için ücretlerle ilgili faturaların her ayın sekizinci ' inden daha sonra yer alacak.  

Aşağıda, fatura PDF belgesinde önemli alanlardan bazıları verilmiştir:

**Fatura numarası**: ilgili fatura dönemi için oluşturulan fatura belgesi için benzersiz tanımlayıcı. 

**Fatura dönemi**: Bu, kullanımlarının ve lisans tabanlı hizmetlerin bulunduğu dönemdir. 

**Fatura tarihi**: faturalandırınızın her ay oluşturulduğu faturalandırma tarihi veya yıldönümü tarihi. 

**Ödeme bitiş tarihi**: ödemenizin alınması gereken tarih. 

**Ücretler**: ilgili fatura dönemi için faturalandırma para biriminiz ödenmesi gereken miktar. 

**Jenerik**: kredi (hizmet düzeyi SÖZLEŞMESI (SLA) gibi) veya Aboneliklerde yapılan değişikliklere yönelik ayarlamalar (örneğin, lisans artışları veya azalmaları). 

**Ödeme yönergeleri**: bölgenize göre faturanızı nasıl ödeymeyle ilgili açıklama. Ödeme yaparken her zaman fatura numaranızı eklediğinizden emin olun. 

Fatura dosyanızdaki tüm alanların ayrıntılı bir açıklaması için (tek seferlik ücretler için alanlar dahil), bkz. [fatura dosyası alanları](invoice-file.md). 

## <a name="understand-reconciliation-files"></a>Karşılaştırma dosyalarını anlama

 Ücretlerinizin detaya gitme/ayrıntılı ayrıntılarını sağlayan mutabakat dosyaları, fatura PDF 'siyle birlikte indirilebilir. Mutabakat dosyaları müşteri tanımlayıcıları ve müşteri faturaları oluşturmak için kullanabileceğiniz abonelik tanımlayıcılarını içerir. Karşılaştırma dosyaları hakkında daha fazla bilgi için bkz. [karşılaştırma dosyalarını kullanma](use-the-reconciliation-files.md). 

## <a name="next-steps"></a>Sonraki adımlar

- [Karşılaştırma dosyalarını kullanma](use-the-reconciliation-files.md)