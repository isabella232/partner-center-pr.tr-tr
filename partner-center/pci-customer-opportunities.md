---
title: İş Ortağı Merkezi öngörüleri-Cloudadscent eğilimini raporları
description: Iş Ortağı Merkezi 'nde Cloudadscent eğilimini raporları hakkında bilgi edinin. Microsoft ürünlerini satın almak için bir müşterinin eğilimini hakkında bilgiler içerir.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 430aea81964d1b75514b6e1377bd2ba1af41b538
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110153047"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>Cloudadscent eğilimini raporları Iş Ortağı Merkezi panosundan kullanılabilir

**Uygun roller**: Executive rapor Görüntüleyici | Rapor Görüntüleyicisi

Iş Ortağı Merkezi panosu, Cloudadscent programından indirilebilir eğilimini verileri sağlar. Veriler, müşterilerin Microsoft ürünlerini satın alma olasılığını gösterir.  Bu makalede bu verilerin dökümü, Puanlama kullanımı ve ne anlama geldiğini açıklanmaktadır.

## <a name="summary-definitions"></a>Özet tanımları

- **SMC müşterileri**: Bu, eğilimini indirmelerinde bulunan toplam müşteri sayısıdır.  Müşteriler, kayıt ortağı tarafından tanımlanır.
- **Süresi dolan anlaşmalar**: geçerli mali yıl içinde, süresi dolan sözleşmelerin sayısını sağlıyoruz.
- **Süresi dolan gelir**: açık süresi dolan anlaşmalarla ilişkili gelir.

:::image type="content" source="images/pci/cust-oppor-11.png" alt-text="Müşteriler fırsatlar Özet Panosu ekran görüntüsü.":::

## <a name="cloudascent-smb-segmentation"></a>Cloudadtik SMB kesimlemesi

Küçük ve orta ölçekli iş (SMB) segmenti üç farklı alt parçaya bölünür.

1. **En Iyi yönetilmeyen** , Microsoft için en çok fırsat olan en büyük SMB müşterilerini içerir. Tipik En Iyi yönetilmeyen müşteriler benzer özellikleri, çok sayıda çalışan, büyük BT bütçeleri ve harcama ve Microsoft için büyük miktarda potansiyel gelir ile yönetilen hesaplara paylaşır.

   En üst yönetilmeyen olarak iki şekilde tanımlanır:

   - **Üst yönetilmeyen Kullanıcı tabanlı**– 300 veya daha fazla çalışan hesapları içerir. User-Based hesapları ilk kez satın alma veya Microsoft 365, Dynamics 365 veya Surface gibi kullanıcı tabanlı abonelik ürünlerinin genişletilmesi için harika hedeflerdir.
   - **En İyi Unmanaged Compute Based:** Azure potansiyeli 10 bin ABD dolarından büyük olan hesapları içerir. İşlem tabanlı hesaplar mevcut Azure'ları içerir. gelecek yıl için önemli bir potansiyele sahip olan hesaplar ve henüz Azure'a satın almamış ancak Azure için 10 bin DOlardan fazla potansiyele sahip olan hesaplar.

2. **Medium Business,** 25-300 çalışanı olan mevcut müşterileri ve potansiyel müşteri hesaplarını içerir.

3. **Small Business,** 10-25 çalışanı olan işletmeler içerir.

4. **Çok Küçük İşletmeler,** 1-9 çalışanı olan işletmeler içerir.

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="SMC türüne göre müşteri.":::

**En İyi Unmanaged** **ve Medium Business** alt kesimleri, Microsoft ve Microsoft İş Ortakları için yüksek yaşam süresi değeri (LTV) müşterilerini temsil eder. Bu nedenle, bu segmentte büyümeyi devamtırma odak noktası bunlardır. Bu iki alt abonelikte yuvayı Microsoft 365 ile almak, D365/Azure iş hattı (LOB) uygulamalarıyla daha fazla gelir elde etmek ve Microsoft için yüksek bir LTV gerçekleştirmek için daha iyi konumlara sahip oluruz.

Bugün iki önemli fırsat alanımız vardır: 1. müşterimiz büyümeye devam ediyor; 2. Bulut yuvalarını en iyi şekilde Microsoft 365 dynamics 365 ve Azure'da büyük bir fırsatımız var.

Aşağıdaki ekran görüntüsü dört SMB Altgegment'larını temsil eder. CloudAscent, tüm En İyi Unmanaged ve Medium Business hesaplarının profil oluşturma, puanlama ve modelleme önceliklerini belirleme.

:::image type="content" source="images/pci/cust-oppor-32.png" alt-text="SMB alt ayrımlarının ekran görüntüsü.":::

## <a name="cloudascent-machine-learning"></a>CloudAscent Machine Learning

SMB, En İyi Unmanaged ve Medium Business segmentleri içinde satış ve pazarlama müşterisi tahminlerini sağlamak için makine öğrenmesi teknolojisini kullanır. Sinyaller nasıl toplanır ve yayma önerilerine nasıl dönüşer?

- **Veri toplama**: web gezginleri şirket etki alanlarını ve blog yayınlarını izleyerek, yayınlar, sosyal akışlar ve teknik Forumlar ' e basarak milyarlarca müşteri sinyalleri tarar ve toplar.  Toplanan sinyallere ek olarak, firmograf bilgileri, D&B, Microsoft Iç aboneliği ve işlem verileri gibi iç ve dış kaynaklardan toplanır.

