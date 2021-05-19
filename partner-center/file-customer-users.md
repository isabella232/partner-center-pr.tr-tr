---
title: Bir müşteri hesabı için birden çok kullanıcının içeri aktarılacağı. csv dosyası alanları
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Bir müşteri hesabına birden çok kullanıcı eklemek için uygun alanlara sahip bir virgülle ayrılmış değer (. csv) dosyası oluşturun.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 152daadde25a9325937797f7a3daa90dfb59a9b4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150990"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>Bir. csv dosyası oluşturarak müşteri hesabına birden çok kullanıcı ekleme

**Uygun roller**: genel yönetici

Bir veri dosyasını, virgülle ayrılmış değer dosya biçimi 'ne (. csv) Iş Ortağı Merkezi 'ne yükleyerek bir müşterinin hesabına tek seferde birden fazla kullanıcı ekleyin. Ortak merkezinden bir örnek veri dosyası indirebilir ve ardından kullanım için düzenleyebilir veya aşağıda tanımlanan veri modelini kullanarak yeni bir veri dosyası oluşturabilirsiniz.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>Veri dosyası gereksinimleri

Toplu karşıya yükleme işlemini kullanarak bir müşterinin hesabına birden çok kullanıcı eklemek için aşağıdaki gereksinimleri karşılamanız gerekir:

- Müşteri hesabı için genel yönetici izinlerine sahip olmanız gerekir;
- Her kullanıcının e-posta etki alanına (ler) eklenen benzersiz bir e-posta adresi olmalıdır.
- Tek seferde en fazla 100 kayıt yükleyebilirsiniz. 100 'den fazla Kullanıcı eklemeniz gerekiyorsa, ek veri dosyaları oluşturun ve karşıya yükleyin.
- Tüm kullanıcılar aynı coğrafi **konumda** olmalıdır.
- Yalnızca aşağıda açıklanan verileri girin. Gereksiz veriler karşıya yüklemenin başarısız olmasına neden olur.

Veri dosyasına aşağıdaki verileri girin:

| **Sütun adı** | **Açıklama**  | **Sınırlama**  |
|:-------- |:------  |:----- |
| Ad  | Kullanıcının adı (isteğe bağlı alan)  | 50-karakter sınırı  |
| Soyadı  | Kullanıcının Soyadı (isteğe bağlı alan)  | 50-karakter sınırı  |
| Görünen ad    | Ad, İş Ortağı Merkezi (gerekli alan)                            | 50 karakterlik sınır                         |
| E-posta   | Müşterinin müşteri şirketinde iş e-posta adresi (gerekli alan)           | Her kullanıcının benzersiz bir e-posta adresi olmalıdır |
| Durum güncelleştirmesi   | Yeni kullanıcı kaydının başarıyla oluşturulıp oluşturula olmadığını belirtmek için kullanılır | \*\*Boş bırakın\*\*                        |

## <a name="next-steps"></a>Sonraki adımlar

- [Bir müşteri için birden çok kullanıcı ekleme](adding-multiple-users-to-a-customer-account.md)