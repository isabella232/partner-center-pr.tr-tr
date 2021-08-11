---
title: İş Ortağı Merkezi Analizler - CloudAscent Propensity raporları
description: İş Ortağı Merkezi'daki CloudAscent Propensity raporları hakkında bilgi İş Ortağı Merkezi. Müşterinin Microsoft ürünlerini satın alma eğilimi hakkında bilgi içerir.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 9c9c592a5720642c9d2d0c7b5ac8c2a4aa23387d4d6c063ca1e064959a340c1e
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115686345"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>CloudAscent Propensity raporları panodan İş Ortağı Merkezi kullanılabilir

**Uygun roller:** Yönetici rapor görüntüleyicisi | Rapor görüntüleyicisi

İş Ortağı Merkezi panosu, CloudAscent programından indirilebilir teklif verileri sağlar. Veriler, müşterilerin Microsoft ürünlerini satın alma olasılığını gösterir.  Bu makalede bu verilerin dökümü, puanlamanın nasıl kullanımı ve ne anlama geldiğini açıklanmıştır.

## <a name="summary-definitions"></a>Özet tanımları

- **SMC Müşterileri**– Bu, teklif indirmelerinde toplam müşteri sayısıdır.  Müşteriler, kaydın iş ortağı tarafından tanımlanır.
- **Sözleşme süre** sonu– Geçerli mali yıl içinde süresi dolan sözleşme sayısını sağlıyoruz.
- **Süresi Dolan Geliri Aç:** Açık süresi dolan sözleşmelerle ilişkili gelir.

:::image type="content" source="images/insights/customer-opportunity-1.png" alt-text="Müşteri Fırsatları Özeti panosunun ekran görüntüsü.":::

## <a name="cloudascent-smb-segmentation"></a>CloudAscent SMB segmentasyon

Küçük ve orta ölçekli işletme (SMB) segmenti üç ayrı alt segmente ayrılır.

1. **En İyi Unmanaged,** Microsoft için en fazla fırsata sahip olan en büyük SMB müşterilerini içerir. Tipik En İyi Yönetilemeyen müşteriler, Çok sayıda çalışan, büyük IT bütçeleri ve harcamaları ve Microsoft için büyük miktarlarda potansiyel gelirle Yönetilen hesaplara benzer özelliklere sahiptir.

   En İyi Unmanaged'ı iki şekilde tanımlamış oluruz:

   - **En İyi Unmanaged User Based :** 300 veya daha fazla çalışanı olan hesapları içerir. User-Based hesapları ilk kez satın almak veya Microsoft 365, Dynamics 365 veya Surface gibi kullanıcı tabanlı abonelik ürünlerinin genişletilmesi için harika hedeflerdir.
   - **En İyi Unmanaged Compute Based:** Azure potansiyeli 10 bin ABD dolarından büyük olan hesapları içerir. İşlem tabanlı hesaplar mevcut Azure'ları içerir. gelecek yıl için önemli bir potansiyele sahip olan hesaplar ve henüz Azure'a satın almamış ancak Azure için 10 bin DOlardan fazla potansiyele sahip olan hesaplar.

2. **Medium Business,** 25-300 çalışanı olan mevcut müşterileri ve potansiyel müşteri hesaplarını içerir.

3. **Small Business,** 10-25 çalışanı olan işletmeler içerir.

4. **Çok Küçük İşletmeler,** 1-9 çalışanı olan işletmeler içerir.

:::image type="content" source="images/insights/customer-opportunity-2.png" alt-text="SMC türüne göre müşteri.":::

**En İyi Unmanaged** **ve Medium Business** alt kesimleri, Microsoft ve Microsoft İş Ortakları için yüksek yaşam süresi değeri (LTV) müşterilerini temsil eder. Bu nedenle, bu segmentte büyümeyi devamtırma odak noktası bunlardır. Bu iki alt abonelikte yuvayı Microsoft 365 ile almak, D365/Azure iş hattı (LOB) uygulamalarıyla daha fazla gelir elde etmek ve Microsoft için yüksek bir LTV gerçekleştirmek için daha iyi konumlara sahip oluruz.

Bugün iki önemli fırsat alanımız vardır: 1. müşterimiz büyümeye devam ediyor; 2. Bulut yuvalarını en iyi şekilde Microsoft 365 dynamics 365 ve Azure'da büyük bir fırsatımız var.

Aşağıdaki ekran görüntüsü dört SMB Altgegment'larını temsil eder. CloudAscent, tüm En İyi Unmanaged ve Medium Business hesaplarının profil oluşturma, puanlama ve modelleme önceliklerini belirleme.

:::image type="content" source="images/insights/customer-opportunity-3.png" alt-text="SMB alt ayrımlarının ekran görüntüsü.":::

## <a name="cloudascent-machine-learning"></a>CloudAscent Machine Learning

SMB, En İyi Unmanaged ve Medium Business segmentleri içinde satış ve pazarlama müşterisi tahminlerini sağlamak için makine öğrenmesi teknolojisini kullanır. Sinyaller nasıl toplanır ve yayma önerilerine nasıl dönüşer?

- **Veri Toplama:** Web tarayıcıları şirket etki alanlarına ping atarak ve blog gönderilerini, basın yayınlarını, sosyal akışları ve teknik forumları izleerek milyarlarca müşteri sinyalini tarar ve toplar.  Toplanan sinyallere ek olarak D&B, Microsoft İç aboneliği ve işlem verileri gibi hem iç hem de dış kaynaklardan sıkı bilgiler toplanır.

