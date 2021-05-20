---
title: Öngörüler Indirme raporu panosu
ms.topic: article
ms.date: 10/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Iş Ortağı Merkezi Birleşik raporlama panosundan ve Iş Ortağı Merkezi öngörülerinin verilerini indirme ve dışa aktarma hakkında bilgi edinin.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 266baf0eb3501cba984ec0fbaed4508366b92b8b
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152792"
---
# <a name="download-reports"></a>Raporları indir

**Uygun roller**: Executive rapor Görüntüleyici | Rapor Görüntüleyicisi

## <a name="introduction"></a>Giriş

Öngörüler panosundaki rapor Indirme Merkezi, Iş Ortağı Merkezi öngörülerinin sekmeyle ayrılmış değer (TSV) biçiminde gücünü sağlayan ham veri kümelerini dışa aktarabilirsiniz. Bu, iş gereksinimlerine bağlı olarak veriler üzerinde ayrıntılı analiz yapmanızı sağlar.

Oluşturulduktan sonra rapor, Microsoft Excel gibi araçları kullanarak indirmeniz ve çözümlemeniz için **oluşturulan raporlar** bölümünde kullanılabilir olacaktır.

**Yeni rapor oluştur**

Bir rapor oluşturmak için önce rapor **Seç** açılan listesinden raporu seçin. Ardından **Tarih aralığı Seç** açılan menüsünden Tarih aralığını seçin. **Oluştur**' u seçin. Rapor, sekmeyle ayrılmış değer (TSV) biçiminde oluşturulur ve birkaç dakika içinde **oluşturulan raporlar** bölümünde indirilebilir. Önceki 14 gün içinde oluşturulan raporlar indirilmek üzere kullanılabilir olacaktır.

:::image type="content" source="images/pci/create-new-report.png" alt-text="Yeni rapor oluştur":::

:::image type="content" source="images/pci/generated-reports.png" alt-text="Oluşturulan raporlar":::

>[!NOTE] 
>Yalnızca Executive rapor izleyicileri olan kullanıcılar raporları indirebilir. Öngörüler panosu raporlarına rol tabanlı erişim hakkında daha fazla bilgi için lütfen [PCI rollerine](pci-roles.md)bakın. 

## <a name="available-reports"></a>Kullanılabilir raporlar

Aşağıdaki raporlar indirilebilir:

**Iş ortağı profili** , iş ortağıyla ilgili ayrıntıları sağlar. Iş ortağı KIMLIĞI, Iş ortağı adı, Iş ortağı şehri ve Iş ortağı ülkesi gibi ayrıntılar raporda bulunabilir. Bu rapor için toplama veya geri arama geçerli olmayacaktır.

**Müşteri ayrıntıları,** bir İş Ortağının ilişkili olduğu müşterilerin ayrıntılarını sağlar. Ayrıca satılan lisanslar, toplu ACR gibi önemli ölçümler de sağlar. Rapor aylık olarak toplanır.

**Abonelik ayrıntıları,** müşteri bilgileriyle birlikte İş Ortağı tarafından satılan veya yönetilen aboneliklerin ayrıntılarını sağlar. Rapor aylık olarak toplanır.

**Azure kullanımı,** Azure kullanım ayrıntılarını sağlar. Bu ayrıntılar İş Ortağı tarafından satılan veya yönetilen Azure abonelikleri için geçerlidir. Kullanım ayrıntıları ölçüm kategorisine ve diğer anahtar boyutlara göre ayrılır. Rapor aylık olarak toplanır.

**Office365 - Lisans Kullanımı,** İş Ortağı tarafından satılan veya yönetilen O365 lisanslarının kullanım ayrıntılarını sağlar. Ayrıca müşteri bilgilerini ve Aylık Etkin Kullanıcılar (MAU), nitelikli yetkilendirmeler gibi temel ölçümleri de sağlar. Rapor aylık olarak toplanır.

**Enterprise Mobility – Lisans Kullanımı,**  İş Ortağı tarafından satılan veya yönetilen Enterprise Mobility lisanslarının kullanım ayrıntılarını sağlar. Ayrıca müşteri bilgilerini ve Aylık Etkin Kullanıcılar (MAU), nitelikli yetkilendirmeler gibi temel ölçümleri sağlar. Rapor aylık olarak toplanır.

**Dynamics 365 – Lisans Kullanımı,** İş Ortağı tarafından satılan veya yönetilen D365 lisanslarının kullanım ayrıntılarını sağlar. Ayrıca müşteri bilgilerini ve Aylık Etkin Kullanıcılar (MAU), nitelikli yetkilendirmeler gibi temel ölçümleri de sağlar. Rapor aylık olarak toplanır.

**Power BI - Lisans Kullanımı,** İş Ortağı tarafından satılan veya Power BI lisansların kullanım ayrıntılarını sağlar. Ayrıca müşteri bilgilerini ve Aylık Etkin Kullanıcılar (MAU), nitelikli yetkilendirmeler gibi temel ölçümleri de sağlar. Rapor aylık olarak toplanır.

**Eğitimler;** iş ortağının çalışanları tarafından tamamlanan veya alınan sınavlar, sertifikalar, değerlendirmeler, parçalar, kurslar gibi ayrıntıları sağlar.

**Microsoft Learn** modüllerle ilgili ayrıntıları, öğrenme yolu tamamlama ayrıntılarını ve iş ortağının kullanıcı ayrıntılarını sağlar.

**Yetkinlikler : Özet ve geçmiş,** etkin, devam eden veya bu İş Ortağı için risk altında olan tüm yetkinliklerin ayrıntılarını sağlar. Ayrıca iş ortağı tarafından elde edilen tüm yetkinliklerin geçmişini içerir.

**Yetkinlikler – Performans ayrıntıları,** iş ortağının belirli bir yetkinlik kümesine ulaşmak için KIP'lere göre nasıl performans sergileye dair ayrıntılı bilgiler sağlar.