- **Machine Learning**: sinyaller, bulut ürünü ve kümesi tarafından her müşteri için yapılandırılmış veri satış ve pazarlama tahminleri kümesini veren makine öğrenimi modeline dağıtılır.  Her müşteri, Microsoft 'un müşterinin sığdırmasını belirleyen ve müşterinin çevrimiçi davranışını tümleştiren makine öğrenimi algoritmalarının amaç olarak tanımladıkları, benzer bir model ile Microsoft 'un en üst SMB 'sini kullanarak puanlanır. Puanlama, Microsoft Bulut ürünlerini satın almak için müşterinin eğilimini gösteren kümeler halinde birleştirilir.

- **İyileştirme**: Machine Learning sistemi işlem verilerini aylık ve abonelik verilerini üç ayda bir tüketerek modelleri iyileştirir.  Win/kaybetme verilerini kullanarak, Machine Learning algoritmaları ayarlar ve küme önerilerini MSX bölümünde işlem yapılan fırsatlarla karşılaştırarak modellerin beklendiği gibi çalıştığını doğrular.

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="SMB Machine Learning 'in ekran görüntüsü.":::

## <a name="cloudascent-propensity"></a>Cloudadscent eğilimini

Eğilimini önerileri nasıl oluşturulur?

Web gezginleri aracılığıyla toplanan sinyalleri ve çeşitli kaynaklardan gelen verileri kullanarak, firmograf verilerini ve müşterinin sosyal medya sinyallerini birleştirdik.  Puanlama, bu sinyalleri ve verileri, amaç için uyum ve Puanlama modelleri için karşılaştırma modelleriyle kullanır.

1. Müşteri hesabına Sığdır

   - Firmografları tanımlayan iç ve dış veri noktaları.

   - Kullanım Puanlama, müşterileri karşılaştırmak için en iyi SMB 'ye benzer bir model kullanır ve Microsoft Bulut ürünlere yönelik potansiyel bir uyum olup olmadığını görür.

   - Puanlama Sığdır üç ayda bir güncelleştirilir

2. Müşteri hesabı hedefi

   - Sosyal medya ve müşterinin çevrimiçi davranışı ile ilgili sinyaller amaç tanımlar.

   - Amaç puanlama, kümeleri tanımlamak için uygun olan üst düzeye atlar.

   - Amaç puanlama aylık olarak güncelleştirilir.

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="CloudAscent SMB tahmine dayalı modelleri.":::

3. Kümeleme

   Fit ve amaç sinyalleri bir kümeleme puanında birleştirilmiştir. CloudAscent dört kümeye sahip:

      - Hemen Harekete Geç - satışa hazır müşteriler
      - Değerlendirme - pazarlamaya hazır müşteriler
      - Besleme - farkındalık kampanyalarını artırma
      - Eğitin - amaç için eğitin ve izleme

   Kümeleme, kullanıcıların segment faktörlerine (örneğin ürün, coğrafi, sektör ve dikey) göre satış ve pazarlama girişimleri için belirli müşterileri hedeflemelerine olanak sağlar.

   CloudAscent Workbooks'daki Yayma modeli sekmesi, eğilimi ve tahmini boşluk gelirini paylaşıyor.  Fit ve Intent kümelelerini tanımlamak için aşağıdaki adımları izleyin:

      1. ML Modellerini kullanarak önce 100 ölçeğinde Customer Fit Score ve intent Score hesaplarız.  Tam Puanlar ML Modellerine göre farklılık gösterir.  Aşağıdaki Örnek Puanlar:

         |**Sınıflandırma**|**Puan**|
         |---------|:---------|
         |Yüksek|75 - 100|
         |Orta|55 - 74|
         |Düşük|30 - 54|
         |Çok Düşük|0 - 29|

      2. Yukarıdaki kuralı kullanarak, şirketlerin hem müşteri hem de amaç sinyallerine göre yüksek, orta, düşük ve çok düşük olmasını sağladık.

      3. Eğilimini temsil eden her kesişmeyle, bir 2B matriste müşterinin sığdırmasını ve amaç sinyallerini çiztik. Örneğin, en yüksek eğilimini temsil eden üst düzey + yüksek amaç = a1.

      4. Son olarak, bu segmentler grupları kümeler halinde oluşturur.  Örneğin, a1, a2, a3, A4, şimdi davran kümesi.

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="Cloudadscent modelleri.":::

   Bu müşteriler için, şimdi davran 'ın hedeflenmesini ve müşterileri değerlendirmesini öneririz.

## <a name="cloudascent-products--models"></a>Clouduscent ürünleri & modelleri

Aşağıdaki grafik, Clouthscent içindeki her eğilimini modelinin bir görünümünü sağlar:

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="Cloudadscent eğilimini modeli.":::

Boşluk modelleri, bir ürünün olmadığı ve/veya net yeni aday müşteriler müşterileri olmayan mevcut Microsoft müşterilerinin tahminlerden oluşur.

Büyük satış modelleri, Azure ve Microsoft 365 SKU 'Larında büyük satış potansiyelini tahmin etmek için işlem verilerini kullanır.

Bu müşterilerin hem Azure hem de Microsoft 365 sahip olacağı ve büyük satış modeli, mevcut SKU 'sunun daha fazlasını satın aldıklarından emin olur.

EOS, Win 7, Office 2010, SQL Server ve Windows Server için hizmet sonu (EOS) müşterilerini paylaşır. EOS verileri MS Sales 'ten çekilir ve kullanılabilir olduğunda CloudAscent eğilimini modellemesiyle yer alýr. EOS verileri, modern Iş ve Azure satış oynatılırken yaşar.
