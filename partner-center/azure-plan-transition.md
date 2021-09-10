---
title: Müşterileri geçerli Azure tekliflerden Azure planına taşıyın
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: CSP iş ortaklarının, müşterileri mevcut CSP Azure tekliflerden Azure planı kapsamındaki Azure hizmetlerine taşımak için Iş Ortağı Merkezi 'ni nasıl kullanabileceğinizi öğrenin.
author: mowree
ms.author: mowrim
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/16/2020
ms.openlocfilehash: eb9d88935bdc339c01ac47153c3d4a23047dc406
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960014"
---
# <a name="transition-customers-to-azure-plan-from-existing-csp-azure-offers"></a>Mevcut CSP Azure tekliflerden müşterilerin Azure planına geçiş yapın

**Uygulama hedefi**: Iş Ortağı Merkezi 

**Uygun roller**: yönetici Aracısı | Faturalandırma Yöneticisi | Genel yönetici | Yardım Masası Aracısı | Satış Aracısı | Kullanıcı Yönetimi Yöneticisi

Bu makalede, CSP iş ortaklarının, müşterileri mevcut CSP Azure tekliflerden Azure planı kapsamındaki Azure hizmetlerine taşımak için Iş Ortağı Merkezi 'ni nasıl kullanabileceği açıklanmaktadır. Dolaylı sağlayıcılar ve doğrudan fatura ortakları, Azure için Microsoft Bulut Service Provider programında (CSP) bulunan yeni ticari deneyime geçiş yapabilir. (Dolaylı satıcıların dolaylı sağlayıcıları aracılığıyla çalışması gerekir.) Müşteriler, iş ortakları, Microsoft satıcıları veya doğrudan Web üzerinden satın alma, bulut hizmetleri satın almak için kolaylaştırılmış bir yönteme sahip olacaktır.

Geçiş özelliği yalnızca Azure 'a yönelik yeni ticari deneyim ve Microsoft Müşteri anlaşmasını imzalayan müşteriler içindir. CSP 'deki Office 365 veya Dynamics 365 gibi diğer tekliflere yönelik değildir.

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>Mevcut CSP tekliflerinin bir Azure planına geçişini sağlar

Mevcut CSP Azure tekliflerinden bir müşteriyi, Iş Ortağı Merkezi ' nden CSP programındaki yeni ticaret deneyiminde Azure planı kapsamındaki Azure Hizmetleri ' ne getirebilirsiniz. Bunu yapmak için iş ortağı ve müşterinin Iş Ortağı Merkezi aracılığıyla kurulu bir satıcı ilişkisi olması ve müşterinin Microsoft Müşteri anlaşmasını imzalamış olması gerekir.

### <a name="select-transition-to-azure-plan"></a>Azure planına geçişi seçin

1. Müşteriniz için Azure planı ' nı seçin.

2. **Azure planına geçiş faturalandırma**' i seçin.

   :::image type="content" source="images/azure/transition1.png" alt-text="Kullanım tabanlı abonelikler rapor bilgilerini, seçilebilir bir seçenekle gösteren ekran görüntüsü: Azure aboneliği ile Azure planına geçiş geçişi.":::

3. **Devam**'ı seçin

   :::image type="content" source="images/azure/transition2.png" alt-text="Azure planına geçiş başlıklı iletişim kutusu, geçiş ve seçme, devam etme veya Iptal etme için iki seçenek hakkında bilgi edinin.":::

   Müşteriniz Azure planına geçirilir.

   **Geçiş iş akışı, önkoşul adımlarını otomatik hale getirir**:

   - Azure planı satın alma
   - Doğrudan CSP senaryolarında müşteri başına bir plan  
   - Satıcı başına bir plan  

   bir örnek için, bir iş ortağı iki Microsoft Azure teklifi satın almış ve satın alma sırasında iki ayrı por içerir. Bu durumda, geçiş iş akışı iki Azure planı (satıcı başına bir tane) satın alacak ve Azure planlarındaki ilgili Azure aboneliklerini otomatik olarak eşleyebilir.  

   **Azure aboneliğini Azure planına eşleme**

   Azure planı satın aldıktan sonra sistemimiz mevcut Azure aboneliklerini Azure planlarına eşleyebilir. İlerleme, Iş Ortağı Merkezi 'nin yanı sıra Azure portal de görüntülenebilir.

