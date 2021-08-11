---
title: Masaüstü sayısını ve ücret düzeyini bulma
ms.topic: how-to
ms.date: 02/18/2021
description: Bir sözleşmenin masaüstü sayısı ve ücret düzeyi bilgilerini bulmak için Channel Incentives platformunu (CHIP) kullanmayı öğrenin.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c2ae28bd6291af9c4a4445dcc4010b817e533c34b339b137b67ae1a99b5f4e2c
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115692796"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>Bir sözleşmenin masaüstü cihaz sayısını ve ücret düzeyini bulma

**Uygun roller:** Birincil kişi veya program yöneticisi

Sözleşmeyi gözden geçirmek [için explore.ms](https://www.explore.ms/) oturum açabilirsiniz veya masaüstü sayısı ve ücret düzeyi için sözleşme ayrıntılarını sağlayan bir dosya indirebilirsiniz.

## <a name="to-locate-the-information"></a>Bilgileri bulmak için

### <a name="method-1--explorems"></a>Yöntem 1 – Explore.ms

1. [Explore.ms'de](https://www.explore.ms/) Internet Explorer. 

>[!Note]
>Bu işlevi Google Chrome veya Microsoft Edge.

2. İş/Okul hesabınızla veya canlı kimliğinizle oturum açın.  

3. Raporlar **alanında** Sözleşmeler'i **seçin.**

4. Sonuçta elde edilen sayfada, Arama alanına sözleşme numarasını **girin** ve ardından Sütunları **Seç/SiparişLe'yi seçin.**

5. Açılan pencerede, kullanılabilir sütunlar **listesinden Sözleşme Masaüstü** Sayısı'na tıklayın ve ardından sütunu eklemek için sağ oku seçin. **Tamam**’ı seçin.

6. **Ara'ya seçin.**

7. Sonuçta elde edilen ekranda, Sözleşme Masaüstü Sayısı sütununu bulmak için **sonuçlarda ilerleyin.** 

8. Aşağıdaki fiyat tablosuna göre ücret düzeyini belirlemek için masaüstü sayısını kullanın.  

| Ücret düzeyi | Masaüstü sayısı |
| ------ | :-----------: |
|  A | 0 – 2,399    |
|  B | 2,400 – 5,999    |
|  C | 6,000 – 14,999    |
|  D | 15,000+   |

>[!NOTE]
>Enterprise Teşvik düzeyleri, Ticari ve Kamu Sektörü (PS) kayıtlarında masaüstü veya kullanıcı sayısına (hangisi daha yüksekse) göredir. Doğal olarak ilişkili masaüstü veya kullanıcı sayısına sahip kayıtlarda Microsoft, eşlik eden EA'nın masaüstü sayısına veya kullanıcı sayısına göre bir masaüstü sayısı uygular. <br><br>Eşlik eden EA yoksa Ücret Düzeyi, kaydın fiyatlandırma düzeyine göredir. Anlaşmanın fiyatlandırma düzeyi, [www.explore.ms.](https://www.explore.ms/) <br><br>Mevcut EA/EAS üzerinde birden çok havuz ve/veya fiyatlandırma düzeyi varsa, Microsoft teşvikleri en yüksek atanan fiyatlandırma/havuz düzeyinde, A düzeyi ise en düşük ve D düzeyi en yüksek düzeyde öder.

#### <a name="pool-and-pricing-levels"></a>Havuz ve Fiyatlandırma Düzeyleri

Yukarıda açıklanan adımları kullanarak explore.ms numarasını arayarak anlaşma numarasını seçin. Bu sizi Sözleşme Özeti ve Teklifleri'nin göster olduğu **sözleşme ayrıntıları** **sayfasına alır.** Teklifler bölümünde fiyatlandırma düzeyleri yer almaktadır.

## <a name="method-2---chip"></a>Yöntem 2 - CHIP

1. CHIP'de oturum açma ve LSP Teşvikleri'ne kaydolma.

2. İş Ortağı **Ödeme Özeti sayfasında** görüntülemek istediğiniz raporlama ayını  seçin ve ardından Dışarı Aktar altındaki Açılan listeden Hesaplama Ayrıntıları'Excel: 

:::image type="content" source="images/chip/chiplocate.png" alt-text="Program ayrıntılarını bulun.":::

3. Dışarı aktarma başlar ve dosyayı açabilir veya bir hedefe kaydedebilir/kaydedebilirsiniz.

4. Rapor açıkken sol alttaki **DetailReport-FlatFile** sekmesine gidin:

:::image type="content" source="images/chip/flatfile.png" alt-text="Düz dosya indirme.":::

Artık J sütununda istediğiniz sözleşme numarasını arayabilirsiniz. Atanan masaüstü sayısını R sütununda ve bu sütunda Agreement_DesktopCount. Bu sözleşmenin Ücret Düzeyini Katman olarak etiketlenmiş 'AI' sütununda da onaylayın.

## <a name="next-steps"></a>Sonraki adımlar

- [CHIP erişim sorunlarını giderme](chip-access-trouble.md)
