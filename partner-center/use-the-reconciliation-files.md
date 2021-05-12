---
title: Mutabakat dosyalarınızı kullanma
ms.topic: article
ms.date: 03/26/2021
description: Hesap hesaplarında mutabakat İş Ortağı Merkezi ve verilen faturalama dönemi için ücretlerin ayrıntılı, satır öğesi görünümlerini yorumlama hakkında bilgi öğrenin.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 755881d0bd96b9d601346ebb6271bd524c31d0a3
ms.sourcegitcommit: 837d3c5b52ab056b2b761cd85eb2426f56b62614
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/12/2021
ms.locfileid: "109794964"
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

1. Mutabakat dosyasını (.csv biçiminde) Microsoft Excel'de açın.
2. Dosyadaki ilk sütunu seçin.
3. Metni **Sütunlara Dönüştürme Sihirbazı'nı açın.** Şeritte Veri'yi **ve ardından** Metinden **Sütunlar'a'ı seçin.**
4. Sihirbazda Sınırlandırılmış **dosya türü'ne tıklayın.** Ardından **İleri**' yi seçin.
5. **Sınırlayıcılar** alanında **virgül**' yi seçin. ( **Sekmesi** zaten seçildiyse, bu seçeneği seçili bırakabilirsiniz.) Ardından **İleri**' yi seçin.
6. **Sütun veri biçimi** alanında **Tarih: mdy**' yi seçin. Ardından **İleri**' yi seçin.
7. **Sütun veri biçimi** alanında, tüm miktar sütunları için **metin** ' i seçin. Ardından **Son**'u seçin.

## <a name="download-reconciliation-files-programmatically"></a>Karşılaştırma dosyalarını programlı olarak indir

Mutabakat dosyaları çok büyük olabilir ve bazen indirmek zordur. Karşılaştırma dosyalarını program aracılığıyla indirmek için bkz. [fatura satırı öğelerini Al](/partner-center/develop/get-invoiceline-items).

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a>Dosyanız Excel 'deki satır sınırını aşarsa

Bir mutabakat dosyasını indirebiliyor ancak Microsoft Excel 'de açmadıysanız, dosyada Excel 'In izin vermeyeceği daha fazla satır bulunduğu anlamına gelir. Bu durumda, dosyayı açmak için aşağıdaki yordamlardan birini kullanabilirsiniz.

### <a name="open-a-recon-file-in-power-bi"></a>Power BI bir keşfi dosyası açın

1. Mutabakat dosyasını normalde yaptığınız gibi indirin.
2. Power BI örneğini indirin, yükleyin ve açın.
3. Power BI **giriş** sekmesinde **veri al**' ı seçin.
4. **Ortak veri kaynakları** listesinde **metin/CSV**' yi seçin.
5. İstendiğinde, keşfi dosyanızı açın.

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a>Excel Pivot tablosunda bir keşfi dosyası açma

1. Mutabakat dosyasını normalde yaptığınız gibi indirin.
2. Microsoft Excel'de yeni bir dosya açın.
3. Veri sekmesinde **Veri al'ı** seçin, **Dosyadan'ı ve ardından** **Metin/CSV'yi seçin.** 
4. İstendiğinde, mutabakat dosyanızı açın. Verileriniz görüntülenir.
5. Yükle **açılan menüsünde,** Üzerine **yükle'yi ve ardından** Tamam'ı **seçin.**
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
| MPN Kimliği | Microsoft İş Ortağı Ağı (CSP) iş ortağının Bulut Çözümü Sağlayıcısı (MPN) tanımlayıcısını (doğrudan veya dolaylı). |
| [Kurumsal Bayi MPN Kimliği](#reseller-mpn-id) | Aboneliğin [kaydının kurumsal bayisinde MPN tanımlayıcısı.](#reseller-mpn-id) Bu alan, belirli bir abonelik için listelenen kurumsal bayi kimliğine karşılık İş Ortağı Merkezi. Yalnızca dolaylı modeldeki iş ortakları için mutabakat dosyaları üzerinde görüntülenir. |

### <a name="reseller-mpn-id"></a>Satıcı MPN KIMLIĞI

Bir CSP iş ortağı aboneliği doğrudan müşteriye satmışsa **MPN kimliği** , hem **MPN kimliği** hem de **satıcı MPN kimliği** olarak iki kez listelenir.

Bir CSP iş ortağının **MPN kimliği** olmayan bir satıcısı varsa, bu değer bunun yerine ortağın **MPN kimliğine** ayarlanır.

CSP iş ortağı bir **satıcı MPN kimliğini** kaldırdığında bu değer *-1* olarak ayarlanır.

**Satıcı MPN kimliğini** görüntülemek veya güncelleştirmek için:

1. İş Ortağı Merkezi'nde oturum açın.
2. Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin.
3. Listeden müşteriyi seçin.
4. Müşteri menüsünde **abonelikler**' i seçin.
5. Listeden aboneliği seçin.
6. **Satıcıdan (MPN kimliği)** değiştirmek için **Güncelleştir** ' i seçin.

## <a name="next-steps"></a>Sonraki adımlar

- [Faturanız & keşfi dosyanızı okuma](read-your-bill.md) 