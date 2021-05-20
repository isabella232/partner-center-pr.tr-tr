---
title: Başvurulardaki Excel/CSV dosyaları aracılığıyla ortak satış fırsatlarını toplu dışa aktarma ve içeri aktarma
description: Iş Ortağı Merkezi 'nde Excel (CSV) dosyalarını kullanarak ortak satış fırsatlarını indirme, oluşturma veya güncelleştirme hakkında bilgi edinin
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 02/03/2021
ms.openlocfilehash: af567b9b8b36841b6e6fd7e18a34e1c4b6b81f2e
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149171"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-value-csv-files"></a>Virgülle ayrılmış değer (CSV) dosyaları kullanan ortak satış fırsatları için toplu işlemler

**Uygun roller**: başvuru Yöneticisi | Başvuru kullanıcısı

Iş Ortağı Merkezi 'nde toplu işlemler, şirketinizin ortak satış fırsatları verilerini dışa ve içe aktarmanıza yardımcı olur. Sayfa başlığı başlığının sağ üst köşesindeki **içeri** ve **dışarı aktarma** bağlantılarını bulmak için **ortak satış fırsatları** sayfasına gidin. Hem **başvuru Yöneticisi** hem de **başvuru Kullanıcı** izinleri olan kullanıcılar bu işlevi kullanabilir.

> [!IMPORTANT]
> Toplu içeri aktarma aracılığıyla gerçekleştirilen oluşturma/güncelleştirme eylemleri geri alınamaz. Çok sayıda kayıt değiştirirken veya oluştururken dikkatli olun. Bir anlaşma oluşturulduktan sonra, alanların yalnızca bir alt kümesi değiştirilebilir. **Herhangi bir anlaşma reddedildi/zaman aşımına uğradı/kazanıldı/kaybedildi gibi bir Terminal durumuna ulaştığında hiçbir eyleme izin verilmez.**

## <a name="export-co-sell-opportunities"></a>Ortak satış fırsatlarını dışarı aktarma

Aşağıdaki bilgiler dışa aktarma işlevini açıklar:

- **Dışarı aktar** düğmesine tıklayarak **en fazla 5000 kaydı** dışarı aktarabilirsiniz.
- İndirilen anlaşmalar erişim düzeylerinizi temel alır. Başvuru yöneticileri ve başvuru kullanıcıları, kapsamlarına bağlı olarak farklı sonuçlar alabilir ve ekipteki ekip üyeleri olarak dahil edebilir. [Başvurular izinleri](permissions-overview.md#manage-referrals)hakkında daha fazla bilgi edinin.
- Dışa aktarma işlevi, ortak satış fırsatları sayfasında geçerli sekmeyi ve uygulanan filtreleri hesaba göre alır.
- Uygulanan filtreleri temel alan tüm verileri içeren bir CSV dosyası oluşturulacaktır.
- Kayıtların indirilmesi bir dakika kadar sürebilir.
- İndirme eyleminin tamamlandıktan sonra tamamlanır. Uygulama içinde diğer sayfalara İş Ortağı Merkezi bile, dışarı aktarma işlevi tamamlandıktan hemen sonra dosya indirilir.
- Anlaşma ayrıntılarını değiştirmek ve tüm kayıtları güncelleştirmek için karşıya yüklemek üzere indirilen dosyayı yeniden kullanabilirsiniz.

## <a name="import-co-sell-opportunities"></a>Ortak satış fırsatlarını içeri aktarma

- İçeri aktarma işlevini kullanarak en **fazla 1000 kayıt oluşturabilir** veya güncelleştirin.
- Şablonu, uygulamanın İçeri Aktar sayfasından indirerek sıfırdan İş Ortağı Merkezi.
- Var olan kayıtları indirmek ve güncelleştirmek için Dışarı Aktar işlevini de kullanabilirsiniz.
- Dosyada 1000'den fazla kayıt varsa işlenemez.
- Dosya işlendikten sonra, oluşturulan, güncelleştirilen ve işlenmemiş olan referansların sayısının bir özeti son işlem dosyası kartında gösterilir.
- İşlenen kayıtların ayrıntılarını indirebilir, hataları düzeltebilir ve önceki çalıştırmada başarısız olan kayıtları oluşturmak veya güncelleştirmek için aynı dosyayı karşıya yükleyebilirsiniz. **Önceki çalıştırmada başarısız olan düzeltilmiş kayıtları karşıya yüklemeden önce dosyadan tüm başarılı kayıtları kaldırın.**
- Daha fazla çözüm eklemek için çözüm 1'in yanına ek sütunlar ekleyin ve sütun adını Çözüm X olarak kullanın. Burada X, anlaşmadaki çözüm sayısını temsil eder. Örneğin, Çözüm 2, Çözüm 3.
- Bir anlaşma için en fazla 50 çözüm ekleme.
- Daha fazla takım üyesi eklemek için, Takım üyesi 1'in yanına ek sütunlar ekleyin ve sütun adını Takım üyesi X olarak kullanın; burada X, anlaşmadaki takım üyesinin sayısını temsil eder. Örneğin, Takım üyesi 2, Takım üyesi 3.
- Anlaşma için en fazla 50 ekip üyesi ekleme.

> [!NOTE]
> İşlemenin tamamlandıktan sonra tamamlanır. İşlem tamamlandıktan sonra son işlenen dosyanın ayrıntıları indirilebilir. **1000 kaydı olan dosyaları karşıya yüklerken bu süre 10 dakika kadar sürebilir.**

> [!IMPORTANT]
> Tüm yönergeleri dikkatle okuyun ve Iş Ortağı Merkezi 'nde CSV dosyalarını kullanarak anlaşmalar oluşturmadan veya güncelleştirmeden önce aşağıdaki tablodaki her bir sütunun biçimini denetleyin.

|**Sütun adı**|**Zorunlu mu?**|**Açıklama**|**Örnek değer (ler)**|
|-----|:-----|:---------|:---|
Hatalar|No|Başvurular için oluşturma/güncelleştirme işlemleriyle ilgili varsa hatalar bu sütuna dahil edilir. Birden çok hata varsa, bunların hepsi noktalı virgülle ayrılmış olarak listelenir.|Zorunlu alan çözümü 1 eksik|
Katılım KIMLIĞI|No|Katılım KIMLIĞI, Microsoft iş ortağı merkezi başvuruları sistemi tarafından oluşturulur. Yeni başvuru oluşturma için gerekli değildir. Bir kaydı güncelleştiriyorsanız, var olan katılım KIMLIĞINI kullanabilirsiniz.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
Referans kimliği|No|Başvuru KIMLIĞI, Microsoft iş ortağı merkezi başvuruları sistemi tarafından oluşturulur. Yeni başvuru oluşturma için gerekli değildir. Mevcut bir kaydı güncelleştiriyorsanız, bunu referans KIMLIĞIYLE doldurabilirsiniz.|ebacdkdc-0b84-4ac4-B4EA-5b2587d42cee
Anlaşma adı|Yes|Başvurunuz için anlaşma için kolay ad.|UK yay
Müşteri Adı|Yes|Müşteri şirketinin adı. Microsoft tarafında hızlı eşleştirme için kuruluşun yasal adını kullanın.|Contoso Corporation
Müşteri adresi satırı 1|Yes|Müşteri şirketinin Adres satırı 1. |Tek contoso yöntemi
Müşteri adresi satırı 2|No|Müşteri şirketinin Adres satırı 2.|NE 148 Caddesi
Müşteri şehri|Yes|Müşteri kuruluşunun bulunduğu şehir.|Redmond
Müşteri durumu|No|Müşteri kuruluşunun bulunduğu eyalet.|Washington
Müşteri posta kodu|No|Müşteri kuruluşunun bulunduğu bölgenin posta kodu.|98052
Müşteri ülkesi|Yes|Müşteri kuruluşunun bulunduğu ülke/bölge. [Burada]( https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes)bahsedilen iki harfli ülke kodlarını kullanın.|ABD
Müşteri D-U-N-S KIMLIĞI|No|Müşteri kuruluşunun DÇALıŞTıRAL KIMLIĞINI getirmeye çalışın. Bu, daha hızlı satıcı atamasına yardımcı olan Microsoft tarafında müşteri kuruluşunun daha hızlı eşleştirmesine yardımcı olur. DBIR ID 'yi bu [Web SITESINDEN](https://www.dnb.com/duns-number/lookup.html)ücretsiz edinebilirsiniz.|81466849
Müşterinin kişi adı soyadı|Şekline|İlk adı yalnızca Microsoft Yardım 'a ihtiyacınız varsa zorunludur. Müşteri kuruluşundan bu anlaşma üzerinde çalışan birincil kişinin adı.|John
Müşterinin kişi adı soyadı|Şekline|Soyadı yalnızca Microsoft Yardım gerekirse zorunludur. Bu anlaşma üzerinde çalışan müşteri kuruluşundan birincil kişinin soyadı.|Müşteri
Müşteri Irtibat telefon numarası|Şekline|Telefon numarası yalnızca Microsoft Yardım gerekirse zorunludur. Müşteri kuruluşundan bu anlaşma üzerinde çalışan birincil ilgili kişinin telefon numarası.|9999999999
Müşteri Iletişim e-posta adresi|Şekline|E-posta adresi yalnızca Microsoft Yardım 'a ihtiyacınız varsa zorunludur. Bu anlaşma üzerinde çalışan müşteri kuruluşundan birincil kişinin e-posta adresi.|john.customer@contoso.com
İş ortağı başvuru durumu|Yes|Şirketin bakış açısından anlaşma durumunu gösterir. Referans oluşturma veya değiştirme denemesi yapmak için gereklidir. Yeni **bir** satış anlaşması oluşturmak için Yeni'leri kullanın. Kabul edilen değerler burada [belgelenmiştir.](/partner/develop/referral-resources#referralstatus)|Etkin
İş Ortağı Referansı Alt İstatistikleri|Yes|Anlaşmanın tam durumunu gösterir. Yeni **bir anlaşma** oluşturmak için Kabul Edildi'i kullanın. Mevcut bir referansı değiştirirken de gereklidir. Kabul edilen değerler burada [belgelenmiştir.](/partner/develop/referral-resources#referralsubstatus)|Kabul edildi
Microsoft Referans Durumu|-sına bağ -lıdır|Yardım almak için Microsoft'a gönderdiğiniz ortak satış isteğinin durumunu gösterir. Bu salt okunur bir alandır. Veriler içeri aktarılırken bu alanda yapılan tüm değişiklik yoksayılır.| Beklemede
Reddedildi/Neden kaybedildi|-sına bağ -lıdır| Bu bilgileri yalnızca alanınıza ilişkin alt durumu Reddedildi veya Kayıp olarak değiştirerek sağlamanız gerekir. Aksi takdirde bu sütunu yoksayabilirsiniz. <br/> **Aşağıdaki seçeneklere göre bir sayı girin** <br/><br/> **1**- Proje bütçesi yeterli değil  <br/> **2**-müşteri yanıt vermedi  <br/> **3**-müşteri başka bir satıcı seçti  <br/> **4** -müşteri gereksinimi karşılanmadı  <br/> **5** -müşteri değil <br/> **6**-önerilen zaman satırı çok kısa <br/> **7** -kötüye kullanma, istenmeyen posta veya kimlik avı olarak raporla <br/> **8** -diğerleri |6|
Satış Aşaması|No|Bu, başvurunun ayrıntılı satış aşamasını belirten alandır. Satış aşamaları hakkında [buradan](./manage-co-sell-opportunities.md) daha fazla bilgi edinin|40
Tahmini anlaşma değeri|Yes|Müşteriyle ilk konuşmaları temel alan işlem değeri. Bu, bu durum, işlem, **kazanılan** veya kaybolan Terminal durumlarından birine ulaştığında değiştirilebilir **.**|12563
Para Birimi|Yes|Anlaşma değerinin girildiği para birimi. Para birimi kodlarını [buradan](https://en.wikipedia.org/wiki/ISO_4217)bulabilirsiniz.|USD
Tahmini kapanış tarihi|Yes|Müşterinin AA/GG/YYYY biçiminde ilk konuşmaları temel alan tahmini kapanış tarihi. <br/> **Tarih UTC saat diliminde olmalıdır. Iş Ortağı Merkezi Kullanıcı arabiriminde görüntülenen tüm tarihler yerelleştirilmiş Timezones tabanlıdır. UTC saat diliminde tarihi sağladığınız başvuruya bakıyorsanız, Iş Ortağı Merkezi Kullanıcı arabiriminde +/-bir gün farkı olabilir.**|1/30/2020
CRM KIMLIĞI|No|Varsa CRM sisteminize bu referansı tanımlayıcı. Bu, serbest biçimli bir metin girişi alanıdır.|34234324-sdfsdf-345345-sfd
Pazarlama Kampanyası Kimliği|No|Bu alan, pazarlama kampanyasının bu referansla sonuçlanmasına neden olduğunu gösterir. Genellikle yatırım getiri hesaplaması için kullanılır|BingSummer2020
Notlar|No|Referansla ilgili güncelleştirmeleri gösteren ayrıntılı notlar|Bu örnek bir not
Microsoft yardım gerekiyor mu?|Yes|Bu, Microsoft'un bu ortak satış isteği için size yardımcı olup olmadığını belirtmektir|Yes
Microsoft'tan hangi özel yardım?|-sına bağ -lıdır|Microsoft'un size yardımcı olmak için altı farklı yoldan biri. Bu yalnızca "Microsoft yardımı gerekiyor mu? sorusu için Evet'i seçerseniz geçerlidir. " <br/> **Aşağıdaki seçeneklere göre bir sayı girin** <br/><br/> **1**- İş yükü - belirli bir değer teklifi  <br/> **2**- Müşteri teknik mimarisi  <br/> **3**- Kavram kanıtı /Tanıtım  <br/> **4**- Teklifler ve Lisanslama  <br/> **5**-satış sonrası müşteri başarısı  <br/> **6**-genel veya diğer|1|
Microsoft Sales Team ile paylaşma|Yes|Bu, Microsoft satış ekibi ile ilgilenmenin ayrıntılarını paylaşmak isteyip istemediğinizi belirtmek için kullanılır. Bu yalnızca, "Microsoft yardımı gerekli" sorusu için Hayır 'ı seçerseniz geçerlidir. "|Yes
Microsoft 'a notlar|No|Microsoft 'a yönelik yardıma ihtiyacınız varsa Microsoft 'a özgü notlar|Contoso müşterisi için POC ile ilgili yardım gerekiyor
Müşteri/Iş ortağı ilgili kişisini paylaşma onayı|Yes|Müşteri iletişim ayrıntılarını ve şirketinizin çalışanlarınızı paylaşma onayı, anlaşma üzerinde çalışan ayrıntıları ile iletişim kurun. **Bu sütun için Hayır ' ı seçerseniz anlaşmalar oluşturulmaz veya güncellenmez.** |Yes
Çözüm 1|Yes|Çözüm KIMLIĞI (gerekli), anlaşma değerinin girildiği para birimi (Isteğe bağlı). Döviz cinslerini [buradan](https://en.wikipedia.org/wiki/ISO_4217), SKU 'nun fiyatını (isteğe bağlı) ve SKU 'nun miktarına (isteğe bağlı) ulaşabilirsiniz.  |NUEVO-1234-PQRS, USD, 10, 100
Takım üyesi 1|Yes|İlgili takım üyesinin adı, soyadı, cep telefonu numarası ve e-posta KIMLIĞI.| Bob, Iş ortağı, 999999, Bob.partner@Contoso.com

## <a name="next-steps"></a>Sonraki adımlar

Bu Iş Ortağı Merkezi ortak satış bağlayıcılarını, CRM sistemlerinizden Microsoft ile birlikte satın almak için kullanabilirsiniz.

- [Dynamics 365 CRM için ortak satış Bağlayıcısı – genel bakış](connector-dynamics.md)
- [Salesforce için ortak satış Bağlayıcısı CRM-genel bakış](connector-salesforce.md)
