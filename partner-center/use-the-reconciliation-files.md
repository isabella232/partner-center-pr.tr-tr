---
title: Mutabakat dosyalarınızı kullanma
ms.topic: article
ms.date: 03/26/2021
description: Iş Ortağı Merkezi 'nde mutabakat dosyaları ve belirli bir faturalandırma döngüsünün ücretlendirdiği ayrıntılı, satır öğesi görünümlerinin nasıl yorumlanacağı hakkında bilgi edinin.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e5fae4c9b9b40c8a71b56c46d0d1be629f832842
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961034"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Iş Ortağı Merkezi mutabakatı dosyalarınızda satır öğelerini okumayı öğrenin

**Uygun roller**: Faturalandırma Yöneticisi | Genel yönetici

Bir fatura döngüsündeki her bir ücret için ayrıntılı, satır öğesi görünümü için Iş Ortağı Merkezi ' nden mutabakat dosyalarınızı indirebilirsiniz. Satır öğesi ayrıntıları, her bir müşterinin aboneliğine ilişkin ücretleri ve ayrıntılı olayları (bir aboneliğe yönelik bir abonelik için orta dönem ekleme gibi) içerir.

**Faturanızı** okuma hakkında daha fazla bilgi için bkz. [faturanızı okuyun](read-your-bill.md).

## <a name="understand-reconciliation-file-fields"></a>Mutabakat dosyası alanlarını anlama

- [Lisans tabanlı mutabakat dosyası alanları](license-based-recon-files.md)
- [Kullanım tabanlı mutabakat dosyası alanları](usage-based-recon-files.md)
- [Günlük fiyatlandırılan kullanım mutabakat dosyası alanları](daily-rated-usage-recon-files.md)
- [Bir kerelik satın alma CSP 'si mutabakatı dosya alanları](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Mutabakat dosyalarındaki ücretlendirme türlerini anlama

Mutabakat dosyalarındaki ( **Chargetype** sütunu) ücret türlerini anlamak için bkz. [mutabakatı dosya ücreti türleri](recon-file-charge-types.md).

## <a name="fix-formatting-issues"></a>Biçimlendirme sorunlarını giderme

Bazen bir mutabakat dosyasında biçimlendirme sorunları bulunabilir. Örneğin, en-US yerel ayarı kullanılmazsa bu sorun oluşabilir.

Mutabakat dosyalarınızda biçimlendirme sorunlarını gidermek için aşağıdaki adımları izleyin:

1. Microsoft Excel ' de mutabakat dosyasını (.csv biçiminde) açın.
2. Dosyadaki ilk sütunu seçin.
3. **Metni sütunlara dönüştürme Sihirbazı**' nı açın. Şeritte, **veriler**' i seçin ve **sütunlar**' ı seçin.
4. Sihirbazda, **ayrılmış dosya türü**' nü seçin. Ardından **İleri**' yi seçin.
5. **Sınırlayıcılar** alanında **virgül**' yi seçin. ( **Sekmesi** zaten seçildiyse, bu seçeneği seçili bırakabilirsiniz.) Ardından **İleri**' yi seçin.
6. **Sütun veri biçimi** alanında **Tarih: mdy**' yi seçin. Ardından **İleri**' yi seçin.
7. **Sütun veri biçimi** alanında, tüm miktar sütunları için **metin** ' i seçin. Ardından **Son**'u seçin.

## <a name="download-reconciliation-files-programmatically"></a>Karşılaştırma dosyalarını programlı olarak indir

Mutabakat dosyaları çok büyük olabilir ve bazen indirmek zordur. Karşılaştırma dosyalarını program aracılığıyla indirmek için bkz. [fatura satırı öğelerini Al](/partner-center/develop/get-invoiceline-items).

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a>Dosyanız Excel satır sınırını aşarsa

bir mutabakat dosyası indirebiliyor ancak Microsoft Excel içinde açmadıysanız, dosyanın izin vermeyeceği kadar fazla Excel satır içerdiği anlamına gelir. Bu durumda, dosyayı açmak için aşağıdaki yordamlardan birini kullanabilirsiniz.

### <a name="open-a-recon-file-in-power-bi"></a>Power BI bir keşfi dosyası açın

1. Mutabakat dosyasını normalde yaptığınız gibi indirin.
2. Microsoft Power BI bir örneğini indirin, yükleyin ve açın.
3. Power BI **giriş** sekmesinde **veri al**' ı seçin.
4. **Ortak veri kaynakları** listesinde **metin/CSV**' yi seçin.
5. İstendiğinde, keşfi dosyanızı açın.

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a>Excel pivot tablosunda bir keşfi dosyası açın

1. Mutabakat dosyasını normalde yaptığınız gibi indirin.
2. Microsoft Excel yeni bir dosya açın.
3. **Veri** sekmesinde **veri al**' ı seçin, dosyadan ' **ı SEÇIN ve** ardından **metin/CSV**' yi seçin.
4. İstendiğinde, keşfi dosyanızı açın. Verileriniz görüntülenecektir.
5. **Yük** açılır menüsünde, **Yükle**' yi seçin ve ardından **Tamam**' ı seçin.
6. **Verileri Içeri aktar** iletişim kutusunda Dosyanızı açmak Için **PivotTable raporu** ' nu seçin.

## <a name="negative-amount-displayed"></a>Negatif miktar görüntülendi

Mutabakat dosyanızda negatif bir miktar görebilirsiniz. Bu sorun büyük olasılıkla aşağıdakilerden biri nedeniyle oluşur:

- Son zamanlarda lisans numaranızı iptal etmiş veya azalttı
- Bir hizmet Lisans Sözleşmesi (SLA) ya da Azure tüketimi için kredi aldınız

Bu işlem hakkında daha fazla bilgi edinmek için mutabakat dosyanızda işlemin ödeme türü özniteliğini gözden geçirin.

## <a name="map-taxes-or-vat"></a>Vergiler veya KDV 'yi eşleştirin

Vergiler veya katma değer vergi (KDV) faturanızı eşlemek için:

- Lisans tabanlı dosyadaki **vergi** sütununu toplayın.
- Kullanım tabanlı dosyadaki **TaxAmount** sütununu toplayın.

## <a name="itemize-reconciliation-files-by-partner"></a>İş ortağına göre mutabakat dosyalarını dök

**Dolaylı modeldeki** iş ortakları, bu ek alanları hem lisans tabanlı hem de kullanım tabanlı mutabakat dosyalarında kullanarak dosyaları satıcıya göre silebilirsiniz.

| MPN Kimliği | Description |
| ------ | ----------- |
| MPN Kimliği | Bulut Çözümü Sağlayıcısı (CSP) ortağının (doğrudan veya dolaylı) Microsoft İş Ortağı Ağı (mpn) tanımlayıcısı. |
| [Satıcı MPN KIMLIĞI](#reseller-mpn-id) | [Abonelik için kayıt satıcısının MPN tanımlayıcısı](#reseller-mpn-id). Bu alan, Iş Ortağı Merkezi 'nde belirli bir abonelik için listelenen satıcı KIMLIĞINE karşılık gelir. Yalnızca dolaylı modeldeki iş ortakları için mutabakat dosyaları üzerinde görüntülenir. |

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