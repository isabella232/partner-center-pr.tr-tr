---
title: Müşteri listenizi yönetme
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Müşteri kayıtları en önemli bilgi varlıkları arasında yer alan varlıklardır. Müşteri listenizin bilgilerini görüntülemeyi, aramayı, & ve dışarı aktarmayı İş Ortağı Merkezi öğrenin.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: df0f72deb14eac6d75f8579f7099ab3c6b6a2905
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248301"
---
# <a name="manage-your-customer-list---search-update-or-export-customers-in-partner-center"></a>Müşteri listenizi yönetme - müşteriler için arama, güncelleştirme veya dışarı İş Ortağı Merkezi

**Için geçerlidir:** İş Ortağı Merkezi | İş Ortağı Merkezi için Microsoft Cloud for US Government

**Uygun roller:** Yönetici aracısı | Genel yönetici

Müşteri kayıtları, en önemli bilgi varlıklarınızı İş Ortağı Merkezi. Müşteri hesapları veritabanınızı arayabilir, tüm müşteri veritabanını dışarı aktarabilir veya bir alt kümeyi, Excel uyumlu virgülle ayrılmış değer dosya biçimine (.csv) aktarabilirsiniz. Ayrıca müşterinin abonelik bilgilerini bir .csv aktarabilirsiniz.

Etkinlik günlükleri ayrıca müşteriler için işlemler ve yönetim eylemleriyle ilgili dışarı aktarılabilir veriler sağlar. Daha fazla bilgi için [bkz. Müşteri etkinlik günlüklerini görüntüleme.](activity-logs.md)

## <a name="search-for-a-customer"></a>Müşteri arama

1. Veri **İş Ortağı Merkezi** Müşteriler'i **seçin.**
2. Müşteri aramak için arama kutusuna müşteri adını veya etki alanı adını girin.
3. Microsoft **kimliklerini ve** ilişkili abonelikleri ve hizmetleri hızlı bağlantılarını görmek için müşteri satırı sonundaki aşağı oku seçin.

## <a name="update-a-customers-company-name"></a>Müşterinin şirket adını güncelleştirme

Veri **İş Ortağı Merkezi** Müşteriler'i **seçin.**
2. Müşteri aramak için arama kutusuna müşteri adını veya etki alanı adını girin.
3. Microsoft **kimliklerini ve** ilişkili abonelikleri ve hizmetleri hızlı bağlantılarını görmek için müşteri satırı sonundaki aşağı oku seçin.
4. Müşterinin Fatura bilgileri **altında** şirket adını güncelleştirin. Yeni değeri kaydetmeniz, müşteri listesine yansıtacak. Bu, yalnızca Fatura şirketi adını ve müşteri listesi değerini değiştirir. Bu durum başka bir yere yansıtmayacak.

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

3. Abonelikleri **dışarı aktar'ı seçin.** İş Ortağı Merkezi, müşterinin abonelik verilerini bir .csv dosyasına dönüştürür ve bilgisayarınızda varsayılan indirme klasörüne yükler. Veri sütunları aşağıdakileri içerir:
   - **Abonelik Kimliği**;
   - **Abonelik**— aboneliğin ürün adı;
   - **Miktar**—satın alınan lisans sayısı;
   - **Durum;**
   - **Kurumsal** Bayi — Aboneliğin sahibi olan ve aboneliği yöneten kurumsal bayinin kimliği.

> [!NOTE]  
> Abonelik yönetimi hakkında daha fazla bilgi için bkz. [Müşteri abonelikleri.](customer-subscriptions.md)
