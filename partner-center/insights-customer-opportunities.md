---
title: iş ortağı merkezi Analizler-cloudadscent eğilimini raporları
description: Iş Ortağı Merkezi 'nde Cloudadscent eğilimini raporları hakkında bilgi edinin. Microsoft ürünlerini satın almak için bir müşterinin eğilimini hakkında bilgiler içerir.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 14e0ceb931a5eb58dcbab480617e093ebc36df43
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129070867"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>Cloudadscent eğilimini raporları Iş Ortağı Merkezi panosundan kullanılabilir

**Uygun roller**: Executive rapor Görüntüleyici | Rapor Görüntüleyicisi

Iş Ortağı Merkezi panosu, Cloudadscent programından indirilebilir eğilimini verileri sağlar. Veriler, müşterilerin Microsoft ürünlerini satın alma olasılığını gösterir.  Bu makalede bu verilerin dökümü, Puanlama kullanımı ve ne anlama geldiğini açıklanmaktadır.

## <a name="summary-definitions"></a>Özet tanımları

- **SMC müşterileri**: Bu, eğilimini indirmelerinde bulunan toplam müşteri sayısıdır.  Müşteriler, kayıt ortağı tarafından tanımlanır.
- **Süresi dolan anlaşmalar**: geçerli mali yıl içinde, süresi dolan sözleşmelerin sayısını sağlıyoruz.
- **Süresi dolan gelir**: açık süresi dolan anlaşmalarla ilişkili gelir.

:::image type="content" source="images/insights/customer-opportunity-1.png" alt-text="Müşteriler fırsatlar Özet Panosu ekran görüntüsü.":::

## <a name="cloudascent-smb-segmentation"></a>Cloudadtik SMB kesimlemesi

Küçük ve orta ölçekli iş (SMB) segmenti üç farklı alt parçaya bölünür.

1. **En Iyi yönetilmeyen** , Microsoft için en çok fırsat olan en büyük SMB müşterilerini içerir. Tipik En Iyi yönetilmeyen müşteriler benzer özellikleri, çok sayıda çalışan, büyük BT bütçeleri ve harcama ve Microsoft için büyük miktarda potansiyel gelir ile yönetilen hesaplara paylaşır.

   En üst yönetilmeyen olarak iki şekilde tanımlanır:

   - **Üst yönetilmeyen Kullanıcı tabanlı**– 300 veya daha fazla çalışan hesapları içerir. User-Based hesapları, Microsoft 365, Dynamics 365 veya yüzey gibi kullanıcı tabanlı abonelik ürünlerinin ilk kez satın alınması veya genişletilmesi için harika hedeflerdir.
   - **Üst yönetilmeyen Işlem tabanlı** – Azure, $10.000 ' den büyük olan hesapları içerir. İşlem tabanlı hesaplar var olan Azure 'ı içerir. daha önce Azure satın alma, ancak Azure 'un en fazla $10.000 ' den büyük olması gereken önemli gelecek yıl potansiyeli hesaplar.

2. **Orta ölçekli işletmeler** , 25 ila 300 çalışanı olan mevcut müşterileri ve aday hesap hesaplarını içerir.

3. **Küçük işletmeler** , 10-25 çalışanı olan işletmeler içerir.

4. **Çok küçük işletmeler** , 1-9 çalışanı olan işletmeler içerir.

:::image type="content" source="images/insights/customer-opportunity-2.png" alt-text="Müşteri, SMC türüne göre.":::

**En Iyi yönetilmeyen** ve **Orta ölçekli iş** alt kesimleri, Microsoft ve Microsoft iş ortakları için yüksek yaşam süresi değeri (LTV) müşterilerini temsil eder. Bu nedenle, bu kesimde büyüme için odaklanabilecek öncü alanlardır. bu iki alt kesimde, yuvayı Microsoft 365, D365/Azure iş kolu (LOB) uygulamaları ile daha iyi bir şekilde almak ve Microsoft için yüksek bir ktv hakkında daha iyi konumlandırılıyoruz.

Bugün, 1. fırsat için iki temel alan sunuyoruz. müşterimiz büyüme ekliyor; iki. bulut yuvalarını Microsoft 365 önde edindiğimiz için, Dynamics 365 ve Azure 'da büyük bir fırsattır.

Aşağıdaki ekran görüntüsünde dört SMB alt bölümü temsil eder. Cloudadtik, tüm üst yönetilmeyen ve orta ölçekli Iş hesaplarının profil oluşturma, Puanlama ve modellemesini önceliklendirmez.

:::image type="content" source="images/insights/customer-opportunity-3.png" alt-text="SMB alt kesimlerinin ekran görüntüsü.":::

## <a name="cloudascent-machine-learning"></a>Cloudadsent Machine Learning

SMB, en üst yönetilmeyen ve orta ölçekli Iş segmentlerinde satış ve pazarlama müşteri tahminlerini yönlendirmek için makine öğrenimi teknolojisini kullanır. Sinyaller nasıl toplanır ve eğilimini önerilere nasıl etkinleştirilir?

- **Veri toplama**: web gezginleri şirket etki alanlarını ve blog yayınlarını izleyerek, yayınlar, sosyal akışlar ve teknik Forumlar ' e basarak milyarlarca müşteri sinyalleri tarar ve toplar.  Toplanan sinyallere ek olarak, firmograf bilgileri, D&B, Microsoft Iç aboneliği ve işlem verileri gibi iç ve dış kaynaklardan toplanır.

