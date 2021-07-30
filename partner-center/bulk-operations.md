---
title: Referanslar'da csv dosyalarını kullanarak toplu Excel ve içeri aktarma ortak satış fırsatları
description: Excel (CSV) dosyalarını kullanarak ortak satış fırsatlarını indirmeyi, oluşturmayı veya güncelleştirmeyi İş Ortağı Merkezi
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 02/03/2021
ms.openlocfilehash: 91490f3c0104b4807e6178f51a7504dc22d70236
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114842737"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-value-csv-files"></a>Ortak satış fırsatları için virgülle ayrılmış değer (CSV) dosyalarının kullanıldığı toplu işlemler

**Uygun roller:** Referans yöneticisi | Referans kullanıcısı

İş Ortağı Merkezi'ndeki toplu işlemler şirketinizin ortak satış fırsatı verilerini dışarı ve içeri aktarmasına yardımcı olur. **Ortak satış fırsatları** sayfasına gidin ve sayfa başlığının sağ üst kısmındaki **içeri aktar** ve **dışarı aktar** bağlantılarını bulun. Hem **Referans yöneticisi** hem de **Referans Kullanıcısı** izinleri olan kullanıcılar bu işlevselliği kullanabilir.

> [!IMPORTANT]
> Toplu içeri aktarma aracılığıyla yapılan oluşturma/güncelleştirme eylemleri geri alınamaz. Çok fazla sayıda kaydı değiştirir veya oluştururken dikkatli olun. Satış anlaşması oluşturulduktan sonra alanların yalnızca bir alt kümesi değiştirilebilir. **Satış anlaşması Reddedildi/Süresi Doldu/Kazanıldı/Kaybedildi gibi bir son duruma ulaştığında hiçbir eyleme izin verilmez.**

## <a name="export-co-sell-opportunities"></a>Ortak satış fırsatlarını dışarı aktarma

Aşağıdaki bilgiler dışarı aktarma işlevini açıklar:

