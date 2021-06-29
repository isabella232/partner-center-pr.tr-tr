---
title: Müşterileri geçerli Azure tekliflerinden Azure planına taşıma
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP iş ortaklarının mevcut CSP Azure tekliflerinden Azure İş Ortağı Merkezi Azure planı kapsamındaki Azure hizmetlerine müşteri taşımak için bu hizmetleri nasıl kullanabileceğini öğrenin.
author: mowree
ms.author: mowrim
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/16/2020
ms.openlocfilehash: 770df3cff40b8cc51eab16fb95d0bd43967a5a69
ms.sourcegitcommit: 3ac88f7925bfe1df90e267ee5c1ee4d752ac92d4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/29/2021
ms.locfileid: "113013276"
---
# <a name="transition-customers-to-azure-plan-from-existing-csp-azure-offers"></a>Müşterileri mevcut CSP Azure tekliflerinden Azure planına geçiş

**Için geçerlidir:** İş Ortağı Merkezi 

**Uygun roller:** Yönetici aracısı | Faturalama yöneticisi | Genel yönetici | Yardım masası aracısı | Satış aracısı | Kullanıcı yönetimi yöneticisi

Bu makalede, CSP iş ortaklarının mevcut CSP Azure tekliflerinden Azure İş Ortağı Merkezi Azure planı kapsamındaki Azure hizmetlerine müşteri taşımak için bu hizmetleri nasıl kullanabileceği açıklanmıştır. Dolaylı sağlayıcılar ve doğrudan fatura iş ortakları, Azure için Microsoft Bulut Hizmeti Sağlayıcısı Programı'nda (CSP) bulunan yeni ticaret deneyimine geçiş olabilir. (Dolaylı kurumsal bayilerin dolaylı sağlayıcıları üzerinden çalışması gerekir.) Müşterilerin iş ortaklarından, Microsoft satıcılarından veya doğrudan web'den satın alma gibi bulut hizmetlerini satın almak için kolaylaştırılmış bir yolu olacak.

Geçiş özelliği yalnızca Azure için yeni ticari deneyime geçiş yapan ve bu deneyimi imzalayan müşterilere Microsoft Müşteri Sözleşmesi. Bu, CSP'de Office 365 veya Dynamics 365 gibi diğer teklifler için değildir.

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>Mevcut CSP tekliflerini bir Azure planına geçiş

Bir müşteriyi mevcut CSP Azure tekliflerinden, CSP programı içindeki yeni ticaret deneyiminde Azure planı altındaki Azure hizmetlerine İş Ortağı Merkezi. Bunu yapmak için iş ortağının ve müşterinin İş Ortağı Merkezi kurumsal bayi ilişkisine sahip olması ve müşterinin Microsoft Müşteri Sözleşmesi.

### <a name="select-transition-to-azure-plan"></a>Azure planına geçişi seçme

1. Müşteriniz için Azure planı'ı seçin.

2. Faturalamayı **Azure planına geç'i seçin.**

   :::image type="content" source="images/azure/transition1.png" alt-text="Kullanım tabanlı abonelikler rapor bilgilerini şu şekilde adlandırılan seçilebilir bir seçenekle gösteren ekran görüntüsü: Azure aboneliği faturalamayı Azure planına geçiş.":::

3. **Devam**'ı seçin

   :::image type="content" source="images/azure/transition2.png" alt-text="Geçiş hakkında okumanın etkileri olan Azure planına geçiş başlıklı iletişim kutusu ve Devam veya İptal seçeneğinin işaret edildiği iki seçenek.":::

   Müşteriniz Azure planına geçişini sağlar.

   **Geçiş iş akışı, önkquisite adımlarını otomatik hale ekler:**

   - Azure planlarını satın alma
   - Doğrudan CSP senaryolarında müşteri başına bir plan  
   - Kurumsal bayi başına bir plan  

   Örneğin, bir iş ortağı iki farklı teklif Microsoft Azure satın aldı ve satın almada iki ayrı AYRı ÜÇ TÜR EKİP etti. Bu durumda, geçiş iş akışı iki Azure planı (bayi başına bir tane) satın alır ve ilgili Azure aboneliklerini Azure planları kapsamında otomatik olarak eşler.  

   **Azure aboneliğini Azure planıyla eşleme**

   Azure planlarınızı satın aldığınız zaman sistemimiz mevcut Azure aboneliklerini Azure planlarına eşler. İlerleme durumu hem iş Azure portal hem de İş Ortağı merkezi'nde view viewed.

