---
title: Power BI için Iş Ortağı Merkezi analizlerini kullanma
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Power BI için Partner Center Analytics uygulamasını kullanarak iş verilerinizi görüntülemeyi öğrenin (CSP 'deki doğrudan iş ortakları için).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f5bdb166562593b970f40c23921dc80b2a1cb8ad
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633873"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a>İş verilerinizi Microsoft için Partner Center Analytics uygulaması ile görüntüleyin Power BI



**Uygun roller**

- Genel yönetici
- Kullanıcı Yönetimi Yöneticisi
- Satış Aracısı
- Yönetim Aracısı

## <a name="view-your-business-data"></a>İş verilerinizi görüntüleyin

Aşağıdakiler de dahil olmak üzere, Power BI için Partner Center Analytics uygulaması ile iş verilerinizin görsel bir temsilini alın:

- Müşteri tabanınız, abonelikleriniz ve lisanslarınızın büyümesi

- Office 365, Microsoft Dynamics ve Microsoft Azure ürünlerinin kullanımı

- Son 60 güne ait her bir Azure aboneliğinde ölçülen her kaynak için günlük tüketim birimleri

- Tahmini maliyet (en son fiyat kartına göre)

- Veri kümelerini dışarı aktarma ve müşteri başına dahil özel raporlar oluşturma özelliği.

### <a name="about-the-partner-center-analytics-app-preview-release"></a>Iş ortağı merkezi analizi uygulama Önizleme sürümü hakkında

- Bu uygulama yalnızca bulut çözüm sağlayıcısı programındaki doğrudan iş ortakları içindir. CSP 'deki diğer iş ortakları (örneğin, dolaylı satıcılar) oturum açamaz.

- Tüm tahmini maliyetler ön vergi faturalandırma/fatura verileri olduğundan, yasal olmayan bir şekilde bağlanmamalıdır. Tahmini maliyetlerin yalnızca veri öngörüleri için kullanılması amaçlanmıştır.

- Müşteri bilgileri, abonelikleri temel alır. Son zamanlarda hesap oluşturduğunuz, ancak henüz abonelikleri olmayan müşteriler, sayımlar halinde dahil değildir.

- Tahmini maliyet, CSP fiyatlandırmasını temel alan en son fiyat kartını temel alır.

- Gün sayısı takvim gündür.

### <a name="business-insights-report"></a>İş öngörüleri raporu

- **Müşteri kiracılar**: abonelikleri satın almış olan müşterilerin farklı Azure AD kiracılarının sayısı

- **Yeni (son 30 gün)**: son 30 gün içinde en az bir abonelik satın alan yeni müşteriler

- **Karmaşıklık (son 30 gün)**: "etkin", "yetkisiz kullanım" veya "devre dışı" abonelikler olmadan müşteriler

- **Yeni (son 24 saat)**: son 24 saat içinde en az bir abonelik satın alan yeni müşteriler

- **Son 12 ay Içinde tahmini aylık maliyet**: aylık aylık, son 12 ay boyunca aylık olarak toplanan tahmini vergi öncesi fatura doları tutarının aylık eğilimi

- **Son 12 ay içinde ürüne göre tahmini maliyet**: satılan ürünler, son 12 ay süresince toplanan tahmini vergi öncesi fatura doları tutarına göre sıralanır. Bu durum, en fazla gelir getiren en popüler ürünleri gösterir.

- **Son 12 ay Içindeki müşteriler**: aylık son 12 ay boyunca aylık olarak toplanan yeni müşteriler ve değişim müşterilerinin aylık ayı eğilimi

- **Son 12 ay boyunca müşteriye göre tahmini maliyet**: müşteriler, son 12 ay süresince toplanan tahmini vergi öncesi fatura dolar tutarına göre sıralanır. Bu durum, en çok gelir getiren popüler müşterileri gösterir.

- **Ürüne göre müşteri sayısı**: satılan ürünler, ilişkili müşterilere göre sıralanır. Bu durum, çoğu müşteriye satılan en popüler ürünleri gösterir.

### <a name="subscription-insights-report"></a>Abonelik öngörüleri raporu

- **Abonelik durumu**:

- Etkin: "etkin" ya da "yetkisiz kullanım" durumuna ait abonelikler

  - Askıya alındı: "devre dışı" durumuna ait abonelikler

  - Serbest sağlanmış: "önceden sağlanmış" veya "süre sonu" durumuna ait abonelikler

- **Süre sonu durumu**:

  - Süresi geçti: süresi zaten geçmiş abonelikler (abonelik bitiş tarihi geçmiş)

  - 30 gün sonra süresi doluyor: 30 gün sonra süresi dolacak abonelikler (abonelik bitiş tarihi sonraki 30 gün sonra olduğunda)

  - 30 gün içinde süresi doluyor: sonraki 30 gün içinde süresi dolacak abonelikler (abonelik bitiş tarihi bugün ve sonraki 30 gün arasındadır)

- **Toplam abonelikler**: "etkin", "yetkisiz kullanım" veya "devre dışı" durumundaki abonelikler

- **Yeni (son 30 gün)**: son 30 gün içinde müşteriler tarafından satın alınan yeni abonelikler

- **Yeni (son 24 saat)**: son 24 saat içinde müşteriler tarafından satın alınan yeni abonelikler

- **30 gün Içinde süresi doluyor**: sonraki 30 gün içinde süresi dolacak abonelikler

- **Dalgalanma (son 30 gün)**: son 30 gün içinde zaten sağlanmış veya askıya alınmış (devre dışı) abonelikler

- **Abonelik türlerine göre dağıtım**: Toplam aboneliklerin lisans tabanlı ve kullanım tabanlı abonelik türüne göre dağılımı

- **Ürüne göre etkin abonelik sayısı**: satılan ürünler, etkin abonelik sayısına göre sıralanır

- **Son** 12 aya ait abonelikler: son 12 ay boyunca aylık olarak toplanan yeni aboneliklerin ve değişim aboneliklerinin ayda ayı eğilimi

- **Müşteri aboneliği ayrıntıları**: müşterilerin, aboneliklerin ve tekliflerin ayrıntılı görünümü

### <a name="license-insights-report"></a>Lisans öngörüleri raporu:

- **Toplam** lisans sayısı: lisans tabanlı tüm abonelikler genelinde toplanan toplam lisans sayısı

- **Yeni (son 30 gün)**: son 30 gün içinde lisans ekleme

- **Karmaşıklık (son 30 gün)**: son 30 gün içinde lisans azaltma

- **Yeni (son 24 saat)**: son 24 saat içinde lisans ekleme

- **Son 90 gün Içindeki lisanslar**: son 90 günün süresi boyunca aylık olarak toplanan lisans eklemeleri ve indirimlerinin ayda ayı eğilimi

- **Ürüne göre etkin lisans sayısı**: satılan ürünler, etkin lisans sayısına göre sıralanır

- **Müşteriye göre etkin lisans sayısı**: müşteriler etkin lisans sayısına göre sıralanır

- **Son 90 gün Içindeki müşteri lisans olay ayrıntıları**: olay tarihi, olay adı, miktar ve miktar değişikliği dahil olmak üzere müşteriler, abonelikler ve abonelik olaylarının ayrıntılı görünümü.

### <a name="licenses-usage-report"></a>Lisans kullanım raporu:

- **Ürüne göre atanan lisanslar**: lisans atama sayısına göre sıralanan ürünler

- **Ürün tarafından kullanılan lisanslar**: lisans kullanım sayısına göre sıralanan ürünler

- **Atanan lisansların müşteri dağılımı**:% %20 ' nin %20 ' si için lisans ataması ile toplam müşterilerin dağılımı

- **Kullanımdaki lisansların müşteri dağılımı**: %20 ' nin lisans kullanımına göre %20 aralığında bozuk toplam müşterilerin dağılımı%

- **Müşteri tarafından atanan lisanslar**: satılan lisansların ayrıntılı görünümü ve müşteriler ve ürünler tarafından atanan lisanslar

- **Müşteri tarafından kullanılan lisanslar**: müşteriler ve ürünler tarafından kullanılan lisansların ve lisansların ayrıntılı görünümü

### <a name="azure-insights-report"></a>Azure Insights raporu:

- **Son 12 ay Içinde kullanım tabanlı müşteriler**: son 12 ay boyunca aylık olarak toplanan yeni kullanım tabanlı müşterilerin aylık ayı eğilimi ve tek başına kullanılan kullanım tabanlı müşteriler

- **Son 12 aya göre kullanım tabanlı abonelikler**: son 12 ay boyunca aylık olarak toplanan yeni kullanım tabanlı aboneliklerin ve tek başına kullanılan kullanım tabanlı aboneliklerin aya göre ayı eğilimi

- **Son 60 gün içinde müşterinin tahmin edilen kullanım maliyeti**: Kullanım tabanlı müşteriler, son 60 günün dönemi boyunca toplanan tahmini vergi öncesi fatura doları tutarına göre sıralanır. Bu durum, en çok geliri getiren en popüler kullanım tabanlı müşterileri gösterir

- **Son 60 gün içinde kategoriye göre tahmini kullanım maliyeti**: Kullanım tabanlı aboneliklerin ölçüm kategorileri, son 60 günün dönemi boyunca toplanan tahmini vergi öncesi fatura dolar tutarına göre sıralanır.

- **Son 60 gün içinde abonelik tarafından tahmini kullanım maliyeti**: son 60 günün dönemi boyunca toplanan tahmini vergi öncesi fatura doları tutarına göre kullanım tabanlı abonelikler.

- **Bütçe harcamasına göre müşterinin tahmini kullanım maliyeti**: müşteriler, geçerli kullanım harcama bütçesi yüzdesine göre sıralanır (%100%).

### <a name="azure-resource-usage-report"></a>Azure Kaynak kullanımı raporu:

- **Seçili dönem için güne göre Azure kaynakları kullanımı**: son 60 gün içindeki seçili dönem için her bir kullanım tabanlı abonelikte her bir ölçülen kaynak için günlük tüketim birimleri.

- **Seçili dönem Için Azure kaynaklarının tahmini kullanım maliyeti**: son 60 gün içindeki seçili dönem için her bir kullanım tabanlı abonelikte her bir ölçülen kaynak için en son fiyat kartına göre tahmini maliyet. 

## <a name="next-steps"></a>Sonraki adımlar

- [Power BI uygulamasına genel bakış için iş ortağı merkezi analizi](power-bi-app-for-direct-partners.md)

- [Microsoft Power BI için İş Ortağı Merkezi Analizi uygulamasını yükleme ve önizleme](power-bi-app-for-direct-partners-install.md)
