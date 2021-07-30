---
title: Bir .csv hesabı için birden çok kullanıcı içeri aktarmaya uygun dosyanın alanları
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Bir müşteri hesabına birden çok kullanıcı eklemek için uygun alanlara sahip bir virgülle .csv (.csv) dosyası oluşturun.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7d8cbeecf081dc82448625daeedc0ce21b31174e
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114838351"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>Bir .csv dosyası oluşturarak müşteri hesabına birden .csv ekleme

**Uygun roller:** Genel yönetici

Virgülle ayrılmış değer dosyası biçimindeki (.csv) bir veri dosyasını aynı anda müşterinin hesabına yük İş Ortağı Merkezi. Örnek veri dosyasını dosyadan indirip İş Ortağı Merkezi için düzenleyebilir veya aşağıda tanımlanan veri modelini kullanarak yeni bir veri dosyası oluşturabilirsiniz.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>Veri dosyası gereksinimleri

Toplu karşıya yükleme işlemini kullanarak müşterinin hesabına birden çok kullanıcı eklemek için aşağıdaki gereksinimleri karşılamanız gerekir:

- Müşteri hesabı üzerinde genel yönetici izinlerine sahip olmak;
- Her kullanıcının, müşterinin e-posta etki alan adlarının sonuna benzersiz bir e-posta adresi eklemesi gerekir;
- Aynı anda en fazla 100 kayıt yükleyebilirsiniz. 100'den fazla kullanıcı eklemeniz gerekirse ek veri dosyaları oluşturun ve karşıya yükleyin.
- Tüm kullanıcıların aynı coğrafi Konumda olması **gerekir.**
- Yalnızca aşağıda açıklanan verileri girin. Fazlalık veriler karşıya yüklemenin başarısız olmasına neden olur.

Veri dosyasına aşağıdaki verileri girin:

| **Sütun adı** | **Açıklama**  | **Sınırlama**  |
|:-------- |:------  |:----- |
| Ad  | Kullanıcının adı (isteğe bağlı alan)  | 50 karakterlik sınır  |
| Soyadı  | Kullanıcının soyadı (isteğe bağlı alan)  | 50 karakterlik sınır  |
| Görünen ad    | Ad, İş Ortağı Merkezi (gerekli alan)                            | 50 karakterlik sınır                         |
| E-posta   | Müşterinin müşteri şirketinde iş e-posta adresi (gerekli alan)           | Her kullanıcının benzersiz bir e-posta adresi olmalıdır |
| Durum güncelleştirmesi   | Yeni kullanıcı kaydının başarıyla oluşturulıp oluşturula olmadığını belirtmek için kullanılır | \*\*Boş bırakın\*\*                        |

## <a name="next-steps"></a>Sonraki adımlar

- [Bir müşteri için birden çok kullanıcı ekleme](adding-multiple-users-to-a-customer-account.md)