- **Machine Learning:** Sinyaller, bulut ürünü ve kümesine göre her müşteri için yapılandırılmış bir Satış ve Pazarlama tahminleri veri kümesi çıkışına sahip makine öğrenmesi modeline beslenir.  Her müşteri, Microsoft'un müşterinin Uygun olup olmadığını belirleyen en iyi SMB modeline benzer bir görünüm kullanılarak puanlandı ve müşterinin çevrimiçi davranışını tümleştiren makine öğrenmesi algoritmaları Amaç olarak tanımlandı. Puanlama, müşterinin Microsoft Bulut Ürünleri satın alma eğilimini göstermek için kümeler ile birleştirilir.

- **İyileştirme:** Machine Learning sistemi, işlem verilerini aylık olarak ve abonelik verilerini üç ayda bir kullanarak modelleri iyiler.  Win/loss verilerini kullanarak Machine Learning, küme önerilerini MSX üzerinde işlem yapılan fırsatlarla karşılaştırarak algoritmaları ayarlar ve modellerin beklendiği gibi çalıştığını doğrular.

:::image type="content" source="images/insights/customer-opportunity-4.png" alt-text="SMB makine öğrenmesi ekran görüntüsü.":::

## <a name="cloudascent-propensity"></a>CloudAscent Propensity

Yayma önerileri nasıl oluşturulur?

Web gezginleri aracılığıyla toplanan sinyalleri ve çeşitli kaynaklardan sağlanan verileri kullanarak, sıkı grafik verilerini ve müşterinin sosyal medya sinyallerini birleştiriyoruz.  Puanlama, Amaç için uygun ve puanlama modelleri için karşılaştırma modellerinde bu sinyalleri ve verileri kullanır.

1. Müşteri Hesabı Sığdırma

   - Sıkı grafiği tanımlayan iç ve dış veri noktaları.

   - Uygun puanlama, müşterileri karşılaştırmak ve Microsoft Cloud Products için potansiyel olarak uygun olup olduklarını görmek için en iyi SMB'mize benzer bir model kullanır.

   - Fit puanlama üç aylık olarak güncelleştirilir

2. Müşteri Hesabı Amacı

   - Sosyal medya ve müşterinin çevrimiçi davranışıyla ilgili sinyaller Amacı tanımlar.

   - Amaç puanlama, kümeleri tanımlamak için uygun olan üst düzeye atlar.

   - Amaç puanlama aylık olarak güncelleştirilir.

   :::image type="content" source="images/insights/customer-opportunity-5.png" alt-text="CloudAscent SMB tahmine dayalı modelleri.":::

3. Kümeleme

   Fit ve amaç sinyalleri bir kümeleme puanında birleştirilmiştir. CloudAscent dört kümeye sahip:

      - Hemen Harekete Geç - satışa hazır müşteriler
      - Değerlendirme - pazarlamaya hazır müşteriler
      - Besleme - farkındalık kampanyalarını artırma
      - Eğitin - amaç için eğitin ve izleme

   Kümeleme, kullanıcıların segment faktörlerine (örneğin ürün, coğrafi, sektör ve dikey) göre satış ve pazarlama girişimleri için belirli müşterileri hedeflemelerine olanak sağlar.

   CloudAscent Workbooks'daki Yayma modeli sekmesi, eğilimi ve tahmini boşluk gelirini paylaşıyor.  Fit ve Intent kümelelerini tanımlamak için aşağıdaki adımları izleyin:

      1. ML Modellerini kullanarak önce 100 ölçeğinde Customer Fit Score ve intent Score hesaplarız.  Tam Puanlar, ML göre değişir.  Aşağıdaki Örnek Puanlar:

         |**Sınıflandırma**|**Puan**|
         |---------|:---------|
         |Yüksek|75 - 100|
         |Orta|55 - 74|
         |Düşük|30 - 54|
         |Çok Düşük|0 - 29|

      2. Yukarıdaki kuralı kullanarak, şirketleri hem Müşteri Uyumu hem de Amaç Sinyalleri genelinde Yüksek, Orta, Düşük ve Çok Düşük olarak sınıflandırabilirsiniz.

      3. Her kesişim eğilimi temsil eden bir 2 boyutlu matriste müşteri uyum ve amaç sinyallerini çizeriz. Örneğin, en yüksek eğilimi temsil eden High Fit + High Intent = A1.

      4. Son olarak, bu segmentler kümeler oluşturmak için grup oluşturur.  Örneğin, A1, A2, A3, A4 Şimdi Harekete Geç kümesidir.

         :::image type="content" source="images/insights/customer-opportunity-6.png" alt-text="CloudAscent modelleri.":::

   Bu müşteriler için Şimdi Harekete Geç ve Müşterileri Değerlendir'i hedeflemenizi öneririz.

## <a name="cloudascent-products--models"></a>CloudAscent Products & Modelleri

Aşağıdaki grafik, CloudAscent içindeki her bir yayma modelinin görünümünü sağlar:

:::image type="content" source="images/insights/customer-opportunity-7.png" alt-text="CloudAscent propensity model.":::

Boşluk modelleri, ürüne sahip değil ve/veya net yeni potansiyel müşterileri olan mevcut Microsoft müşterileri için tahminlerden oluşur.

Satış modelleri, Azure'da satış potansiyelini tahmin etmek ve SKUS'ları kullanmak için işlem Microsoft 365 kullanır.

Bu müşteriler zaten hem Azure hem de Microsoft 365 sahip olacak ve satış modeli, mevcut SKU'larından daha fazla satın alma olasılığı olduğunu gösteriyor.

EOS; Win 7, Office 2010, SQL Server ve Windows Server için hizmet sonu (EOS) müşterilerini paylaşıyor. EOS verileri MS Sales'den çekilir ve cloudAscent eğilimi modellemesi (varsa) ile birlikte kullanılır. EOS verileri Modern Çalışma ve Azure Satış oyunlarında yer alır.
