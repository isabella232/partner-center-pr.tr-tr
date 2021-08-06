---
title: Mutabakat dosyalarınızı kullanma
ms.topic: article
ms.date: 03/26/2021
description: Hesap hesaplarında mutabakat İş Ortağı Merkezi ve verilen faturalama dönemi için ücretlerin ayrıntılı, satır öğesi görünümlerini yorumlama hakkında bilgi edinmek.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2b14379f7e7750b3423d03be4addaca4e4a6a94834709b9f0b6e5891a185bb0c
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115681204"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Mutabakat dosyalarında satır öğelerini okumayı İş Ortağı Merkezi öğrenin

**Uygun roller:** Faturalama yöneticisi | Genel yönetici

Bir faturalama döngüsünde her bir İş Ortağı Merkezi ayrıntılı ve satır öğesi görünümü için mutabakat dosyalarınızı bir hesaptan indirebilirsiniz. Satır öğesi ayrıntıları, her müşterinin aboneliklerinin ücretlerini ve ayrıntılı olayları (bir aboneliğe lisansların orta dönem eklemesi gibi) içerir.

Faturanızı okuma hakkında bilgi **için bkz.** [Faturanızı okuma.](read-your-bill.md)

## <a name="understand-reconciliation-file-fields"></a>Mutabakat dosyası alanlarını anlama

