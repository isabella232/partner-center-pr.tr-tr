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
ms.openlocfilehash: 6e73aa98e0cfaf82521a5fe63e34ebf0b44363fb
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854511"
---
# <a name="manage-your-customer-list---search-update-or-export-customers-in-partner-center"></a>Müşteri listenizi yönetme-Iş Ortağı Merkezi 'nde müşterileri arama, güncelleştirme veya dışarı aktarma

**Uygulama hedefi**: Iş Ortağı Merkezi | ABD kamu için Microsoft Bulut iş ortağı Merkezi

**Uygun roller**: yönetici Aracısı | Genel yönetici

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
4. Müşterinin **Fatura** bilgileri altında şirket adını güncelleştirin. Yeni değeri kaydetmeniz, müşteri listesine yansıtacak. Bu, yalnızca Fatura şirketi adını ve müşteri listesi değerini değiştirir. Bu durum başka bir yere yansıtmayacak.

## <a name="export-your-customer-list"></a>Müşteri listenizi dışarı aktarma

1. Veri **İş Ortağı Merkezi** Müşteriler'i **seçin.**
2. Müşterileri dışarı **aktar'ı seçin.**

   İş Ortağı Merkezi tam müşteri listenizi bir .csv dosyasına dönüştürür ve bilgisayarınızda varsayılan indirme klasörüne yükler. Ayrıca müşteri verisi alt kümelerini dışarı aktarabilirsiniz. Veri sütunları aşağıdakileri içerir:

   - **Microsoft Kimliği**;
   - **Şirket adı;**
   - **Birincil etki alanı adı;**
   - **İlişki—** İş Ortağının listelenen her müşteriyle iş ilişkisi.

    Varsayılan olarak, İş Ortağı Merkezi ne olursa olsun tüm müşteri listesini dışarı aktarabilirsiniz. Ayrıca, şirket adına veya etki alanına göre müşteri listesinde arama ve bu veri alt kümesini dışarı aktarabilirsiniz.

3. Dolaylı sağlayıcıysanız, müşteri listenizi dolaylı kurumsal bayiye göre filtre alabilirsiniz. Listeden **Dolaylı kurumsal bayiye göre** filtrele'yi ve ardından bir kurumsal bayi seçin.


## <a name="export-customer-subscription-information"></a>Müşteri aboneliği bilgilerini dışarı aktarma

1. Veri **İş Ortağı Merkezi** Müşteriler'i **seçin.**

2. Herhangi bir **müşteri için** Şirket adı'ı seçin. Müşterinin Abonelikler **sayfası** açılır ve ürün aboneliklerinin tam listesi görüntülenir.

3. Abonelikleri **dışarı aktar'ı seçin.** İş Ortağı Merkezi müşterinin abonelik verilerini bir .csv dosyasına dönüştürür ve bilgisayarınızda varsayılan indirme klasörüne yükler. Veri sütunları aşağıdakileri içerir:
   - **Abonelik Kimliği**;
   - **Abonelik**— aboneliğin ürün adı;
   - **Miktar**—satın alınan lisans sayısı;
   - **Durum;**
   - **Kurumsal** Bayi — Aboneliğin sahibi olan ve aboneliği yöneten kurumsal bayinin kimliği.

> [!NOTE]  
> Abonelik yönetimi hakkında daha fazla bilgi için bkz. [Müşteri abonelikleri.](customer-subscriptions.md)
