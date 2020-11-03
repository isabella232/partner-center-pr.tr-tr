---
title: Faturanız & keşfi dosyanızı okuma
ms.topic: article
ms.date: 06/05/2020
description: Faturanızda & mutabakat dosyaları hakkında bilgi edinin. Faturanızda, bu aylık dönem için program, ürün ve müşteriler genelinde Iş Ortağı Merkezi ücretleri gösterilmektedir.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: edb2d25b49bd5c40dfd30e9f21d2d8537a5669c4
ms.sourcegitcommit: e1c8bea4aaf807aebe99c125cb1fb6dc8fdfa210
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/30/2020
ms.locfileid: "92531106"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>Faturanızı ve mutabakat dosyanızı anlayın-bunları Iş Ortağı Merkezi 'nde nasıl bulacağınızı öğrenin

**Uygulama hedefi**

- İş Ortağı Merkezi
- ABD kamu için Microsoft Bulut iş ortağı Merkezi

**Uygun roller**

- Genel yönetici
- Faturalama yöneticisi
- Yönetim Aracısı


**Faturanızda** **tüm iş ortağı merkezi ücretlerinizin** (program, tüm ürünler ve tüm müşteriler) bir özeti yer alınmaktadır. 

## <a name="invoice-types"></a>Fatura türleri

Microsoft, lisans tabanlı ücretler (Office 365 gibi) ve kullanım tabanlı ücretler (Azure gibi) için bir fatura ve tek seferlik ücretler (Azure RI, Market veya Azure planı gibi) için ayrı bir fatura yayımlayacak.

Örneğin,  

**Senaryo 1 [tek para birimi]** : Iş ortağının 145P teklifi ve O365 lisansları için satın alma işlemleri vardır.  

- İş ortağı, hem O365 hem de Azure için ücretleri kapsayan bir fatura PDF 'si ve 2 mutabakatı dosyası alır (145p).  

**Senaryo 2 [tek para birimi]** : iş ortağı, 145p satın alımlarıyla bırlıkte Azure RI, Market ve/veya Azure planına yönelik satın alımları içerir

- İş ortağı bir fatura PDF 'si ve Azure ücretini kapsayan bir mutabakat dosyası alacak (145p). 

- İş ortağı başka bir fatura PDF 'sini ve Azure RI, Market, Azure planına ilişkin ücretleri kapsayan bir mutabakat dosyası alır. 

**Senaryo 3 [çoklu para birimi]** : Iş ortağı DKK 'de Azure RI ve EUR 'deki 145p satın alımlarıyla birlikte satın alma işlemleri içerir.

- İş ortağı, bir fatura PDF 'sini ve DKK ' de Azure RI ücretlerini kapsayan bir mutabakat dosyası alır. 

- İş ortağı, EUR 'deki Azure planına yönelik ücretleri kapsayan bir fatura PDF ve mutabakat dosyası alır. 

- İş ortağı, farklı bir fatura PDF 'si ve EUR (veya iş ortağı faturalandırma para birimi) ile 145p teklifi için ücretleri kapsayan bir mutabakat dosyası alır. 

## <a name="find-your-bill"></a>Faturanızı bulun 

Faturanızı, Iş Ortağı Merkezi ' nde panonun faturalama sayfasında bulabilirsiniz. Bu sayfada faturalandırma geçmişinizi, harcama eğilimlerini ve mutabakatı dosyalarını da bulabilirsiniz. 

1. Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard/home)oturum açın. 

2. Sol taraftaki menüde **faturalandırma** ' i seçin. 

3. Faturalama sayfasında, indirmek istediğiniz faturayı seçin. 

En son faturanızda bir bağlantıyı, son fatura tarihinden itibaren hesap bakiyesi altında sayfanın en üstünde bulabilirsiniz. 

Önceki faturaları faturalandırma geçmişi bölümünde bulabilirsiniz. Uygun yılı seçin ve ardından uygun fatura döneminin yanındaki aşağı açılan oku seçin. Bu dönemin faturasını indirmek için faturalar (. PDF) yanındaki bağlantıyı seçin. 

## <a name="understanding-invoice-pdf"></a>Fatura PDF 'sini anlama 

**Kullanım ve lisans tabanlı ücretler Için faturalar** : Office 365 ve Azure gibi hizmetlerin ücretlerine yönelik faturalar, seçtiğiniz faturalandırma tarihinin iki (2) günü IÇINDE (UTC]) kullanılabilir.  

**Kerelik ve tekrarlayan ücretler için faturalar** : Azure RI, Azure planı, Market gibi hizmetlere yönelik ücretlere yönelik faturalar, her ayın 8 ' inden daha geç bir şekilde kullanıma sunulacaktır.  

Aşağıda, fatura PDF belgesinde önemli alanlardan bazıları verilmiştir:

**Fatura numarası** : ilgili fatura dönemi için oluşturulan fatura belgesi için benzersiz tanımlayıcı. 

**Fatura dönemi** : Bu, kullanımlarının ve lisans tabanlı hizmetlerin bulunduğu dönemdir. 

**Fatura tarihi** : faturalandırınızın her ay oluşturulduğu faturalandırma tarihi veya yıldönümü tarihi. 

**Ödeme bitiş tarihi** : ödemenizin alınması gereken tarih. 

**Ücretler** : ilgili fatura dönemi için faturalandırma para biriminiz ödenmesi gereken miktar. 

**Jenerik** : KREDILERIN (SLA gibi) veya Aboneliklerde yapılan değişikliklere yönelik ayarlamalar (örneğin, lisans artar veya azalır). 

**Ödeme yönergeleri** : bölgenize göre faturanızı nasıl ödeymeyle ilgili açıklama. Ödeme yaparken her zaman fatura numaranızı eklediğinizden emin olun. 

Fatura dosyanızdaki tüm alanların ayrıntılı bir açıklaması için (tek seferlik ücretler için alanlar dahil), bkz. [fatura dosyası alanları](invoice-file.md). 

## <a name="understand-reconciliation-files"></a>Karşılaştırma dosyalarını anlama

 Ücretlerinizin ayrıntılarına inmek/listelenen ayrıntılarını sağlayan mutabakat dosyaları, fatura PDF 'siyle birlikte indirilebilir. Mutabakat dosyaları müşteri tanımlayıcıları ve müşteri faturaları oluşturmak için kullanabileceğiniz abonelik tanımlayıcılarını içerir. Lütfen keşfi dosyaları hakkında daha fazla bilgi edinmek için  [bkz. karşılaştırma dosyalarını kullanma](use-the-reconciliation-files.md) . 
