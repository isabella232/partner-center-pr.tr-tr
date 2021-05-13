---
title: İş Ortağı Merkezi Analytics'i Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Power BI için İş Ortağı Merkezi Analiz uygulaması kullanarak iş verilerinizi görüntülemeyi öğrenin (CSP'de doğrudan iş ortakları için).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 96fe57f6e89928a69051c2e201c444882500b844
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855038"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Microsoft Power BI için İş Ortağı Merkezi Analytics uygulamasıyla iş verilerinizi Power BI



**Uygun roller:** Genel yönetici | Kullanıcı yönetimi yönetici | Satış aracısı | Yönetici aracısı

## <a name="view-your-business-data"></a>İş verilerinizi görüntüleme

Aşağıdakiler dahil olmak üzere iş verilerinizin görsel bir Power BI için İş Ortağı Merkezi Analiz uygulaması elde elde Power BI için İş Ortağı Merkezi Analiz uygulaması:

- Müşteri tabanınızı, aboneliklerinizi ve lisanslarınızı büyüme

- Office 365, Microsoft Dynamics ve Microsoft Azure kullanımı

- Son 60 gün boyunca her Azure aboneliğinde tarifeli her kaynağın günlük tüketim birimleri

- Tahmini maliyet (en son fiyat kartına göre)

- Müşteri başına dahil olmak üzere veri kümelerini dışarı aktarma ve özel raporlar oluşturma olanağı.

### <a name="about-the-partner-center-analytics-app-preview-release"></a>İş Ortağı Merkezi Analytics uygulaması önizleme sürümü hakkında

- Bu uygulama, yalnızca Bulut Çözümü Sağlayıcısı iş ortaklarına yöneliktir. CSP'de (örneğin dolaylı kurumsal bayiler) diğer iş ortakları oturum açmayacak.

- Tahmini maliyetler vergi öncesi faturalama/fatura verileridir ve yasal olarak bağlayıcı değildir. Tahmini maliyetler yalnızca veri içgörüleri için kullanılır.

- Müşteri bilgileri abonelikleri temel alan bilgilerdir. Kısa süre önce hesap oluşturduğunuz ancak henüz abonelikleri olmayan müşteriler sayılara dahil değildir.

- Tahmini maliyet, CSP fiyatlandırması temel alınan en son fiyat kartına göredir.

- Günler takvim günleridir.

### <a name="business-insights-report"></a>Business Insights raporu

- **Müşteri kiracıları:** Abonelik satın alan müşterilerin farklı Azure AD kiracılarının sayısı

- **Yeni (son 30 gün)**: Son 30 gün içinde en az bir abonelik satın alan yeni müşteriler

- **Churn (son 30 gün):**"etkin", "yetkisiz kullanım" veya "devre dışı" abonelikleri olmayan müşteriler

- **Yeni (son 24 saat)**: Son 24 saat içinde en az bir abonelik satın alan yeni müşteriler

- **Son 12 aya** göre tahmini aylık maliyet: Son 12 aylık dönemde aylık olarak toplanan tahmini vergi öncesi fatura dolar tutarı eğilimi

- **Son 12 aya** göre tahmini ürün maliyeti: Satılan ürünler, son 12 aylık dönemde toplanmış tahmini vergi öncesi fatura dolar tutarına göre sıralanmış. Bu durum en çok gelir getiren ürünleri gösterir.

- **Son 12** ay boyunca müşteriler: Son 12 aylık dönemde aylık olarak toplanan yeni müşterilerin ve veri düşüşlerinin aylara göre eğilimi

- **Son 12 ay** içinde müşteriye göre tahmini maliyet: Müşteriler, son 12 aylık dönemde toplanan tahmini vergi öncesi fatura dolar tutarına göre sıralanmış. Bu durum, en çok gelir elde edilen müşterilerin olduğunu gösterir.

- **Ürüne göre müşteri sayısı:** Satılan ürünler ilişkili müşterilere göre sıralanmış. Bu durum, müşterilerin çoğuna en çok satılan ürünleri gösterir.

### <a name="subscription-insights-report"></a>Subscription Insights raporu

- **Abonelik durumu:**

- Etkin: "etkin" veya "yetkisiz kullanım" durumuna sahip abonelikler

  - Askıya alındı: "devre dışı" duruma ait abonelikler

  - Sağlamayı geri alındı: "sağlamayı geri alındı" veya "süresi doldu" durumuna ait abonelikler

- **Süre sonu durumu:**

  - Süresi Doldu: Süresi dolmuş abonelikler (aboneliğin bitiş tarihi geçmiştir)

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

- **Harcama bütçesine göre müşteri tahmini** kullanım maliyeti: Müşteriler, geçerli kullanım harcaması bütçesinin eşiğini (%100) aşan yüzdesine göre sıralanmış.

### <a name="azure-resource-usage-report"></a>Azure Kaynak Kullanımı raporu:

- **Azure kaynaklarının seçilen dönem** için güne göre kullanımı: Son 60 gün içindeki seçili dönem için her kullanım tabanlı abonelikte tarifeli her kaynak için günlük tüketim birimleri.

- **Seçilen dönem için Azure** kaynaklarının tahmini kullanım maliyeti: Son 60 gün içindeki belirli bir dönem için her kullanım tabanlı abonelikte tarifeli her kaynağın en son fiyat kartına göre tahmini maliyet. 

## <a name="next-steps"></a>Sonraki adımlar

- [İş Ortağı Merkezi için Power BI Analytics'e genel bakış](power-bi-app-for-direct-partners.md)

- [Microsoft Power BI için İş Ortağı Merkezi Analizi uygulamasını yükleme ve önizleme](power-bi-app-for-direct-partners-install.md)