- Dışarı aktar düğmesine **tıklayarak en fazla 5000** kaydı dışarı **aktarabilirsiniz.**
- İndirilen anlaşmalar, erişim düzeylerinize göre olacaktır. Referans yöneticileri ve Referans kullanıcıları, anlaşmalara takım üyeleri olarak dahil edildiklerine ve kapsamına göre farklı sonuçlar elde ediyor olabilir. Referans izinleri hakkında [daha fazla bilgi.](permissions-overview.md#manage-referrals)
- Dışarı aktarma işlevi, ortak satış fırsatları sayfasındaki geçerli sekmeyi ve uygulanmış filtreleri hesaba katmayı alır.
- Uygulanan filtreleri temel alan tüm verilerin bulunduğu bir CSV dosyası oluşturulur.
- Kayıtları indirmek bir dakika kadar zaman alır.
- İndirme eyleminin tamamlandıktan sonra tamamlanır. Uygulama içinde diğer sayfalara İş Ortağı Merkezi bile, dışarı aktarma işlevi tamamlandıktan hemen sonra dosya indirilir.
- Anlaşma ayrıntılarını değiştirmek ve tüm kayıtları güncelleştirmek için karşıya yüklemek üzere indirilen dosyayı yeniden kullanabilirsiniz.

## <a name="import-co-sell-opportunities"></a>Ortak satış fırsatlarını içeri aktarma

- İçeri aktarma işlevini kullanarak en **fazla 1000 kayıt** oluşturabilir veya güncelleştirin.
- Şablonu, uygulamanın İçeri Aktarma sayfasından indirerek sıfırdan İş Ortağı Merkezi.
- Var olan kayıtları indirmek ve güncelleştirmek için Dışarı Aktarma işlevini de kullanabilirsiniz.
- Dosyada 1000'den fazla kayıt varsa işlenemez.
- Dosya işlendikten sonra, oluşturulan, güncelleştirilen ve işlenmemiş olan referansların sayısının bir özeti son işlem dosyası kartında gösterilir.
- İşlenen kayıtların ayrıntılarını indirebilir, hataları düzeltebilir ve önceki çalıştırmada başarısız olan kayıtları oluşturmak veya güncelleştirmek için aynı dosyayı karşıya yükleyebilirsiniz. **Önceki çalıştırmada başarısız olan düzeltilmiş kayıtları karşıya yüklemeden önce dosyadan tüm başarılı kayıtları kaldırın.**
- Daha fazla çözüm eklemek için çözüm 1'in yanına ek sütunlar ekleyin ve sütun adını Çözüm X olarak kullanın. Burada X, anlaşmadaki çözüm sayısını temsil eder. Örneğin, Çözüm 2, Çözüm 3.
- Anlaşma için en fazla 50 çözüm ekleme.
- Daha fazla takım üyesi eklemek için, Takım üyesi 1'in yanına ek sütunlar ekleyin ve sütun adını Takım üyesi X olarak kullanın; burada X, anlaşmadaki takım üyesinin sayısını temsil eder. Örneğin, Takım üyesi 2, Takım üyesi 3.
- Anlaşma için en fazla 50 ekip üyesi ekleme.

> [!NOTE]
> İşlemenin tamamlandıktan sonra tamamlanır. İşlem tamamlandıktan sonra son işlenen dosyanın ayrıntıları indirilebilir. **1000 kaydı olan dosyaları karşıya yüklerken bu süre 10 dakika kadar sürebilir.**

> [!IMPORTANT]
> Tüm yönergeleri dikkatle okuyun ve aşağıdaki tabloda yer alan her sütunun biçimini, aşağıdaki tabloda csv dosyalarını kullanarak satış anlaşması oluşturmadan veya güncelleştirmeden İş Ortağı Merkezi.

|**Sütun adı**|**Zorunlu mu?**|**Açıklama**|**Örnek değer**|
|-----|:-----|:---------|:---|
Hatalar|No|Başvurulara yönelik w.r.t oluşturma/güncelleştirme işlemleriyle ilgili hatalar bu sütuna dahil edilir. Birden çok hata varsa bunların hepsi noktalı virgülle ayrılmış olarak listelenir.|Zorunlu alan Çözüm 1 eksik|
Katılım Kimliği|No|Katılım kimliği Microsoft iş ortağı merkezi referans sistemi tarafından oluşturulur. Yeni referans oluşturma için gerekli değildir. Bir kaydı güncelleştiriyorsanız mevcut katılım kimliğini kullanabilirsiniz.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
Referans kimliği|No|Referans kimliği, Microsoft iş ortağı merkezi referans sistemi tarafından oluşturulur. Yeni referans oluşturma için gerekli değildir. Mevcut bir kaydı güncelleştiriyorsanız referans kimliğiyle doldurun.|ebacdkdc-0b84-4ac4-b4ea-5b2587d42cee
Anlaşma Adı|Yes|Başvuru için anlaşmanın kolay adı.|Birleşik Krallık spring deal
Müşteri Adı|Yes|Müşteri şirketinin adı. Microsoft tarafında hızlı eşleştirme için kuruluşun yasal adını kullanın.|Contoso Corporation
Müşteri Adres Satırı 1|Yes|Müşteri şirketinin 1. satırına adresle. |Tek Contoso Yolu
Müşteri Adres Satırı 2|No|Müşteri şirketinin 2. adres satırı.|NE 148 sokağı
Customer City|Yes|Müşteri kuruluşlarının bulunduğu şehir.|Redmond
Müşteri Durumu|No|Müşteri kuruluşlarının bulunduğu yeri ifade.|Washington
Müşteri Posta Kodu|No|Müşteri kuruluşlarının bulunduğu bölgenin Posta Kodu.|98052
Müşteri Ülkesi|Yes|Müşteri kuruluşlarının bulunduğu Ülke/Bölge. Burada belirtildiği gibi iki harfli ülke kodlarını [kullanın.]( https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes)|ABD
Müşteri D-U-N-S Kimliği|No|Müşteri kuruluşlarının DUNS kimliğini getirmeye çalışma. Bu, Microsoft tarafında müşteri kuruluşlarının daha hızlı eşleşmesi için yardımcı olur ve bu da satıcı atamalarının daha hızlı tamamlansa da yardımcı olur. DBIR ID 'yi bu [Web SITESINDEN](https://www.dnb.com/duns-number/lookup.html)ücretsiz edinebilirsiniz.|81466849
Müşterinin kişi adı soyadı|Şekline|İlk adı yalnızca Microsoft Yardım 'a ihtiyacınız varsa zorunludur. Müşteri kuruluşundan bu anlaşma üzerinde çalışan birincil kişinin adı.|John
Müşterinin kişi adı soyadı|Şekline|Soyadı yalnızca Microsoft Yardım gerekirse zorunludur. Bu anlaşma üzerinde çalışan müşteri kuruluşundan birincil kişinin soyadı.|Müşteri
müşteri iletişim Telefon numarası|Şekline|Telefon numarası yalnızca Microsoft yardım gerekirse zorunludur. bu işlem sırasında çalışan müşteri kuruluşundaki birincil ilgili kişinin Telefon numarası.|9999999999
Müşteri Iletişim e-posta adresi|Şekline|E-posta adresi yalnızca Microsoft Yardım 'a ihtiyacınız varsa zorunludur. Bu anlaşma üzerinde çalışan müşteri kuruluşundan birincil kişinin e-posta adresi.|john.customer@contoso.com
İş ortağı başvuru durumu|Yes|Şirketinizin perspektifinden ilgili durumunu gösterir. Bir başvuruyu oluşturmaya veya değiştirmeye çalıştığınızda gereklidir. Yeni bir anlaşma oluşturmaya çalışıyorsanız **Yeni** ' ye kullanın. Kabul edilen değerler [burada](/partner/develop/referral-resources#referralstatus)belgelenmiştir.|Etkin
İş ortağı başvurusu alt durumu|Yes|İşlem durumunun tam durumunu gösterir. Yeni bir anlaşma oluşturmaya çalışıyorsanız **kabul edildi** ' i kullanın. Mevcut bir başvuruyu değiştiriyorsanız de gereklidir. Kabul edilen değerler [burada](/partner/develop/referral-resources#referralsubstatus)belgelenmiştir.|Kabul edildi
Microsoft başvuru durumu|Şekline|Microsoft arama yardımı 'na gönderdiğiniz ortak satış isteğinin durumunu gösterir. Bu salt okunurdur. Verilerin içeri aktarılması sırasında bu alanda yapılan herhangi bir değişiklik yok sayılır.| Beklemede
Reddedilen/kayıp nedeni|Şekline| Bu bilgileri yalnızca, alanın alt durumunu reddedilmiş veya kayıp olarak değiştiriyorsanız sağlamanız gerekir. Bu sütunu, aksi takdirde yoksayabilirsiniz. <br/> **Aşağıdaki seçeneklere göre bir sayı girin** <br/><br/> **1**-Project bütçe yeterli değil  <br/> **2**-müşteri yanıt vermedi  <br/> **3**-müşteri başka bir satıcı seçti  <br/> **4** -müşteri gereksinimi karşılanmadı  <br/> **5** -müşteri değil <br/> **6**-önerilen zaman satırı çok kısa <br/> **7** -kötüye kullanma, istenmeyen posta veya kimlik avı olarak raporla <br/> **8** -diğerleri |6|
Satış Aşaması|No|Bu, başvurunun ayrıntılı satış aşamasını belirten alandır. Satış aşamaları hakkında [buradan](./manage-co-sell-opportunities.md) daha fazla bilgi edinin|40
Tahmini anlaşma değeri|Yes|Müşteriyle ilk konuşmaları temel alan işlem değeri. Bu, bu durum, işlem, **kazanılan** veya kaybolan Terminal durumlarından birine ulaştığında değiştirilebilir **.**|12563
Para Birimi|Yes|Anlaşma değerinin girildiği para birimi. Para birimi kodlarını [buradan](https://en.wikipedia.org/wiki/ISO_4217)bulabilirsiniz.|USD
Tahmini kapanış tarihi|Yes|Müşterinin AA/GG/YYYY biçiminde ilk konuşmaları temel alan tahmini kapanış tarihi. <br/> **Tarih UTC saat diliminde olmalıdır. Iş Ortağı Merkezi Kullanıcı arabiriminde görüntülenen tüm tarihler yerelleştirilmiş Timezones tabanlıdır. UTC saat diliminde tarihi sağladığınız başvuruya bakıyorsanız, Iş Ortağı Merkezi Kullanıcı arabiriminde +/-bir gün farkı olabilir.**|1/30/2020
CRM KIMLIĞI|No|Varsa, CRM sisteminizde bu özel başvurunun tanımlayıcısı. Bu, ücretsiz bir form metin girişi alanıdır.|34234324-sdfsdf-345345-sfd
Pazarlama kampanyası KIMLIĞI|No|Bu alan, bu özel başvurunun sonucu olan pazarlama kampanyasını gösterir. Genellikle ROı hesaplama için kullanılır|BingSummer2020
Notlar|No|Başvuruya ilişkin güncelleştirmeleri gösteren ayrıntılı notlar|Bu örnek bir notdır
Microsoft yardımı gerekli mi?|Yes|Bu, Microsoft 'un bu ortak satış isteğini yaparken size yardımcı olmasını isteyip istemediğinizi belirtir|Yes
Microsoft 'a özgü yardım nedir?|Şekline|Microsoft 'un size yardımcı olabilecek altı farklı yönden biri. Bu yalnızca, "Microsoft Yardım gerekli" sorusu için Evet ' i seçerseniz geçerlidir. " <br/> **Aşağıdaki seçeneklere göre bir sayı girin** <br/><br/> **1**-iş yüküne özgü değer teklifi  <br/> **2**-müşteri teknik mimarisi  <br/> **3**- Kavram kanıtı /Tanıtım  <br/> **4**- Teklifler ve Lisanslama  <br/> **5**- Gönderi - satış müşteri başarısı  <br/> **6**- Genel veya diğer|1|
Microsoft satış ekibiyle paylaşma|Yes|Bu, satış anlaşmasıyla ilgili ayrıntıları Microsoft satış ekibiyle paylaşmak isteyip istemeyebilirsiniz. Bu yalnızca "Microsoft yardımı gerekiyor mu? sorusu için Hayır'ı seçerseniz geçerlidir. "|Yes
Microsoft'a notlar|No|Microsoft'tan yardıma ihtiyacınız varsa Microsoft'a özgü notlar|Contoso müşterisi için POC ile ilgili yardım gerekiyor
Müşteri/İş Ortağı kişisi paylaşma onayı|Yes|Müşterinin iletişim ayrıntılarını ve şirket çalışanlarının anlaşma üzerinde çalışan kişi ayrıntılarını paylaşma onayı. **Bu sütun için Hayır'ı seçerseniz anlaşmalar oluşturulmaz veya güncelleştirilmez.** |Yes
1\. Çözüm|Yes|Çözüm Kimliği (Gerekli), Anlaşma değerinin girilir olduğu para birimi (İsteğe bağlı). Para birimi kodlarını [burada,](https://en.wikipedia.org/wiki/ISO_4217)SKU fiyatı (İsteğe bağlı) ve SKU Miktarı (İsteğe bağlı) bulabilirsiniz  |SOL-1234-PQRS, USD, 10, 100
Takım üyesi 1|Yes|İlgili ekip üyesinin ad, Soyadı, mobil numarası ve e-posta kimliği.| Bob, Partner, 999999, Bob.partner@Contoso.com

## <a name="next-steps"></a>Sonraki adımlar

CRM sistemlerinizin İş Ortağı Merkezi Microsoft ile ortak satış yapmak için bu ortak satış bağlayıcılarını kullanabilirsiniz.

- [Dynamics 365 CRM için ortak satış bağlayıcısı – Genel Bakış](connector-dynamics.md)
- [Salesforce CRM için ortak satış bağlayıcısı - genel bakış](connector-salesforce.md)
