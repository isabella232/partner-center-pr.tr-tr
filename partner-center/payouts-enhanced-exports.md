---
title: Ödemelerin verileri dışarı aktarma sayfası
description: Özelleştirilmiş işlem geçmişi raporları oluşturmak için gelişmiş dışarı aktarma verileri sayfasının nasıl kullanılası açıklandı
author: Satinder37
ms.author: sabajaj
ms.topic: how-to
ms.date: 10/04/2021
ms.custom: template-how-to
ms.openlocfilehash: 9ac19a8ea42020b4ec2543d9f4ef197eb95e3a61
ms.sourcegitcommit: cf8c78e0c8831371432007d5ab05f934f15a77b5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/05/2021
ms.locfileid: "129528673"
---
# <a name="payouts-export-data-page"></a>Ödemelerin verileri dışarı aktarma sayfası
**Uygun roller:** Teşvik yöneticisi | Teşvikler kullanıcısı

Bu makalede, İş Ortağı Merkezi'de Ödemelerin veri **dışarı aktarma deneyiminde** yapılan geliştirmeler ele İş Ortağı Merkezi. Bu kılavuzlu deneyim, işlem geçmişi raporlarınızı dışarı aktarmaya için yeni varsayılan şablonlar sağlar. Ayrıca, işlem geçmişi raporlarınız için kendi özelleştirilmiş şablonlarınızı oluşturmanızı sağlamak için dinamik bir özelliğe sahiptir.

## <a name="access-the-export-data-page"></a>Verileri dışarı aktarma sayfasına erişme
1.  [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/home) oturum açın.
2.  **Ödemeler'i ve** ardından **menüden Teşvik dışarı** **aktarma'ya veya İşlem geçmişi'ne** tıklayın.

