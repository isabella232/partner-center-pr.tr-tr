---
title: Müşteri listenizi yönetin
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Müşteri kayıtları en önemli bilgi varlıklarının arasındadır. Iş ortağı merkezi müşteri listenizde bilgileri görüntülemeyi, aramanızı, güncelleştirmeyi, & dışarı aktarmayı öğrenin.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 244a8cfc661b371b611a19a5c90ddf131b42a46a
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441974"
---
# <a name="manage-your-customer-list---search-update-or-export-customers-in-partner-center"></a>Müşteri listenizi yönetme-Iş Ortağı Merkezi 'nde müşterileri arama, güncelleştirme veya dışarı aktarma

**Şunlara uygulanır**

- Microsoft Cloud for US Government için İş Ortağı Merkezi

Müşteri kayıtları, Iş Ortağı Merkezi 'nde en önemli bilgi varlıklarınız arasındadır. Müşteri hesabı veritabanınızda arama yapabilir, tüm müşteri veritabanını dışarı aktarabilir veya bir alt kümeyi Excel uyumlu bir virgülle ayrılmış değer dosya biçimine (. csv) aktarabilirsiniz. Ayrıca, bir müşterinin abonelik bilgilerini bir. csv dosyasına dışarı aktarabilirsiniz.

Etkinlik günlükleri, müşterilere yönelik işlemler ve yönetim eylemleri üzerinde dışarı aktarılabilir veriler de sağlar. Daha fazla bilgi için bkz. [Müşteri etkinlik günlüklerini görüntüleme](activity-logs.md).

## <a name="search-for-a-customer"></a>Müşteri arayın

1. **Iş Ortağı Merkezi** menüsünde **müşteriler**' i seçin.
2. Bir müşteriyi aramak için, arama kutusuna müşteri adını veya etki alanı adını girin.
3. Microsoft KIMLIKLERINI ve bunlarla ilişkili abonelikleri ve hizmetleri hızlı bağlantılarını görmek için bir müşteri satırının sonundaki **aşağı oku** seçin.

## <a name="update-a-customers-company-name"></a>Müşterinin şirket adını güncelleştirme

**Iş Ortağı Merkezi** menüsünde **müşteriler**' i seçin.
2. Bir müşteriyi aramak için, arama kutusuna müşteri adını veya etki alanı adını girin.
3. Microsoft KIMLIKLERINI ve bunlarla ilişkili abonelikleri ve hizmetleri hızlı bağlantılarını görmek için bir müşteri satırının sonundaki **aşağı oku** seçin.
4. Müşterinin **Fatura** bilgileri altında şirket adını güncelleştirin. Yeni değeri kaydettiğinizde, müşteri listesine yansıtılır. Bu, yalnızca fatura-şirket adı ve müşteri listesi değerini değiştirir. Başka herhangi bir yere yansıtılmayacaktır.

## <a name="export-your-customer-list"></a>Müşteri listenizi dışarı aktarma

1. **Iş Ortağı Merkezi** menüsünde **müşteriler**' i seçin.
2. **Müşterileri dışarı aktar**' ı seçin.

   İş Ortağı Merkezi, tüm müşteri listenizi bir. csv dosyasına dönüştürür ve bilgisayarınızdaki varsayılan indirme klasörüne yükler. Ayrıca, müşteri verilerinin alt kümelerini de dışarı aktarabilirsiniz. Veri sütunları şunları içerir:

   - **MICROSOFT kimliği**;
   - **Şirket adı**;
   - **Birincil etki alanı adı**;
   - **İlişki**— iş ortağının listelenen her müşteriyle iş ilişkisi.

    Varsayılan olarak, Iş Ortağı Merkezi, uzunluktan bağımsız olarak tüm müşteri listesini dışarı aktarır. Ayrıca müşteri listesini şirket adına veya etki alanına göre arayabilir ve bu veri alt kümesini dışarı aktarabilirsiniz.

3. Dolaylı bir Sağlayıcıysanız, müşteri listenizi dolaylı satıcıya göre filtreleyebilirsiniz. Listeden **dolaylı satıcıya göre filtrele** ' yi seçin ve ardından bir satıcı seçin.


## <a name="export-customer-subscription-information"></a>Müşteri abonelik bilgilerini dışarı aktar

1. **Iş Ortağı Merkezi** menüsünde **müşteriler**' i seçin.

2. Herhangi bir müşteri için **şirket adını** seçin. Ürün aboneliklerinin tüm listesini gösteren müşterinin **abonelikler** sayfası açılır.

3. **Abonelikleri dışarı aktar**' ı seçin. İş Ortağı Merkezi, müşterinin abonelik verilerini bir. csv dosyasına dönüştürür ve bilgisayarınızdaki varsayılan indirme klasörüne yükler. Veri sütunları şunları içerir:
   - **ABONELIK kimliği**;
   - **Abonelik**— aboneliğin ürün adı;
   - **Miktar**— satın alınan lisans sayısı;
   - **Durum**;
   - **Satıcı**— aboneliği karşılayan ve yöneten satıcının kimliği.

> [!NOTE]  
> Abonelik yönetimi hakkında daha fazla bilgi için bkz. [Müşteri abonelikleri](customer-subscriptions.md).
