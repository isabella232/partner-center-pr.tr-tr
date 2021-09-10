---
title: İş Ortağı Merkezi Analytics'i Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Power BI için İş Ortağı Merkezi Analiz uygulaması (CSP) programında doğrudan iş ortakları için) kullanarak iş Bulut Çözümü Sağlayıcısı görüntülemeyi öğrenin.
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eea221af22e9bd7aa684bc5120b0799f083f8663
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961344"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Microsoft Power BI için İş Ortağı Merkezi Analytics uygulamasıyla iş verilerinizi Power BI



**Uygun roller:** Genel yönetici | Kullanıcı yönetimi yönetici | Satış aracısı | Yönetici aracısı

## <a name="view-your-business-data"></a>İş verilerinizi görüntüleme

Aşağıdakiler dahil olmak üzere Microsoft İş Ortağı Merkezi Analytics uygulamasıyla iş verilerinizin görsel Power BI elde edin:

- Müşteri tabanınızı, aboneliklerinizi ve lisanslarınızı büyüme

- Office 365, Microsoft Dynamics ve Microsoft Azure kullanımı

- Son 60 gün boyunca her Azure aboneliğinde tarifeli her kaynağın günlük tüketim birimleri

- Tahmini maliyet (en son fiyat kartına göre)

- Müşteri başına dahil olmak üzere veri kümelerini dışarı aktarma ve özel raporlar oluşturma olanağı.

### <a name="about-the-partner-center-analytics-app-preview-release"></a>İş Ortağı Merkezi Analytics uygulaması önizleme sürümü hakkında

- Bu uygulama yalnızca Bulut Çözümü Sağlayıcısı (CSP) programında doğrudan iş ortaklarına yöneliktir. CSP'de (örneğin dolaylı kurumsal bayiler) diğer iş ortakları oturum açmayacak.

- Tahmini maliyetler vergi öncesi faturalama/fatura verileridir ve yasal olarak bağlayıcı değildir. Tahmini maliyetler yalnızca veri içgörüleri için kullanılır.

- Müşteri bilgileri abonelikleri temel alan bilgilerdir. Kısa süre önce hesap oluşturduğunuz ancak henüz abonelikleri olmayan müşteriler sayılara dahil değildir.

- Tahmini maliyet, CSP fiyatlandırması temel alınan en son fiyat kartına göredir.

- Günler takvim günleridir.

### <a name="business-insights-report"></a>İş Analizler raporu

- **Müşteri kiracıları:** Abonelik satın Azure Active Directory müşterilerin farklı kiracı (Azure AD) kiracılarının sayısı

- **Yeni (son 30 gün)**: Son 30 gün içinde en az bir abonelik satın alan yeni müşteriler

- **Churn (son 30 gün):**"etkin", "yetkisiz kullanım" veya "devre dışı" abonelikleri olmayan müşteriler

- **Yeni (son 24 saat)**: Son 24 saat içinde en az bir abonelik satın alan yeni müşteriler

- **Son 12 aya** göre tahmini aylık maliyet: Son 12 aylık dönemde aylık olarak toplanan tahmini vergi öncesi fatura dolar tutarının aylık eğilimi

- **Son 12 aya** göre tahmini ürün maliyeti: Satılan ürünler, son 12 aylık dönemde toplanmış tahmini vergi öncesi fatura dolar tutarına göre sıralanmış. Bu durum en çok gelir getiren ürünleri gösterir.

- **Son 12** ay boyunca müşteriler: Son 12 aylık dönemde aylık olarak toplanan yeni müşterilerin ve veri düşüşlerinin aylara göre eğilimi

- **Son 12 ay** içinde müşteriye göre tahmini maliyet: Müşteriler, son 12 aylık dönemde toplanan tahmini vergi öncesi fatura dolar tutarına göre sıralanmış. Bu durum, en çok gelir elde edilen müşterilerin olduğunu gösterir.

- **Ürüne göre müşteri sayısı:** Satılan ürünler ilişkili müşterilere göre sıralanmış. Bu durum, müşterilerin çoğuna en çok satılan ürünleri gösterir.

### <a name="subscription-insights-report"></a>Abonelik Analizler raporu

- **Abonelik durumu:**

- Etkin: "etkin" veya "yetkisiz" durumda olan abonelikler

  - Askıya alındı: "devre dışı" duruma ait abonelikler

  - Sağlamayı geri alındı: "sağlamayı geri alındı" veya "süresi doldu" durumuna ait abonelikler

- **Süre sonu durumu:**

  - Süresi Doldu: Süresi dolmuş abonelikler (aboneliğin bitiş tarihi geçmiştir)

  - 30 gün sonra sona erer: 30 gün sonra süresi dolacak abonelikler (abonelik bitiş tarihi sonraki 30 gün sonra olur)

  - 30 gün içinde süre sonu: Sonraki 30 gün içinde süresi dolacak abonelikler (aboneliğin bitiş tarihi bugün ile sonraki 30 gün arasında)

- **Toplam abonelik** sayısı: "etkin", "yetkisiz kullanım durumunda" veya "devre dışı" durumdaki abonelikler

- **Yeni (son 30 gün)**: Son 30 gün içinde müşteriler tarafından satın alınan yeni abonelikler

- **Yeni (son 24 saat)**: Son 24 saat içinde müşteriler tarafından satın alınan yeni abonelikler

