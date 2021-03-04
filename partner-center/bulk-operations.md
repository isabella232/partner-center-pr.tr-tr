---
title: Başvurulardaki Excel dosyaları aracılığıyla toplu Işlemler
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Excel dosyalarını kullanarak ortak satış fırsatlarını indirme, oluşturma veya güncelleştirme hakkında bilgi edinin
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 02/03/2021
ms.openlocfilehash: d601fec4bbdaad72f02c16b399cc320cc607d8ed
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756073"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-valuecsv-files"></a>Virgülle ayrılmış değer (CSV) dosyaları kullanan ortak satış fırsatları için toplu işlemler

**Uygun roller**

- Başvuru Yöneticisi
- Başvuru kullanıcısı

Iş Ortağı Merkezi 'nde toplu işlemler, şirketinizin ortak satış fırsatları verilerini dışarı ve içeri aktarmanıza yardımcı olur. Sayfa başlığı başlığının sağ üst köşesindeki içeri ve dışarı aktarma bağlantılarını bulmak için ortak satış fırsatları sayfasına gidin. Hem **başvuru Yöneticisi** hem de **başvuru Kullanıcı** izinleri olan kullanıcılar bu işlevi kullanabilir.

> [!IMPORTANT]
> Toplu içeri aktarma aracılığıyla gerçekleştirilen oluşturma/güncelleştirme eylemleri geri alınamaz. Çok sayıda kayıt değiştirirken veya oluştururken dikkatli olun. Bir anlaşma oluşturulduktan sonra, alanların yalnızca bir alt kümesi değiştirilebilir. **Herhangi bir anlaşma reddedildi/zaman aşımına uğradı/kazanıldı/kaybedildi gibi bir Terminal durumuna ulaştığında hiçbir eyleme izin verilmez.**

## <a name="exporting-co-sell-opportunities"></a>Ortak satış fırsatlarını dışarı aktarma

Aşağıda dışa aktarma işlevinin ayrıntıları verilmiştir