> [!Note] 
> Teşvik yöneticisi veya teşvik kullanıcısıysanız bu [sayfaya erişebilirsiniz.](/payout-statement#roles-and-permissionsData) Göreceğiniz, erişiminiz olan program ve Microsoft İş Ortağı Ağı (MPN) birleşimlerine (İşlem geçmişi  ve Ödeme sayfalarına benzer) **bağlıdır.**

## <a name="export-your-data"></a>Verilerinizi dışa aktarma
1.   Dışarı aktarmayı istediğiniz veri türünü seçin. 
      - bir işlem geçmişi raporu için Kazanç, **işlem, ödeme durumu ayrıntıları'ı seçin.**  Kazanç, **işlem, ödeme durumu ayrıntıları (büyüme kaldıraçları)** ticari marketler için geçerli değildir. 
      - Ödeme raporu için Ödeme **ayrıntıları'ı seçin.**
   :::image type="content" source="images/payouts/type-of-data.png" lightbox="images/payouts/type-of-data.png" alt-text="Veri seçimlerinin türünü gösteren ekran görüntüsü.":::

2.   Bir rapor şablonu türü seçin.

      :::image type="content" source="images/payouts/report-template-type.png" lightbox="images/payouts/report-template-type.png" alt-text="Rapor şablonu türü seçimlerini gösteren ekran görüntüsü.":::

      1. adım için seçiminiz, 2. adım için şablon seçeneklerinizi belirler. Örneğin, 1. **adımda Kazanç, işlem ve** ödeme durumu ayrıntılarını seçmeniz durumunda dört farklı şablon seçeneğiyle karşına gelirsiniz:
      - **Varsayılan işlem geçmişi:** Bu rapor, raporda tüm programlarda (teşvikler, ticari ve tüketici marketleri) kullanılabilen tüm olası öznitelikleri gösterir. Bu, Ekim 2021'den önce kullanılabilen indirme şablonudur.
      - **Varsayılan pazar yeri:** Bu rapor, ticari market programlarına kayıtlı MPN üyeleri için gereken tüm öznitelikleri (örneğin, Azure Market. 
      - **Varsayılan depo:** Bu rapor, Microsoft Store, Minecraft ve MS Flight Simulator gibi tüketici deposu programlarına kayıtlı MPN üyeleri için gereken tüm öznitelikleri gösterir. 
      - **Özel işlem geçmişi:** Bu rapor, işlem geçmişi raporlarınızı özelleştirmenize olanak sağlar.

      1. **adımda Kazanç, işlem,** ödeme durumu ayrıntılarını seçerse 2. adımda İşlem **özeti** şablonunu seçebilirsiniz. 1. **adımda** Ödeme ayrıntıları'nın seçerek 2. adımda bir "Ödemeler" şablonuyla karşına çıktı. 1. **adımda AGI** geliri ayrıntılarını seçerseniz Program geliri  veya Müşteri 2. adımda **şablon** ekler arasında seçim yapmak mümkün olur.

3. Bir rapor dosyası biçimi seçin.
   
      :::image type="content" source="images/payouts/report-file-format.png" lightbox="images/payouts/report-file-format.png" alt-text="Rapor dosyası biçimi seçimlerini gösteren ekran görüntüsü.":::

4.   Zaman döneminizi seçin ve diğer filtreleri uygulayın ve ardından Verileri **indir'i seçin.**
   
      :::image type="content" source="images/payouts/time-period-filters.png" lightbox="images/payouts/time-period-filters.png" alt-text="Rapor zaman dönemi seçimini ve filtre seçeneğini gösteren ekran görüntüsü.":::

> [!Note] 
> İndirme istekleri tablosundan verileri dışarı aktarabilirsiniz **ve istekleri yönetebilirsiniz.**

## <a name="create-your-customized-transaction-history-report"></a>Özelleştirilmiş işlem geçmişi raporlarınızı oluşturma

İşlem geçmişi mutabakat raporlarınızı ihtiyaçlarınıza uyacak şekilde özelleştirin. En fazla beş rapor şablonu oluşturabilir ve yönetebilirsiniz. 

1.  Yeni **mutabakat şablonu ayarlamak için +** Özel işlem geçmişi'ne seçin. 
   
      :::image type="content" source="images/payouts/custom-trans-history.png" lightbox="images/payouts/custom-trans-history.png" alt-text="Özel işlem geçmişi kurulumunu gösteren ekran görüntüsü.":::


2.   Bir şablon adı ve kısa bir açıklama girin ve ardından Sonraki'yi **seçin.**
   
      :::image type="content" source="images/payouts/template-name.png" lightbox="images/payouts/template-name.png" alt-text="Yeni özel mutabakat şablonu alanlarını gösteren ekran görüntüsü.":::


3.  Dahil etmek istediğiniz veri sütunlarını seçin ve raporda zaten listelenen varsayılan sütunları gözden geçirebilirsiniz. **İleri**’yi seçin.
   
     :::image type="content" source="images/payouts/data-selection.png" lightbox="images/payouts/data-selection.png" alt-text="Yeni özel mutabakat şablonu veri seçimi seçeneklerini gösteren ekran görüntüsü.":::

4.  Şablon ayrıntılarınızı ve veri seçimlerinizi gözden geçirin, gerekirse düzenlemeler yapın ve özel şablon **oluştur'a tıklayın.**
   
      :::image type="content" source="images/payouts/new-custom-template.png" lightbox="images/payouts/new-custom-template.png" alt-text="Yeni özel mutabakat şablonunun onay ekran görüntüsünü gösteren ekran görüntüsü.":::

5.  Verilerinizi **dışarı aktarmanız** için sonraki ekrandan İndir'i seçin. Ayrıca bu ekrandan başka şablonlar ekleyebilir, düzenleyebilir, indirebilir veya silebilirsiniz.
   
      :::image type="content" source="images/payouts/download-manage-templates.png" lightbox="images/payouts/download-manage-templates.png" alt-text="Şablonları yönetme ve veri indirme seçeneklerini gösteren ekran görüntüsü.":::

## <a name="next-steps"></a>Sonraki adımlar
- [Ödemelere genel bakış](non-payment-fraud-misuse.md)
- [Gelir özeti](revenue-summary.md)
- [Ödeme deyimleri](payout-statement.md)
- [Ödeme ve vergiler hakkında sık sorulan sorular](payout-faq.yml)
