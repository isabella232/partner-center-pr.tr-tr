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
ms.openlocfilehash: b7d963bffcfeebed3b7540dfd02aadd876dfcaa6
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/31/2021
ms.locfileid: "106086235"
---
# <a name="download-reports"></a>Raporları indir

**Uygun roller**

- Executive rapor Görüntüleyicisi
- Rapor Görüntüleyicisi

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

**Iş ortağı profili** , iş ortağıyla ilgili ayrıntıları sağlar. Iş ortağı KIMLIĞI, Iş ortağı adı, Iş ortağı şehri ve Iş ortağı ülkesi gibi ayrıntılar raporda bulunabilir. Bu rapor için toplama veya geri dönüş uygulanmaz.

**Müşteri ayrıntıları** , bir ortağın ilişkilendirildiği müşterilerin ayrıntılarını sağlar. Ayrıca, satılan lisanslar, toplanan ACR gibi temel ölçümler de sağlar. Rapor aylık olarak toplanır.

**Abonelik ayrıntıları** , iş ortağı tarafından satılan veya yönetilen aboneliklerin ayrıntılarını müşteri bilgileriyle birlikte sağlar. Rapor aylık olarak toplanır.

**Azure kullanımı** , Azure kullanım ayrıntılarını sağlar. Bu ayrıntılar, Iş ortağı tarafından satılan veya yönetilen Azure aboneliklerine yöneliktir. Kullanım ayrıntıları ölçüm kategorisine ve diğer anahtar boyutlarına göre bölünür. Rapor aylık olarak toplanır.

**Office365-lisans kullanımı** , iş ortağı tarafından satılan veya yönetilen O365 lisanslarının kullanım ayrıntılarını sağlar. Ayrıca, aylık etkin kullanıcılar (MAU) ve uygun yetkilendirmeler gibi müşteri bilgilerini ve önemli ölçümleri de sağlar. Rapor aylık olarak toplanır.

**Enterprise Mobility – lisans kullanımı**  , iş ortağı tarafından satılan veya yönetilen kurumsal Mobility lisanslarının kullanım ayrıntılarını sağlar. Ayrıca, aylık etkin kullanıcılar (MAU) ve uygun yetkilendirmeler gibi müşteri bilgilerini ve önemli ölçümleri de sağlar. Rapor aylık olarak toplanır.

**Dynamics 365 – lisans kullanımı** , iş ortağı tarafından satılan veya yönetilen D365 lisanslarının kullanım ayrıntılarını sağlar. Ayrıca, aylık etkin kullanıcılar (MAU) ve uygun yetkilendirmeler gibi müşteri bilgilerini ve önemli ölçümleri de sağlar. Rapor aylık olarak toplanır.

**Power BI-lisans kullanımı** , iş ortağı tarafından satılan veya yönetilen Power BI lisansların kullanım ayrıntılarını sağlar. Ayrıca, aylık etkin kullanıcılar (MAU) ve uygun yetkilendirmeler gibi müşteri bilgilerini ve önemli ölçümleri de sağlar. Rapor aylık olarak toplanır.

Bu işlemler, iş ortağının çalışanları tarafından tamamlanan veya alınan sınavlar, sertifikalar, değerlendirmeler, parçalar, kurslar gibi **ayrıntıları sağlar.**

**Microsoft Learn** , iş ortağının Kullanıcı ayrıntılarıyla birlikte modüller, öğrenme yolu tamamlanma ayrıntıları hakkında ayrıntılı bilgi sağlar.

**Uzmanlıklar: Özet ve geçmiş** , bu iş ortağı için etkin, devam eden veya risk altında olan tüm uzmanlardan oluşan ayrıntıları sağlar. Ayrıca iş ortağının elde ettiği tüm uzmanlık geçmişini içerir.

**Uzmanlıklar: performans ayrıntıları** , belirli bir uzmanlık kümesini elde etmek üzere KPI 'lara yönelik olarak iş ortağının nasıl yaptığı hakkında ayrıntılı bilgi sağlar.