- Dışarı Aktar düğmesine tıklayarak **en fazla 5000 kaydı** dışarı aktarabilirsiniz.
- İndirilen anlaşmalar erişim düzeylerinizi temel alır. Başvuru yöneticileri ve başvuru kullanıcıları, kapsamlarına bağlı olarak farklı sonuçlar alabilir ve ekipteki ekip üyeleri olarak dahil edebilir. [Başvurular izinleri](permissions-overview.md#manage-referrals)hakkında daha fazla bilgi edinin.
- Dışa aktarma işlevi, ortak satış fırsatları sayfasında geçerli sekmeyi ve uygulanan filtreleri hesaba göre alır.
- Uygulanan filtreleri temel alan tüm verileri içeren bir CSV dosyası oluşturulacaktır.
- Kayıtların indirilmesi bir dakika kadar sürebilir.
- İndirme eyleminin tamamlanmasını beklemeniz gerekmez. Iş Ortağı Merkezi 'nde diğer sayfalara gitseniz bile, dışa aktarma işlevi tamamlandıktan hemen sonra dosya indirilir.
- İndirilen dosyayı, işlem ayrıntılarını değiştirmek ve kayıtları güncelleştirmek üzere karşıya yüklemek için yeniden kullanabilirsiniz.

## <a name="importing-co-sell-opportunities"></a>Ortak satış fırsatlarını içeri aktarma

- İçeri aktarma işlevini kullanarak **en fazla 1000 kayıt** oluşturabilir veya güncelleyebilirsiniz.
- Şablonu, Iş ortağı merkezindeki Içeri aktarma sayfasından indirerek sıfırdan oluşturabilirsiniz.
- Ayrıca, var olan kayıtları indirmek ve güncelleştirmek için dışarı aktarma işlevini de kullanabilirsiniz.
- Dosyada 1000 'den fazla kayıt varsa, işlem işlenemiyor.
- Dosya işlendikten sonra, oluşturulan, güncellenen ve işlenmemiş başvuruların sayısına sahip bir Özet, son işlem dosyası kartında gösterilir.
- İşlenen kayıtların ayrıntılarını indirebilir, hataları giderebilir ve önceki çalıştırmada başarısız olan kayıtları oluşturmak veya güncelleştirmek için aynı dosyayı karşıya yükleyebilirsiniz. **Önceki çalıştırmada başarısız olan düzeltilen kayıtları karşıya yüklemeden önce dosyadaki tüm başarılı kayıtları kaldırın.**
- Daha fazla çözüm eklemek için, çözüm 1 ' in yanına ek sütunlar ekleyin ve sütun adını çözüm X olarak kullanın; burada X, anlaşma içindeki çözümün numarasını temsil eder. Örneğin, çözüm 2, çözüm 3.
- Bir başa 50 çözüm ekleyebilirsiniz.
- Daha fazla takım üyesi eklemek için, takım üyesi 1 ' in yanına ek sütunlar ekleyin ve sütun adını takım üyesi X olarak kullanın; burada X, anlaşma içindeki takım üyesinin numarasını temsil eder. Örneğin, takım üyesi 2, takım üyesi 3.
- Bir anlaşma için en fazla 50 takım üyesi ekleyebilirsiniz.

> [!NOTE]
> İşlemin tamamlanmasını beklemeniz gerekmez. İşlenen son dosyanın ayrıntıları, işlem tamamlandıktan sonra indirilecektir. **1000 kayıtla dosya yüklüyorsanız, bu işlem 10 dakikaya kadar sürebilir.**

> [!IMPORTANT]
> Tüm yönergeleri dikkatle okuyun ve Iş Ortağı Merkezi 'nde CSV dosyalarını kullanarak anlaşmalar oluşturmadan veya güncelleştirmeden önce aşağıdaki tablodaki her bir sütunun biçimini denetleyin.

|**Sütun adı**|**Zorunlu mu?**|**Açıklama**|**Örnek değer (ler)**|
|-----|:-----|:---------|:---|
Hatalar|Hayır|Başvurular için oluşturma/güncelleştirme işlemleriyle ilgili varsa hatalar bu sütuna dahil edilir. Birden çok hata varsa, bunların hepsi noktalı virgülle ayrılmış olarak listelenir.|Zorunlu alan çözümü 1 eksik|
Katılım KIMLIĞI|Hayır|Katılım KIMLIĞI, Microsoft iş ortağı merkezi başvuruları sistemi tarafından oluşturulur. Yeni başvuru oluşturma için gerekli değildir. Bir kaydı güncelleştiriyorsanız, var olan katılım KIMLIĞINI kullanabilirsiniz.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
Referans kimliği|Hayır|Başvuru KIMLIĞI, Microsoft iş ortağı merkezi başvuruları sistemi tarafından oluşturulur. Yeni başvuru oluşturma için gerekli değildir. Mevcut bir kaydı güncelleştiriyorsanız, bunu referans KIMLIĞIYLE doldurabilirsiniz.|ebacdkdc-0b84-4ac4-B4EA-5b2587d42cee
Anlaşma adı|Yes|Başvurunuz için anlaşma için kolay ad.|UK yay
Müşteri Adı|Yes|Müşteri şirketinin adı. Microsoft tarafında hızlı eşleştirme için kuruluşun yasal adını kullanın.|Contoso Corporation
Müşteri adresi satırı 1|Yes|Müşteri şirketinin Adres satırı 1. |Tek contoso yöntemi
Müşteri adresi satırı 2|Hayır|Müşteri şirketinin Adres satırı 2.|NE 148 Caddesi
Müşteri şehri|Yes|Müşteri kuruluşunun bulunduğu şehir.|Redmond
Müşteri durumu|Hayır|Müşteri kuruluşunun bulunduğu eyalet.|Washington
Müşteri posta kodu|Hayır|Müşteri kuruluşunun bulunduğu bölgenin posta kodu.|98052
Müşteri ülkesi|Yes|Müşteri kuruluşunun bulunduğu ülke/bölge. [Burada]( https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes)bahsedilen iki harfli ülke kodlarını kullanın.|ABD
Müşteri D-U-N-S KIMLIĞI|Hayır|Müşteri kuruluşunun DÇALıŞTıRAL KIMLIĞINI getirmeye çalışın. Bu, daha hızlı satıcı atamasına yardımcı olan Microsoft tarafında müşteri kuruluşunun daha hızlı eşleştirmesine yardımcı olur. DBIR ID 'yi bu [Web SITESINDEN](https://www.dnb.com/duns-number/lookup.html)ücretsiz edinebilirsiniz.|81466849
Müşterinin kişi adı soyadı|Şekline|İlk adı yalnızca Microsoft Yardım 'a ihtiyacınız varsa zorunludur. Müşteri kuruluşundan bu anlaşma üzerinde çalışan birincil kişinin adı.|John
Müşterinin kişi adı soyadı|Şekline|Soyadı yalnızca Microsoft Yardım gerekirse zorunludur. Bu anlaşma üzerinde çalışan müşteri kuruluşundan birincil kişinin soyadı.|Müşteri
Müşteri Irtibat telefon numarası|Şekline|Telefon numarası yalnızca Microsoft Yardım gerekirse zorunludur. Müşteri kuruluşundan bu anlaşma üzerinde çalışan birincil ilgili kişinin telefon numarası.|9999999999
Müşteri Iletişim e-posta adresi|Şekline|E-posta adresi yalnızca Microsoft Yardım 'a ihtiyacınız varsa zorunludur. Bu anlaşma üzerinde çalışan müşteri kuruluşundan birincil kişinin e-posta adresi.|john.customer@contoso.com
İş ortağı başvuru durumu|Yes|Şirketinizin perspektifinden ilgili durumunu gösterir. Bir başvuruyu oluşturmaya veya değiştirmeye çalıştığınızda gereklidir. Yeni bir anlaşma oluşturmaya çalışıyorsanız **Yeni** ' ye kullanın. Kabul edilen değerler [burada](/partner/develop/referral-resources#referralstatus)belgelenmiştir.|Etkin
İş ortağı başvurusu alt durumu|Yes|İşlem durumunun tam durumunu gösterir. Yeni bir anlaşma oluşturmaya çalışıyorsanız **kabul edildi** ' i kullanın. Mevcut bir başvuruyu değiştiriyorsanız de gereklidir. Kabul edilen değerler [burada](/partner/develop/referral-resources#referralsubstatus)belgelenmiştir.|Kabul edildi
Microsoft başvuru durumu|Şekline|Microsoft arama yardımı 'na gönderdiğiniz ortak satış isteğinin durumunu gösterir. Bu salt okunurdur. Verilerin içeri aktarılması sırasında bu alanda yapılan herhangi bir değişiklik yok sayılır.| Beklemede
Reddedilen/kayıp nedeni|Şekline| Bu bilgileri yalnızca, alanın alt durumunu reddedilmiş veya kayıp olarak değiştiriyorsanız sağlamanız gerekir. Bu sütunu, aksi takdirde yoksayabilirsiniz. <br/> **Aşağıdaki seçeneklere göre bir sayı girin** <br/><br/> **1**-proje bütçesi yeterli değil  <br/> **2**-müşteri yanıt vermedi  <br/> **3**-müşteri başka bir satıcı seçti  <br/> **4** -müşteri gereksinimi karşılanmadı  <br/> **5** -müşteri değil <br/> **6**-önerilen zaman satırı çok kısa <br/> **7** -kötüye kullanma, istenmeyen posta veya kimlik avı olarak raporla <br/> **8** -diğerleri |6|
Satış Aşaması|Hayır|Bu, başvurunun ayrıntılı satış aşamasını belirten alandır. Satış aşamaları hakkında [buradan](./manage-co-sell-opportunities.md) daha fazla bilgi edinin|40
Tahmini anlaşma değeri|Yes|"Müşteri ile ilk konuşmaları temel alan işlem değeri. Bu, anlaşma Terminal durumlarından birine ulaşana kadar değiştirilebilir| kazanıldı veya kaybedildi. "|12563
Para Birimi|Yes|Anlaşma değerinin girildiği para birimi. Para birimi kodlarını [buradan](https://en.wikipedia.org/wiki/ISO_4217)bulabilirsiniz.|USD
Tahmini kapanış tarihi|Yes|Müşterinin AA/GG/YYYY biçiminde ilk konuşmaları temel alan tahmini kapanış tarihi. <br/> **Tarih UTC saat diliminde olmalıdır. Iş Ortağı Merkezi Kullanıcı arabiriminde görüntülenen tüm tarihler yerelleştirilmiş Timezones tabanlıdır. UTC saat diliminde tarihi sağladığınız başvuruya bakıyorsanız, Iş Ortağı Merkezi Kullanıcı arabiriminde +/-bir gün farkı olabilir.**|1/30/2020
CRM KIMLIĞI|Hayır|Varsa, CRM sisteminizde bu özel başvurunun tanımlayıcısı. Bu, ücretsiz bir form metin girişi alanıdır.|34234324-sdfsdf-345345-sfd
Pazarlama kampanyası KIMLIĞI|Hayır|Bu alan, bu özel başvurunun sonucu olan pazarlama kampanyasını gösterir. Genellikle ROı hesaplama için kullanılır|BingSummer2020
Notlar|Hayır|Başvuruya ilişkin güncelleştirmeleri gösteren ayrıntılı notlar|Bu örnek bir notdır
Microsoft yardımı gerekli mi?|Yes|Bu, Microsoft 'un bu ortak satış isteğini yaparken size yardımcı olmasını isteyip istemediğinizi belirtir|Yes
Microsoft 'a özgü yardım nedir?|Şekline|Microsoft 'un size yardımcı olabilecek altı farklı yönden biri. Bu yalnızca, "Microsoft yardımı gerekli" sorusu için Hayır 'ı seçerseniz geçerlidir. " <br/> **Aşağıdaki seçeneklere göre bir sayı girin** <br/><br/> **1**-iş yüküne özgü değer teklifi  <br/> **2**-müşteri teknik mimarisi  <br/> **3**-kavram kanıtı/demo  <br/> **4**-teklifler ve lisanslama  <br/> **5**-satış sonrası müşteri başarısı  <br/> **6**-genel veya diğer|1|
Microsoft Sales Team ile paylaşma|Yes|Bu, Microsoft satış ekibi ile ilgilenmenin ayrıntılarını paylaşmak isteyip istemediğinizi belirtmek için kullanılır. Bu yalnızca, "Microsoft yardımı gerekli" sorusu için Hayır 'ı seçerseniz geçerlidir. "|Yes
Microsoft 'a notlar|Hayır|Microsoft 'a yönelik yardıma ihtiyacınız varsa Microsoft 'a özgü notlar|Contoso müşterisi için POC ile ilgili yardım gerekiyor
Müşteri/Iş ortağı ilgili kişisini paylaşma onayı|Yes|Müşteri iletişim ayrıntılarını ve şirketinizin çalışanlarınızı paylaşma onayı, anlaşma üzerinde çalışan ayrıntıları ile iletişim kurun. **Bu sütun için Hayır ' ı seçerseniz anlaşmalar oluşturulmaz veya güncellenmez.** |Yes
Çözüm 1|Yes|Çözüm KIMLIĞI (gerekli), anlaşma değerinin girildiği para birimi (Isteğe bağlı). Döviz cinslerini [buradan](https://en.wikipedia.org/wiki/ISO_4217), SKU 'nun fiyatını (isteğe bağlı) ve SKU 'nun miktarına (isteğe bağlı) ulaşabilirsiniz.  |NUEVO-1234-PQRS, USD, 10, 100
Takım üyesi 1|Yes|İlgili takım üyesinin adı, soyadı, cep telefonu numarası ve e-posta KIMLIĞI.| Bob, Iş ortağı, 999999, Bob.partner@Contoso.com