4. Yerel para birimini kullanarak İş Ortağı Merkezi **limitini** güncelleştirmek için müşterinizin Abonelikler sayfasına geri gidin.

   :::image type="content" source="images/azure/transition3.png" alt-text="Faturalama dönemi İş Ortağı Merkezi yerel para birimi cinsinden ayarlanmış bütçe sınırlarına sahip Abonelikler sayfasının kısmi görünümü.":::

   >[!NOTE]
   >Bu kümede ayar İş Ortağı Merkezi bütçe, Azure portal. Ayrıca bütçeyi ve uyarıyı da Azure portal.

   Azure planına geçebilirsiniz, artık bu müşteri için Azure abonelikleri satın alaamazsınız. Abonelikleri Azure planı altında, abonelikler Azure portal.

   >[!NOTE]
   > Azure planı kapsamında RBAC aracılığıyla satın alınan tüm Azure abonelikleri yerel para birimiyle fiyatlandır ve faturalandırıldı. FX oranları kullanılmaz.

### <a name="track-your-transition-details"></a>Geçiş ayrıntılarınızı izleme

Hem Azure portal hem de İş Ortağı Merkezi.

:::image type="content" source="images/azure/details1.png" alt-text="Abonelik başına geçiş ayrıntılarının listesini içeren tabloyu gösteren ekran görüntüsü: Abonelik I D, geçiş tarihi ve geçiş durumu içerir.":::

### <a name="billing-impact-to-partners"></a>İş ortakları için faturalama etkisi

Mevcut CSP Azure teklifinden bir müşteriyi geçiştirersiniz, aşağıdaki faturalama etkileri olur:

- Özgün CSP Azure aboneliğini çıkış noktasına kadar olan tüm kullanımlar için mevcut CSP faturanız üzerinden faturalandırabilirsiniz.

- Mevcut CSP aboneliğine yönetici erişimi haklarınız varsa, bu abonelik geçirilirken erişiminiz olmaya devam edersiniz.

Doğrudan Kurumsal Anlaşmaları CSP ve Sunucu ve Bulut kayıtlarına Azure hizmetleri arasında geçiş yapmak için Azure aboneliklerinin fatura sahipliğini alma [makale Microsoft İş Ortağı Sözleşmesi](/azure/billing/mpa-request-ownership)

### <a name="audit-log"></a>Denetim günlüğü

Faturalamayı mu mutabakata varmak için Abonelikler sayfasında "Microsoft Azure" (0145P) abonelik **geçmişinizi** görüntüleyebilirsiniz.

"Microsoft Azure" (0145P) aboneliği iki bölümden oluşur:

1. Ticari abonelik
2. Azure aboneliği (yetkilendirme)

Geçiş tamamlandığında, Azure aboneliği yeni Azure planı altına taşınır ve ticari abonelik askıya alınır, böylece başka bir kullanım bildirgesi olmaz.  

>[!NOTE]
>CSP Microsoft Azure (0145P) aboneliği satın alınca hem ticari abonelik hem de Azure aboneliği (yetkilendirme) aynı değere sahip olur. Yalnızca faturalama sahipliği değişiklikleri veya aktarımları için değerler farklılık gösterir.

### <a name="transition-issues"></a>Geçiş sorunları

Geçişler sırasında herhangi bir sorun olacağını tahmin etmeyiz. Bir tane oluşursa, sizi geçiş iş akışının kendisinde güncelleştirin. Azure kullanımında bir sorun olmayacaktır.  

## <a name="next-steps"></a>Sonraki adımlar

- [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md)

- [İş ortağı tarafından kazanılan kredi - genel bakış](partner-earned-credit.md)
