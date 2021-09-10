---
title: Masaüstü sayısını ve ücret düzeyini bulma
ms.topic: how-to
ms.date: 02/18/2021
description: Bir sözleşmenin masaüstü sayısını ve ücret düzeyini bulmak için kanal teşvikleri platformunu (yonga) nasıl kullanacağınızı öğrenin.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 288e4ebb224d3ff1b0d4050691b733e678ec29a3
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961255"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>Bir sözleşmenin masaüstü cihaz sayısını ve ücret düzeyini bulma

**Uygun roller**: birincil iletişim veya Program Yöneticisi

Sözleşmeyi gözden geçirmek için [Explore.MS](https://www.explore.ms/) 'de oturum açabilir veya Masaüstü sayısı ile ücret düzeyi için anlaşma ayrıntılarını sağlayan bir dosyayı indirebilirsiniz.

## <a name="to-locate-the-information"></a>Bilgileri bulmak için

### <a name="method-1--explorems"></a>Yöntem 1 – Explore.ms

1. Internet Explorer 'da [Explore.MS](https://www.explore.ms/) 'yi açın. 

>[!Note]
>Bu işlevi Google Chrome veya Microsoft Edge gerçekleştiremezsiniz.

2. Iş/okul hesabınızla veya canlı KIMLIĞINIZ ile oturum açın.  

3. **Raporlar** alanında **anlaşmalar**' ı seçin.

4. Sonuç sayfasında, **arama** alanına anlaşma numarasını girin ve ardından **Sütunları Seç/Sırala**' yı seçin.

5. Açılır pencerede, kullanılabilir sütunlar listesinden **anlaşma Masaüstü sayısı** ' nı seçin ve ardından sütunu eklemek için sağ oku seçin. **Tamam**’ı seçin.

6. Ara ' yı seçin **.**

7. Elde edilen ekranda, **sözleşme Masaüstü sayısı** sütununu bulmak için sonuçların içinde ilerleyin. 

8. Aşağıdaki fiyat tablosuna göre ücret düzeyini öğrenmek için masaüstü sayısını kullanın.  

| Ücret düzeyi | Masaüstü sayısı |
| ------ | :-----------: |
|  A | 0 – 2.399    |
|  B | 2.400 – 5.999    |
|  C | 6.000 – 14.999    |
|  D | 15000 +   |

>[!NOTE]
>Enterprise Bu düzeyler, ticari ve kamu sektörü (PS) kayıtları 'nda masaüstü veya kullanıcı sayısını (hangisi daha yüksektir) temel alır. Doğal ilişkili masaüstü veya Kullanıcı sayısı olmayan kayıtlar için, Microsoft, eşlik eden EA 'nın masaüstü sayısını veya kullanıcı sayısını temel alan bir masaüstü sayısı uygular. <br><br>Eşlik eden bir EA yoksa, ücret düzeyi kaydın fiyatlandırma düzeyine dayanır. [Www.explore.MS](https://www.explore.ms/)' de, anlaşma fiyatlandırma düzeyi de görüntülenebilir. <br><br>Mevcut EA/EAS üzerinde birden fazla havuz ve/veya fiyatlandırma düzeyi varsa, Microsoft, en yüksek ve en düşük düzey olan D düzeyi olacak şekilde teşvikleri, en yüksek fiyatlandırma/havuz düzeyinde ödeme yapar.

#### <a name="pool-and-pricing-levels"></a>Havuz ve fiyatlandırma düzeyleri

Yukarıda özetlenen adımları kullanarak explore.ms içindeki anlaşma numarasını aradıktan sonra anlaşma numarasını seçin. Bu işlem sizi sözleşme ayrıntıları sayfasına götürür ve bu, **sözleşme özetini** ve **tekliflerini** gösterecektir. Teklifler bölümü Fiyatlandırma düzeylerini içerir.

## <a name="method-2---chip"></a>Yöntem 2-yonga

1. YONGASıNDA oturum açın ve LSP teşvikleri ' ı seçin.

2. **Iş ortağı ödeme Özeti** sayfasında, görüntülemek istediğiniz raporlama ayını seçin ve ardından **Excel için dışarı aktar**' ın altındaki açılır listeden **Hesaplama ayrıntıları** ' nı seçin:

:::image type="content" source="images/chip/chiplocate.png" alt-text="Program ayrıntılarını bulun.":::

3. Dışarı aktarma başlar ve dosyayı açabilir veya bir hedefe kaydedebilir/kaydedebilirsiniz.

4. Rapor açık olduğunda, sol alt kısımdaki **DetailReport-Yataydosya** sekmesine gidin:

:::image type="content" source="images/chip/flatfile.png" alt-text="Düz dosya indirme.":::

Artık J sütununda aradığınız sözleşme numarasını arayabilirsiniz. Agreement_DesktopCount etiketli, atanan masaüstü sayısını R sütununda bulabilirsiniz. Ayrıca, bu sözleşmenin, katman etiketli ' AI ' sütununda bu sözleşmenin ücret düzeyini de doğrulayabilirsiniz.

## <a name="next-steps"></a>Sonraki adımlar

- [YONGA erişimi sorunlarını giderme](chip-access-trouble.md)