- **30 gün içinde sona erer:** Sonraki 30 gün içinde süresi dolacak abonelikler

- **Churn (son 30 gün)**: Son 30 gün içinde sağlanan veya askıya alınmış (devre dışı) abonelikler

- **Abonelik türlerine göre dağıtım:** Lisans tabanlı ve kullanım tabanlı abonelik türüne göre toplam aboneliklerin dağılımının %

- **Ürüne göre etkin abonelik sayısı:** Satılan ürünler, etkin abonelik sayısına göre sıralanmış

- **Son 12 aya** göre abonelikler: Son 12 aylık dönemde aylık olarak toplanan yeni aboneliklerin ve churn aboneliklerinin aylara göre eğilimi

- **Müşteri aboneliği ayrıntıları:** Müşterilerin, aboneliklerin ve tekliflerin ayrıntılı görünümü

### <a name="license-insights-report"></a>Lisans Analizler raporu:

- **Toplam lisans sayısı:** Tüm lisans tabanlı aboneliklerde toplam lisans sayısı

- **Yeni (son 30 gün)**: Son 30 gün içinde lisans ekleme

- **Churn (son 30 gün)**: Son 30 gün içinde lisans azaltma

- **Yeni (son 24 saat)**: Son 24 saat içinde lisans ekleme

- **Son 90** gün içinde lisanslar: Son 90 gün içinde aylık olarak toplanan lisans ekleme ve azaltmalarının aylara göre eğilimi

- **Ürüne göre etkin lisans sayısı:** Satılan ürünler etkin lisans sayısına göre sıralanmış

- **Müşteriye göre etkin lisans sayısı:** Etkin lisans sayısına göre sıralanmış müşteriler

- **Son 90 gün** içinde müşteri lisans olayı ayrıntıları: Olay tarihi, olay adı, miktar ve miktar değişikliği dahil olmak üzere müşterilerin, aboneliklerin ve abonelik olaylarının ayrıntılı görünümü.

### <a name="licenses-usage-report"></a>Lisans Kullanımı raporu:

- **Ürüne göre atanan lisanslar:** Satılan ürünler lisans atama sayısına göre sıralanmış

- **Ürüne göre kullanım lisansları:** Satılan ürünler lisans kullanım sayısına göre sıralanmış

- **Atanan lisansların müşteri dağılımı:** Toplam müşterilerin %20'lik aralıkta lisans ataması % aralığına göre dağılımı

- **Kullanımdaki lisansların müşteri dağılımı:** Toplam müşterilerin %20'lik aralıkta lisans kullanımına göre dağılımı %

- **Müşteri tarafından atanan lisanslar:** Satılan lisansların ve müşteriler ve ürünler tarafından atanan lisansların ayrıntılı görünümü

- **Müşteri tarafından kullanımda olan lisanslar:** Müşteriler ve ürünler tarafından satılan lisansların ve kullanım lisanslarının ayrıntılı görünümü

### <a name="azure-insights-report"></a>Azure Analizler raporu:

- **Son 12** ay içinde kullanım tabanlı müşteriler: Son 12 aylık dönemde aylık olarak toplanan yeni kullanım tabanlı müşterilerin ve kullanım tabanlı müşterilerin aylık eğilimi

- **Son 12** ay içinde kullanım tabanlı abonelikler: Son 12 aylık dönemde aylık olarak toplanan yeni kullanım tabanlı aboneliklerin ve kullanım tabanlı aboneliklerin aylık eğilimi

- **Son 60** gün içinde müşteriye göre tahmini kullanım maliyeti: Kullanım tabanlı müşteriler, son 60 gün içinde toplanan tahmini vergi öncesi fatura dolar tutarına göre sıralanmış. Bu durum, en fazla gelir elde edilen kullanım tabanlı müşterileri gösterir

- **Son 60** gün içinde kategoriye göre tahmini kullanım maliyeti: Kullanım tabanlı aboneliklerin ölçüm kategorileri, son 60 günlük dönemde toplanan tahmini vergi öncesi fatura dolar tutarına göre sıralanmış.

- **Son 60 gün** içinde aboneliğe göre tahmini kullanım maliyeti: Son 60 gün içinde toplanan tahmini vergi öncesi fatura dolar tutarına göre kullanım tabanlı abonelikler.

- **Harcama bütçesine göre müşteri tahmini** kullanım maliyeti: Müşteriler, geçerli kullanım harcaması bütçesinin eşiğini (%100) aşan yüzdesine göre sıralanmış.

### <a name="azure-resource-usage-report"></a>Azure Kaynak Kullanımı raporu:

- **Azure kaynaklarının seçilen dönem** için güne göre kullanımı: Son 60 gün içindeki seçili dönem için her kullanım tabanlı abonelikte tarifeli her kaynak için günlük tüketim birimleri.

- **Seçilen dönem için Azure** kaynaklarının tahmini kullanım maliyeti: Son 60 gün içindeki belirli bir dönem için her kullanım tabanlı abonelikte tarifeli her kaynağın en son fiyat kartına göre tahmini maliyet. 

## <a name="next-steps"></a>Sonraki adımlar

- [İş Ortağı Merkezi için Power BI Analytics'e genel bakış](power-bi-app-for-direct-partners.md)

- [Microsoft Power BI için İş Ortağı Merkezi Analizi uygulamasını yükleme ve önizleme](power-bi-app-for-direct-partners-install.md)