- **Machine Learning**: sinyaller, bulut ürünü ve kümesi tarafından her müşteri için yapılandırılmış veri satış ve pazarlama tahminleri kümesini veren makine öğrenimi modeline dağıtılır.  Her müşteri, Microsoft 'un müşterinin sığdırmasını belirleyen ve müşterinin çevrimiçi davranışını tümleştiren makine öğrenimi algoritmalarının amaç olarak tanımladıkları, benzer bir model ile Microsoft 'un en üst SMB 'sini kullanarak puanlanır. Puanlama, Microsoft Bulut ürünlerini satın almak için müşterinin eğilimini gösteren kümeler halinde birleştirilir.

- **iyileştirme**: Machine Learning sistemi işlem verilerini aylık ve abonelik verilerini üç ayda bir tüketerek modelleri iyileştirir.  win/kaybetme verilerini kullanarak, Machine Learning algoritmaları ayarlar ve küme önerilerini MSX bölümünde işlem yapılan fırsatlarla karşılaştırarak modellerin beklendiği gibi çalıştığını doğrular.

:::image type="content" source="images/insights/customer-opportunity-4.png" alt-text="SMB Machine Learning 'in ekran görüntüsü.":::

## <a name="cloudascent-propensity"></a>Cloudadscent eğilimini

Eğilimini önerileri nasıl oluşturulur?

Web gezginleri aracılığıyla toplanan sinyalleri ve çeşitli kaynaklardan gelen verileri kullanarak, firmograf verilerini ve müşterinin sosyal medya sinyallerini birleştirdik.  Puanlama, bu sinyalleri ve verileri, amaç için uyum ve Puanlama modelleri için karşılaştırma modelleriyle kullanır.

1. Müşteri hesabına Sığdır

   - Firmografları tanımlayan iç ve dış veri noktaları.

   - Kullanım Puanlama, müşterileri karşılaştırmak için en iyi SMB 'ye benzer bir model kullanır ve Microsoft Bulut ürünlere yönelik potansiyel bir uyum olup olmadığını görür.

   - Puanlama Sığdır üç ayda bir güncelleştirilir

2. Müşteri hesabı hedefi

   - Sosyal medya ve müşterinin çevrimiçi davranışı ile ilgili sinyaller amaç tanımlar.

   - Amaç Puanlama, kümeleri tanımlamak için sığacak kadar yer alır.

   - Amaç Puanlama aylık olarak güncelleştirilir.

   :::image type="content" source="images/insights/customer-opportunity-5.png" alt-text="Cloudadtik SMB tahmine dayalı modeller.":::

3. Kümeleme

   Sığdırma ve amaç sinyalleri bir kümeleme puanına birleştirilir. Cloudadtik dört kümeye sahiptir:

      - Şimdi davran-satış için hazır müşteriler
      - Değerlendirme-pazarlama için hazırlık müşterileri
      - Nurture-Drive tanıma kampanyaları
      - Eğitime-amacı ve izleyiciyi eğitin

   Kümeleme, kullanıcıların belirli müşterileri, segment faktörlerine göre satış ve pazarlama girişimleri için hedeflemesini sağlar, örneğin: ürün, coğrafi, sektör ve dikey.

   Clouduscent çalışma kitaplarındaki **eğilimini model** sekmesi, eğilimini ve tahmini boşluk gelirini paylaşır. Sığdırma ve amaç kümelemesini tanımlamak için aşağıdaki adımlardan ilerliyoruz:

      1. ML modellerini kullanarak, ilk olarak 100 ölçeğinde müşterinin sığması puanı ve amaç puanı hesaplandık.  tam puanlar, ML modellere göre değişir.  Aşağıdaki örnek puanları:

         |**Sınıflandırma**|**Inızı**|
         |---------|:---------|
         |Yüksek|75-100|
         |Orta|55-74|
         |Düşük|30 - 54|
         |Çok düşük|0 - 29|

      2. Yukarıdaki kuralı kullanarak, şirketlerin hem müşteri hem de amaç sinyallerine göre yüksek, orta, düşük ve çok düşük olmasını sağladık.

      3. Eğilimini temsil eden her kesişmeyle, bir 2B matriste müşterinin sığdırmasını ve amaç sinyallerini çiztik. Örneğin, en yüksek eğilimini temsil eden üst düzey + yüksek amaç = a1.

      4. Son olarak, bu segmentler grupları kümeler halinde oluşturur.  Örneğin, a1, a2, a3, A4, şimdi davran kümesi.

         :::image type="content" source="images/insights/customer-opportunity-6.png" alt-text="Cloudadscent modelleri.":::

   Bu müşteriler için, şimdi davran 'ın hedeflenmesini ve müşterileri değerlendirmesini öneririz.

## <a name="cloudascent-products--models"></a>Clouduscent ürünleri & modelleri

Aşağıdaki grafik, Clouthscent içindeki her eğilimini modelinin bir görünümünü sağlar:

:::image type="content" source="images/insights/customer-opportunity-7.png" alt-text="Cloudadscent eğilimini modeli.":::

Boşluk modelleri, bir ürünün olmadığı ve/veya net yeni aday müşteriler müşterileri olmayan mevcut Microsoft müşterilerinin tahminlerden oluşur.

büyük satış modelleri, Azure ve Microsoft 365 sku 'larında büyük satış potansiyelini tahmin etmek için işlem verilerini kullanır.

bu müşterilerin hem Azure hem de Microsoft 365 sahip olacağı ve büyük satış modeli, mevcut SKU 'sunun daha fazlasını satın aldıklarından emin olur.

eos, Win 7, Office 2010, SQL Server ve Windows sunucusu için hizmet sonu (eos) müşterilerini paylaşır. EOS verileri MS Sales 'ten çekilir ve kullanılabilir olduğunda CloudAscent eğilimini modellemesiyle yer alýr. EOS verileri, modern Iş ve Azure satış oynatılırken yaşar.