- [Lisans tabanlı mutabakat dosyası alanları](license-based-recon-files.md)
- [Kullanım tabanlı mutabakat dosyası alanları](usage-based-recon-files.md)
- [Günlük fiyatlandırılan kullanım mutabakat dosyası alanları](daily-rated-usage-recon-files.md)
- [Tek sefer satın alma CSP mutabakat dosyası alanları](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Mutabakat dosyalarında ücret türlerini anlama

Mutabakat dosyalarında **(ChargeType** sütunu) ücret türlerini anlamak için [bkz. Mutabakat dosyası ücret türleri.](recon-file-charge-types.md)

## <a name="fix-formatting-issues"></a>Biçimlendirme sorunlarını düzeltme

Bazen bir mutabakat dosyası biçimlendirme sorunları içerebilir. Örneğin, en-US yerel yereli kullanılmazsa bu sorun oluşabilir.

Mutabakat dosyalarınıza ilişkin biçimlendirme sorunlarını düzeltmek için şu adımları izleyin:

1. Mutabakat dosyasını (.csv biçiminde) Microsoft Excel.
2. Dosyadaki ilk sütunu seçin.
3. Metni **Sütunlara Dönüştürme Sihirbazı'nı açın.** Şeritte Veri'yi **ve ardından** Metinden **Sütunlar'a'ı seçin.**
4. Sihirbazda Sınırlandırılmış **dosya türü'ne tıklayın.** Ardından, **Sonraki'yi seçin.**
5. **Sınırlayıcılar alanında Virgül'i** **seçin.** (Sekme **zaten** seçiliyse, bu seçeneği seçili bırakın.) Ardından, **Sonraki'yi seçin.**
6. Sütun veri biçimi alanında **Tarih:MDY'yi seçin.**  Ardından, **Sonraki'yi seçin.**
7. Sütun veri **biçimi alanında tüm** tutar sütunları için **Metin'i** seçin. Ardından **Son**'u seçin.

## <a name="download-reconciliation-files-programmatically"></a>Mutabakat dosyalarını program aracılığıyla indirme

Mutabakat dosyaları çok büyük olabilir ve bazen indirmek zordur. Mutabakat dosyalarını program aracılığıyla indirmek için [bkz. Fatura satırı öğelerini al.](/partner-center/develop/get-invoiceline-items)

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a>Dosyanız, dosyanız içinde satır sınırını Excel

Bir mutabakat dosyasını indire ancak dosyada açamıyorsanız Microsoft Excel dosyanın izin verecekleri satırlardan daha fazla satır içerdiği Excel gelir. Bu durumda, dosyayı açmak için aşağıdaki yordamlardan birini kullanabilirsiniz.

### <a name="open-a-recon-file-in-power-bi"></a>Bir mutabakat dosyasını Power BI

1. Mutabakat dosyasını normalde olduğu gibi indirin.
2. Microsoft Power BI'nin bir örneğini indirin, yükleyin ve açın.
3. Giriş sekmesinde Power BI  al'ı **seçin.**
4. Ortak veri kaynakları listesinde **Metin/CSV'yi seçin.** 
5. İstendiğinde, mutabakat dosyanızı açın.

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a>Özet tabloda mutabakat Excel açma

1. Mutabakat dosyasını normalde olduğu gibi indirin.
2. Dosyada yeni bir Microsoft Excel.
3. Veri sekmesinde **Veri al'ı** **seçin,** **Dosyadan'ı ve** ardından **Metin/CSV'yi seçin.**
4. İstendiğinde, mutabakat dosyanızı açın. Verileriniz görüntülenir.
5. Yükle açılan **menüsünde,** Üzerine **yükle'yi ve ardından** Tamam'ı **seçin.**
6. Verilerinizi İçeri **Aktar iletişim** kutusunda **PivotTable Raporu'nı seçerek** dosyanızı açın.

## <a name="negative-amount-displayed"></a>Negatif tutar görüntülenir

Mutabakat dosyanız negatif bir tutar görebilir. Bu sorun büyük olasılıkla aşağıdakilerden biri nedeniyle oluşur:

- Kısa süre önce lisanslarınızı iptal etti veya azalttınız
- Hizmet lisans sözleşmesi (SLA) veya Azure tüketimi için kredi aldınız

Bu işlem hakkında daha fazla bilgi edinmek için mutabakat dosyanızda işlemin ödeme türü özniteliğini gözden geçirin.

## <a name="map-taxes-or-vat"></a>Vergileri veya KDV'yi eşleme

Vergileri veya katma değerli vergileri (KDV) faturanıza eşlemek için:

- Lisans **tabanlı** dosyadan Vergi sütununu toplama.
- Kullanım tabanlı **dosyadan TaxAmount** sütununu toplama.

## <a name="itemize-reconciliation-files-by-partner"></a>Mutabakat dosyalarını iş ortağına göre öğeleştirme

Dolaylı modelde **iş ortakları,** bu ek alanları hem lisans tabanlı hem de kullanım tabanlı mutabakat dosyalarında kullanarak dosyaları kurumsal bayiye göre öğe hale kullanabilir.

| MPN Kimliği | Description |
| ------ | ----------- |
| MPN Kimliği | Microsoft İş Ortağı Ağı (CSP) iş ortağının Bulut Çözümü Sağlayıcısı (MPN) tanımlayıcısı. |
| [Kurumsal Bayi MPN Kimliği](#reseller-mpn-id) | aboneliği [için kayıt kurumsal bayinin MPN tanımlayıcısı.](#reseller-mpn-id) Bu alan, belirli bir abonelik için listelenen kurumsal bayi kimliğine karşılık İş Ortağı Merkezi. Yalnızca dolaylı modelde iş ortakları için mutabakat dosyalarında görünür. |

### <a name="reseller-mpn-id"></a>Kurumsal Bayi MPN Kimliği

CsP iş ortağı aboneliği doğrudan müşteriye satsa **MPN** kimliği iki kez listelenir ve **hem MPN Kimliği** hem de **Kurumsal Bayi MPN Kimliği olarak listelenir.**

CSP iş ortağının **MPN** kimliğine sahip bir kurumsal bayisi varsa, bu değer bunun yerine iş **ortağının MPN kimliğine** ayarlanır.

CSP iş ortağı kurumsal bayi **MPN kimliğini** kaldırırsa bu değer *-1 olarak ayarlanır.*

Kurumsal Bayi MPN Kimliğini **görüntülemek veya güncelleştirmek için:**

1. İş Ortağı Merkezi'nde oturum açın.
2. Veri İş Ortağı Merkezi Müşteriler'i **seçin.**
3. Listeden müşteriyi seçin.
4. Müşteri menüsünde Abonelikler'i **seçin.**
5. Listeden aboneliği seçin.
6. Kurumsal **Bayiyi** **(MPN KIMLIĞI) değiştirmek için güncelleştir'i seçin.**

## <a name="next-steps"></a>Sonraki adımlar

- [Mutabakat dosyası için faturanızı & okuma](read-your-bill.md) 