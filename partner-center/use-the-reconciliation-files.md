---
title: Karşılaştırma dosyalarınızı kullanın
ms.topic: article
ms.date: 03/10/2021
description: Iş Ortağı Merkezi 'nde mutabakat dosyaları ve belirli bir faturalandırma döngüsünün ücretlendirdiği ayrıntılı, satır öğesi görünümlerinin nasıl yorumlanacağı hakkında bilgi edinin.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e6b9e466402d71c988729052bd72ba2346a9d977
ms.sourcegitcommit: 868f90c54f26a037eee29749c207a7316bb4b475
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "103022783"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Iş Ortağı Merkezi mutabakatı dosyalarınızda satır öğelerini okumayı öğrenin

**Uygun roller**

- Faturalama yöneticisi
- Genel yönetici

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

1. Microsoft Excel 'de mutabakat dosyasını (. csv biçiminde) açın.
2. Dosyadaki ilk sütunu seçin.
3. **Metni sütunlara dönüştürme Sihirbazı**' nı açın. Şeritte, **veriler**' i seçin ve **sütunlar**' ı seçin.
4. Sihirbazda, **ayrılmış dosya türü**' nü seçin. Ardından **İleri**' yi seçin.
5. **Sınırlayıcılar** alanında **virgül**' yi seçin. ( **Sekmesi** zaten seçildiyse, bu seçeneği seçili bırakabilirsiniz.) Ardından **İleri**' yi seçin.
6. **Sütun veri biçimi** alanında **Tarih: mdy**' yi seçin. Ardından **İleri**' yi seçin.
7. **Sütun veri biçimi** alanında, tüm miktar sütunları için **metin** ' i seçin. Ardından **Son**'u seçin.

## <a name="download-reconciliation-files-programmatically"></a>Karşılaştırma dosyalarını programlı olarak indir

Mutabakat dosyaları çok büyük olabilir ve bazen indirmek zordur. Karşılaştırma dosyalarını program aracılığıyla indirmek için bkz. [fatura satırı öğelerini Al](/partner-center/develop/get-invoiceline-items).

## <a name="map-taxes-or-vat"></a>Vergiler veya KDV 'yi eşleştirin

Vergiler veya katma değer vergi (KDV) faturanızı eşlemek için:

- Lisans tabanlı dosyadaki **vergi** sütununu toplayın.
- Kullanım tabanlı dosyadaki **TaxAmount** sütununu toplayın.

## <a name="itemize-reconciliation-files-by-partner"></a>İş ortağına göre mutabakat dosyalarını dök

**Dolaylı modeldeki** iş ortakları, bu ek alanları hem lisans tabanlı hem de kullanım tabanlı mutabakat dosyalarında kullanarak dosyaları satıcıya göre silebilirsiniz.

| MPN Kimliği | Description |
| ------ | ----------- |
| MPN Kimliği | Bulut çözümü sağlayıcısı (CSP) ortağının (doğrudan veya dolaylı) Microsoft İş Ortağı Ağı (MPN) tanımlayıcısı. |
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