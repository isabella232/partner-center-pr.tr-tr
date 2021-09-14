---
title: başvurularda Excel/csv dosyaları aracılığıyla ortak satış fırsatlarını toplu dışa aktarma ve içeri aktarma
description: iş ortağı merkezi 'nde Excel (CSV) dosyalarını kullanarak ortak satış fırsatlarını indirme, oluşturma veya güncelleştirme hakkında bilgi edinin
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 09/08/2021
ms.openlocfilehash: eb0f85eab9340d08a1f121c27f9a1956f5b71635
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248299"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-value-csv-files"></a>Virgülle ayrılmış değer (CSV) dosyaları kullanan ortak satış fırsatları için toplu işlemler

**Uygun roller**: başvuru Yöneticisi | Başvuru kullanıcısı

İş Ortağı Merkezi'ndeki toplu işlemler şirketinizin ortak satış fırsatı verilerini dışarı ve içeri aktarmasına yardımcı olur. **Ortak satış fırsatları** sayfasına gidin ve sayfa başlığının sağ üst kısmındaki **içeri aktar** ve **dışarı aktar** bağlantılarını bulun. Hem **Referans yöneticisi** hem de **Referans Kullanıcısı** izinleri olan kullanıcılar bu işlevselliği kullanabilir.

> [!IMPORTANT]
> Toplu içeri aktarma aracılığıyla gerçekleştirilen oluşturma/güncelleştirme eylemleri geri alınamaz. Çok fazla sayıda kaydı değiştirir veya oluştururken dikkatli olun. Satış anlaşması oluşturulduktan sonra alanların yalnızca bir alt kümesi değiştirilebilir. **Satış anlaşması Reddedildi/Süresi Doldu/Kazanıldı/Kaybedildi gibi bir son duruma ulaştığında hiçbir eyleme izin verilmez.**

## <a name="export-co-sell-opportunities"></a>Ortak satış fırsatlarını dışarı aktarma

Aşağıdaki bilgiler dışa aktarma işlevini açıklar:

- **Dışarı aktar** düğmesine tıklayarak **en fazla 5000 kaydı** dışarı aktarabilirsiniz.
- İndirilen anlaşmalar erişim düzeylerinizi temel alır. Başvuru yöneticileri ve başvuru kullanıcıları, kapsamlarına bağlı olarak farklı sonuçlar alabilir ve ekipteki ekip üyeleri olarak dahil edebilir. [Başvurular izinleri](permissions-overview.md#manage-referrals)hakkında daha fazla bilgi edinin.
- Dışa aktarma işlevi, ortak satış fırsatları sayfasında geçerli sekmeyi ve uygulanan filtreleri hesaba göre alır.
- Uygulanan filtreleri temel alan tüm verileri içeren bir CSV dosyası oluşturulacaktır.
- Kayıtların indirilmesi bir dakika kadar sürebilir.
- İndirme eyleminin tamamlanmasını beklemeniz gerekmez. Iş Ortağı Merkezi 'nde diğer sayfalara gitseniz bile, dışa aktarma işlevi tamamlandıktan hemen sonra dosya indirilir.
- İndirilen dosyayı, işlem ayrıntılarını değiştirmek ve kayıtları güncelleştirmek üzere karşıya yüklemek için yeniden kullanabilirsiniz.

## <a name="import-co-sell-opportunities"></a>Ortak satış fırsatlarını içeri aktarma

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
Hatalar|No|Başvurular için oluşturma/güncelleştirme işlemleriyle ilgili varsa hatalar bu sütuna dahil edilir. Birden çok hata varsa, bunların hepsi noktalı virgülle ayrılmış olarak listelenir.|Zorunlu alan çözümü 1 eksik|
Katılım KIMLIĞI|No|Katılım KIMLIĞI, Microsoft Iş Ortağı Merkezi başvuruları sistemi tarafından oluşturulur. Yeni başvuru oluşturma için gerekli değildir. Bir kaydı güncelleştiriyorsanız, var olan katılım KIMLIĞINI kullanabilirsiniz.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
Referans kimliği|No|Başvuru KIMLIĞI, Microsoft Iş Ortağı Merkezi başvuruları sistemi tarafından oluşturulur. Yeni başvuru oluşturma için gerekli değildir. Mevcut bir kaydı güncelleştiriyorsanız, bunu referans KIMLIĞIYLE doldurabilirsiniz.|ebacdkdc-0b84-4ac4-B4EA-5b2587d42cee
Anlaşma adı|Yes|Başvurunuz için anlaşma için kolay ad.|UK yay
Müşteri Adı|Yes|Müşteri şirketinin adı. Microsoft tarafında hızlı eşleştirme için kuruluşun yasal adını kullanın.|Contoso Corporation
Müşteri adresi satırı 1|Yes|Müşteri şirketinin Adres satırı 1. |Tek contoso yöntemi
Müşteri adresi satırı 2|No|Müşteri şirketinin Adres satırı 2.|NE 148 Caddesi
Müşteri şehri|Yes|Müşteri kuruluşunun bulunduğu şehir.|Redmond
Müşteri durumu|No|Müşteri kuruluşunun bulunduğu eyalet.|Washington
Müşteri posta kodu|No|Müşteri kuruluşunun bulunduğu bölgenin posta kodu.|98052
Müşteri ülkesi|Yes|Müşteri kuruluşunun bulunduğu ülke/bölge. [Burada]( https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes)bahsedilen iki harfli ülke kodlarını kullanın.|ABD
Müşteri D-U-N-S KIMLIĞI|No|Müşteri kuruluşunun DÇALıŞTıRAL KIMLIĞINI getirmeye çalışın. Bu, daha hızlı satıcı atamasına yardımcı olan Microsoft tarafında müşteri kuruluşunun daha hızlı eşleştirmesine yardımcı olur. BU web sitesinden ÜCRETSİZ OLARAK DUNS ID [edinebilirsiniz.](https://www.dnb.com/duns-number/lookup.html)|81466849
Müşteri Kişisi Adı|-Sına bağ -lıdır|Ad yalnızca Microsoft yardıma ihtiyacınız varsa zorunludur. Bu anlaşma üzerinde çalışan müşteri kuruluşundan birincil ilgili kişinin adı.|John
Müşteri Kişisi Soyadı|-Sına bağ -lıdır|Soyadı yalnızca Microsoft yardıma ihtiyacınız varsa zorunludur. Bu anlaşma üzerinde çalışan müşteri kuruluşundan birincil ilgili kişinin soyadı.|Müşteri
Müşteri İletişim Telefon numarası|-Sına bağ -lıdır|Telefon numarası yalnızca Microsoft yardıma ihtiyacınız varsa zorunludur. Telefon satış anlaşması üzerinde çalışan müşteri kuruluşundan birincil ilgili kişinin numarasını girin.|9999999999
Müşteri İletişim e-posta Adresi|-Sına bağ -lıdır|E-posta adresi yalnızca Microsoft yardıma ihtiyacınız varsa zorunludur. Bu anlaşma üzerinde çalışan müşteri kuruluşundan birincil ilgili kişinin e-posta adresi.|john.customer@contoso.com
İş Ortağı Referans Durumu|Yes|Şirketin bakış açısından anlaşma durumunu gösterir. Referans oluşturma veya değiştirme denemesi yapmak için gereklidir. Yeni **bir** satış anlaşması oluşturmak için Yeni'leri kullanın. Kabul edilen değerler burada [belgelenmiştir.](/partner/develop/referral-resources#referralstatus)|Etkin
İş Ortağı Referansı Alt İstatistikleri|Yes|Anlaşmanın tam durumunu gösterir. Yeni **bir satış** anlaşması oluşturmak için Kabul Edildi'i kullanın. Mevcut bir referansı değiştirirken de gereklidir. Kabul edilen değerler burada [belgelenmiştir.](/partner/develop/referral-resources#referralsubstatus)|Kabul edildi
Microsoft Referans Durumu|-Sına bağ -lıdır|Yardım almak için Microsoft'a gönderdiğiniz ortak satış isteğinin durumunu gösterir. Bu salt okunur bir alandır. Veriler içeri aktarılırken bu alanda yapılan tüm değişiklik yoksayılır.| Beklemede
Reddedildi/Neden kaybedildi|-Sına bağ -lıdır| Bu bilgileri yalnızca alanınıza ilişkin alt durumu Reddedildi veya Kayıp olarak değiştirerek sağlamanız gerekir. Aksi takdirde bu sütunu yoksayabilirsiniz. <br/> **Aşağıdaki seçeneklere göre bir sayı girin** <br/><br/> **1**- Project bütçe yeterli değil  <br/> **2**- Müşteri yanıt vermedi  <br/> **3**- Müşteri başka bir satıcı seçti  <br/> **4** - Müşteri gereksinimi karşılanmaz  <br/> **5** - Müşteri değil <br/> **6**- Önerilen zaman çizgisi çok kısa <br/> **7** - Kötüye kullanım, istenmeyen posta veya kimlik avı olarak bildirme <br/> **8** - Diğer |6|
Satış Aşaması|No|Bu, referans için ayrıntılı satış aşamalarını gösteren alandır. Satış aşamaları hakkında daha fazla bilgi için buraya [tıklayın](./manage-co-sell-opportunities.md)|40
Tahmini Satış Değeri|Yes|Müşteriyle yapılan ilk konuşmaları temel alan satış anlaşması değeri. Anlaşma kazanildi veya kaybedildi terminal durumlarından biri olana kadar bu **değiştirilebilir.** |12563
Para Birimi|Yes|Anlaşma değerinin girilir olduğu para birimi. Para birimi kodlarını burada [bulabilirsiniz.](https://en.wikipedia.org/wiki/ISO_4217)|USD
Tahmini Kapatma Tarihi|Yes|AA/D/YYYY biçiminde müşteriyle yapılan ilk konuşmaları temel alarak satış anlaşması tahmini kapanış tarihi. <br/> **Tarih UTC saat diliminde olmalıdır. Kullanıcı arabiriminde görüntülenen İş Ortağı Merkezi tarihler yerelleştirilmiş saat dilimlerini temel almaktadır. UTC saat diliminde tarihi temin edilen referansa bakıyorsanız kullanıcı arabiriminde +/- bir gün fark İş Ortağı Merkezi olabilir.**|1/30/2020
CRM Kimliği|No|Varsa CRM sisteminize bu referansı tanımlayıcı. Bu, serbest biçimli bir metin girişi alanıdır.|34234324-sdfsdf-345345-sfd
Pazarlama Kampanyası Kimliği|No|Bu alan, pazarlama kampanyasının bu referansla sonuçlanmasına neden olduğunu gösterir. Genellikle yatırım getiri hesaplaması için kullanılır|BingSummer2020
Notlar|No|Referansla ilgili güncelleştirmeleri gösteren ayrıntılı notlar|Bu örnek bir not
Microsoft yardım gerekiyor mu?|Yes|Bu, Microsoft'un bu ortak satış isteği için size yardımcı olup olmadığını belirtmektir|Yes
Microsoft'tan hangi özel yardım?|-Sına bağ -lıdır|Microsoft'un size yardımcı olmak için altı farklı yoldan biri. Bu yalnızca "Microsoft yardımı gerekiyor mu? sorusu için Evet'i seçerseniz geçerlidir. " <br/> **Aşağıdaki seçeneklere göre bir sayı girin** <br/><br/> **1**- İş yükü - belirli bir değer teklifi  <br/> **2**- Müşteri teknik mimarisi  <br/> **3**-kavram kanıtı/demo  <br/> **4**-teklifler ve lisanslama  <br/> **5**-satış sonrası müşteri başarısı  <br/> **6**-genel veya diğer|1|
Microsoft Sales Team ile paylaşma|Yes|Bu, Microsoft satış ekibi ile ilgilenmenin ayrıntılarını paylaşmak isteyip istemediğinizi belirtmek için kullanılır. Bu yalnızca, "Microsoft yardımı gerekli" sorusu için Hayır 'ı seçerseniz geçerlidir. "|Yes
Microsoft 'a notlar|No|Microsoft 'a yönelik yardıma ihtiyacınız varsa Microsoft 'a özgü notlar|Contoso müşterisi için POC ile ilgili yardım gerekiyor
Müşteri/Iş ortağı ilgili kişisini paylaşma onayı|Yes|Müşteri iletişim ayrıntılarını ve şirketinizin çalışanlarınızı paylaşma onayı, anlaşma üzerinde çalışan ayrıntıları ile iletişim kurun. **Bu sütun için Hayır ' ı seçerseniz anlaşmalar oluşturulmaz veya güncellenmez.** |Yes
CLA numarası|Şekline|IOT anlaşmayı oluştururken veya güncelleştirirken CLA numarası gerekli değildir. Design WIN aşamasına geçtiğinizde bu gerekli hale gelir.
Cihaz Kategorisi|No|Tüm IoT cihaz kategorilerinin listesi. Aşağıdaki seçeneklerden bir kategori seçin <br>Aron veya tüketici oyun cihazı <br> ATM <br> & taşımacılık sistemlerini oto <br> Azure Sphere panosu<br> Azure Sphere bileşeni <br> Azure Sphere koruyucu<br> Azure Sphere modülü <br> Otomasyon oluşturma<br> Casino oyun cihazı <br> İletişim cihazları<br> Tüketici Internet cihazı <br> Tüketici takılabilir<br> Dijital resim çerçevesi <br> Dijital Imza <br> Ağ geçidi <br> SST/mobil<br> Endüstriyel otomasyon cihazı<br> Endüstri tabletini (POS dışı) <br> Bilgi noktası<br> Media Player<br> Medya cihazı <br> Mobil POS <br> Gezinti cihazı<br> Ağ projektörü<br> Diğer<br> Diğer bankacılık cihazı<br> Diğer tüketici elektronik cihazı<br> Diğer cihaz<br> diğer Enterprise cihaz<br>  Diğer algılayıcı/düğüm <br> Satış noktası cihazı<br> Yazdırma cihazı <br> Güvenlik/araştırma <br>  Sunucu<br> Set-Top kutusu<br> Akıllı TV <br> Test ve ölçüm cihazı<br> İnce Istemci cihaz <br/>
Silicon Type|No|Aşağıdaki listeden bir seçenek belirleyerek yonga kümesi modeli bilgilerini girin <br> AMD-A10 <br> AMD-A4 <br> AMD-A6 <br> AMD-A8 <br> AMD-E2 <br> AMD-FX 7500 <br> AMD-FX 7600P <br> AMD-FX 9370 <br> AMD-FX 9590 <br> AMD-G serisi <br> AMD-diğerleri <br> AMD-R serisi <br> AMD-FX modellerinin geri kalanı <br> Intel-Atom <br> Intel-Celeron-N1900 <br> Intel-Celeron-N2807 <br> Intel-Celeron-N2930 <br> Intel-Celeron-N3060 <br> Intel-Celeron-N3160 <br> Intel-Core i3 <br> Intel-Core i5 <br> Intel-Core i7 <br> Intel-Core d <br> Intel-diğerleri <br> Intel-Pentium <br> Intel-Celeron 'nin geri kalanı <br> Intel-XEON <br> MediaTek MT3620 <br> NXP 8ULP-CS <br> Diğer <br/>
Azure Sertifikalı cihaz|No|Bu, cihaz için Azure uyumluluk sertifikası 'nın elde edildiğini belirtir
Hizmetleri Ekle|No|Bu, Azure hizmetlerinin dağıtımda IoT çözümüyle birlikte paketlenebilir olduğunu belirtir
Microsoft MSX KIMLIĞI|No|Yalnızca ortak satış fırsatları için kullanılabilen Microsoft MSX sisteminde bir işlem KIMLIĞI
Geçirilen PSC anlaşma KIMLIĞI|No|PSC anlaşma KIMLIĞI, yalnızca PSC 'den BILGISAYARA geçirilen bir anlaşma için kullanılabilir
MPN Kimliği|No|MPN ortak satış fırsatlarının oluşturulduğu kuruluşun KIMLIĞI
1\. Çözüm|Yes|Çözüm KIMLIĞI (gerekli), anlaşma değerinin girildiği para birimi (isteğe bağlı). [Para birimi kodlarını](https://en.wikipedia.org/wiki/ISO_4217), SKU 'nun fiyatını (isteğe bağlı) ve SKU 'nun miktarını bulabilirsiniz (isteğe bağlı)  |NUEVO-1234-PQRS, USD, 10, 100
Takım üyesi 1|Yes|İlgili takım üyesinin adı, soyadı, cep telefonu numarası ve e-posta KIMLIĞI.| Bob, Iş ortağı, 999999, Bob.partner@Contoso.com
Microsoft takım üyesi 1|No|Ortak satış fırsatı üzerinde çalışan ilgili Microsoft ekibi üyesinin adı, soyadı, cep telefonu numarası ve e-posta KIMLIĞI.| Sam, satıcı, 999999, Sam.seller@Microsoft.com

## <a name="next-steps"></a>Sonraki adımlar

Bu Iş Ortağı Merkezi ortak satış bağlayıcılarını, CRM sistemlerinizden Microsoft ile birlikte satın almak için kullanabilirsiniz.

- [Dynamics 365 CRM için ortak satış Bağlayıcısı – genel bakış](connector-dynamics.md)
- [Salesforce için ortak satış Bağlayıcısı CRM-genel bakış](connector-salesforce.md)