4. Kendi yerel para birimini kullanarak bütçe limitini güncelleştirmek için müşterinizin Iş Ortağı Merkezi **abonelikleri** sayfasına dönün.

   :::image type="content" source="images/azure/transition3.png" alt-text="Bir fatura dönemi için yerel para biriminde ayarlanan bütçe limitleriyle Iş Ortağı Merkezi abonelikleri sayfasının kısmi görünümü.":::

   >[!NOTE]
   >Iş Ortağı Merkezi 'nde ayarladığınız bütçe Azure portal üzerinden taşınmaz. Ayrıca, Azure portal de bütçesini ve uyarıyı ayarlamanız gerekir.

   Azure planına geçtiğinizde, artık bu müşteri için Azure abonelikleri satın alınmaz. Abonelikleri Azure portal Azure planı altında oluşturursunuz.

   >[!NOTE]
   > Azure planı kapsamındaki RBAC aracılığıyla satın alınan tüm Azure abonelikleri, yerel para birimiyle fiyatlandırılır ve faturalandırılır. FX ücretleri kullanılmaz.

### <a name="track-your-transition-details"></a>Geçiş ayrıntılarınızı izleyin

Azure portal ve Iş Ortağı Merkezi 'nde geçiş ilerlemesini izleyin.

:::image type="content" source="images/azure/details1.png" alt-text="Abonelik başına geçiş ayrıntıları listesinin bulunduğu tabloyu gösteren ekran görüntüsü-abonelik ı D, geçiş tarihi ve geçiş durumu içerir.":::

### <a name="billing-impact-to-partners"></a>İş ortaklarına faturalandırma etkisi

Bir müşteriyi mevcut bir CSP Azure teklifinden geçirirsiniz, aşağıdaki faturalandırma etkileri olur:

- Özgün CSP Azure aboneliğinden çıkma noktasına kadar tüm kullanımlar için mevcut CSP faturanızda faturalandırılırsınız.

- Mevcut CSP aboneliğine yönetici erişimi haklarınız varsa, bu abonelik geçirildiğinde erişime sahip olmaya devam edersiniz.

doğrudan Enterprise sözleşmelerini CSP 'ye ve sunucu ve bulut kayıtlarına azure hizmetlerine geçirme için, [Microsoft iş ortağı sözleşmesi için azure aboneliklerinin fatura sahipliğini alma](/azure/billing/mpa-request-ownership) konusunu okuyun.

### <a name="audit-log"></a>Denetim günlüğü

faturalandırmayı mutabık kılmak için **abonelikler** sayfasında "Microsoft Azure" (0145p) aboneliklerinizin geçmişini görüntüleyin.

"Microsoft Azure" (0145p) abonelik iki bölümden oluşur:

1. Ticari abonelik
2. Azure aboneliği (yetkilendirme)

Geçiş tamamlandığında, Azure aboneliği yeni Azure planı altına taşınır ve daha fazla kullanım raporlanmayacak şekilde ticari abonelik askıya alınır.  

>[!NOTE]
>CSP 'de Microsoft Azure (0145p) aboneliği satın alındığında hem ticari abonelik hem de Azure aboneliği (yetkilendirme) aynı değere sahiptir. Yalnızca faturalandırma sahipliği değişiklikleri veya aktarımları söz konusu olduğunda değerler farklılık gösterir.

### <a name="transition-issues"></a>Geçiş sorunları

Geçiş sırasında herhangi bir sorunu tahmin etmedik. Bir durum oluşursa, sizi geçiş iş akışının kendisinde güncelleştireceğiz. Azure kullanımına yönelik bir sorun olmayacaktır.  

## <a name="next-steps"></a>Sonraki adımlar

- [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)

- [İş ortağı kazanılmış kredi-genel bakış](partner-earned-credit.md)
