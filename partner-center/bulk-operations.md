---
title: Referanslar'da csv dosyalarını kullanarak ortak satış fırsatlarını toplu Excel ve içeri aktarma
description: Excel (CSV) dosyalarını kullanarak ortak satış fırsatlarını indirmeyi, oluşturmayı veya güncelleştirmeyi İş Ortağı Merkezi
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 02/03/2021
ms.openlocfilehash: 15739d382d736fc9b98b1f9a1f2331f99d6ddeaf
ms.sourcegitcommit: 815760499700bf2c947550524cbddd091622081f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "121915436"
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
- Şablonu, uygulama sayfasındaki İçeri Aktar sayfasından indirerek sıfırdan İş Ortağı Merkezi.
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
> Tüm yönergeleri dikkatle okuyun ve aşağıdaki tabloda yer alan her sütunun biçimini, aşağıdaki tabloda yer alan CSV dosyalarını kullanarak satış anlaşmalarını oluşturmadan veya güncelleştirmeden İş Ortağı Merkezi.

|**Sütun adı**|**Zorunlu mu?**|**Açıklama**|**Örnek değer(ler)**|
|-----|:-----|:---------|:---|
Hatalar|Hayır|Başvurulara yönelik w.r.t oluşturma/güncelleştirme işlemleriyle ilgili hatalar bu sütuna dahil edilir. Birden çok hata varsa bunların hepsi noktalı virgülle ayrılmış olarak listelenir.|Zorunlu alan Çözüm 1 eksik|
Katılım Kimliği|Hayır|Katılım kimliği, Microsoft İş Ortağı Merkezi tarafından oluşturulur. Yeni referans oluşturma için gerekli değildir. Bir kaydı güncelleştiriyorsanız mevcut katılım kimliğini kullanabilirsiniz.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
Referans kimliği|Hayır|Referans kimliği, Microsoft İş Ortağı Merkezi sistemi tarafından oluşturulur. Yeni referans oluşturma için gerekli değildir. Mevcut bir kaydı güncelleştiriyorsanız referans kimliğiyle doldurun.|ebacdkdc-0b84-4ac4-b4ea-5b2587d42cee
Anlaşma Adı|Yes|Başvuru için anlaşmanın kolay adı.|Birleşik Krallık spring deal
Müşteri Adı|Yes|Müşteri şirketinin adı. Microsoft tarafında hızlı eşleştirme için kuruluşun yasal adını kullanın.|Contoso Corporation
Müşteri Adres Satırı 1|Yes|Müşteri şirketinin adres satırı 1. |Tek Contoso Yolu
Müşteri Adres Satırı 2|Hayır|Müşteri şirketinin 2. adres satırı.|NE 148 sokağı
Customer City|Yes|Müşteri kuruluşlarının bulunduğu şehir.|Redmond
Müşteri Durumu|Hayır|Müşteri kuruluşlarının bulunduğu yeri ifade.|Washington
Müşteri Posta Kodu|Hayır|Müşteri kuruluşlarının bulunduğu bölgenin Posta Kodu.|98052
Müşteri Ülkesi|Yes|Müşteri kuruluşlarının bulunduğu Ülke/Bölge. Burada belirtildiği gibi iki harfli ülke kodlarını [kullanın.]( https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes)|ABD
Müşteri D-U-N-S Kimliği|Hayır|Müşteri kuruluşlarının DUNS kimliğini getirmeye çalışma. Bu, Microsoft tarafında müşteri kuruluşlarının daha hızlı eşleşmesi için yardımcı olur ve bu da satıcı atamalarının daha hızlı tamamlansa da yardımcı olur. BU web sitesinden ÜCRETSİZ OLARAK DUNS ID [edinebilirsiniz.](https://www.dnb.com/duns-number/lookup.html)|81466849
Müşteri Kişisi Adı|-sına bağ -lıdır|Ad yalnızca Microsoft yardıma ihtiyacınız varsa zorunludur. Bu anlaşma üzerinde çalışan müşteri kuruluşundan birincil ilgili kişinin adı.|John
Müşteri Kişisi Soyadı|-sına bağ -lıdır|Soyadı yalnızca Microsoft yardıma ihtiyacınız varsa zorunludur. Bu anlaşma üzerinde çalışan müşteri kuruluşundan birincil ilgili kişinin soyadı.|Müşteri
Müşteri İletişim Telefon numarası|-sına bağ -lıdır|Telefon numarası yalnızca Microsoft yardıma ihtiyacınız varsa zorunludur. Telefon satış anlaşması üzerinde çalışan müşteri kuruluşundan birincil ilgili kişinin numarasını girin.|9999999999
Müşteri İletişim e-posta Adresi|-sına bağ -lıdır|E-posta adresi yalnızca Microsoft yardıma ihtiyacınız varsa zorunludur. Bu anlaşma üzerinde çalışan müşteri kuruluşundan birincil ilgili kişinin e-posta adresi.|john.customer@contoso.com
İş Ortağı Referans Durumu|Yes|Şirketin bakış açısından anlaşma durumunu gösterir. Referans oluşturma veya değiştirme denemesi yapmak için gereklidir. Yeni **bir** satış anlaşması oluşturmak için Yeni'leri kullanın. Kabul edilen değerler burada [belgelenmiştir.](/partner/develop/referral-resources#referralstatus)|Etkin
İş Ortağı Referansı Alt İstatistikleri|Yes|Anlaşmanın tam durumunu gösterir. Yeni **bir anlaşma** oluşturmak için Kabul Edildi'i kullanın. Mevcut bir referansı değiştirirken de gereklidir. Kabul edilen değerler burada [belgelenmiştir.](/partner/develop/referral-resources#referralsubstatus)|Kabul edildi
Microsoft Referans Durumu|-sına bağ -lıdır|Yardım almak için Microsoft'a gönderdiğiniz ortak satış isteğinin durumunu gösterir. Bu salt okunur bir alandır. Veriler içeri aktarılırken bu alanda yapılan tüm değişiklik yoksayılır.| Beklemede
Reddedildi/Neden kaybedildi|-sına bağ -lıdır| Bu bilgileri yalnızca alanınıza ilişkin alt durumu Reddedildi veya Kayıp olarak değiştirerek sağlamanız gerekir. Aksi takdirde bu sütunu yoksayabilirsiniz. <br/> **Aşağıdaki seçeneklere göre bir sayı girin** <br/><br/> **1**- Project bütçe yeterli değil  <br/> **2**- Müşteri yanıt vermedi  <br/> **3**- Müşteri başka bir satıcı seçti  <br/> **4** - Müşteri gereksinimi karşılanmaz  <br/> **5** - Müşteri değil <br/> **6**- Önerilen zaman çizgisi çok kısa <br/> **7** - Kötüye kullanım, istenmeyen posta veya kimlik avı olarak bildirme <br/> **8** - Diğer |6|
Satış Aşaması|Hayır|Bu, referans için ayrıntılı satış aşamalarını gösteren alandır. Satış aşamaları hakkında daha fazla bilgi için buraya [tıklayın](./manage-co-sell-opportunities.md)|40
Tahmini Satış Değeri|Yes|Müşteriyle yapılan ilk konuşmaları temel alan satış anlaşması değeri. Anlaşma kazanildi veya kaybedildi terminal durumlarından biri olana kadar bu **değiştirilebilir.** |12563
Para Birimi|Yes|Anlaşma değerinin girilir olduğu para birimi. Para birimi kodlarını burada [bulabilirsiniz.](https://en.wikipedia.org/wiki/ISO_4217)|USD
Tahmini Kapatma Tarihi|Yes|AA/D/YYYY biçiminde müşteriyle yapılan ilk konuşmaları temel alarak satış anlaşması tahmini kapanış tarihi. <br/> **Tarih UTC saat diliminde olmalıdır. Kullanıcı arabiriminde görüntülenen İş Ortağı Merkezi tarihler yerelleştirilmiş saat dilimlerini temel almaktadır. UTC saat diliminde tarihi temin edilen referansa bakıyorsanız kullanıcı arabiriminde +/- İş Ortağı Merkezi bir gün fark olabilir.**|1/30/2020
CRM Kimliği|Hayır|Varsa CRM sisteminize bu referansı tanımlayıcı. Bu, serbest biçimli bir metin girişi alanıdır.|34234324-sdfsdf-345345-sfd
Pazarlama Kampanyası Kimliği|Hayır|Bu alan, pazarlama kampanyasının bu referansla sonuçlanmasına neden olduğunu gösterir. Genellikle yatırım getiri hesaplaması için kullanılır|BingSummer2020
Notlar|Hayır|Referansla ilgili güncelleştirmeleri gösteren ayrıntılı notlar|Bu örnek bir not
Microsoft yardım gerekiyor mu?|Yes|Bu, Microsoft'un bu ortak satış isteği için size yardımcı olup olmadığını belirtmektir|Yes
Microsoft'tan hangi özel yardım?|-sına bağ -lıdır|Microsoft'un size yardımcı olmak için altı farklı yoldan biri. Bu yalnızca "Microsoft yardımı gerekiyor mu? sorusu için Evet'i seçerseniz geçerlidir. " <br/> **Aşağıdaki seçeneklere göre bir sayı girin** <br/><br/> **1**- İş yükü - belirli bir değer teklifi  <br/> **2**- Müşteri teknik mimarisi  <br/> **3**-kavram kanıtı/demo  <br/> **4**-teklifler ve lisanslama  <br/> **5**-satış sonrası müşteri başarısı  <br/> **6**-genel veya diğer|1|
Microsoft Sales Team ile paylaşma|Yes|Bu, Microsoft satış ekibi ile ilgilenmenin ayrıntılarını paylaşmak isteyip istemediğinizi belirtmek için kullanılır. Bu yalnızca, "Microsoft yardımı gerekli" sorusu için Hayır 'ı seçerseniz geçerlidir. "|Yes
Microsoft 'a notlar|Hayır|Microsoft 'a yönelik yardıma ihtiyacınız varsa Microsoft 'a özgü notlar|Contoso müşterisi için POC ile ilgili yardım gerekiyor
Müşteri/Iş ortağı ilgili kişisini paylaşma onayı|Yes|Müşteri iletişim ayrıntılarını ve şirketinizin çalışanlarınızı paylaşma onayı, anlaşma üzerinde çalışan ayrıntıları ile iletişim kurun. **Bu sütun için Hayır ' ı seçerseniz anlaşmalar oluşturulmaz veya güncellenmez.** |Yes
1\. Çözüm|Yes|Çözüm KIMLIĞI (gerekli), anlaşma değerinin girildiği para birimi (Isteğe bağlı). Döviz cinslerini [buradan](https://en.wikipedia.org/wiki/ISO_4217), SKU 'nun fiyatını (isteğe bağlı) ve SKU 'nun miktarına (isteğe bağlı) ulaşabilirsiniz.  |NUEVO-1234-PQRS, USD, 10, 100
Takım üyesi 1|Yes|İlgili takım üyesinin adı, soyadı, cep telefonu numarası ve e-posta KIMLIĞI.| Bob, Iş ortağı, 999999, Bob.partner@Contoso.com

## <a name="next-steps"></a>Sonraki adımlar

Bu Iş Ortağı Merkezi ortak satış bağlayıcılarını, CRM sistemlerinizden Microsoft ile birlikte satın almak için kullanabilirsiniz.

- [Dynamics 365 CRM için ortak satış Bağlayıcısı – genel bakış](connector-dynamics.md)
- [Salesforce için ortak satış Bağlayıcısı CRM-genel bakış](connector-salesforce.md)
